The following text has been accessed from https://en.wikipedia.org/wiki/Linear_algebra at Thu Aug 8 23:00:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Linear algebra ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with Elementary_algebra.
In the three-dimensional Euclidean_space, these three planes represent
solutions of linear equations and their intersection represents the set of
common solutions: in this case, a unique point. The blue line is the common
solution of a pair of linear equations.
Linear algebra is the branch of mathematics concerning linear_equations such as
          a  1    x  1   + &#x22EF; +  a  n    x  n   = b ,   {\displaystyle a_
      {1}x_{1}+\cdots +a_{n}x_{n}=b,}  [{\displaystyle a_{1}x_{1}+\cdots +a_
      {n}x_{n}=b,}]
linear_functions such as
         (  x  1   , &#x2026; ,  x  n   ) &#x21A6;  a  1    x  1   + &#x2026; +
      a  n    x  n   ,   {\displaystyle (x_{1},\ldots ,x_{n})\mapsto a_{1}x_
      {1}+\ldots +a_{n}x_{n},}  [{\displaystyle (x_{1},\ldots ,x_{n})\mapsto a_
      {1}x_{1}+\ldots +a_{n}x_{n},}]
and their representations through matrices and vector_spaces.[1][2][3]
Linear algebra is central to almost all areas of mathematics. For instance,
linear algebra is fundamental in modern presentations of geometry, including
for defining basic objects such as lines, planes and rotations. Also,
functional_analysis may be basically viewed as the application of linear
algebra to spaces of functions. Linear algebra is also used in most sciences
and engineering areas, because it allows modeling many natural phenomena, and
efficiently computing with such models. For nonlinear_systems, which cannot be
modeled with linear algebra, linear algebra is often used as a first-order
approximation.
⁰
***** Contents *****
    * 1_History
    * 2_Vector_spaces
          o 2.1_Linear_maps
          o 2.2_Subspaces,_span,_and_basis
    * 3_Matrices
    * 4_Linear_systems
    * 5_Endomorphisms_and_square_matrices
          o 5.1_Determinant
          o 5.2_Eigenvalues_and_eigenvectors
    * 6_Duality
          o 6.1_Dual_map
          o 6.2_Inner-product_spaces
    * 7_Relationship_with_geometry
    * 8_Usage_and_applications
          o 8.1_Geometry_of_our_ambient_space
          o 8.2_Functional_analysis
          o 8.3_Study_of_complex_systems
          o 8.4_Scientific_computation
    * 9_Extensions_and_generalizations
          o 9.1_Module_theory
          o 9.2_Multilinear_algebra_and_tensors
          o 9.3_Topological_vector_spaces
          o 9.4_Homological_algebra
    * 10_See_also
    * 11_Notes
    * 12_Further_reading
          o 12.1_History
          o 12.2_Introductory_textbooks
          o 12.3_Advanced_textbooks
          o 12.4_Study_guides_and_outlines
    * 13_External_links
          o 13.1_Online_Resources
          o 13.2_Online_books
***** History[edit] *****
The procedure for solving simultaneous linear equations now called Gaussian
elimination appears in the ancient Chinese mathematical text Chapter_Eight:
Rectangular_Arrays of The_Nine_Chapters_on_the_Mathematical_Art. Its use is
illustrated in eighteen problems, with two to five equations.[4]
Systems_of_linear_equations arose in Europe with the introduction in 1637 by
RenÃ©_Descartes of coordinates in geometry. In fact, in this new geometry, now
called Cartesian_geometry, lines and planes are represented by linear
equations, and computing their intersections amounts to solving systems of
linear equations.
The first systematic methods for solving linear systems used determinants,
first considered by Leibniz in 1693. In 1750, Gabriel_Cramer used them for
giving explicit solutions of linear systems, now called Cramer's_rule. Later,
Gauss further described the method of elimination, which was initially listed
as an advancement in geodesy.[5]
In 1844 Hermann_Grassmann published his "Theory of Extension" which included
foundational new topics of what is today called linear algebra. In 1848, James
Joseph_Sylvester introduced the term matrix, which is Latin for womb.
Linear algebra grew with ideas noted in the complex_plane. For instance, two
numbers w and z in â have a difference w â z, and the line segments
w z  &#x00AF;   &#xA0; &#xA0;  and  &#xA0; &#xA0;    0 ( w &#x2212; z )
&#x00AF;     {\displaystyle {\overline {wz}}\ \ {\text{and}}\ \ {\overline {0
(w-z)}}}  [{\displaystyle {\overline {wz}}\ \ {\text{and}}\ \ {\overline {0(w-
z)}}}] are of the same length and direction. The segments are equipollent. The
four-dimensional system â of quaternions was started in 1843. The term vector
was introduced as v = x i + y j + z k representing a point in space. The
quaternion difference p â q also produces a segment equipollent to        p q
&#x00AF;   .   {\displaystyle {\overline {pq}}.}  [{\displaystyle {\overline
{pq}}.}] Other hypercomplex_number systems also used the idea of a linear space
with a basis.
Arthur_Cayley introduced matrix_multiplication and the inverse_matrix in 1856,
making possible the general_linear_group. The mechanism of group_representation
became available for describing complex and hypercomplex numbers. Crucially,
Cayley used a single letter to denote a matrix, thus treating a matrix as an
aggregate object. He also realized the connection between matrices and
determinants, and wrote "There would be many things to say about this theory of
matrices which should, it seems to me, precede the theory of determinants".[5]
Benjamin_Peirce published his Linear Associative Algebra (1872), and his son
Charles_Sanders_Peirce extended the work later.[6]
The telegraph required an explanatory system, and the 1873 publication of A
Treatise_on_Electricity_and_Magnetism instituted a field_theory of forces and
required differential_geometry for expression. Linear algebra is flat
differential geometry and serves in tangent spaces to manifolds.
Electromagnetic symmetries of spacetime are expressed by the Lorentz
transformations, and much of the history of linear algebra is the history_of
Lorentz_transformations.
The first modern and more precise definition of a vector space was introduced
by Peano in 1888;[5] by 1900, a theory of linear transformations of finite-
dimensional vector spaces had emerged. Linear algebra took its modern form in
the first half of the twentieth century, when many ideas and methods of
previous centuries were generalized as abstract_algebra. The development of
computers led to increased research in efficient algorithms for Gaussian
elimination and matrix decompositions, and linear algebra became an essential
tool for modelling and simulations.[5]
See also Determinant_Â§ History and Gaussian_elimination_Â§ History.
***** Vector spaces[edit] *****
Main article: Vector_space
Until the 19th century, linear algebra was introduced through systems_of_linear
equations and matrices. In modern mathematics, the presentation through vector
spaces is generally preferred, since it is more synthetic, more general (not
limited to the finite-dimensional case), and conceptually simpler, although
more abstract.
A vector space over a field F (often the field of the real_numbers) is a set V
equipped with two binary_operations satisfying the following axioms. Elements
of V are called vectors, and elements of F are called scalars. The first
operation, vector_addition, takes any two vectors v and w and outputs a third
vector v + w. The second operation, scalar_multiplication, takes any scalar a
and any vector v and outputs a new vector av. The axioms that addition and
scalar multiplication must satisfy are the following. (In the list below, u, v
and w are arbitrary elements of V, and a and b are arbitrary scalars in the
field F.)[7]
Axiom                                       Signification
Associativity of addition                   u + (v + w) = (u + v) + w
Commutativity of addition                   u + v = v + u
Identity_element of addition                There exists an element 0 in V, called the zero_vector (or
                                            simply zero), such that v + 0 = v for all v in V.
