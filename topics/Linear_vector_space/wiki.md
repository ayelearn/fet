The following text has been accessed from https://en.wikipedia.org/wiki/Vector_space at Fri Aug 9 03:10:56 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















[This_is_a_good_article._Follow_the_link_for_more_information.]
****** Vector space ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Algebraic structure which is fundamental for linear algebra
Not to be confused with Vector_field.
This article is about linear (vector) spaces. For the structure in incidence
geometry, see Linear_space_(geometry). For the space technology company, see
Vector_Space_Systems.
Vector addition and scalar multiplication: a vector v (blue) is added to
another vector w (red, upper illustration). Below, w is stretched by a factor
of 2, yielding the sum v + 2w.
A vector space (also called a linear space) is a collection of objects called
vectors, which may be added together and multiplied ("scaled") by numbers,
called scalars. Scalars are often taken to be real_numbers, but there are also
vector spaces with scalar multiplication by complex_numbers, rational_numbers,
or generally any field. The operations of vector addition and scalar
multiplication must satisfy certain requirements, called axioms, listed below.
[clarification_needed]
Euclidean_vectors are an example of a vector space. They represent physical
quantities such as forces: any two forces (of the same type) can be added to
yield a third, and the multiplication of a force_vector by a real multiplier is
another force vector. In the same vein, but in a more geometric sense, vectors
representing displacements in the plane or in three-dimensional_space also form
vector spaces. Vectors in vector spaces do not necessarily have to be arrow-
like objects as they appear in the mentioned examples: vectors are regarded as
abstract mathematical objects with particular properties, which in some cases
can be visualized as arrows.
Vector spaces are the subject of linear_algebra and are well characterized by
their dimension, which, roughly speaking, specifies the number of independent
directions in the space. Infinite-dimensional vector spaces arise naturally in
mathematical_analysis, as function_spaces, whose vectors are functions. These
vector spaces are generally endowed with additional structure, which may be a
topology, allowing the consideration of issues of proximity and continuity.
Among these topologies, those that are defined by a norm or inner_product are
more commonly used, as having a notion of distance between two vectors. This is
particularly the case of Banach_spaces and Hilbert_spaces, which are
fundamental in mathematical analysis.
Historically, the first ideas leading to vector spaces can be traced back as
far as the 17th century's analytic_geometry, matrices, systems of linear
equations, and Euclidean vectors. The modern, more abstract treatment, first
formulated by Giuseppe_Peano in 1888, encompasses more general objects than
Euclidean_space, but much of the theory can be seen as an extension of
classical geometric ideas like lines, planes and their higher-dimensional
analogs.
Today, vector spaces are applied throughout mathematics, science and
engineering. They are the appropriate linear-algebraic notion to deal with
systems_of_linear_equations. They offer a framework for Fourier_expansion,
which is employed in image_compression routines, and they provide an
environment that can be used for solution techniques for partial_differential
equations. Furthermore, vector spaces furnish an abstract, coordinate-free way
of dealing with geometrical and physical objects such as tensors. This in turn
allows the examination of local properties of manifolds by linearization
techniques. Vector spaces may be generalized in several ways, leading to more
advanced notions in geometry and abstract_algebra.
Algebraic_structures
Group-like
    * Group
    * Semigroup / Monoid
    * Rack_and_quandle
    * Quasigroup_and_loop
    * Abelian_group
    * Magma
    * Lie_group
Group_theory
Ring-like
    * Ring
    * Semiring
    * Near-ring
    * Commutative_ring
    * Integral_domain
    * Field
    * Division_ring
Ring_theory
Lattice-like
    * Lattice
    * Semilattice
    * Complemented_lattice
    * Total_order
    * Heyting_algebra
    * Boolean_algebra
    * Map_of_lattices
    * Lattice_theory
Module-like
    * Module
    * Group_with_operators
    * Vector space
    * Linear_algebra
Algebra-like
    * Algebra
    * Associative
    * Non-associative
    * Composition_algebra
    * Lie_algebra
    * Graded
    * Bialgebra
    * v
    * t
    * e
⁰
***** Contents *****
    * 1_Introduction_and_definition
          o 1.1_First_example:_arrows_in_the_plane
          o 1.2_Second_example:_ordered_pairs_of_numbers
          o 1.3_Definition
          o 1.4_Alternative_formulations_and_elementary_consequences
    * 2_History
    * 3_Examples
          o 3.1_Coordinate_spaces
          o 3.2_Complex_numbers_and_other_field_extensions
          o 3.3_Function_spaces
          o 3.4_Linear_equations
    * 4_Basis_and_dimension
    * 5_Linear_maps_and_matrices
          o 5.1_Matrices
          o 5.2_Eigenvalues_and_eigenvectors
    * 6_Basic_constructions
          o 6.1_Subspaces_and_quotient_spaces
          o 6.2_Direct_product_and_direct_sum
          o 6.3_Tensor_product
    * 7_Vector_spaces_with_additional_structure
          o 7.1_Normed_vector_spaces_and_inner_product_spaces
          o 7.2_Topological_vector_spaces
                # 7.2.1_Banach_spaces
                # 7.2.2_Hilbert_spaces
          o 7.3_Algebras_over_fields
    * 8_Applications
          o 8.1_Distributions
          o 8.2_Fourier_analysis
          o 8.3_Differential_geometry
    * 9_Generalizations
          o 9.1_Vector_bundles
          o 9.2_Modules
          o 9.3_Affine_and_projective_spaces
    * 10_See_also
    * 11_Notes
    * 12_Citations
    * 13_References
          o 13.1_Algebra
          o 13.2_Analysis
          o 13.3_Historical_references
          o 13.4_Further_references
    * 14_External_links
***** Introduction and definition[edit] *****
The concept of vector space will first be explained by describing two
particular examples:
**** First example: arrows in the plane[edit] ****
The first example of a vector space consists of arrows in a fixed plane,
starting at one fixed point. This is used in physics to describe forces or
velocities. Given any two such arrows, v and w, the parallelogram spanned by
these two arrows contains one diagonal arrow that starts at the origin, too.
This new arrow is called the sum of the two arrows and is denoted v + w. In the
special case of two arrows on the same line, their sum is the arrow on this
line whose length is the sum or the difference of the lengths, depending on
whether the arrows have the same direction. Another operation that can be done
with arrows is scaling: given any positive real_number a, the arrow that has
the same direction as v, but is dilated or shrunk by multiplying its length by
a, is called multiplication of v by a. It is denoted av. When a is negative, av
is defined as the arrow pointing in the opposite direction, instead.
The following shows a few examples: if a = 2, the resulting vector aw has the
same direction as w, but is stretched to the double length of w (right image
below). Equivalently, 2w is the sum w + w. Moreover, (â1)v = âv has the
opposite direction and the same length as v (blue vector pointing down in the
right image).
[Vector_addition:_the
sum_v_+_w_(black)_of   [Scalar_multiplication:_the_multiples_âv_and_2w_are
the_vectors_v_(blue)   shown.]
and_w_(red)_is_shown.]
**** Second example: ordered pairs of numbers[edit] ****
A second key example of a vector space is provided by pairs of real numbers x
and y. (The order of the components x and y is significant, so such a pair is
also called an ordered_pair.) Such a pair is written as (x, y). The sum of two
such pairs and multiplication of a pair with a number is defined as follows:
      (x1, y1) + (x2, y2) = (x1 + x2, y1 + y2)
and
      a (x, y) = (ax, ay).
The first example above reduces to this one if the arrows are represented by
the pair of Cartesian_coordinates of their end points.
**** Definition[edit] ****
In this article, vectors are represented in boldface to distinguish them from
scalars.[nb_1]
A vector space over a field F is a set V together with two operations that
satisfy the eight axioms listed below.
    * The first operation, called vector addition or simply addition  + : V Ã
      V â V, takes any two vectors v and w and assigns to them a third vector
      which is commonly written as v + w, and called the sum of these two
      vectors. (Note that the resultant vector is also an element of the set V
      ).
    * The second operation, called scalar_multiplication  Â· : F Ã V â Vï¼
      takes any scalar a and any vector v and gives another vector av.
      (Similarly, the vector av is an element of the set V).
Elements of V are commonly called vectors. Elements of F are commonly called
scalars.
In the two examples above, the field is the field of the real numbers and the
set of the vectors consists of the planar arrows with fixed starting point and
of pairs of real numbers, respectively.
To qualify as a vector space, the set V and the operations of addition and
multiplication must adhere to a number of requirements called axioms.[1] In the
list below, let u, v and w be arbitrary vectors in V, and a and b scalars in F.
Axiom                 Meaning
Associativity of      u + (v + w) = (u + v) + w
addition
Commutativity of      u + v = v + u
addition
Identity_element of   There exists an element 0 â V, called the zero_vector, such that v + 0 = v for
addition              all v â V.
Inverse_elements of   For every v â V, there exists an element âv â V, called the additive
addition              inverse of v, such that v + (âv) = 0.
Compatibility of
scalar multiplication a(bv) = (ab)v [nb_2]
with field
multiplication
Identity element of   1v = v, where 1 denotes the multiplicative_identity in F.
scalar multiplication
Distributivity of
scalar multiplication a(u + v) = au + av
with respect to
vector addition  
Distributivity of
scalar multiplication (a + b)v = av + bv
with respect to field
addition
These axioms generalize properties of the vectors introduced in the above
examples. Indeed, the result of addition of two ordered pairs (as in the second
example above) does not depend on the order of the summands:
      (xv, yv) + (xw, yw) = (xw, yw) + (xv, yv).
Likewise, in the geometric example of vectors as arrows, v + w = w + v since
the parallelogram defining the sum of the vectors is independent of the order
of the vectors. All other axioms can be checked in a similar manner in both
examples. Thus, by disregarding the concrete nature of the particular type of
vectors, the definition incorporates these two and many more examples in one
notion of vector space.
Subtraction of two vectors and division by a (non-zero) scalar can be defined
as
              v  &#x2212;  w     =  v  + ( &#x2212;  w  )        v  a      =
      1 a    v        {\displaystyle {\begin{aligned}\mathbf {v} -\mathbf {w}
      &=\mathbf {v} +(-\mathbf {w} )\\{\frac {\mathbf {v} }{a}}&={\frac {1}
      {a}}\mathbf {v} \end{aligned}}}  [{\displaystyle {\begin{aligned}\mathbf
      {v} -\mathbf {w} &=\mathbf {v} +(-\mathbf {w} )\\{\frac {\mathbf {v} }
      {a}}&={\frac {1}{a}}\mathbf {v} \end{aligned}}}].
