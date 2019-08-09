The following text has been accessed from https://en.wikipedia.org/wiki/Eigenvalues_and_eigenvectors at Fri Aug 9 02:50:00 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Eigenvalues and eigenvectors ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Characteristic root" redirects here. For other uses, see Characteristic_root_
(disambiguation).
Vectors that map to their scalar multiples, and the associated scalars
In linear_algebra, an eigenvector (/ËaÉªÉ¡ÉnËvÉktÉr/) or characteristic
vector of a linear_transformation is a non-zero vector that changes by only a
scalar factor when that linear transformation is applied to it. More formally,
if T is a linear transformation from a vector_space V over a field F into
itself and v is a vector in V that is not the zero_vector, then v is an
eigenvector of T if T(v) is a scalar multiple of v. This condition can be
written as the equation
         T (  v  ) = &#x03BB;  v  ,   {\displaystyle T(\mathbf {v} )=\lambda
      \mathbf {v} ,}  [{\displaystyle T(\mathbf {v} )=\lambda \mathbf {v} ,}]
where Î» is a scalar in the field F, known as the eigenvalue, characteristic
value, or characteristic root associated with the eigenvector v.
If the vector space V is finite-dimensional, then the linear transformation T
can be represented as a square_matrix A, and the vector v by a column_vector,
rendering the above mapping as a matrix_multiplication on the left-hand side
and a scaling of the column vector on the right-hand side in the equation
         A  v  = &#x03BB;  v  .   {\displaystyle A\mathbf {v} =\lambda \mathbf
      {v} .}  [{\displaystyle A\mathbf {v} =\lambda \mathbf {v} .}]
There is a direct correspondence between n-by-n square matrices and linear
transformations from an n-dimensional vector space to itself, given any basis
of the vector space. For this reason, it is equivalent to define eigenvalues
and eigenvectors using either the language of matrices or the language of
linear transformations.[1][2]
Geometrically, an eigenvector, corresponding to a real nonzero eigenvalue,
points in a direction that is stretched by the transformation and the
eigenvalue is the factor by which it is stretched. If the eigenvalue is
negative, the direction is reversed.[3]
⁰
***** Contents *****
    * 1_Overview
    * 2_History
    * 3_Eigenvalues_and_eigenvectors_of_matrices
          o 3.1_Eigenvalues_and_the_characteristic_polynomial
          o 3.2_Algebraic_multiplicity
          o 3.3_Eigenspaces,_geometric_multiplicity,_and_the_eigenbasis_for
            matrices
          o 3.4_Additional_properties_of_eigenvalues
          o 3.5_Left_and_right_eigenvectors
          o 3.6_Diagonalization_and_the_eigendecomposition
          o 3.7_Variational_characterization
          o 3.8_Matrix_examples
                # 3.8.1_Two-dimensional_matrix_example
                # 3.8.2_Three-dimensional_matrix_example
                # 3.8.3_Three-dimensional_matrix_example_with_complex
                  eigenvalues
                # 3.8.4_Diagonal_matrix_example
                # 3.8.5_Triangular_matrix_example
                # 3.8.6_Matrix_with_repeated_eigenvalues_example
    * 4_Eigenvalues_and_eigenfunctions_of_differential_operators
          o 4.1_Derivative_operator_example
    * 5_General_definition
          o 5.1_Eigenspaces,_geometric_multiplicity,_and_the_eigenbasis
          o 5.2_Zero_vector_as_an_eigenvector
          o 5.3_Spectral_theory
          o 5.4_Associative_algebras_and_representation_theory
    * 6_Dynamic_equations
    * 7_Calculation
          o 7.1_Classical_method
                # 7.1.1_Eigenvalues
                # 7.1.2_Eigenvectors
          o 7.2_Simple_iterative_methods
          o 7.3_Modern_methods
    * 8_Applications
          o 8.1_Eigenvalues_of_geometric_transformations
          o 8.2_SchrÃ¶dinger_equation
          o 8.3_Molecular_orbitals
          o 8.4_Geology_and_glaciology
          o 8.5_Principal_component_analysis
          o 8.6_Vibration_analysis
          o 8.7_Eigenfaces
          o 8.8_Tensor_of_moment_of_inertia
          o 8.9_Stress_tensor
          o 8.10_Graphs
          o 8.11_Basic_reproduction_number
    * 9_See_also
    * 10_Notes
    * 11_References
          o 11.1_Citations
          o 11.2_Sources
    * 12_External_links
          o 12.1_Theory
          o 12.2_Demonstration_applets
***** Overview[edit] *****
Eigenvalues and eigenvectors feature prominently in the analysis of linear
transformations. The prefix eigen- is adopted from the German word eigen for
"proper", "characteristic".[4] Originally utilized to study principal_axes of
the rotational motion of rigid_bodies, eigenvalues and eigenvectors have a wide
range of applications, for example in stability_analysis, vibration_analysis,
atomic_orbitals, facial_recognition, and matrix_diagonalization.
In essence, an eigenvector v of a linear transformation T is a non-zero vector
that, when T is applied to it, does not change direction. Applying T to the
eigenvector only scales the eigenvector by the scalar value Î», called an
eigenvalue. This condition can be written as the equation
         T (  v  ) = &#x03BB;  v  ,   {\displaystyle T(\mathbf {v} )=\lambda
      \mathbf {v} ,}  [{\displaystyle T(\mathbf {v} )=\lambda \mathbf {v} ,}]
referred to as the eigenvalue equation or eigenequation. In general, Î» may be
any scalar. For example, Î» may be negative, in which case the eigenvector
reverses direction as part of the scaling, or it may be zero or complex.
In this shear_mapping the red arrow changes direction but the blue arrow does
not. The blue arrow is an eigenvector of this shear mapping because it does not
change direction, and since its length is unchanged, its eigenvalue is 1.
The Mona_Lisa example pictured at right provides a simple illustration. Each
point on the painting can be represented as a vector pointing from the center
of the painting to that point. The linear transformation in this example is
called a shear_mapping. Points in the top half are moved to the right and
points in the bottom half are moved to the left proportional to how far they
are from the horizontal axis that goes through the middle of the painting. The
vectors pointing to each point in the original image are therefore tilted right
or left and made longer or shorter by the transformation. Notice that points
along the horizontal axis do not move at all when this transformation is
applied. Therefore, any vector that points directly to the right or left with
no vertical component is an eigenvector of this transformation because the
mapping does not change its direction. Moreover, these eigenvectors all have an
eigenvalue equal to one because the mapping does not change their length,
either.
Linear transformations can take many different forms, mapping vectors in a
variety of vector_spaces, so the eigenvectors can also take many forms. For
example, the linear transformation could be a differential_operator like
d  d x       {\displaystyle {\tfrac {d}{dx}}}  [{\tfrac  {d}{dx}}], in which
case the eigenvectors are functions called eigenfunctions that are scaled by
that differential operator, such as
           d  d x     e  &#x03BB; x   = &#x03BB;  e  &#x03BB; x   .
      {\displaystyle {\frac {d}{dx}}e^{\lambda x}=\lambda e^{\lambda x}.}  [
      {\displaystyle {\frac {d}{dx}}e^{\lambda x}=\lambda e^{\lambda x}.}]
Alternatively, the linear transformation could take the form of an n by n
matrix, in which case the eigenvectors are n by 1 matrices that are also
referred to as eigenvectors. If the linear transformation is expressed in the
form of an n by n matrix A, then the eigenvalue equation above for a linear
transformation can be rewritten as the matrix multiplication
         A v = &#x03BB; v ,   {\displaystyle Av=\lambda v,}  [{\displaystyle
      Av=\lambda v,}]
where the eigenvector v is an n by 1 matrix. For a matrix, eigenvalues and
eigenvectors can be used to decompose_the_matrix, for example by diagonalizing
it.
Eigenvalues and eigenvectors give rise to many closely related mathematical
concepts, and the prefix eigen- is applied liberally when naming them:
    * The set of all eigenvectors of a linear transformation, each paired with
      its corresponding eigenvalue, is called the eigensystem of that
      transformation.[5][6]
    * The set of all eigenvectors of T corresponding to the same eigenvalue,
      together with the zero vector, is called an eigenspace or characteristic
      space of T.[7]
    * If a set of eigenvectors of T forms a basis of the domain of T, then this
      basis is called an eigenbasis.
***** History[edit] *****
Eigenvalues are often introduced in the context of linear_algebra or matrix
theory. Historically, however, they arose in the study of quadratic_forms and
differential_equations.
In the 18th century Euler studied the rotational motion of a rigid_body and
discovered the importance of the principal_axes.[8] Lagrange realized that the
principal axes are the eigenvectors of the inertia matrix.[9] In the early 19th
century, Cauchy saw how their work could be used to classify the quadric
surfaces, and generalized it to arbitrary dimensions.[10] Cauchy also coined
the term racine caractÃ©ristique (characteristic root) for what is now called
eigenvalue; his term survives in characteristic_equation.[11]
Fourier used the work of Laplace and Lagrange to solve the heat_equation by
separation_of_variables in his famous 1822 book ThÃ©orie_analytique_de_la
chaleur.[12] Sturm developed Fourier's ideas further and brought them to the
attention of Cauchy, who combined them with his own ideas and arrived at the
fact that real symmetric matrices have real eigenvalues.[13] This was extended
by Hermite in 1855 to what are now called Hermitian_matrices.[14] Around the
same time, Brioschi proved that the eigenvalues of orthogonal_matrices lie on
the unit_circle,[13] and Clebsch found the corresponding result for skew-
symmetric_matrices.[14] Finally, Weierstrass clarified an important aspect in
the stability_theory started by Laplace by realizing that defective_matrices
can cause instability.[13]
In the meantime, Liouville studied eigenvalue problems similar to those of
Sturm; the discipline that grew out of their work is now called
SturmâLiouville_theory.[15] Schwarz studied the first eigenvalue of Laplace's
equation on general domains towards the end of the 19th century, while
PoincarÃ© studied Poisson's_equation a few years later.[16]
At the start of the 20th century, Hilbert studied the eigenvalues of integral
operators by viewing the operators as infinite matrices.[17] He was the first
to use the German word eigen, which means "own", to denote eigenvalues and
eigenvectors in 1904,[18] though he may have been following a related usage by
Helmholtz. For some time, the standard term in English was "proper value", but
the more distinctive term "eigenvalue" is standard today.[19]
The first numerical algorithm for computing eigenvalues and eigenvectors
appeared in 1929, when Von_Mises published the power_method. One of the most
popular methods today, the QR_algorithm, was proposed independently by John
G.F._Francis[20] and Vera_Kublanovskaya[21] in 1961.[22][23]
***** Eigenvalues and eigenvectors of matrices[edit] *****
See also: Euclidean_vector and Matrix_(mathematics)
Eigenvalues and eigenvectors are often introduced to students in the context of
linear algebra courses focused on matrices.[24][25] Furthermore, linear
transformations over a finite-dimensional vector space can be represented using
matrices,[1][2] which is especially common in numerical and computational
applications.[26]
Matrix A acts by stretching the vector x, not changing its direction, so x is
an eigenvector of A.
Consider n-dimensional vectors that are formed as a list of n scalars, such as
the three-dimensional vectors
         x =   [    1     3     4    ]      and    y =   [    &#x2212; 20
      &#x2212; 60     &#x2212; 80    ]   .   {\displaystyle x={\begin
      {bmatrix}1\\3\\4\end{bmatrix}}\quad {\mbox{and}}\quad y={\begin{bmatrix}-
      20\\-60\\-80\end{bmatrix}}.}  [{\displaystyle x={\begin
      {bmatrix}1\\3\\4\end{bmatrix}}\quad {\mbox{and}}\quad y={\begin{bmatrix}-
      20\\-60\\-80\end{bmatrix}}.}]
These vectors are said to be scalar_multiples of each other, or parallel or
collinear, if there is a scalar Î» such that
         x = &#x03BB; y .   {\displaystyle x=\lambda y.}  [{\displaystyle
      x=\lambda y.}]
In this case Î» = â1/20.
Now consider the linear transformation of n-dimensional vectors defined by an n
by n matrix A,
         A v = w ,   {\displaystyle Av=w,}  [{\displaystyle Av=w,}]
or
           [     A  11      A  12     &#x2026;    A  1 n        A  21      A
      22     &#x2026;    A  2 n       &#x22EE;   &#x22EE;   &#x22F1;   &#x22EE;
      A  n 1      A  n 2     &#x2026;    A  n n      ]     [     v  1        v
      2       &#x22EE;      v  n      ]   =   [     w  1        w  2
      &#x22EE;      w  n      ]     {\displaystyle {\begin{bmatrix}A_{11}&A_
      {12}&\ldots &A_{1n}\\A_{21}&A_{22}&\ldots &A_{2n}\\\vdots &\vdots &\ddots
      &\vdots \\A_{n1}&A_{n2}&\ldots &A_{nn}\\\end{bmatrix}}{\begin{bmatrix}v_
      {1}\\v_{2}\\\vdots \\v_{n}\end{bmatrix}}={\begin{bmatrix}w_{1}\\w_
      {2}\\\vdots \\w_{n}\end{bmatrix}}}  [{\displaystyle {\begin{bmatrix}A_
      {11}&A_{12}&\ldots &A_{1n}\\A_{21}&A_{22}&\ldots &A_{2n}\\\vdots &\vdots
      &\ddots &\vdots \\A_{n1}&A_{n2}&\ldots &A_{nn}\\\end{bmatrix}}{\begin
      {bmatrix}v_{1}\\v_{2}\\\vdots \\v_{n}\end{bmatrix}}={\begin{bmatrix}w_
      {1}\\w_{2}\\\vdots \\w_{n}\end{bmatrix}}}]
where, for each row,
          w  i   =  A  i 1    v  1   +  A  i 2    v  2   + &#x22EF; +  A  i n
      v  n   =  &#x2211;  j = 1   n    A  i j    v  j     {\displaystyle w_
      {i}=A_{i1}v_{1}+A_{i2}v_{2}+\cdots +A_{in}v_{n}=\sum _{j=1}^{n}A_{ij}v_
      {j}}  [{\displaystyle w_{i}=A_{i1}v_{1}+A_{i2}v_{2}+\cdots +A_{in}v_
      {n}=\sum _{j=1}^{n}A_{ij}v_{j}}].
If it occurs that v and w are scalar multiples, that is if
         A v = w = &#x03BB; v ,   {\displaystyle Av=w=\lambda v,}  [    (1)
      {\displaystyle Av=w=\lambda v,}]                                  
then v is an eigenvector of the linear transformation A and the scale factor Î»
is the eigenvalue corresponding to that eigenvector. Equation (1) is the
eigenvalue equation for the matrix A.
Equation (1) can be stated equivalently as
         ( A &#x2212; &#x03BB; I ) v = 0 ,   {\displaystyle (A-    (2 )
      \lambda I)v=0,}  [{\displaystyle (A-\lambda I)v=0,}]         
where I is the n by n identity_matrix and 0 is the zero vector.
**** Eigenvalues and the characteristic polynomial[edit] ****
Main article: Characteristic_polynomial
Equation (2) has a non-zero solution v if_and_only_if the determinant of the
matrix (A â Î»I) is zero. Therefore, the eigenvalues of A are values of Î»
that satisfy the equation
          |  A &#x2212; &#x03BB; I  |  = 0   {\displaystyle |A-    (3 )
      \lambda I|=0}  [{\displaystyle |A-\lambda I|=0}]             
Using Leibniz'_rule for the determinant, the left-hand side of Equation (3) is
a polynomial function of the variable Î» and the degree of this polynomial is
n, the order of the matrix A. Its coefficients depend on the entries of A,
except that its term of degree n is always (â1)nÎ»n. This polynomial is
called the characteristic_polynomial of A. Equation (3) is called the
characteristic equation or the secular equation of A.
The fundamental_theorem_of_algebra implies that the characteristic polynomial
of an n-by-n matrix A, being a polynomial of degree n, can be factored into the
product of n linear terms,
          |  A &#x2212; &#x03BB; I  |  = (  &#x03BB;  1   &#x2212;
      &#x03BB; ) (  &#x03BB;  2   &#x2212; &#x03BB; ) &#x22EF;
      (  &#x03BB;  n   &#x2212; &#x03BB; ) ,   {\displaystyle |A-      
      \lambda I|=(\lambda _{1}-\lambda )(\lambda _{2}-\lambda            (4 )
      )\cdots (\lambda _{n}-\lambda ),}  [{\displaystyle |A-\lambda
      I|=(\lambda _{1}-\lambda )(\lambda _{2}-\lambda )\cdots
      (\lambda _{n}-\lambda ),}]
where each Î»i may be real but in general is a complex number. The numbers Î»1,
Î»2, â¦ Î»n, which may not all have distinct values, are roots of the
polynomial and are the eigenvalues of A.
As a brief example, which is described in more detail in the examples section
later, consider the matrix
         M =   [    2   1     1   2    ]   .   {\displaystyle M={\begin
      {bmatrix}2&1\\1&2\end{bmatrix}}.}  [{\displaystyle M={\begin
      {bmatrix}2&1\\1&2\end{bmatrix}}.}]