Inverse_elements of addition                For every v in V, there exists an element âv in V, called
                                            the additive_inverse of v, such that v + (âv) = 0
Distributivity of scalar multiplication     a(u + v) = au + av
with respect to vector additionââ
Distributivity of scalar multiplication     (a + b)v = av + bv
with respect to field addition
Compatibility of scalar multiplication with a(bv) = (ab)v [nb_1]
field multiplication
Identity element of scalar multiplication   1v = v, where 1 denotes the multiplicative_identity of F.
The first four axioms mean that V is an abelian_group under addition.
Elements of a vector space may have various nature; for example, they can be
sequences, functions, polynomials or matrices. Linear algebra is concerned with
properties common to all vector spaces.
**** Linear maps[edit] ****
Main article: Linear_map
Linear maps are mappings between vector spaces that preserve the vector-space
structure. Given two vector spaces V and W over a field F, a linear map (also
called, in some contexts, linear transformation, linear mapping or linear
operator) is a map
         T : V &#x2192; W   {\displaystyle T:V\to W}  [T:V\to W]
that is compatible with addition and scalar multiplication, that is
         T ( u + v ) = T ( u ) + T ( v ) ,  T ( a v ) = a T ( v )
      {\displaystyle T(u+v)=T(u)+T(v),\quad T(av)=aT(v)}  [T(u+v)=T(u)+T
      (v),\quad T(av)=aT(v)]
for any vectors u,v in V and scalar a in F.
This implies that for any vectors u, v in V and scalars a, b in F, one has
         T ( a u + b v ) = T ( a u ) + T ( b v ) = a T ( u ) + b T ( v )
      {\displaystyle T(au+bv)=T(au)+T(bv)=aT(u)+bT(v)}  [{\displaystyle T
      (au+bv)=T(au)+T(bv)=aT(u)+bT(v)}]
When a bijective linear map exists between two vector spaces (that is, every
vector from the second space is associated with exactly one in the first), the
two spaces are isomorphic. Because an isomorphism preserves linear structure,
two isomorphic vector spaces are "essentially the same" from the linear algebra
point of view, in the sense that they cannot be distinguished by using vector
space properties. An essential question in linear algebra is testing whether a
linear map is an isomorphism or not, and, if it is not an isomorphism, finding
its range (or image) and the set of elements that are mapped to the zero
vector, called the kernel of the map. All these questions can be solved by
using Gaussian_elimination or some variant of this algorithm.
**** Subspaces, span, and basis[edit] ****
Main articles: Linear_subspace, Linear_span, and Basis_(linear_algebra)
The study of subsets of vector spaces that are themselves vector spaces for the
induced operations is fundamental, similarly as for many mathematical
structures. These subsets are called linear_subspaces. More precisely, a linear
subspace of a vector space V over a field F is a subset W of V such that u + v
and au are in W, for every u, v in W, and every a in F. (These conditions
suffices for implying that W is a vector space.)
For example, the image of a linear map, and the inverse_image of 0 by a linear
map (called kernel or null_space) are linear subspaces.
Another important way of forming a subspace is to consider linear_combinations
of a set S of vectors: the set of all sums
          a  1    v  1   +  a  2    v  2   + &#x22EF; +  a  k    v  k   ,
      {\displaystyle a_{1}v_{1}+a_{2}v_{2}+\cdots +a_{k}v_{k},}  [a_{1}v_{1}+a_
      {2}v_{2}+\cdots +a_{k}v_{k},]
where v1, v2, ..., vk are in V, and a1, a2, ..., ak are in F form a linear
subspace called the span of S. The span of S is also the intersection of all
linear subspaces containing S. In other words, it is the (smallest for the
inclusion relation) linear subspace containing S.
A set of vectors is linearly_independent if none is in the span of the others.
Equivalently, a set S of vector is linearly independent if the only way to
express the zero vector as a linear combination of elements of S is to take
zero for every coefficient      a  i   .   {\displaystyle a_{i}.}  [a_i.]
A set of vectors that spans a vector space is called a spanning_set or
generating_set. If a spanning set S is linearly dependent (that is not linearly
independent), then some element w of S is in the span of the other elements of
S, and the span would remain the same if one remove w from S. One may continue
to remove elements of S until getting a linearly independent spanning set. Such
a linearly independent set that spans a vector space V is called a basis of V.
The importance of bases lies in the fact that there are together minimal
generating sets and maximal independent sets. More precisely, if S is a
linearly independent set, and T is a spanning set such that     S &#x2286; T ,
{\displaystyle S\subseteq T,}  [{\displaystyle S\subseteq T,}] then there is a
basis B such that     S &#x2286; B &#x2286; T .   {\displaystyle S\subseteq
B\subseteq T.}  [{\displaystyle S\subseteq B\subseteq T.}]
Any two bases of a vector space V have the same cardinality, which is called
the dimension of V; this is the dimension_theorem_for_vector_spaces. Moreover,
two vector spaces over the same field F are isomorphic if and only if they have
the same dimension.[8]
If any basis of V (and therefore every basis) has a finite number of elements,
V is a finite-dimensional vector space. If U is a subspace of V, then dim U â¤
dim V. In the case where V is finite-dimensional, the equality of the
dimensions implies U = V.
If U1 and U2 are subspaces of V, then
         dim &#x2061; (  U  1   +  U  2   ) = dim &#x2061;  U  1   + dim
      &#x2061;  U  2   &#x2212; dim &#x2061; (  U  1   &#x2229;  U  2   ) ,
      {\displaystyle \dim(U_{1}+U_{2})=\dim U_{1}+\dim U_{2}-\dim(U_{1}\cap U_
      {2}),}  [{\displaystyle \dim(U_{1}+U_{2})=\dim U_{1}+\dim U_{2}-\dim(U_
      {1}\cap U_{2}),}]
where      U  1   +  U  2     {\displaystyle U_{1}+U_{2}}  [{\displaystyle U_
{1}+U_{2}}]denotes the span of      U  1   &#x222A;  U  2   .   {\displaystyle
U_{1}\cup U_{2}.}  [{\displaystyle U_{1}\cup U_{2}.}][9]
***** Matrices[edit] *****
Main article: Matrix_(mathematics)
Matrices allow explicit manipulation of finite-dimensional vector spaces and
linear_maps. Their theory is thus an essential part of linear algebra.
Let V be a finite-dimensional vector space over a field F, and (v1, v2, ...,
vm) be a basis of V (thus m is the dimension of V). By definition of a basis,
the map
             (  a  1   , &#x2026; ,  a  m   )    &#x21A6;  a  1    v  1   +
      &#x22EF;  a  m    v  m        F  m      &#x2192; V       {\displaystyle
      {\begin{aligned}(a_{1},\ldots ,a_{m})&\mapsto a_{1}v_{1}+\cdots a_{m}v_
      {m}\\F^{m}&\to V\end{aligned}}}  [{\displaystyle {\begin{aligned}(a_
      {1},\ldots ,a_{m})&\mapsto a_{1}v_{1}+\cdots a_{m}v_{m}\\F^{m}&\to V\end
      {aligned}}}]