When the scalar field F is the real_numbers R, the vector space is called a
real vector space. When the scalar field is the complex_numbers C, the vector
space is called a complex vector space. These two cases are the ones used most
often in engineering. The general definition of a vector space allows scalars
to be elements of any fixed field F. The notion is then known as an F-vector
spaces or a vector space over F. A field is, essentially, a set of numbers
possessing addition, subtraction, multiplication and division operations.[nb_3]
For example, rational_numbers form a field.
In contrast to the intuition stemming from vectors in the plane and higher-
dimensional cases, there is, in general vector spaces, no notion of nearness,
angles or distances. To deal with such matters, particular types of vector
spaces are introduced; see below.[clarification_needed]
**** Alternative formulations and elementary consequences[edit] ****
Vector addition and scalar multiplication are operations, satisfying the
closure property: u + v and av are in V for all a in F, and u, v in V. Some
older sources mention these properties as separate axioms.[2]
In the parlance of abstract_algebra, the first four axioms are equivalent to
requiring the set of vectors to be an abelian_group under addition. The
remaining axioms give this group an F-module structure. In other words, there
is a ring_homomorphism f from the field F into the endomorphism_ring of the
group of vectors. Then scalar multiplication av is defined as (f(a))(v).[3]
There are a number of direct consequences of the vector space axioms. Some of
them derive from elementary_group_theory, applied to the additive group of
vectors: for example, the zero vector 0 of V and the additive inverse âv of
any vector v are unique. Further properties follow by employing also the
distributive law for the scalar multiplication, for example av equals 0 if and
only if a equals 0 or v equals 0.
***** History[edit] *****
Vector spaces stem from affine_geometry via the introduction of coordinates in
the plane or three-dimensional space. Around 1636, Descartes and Fermat founded
analytic_geometry by equating solutions to an equation of two variables with
points on a plane curve.[4] In 1804, to achieve geometric solutions without
using coordinates, Bolzano introduced certain operations on points, lines and
planes, which are predecessors of vectors.[5] His work was then used in the
conception of barycentric_coordinates by MÃ¶bius in 1827.[6] In 1828 C._V.
Mourey suggested the existence of an algebra surpassing not only ordinary
algebra but also two-dimensional algebra created by him searching a geometrical
interpretation of complex numbers.[7]
The definition of vectors was founded on Bellavitis' notion of the bipoint, an
oriented segment of which one end is the origin and the other a target, then
further elaborated with the presentation of complex_numbers by Argand and
Hamilton and the introduction of quaternions and biquaternions by the latter.
[8] They are elements in R2, R4, and R8; their treatment as linear_combinations
can be traced back to Laguerre in 1867, who also defined systems_of_linear
equations.
In 1857, Cayley introduced matrix_notation, which allows for a harmonization
and simplification of linear_maps. Around the same time, Grassmann studied the
barycentric calculus initiated by MÃ¶bius. He envisaged sets of abstract
objects endowed with operations.[9] In his work, the concepts of linear
independence and dimension, as well as scalar_products, are present. In fact,
Grassmann's 1844 work extended a vector space of n dimensions to one of 2n
dimensions by consideration of 2-vectors     u &#x2227; v   {\displaystyle
u\wedge v}  [{\displaystyle u\wedge v}] and 3-vectors     u &#x2227; v &#x2227;
w   {\displaystyle u\wedge v\wedge w}  [{\displaystyle u\wedge v\wedge w}]
called multivectors. This extension, called multilinear_algebra, is governed by
the rules of exterior_algebra. Peano was the first to give the modern
definition of vector spaces and linear maps in 1888.[10]
An important development of vector spaces is due to the construction of
function_spaces by Lebesgue. This was later formalized by Banach and Hilbert,
around 1920.[11] At that time, algebra and the new field of functional_analysis
began to interact, notably with key concepts such as spaces_of_p-integrable
functions and Hilbert_spaces.[12] Vector spaces, including infinite-dimensional
ones, then became a firmly established notion, and many mathematical branches
started making use of this concept.
***** Examples[edit] *****
Main article: Examples_of_vector_spaces
**** Coordinate spaces[edit] ****
Main article: Coordinate_space
The simplest example of a vector space over a field F is the field itself,
equipped with its standard addition and multiplication. More generally, all n-
tuples (sequences of length n)
      (a1, a2, ..., an)
of elements of F form a vector space that is usually denoted Fn and called a
coordinate_space.[13] The case n = 1 is the above-mentioned simplest example,
in which the field F is also regarded as a vector space over itself. The case F
= R and n = 2 was discussed in the introduction above.
**** Complex numbers and other field extensions[edit] ****
The set of complex_numbers C, i.e., numbers that can be written in the form x +
iy for real_numbers x and y where i is the imaginary_unit, form a vector space
over the reals with the usual addition and multiplication: (x + iy) + (a + ib)
= (x + a) + i(y + b) and c â (x + iy) = (c â x) + i(c â y) for real
numbers x, y, a, b and c. The various axioms of a vector space follow from the
fact that the same rules hold for complex number arithmetic.
In fact, the example of complex numbers is essentially the same (i.e., it is
isomorphic) to the vector space of ordered pairs of real numbers mentioned
above: if we think of the complex number x + i y as representing the ordered
pair (x, y) in the complex_plane then we see that the rules for sum and scalar
product correspond exactly to those in the earlier example.
More generally, field_extensions provide another class of examples of vector
spaces, particularly in algebra and algebraic_number_theory: a field F
containing a smaller_field E is an E-vector space, by the given multiplication
and addition operations of F.[14] For example, the complex numbers are a vector
space over R, and the field extension      Q  ( i   5   )   {\displaystyle
\mathbf {Q} (i{\sqrt {5}})}  [\mathbf {Q} (i{\sqrt {5}})] is a vector space
over Q.
**** Function spaces[edit] ****
Main article: Function_space
Addition of functions: The sum of the sine and the exponential function is
sin + exp :  R  &#x2192;  R    {\displaystyle \sin +\exp :\mathbb {R} \to
\mathbb {R} }  [{\displaystyle \sin +\exp :\mathbb {R} \to \mathbb {R} }] with
( sin + exp ) ( x ) = sin &#x2061; ( x ) + exp &#x2061; ( x )   {\displaystyle
(\sin +\exp )(x)=\sin(x)+\exp(x)}  [{\displaystyle (\sin +\exp )(x)=\sin
(x)+\exp(x)}]
Functions from any fixed set Î© to a field F also form vector spaces, by
performing addition and scalar multiplication pointwise. That is, the sum of
two functions f and g is the function (f + g) given by
      (f + g)(w) = f(w) + g(w),
and similarly for multiplication. Such function spaces occur in many geometric
situations, when Î© is the real_line or an interval, or other subsets of R.
Many notions in topology and analysis, such as continuity, integrability or
differentiability are well-behaved with respect to linearity: sums and scalar
multiples of functions possessing such a property still have that property.[15]
Therefore, the set of such functions are vector spaces. They are studied in
greater detail using the methods of functional_analysis, see below.
[clarification_needed] Algebraic constraints also yield vector spaces: the
vector_space_F[x] is given by polynomial_functions:
      f(x) = r0 + r1x + ... + rnâ1xnâ1 + rnxn, where the coefficients r0,
      ..., rn are in F.[16]
**** Linear equations[edit] ****
Main articles: Linear_equation, Linear_differential_equation, and Systems_of
linear_equations
Systems of homogeneous_linear_equations are closely tied to vector spaces.[17]
For example, the solutions of
      a  + 3b + c  = 0
      4a + 2b + 2c = 0
are given by triples with arbitrary a, b = a/2, and c = â5a/2. They form a
vector space: sums and scalar multiples of such triples still satisfy the same
ratios of the three variables; thus they are solutions, too. Matrices can be
used to condense multiple linear equations as above into one vector equation,
namely
      Ax = 0,
where A =       [    1   3   1     4   2   2    ]     {\displaystyle {\begin
{bmatrix}1&3&1\\4&2&2\end{bmatrix}}}  [{\begin{bmatrix}1&3&1\\4&2&2\end
{bmatrix}}] is the matrix containing the coefficients of the given equations, x
is the vector (a, b, c), Ax denotes the matrix_product, and 0 = (0, 0) is the
zero vector. In a similar vein, the solutions of homogeneous linear
differential equations form vector spaces. For example,
      fâ²â²(x) + 2fâ²(x) + f(x) = 0
yields f(x) = a eâx + bx eâx, where a and b are arbitrary constants, and ex
is the natural_exponential_function.
***** Basis and dimension[edit] *****
Main articles: Basis and Dimension
A vector v in R2 (blue) expressed in terms of different bases: using the
standard_basis of R2 v = xe1 + ye2 (black), and using a different, non-
orthogonal basis: v = f1 + f2 (red).
Bases allow one to represent vectors by a sequence of scalars called
coordinates or components. A basis is a (finite or infinite) set B = {bi}i â
I of vectors bi, for convenience often indexed by some index_set I, that spans
the whole space and is linearly_independent. "Spanning the whole space" means
that any vector v can be expressed as a finite sum (called a linear
combination) of the basis elements:
          v  =  a  1     b    i  1     +  a  2     b    i  2     +
      &#x22EF; +  a  n     b    i  n     ,   {\displaystyle \mathbf
      {v} =a_{1}\mathbf {b} _{i_{1}}+a_{2}\mathbf {b} _{i_{2}}+\cdots    (1)
      +a_{n}\mathbf {b} _{i_{n}},}  [\mathbf {v} =a_{1}\mathbf {b} _     
      {i_{1}}+a_{2}\mathbf {b} _{i_{2}}+\cdots +a_{n}\mathbf {b} _{i_
      {n}},]
where the ak are scalars, called the coordinates (or the components) of the
vector v with respect to the basis B, and bik (k = 1, ..., n) elements of B.
Linear independence means that the coordinates ak are uniquely determined for
any vector in the vector space.
For example, the coordinate_vectors e1 = (1, 0, ..., 0), e2 = (0, 1, 0, ...,
0), to en = (0, 0, ..., 0, 1), form a basis of Fn, called the standard_basis,
since any vector (x1, x2, ..., xn) can be uniquely expressed as a linear
combination of these vectors:
      (x1, x2, ..., xn) = x1(1, 0, ..., 0) + x2(0, 1, 0, ..., 0) + ... + xn(0,
      ..., 0, 1) = x1e1 + x2e2 + ... + xnen.
The corresponding coordinates x1, x2, ..., xn are just the Cartesian
coordinates of the vector.
Every vector space has a basis. This follows from Zorn's_lemma, an equivalent
formulation of the Axiom_of_Choice.[18] Given the other axioms of
ZermeloâFraenkel_set_theory, the existence of bases is equivalent to the
axiom of choice.[19] The ultrafilter_lemma, which is weaker than the axiom of
choice, implies that all bases of a given vector space have the same number of
elements, or cardinality (cf. Dimension_theorem_for_vector_spaces).[20] It is
called the dimension of the vector space, denoted by dim V. If the space is
spanned by finitely many vectors, the above statements can be proven without
such fundamental input from set theory.[21]
The dimension of the coordinate space Fn is n, by the basis exhibited above.
The dimension of the polynomial ring F[x] introduced above[clarification
needed] is countably_infinite, a basis is given by 1, x, x2, ... A_fortiori,
the dimension of more general function spaces, such as the space of functions
on some (bounded or unbounded) interval, is infinite.[nb_4] Under suitable
regularity assumptions on the coefficients involved, the dimension of the
solution space of a homogeneous ordinary_differential_equation equals the
degree of the equation.[22] For example, the solution space for the above
equation[clarification_needed] is generated by eâx and xeâx. These two
functions are linearly independent over R, so the dimension of this space is
two, as is the degree of the equation.
A field extension over the rationals Q can be thought of as a vector space over
Q (by defining vector addition as field addition, defining scalar
multiplication as field multiplication by elements of Q, and otherwise ignoring
the field multiplication). The dimension (or degree) of the field extension Q
(Î±) over Q depends on Î±. If Î± satisfies some polynomial equation
    q  n    &#x03B1;  n   +  q  n &#x2212; 1    &#x03B1;  n &#x2212; 1   +
