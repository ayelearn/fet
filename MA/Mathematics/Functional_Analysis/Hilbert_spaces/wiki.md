The following text has been accessed from https://en.wikipedia.org/wiki/Hilbert_space at Fri Aug 9 02:39:00 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















[This_is_a_good_article._Follow_the_link_for_more_information.]
****** Hilbert space ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
inner product space that is metrically complete; a Banach space whose norm
induces an inner product (follows the parallelogram identity)
For the Hilbert space-filling curve, see Hilbert_curve.
The state of a vibrating_string can be modeled as a point in a Hilbert space.
The decomposition of a vibrating string into its vibrations in distinct
overtones is given by the projection of the point onto the coordinate axes in
the space.
The mathematical concept of a Hilbert space, named after David_Hilbert,
generalizes the notion of Euclidean_space. It extends the methods of vector
algebra and calculus from the two-dimensional Euclidean_plane and three-
dimensional space to spaces with any finite or infinite number of dimensions. A
Hilbert space is an abstract vector_space possessing the structure of an inner
product that allows length and angle to be measured. Furthermore, Hilbert
spaces are complete: there are enough limits in the space to allow the
techniques of calculus to be used.
Hilbert spaces arise naturally and frequently in mathematics and physics,
typically as infinite-dimensional function_spaces. The earliest Hilbert spaces
were studied from this point of view in the first decade of the 20th century by
David_Hilbert, Erhard_Schmidt, and Frigyes_Riesz. They are indispensable tools
in the theories of partial_differential_equations, quantum_mechanics, Fourier
analysis (which includes applications to signal_processing and heat transfer),
and ergodic_theory (which forms the mathematical underpinning of
thermodynamics). John_von_Neumann coined the term Hilbert space for the
abstract concept that underlies many of these diverse applications. The success
of Hilbert space methods ushered in a very fruitful era for functional
analysis. Apart from the classical Euclidean spaces, examples of Hilbert spaces
include spaces_of_square-integrable_functions, spaces_of_sequences, Sobolev
spaces consisting of generalized_functions, and Hardy_spaces of holomorphic
functions.
Geometric intuition plays an important role in many aspects of Hilbert space
theory. Exact analogs of the Pythagorean_theorem and parallelogram_law hold in
a Hilbert space. At a deeper level, perpendicular projection onto a subspace
(the analog of "dropping_the_altitude" of a triangle) plays a significant role
in optimization problems and other aspects of the theory. An element of a
Hilbert space can be uniquely specified by its coordinates with respect to a
set of coordinate_axes (an orthonormal_basis), in analogy with Cartesian
coordinates in the plane. When that set of axes is countably_infinite, the
Hilbert space can also be usefully thought of in terms of the space of infinite
sequences that are square-summable. The latter space is often in the older
literature referred to as the Hilbert space. Linear_operators on a Hilbert
space are likewise fairly concrete objects: in good cases, they are simply
transformations that stretch the space by different factors in mutually
perpendicular directions in a sense that is made precise by the study of their
spectrum.
⁰
***** Contents *****
    * 1_Definition_and_illustration
          o 1.1_Motivating_example:_Euclidean_space
          o 1.2_Definition
          o 1.3_Second_example:_sequence_spaces
    * 2_History
    * 3_Examples
          o 3.1_Lebesgue_spaces
          o 3.2_Sobolev_spaces
          o 3.3_Spaces_of_holomorphic_functions
                # 3.3.1_Hardy_spaces
                # 3.3.2_Bergman_spaces
    * 4_Applications
          o 4.1_SturmâLiouville_theory
          o 4.2_Partial_differential_equations
          o 4.3_Ergodic_theory
          o 4.4_Fourier_analysis
          o 4.5_Quantum_mechanics
          o 4.6_Color_perception
    * 5_Properties
          o 5.1_Pythagorean_identity
          o 5.2_Parallelogram_identity_and_polarization
          o 5.3_Best_approximation
          o 5.4_Duality
          o 5.5_Weakly-convergent_sequences
          o 5.6_Banach_space_properties
    * 6_Operators_on_Hilbert_spaces
          o 6.1_Bounded_operators
          o 6.2_Unbounded_operators
    * 7_Constructions
          o 7.1_Direct_sums
          o 7.2_Tensor_products
    * 8_Orthonormal_bases
          o 8.1_Sequence_spaces
          o 8.2_Bessel's_inequality_and_Parseval's_formula
          o 8.3_Hilbert_dimension
          o 8.4_Separable_spaces
    * 9_Orthogonal_complements_and_projections
    * 10_Spectral_theory
    * 11_In_popular_culture
    * 12_See_also
    * 13_Remarks
    * 14_Notes
    * 15_References
    * 16_External_links
***** Definition and illustration[edit] *****
**** Motivating example: Euclidean space[edit] ****
One of the most familiar examples of a Hilbert space is the Euclidean_space
consisting of three-dimensional vectors, denoted by â3, and equipped with the
dot_product. The dot product takes two vectors x and y, and produces a real
number x Â· y. If x and y are represented in Cartesian_coordinates, then the
dot product is defined by
           (     x  1        x  2        x  3      )   &#x22C5;   (     y  1
      y  2        y  3      )   =  x  1    y  1   +  x  2    y  2   +  x  3
      y  3    .   {\displaystyle {\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end
      {pmatrix}}\cdot {\begin{pmatrix}y_{1}\\y_{2}\\y_{3}\end{pmatrix}}=x_{1}y_
      {1}+x_{2}y_{2}+x_{3}y_{3}\,.}  [{\displaystyle {\begin{pmatrix}x_{1}\\x_
      {2}\\x_{3}\end{pmatrix}}\cdot {\begin{pmatrix}y_{1}\\y_{2}\\y_{3}\end
      {pmatrix}}=x_{1}y_{1}+x_{2}y_{2}+x_{3}y_{3}\,.}]
The dot product satisfies the properties:
   1. It is symmetric in x and y: x Â· y = y Â· x.
   2. It is linear in its first argument: (ax1 + bx2) Â· y = ax1 Â· y + bx2 Â·
      y for any scalars a, b, and vectors x1, x2, and y.
   3. It is positive_definite: for all vectors x, x Â· x â¥ 0 , with equality
      if_and_only_if  x = 0.
An operation on pairs of vectors that, like the dot product, satisfies these
three properties is known as a (real) inner_product. A vector_space equipped
with such an inner product is known as a (real) inner_product_space. Every
finite-dimensional inner product space is also a Hilbert space. The basic
feature of the dot product that connects it with Euclidean geometry is that it
is related to both the length (or norm) of a vector, denoted ||x||, and to the
angle Î¸ between two vectors x and y by means of the formula
          x  &#x22C5;  y  = &#x2016;  x  &#x2016;  &#x2016;  y  &#x2016;  cos
      &#x2061; &#x03B8;  .   {\displaystyle \mathbf {x} \cdot \mathbf {y}
      =\|\mathbf {x} \|\,\|\mathbf {y} \|\,\cos \theta \,.}  [{\displaystyle
      \mathbf {x} \cdot \mathbf {y} =\|\mathbf {x} \|\,\|\mathbf {y} \|\,\cos
      \theta \,.}]
Completeness means that if a particle moves along the broken path (in blue)
travelling a finite total distance, then the particle has a well-defined net
displacement (in orange).
Multivariable_calculus in Euclidean space relies on the ability to compute
limits, and to have useful criteria for concluding that limits exist. A
mathematical_series
          &#x2211;  n = 0   &#x221E;     x   n     {\displaystyle \sum _{n=0}^
      {\infty }\mathbf {x} _{n}}  [\sum _{n=0}^{\infty }\mathbf {x} _{n}]
consisting of vectors in â3 is absolutely_convergent provided that the sum of
the lengths converges as an ordinary series of real numbers:[1]
          &#x2211;  k = 0   &#x221E;   &#x2016;   x   k   &#x2016; < &#x221E;
      .   {\displaystyle \sum _{k=0}^{\infty }\|\mathbf {x} _{k}\|<\infty \,.}
      [{\displaystyle \sum _{k=0}^{\infty }\|\mathbf {x} _{k}\|<\infty \,.}]
Just as with a series of scalars, a series of vectors that converges absolutely
also converges to some limit vector L in the Euclidean space, in the sense that
          &#x2016;   L  &#x2212;  &#x2211;  k = 0   N     x   k    &#x2016;
      &#x2192; 0   as&#xA0;  N &#x2192; &#x221E;  .   {\displaystyle
      \left\|\mathbf {L} -\sum _{k=0}^{N}\mathbf {x} _{k}\right\|\to 0\quad
      {\text{as }}N\to \infty \,.}  [{\displaystyle \left\|\mathbf {L} -\sum _
      {k=0}^{N}\mathbf {x} _{k}\right\|\to 0\quad {\text{as }}N\to \infty \,.}]
This property expresses the completeness of Euclidean space: that a series that
converges absolutely also converges in the ordinary sense.
Hilbert spaces are often taken over the complex_numbers. The complex_plane
denoted by â is equipped with a notion of magnitude, the complex_modulus |z|
which is defined as the square root of the product of z with its complex
conjugate:
          |  z   |   2   = z   z &#x00AF;    .   {\displaystyle |z|^{2}=z
      {\overline {z}}\,.}  [{\displaystyle |z|^{2}=z{\overline {z}}\,.}]
If z = x + iy is a decomposition of z into its real and imaginary parts, then
the modulus is the usual Euclidean two-dimensional length:
          |  z  |  =    x  2   +  y  2      .   {\displaystyle |z|={\sqrt {x^
      {2}+y^{2}}}\,.}  [{\displaystyle |z|={\sqrt {x^{2}+y^{2}}}\,.}]
The inner product of a pair of complex numbers z and w is the product of z with
the complex conjugate of w:
         &#x27E8; z , w &#x27E9; = z   w &#x00AF;    .   {\displaystyle \langle
      z,w\rangle =z{\overline {w}}\,.}  [{\displaystyle \langle z,w\rangle =z
      {\overline {w}}\,.}]
This is complex-valued. The real part of &#x27e8;z, w&#x27e9; gives the usual
two-dimensional Euclidean dot_product.
A second example is the space â2 whose elements are pairs of complex numbers
z = (z1, z2). Then the inner product of z with another such vector w = (w1, w2)
is given by
         &#x27E8; z , w &#x27E9; =  z  1      w &#x00AF;    1   +  z  2      w
      &#x00AF;    2    .   {\displaystyle \langle z,w\rangle =z_{1}{\overline
      {w}}_{1}+z_{2}{\overline {w}}_{2}\,.}  [{\displaystyle \langle z,w\rangle
      =z_{1}{\overline {w}}_{1}+z_{2}{\overline {w}}_{2}\,.}]
The real part of &#x27e8;z, w&#x27e9; is then the four-dimensional Euclidean
dot product. This inner product is Hermitian symmetric, which means that the
result of interchanging z and w is the complex conjugate:
         &#x27E8; w , z &#x27E9; =    &#x27E8; z , w &#x27E9;  &#x00AF;    .
      {\displaystyle \langle w,z\rangle ={\overline {\langle z,w\rangle }}\,.}
      [{\displaystyle \langle w,z\rangle ={\overline {\langle z,w\rangle
      }}\,.}]
**** Definition[edit] ****
A Hilbert space H is a real or complex inner_product_space that is also a
complete_metric_space with respect to the distance function induced by the
inner product.[2]
To say that H is a complex inner product space means that H is a complex vector
space on which there is an inner product &#x27e8;x, y&#x27e9; associating a
complex number to each pair of elements x, y of H that satisfies the following
properties:
   1. The inner product is conjugate symmetric; that is, the inner product of a
      pair of elements is equal to the complex_conjugate of the inner product
      of the swapped elements:
               &#x27E8; y , x &#x27E9; =    &#x27E8; x , y &#x27E9;  &#x00AF;
            .   {\displaystyle \langle y,x\rangle ={\overline {\langle
            x,y\rangle }}\,.}  [{\displaystyle \langle y,x\rangle ={\overline
            {\langle x,y\rangle }}\,.}]
   2. The inner product is linear in its first[nb_1] argument. For all complex
      numbers a and b,
               &#x27E8; a  x  1   + b  x  2   , y &#x27E9; = a &#x27E8;  x  1
            , y &#x27E9; + b &#x27E8;  x  2   , y &#x27E9;  .   {\displaystyle
            \langle ax_{1}+bx_{2},y\rangle =a\langle x_{1},y\rangle +b\langle
            x_{2},y\rangle \,.}  [{\displaystyle \langle ax_{1}+bx_{2},y\rangle
            =a\langle x_{1},y\rangle +b\langle x_{2},y\rangle \,.}]
   3. The inner product of an element with itself is positive_definite:
                 {    &#x27E8; x , x &#x27E9; > 0   x &#x2260; 0     &#x27E8; x
            , x &#x27E9; = 0   x = 0  .         {\displaystyle {\begin
            {cases}\langle x,x\rangle >0&x\neq 0\\\langle x,x\rangle
            =0&x=0\,.\end{cases}}}  [{\displaystyle {\begin{cases}\langle
            x,x\rangle >0&x\neq 0\\\langle x,x\rangle =0&x=0\,.\end{cases}}}]
It follows from properties 1 and 2 that a complex inner product is conjugate
linear in its second argument, meaning that
         &#x27E8; x , a  y  1   + b  y  2   &#x27E9; =    a &#x00AF;
      &#x27E8; x ,  y  1   &#x27E9; +    b &#x00AF;    &#x27E8; x ,  y  2
      &#x27E9;  .   {\displaystyle \langle x,ay_{1}+by_{2}\rangle ={\bar
      {a}}\langle x,y_{1}\rangle +{\bar {b}}\langle x,y_{2}\rangle \,.}  [
      {\displaystyle \langle x,ay_{1}+by_{2}\rangle ={\bar {a}}\langle x,y_
      {1}\rangle +{\bar {b}}\langle x,y_{2}\rangle \,.}]
A real inner product space is defined in the same way, except that H is a real
vector space and the inner product takes real values. Such an inner product
will be bilinear: that is, linear in each argument.
The norm is the real-valued function
         &#x2016; x &#x2016; =   &#x27E8; x , x &#x27E9;    ,   {\displaystyle
      \|x\|={\sqrt {\langle x,x\rangle }}\,,}  [{\displaystyle \|x\|={\sqrt
      {\langle x,x\rangle }}\,,}]
and the distance d between two points x, y in H is defined in terms of the norm
by
         d ( x , y ) = &#x2016; x &#x2212; y &#x2016; =   &#x27E8; x &#x2212; y
      , x &#x2212; y &#x27E9;    .   {\displaystyle d(x,y)=\|x-y\|={\sqrt
      {\langle x-y,x-y\rangle }}\,.}  [{\displaystyle d(x,y)=\|x-y\|={\sqrt
      {\langle x-y,x-y\rangle }}\,.}]
That this function is a distance function means firstly that it is symmetric in
x and y, secondly that the distance between x and itself is zero, and otherwise
the distance between x and y must be positive, and lastly that the triangle
inequality holds, meaning that the length of one leg of a triangle xyz cannot
exceed the sum of the lengths of the other two legs:
         d ( x , z ) &#x2264; d ( x , y ) + d ( y , z )  .   {\displaystyle d
      (x,z)\leq d(x,y)+d(y,z)\,.}  [{\displaystyle d(x,z)\leq d(x,y)+d
      (y,z)\,.}]
      [Triangle_inequality_in_a_metric_space.svg]
This last property is ultimately a consequence of the more fundamental
CauchyâSchwarz_inequality, which asserts
           |   &#x27E8; x , y &#x27E9;   |   &#x2264; &#x2016; x &#x2016;
      &#x2016; y &#x2016;   {\displaystyle {\bigl |}\langle x,y\rangle {\bigr
      |}\leq \|x\|\,\|y\|}  [{\displaystyle {\bigl |}\langle x,y\rangle {\bigr
      |}\leq \|x\|\,\|y\|}]
with equality if and only if x and y are linearly_dependent.
With a distance function defined in this way, any inner product space is a
metric_space, and sometimes is known as a pre-Hilbert space.[3] Any pre-Hilbert
space that is additionally also a complete space is a Hilbert space.
The completeness of H is expressed using a form of the Cauchy_criterion for
sequences in H: a pre-Hilbert space H is complete if every Cauchy_sequence
converges_with_respect_to_this_norm to an element in the space. Completeness
can be characterized by the following equivalent condition: if a series of
vectors
          &#x2211;  k = 0   &#x221E;    u  k     {\displaystyle \sum _{k=0}^
      {\infty }u_{k}}  [{\displaystyle \sum _{k=0}^{\infty }u_{k}}]