Taking the determinant of (M â Î»I), the characteristic polynomial of M is
          |  M &#x2212; &#x03BB; I  |  =   |    2 &#x2212; &#x03BB;   1     1
      2 &#x2212; &#x03BB;    |   = 3 &#x2212; 4 &#x03BB; +  &#x03BB;  2   .
      {\displaystyle |M-\lambda I|={\begin{vmatrix}2-\lambda &1\\1&2-\lambda
      \end{vmatrix}}=3-4\lambda +\lambda ^{2}.}  [{\displaystyle |M-\lambda I|=
      {\begin{vmatrix}2-\lambda &1\\1&2-\lambda \end{vmatrix}}=3-4\lambda
      +\lambda ^{2}.}]
Setting the characteristic polynomial equal to zero, it has roots at Î» = 1 and
Î» = 3, which are the two eigenvalues of M. The eigenvectors corresponding to
each eigenvalue can be found by solving for the components of v in the equation
Mv = Î»v. In this example, the eigenvectors are any non-zero scalar multiples
of
          v  &#x03BB; = 1   =   [    1     &#x2212; 1    ]   ,   v  &#x03BB; =
      3   =   [    1     1    ]   .   {\displaystyle v_{\lambda =1}={\begin
      {bmatrix}1\\-1\end{bmatrix}},\quad v_{\lambda =3}={\begin
      {bmatrix}1\\1\end{bmatrix}}.}  [{\displaystyle v_{\lambda =1}={\begin
      {bmatrix}1\\-1\end{bmatrix}},\quad v_{\lambda =3}={\begin
      {bmatrix}1\\1\end{bmatrix}}.}]
If the entries of the matrix A are all real numbers, then the coefficients of
the characteristic polynomial will also be real numbers, but the eigenvalues
may still have non-zero imaginary parts. The entries of the corresponding
eigenvectors therefore may also have non-zero imaginary parts. Similarly, the
eigenvalues may be irrational_numbers even if all the entries of A are rational
numbers or even if they are all integers. However, if the entries of A are all
algebraic_numbers, which include the rationals, the eigenvalues are complex
algebraic numbers.
The non-real roots of a real polynomial with real coefficients can be grouped
into pairs of complex_conjugates, namely with the two members of each pair
having imaginary parts that differ only in sign and the same real part. If the
degree is odd, then by the intermediate_value_theorem at least one of the roots
is real. Therefore, any real_matrix with odd order has at least one real
eigenvalue, whereas a real matrix with even order may not have any real
eigenvalues. The eigenvectors associated with these complex eigenvalues are
also complex and also appear in complex conjugate pairs.
**** Algebraic multiplicity[edit] ****
Let Î»i be an eigenvalue of an n by n matrix A. The algebraic multiplicity Î¼A
(Î»i) of the eigenvalue is its multiplicity_as_a_root of the characteristic
polynomial, that is, the largest integer k such that (Î» â Î»i)k divides
evenly that polynomial.[7][27][28]
Suppose a matrix A has dimension n and d â¤ n distinct eigenvalues. Whereas
Equation (4) factors the characteristic polynomial of A into the product of n
linear terms with some terms potentially repeating, the characteristic
polynomial can instead be written as the product of d terms each corresponding
to a distinct eigenvalue and raised to the power of the algebraic multiplicity,
          |  A &#x2212; &#x03BB; I  |  = (  &#x03BB;  1   &#x2212; &#x03BB;  )
      &#x03BC;  A   (  &#x03BB;  1   )   (  &#x03BB;  2   &#x2212; &#x03BB;  )
      &#x03BC;  A   (  &#x03BB;  2   )   &#x22EF; (  &#x03BB;  d   &#x2212;
      &#x03BB;  )   &#x03BC;  A   (  &#x03BB;  d   )   .   {\displaystyle |A-
      \lambda I|=(\lambda _{1}-\lambda )^{\mu _{A}(\lambda _{1})}(\lambda _{2}-
      \lambda )^{\mu _{A}(\lambda _{2})}\cdots (\lambda _{d}-\lambda )^{\mu _
      {A}(\lambda _{d})}.}  [{\displaystyle |A-\lambda I|=(\lambda _{1}-\lambda
      )^{\mu _{A}(\lambda _{1})}(\lambda _{2}-\lambda )^{\mu _{A}(\lambda _
      {2})}\cdots (\lambda _{d}-\lambda )^{\mu _{A}(\lambda _{d})}.}]
If d = n then the right-hand side is the product of n linear terms and this is
the same as Equation (4). The size of each eigenvalue's algebraic multiplicity
is related to the dimension n as
             1    &#x2264;  &#x03BC;  A   (  &#x03BB;  i   ) &#x2264; n ,
      &#x03BC;  A      =  &#x2211;  i = 1   d    &#x03BC;  A    (  &#x03BB;  i
      )  = n .       {\displaystyle {\begin{aligned}1&\leq \mu _{A}(\lambda _
      {i})\leq n,\\\mu _{A}&=\sum _{i=1}^{d}\mu _{A}\left(\lambda _
      {i}\right)=n.\end{aligned}}}  [{\displaystyle {\begin{aligned}1&\leq \mu
      _{A}(\lambda _{i})\leq n,\\\mu _{A}&=\sum _{i=1}^{d}\mu _{A}\left(\lambda
      _{i}\right)=n.\end{aligned}}}]
If Î¼A(Î»i) = 1, then Î»i is said to be a simple eigenvalue.[28] If Î¼A(Î»i)
equals the geometric multiplicity of Î»i, Î³A(Î»i), defined in the next
section, then Î»i is said to be a semisimple eigenvalue.
**** Eigenspaces, geometric multiplicity, and the eigenbasis for matrices[edit]
****
Given a particular eigenvalue Î» of the n by n matrix A, define the set E to be
all vectors v that satisfy Equation (2),
         E =  {   v  : ( A &#x2212; &#x03BB; I )  v  = 0  }  .   {\displaystyle
      E=\left\{\mathbf {v} :(A-\lambda I)\mathbf {v} =0\right\}.}  [
      {\displaystyle E=\left\{\mathbf {v} :(A-\lambda I)\mathbf {v}
      =0\right\}.}]
On one hand, this set is precisely the kernel or nullspace of the matrix (A â
Î»I). On the other hand, by definition, any non-zero vector that satisfies this
condition is an eigenvector of A associated with Î». So, the set E is the union
of the zero vector with the set of all eigenvectors of A associated with Î»,
and E equals the nullspace of (A â Î»I). E is called the eigenspace or
characteristic space of A associated with Î».[29][7] In general Î» is a complex
number and the eigenvectors are complex n by 1 matrices. A property of the
nullspace is that it is a linear_subspace, so E is a linear subspace of ân.
Because the eigenspace E is a linear subspace, it is closed under addition.
That is, if two vectors u and v belong to the set E, written (u,v) â E, then
(u + v) â E or equivalently A(u + v) = Î»(u + v). This can be checked using
the distributive_property of matrix multiplication. Similarly, because E is a
linear subspace, it is closed under scalar multiplication. That is, if v â E
and Î± is a complex number, (Î±v) â E or equivalently A(Î±v) = Î»(Î±v). This
can be checked by noting that multiplication of complex matrices by complex
numbers is commutative. As long as u + v and Î±v are not zero, they are also
eigenvectors of A associated with Î».
The dimension of the eigenspace E associated with Î», or equivalently the
maximum number of linearly independent eigenvectors associated with Î», is
referred to as the eigenvalue's geometric multiplicity Î³A(Î»). Because E is
also the nullspace of (A â Î»I), the geometric multiplicity of Î» is the
dimension of the nullspace of (A â Î»I), also called the nullity of (A â
Î»I), which relates to the dimension and rank of (A â Î»I) as
          &#x03B3;  A   ( &#x03BB; ) = n &#x2212; rank &#x2061; ( A &#x2212;
      &#x03BB; I ) .   {\displaystyle \gamma _{A}(\lambda )=n-\operatorname
      {rank} (A-\lambda I).}  [{\displaystyle \gamma _{A}(\lambda )=n-
      \operatorname {rank} (A-\lambda I).}]
Because of the definition of eigenvalues and eigenvectors, an eigenvalue's
geometric multiplicity must be at least one, that is, each eigenvalue has at
least one associated eigenvector. Furthermore, an eigenvalue's geometric
multiplicity cannot exceed its algebraic multiplicity. Additionally, recall
that an eigenvalue's algebraic multiplicity cannot exceed n.
         1 &#x2264;  &#x03B3;  A   ( &#x03BB; ) &#x2264;  &#x03BC;  A
      ( &#x03BB; ) &#x2264; n   {\displaystyle 1\leq \gamma _{A}(\lambda )\leq
      \mu _{A}(\lambda )\leq n}  [{\displaystyle 1\leq \gamma _{A}(\lambda
      )\leq \mu _{A}(\lambda )\leq n}]
To prove the inequality      &#x03B3;  A   ( &#x03BB; ) &#x2264;  &#x03BC;  A
( &#x03BB; )   {\displaystyle \gamma _{A}(\lambda )\leq \mu _{A}(\lambda )}  [
{\displaystyle \gamma _{A}(\lambda )\leq \mu _{A}(\lambda )}], consider how the
definition of geometric multiplicity implies the existence of      &#x03B3;  A
( &#x03BB; )   {\displaystyle \gamma _{A}(\lambda )}  [{\displaystyle \gamma _
{A}(\lambda )}] orthonormal eigenvectors       v   1   ,  &#x2026; ,    v
&#x03B3;  A   ( &#x03BB; )     {\displaystyle {\boldsymbol {v}}_{1},\,\ldots
,\,{\boldsymbol {v}}_{\gamma _{A}(\lambda )}}  [{\displaystyle {\boldsymbol
{v}}_{1},\,\ldots ,\,{\boldsymbol {v}}_{\gamma _{A}(\lambda )}}], such that
A   v   k   = &#x03BB;   v   k     {\displaystyle A{\boldsymbol {v}}_
{k}=\lambda {\boldsymbol {v}}_{k}}  [{\displaystyle A{\boldsymbol {v}}_
{k}=\lambda {\boldsymbol {v}}_{k}}]. We can therefore find a (unitary) matrix
V   {\displaystyle V}  [V] whose first      &#x03B3;  A   ( &#x03BB; )
{\displaystyle \gamma _{A}(\lambda )}  [{\displaystyle \gamma _{A}(\lambda )}]
columns are these eigenvectors, and whose remaining columns can be any
orthonormal set of     n &#x2212;  &#x03B3;  A   ( &#x03BB; )   {\displaystyle
n-\gamma _{A}(\lambda )}  [{\displaystyle n-\gamma _{A}(\lambda )}] vectors
orthogonal to these eigenvectors of     A   {\displaystyle A}  [A]. Then     V
{\displaystyle V}  [V] has full rank and is therefore invertible, and     A V =
V D   {\displaystyle AV=VD}  [AV=VD] with     D   {\displaystyle D}  [D] a
matrix whose top left block is the diagonal matrix     &#x03BB;  I   &#x03B3;
A   ( &#x03BB; )     {\displaystyle \lambda I_{\gamma _{A}(\lambda )}}  [
{\displaystyle \lambda I_{\gamma _{A}(\lambda )}}]. This implies that     ( A
&#x2212; &#x03BE; I ) V = V ( D &#x2212; &#x03BE; I )   {\displaystyle (A-\xi
I)V=V(D-\xi I)}  [{\displaystyle (A-\xi I)V=V(D-\xi I)}]. In other words,     A
&#x2212; &#x03BE; I   {\displaystyle A-\xi I}  [{\displaystyle A-\xi I}] is
similar to     D &#x2212; &#x03BE; I   {\displaystyle D-\xi I}  [{\displaystyle
D-\xi I}], which implies that     det ( A &#x2212; &#x03BE; I ) = det ( D
&#x2212; &#x03BE; I )   {\displaystyle \det(A-\xi I)=\det(D-\xi I)}  [
{\displaystyle \det(A-\xi I)=\det(D-\xi I)}]. But from the definition of     D
{\displaystyle D}  [D] we know that     det ( D &#x2212; &#x03BE; I )
{\displaystyle \det(D-\xi I)}  [{\displaystyle \det(D-\xi I)}] contains a
factor     ( &#x03BE; &#x2212; &#x03BB;  )   &#x03B3;  A   ( &#x03BB; )
{\displaystyle (\xi -\lambda )^{\gamma _{A}(\lambda )}}  [{\displaystyle (\xi -
\lambda )^{\gamma _{A}(\lambda )}}], which means that the algebraic
multiplicity of     &#x03BB;   {\displaystyle \lambda }  [\lambda ] must
satisfy      &#x03BC;  A   ( &#x03BB; ) &#x2265;  &#x03B3;  A   ( &#x03BB; )
{\displaystyle \mu _{A}(\lambda )\geq \gamma _{A}(\lambda )}  [{\displaystyle
\mu _{A}(\lambda )\geq \gamma _{A}(\lambda )}].
Suppose     A   {\displaystyle A}  [A] has     d &#x2264; n   {\displaystyle
d\leq n}  [{\displaystyle d\leq n}] distinct eigenvalues      &#x03BB;  1   , .
. . ,  &#x03BB;  d     {\displaystyle \lambda _{1},...,\lambda _{d}}  [
{\displaystyle \lambda _{1},...,\lambda _{d}}], where the geometric
multiplicity of      &#x03BB;  i     {\displaystyle \lambda _{i}}  [\lambda _
{i}] is      &#x03B3;  A   (  &#x03BB;  i   )   {\displaystyle \gamma _{A}
(\lambda _{i})}  [{\displaystyle \gamma _{A}(\lambda _{i})}]. The total
geometric multiplicity of     A   {\displaystyle A}  [A],
              &#x03B3;  A      =  &#x2211;  i = 1   d    &#x03B3;  A
      (  &#x03BB;  i   ) ,     d    &#x2264;  &#x03B3;  A   &#x2264; n ,
      {\displaystyle {\begin{aligned}\gamma _{A}&=\sum _{i=1}^{d}\gamma _{A}
      (\lambda _{i}),\\d&\leq \gamma _{A}\leq n,\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\gamma _{A}&=\sum _{i=1}^{d}\gamma _{A}
      (\lambda _{i}),\\d&\leq \gamma _{A}\leq n,\end{aligned}}}]
is the dimension of the union of all the eigenspaces of     A   {\displaystyle
A}  [A]'s eigenvalues, or equivalently the maximum number of linearly
independent eigenvectors of     A   {\displaystyle A}  [A]. If      &#x03B3;  A
= n   {\displaystyle \gamma _{A}=n}  [{\displaystyle \gamma _{A}=n}], then
    * The direct sum of the eigenspaces of all of     A   {\displaystyle A}
      [A]'s eigenvalues is the entire vector space       C   n
      {\displaystyle \mathbb {C} ^{n}}  [\mathbb {C} ^{n}].
    * A basis of       C   n     {\displaystyle \mathbb {C} ^{n}}  [\mathbb {C}
      ^{n}] can be formed from     n   {\displaystyle n}  [n] linearly
      independent eigenvectors of     A   {\displaystyle A}  [A]; such a basis
      is called an eigenbasis
    * Any vector in       C   n     {\displaystyle \mathbb {C} ^{n}}  [\mathbb
      {C} ^{n}] can be written as a linear combination of eigenvectors of     A
      {\displaystyle A}  [A].