is a bijection from      F  m   ,   {\displaystyle F^{m},}  [{\displaystyle F^
{m},}] the set of the sequences of m elements of F, onto V. This is an
isomorphism of vector spaces, if      F  m     {\displaystyle F^{m}}  [
{\displaystyle F^{m}}] is equipped of its standard structure of vector space,
where vector addition and scalar multiplication are done component by
component.
This isomorphism allows representing a vector by its inverse_image under this
isomorphism, that is by the coordinates_vector     (  a  1   , &#x2026; ,  a  m
)   {\displaystyle (a_{1},\ldots ,a_{m})}  [{\displaystyle (a_{1},\ldots ,a_
{m})}] or by the column_matrix
           [     a  1       &#x22EE;      a  m      ]   .   {\displaystyle
      {\begin{bmatrix}a_{1}\\\vdots \\a_{m}\end{bmatrix}}.}  [{\displaystyle
      {\begin{bmatrix}a_{1}\\\vdots \\a_{m}\end{bmatrix}}.}]
If W is another finite dimensional vector space (possibly the same), with a
basis     (  w  1   , &#x2026; ,  w  n   ) ,   {\displaystyle (w_{1},\ldots ,w_
{n}),}  [{\displaystyle (w_{1},\ldots ,w_{n}),}] a linear map f from W to V is
well defined by its values on the basis elements, that is     ( f (  w  1   ) ,
&#x2026; , f (  w  n   ) ) .   {\displaystyle (f(w_{1}),\ldots ,f(w_{n})).}  [
{\displaystyle (f(w_{1}),\ldots ,f(w_{n})).}] Thus, f is well represented by
the list of the corresponding column matrices. That is, if
         f (  w  j   ) =  a  1 , j    v  1   + &#x22EF; +  a  m , j    v  m   ,
      {\displaystyle f(w_{j})=a_{1,j}v_{1}+\cdots +a_{m,j}v_{m},}  [
      {\displaystyle f(w_{j})=a_{1,j}v_{1}+\cdots +a_{m,j}v_{m},}]
for j = 1, ..., n, then f is represented by the matrix
           [     a  1 , 1     &#x2026;    a  1 , n       &#x22EE;   &#x2026;
      &#x22EE;      a  m , 1     &#x2026;    a  m , n      ]   ,
      {\displaystyle {\begin{bmatrix}a_{1,1}&\ldots &a_{1,n}\\\vdots &\ldots
      &\vdots \\a_{m,1}&\ldots &a_{m,n}\end{bmatrix}},}  [{\displaystyle
      {\begin{bmatrix}a_{1,1}&\ldots &a_{1,n}\\\vdots &\ldots &\vdots \\a_
      {m,1}&\ldots &a_{m,n}\end{bmatrix}},}]
with m rows and n columns.
Matrix_multiplication is defined in such a way that the product of two matrices
is the matrix of the composition of the corresponding linear maps, and the
product of a matrix and a column matrix is the column matrix representing the
result of applying the represented linear map to the represented vector. It
follows that the theory of finite-dimensional vector spaces and the theory of
matrices are two different languages for expressing exactly the same concepts.
Two matrices that encode the same linear transformation in different bases are
called similar. Equivalently, two matrices are similar if one can transform one
in the other by elementary_row_and_column_operations. For a matrix representing
a linear map from W to V, the row operations correspond to change of bases in V
and the column operations correspond to change of bases in W. Every matrix is
similar to an identity_matrix possibly bordered by zero rows and zero columns.
In terms of vector space, this means that, for any linear map from W to V,
there are bases such that a part of the basis of W is mapped bijectively on a
part of the basis of V, and that the remaining basis elements of W, if any, are
mapped to zero (this is a way of expressing the fundamental_theorem_of_linear
algebra). Gaussian_elimination is the basic algorithm for finding these
elementary operations, and proving this theorem.
***** Linear systems[edit] *****
Main article: System_of_linear_equations
Systems of linear equations form a fundamental part of linear algebra.
Historically, linear algebra and matrix theory has been developed for solving
such systems. In the modern presentation of linear algebra through vector
spaces and matrices, many problems may be interpreted in terms of linear
systems.
For example, let
             2 x     +     y     &#x2212;     z     =     8     &#x2212; 3 x
      &#x2212;     y     +     2 z     =     &#x2212; 11     &#x2212; 2 x     +
      y     +     2 z     =     &#x2212; 3       (S)    {\displaystyle {\begin
      {alignedat}{7}2x&&\;+\;&&y&&\;-\;&&z&&\;=\;&&8\\-3x&&\;-
      \;&&y&&\;+\;&&2z&&\;=\;&&-11\\-2x&&\;+\;&&y&&\;+\;&&2z&&\;=\;&&-3\end
      {alignedat}}\qquad {\text{(S)}}}  [{\displaystyle {\begin{alignedat}
      {7}2x&&\;+\;&&y&&\;-\;&&z&&\;=\;&&8\\-3x&&\;-\;&&y&&\;+\;&&2z&&\;=\;&&-
      11\\-2x&&\;+\;&&y&&\;+\;&&2z&&\;=\;&&-3\end{alignedat}}\qquad {\text{
      (S)}}}]
be a linear system.
To such a system, one may associate its matrix
         M  [     2   1   &#x2212; 1     &#x2212; 3   &#x2212; 1   2
      &#x2212; 2   1   2     ]   .    {\displaystyle M\left[{\begin{array}
      {rrr}2&1&-1\\-3&-1&2\\-2&1&2\end{array}}\right]{\text{.}}}  [
      {\displaystyle M\left[{\begin{array}{rrr}2&1&-1\\-3&-1&2\\-2&1&2\end
      {array}}\right]{\text{.}}}]
and its right member vector
         v =   [    8     &#x2212; 11     &#x2212; 3    ]   .   {\displaystyle
      v={\begin{bmatrix}8\\-11\\-3\end{bmatrix}}.}  [{\displaystyle v={\begin
      {bmatrix}8\\-11\\-3\end{bmatrix}}.}]
Let T be the linear transformation associated to the matrix M. A solution of
the system (S) is a vector
         X =   [    x     y     z    ]     {\displaystyle X={\begin
      {bmatrix}x\\y\\z\end{bmatrix}}}  [{\displaystyle X={\begin
      {bmatrix}x\\y\\z\end{bmatrix}}}]
such that
         T ( X ) = v ,   {\displaystyle T(X)=v,}  [{\displaystyle T(X)=v,}]