converges_absolutely in the sense that
          &#x2211;  k = 0   &#x221E;   &#x2016;  u  k   &#x2016; < &#x221E;  ,
      {\displaystyle \sum _{k=0}^{\infty }\|u_{k}\|<\infty \,,}  [
      {\displaystyle \sum _{k=0}^{\infty }\|u_{k}\|<\infty \,,}]
then the series converges in H, in the sense that the partial sums converge to
an element of H.
As a complete normed space, Hilbert spaces are by definition also Banach
spaces. As such they are topological_vector_spaces, in which topological
notions like the openness and closedness of subsets are well defined. Of
special importance is the notion of a closed linear_subspace of a Hilbert space
that, with the inner product induced by restriction, is also complete (being a
closed set in a complete metric space) and therefore a Hilbert space in its own
right.
**** Second example: sequence spaces[edit] ****
The sequence_space l2 consists of all infinite_sequences z = (z1, z2, â¦) of
complex numbers such that the series
          &#x2211;  n = 1   &#x221E;    |   z  n     |   2     {\displaystyle
      \sum _{n=1}^{\infty }|z_{n}|^{2}}  [\sum _{n=1}^{\infty }|z_{n}|^{2}]
converges. The inner product on l2 is defined by
         &#x27E8;  z  ,  w  &#x27E9; =  &#x2211;  n = 1   &#x221E;    z  n
      w  n   &#x00AF;    ,   {\displaystyle \langle \mathbf {z} ,\mathbf {w}
      \rangle =\sum _{n=1}^{\infty }z_{n}{\overline {w_{n}}}\,,}  [
      {\displaystyle \langle \mathbf {z} ,\mathbf {w} \rangle =\sum _{n=1}^
      {\infty }z_{n}{\overline {w_{n}}}\,,}]
with the latter series converging as a consequence of the CauchyâSchwarz
inequality.
Completeness of the space holds provided that whenever a series of elements
from l2 converges absolutely (in norm), then it converges to an element of l2.
The proof is basic in mathematical_analysis, and permits mathematical series of
elements of the space to be manipulated with the same ease as series of complex
numbers (or vectors in a finite-dimensional Euclidean space).[4]
***** History[edit] *****
David_Hilbert
Prior to the development of Hilbert spaces, other generalizations of Euclidean
spaces were known to mathematicians and physicists. In particular, the idea of
an abstract_linear_space had gained some traction towards the end of the 19th
century:[5] this is a space whose elements can be added together and multiplied
by scalars (such as real or complex_numbers) without necessarily identifying
these elements with "geometric"_vectors, such as position and momentum vectors
in physical systems. Other objects studied by mathematicians at the turn of the
20th century, in particular spaces of sequences (including series) and spaces
of functions,[6] can naturally be thought of as linear spaces. Functions, for
instance, can be added together or multiplied by constant scalars, and these
operations obey the algebraic laws satisfied by addition and scalar
multiplication of spatial vectors.
In the first decade of the 20th century, parallel developments led to the
introduction of Hilbert spaces. The first of these was the observation, which
arose during David_Hilbert and Erhard_Schmidt's study of integral_equations,[7]
that two square-integrable real-valued functions f and g on an interval [a, b]
have an inner product
         &#x27E8; f , g &#x27E9; =  &#x222B;  a   b   f ( x ) g ( x )   d  x
      {\displaystyle \langle f,g\rangle =\int _{a}^{b}f(x)g(x)\,\mathrm {d} x}
      [{\displaystyle \langle f,g\rangle =\int _{a}^{b}f(x)g(x)\,\mathrm {d}
      x}]
which has many of the familiar properties of the Euclidean dot product. In
particular, the idea of an orthogonal family of functions has meaning. Schmidt
exploited the similarity of this inner product with the usual dot product to
prove an analog of the spectral_decomposition for an operator of the form
         f ( x ) &#x21A6;  &#x222B;  a   b   K ( x , y ) f ( y )   d  y
      {\displaystyle f(x)\mapsto \int _{a}^{b}K(x,y)f(y)\,\mathrm {d} y}  [
      {\displaystyle f(x)\mapsto \int _{a}^{b}K(x,y)f(y)\,\mathrm {d} y}]
where K is a continuous function symmetric in x and y. The resulting
eigenfunction_expansion expresses the function K as a series of the form
         K ( x , y ) =  &#x2211;  n    &#x03BB;  n    &#x03C6;  n   ( x )
      &#x03C6;  n   ( y )   {\displaystyle K(x,y)=\sum _{n}\lambda _{n}\varphi
      _{n}(x)\varphi _{n}(y)}  [{\displaystyle K(x,y)=\sum _{n}\lambda _
      {n}\varphi _{n}(x)\varphi _{n}(y)}]
where the functions Ïn are orthogonal in the sense that â¨Ïn, Ïmâ© = 0 for
all n â  m. The individual terms in this series are sometimes referred to as
elementary product solutions. However, there are eigenfunction expansions that
fail to converge in a suitable sense to a square-integrable function: the
missing ingredient, which ensures convergence, is completeness.[8]
The second development was the Lebesgue_integral, an alternative to the Riemann
integral introduced by Henri_Lebesgue in 1904.[9] The Lebesgue integral made it
possible to integrate a much broader class of functions. In 1907, Frigyes_Riesz
and Ernst_Sigismund_Fischer independently proved that the space L2 of square
Lebesgue-integrable functions is a complete_metric_space.[10] As a consequence
of the interplay between geometry and completeness, the 19th century results of
Joseph_Fourier, Friedrich_Bessel and Marc-Antoine_Parseval on trigonometric
series easily carried over to these more general spaces, resulting in a
geometrical and analytical apparatus now usually known as the RieszâFischer
theorem.[11]
Further basic results were proved in the early 20th century. For example, the
Riesz_representation_theorem was independently established by Maurice_FrÃ©chet
and Frigyes_Riesz in 1907.[12] John_von_Neumann coined the term abstract
Hilbert space in his work on unbounded Hermitian_operators.[13] Although other
mathematicians such as Hermann_Weyl and Norbert_Wiener had already studied
particular Hilbert spaces in great detail, often from a physically motivated
point of view, von Neumann gave the first complete and axiomatic treatment of
them.[14] Von Neumann later used them in his seminal work on the foundations of
quantum mechanics,[15] and in his continued work with Eugene_Wigner. The name
"Hilbert space" was soon adopted by others, for example by Hermann Weyl in his
book on quantum mechanics and the theory of groups.[16]
The significance of the concept of a Hilbert space was underlined with the
realization that it offers one of the best mathematical_formulations_of_quantum
mechanics.[17] In short, the states of a quantum mechanical system are vectors
in a certain Hilbert space, the observables are hermitian_operators on that
space, the symmetries of the system are unitary_operators, and measurements are
orthogonal_projections. The relation between quantum mechanical symmetries and
unitary operators provided an impetus for the development of the unitary
representation_theory of groups, initiated in the 1928 work of Hermann Weyl.
[16] On the other hand, in the early 1930s it became clear that classical
mechanics can be described in terms of Hilbert space (Koopmanâvon_Neumann
classical_mechanics) and that certain properties of classical dynamical_systems
can be analyzed using Hilbert space techniques in the framework of ergodic
theory.[18]
The algebra of observables in quantum mechanics is naturally an algebra of
operators defined on a Hilbert space, according to Werner_Heisenberg's matrix
mechanics formulation of quantum theory. Von Neumann began investigating
operator_algebras in the 1930s, as rings of operators on a Hilbert space. The
kind of algebras studied by von Neumann and his contemporaries are now known as
von_Neumann_algebras. In the 1940s, Israel_Gelfand, Mark_Naimark and Irving
Segal gave a definition of a kind of operator algebras called C*-algebras that
on the one hand made no reference to an underlying Hilbert space, and on the
other extrapolated many of the useful features of the operator algebras that
had previously been studied. The spectral theorem for self-adjoint operators in
particular that underlies much of the existing Hilbert space theory was
generalized to C*-algebras. These techniques are now basic in abstract harmonic
analysis and representation theory.
***** Examples[edit] *****
**** Lebesgue spaces[edit] ****
Main article: Lp_space
Lebesgue spaces are function_spaces associated to measure_spaces (X, M, Î¼),
where X is a set, M is a Ï-algebra of subsets of X, and Î¼ is a countably
additive_measure on M. Let L2(X, Î¼) be the space of those complex-valued
measurable functions on X for which the Lebesgue_integral of the square of the
absolute_value of the function is finite, i.e., for a function f in L2(X, Î¼),
          &#x222B;  X    |  f   |   2    d  &#x03BC; < &#x221E;  ,
      {\displaystyle \int _{X}|f|^{2}\mathrm {d} \mu <\infty \,,}  [
      {\displaystyle \int _{X}|f|^{2}\mathrm {d} \mu <\infty \,,}]
and where functions are identified if and only if they differ only on a set_of
measure_zero.
The inner product of functions f and g in L2(X, Î¼) is then defined as
         &#x27E8; f , g &#x27E9; =  &#x222B;  X   f ( t )    g ( t )  &#x00AF;
      d  &#x03BC; ( t )  .   {\displaystyle \langle f,g\rangle =\int _{X}f(t)
      {\overline {g(t)}}\,\mathrm {d} \mu (t)\,.}  [{\displaystyle \langle
      f,g\rangle =\int _{X}f(t){\overline {g(t)}}\,\mathrm {d} \mu (t)\,.}]
For f and g in L2, this integral exists because of the CauchyâSchwarz
inequality, and defines an inner product on the space. Equipped with this inner
product, L2 is in fact complete.[19] The Lebesgue integral is essential to
ensure completeness: on domains of real numbers, for instance, not enough
functions are Riemann_integrable.[20]
The Lebesgue spaces appear in many natural settings. The spaces L2(â) and L2(
[0,1]) of square-integrable functions with respect to the Lebesgue_measure on
the real line and unit interval, respectively, are natural domains on which to
define the Fourier transform and Fourier series. In other situations, the
measure may be something other than the ordinary Lebesgue measure on the real
line. For instance, if w is any positive measurable function, the space of all
measurable functions f on the interval [0, 1] satisfying
          &#x222B;  0   1     |   f ( t )    |    2   w ( t )   d  t < &#x221E;
      {\displaystyle \int _{0}^{1}{\bigl |}f(t){\bigr |}^{2}w(t)\,\mathrm {d}
      t<\infty }  [{\displaystyle \int _{0}^{1}{\bigl |}f(t){\bigr |}^{2}w
      (t)\,\mathrm {d} t<\infty }]
is called the weighted_L2_space L2
w([0, 1]), and w is called the weight function. The inner product is defined by
         &#x27E8; f , g &#x27E9; =  &#x222B;  0   1   f ( t )    g ( t )
      &#x00AF;   w ( t )   d  t  .   {\displaystyle \langle f,g\rangle =\int _
      {0}^{1}f(t){\overline {g(t)}}w(t)\,\mathrm {d} t\,.}  [{\displaystyle
      \langle f,g\rangle =\int _{0}^{1}f(t){\overline {g(t)}}w(t)\,\mathrm {d}
      t\,.}]
The weighted space L2
w([0, 1]) is identical with the Hilbert space L2([0, 1], Î¼) where the measure
Î¼ of a Lebesgue-measurable set A is defined by
         &#x03BC; ( A ) =  &#x222B;  A   w ( t )   d  t  .   {\displaystyle \mu
      (A)=\int _{A}w(t)\,\mathrm {d} t\,.}  [{\displaystyle \mu (A)=\int _{A}w
      (t)\,\mathrm {d} t\,.}]
Weighted L2 spaces like this are frequently used to study orthogonal
polynomials, because different families of orthogonal polynomials are
orthogonal with respect to different weighting functions.
**** Sobolev spaces[edit] ****
Sobolev_spaces, denoted by Hs or Ws, 2, are Hilbert spaces. These are a special
kind of function_space in which differentiation may be performed, but that
(unlike other Banach_spaces such as the HÃ¶lder_spaces) support the structure
of an inner product. Because differentiation is permitted, Sobolev spaces are a
convenient setting for the theory of partial_differential_equations.[21] They
also form the basis of the theory of direct_methods_in_the_calculus_of
variations.[22]
For s a non-negative integer and Î© â ân, the Sobolev space Hs(Î©) contains
L2 functions whose weak_derivatives of order up to s are also L2. The inner
product in Hs(Î©) is
         &#x27E8; f , g &#x27E9; =  &#x222B;  &#x03A9;   f ( x )    g &#x00AF;
      ( x )   d  x +  &#x222B;  &#x03A9;   D f ( x ) &#x22C5; D    g &#x00AF;
      ( x )   d  x + &#x22EF; +  &#x222B;  &#x03A9;    D  s   f ( x ) &#x22C5;
      D  s      g &#x00AF;    ( x )   d  x   {\displaystyle \langle f,g\rangle
      =\int _{\Omega }f(x){\bar {g}}(x)\,\mathrm {d} x+\int _{\Omega }Df
      (x)\cdot D{\bar {g}}(x)\,\mathrm {d} x+\cdots +\int _{\Omega }D^{s}f
      (x)\cdot D^{s}{\bar {g}}(x)\,\mathrm {d} x}  [{\displaystyle \langle
      f,g\rangle =\int _{\Omega }f(x){\bar {g}}(x)\,\mathrm {d} x+\int _{\Omega
      }Df(x)\cdot D{\bar {g}}(x)\,\mathrm {d} x+\cdots +\int _{\Omega }D^{s}f
      (x)\cdot D^{s}{\bar {g}}(x)\,\mathrm {d} x}]
where the dot indicates the dot product in the Euclidean space of partial
derivatives of each order. Sobolev spaces can also be defined when s is not an
integer.
Sobolev spaces are also studied from the point of view of spectral theory,
relying more specifically on the Hilbert space structure. If Î© is a suitable
domain, then one can define the Sobolev space Hs(Î©) as the space of Bessel
potentials;[23] roughly,
          H  s   ( &#x03A9; ) =     {  ( 1 &#x2212; &#x0394;  )  &#x2212;   s 2
      f   |   f &#x2208;  L  2   ( &#x03A9; )  }   .   {\displaystyle H^{s}
      (\Omega )=\left.\left\{(1-\Delta )^{-{\frac {s}{2}}}f\,\right|\,f\in L^
      {2}(\Omega )\right\}\,.}  [{\displaystyle H^{s}(\Omega )=\left.\left\{(1-
      \Delta )^{-{\frac {s}{2}}}f\,\right|\,f\in L^{2}(\Omega )\right\}\,.}]
Here Î is the Laplacian and (1 â Î)âs/2 is understood in terms of the
spectral_mapping_theorem. Apart from providing a workable definition of Sobolev
spaces for non-integer s, this definition also has particularly desirable
properties under the Fourier_transform that make it ideal for the study of
pseudodifferential_operators. Using these methods on a compact Riemannian
manifold, one can obtain for instance the Hodge_decomposition, which is the
basis of Hodge_theory.[24]
**** Spaces of holomorphic functions[edit] ****
*** Hardy spaces[edit] ***
The Hardy_spaces are function spaces, arising in complex_analysis and harmonic
analysis, whose elements are certain holomorphic_functions in a complex domain.
[25] Let U denote the unit_disc in the complex plane. Then the Hardy space H2
(U) is defined as the space of holomorphic functions f on U such that the means
          M  r   ( f ) =   1  2 &#x03C0;     &#x222B;  0   2 &#x03C0;     |  f
      (  r  e  i &#x03B8;    )   |   2     d  &#x03B8;   {\displaystyle M_{r}
      (f)={\frac {1}{2\pi }}\int _{0}^{2\pi }\left|f\left(re^{i\theta
      }\right)\right|^{2}\,\mathrm {d} \theta }  [{\displaystyle M_{r}(f)=
      {\frac {1}{2\pi }}\int _{0}^{2\pi }\left|f\left(re^{i\theta
      }\right)\right|^{2}\,\mathrm {d} \theta }]
remain bounded for r < 1. The norm on this Hardy space is defined by
           &#x2016; f &#x2016;   2   =  lim  r &#x2192; 1      M  r   ( f )
      .   {\displaystyle \left\|f\right\|_{2}=\lim _{r\to 1}{\sqrt {M_{r}
      (f)}}\,.}  [{\displaystyle \left\|f\right\|_{2}=\lim _{r\to 1}{\sqrt {M_
      {r}(f)}}\,.}]