**** Additional properties of eigenvalues[edit] ****
Let     A   {\displaystyle A}  [A] be an arbitrary     n &#x00D7; n
{\displaystyle n\times n}  [n\times n] matrix of complex numbers with
eigenvalues      &#x03BB;  1   , . . . ,  &#x03BB;  n     {\displaystyle
\lambda _{1},...,\lambda _{n}}  [{\displaystyle \lambda _{1},...,\lambda _
{n}}]. Each eigenvalue appears      &#x03BC;  A   (  &#x03BB;  i   )
{\displaystyle \mu _{A}(\lambda _{i})}  [\mu _{A}(\lambda _{i})] times in this
list, where      &#x03BC;  A   (  &#x03BB;  i   )   {\displaystyle \mu _{A}
(\lambda _{i})}  [\mu _{A}(\lambda _{i})] is the eigenvalue's algebraic
multiplicity. The following are properties of this matrix and its eigenvalues:
    * The trace of     A   {\displaystyle A}  [A], defined as the sum of its
      diagonal elements, is also the sum of all eigenvalues,
               tr &#x2061; ( A ) =  &#x2211;  i = 1   n    a  i i   =  &#x2211;
            i = 1   n    &#x03BB;  i   =  &#x03BB;  1   +  &#x03BB;  2   +
            &#x22EF; +  &#x03BB;  n   .   {\displaystyle \operatorname {tr}
            (A)=\sum _{i=1}^{n}a_{ii}=\sum _{i=1}^{n}\lambda _{i}=\lambda _
            {1}+\lambda _{2}+\cdots +\lambda _{n}.}  [{\displaystyle
            \operatorname {tr} (A)=\sum _{i=1}^{n}a_{ii}=\sum _{i=1}^{n}\lambda
            _{i}=\lambda _{1}+\lambda _{2}+\cdots +\lambda _{n}.}][30][31][32]
    * The determinant of     A   {\displaystyle A}  [A] is the product of all
      its eigenvalues,
               det ( A ) =  &#x220F;  i = 1   n    &#x03BB;  i   =  &#x03BB;  1
            &#x03BB;  2   &#x22EF;  &#x03BB;  n   .   {\displaystyle \det
            (A)=\prod _{i=1}^{n}\lambda _{i}=\lambda _{1}\lambda _{2}\cdots
            \lambda _{n}.}  [{\displaystyle \det(A)=\prod _{i=1}^{n}\lambda _
            {i}=\lambda _{1}\lambda _{2}\cdots \lambda _{n}.}][30][33][34]
    * The eigenvalues of the     k   {\displaystyle k}  [k]th power of     A
      {\displaystyle A}  [A]; i.e., the eigenvalues of      A  k
      {\displaystyle A^{k}}  [A^{k}], for any positive integer     k
      {\displaystyle k}  [k], are      &#x03BB;  1   k   , . . . ,  &#x03BB;  n
      k     {\displaystyle \lambda _{1}^{k},...,\lambda _{n}^{k}}  [
      {\displaystyle \lambda _{1}^{k},...,\lambda _{n}^{k}}].
    * The matrix     A   {\displaystyle A}  [A] is invertible if and only if
      every eigenvalue is nonzero.
    * If     A   {\displaystyle A}  [A] is invertible, then the eigenvalues of
      A  &#x2212; 1     {\displaystyle A^{-1}}  [A^{-1}] are       1  &#x03BB;
      1     , . . . ,   1  &#x03BB;  n       {\displaystyle {\frac {1}{\lambda
      _{1}}},...,{\frac {1}{\lambda _{n}}}}  [{\displaystyle {\frac {1}{\lambda
      _{1}}},...,{\frac {1}{\lambda _{n}}}}] and each eigenvalue's geometric
      multiplicity coincides. Moreover, since the characteristic polynomial of
      the inverse is the reciprocal_polynomial of the original, the eigenvalues
      share the same algebraic multiplicity.
    * If     A   {\displaystyle A}  [A] is equal to its conjugate_transpose
      A  &#x2217;     {\displaystyle A^{*}}  [A^{*}], or equivalently if     A
      {\displaystyle A}  [A] is Hermitian, then every eigenvalue is real. The
      same is true of any symmetric real matrix.
    * If     A   {\displaystyle A}  [A] is not only Hermitian but also
      positive-definite, positive-semidefinite, negative-definite, or negative-
      semidefinite, then every eigenvalue is positive, non-negative, negative,
      or non-positive, respectively.
    * If     A   {\displaystyle A}  [A] is unitary, every eigenvalue has
      absolute value      |   &#x03BB;  i    |  = 1   {\displaystyle |\lambda _
      {i}|=1}  [{\displaystyle |\lambda _{i}|=1}].
    * if     A   {\displaystyle A}  [A] is a     n &#x00D7; n   {\displaystyle
      n\times n}  [n\times n] matrix and     {  &#x03BB;  1   , &#x2026; ,
      &#x03BB;  k   }   {\displaystyle \{\lambda _{1},\ldots ,\lambda _{k}\}}
      [{\displaystyle \{\lambda _{1},\ldots ,\lambda _{k}\}}] are its
      eigenvalues, then the eigenvalues of matrix     I + A   {\displaystyle
      I+A}  [{\displaystyle I+A}] (where     I   {\displaystyle I}  [I] is the
      identity matrix) are     {  &#x03BB;  1   + 1 , &#x2026; ,  &#x03BB;  k
      + 1 }   {\displaystyle \{\lambda _{1}+1,\ldots ,\lambda _{k}+1\}}  [
      {\displaystyle \{\lambda _{1}+1,\ldots ,\lambda _{k}+1\}}]. Moreover, if
      &#x03B1; &#x2208;  R    {\displaystyle \alpha \in \mathbb {R} }  [
      {\displaystyle \alpha \in \mathbb {R} }], the eigenvalues of     &#x03B1;
      I + A   {\displaystyle \alpha I+A}  [{\displaystyle \alpha I+A}] are
      {  &#x03BB;  1   + &#x03B1; , &#x2026; ,  &#x03BB;  k   + &#x03B1; }
      {\displaystyle \{\lambda _{1}+\alpha ,\ldots ,\lambda _{k}+\alpha \}}  [
      {\displaystyle \{\lambda _{1}+\alpha ,\ldots ,\lambda _{k}+\alpha \}}].
**** Left and right eigenvectors[edit] ****
See also: left_and_right_(algebra)
Many disciplines traditionally represent vectors as matrices with a single
column rather than as matrices with a single row. For that reason, the word
"eigenvector" in the context of matrices almost always refers to a right
eigenvector, namely a column vector that right multiplies the     n &#x00D7; n
{\displaystyle n\times n}  [n\times n] matrix     A   {\displaystyle A}  [A] in
the defining equation, Equation (1),
         A v = &#x03BB; v .   {\displaystyle Av=\lambda v.}  [{\displaystyle
      Av=\lambda v.}]
The eigenvalue and eigenvector problem can also be defined for row vectors that
left multiply matrix     A   {\displaystyle A}  [A]. In this formulation, the
defining equation is
         u A = &#x03BA; u ,   {\displaystyle uA=\kappa u,}  [{\displaystyle
      uA=\kappa u,}]
where     &#x03BA;   {\displaystyle \kappa }  [\kappa ] is a scalar and     u
{\displaystyle u}  [u] is a     1 &#x00D7; n   {\displaystyle 1\times n}  [
{\displaystyle 1\times n}] matrix. Any row vector     u   {\displaystyle u}
[u] satisfying this equation is called a left eigenvector of     A
{\displaystyle A}  [A] and     &#x03BA;   {\displaystyle \kappa }  [\kappa ] is
its associated eigenvalue. Taking the transpose of this equation,
          A   T     u   T    = &#x03BA;  u   T    .   {\displaystyle A^{\textsf
      {T}}u^{\textsf {T}}=\kappa u^{\textsf {T}}.}  [{\displaystyle A^{\textsf
      {T}}u^{\textsf {T}}=\kappa u^{\textsf {T}}.}]
Comparing this equation to Equation (1), it follows immediately that a left
eigenvector of     A   {\displaystyle A}  [A] is the same as the transpose of a
right eigenvector of      A   T      {\displaystyle A^{\textsf {T}}}  [
{\displaystyle A^{\textsf {T}}}], with the same eigenvalue. Furthermore, since
the characteristic polynomial of      A   T      {\displaystyle A^{\textsf
{T}}}  [{\displaystyle A^{\textsf {T}}}] is the same as the characteristic
polynomial of     A   {\displaystyle A}  [A], the eigenvalues of the left
eigenvectors of     A   {\displaystyle A}  [A] are the same as the eigenvalues
of the right eigenvectors of      A   T      {\displaystyle A^{\textsf {T}}}  [
{\displaystyle A^{\textsf {T}}}].
**** Diagonalization and the eigendecomposition[edit] ****
Main article: Eigendecomposition_of_a_matrix
Suppose the eigenvectors of A form a basis, or equivalently A has n linearly
independent eigenvectors v1, v2, â¦, vn with associated eigenvalues Î»1, Î»2,
â¦, Î»n. The eigenvalues need not be distinct. Define a square matrix Q whose
columns are the n linearly independent eigenvectors of A,
         Q =   [     v  1      v  2     &#x22EF;    v  n      ]   .
      {\displaystyle Q={\begin{bmatrix}v_{1}&v_{2}&\cdots &v_{n}\end
      {bmatrix}}.}  [{\displaystyle Q={\begin{bmatrix}v_{1}&v_{2}&\cdots &v_
      {n}\end{bmatrix}}.}]
Since each column of Q is an eigenvector of A, right multiplying A by Q scales
each column of Q by its associated eigenvalue,
         A Q =   [     &#x03BB;  1    v  1      &#x03BB;  2    v  2
      &#x22EF;    &#x03BB;  n    v  n      ]   .   {\displaystyle AQ={\begin
      {bmatrix}\lambda _{1}v_{1}&\lambda _{2}v_{2}&\cdots &\lambda _{n}v_
      {n}\end{bmatrix}}.}  [{\displaystyle AQ={\begin{bmatrix}\lambda _{1}v_
      {1}&\lambda _{2}v_{2}&\cdots &\lambda _{n}v_{n}\end{bmatrix}}.}]
With this in mind, define a diagonal matrix Î where each diagonal element Îii
is the eigenvalue associated with the ith column of Q. Then
         A Q = Q &#x039B; .   {\displaystyle AQ=Q\Lambda .}  [{\displaystyle
      AQ=Q\Lambda .}]
Because the columns of Q are linearly independent, Q is invertible. Right
multiplying both sides of the equation by Qâ1,
         A = Q &#x039B;  Q  &#x2212; 1   ,   {\displaystyle A=Q\Lambda Q^{-1},}
      [{\displaystyle A=Q\Lambda Q^{-1},}]
or by instead left multiplying both sides by Qâ1,
          Q  &#x2212; 1   A Q = &#x039B; .   {\displaystyle Q^{-1}AQ=\Lambda .}
      [{\displaystyle Q^{-1}AQ=\Lambda .}]
A can therefore be decomposed into a matrix composed of its eigenvectors, a
diagonal matrix with its eigenvalues along the diagonal, and the inverse of the
matrix of eigenvectors. This is called the eigendecomposition and it is a
similarity_transformation. Such a matrix A is said to be similar to the
diagonal matrix Î or diagonalizable. The matrix Q is the change of basis
matrix of the similarity transformation. Essentially, the matrices A and Î
represent the same linear transformation expressed in two different bases. The
eigenvectors are used as the basis when representing the linear transformation
as Î.
Conversely, suppose a matrix A is diagonalizable. Let P be a non-singular
square matrix such that Pâ1AP is some diagonal matrix D. Left multiplying
both by P, AP = PD. Each column of P must therefore be an eigenvector of A
whose eigenvalue is the corresponding diagonal element of D. Since the columns
of P must be linearly independent for P to be invertible, there exist n
linearly independent eigenvectors of A. It then follows that the eigenvectors
of A form a basis if and only if A is diagonalizable.
A matrix that is not diagonalizable is said to be defective. For defective
matrices, the notion of eigenvectors generalizes to generalized_eigenvectors
and the diagonal matrix of eigenvalues generalizes to the Jordan_normal_form.
Over an algebraically closed field, any matrix A has a Jordan_normal_form and
therefore admits a basis of generalized eigenvectors and a decomposition into
generalized_eigenspaces.
**** Variational characterization[edit] ****
Main article: Min-max_theorem
In the Hermitian case, eigenvalues can be given a variational characterization.
The largest eigenvalue of     H   {\displaystyle H}  [H] is the maximum value
of the quadratic_form      x   T    H x  /   x   T    x   {\displaystyle x^
{\textsf {T}}Hx/x^{\textsf {T}}x}  [{\displaystyle x^{\textsf {T}}Hx/x^{\textsf
{T}}x}]. A value of     x   {\displaystyle x}  [x] that realizes that maximum,
is an eigenvector.
**** Matrix examples[edit] ****
*** Two-dimensional matrix example[edit] ***
The transformation matrix A =       [        2   1     1   2        ]
{\displaystyle {\bigl [}{\begin{smallmatrix}2&1\\1&2\end{smallmatrix}}{\bigr
]}}  [{\displaystyle {\bigl [}{\begin{smallmatrix}2&1\\1&2\end{smallmatrix}}
{\bigr ]}}] preserves the direction of vectors parallel to vÎ»=1 = [1 â1]T
(in purple) and vÎ»=3 = [1 1]T (in blue). The vectors in red are not parallel
to either eigenvector, so, their directions are changed by the transformation.
The blue vectors after the transformation are three times the length of the
original (their eigenvalue is 3), while the lengths of the purple vectors are
unchanged (reflecting an eigenvalue of 1). See also: An_extended_version,
showing_all_four_quadrants.
Consider the matrix
         A =   [    2   1     1   2    ]   .   {\displaystyle A={\begin
      {bmatrix}2&1\\1&2\end{bmatrix}}.}  [{\displaystyle A={\begin
      {bmatrix}2&1\\1&2\end{bmatrix}}.}]
The figure on the right shows the effect of this transformation on point
coordinates in the plane. The eigenvectors v of this transformation satisfy
Equation (1), and the values of Î» for which the determinant of the matrix
(A â Î»I) equals zero are the eigenvalues.
Taking the determinant to find characteristic polynomial of A,
              |  A &#x2212; &#x03BB; I  |     =  |    [    2   1     1   2    ]
      &#x2212; &#x03BB;   [    1   0     0   1    ]    |  =   |    2 &#x2212;
      &#x03BB;   1     1   2 &#x2212; &#x03BB;    |   ,       = 3 &#x2212; 4
      &#x03BB; +  &#x03BB;  2   .       {\displaystyle {\begin{aligned}|A-
      \lambda I|&=\left|{\begin{bmatrix}2&1\\1&2\end{bmatrix}}-\lambda {\begin
      {bmatrix}1&0\\0&1\end{bmatrix}}\right|={\begin{vmatrix}2-\lambda &1\\1&2-
      \lambda \end{vmatrix}},\\[6pt]&=3-4\lambda +\lambda ^{2}.\end{aligned}}}
      [{\displaystyle {\begin{aligned}|A-\lambda I|&=\left|{\begin
      {bmatrix}2&1\\1&2\end{bmatrix}}-\lambda {\begin{bmatrix}1&0\\0&1\end
      {bmatrix}}\right|={\begin{vmatrix}2-\lambda &1\\1&2-\lambda \end
      {vmatrix}},\\[6pt]&=3-4\lambda +\lambda ^{2}.\end{aligned}}}]
Setting the characteristic polynomial equal to zero, it has roots at Î» = 1 and
Î» = 3, which are the two eigenvalues of A.
For Î» = 1, Equation (2) becomes,
         ( A &#x2212; I )  v  &#x03BB; = 1   =   [    1   1     1   1    ]
      [     v  1        v  2      ]   =   [    0     0    ]   .
      {\displaystyle (A-I)v_{\lambda =1}={\begin{bmatrix}1&1\\1&1\end{bmatrix}}
      {\begin{bmatrix}v_{1}\\v_{2}\end{bmatrix}}={\begin{bmatrix}0\\0\end
      {bmatrix}}.}  [{\displaystyle (A-I)v_{\lambda =1}={\begin
      {bmatrix}1&1\\1&1\end{bmatrix}}{\begin{bmatrix}v_{1}\\v_{2}\end
      {bmatrix}}={\begin{bmatrix}0\\0\end{bmatrix}}.}]
Any non-zero vector with v1 = âv2 solves this equation. Therefore,
          v  &#x03BB; = 1   =   [    1     &#x2212; 1    ]     {\displaystyle
      v_{\lambda =1}={\begin{bmatrix}1\\-1\end{bmatrix}}}  [{\displaystyle v_
      {\lambda =1}={\begin{bmatrix}1\\-1\end{bmatrix}}}]
is an eigenvector of A corresponding to Î» = 1, as is any scalar multiple of
this vector.
For Î» = 3, Equation (2) becomes
         ( A &#x2212; 3 I )  v  &#x03BB; = 3   =   [    &#x2212; 1   1     1
      &#x2212; 1    ]     [     v  1        v  2      ]   =   [    0     0    ]
      .   {\displaystyle (A-3I)v_{\lambda =3}={\begin{bmatrix}-1&1\\1&-1\end
      {bmatrix}}{\begin{bmatrix}v_{1}\\v_{2}\end{bmatrix}}={\begin
      {bmatrix}0\\0\end{bmatrix}}.}  [{\displaystyle (A-3I)v_{\lambda =3}=
      {\begin{bmatrix}-1&1\\1&-1\end{bmatrix}}{\begin{bmatrix}v_{1}\\v_{2}\end
      {bmatrix}}={\begin{bmatrix}0\\0\end{bmatrix}}.}]
Any non-zero vector with v1 = v2 solves this equation. Therefore,
          v  &#x03BB; = 3   =   [    1     1    ]     {\displaystyle v_{\lambda
      =3}={\begin{bmatrix}1\\1\end{bmatrix}}}  [{\displaystyle v_{\lambda =3}=
      {\begin{bmatrix}1\\1\end{bmatrix}}}]
is an eigenvector of A corresponding to Î» = 3, as is any scalar multiple of
this vector.
Thus, the vectors vÎ»=1 and vÎ»=3 are eigenvectors of A associated with the
eigenvalues Î» = 1 and Î» = 3, respectively.
*** Three-dimensional matrix example[edit] ***
Consider the matrix
         A =   [    2   0   0     0   3   4     0   4   9    ]   .
      {\displaystyle A={\begin{bmatrix}2&0&0\\0&3&4\\0&4&9\end{bmatrix}}.}  [
      {\displaystyle A={\begin{bmatrix}2&0&0\\0&3&4\\0&4&9\end{bmatrix}}.}]