&#x2026; +  q  0   = 0   {\displaystyle q_{n}\alpha ^{n}+q_{n-1}\alpha ^{n-
1}+\ldots +q_{0}=0}
[{\displaystyle q_{n}\alpha ^{n}+q_{n-1}\alpha ^{n-1}+\ldots +q_{0}=0}]
with rational coefficients qn, ..., q0 (in other words, if Î± is algebraic),
the dimension is finite. More precisely, it equals the degree of the minimal
polynomial having Î± as a root.[23] For example, the complex numbers C are a
two-dimensional real vector space, generated by 1 and the imaginary_unit i. The
latter satisfies i2 + 1 = 0, an equation of degree two. Thus, C is a two-
dimensional R-vector space (and, as any field, one-dimensional as a vector
space over itself, C). If Î± is not algebraic, the dimension of Q(Î±) over Q is
infinite. For instance, for Î± = Ï there is no such equation, in other words
Ï is transcendental.[24]
***** Linear maps and matrices[edit] *****
Main article: Linear_map
The relation of two vector spaces can be expressed by linear map or linear
transformation. They are functions that reflect the vector space
structureâi.e., they preserve sums and scalar multiplication:
         f (  v  +  w  ) = f (  v  ) + f (  w  )   {\displaystyle f(\mathbf {v}
      +\mathbf {w} )=f(\mathbf {v} )+f(\mathbf {w} )}  [{\displaystyle f
      (\mathbf {v} +\mathbf {w} )=f(\mathbf {v} )+f(\mathbf {w} )}] and f(a Â·
      v)     =   {\displaystyle =}  [=] a Â· f(v) for all v and w in V, all a
      in F.[25]
An isomorphism is a linear map f : V â W such that there exists an inverse
map g : W â V, which is a map such that the two possible compositions f â
g : W â W and g â f : V â V are identity_maps. Equivalently, f is both
one-to-one (injective) and onto (surjective).[26] If there exists an
isomorphism between V and W, the two spaces are said to be isomorphic; they are
then essentially identical as vector spaces, since all identities holding in V
are, via f, transported to similar ones in W, and vice versa via g.
Describing an arrow vector v by its coordinates x and y yields an isomorphism
of vector spaces.
For example, the "arrows in the plane" and "ordered pairs of numbers" vector
spaces in the introduction are isomorphic: a planar arrow v departing at the
origin of some (fixed) coordinate_system can be expressed as an ordered pair by
considering the x- and y-component of the arrow, as shown in the image at the
right. Conversely, given a pair (x, y), the arrow going by x to the right (or
to the left, if x is negative), and y up (down, if y is negative) turns back
the arrow v.
Linear maps V â W between two vector spaces form a vector space HomF(V, W),
also denoted L(V, W).[27] The space of linear maps from V to F is called the
dual_vector_space, denoted Vâ.[28] Via the injective natural map V â
Vââ, any vector space can be embedded into its bidual; the map is an
isomorphism if and only if the space is finite-dimensional.[29]
Once a basis of V is chosen, linear maps f : V â W are completely determined
by specifying the images of the basis vectors, because any element of V is
expressed uniquely as a linear combination of them.[30] If dim V = dim W, a 1-
to-1_correspondence between fixed bases of V and W gives rise to a linear map
that maps any basis element of V to the corresponding basis element of W. It is
an isomorphism, by its very definition.[31] Therefore, two vector spaces are
isomorphic if their dimensions agree and vice versa. Another way to express
this is that any vector space is completely classified (up_to isomorphism) by
its dimension, a single number. In particular, any n-dimensional F-vector space
V is isomorphic to Fn. There is, however, no "canonical" or preferred
isomorphism; actually an isomorphism Ï : Fn â V is equivalent to the choice
of a basis of V, by mapping the standard basis of Fn to V, via Ï. The freedom
of choosing a convenient basis is particularly useful in the infinite-
dimensional context; see below.[clarification_needed]
**** Matrices[edit] ****
Main articles: Matrix and Determinant
A typical matrix
Matrices are a useful notion to encode linear maps.[32] They are written as a
rectangular array of scalars as in the image at the right. Any m-by-n matrix A
gives rise to a linear map from Fn to Fm, by the following
          x  = (  x  1   ,  x  2   , &#x22EF; ,  x  n   ) &#x21A6;
      (   &#x2211;  j = 1   n    a  1 j    x  j   ,  &#x2211;  j = 1   n    a
      2 j    x  j   , &#x22EF; ,  &#x2211;  j = 1   n    a  m j    x  j    )
      {\displaystyle \mathbf {x} =(x_{1},x_{2},\cdots ,x_{n})\mapsto \left(\sum
      _{j=1}^{n}a_{1j}x_{j},\sum _{j=1}^{n}a_{2j}x_{j},\cdots ,\sum _{j=1}^
      {n}a_{mj}x_{j}\right)}  [\mathbf {x} =(x_{1},x_{2},\cdots ,x_{n})\mapsto
      \left(\sum _{j=1}^{n}a_{1j}x_{j},\sum _{j=1}^{n}a_{2j}x_{j},\cdots ,\sum
      _{j=1}^{n}a_{mj}x_{j}\right)], where     &#x2211;   {\displaystyle \sum }
      [\sum ] denotes summation,
or, using the matrix_multiplication of the matrix A with the coordinate vector
x:
      x â¦ Ax.
Moreover, after choosing bases of V and W, any linear map f : V â W is
uniquely represented by a matrix via this assignment.[33]
The volume of this parallelepiped is the absolute value of the determinant of
the 3-by-3 matrix formed by the vectors r1, r2, and r3.
The determinant det (A) of a square_matrix A is a scalar that tells whether the
associated map is an isomorphism or not: to be so it is sufficient and
necessary that the determinant is nonzero.[34] The linear transformation of Rn
corresponding to a real n-by-n matrix is orientation_preserving if and only if
its determinant is positive.
**** Eigenvalues and eigenvectors[edit] ****
Main article: Eigenvalues_and_eigenvectors
Endomorphisms, linear maps f : V â V, are particularly important since in
this case vectors v can be compared with their image under f, f(v). Any nonzero
vector v satisfying Î»v = f(v), where Î» is a scalar, is called an eigenvector
of f with eigenvalue Î».[nb_5][35] Equivalently, v is an element of the kernel
of the difference f â Î» Â· Id (where Id is the identity_map V â V). If V
is finite-dimensional, this can be rephrased using determinants: f having
eigenvalue Î» is equivalent to
      det(f â Î» Â· Id) = 0.
By spelling out the definition of the determinant, the expression on the left
hand side can be seen to be a polynomial function in Î», called the
characteristic_polynomial of f.[36] If the field F is large enough to contain a
zero of this polynomial (which automatically happens for F algebraically
closed, such as F = C) any linear map has at least one eigenvector. The vector
space V may or may not possess an eigenbasis, a basis consisting of
eigenvectors. This phenomenon is governed by the Jordan_canonical_form of the
map.[37][nb_6] The set of all eigenvectors corresponding to a particular
eigenvalue of f forms a vector space known as the eigenspace corresponding to
the eigenvalue (and f) in question. To achieve the spectral_theorem, the
corresponding statement in the infinite-dimensional case, the machinery of
functional analysis is needed, see below.[clarification_needed]
***** Basic constructions[edit] *****
In addition to the above concrete examples, there are a number of standard
linear algebraic constructions that yield vector spaces related to given ones.
In addition to the definitions given below, they are also characterized by
universal_properties, which determine an object X by specifying the linear maps
from X to any other vector space.
**** Subspaces and quotient spaces[edit] ****
Main articles: Linear_subspace and Quotient_vector_space
A line passing through the origin (blue, thick) in R3 is a linear subspace. It
is the intersection of two planes (green and yellow).
A nonempty subset W of a vector space V that is closed under addition and
scalar multiplication (and therefore contains the 0-vector of V) is called a
linear subspace of V, or simply a subspace of V, when the ambient space is
unambiguously a vector space.[38][nb_7] Subspaces of V are vector spaces (over
the same field) in their own right. The intersection of all subspaces
containing a given set S of vectors is called its span, and it is the smallest
subspace of V containing the set S. Expressed in terms of elements, the span is
the subspace consisting of all the linear_combinations of elements of S.[39]
A linear subspace of dimension 1 is a vector line. A linear subspace of
dimension 2 is a vector plane. A linear subspace that contains all elements but
one of a basis of the ambient space is a vector hyperplane. In a vector space
of finite dimension n, a vector hyperplane is thus a subspace of dimension n
â 1.
The counterpart to subspaces are quotient vector spaces.[40] Given any subspace
W â V, the quotient space V/W ("V modulo W") is defined as follows: as a set,
it consists of v + W = {v + w : w â W}, where v is an arbitrary vector in V.
The sum of two such elements v1 + W and v2 + W is (v1 + v2) + W, and scalar
multiplication is given by a Â· (v + W) = (a Â· v) + W. The key point in this
definition is that v1 + W = v2 + W if_and_only_if the difference of v1 and v2
lies in W.[nb_8] This way, the quotient space "forgets" information that is
contained in the subspace W.
The kernel ker(f) of a linear map f : V â W consists of vectors v that are
mapped to 0 in W.[41] Both kernel and image im(f) = {f(v) : v â V} are
subspaces of V and W, respectively.[42] The existence of kernels and images is
part of the statement that the category_of_vector_spaces (over a fixed field F)
is an abelian_category, i.e. a corpus of mathematical objects and structure-
preserving maps between them (a category) that behaves much like the category
of_abelian_groups.[43] Because of this, many statements such as the first
isomorphism_theorem (also called rankânullity_theorem in matrix-related
terms)
      V / ker(f) â¡ im(f).
and the second and third isomorphism theorem can be formulated and proven in a
way very similar to the corresponding statements for groups.
An important example is the kernel of a linear map x â¦ Ax for some fixed
matrix A, as above.[clarification_needed] The kernel of this map is the
subspace of vectors x such that Ax = 0, which is precisely the set of solutions
to the system of homogeneous linear equations belonging to A. This concept also
extends to linear differential equations
          a  0   f +  a  1      d f   d x    +  a  2       d  2   f   d  x  2
      + &#x22EF; +  a  n       d  n   f   d  x  n      = 0   {\displaystyle a_
      {0}f+a_{1}{\frac {df}{dx}}+a_{2}{\frac {d^{2}f}{dx^{2}}}+\cdots +a_{n}
      {\frac {d^{n}f}{dx^{n}}}=0}  [a_{0}f+a_{1}{\frac {df}{dx}}+a_{2}{\frac
      {d^{2}f}{dx^{2}}}+\cdots +a_{n}{\frac {d^{n}f}{dx^{n}}}=0], where the
      coefficients ai are functions in x, too.
In the corresponding map
         f &#x21A6; D ( f ) =  &#x2211;  i = 0   n    a  i       d  i   f   d
      x  i        {\displaystyle f\mapsto D(f)=\sum _{i=0}^{n}a_{i}{\frac {d^
      {i}f}{dx^{i}}}}  [f\mapsto D(f)=\sum _{i=0}^{n}a_{i}{\frac {d^{i}f}{dx^
      {i}}}],
the derivatives of the function f appear linearly (as opposed to fâ²â²(x)2,
for example). Since differentiation is a linear procedure (i.e., (f + g)â² =
fâ² + g â² and (cÂ·f)â² = cÂ·fâ² for a constant c) this assignment is
linear, called a linear_differential_operator. In particular, the solutions to
the differential equation D(f) = 0 form a vector space (over R or C).
**** Direct product and direct sum[edit] ****
Main articles: Direct_product and Direct_sum_of_modules
The direct product of vector spaces and the direct sum of vector spaces are two
ways of combining an indexed family of vector spaces into a new vector space.
The direct product        &#x220F;  i &#x2208; I    V  i       {\displaystyle
\textstyle {\prod _{i\in I}V_{i}}}  [\textstyle {\prod _{i\in I}V_{i}}] of a
family of vector spaces Vi consists of the set of all tuples (vi)i â I, which
specify for each index i in some index_set I an element vi of Vi.[44] Addition
and scalar multiplication is performed componentwise. A variant of this
construction is the direct sum      &#x2295;  i &#x2208; I    V  i
{\displaystyle \oplus _{i\in I}V_{i}}  [\oplus _{i\in I}V_{i}] (also called
coproduct and denoted        &#x2210;  i &#x2208; I    V  i
{\displaystyle \textstyle {\coprod _{i\in I}V_{i}}}  [\textstyle {\coprod _
{i\in I}V_{i}}]), where only tuples with finitely many nonzero vectors are
allowed. If the index set I is finite, the two constructions agree, but in
general they are different.
**** Tensor product[edit] ****
Main article: Tensor_product_of_vector_spaces
The tensor product V âF W, or simply V â W, of two vector spaces V and W is
one of the central notions of multilinear_algebra which deals with extending
notions such as linear maps to several variables. A map g : V_Ã_W â X is
called bilinear if g is linear in both variables v and w. That is to say, for
fixed w the map v â¦ g(v, w) is linear in the sense above and likewise for
fixed v.
The tensor product is a particular vector space that is a universal recipient
of bilinear maps g, as follows. It is defined as the vector space consisting of
finite (formal) sums of symbols called tensors
      v1 â w1 + v2 â w2 + ... + vn â wn,