Hardy spaces in the disc are related to Fourier series. A function f is in H2
(U) if and only if
         f ( z ) =  &#x2211;  n = 0   &#x221E;    a  n    z  n
      {\displaystyle f(z)=\sum _{n=0}^{\infty }a_{n}z^{n}}  [{\displaystyle f
      (z)=\sum _{n=0}^{\infty }a_{n}z^{n}}]
where
          &#x2211;  n = 0   &#x221E;    |   a  n     |   2   < &#x221E;  .
      {\displaystyle \sum _{n=0}^{\infty }|a_{n}|^{2}<\infty \,.}  [
      {\displaystyle \sum _{n=0}^{\infty }|a_{n}|^{2}<\infty \,.}]
Thus H2(U) consists of those functions that are L2 on the circle, and whose
negative frequency Fourier coefficients vanish.
*** Bergman spaces[edit] ***
The Bergman_spaces are another family of Hilbert spaces of holomorphic
functions.[26] Let D be a bounded open set in the complex_plane (or a higher-
dimensional complex space) and let L2, h(D) be the space of holomorphic
functions f in D that are also in L2(D) in the sense that
         &#x2016; f  &#x2016;  2   =  &#x222B;  D    |  f ( z )   |   2     d
      &#x03BC; ( z ) < &#x221E;  ,   {\displaystyle \|f\|^{2}=\int _{D}|f(z)|^
      {2}\,\mathrm {d} \mu (z)<\infty \,,}  [{\displaystyle \|f\|^{2}=\int _
      {D}|f(z)|^{2}\,\mathrm {d} \mu (z)<\infty \,,}]
where the integral is taken with respect to the Lebesgue measure in D. Clearly
L2, h(D) is a subspace of L2(D); in fact, it is a closed subspace, and so a
Hilbert space in its own right. This is a consequence of the estimate, valid on
compact subsets K of D, that
          sup  z &#x2208; K    |  f ( z )  |  &#x2264;  C  K     &#x2016; f
      &#x2016;   2    ,   {\displaystyle \sup _{z\in K}\left|f(z)\right|\leq C_
      {K}\left\|f\right\|_{2}\,,}  [{\displaystyle \sup _{z\in K}\left|f
      (z)\right|\leq C_{K}\left\|f\right\|_{2}\,,}]
which in turn follows from Cauchy's_integral_formula. Thus convergence of a
sequence of holomorphic functions in L2(D) implies also compact_convergence,
and so the limit function is also holomorphic. Another consequence of this
inequality is that the linear functional that evaluates a function f at a point
of D is actually continuous on L2, h(D). The Riesz representation theorem
implies that the evaluation functional can be represented as an element of L2,
h(D). Thus, for every z â D, there is a function Î·z â L2, h(D) such that
         f ( z ) =  &#x222B;  D   f ( &#x03B6; )     &#x03B7;  z   ( &#x03B6; )
      &#x00AF;     d  &#x03BC; ( &#x03B6; )   {\displaystyle f(z)=\int _{D}f
      (\zeta ){\overline {\eta _{z}(\zeta )}}\,\mathrm {d} \mu (\zeta )}  [
      {\displaystyle f(z)=\int _{D}f(\zeta ){\overline {\eta _{z}(\zeta
      )}}\,\mathrm {d} \mu (\zeta )}]
for all f â L2, h(D). The integrand
         K ( &#x03B6; , z ) =     &#x03B7;  z   ( &#x03B6; )  &#x00AF;
      {\displaystyle K(\zeta ,z)={\overline {\eta _{z}(\zeta )}}}  [
      {\displaystyle K(\zeta ,z)={\overline {\eta _{z}(\zeta )}}}]
is known as the Bergman_kernel of D. This integral_kernel satisfies a
reproducing property
         f ( z ) =  &#x222B;  D   f ( &#x03B6; ) K ( &#x03B6; , z )   d
      &#x03BC; ( &#x03B6; )  .   {\displaystyle f(z)=\int _{D}f(\zeta )K(\zeta
      ,z)\,\mathrm {d} \mu (\zeta )\,.}  [{\displaystyle f(z)=\int _{D}f(\zeta
      )K(\zeta ,z)\,\mathrm {d} \mu (\zeta )\,.}]
A Bergman space is an example of a reproducing_kernel_Hilbert_space, which is a
Hilbert space of functions along with a kernel K(Î¶, z) that verifies a
reproducing property analogous to this one. The Hardy space H2(D) also admits a
reproducing kernel, known as the SzegÅ_kernel.[27] Reproducing kernels are
common in other areas of mathematics as well. For instance, in harmonic
analysis the Poisson_kernel is a reproducing kernel for the Hilbert space of
square-integrable harmonic_functions in the unit_ball. That the latter is a
Hilbert space at all is a consequence of the mean value theorem for harmonic
functions.
***** Applications[edit] *****
Many of the applications of Hilbert spaces exploit the fact that Hilbert spaces
support generalizations of simple geometric concepts like projection and change
of_basis from their usual finite dimensional setting. In particular, the
spectral_theory of continuous self-adjoint linear_operators on a Hilbert space
generalizes the usual spectral_decomposition of a matrix, and this often plays
a major role in applications of the theory to other areas of mathematics and
physics.
**** SturmâLiouville theory[edit] ****
Main articles: SturmâLiouville_theory and Spectral_theory_of_ordinary
differential_equations
The overtones of a vibrating string. These are eigenfunctions of an associated
SturmâLiouville problem. The eigenvalues 1, 1/2, 1/3, â¦ form the (musical)
harmonic_series.
In the theory of ordinary_differential_equations, spectral methods on a
suitable Hilbert space are used to study the behavior of eigenvalues and
eigenfunctions of differential equations. For example, the SturmâLiouville
problem arises in the study of the harmonics of waves in a violin string or a
drum, and is a central problem in ordinary_differential_equations.[28] The
problem is a differential equation of the form
         &#x2212;    d    d  x     [  p ( x )     d  y    d  x     ]  + q ( x )
      y = &#x03BB; w ( x ) y   {\displaystyle -{\frac {\mathrm {d} }{\mathrm
      {d} x}}\left[p(x){\frac {\mathrm {d} y}{\mathrm {d} x}}\right]+q
      (x)y=\lambda w(x)y}  [{\displaystyle -{\frac {\mathrm {d} }{\mathrm {d}
      x}}\left[p(x){\frac {\mathrm {d} y}{\mathrm {d} x}}\right]+q(x)y=\lambda
      w(x)y}]
for an unknown function y on an interval [a, b], satisfying general homogeneous
Robin_boundary_conditions
           {    &#x03B1; y ( a ) +  &#x03B1; &#x2032;   y &#x2032;  ( a )   = 0
      &#x03B2; y ( b ) +  &#x03B2; &#x2032;   y &#x2032;  ( b )   = 0  .
      {\displaystyle {\begin{cases}\alpha y(a)+\alpha 'y'(a)&=0\\\beta y
      (b)+\beta 'y'(b)&=0\,.\end{cases}}}  [{\displaystyle {\begin{cases}\alpha
      y(a)+\alpha 'y'(a)&=0\\\beta y(b)+\beta 'y'(b)&=0\,.\end{cases}}}]
The functions p, q, and w are given in advance, and the problem is to find the
function y and constants Î» for which the equation has a solution. The problem
only has solutions for certain values of Î», called eigenvalues of the system,
and this is a consequence of the spectral theorem for compact_operators applied
to the integral_operator defined by the Green's_function for the system.
Furthermore, another consequence of this general result is that the eigenvalues
Î» of the system can be arranged in an increasing sequence tending to infinity.
[nb_2]
**** Partial differential equations[edit] ****
Hilbert spaces form a basic tool in the study of partial_differential
equations.[21] For many classes of partial differential equations, such as
linear elliptic_equations, it is possible to consider a generalized solution
(known as a weak solution) by enlarging the class of functions. Many weak
formulations involve the class of Sobolev_functions, which is a Hilbert space.
A suitable weak formulation reduces to a geometrical problem the analytic
problem of finding a solution or, often what is more important, showing that a
solution exists and is unique for given boundary data. For linear elliptic
equations, one geometrical result that ensures unique solvability for a large
class of problems is the LaxâMilgram_theorem. This strategy forms the
rudiment of the Galerkin_method (a finite_element_method) for numerical
solution of partial differential equations.[29]
A typical example is the Poisson_equation âÎu = g with Dirichlet_boundary
conditions in a bounded domain Î© in â2. The weak formulation consists of
finding a function u such that, for all continuously differentiable functions v
in Î© vanishing on the boundary:
          &#x222B;  &#x03A9;   &#x2207; u &#x22C5; &#x2207; v =  &#x222B;
      &#x03A9;   g v  .   {\displaystyle \int _{\Omega }\nabla u\cdot \nabla
      v=\int _{\Omega }gv\,.}  [{\displaystyle \int _{\Omega }\nabla u\cdot
      \nabla v=\int _{\Omega }gv\,.}]
This can be recast in terms of the Hilbert space H1
0(Î©) consisting of functions u such that u, along with its weak partial
derivatives, are square integrable on Î©, and vanish on the boundary. The
question then reduces to finding u in this space such that for all v in this
space
         a ( u , v ) = b ( v )   {\displaystyle a(u,v)=b(v)}  [{\displaystyle a
      (u,v)=b(v)}]
where a is a continuous bilinear_form, and b is a continuous linear_functional,
given respectively by
         a ( u , v ) =  &#x222B;  &#x03A9;   &#x2207; u &#x22C5; &#x2207; v ,
      b ( v ) =  &#x222B;  &#x03A9;   g v  .   {\displaystyle a(u,v)=\int _
      {\Omega }\nabla u\cdot \nabla v,\quad b(v)=\int _{\Omega }gv\,.}  [
      {\displaystyle a(u,v)=\int _{\Omega }\nabla u\cdot \nabla v,\quad b
      (v)=\int _{\Omega }gv\,.}]
Since the Poisson equation is elliptic, it follows from PoincarÃ©'s inequality
that the bilinear form a is coercive. The LaxâMilgram theorem then ensures
the existence and uniqueness of solutions of this equation.
Hilbert spaces allow for many elliptic partial differential equations to be
formulated in a similar way, and the LaxâMilgram theorem is then a basic tool
in their analysis. With suitable modifications, similar techniques can be
applied to parabolic_partial_differential_equations and certain hyperbolic
partial_differential_equations.
**** Ergodic theory[edit] ****
The path of a billiard ball in the Bunimovich_stadium is described by an
ergodic dynamical_system.
The field of ergodic_theory is the study of the long-term behavior of chaotic
dynamical_systems. The protypical case of a field that ergodic theory applies
to is thermodynamics, in whichâthough the microscopic state of a system is
extremely complicated (it is impossible to understand the ensemble of
individual collisions between particles of matter)âthe average behavior over
sufficiently long time intervals is tractable. The laws_of_thermodynamics are
assertions about such average behavior. In particular, one formulation of the
zeroth_law_of_thermodynamics asserts that over sufficiently long timescales,
the only functionally independent measurement that one can make of a
thermodynamic system in equilibrium is its total energy, in the form of
temperature.
An ergodic dynamical system is one for which, apart from the energyâmeasured
by the Hamiltonianâthere are no other functionally independent conserved
quantities on the phase_space. More explicitly, suppose that the energy E is
fixed, and let Î©E be the subset of the phase space consisting of all states of
energy E (an energy surface), and let Tt denote the evolution operator on the
phase space. The dynamical system is ergodic if there are no continuous non-
constant functions on Î©E such that
         f (  T  t   w ) = f ( w )   {\displaystyle f(T_{t}w)=f(w)}  [
      {\displaystyle f(T_{t}w)=f(w)}]
for all w on Î©E and all time t. Liouville's_theorem implies that there exists
a measure Î¼ on the energy surface that is invariant under the time
translation. As a result, time translation is a unitary_transformation of the
Hilbert space L2(Î©E, Î¼) consisting of square-integrable functions on the
energy surface Î©E with respect to the inner product
           &#x27E8;  f , g  &#x27E9;    L  2    (   &#x03A9;  E   , &#x03BC;  )
      =  &#x222B;  E   f    g &#x00AF;      d  &#x03BC;  .   {\displaystyle
      \left\langle f,g\right\rangle _{L^{2}\left(\Omega _{E},\mu \right)}=\int
      _{E}f{\bar {g}}\,\mathrm {d} \mu \,.}  [{\displaystyle \left\langle
      f,g\right\rangle _{L^{2}\left(\Omega _{E},\mu \right)}=\int _{E}f{\bar
      {g}}\,\mathrm {d} \mu \,.}]
The von Neumann mean ergodic theorem[18] states the following:
    * If Ut is a (strongly continuous) one-parameter semigroup of unitary
      operators on a Hilbert space H, and P is the orthogonal projection onto
      the space of common fixed points of Ut, {x âH | Utx = x, ât > 0},
      then
               P x =  lim  T &#x2192; &#x221E;     1 T    &#x222B;  0   T    U
            t   x   d  t  .   {\displaystyle Px=\lim _{T\to \infty }{\frac {1}
            {T}}\int _{0}^{T}U_{t}x\,\mathrm {d} t\,.}  [{\displaystyle Px=\lim
            _{T\to \infty }{\frac {1}{T}}\int _{0}^{T}U_{t}x\,\mathrm {d}
            t\,.}]
For an ergodic system, the fixed set of the time evolution consists only of the
constant functions, so the ergodic theorem implies the following:[30] for any
function f â L2(Î©E, Î¼),
             L  2   &#x2212; lim   T &#x2192; &#x221E;      1 T    &#x222B;  0
      T   f (  T  t   w )   d  t =  &#x222B;   &#x03A9;  E     f ( y )   d
      &#x03BC; ( y )  .   {\displaystyle {\underset {T\to \infty }{L^{2}-\lim
      }}{\frac {1}{T}}\int _{0}^{T}f(T_{t}w)\,\mathrm {d} t=\int _{\Omega _
      {E}}f(y)\,\mathrm {d} \mu (y)\,.}  [{\displaystyle {\underset {T\to
      \infty }{L^{2}-\lim }}{\frac {1}{T}}\int _{0}^{T}f(T_{t}w)\,\mathrm {d}
      t=\int _{\Omega _{E}}f(y)\,\mathrm {d} \mu (y)\,.}]
That is, the long time average of an observable f is equal to its expectation
value over an energy surface.
**** Fourier analysis[edit] ****
Superposition of sinusoidal wave basis functions (bottom) to form a sawtooth
wave (top)
Spherical_harmonics, an orthonormal basis for the Hilbert space of square-
integrable functions on the sphere, shown graphed along the radial direction
One of the basic goals of Fourier_analysis is to decompose a function into a
(possibly infinite) linear_combination of given basis functions: the associated
Fourier_series. The classical Fourier series associated to a function f defined
on the interval [0, 1] is a series of the form
          &#x2211;  n = &#x2212; &#x221E;   &#x221E;    a  n    e  2 &#x03C0; i
      n &#x03B8;     {\displaystyle \sum _{n=-\infty }^{\infty }a_{n}e^{2\pi
      in\theta }}  [\sum _{n=-\infty }^{\infty }a_{n}e^{2\pi in\theta }]
where
          a  n   =  &#x222B;  0   1   f ( &#x03B8; )  e  &#x2212; 2 &#x03C0; i
      n &#x03B8;     d  &#x03B8;  .   {\displaystyle a_{n}=\int _{0}^{1}f
      (\theta )e^{-2\pi in\theta }\,\mathrm {d} \theta \,.}  [{\displaystyle a_
      {n}=\int _{0}^{1}f(\theta )e^{-2\pi in\theta }\,\mathrm {d} \theta \,.}]
The example of adding up the first few terms in a Fourier series for a sawtooth
function is shown in the figure. The basis functions are sine waves with
wavelengths Î»/n (for integer n) shorter than the wavelength Î» of the sawtooth
itself (except for n = 1, the fundamental wave). All basis functions have nodes
at the nodes of the sawtooth, but all but the fundamental have additional
nodes. The oscillation of the summed terms about the sawtooth is called the
Gibbs_phenomenon.
A significant problem in classical Fourier series asks in what sense the
Fourier series converges, if at all, to the function f. Hilbert space methods
provide one possible answer to this question.[31] The functions en(Î¸) =
e2ÏinÎ¸ form an orthogonal basis of the Hilbert space L2([0, 1]).
Consequently, any square-integrable function can be expressed as a series
         f ( &#x03B8; ) =  &#x2211;  n    a  n    e  n   ( &#x03B8; )  ,   a  n
      = &#x27E8; f ,  e  n   &#x27E9;   {\displaystyle f(\theta )=\sum _{n}a_
      {n}e_{n}(\theta )\,,\quad a_{n}=\langle f,e_{n}\rangle }  [{\displaystyle
      f(\theta )=\sum _{n}a_{n}e_{n}(\theta )\,,\quad a_{n}=\langle f,e_
      {n}\rangle }]