The characteristic polynomial of A is
              |  A &#x2212; &#x03BB; I  |     =  |    [    2   0   0     0   3
      4     0   4   9    ]   &#x2212; &#x03BB;   [    1   0   0     0   1   0
      0   0   1    ]    |  =   |    2 &#x2212; &#x03BB;   0   0     0   3
      &#x2212; &#x03BB;   4     0   4   9 &#x2212; &#x03BB;    |   ,       =
      ( 2 &#x2212; &#x03BB; )   [   ( 3 &#x2212; &#x03BB; ) ( 9 &#x2212;
      &#x03BB; ) &#x2212; 16   ]   = &#x2212;  &#x03BB;  3   + 14  &#x03BB;  2
      &#x2212; 35 &#x03BB; + 22.       {\displaystyle {\begin{aligned}|A-
      \lambda I|&=\left|{\begin{bmatrix}2&0&0\\0&3&4\\0&4&9\end{bmatrix}}-
      \lambda {\begin{bmatrix}1&0&0\\0&1&0\\0&0&1\end{bmatrix}}\right|={\begin
      {vmatrix}2-\lambda &0&0\\0&3-\lambda &4\\0&4&9-\lambda \end{vmatrix}},\\
      [6pt]&=(2-\lambda ){\bigl [}(3-\lambda )(9-\lambda )-16{\bigr ]}=-\lambda
      ^{3}+14\lambda ^{2}-35\lambda +22.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}|A-\lambda I|&=\left|{\begin
      {bmatrix}2&0&0\\0&3&4\\0&4&9\end{bmatrix}}-\lambda {\begin
      {bmatrix}1&0&0\\0&1&0\\0&0&1\end{bmatrix}}\right|={\begin{vmatrix}2-
      \lambda &0&0\\0&3-\lambda &4\\0&4&9-\lambda \end{vmatrix}},\\[6pt]&=(2-
      \lambda ){\bigl [}(3-\lambda )(9-\lambda )-16{\bigr ]}=-\lambda ^
      {3}+14\lambda ^{2}-35\lambda +22.\end{aligned}}}]
The roots of the characteristic polynomial are 2, 1, and 11, which are the only
three eigenvalues of A. These eigenvalues correspond to the eigenvectors
[    1   0   0    ]     T    ,   {\displaystyle {\begin{bmatrix}1&0&0\end
{bmatrix}}^{\textsf {T}},}  [{\displaystyle {\begin{bmatrix}1&0&0\end
{bmatrix}}^{\textsf {T}},}]        [    0   &#x2212; 2   1    ]     T    ,
{\displaystyle {\begin{bmatrix}0&-2&1\end{bmatrix}}^{\textsf {T}},}  [
{\displaystyle {\begin{bmatrix}0&-2&1\end{bmatrix}}^{\textsf {T}},}] and
[    0   1   2    ]     T      {\displaystyle {\begin{bmatrix}0&1&2\end
{bmatrix}}^{\textsf {T}}}  [{\displaystyle {\begin{bmatrix}0&1&2\end{bmatrix}}^
{\textsf {T}}}], or any non-zero multiple thereof.
*** Three-dimensional matrix example with complex eigenvalues[edit] ***
Consider the cyclic_permutation_matrix
         A =   [    0   1   0     0   0   1     1   0   0    ]   .
      {\displaystyle A={\begin{bmatrix}0&1&0\\0&0&1\\1&0&0\end{bmatrix}}.}  [
      {\displaystyle A={\begin{bmatrix}0&1&0\\0&0&1\\1&0&0\end{bmatrix}}.}]
This matrix shifts the coordinates of the vector up by one position and moves
the first coordinate to the bottom. Its characteristic polynomial is 1 â Î»3,
whose roots are
              &#x03BB;  1      = 1      &#x03BB;  2      = &#x2212;   1 2   +
      i     3  2        &#x03BB;  3      =  &#x03BB;  2   &#x2217;   = &#x2212;
      1 2   &#x2212;  i     3  2         {\displaystyle {\begin{aligned}\lambda
      _{1}&=1\\\lambda _{2}&=-{\frac {1}{2}}+\mathbf {i} {\frac {\sqrt {3}}
      {2}}\\\lambda _{3}&=\lambda _{2}^{*}=-{\frac {1}{2}}-\mathbf {i} {\frac
      {\sqrt {3}}{2}}\end{aligned}}}  [{\displaystyle {\begin{aligned}\lambda _
      {1}&=1\\\lambda _{2}&=-{\frac {1}{2}}+\mathbf {i} {\frac {\sqrt {3}}
      {2}}\\\lambda _{3}&=\lambda _{2}^{*}=-{\frac {1}{2}}-\mathbf {i} {\frac
      {\sqrt {3}}{2}}\end{aligned}}}]
where      i    {\displaystyle \mathbf {i} }  [\mathbf{i}] is an imaginary unit
with       i   2   = &#x2212; 1.   {\displaystyle \mathbf {i} ^{2}=-1.}  [
{\displaystyle \mathbf {i} ^{2}=-1.}]
For the real eigenvalue Î»1 = 1, any vector with three equal non-zero entries
is an eigenvector. For example,
         A   [    5     5     5    ]   =   [    5     5     5    ]   = 1
      &#x22C5;   [    5     5     5    ]   .   {\displaystyle A{\begin
      {bmatrix}5\\5\\5\end{bmatrix}}={\begin{bmatrix}5\\5\\5\end
      {bmatrix}}=1\cdot {\begin{bmatrix}5\\5\\5\end{bmatrix}}.}  [
      {\displaystyle A{\begin{bmatrix}5\\5\\5\end{bmatrix}}={\begin
      {bmatrix}5\\5\\5\end{bmatrix}}=1\cdot {\begin{bmatrix}5\\5\\5\end
      {bmatrix}}.}]
For the complex conjugate pair of imaginary eigenvalues,
          &#x03BB;  2    &#x03BB;  3   = 1 ,   &#x03BB;  2   2   =  &#x03BB;  3
      ,   &#x03BB;  3   2   =  &#x03BB;  2   .   {\displaystyle \lambda _
      {2}\lambda _{3}=1,\quad \lambda _{2}^{2}=\lambda _{3},\quad \lambda _{3}^
      {2}=\lambda _{2}.}  [{\displaystyle \lambda _{2}\lambda _{3}=1,\quad
      \lambda _{2}^{2}=\lambda _{3},\quad \lambda _{3}^{2}=\lambda _{2}.}]
Then
         A   [    1      &#x03BB;  2        &#x03BB;  3      ]   =
      [     &#x03BB;  2        &#x03BB;  3       1    ]   =  &#x03BB;  2
      &#x22C5;   [    1      &#x03BB;  2        &#x03BB;  3      ]   ,
      {\displaystyle A{\begin{bmatrix}1\\\lambda _{2}\\\lambda _{3}\end
      {bmatrix}}={\begin{bmatrix}\lambda _{2}\\\lambda _{3}\\1\end
      {bmatrix}}=\lambda _{2}\cdot {\begin{bmatrix}1\\\lambda _{2}\\\lambda _
      {3}\end{bmatrix}},}  [{\displaystyle A{\begin{bmatrix}1\\\lambda _
      {2}\\\lambda _{3}\end{bmatrix}}={\begin{bmatrix}\lambda _{2}\\\lambda _
      {3}\\1\end{bmatrix}}=\lambda _{2}\cdot {\begin{bmatrix}1\\\lambda _
      {2}\\\lambda _{3}\end{bmatrix}},}]
and
         A   [    1      &#x03BB;  3        &#x03BB;  2      ]   =
      [     &#x03BB;  3        &#x03BB;  2       1    ]   =  &#x03BB;  3
      &#x22C5;   [    1      &#x03BB;  3        &#x03BB;  2      ]   .
      {\displaystyle A{\begin{bmatrix}1\\\lambda _{3}\\\lambda _{2}\end
      {bmatrix}}={\begin{bmatrix}\lambda _{3}\\\lambda _{2}\\1\end
      {bmatrix}}=\lambda _{3}\cdot {\begin{bmatrix}1\\\lambda _{3}\\\lambda _
      {2}\end{bmatrix}}.}  [{\displaystyle A{\begin{bmatrix}1\\\lambda _
      {3}\\\lambda _{2}\end{bmatrix}}={\begin{bmatrix}\lambda _{3}\\\lambda _
      {2}\\1\end{bmatrix}}=\lambda _{3}\cdot {\begin{bmatrix}1\\\lambda _
      {3}\\\lambda _{2}\end{bmatrix}}.}]
Therefore, the other two eigenvectors of A are complex and are      v
&#x03BB;  2     =    [    1    &#x03BB;  2      &#x03BB;  3      ]     T
{\displaystyle v_{\lambda _{2}}={\begin{bmatrix}1&\lambda _{2}&\lambda _{3}\end
{bmatrix}}^{\textsf {T}}}  [{\displaystyle v_{\lambda _{2}}={\begin
{bmatrix}1&\lambda _{2}&\lambda _{3}\end{bmatrix}}^{\textsf {T}}}] and      v
&#x03BB;  3     =    [    1    &#x03BB;  3      &#x03BB;  2      ]     T
{\displaystyle v_{\lambda _{3}}={\begin{bmatrix}1&\lambda _{3}&\lambda _{2}\end
{bmatrix}}^{\textsf {T}}}  [{\displaystyle v_{\lambda _{3}}={\begin
{bmatrix}1&\lambda _{3}&\lambda _{2}\end{bmatrix}}^{\textsf {T}}}] with
eigenvalues Î»2 and Î»3, respectively. The two complex eigenvectors also appear
in a complex conjugate pair,
          v   &#x03BB;  2     =  v   &#x03BB;  3     &#x2217;   .
      {\displaystyle v_{\lambda _{2}}=v_{\lambda _{3}}^{*}.}  [{\displaystyle
      v_{\lambda _{2}}=v_{\lambda _{3}}^{*}.}]
*** Diagonal matrix example[edit] ***
Matrices with entries only along the main diagonal are called diagonal
matrices. The eigenvalues of a diagonal matrix are the diagonal elements
themselves. Consider the matrix
         A =   [    1   0   0     0   2   0     0   0   3    ]   .
      {\displaystyle A={\begin{bmatrix}1&0&0\\0&2&0\\0&0&3\end{bmatrix}}.}  [
      {\displaystyle A={\begin{bmatrix}1&0&0\\0&2&0\\0&0&3\end{bmatrix}}.}]
The characteristic polynomial of A is
          |  A &#x2212; &#x03BB; I  |  = ( 1 &#x2212; &#x03BB; ) ( 2 &#x2212;
      &#x03BB; ) ( 3 &#x2212; &#x03BB; ) ,   {\displaystyle |A-\lambda I|=(1-
      \lambda )(2-\lambda )(3-\lambda ),}  [{\displaystyle |A-\lambda I|=(1-
      \lambda )(2-\lambda )(3-\lambda ),}]
which has the roots Î»1 = 1, Î»2 = 2, and Î»3 = 3. These roots are the diagonal
elements as well as the eigenvalues of A.
Each diagonal element corresponds to an eigenvector whose only non-zero
component is in the same row as that diagonal element. In the example, the
eigenvalues correspond to the eigenvectors,
          v   &#x03BB;  1     =   [    1     0     0    ]   ,   v   &#x03BB;  2
      =   [    0     1     0    ]   ,   v   &#x03BB;  3     =   [    0     0
      1    ]   ,   {\displaystyle v_{\lambda _{1}}={\begin{bmatrix}1\\0\\0\end
      {bmatrix}},\quad v_{\lambda _{2}}={\begin{bmatrix}0\\1\\0\end
      {bmatrix}},\quad v_{\lambda _{3}}={\begin{bmatrix}0\\0\\1\end{bmatrix}},}
      [{\displaystyle v_{\lambda _{1}}={\begin{bmatrix}1\\0\\0\end
      {bmatrix}},\quad v_{\lambda _{2}}={\begin{bmatrix}0\\1\\0\end
      {bmatrix}},\quad v_{\lambda _{3}}={\begin{bmatrix}0\\0\\1\end
      {bmatrix}},}]
respectively, as well as scalar multiples of these vectors.
*** Triangular matrix example[edit] ***
A matrix whose elements above the main diagonal are all zero is called a lower
triangular_matrix, while a matrix whose elements below the main diagonal are
all zero is called an upper triangular matrix. As with diagonal matrices, the
eigenvalues of triangular matrices are the elements of the main diagonal.
Consider the lower triangular matrix,
         A =   [    1   0   0     1   2   0     2   3   3    ]   .
      {\displaystyle A={\begin{bmatrix}1&0&0\\1&2&0\\2&3&3\end{bmatrix}}.}  [
      {\displaystyle A={\begin{bmatrix}1&0&0\\1&2&0\\2&3&3\end{bmatrix}}.}]
The characteristic polynomial of A is
          |  A &#x2212; &#x03BB; I  |  = ( 1 &#x2212; &#x03BB; ) ( 2 &#x2212;
      &#x03BB; ) ( 3 &#x2212; &#x03BB; ) ,   {\displaystyle |A-\lambda I|=(1-
      \lambda )(2-\lambda )(3-\lambda ),}  [{\displaystyle |A-\lambda I|=(1-
      \lambda )(2-\lambda )(3-\lambda ),}]
which has the roots Î»1 = 1, Î»2 = 2, and Î»3 = 3. These roots are the diagonal
elements as well as the eigenvalues of A.
These eigenvalues correspond to the eigenvectors,
          v   &#x03BB;  1     =   [    1     &#x2212; 1       1 2      ]   ,
      v   &#x03BB;  2     =   [    0     1     &#x2212; 3    ]   ,   v
      &#x03BB;  3     =   [    0     0     1    ]   ,   {\displaystyle v_
      {\lambda _{1}}={\begin{bmatrix}1\\-1\\{\frac {1}{2}}\end{bmatrix}},\quad
      v_{\lambda _{2}}={\begin{bmatrix}0\\1\\-3\end{bmatrix}},\quad v_{\lambda
      _{3}}={\begin{bmatrix}0\\0\\1\end{bmatrix}},}  [{\displaystyle v_{\lambda
      _{1}}={\begin{bmatrix}1\\-1\\{\frac {1}{2}}\end{bmatrix}},\quad v_
      {\lambda _{2}}={\begin{bmatrix}0\\1\\-3\end{bmatrix}},\quad v_{\lambda _
      {3}}={\begin{bmatrix}0\\0\\1\end{bmatrix}},}]
respectively, as well as scalar multiples of these vectors.
*** Matrix with repeated eigenvalues example[edit] ***
As in the previous example, the lower triangular matrix
         A =   [    2   0   0   0     1   2   0   0     0   1   3   0     0   0
      1   3    ]   ,   {\displaystyle A={\begin
      {bmatrix}2&0&0&0\\1&2&0&0\\0&1&3&0\\0&0&1&3\end{bmatrix}},}  [
      {\displaystyle A={\begin{bmatrix}2&0&0&0\\1&2&0&0\\0&1&3&0\\0&0&1&3\end
      {bmatrix}},}]
has a characteristic polynomial that is the product of its diagonal elements,
          |  A &#x2212; &#x03BB; I  |  =   |    2 &#x2212; &#x03BB;   0   0   0
      1   2 &#x2212; &#x03BB;   0   0     0   1   3 &#x2212; &#x03BB;   0     0
      0   1   3 &#x2212; &#x03BB;    |   = ( 2 &#x2212; &#x03BB;  )  2   ( 3
      &#x2212; &#x03BB;  )  2   .   {\displaystyle |A-\lambda I|={\begin
      {vmatrix}2-\lambda &0&0&0\\1&2-\lambda &0&0\\0&1&3-\lambda &0\\0&0&1&3-
      \lambda \end{vmatrix}}=(2-\lambda )^{2}(3-\lambda )^{2}.}  [
      {\displaystyle |A-\lambda I|={\begin{vmatrix}2-\lambda &0&0&0\\1&2-
      \lambda &0&0\\0&1&3-\lambda &0\\0&0&1&3-\lambda \end{vmatrix}}=(2-\lambda
      )^{2}(3-\lambda )^{2}.}]
The roots of this polynomial, and hence the eigenvalues, are 2 and 3. The
algebraic multiplicity of each eigenvalue is 2; in other words they are both
double roots. The sum of the algebraic multiplicities of each distinct
eigenvalue is Î¼A = 4 = n, the order of the characteristic polynomial and the
dimension of A.
On the other hand, the geometric multiplicity of the eigenvalue 2 is only 1,
because its eigenspace is spanned by just one vector        [    0   1
&#x2212; 1   1    ]     T      {\displaystyle {\begin{bmatrix}0&1&-1&1\end
{bmatrix}}^{\textsf {T}}}  [{\displaystyle {\begin{bmatrix}0&1&-1&1\end
{bmatrix}}^{\textsf {T}}}] and is therefore 1-dimensional. Similarly, the
geometric multiplicity of the eigenvalue 3 is 1 because its eigenspace is
spanned by just one vector        [    0   0   0   1    ]     T
{\displaystyle {\begin{bmatrix}0&0&0&1\end{bmatrix}}^{\textsf {T}}}  [
{\displaystyle {\begin{bmatrix}0&0&0&1\end{bmatrix}}^{\textsf {T}}}]. The total
geometric multiplicity Î³A is 2, which is the smallest it could be for a matrix
with two distinct eigenvalues. Geometric multiplicities are defined in a later
section.
***** Eigenvalues and eigenfunctions of differential operators[edit] *****
Main article: Eigenfunction
The definitions of eigenvalue and eigenvectors of a linear transformation T
remains valid even if the underlying vector space is an infinite-dimensional
Hilbert or Banach_space. A widely used class of linear transformations acting
on infinite-dimensional spaces are the differential_operators on function
spaces. Let D be a linear differential operator on the space Câ of infinitely
differentiable real functions of a real argument t. The eigenvalue equation for
D is the differential_equation
         D f ( t ) = &#x03BB; f ( t )   {\displaystyle Df(t)=\lambda f(t)}  [
      {\displaystyle Df(t)=\lambda f(t)}]
The functions that satisfy this equation are eigenvectors of D and are commonly
called eigenfunctions.
**** Derivative operator example[edit] ****
Consider the derivative operator        d  d t       {\displaystyle {\tfrac {d}
{dt}}}  [{\displaystyle {\tfrac {d}{dt}}}] with eigenvalue equation
           d  d t    f ( t ) = &#x03BB; f ( t ) .   {\displaystyle {\frac {d}
      {dt}}f(t)=\lambda f(t).}  [{\displaystyle {\frac {d}{dt}}f(t)=\lambda f
      (t).}]