subject to the rules
      a · (v â w) = (a · v) â w = v â (a · w), where a is a scalar,
      (v1 + v2) â w = v1 â w + v2 â w, and
      v â (w1 + w2) = v â w1 + v â w2.[45]
Commutative_diagram depicting the universal property of the tensor product.
These rules ensure that the map f from the V Ã W to V â W that maps a tuple
(v, w) to v â w is bilinear. The universality states that given any vector
space X and any bilinear map g : V Ã W â X, there exists a unique map u,
shown in the diagram with a dotted arrow, whose composition with f equals g: u
(v â w) = g(v, w).[46] This is called the universal_property of the tensor
product, an instance of the methodâmuch used in advanced abstract
algebraâto indirectly define objects by specifying maps from or to this
object.
***** Vector spaces with additional structure[edit] *****
From the point of view of linear algebra, vector spaces are completely
understood insofar as any vector space is characterized, up to isomorphism, by
its dimension. However, vector spaces per se do not offer a framework to deal
with the questionâcrucial to analysisâwhether a sequence of functions
converges to another function. Likewise, linear algebra is not adapted to deal
with infinite_series, since the addition operation allows only finitely many
terms to be added. Therefore, the needs of functional_analysis require
considering additional structures.
A vector space may be given a partial_order â¤, under which some vectors can
be compared.[47] For example, n-dimensional real space Rn can be ordered by
comparing its vectors componentwise. Ordered_vector_spaces, for example Riesz
spaces, are fundamental to Lebesgue_integration, which relies on the ability to
express a function as a difference of two positive functions
      f = f+ â fâ,
where f+ denotes the positive part of f and fâ the negative part.[48]
**** Normed vector spaces and inner product spaces[edit] ****
Main articles: Normed_vector_space and Inner_product_space
"Measuring" vectors is done by specifying a norm, a datum which measures
lengths of vectors, or by an inner_product, which measures angles between
vectors. Norms and inner products are denoted      |   v   |    {\displaystyle
|\mathbf {v} |}  [|\mathbf {v} |] and     &#x27E8;  v  ,  w  &#x27E9;
{\displaystyle \langle \mathbf {v} ,\mathbf {w} \rangle }  [\langle \mathbf {v}
,\mathbf {w} \rangle ], respectively. The datum of an inner product entails
that lengths of vectors can be defined too, by defining the associated norm
|   v   |  :=   &#x27E8;  v  ,  v  &#x27E9;     {\displaystyle |\mathbf {v} |:=
{\sqrt {\langle \mathbf {v} ,\mathbf {v} \rangle }}}  [|\mathbf {v} |:={\sqrt
{\langle \mathbf {v} ,\mathbf {v} \rangle }}]. Vector spaces endowed with such
data are known as normed vector spaces and inner product spaces, respectively.
[49]
Coordinate space Fn can be equipped with the standard dot_product:
         &#x27E8;  x  ,  y  &#x27E9; =  x  &#x22C5;  y  =  x  1    y  1   +
      &#x22EF; +  x  n    y  n   .   {\displaystyle \langle \mathbf {x}
      ,\mathbf {y} \rangle =\mathbf {x} \cdot \mathbf {y} =x_{1}y_{1}+\cdots
      +x_{n}y_{n}.}  [\langle \mathbf {x} ,\mathbf {y} \rangle =\mathbf {x}
      \cdot \mathbf {y} =x_{1}y_{1}+\cdots +x_{n}y_{n}.]
In R2, this reflects the common notion of the angle between two vectors x and
y, by the law_of_cosines:
          x  &#x22C5;  y  = cos &#x2061;  (  &#x2220; (  x  ,  y  )  )
      &#x22C5;  |   x   |  &#x22C5;  |   y   |  .   {\displaystyle \mathbf {x}
      \cdot \mathbf {y} =\cos \left(\angle (\mathbf {x} ,\mathbf {y}
      )\right)\cdot |\mathbf {x} |\cdot |\mathbf {y} |.}  [\mathbf {x} \cdot
      \mathbf {y} =\cos \left(\angle (\mathbf {x} ,\mathbf {y} )\right)\cdot
      |\mathbf {x} |\cdot |\mathbf {y} |.]
Because of this, two vectors satisfying     &#x27E8;  x  ,  y  &#x27E9; = 0
{\displaystyle \langle \mathbf {x} ,\mathbf {y} \rangle =0}  [\langle \mathbf
{x} ,\mathbf {y} \rangle =0] are called orthogonal. An important variant of the
standard dot product is used in Minkowski_space: R4 endowed with the Lorentz
product
         &#x27E8;  x   |   y  &#x27E9; =  x  1    y  1   +  x  2    y  2   +  x
      3    y  3   &#x2212;  x  4    y  4   .   {\displaystyle \langle \mathbf
      {x} |\mathbf {y} \rangle =x_{1}y_{1}+x_{2}y_{2}+x_{3}y_{3}-x_{4}y_{4}.}
      [\langle \mathbf {x} |\mathbf {y} \rangle =x_{1}y_{1}+x_{2}y_{2}+x_{3}y_
      {3}-x_{4}y_{4}.][50]
In contrast to the standard dot product, it is not positive_definite:
&#x27E8;  x   |   x  &#x27E9;   {\displaystyle \langle \mathbf {x} |\mathbf {x}
\rangle }  [\langle \mathbf {x} |\mathbf {x} \rangle ] also takes negative
values, for example for      x  = ( 0 , 0 , 0 , 1 )   {\displaystyle \mathbf
{x} =(0,0,0,1)}  [\mathbf {x} =(0,0,0,1)]. Singling out the fourth
coordinateâcorresponding_to_time, as opposed to three space-
dimensionsâmakes it useful for the mathematical treatment of special
relativity.
**** Topological vector spaces[edit] ****
Main article: Topological_vector_space
Convergence questions are treated by considering vector spaces V carrying a
compatible topology, a structure that allows one to talk about elements being
close_to_each_other.[51][52] Compatible here means that addition and scalar
multiplication have to be continuous_maps. Roughly, if x and y in V, and a in F
vary by a bounded amount, then so do x + y and ax.[nb_9] To make sense of
specifying the amount a scalar changes, the field F also has to carry a
topology in this context; a common choice are the reals or the complex numbers.
In such topological vector spaces one can consider series of vectors. The
infinite_sum
          &#x2211;  i = 0   &#x221E;    f  i     {\displaystyle \sum _{i=0}^
      {\infty }f_{i}}  [\sum _{i=0}^{\infty }f_{i}]
denotes the limit of the corresponding finite partial sums of the sequence
(fi)iâN of elements of V. For example, the fi could be (real or complex)
functions belonging to some function_space V, in which case the series is a
function_series. The mode_of_convergence of the series depends on the topology
imposed on the function space. In such cases, pointwise_convergence and uniform
convergence are two prominent examples.
Unit_"spheres" in R2 consist of plane vectors of norm 1. Depicted are the unit
spheres in different p-norms, for p = 1, 2, and â. The bigger diamond depicts
points of 1-norm equal to 2.
A way to ensure the existence of limits of certain infinite series is to
restrict attention to spaces where any Cauchy_sequence has a limit; such a
vector space is called complete. Roughly, a vector space is complete provided
that it contains all necessary limits. For example, the vector space of
polynomials on the unit interval [0,1], equipped with the topology_of_uniform
convergence is not complete because any continuous function on [0,1] can be
uniformly approximated by a sequence of polynomials, by the Weierstrass
approximation_theorem.[53] In contrast, the space of all continuous functions
on [0,1] with the same topology is complete.[54] A norm gives rise to a
topology by defining that a sequence of vectors vn converges to v if and only
if
           lim   n &#x2192; &#x221E;    |    v   n   &#x2212;  v   |  = 0.
      {\displaystyle {\text{lim}}_{n\rightarrow \infty }|\mathbf {v} _{n}-
      \mathbf {v} |=0.}  [{\text{lim}}_{n\rightarrow \infty }|\mathbf {v} _{n}-
      \mathbf {v} |=0.]
Banach and Hilbert spaces are complete topological vector spaces whose
topologies are given, respectively, by a norm and an inner product. Their
studyâa key piece of functional_analysisâfocusses on infinite-dimensional
vector spaces, since all norms on finite-dimensional topological vector spaces
give rise to the same notion of convergence.[55] The image at the right shows
the equivalence of the 1-norm and â-norm on R2: as the unit "balls" enclose
each other, a sequence converges to zero in one norm if and only if it so does
in the other norm. In the infinite-dimensional case, however, there will
generally be inequivalent topologies, which makes the study of topological
vector spaces richer than that of vector spaces without additional data.
From a conceptual point of view, all notions related to topological vector
spaces should match the topology. For example, instead of considering all
linear maps (also called functionals) V â W, maps between topological vector
spaces are required to be continuous.[56] In particular, the (topological) dual
space Vâ consists of continuous functionals V â R (or to C). The
fundamental HahnâBanach_theorem is concerned with separating subspaces of
appropriate topological vector spaces by continuous functionals.[57]
*** Banach spaces[edit] ***
Main article: Banach_space
Banach spaces, introduced by Stefan_Banach, are complete normed vector spaces.
[58]
A first example is the_vector_space______&#x2113;__p_____{\displaystyle_\ell_^
{p}}__[{\displaystyle_\ell_^{p}}] consisting of infinite vectors with real
entries      x  =  (   x  1   ,  x  2   , &#x2026; ,  x  n   , &#x2026;  )
{\displaystyle \mathbf {x} =\left(x_{1},x_{2},\ldots ,x_{n},\ldots \right)}  [
{\displaystyle \mathbf {x} =\left(x_{1},x_{2},\ldots ,x_{n},\ldots \right)}]
whose ___p___{\displaystyle_p}__[p]-norm     ( 1 &#x2264;  p  &#x2264; &#x221E;
)   {\displaystyle (1\leq {p}\leq \infty )}  [{\displaystyle (1\leq {p}\leq
\infty )}] given by
           &#x2016;  x  &#x2016;   p   :=   (   &#x2211;  i     |  x  i   |   p
      )    1 p      {\displaystyle \left\Vert \mathbf {x} \right\Vert _{p}:
      =\left(\sum _{i}\left\vert x_{i}\right\vert ^{p}\right)^{\frac {1}{p}}}
      [{\displaystyle \left\Vert \mathbf {x} \right\Vert _{p}:=\left(\sum _
      {i}\left\vert x_{i}\right\vert ^{p}\right)^{\frac {1}{p}}}] for     p <
      &#x221E;   {\displaystyle p<\infty }  [{\displaystyle p<\infty }]   and  
      &#x2016;  x  &#x2016;   &#x221E;   :=   sup   i    |  x  i   |
      {\displaystyle \left\Vert \mathbf {x} \right\Vert _{\infty }:={\text
      {sup}}_{i}\left\vert x_{i}\right\vert }  [{\displaystyle \left\Vert
      \mathbf {x} \right\Vert _{\infty }:={\text{sup}}_{i}\left\vert x_
      {i}\right\vert }].