and, moreover, this series converges in the Hilbert space sense (that is, in
the L2_mean).
The problem can also be studied from the abstract point of view: every Hilbert
space has an orthonormal_basis, and every element of the Hilbert space can be
written in a unique way as a sum of multiples of these basis elements. The
coefficients appearing on these basis elements are sometimes known abstractly
as the Fourier coefficients of the element of the space.[32] The abstraction is
especially useful when it is more natural to use different basis functions for
a space such as L2([0, 1]). In many circumstances, it is desirable not to
decompose a function into trigonometric functions, but rather into orthogonal
polynomials or wavelets for instance,[33] and in higher dimensions into
spherical_harmonics.[34]
For instance, if en are any orthonormal basis functions of L2[0, 1], then a
given function in L2[0, 1] can be approximated as a finite linear combination
[35]
         f ( x ) &#x2248;  f  n   ( x ) =  a  1    e  1   ( x ) +  a  2    e  2
      ( x ) + &#x22EF; +  a  n    e  n   ( x )  .   {\displaystyle f(x)\approx
      f_{n}(x)=a_{1}e_{1}(x)+a_{2}e_{2}(x)+\cdots +a_{n}e_{n}(x)\,.}  [
      {\displaystyle f(x)\approx f_{n}(x)=a_{1}e_{1}(x)+a_{2}e_{2}(x)+\cdots
      +a_{n}e_{n}(x)\,.}]
The coefficients {aj} are selected to make the magnitude of the difference ||f
â fn||2 as small as possible. Geometrically, the best_approximation is the
orthogonal_projection of f onto the subspace consisting of all linear
combinations of the {ej}, and can be calculated by[36]
          a  j   =  &#x222B;  0   1       e  j   ( x )  &#x00AF;   f ( x )   d
      x  .   {\displaystyle a_{j}=\int _{0}^{1}{\overline {e_{j}(x)}}f
      (x)\,\mathrm {d} x\,.}  [{\displaystyle a_{j}=\int _{0}^{1}{\overline {e_
      {j}(x)}}f(x)\,\mathrm {d} x\,.}]
That this formula minimizes the difference ||f â fn||2 is a consequence of
Bessel's_inequality_and_Parseval's_formula.
In various applications to physical problems, a function can be decomposed into
physically meaningful eigenfunctions of a differential_operator (typically the
Laplace_operator): this forms the foundation for the spectral study of
functions, in reference to the spectrum of the differential operator.[37] A
concrete physical application involves the problem of hearing_the_shape_of_a
drum: given the fundamental modes of vibration that a drumhead is capable of
producing, can one infer the shape of the drum itself?[38] The mathematical
formulation of this question involves the Dirichlet_eigenvalues of the Laplace
equation in the plane, that represent the fundamental modes of vibration in
direct analogy with the integers that represent the fundamental modes of
vibration of the violin string.
Spectral_theory also underlies certain aspects of the Fourier_transform of a
function. Whereas Fourier analysis decomposes a function defined on a compact
set into the discrete spectrum of the Laplacian (which corresponds to the
vibrations of a violin string or drum), the Fourier transform of a function is
the decomposition of a function defined on all of Euclidean space into its
components in the continuous_spectrum of the Laplacian. The Fourier
transformation is also geometrical, in a sense made precise by the Plancherel
theorem, that asserts that it is an isometry of one Hilbert space (the "time
domain") with another (the "frequency domain"). This isometry property of the
Fourier transformation is a recurring theme in abstract harmonic_analysis, as
evidenced for instance by the Plancherel_theorem_for_spherical_functions
occurring in noncommutative_harmonic_analysis.
**** Quantum mechanics[edit] ****
The orbitals of an electron in a hydrogen_atom are eigenfunctions of the
energy.
In the mathematically rigorous formulation of quantum_mechanics, developed by
John_von_Neumann,[39] the possible states (more precisely, the pure_states) of
a quantum mechanical system are represented by unit_vectors (called state
vectors) residing in a complex separable Hilbert space, known as the state
space, well defined up to a complex number of norm 1 (the phase_factor). In
other words, the possible states are points in the projectivization of a
Hilbert space, usually called the complex_projective_space. The exact nature of
this Hilbert space is dependent on the system; for example, the position and
momentum states for a single non-relativistic spin zero particle is the space
of all square-integrable functions, while the states for the spin of a single
proton are unit elements of the two-dimensional complex Hilbert space of
spinors. Each observable is represented by a self-adjoint linear_operator
acting on the state space. Each eigenstate of an observable corresponds to an
eigenvector of the operator, and the associated eigenvalue corresponds to the
value of the observable in that eigenstate.
The inner product between two state vectors is a complex number known as a
probability_amplitude. During an ideal measurement of a quantum mechanical
system, the probability that a system collapses from a given initial state to a
particular eigenstate is given by the square of the absolute_value of the
probability amplitudes between the initial and final states. The possible
results of a measurement are the eigenvalues of the operatorâwhich explains
the choice of self-adjoint operators, for all the eigenvalues must be real. The
probability distribution of an observable in a given state can be found by
computing the spectral decomposition of the corresponding operator.
For a general system, states are typically not pure, but instead are
represented as statistical mixtures of pure states, or mixed states, given by
density_matrices: self-adjoint operators of trace one on a Hilbert space.
Moreover, for general quantum mechanical systems, the effects of a single
measurement can influence other parts of a system in a manner that is described
instead by a positive_operator_valued_measure. Thus the structure both of the
states and observables in the general theory is considerably more complicated
than the idealization for pure states.
**** Color perception[edit] ****
Main article: Color_vision_Â§ Mathematics_of_color_perception
Any true physical color can be represented by a combination of pure spectral
colors. As physical colors can be composed of any number of spectral colors,
the space of physical colors may aptly be represented by a Hilbert space over
spectral colors. Humans have three_types_of_cone_cells for color perception, so
the perceivable colors can be represented by 3-dimensional Euclidean space. The
many-to-one linear mapping from the Hilbert space of physical colors to the
Euclidean space of human perceivable colors explains why many distinct physical
colors may be perceived by humans to be identical (e.g., pure yellow light
versus a mix of red and green light, see metamerism).
***** Properties[edit] *****
**** Pythagorean identity[edit] ****
Two vectors u and v in a Hilbert space H are orthogonal when &#x27e8;u,
v&#x27e9; = 0. The notation for this is u â¥ v. More generally, when S is a
subset in H, the notation u â¥ S means that u is orthogonal to every element
from S.
When u and v are orthogonal, one has
         &#x2016; u + v  &#x2016;  2   = &#x27E8; u + v , u + v &#x27E9; =
      &#x27E8; u , u &#x27E9; + 2  Re &#x2061; &#x27E8; u , v &#x27E9; +
      &#x27E8; v , v &#x27E9; = &#x2016; u  &#x2016;  2   + &#x2016; v
      &#x2016;  2    .   {\displaystyle \|u+v\|^{2}=\langle u+v,u+v\rangle
      =\langle u,u\rangle +2\,\operatorname {Re} \langle u,v\rangle +\langle
      v,v\rangle =\|u\|^{2}+\|v\|^{2}\,.}  [{\displaystyle \|u+v\|^{2}=\langle
      u+v,u+v\rangle =\langle u,u\rangle +2\,\operatorname {Re} \langle
      u,v\rangle +\langle v,v\rangle =\|u\|^{2}+\|v\|^{2}\,.}]
By induction on n, this is extended to any family u1, â¦, un of n orthogonal
vectors,
         &#x2016;  u  1   + &#x22EF; +  u  n    &#x2016;  2   = &#x2016;  u  1
      &#x2016;  2   + &#x22EF; + &#x2016;  u  n    &#x2016;  2    .
      {\displaystyle \|u_{1}+\cdots +u_{n}\|^{2}=\|u_{1}\|^{2}+\cdots +\|u_
      {n}\|^{2}\,.}  [{\displaystyle \|u_{1}+\cdots +u_{n}\|^{2}=\|u_{1}\|^
      {2}+\cdots +\|u_{n}\|^{2}\,.}]
Whereas the Pythagorean identity as stated is valid in any inner product space,
completeness is required for the extension of the Pythagorean identity to
series. A series âuk of orthogonal vectors converges in H if and only if the
series of squares of norms converges, and
           &#x2016;   &#x2211;  k = 0   &#x221E;    u  k    &#x2016;   2   =
      &#x2211;  k = 0   &#x221E;     &#x2016;  u  k   &#x2016;   2    .
      {\displaystyle \left\|\sum _{k=0}^{\infty }u_{k}\right\|^{2}=\sum _{k=0}^
      {\infty }\left\|u_{k}\right\|^{2}\,.}  [{\displaystyle \left\|\sum _
      {k=0}^{\infty }u_{k}\right\|^{2}=\sum _{k=0}^{\infty }\left\|u_
      {k}\right\|^{2}\,.}]
Furthermore, the sum of a series of orthogonal vectors is independent of the
order in which it is taken.
**** Parallelogram identity and polarization[edit] ****
Geometrically, the parallelogram identity asserts that AC2 + BD2 = 2(AB2 +
AD2). In words, the sum of the squares of the diagonals is twice the sum of the
squares of any two adjacent sides.
By definition, every Hilbert space is also a Banach_space. Furthermore, in
every Hilbert space the following parallelogram_identity holds:
         &#x2016; u + v  &#x2016;  2   + &#x2016; u &#x2212; v  &#x2016;  2   =
      2  (  &#x2016; u  &#x2016;  2   + &#x2016; v  &#x2016;  2    )   .
      {\displaystyle \|u+v\|^{2}+\|u-v\|^{2}=2\left(\|u\|^{2}+\|v\|^
      {2}\right)\,.}  [{\displaystyle \|u+v\|^{2}+\|u-v\|^{2}=2\left(\|u\|^
      {2}+\|v\|^{2}\right)\,.}]
Conversely, every Banach space in which the parallelogram identity holds is a
Hilbert space, and the inner product is uniquely determined by the norm by the
polarization_identity.[40] For real Hilbert spaces, the polarization identity
is
         &#x27E8; u , v &#x27E9; =   1 4    (  &#x2016; u + v  &#x2016;  2
      &#x2212; &#x2016; u &#x2212; v  &#x2016;  2    )   .   {\displaystyle
      \langle u,v\rangle ={\frac {1}{4}}\left(\|u+v\|^{2}-\|u-v\|^
      {2}\right)\,.}  [{\displaystyle \langle u,v\rangle ={\frac {1}{4}}\left
      (\|u+v\|^{2}-\|u-v\|^{2}\right)\,.}]
For complex Hilbert spaces, it is
         &#x27E8; u , v &#x27E9; =    1 4     (  &#x2016; u + v  &#x2016;  2
      &#x2212; &#x2016; u &#x2212; v  &#x2016;  2   + i &#x2016; u + i v
      &#x2016;  2   &#x2212; i &#x2016; u &#x2212; i v  &#x2016;  2    )   .
      {\displaystyle \langle u,v\rangle ={\tfrac {1}{4}}\left(\|u+v\|^{2}-\|u-
      v\|^{2}+i\|u+iv\|^{2}-i\|u-iv\|^{2}\right)\,.}  [{\displaystyle \langle
      u,v\rangle ={\tfrac {1}{4}}\left(\|u+v\|^{2}-\|u-v\|^{2}+i\|u+iv\|^{2}-
      i\|u-iv\|^{2}\right)\,.}]
The parallelogram law implies that any Hilbert space is a uniformly_convex
Banach_space.[41]
**** Best approximation[edit] ****
This subsection employs the Hilbert_projection_theorem. If C is a non-empty
closed convex subset of a Hilbert space H and x a point in H, there exists a
unique point y â C that minimizes the distance between x and points in C,[42]
         y &#x2208; C  ,  &#x2016; x &#x2212; y &#x2016; = dist &#x2061; ( x ,
      C ) = min { &#x2016; x &#x2212; z &#x2016; : z &#x2208; C }  .
      {\displaystyle y\in C\,,\quad \|x-y\|=\operatorname {dist} (x,C)=\min\
      {\|x-z\|:z\in C\}\,.}  [{\displaystyle y\in C\,,\quad \|x-
      y\|=\operatorname {dist} (x,C)=\min\{\|x-z\|:z\in C\}\,.}]
This is equivalent to saying that there is a point with minimal norm in the
translated convex set D = C â x. The proof consists in showing that every
minimizing sequence (dn) â D is Cauchy (using the parallelogram identity)
hence converges (using completeness) to a point in D that has minimal norm.
More generally, this holds in any uniformly convex Banach space.[43]
When this result is applied to a closed subspace F of H, it can be shown that
the point y â F closest to x is characterized by[44]
         y &#x2208; F  ,  x &#x2212; y &#x22A5; F  .   {\displaystyle y\in
      F\,,\quad x-y\perp F\,.}  [{\displaystyle y\in F\,,\quad x-y\perp F\,.}]
This point y is the orthogonal projection of x onto F, and the mapping PF : x
â y is linear (see Orthogonal_complements_and_projections). This result is
especially significant in applied_mathematics, especially numerical_analysis,
where it forms the basis of least_squares methods.[45]
In particular, when F is not equal to H, one can find a nonzero vector v
orthogonal to F (select x â F and v = x â y). A very useful criterion is
obtained by applying this observation to the closed subspace F generated by a
subset S of H.
      A subset S of H spans a dense vector subspace if (and only if) the vector
      0 is the sole vector v â H orthogonal to S.
**** Duality[edit] ****
The dual_space H* is the space of all continuous linear functions from the
space H into the base field. It carries a natural norm, defined by
         &#x2016; &#x03C6; &#x2016; =  sup  &#x2016; x &#x2016; = 1 , x
      &#x2208; H    |  &#x03C6; ( x )  |   .   {\displaystyle \|\varphi \|=\sup
      _{\|x\|=1,x\in H}|\varphi (x)|\,.}  [{\displaystyle \|\varphi \|=\sup _
      {\|x\|=1,x\in H}|\varphi (x)|\,.}]
This norm satisfies the parallelogram_law, and so the dual space is also an
inner product space. The dual space is also complete, and so it is a Hilbert
space in its own right.
The Riesz_representation_theorem affords a convenient description of the dual.
To every element u of H, there is a unique element Ïu of H*, defined by
          &#x03C6;  u   ( x ) = &#x27E8; x , u &#x27E9;  .   {\displaystyle
      \varphi _{u}(x)=\langle x,u\rangle \,.}  [{\displaystyle \varphi _{u}
      (x)=\langle x,u\rangle \,.}]
The mapping u â¦ Ïu is an antilinear_mapping from H to H*. The Riesz
representation theorem states that this mapping is an antilinear isomorphism.
[46] Thus to every element Ï of the dual H* there exists one and only one uÏ
in H such that
         &#x27E8; x ,  u  &#x03C6;   &#x27E9; = &#x03C6; ( x )   {\displaystyle
      \langle x,u_{\varphi }\rangle =\varphi (x)}  [\langle x,u_{\varphi
      }\rangle =\varphi (x)]
for all x â H. The inner product on the dual space H* satisfies
         &#x27E8; &#x03C6; , &#x03C8; &#x27E9; = &#x27E8;  u  &#x03C8;   ,  u
      &#x03C6;   &#x27E9;  .   {\displaystyle \langle \varphi ,\psi \rangle
      =\langle u_{\psi },u_{\varphi }\rangle \,.}  [{\displaystyle \langle
      \varphi ,\psi \rangle =\langle u_{\psi },u_{\varphi }\rangle \,.}]
The reversal of order on the right-hand side restores linearity in Ï from the
antilinearity of uÏ. In the real case, the antilinear isomorphism from H to
its dual is actually an isomorphism, and so real Hilbert spaces are naturally
isomorphic to their own duals.
The representing vector uÏ is obtained in the following way. When Ï â  0,
the kernel F = Ker(Ï) is a closed vector subspace of H, not equal to H, hence
there exists a nonzero vector v orthogonal to F. The vector u is a suitable
scalar multiple Î»v of v. The requirement that Ï(v) = â¨v, uâ© yields
         u = &#x27E8; v , v  &#x27E9;  &#x2212; 1       &#x03C6; ( v )
      &#x00AF;    v  .   {\displaystyle u=\langle v,v\rangle ^{-1}\,{\overline
      {\varphi (v)}}\,v\,.}  [{\displaystyle u=\langle v,v\rangle ^{-1}\,
      {\overline {\varphi (v)}}\,v\,.}]