that is an element of the preimage of v by T.
Let (S') be the associated homogeneous_system, where the right-hand sides of
the equations are put to zero. The solutions of (S') are exactly the elements
of the kernel of T or, equivalently, M.
The Gaussian-elimination consists of performing elementary_row_operations on
the augmented_matrix
         M  [     2   1   &#x2212; 1   8     &#x2212; 3   &#x2212; 1   2
      &#x2212; 11     &#x2212; 2   1   2   &#x2212; 3     ]    {\displaystyle
      M\left[{\begin{array}{rrr|r}2&1&-1&8\\-3&-1&2&-11\\-2&1&2&-3\end
      {array}}\right]}  [{\displaystyle M\left[{\begin{array}{rrr|r}2&1&-1&8\\-
      3&-1&2&-11\\-2&1&2&-3\end{array}}\right]}]
for putting it in reduced_row_echelon_form. These row operations do not change
the set of solutions of the system of equations. In the example, the reduced
echelon form is
         M  [     1   0   0   2     0   1   0   3     0   0   1   &#x2212; 1
      ]  ,   {\displaystyle M\left[{\begin{array}
      {rrr|r}1&0&0&2\\0&1&0&3\\0&0&1&-1\end{array}}\right],}  [{\displaystyle
      M\left[{\begin{array}{rrr|r}1&0&0&2\\0&1&0&3\\0&0&1&-1\end
      {array}}\right],}]
showing that the system (S) has the unique solution
             x    = 2     y    = 3     z    = &#x2212; 1.       {\displaystyle
      {\begin{aligned}x&=2\\y&=3\\z&=-1.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}x&=2\\y&=3\\z&=-1.\end{aligned}}}]
It follows from this matrix interpretation of linear systems that the same
methods can be applied for solving linear systems and for many operations on
matrices and linear transformations, which include the computation of the
ranks, kernels, matrix_inverses.
***** Endomorphisms and square matrices[edit] *****
Main article: Square_matrix
A linear endomorphism is a linear map that maps a vector space V to itself. If
V has a basis of n elements, such an endomorphism is represented by a square
matrix of size n.
With respect to general linear maps, linear endomorphisms and square matrices
have some specific properties that make their study an important part of linear
algebra, which is used in many parts of mathematics, including geometric
transformations, coordinate_changes, quadratic_forms, and many other part of
mathematics.
**** Determinant[edit] ****
Main article: Determinant
The determinant of a square matrix is a polynomial_function of the entries of
the matrix, such that the matrix is invertible if and only if the determinant
is not zero. This results from the fact that the determinant of a product of
matrices is the product of the determinants, and thus that a matrix is
invertible if and only if its determinant is invertible.
Cramer's_rule is a closed-form_expression, in terms of determinants, of the
solution of a system_of_n_linear_equations_in_n_unknowns. Cramer's rule is
useful for reasoning about the solution, but, except for n = 2 or 3, it is
rarely used for computing a solution, since Gaussian_elimination is a faster
algorithm.
The determinant of an endomorphism is the determinant of the matrix
representing the endomorphism in terms of some ordered basis. This definition
makes sense, since this determinant is independent of the choice of the basis.
**** Eigenvalues and eigenvectors[edit] ****
Main article: Eigenvalues_and_eigenvectors
If f is a linear endomorphism of a vector space V over a field F, an
eigenvector of f is a nonzero vector v of V such that f(v) = av for some scalar
a in F. This scalar a is an eigenvalue of f.
If the dimension of V is finite, and a basis has been chosen, f and v may be
represented, respectively, by a square matrix M and a column matrix z; the
equation defining eigenvectors and eigenvalues becomes
         M z = a z .   {\displaystyle Mz=az.}  [{\displaystyle Mz=az.}]
Using the identity_matrix I, whose entries are all zero, except those of the
main diagonal, which are equal to one, this may be rewritten
         ( M &#x2212; a I ) z = 0.   {\displaystyle (M-aI)z=0.}  [
      {\displaystyle (M-aI)z=0.}]
As z is supposed to be nonzero, this means that M â aI is a singular_matrix,
and thus that its determinant     det ( M &#x2212; a I )   {\displaystyle \det
(M-aI)}  [{\displaystyle \det(M-aI)}] equals zero. The eigenvalues are thus the
roots of the polynomial
         det ( x I &#x2212; M ) .   {\displaystyle \det(xI-M).}  [
      {\displaystyle \det(xI-M).}]
If V is of dimension n, this is a monic_polynomial of degree n, called the
characteristic_polynomial of the matrix (or of the endomorphism), and there
are, at most, n eigenvalues.
If a basis exists that consists only of eigenvectors, the matrix of f on this
basis has a very simple structure: it is a diagonal_matrix such that the
entries on the main_diagonal are eigenvalues, and the other entries are zero.
In this case, the endomorphism and the matrix are said diagonalizable. More
generally, an endomorphism and a matrix are also said diagonalizable, if they
become diagonalizable after extending the field of scalars. In this extended
sense, if the characteristic polynomial is square-free, then the matrix is
diagonalizable.
A symmetric_matrix is always diagonalizable. There are non-diagonalizable
matrices, the simplest being
           [    0   1     0   0    ]     {\displaystyle {\begin
      {bmatrix}0&1\\0&0\end{bmatrix}}}  [{\begin{bmatrix}0&1\\0&0\end
      {bmatrix}}]
(it cannot be diagonalizable since its square is the zero_matrix, and the
square of a nonzero diagonal matrix is never zero).
When an endomorphism is not diagonalizable, there are bases on which it has a
simple form, although not as simple as the diagonal form. The Frobenius_normal
form does not need of extending the field of scalars and makes the
characteristic polynomial immediately readable on the matrix. The Jordan_normal
form requires to extend the field of scalar for containing all eigenvalues, and
differs from the diagonal form only by some entries that are just above the
main diagonal and are equal to 1.
***** Duality[edit] *****
Main article: Dual_space
A linear_form is a linear map from a vector space V over a field F to the field
of scalars F, viewed as a vector space over itself. Equipped by pointwise
addition and multiplication by a scalar, the linear forms form a vector space,
called the dual space of V, and usually denoted      V  &#x2217;   .
{\displaystyle V^{*}.}  [{\displaystyle V^{*}.}]
If      v  1   , &#x2026; ,  v  n     {\displaystyle v_{1},\ldots ,v_{n}}  [
{\displaystyle v_{1},\ldots ,v_{n}}] is a basis of V (this implies that V is
finite-dimensional), then one can define, for i = 1, ..., n, a linear map
v  i   &#x2217;     {\displaystyle v_{i}^{*}}  [{\displaystyle v_{i}^{*}}] such
that      v  i   &#x2217;   (  e  i   ) = 1   {\displaystyle v_{i}^{*}(e_
{i})=1}  [{\displaystyle v_{i}^{*}(e_{i})=1}] and      v  i   &#x2217;   (  e
j   ) = 0   {\displaystyle v_{i}^{*}(e_{j})=0}  [{\displaystyle v_{i}^{*}(e_
{j})=0}] if j â  i. These linear maps form a basis of      V  &#x2217;   ,
{\displaystyle V^{*},}  [V^{*},] called the dual_basis of      v  1   ,
&#x2026; ,  v  n   .   {\displaystyle v_{1},\ldots ,v_{n}.}  [{\displaystyle v_
{1},\ldots ,v_{n}.}] (If V is not finite-dimensional, the      v  i   &#x2217;
{\displaystyle v_{i}^{*}}  [v_{i}^{*}] may be defined similarly; they are
linearly independent, but do not form a basis.)
For v in V, the map
         f &#x2192; f ( v )   {\displaystyle f\to f(v)}  [{\displaystyle f\to f
      (v)}]