The topologies on the infinite-dimensional space      &#x2113;  p
{\displaystyle \ell ^{p}}  [{\displaystyle \ell ^{p}}] are inequivalent for
different     p   {\displaystyle p}  [p]. E.g. the sequence of vectors       x
n   =  (   2  &#x2212; n   ,  2  &#x2212; n   , &#x2026; ,  2  &#x2212; n   , 0
, 0 , &#x2026;  )    {\displaystyle \mathbf {x} _{n}=\left(2^{-n},2^{-n},\ldots
,2^{-n},0,0,\ldots \right)}  [{\displaystyle \mathbf {x} _{n}=\left(2^{-n},2^{-
n},\ldots ,2^{-n},0,0,\ldots \right)}], i.e. the first      2  n
{\displaystyle 2^{n}}  [2^{n}] components are      2  &#x2212; n
{\displaystyle 2^{-n}}  [2^{-n}], the following ones are     0   {\displaystyle
0}  [{\displaystyle 0}], converges to the zero_vector for     p = &#x221E;
{\displaystyle p=\infty }  [{\displaystyle p=\infty }], but does not for     p
= 1   {\displaystyle p=1}  [p = 1]:
           &#x2016;   x   n   &#x2016;      &#x221E;     = sup (  2  &#x2212; n
      , 0 ) =  2  &#x2212; n   &#x2192; 0   {\displaystyle \left\Vert \mathbf
      {x} _{n}\right\Vert _{_{\infty }}=\sup(2^{-n},0)=2^{-n}\rightarrow 0}  [
      {\displaystyle \left\Vert \mathbf {x} _{n}\right\Vert _{_{\infty }}=\sup
      (2^{-n},0)=2^{-n}\rightarrow 0}], but       &#x2016;   x   n   &#x2016;
      1   =  &#x2211;  i = 1    2  n      2  &#x2212; n   =  2  n   &#x22C5;  2
      &#x2212; n   = 1.   {\displaystyle \left\Vert \mathbf {x} _{n}\right\Vert
      _{1}=\sum _{i=1}^{2^{n}}2^{-n}=2^{n}\cdot 2^{-n}=1.}  [{\displaystyle
      \left\Vert \mathbf {x} _{n}\right\Vert _{1}=\sum _{i=1}^{2^{n}}2^{-n}=2^
      {n}\cdot 2^{-n}=1.}]
More generally than sequences of real numbers, functions     f &#x003A;
&#x03A9; &#x2192;  R    {\displaystyle f\colon \Omega \to \mathbb {R} }  [
{\displaystyle f\colon \Omega \to \mathbb {R} }] are endowed with a norm that
replaces the above sum by the Lebesgue_integral
           &#x2016;  f  &#x2016;   p   :=   (   &#x222B;  &#x03A9;     |   f
      ( x )   |   p     d &#x03BC;  ( x )    )    1 p    .   {\displaystyle
      \left\Vert {f}\right\Vert _{p}:=\left(\int _{\Omega }\left\vert {f}\left
      (x\right)\right\vert ^{p}\,{d\mu \left(x\right)}\right)^{\frac {1}{p}}.}
      [{\displaystyle \left\Vert {f}\right\Vert _{p}:=\left(\int _{\Omega
      }\left\vert {f}\left(x\right)\right\vert ^{p}\,{d\mu \left
      (x\right)}\right)^{\frac {1}{p}}.}]
The space of integrable_functions on a given domain     &#x03A9;
{\displaystyle \Omega }  [\Omega ] (for example an interval) satisfying
&#x2016;  f  &#x2016;   p   < &#x221E;   {\displaystyle \left\Vert
{f}\right\Vert _{p}<\infty }  [{\displaystyle \left\Vert {f}\right\Vert _
{p}<\infty }], and equipped with this norm are called Lebesgue_spaces, denoted
L    p    ( &#x03A9; )    {\displaystyle L^{\;\!p}\left(\Omega \right)}  [
{\displaystyle L^{\;\!p}\left(\Omega \right)}].[nb_10]
These spaces are complete.[59] (If one uses the Riemann_integral instead, the
space is not complete, which may be seen as a justification for Lebesgue's
integration theory.[nb_11]) Concretely this means that for any sequence of
Lebesgue-integrable functions        f  1   ,  f  2   , &#x2026; ,  f  n   ,
&#x2026;   {\displaystyle f_{1},f_{2},\ldots ,f_{n},\ldots }  [{\displaystyle
f_{1},f_{2},\ldots ,f_{n},\ldots }]   with       &#x2016;   f   n   &#x2016;
p   < &#x221E;   {\displaystyle \left\Vert {f}_{n}\right\Vert _{p}<\infty }  [
{\displaystyle \left\Vert {f}_{n}\right\Vert _{p}<\infty }], satisfying the
condition
          lim  k , &#xA0; n &#x2192; &#x221E;    &#x222B;  &#x03A9;     |    f
      k   ( x ) &#x2212;   f   n   ( x )  |   p     d &#x03BC;  ( x )   = 0
      {\displaystyle \lim _{k,\ n\to \infty }\int _{\Omega }\left\vert {f}_{k}
      (x)-{f}_{n}(x)\right\vert ^{p}\,{d\mu \left(x\right)}=0}  [{\displaystyle
      \lim _{k,\ n\to \infty }\int _{\Omega }\left\vert {f}_{k}(x)-{f}_{n}
      (x)\right\vert ^{p}\,{d\mu \left(x\right)}=0}]
there exists a function      f   ( x )    {\displaystyle {f}\left(x\right)}  [
{\displaystyle {f}\left(x\right)}] belonging to the vector space      L    p
( &#x03A9; )    {\displaystyle L^{\;\!p}\left(\Omega \right)}  [{\displaystyle
L^{\;\!p}\left(\Omega \right)}] such that
          lim  k &#x2192; &#x221E;    &#x222B;  &#x03A9;     |   f   ( x )
      &#x2212;   f   k    ( x )   |   p     d &#x03BC;  ( x )   = 0.
      {\displaystyle \lim _{k\to \infty }\int _{\Omega }\left\vert {f}\left
      (x\right)-{f}_{k}\left(x\right)\right\vert ^{p}\,{d\mu \left
      (x\right)}=0.}  [{\displaystyle \lim _{k\to \infty }\int _{\Omega
      }\left\vert {f}\left(x\right)-{f}_{k}\left(x\right)\right\vert ^{p}\,
      {d\mu \left(x\right)}=0.}]
Imposing boundedness conditions not only on the function, but also on its
derivatives leads to Sobolev_spaces.[60]
*** Hilbert spaces[edit] ***
Main article: Hilbert_space
The succeeding snapshots show summation of 1 to 5 terms in approximating a
periodic function (blue) by finite sum of sine functions (red).
Complete inner product spaces are known as Hilbert spaces, in honor of David
Hilbert.[61] The Hilbert space L2(Î©), with inner product given by
         &#x27E8; f &#xA0; , &#xA0; g &#x27E9; =  &#x222B;  &#x03A9;   f ( x )
      g ( x )  &#x00AF;    d x ,   {\displaystyle \langle f\ ,\ g\rangle =\int
      _{\Omega }f(x){\overline {g(x)}}\,dx,}  [{\displaystyle \langle f\ ,\
      g\rangle =\int _{\Omega }f(x){\overline {g(x)}}\,dx,}]
where        g ( x )  &#x00AF;     {\displaystyle {\overline {g(x)}}}  [
{\overline {g(x)}}] denotes the complex_conjugate of g(x),[62][nb_12] is a key
case.
By definition, in a Hilbert space any Cauchy sequence converges to a limit.
Conversely, finding a sequence of functions fn with desirable properties that
approximates a given limit function, is equally crucial. Early analysis, in the
guise of the Taylor_approximation, established an approximation of
differentiable_functions f by polynomials.[63] By the StoneâWeierstrass
theorem, every continuous function on [a, b] can be approximated as closely as
desired by a polynomial.[64] A similar approximation technique by trigonometric
functions is commonly called Fourier_expansion, and is much applied in
engineering, see below.[clarification_needed] More generally, and more
conceptually, the theorem yields a simple description of what "basic
functions", or, in abstract Hilbert spaces, what basic vectors suffice to
generate a Hilbert space H, in the sense that the closure of their span (i.e.,
finite linear combinations and limits of those) is the whole space. Such a set
of functions is called a basis of H, its cardinality is known as the Hilbert
space_dimension.[nb_13] Not only does the theorem exhibit suitable basis
functions as sufficient for approximation purposes, but together with the
GramâSchmidt_process, it enables one to construct a basis_of_orthogonal
vectors.[65] Such orthogonal bases are the Hilbert space generalization of the
coordinate axes in finite-dimensional Euclidean_space.
The solutions to various differential_equations can be interpreted in terms of
Hilbert spaces. For example, a great many fields in physics and engineering
lead to such equations and frequently solutions with particular physical
properties are used as basis functions, often orthogonal.[66] As an example
from physics, the time-dependent SchrÃ¶dinger_equation in quantum_mechanics
describes the change of physical properties in time by means of a partial
differential_equation, whose solutions are called wavefunctions.[67] Definite
values for physical properties such as energy, or momentum, correspond to
eigenvalues of a certain (linear) differential_operator and the associated
wavefunctions are called eigenstates. The spectral_theorem decomposes a linear
compact_operator acting on functions in terms of these eigenfunctions and their
eigenvalues.[68]
**** Algebras over fields[edit] ****
Main articles: Algebra_over_a_field and Lie_algebra
A hyperbola, given by the equation x â y = 1. The coordinate_ring of
functions on this hyperbola is given by R[x, y] / (x · y â 1), an infinite-
dimensional vector space over R.
General vector spaces do not possess a multiplication between vectors. A vector
space equipped with an additional bilinear_operator defining the multiplication
of two vectors is an algebra over a field.[69] Many algebras stem from
functions on some geometrical object: since functions with values in a given
field can be multiplied pointwise, these entities form algebras. The
StoneâWeierstrass theorem, for example, relies on Banach_algebras which are
both Banach spaces and algebras.
Commutative_algebra makes great use of rings_of_polynomials in one or several
variables, introduced above.[clarification_needed] Their multiplication is both
commutative and associative. These rings and their quotients form the basis of
algebraic_geometry, because they are rings_of_functions_of_algebraic_geometric
objects.[70]
Another crucial example are Lie algebras, which are neither commutative nor
associative, but the failure to be so is limited by the constraints ([x, y]
denotes the product of x and y):
    * [x, y] = â[y, x] (anticommutativity), and
    * [x, [y, z]] + [y, [z, x]] + [z, [x, y]] = 0 (Jacobi_identity).[71]
Examples include the vector space of n-by-n matrices, with [x, y] = xy â yx,
the commutator of two matrices, and R3, endowed with the cross_product.
The tensor_algebra T(V) is a formal way of adding products to any vector space
V to obtain an algebra.[72] As a vector space, it is spanned by symbols, called
simple tensors
      v1 â v2 â ... â vn, where the degree n varies.