This differential equation can be solved by multiplying both sides by dt/f(t)
and integrating. Its solution, the exponential_function
         f ( t ) = f ( 0 )  e  &#x03BB; t   ,   {\displaystyle f(t)=f(0)e^
      {\lambda t},}  [{\displaystyle f(t)=f(0)e^{\lambda t},}]
is the eigenfunction of the derivative operator. In this case the eigenfunction
is itself a function of its associated eigenvalue. In particular, for Î» = 0
the eigenfunction f(t) is a constant.
The main eigenfunction article gives other examples.
***** General definition[edit] *****
The concept of eigenvalues and eigenvectors extends naturally to arbitrary
linear_transformations on arbitrary vector_spaces. Let V be any vector space
over some field K of scalars, and let T be a linear transformation mapping V
into V,
         T : V &#x2192; V .   {\displaystyle T:V\to V.}  [{\displaystyle T:V\to
      V.}]
We say that a non-zero vector v â V is an eigenvector of T if and only if
there exists a scalar Î» â K such that
         T (  v  ) = &#x03BB;  v  .   {\displaystyle T(\mathbf {v}    
      )=\lambda \mathbf {v} .}  [{\displaystyle T(\mathbf {v}           ( 5 )
      )=\lambda \mathbf {v} .}]
This equation is called the eigenvalue equation for T, and the scalar Î» is the
eigenvalue of T corresponding to the eigenvector v. T(v) is the result of
applying the transformation T to the vector v, while Î»v is the product of the
scalar Î» with v.[35][36]
**** Eigenspaces, geometric multiplicity, and the eigenbasis[edit] ****
Given an eigenvalue Î», consider the set
         E =  {   v  : T (  v  ) = &#x03BB;  v   }  ,   {\displaystyle E=\left\
      {\mathbf {v} :T(\mathbf {v} )=\lambda \mathbf {v} \right\},}  [
      {\displaystyle E=\left\{\mathbf {v} :T(\mathbf {v} )=\lambda \mathbf {v}
      \right\},}]
which is the union of the zero vector with the set of all eigenvectors
associated with Î». E is called the eigenspace or characteristic space of T
associated with Î».
By definition of a linear transformation,
             T (  x  +  y  )    = T (  x  ) + T (  y  ) ,     T ( &#x03B1;  x
      )    = &#x03B1; T (  x  ) ,       {\displaystyle {\begin{aligned}T
      (\mathbf {x} +\mathbf {y} )&=T(\mathbf {x} )+T(\mathbf {y} ),\\T(\alpha
      \mathbf {x} )&=\alpha T(\mathbf {x} ),\end{aligned}}}  [{\displaystyle
      {\begin{aligned}T(\mathbf {x} +\mathbf {y} )&=T(\mathbf {x} )+T(\mathbf
      {y} ),\\T(\alpha \mathbf {x} )&=\alpha T(\mathbf {x} ),\end{aligned}}}]
for (x,y) â V and Î± â K. Therefore, if u and v are eigenvectors of T
associated with eigenvalue Î», namely u,v â E, then
             T (  u  +  v  )    = &#x03BB; (  u  +  v  ) ,     T ( &#x03B1;  v
      )    = &#x03BB; ( &#x03B1;  v  ) .       {\displaystyle {\begin{aligned}T
      (\mathbf {u} +\mathbf {v} )&=\lambda (\mathbf {u} +\mathbf {v} ),\\T
      (\alpha \mathbf {v} )&=\lambda (\alpha \mathbf {v} ).\end{aligned}}}  [
      {\displaystyle {\begin{aligned}T(\mathbf {u} +\mathbf {v} )&=\lambda
      (\mathbf {u} +\mathbf {v} ),\\T(\alpha \mathbf {v} )&=\lambda (\alpha
      \mathbf {v} ).\end{aligned}}}]
So, both u + v and Î±v are either zero or eigenvectors of T associated with Î»,
namely u + v, Î±v â E, and E is closed under addition and scalar
multiplication. The eigenspace E associated with Î» is therefore a linear
subspace of V.[37] If that subspace has dimension 1, it is sometimes called an
eigenline.[38]
The geometric multiplicity Î³T(Î») of an eigenvalue Î» is the dimension of the
eigenspace associated with Î», i.e., the maximum number of linearly independent
eigenvectors associated with that eigenvalue.[7][28] By the definition of
eigenvalues and eigenvectors, Î³T(Î») â¥ 1 because every eigenvalue has at
least one eigenvector.
The eigenspaces of T always form a direct_sum. As a consequence, eigenvectors
of different eigenvalues are always linearly independent. Therefore, the sum of
the dimensions of the eigenspaces cannot exceed the dimension n of the vector
space on which T operates, and there cannot be more than n distinct
eigenvalues.[39]
Any subspace spanned by eigenvectors of T is an invariant_subspace of T, and
the restriction of T to such a subspace is diagonalizable. Moreover, if the
entire vector space V can be spanned by the eigenvectors of T, or equivalently
if the direct sum of the eigenspaces associated with all the eigenvalues of T
is the entire vector space V, then a basis of V called an eigenbasis can be
formed from linearly independent eigenvectors of T. When T admits an
eigenbasis, T is diagonalizable.
**** Zero vector as an eigenvector[edit] ****
While the definition of an eigenvector used in this article excludes the zero
vector, it is possible to define eigenvalues and eigenvectors such that the
zero vector is an eigenvector.[40]
Consider again the eigenvalue equation, Equation (5). Define an eigenvalue to
be any scalar Î» â K such that there exists a non-zero vector v â V
satisfying Equation (5). It is important that this version of the definition of
an eigenvalue specify that the vector be non-zero, otherwise by this definition
the zero vector would allow any scalar in K to be an eigenvalue. Define an
eigenvector v associated with the eigenvalue Î» to be any vector that, given
Î», satisfies Equation (5). Given the eigenvalue, the zero vector is among the
vectors that satisfy Equation (5), so the zero vector is included among the
eigenvectors by this alternate definition.
**** Spectral theory[edit] ****
Main article: Spectral_theory
If Î» is an eigenvalue of T, then the operator (T â Î»I) is not one-to-one,
and therefore its inverse (T â Î»I)â1 does not exist. The converse is true
for finite-dimensional vector spaces, but not for infinite-dimensional vector
spaces. In general, the operator (T â Î»I) may not have an inverse even if Î»
is not an eigenvalue.
For this reason, in functional_analysis eigenvalues can be generalized to the
spectrum_of_a_linear_operator T as the set of all scalars Î» for which the
operator (T â Î»I) has no bounded inverse. The spectrum of an operator always
contains all its eigenvalues but is not limited to them.
**** Associative algebras and representation theory[edit] ****
Main article: Weight_(representation_theory)
One can generalize the algebraic object that is acting on the vector space,
replacing a single operator acting on a vector space with an algebra
representation â an associative_algebra acting on a module. The study of such
actions is the field of representation_theory.
The representation-theoretical_concept_of_weight is an analog of eigenvalues,
while weight vectors and weight spaces are the analogs of eigenvectors and
eigenspaces, respectively.
***** Dynamic equations[edit] *****
The simplest difference_equations have the form
          x  t   =  a  1    x  t &#x2212; 1   +  a  2    x  t &#x2212; 2   +
      &#x22EF; +  a  k    x  t &#x2212; k   .   {\displaystyle x_{t}=a_{1}x_{t-
      1}+a_{2}x_{t-2}+\cdots +a_{k}x_{t-k}.}  [{\displaystyle x_{t}=a_{1}x_{t-
      1}+a_{2}x_{t-2}+\cdots +a_{k}x_{t-k}.}]
The solution of this equation for x in terms of t is found by using its
characteristic equation
          &#x03BB;  k   &#x2212;  a  1    &#x03BB;  k &#x2212; 1   &#x2212;  a
      2    &#x03BB;  k &#x2212; 2   &#x2212; &#x22EF; &#x2212;  a  k &#x2212; 1
      &#x03BB; &#x2212;  a  k   = 0 ,   {\displaystyle \lambda ^{k}-a_
      {1}\lambda ^{k-1}-a_{2}\lambda ^{k-2}-\cdots -a_{k-1}\lambda -a_{k}=0,}
      [{\displaystyle \lambda ^{k}-a_{1}\lambda ^{k-1}-a_{2}\lambda ^{k-2}-
      \cdots -a_{k-1}\lambda -a_{k}=0,}]
which can be found by stacking into matrix form a set of equations consisting
of the above difference equation and the k â 1 equations      x  t &#x2212; 1
=  x  t &#x2212; 1   , &#xA0; &#x2026; , &#xA0;  x  t &#x2212; k + 1   =  x  t
&#x2212; k + 1   ,   {\displaystyle x_{t-1}=x_{t-1},\ \dots ,\ x_{t-k+1}=x_{t-
k+1},}  [{\displaystyle x_{t-1}=x_{t-1},\ \dots ,\ x_{t-k+1}=x_{t-k+1},}]
giving a k-dimensional system of the first order in the stacked variable vector
[     x  t     &#x22EF;    x  t &#x2212; k + 1      ]     {\displaystyle
{\begin{bmatrix}x_{t}&\cdots &x_{t-k+1}\end{bmatrix}}}  [{\displaystyle {\begin
{bmatrix}x_{t}&\cdots &x_{t-k+1}\end{bmatrix}}}] in terms of its once-lagged
value, and taking the characteristic equation of this system's matrix. This
equation gives k characteristic roots      &#x03BB;  1   ,  &#x2026; ,
&#x03BB;  k   ,   {\displaystyle \lambda _{1},\,\ldots ,\,\lambda _{k},}  [
{\displaystyle \lambda _{1},\,\ldots ,\,\lambda _{k},}] for use in the solution
equation
          x  t   =  c  1    &#x03BB;  1   t   + &#x22EF; +  c  k    &#x03BB;  k
      t   .   {\displaystyle x_{t}=c_{1}\lambda _{1}^{t}+\cdots +c_{k}\lambda _
      {k}^{t}.}  [{\displaystyle x_{t}=c_{1}\lambda _{1}^{t}+\cdots +c_
      {k}\lambda _{k}^{t}.}]
A similar procedure is used for solving a differential_equation of the form
             d  k   x   d  t  k      +  a  k &#x2212; 1       d  k &#x2212; 1
      x   d  t  k &#x2212; 1      + &#x22EF; +  a  1      d x   d t    +  a  0
      x = 0.   {\displaystyle {\frac {d^{k}x}{dt^{k}}}+a_{k-1}{\frac {d^{k-1}x}
      {dt^{k-1}}}+\cdots +a_{1}{\frac {dx}{dt}}+a_{0}x=0.}  [{\displaystyle
      {\frac {d^{k}x}{dt^{k}}}+a_{k-1}{\frac {d^{k-1}x}{dt^{k-1}}}+\cdots +a_
      {1}{\frac {dx}{dt}}+a_{0}x=0.}]