is a linear form on      V  &#x2217;   .   {\displaystyle V^{*}.}  [
{\displaystyle V^{*}.}] This defines the canonical_linear_map from V into
V  &#x2217; &#x2217;   ,   {\displaystyle V^{**},}  [{\displaystyle V^{**},}]
the dual of      V  &#x2217;   ,   {\displaystyle V^{*},}  [V^{*},] called the
bidual of V. This canonical map is an isomorphism if V is finite-dimensional,
and this allows identifying V with its bidual. (In the infinite dimensional
case, the canonical map is injective, but not surjective.)
There is thus a complete symmetry between a finite-dimensional vector space and
its dual. This motivates the frequent use, in this context, of the braâket
notation
         &#x27E8; f , x &#x27E9;   {\displaystyle \langle f,x\rangle }  [
      {\displaystyle \langle f,x\rangle }]
for denoting f (x).
**** Dual map[edit] ****
Main article: Transpose_of_a_linear_map
Let
         f : V &#x2192; W   {\displaystyle f:V\to W}  [f:V\to W]
be a linear map. For every linear form h on W, the composite_function h â f
is a linear form on V. This defines a linear map
          f  &#x2217;   :  W  &#x2217;   &#x2192;  V  &#x2217;
      {\displaystyle f^{*}:W^{*}\to V^{*}}  [{\displaystyle f^{*}:W^{*}\to V^
      {*}}]
between the dual spaces, which is called the dual or the transpose of f.
If V and W are finite dimensional, and M is the matrix of f in terms of some
ordered bases, then the matrix of      f  &#x2217;     {\displaystyle f^{*}}
[f^{*}] over the dual bases is the transpose      M   T      {\displaystyle M^
{\mathsf {T}}}  [{\displaystyle M^{\mathsf {T}}}] of M, obtained by exchanging
rows and columns.
If elements of vector spaces and their duals are represented by column vectors,
this duality may be expressed in braâket_notation by
         &#x27E8;  h   T    , M v &#x27E9; = &#x27E8;  h   T    M , v &#x27E9;
      .   {\displaystyle \langle h^{\mathsf {T}},Mv\rangle =\langle h^{\mathsf
      {T}}M,v\rangle .}  [{\displaystyle \langle h^{\mathsf {T}},Mv\rangle
      =\langle h^{\mathsf {T}}M,v\rangle .}]
For highlighting this symmetry, the two members of this equality are sometimes
written
         &#x27E8;  h   T    &#x2223; M &#x2223; v &#x27E9; .   {\displaystyle
      \langle h^{\mathsf {T}}\mid M\mid v\rangle .}  [{\displaystyle \langle h^
      {\mathsf {T}}\mid M\mid v\rangle .}]
**** Inner-product spaces[edit] ****
 This section may require cleanup to meet Wikipedia's quality_standards. The
 specific problem is: Need for a more encyclopedic style, which is homogeneous
 with the style of preceding sections. Also, some details do not belong to this
 general article but to more specialized ones. Also, inner product spaces
 should appear as a special instance of the more general concept of bilinear
 form. Finally, complex conjugation should appear in a specific section on
 linear algebra over the complexes. Please help improve_this_section if you
 can. (August 2018)(Learn_how_and_when_to_remove_this_template_message)
Main article: Inner_product_space
Besides these basic concepts, linear algebra also studies vector spaces with
additional structure, such as an inner_product. The inner product is an example
of a bilinear_form, and it gives the vector space a geometric structure by
allowing for the definition of length and angles. Formally, an inner product is
a map
         &#x27E8; &#x22C5; , &#x22C5; &#x27E9; : V &#x00D7; V &#x2192; F
      {\displaystyle \langle \cdot ,\cdot \rangle :V\times V\rightarrow F}
      [\langle \cdot ,\cdot \rangle :V\times V\rightarrow F]
that satisfies the following three axioms for all vectors u, v, w in V and all
scalars a in F:[10][11]
    * Conjugate symmetry:
               &#x27E8; u , v &#x27E9; =    &#x27E8; v , u &#x27E9;  &#x00AF;
            .   {\displaystyle \langle u,v\rangle ={\overline {\langle
            v,u\rangle }}.}  [\langle u,v\rangle ={\overline {\langle
            v,u\rangle }}.]
Note that in R, it is symmetric.
    * Linearity in the first argument:
               &#x27E8; a u , v &#x27E9; = a &#x27E8; u , v &#x27E9; .
            {\displaystyle \langle au,v\rangle =a\langle u,v\rangle .}
            [\langle au,v\rangle =a\langle u,v\rangle .]
               &#x27E8; u + v , w &#x27E9; = &#x27E8; u , w &#x27E9; + &#x27E8;
            v , w &#x27E9; .   {\displaystyle \langle u+v,w\rangle =\langle
            u,w\rangle +\langle v,w\rangle .}  [\langle u+v,w\rangle =\langle
            u,w\rangle +\langle v,w\rangle .]
    * Positive-definiteness:
               &#x27E8; v , v &#x27E9; &#x2265; 0   {\displaystyle \langle
            v,v\rangle \geq 0}  [\langle v,v\rangle \geq 0] with equality only
            for v = 0.
We can define the length of a vector v in V by
         &#x2016; v  &#x2016;  2   = &#x27E8; v , v &#x27E9; ,   {\displaystyle
      \|v\|^{2}=\langle v,v\rangle ,}  [\|v\|^{2}=\langle v,v\rangle ,]
and we can prove the CauchyâSchwarz_inequality:
          |  &#x27E8; u , v &#x27E9;  |  &#x2264; &#x2016; u &#x2016; &#x22C5;
      &#x2016; v &#x2016; .   {\displaystyle |\langle u,v\rangle |\leq
      \|u\|\cdot \|v\|.}  [|\langle u,v\rangle |\leq \|u\|\cdot \|v\|.]
In particular, the quantity
             |  &#x27E8; u , v &#x27E9;  |    &#x2016; u &#x2016; &#x22C5;
      &#x2016; v &#x2016;    &#x2264; 1 ,   {\displaystyle {\frac {|\langle
      u,v\rangle |}{\|u\|\cdot \|v\|}}\leq 1,}  [{\frac {|\langle u,v\rangle |}
      {\|u\|\cdot \|v\|}}\leq 1,]
and so we can call this quantity the cosine of the angle between the two
vectors.
Two vectors are orthogonal if     &#x27E8; u , v &#x27E9; = 0   {\displaystyle
\langle u,v\rangle =0}  [\langle u,v\rangle =0]. An orthonormal basis is a
basis where all basis vectors have length 1 and are orthogonal to each other.
Given any finite-dimensional vector space, an orthonormal basis could be found
by the GramâSchmidt procedure. Orthonormal bases are particularly easy to
deal with, since if v = a1 v1 + ... + an vn, then      a  i   = &#x27E8; v ,  v
i   &#x27E9;   {\displaystyle a_{i}=\langle v,v_{i}\rangle }  [a_{i}=\langle
v,v_{i}\rangle ].
The inner product facilitates the construction of many useful concepts. For
instance, given a transform T, we can define its Hermitian_conjugate T* as the
linear transform satisfying
         &#x27E8; T u , v &#x27E9; = &#x27E8; u ,  T  &#x2217;   v &#x27E9; .
      {\displaystyle \langle Tu,v\rangle =\langle u,T^{*}v\rangle .}  [\langle
      Tu,v\rangle =\langle u,T^{*}v\rangle .]