The multiplication is given by concatenating such symbols, imposing the
distributive_law under addition, and requiring that scalar multiplication
commute with the tensor product â, much the same way as with the tensor
product of two vector spaces introduced above.[clarification_needed] In
general, there are no relations between v1 â v2 and v2 â v1. Forcing two
such elements to be equal leads to the symmetric_algebra, whereas forcing v1
â v2 = â v2 â v1 yields the exterior_algebra.[73]
When a field, F is explicitly stated, a common term used is F-algebra.
***** Applications[edit] *****
Vector spaces have many applications as they occur frequently in common
circumstances, namely wherever functions with values in some field are
involved. They provide a framework to deal with analytical and geometrical
problems, or are used in the Fourier transform. This list is not exhaustive:
many more applications exist, for example in optimization. The minimax_theorem
of game_theory stating the existence of a unique payoff when all players play
optimally can be formulated and proven using vector spaces methods.[74]
Representation_theory fruitfully transfers the good understanding of linear
algebra and vector spaces to other mathematical domains such as group_theory.
[75]
**** Distributions[edit] ****
Main article: Distribution
A distribution (or generalized function) is a linear map assigning a number to
each "test"_function, typically a smooth_function with compact_support, in a
continuous way: in the above[clarification_needed] terminology the space of
distributions is the (continuous) dual of the test function space.[76] The
latter space is endowed with a topology that takes into account not only f
itself, but also all its higher derivatives. A standard example is the result
of integrating a test function f over some domain Î©:
         I ( f ) =  &#x222B;  &#x03A9;   f ( x )  d x .   {\displaystyle I
      (f)=\int _{\Omega }f(x)\,dx.}  [I(f)=\int _{\Omega }f(x)\,dx.]
When Î© = {p}, the set consisting of a single point, this reduces to the Dirac
distribution, denoted by Î´, which associates to a test function f its value at
the p: Î´(f) = f(p). Distributions are a powerful instrument to solve
differential equations. Since all standard analytic notions such as derivatives
are linear, they extend naturally to the space of distributions. Therefore, the
equation in question can be transferred to a distribution space, which is
bigger than the underlying function space, so that more flexible methods are
available for solving the equation. For example, Green's_functions and
fundamental_solutions are usually distributions rather than proper functions,
and can then be used to find solutions of the equation with prescribed boundary
conditions. The found solution can then in some cases be proven to be actually
a true function, and a solution to the original equation (e.g., using the
LaxâMilgram_theorem, a consequence of the Riesz_representation_theorem).[77]
**** Fourier analysis[edit] ****
Main article: Fourier_analysis
The heat equation describes the dissipation of physical properties over time,
such as the decline of the temperature of a hot body placed in a colder
environment (yellow depicts colder regions than red).
Resolving a periodic_function into a sum of trigonometric_functions forms a
Fourier_series, a technique much used in physics and engineering.[nb_14][78]
The underlying vector space is usually the Hilbert_space L2(0, 2Ï), for which
the functions sin mx and cos mx (m an integer) form an orthogonal basis.[79]
The Fourier_expansion of an L2 function f is
            a  0   2   +  &#x2211;  m = 1   &#x221E;    [   a  m   cos &#x2061;
      (  m x  )  +  b  m   sin &#x2061;  (  m x  )   ]  .   {\displaystyle
      {\frac {a_{0}}{2}}+\sum _{m=1}^{\infty }\left[a_{m}\cos \left
      (mx\right)+b_{m}\sin \left(mx\right)\right].}  [{\frac {a_{0}}{2}}+\sum _
      {m=1}^{\infty }\left[a_{m}\cos \left(mx\right)+b_{m}\sin \left
      (mx\right)\right].]
The coefficients am and bm are called Fourier_coefficients of f, and are
calculated by the formulas[80]
          a  m   =   1 &#x03C0;    &#x222B;  0   2 &#x03C0;   f ( t ) cos
      &#x2061; ( m t )  d t   {\displaystyle a_{m}={\frac {1}{\pi }}\int _{0}^
      {2\pi }f(t)\cos(mt)\,dt}  [a_{m}={\frac {1}{\pi }}\int _{0}^{2\pi }f
      (t)\cos(mt)\,dt],      b  m   =   1 &#x03C0;    &#x222B;  0   2 &#x03C0;
      f ( t ) sin &#x2061; ( m t )  d t .   {\displaystyle b_{m}={\frac {1}{\pi
      }}\int _{0}^{2\pi }f(t)\sin(mt)\,dt.}  [b_{m}={\frac {1}{\pi }}\int _{0}^
      {2\pi }f(t)\sin(mt)\,dt.]
In physical terms the function is represented as a superposition of sine_waves
and the coefficients give information about the function's frequency_spectrum.
[81] A complex-number form of Fourier series is also commonly used.[80] The
concrete formulae above are consequences of a more general mathematical_duality
called Pontryagin_duality.[82] Applied to the group R, it yields the classical
Fourier transform; an application in physics are reciprocal_lattices, where the
underlying group is a finite-dimensional real vector space endowed with the
additional datum of a lattice encoding positions of atoms in crystals.[83]
Fourier series are used to solve boundary_value_problems in partial
differential_equations.[84] In 1822, Fourier first used this technique to solve
the heat_equation.[85] A discrete version of the Fourier series can be used in
sampling applications where the function value is known only at a finite number
of equally spaced points. In this case the Fourier series is finite and its
value is equal to the sampled values at all points.[86] The set of coefficients
is known as the discrete_Fourier_transform (DFT) of the given sample sequence.
The DFT is one of the key tools of digital_signal_processing, a field whose
applications include radar, speech_encoding, image_compression.[87] The JPEG
image format is an application of the closely related discrete_cosine
transform.[88]
The fast_Fourier_transform is an algorithm for rapidly computing the discrete
Fourier transform.[89] It is used not only for calculating the Fourier
coefficients but, using the convolution_theorem, also for computing the
convolution of two finite sequences.[90] They in turn are applied in digital
filters[91] and as a rapid multiplication_algorithm for polynomials and large
integers (SchÃ¶nhageâStrassen_algorithm).[92][93]
**** Differential geometry[edit] ****
Main article: Tangent_space
The tangent space to the 2-sphere at some point is the infinite plane touching
the sphere in this point.
The tangent_plane to a surface at a point is naturally a vector space whose
origin is identified with the point of contact. The tangent plane is the best
linear_approximation, or linearization, of a surface at a point.[nb_15] Even in
a three-dimensional Euclidean space, there is typically no natural way to
prescribe a basis of the tangent plane, and so it is conceived of as an
abstract vector space rather than a real coordinate space. The tangent space is
the generalization to higher-dimensional differentiable_manifolds.[94]
Riemannian_manifolds are manifolds whose tangent spaces are endowed with a
suitable_inner_product.[95] Derived therefrom, the Riemann_curvature_tensor
encodes all curvatures of a manifold in one object, which finds applications in
general_relativity, for example, where the Einstein_curvature_tensor describes
the matter and energy content of space-time.[96][97] The tangent space of a Lie
group can be given naturally the structure of a Lie algebra and can be used to
classify compact_Lie_groups.[98]
***** Generalizations[edit] *****
**** Vector bundles[edit] ****
Main articles: Vector_bundle and Tangent_bundle
A MÃ¶bius strip. Locally, it looks_like U Ã R.
A vector bundle is a family of vector spaces parametrized continuously by a
topological_space X.[94] More precisely, a vector bundle over X is a
topological space E equipped with a continuous map
      Ï : E â X
such that for every x in X, the fiber Ïâ1(x) is a vector space. The case dim
V = 1 is called a line_bundle. For any vector space V, the projection X Ã V
â X makes the product X Ã V into a "trivial"_vector_bundle. Vector bundles
over X are required to be locally a product of X and some (fixed) vector space
V: for every x in X, there is a neighborhood U of x such that the restriction
of Ï to Ïâ1(U) is isomorphic[nb_16] to the trivial bundle U Ã V â U.
Despite their locally trivial character, vector bundles may (depending on the
shape of the underlying space X) be "twisted" in the large (i.e., the bundle
need not be (globally isomorphic to) the trivial bundle X Ã V). For example,
the MÃ¶bius_strip can be seen as a line bundle over the circle S1 (by
identifying_open_intervals_with_the_real_line). It is, however, different from
the cylinder S1 Ã R, because the latter is orientable whereas the former is
not.[99]
Properties of certain vector bundles provide information about the underlying
topological space. For example, the tangent_bundle consists of the collection
of tangent_spaces parametrized by the points of a differentiable manifold. The
tangent bundle of the circle S1 is globally isomorphic to S1 Ã R, since there
is a global nonzero vector_field on S1.[nb_17] In contrast, by the hairy_ball
theorem, there is no (tangent) vector field on the 2-sphere S2 which is
everywhere nonzero.[100] K-theory studies the isomorphism classes of all vector
bundles over some topological space.[101] In addition to deepening topological
and geometrical insight, it has purely algebraic consequences, such as the
classification of finite-dimensional real division_algebras: R, C, the
quaternions H and the octonions O.
The cotangent_bundle of a differentiable manifold consists, at every point of
the manifold, of the dual of the tangent space, the cotangent_space. Sections
of that bundle are known as differential_one-forms.
**** Modules[edit] ****
Main article: Module
Modules are to rings what vector spaces are to fields: the same axioms, applied
to a ring R instead of a field F, yield modules.[102] The theory of modules,
compared to that of vector spaces, is complicated by the presence of ring
elements that do not have multiplicative_inverses. For example, modules need
not have bases, as the Z-module (i.e., abelian_group) Z/2Z shows; those modules
that do (including all vector spaces) are known as free_modules. Nevertheless,
a vector space can be compactly defined as a module over a ring which is a
field with the elements being called vectors. Some authors use the term vector
space to mean modules over a division_ring.[103] The algebro-geometric
interpretation of commutative rings via their spectrum allows the development
of concepts such as locally_free_modules, the algebraic counterpart to vector
bundles.
**** Affine and projective spaces[edit] ****
Main articles: Affine_space and Projective_space
An affine_plane (light blue) in R3. It is a two-dimensional subspace shifted by
a vector x (red).
Roughly, affine spaces are vector spaces whose origins are not specified.[104]
More precisely, an affine space is a set with a free_transitive vector space
action. In particular, a vector space is an affine space over itself, by the
map
      V Ã V â V, (v, a) â¦ a + v.
If W is a vector space, then an affine subspace is a subset of W obtained by
translating a linear subspace V by a fixed vector x â W; this space is
denoted by x + V (it is a coset of V in W) and consists of all vectors of the
form x + v for v â V. An important example is the space of solutions of a
system of inhomogeneous linear equations
      Ax = b
generalizing the homogeneous case b = 0 above.[clarification_needed][105] The
space of solutions is the affine subspace x + V where x is a particular
solution of the equation, and V is the space of solutions of the homogeneous
equation (the nullspace of A).
The set of one-dimensional subspaces of a fixed finite-dimensional vector space
V is known as projective space; it may be used to formalize the idea of
parallel lines intersecting at infinity.[106] Grassmannians and flag_manifolds
generalize this by parametrizing linear subspaces of fixed dimension k and
flags of subspaces, respectively.
***** See also[edit] *****
    * Vector_(mathematics_and_physics), for a list of various kinds of vectors
    * Cartesian
      coordinate_system                                      * Space_
    * Euclidean_vector,     * Metric_space                     (mathematics)
      for vectors in        * P-vector                       * Ordered_vector
      physics               * RieszâFischer_theorem       space
    * Graded_vector
      space