This correspondence Ï â u is exploited by the braâket_notation popular in
physics. It is common in physics to assume that the inner product, denoted by
&#x27e8;x|y&#x27e9;, is linear on the right,
         &#x27E8; x  |  y &#x27E9; = &#x27E8; y , x &#x27E9;  .
      {\displaystyle \langle x|y\rangle =\langle y,x\rangle \,.}  [
      {\displaystyle \langle x|y\rangle =\langle y,x\rangle \,.}]
The result &#x27e8;x|y&#x27e9; can be seen as the action of the linear
functional &#x27e8;x| (the bra) on the vector |y&#x27e9; (the ket).
The Riesz representation theorem relies fundamentally not just on the presence
of an inner product, but also on the completeness of the space. In fact, the
theorem implies that the topological_dual of any inner product space can be
identified with its completion. An immediate consequence of the Riesz
representation theorem is also that a Hilbert space H is reflexive, meaning
that the natural map from H into its double_dual_space is an isomorphism.
**** Weakly-convergent sequences[edit] ****
Main article: Weak_convergence_(Hilbert_space)
In a Hilbert space H, a sequence {xn} is weakly_convergent to a vector x â H
when
          lim  n   &#x27E8;  x  n   , v &#x27E9; = &#x27E8; x , v &#x27E9;
      {\displaystyle \lim _{n}\langle x_{n},v\rangle =\langle x,v\rangle }
      [\lim _{n}\langle x_{n},v\rangle =\langle x,v\rangle ]
for every v â H.
For example, any orthonormal sequence {fn} converges weakly to 0, as a
consequence of Bessel's_inequality. Every weakly convergent sequence {xn} is
bounded, by the uniform_boundedness_principle.
Conversely, every bounded sequence in a Hilbert space admits weakly convergent
subsequences (Alaoglu's_theorem).[47] This fact may be used to prove
minimization results for continuous convex_functionals, in the same way that
the BolzanoâWeierstrass_theorem is used for continuous functions on âd.
Among several variants, one simple statement is as follows:[48]
      If f : H â â is a convex continuous function such that f(x) tends to
      +â when ||x|| tends to â, then f admits a minimum at some point x0
      â H.
This fact (and its various generalizations) are fundamental for direct_methods
in the calculus_of_variations. Minimization results for convex functionals are
also a direct consequence of the slightly more abstract fact that closed
bounded convex subsets in a Hilbert space H are weakly_compact, since H is
reflexive. The existence of weakly convergent subsequences is a special case of
the EberleinâÅ mulian_theorem.
**** Banach space properties[edit] ****
Any general property of Banach_spaces continues to hold for Hilbert spaces. The
open_mapping_theorem states that a continuous surjective linear transformation
from one Banach space to another is an open_mapping meaning that it sends open
sets to open sets. A corollary is the bounded_inverse_theorem, that a
continuous and bijective linear function from one Banach space to another is an
isomorphism (that is, a continuous linear map whose inverse is also
continuous). This theorem is considerably simpler to prove in the case of
Hilbert spaces than in general Banach spaces.[49] The open mapping theorem is
equivalent to the closed_graph_theorem, which asserts that a function from one
Banach space to another is continuous if and only if its graph is a closed_set.
[50] In the case of Hilbert spaces, this is basic in the study of unbounded
operators (see closed_operator).
The (geometrical) HahnâBanach_theorem asserts that a closed convex set can be
separated from any point outside it by means of a hyperplane of the Hilbert
space. This is an immediate consequence of the best_approximation property: if
y is the element of a closed convex set F closest to x, then the separating
hyperplane is the plane perpendicular to the segment xy passing through its
midpoint.[51]
***** Operators on Hilbert spaces[edit] *****
**** Bounded operators[edit] ****
The continuous linear_operators A : H1 â H2 from a Hilbert space H1 to a
second Hilbert space H2 are bounded in the sense that they map bounded_sets to
bounded sets. Conversely, if an operator is bounded, then it is continuous. The
space of such bounded_linear_operators has a norm, the operator_norm given by
         &#x2016; A &#x2016; = sup  {   &#x2016; A x &#x2016; : &#x2016; x
      &#x2016; &#x2264; 1   }   .   {\displaystyle \lVert A\rVert =\sup \left\
      {\,\lVert Ax\rVert :\lVert x\rVert \leq 1\,\right\}\,.}  [{\displaystyle
      \lVert A\rVert =\sup \left\{\,\lVert Ax\rVert :\lVert x\rVert \leq
      1\,\right\}\,.}]
The sum and the composite of two bounded linear operators is again bounded and
linear. For y in H2, the map that sends x â H1 to â¨Ax, yâ© is linear and
continuous, and according to the Riesz_representation_theorem can therefore be
represented in the form
          &#x27E8;  x ,  A  &#x2217;   y  &#x27E9;  = &#x27E8; A x , y &#x27E9;
      {\displaystyle \left\langle x,A^{*}y\right\rangle =\langle Ax,y\rangle }
      [{\displaystyle \left\langle x,A^{*}y\right\rangle =\langle Ax,y\rangle
      }]
for some vector A*y in H1. This defines another bounded linear operator A* : H2
â H1, the adjoint of A. One can see that A** = A.
The set B(H) of all bounded linear operators on H (operators H â H), together
with the addition and composition operations, the norm and the adjoint
operation, is a C*-algebra, which is a type of operator_algebra.
An element A of B(H) is called 'self-adjoint' or 'Hermitian' if A* = A. If A is
Hermitian and â¨Ax, xâ© â¥ 0 for every x, then A is called 'nonnegative',
written A â¥ 0; if equality holds only when x = 0, then A is called
'positive'. The set of self adjoint operators admits a partial_order, in which
A â¥ B if A â B â¥ 0. If A has the form B*B for some B, then A is
nonnegative; if B is invertible, then A is positive. A converse is also true in
the sense that, for a non-negative operator A, there exists a unique non-
negative square_root B such that
         A =  B  2   =  B  &#x2217;   B  .   {\displaystyle A=B^{2}=B^{*}B\,.}
      [{\displaystyle A=B^{2}=B^{*}B\,.}]
In a sense made precise by the spectral_theorem, self-adjoint operators can
usefully be thought of as operators that are "real". An element A of B(H) is
called normal if A*A = AA*. Normal operators decompose into the sum of a self-
adjoint operators and an imaginary multiple of a self adjoint operator
         A =    A +  A  &#x2217;    2   + i    A &#x2212;  A  &#x2217;     2 i
      {\displaystyle A={\frac {A+A^{*}}{2}}+i{\frac {A-A^{*}}{2i}}}  [
      {\displaystyle A={\frac {A+A^{*}}{2}}+i{\frac {A-A^{*}}{2i}}}]
that commute with each other. Normal operators can also usefully be thought of
in terms of their real and imaginary parts.
An element U of B(H) is called unitary if U is invertible and its inverse is
given by U*. This can also be expressed by requiring that U be onto and â¨Ux,
Uyâ© = â¨x, yâ© for all x, y â H. The unitary operators form a group under
composition, which is the isometry_group of H.
An element of B(H) is compact if it sends bounded sets to relatively_compact
sets. Equivalently, a bounded operator T is compact if, for any bounded
sequence {xk}, the sequence {Txk} has a convergent subsequence. Many integral
operators are compact, and in fact define a special class of operators known as
HilbertâSchmidt_operators that are especially important in the study of
integral_equations. Fredholm_operators differ from a compact operator by a
multiple of the identity, and are equivalently characterized as operators with
a finite dimensional kernel and cokernel. The index of a Fredholm operator T is
defined by
         index &#x2061; T = dim &#x2061; ker &#x2061; T &#x2212; dim &#x2061;
      coker &#x2061; T  .   {\displaystyle \operatorname {index} T=\dim \ker T-
      \dim \operatorname {coker} T\,.}  [{\displaystyle \operatorname {index}
      T=\dim \ker T-\dim \operatorname {coker} T\,.}]
The index is homotopy invariant, and plays a deep role in differential_geometry
via the AtiyahâSinger_index_theorem.
**** Unbounded operators[edit] ****
Unbounded_operators are also tractable in Hilbert spaces, and have important
applications to quantum_mechanics.[52] An unbounded operator T on a Hilbert
space H is defined as a linear operator whose domain D(T) is a linear subspace
of H. Often the domain D(T) is a dense subspace of H, in which case T is known
as a densely_defined_operator.
The adjoint of a densely defined unbounded operator is defined in essentially
the same manner as for bounded operators. Self-adjoint_unbounded_operators play
the role of the observables in the mathematical formulation of quantum
mechanics. Examples of self-adjoint unbounded operators on the Hilbert space L2
(â) are:[53]
    * A suitable extension of the differential operator
               ( A f ) ( x ) = &#x2212; i    d    d  x    f ( x )  ,
            {\displaystyle (Af)(x)=-i{\frac {\mathrm {d} }{\mathrm {d} x}}f
            (x)\,,}  [{\displaystyle (Af)(x)=-i{\frac {\mathrm {d} }{\mathrm
            {d} x}}f(x)\,,}]
      where i is the imaginary unit and f is a differentiable function of
      compact support.
    * The multiplication-by-x operator:
               ( B f ) ( x ) = x f ( x )  .   {\displaystyle (Bf)(x)=xf(x)\,.}
            [{\displaystyle (Bf)(x)=xf(x)\,.}]
These correspond to the momentum and position observables, respectively. Note
that neither A nor B is defined on all of H, since in the case of A the
derivative need not exist, and in the case of B the product function need not
be square integrable. In both cases, the set of possible arguments form dense
subspaces of L2(â).
***** Constructions[edit] *****
**** Direct sums[edit] ****
Two Hilbert spaces H1 and H2 can be combined into another Hilbert space, called
the (orthogonal)_direct_sum,[54] and denoted
          H  1   &#x2295;  H  2    ,   {\displaystyle H_{1}\oplus H_{2}\,,}  [
      {\displaystyle H_{1}\oplus H_{2}\,,}]
consisting of the set of all ordered_pairs (x1, x2) where xi â Hi, i = 1, 2,
and inner product defined by
           &#x27E8;   (  x  1   ,  x  2   ) , (  y  1   ,  y  2   )    &#x27E9;
      H  1   &#x2295;  H  2     =   &#x27E8;   x  1   ,  y  1    &#x27E9;    H
      1     +   &#x27E8;   x  2   ,  y  2    &#x27E9;    H  2      .
      {\displaystyle {\bigl \langle }(x_{1},x_{2}),(y_{1},y_{2}){\bigr \rangle
      }_{H_{1}\oplus H_{2}}=\left\langle x_{1},y_{1}\right\rangle _{H_
      {1}}+\left\langle x_{2},y_{2}\right\rangle _{H_{2}}\,.}  [{\displaystyle
      {\bigl \langle }(x_{1},x_{2}),(y_{1},y_{2}){\bigr \rangle }_{H_{1}\oplus
      H_{2}}=\left\langle x_{1},y_{1}\right\rangle _{H_{1}}+\left\langle x_
      {2},y_{2}\right\rangle _{H_{2}}\,.}]
More generally, if Hi is a family of Hilbert spaces indexed by i â I, then
the direct sum of the Hi, denoted
          &#x2A01;  i &#x2208; I    H  i     {\displaystyle \bigoplus _{i\in
      I}H_{i}}  [{\displaystyle \bigoplus _{i\in I}H_{i}}]
consists of the set of all indexed families
         x = (  x  i   &#x2208;  H  i    |  i &#x2208; I ) &#x2208;  &#x220F;
      i &#x2208; I    H  i     {\displaystyle x=(x_{i}\in H_{i}|i\in I)\in
      \prod _{i\in I}H_{i}}  [{\displaystyle x=(x_{i}\in H_{i}|i\in I)\in \prod
      _{i\in I}H_{i}}]
in the Cartesian_product of the Hi such that
          &#x2211;  i &#x2208; I   &#x2016;  x  i    &#x2016;  2   < &#x221E;
      .   {\displaystyle \sum _{i\in I}\|x_{i}\|^{2}<\infty \,.}  [
      {\displaystyle \sum _{i\in I}\|x_{i}\|^{2}<\infty \,.}]
The inner product is defined by
         &#x27E8; x , y &#x27E9; =  &#x2211;  i &#x2208; I     &#x27E8;   x  i
      ,  y  i    &#x27E9;    H  i      .   {\displaystyle \langle x,y\rangle
      =\sum _{i\in I}\left\langle x_{i},y_{i}\right\rangle _{H_{i}}\,.}  [
      {\displaystyle \langle x,y\rangle =\sum _{i\in I}\left\langle x_{i},y_
      {i}\right\rangle _{H_{i}}\,.}]
Each of the Hi is included as a closed subspace in the direct sum of all of the
Hi. Moreover, the Hi are pairwise orthogonal. Conversely, if there is a system
of closed subspaces, Vi, i â I, in a Hilbert space H, that are pairwise
orthogonal and whose union is dense in H, then H is canonically isomorphic to
the direct sum of Vi. In this case, H is called the internal direct sum of the
Vi. A direct sum (internal or external) is also equipped with a family of
orthogonal projections Ei onto the ith direct summand Hi. These projections are
bounded, self-adjoint, idempotent operators that satisfy the orthogonality
condition
          E  i    E  j   = 0 ,  i &#x2260; j  .   {\displaystyle E_{i}E_
      {j}=0,\quad i\neq j\,.}  [{\displaystyle E_{i}E_{j}=0,\quad i\neq j\,.}]
The spectral_theorem for compact self-adjoint operators on a Hilbert space H
states that H splits into an orthogonal direct sum of the eigenspaces of an
operator, and also gives an explicit decomposition of the operator as a sum of
projections onto the eigenspaces. The direct sum of Hilbert spaces also appears
in quantum mechanics as the Fock_space of a system containing a variable number
of particles, where each Hilbert space in the direct sum corresponds to an
additional degree_of_freedom for the quantum mechanical system. In
representation_theory, the PeterâWeyl_theorem guarantees that any unitary
representation of a compact_group on a Hilbert space splits as the direct sum
of finite-dimensional representations.
**** Tensor products[edit] ****
Main article: Tensor_product_of_Hilbert_spaces
If x1, y1 â H1 and x2, y2 â H2, then one defines an inner product on the
(ordinary) tensor_product as follows. On simple_tensors, let
         &#x27E8;  x  1   &#x2297;  x  2   ,   y  1   &#x2297;  y  2   &#x27E9;
      = &#x27E8;  x  1   ,  y  1   &#x27E9;  &#x27E8;  x  2   ,  y  2
      &#x27E9;  .   {\displaystyle \langle x_{1}\otimes x_{2},\,y_{1}\otimes y_
      {2}\rangle =\langle x_{1},y_{1}\rangle \,\langle x_{2},y_{2}\rangle \,.}
      [{\displaystyle \langle x_{1}\otimes x_{2},\,y_{1}\otimes y_{2}\rangle
      =\langle x_{1},y_{1}\rangle \,\langle x_{2},y_{2}\rangle \,.}]
This formula then extends by sesquilinearity to an inner product on H1 â H2.
The Hilbertian tensor product of H1 and H2, sometimes denoted by H1
&#x2297; &#x005E;      {\displaystyle {\widehat {\otimes }}}  [\widehat
{\otimes}] H2, is the Hilbert space obtained by completing H1 â H2 for the
metric associated to this inner product.[55]
An example is provided by the Hilbert space L2([0, 1]). The Hilbertian tensor
product of two copies of L2([0, 1]) is isometrically and linearly isomorphic to
the space L2([0, 1]2) of square-integrable functions on the square [0, 1]2.
This isomorphism sends a simple tensor f1 â f2 to the function
         ( s , t ) &#x21A6;  f  1   ( s )   f  2   ( t )   {\displaystyle
      (s,t)\mapsto f_{1}(s)\,f_{2}(t)}  [{\displaystyle (s,t)\mapsto f_{1}
      (s)\,f_{2}(t)}]
on the square.
This example is typical in the following sense.[56] Associated to every simple
tensor product x1 â x2 is the rank one operator from Hâ
1 to H2 that maps a given x* â Hâ
1 as
          x  &#x2217;   &#x21A6;  x  &#x2217;   (  x  1   )  x  2    .
      {\displaystyle x^{*}\mapsto x^{*}(x_{1})x_{2}\,.}  [{\displaystyle x^
      {*}\mapsto x^{*}(x_{1})x_{2}\,.}]