If T satisfies TT* = T*T, we call T normal. It turns out that normal matrices
are precisely the matrices that have an orthonormal system of eigenvectors that
span V.
***** Relationship with geometry[edit] *****
There is a strong relationship between linear algebra and geometry, which
started with the introduction by RenÃ©_Descartes, in 1637, of Cartesian
coordinates. In this new (at that time) geometry, now called Cartesian
geometry, points are represented by Cartesian_coordinates, which are sequences
of three real numbers (in the case of the usual three-dimensional_space). The
basic objects of geometry, which are lines and planes are represented by linear
equations. Thus, computing intersections of lines and planes amounts to solving
systems of linear equations. This was one of the main motivations for
developing linear algebra.
Most geometric_transformation, such as translations, rotations, reflections,
rigid_motions, isometries, and projections transform lines into lines. It
follows that they can be defined, specified and studied in terms of linear
maps. This is also the case of homographies and MÃ¶bius_transformations, when
considered as transformations of a projective_space.
Until the end of 19th century, geometric spaces were defined by axioms relating
points, lines and planes (synthetic_geometry). Around this date, it appeared
that one may also define geometric spaces by constructions involving vector
spaces (see, for example, Projective_space and Affine_space) It has been shown
that the two approaches are essentially equivalent.[12] In classical geometry,
the involved vector spaces are vector spaces over the reals, but the
constructions may be extended to vector spaces over any field, allowing
considering geometry over arbitrary fields, including finite_fields.
Presently, most textbooks, introduce geometric spaces from linear algebra, and
geometry is often presented, at elementary level, as a subfield of linear
algebra.
***** Usage and applications[edit] *****
Linear algebra is used in almost all areas of mathematics, thus making it
relevant in almost all scientific domains that use mathematics. These
applications may be divided into several wide categories.
**** Geometry of our ambient space[edit] ****
The modeling of our ambient_space is based on geometry. Sciences concerned with
this space use geometry widely. This is the case with mechanics and robotics,
for describing rigid_body_dynamics; geodesy for describing Earth_shape;
perspectivity, computer_vision, and computer_graphics, for describing the
relationship between a scene and its plane representation; and many other
scientific domains.
In all these applications, synthetic_geometry is often used for general
descriptions and a qualitative approach, but for the study of explicit
situations, one must compute with coordinates. This requires the heavy use of
linear algebra.
**** Functional analysis[edit] ****
Functional_analysis studies function_spaces. These are vector spaces with
additional structure, such as Hilbert_spaces. Linear algebra is thus a
fundamental part of functional analysis and its applications, which include, in
particular, quantum_mechanics (wave_functions).
**** Study of complex_systems[edit] ****
Most physical phenomena are modeled by partial_differential_equations. To solve
them, one usually decomposes the space in which the solutions are searched into
small, mutually interacting cells. For linear_systems this interaction involves
linear_functions. For nonlinear_systems, this interaction is often approximated
by linear functions.[13] In both cases, very large matrices are generally
involved. Weather_forecasting is a typical example, where the whole Earth
atmosphere is divided in cells of, say, 100 km of width and 100 m of height.
**** Scientific computation[edit] ****
Nearly all scientific_computations involve linear algebra. Consequently, linear
algebra algorithms have been highly optimized. BLAS and LAPACK are the best
known implementations. For improving efficiency, some of them configure the
algorithms automatically, at run time, for adapting them to the specificities
of the computer (cache size, number of available cores, ...).
Some processors, typically graphics_processing_units (GPU), are designed with a
matrix structure, for optimizing the operations of linear algebra.
***** Extensions and generalizations[edit] *****
This section presents several related topics that do not appear generally in
elementary textbooks on linear algebra, but are commonly considered, in
advanced mathematics, as parts of linear algebra.
**** Module theory[edit] ****
Main article: Module_(mathematics)
The existence of multiplicative inverses in fields is not involved in the
axioms defining a vector space. One may thus replace the field of scalars by a
ring R, and this gives a structure called module over R, or R-module.
The concepts of linear independence, span, basis, and linear maps (also called
module_homomorphisms) are defined for modules exactly as for vector spaces,
with the essential difference that, if R is not a field, there are modules that
do not have any basis. The modules that have a basis are the free_modules, and
those that are spanned by a finite set are the finitely_generated_modules.
Module homomorphisms between finitely generated free modules may be represented
by matrices. The theory of matrices over a ring is similar to that of matrices
over a field, except that determinants exist only if the ring is commutative,
and that a square matrix over a commutative ring is invertible only if its
determinant has a multiplicative_inverse in the ring.
Vector spaces are completely characterized by their dimension (up to an
isomorphism). In general, there is not such a complete classification for
modules, even if one restricts oneself to finitely generated modules. However,
every module is a cokernel of a homomorphism of free modules.
Modules over the integers can be identified with abelian_groups, since the
multiplication by an integer may identified to a repeated addition. Most of the
theory of abelian groups may be extended to modules over a principal_ideal
domain. In particular, over a principal ideal domain, every submodule of a free
module is free, and the fundamental_theorem_of_finitely_generated_abelian
groups may be extended straightforwardly to finitely generated modules over a
principal ring.
There are many rings for which there are algorithms for solving linear
equations and systems of linear equations. However, these algorithms have
generally a computational_complexity that is much higher than the similar
algorithms over a field. For more details, see Linear_equation_over_a_ring.
**** Multilinear algebra and tensors[edit] ****
 This section may require cleanup to meet Wikipedia's quality_standards. The
 specific problem is: The dual space is considered above, and the section must
 be rewritten for given a understandable summary of this subject Please help
 improve_this_section if you can. (September 2018)(Learn_how_and_when_to_remove
 this_template_message)
In multilinear_algebra, one considers multivariable linear transformations,
that is, mappings that are linear in each of a number of different variables.
This line of inquiry naturally leads to the idea of the dual_space, the vector
space Vâ consisting of linear maps f: V â F where F is the field of
scalars. Multilinear maps T: Vn â F can be described via tensor_products of
elements of Vâ.
If, in addition to vector addition and scalar multiplication, there is a
bilinear vector product V Ã V â V, the vector space is called an algebra;
for instance, associative algebras are algebras with an associate vector
product (like the algebra of square matrices, or the algebra of polynomials).
**** Topological vector spaces[edit] ****
[[icon]] This section needs expansion. You can help by adding_to_it. (September
         2018)
Main articles: Topological_vector_space, Normed_vector_space, and Hilbert_space
Vector spaces that are not finite dimensional often require additional
structure to be tractable. A normed_vector_space is a vector space along with a
function called a norm, which measures the "size" of elements. The norm induces
a metric, which measures the distance between elements, and induces a topology,
which allows for a definition of continuous maps. The metric also allows for a
definition of limits and completeness - a metric space that is complete is
known as a Banach_space. A complete metric space along with the additional
structure of an inner_product (a conjugate symmetric sesquilinear_form) is
known as a Hilbert_space, which is in some sense a particularly well-behaved
Banach space. Functional_analysis applies the methods of linear algebra
alongside those of mathematical_analysis to study various function spaces; the
central objects of study in functional analysis are Lp_spaces, which are Banach
spaces, and especially the L2 space of square integrable functions, which is
the only Hilbert space among them. Functional analysis is of particular
importance to quantum mechanics, the theory of partial differential equations,
digital signal processing, and electrical engineering. It also provides the
foundation and theoretical framework that underlies the Fourier transform and
related methods.
**** Homological algebra[edit] ****
[[icon]] This section needs expansion. You can help by adding_to_it. (September
         2018)