***** Notes[edit] *****
   1. ^ It is also common, especially in physics, to denote vectors with an
      arrow on top: vâ.
   2. ^ This axiom and the next refer to two different operations: scalar
      multiplication: bv; and field multiplication: ab. They do not assert the
      associativity of either operation. More formally, scalar multiplication
      is a monoid_action of the multiplicative monoid of the field F on the
      vector space V.
   3. ^ Some authors (such as Brown 1991) restrict attention to the fields R or
      C, but most of the theory is unchanged for an arbitrary field.
   4. ^ The indicator_functions of intervals (of which there are infinitely
      many) are linearly independent, for example.
   5. ^ The nomenclature derives from German "eigen", which means own or
      proper.
   6. ^  See also JordanâChevalley_decomposition.
   7. ^ This is typically the case when a vector space is also considered as an
      affine_space. In this case, a linear subspace contains the zero_vector,
      while an affine subspace does not necessarily contain it.
   8. ^ Some authors (such as Roman 2005) choose to start with this equivalence
      relation and derive the concrete shape of V/W from this.
   9. ^ This requirement implies that the topology gives rise to a uniform
      structure, Bourbaki 1989, ch. II
  10. ^  The triangle_inequality for       &#x2016;  f + g  &#x2016;   p
      &#x2264;   &#x2016;  f  &#x2016;   p   +   &#x2016;  g  &#x2016;   p
      {\displaystyle \left\Vert {f+g}\right\Vert _{p}\leq \left\Vert
      {f}\right\Vert _{p}+\left\Vert {g}\right\Vert _{p}}  [{\displaystyle
      \left\Vert {f+g}\right\Vert _{p}\leq \left\Vert {f}\right\Vert _
      {p}+\left\Vert {g}\right\Vert _{p}}] is provided by the Minkowski
      inequality. For technical reasons, in the context of functions one has to
      identify functions that agree almost_everywhere to get a norm, and not
      only a seminorm.
  11. ^  "Many functions in      L  2     {\displaystyle L^{2}}  [L^{{2}}] of
      Lebesgue measure, being unbounded, cannot be integrated with the
      classical Riemann integral. So spaces of Riemann integrable functions
      would not be complete in the      L  2     {\displaystyle L^{2}}  [L^{
      {2}}] norm, and the orthogonal decomposition would not apply to them.
      This shows one of the advantages of Lebesgue integration.",
      Dudley 1989, Â§5.3, p. 125
  12. ^ For p â 2, Lp(Î©) is not a Hilbert space.
  13. ^ A basis of a Hilbert space is not the same thing as a basis in the
      sense of linear algebra above.[clarification_needed] For distinction, the
      latter is then called a Hamel_basis.
  14. ^ Although the Fourier series is periodic, the technique can be applied
      to any L2 function on an interval by considering the function to be
      continued periodically outside the interval. See Kreyszig 1988, p. 601
  15. ^ That is to say (BSE-3_2001), the plane passing through the point of
      contact P such that the distance from a point P1 on the surface to the
      plane is infinitesimally_small compared to the distance from P1 to P in
      the limit as P1 approaches P along the surface.
  16. ^ That is, there is a homeomorphism from Ïâ1(U) to V Ã U which
      restricts to linear isomorphisms between fibers.
  17. ^ A line bundle, such as the tangent bundle of S1 is trivial if and only
      if there is a section that vanishes nowhere, see
      Husemoller 1994, Corollary 8.3. The sections of the tangent bundle are
      just vector_fields.
***** Citations[edit] *****
   1. ^ Roman 2005, ch. 1, p. 27
   2. ^ van der Waerden 1993, Ch. 19
   3. ^ Bourbaki 1998, Â§II.1.1. Bourbaki calls the group homomorphisms f(a)
      homotheties.
   4. ^ Bourbaki 1969, ch. "AlgÃ¨bre linÃ©aire et algÃ¨bre multilinÃ©aire", pp.
      78â91
   5. ^ Bolzano 1804
   6. ^ MÃ¶bius 1827
   7. ^Crowe, Michel J. (1994), A History of Vector Analysis: The Evolution of
      the Idea of a Vectorial System, Dover, p. 11 and 16, ISBN 978-0-486-
      67910-5
   8. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   9. ^ Hamilton 1853
  10. ^ Grassmann 1844
  11. ^ Peano 1888, ch. IX
  12. ^ Banach 1922
  13. ^ Dorier 1995, Moore 1995
  14. ^ Lang 1987, ch. I.1
  15. ^ Lang 2002, ch. V.1
  16. ^ e.g. Lang 1993, ch. XII.3., p. 335
  17. ^ Lang 1987, ch. IX.1
  18. ^ Lang 1987, ch. VI.3.
  19. ^ Roman 2005, Theorem 1.9, p. 43
  20. ^ Blass 1984
  21. ^ Halpern 1966, pp. 670â673
  22. ^ Artin 1991, Theorem 3.3.13
  23. ^ Braun 1993, Th. 3.4.5, p. 291
  24. ^ Stewart 1975, Proposition 4.3, p. 52
  25. ^ Stewart 1975, Theorem 6.5, p. 74
  26. ^ Roman 2005, ch. 2, p. 45
  27. ^ Lang 1987, ch. IV.4, Corollary, p. 106
  28. ^ Lang 1987, Example IV.2.6
  29. ^ Lang 1987, ch. VI.6
  30. ^ Halmos 1974, p. 28, Ex. 9
  31. ^ Lang 1987, Theorem IV.2.1, p. 95
  32. ^ Roman 2005, Th. 2.5 and 2.6, p. 49
  33. ^ Lang 1987, ch. V.1
  34. ^ Lang 1987, ch. V.3., Corollary, p. 106
  35. ^ Lang 1987, Theorem VII.9.8, p. 198
  36. ^ Roman 2005, ch. 8, p. 135â156
  37. ^ Lang 1987, ch. IX.4
  38. ^ Roman 2005, ch. 8, p. 140.
  39. ^ Roman 2005, ch. 1, p. 29
  40. ^ Roman 2005, ch. 1, p. 35
  41. ^ Roman 2005, ch. 3, p. 64
  42. ^ Lang 1987, ch. IV.3.
  43. ^ Roman 2005, ch. 2, p. 48
  44. ^ Mac Lane 1998
  45. ^ Roman 2005, ch. 1, pp. 31â32
  46. ^ Lang 2002, ch. XVI.1
  47. ^ Roman 2005, Th. 14.3. See also Yoneda_lemma.
  48. ^ Schaefer & Wolff 1999, pp. 204â205
  49. ^ Bourbaki 2004, ch. 2, p. 48
  50. ^ Roman 2005, ch. 9
  51. ^ Naber 2003, ch. 1.2
  52. ^ Treves 1967
  53. ^ Bourbaki 1987
  54. ^ Kreyszig_1989, Â§4.11-5
  55. ^ Kreyszig_1989, Â§1.5-5
  56. ^ Choquet 1966, Proposition III.7.2
  57. ^ Treves 1967, p. 34â36
  58. ^ Lang 1983, Cor. 4.1.2, p. 69
  59. ^ Treves 1967, ch. 11
  60. ^ Treves 1967, Theorem 11.2, p. 102
  61. ^ Evans 1998, ch. 5
  62. ^ Treves 1967, ch. 12
  63. ^ Dennery 1996, p.190
  64. ^ Lang 1993, Th. XIII.6, p. 349
  65. ^ Lang 1993, Th. III.1.1
  66. ^ Choquet 1966, Lemma III.16.11
  67. ^ Kreyszig 1999, Chapter 11
  68. ^ Griffiths 1995, Chapter 1
  69. ^ Lang 1993, ch. XVII.3
  70. ^ Lang 2002, ch. III.1, p. 121
  71. ^ Eisenbud 1995, ch. 1.6
  72. ^ Varadarajan 1974
  73. ^ Lang 2002, ch. XVI.7
  74. ^ Lang 2002, ch. XVI.8
  75. ^ Luenberger 1997, Â§7.13
  76. ^ See representation_theory and group_representation.
  77. ^ Lang 1993, Ch. XI.1
  78. ^ Evans 1998, Th. 6.2.1
  79. ^ Folland 1992, p. 349 ff
  80. ^ Gasquet & Witomski 1999, p. 150
  81. ^ a b Gasquet & Witomski 1999, Â§4.5
  82. ^ Gasquet & Witomski 1999, p. 57
  83. ^ Loomis 1953, Ch. VII
  84. ^ Ashcroft & Mermin 1976, Ch. 5
  85. ^ Kreyszig 1988, p. 667
  86. ^ Fourier 1822
  87. ^ Gasquet & Witomski 1999, p. 67
  88. ^ Ifeachor & Jervis 2002, pp. 3â4, 11
  89. ^ Wallace Feb_1992
  90. ^ Ifeachor & Jervis 2002, p. 132
  91. ^ Gasquet & Witomski 1999, Â§10.2
  92. ^ Ifeachor & Jervis 2002, pp. 307â310
  93. ^ Gasquet & Witomski 1999, Â§10.3
  94. ^ SchÃ¶nhage & Strassen 1971
  95. ^ a b Spivak 1999, ch. 3
  96. ^ Jost 2005. See also Lorentzian_manifold.
  97. ^ Misner, Thorne & Wheeler 1973, ch. 1.8.7, p. 222 and ch. 2.13.5, p. 325
  98. ^ Jost 2005, ch. 3.1
  99. ^ Varadarajan 1974, ch. 4.3, Theorem 4.3.27
 100. ^ Kreyszig 1991, Â§34, p. 108
 101. ^ Eisenberg & Guy 1979
 102. ^ Atiyah 1989
 103. ^ Artin 1991, ch. 12
 104. ^ Grillet, Pierre Antoine. Abstract algebra. Vol. 242. Springer Science &
      Business Media, 2007.
 105. ^ Meyer 2000, Example 5.13.5, p. 436
 106. ^ Meyer 2000, Exercise 5.13.15â17, p. 442
 107. ^ Coxeter 1987
***** References[edit] *****
**** Algebra[edit] ****
    * Artin,_Michael (1991), Algebra, Prentice_Hall, ISBN 978-0-89871-510-1
Blass, Andreas (1984), "Existence of bases implies the axiom of choice",
Axiomatic set theory (Boulder, Colorado, 1983), Contemporary Mathematics, 31,
Providence, R.I.: American_Mathematical_Society, pp. 31â33, MR 0763890
Brown, William A. (1991), Matrices and vector spaces, New York: M. Dekker,
ISBN 978-0-8247-8419-5
Lang,_Serge (1987), Linear algebra, Berlin, New York: Springer-Verlag,
ISBN 978-0-387-96412-6
Lang,_Serge (2002), Algebra, Graduate_Texts_in_Mathematics, 211 (Revised third
ed.), New York: Springer-Verlag, ISBN 978-0-387-95385-4, MR 1878556
Mac_Lane,_Saunders (1999), Algebra (3rd ed.), pp. 193â222, ISBN 978-0-8218-
1646-2
Meyer, Carl D. (2000), Matrix_Analysis_and_Applied_Linear_Algebra, SIAM,
ISBN 978-0-89871-454-8
Roman, Steven (2005), Advanced Linear Algebra, Graduate Texts in Mathematics,
135 (2nd ed.), Berlin, New York: Springer-Verlag, ISBN 978-0-387-24766-3
Spindler, Karlheinz (1993), Abstract Algebra with Applications: Volume 1:
Vector spaces and groups, CRC, ISBN 978-0-8247-9144-5
van_der_Waerden,_Bartel_Leendert (1993), Algebra (in German) (9th ed.), Berlin,
New York: Springer-Verlag, ISBN 978-3-540-56799-8
**** Analysis[edit] ****
    * Bourbaki,_Nicolas (1987), Topological vector spaces, Elements of
      mathematics, Berlin, New York: Springer-Verlag, ISBN 978-3-540-13627-9