This mapping defined on simple tensors extends to a linear identification
between H1 â H2 and the space of finite rank operators from Hâ
1 to H2. This extends to a linear isometry of the Hilbertian tensor product H1
&#x2297; &#x005E;      {\displaystyle {\widehat {\otimes }}}  [\widehat
{\otimes}] H2 with the Hilbert space HS(Hâ
1, H2) of HilbertâSchmidt_operators from Hâ
1 to H2.
***** Orthonormal bases[edit] *****
The notion of an orthonormal_basis from linear algebra generalizes over to the
case of Hilbert spaces.[57] In a Hilbert space H, an orthonormal basis is a
family {ek}k â B of elements of H satisfying the conditions:
   1. Orthogonality: Every two different elements of B are orthogonal: â¨ek,
      ejâ© = 0 for all k, j â B with k â  j.
   2. Normalization: Every element of the family has norm 1: ||ek|| = 1 for all
      k â B.
   3. Completeness: The linear_span of the family ek, k â B, is dense in H.
A system of vectors satisfying the first two conditions basis is called an
orthonormal system or an orthonormal set (or an orthonormal sequence if B is
countable). Such a system is always linearly_independent. Completeness of an
orthonormal system of vectors of a Hilbert space can be equivalently restated
as:
      if â¨v, ekâ© = 0 for all k â B and some v â H then v = 0.
This is related to the fact that the only vector orthogonal to a dense linear
subspace is the zero vector, for if S is any orthonormal set and v is
orthogonal to S, then v is orthogonal to the closure of the linear span of S,
which is the whole space.
Examples of orthonormal bases include:
    * the set {(1, 0, 0), (0, 1, 0), (0, 0, 1)} forms an orthonormal basis of
      â3 with the dot_product;
    * the sequence {fn : n â â¤} with fn(x) = exp(2Ïinx) forms an
      orthonormal basis of the complex space L2([0, 1]);
In the infinite-dimensional case, an orthonormal basis will not be a basis in
the sense of linear_algebra; to distinguish the two, the latter basis is also
called a Hamel_basis. That the span of the basis vectors is dense implies that
every vector in the space can be written as the sum of an infinite series, and
the orthogonality implies that this decomposition is unique.
**** Sequence spaces[edit] ****
The space l2 of square-summable sequences of complex numbers is the set of
infinite sequences
         (  c  1   ,  c  2   ,  c  3   , &#x2026; )   {\displaystyle (c_{1},c_
      {2},c_{3},\dots )}  [{\displaystyle (c_{1},c_{2},c_{3},\dots )}]
of complex numbers such that
           |  c  1   |   2   +   |  c  2   |   2   +   |  c  3   |   2   +
      &#x22EF; < &#x221E;  .   {\displaystyle \left|c_{1}\right|^{2}+\left|c_
      {2}\right|^{2}+\left|c_{3}\right|^{2}+\cdots <\infty \,.}  [
      {\displaystyle \left|c_{1}\right|^{2}+\left|c_{2}\right|^{2}+\left|c_
      {3}\right|^{2}+\cdots <\infty \,.}]
This space has an orthonormal basis:
              e  1      = ( 1 , 0 , 0 , &#x2026; )      e  2      = ( 0 , 1 , 0
      , &#x2026; )      &#xA0; &#xA0; &#x22EE;       {\displaystyle {\begin
      {aligned}e_{1}&=(1,0,0,\dots )\\e_{2}&=(0,1,0,\dots )\\&\ \ \vdots \end
      {aligned}}}  [{\displaystyle {\begin{aligned}e_{1}&=(1,0,0,\dots )\\e_
      {2}&=(0,1,0,\dots )\\&\ \ \vdots \end{aligned}}}]
More generally, if B is any set, then one can form a Hilbert space of sequences
with index set B, defined by
          l  2   ( B ) =  {  x : B   &#x2192;  x     C    |    &#x2211;  b
      &#x2208; B     |  x ( b )  |   2   < &#x221E;     }   .   {\displaystyle
      l^{2}(B)=\left\{x:B{\xrightarrow {x}}\mathbb {C} \,\left|\,\sum _{b\in
      B}\left|x(b)\right|^{2}<\infty \right.\right\}\,.}  [{\displaystyle l^{2}
      (B)=\left\{x:B{\xrightarrow {x}}\mathbb {C} \,\left|\,\sum _{b\in
      B}\left|x(b)\right|^{2}<\infty \right.\right\}\,.}]
The summation over B is here defined by
          &#x2211;  b &#x2208; B     |  x ( b )  |   2   = sup  &#x2211;  n = 1
      N     |  x (  b  n   )  |   2     {\displaystyle \sum _{b\in B}\left|x
      (b)\right|^{2}=\sup \sum _{n=1}^{N}\left|x(b_{n})\right|^{2}}  [
      {\displaystyle \sum _{b\in B}\left|x(b)\right|^{2}=\sup \sum _{n=1}^
      {N}\left|x(b_{n})\right|^{2}}]
the supremum being taken over all finite subsets of B. It follows that, for
this sum to be finite, every element of l2(B) has only countably many nonzero
terms. This space becomes a Hilbert space with the inner product
         &#x27E8; x , y &#x27E9; =  &#x2211;  b &#x2208; B   x ( b )    y ( b )
      &#x00AF;     {\displaystyle \langle x,y\rangle =\sum _{b\in B}x(b)
      {\overline {y(b)}}}  [\langle x,y\rangle =\sum _{b\in B}x(b){\overline {y
      (b)}}]
for all x, y â l2(B). Here the sum also has only countably many nonzero
terms, and is unconditionally convergent by the CauchyâSchwarz inequality.
An orthonormal basis of l2(B) is indexed by the set B, given by
          e  b    (  b &#x2032;  )  =   {    1    if&#xA0;  b =  b &#x2032;
      0    otherwise.          {\displaystyle e_{b}\left(b'\right)={\begin
      {cases}1&{\text{if }}b=b'\\0&{\text{otherwise.}}\end{cases}}}  [
      {\displaystyle e_{b}\left(b'\right)={\begin{cases}1&{\text{if }}b=b'\\0&
      {\text{otherwise.}}\end{cases}}}]
**** Bessel's inequality and Parseval's formula[edit] ****
Let f1, ..., fn be a finite orthonormal system in H. For an arbitrary vector x
â H, let
         y =  &#x2211;  j = 1   n   &#x27E8; x ,  f  j   &#x27E9;   f  j    .
      {\displaystyle y=\sum _{j=1}^{n}\langle x,f_{j}\rangle \,f_{j}\,.}  [
      {\displaystyle y=\sum _{j=1}^{n}\langle x,f_{j}\rangle \,f_{j}\,.}]
Then â¨x, fkâ© = â¨y, fkâ© for every k = 1, â¦, n. It follows that x â y
is orthogonal to each fk, hence x â y is orthogonal to y. Using the
Pythagorean identity twice, it follows that
         &#x2016; x  &#x2016;  2   = &#x2016; x &#x2212; y  &#x2016;  2   +
      &#x2016; y  &#x2016;  2   &#x2265; &#x2016; y  &#x2016;  2   =  &#x2211;
      j = 1   n     |   &#x27E8; x ,  f  j   &#x27E9;    |    2    .
      {\displaystyle \|x\|^{2}=\|x-y\|^{2}+\|y\|^{2}\geq \|y\|^{2}=\sum _{j=1}^
      {n}{\bigl |}\langle x,f_{j}\rangle {\bigr |}^{2}\,.}  [{\displaystyle
      \|x\|^{2}=\|x-y\|^{2}+\|y\|^{2}\geq \|y\|^{2}=\sum _{j=1}^{n}{\bigl
      |}\langle x,f_{j}\rangle {\bigr |}^{2}\,.}]
Let {fi}, i â I, be an arbitrary orthonormal system in H. Applying the
preceding inequality to every finite subset J of I gives Bessel's inequality:
[58]
          &#x2211;  i &#x2208; I     |   &#x27E8; x ,  f  i   &#x27E9;    |
      2   &#x2264; &#x2016; x  &#x2016;  2   ,  x &#x2208; H   {\displaystyle
      \sum _{i\in I}{\bigl |}\langle x,f_{i}\rangle {\bigr |}^{2}\leq \|x\|^
      {2},\quad x\in H}  [{\displaystyle \sum _{i\in I}{\bigl |}\langle x,f_
      {i}\rangle {\bigr |}^{2}\leq \|x\|^{2},\quad x\in H}]
(according to the definition of the sum_of_an_arbitrary_family of non-negative
real numbers).
Geometrically, Bessel's inequality implies that the orthogonal projection of x
onto the linear subspace spanned by the fi has norm that does not exceed that
of x. In two dimensions, this is the assertion that the length of the leg of a
right triangle may not exceed the length of the hypotenuse.
Bessel's inequality is a stepping stone to the stronger result called
Parseval's_identity, which governs the case when Bessel's inequality is
actually an equality. By definition, if {ek}k â B is an orthonormal basis of
H, then every element x of H may be written as
         x =  &#x2211;  k &#x2208; B    &#x27E8;  x ,  e  k    &#x27E9;    e  k
      .   {\displaystyle x=\sum _{k\in B}\left\langle x,e_{k}\right\rangle \,e_
      {k}\,.}  [{\displaystyle x=\sum _{k\in B}\left\langle x,e_
      {k}\right\rangle \,e_{k}\,.}]
Even if B is uncountable, Bessel's inequality guarantees that the expression is
well-defined and consists only of countably many nonzero terms. This sum is
called the Fourier expansion of x, and the individual coefficients â¨x, ekâ©
are the Fourier coefficients of x. Parseval's identity then asserts that
         &#x2016; x  &#x2016;  2   =  &#x2211;  k &#x2208; B    |  &#x27E8; x ,
      e  k   &#x27E9;   |   2    .   {\displaystyle \|x\|^{2}=\sum _{k\in
      B}|\langle x,e_{k}\rangle |^{2}\,.}  [{\displaystyle \|x\|^{2}=\sum _
      {k\in B}|\langle x,e_{k}\rangle |^{2}\,.}]
Conversely, if {ek} is an orthonormal set such that Parseval's identity holds
for every x, then {ek} is an orthonormal basis.
**** Hilbert dimension[edit] ****
As a consequence of Zorn's_lemma, every Hilbert space admits an orthonormal
basis; furthermore, any two orthonormal bases of the same space have the same
cardinality, called the Hilbert dimension of the space.[59] For instance, since
l2(B) has an orthonormal basis indexed by B, its Hilbert dimension is the
cardinality of B (which may be a finite integer, or a countable or uncountable
cardinal_number).
As a consequence of Parseval's identity, if {ek}k â B is an orthonormal basis
of H, then the map Î¦ : H â l2(B) defined by Î¦(x) = â¨x, ekâ©kâB is an
isometric isomorphism of Hilbert spaces: it is a bijective linear mapping such
that
           &#x27E8;   &#x03A6; ( x ) , &#x03A6; ( y )    &#x27E9;     l  2
      ( B )   =   &#x27E8;  x , y  &#x27E9;   H     {\displaystyle {\bigl
      \langle }\Phi (x),\Phi (y){\bigr \rangle }_{l^{2}(B)}=\left\langle
      x,y\right\rangle _{H}}  [{\displaystyle {\bigl \langle }\Phi (x),\Phi (y)
      {\bigr \rangle }_{l^{2}(B)}=\left\langle x,y\right\rangle _{H}}]
for all x, y â H. The cardinal_number of B is the Hilbert dimension of H.
Thus every Hilbert space is isometrically isomorphic to a sequence space l2(B)
for some set B.
**** Separable spaces[edit] ****
By definition, a Hilbert space is separable provided it contains a dense
countable subset. Along with Zorn's lemma, this means a Hilbert space is
separable if and only if it admits a countable orthonormal basis. All infinite-
dimensional separable Hilbert spaces are therefore isometrically isomorphic to
l2.any
In the past, Hilbert spaces were often required to be separable as part of the
definition.[60] Most spaces used in physics are separable, and since these are
all isomorphic to each other, one often refers to any infinite-dimensional
separable Hilbert space as "the Hilbert space" or just "Hilbert space".[61]
Even in quantum_field_theory, most of the Hilbert spaces are in fact separable,
as stipulated by the Wightman_axioms. However, it is sometimes argued that non-
separable Hilbert spaces are also important in quantum field theory, roughly
because the systems in the theory possess an infinite number of degrees_of
freedom and any infinite Hilbert_tensor_product (of spaces of dimension greater
than one) is non-separable.[62] For instance, a bosonic_field can be naturally
thought of as an element of a tensor product whose factors represent harmonic
oscillators at each point of space. From this perspective, the natural state
space of a boson might seem to be a non-separable space.[62] However, it is
only a small separable subspace of the full tensor product that can contain
physically meaningful fields (on which the observables can be defined). Another
non-separable Hilbert space models the state of an infinite collection of
particles in an unbounded region of space. An orthonormal basis of the space is
indexed by the density of the particles, a continuous parameter, and since the
set of possible densities is uncountable, the basis is not countable.[62]
***** Orthogonal complements and projections[edit] *****
If S is a subset of a Hilbert space H, the set of vectors orthogonal to S is
defined by
          S  &#x22A5;   =  {  x &#x2208; H : &#x27E8; x , s &#x27E9; = 0 &#xA0;
      &#x2200; s &#x2208; S  }   .   {\displaystyle S^{\perp }=\left\{x\in H:
      \langle x,s\rangle =0\ \forall s\in S\right\}\,.}  [{\displaystyle S^
      {\perp }=\left\{x\in H:\langle x,s\rangle =0\ \forall s\in S\right\}\,.}]
Sâ¥ is a closed subspace of H (can be proved easily using the linearity and
continuity of the inner product) and so forms itself a Hilbert space. If V is a
closed subspace of H, then Vâ¥ is called the orthogonal complement of V. In
fact, every x â H can then be written uniquely as x = v + w, with v â V and
w â Vâ¥. Therefore, H is the internal Hilbert direct sum of V and Vâ¥.
The linear operator PV : H â H that maps x to v is called the orthogonal
projection onto V. There is a natural one-to-one correspondence between the set
of all closed subspaces of H and the set of all bounded self-adjoint operators
P such that P2 = P. Specifically,
      Theorem. The orthogonal projection PV is a self-adjoint linear operator
      on H of norm â¤ 1 with the property P2
      V = PV. Moreover, any self-adjoint linear operator E such that E2 = E is
      of the form PV, where V is the range of E. For every x in H, PV(x) is the
      unique element v of V that minimizes the distance ||x â v||.
This provides the geometrical interpretation of PV(x): it is the best
approximation to x by elements of V.[63]
Projections PU and PV are called mutually orthogonal if PUPV = 0. This is
equivalent to U and V being orthogonal as subspaces of H. The sum of the two
projections PU and PV is a projection only if U and V are orthogonal to each
other, and in that case PU + PV = PU+V. The composite PUPV is generally not a
projection; in fact, the composite is a projection if and only if the two
projections commute, and in that case PUPV = PUâ©V.
By restricting the codomain to the Hilbert space V, the orthogonal projection
PV gives rise to a projection mapping Ï : H â V; it is the adjoint of the
inclusion_mapping
         i : V &#x2192; H  ,   {\displaystyle i:V\to H\,,}  [{\displaystyle i:
      V\to H\,,}]
meaning that
           &#x27E8;  i x , y  &#x27E9;   H   =   &#x27E8;  x , &#x03C0; y
      &#x27E9;   V     {\displaystyle \left\langle ix,y\right\rangle _
      {H}=\left\langle x,\pi y\right\rangle _{V}}  [{\displaystyle \left\langle
      ix,y\right\rangle _{H}=\left\langle x,\pi y\right\rangle _{V}}]
for all x â V and y â H.
The operator norm of the orthogonal projection PV onto a nonzero closed
subspace V is equal to 1:
         &#x2016;  P  V   &#x2016; =  sup  x &#x2208; H , x &#x2260; 0
      &#x2016;  P  V   x &#x2016;   &#x2016; x &#x2016;    = 1  .
      {\displaystyle \|P_{V}\|=\sup _{x\in H,x\not =0}{\frac {\|P_{V}x\|}
      {\|x\|}}=1\,.}  [{\displaystyle \|P_{V}\|=\sup _{x\in H,x\not =0}{\frac
      {\|P_{V}x\|}{\|x\|}}=1\,.}]
Every closed subspace V of a Hilbert space is therefore the image of an
operator P of norm one such that P2 = P. The property of possessing appropriate
projection operators characterizes Hilbert spaces:[64]
    * A Banach space of dimension higher than 2 is (isometrically) a Hilbert
      space if and only if, for every closed subspace V, there is an operator
      PV of norm one whose image is V such that P2
      V = PV.