Main article: Homological_algebra
***** See also[edit] *****
    * Linear_equation_over_a_ring
    * Fundamental_matrix in computer_vision
    * Linear_regression, a statistical estimation method
    * List_of_linear_algebra_topics
    * Numerical_linear_algebra
    * Linear_programming
    * Transformation_matrix
***** Notes[edit] *****
   1. ^Banerjee, Sudipto; Roy, Anindya (2014), Linear Algebra and Matrix
      Analysis for Statistics, Texts in Statistical Science (1st ed.), Chapman
      and Hall/CRC, ISBN 978-1420095388
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
   3. ^Strang, Gilbert (July 19, 2005), Linear Algebra and Its Applications
      (4th ed.), Brooks Cole, ISBN 978-0-03-010567-8
   4. ^Weisstein, Eric. "Linear_Algebra". From MathWorld--A Wolfram Web
      Resource. Wolfram. Retrieved 16 April 2012.
   5. ^Hart, Roger (2010). The_Chinese_Roots_of_Linear_Algebra. JHU_Press.
      ISBN 9780801899584.
   6. ^ a b c dVitulli,_Marie. "A_Brief_History_of_Linear_Algebra_and_Matrix
      Theory". Department of Mathematics. University of Oregon. Archived from
      the_original on 2012-09-10. Retrieved 2014-07-08.
   7. ^ Benjamin_Peirce (1872) Linear Associative Algebra, lithograph, new
      edition with corrections, notes, and an added 1875 paper by Peirce, plus
      notes by his son Charles_Sanders_Peirce, published in the American
      Journal of Mathematics v. 4, 1881, Johns Hopkins University,
      pp. 221â226, Google Eprint and as an extract, D. Van Nostrand, 1882,
      Google Eprint.
   8. ^ Roman 2005, ch. 1, p. 27
   9. ^ Axler (2004), p. 55
  10. ^ Axler (2204), p. 33
  11. ^P. K. Jain, Khalil Ahmad (1995). "5.1_Definitions_and_basic_properties
      of_inner_product_spaces_and_Hilbert_spaces". Functional analysis (2nd
      ed.). New Age International. p. 203. ISBN 81-224-0801-X.
  12. ^Eduard PrugovecÌki (1981). "Definition_2.1". Quantum mechanics in
      Hilbert space (2nd ed.). Academic Press. pp. 18 ff. ISBN 0-12-566060-X.
  13. ^ Emil_Artin (1957) Geometric_Algebra Interscience_Publishers
  14. ^ This may have the consequence that some physically interesting
      solutions are omitted.
   1. ^ This axiom is not asserting the associativity of an operation, since
      there are two operations in question, scalar multiplication: bv; and
      field multiplication: ab.
***** Further reading[edit] *****
**** History[edit] ****
    * Fearnley-Sander, Desmond, "Hermann_Grassmann_and_the_Creation_of_Linear
      Algebra", American Mathematical Monthly 86 (1979), pp. 809â817.
    * Grassmann,_Hermann (1844), Die lineale Ausdehnungslehre ein neuer Zweig
      der Mathematik: dargestellt und durch Anwendungen auf die Ã¼brigen Zweige
      der Mathematik, wie auch auf die Statik, Mechanik, die Lehre vom
      Magnetismus und die Krystallonomie erlÃ¤utert, Leipzig: O. Wigand
**** Introductory textbooks[edit] ****
    * Anton, Howard (2005), Elementary Linear Algebra (Applications Version)
      (9th ed.), Wiley International
Banerjee, Sudipto; Roy, Anindya (2014), Linear Algebra and Matrix Analysis for
Statistics, Texts in Statistical Science (1st ed.), Chapman and Hall/CRC,
ISBN 978-1420095388
Bretscher, Otto (2004), Linear Algebra with Applications (3rd ed.), Prentice
Hall, ISBN 978-0-13-145334-0
Farin, Gerald; Hansford, Dianne (2004), Practical Linear Algebra: A Geometry
Toolbox, AK Peters, ISBN 978-1-56881-234-2
Hefferon, Jim (2008), Linear_Algebra
Kolman, Bernard; Hill, David R. (2007), Elementary Linear Algebra with
Applications (9th ed.), Prentice Hall, ISBN 978-0-13-229654-0
Lay, David C. (2005), Linear Algebra and Its Applications (3rd ed.), Addison
Wesley, ISBN 978-0-321-28713-7
Leon, Steven J. (2006), Linear Algebra With Applications (7th ed.), Pearson
Prentice Hall, ISBN 978-0-13-185785-8
Murty, Katta G. (2014) Computational_and_Algorithmic_Linear_Algebra_and_n-
Dimensional_Geometry, World Scientific Publishing,
ISBN 978-981-4366-62-5. Chapter_1:_Systems_of_Simultaneous_Linear_Equations
Poole, David (2010), Linear Algebra: A Modern Introduction (3rd ed.),
Cengage â Brooks/Cole, ISBN 978-0-538-73545-2
Ricardo, Henry (2010), A Modern Introduction To Linear Algebra (1st ed.), CRC
Press, ISBN 978-1-4398-0040-9
Sadun, Lorenzo (2008), Applied Linear Algebra: the decoupling principle (2nd
ed.), AMS, ISBN 978-0-8218-4441-0
Strang,_Gilbert (2016), Introduction to Linear Algebra (5th ed.), Wellesley-
Cambridge Press, ISBN 978-09802327-7-6
The Manga Guide to Linear Algebra (2012), by Shin_Takahashi, Iroha Inoue and
Trend-Pro Co., Ltd.,
ISBN 978-1-59327-413-9
**** Advanced textbooks[edit] ****
    * Axler,_Sheldon (February 26, 2004), Linear Algebra Done Right (2nd ed.),
      Springer, ISBN 978-0-387-98258-8