Bourbaki,_Nicolas (2004), Integration I, Berlin, New York: Springer-Verlag,
ISBN 978-3-540-41129-1
Braun, Martin (1993), Differential equations and their applications: an
introduction to applied mathematics, Berlin, New York: Springer-Verlag,
ISBN 978-0-387-97894-9
BSE-3 (2001) [1994], "Tangent_plane", in Hazewinkel,_Michiel (ed.),
Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. / Kluwer
Academic Publishers, ISBN 978-1-55608-010-4
Choquet,_Gustave (1966), Topology, Boston, MA: Academic_Press
Dennery, Philippe; Krzywicki, Andre (1996), Mathematics for Physicists, Courier
Dover Publications, ISBN 978-0-486-69193-0
Dudley, Richard M. (1989), Real analysis and probability, The Wadsworth &
Brooks/Cole Mathematics Series, Pacific Grove, CA: Wadsworth & Brooks/Cole
Advanced Books & Software, ISBN 978-0-534-10050-6
Dunham, William (2005), The Calculus Gallery, Princeton_University_Press,
ISBN 978-0-691-09565-3
Evans, Lawrence C. (1998), Partial differential equations, Providence, R.I.:
American_Mathematical_Society, ISBN 978-0-8218-0772-9
Folland, Gerald B. (1992), Fourier Analysis and Its Applications, Brooks-Cole,
ISBN 978-0-534-17094-3
Gasquet, Claude; Witomski, Patrick (1999), Fourier Analysis and Applications:
Filtering, Numerical Computation, Wavelets, Texts in Applied Mathematics, New
York: Springer-Verlag, ISBN 978-0-387-98485-8
Ifeachor, Emmanuel C.; Jervis, Barrie W. (2001), Digital Signal Processing: A
Practical Approach (2nd ed.), Harlow, Essex, England: Prentice-Hall (published
2002), ISBN 978-0-201-59619-9
Krantz, Steven G. (1999), A Panorama of Harmonic Analysis, Carus Mathematical
Monographs, Washington, DC: Mathematical Association of America, ISBN 978-0-
88385-031-2
Kreyszig,_Erwin (1988), Advanced Engineering Mathematics (6th ed.), New York:
John Wiley & Sons, ISBN 978-0-471-85824-9
Kreyszig,_Erwin (1989), Introductory functional analysis with applications,
Wiley Classics Library, New York: John_Wiley_&_Sons, ISBN 978-0-471-50459-7,
MR 0992618
Lang,_Serge (1983), Real analysis, Addison-Wesley, ISBN 978-0-201-14179-5
Lang,_Serge (1993), Real and functional analysis, Berlin, New York: Springer-
Verlag, ISBN 978-0-387-94001-4
Loomis, Lynn H. (1953), An introduction to abstract harmonic analysis, Toronto-
New YorkâLondon: D. Van Nostrand Company, Inc., pp. x+190
Schaefer,_Helmut_H.; Wolff, M.P. (1999), Topological vector spaces (2nd ed.),
Berlin, New York: Springer-Verlag, ISBN 978-0-387-98726-2
Treves, FranÃ§ois (1967), Topological vector spaces, distributions and kernels,
Boston, MA: Academic_Press
**** Historical references[edit] ****
    * Banach,_Stefan (1922), "Sur_les_opÃ©rations_dans_les_ensembles_abstraits
      et_leur_application_aux_Ã©quations_intÃ©grales_(On_operations_in_abstract
      sets_and_their_application_to_integral_equations)" (PDF), Fundamenta
      Mathematicae (in French), 3: 133â181, doi:10.4064/fm-3-1-133-181,
      ISSN 0016-2736
Bolzano,_Bernard (1804), Betrachtungen_Ã¼ber_einige_GegenstÃ¤nde_der
Elementargeometrie_(Considerations_of_some_aspects_of_elementary_geometry) (in
German)
Bourbaki,_Nicolas (1969), ÃlÃ©ments d'histoire des mathÃ©matiques (Elements of
history of mathematics) (in French), Paris: Hermann
Dorier, Jean-Luc (1995), "A_general_outline_of_the_genesis_of_vector_space
theory", Historia_Mathematica, 22 (3): 227â261, doi:10.1006/hmat.1995.1024,
MR 1347828
Fourier,_Jean_Baptiste_Joseph (1822), ThÃ©orie_analytique_de_la_chaleur (in
French), Chez Firmin Didot, pÃ¨re et fils
Grassmann,_Hermann (1844), Die_Lineale_Ausdehnungslehre_-_Ein_neuer_Zweig_der
Mathematik (in German), O. Wigand
, reprint:Hermann Grassmann. Translated by Lloyd C. Kannenberg. (2000),
Kannenberg, L.C. (ed.), Extension Theory, Providence, R.I.: American
Mathematical_Society, ISBN 978-0-8218-2031-5
Hamilton,_William_Rowan (1853), Lectures_on_Quaternions, Royal Irish Academy
MÃ¶bius,_August_Ferdinand (1827), Der_Barycentrische_Calcul :_ein_neues
HÃ¼lfsmittel_zur_analytischen_Behandlung_der_Geometrie_(Barycentric_calculus:_a
new_utility_for_an_analytic_treatment_of_geometry) (in German), archived from
the_original on 2006-11-23
Moore, Gregory H. (1995), "The axiomatization of linear algebra: 1875â1940",
Historia_Mathematica, 22 (3): 262â303, doi:10.1006/hmat.1995.1025
Peano,_Giuseppe (1888), Calcolo Geometrico secondo l'Ausdehnungslehre di H.
Grassmann preceduto dalle Operazioni della Logica Deduttiva (in Italian), Turin
**** Further references[edit] ****
    * Ashcroft,_Neil; Mermin,_N._David (1976), Solid State Physics, Toronto:
      Thomson Learning, ISBN 978-0-03-083993-1
Atiyah,_Michael_Francis (1989), K-theory, Advanced Book Classics (2nd ed.),
Addison-Wesley, ISBN 978-0-201-09394-0, MR 1043170
Bourbaki,_Nicolas (1998), Elements of Mathematics : Algebra I Chapters 1-3,
Berlin, New York: Springer-Verlag, ISBN 978-3-540-64243-5
Bourbaki,_Nicolas (1989), General Topology. Chapters 1-4, Berlin, New York:
Springer-Verlag, ISBN 978-3-540-64241-1
Coxeter,_Harold_Scott_MacDonald (1987), Projective Geometry (2nd ed.), Berlin,
New York: Springer-Verlag, ISBN 978-0-387-96532-1
Eisenberg, Murray; Guy, Robert (1979), "A proof of the hairy ball theorem", The
American_Mathematical_Monthly, 86 (7): 572â574, doi:10.2307/2320587,
JSTOR 2320587
Eisenbud,_David (1995), Commutative algebra, Graduate Texts in Mathematics,
150, Berlin, New York: Springer-Verlag, ISBN 978-0-387-94269-8, MR 1322960
Goldrei, Derek (1996), Classic Set Theory: A guided independent study (1st
ed.), London: Chapman_and_Hall, ISBN 978-0-412-60610-6
Griffiths,_David_J. (1995), Introduction to Quantum Mechanics, Upper Saddle
River, NJ: Prentice_Hall, ISBN 978-0-13-124405-4
Halmos,_Paul_R. (1974), Finite-dimensional vector spaces, Berlin, New York:
Springer-Verlag, ISBN 978-0-387-90093-3
Halpern, James D. (Jun 1966), "Bases in Vector Spaces and the Axiom of Choice",
Proceedings_of_the_American_Mathematical_Society, 17 (3): 670â673, doi:
10.2307/2035388, JSTOR 2035388
Hughes-Hallett, Deborah; McCallum, William G.; Gleason, Andrew M. (2013),
Calculus : Single and Multivariable (6 ed.), John_Wiley_&_Sons, ISBN 978-0470-
88861-2
Husemoller, Dale (1994), Fibre Bundles (3rd ed.), Berlin, New York: Springer-
Verlag, ISBN 978-0-387-94087-8
Jost, JÃ¼rgen (2005), Riemannian Geometry and Geometric Analysis (4th ed.),
Berlin, New York: Springer-Verlag, ISBN 978-3-540-25907-7
Kreyszig,_Erwin (1991), Differential geometry, New York: Dover_Publications,
pp. xiv+352, ISBN 978-0-486-66721-8
Kreyszig, Erwin (1999), Advanced Engineering Mathematics (8th ed.), New York:
John_Wiley_&_Sons, ISBN 978-0-471-15496-9
Luenberger, David (1997), Optimization by vector space methods, New York: John
Wiley_&_Sons, ISBN 978-0-471-18117-0
Mac_Lane,_Saunders (1998), Categories_for_the_Working_Mathematician (2nd ed.),
Berlin, New York: Springer-Verlag, ISBN 978-0-387-98403-2
Misner,_Charles_W.; Thorne,_Kip; Wheeler,_John_Archibald (1973), Gravitation,
W. H. Freeman, ISBN 978-0-7167-0344-0
Naber, Gregory L. (2003), The geometry of Minkowski spacetime, New York: Dover
Publications, ISBN 978-0-486-43235-9, MR 2044239
SchÃ¶nhage,_A.; Strassen,_Volker (1971), "Schnelle Multiplikation groÃer
Zahlen (Fast multiplication of big numbers)", Computing (in German), 7 (3â4):
281â292, doi:10.1007/bf02242355, ISSN 0010-485X
Spivak,_Michael (1999), A Comprehensive Introduction to Differential Geometry
(Volume Two), Houston, TX: Publish or Perish
Stewart,_Ian (1975), Galois Theory, Chapman_and_Hall Mathematics Series,
London: Chapman_and_Hall, ISBN 978-0-412-10800-6
Varadarajan, V. S. (1974), Lie groups, Lie algebras, and their representations,
Prentice_Hall, ISBN 978-0-13-535732-3
Wallace, G.K. (Feb 1992), "The_JPEG_still_picture_compression_standard" (PDF),
IEEE Transactions on Consumer Electronics, 38 (1): xviiiâxxxiv,
CiteSeerX 10.1.1.318.4292, doi:10.1109/30.125072, ISSN 0098-3063
Weibel,_Charles_A. (1994). An introduction to homological algebra. Cambridge
Studies in Advanced Mathematics. 38. Cambridge University Press. ISBN 978-0-
521-55987-4. MR 1269324. OCLC 36131259.
***** External links[edit] *****
 The Wikibook Linear_Algebra has a page on the topic of: Real_vector_spaces
 The Wikibook Linear_Algebra has a page on the topic of: Vector_spaces
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Vector_space", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
    * v
    * t
    * e
Linear_algebra
                            * Scalar
                            * Vector
                            * Vector space
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
index.php?title=Vector_space&oldid=902198844"
Categories:
    * Concepts_in_physics
    * Group_theory
    * Mathematical_structures
    * Vectors_(mathematics_and_physics)
    * Vector_spaces
Hidden categories:
    * Wikipedia_articles_needing_clarification_from_February_2019
    * Articles_with_short_description
    * CS1_German-language_sources_(de)
    * CS1_French-language_sources_(fr)
    * CS1_Italian-language_sources_(it)
    * Good_articles
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐ°ÑÒ¡Ð¾ÑÑÑÐ°
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
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
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Interlingua
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * àº¥àº²àº§
    * Latina
    * LatvieÅ¡u
    * LietuviÅ³
    * Lumbaart
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Occitan
    * à¨ªà©°à¨à¨¾à¨¬à©
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
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
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * VÃ¨neto
    * Tiáº¿ng_Viá»t
    * æè¨
    * å´è¯­
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 17 June 2019, at 08:00 (UTC).
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