While this result characterizes the metric structure of a Hilbert space, the
structure of a Hilbert space as a topological_vector_space can itself be
characterized in terms of the presence of complementary subspaces:[65]
    * A Banach space X is topologically and linearly isomorphic to a Hilbert
      space if and only if, to every closed subspace V, there is a closed
      subspace W such that X is equal to the internal direct sum V â W.
The orthogonal complement satisfies some more elementary results. It is a
monotone_function in the sense that if U â V, then Vâ¥ â Uâ¥ with
equality holding if and only if V is contained in the closure of U. This result
is a special case of the HahnâBanach_theorem. The closure of a subspace can
be completely characterized in terms of the orthogonal complement: if V is a
subspace of H, then the closure of V is equal to Vâ¥â¥. The orthogonal
complement is thus a Galois_connection on the partial_order of subspaces of a
Hilbert space. In general, the orthogonal complement of a sum of subspaces is
the intersection of the orthogonal complements:[66]
           (   &#x2211;  i    V  i    )   &#x22A5;   =  &#x22C2;  i    V  i
      &#x22A5;    .   {\displaystyle \left(\sum _{i}V_{i}\right)^{\perp
      }=\bigcap _{i}V_{i}^{\perp }\,.}  [{\displaystyle \left(\sum _{i}V_
      {i}\right)^{\perp }=\bigcap _{i}V_{i}^{\perp }\,.}]
If the Vi are in addition closed, then
             &#x2211;  i    V  i   &#x22A5;    &#x00AF;   =   (   &#x22C2;  i
      V  i    )   &#x22A5;    .   {\displaystyle {\overline {\sum _{i}V_{i}^
      {\perp }}}=\left(\bigcap _{i}V_{i}\right)^{\perp }\,.}  [{\displaystyle
      {\overline {\sum _{i}V_{i}^{\perp }}}=\left(\bigcap _{i}V_{i}\right)^
      {\perp }\,.}]
***** Spectral theory[edit] *****
There is a well-developed spectral_theory for self-adjoint operators in a
Hilbert space, that is roughly analogous to the study of symmetric_matrices
over the reals or self-adjoint matrices over the complex numbers.[67] In the
same sense, one can obtain a "diagonalization" of a self-adjoint operator as a
suitable sum (actually an integral) of orthogonal projection operators.
The spectrum_of_an_operator T, denoted Ï(T), is the set of complex numbers Î»
such that T â Î» lacks a continuous inverse. If T is bounded, then the
spectrum is always a compact_set in the complex plane, and lies inside the disc
|z| â¤ ||T||. If T is self-adjoint, then the spectrum is real. In fact, it is
contained in the interval [m, M] where
         m =  inf  &#x2016; x &#x2016; = 1   &#x27E8; T x , x &#x27E9;  ,  M =
      sup  &#x2016; x &#x2016; = 1   &#x27E8; T x , x &#x27E9;  .
      {\displaystyle m=\inf _{\|x\|=1}\langle Tx,x\rangle \,,\quad M=\sup _
      {\|x\|=1}\langle Tx,x\rangle \,.}  [{\displaystyle m=\inf _
      {\|x\|=1}\langle Tx,x\rangle \,,\quad M=\sup _{\|x\|=1}\langle
      Tx,x\rangle \,.}]
Moreover, m and M are both actually contained within the spectrum.
The eigenspaces of an operator T are given by
          H  &#x03BB;   = ker &#x2061; ( T &#x2212; &#x03BB; )  .
      {\displaystyle H_{\lambda }=\ker(T-\lambda )\,.}  [{\displaystyle H_
      {\lambda }=\ker(T-\lambda )\,.}]
Unlike with finite matrices, not every element of the spectrum of T must be an
eigenvalue: the linear operator T â Î» may only lack an inverse because it is
not surjective. Elements of the spectrum of an operator in the general sense
are known as spectral values. Since spectral values need not be eigenvalues,
the spectral decomposition is often more subtle than in finite dimensions.
However, the spectral_theorem of a self-adjoint operator T takes a particularly
simple form if, in addition, T is assumed to be a compact_operator. The
spectral_theorem_for_compact_self-adjoint_operators states:[68]
    * A compact self-adjoint operator T has only countably (or finitely) many
      spectral values. The spectrum of T has no limit_point in the complex
      plane except possibly zero. The eigenspaces of T decompose H into an
      orthogonal direct sum:
               H =  &#x2A01;  &#x03BB; &#x2208; &#x03C3; ( T )    H  &#x03BB;
            .   {\displaystyle H=\bigoplus _{\lambda \in \sigma (T)}H_{\lambda
            }\,.}  [{\displaystyle H=\bigoplus _{\lambda \in \sigma (T)}H_
            {\lambda }\,.}]
      Moreover, if EÎ» denotes the orthogonal projection onto the eigenspace
      HÎ», then
               T =  &#x2211;  &#x03BB; &#x2208; &#x03C3; ( T )   &#x03BB;  E
            &#x03BB;    ,   {\displaystyle T=\sum _{\lambda \in \sigma
            (T)}\lambda E_{\lambda }\,,}  [{\displaystyle T=\sum _{\lambda \in
            \sigma (T)}\lambda E_{\lambda }\,,}]
      where the sum converges with respect to the norm on B(H).
This theorem plays a fundamental role in the theory of integral_equations, as
many integral operators are compact, in particular those that arise from
HilbertâSchmidt_operators.
The general spectral theorem for self-adjoint operators involves a kind of
operator-valued RiemannâStieltjes_integral, rather than an infinite
summation.[69] The spectral family associated to T associates to each real
number Î» an operator EÎ», which is the projection onto the nullspace of the
operator (T â Î»)+, where the positive part of a self-adjoint operator is
defined by
          A  +   =    1 2     (     A  2     + A  )   .   {\displaystyle A^{+}=
      {\tfrac {1}{2}}\left({\sqrt {A^{2}}}+A\right)\,.}  [{\displaystyle A^{+}=
      {\tfrac {1}{2}}\left({\sqrt {A^{2}}}+A\right)\,.}]
The operators EÎ» are monotone increasing relative to the partial order defined
on self-adjoint operators; the eigenvalues correspond precisely to the jump
discontinuities. One has the spectral theorem, which asserts
         T =  &#x222B;   R    &#x03BB;   d   E  &#x03BB;    .   {\displaystyle
      T=\int _{\mathbb {R} }\lambda \,\mathrm {d} E_{\lambda }\,.}  [
      {\displaystyle T=\int _{\mathbb {R} }\lambda \,\mathrm {d} E_{\lambda
      }\,.}]
The integral is understood as a RiemannâStieltjes integral, convergent with
respect to the norm on B(H). In particular, one has the ordinary scalar-valued
integral representation
         &#x27E8; T x , y &#x27E9; =  &#x222B;   R    &#x03BB;   d  &#x27E8;  E
      &#x03BB;   x , y &#x27E9;  .   {\displaystyle \langle Tx,y\rangle =\int _
      {\mathbb {R} }\lambda \,\mathrm {d} \langle E_{\lambda }x,y\rangle \,.}
      [{\displaystyle \langle Tx,y\rangle =\int _{\mathbb {R} }\lambda
      \,\mathrm {d} \langle E_{\lambda }x,y\rangle \,.}]
A somewhat similar spectral decomposition holds for normal operators, although
because the spectrum may now contain non-real complex numbers, the operator-
valued Stieltjes measure dEÎ» must instead be replaced by a resolution_of_the
identity.
A major application of spectral methods is the spectral_mapping_theorem, which
allows one to apply to a self-adjoint operator T any continuous complex
function f defined on the spectrum of T by forming the integral
         f ( T ) =  &#x222B;  &#x03C3; ( T )   f ( &#x03BB; )   d   E  &#x03BB;
      .   {\displaystyle f(T)=\int _{\sigma (T)}f(\lambda )\,\mathrm {d} E_
      {\lambda }\,.}  [{\displaystyle f(T)=\int _{\sigma (T)}f(\lambda
      )\,\mathrm {d} E_{\lambda }\,.}]
The resulting continuous_functional_calculus has applications in particular to
pseudodifferential_operators.[70]
The spectral theory of unbounded self-adjoint operators is only marginally more
difficult than for bounded operators. The spectrum of an unbounded operator is
defined in precisely the same way as for bounded operators: Î» is a spectral
value if the resolvent_operator
          R  &#x03BB;   = ( T &#x2212; &#x03BB;  )  &#x2212; 1
      {\displaystyle R_{\lambda }=(T-\lambda )^{-1}}  [{\displaystyle R_
      {\lambda }=(T-\lambda )^{-1}}]
fails to be a well-defined continuous operator. The self-adjointness of T still
guarantees that the spectrum is real. Thus the essential idea of working with
unbounded operators is to look instead at the resolvent RÎ» where Î» is
nonreal. This is a bounded normal operator, which admits a spectral
representation that can then be transferred to a spectral representation of T
itself. A similar strategy is used, for instance, to study the spectrum of the
Laplace operator: rather than address the operator directly, one instead looks
as an associated resolvent such as a Riesz_potential or Bessel_potential.
A precise version of the spectral theorem in this case is:[71]
      Given a densely defined self-adjoint operator T on a Hilbert space H,
      there corresponds a unique resolution_of_the_identity E on the Borel sets
      of â, such that
               &#x27E8; T x , y &#x27E9; =  &#x222B;   R    &#x03BB;   d   E  x
            , y   ( &#x03BB; )   {\displaystyle \langle Tx,y\rangle =\int _
            {\mathbb {R} }\lambda \,\mathrm {d} E_{x,y}(\lambda )}  [
            {\displaystyle \langle Tx,y\rangle =\int _{\mathbb {R} }\lambda
            \,\mathrm {d} E_{x,y}(\lambda )}]
      for all x â D(T) and y â H. The spectral measure E is concentrated on
      the spectrum of T.
There is also a version of the spectral theorem that applies to unbounded
normal operators.
***** In popular culture[edit] *****
Thomas_Pynchon introduced the fictional character, Sammy Hilbert-Spaess (a pun
on "Hilbert Space"), in his 1973 novel, Gravity's_Rainbow. Hilbert-Spaess is
first described as a "a ubiquitous double agent" and later as "at least a
double agent". The novel had earlier referenced the work of fellow German
mathematician Kurt_GÃ¶del's Incompleteness_Theorems which showed that Hilbert's
Program, Hilbert's formalized plan to unify mathematics into a single set of
axioms, was not possible.[72][73][74]
***** See also[edit] *****
    * [icon]Mathematics_portal
    * Hadamard_space
    * Hilbert_algebra
    * Hilbert_C*-module
    * Hilbert_manifold
    * Operator_theory
    * Operator_topologies
    * Rigged_Hilbert_space
***** Remarks[edit] *****
   1. ^ In some conventions, inner products are linear in their second
      arguments instead.
   2. ^ The eigenvalues of the Fredholm kernel are 1/Î», which tend to zero.
***** Notes[edit] *****
   1. ^ Marsden_1974, Â§2.8
   2. ^ The mathematical material in this section can be found in any good
      textbook on functional analysis, such as DieudonnÃ©_(1960), Hewitt_&
      Stromberg_(1965), Reed_&_Simon_(1980) or Rudin_(1980).
   3. ^ DieudonnÃ©_1960, Â§6.2
   4. ^ DieudonnÃ©_1960
   5. ^ Largely from the work of Hermann_Grassmann, at the urging of August
      Ferdinand_MÃ¶bius (Boyer_&_Merzbach_1991, pp. 584â586). The first
      modern axiomatic account of abstract vector spaces ultimately appeared in
      Giuseppe_Peano's 1888 account (Grattan-Guinness_2000, Â§5.2.2; O'Connor_&
      Robertson_1996).
   6. ^ A detailed account of the history of Hilbert spaces can be found in
      Bourbaki_1987.
   7. ^ Schmidt_1908
   8. ^ Titchmarsh_1946, Â§IX.1
   9. ^ Lebesgue_1904. Further details on the history of integration theory can
      be found in Bourbaki_(1987) and Saks_(2005).
  10. ^ Bourbaki_1987.
  11. ^ Dunford_&_Schwartz_1958, Â§IV.16
  12. ^ In Dunford_&_Schwartz_(1958, Â§IV.16), the result that every linear
      functional on L2[0,1] is represented by integration is jointly attributed
      to FrÃ©chet_(1907) and Riesz_(1907). The general result, that the dual of
      a Hilbert space is identified with the Hilbert space itself, can be found
      in Riesz_(1934).
  13. ^ von_Neumann_1929.
  14. ^ Kline_1972, p. 1092
  15. ^ Hilbert,_Nordheim_&_von_Neumann_1927
  16. ^ a b Weyl_1931.
  17. ^ PrugoveÄki_1981, pp. 1â10.
  18. ^ a b von_Neumann_1932
  19. ^ Halmos_1957, Section 42.
  20. ^ Hewitt_&_Stromberg_1965.
  21. ^ a b Bers,_John_&_Schechter_1981.
  22. ^ Giusti_2003.
  23. ^ Stein_1970
  24. ^ Details can be found in Warner_(1983).
  25. ^ A general reference on Hardy spaces is the book Duren_(1970).
  26. ^ Krantz_2002, Â§1.4
  27. ^ Krantz_2002, Â§1.5
  28. ^ Young_1988, Chapter 9.
  29. ^ More detail on finite element methods from this point of view can be
      found in Brenner_&_Scott_(2005).
  30. ^ Reed_&_Simon_1980
  31. ^ A treatment of Fourier series from this point of view is available, for
      instance, in Rudin_(1987) or Folland_(2009).
  32. ^ Halmos_1957, Â§5
  33. ^ Bachman,_Narici_&_Beckenstein_2000
  34. ^ Stein_&_Weiss_1971, Â§IV.2.
  35. ^ Lancos_1988, pp. 212â213
  36. ^ Lanczos_1988, Equation 4-3.10
  37. ^ The classic reference for spectral methods is Courant_&_Hilbert_1953. A
      more up-to-date account is Reed_&_Simon_1975.
  38. ^ Kac_1966
  39. ^ von_Neumann_1955
  40. ^ Young_1988, p. 23.
  41. ^ Clarkson_1936.
  42. ^ Rudin_1987, Theorem 4.10
  43. ^ Dunford_&_Schwartz_1958, II.4.29
  44. ^ Rudin_1987, Theorem 4.11
  45. ^Blanchet, GÃ©rard; Charbit, Maurice (2014). Digital Signal and Image
      Processing Using MATLAB. Digital Signal and Image Processing. 1 (Second
      ed.). New Jersey: Wiley. pp. 349â360. ISBN 978-1848216402.
  46. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
  47. ^ Weidmann_1980, Theorem 4.8
  48. ^ Weidmann_1980, Â§4.5
  49. ^ Buttazzo,_Giaquinta_&_Hildebrandt_1998, Theorem 5.17
  50. ^ Halmos_1982, Problem 52, 58
  51. ^ Rudin_1973
  52. ^ TrÃ¨ves_1967, Chapter 18
  53. ^ See PrugoveÄki_(1981), Reed_&_Simon_(1980, Chapter VIII) and Folland_
      (1989).
  54. ^ PrugoveÄki_1981, III, Â§1.4
  55. ^ Dunford_&_Schwartz_1958, IV.4.17-18
  56. ^ Weidmann_1980, Â§3.4
  57. ^ Kadison_&_Ringrose_1983, Theorem 2.6.4
  58. ^ Dunford_&_Schwartz_1958, Â§IV.4.
  59. ^ For the case of finite index sets, see, for instance, Halmos_1957, Â§5.
      For infinite index sets, see Weidmann_1980, Theorem 3.6.
  60. ^ Levitan_2001. Many authors, such as Dunford_&_Schwartz_(1958, Â§IV.4),
      refer to this just as the dimension. Unless the Hilbert space is finite
      dimensional, this is not the same thing as its dimension as a linear
      space (the cardinality of a Hamel basis).
  61. ^ PrugoveÄki_1981, I, Â§4.2
  62. ^ von_Neumann_(1955) defines a Hilbert space via a countable Hilbert
      basis, which amounts to an isometric isomorphism with l2. The convention
      still persists in most rigorous treatments of quantum mechanics; see for
      instance Sobrino_1996, Appendix B.
  63. ^ a b c Streater_&_Wightman_1964, pp. 86â87
  64. ^ Young_1988, Theorem 15.3
  65. ^ Kakutani_1939
  66. ^ Lindenstrauss_&_Tzafriri_1971
  67. ^ Halmos_1957, Â§12
  68. ^ A general account of spectral theory in Hilbert spaces can be found in
      Riesz_&_Sz_Nagy_(1990). A more sophisticated account in the language of
      C*-algebras is in Rudin_(1973) or Kadison_&_Ringrose_(1997)
  69. ^ See, for instance, Riesz_&_Sz_Nagy_(1990, Chapter VI) or Weidmann_1980,
      Chapter 7. This result was already known to Schmidt_(1907) in the case of
      operators arising from integral kernels.
  70. ^ Riesz_&_Sz_Nagy_1990, Â§Â§107â108
  71. ^ Shubin_1987
  72. ^ Rudin_1973, Theorem 13.30.
  73. ^"H_-_Thomas_Pynchon_Wiki_|_Gravity's_Rainbow". gravitys-
      rainbow.pynchonwiki.com. Retrieved 2018-10-23.
  74. ^"G_-_Thomas_Pynchon_Wiki_|_Gravity's_Rainbow". gravitys-
      rainbow.pynchonwiki.com. Retrieved 2018-10-23.
  75. ^Thomas, Pynchon (1973). Gravity's Rainbow. Viking Press. pp. 217, 275.
      ISBN 978-0143039945.