Bhatia, Rajendra (November 15, 1996), Matrix Analysis, Graduate_Texts_in
Mathematics, Springer, ISBN 978-0-387-94846-1
Demmel,_James_W. (August 1, 1997), Applied Numerical Linear Algebra, SIAM,
ISBN 978-0-89871-389-3
Dym, Harry (2007), Linear Algebra in Action, AMS, ISBN 978-0-8218-3813-6
Gantmacher,_Felix_R. (2005), Applications of the Theory of Matrices, Dover
Publications, ISBN 978-0-486-44554-0
Gantmacher, Felix R. (1990), Matrix Theory Vol. 1 (2nd ed.), American
Mathematical Society, ISBN 978-0-8218-1376-8
Gantmacher, Felix R. (2000), Matrix Theory Vol. 2 (2nd ed.), American
Mathematical Society, ISBN 978-0-8218-2664-5
Gelfand,_Israel_M. (1989), Lectures on Linear Algebra, Dover Publications,
ISBN 978-0-486-66082-0
Glazman, I. M.; Ljubic, Ju. I. (2006), Finite-Dimensional Linear Analysis,
Dover Publications, ISBN 978-0-486-45332-3
Golan, Johnathan S. (January 2007), The Linear Algebra a Beginning Graduate
Student Ought to Know (2nd ed.), Springer, ISBN 978-1-4020-5494-5
Golan, Johnathan S. (August 1995), Foundations of Linear Algebra, Kluwer,
ISBN 0-7923-3614-3
Golub, Gene H.; Van Loan, Charles F. (October 15, 1996), Matrix Computations,
Johns Hopkins Studies in Mathematical Sciences (3rd ed.), The Johns Hopkins
University Press, ISBN 978-0-8018-5414-9
Greub, Werner H. (October 16, 1981), Linear Algebra, Graduate Texts in
Mathematics (4th ed.), Springer, ISBN 978-0-8018-5414-9
Hoffman, Kenneth; Kunze,_Ray (1971), Linear algebra (2nd ed.), Englewood
Cliffs, N.J.: Prentice-Hall, Inc., MR 0276251
Halmos,_Paul_R. (August 20, 1993), Finite-Dimensional Vector Spaces,
Undergraduate_Texts_in_Mathematics, Springer, ISBN 978-0-387-90093-3
Friedberg, Stephen H.; Insel, Arnold J.; Spence, Lawrence E. (September 7,
2018), Linear Algebra (5th ed.), Pearson, ISBN 978-0-13-486024-4
Horn, Roger A.; Johnson, Charles R. (February 23, 1990), Matrix Analysis,
Cambridge University Press, ISBN 978-0-521-38632-6
Horn, Roger A.; Johnson, Charles R. (June 24, 1994), Topics in Matrix Analysis,
Cambridge University Press, ISBN 978-0-521-46713-1
Lang, Serge (March 9, 2004), Linear Algebra, Undergraduate Texts in Mathematics
(3rd ed.), Springer, ISBN 978-0-387-96412-6
Marcus, Marvin; Minc, Henryk (2010), A Survey of Matrix Theory and Matrix
Inequalities, Dover Publications, ISBN 978-0-486-67102-4
Meyer, Carl D. (February 15, 2001), Matrix_Analysis_and_Applied_Linear_Algebra,
Society for Industrial and Applied Mathematics (SIAM), ISBN 978-0-89871-454-8,
archived from the_original on October 31, 2009
Mirsky,_L. (1990), An Introduction to Linear Algebra, Dover Publications,
ISBN 978-0-486-66434-7
Roman, Steven (March 22, 2005), Advanced Linear Algebra, Graduate Texts in
Mathematics (2nd ed.), Springer, ISBN 978-0-387-24766-3
Shafarevich,_I._R.; Remizov, A. O (2012), Linear_Algebra_and_Geometry,
Springer, ISBN 978-3-642-30993-9
Shilov,_Georgi_E. (June 1, 1977), Linear algebra, Dover Publications, ISBN 978-
0-486-63518-7
Shores, Thomas S. (December 6, 2006), Applied Linear Algebra and Matrix
Analysis, Undergraduate Texts in Mathematics, Springer, ISBN 978-0-387-33194-2
Smith, Larry (May 28, 1998), Linear Algebra, Undergraduate Texts in
Mathematics, Springer, ISBN 978-0-387-98455-1
Trefethen, Lloyd N.; Bau, David (1997), Numerical Linear Algebra, SIAM,
ISBN 978-0-898-71361-9
**** Study guides and outlines[edit] ****
    * Leduc, Steven A. (May 1, 1996), Linear Algebra (Cliffs Quick Review),
      Cliffs Notes, ISBN 978-0-8220-5331-6
Lipschutz, Seymour; Lipson, Marc (December 6, 2000), Schaum's Outline of Linear
Algebra (3rd ed.), McGraw-Hill, ISBN 978-0-07-136200-9
Lipschutz, Seymour (January 1, 1989), 3,000 Solved Problems in Linear Algebra,
McGrawâHill, ISBN 978-0-07-038023-3
McMahon, David (October 28, 2005), Linear Algebra Demystified, McGrawâHill
Professional, ISBN 978-0-07-146579-3
Zhang, Fuzhen (April 7, 2009), Linear Algebra: Challenging Problems for
Students, The Johns Hopkins University Press, ISBN 978-0-8018-9125-0
***** External links[edit] *****
 Wikibooks has a book on the topic of: Linear_Algebra
**** Online Resources[edit] ****
 Wikimedia Commons has media related to Linear_algebra.
    * MIT_Linear_Algebra_Video_Lectures, a series of 34 recorded lectures by
      professor Gilbert Strang (Spring 2010)
    * International_Linear_Algebra_Society
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Linear_algebra", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Linear_Algebra on MathWorld.
Matrix_and_Linear_Algebra_Terms on Earliest_Known_Uses_of_Some_of_the_Words_of
Mathematics
Earliest_Uses_of_Symbols_for_Matrices_and_Vectors on Earliest_Uses_of_Various
Mathematical_Symbols
Essence_of_linear_algebra, a video presentation of the basics of linear
algebra, with emphasis on the relationship between the geometric, the matrix
and the abstract points of view
**** Online books[edit] ****
    * Beezer, Rob, A_First_Course_in_Linear_Algebra
    * Connell, Edwin H., Elements_of_Abstract_and_Linear_Algebra
    * Hefferon, Jim, Linear_Algebra
    * Matthews, Keith, Elementary_Linear_Algebra
    * Sharipov, Ruslan, Course_of_linear_algebra_and_multidimensional_geometry
    * Treil, Sergei, Linear_Algebra_Done_Wrong
    * v
    * t
    * e
Linear algebra
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
                                              * BNF: cb11937509n (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4035811-2
                                              * LCCN: sh85003441
                                              * NDL: 00570681

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Linear_algebra&oldid=909708901"
Categories:
    * Linear_algebra
    * Numerical_analysis
Hidden categories:
    * Articles_needing_cleanup_from_August_2018
    * All_pages_needing_cleanup
    * Cleanup_tagged_articles_with_a_reason_field_from_August_2018
    * Wikipedia_pages_needing_cleanup_from_August_2018
    * Articles_needing_cleanup_from_September_2018
    * Cleanup_tagged_articles_with_a_reason_field_from_September_2018
    * Wikipedia_pages_needing_cleanup_from_September_2018
    * Articles_to_be_expanded_from_September_2018
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
    * Commons_category_link_from_Wikidata
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
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
    * Wikiversity
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Alemannisch
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AragonÃ©s
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐ°ÑÒ¡Ð¾ÑÑÑÐ°
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * Ð§ÓÐ²Ð°ÑÐ»Ð°
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * è´èª
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Interlingua
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Kiswahili
    * Latina
    * LatvieÅ¡u
    * ÐÐµÐ·Ð³Ð¸
    * LietuviÅ³
    * Lingua_Franca_Nova
    * Lumbaart
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Nordfriisk
    * Norsk
    * Norsk_nynorsk
    * Occitan
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Patois
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Sicilianu
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * Winaray
    * å´è¯­
    * ××Ö´×××©
    * YorÃ¹bÃ¡
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 02:56 (UTC).
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