***** Calculation[edit] *****
Main article: Eigenvalue_algorithm
The calculation of eigenvalues and eigenvectors is a topic where theory, as
presented in elementary linear algebra textbooks, is often very far from
practice.
**** Classical method[edit] ****
The classical method is to first find the eigenvalues, and then calculate the
eigenvectors for each eigenvalue. It is in several ways poorly suited for non-
exact arithmetics such as floating-point.
*** Eigenvalues[edit] ***
The eigenvalues of a matrix     A   {\displaystyle A}  [A] can be determined by
finding the roots of the characteristic polynomial. This is easy for     2
&#x00D7; 2   {\displaystyle 2\times 2}  [{\displaystyle 2\times 2}] matrices,
but the difficulty increases rapidly with the size of the matrix.
In theory, the coefficients of the characteristic polynomial can be computed
exactly, since they are sums of products of matrix elements; and there are
algorithms that can find all the roots of a polynomial of arbitrary degree to
any required accuracy.[41] However, this approach is not viable in practice
because the coefficients would be contaminated by unavoidable round-off_errors,
and the roots of a polynomial can be an extremely sensitive function of the
coefficients (as exemplified by Wilkinson's_polynomial).[41] Even for matrices
whose elements are integers the calculation becomes nontrivial, because the
sums are very long; the constant term is the determinant, which for an     n
&#x00D7; n   {\displaystyle n\times n}  [n\times n] is a sum of     n !
{\displaystyle n!}  [{\displaystyle n!}] different products.[note_1]
Explicit algebraic_formulas for the roots of a polynomial exist only if the
degree     n   {\displaystyle n}  [n] is 4 or less. According to the
AbelâRuffini_theorem there is no general, explicit and exact algebraic
formula for the roots of a polynomial with degree 5 or more. (Generality
matters because any polynomial with degree     n   {\displaystyle n}  [n] is
the characteristic polynomial of some companion_matrix of order     n
{\displaystyle n}  [n].) Therefore, for matrices of order 5 or more, the
eigenvalues and eigenvectors cannot be obtained by an explicit algebraic
formula, and must therefore be computed by approximate numerical_methods. Even
the exact_formula for the roots of a degree 3 polynomial is numerically
impractical.
*** Eigenvectors[edit] ***
Once the (exact) value of an eigenvalue is known, the corresponding
eigenvectors can be found by finding non-zero solutions of the eigenvalue
equation, that becomes a system_of_linear_equations with known coefficients.
For example, once it is known that 6 is an eigenvalue of the matrix
         A =   [    4   1     6   3    ]     {\displaystyle A={\begin
      {bmatrix}4&1\\6&3\end{bmatrix}}}  [{\displaystyle A={\begin
      {bmatrix}4&1\\6&3\end{bmatrix}}}]
we can find its eigenvectors by solving the equation     A v = 6 v
{\displaystyle Av=6v}  [Av=6v], that is
           [    4   1     6   3    ]     [    x     y    ]   = 6 &#x22C5;
      [    x     y    ]     {\displaystyle {\begin{bmatrix}4&1\\6&3\end
      {bmatrix}}{\begin{bmatrix}x\\y\end{bmatrix}}=6\cdot {\begin
      {bmatrix}x\\y\end{bmatrix}}}  [{\displaystyle {\begin
      {bmatrix}4&1\\6&3\end{bmatrix}}{\begin{bmatrix}x\\y\end{bmatrix}}=6\cdot
      {\begin{bmatrix}x\\y\end{bmatrix}}}]
This matrix equation is equivalent to two linear_equations
          {     4 x + y    = 6 x     6 x + 3 y    = 6 y         {\displaystyle
      \left\{{\begin{aligned}4x+y&=6x\\6x+3y&=6y\end{aligned}}\right.}  [
      {\displaystyle \left\{{\begin{aligned}4x+y&=6x\\6x+3y&=6y\end
      {aligned}}\right.}]      that is           {     &#x2212; 2 x + y    = 0
      6 x &#x2212; 3 y    = 0         {\displaystyle \left\{{\begin{aligned}-
      2x+y&=0\\6x-3y&=0\end{aligned}}\right.}  [{\displaystyle \left\{{\begin
      {aligned}-2x+y&=0\\6x-3y&=0\end{aligned}}\right.}]
Both equations reduce to the single linear equation     y = 2 x
{\displaystyle y=2x}  [y=2x]. Therefore, any vector of the form       [    a
2 a    ]     {\displaystyle {\begin{bmatrix}a\\2a\end{bmatrix}}}  [
{\displaystyle {\begin{bmatrix}a\\2a\end{bmatrix}}}], for any non-zero real
number     a   {\displaystyle a}  [a], is an eigenvector of     A
{\displaystyle A}  [A] with eigenvalue     &#x03BB; = 6   {\displaystyle
\lambda =6}  [\lambda =6].
The matrix     A   {\displaystyle A}  [A] above has another eigenvalue
&#x03BB; = 1   {\displaystyle \lambda =1}  [\lambda =1]. A similar calculation
shows that the corresponding eigenvectors are the non-zero solutions of     3 x
+ y = 0   {\displaystyle 3x+y=0}  [3x+y=0], that is, any vector of the form
[    b     &#x2212; 3 b    ]     {\displaystyle {\begin{bmatrix}b\\-3b\end
{bmatrix}}}  [{\displaystyle {\begin{bmatrix}b\\-3b\end{bmatrix}}}], for any
non-zero real number     b   {\displaystyle b}  [b].
**** Simple iterative methods[edit] ****
Main article: Power_iteration
The converse approach, of first seeking the eigenvectors and then determining
each eigenvalue from its eigenvector, turns out to be far more tractable for
computers. The easiest algorithm here consists of picking an arbitrary starting
vector and then repeatedly multiplying it with the matrix (optionally
normalising the vector to keep its elements of reasonable size); surprisingly
this makes the vector converge towards an eigenvector. A_variation is to
instead multiply the vector by     ( A &#x2212; &#x03BC; I  )  &#x2212; 1
{\displaystyle (A-\mu I)^{-1}}  [(A-\mu I)^{{-1}}]; this causes it to converge
to an eigenvector of the eigenvalue closest to     &#x03BC; &#x2208;  C
{\displaystyle \mu \in \mathbb {C} }  [{\displaystyle \mu \in \mathbb {C} }].
If      v    {\displaystyle \mathbf {v} }  [\mathbf {v} ] is (a good
approximation of) an eigenvector of     A   {\displaystyle A}  [A], then the
corresponding eigenvalue can be computed as
         &#x03BB; =      v   &#x2217;   A  v      v   &#x2217;    v
      {\displaystyle \lambda ={\frac {\mathbf {v} ^{*}A\mathbf {v} }{\mathbf
      {v} ^{*}\mathbf {v} }}}  [{\displaystyle \lambda ={\frac {\mathbf {v} ^
      {*}A\mathbf {v} }{\mathbf {v} ^{*}\mathbf {v} }}}]
where       v   &#x2217;     {\displaystyle \mathbf {v} ^{*}}  [{\displaystyle
\mathbf {v} ^{*}}] denotes the conjugate_transpose of      v    {\displaystyle
\mathbf {v} }  [\mathbf {v} ].
**** Modern methods[edit] ****
Efficient, accurate methods to compute eigenvalues and eigenvectors of
arbitrary matrices were not known until the QR_algorithm was designed in 1961.
[41] Combining the Householder_transformation with the LU decomposition results
in an algorithm with better convergence than the QR algorithm.[citation_needed]
For large Hermitian sparse_matrices, the Lanczos_algorithm is one example of an
efficient iterative_method to compute eigenvalues and eigenvectors, among
several other possibilities.[41]
Most numeric methods that compute the eigenvalues of a matrix also determine a
set of corresponding eigenvectors as a by-product of the computation, although
sometimes implementors choose to discard the eigenvector information as soon as
it is no longer needed.
***** Applications[edit] *****
**** Eigenvalues of geometric transformations[edit] ****
The following table presents some example transformations in the plane along
with their 2Ã2 matrices, eigenvalues, and eigenvectors.
               Scaling               Unequal scaling   Rotation       Horizontal_shear      Hyperbolic_rotation
                                     [Vertical_shrink
Illustration   [Equal_scaling_       and_horizontal    [Rotation_by   [Horizontal_shear     [Squeeze_r=1.5.svg]
               (homothety)]          stretch_of_a_unit 50_degrees]    mapping]
                                     square.]
                                                            [    c
                                                       &#x2212; s
                                                       s   c    ]
                                                       {\displaystyle
                                                       {\begin                                   [    c   s     s
                                                       {bmatrix}c&-                         c    ]
                                                       s\\s&c\end                           {\displaystyle
                                                       {bmatrix}}}  [                       {\begin
                                          [     k  1   {\displaystyle                       {bmatrix}c&s\\s&c\end
                                     0     0    k  2   {\begin                              {bmatrix}}}  [
                    [    k   0     0 ]                 {bmatrix}c&-        [    1   k     0 {\displaystyle
               k    ]                {\displaystyle    s\\s&c\end     1    ]                {\begin
               {\displaystyle        {\begin           {bmatrix}}}]   {\displaystyle        {bmatrix}c&s\\s&c\end
               {\begin               {bmatrix}k_          c = cos     {\begin               {bmatrix}}}]
               {bmatrix}k&0\\0&k\end {1}&0\\0&k_       &#x2061;       {bmatrix}1&k\\0&1\end    c = cosh &#x2061;
Matrix         {bmatrix}}}  [        {2}\end           &#x03B8;       {bmatrix}}}  [        &#x03C6;
               {\displaystyle        {bmatrix}}}  [    {\displaystyle {\displaystyle        {\displaystyle
               {\begin               {\displaystyle    c=\cos \theta  {\begin               c=\cosh \varphi }  [
               {bmatrix}k&0\\0&k\end {\begin           }  [           {bmatrix}1&k\\0&1\end {\displaystyle
               {bmatrix}}}]          {bmatrix}k_       {\displaystyle {bmatrix}}}]          c=\cosh \varphi }]
                                     {1}&0\\0&k_       c=\cos \theta                           s = sinh &#x2061;
                                     {2}\end           }]                                   &#x03C6;
                                     {bmatrix}}}]         s = sin                           {\displaystyle
                                                       &#x2061;                             s=\sinh \varphi }  [
                                                       &#x03B8;                             {\displaystyle
                                                       {\displaystyle                       s=\sinh \varphi }]
                                                       s=\sin \theta
                                                       }  [
                                                       {\displaystyle
                                                       s=\sin \theta
                                                       }]
                                        ( &#x03BB;
                                     &#x2212;  k  1        &#x03BB;                             &#x03BB;  2
                  &#xA0; ( &#x03BB;  ) ( &#x03BB;      2   &#x2212; 2    &#xA0; ( &#x03BB;  &#x2212; 2 c &#x03BB;
               &#x2212; k  )  2      &#x2212;  k  2    c &#x03BB; + 1 &#x2212; 1  )  2      + 1   {\displaystyle
Characteristic {\displaystyle \      )                 {\displaystyle {\displaystyle \      \lambda ^{2}-
polynomial     (\lambda -k)^{2}}  [\ {\displaystyle    \lambda ^{2}-  (\lambda -1)^{2}}  [\ 2c\lambda +1}
               (\lambda -k)^{2}]     (\lambda -k_{1})  2c\lambda +1}  (\lambda -1)^{2}]     [\lambda ^{2}-
                                     (\lambda -k_{2})} [\lambda ^{2}-                       2c\lambda +1]
                                     [(\lambda -k_{1}) 2c\lambda +1]
                                     (\lambda -k_{2})]
                                                           &#x03BB;
                                                       1   =  e   i
                                                       &#x03B8;   = c
                                                       + s  i
                                                       {\displaystyle
                                                       \lambda _
                                                       {1}=e^{\mathbf
                                                       {i} \theta
                                                       }=c+s\mathbf
                                                       {i} }  [
                                                       {\displaystyle
                                         &#x03BB;  1   \lambda _                                &#x03BB;  1   =
                                     =  k  1           {1}=e^{\mathbf                       e  &#x03C6;
                                     {\displaystyle    {i} \theta                           {\displaystyle
                   &#x03BB;  1   =   \lambda _{1}=k_   }=c+s\mathbf       &#x03BB;  1   =   \lambda _{1}=e^
Eigenvalues,   &#x03BB;  2   = k     {1}}  [\lambda _  {i} }]         &#x03BB;  2   = 1     {\varphi }}  [\lambda
&#x03BB;  i    {\displaystyle        {1}=k_{1}]            &#x03BB;   {\displaystyle        _{1}=e^{\varphi }]
{\displaystyle \lambda _{1}=\lambda      &#x03BB;  2   2   =  e       \lambda _{1}=\lambda      &#x03BB;  2   =
\lambda _{i}}  _{2}=k}  [\lambda _   =  k  2           &#x2212;  i    _{2}=1}  [\lambda _   e  &#x2212; &#x03C6;
[\lambda _{i}] {1}=\lambda _{2}=k]   {\displaystyle    &#x03B8;   = c {1}=\lambda _{2}=1]   {\displaystyle
                                     \lambda _{2}=k_   &#x2212; s  i                        \lambda _{2}=e^{-
                                     {2}}  [\lambda _  {\displaystyle                       \varphi }}  [\lambda
                                     {2}=k_{2}]        \lambda _                            _{2}=e^{-\varphi }],
                                                       {2}=e^{-
                                                       \mathbf {i}
                                                       \theta }=c-
                                                       s\mathbf {i} }
                                                       [
                                                       {\displaystyle
                                                       \lambda _
                                                       {2}=e^{-
                                                       \mathbf {i}
                                                       \theta }=c-
                                                       s\mathbf {i}
                                                       }]
Algebraic
mult.,
    &#x03BC;                             &#x03BC;  1       &#x03BC;
i   = &#x03BC;                       = 1               1   = 1
(  &#x03BB;  i                       {\displaystyle    {\displaystyle                           &#x03BC;  1   = 1
)                  &#x03BC;  1   = 2 \mu _{1}=1}  [\mu \mu _{1}=1}        &#x03BC;  1   = 2 {\displaystyle \mu _
{\displaystyle {\displaystyle \mu _  _{1}=1]           [\mu _{1}=1]   {\displaystyle \mu _  {1}=1}  [\mu _{1}=1]
\mu _{i}=\mu   {1}=2}  [\mu _{1}=2]      &#x03BC;  2       &#x03BC;   {1}=2}  [\mu _{1}=2]      &#x03BC;  2   = 1
(\lambda _                           = 1               2   = 1                              {\displaystyle \mu _
{i})}  [                             {\displaystyle    {\displaystyle                       {2}=1}  [\mu _{2}=1]
{\displaystyle                       \mu _{2}=1}  [\mu \mu _{2}=1}
\mu _{i}=\mu                         _{2}=1]           [\mu _{2}=1]
(\lambda _
{i})}]
Geometric
mult.,                                                     &#x03B3;
    &#x03B3;                             &#x03B3;  1   1   = 1
i   = &#x03B3;                       = 1               {\displaystyle                           &#x03B3;  1   = 1
(  &#x03BB;  i                       {\displaystyle    \gamma _{1}=1}                       {\displaystyle \gamma
)                  &#x03B3;  1   = 2 \gamma _{1}=1}    [\gamma _          &#x03B3;  1   = 1 _{1}=1}  [\gamma _
{\displaystyle {\displaystyle \gamma [\gamma _{1}=1]   {1}=1]         {\displaystyle \gamma {1}=1]
\gamma _       _{1}=2}  [\gamma _        &#x03B3;  2       &#x03B3;   _{1}=1}  [\gamma _        &#x03B3;  2   = 1
{i}=\gamma     {1}=2]                = 1               2   = 1        {1}=1]                {\displaystyle \gamma
(\lambda _                           {\displaystyle    {\displaystyle                       _{2}=1}  [\gamma _
{i})}  [\gamma                       \gamma _{2}=1}    \gamma _{2}=1}                       {2}=1]
_{i}=\gamma                          [\gamma _{2}=1]   [\gamma _
(\lambda _                                             {2}=1]
{i})]
                                                               u  1
                                                       =
                                                       [     &#xA0;
                                                       1     &#x2212;
                                                       i     ]
                                                       u  2      =
                                             u  1      [     &#xA0;                                 u  1      =
                                     =   [    1     0  1     +  i                           [     &#xA0;  1
                                     ]        u  2     ]                                    &#xA0;  1    ]
                                     =   [    0     1  {\displaystyle                       u  2      =
                                     ]                 {\begin                              [     &#xA0;  1
                                     {\displaystyle    {aligned}u_                          &#x2212; 1    ]   .
                                     {\begin           {1}&={\begin                         {\displaystyle
                                     {aligned}u_{1}&=  {bmatrix}{\        u  1   =   [    1 {\begin{aligned}u_
                                     {\begin           }1\\-\mathbf   0    ]                {1}&={\begin{bmatrix}
                                     {bmatrix}1\\0\end {i} \end       {\displaystyle u_{1}= {\ }1\\{\ }1\end
                                     {bmatrix}}\\u_    {bmatrix}}\\u_ {\begin               {bmatrix}}\\u_{2}&=
                                     {2}&={\begin      {2}&={\begin   {bmatrix}1\\0\end     {\begin{bmatrix}{\
Eigenvectors   All non-zero vectors  {bmatrix}0\\1\end {bmatrix}{\    {bmatrix}}}  [        }1\\-1\end
                                     {bmatrix}}\end    }1\\+\mathbf   {\displaystyle u_{1}= {bmatrix}}.\end
                                     {aligned}}}  [    {i} \end       {\begin               {aligned}}}  [
                                     {\displaystyle    {bmatrix}}\end {bmatrix}1\\0\end     {\displaystyle
                                     {\begin           {aligned}}}  [ {bmatrix}}}]          {\begin{aligned}u_
                                     {aligned}u_{1}&=  {\displaystyle                       {1}&={\begin{bmatrix}
                                     {\begin           {\begin                              {\ }1\\{\ }1\end
                                     {bmatrix}1\\0\end {aligned}u_                          {bmatrix}}\\u_{2}&=
                                     {bmatrix}}\\u_    {1}&={\begin                         {\begin{bmatrix}{\
                                     {2}&={\begin      {bmatrix}{\                          }1\\-1\end
                                     {bmatrix}0\\1\end }1\\-\mathbf                         {bmatrix}}.\end
                                     {bmatrix}}\end    {i} \end                             {aligned}}}]
                                     {aligned}}}]      {bmatrix}}\\u_
                                                       {2}&={\begin
                                                       {bmatrix}{\
                                                       }1\\+\mathbf
                                                       {i} \end
                                                       {bmatrix}}\end
                                                       {aligned}}}]
The characteristic equation for a rotation is a quadratic_equation with
discriminant     D = &#x2212; 4 ( sin &#x2061; &#x03B8;  )  2
{\displaystyle D=-4(\sin \theta )^{2}}  [D=-4(\sin \theta )^{2}], which is a
negative number whenever Î¸ is not an integer multiple of 180Â°. Therefore,
except for these special cases, the two eigenvalues are complex numbers,
cos &#x2061; &#x03B8; &#x00B1;  i  sin &#x2061; &#x03B8;   {\displaystyle \cos
\theta \pm \mathbf {i} \sin \theta }  [\cos \theta \pm \mathbf {i} \sin \theta
]; and all eigenvectors have non-real entries. Indeed, except for those special
cases, a rotation changes the direction of every nonzero vector in the plane.
A linear transformation that takes a square to a rectangle of the same area (a
squeeze_mapping) has reciprocal eigenvalues.
**** SchrÃ¶dinger equation[edit] ****
The wavefunctions associated with the bound_states of an electron in a hydrogen
atom can be seen as the eigenvectors of the hydrogen_atom_Hamiltonian as well
as of the angular_momentum_operator. They are associated with eigenvalues
interpreted as their energies (increasing downward:     n = 1 ,  2 ,  3 ,
&#x2026;   {\displaystyle n=1,\,2,\,3,\,\ldots }  [{\displaystyle
n=1,\,2,\,3,\,\ldots }]) and angular_momentum (increasing across: s, p, d,
â¦). The illustration shows the square of the absolute value of the
wavefunctions. Brighter areas correspond to higher probability_density for a
position measurement. The center of each figure is the atomic_nucleus, a
proton.
An example of an eigenvalue equation where the transformation     T
{\displaystyle T}  [T] is represented in terms of a differential operator is
the time-independent SchrÃ¶dinger_equation in quantum_mechanics:
         H  &#x03C8;  E   = E  &#x03C8;  E      {\displaystyle H\psi _{E}=E\psi
      _{E}\,}  [H\psi _{E}=E\psi _{E}\,]
where     H   {\displaystyle H}  [H], the Hamiltonian, is a second-order
differential_operator and      &#x03C8;  E     {\displaystyle \psi _{E}}  [\psi
_{E}], the wavefunction, is one of its eigenfunctions corresponding to the
eigenvalue     E   {\displaystyle E}  [E], interpreted as its energy.
However, in the case where one is interested only in the bound_state solutions
of the SchrÃ¶dinger equation, one looks for      &#x03C8;  E     {\displaystyle
\psi _{E}}  [\psi _{E}] within the space of square_integrable functions. Since
this space is a Hilbert_space with a well-defined scalar_product, one can
introduce a basis_set in which      &#x03C8;  E     {\displaystyle \psi _{E}}
[\psi _{E}] and     H   {\displaystyle H}  [H] can be represented as a one-
dimensional array (i.e., a vector) and a matrix respectively. This allows one
to represent the SchrÃ¶dinger equation in a matrix form.
The braâket_notation is often used in this context. A vector, which
represents a state of the system, in the Hilbert space of square integrable
functions is represented by      |   &#x03A8;  E   &#x27E9;   {\displaystyle
|\Psi _{E}\rangle }  [|\Psi _{E}\rangle ]. In this notation, the SchrÃ¶dinger
equation is:
         H  |   &#x03A8;  E   &#x27E9; = E  |   &#x03A8;  E   &#x27E9;
      {\displaystyle H|\Psi _{E}\rangle =E|\Psi _{E}\rangle }  [H|\Psi _
      {E}\rangle =E|\Psi _{E}\rangle ]