***** References[edit] *****
    * Bachman, George; Narici, Lawrence; Beckenstein, Edward (2000), Fourier
      and wavelet analysis, Universitext, Berlin, New York: Springer-Verlag,
      ISBN 978-0-387-98899-3, MR 1729490
.
Bers,_Lipman; John,_Fritz; Schechter, Martin (1981), Partial differential
equations, American Mathematical Society, ISBN 978-0-8218-0049-2
.
Bourbaki,_Nicolas (1986), Spectral theories, Elements of mathematics, Berlin:
Springer-Verlag, ISBN 978-0-201-00767-1
.
Bourbaki,_Nicolas (1987), Topological vector spaces, Elements of mathematics,
Berlin: Springer-Verlag, ISBN 978-3-540-13627-9
.
Boyer,_Carl_Benjamin; Merzbach,_Uta_C (1991), A_History_of_Mathematics (2nd
ed.), John Wiley & Sons, Inc., ISBN 978-0-471-54397-8
.
Brenner, S.; Scott, R. L. (2005), The Mathematical Theory of Finite Element
Methods (2nd ed.), Springer, ISBN 978-0-387-95451-6
.
Buttazzo, Giuseppe; Giaquinta, Mariano; Hildebrandt, Stefan (1998), One-
dimensional variational problems, Oxford Lecture Series in Mathematics and its
Applications, 15, The Clarendon Press Oxford University Press, ISBN 978-0-19-
850465-8, MR 1694383
.
Clarkson, J. A. (1936), "Uniformly convex spaces", Trans. Amer. Math. Soc., 40
(3): 396â414, doi:10.2307/1989630, JSTOR 1989630
.
Courant,_Richard; Hilbert,_David (1953), Methods of Mathematical Physics, Vol.
I, Interscience
.
DieudonnÃ©,_Jean (1960), Foundations of Modern Analysis, Academic Press
.
Dirac,_P.A.M. (1930), Principles_of_Quantum_Mechanics, Oxford: Clarendon Press
.
Dunford, N.; Schwartz,_J.T. (1958), Linear operators, Parts I and II, Wiley-
Interscience
.
Duren, P. (1970), Theory of Hp-Spaces, New York: Academic Press
.
Folland, Gerald B. (2009), Fourier_analysis_and_its_application (Reprint of
Wadsworth and Brooks/Cole 1992 ed.), American Mathematical Society Bookstore,
ISBN 978-0-8218-4790-9
.
Folland, Gerald B. (1989), Harmonic analysis in phase space, Annals of
Mathematics Studies, 122, Princeton University Press, ISBN 978-0-691-08527-2
.
FrÃ©chet, Maurice (1907), "Sur les ensembles de fonctions et les opÃ©rations
linÃ©aires", C. R. Acad. Sci. Paris, 144: 1414â1416
.
FrÃ©chet, Maurice (1904â1907), Sur les opÃ©rations linÃ©aires
.
Giusti, Enrico (2003), Direct Methods in the Calculus of Variations, World
Scientific, ISBN 978-981-238-043-2
.
Grattan-Guinness, Ivor (2000), The search for mathematical roots, 1870â1940,
Princeton Paperbacks, Princeton_University_Press, ISBN 978-0-691-05858-0,
MR 1807717
.
Halmos,_Paul (1957), Introduction to Hilbert Space and the Theory of Spectral
Multiplicity, Chelsea Pub. Co
Halmos,_Paul (1982), A Hilbert Space Problem Book, Springer-Verlag, ISBN 978-0-
387-90685-0
.
Hewitt, Edwin; Stromberg, Karl (1965), Real and Abstract Analysis, New York:
Springer-Verlag
.
Hilbert,_David; Nordheim,_Lothar_(Wolfgang); von_Neumann,_John (1927), "Ãber
die_Grundlagen_der_Quantenmechanik", Mathematische Annalen, 98: 1â30, doi:
10.1007/BF01451579
[dead_link].
Kac,_Mark (1966), "Can one hear the shape of a drum?", American_Mathematical
Monthly, 73 (4, part 2): 1â23, doi:10.2307/2313748, JSTOR 2313748
.
Kadison, Richard V.; Ringrose, John R. (1997), Fundamentals of the theory of
operator algebras. Vol. I, Graduate Studies in Mathematics, 15, Providence,
R.I.: American_Mathematical_Society, ISBN 978-0-8218-0819-1, MR 1468229
.
Kakutani,_Shizuo (1939), "Some characterizations of Euclidean space", Japanese
Journal of Mathematics, 16: 93â97, MR 0000895
.
Kline,_Morris (1972), Mathematical_thought_from_ancient_to_modern_times,_Volume
3 (3rd ed.), Oxford_University_Press (published 1990), ISBN 978-0-19-506137-6
.
Kolmogorov,_Andrey; Fomin,_Sergei_V. (1970), Introductory_Real_Analysis
(Revised English edition, trans. by Richard A. Silverman (1975) ed.), Dover
Press, ISBN 978-0-486-61226-3
.
Krantz,_Steven_G. (2002), Function Theory of Several Complex Variables,
Providence, R.I.: American_Mathematical_Society, ISBN 978-0-8218-2724-6
.
Lanczos, Cornelius (1988), Applied_analysis (Reprint of 1956 Prentice-Hall
ed.), Dover Publications, ISBN 978-0-486-65656-4
.
Lindenstrauss, J.; Tzafriri, L. (1971), "On the complemented subspaces
problem", Israel Journal of Mathematics, 9 (2): 263â269, doi:10.1007/
BF02771592, ISSN 0021-2172, MR 0276734
.
O'Connor,_John_J.; Robertson,_Edmund_F. (1996), "Abstract_linear_spaces",
MacTutor_History_of_Mathematics_archive, University_of_St_Andrews
..
Lebesgue, Henri (1904), LeÃ§ons_sur_l'intÃ©gration_et_la_recherche_des
fonctions_primitives, Gauthier-Villars
.
B.M. Levitan (2001) [1994], "Hilbert_space", in Hazewinkel,_Michiel (ed.),
Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. / Kluwer
Academic Publishers, ISBN 978-1-55608-010-4
.
Marsden,_Jerrold_E. (1974), Elementary classical analysis, W. H. Freeman and
Co., MR 0357693
.
von_Neumann,_John (1929), "Allgemeine Eigenwerttheorie Hermitescher
Funktionaloperatoren", Mathematische Annalen, 102: 49â131, doi:10.1007/
BF01782338
.
von_Neumann,_John (1932), "Physical Applications of the Ergodic Hypothesis",
Proc Natl Acad Sci USA, 18 (3): 263â266, Bibcode:1932PNAS...18..263N, doi:
10.1073/pnas.18.3.263, JSTOR 86260, PMC 1076204, PMID 16587674
.
von_Neumann,_John (1932), Mathematical_Foundations_of_Quantum_Mechanics,
Princeton Landmarks in Mathematics, Princeton_University_Press (published
1996), ISBN 978-0-691-02893-4, MR 1435976
.
PrugoveÄki, Eduard (1981), Quantum mechanics in Hilbert space (2nd ed.), Dover
(published 2006), ISBN 978-0-486-45327-9
.
Reed,_Michael; Simon,_Barry (1980), Functional Analysis, Methods of Modern
Mathematical Physics, Academic Press, ISBN 978-0-12-585050-6
.
Reed,_Michael; Simon,_Barry (1975), Fourier Analysis, Self-Adjointness, Methods
of Modern Mathematical Physics, Academic Press, ISBN 9780125850025
.
Riesz,_Frigyes (1907), "Sur une espÃ¨ce de GÃ©omÃ©trie analytique des systÃ¨mes
de fonctions sommables", C. R. Acad. Sci. Paris, 144: 1409â1411
.
Riesz,_Frigyes (1934), "Zur Theorie des Hilbertschen Raumes", Acta Sci. Math.
Szeged, 7: 34â38
.
Riesz,_Frigyes; Sz.-Nagy,_BÃ©la (1990), Functional analysis, Dover, ISBN 978-0-
486-66289-3
.
Rudin,_Walter (1973), Functional analysis, Tata MacGraw-Hill
.
Rudin,_Walter (1987), Real and Complex Analysis, McGraw-Hill, ISBN 978-0-07-
100276-9
.
Saks,_StanisÅaw (2005), Theory of the integral (2nd Dover ed.), Dover,
ISBN 978-0-486-44648-6
; originally published Monografje Matematyczne, vol. 7, Warszawa, 1937.
Schmidt,_Erhard (1908), "Ãber die AuflÃ¶sung linearer Gleichungen mit
unendlich vielen Unbekannten", Rend. Circ. Mat. Palermo, 25: 63â77, doi:
10.1007/BF03029116
.
Shubin, M. A. (1987), Pseudodifferential operators and spectral theory,
Springer Series in Soviet Mathematics, Berlin, New York: Springer-Verlag,
ISBN 978-3-540-13621-7, MR 0883081
.
Sobrino, Luis (1996), Elements of non-relativistic quantum mechanics, River
Edge, New Jersey: World Scientific Publishing Co. Inc., Bibcode:
1996lnrq.book.....S, doi:10.1142/2865, ISBN 978-981-02-2386-1, MR 1626401
.
Stewart, James (2006), Calculus: Concepts and Contexts (3rd ed.), Thomson/
Brooks/Cole
.
Stein, E (1970), Singular Integrals and Differentiability Properties of
Functions, Princeton Univ. Press, ISBN 978-0-691-08079-6
.
Stein,_Elias; Weiss,_Guido (1971), Introduction to Fourier Analysis on
Euclidean Spaces, Princeton, N.J.: Princeton University Press, ISBN 978-0-691-
08078-9
.
Streater,_Ray; Wightman,_Arthur (1964), PCT, Spin and Statistics and All That,
W. A. Benjamin, Inc
.
Teschl,_Gerald (2009). Mathematical_Methods_in_Quantum_Mechanics;_With
Applications_to_SchrÃ¶dinger_Operators. Providence: American_Mathematical
Society. ISBN 978-0-8218-4660-5.
.
Titchmarsh,_Edward_Charles (1946), Eigenfunction expansions, part 1, Oxford
University: Clarendon Press
.
TrÃ¨ves, FranÃ§ois (1967), Topological Vector Spaces, Distributions and
Kernels, Academic Press
.
Warner, Frank (1983), Foundations of Differentiable Manifolds and Lie Groups,
Berlin, New York: Springer-Verlag, ISBN 978-0-387-90894-6
.
Weidmann, Joachim (1980), Linear operators in Hilbert spaces, Graduate Texts in
Mathematics, 68, Berlin, New York: Springer-Verlag, ISBN 978-0-387-90427-6,
MR 0566954
.
Weyl,_Hermann (1931), The Theory of Groups and Quantum Mechanics (English 1950
ed.), Dover Press, ISBN 978-0-486-60269-1
.
Young, Nicholas (1988), An introduction to Hilbert space, Cambridge University
Press, ISBN 978-0-521-33071-8, Zbl 0645.46024
.
***** External links[edit] *****
 Wikibooks has a book on the topic of: Functional_Analysis/Hilbert_spaces
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Hilbert_space", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Hilbert_space_at_Mathworld
245B,_notes_5:_Hilbert_spaces by Terence_Tao
    * v
    * t
    * e
Functional_analysis (topics)
                       * Asplund
                       * Banach (list)
                       * Banach_Lattice
                       * Barrelled
                       * Bornological
                       * Brauner
                       * F-space
                       * Finite-dimensional
                       * FrÃ©chet (tame)
                       * Hilbert (pre-Hilbert
                       * Polarization_identity)
                       * LF-space
TVS types              * Locally_convex (Seminorms/Minkowski_functionals)
                       * Mackey
                       * Montel
                       * Nuclear
                       * Normed (norm)
                       * Quasinormed
                       * Reflexive
                       * Riesz
                       * Smith
                       * Stereotype
                       * Strictly_convex
                       * Webbed
                       * Topological_tensor_product (of_Hilbert_spaces)
                       * Dual
                       * Dual_space (Dual_norm)
                       * Operator
                       * Ultraweak
                       * Weak (polar
Mapping topologies     * operator)
                       * Mackey
                       * Strong (polar
                       * operator)
                       * Ultrastrong
                       * Uniform_convergence
                       * Adjoint
                       * Bilinear (form
                       * operator
                       * sesquilinear)
                       * (Un)Bounded
                       * Closed
                       * Compact (on_Hilbert_spaces)
                       * (Dis)Continuous
                       * Densely_defined
Linear_operators       * Fredholm
                       * HilbertâSchmidt
                       * Functionals (positive)
                       * Normal
                       * Nuclear
                       * Self-adjoint
                       * Strictly_singular
                       * Trace_class
                       * Transpose
                       * Unitary
                       * Banach_algebras
                       * C*-algebras
                       * Spectrum (C*-algebra
Operator_theory        * radius)
                       * Spectral_theory (of_ODEs
                       * Spectral_theorem)
                       * Polar_decomposition
                       * Singular_value_decomposition
                       * BanachâAlaoglu
                       * BanachâMazur
                       * BanachâSaks
                       * BanachâSchauder_(open_mapping)
                       * BanachâSteinhaus_(Uniform_boundedness)
                       * Bessel's_inequality
                       * CauchyâSchwarz_inequality
                       * Closed_graph
                       * Closed_range
                       * EberleinâÅ mulian
                       * Freudenthal_spectral
Theorems               * GelfandâMazur
                       * GelfandâNaimark
                       * Goldstine
                       * HahnâBanach (hyperplane_separation)
                       * Kakutani_fixed-point
                       * KreinâMilman
                       * Lomonosov's_invariant_subspace
                       * MackeyâArens
                       * Mazur's_lemma
                       * M._Riesz_extension
                       * Riesz_representation
                       * Parseval's_identity
                       * Schauder_fixed-point
                       * Abstract_Wiener_space
                       * Bochner_space
                       * Differentiation_in_FrÃ©chet_spaces
                       * Derivatives (FrÃ©chet
                       * Gateaux
                       * functional
                       * holomorphic)
                       * Integrals (Bochner
                       * Dunford
                       * GelfandâPettis
Analysis               * regulated
                       * PaleyâWiener
                       * weak)
                       * Functional_calculus (Borel
                       * continuous
                       * holomorphic)
                       * Inverse_function_theorem (NashâMoser_theorem)
                       * Measures (Lebesgue
                       * Projection-valued
                       * Vector)
                       * Weakly_measurable_function
                       * Absolutely_convex
                       * Absorbing
                       * Balanced
                       * Bounded
                       * Convex
Types of sets          * Convex_cone_(subset)
                       * Linear_cone_(subset)
                       * Radial
                       * Star-shaped
                       * Symmetric
                       * Zonotope
                       * Algebraic_interior_(core)
                       * Bounding_points
Subsets / set         * Convex_hull
operations             * Extreme_point
                       * Interior
                       * Minkowski_addition
                       * Polar
                                              * GND: 4159850-7
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85060803
                                              * NDL: 00563198

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Hilbert_space&oldid=909691430"
Categories:
    * Hilbert_space
    * Linear_algebra
    * Operator_theory
    * Quantum_mechanics
    * Functional_analysis
    * David_Hilbert
Hidden categories:
    * Articles_with_short_description
    * Wikipedia_indefinitely_move-protected_pages
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_July_2016
    * Good_articles
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Italiano
    * ×¢××¨××ª
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Ù¾ÙØ¬Ø§Ø¨Û
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 00:12 (UTC).
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