where      |   &#x03A8;  E   &#x27E9;   {\displaystyle |\Psi _{E}\rangle }
[|\Psi _{E}\rangle ] is an eigenstate of     H   {\displaystyle H}  [H] and
E   {\displaystyle E}  [E] represents the eigenvalue.     H   {\displaystyle H}
[H] is an observable self_adjoint_operator, the infinite-dimensional analog of
Hermitian matrices. As in the matrix case, in the equation above     H  |
&#x03A8;  E   &#x27E9;   {\displaystyle H|\Psi _{E}\rangle }  [H|\Psi _
{E}\rangle ] is understood to be the vector obtained by application of the
transformation     H   {\displaystyle H}  [H] to      |   &#x03A8;  E
&#x27E9;   {\displaystyle |\Psi _{E}\rangle }  [|\Psi _{E}\rangle ].
**** Molecular orbitals[edit] ****
In quantum_mechanics, and in particular in atomic and molecular_physics, within
the HartreeâFock theory, the atomic and molecular_orbitals can be defined by
the eigenvectors of the Fock_operator. The corresponding eigenvalues are
interpreted as ionization_potentials via Koopmans'_theorem. In this case, the
term eigenvector is used in a somewhat more general meaning, since the Fock
operator is explicitly dependent on the orbitals and their eigenvalues. Thus,
if one wants to underline this aspect, one speaks of nonlinear eigenvalue
problems. Such equations are usually solved by an iteration procedure, called
in this case self-consistent_field method. In quantum_chemistry, one often
represents the HartreeâFock equation in a non-orthogonal basis_set. This
particular representation is a generalized_eigenvalue_problem called Roothaan
equations.
**** Geology and glaciology[edit] ****
In geology, especially in the study of glacial_till, eigenvectors and
eigenvalues are used as a method by which a mass of information of a clast
fabric's constituents' orientation and dip can be summarized in a 3-D space by
six numbers. In the field, a geologist may collect such data for hundreds or
thousands of clasts in a soil sample, which can only be compared graphically
such as in a Tri-Plot (Sneed and Folk) diagram,[42][43] or as a Stereonet on a
Wulff Net.[44]
The output for the orientation tensor is in the three orthogonal
(perpendicular) axes of space. The three eigenvectors are ordered      v  1   ,
v  2   ,  v  3     {\displaystyle v_{1},v_{2},v_{3}}  [v_{1},v_{2},v_{3}] by
their eigenvalues      E  1   &#x2265;  E  2   &#x2265;  E  3
{\displaystyle E_{1}\geq E_{2}\geq E_{3}}  [E_{1}\geq E_{2}\geq E_{3}];[45]
v  1     {\displaystyle v_{1}}  [v_{1}] then is the primary orientation/dip of
clast,      v  2     {\displaystyle v_{2}}  [v_{2}] is the secondary and      v
3     {\displaystyle v_{3}}  [v_{3}] is the tertiary, in terms of strength. The
clast orientation is defined as the direction of the eigenvector, on a compass
rose of 360Â°. Dip is measured as the eigenvalue, the modulus of the tensor:
this is valued from 0Â° (no dip) to 90Â° (vertical). The relative values of
E  1     {\displaystyle E_{1}}  [E_{1}],      E  2     {\displaystyle E_{2}}
[E_{2}], and      E  3     {\displaystyle E_{3}}  [E_{3}] are dictated by the
nature of the sediment's fabric. If      E  1   =  E  2   =  E  3
{\displaystyle E_{1}=E_{2}=E_{3}}  [E_{1}=E_{2}=E_{3}], the fabric is said to
be isotropic. If      E  1   =  E  2   >  E  3     {\displaystyle E_{1}=E_
{2}>E_{3}}  [E_{1}=E_{2}>E_{3}], the fabric is said to be planar. If      E  1
>  E  2   >  E  3     {\displaystyle E_{1}>E_{2}>E_{3}}  [E_{1}>E_{2}>E_{3}],
the fabric is said to be linear.[46]
**** Principal component analysis[edit] ****
PCA of the multivariate_Gaussian_distribution centered at     ( 1 , 3 )
{\displaystyle (1,3)}  [{\displaystyle (1,3)}] with a standard deviation of 3
in roughly the     ( 0.878 , 0.478 )   {\displaystyle (0.878,0.478)}  [
{\displaystyle (0.878,0.478)}] direction and of 1 in the orthogonal direction.
The vectors shown are unit eigenvectors of the (symmetric, positive-
semidefinite) covariance_matrix scaled by the square root of the corresponding
eigenvalue. (Just as in the one-dimensional case, the square root is taken
because the standard_deviation is more readily visualized than the variance.
Main article: Principal_component_analysis
See also: Positive_semidefinite_matrix and Factor_analysis
The eigendecomposition of a symmetric positive_semidefinite (PSD) matrix yields
an orthogonal_basis of eigenvectors, each of which has a nonnegative
eigenvalue. The orthogonal decomposition of a PSD matrix is used in
multivariate_analysis, where the sample covariance_matrices are PSD. This
orthogonal decomposition is called principal_components_analysis (PCA) in
statistics. PCA studies linear_relations among variables. PCA is performed on
the covariance_matrix or the correlation_matrix (in which each variable is
scaled to have its sample_variance equal to one). For the covariance or
correlation matrix, the eigenvectors correspond to principal_components and the
eigenvalues to the variance_explained by the principal components. Principal
component analysis of the correlation matrix provides an orthonormal_eigen-
basis for the space of the observed data: In this basis, the largest
eigenvalues correspond to the principal components that are associated with
most of the covariability among a number of observed data.
Principal component analysis is used to study large data_sets, such as those
encountered in bioinformatics, data_mining, chemical_research, psychology, and
in marketing. PCA is also popular in psychology, especially within the field of
psychometrics. In Q_methodology, the eigenvalues of the correlation matrix
determine the Q-methodologist's judgment of practical significance (which
differs from the statistical_significance of hypothesis_testing; cf. criteria
for_determining_the_number_of_factors). More generally, principal component
analysis can be used as a method of factor_analysis in structural_equation
modeling.
**** Vibration analysis[edit] ****
Mode shape of a tuning fork at eigenfrequency 440.09 Hz
Main article: Vibration
Eigenvalue problems occur naturally in the vibration analysis of mechanical
structures with many degrees_of_freedom. The eigenvalues are the natural
frequencies (or eigenfrequencies) of vibration, and the eigenvectors are the
shapes of these vibrational modes. In particular, undamped vibration is
governed by
         m    x &#x00A8;    + k x = 0   {\displaystyle m{\ddot {x}}+kx=0}  [
      {\displaystyle m{\ddot {x}}+kx=0}]
or
         m    x &#x00A8;    = &#x2212; k x   {\displaystyle m{\ddot {x}}=-kx}
      [{\displaystyle m{\ddot {x}}=-kx}]
that is, acceleration is proportional to position (i.e., we expect     x
{\displaystyle x}  [x] to be sinusoidal in time).
In     n   {\displaystyle n}  [n] dimensions,     m   {\displaystyle m}  [m]
becomes a mass_matrix and     k   {\displaystyle k}  [k] a stiffness_matrix.
Admissible solutions are then a linear combination of solutions to the
generalized_eigenvalue_problem
         k x =  &#x03C9;  2   m x   {\displaystyle kx=\omega ^{2}mx}  [
      {\displaystyle kx=\omega ^{2}mx}]
where      &#x03C9;  2     {\displaystyle \omega ^{2}}  [\omega ^{2}] is the
eigenvalue and     &#x03C9;   {\displaystyle \omega }  [\omega ] is the
(imaginary) angular_frequency. The principal vibration modes are different from
the principal compliance modes, which are the eigenvectors of     k
{\displaystyle k}  [k] alone. Furthermore, damped_vibration, governed by
         m    x &#x00A8;    + c    x &#x02D9;    + k x = 0   {\displaystyle m
      {\ddot {x}}+c{\dot {x}}+kx=0}  [{\displaystyle m{\ddot {x}}+c{\dot
      {x}}+kx=0}]
leads to a so-called quadratic_eigenvalue_problem,
          (   &#x03C9;  2   m + &#x03C9; c + k  )  x = 0.   {\displaystyle
      \left(\omega ^{2}m+\omega c+k\right)x=0.}  [{\displaystyle \left(\omega ^
      {2}m+\omega c+k\right)x=0.}]
This can be reduced to a generalized eigenvalue problem by algebraic
manipulation at the cost of solving a larger system.
The orthogonality properties of the eigenvectors allows decoupling of the
differential equations so that the system can be represented as linear
summation of the eigenvectors. The eigenvalue problem of complex structures is
often solved using finite_element_analysis, but neatly generalize the solution
to scalar-valued vibration problems.
**** Eigenfaces[edit] ****
Eigenfaces as examples of eigenvectors
Main article: Eigenface
In image_processing, processed images of faces can be seen as vectors whose
components are the brightnesses of each pixel.[47] The dimension of this vector
space is the number of pixels. The eigenvectors of the covariance_matrix
associated with a large set of normalized pictures of faces are called
eigenfaces; this is an example of principal_component_analysis. They are very
useful for expressing any face image as a linear_combination of some of them.
In the facial_recognition branch of biometrics, eigenfaces provide a means of
applying data_compression to faces for identification purposes. Research
related to eigen vision systems determining hand gestures has also been made.
Similar to this concept, eigenvoices represent the general direction of
variability in human pronunciations of a particular utterance, such as a word
in a language. Based on a linear combination of such eigenvoices, a new voice
pronunciation of the word can be constructed. These concepts have been found
useful in automatic speech recognition systems for speaker adaptation.
**** Tensor of moment of inertia[edit] ****
In mechanics, the eigenvectors of the moment_of_inertia_tensor define the
principal_axes of a rigid_body. The tensor of moment of inertia is a key
quantity required to determine the rotation of a rigid body around its center
of_mass.
**** Stress tensor[edit] ****
In solid_mechanics, the stress tensor is symmetric and so can be decomposed
into a diagonal tensor with the eigenvalues on the diagonal and eigenvectors as
a basis. Because it is diagonal, in this orientation, the stress tensor has no
shear components; the components it does have are the principal components.
**** Graphs[edit] ****
In spectral_graph_theory, an eigenvalue of a graph is defined as an eigenvalue
of the graph's adjacency_matrix     A   {\displaystyle A}  [A], or
(increasingly) of the graph's Laplacian_matrix due to its discrete_Laplace
operator, which is either     D &#x2212; A   {\displaystyle D-A}  [
{\displaystyle D-A}] (sometimes called the combinatorial Laplacian) or     I
&#x2212;  D  &#x2212; 1  /  2   A  D  &#x2212; 1  /  2     {\displaystyle I-D^
{-1/2}AD^{-1/2}}  [{\displaystyle I-D^{-1/2}AD^{-1/2}}] (sometimes called the
normalized Laplacian), where     D   {\displaystyle D}  [D] is a diagonal
matrix with      D  i i     {\displaystyle D_{ii}}  [{\displaystyle D_{ii}}]
equal to the degree of vertex      v  i     {\displaystyle v_{i}}  [v_{i}], and
in      D  &#x2212; 1  /  2     {\displaystyle D^{-1/2}}  [D^{-1/2}], the     i
{\displaystyle i}  [i]th diagonal entry is     1  /    deg &#x2061; (  v  i   )
{\displaystyle 1/{\sqrt {\deg(v_{i})}}}  [{\displaystyle 1/{\sqrt {\deg(v_
{i})}}}]. The     k   {\displaystyle k}  [k]th principal eigenvector of a graph
is defined as either the eigenvector corresponding to the     k
{\displaystyle k}  [k]th largest or     k   {\displaystyle k}  [k]th smallest
eigenvalue of the Laplacian. The first principal eigenvector of the graph is
also referred to merely as the principal eigenvector.
The principal eigenvector is used to measure the centrality of its vertices. An
example is Google's PageRank algorithm. The principal eigenvector of a modified
adjacency_matrix of the World Wide Web graph gives the page ranks as its
components. This vector corresponds to the stationary_distribution of the
Markov_chain represented by the row-normalized adjacency matrix; however, the
adjacency matrix must first be modified to ensure a stationary distribution
exists. The second smallest eigenvector can be used to partition the graph into
clusters, via spectral_clustering. Other methods are also available for
clustering.
**** Basic reproduction number[edit] ****
Main article: Basic_reproduction_number
The basic reproduction number (     R  0     {\displaystyle R_{0}}  [R_{0}]) is
a fundamental number in the study of how infectious diseases spread. If one
infectious person is put into a population of completely susceptible people,
then      R  0     {\displaystyle R_{0}}  [R_{0}] is the average number of
people that one typical infectious person will infect. The generation time of
an infection is the time,      t  G     {\displaystyle t_{G}}  [t_{G}], from
one person becoming infected to the next person becoming infected. In a
heterogeneous population, the next generation matrix defines how many people in
the population will become infected after time      t  G     {\displaystyle t_
{G}}  [t_{G}] has passed.      R  0     {\displaystyle R_{0}}  [R_{0}] is then
the largest eigenvalue of the next generation matrix.[48][49]
***** See also[edit] *****
    * Antieigenvalue_theory
    * Eigenoperator
    * Eigenplane
    * Eigenvalue_algorithm
    * Introduction_to_eigenstates
    * Jordan_normal_form
    * List_of_numerical_analysis_software
    * Nonlinear_eigenproblem
    * Quadratic_eigenvalue_problem
    * Singular_value
***** Notes[edit] *****
   1. ^ By doing Gaussian_elimination over formal_power_series truncated to
      n   {\displaystyle n}  [n] terms it is possible to get away with     O
      (  n  4   )   {\displaystyle O(n^{4})}  [O(n^{4})] operations, but that
      does not take combinatorial_explosion into account.
***** References[edit] *****
**** Citations[edit] ****
   1. ^ a b Herstein_1964, pp. 228,229.
   2. ^ a b Nering_1970, p. 38.
   3. ^ Burden_&_Faires_1993, p. 401.
   4. ^ Betteridge_1965.
   5. ^ Press_2007, p. 536.
   6. ^Weisstein, Eric W. "Eigenvector". mathworld.wolfram.com. Retrieved 2019-
      08-04.
   7. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   8. ^ a b c d Nering_1970, p. 107.
   9. ^ Note:
          o In 1751, Leonhard Euler proved that any body has a principal axis
            of rotation: Leonhard Euler (presented: October 1751 ; published:
            1760) "Du_mouvement_d'un_corps_solide_quelconque_lorsqu'il_tourne
            autour_d'un_axe_mobile" (On the movement of any solid body while it
            rotates around a moving axis), Histoire de l'AcadÃ©mie royale des
            sciences et des belles lettres de Berlin, pp. 176â227. On_p._212,
            Euler proves that any body contains a principal axis of rotation:
            "ThÃ©orem. 44. De quelque figure que soit le corps, on y peut
            toujours assigner un tel axe, qui passe par son centre de gravitÃ©,
            autour duquel le corps peut tourner librement & d'un mouvement
            uniforme." (Theorem. 44. Whatever be the shape of the body, one can
            always assign to it such an axis, which passes through its center
            of gravity, around which it can rotate freely and with a uniform
            motion.)
          o In 1755, Johann_Andreas_Segner proved that any body has three
            principal axes of rotation: Johann Andreas Segner, Specimen
            theoriae turbinum [Essay on the theory of tops (i.e., rotating
            bodies)] ( Halle ("Halae"), (Germany) : Gebauer, 1755). p._XXVIIII_
            (i.e.,_29), Segner derives a third-degree equation in t, which
            proves that a body has three principal axes of rotation. He then
            states (on the same page): "Non autem repugnat tres esse eiusmodi
            positiones plani HM, quia in aequatione cubica radices tres esse
            possunt, et tres tangentis t valores." (However, it is not
            inconsistent [that there] be three such positions of the plane HM,
            because in cubic equations, [there] can be three roots, and three
            values of the tangent t.)
          o The relevant passage of Segner's work was discussed briefly by
            Arthur_Cayley. See: A. Cayley (1862) "Report on the progress of the
            solution of certain special problems of dynamics," Report of the
            Thirty-second meeting of the British Association for the
            Advancement of Science; held at Cambridge in October 1862, 32 :
            184â252 ; see especially 225â226.
  10. ^ Hawkins_1975, Â§2.
  11. ^ Hawkins_1975, Â§3.
  12. ^ Kline_1972, pp. 807â808 Augustin Cauchy (1839) "MÃ©moire sur
      l'intÃ©gration des Ã©quations linÃ©aires" (Memoir on the integration of
      linear equations), Comptes rendus, 8 : 827â830, 845â865, 889â907,
      931â937. From_p._827: "On sait d'ailleurs qu'en suivant la mÃ©thode de
      Lagrange, on obtient pour valeur gÃ©nÃ©rale de la variable prinicipale
      une fonction dans laquelle entrent avec la variable principale les
      racines d'une certaine Ã©quation que j'appellerai l'Ã©quation
      caractÃ©ristique, le degrÃ© de cette Ã©quation Ã©tant prÃ©cisÃ©ment
      l'order de l'Ã©quation diffÃ©rentielle qu'il s'agit d'intÃ©grer." (One
      knows, moreover, that by following Lagrange's method, one obtains for the
      general value of the principal variable a function in which there appear,
      together with the principal variable, the roots of a certain equation
      that I will call the "characteristic equation", the degree of this
      equation being precisely the order of the differential equation that must
      be integrated.)
  13. ^ Kline_1972, p. 673.
  14. ^ a b c See Hawkins_1975, Â§3
  15. ^ a b See Kline_1972, pp. 807â808
  16. ^ Kline_1972, pp. 715â716.
  17. ^ Kline_1972, pp. 706â707.
  18. ^ Kline_1972, p. 1063.
  19. ^ See:
          o David Hilbert (1904) "GrundzÃ¼ge_einer_allgemeinen_Theorie_der
            linearen_Integralgleichungen._(Erste_Mitteilung)" (Fundamentals of
            a general theory of linear integral equations. (First report)),
            Nachrichten von der Gesellschaft der Wissenschaften zu GÃ¶ttingen,
            Mathematisch-Physikalische Klasse (News of the Philosophical
            Society at GÃ¶ttingen, mathematical-physical section), pp. 49â91.
            From_page_51: "Insbesondere in dieser ersten Mitteilung gelange ich
            zu Formeln, die die Entwickelung einer willkÃ¼rlichen Funktion nach
            gewissen ausgezeichneten Funktionen, die ichEigenfunktionennenne,
            liefern: â¦ (In particular, in this first report I arrive at
            formulas that provide the [series] development of an arbitrary
            function in terms of some distinctive functions, which I call
            eigenfunctions: â¦ ) Later on the same page: "Dieser Erfolg ist
            wesentlich durch den Umstand bedingt, daÃ ich nicht, wie es bisher
            geschah, in erster Linie auf den Beweis fÃ¼r die Existenz der
            Eigenwerte ausgehe, â¦ " (This success is mainly attributable to
            the fact that I do not, as it has happened until now, first of all
            aim at a proof of the existence of eigenvalues, â¦ )
          o For the origin and evolution of the terms eigenvalue,
            characteristic value, etc., see: Earliest_Known_Uses_of_Some_of_the
            Words_of_Mathematics_(E)
  20. ^ Aldrich_2006.
  21. ^Francis, J. G. F. (1961), "The QR Transformation, I (part 1)", The
      Computer Journal, 4 (3): 265â271, doi:10.1093/comjnl/4.3.265
  22.  andFrancis, J. G. F. (1962), "The QR Transformation, II (part 2)", The
      Computer Journal, 4 (4): 332â345, doi:10.1093/comjnl/4.4.332
  23. ^Kublanovskaya, Vera N. (1961), "On some algorithms for the solution of
      the complete eigenvalue problem", USSR Computational Mathematics and
      Mathematical Physics, 3: 637â657
  24. . Also published in:"Ð Ð½ÐµÐºÐ¾ÑÐ¾ÑÑÑ Ð°Ð»Ð³Ð¾ÑÐ¸ÑÐ¼Ð°Ñ Ð´Ð»Ñ
      ÑÐµÑÐµÐ½Ð¸Ñ Ð¿Ð¾Ð»Ð½Ð¾Ð¹ Ð¿ÑÐ¾Ð±Ð»ÐµÐ¼Ñ ÑÐ¾Ð±ÑÑÐ²ÐµÐ½Ð½ÑÑ
      Ð·Ð½Ð°ÑÐµÐ½Ð¸Ð¹" [On certain algorithms for the solution of the complete
      eigenvalue problem], ÐÑÑÐ½Ð°Ð» Ð²ÑÑÐ¸ÑÐ»Ð¸ÑÐµÐ»ÑÐ½Ð¾Ð¹
      Ð¼Ð°ÑÐµÐ¼Ð°ÑÐ¸ÐºÐ¸ Ð¸ Ð¼Ð°ÑÐµÐ¼Ð°ÑÐ¸ÑÐµÑÐºÐ¾Ð¹ ÑÐ¸Ð·Ð¸ÐºÐ¸
      (Journal of Computational Mathematics and Mathematical Physics), 1 (4):
      555â570, 1961
  25. ^ Golub_&_van_Loan_1996, Â§7.3.
  26. ^ Meyer_2000, Â§7.3.
  27. ^ Cornell University Department of Mathematics (2016) Lower-Level_Courses
      for_Freshmen_and_Sophomores. Accessed on 2016-03-27.
  28. ^ University of Michigan Mathematics (2016) Math_Course_Catalogue
      Archived 2015-11-01 at the Wayback_Machine. Accessed on 2016-03-27.
  29. ^ Press_2007, pp. 38.
  30. ^ Fraleigh_1976, p. 358.
  31. ^ a b c Golub_&_Van_Loan_1996, p. 316.
  32. ^ Anton_1987, pp. 305,307.
  33. ^ a b Beauregard_&_Fraleigh_1973, p. 307.
  34. ^ Herstein_1964, p. 272.
  35. ^ Nering_1970, pp. 115â116.
  36. ^ Herstein_1964, p. 290.
  37. ^ Nering_1970, p. 116.
  38. ^ Korn_&_Korn_2000, Section 14.3.5a.
  39. ^ et_al._1989, p. 217.
  40. ^ Nering_1970, p. 107; Shilov_1977, p. 109 Lemma_for_the_eigenspace
  41. ^Lipschutz, Seymour; Lipson, Marc (2002-08-12). Schaum's_Easy_Outline_of
      Linear_Algebra. McGraw Hill Professional. p. 111. ISBN 9780071398800.
  42. ^ For a proof of this lemma, see Roman_2008, Theorem 8.2 on p. 186;
      Shilov_1977, p. 109; Hefferon_2001, p. 364; Beezer_2006, Theorem EDELI on
      p. 469; and Lemma_for_linear_independence_of_eigenvectors
  43. ^Axler, Sheldon, "Ch. 5", Linear Algebra Done Right (2nd ed.), p. 77
  44. ^ a b c dTrefethen, Lloyd N.; Bau, David (1997), Numerical Linear
      Algebra, SIAM
  45. ^Graham, D.; Midgley, N. (2000), "Graphical representation of particle
      shape using triangular diagrams: an Excel spreadsheet method", Earth
      Surface_Processes_and_Landforms, 25 (13): 1473â1477, Bibcode:
      2000ESPL...25.1473G, doi:10.1002/1096-9837(200012)25:13<1473::AID-
      ESP158>3.0.CO;2-C
  46. ^Sneed, E. D.; Folk, R. L. (1958), "Pebbles in the lower Colorado River,
      Texas, a study of particle morphogenesis", Journal of Geology, 66 (2):
      114â150, Bibcode:1958JG.....66..114S, doi:10.1086/626490
  47. ^Knox-Robinson, C.; Gardoll, Stephen J. (1998), "GIS-stereoplot: an
      interactive stereonet plotting module for ArcView 3.0 geographic
      information system", Computers & Geosciences, 24 (3): 243, Bibcode:
      1998CG.....24..243K, doi:10.1016/S0098-3004(97)00122-2
  48. ^ Stereo32_software
  49. ^Benn, D.; Evans, D. (2004), A Practical Guide to the study of Glacial
      Sediments, London: Arnold, pp. 103â107
  50. ^Xirouhakis, A.; Votsis, G.; Delopoulus, A. (2004), Estimation_of_3D
      motion_and_structure_of_human_faces (PDF), National Technical University
      of Athens
  51. ^ Diekmann O, Heesterbeek JA, Metz JA (1990), "On the definition and the
      computation of the basic reproduction ratio R0 in models for infectious
      diseases in heterogeneous populations", Journal of Mathematical Biology,
      28 (4): 365â382, doi:10.1007/BF00178324, PMID 2117040
  52. ^ Odo Diekmann; J. A. P. Heesterbeek (2000), Mathematical_epidemiology_of
      infectious_diseases, Wiley series in mathematical and computational
      biology, West Sussex, England: John Wiley & Sons
**** Sources[edit] ****
    * Akivis, Max A.; Goldberg, Vladislav V. (1969), Tensor calculus, Russian,
      Science Publishers, Moscow
Aldrich, John (2006), "Eigenvalue,_eigenfunction,_eigenvector,_and_related
terms", in Jeff Miller (ed.), Earliest_Known_Uses_of_Some_of_the_Words_of
Mathematics, retrieved 2006-08-22
Alexandrov, Pavel S. (1968), Lecture notes in analytical geometry, Russian,
Science Publishers, Moscow
Anton, Howard (1987), Elementary Linear Algebra (5th ed.), New York: Wiley,
ISBN 0-471-84819-0
Beauregard, Raymond A.; Fraleigh, John B. (1973), A First Course In Linear
Algebra: with Optional Introduction to Groups, Rings, and Fields, Boston:
Houghton_Mifflin_Co., ISBN 0-395-14017-X
Beezer, Robert A. (2006), A_first_course_in_linear_algebra, Free online book
under GNU licence, University of Puget Sound
Betteridge, Harold T. (1965), The New Cassell's German Dictionary, New York:
Funk_&_Wagnall, LCCN 58-7924
Bowen, Ray M.; Wang, Chao-Cheng (1980), Linear and multilinear algebra, Plenum
Press, New York, ISBN 0-306-37508-7
Burden, Richard L.; Faires, J. Douglas (1993), Numerical Analysis (5th ed.),
Boston: Prindle,_Weber_and_Schmidt, ISBN 0-534-93219-3
Carter, Tamara A.; Tapia, Richard A.; Papaconstantinou, Anne, Linear_Algebra:
An_Introduction_to_Linear_Algebra_for_Pre-Calculus_Students, Rice University,
Online Edition, retrieved 2008-02-19
Cohen-Tannoudji,_Claude (1977), "Chapter II. The mathematical tools of quantum
mechanics", Quantum mechanics, John Wiley & Sons, ISBN 0-471-16432-1
Curtis,_Charles_W. (1999), Linear Algebra: An Introductory Approach (4th ed.),
Springer, ISBN 0-387-90992-3
Demmel,_James_W. (1997), Applied numerical linear algebra, SIAM, ISBN 0-89871-
389-7
Fraleigh, John B. (1976), A First Course In Abstract Algebra (2nd ed.),
Reading: Addison-Wesley, ISBN 0-201-01984-1
Fraleigh, John B.; Beauregard, Raymond A. (1995), Linear algebra (3rd ed.),
Addison-Wesley Publishing Company, ISBN 0-201-83999-7
Friedberg, Stephen H.; Insel, Arnold J.; Spence, Lawrence E. (1989), Linear
algebra (2nd ed.), Englewood Cliffs, New Jersey 07632: Prentice Hall, ISBN 0-
13-537102-3
Gelfand, I. M. (1971), Lecture notes in linear algebra, Russian, Science
Publishers, Moscow
Gohberg, Israel; Lancaster, Peter; Rodman, Leiba (2005), Indefinite linear
algebra and applications, Basel-Boston-Berlin: BirkhÃ¤user Verlag, ISBN 3-7643-
7349-0
Golub, Gene F.; van der Vorst, Henk A. (2000), "Eigenvalue computation in the
20th century", Journal of Computational and Applied Mathematics, 123: 35â65,
Bibcode:2000JCoAM.123...35G, doi:10.1016/S0377-0427(00)00413-1
Golub,_Gene_H.; Van_Loan,_Charles_F. (1996), Matrix computations (3rd ed.),
Johns Hopkins University Press, Baltimore, Maryland, ISBN 978-0-8018-5414-9
Greub, Werner H. (1975), Linear Algebra (4th ed.), Springer-Verlag, New York,
ISBN 0-387-90110-8
Halmos,_Paul_R. (1987), Finite-dimensional vector spaces (8th ed.), New York:
Springer-Verlag, ISBN 0-387-90093-4
Hawkins, T. (1975), "Cauchy and the spectral theory of matrices", Historia
Mathematica, 2: 1â29, doi:10.1016/0315-0860(75)90032-4
Hefferon, Jim (2001), Linear_Algebra, Online book, St Michael's College,
Colchester, Vermont, USA
Herstein, I. N. (1964), Topics In Algebra, Waltham: Blaisdell_Publishing
Company, ISBN 978-1114541016
Horn, Roger A.; Johnson, Charles F. (1985), Matrix analysis, Cambridge
University Press, ISBN 0-521-30586-1
Kline, Morris (1972), Mathematical thought from ancient to modern times, Oxford
University Press, ISBN 0-19-501496-0
Korn, Granino A.; Korn, Theresa M. (2000), "Mathematical Handbook for
Scientists and Engineers: Definitions, Theorems, and Formulas for Reference and
Review", New York: McGraw-Hill (2nd Revised ed.), Dover Publications, Bibcode:
1968mhse.book.....K, ISBN 0-486-41147-8
Kuttler, Kenneth (2007), An_introduction_to_linear_algebra (PDF), Online e-book
in PDF format, Brigham Young University
Lancaster, P. (1973), Matrix theory, Russian, Moscow, Russia: Science
Publishers
Larson, Ron; Edwards, Bruce H. (2003), Elementary linear algebra (5th ed.),
Houghton Mifflin Company, ISBN 0-618-33567-6
Lipschutz, Seymour (1991), Schaum's outline of theory and problems of linear
algebra, Schaum's outline series (2nd ed.), New York: McGraw-Hill Companies,
ISBN 0-07-038007-4
Meyer, Carl D. (2000), Matrix analysis and applied linear algebra, Society for
Industrial and Applied Mathematics (SIAM), Philadelphia, ISBN 978-0-89871-454-8
Nering, Evar D. (1970), Linear Algebra and Matrix Theory (2nd ed.), New York:
Wiley, LCCN 76091646
(in Russian)Pigolkina, T. S.; Shulman, V. S. (1977). "Eigenvalue". In
Vinogradov, I. M. (ed.). Mathematical Encyclopedia. 5. Moscow: Soviet
Encyclopedia.
Press, William H.; Teukolsky,_Saul_A.; Vetterling, William T.; Flannery, Brian
P. (2007), Numerical Recipes: The Art of Scientific Computing (3rd ed.),
ISBN 9780521880688
Roman, Steven (2008), Advanced linear algebra (3rd ed.), New York: Springer
Science + Business Media, LLC, ISBN 978-0-387-72828-5
Sharipov, Ruslan A. (1996), Course of Linear Algebra and Multidimensional
Geometry: the textbook, arXiv:math/0405323, Bibcode:2004math......5323S,
ISBN 5-7477-0099-5
Shilov, Georgi E. (1977), Linear algebra, Translated and edited by Richard A.
Silverman, New York: Dover Publications, ISBN 0-486-63518-X
Shores, Thomas S. (2007), Applied linear algebra and matrix analysis, Springer
Science+Business Media, LLC, ISBN 0-387-33194-8
Strang, Gilbert (1993), Introduction to linear algebra, Wellesley-Cambridge
Press, Wellesley, Massachusetts, ISBN 0-9614088-5-5
Strang, Gilbert (2006), Linear algebra and its applications, Thomson, Brooks/
Cole, Belmont, California, ISBN 0-03-010567-6
***** External links[edit] *****
 The Wikibook Linear_Algebra has a page on the topic of: Eigenvalues_and
 Eigenvectors
    * What_are_Eigen_Values? â non-technical introduction from PhysLink.com's
      "Ask the Experts"
    * Eigen_Values_and_Eigen_Vectors_Numerical_Examples â Tutorial and
      Interactive Program from Revoledu.
    * Introduction_to_Eigen_Vectors_and_Eigen_Values â lecture from Khan
      Academy
    * Hill, Roger (2009). "Î»_â_Eigenvalues". Sixty Symbols. Brady_Haran for
      the University_of_Nottingham.
"A_Beginner's_Guide_to_Eigenvectors". Deeplearning4j. 2015. Archived from the
original on 2018-07-21. Retrieved 2015-08-18.
Eigenvectors_and_eigenvalues_|_Essence_of_linear_algebra,_chapter_10 â A
visual explanation with 3Blue1Brown
Matrix_Eigenvectors_Calculator from Symbolab (Click on the bottom right button
of the 2x12 grid to select a matrix size. Select an     n &#x00D7; n
{\displaystyle n\times n}  [n\times n] size (for a square matrix), then fill
out the entries numerically and click on the Go button. It can accept complex
numbers as well.)
**** Theory[edit] ****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Eigen_value", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Hazewinkel,_Michiel, ed. (2001) [1994], "Eigen_vector", Encyclopedia_of
Mathematics, Springer Science+Business Media B.V. / Kluwer Academic Publishers,
ISBN 978-1-55608-010-4
"Eigenvalue_(of_a_matrix)". PlanetMath.
Eigenvector â Wolfram MathWorld
Eigen_Vector_Examination_working_applet
Same_Eigen_Vector_Examination_as_above_in_a_Flash_demo_with_sound
Computation_of_Eigenvalues
Numerical_solution_of_eigenvalue_problems Edited by Zhaojun Bai, James_Demmel,
Jack Dongarra, Axel Ruhe, and Henk_van_der_Vorst
Eigenvalues and Eigenvectors on the Ask Dr. Math forums: [1], [2]
**** Demonstration applets[edit] ****
    * Java_applet_about_eigenvectors_in_the_real_plane
    * Wolfram_Language_functionality_for_Eigenvalues,_Eigenvectors_and
      Eigensystems
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
                            * Eigenvalues and
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
    * v
    * t
    * e
Areas_of_mathematics
                  * Category_theory
                  * Information_theory
Foundations       * Mathematical_logic
                  * Philosophy_of_mathematics
                  * Set_theory
                  * Abstract
Algebra           * Elementary
                  * Linear
                  * Multilinear
                  * Calculus
                  * Real_analysis
Analysis          * Complex_analysis
                  * Differential_equations
                  * Functional_analysis
                  * Combinatorics
Discrete          * Graph_theory
                  * Order_theory
                  * Game_theory
                  * Algebraic
                  * Analytic
Geometry          * Differential
                  * Discrete
                  * Euclidean
                  * Finite
                  * Arithmetic
Number_theory     * Algebraic_number_theory
                  * Analytic_number_theory
                  * Diophantine_geometry
                  * Algebraic
Topology          * Differential
                  * Geometric
                  * Control_theory
                  * Mathematical_economics
                  * Mathematical_finance
Applied           * Mathematical_physics
                  * Mathematical_statistics
                  * Probability
                  * Statistics
                  * Computer_science
                  * Theory_of_computation
Computational     * Numerical_analysis
                  * Optimization
                  * Computer_algebra
                  * History_of_mathematics
Others            * Recreational_mathematics
                  * Mathematics_and_art
                  * Mathematics_education
    * [Category] Category
    * [Portal] Portal
    * [Commons page]Commons
    * [WikiProject]WikiProject

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Eigenvalues_and_eigenvectors&oldid=909463498"
Categories:
    * Mathematical_physics
    * Abstract_algebra
    * Linear_algebra
    * Matrix_theory
    * Singular_value_decomposition
Hidden categories:
    * Webarchive_template_wayback_links
    * Use_American_English_from_January_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_March_2013
    * Articles_with_Russian-language_external_links
    * Articles_including_recorded_pronunciations
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
    * Asturianu
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Interlingua
    * Italiano
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * Norsk_nynorsk
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 5 August 2019, at 16:15 (UTC).
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
