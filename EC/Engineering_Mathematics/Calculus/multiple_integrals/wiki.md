The following text has been accessed from https://en.wikipedia.org/wiki/Multiple_integral at Fri Aug 9 03:41:19 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Multiple integral ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Part of a series of articles about
Calculus
    * Fundamental_theorem
    * Limits_of_functions
    * Continuity
    * Mean_value_theorem
    * Rolle's_theorem
Differential
Definitions
    * Derivative (generalizations)
    * Differential
          o infinitesimal
          o of_a_function
          o total
Concepts
    * Differentiation_notation
    * Second_derivative
    * Third_derivative
    * Change_of_variables
    * Implicit_differentiation
    * Related_rates
    * Taylor's_theorem
Rules_and_identities
    * Sum
    * Product
    * Chain
    * Power
    * Quotient
    * Inverse
    * General_Leibniz
    * FaÃ _di_Bruno's_formula
Integral
    * Lists_of_integrals
Definitions
    * Antiderivative
    * Integral (improper)
    * Riemann_integral
    * Lebesgue_integration
    * Contour_integration
Integration by
    * Parts
    * Discs
    * Cylindrical_shells
    * Substitution (trigonometric)
    * Partial_fractions
    * Order
    * Reduction_formulae
Series
    * Geometric (arithmetico-geometric)
    * Harmonic
    * Alternating
    * Power
    * Binomial
    * Taylor
Convergence_tests
    * Summand_limit_(term_test)
    * Ratio
    * Root
    * Integral
    * Direct_comparison
    *
      Limit_comparison
    * Alternating_series
    * Cauchy_condensation
    * Dirichlet
    * Abel
Vector
    * Gradient
    * Divergence
    * Curl
    * Laplacian
    * Directional_derivative
    * Identities
Theorems
    * Divergence
    * Gradient
    * Green's
    * KelvinâStokes
    * Stokes
Multivariable
Formalisms
    * Matrix
    * Tensor
    * Exterior
    * Geometric
Definitions
    * Partial_derivative
    * Multiple integral
    * Line_integral
    * Surface_integral
    * Volume_integral
    * Jacobian
    * Hessian
Specialized
    * Fractional
    * Malliavin
    * Stochastic
    * Variations
Glossary_of_calculus
    * Glossary_of_calculus
    * v
    * t
    * e
Integral as area between two curves.
Double integral as volume under a surface z = 10 â x2 â y2/8. The
rectangular region at the bottom of the body is the domain of integration,
while the surface is the graph of the two-variable function to be integrated.
The multiple integral is a definite_integral of a function of more than one
real variable, for example, f(x, y) or f(x, y, z). Integrals of a function of
two variables over a region in R2 are called double_integrals, and integrals of
a function of three variables over a region of R3 are called triple_integrals.
[1]
⁰
***** Contents *****
    * 1_Introduction
    * 2_Mathematical_definition
          o 2.1_Properties
          o 2.2_Particular_cases
    * 3_Methods_of_integration
          o 3.1_Integrating_constant_functions
          o 3.2_Use_of_symmetry
          o 3.3_Normal_domains_on_R2
                # 3.3.1_x-axis
                # 3.3.2_y-axis
                # 3.3.3_Normal_domains_on_R3
          o 3.4_Change_of_variables
                # 3.4.1_Polar_coordinates
                # 3.4.2_Cylindrical_coordinates
                # 3.4.3_Spherical_coordinates
    * 4_Examples
          o 4.1_Double_integral_over_a_rectangle
          o 4.2_Double_integral_over_a_normal_domain
          o 4.3_Calculating_volume
    * 5_Multiple_improper_integral
    * 6_Multiple_integrals_and_iterated_integrals
    * 7_Some_practical_applications
    * 8_See_also
    * 9_References
    * 10_Further_reading
    * 11_External_links
***** Introduction[edit] *****
Just as the definite integral of a positive function of one variable represents
the area of the region between the graph of the function and the x-axis, the
double integral of a positive function of two variables represents the volume
of the region between the surface defined by the function (on the three-
dimensional Cartesian_plane where z = f(x, y) and the plane which contains its
domain. [1] If there are more variables, a multiple integral will yield
hypervolumes of multidimensional functions.
Multiple integration of a function in n variables: f(x1, x2, ..., xn) over a
domain D is most commonly represented by nested integral signs in the reverse
order of execution (the leftmost integral sign is computed last), followed by
the function and integrand arguments in proper order (the integral with respect
to the rightmost argument is computed last). The domain of integration is
either represented symbolically for every argument over each integral sign, or
is abbreviated by a variable at the rightmost integral sign:[2]
         &#x222B; &#x22EF;  &#x222B;   D     f (  x  1   ,  x  2   , &#x2026; ,
      x  n   )  d  x  1    &#x22EF; d  x  n     {\displaystyle \int \cdots \int
      _{\mathbf {D} }\,f(x_{1},x_{2},\ldots ,x_{n})\,dx_{1}\!\cdots dx_{n}}  [
      {\displaystyle \int \cdots \int _{\mathbf {D} }\,f(x_{1},x_{2},\ldots ,x_
      {n})\,dx_{1}\!\cdots dx_{n}}]
Since the concept of an antiderivative is only defined for functions of a
single real variable, the usual definition of the indefinite_integral does not
immediately extend to the multiple integral.
***** Mathematical definition[edit] *****
For n > 1, consider a so-called "half-open" n-dimensional hyperrectangular
domain T, defined as:
         T = [  a  1   ,  b  1   ) &#x00D7; [  a  2   ,  b  2   ) &#x00D7;
      &#x22EF; &#x00D7; [  a  n   ,  b  n   ) &#x2286;   R   n   .
      {\displaystyle T=[a_{1},b_{1})\times [a_{2},b_{2})\times \cdots \times
      [a_{n},b_{n})\subseteq \mathbf {R} ^{n}.}  [{\displaystyle T=[a_{1},b_
      {1})\times [a_{2},b_{2})\times \cdots \times [a_{n},b_{n})\subseteq
      \mathbf {R} ^{n}.}]
Partition each interval [aj, bj) into a finite family Ij of non-overlapping
subintervals ijÎ±, with each subinterval closed at the left end, and open at
the right end.
Then the finite family of subrectangles C given by
         C =  I  1   &#x00D7;  I  2   &#x00D7; &#x22EF; &#x00D7;  I  n
      {\displaystyle C=I_{1}\times I_{2}\times \cdots \times I_{n}}  [C=I_
      {1}\times I_{2}\times \cdots \times I_{n}]
is a partition of T; that is, the subrectangles Ck are non-overlapping and
their union is T.
Let f : T â R be a function defined on T. Consider a partition C of T as
defined above, such that C is a family of m subrectangles Cm and
         T =  C  1   &#x222A;  C  2   &#x222A; &#x22EF; &#x222A;  C  m
      {\displaystyle T=C_{1}\cup C_{2}\cup \cdots \cup C_{m}}  [T=C_{1}\cup C_
      {2}\cup \cdots \cup C_{m}]
We can approximate the total (n + 1)th-dimensional volume bounded below by the
n-dimensional hyperrectangle T and above by the n-dimensional graph of f with
the following Riemann_sum:
          &#x2211;  k = 1   m   f (  P  k   )  m &#x2061; (  C  k   )
      {\displaystyle \sum _{k=1}^{m}f(P_{k})\,\operatorname {m} (C_{k})}  [\sum
      _{k=1}^{m}f(P_{k})\,\operatorname {m} (C_{k})]
where Pk is a point in Ck and m(Ck) is the product of the lengths of the
intervals whose Cartesian product is Ck, also known as the measure of Ck.
The diameter of a subrectangle Ck is the largest of the lengths of the
intervals whose Cartesian_product is Ck. The diameter of a given partition of T
is defined as the largest of the diameters of the subrectangles in the
partition. Intuitively, as the diameter of the partition C is restricted
smaller and smaller, the number of subrectangles m gets larger, and the measure
m(Ck) of each subrectangle grows smaller. The function f is said to be Riemann
integrable if the limit
         S =  lim  &#x03B4; &#x2192; 0    &#x2211;  k = 1   m   f (  P  k   )
      m  (  C  k   )   {\displaystyle S=\lim _{\delta \to 0}\sum _{k=1}^{m}f(P_
      {k})\,\operatorname {m} \,(C_{k})}  [S=\lim _{\delta \to 0}\sum _{k=1}^
      {m}f(P_{k})\,\operatorname {m} \,(C_{k})]
exists, where the limit is taken over all possible partitions of T of diameter
at most Î´.[3]
If f is Riemann integrable, S is called the Riemann integral of f over T and is
denoted
         &#x222B; &#x22EF;  &#x222B;  T    f (  x  1   ,  x  2   , &#x2026; ,
      x  n   )  d  x  1    &#x22EF; d  x  n     {\displaystyle \int \cdots \int
      _{T}\,f(x_{1},x_{2},\ldots ,x_{n})\,dx_{1}\!\cdots dx_{n}}  [
      {\displaystyle \int \cdots \int _{T}\,f(x_{1},x_{2},\ldots ,x_{n})\,dx_
      {1}\!\cdots dx_{n}}]
Frequently this notation is abbreviated as
          &#x222B;  T    f (  x  )   d  n    x  .   {\displaystyle \int _{T}\!f
      (\mathbf {x} )\,d^{n}\mathbf {x} .}  [\int _{T}\!f(\mathbf {x} )\,d^
      {n}\mathbf {x} .]
where x represents the n-tuple (x1, ... xn) and dnx is the n-dimensional volume
differential.
The Riemann integral of a function defined over an arbitrary bounded n-
dimensional set can be defined by extending that function to a function defined
over a half-open rectangle whose values are zero outside the domain of the
original function. Then the integral of the original function over the original
domain is defined to be the integral of the extended function over its
rectangular domain, if it exists.
In what follows the Riemann integral in n dimensions will be called the
multiple integral.
**** Properties[edit] ****
Multiple integrals have many properties common to those of integrals of
functions of one variable (linearity, commutativity, monotonicity, and so on).
One important property of multiple integrals is that the value of an integral
is independent of the order of integrands under certain conditions. This
property is popularly known as Fubini's_theorem.[4]
**** Particular cases[edit] ****
In the case of T â R2, the integral
         l =  &#x222C;  T   f ( x , y )  d x  d y   {\displaystyle l=\iint _
      {T}f(x,y)\,dx\,dy}  [{\displaystyle l=\iint _{T}f(x,y)\,dx\,dy}]
is the double integral of f on T, and if T â R3 the integral
         l =  &#x222D;  T   f ( x , y , z )  d x  d y  d z   {\displaystyle
      l=\iiint _{T}f(x,y,z)\,dx\,dy\,dz}  [{\displaystyle l=\iiint _{T}f
      (x,y,z)\,dx\,dy\,dz}]
is the triple integral of f on T.
Notice that, by convention, the double integral has two integral signs, and the
triple integral has three; this is a notational convention which is convenient
when computing a multiple integral as an iterated integral, as shown later in
this article.
***** Methods of integration[edit] *****
The resolution of problems with multiple integrals consists, in most cases, of
finding a way to reduce the multiple integral to an iterated_integral, a series
of integrals of one variable, each being directly solvable. For continuous
functions, this is justified by Fubini's_theorem. Sometimes, it is possible to
obtain the result of the integration by direct examination without any
calculations.
The following are some simple methods of integration:[1]
**** Integrating constant functions[edit] ****
When the integrand is a constant_function c, the integral is equal to the
product of c and the measure of the domain of integration. If c = 1 and the
domain is a subregion of R2, the integral gives the area of the region, while
if the domain is a subregion of R3, the integral gives the volume of the
region.
     Example. Let f(x, y) = 2 and
              D =  {  ( x , y ) &#x2208;   R   2   &#xA0; : &#xA0; 2
           &#x2264; x &#x2264; 4 &#xA0; ; &#xA0; 3 &#x2264; y &#x2264; 6
           }    {\displaystyle D=\left\{(x,y)\in \mathbf {R} ^{2}\ :
           \ 2\leq x\leq 4\ ;\ 3\leq y\leq 6\right\}}  [{\displaystyle
           D=\left\{(x,y)\in \mathbf {R} ^{2}\ :\ 2\leq x\leq 4\ ;\ 3\leq
           y\leq 6\right\}}]
     in which case
               &#x222B;  3   6    &#x222B;  2   4   &#xA0; 2 &#xA0; d x  d
           y = 2  &#x222B;  3   6    &#x222B;  2   4   &#xA0; 1 &#xA0; d x
           d y = 2 &#x22C5; area &#x2061; ( D ) = 2 &#x22C5; ( 2 &#x22C5;
           3 ) = 12 ,   {\displaystyle \int _{3}^{6}\int _{2}^{4}\ 2\
           dx\,dy=2\int _{3}^{6}\int _{2}^{4}\ 1\ dx\,dy=2\cdot
           \operatorname {area} (D)=2\cdot (2\cdot 3)=12,}  [
           {\displaystyle \int _{3}^{6}\int _{2}^{4}\ 2\ dx\,dy=2\int _
           {3}^{6}\int _{2}^{4}\ 1\ dx\,dy=2\cdot \operatorname {area}
           (D)=2\cdot (2\cdot 3)=12,}]
     since by definition we have:
               &#x222B;  3   6    &#x222B;  2   4   &#xA0; 1 &#xA0; d x  d
           y = area &#x2061; ( D ) .   {\displaystyle \int _{3}^{6}\int _
           {2}^{4}\ 1\ dx\,dy=\operatorname {area} (D).}  [{\displaystyle
           \int _{3}^{6}\int _{2}^{4}\ 1\ dx\,dy=\operatorname {area}
           (D).}]
**** Use of symmetry[edit] ****
When the domain of integration is symmetric about the origin with respect to at
least one of the variables of integration and the integrand is odd with respect
to this variable, the integral is equal to zero, as the integrals over the two
halves of the domain have the same absolute value but opposite signs. When the
integrand is even with respect to this variable, the integral is equal to twice
the integral over one half of the domain, as the integrals over the two halves
of the domain are equal.
     Example 1. Consider the function f(x,y) = 2 sin(x) â 3y3 + 5
     integrated over the domain
              T =  {  ( x , y ) &#x2208;   R   2   &#xA0; : &#xA0;  x  2
           +  y  2   &#x2264; 1  }  ,   {\displaystyle T=\left\{(x,y)\in
           \mathbf {R} ^{2}\ :\ x^{2}+y^{2}\leq 1\right\},}  [T=\left\{
           (x,y)\in \mathbf {R} ^{2}\ :\ x^{2}+y^{2}\leq 1\right\},]
     a disc with radius 1 centered at the origin with the boundary
     included.
     Using the linearity property, the integral can be decomposed into
     three pieces:
               &#x222C;  T    (  2 sin &#x2061; x &#x2212; 3  y  3   + 5
           )   d x  d y =  &#x222C;  T   2 sin &#x2061; x  d x  d y
           &#x2212;  &#x222C;  T   3  y  3    d x  d y +  &#x222C;  T   5
           d x  d y   {\displaystyle \iint _{T}\left(2\sin x-3y^
           {3}+5\right)\,dx\,dy=\iint _{T}2\sin x\,dx\,dy-\iint _{T}3y^
           {3}\,dx\,dy+\iint _{T}5\,dx\,dy}  [{\displaystyle \iint _
           {T}\left(2\sin x-3y^{3}+5\right)\,dx\,dy=\iint _{T}2\sin
           x\,dx\,dy-\iint _{T}3y^{3}\,dx\,dy+\iint _{T}5\,dx\,dy}]
     The function 2 sin(x) is an odd function in the variable x and the
     disc T is symmetric with respect to the y-axis, so the value of the
     first integral is 0. Similarly, the function 3y3 is an odd function
     of y, and T is symmetric with respect to the x-axis, and so the only
     contribution to the final result is that of the third integral.
     Therefore the original integral is equal to the area of the disk
     times 5, or 5Ï.
     Example 2. Consider the function f(x, y, z) = x exp(y2 + z2) and as
     integration region the sphere with radius 2 centered at the origin,
              T =  {  ( x , y , z ) &#x2208;   R   3   &#xA0; : &#xA0;  x
           2   +  y  2   +  z  2   &#x2264; 4  }  .   {\displaystyle
           T=\left\{(x,y,z)\in \mathbf {R} ^{3}\ :\ x^{2}+y^{2}+z^{2}\leq
           4\right\}.}  [T=\left\{(x,y,z)\in \mathbf {R} ^{3}\ :\ x^{2}+y^
           {2}+z^{2}\leq 4\right\}.]
     The "ball" is symmetric about all three axes, but it is sufficient to
     integrate with respect to x-axis to show that the integral is 0,
     because the function is an odd function of that variable.
**** Normal domains on R2[edit] ****
See also: Order_of_integration_(calculus)
This method is applicable to any domain D for which:
    * the projection of D onto either the x-axis or the y-axis is bounded by
      the two values, a and b
    * any line perpendicular to this axis that passes between these two values
      intersects the domain in an interval whose endpoints are given by the
      graphs of two functions, Î± and Î².
Such a domain will be here called a normal domain. Elsewhere in the literature,
normal domains are sometimes called type I or type II domains, depending on
which axis the domain is fibred over. In all cases, the function to be
integrated must be Riemann integrable on the domain, which is true (for
instance) if the function is continuous.
*** x-axis[edit] ***
If the domain D is normal with respect to the x-axis, and f : D â R is a
continuous_function; then Î±(x) and Î²(x) (both of which are defined on the
interval [a, b]) are the two functions that determine D. Then, by Fubini's
theorem:[5]
          &#x222C;  D   f ( x , y )  d x  d y =  &#x222B;  a   b   d x
      &#x222B;  &#x03B1; ( x )   &#x03B2; ( x )   f ( x , y )  d y .
      {\displaystyle \iint _{D}f(x,y)\,dx\,dy=\int _{a}^{b}dx\int _{\alpha
      (x)}^{\beta (x)}f(x,y)\,dy.}  [{\displaystyle \iint _{D}f
      (x,y)\,dx\,dy=\int _{a}^{b}dx\int _{\alpha (x)}^{\beta (x)}f(x,y)\,dy.}]
*** y-axis[edit] ***
If D is normal with respect to the y-axis and f : D â R is a continuous
function; then Î±(y) and Î²(y) (both of which are defined on the interval [a,
b]) are the two functions that determine D. Again, by Fubini's theorem:
          &#x222C;  D   f ( x , y )  d x  d y =  &#x222B;  a   b   d y
      &#x222B;  &#x03B1; ( y )   &#x03B2; ( y )   f ( x , y )  d x .
      {\displaystyle \iint _{D}f(x,y)\,dx\,dy=\int _{a}^{b}dy\int _{\alpha
      (y)}^{\beta (y)}f(x,y)\,dx.}  [{\displaystyle \iint _{D}f
      (x,y)\,dx\,dy=\int _{a}^{b}dy\int _{\alpha (y)}^{\beta (y)}f(x,y)\,dx.}]
*** Normal domains on R3[edit] ***
If T is a domain that is normal with respect to the xy-plane and determined by
the functions Î±(x, y) and Î²(x, y), then
          &#x222D;  T   f ( x , y , z )  d x  d y  d z =  &#x222C;  D
      &#x222B;  &#x03B1; ( x , y )   &#x03B2; ( x , y )   f ( x , y , z )  d z
      d x  d y   {\displaystyle \iiint _{T}f(x,y,z)\,dx\,dy\,dz=\iint _{D}\int
      _{\alpha (x,y)}^{\beta (x,y)}f(x,y,z)\,dz\,dx\,dy}  [{\displaystyle
      \iiint _{T}f(x,y,z)\,dx\,dy\,dz=\iint _{D}\int _{\alpha (x,y)}^{\beta
      (x,y)}f(x,y,z)\,dz\,dx\,dy}]
This definition is the same for the other five normality cases on R3. It can be
generalized in a straightforward way to domains in Rn.
**** Change of variables[edit] ****
See also: Integration_by_substitution_Â§ Substitution_for_multiple_variables
The limits of integration are often not easily interchangeable (without
normality or with complex formulae to integrate). One makes a change_of
variables to rewrite the integral in a more "comfortable" region, which can be
described in simpler formulae. To do so, the function must be adapted to the
new coordinates.
     Example 1a. The function is f(x, y) = (x â 1)2 + √y; if one adopts
     the substitution xâ² = x â 1, yâ² = y therefore x = xâ² + 1, y =
     yâ² one obtains the new function f2(x, y) = (xâ²)2 + √y.
    * Similarly for the domain because it is delimited by the original
      variables that were transformed before (x and y in example).
    * the differentials dx and dy transform via the absolute value of the
      determinant_of_the_Jacobian_matrix containing the partial derivatives of
      the transformations regarding the new variable (consider, as an example,
      the differential transformation in polar coordinates).
There exist three main "kinds" of changes of variable (one in R2, two in R3);
however, more general substitutions can be made using the same principle.
*** Polar coordinates[edit] ***
See also: Polar_coordinate_system
Transformation from cartesian to polar coordinates.
In R2 if the domain has a circular symmetry and the function has some
particular characteristics one can apply the transformation to polar
coordinates (see the example in the picture) which means that the generic
points P(x, y) in Cartesian coordinates switch to their respective points in
polar coordinates. That allows one to change the shape of the domain and
simplify the operations.
The fundamental relation to make the transformation is the following:
         f ( x , y ) &#x2192; f ( &#x03C1; cos &#x2061; &#x03C6; , &#x03C1; sin
      &#x2061; &#x03C6; ) .   {\displaystyle f(x,y)\rightarrow f(\rho \cos
      \varphi ,\rho \sin \varphi ).}  [{\displaystyle f(x,y)\rightarrow f(\rho
      \cos \varphi ,\rho \sin \varphi ).}]
     Example 2a. The function is f(x, y) = x + y and applying the
     transformation one obtains
              f ( &#x03C1; , &#x03C6; ) = &#x03C1; cos &#x2061; &#x03C6; +
           &#x03C1; sin &#x2061; &#x03C6; = &#x03C1; ( cos &#x2061;
           &#x03C6; + sin &#x2061; &#x03C6; ) .   {\displaystyle f(\rho
           ,\varphi )=\rho \cos \varphi +\rho \sin \varphi =\rho (\cos
           \varphi +\sin \varphi ).}  [{\displaystyle f(\rho ,\varphi
           )=\rho \cos \varphi +\rho \sin \varphi =\rho (\cos \varphi
           +\sin \varphi ).}]
     Example 2b. The function is f(x, y) = x2 + y2, in this case one has:
              f ( &#x03C1; , &#x03C6; ) =  &#x03C1;  2    (   cos  2
           &#x2061; &#x03C6; +  sin  2   &#x2061; &#x03C6;  )  =  &#x03C1;
           2     {\displaystyle f(\rho ,\varphi )=\rho ^{2}\left(\cos ^
           {2}\varphi +\sin ^{2}\varphi \right)=\rho ^{2}}  [
           {\displaystyle f(\rho ,\varphi )=\rho ^{2}\left(\cos ^
           {2}\varphi +\sin ^{2}\varphi \right)=\rho ^{2}}]
     using the Pythagorean_trigonometric_identity (very useful to simplify
     this operation).
The transformation of the domain is made by defining the radius' crown length
and the amplitude of the described angle to define the Ï, Ï intervals
starting from x, y.
Example of a domain transformation from cartesian to polar.
     Example 2c. The domain is D = {x2 + y2 â¤ 4}, that is a
     circumference of radius 2; it's evident that the covered angle is the
     circle angle, so Ï varies from 0 to 2Ï, while the crown radius
     varies from 0 to 2 (the crown with the inside radius null is just a
     circle).
     Example 2d. The domain is D = {x2 + y2 â¤ 9, x2 + y2 â¥ 4, y â¥
     0}, that is the circular crown in the positive y half-plane (please
     see the picture in the example); Ï describes a plane angle while Ï
     varies from 2 to 3. Therefore the transformed domain will be the
     following rectangle:
              T = { 2 &#x2264; &#x03C1; &#x2264; 3 , &#xA0; 0 &#x2264;
           &#x03C6; &#x2264; &#x03C0; } .   {\displaystyle T=\{2\leq \rho
           \leq 3,\ 0\leq \varphi \leq \pi \}.}  [{\displaystyle T=\{2\leq
           \rho \leq 3,\ 0\leq \varphi \leq \pi \}.}]
     The Jacobian_determinant of that transformation is the following:
                 &#x2202; ( x , y )   &#x2202; ( &#x03C1; , &#x03C6; )
           =   |    cos &#x2061; &#x03C6;   &#x2212; &#x03C1; sin &#x2061;
           &#x03C6;     sin &#x2061; &#x03C6;   &#x03C1; cos &#x2061;
           &#x03C6;    |   = &#x03C1;   {\displaystyle {\frac {\partial
           (x,y)}{\partial (\rho ,\varphi )}}={\begin{vmatrix}\cos \varphi
           &-\rho \sin \varphi \\\sin \varphi &\rho \cos \varphi \end
           {vmatrix}}=\rho }  [{\displaystyle {\frac {\partial (x,y)}
           {\partial (\rho ,\varphi )}}={\begin{vmatrix}\cos \varphi &-
           \rho \sin \varphi \\\sin \varphi &\rho \cos \varphi \end
           {vmatrix}}=\rho }]
     which has been obtained by inserting the partial derivatives of x =
     Ï cos(Ï), y = Ï sin(Ï) in the first column respect to Ï and in
     the second respect to Ï, so the dx dy differentials in this
     transformation become Ï dÏ dÏ.
     Once the function is transformed and the domain evaluated, it is
     possible to define the formula for the change of variables in polar
     coordinates:
               &#x222C;  D   f ( x , y )  d x  d y =  &#x222C;  T   f
           ( &#x03C1; cos &#x2061; &#x03C6; , &#x03C1; sin &#x2061;
           &#x03C6; ) &#x03C1;  d &#x03C1;  d &#x03C6; .   {\displaystyle
           \iint _{D}f(x,y)\,dx\,dy=\iint _{T}f(\rho \cos \varphi ,\rho
           \sin \varphi )\rho \,d\rho \,d\varphi .}  [{\displaystyle \iint
           _{D}f(x,y)\,dx\,dy=\iint _{T}f(\rho \cos \varphi ,\rho \sin
           \varphi )\rho \,d\rho \,d\varphi .}]
     Ï is valid in the [0, 2Ï] interval while Ï, which is a measure of
     a length, can only have positive values.
     Example 2e. The function is f(x, y) = x and the domain is the same as
     in Example 2d. From the previous analysis of D we know the intervals
     of Ï (from 2 to 3) and of Ï (from 0 to Ï). Now we change the
     function:
              f ( x , y ) = x &#x27F6; f ( &#x03C1; , &#x03C6; ) =
           &#x03C1; cos &#x2061; &#x03C6; .   {\displaystyle f
           (x,y)=x\longrightarrow f(\rho ,\varphi )=\rho \cos \varphi .}
           [{\displaystyle f(x,y)=x\longrightarrow f(\rho ,\varphi )=\rho
           \cos \varphi .}]
     finally let's apply the integration formula:
               &#x222C;  D   x  d x  d y =  &#x222C;  T   &#x03C1; cos
           &#x2061; &#x03C6; &#x03C1;  d &#x03C1;  d &#x03C6; .
           {\displaystyle \iint _{D}x\,dx\,dy=\iint _{T}\rho \cos \varphi
           \rho \,d\rho \,d\varphi .}  [{\displaystyle \iint _
           {D}x\,dx\,dy=\iint _{T}\rho \cos \varphi \rho \,d\rho
           \,d\varphi .}]
     Once the intervals are known, you have
               &#x222B;  0   &#x03C0;    &#x222B;  2   3    &#x03C1;  2
           cos &#x2061; &#x03C6;  d &#x03C1;  d &#x03C6; =  &#x222B;  0
           &#x03C0;   cos &#x2061; &#x03C6; &#xA0; d &#x03C6;
           [    &#x03C1;  3   3   ]   2   3   =   [   sin &#x2061;
           &#x03C6;    ]    0   &#x03C0;   &#xA0;  (  9 &#x2212;   8 3
           )  = 0.   {\displaystyle \int _{0}^{\pi }\int _{2}^{3}\rho ^
           {2}\cos \varphi \,d\rho \,d\varphi =\int _{0}^{\pi }\cos
           \varphi \ d\varphi \left[{\frac {\rho ^{3}}{3}}\right]_{2}^{3}=
           {\Big [}\sin \varphi {\Big ]}_{0}^{\pi }\ \left(9-{\frac {8}
           {3}}\right)=0.}  [{\displaystyle \int _{0}^{\pi }\int _{2}^
           {3}\rho ^{2}\cos \varphi \,d\rho \,d\varphi =\int _{0}^{\pi
           }\cos \varphi \ d\varphi \left[{\frac {\rho ^{3}}{3}}\right]_
           {2}^{3}={\Big [}\sin \varphi {\Big ]}_{0}^{\pi }\ \left(9-
           {\frac {8}{3}}\right)=0.}]
*** Cylindrical coordinates[edit] ***
Cylindrical coordinates.
In R3 the integration on domains with a circular base can be made by the
passage to cylindrical_coordinates; the transformation of the function is made
by the following relation:
         f ( x , y , z ) &#x2192; f ( &#x03C1; cos &#x2061; &#x03C6; , &#x03C1;
      sin &#x2061; &#x03C6; , z )   {\displaystyle f(x,y,z)\rightarrow f(\rho
      \cos \varphi ,\rho \sin \varphi ,z)}  [{\displaystyle f(x,y,z)\rightarrow
      f(\rho \cos \varphi ,\rho \sin \varphi ,z)}]
The domain transformation can be graphically attained, because only the shape
of the base varies, while the height follows the shape of the starting region.
     Example 3a. The region is D = {x2 + y2 â¤ 9, x2 + y2 â¥ 4, 0 â¤ z
     â¤ 5} (that is the "tube" whose base is the circular crown of
     Example 2d and whose height is 5); if the transformation is applied,
     this region is obtained:
              T = { 2 &#x2264; &#x03C1; &#x2264; 3 , &#xA0; 0 &#x2264;
           &#x03C6; &#x2264; 2 &#x03C0; , &#xA0; 0 &#x2264; z &#x2264; 5 }
           {\displaystyle T=\{2\leq \rho \leq 3,\ 0\leq \varphi \leq 2\pi
           ,\ 0\leq z\leq 5\}}  [{\displaystyle T=\{2\leq \rho \leq 3,\
           0\leq \varphi \leq 2\pi ,\ 0\leq z\leq 5\}}]
     (that is, the parallelepiped whose base is similar to the rectangle
     in Example 2d and whose height is 5).
     Because the z component is unvaried during the transformation, the dx
     dy dz differentials vary as in the passage to polar coordinates:
     therefore, they become Ï dÏ dÏ dz.
     Finally, it is possible to apply the final formula to cylindrical
     coordinates:
               &#x222D;  D   f ( x , y , z )  d x  d y  d z =  &#x222D;  T
           f ( &#x03C1; cos &#x2061; &#x03C6; , &#x03C1; sin &#x2061;
           &#x03C6; , z ) &#x03C1;  d &#x03C1;  d &#x03C6;  d z .
           {\displaystyle \iiint _{D}f(x,y,z)\,dx\,dy\,dz=\iiint _{T}f
           (\rho \cos \varphi ,\rho \sin \varphi ,z)\rho \,d\rho
           \,d\varphi \,dz.}  [{\displaystyle \iiint _{D}f
           (x,y,z)\,dx\,dy\,dz=\iiint _{T}f(\rho \cos \varphi ,\rho \sin
           \varphi ,z)\rho \,d\rho \,d\varphi \,dz.}]
     This method is convenient in case of cylindrical or conical domains
     or in regions where it is easy to individuate the z interval and even
     transform the circular base and the function.
     Example 3b. The function is f(x, y, z) = x2 + y2 + z and as
     integration domain this cylinder: D = {x2 + y2 â¤ 9, â5 â¤ z â¤
     5 }. The transformation of D in cylindrical coordinates is the
     following:
              T = { 0 &#x2264; &#x03C1; &#x2264; 3 , &#xA0; 0 &#x2264;
           &#x03C6; &#x2264; 2 &#x03C0; , &#xA0; &#x2212; 5 &#x2264; z
           &#x2264; 5 } .   {\displaystyle T=\{0\leq \rho \leq 3,\ 0\leq
           \varphi \leq 2\pi ,\ -5\leq z\leq 5\}.}  [{\displaystyle T=\
           {0\leq \rho \leq 3,\ 0\leq \varphi \leq 2\pi ,\ -5\leq z\leq
           5\}.}]
     while the function becomes
              f ( &#x03C1; cos &#x2061; &#x03C6; , &#x03C1; sin &#x2061;
           &#x03C6; , z ) =  &#x03C1;  2   + z   {\displaystyle f(\rho
           \cos \varphi ,\rho \sin \varphi ,z)=\rho ^{2}+z}  [
           {\displaystyle f(\rho \cos \varphi ,\rho \sin \varphi ,z)=\rho
           ^{2}+z}]
     Finally one can apply the integration formula:
               &#x222D;  D    (   x  2   +  y  2   + z  )   d x  d y  d z
           =  &#x222D;  T    (   &#x03C1;  2   + z  )  &#x03C1;  d
           &#x03C1;  d &#x03C6;  d z ;   {\displaystyle \iiint _{D}\left
           (x^{2}+y^{2}+z\right)\,dx\,dy\,dz=\iiint _{T}\left(\rho ^
           {2}+z\right)\rho \,d\rho \,d\varphi \,dz;}  [{\displaystyle
           \iiint _{D}\left(x^{2}+y^{2}+z\right)\,dx\,dy\,dz=\iiint _
           {T}\left(\rho ^{2}+z\right)\rho \,d\rho \,d\varphi \,dz;}]
     developing the formula you have
               &#x222B;  &#x2212; 5   5   d z  &#x222B;  0   2 &#x03C0;
           d &#x03C6;  &#x222B;  0   3    (   &#x03C1;  3   + &#x03C1; z
           )   d &#x03C1; = 2 &#x03C0;  &#x222B;  &#x2212; 5   5
           [     &#x03C1;  4   4   +     &#x03C1;  2   z  2    ]   0   3
           d z = 2 &#x03C0;  &#x222B;  &#x2212; 5   5    (    81 4   +   9
           2   z  )   d z = &#x22EF; = 405 &#x03C0; .   {\displaystyle
           \int _{-5}^{5}dz\int _{0}^{2\pi }d\varphi \int _{0}^{3}\left
           (\rho ^{3}+\rho z\right)\,d\rho =2\pi \int _{-5}^{5}\left[
           {\frac {\rho ^{4}}{4}}+{\frac {\rho ^{2}z}{2}}\right]_{0}^
           {3}\,dz=2\pi \int _{-5}^{5}\left({\frac {81}{4}}+{\frac {9}
           {2}}z\right)\,dz=\cdots =405\pi .}  [{\displaystyle \int _{-5}^
           {5}dz\int _{0}^{2\pi }d\varphi \int _{0}^{3}\left(\rho ^
           {3}+\rho z\right)\,d\rho =2\pi \int _{-5}^{5}\left[{\frac {\rho
           ^{4}}{4}}+{\frac {\rho ^{2}z}{2}}\right]_{0}^{3}\,dz=2\pi \int
           _{-5}^{5}\left({\frac {81}{4}}+{\frac {9}
           {2}}z\right)\,dz=\cdots =405\pi .}]
*** Spherical coordinates[edit] ***
Spherical coordinates.
In R3 some domains have a spherical symmetry, so it's possible to specify the
coordinates of every point of the integration region by two angles and one
distance. It's possible to use therefore the passage to spherical_coordinates;
the function is transformed by this relation:
         f ( x , y , z ) &#x27F6; f ( &#x03C1; cos &#x2061; &#x03B8; sin
      &#x2061; &#x03C6; , &#x03C1; sin &#x2061; &#x03B8; sin &#x2061; &#x03C6;
      , &#x03C1; cos &#x2061; &#x03C6; )   {\displaystyle f
      (x,y,z)\longrightarrow f(\rho \cos \theta \sin \varphi ,\rho \sin \theta
      \sin \varphi ,\rho \cos \varphi )}  [{\displaystyle f
      (x,y,z)\longrightarrow f(\rho \cos \theta \sin \varphi ,\rho \sin \theta
      \sin \varphi ,\rho \cos \varphi )}]
Points on the z-axis do not have a precise characterization in spherical
coordinates, so Î¸ can vary between 0 and 2Ï.
The better integration domain for this passage is the sphere.
     Example 4a. The domain is D = x2 + y2 + z2 â¤ 16 (sphere with radius
     4 and center at the origin); applying the transformation you get the
     region
              T = { 0 &#x2264; &#x03C1; &#x2264; 4 , &#xA0; 0 &#x2264;
           &#x03C6; &#x2264; &#x03C0; , &#xA0; 0 &#x2264; &#x03B8;
           &#x2264; 2 &#x03C0; } .   {\displaystyle T=\{0\leq \rho \leq
           4,\ 0\leq \varphi \leq \pi ,\ 0\leq \theta \leq 2\pi \}.}  [
           {\displaystyle T=\{0\leq \rho \leq 4,\ 0\leq \varphi \leq \pi
           ,\ 0\leq \theta \leq 2\pi \}.}]
     The Jacobian determinant of this transformation is the following:
                 &#x2202; ( x , y , z )   &#x2202; ( &#x03C1; , &#x03B8; ,
           &#x03C6; )    =   |    cos &#x2061; &#x03B8; sin &#x2061;
           &#x03C6;   &#x2212; &#x03C1; sin &#x2061; &#x03B8; sin &#x2061;
           &#x03C6;   &#x03C1; cos &#x2061; &#x03B8; cos &#x2061; &#x03C6;
           sin &#x2061; &#x03B8; sin &#x2061; &#x03C6;   &#x03C1; cos
           &#x2061; &#x03B8; sin &#x2061; &#x03C6;   &#x03C1; sin &#x2061;
           &#x03B8; cos &#x2061; &#x03C6;     cos &#x2061; &#x03C6;   0
           &#x2212; &#x03C1; sin &#x2061; &#x03C6;    |   =  &#x03C1;  2
           sin &#x2061; &#x03C6;   {\displaystyle {\frac {\partial
           (x,y,z)}{\partial (\rho ,\theta ,\varphi )}}={\begin
           {vmatrix}\cos \theta \sin \varphi &-\rho \sin \theta \sin
           \varphi &\rho \cos \theta \cos \varphi \\\sin \theta \sin
           \varphi &\rho \cos \theta \sin \varphi &\rho \sin \theta \cos
           \varphi \\\cos \varphi &0&-\rho \sin \varphi \end
           {vmatrix}}=\rho ^{2}\sin \varphi }  [{\displaystyle {\frac
           {\partial (x,y,z)}{\partial (\rho ,\theta ,\varphi )}}={\begin
           {vmatrix}\cos \theta \sin \varphi &-\rho \sin \theta \sin
           \varphi &\rho \cos \theta \cos \varphi \\\sin \theta \sin
           \varphi &\rho \cos \theta \sin \varphi &\rho \sin \theta \cos
           \varphi \\\cos \varphi &0&-\rho \sin \varphi \end
           {vmatrix}}=\rho ^{2}\sin \varphi }]
     The dx dy dz differentials therefore are transformed to Ï2 sin(Ï)
     dÏ dÎ¸ dÏ.
     This yields the final integration formula:
               &#x222D;  D   f ( x , y , z )  d x  d y  d z =  &#x222D;  T
           f ( &#x03C1; sin &#x2061; &#x03C6; cos &#x2061; &#x03B8; ,
           &#x03C1; sin &#x2061; &#x03C6; sin &#x2061; &#x03B8; , &#x03C1;
           cos &#x2061; &#x03C6; )  &#x03C1;  2   sin &#x2061; &#x03C6;  d
           &#x03C1;  d &#x03B8;  d &#x03C6; .   {\displaystyle \iiint _
           {D}f(x,y,z)\,dx\,dy\,dz=\iiint _{T}f(\rho \sin \varphi \cos
           \theta ,\rho \sin \varphi \sin \theta ,\rho \cos \varphi )\rho
           ^{2}\sin \varphi \,d\rho \,d\theta \,d\varphi .}  [
           {\displaystyle \iiint _{D}f(x,y,z)\,dx\,dy\,dz=\iiint _{T}f
           (\rho \sin \varphi \cos \theta ,\rho \sin \varphi \sin \theta
           ,\rho \cos \varphi )\rho ^{2}\sin \varphi \,d\rho \,d\theta
           \,d\varphi .}]
It is better to use this method in case of spherical domains and in case of
functions that can be easily simplified by the first fundamental relation of
trigonometry extended to R3 (see Example 4b); in other cases it can be better
to use cylindrical coordinates (see Example 4c).
          &#x222D;  T   f ( a , b , c )  &#x03C1;  2   sin &#x2061; &#x03C6;  d
      &#x03C1;  d &#x03B8;  d &#x03C6; .   {\displaystyle \iiint _{T}f
      (a,b,c)\rho ^{2}\sin \varphi \,d\rho \,d\theta \,d\varphi .}  [
      {\displaystyle \iiint _{T}f(a,b,c)\rho ^{2}\sin \varphi \,d\rho \,d\theta
      \,d\varphi .}]
The extra Ï2 and sin Ï come from the Jacobian.
In the following examples the roles of Ï and Î¸ have been reversed.
     Example 4b. D is the same region as in Example 4a and f(x, y, z) = x2
     + y2 + z2 is the function to integrate. Its transformation is very
     easy:
              f ( &#x03C1; sin &#x2061; &#x03C6; cos &#x2061; &#x03B8; ,
           &#x03C1; sin &#x2061; &#x03C6; sin &#x2061; &#x03B8; , &#x03C1;
           cos &#x2061; &#x03C6; ) =  &#x03C1;  2   ,   {\displaystyle f
           (\rho \sin \varphi \cos \theta ,\rho \sin \varphi \sin \theta
           ,\rho \cos \varphi )=\rho ^{2},}  [{\displaystyle f(\rho \sin
           \varphi \cos \theta ,\rho \sin \varphi \sin \theta ,\rho \cos
           \varphi )=\rho ^{2},}]
     while we know the intervals of the transformed region T from D:
              T = { 0 &#x2264; &#x03C1; &#x2264; 4 , &#xA0; 0 &#x2264;
           &#x03C6; &#x2264; &#x03C0; , &#xA0; 0 &#x2264; &#x03B8;
           &#x2264; 2 &#x03C0; } .   {\displaystyle T=\{0\leq \rho \leq
           4,\ 0\leq \varphi \leq \pi ,\ 0\leq \theta \leq 2\pi \}.}  [
           {\displaystyle T=\{0\leq \rho \leq 4,\ 0\leq \varphi \leq \pi
           ,\ 0\leq \theta \leq 2\pi \}.}]
     We therefore apply the integration formula:
               &#x222D;  D    (   x  2   +  y  2   +  z  2    )   d x  d y
           d z =  &#x222D;  T    &#x03C1;  2     &#x03C1;  2   sin
           &#x2061; &#x03B8;  d &#x03C1;  d &#x03B8;  d &#x03C6; ,
           {\displaystyle \iiint _{D}\left(x^{2}+y^{2}+z^
           {2}\right)\,dx\,dy\,dz=\iiint _{T}\rho ^{2}\,\rho ^{2}\sin
           \theta \,d\rho \,d\theta \,d\varphi ,}  [{\displaystyle \iiint
           _{D}\left(x^{2}+y^{2}+z^{2}\right)\,dx\,dy\,dz=\iiint _{T}\rho
           ^{2}\,\rho ^{2}\sin \theta \,d\rho \,d\theta \,d\varphi ,}]
     and, developing, we get
               &#x222D;  T    &#x03C1;  4   sin &#x2061; &#x03B8;  d
           &#x03C1;  d &#x03B8;  d &#x03C6; =  &#x222B;  0   &#x03C0;
           sin &#x2061; &#x03C6;  d &#x03C6;  &#x222B;  0   4    &#x03C1;
           4   d &#x03C1;  &#x222B;  0   2 &#x03C0;   d &#x03B8; = 2
           &#x03C0;  &#x222B;  0   &#x03C0;   sin &#x2061; &#x03C6;
           [    &#x03C1;  5   5   ]   0   4    d &#x03C6; = 2 &#x03C0;
           [    &#x03C1;  5   5   ]   0   4     [   &#x2212; cos &#x2061;
           &#x03C6;    ]    0   &#x03C0;   =    4096 &#x03C0;  5   .
           {\displaystyle \iiint _{T}\rho ^{4}\sin \theta \,d\rho
           \,d\theta \,d\varphi =\int _{0}^{\pi }\sin \varphi \,d\varphi
           \int _{0}^{4}\rho ^{4}d\rho \int _{0}^{2\pi }d\theta =2\pi \int
           _{0}^{\pi }\sin \varphi \left[{\frac {\rho ^{5}}{5}}\right]_
           {0}^{4}\,d\varphi =2\pi \left[{\frac {\rho ^{5}}{5}}\right]_
           {0}^{4}{\Big [}-\cos \varphi {\Big ]}_{0}^{\pi }={\frac
           {4096\pi }{5}}.}  [{\displaystyle \iiint _{T}\rho ^{4}\sin
           \theta \,d\rho \,d\theta \,d\varphi =\int _{0}^{\pi }\sin
           \varphi \,d\varphi \int _{0}^{4}\rho ^{4}d\rho \int _{0}^{2\pi
           }d\theta =2\pi \int _{0}^{\pi }\sin \varphi \left[{\frac {\rho
           ^{5}}{5}}\right]_{0}^{4}\,d\varphi =2\pi \left[{\frac {\rho ^
           {5}}{5}}\right]_{0}^{4}{\Big [}-\cos \varphi {\Big ]}_{0}^{\pi
           }={\frac {4096\pi }{5}}.}]
     Example 4c. The domain D is the ball with center at the origin and
     radius 3a,
              D =  {   x  2   +  y  2   +  z  2   &#x2264; 9  a  2    }
           {\displaystyle D=\left\{x^{2}+y^{2}+z^{2}\leq 9a^{2}\right\}}
           [D=\left\{x^{2}+y^{2}+z^{2}\leq 9a^{2}\right\}]
     and f(x, y, z) = x2 + y2 is the function to integrate.
     Looking at the domain, it seems convenient to adopt the passage to
     spherical coordinates, in fact, the intervals of the variables that
     delimit the new T region are obviously:
              T = { 0 &#x2264; &#x03C1; &#x2264; 3 a , &#xA0; 0 &#x2264;
           &#x03C6; &#x2264; 2 &#x03C0; , &#xA0; 0 &#x2264; &#x03B8;
           &#x2264; &#x03C0; } .   {\displaystyle T=\{0\leq \rho \leq 3a,\
           0\leq \varphi \leq 2\pi ,\ 0\leq \theta \leq \pi \}.}  [
           {\displaystyle T=\{0\leq \rho \leq 3a,\ 0\leq \varphi \leq 2\pi
           ,\ 0\leq \theta \leq \pi \}.}]
     However, applying the transformation, we get
              f ( x , y , z ) =  x  2   +  y  2   &#x27F6;  &#x03C1;  2
           sin  2   &#x2061; &#x03B8;  cos  2   &#x2061; &#x03C6; +
           &#x03C1;  2    sin  2   &#x2061; &#x03B8;  sin  2   &#x2061;
           &#x03C6; =  &#x03C1;  2    sin  2   &#x2061; &#x03B8;
           {\displaystyle f(x,y,z)=x^{2}+y^{2}\longrightarrow \rho ^
           {2}\sin ^{2}\theta \cos ^{2}\varphi +\rho ^{2}\sin ^{2}\theta
           \sin ^{2}\varphi =\rho ^{2}\sin ^{2}\theta }  [{\displaystyle f
           (x,y,z)=x^{2}+y^{2}\longrightarrow \rho ^{2}\sin ^{2}\theta
           \cos ^{2}\varphi +\rho ^{2}\sin ^{2}\theta \sin ^{2}\varphi
           =\rho ^{2}\sin ^{2}\theta }].
     Applying the formula for integration we obtain:
               &#x222D;  T    &#x03C1;  2    sin  2   &#x2061; &#x03B8;
           &#x03C1;  2   sin &#x2061; &#x03B8;  d &#x03C1;  d &#x03B8;  d
           &#x03C6; =  &#x222D;  T    &#x03C1;  4    sin  3   &#x2061;
           &#x03B8;  d &#x03C1;  d &#x03B8;  d &#x03C6;   {\displaystyle
           \iiint _{T}\rho ^{2}\sin ^{2}\theta \rho ^{2}\sin \theta
           \,d\rho \,d\theta \,d\varphi =\iiint _{T}\rho ^{4}\sin ^
           {3}\theta \,d\rho \,d\theta \,d\varphi }  [{\displaystyle
           \iiint _{T}\rho ^{2}\sin ^{2}\theta \rho ^{2}\sin \theta
           \,d\rho \,d\theta \,d\varphi =\iiint _{T}\rho ^{4}\sin ^
           {3}\theta \,d\rho \,d\theta \,d\varphi }]
     which is very hard to solve. This problem will be solved by using the
     passage to cylindrical coordinates. The new T intervals are
              T =  {  0 &#x2264; &#x03C1; &#x2264; 3 a , &#xA0; 0 &#x2264;
           &#x03C6; &#x2264; 2 &#x03C0; , &#xA0; &#x2212;   9  a  2
           &#x2212;  &#x03C1;  2     &#x2264; z &#x2264;   9  a  2
           &#x2212;  &#x03C1;  2      }  ;   {\displaystyle T=\left\{0\leq
           \rho \leq 3a,\ 0\leq \varphi \leq 2\pi ,\ -{\sqrt {9a^{2}-\rho
           ^{2}}}\leq z\leq {\sqrt {9a^{2}-\rho ^{2}}}\right\};}  [
           {\displaystyle T=\left\{0\leq \rho \leq 3a,\ 0\leq \varphi \leq
           2\pi ,\ -{\sqrt {9a^{2}-\rho ^{2}}}\leq z\leq {\sqrt {9a^{2}-
           \rho ^{2}}}\right\};}]
     the z interval has been obtained by dividing the ball into two
     hemispheres simply by solving the inequality from the formula of D
     (and then directly transforming x2 + y2 into Ï2). The new function
     is simply Ï2. Applying the integration formula
               &#x222D;  T    &#x03C1;  2   &#x03C1;  d &#x03C1;  d
           &#x03C6;  d z .   {\displaystyle \iiint _{T}\rho ^{2}\rho
           \,d\rho \,d\varphi \,dz.}  [{\displaystyle \iiint _{T}\rho ^
           {2}\rho \,d\rho \,d\varphi \,dz.}]
     Then we get
                   &#x222B;  0   2 &#x03C0;   d &#x03C6;  &#x222B;  0   3
           a    &#x03C1;  3   d &#x03C1;  &#x222B;  &#x2212;   9  a  2
           &#x2212;  &#x03C1;  2        9  a  2   &#x2212;  &#x03C1;  2
           d z    = 2 &#x03C0;  &#x222B;  0   3 a   2  &#x03C1;  3     9
           a  2   &#x2212;  &#x03C1;  2      d &#x03C1;       = &#x2212; 2
           &#x03C0;  &#x222B;  9  a  2     0   ( 9  a  2   &#x2212; t )
           t    d t    t = 9  a  2   &#x2212;  &#x03C1;  2         = 2
           &#x03C0;  &#x222B;  0   9  a  2      (  9  a  2     t
           &#x2212; t   t    )   d t       = 2 &#x03C0;  (   &#x222B;  0
           9  a  2     9  a  2     t    d t &#x2212;  &#x222B;  0   9  a
           2     t   t    d t  )        = 2 &#x03C0;   [  9  a  2     2 3
           t   3 2    &#x2212;   2 5    t   5 2     ]   0   9  a  2
           = 2 &#x22C5; 27 &#x03C0;  a  5    (  6 &#x2212;   18 5    )
           =    648 &#x03C0;  5    a  5   .       {\displaystyle {\begin
           {aligned}\int _{0}^{2\pi }d\varphi \int _{0}^{3a}\rho ^{3}d\rho
           \int _{-{\sqrt {9a^{2}-\rho ^{2}}}}^{\sqrt {9a^{2}-\rho ^
           {2}}}\,dz&=2\pi \int _{0}^{3a}2\rho ^{3}{\sqrt {9a^{2}-\rho ^
           {2}}}\,d\rho \\&=-2\pi \int _{9a^{2}}^{0}(9a^{2}-t){\sqrt
           {t}}\,dt&&t=9a^{2}-\rho ^{2}\\&=2\pi \int _{0}^{9a^{2}}\left
           (9a^{2}{\sqrt {t}}-t{\sqrt {t}}\right)\,dt\\&=2\pi \left(\int _
           {0}^{9a^{2}}9a^{2}{\sqrt {t}}\,dt-\int _{0}^{9a^{2}}t{\sqrt
           {t}}\,dt\right)\\&=2\pi \left[9a^{2}{\frac {2}{3}}t^{\frac {3}
           {2}}-{\frac {2}{5}}t^{\frac {5}{2}}\right]_{0}^{9a^
           {2}}\\&=2\cdot 27\pi a^{5}\left(6-{\frac {18}{5}}\right)\\&=
           {\frac {648\pi }{5}}a^{5}.\end{aligned}}}  [{\displaystyle
           {\begin{aligned}\int _{0}^{2\pi }d\varphi \int _{0}^{3a}\rho ^
           {3}d\rho \int _{-{\sqrt {9a^{2}-\rho ^{2}}}}^{\sqrt {9a^{2}-
           \rho ^{2}}}\,dz&=2\pi \int _{0}^{3a}2\rho ^{3}{\sqrt {9a^{2}-
           \rho ^{2}}}\,d\rho \\&=-2\pi \int _{9a^{2}}^{0}(9a^{2}-t){\sqrt
           {t}}\,dt&&t=9a^{2}-\rho ^{2}\\&=2\pi \int _{0}^{9a^{2}}\left
           (9a^{2}{\sqrt {t}}-t{\sqrt {t}}\right)\,dt\\&=2\pi \left(\int _
           {0}^{9a^{2}}9a^{2}{\sqrt {t}}\,dt-\int _{0}^{9a^{2}}t{\sqrt
           {t}}\,dt\right)\\&=2\pi \left[9a^{2}{\frac {2}{3}}t^{\frac {3}
           {2}}-{\frac {2}{5}}t^{\frac {5}{2}}\right]_{0}^{9a^
           {2}}\\&=2\cdot 27\pi a^{5}\left(6-{\frac {18}{5}}\right)\\&=
           {\frac {648\pi }{5}}a^{5}.\end{aligned}}}]
     Thanks to the passage to cylindrical coordinates it was possible to
     reduce the triple integral to an easier one-variable integral.
See also the differential volume entry in nabla_in_cylindrical_and_spherical
coordinates.
***** Examples[edit] *****
**** Double integral over a rectangle[edit] ****
Let us assume that we wish to integrate a multivariable function f over a
region A:
         A =  {  ( x , y ) &#x2208;   R   2   &#xA0; : &#xA0; 11 &#x2264; x
      &#x2264; 14 &#xA0; ; &#xA0; 7 &#x2264; y &#x2264; 10  }
      &#xA0;and&#xA0;   f ( x , y ) =  x  2   + 4 y    {\displaystyle A=\left\{
      (x,y)\in \mathbf {R} ^{2}\ :\ 11\leq x\leq 14\ ;\ 7\leq y\leq 10\right\}
      {\mbox{ and }}f(x,y)=x^{2}+4y\,}  [{\displaystyle A=\left\{(x,y)\in
      \mathbf {R} ^{2}\ :\ 11\leq x\leq 14\ ;\ 7\leq y\leq 10\right\}{\mbox
      { and }}f(x,y)=x^{2}+4y\,}]
From this we formulate the iterated integral
          &#x222B;  7   10    &#x222B;  11   14   (  x  2   + 4 y )  d x  d y
      {\displaystyle \int _{7}^{10}\int _{11}^{14}(x^{2}+4y)\,dx\,dy}  [
      {\displaystyle \int _{7}^{10}\int _{11}^{14}(x^{2}+4y)\,dx\,dy}]
The inner integral is performed first, integrating with respect to x and taking
y as a constant, as it is not the variable_of_integration. The result of this
integral, which is a function depending only on y, is then integrated with
respect to y.
              &#x222B;  11   14    (   x  2   + 4 y  )   d x    =   [    1 3
      x  3   + 4 y x  ]   x = 11   x = 14         =   1 3   ( 14  )  3   + 4 y
      ( 14 ) &#x2212;   1 3   ( 11  )  3   &#x2212; 4 y ( 11 )       = 471 + 12
      y       {\displaystyle {\begin{aligned}\int _{11}^{14}\left(x^
      {2}+4y\right)\,dx&=\left[{\frac {1}{3}}x^{3}+4yx\right]_{x=11}^{x=14}\\&=
      {\frac {1}{3}}(14)^{3}+4y(14)-{\frac {1}{3}}(11)^{3}-4y
      (11)\\&=471+12y\end{aligned}}}  [{\displaystyle {\begin{aligned}\int _
      {11}^{14}\left(x^{2}+4y\right)\,dx&=\left[{\frac {1}{3}}x^{3}+4yx\right]_
      {x=11}^{x=14}\\&={\frac {1}{3}}(14)^{3}+4y(14)-{\frac {1}{3}}(11)^{3}-4y
      (11)\\&=471+12y\end{aligned}}}]
We then integrate the result with respect to y.
              &#x222B;  7   10   ( 471 + 12 y ) &#xA0; d y    =   [   471 y + 6
      y  2      ]    y = 7   y = 10         = 471 ( 10 ) + 6 ( 10  )  2
      &#x2212; 471 ( 7 ) &#x2212; 6 ( 7  )  2         = 1719
      {\displaystyle {\begin{aligned}\int _{7}^{10}(471+12y)\ dy&={\Big
      [}471y+6y^{2}{\Big ]}_{y=7}^{y=10}\\&=471(10)+6(10)^{2}-471(7)-6(7)^
      {2}\\&=1719\end{aligned}}}  [{\displaystyle {\begin{aligned}\int _{7}^
      {10}(471+12y)\ dy&={\Big [}471y+6y^{2}{\Big ]}_{y=7}^{y=10}\\&=471(10)+6
      (10)^{2}-471(7)-6(7)^{2}\\&=1719\end{aligned}}}]
In cases where the double integral of the absolute value of the function is
finite, the order of integration is interchangeable, that is, integrating with
respect to x first and integrating with respect to y first produce the same
result. That is Fubini's_theorem. For example, doing the previous calculation
with order reversed gives the same result:
              &#x222B;  11   14    &#x222B;  7   10     (   x  2   + 4 y  )   d
      y  d x    =  &#x222B;  11   14     [    x  2   y + 2  y  2      ]    y =
      7   y = 10    d x       =  &#x222B;  11   14    ( 3  x  2   + 102 )  d x
      =   [    x  3   + 102 x    ]    x = 11   x = 14         = 1719.
      {\displaystyle {\begin{aligned}\int _{11}^{14}\int _{7}^{10}\,\left(x^
      {2}+4y\right)\,dy\,dx&=\int _{11}^{14}{\Big [}x^{2}y+2y^{2}{\Big ]}_
      {y=7}^{y=10}\,dx\\&=\int _{11}^{14}\,(3x^{2}+102)\,dx\\&={\Big [}x^
      {3}+102x{\Big ]}_{x=11}^{x=14}\\&=1719.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}\int _{11}^{14}\int _{7}^{10}\,\left(x^
      {2}+4y\right)\,dy\,dx&=\int _{11}^{14}{\Big [}x^{2}y+2y^{2}{\Big ]}_
      {y=7}^{y=10}\,dx\\&=\int _{11}^{14}\,(3x^{2}+102)\,dx\\&={\Big [}x^
      {3}+102x{\Big ]}_{x=11}^{x=14}\\&=1719.\end{aligned}}}]
**** Double integral over a normal domain[edit] ****
Example: double integral over the normal region D
Consider the region (please see the graphic in the example):
         D = { ( x , y ) &#x2208;   R   2   &#xA0; : &#xA0; x &#x2265; 0 , y
      &#x2264; 1 , y &#x2265;  x  2   }   {\displaystyle D=\{(x,y)\in \mathbf
      {R} ^{2}\ :\ x\geq 0,y\leq 1,y\geq x^{2}\}}  [D=\{(x,y)\in \mathbf {R} ^
      {2}\ :\ x\geq 0,y\leq 1,y\geq x^{2}\}]
Calculate
          &#x222C;  D   ( x + y )  d x  d y .   {\displaystyle \iint _{D}
      (x+y)\,dx\,dy.}  [\iint _{D}(x+y)\,dx\,dy.]
This domain is normal with respect to both the x- and y-axes. To apply the
formulae it is required to find the functions that determine D and the
intervals over which these functions are defined. In this case the two
functions are:
         &#x03B1; ( x ) =  x  2    &#xA0;and&#xA0;  &#x03B2; ( x ) = 1
      {\displaystyle \alpha (x)=x^{2}{\text{ and }}\beta (x)=1}  [\alpha (x)=x^
      {2}{\text{ and }}\beta (x)=1]
while the interval is given by the intersections of the functions with x = 0,
so the interval is [a, b] = [0, 1] (normality has been chosen with respect to
the x-axis for a better visual understanding).
It is now possible to apply the formula:
          &#x222C;  D   ( x + y )  d x  d y =  &#x222B;  0   1   d x  &#x222B;
      x  2     1   ( x + y )  d y =  &#x222B;  0   1   d x &#xA0;   [  x y +
      y  2   2    ]    x  2     1     {\displaystyle \iint _{D}
      (x+y)\,dx\,dy=\int _{0}^{1}dx\int _{x^{2}}^{1}(x+y)\,dy=\int _{0}^{1}dx\
      \left[xy+{\frac {y^{2}}{2}}\right]_{x^{2}}^{1}}  [\iint _{D}
      (x+y)\,dx\,dy=\int _{0}^{1}dx\int _{x^{2}}^{1}(x+y)\,dy=\int _{0}^{1}dx\
      \left[xy+{\frac {y^{2}}{2}}\right]_{x^{2}}^{1}]
(at first the second integral is calculated considering x as a constant). The
remaining operations consist of applying the basic techniques of integration:
          &#x222B;  0   1     [  x y +    y  2   2    ]    x  2     1    d x =
      &#x222B;  0   1    (  x +   1 2   &#x2212;  x  3   &#x2212;    x  4   2
      )  d x = &#x22EF; =   13 20   .   {\displaystyle \int _{0}^{1}\left[xy+
      {\frac {y^{2}}{2}}\right]_{x^{2}}^{1}\,dx=\int _{0}^{1}\left(x+{\frac {1}
      {2}}-x^{3}-{\frac {x^{4}}{2}}\right)dx=\cdots ={\frac {13}{20}}.}  [\int
      _{0}^{1}\left[xy+{\frac {y^{2}}{2}}\right]_{x^{2}}^{1}\,dx=\int _{0}^
      {1}\left(x+{\frac {1}{2}}-x^{3}-{\frac {x^{4}}{2}}\right)dx=\cdots =
      {\frac {13}{20}}.]
If we choose normality with respect to the y-axis we could calculate
          &#x222B;  0   1   d y  &#x222B;  0    y    ( x + y )  d x .
      {\displaystyle \int _{0}^{1}dy\int _{0}^{\sqrt {y}}(x+y)\,dx.}  [\int _
      {0}^{1}dy\int _{0}^{\sqrt {y}}(x+y)\,dx.]
and obtain the same value.
Example of domain in R3 that is normal with respect to the xy-plane.
**** Calculating volume[edit] ****
Using the methods previously described, it is possible to calculate the volumes
of some common solids.
    * Cylinder: The volume of a cylinder with height h and circular base of
      radius R can be calculated by integrating the constant function h over
      the circular base, using polar coordinates.
                V o l u m e  =  &#x222B;  0   2 &#x03C0;   d &#x03C6;
            &#x222B;  0   R   h &#x03C1;  d &#x03C1; = 2 &#x03C0; h
            [    &#x03C1;  2   2   ]   0   R   = &#x03C0;  R  2   h
            {\displaystyle \mathrm {Volume} =\int _{0}^{2\pi }d\varphi \,\int _
            {0}^{R}h\rho \,d\rho =2\pi h\left[{\frac {\rho ^{2}}{2}}\right]_
            {0}^{R}=\pi R^{2}h}  [{\displaystyle \mathrm {Volume} =\int _{0}^
            {2\pi }d\varphi \,\int _{0}^{R}h\rho \,d\rho =2\pi h\left[{\frac
            {\rho ^{2}}{2}}\right]_{0}^{R}=\pi R^{2}h}]
This is in agreement with the formula for the volume of a prism
                V o l u m e  =  base area  &#x00D7;  height  .   {\displaystyle
            \mathrm {Volume} ={\text{base area}}\times {\text{height}}.}  [
            {\displaystyle \mathrm {Volume} ={\text{base area}}\times {\text
            {height}}.}]
    * Sphere: The volume of a sphere with radius R can be calculated by
      integrating the constant function 1 over the sphere, using spherical
      coordinates.
                    Volume     =  &#x222D;  D   f ( x , y , z )  d x  d y  d z
            =  &#x222D;  D   1  d V       =  &#x222D;  S    &#x03C1;  2   sin
            &#x2061; &#x03C6;  d &#x03C1;  d &#x03B8;  d &#x03C6;       =
            &#x222B;  0   2 &#x03C0;    d &#x03B8;  &#x222B;  0   &#x03C0;
            sin &#x2061; &#x03C6;  d &#x03C6;  &#x222B;  0   R    &#x03C1;  2
            d &#x03C1;       = 2 &#x03C0;  &#x222B;  0   &#x03C0;   sin
            &#x2061; &#x03C6;  d &#x03C6;  &#x222B;  0   R    &#x03C1;  2    d
            &#x03C1;       = 2 &#x03C0;  &#x222B;  0   &#x03C0;   sin &#x2061;
            &#x03C6;    R  3   3    d &#x03C6;       =   2 3   &#x03C0;  R  3
            [   &#x2212; cos &#x2061; &#x03C6;    ]    0   &#x03C0;   =   4 3
            &#x03C0;  R  3   .       {\displaystyle {\begin{aligned}{\text
            {Volume}}&=\iiint _{D}f(x,y,z)\,dx\,dy\,dz\\&=\iiint _
            {D}1\,dV\\&=\iiint _{S}\rho ^{2}\sin \varphi \,d\rho \,d\theta
            \,d\varphi \\&=\int _{0}^{2\pi }\,d\theta \int _{0}^{\pi }\sin
            \varphi \,d\varphi \int _{0}^{R}\rho ^{2}\,d\rho \\&=2\pi \int _
            {0}^{\pi }\sin \varphi \,d\varphi \int _{0}^{R}\rho ^{2}\,d\rho
            \\&=2\pi \int _{0}^{\pi }\sin \varphi {\frac {R^{3}}{3}}\,d\varphi
            \\&={\frac {2}{3}}\pi R^{3}{\Big [}-\cos \varphi {\Big ]}_{0}^{\pi
            }={\frac {4}{3}}\pi R^{3}.\end{aligned}}}  [{\displaystyle {\begin
            {aligned}{\text{Volume}}&=\iiint _{D}f(x,y,z)\,dx\,dy\,dz\\&=\iiint
            _{D}1\,dV\\&=\iiint _{S}\rho ^{2}\sin \varphi \,d\rho \,d\theta
            \,d\varphi \\&=\int _{0}^{2\pi }\,d\theta \int _{0}^{\pi }\sin
            \varphi \,d\varphi \int _{0}^{R}\rho ^{2}\,d\rho \\&=2\pi \int _
            {0}^{\pi }\sin \varphi \,d\varphi \int _{0}^{R}\rho ^{2}\,d\rho
            \\&=2\pi \int _{0}^{\pi }\sin \varphi {\frac {R^{3}}{3}}\,d\varphi
            \\&={\frac {2}{3}}\pi R^{3}{\Big [}-\cos \varphi {\Big ]}_{0}^{\pi
            }={\frac {4}{3}}\pi R^{3}.\end{aligned}}}]
    * Tetrahedron (triangular pyramid or 3-simplex): The volume of a
      tetrahedron with its apex at the origin and edges of length â along the
      x-, y- and z-axes can be calculated by integrating the constant function
      1 over the tetrahedron.
                    Volume     =  &#x222B;  0   &#x2113;   d x  &#x222B;  0
            &#x2113; &#x2212; x    d y  &#x222B;  0   &#x2113; &#x2212; x
            &#x2212; y    d z       =  &#x222B;  0   &#x2113;   d x  &#x222B;
            0   &#x2113; &#x2212; x   ( &#x2113; &#x2212; x &#x2212; y )  d y
            =  &#x222B;  0   &#x2113;    (   l  2   &#x2212; 2 &#x2113; x +  x
            2   &#x2212;    ( &#x2113; &#x2212; x  )  2    2    )   d x       =
            &#x2113;  3   &#x2212; &#x2113;  &#x2113;  2   +    &#x2113;  3   3
            &#x2212;   [      &#x2113;  2   x  2   &#x2212;    &#x2113;  x  2
            2   +    x  3   6    ]   0   &#x2113;         =    &#x2113;  3   3
            &#x2212;    &#x2113;  3   6   =    &#x2113;  3   6
            {\displaystyle {\begin{aligned}{\text{Volume}}&=\int _{0}^{\ell
            }dx\int _{0}^{\ell -x}\,dy\int _{0}^{\ell -x-y}\,dz\\&=\int _{0}^
            {\ell }dx\int _{0}^{\ell -x}(\ell -x-y)\,dy\\&=\int _{0}^{\ell
            }\left(l^{2}-2\ell x+x^{2}-{\frac {(\ell -x)^{2}}
            {2}}\right)\,dx\\&=\ell ^{3}-\ell \ell ^{2}+{\frac {\ell ^{3}}{3}}-
            \left[{\frac {\ell ^{2}x}{2}}-{\frac {\ell x^{2}}{2}}+{\frac {x^
            {3}}{6}}\right]_{0}^{\ell }\\&={\frac {\ell ^{3}}{3}}-{\frac {\ell
            ^{3}}{6}}={\frac {\ell ^{3}}{6}}\end{aligned}}}  [{\displaystyle
            {\begin{aligned}{\text{Volume}}&=\int _{0}^{\ell }dx\int _{0}^{\ell
            -x}\,dy\int _{0}^{\ell -x-y}\,dz\\&=\int _{0}^{\ell }dx\int _{0}^
            {\ell -x}(\ell -x-y)\,dy\\&=\int _{0}^{\ell }\left(l^{2}-2\ell x+x^
            {2}-{\frac {(\ell -x)^{2}}{2}}\right)\,dx\\&=\ell ^{3}-\ell \ell ^
            {2}+{\frac {\ell ^{3}}{3}}-\left[{\frac {\ell ^{2}x}{2}}-{\frac
            {\ell x^{2}}{2}}+{\frac {x^{3}}{6}}\right]_{0}^{\ell }\\&={\frac
            {\ell ^{3}}{3}}-{\frac {\ell ^{3}}{6}}={\frac {\ell ^{3}}{6}}\end
            {aligned}}}]
      This is in agreement with the formula for the volume of a pyramid
                V o l u m e  =   1 3   &#x00D7;  base area  &#x00D7;  height  =
            1 3   &#x00D7;    &#x2113;  2   2   &#x00D7; &#x2113; =    &#x2113;
            3   6   .   {\displaystyle \mathrm {Volume} ={\frac {1}{3}}\times
            {\text{base area}}\times {\text{height}}={\frac {1}{3}}\times
            {\frac {\ell ^{2}}{2}}\times \ell ={\frac {\ell ^{3}}{6}}.}  [
            {\displaystyle \mathrm {Volume} ={\frac {1}{3}}\times {\text{base
            area}}\times {\text{height}}={\frac {1}{3}}\times {\frac {\ell ^
            {2}}{2}}\times \ell ={\frac {\ell ^{3}}{6}}.}]
Example of an improper domain.
***** Multiple improper integral[edit] *****
In case of unbounded domains or functions not bounded near the boundary of the
domain, we have to introduce the double improper_integral or the triple
improper integral.
***** Multiple integrals and iterated integrals[edit] *****
See also: Order_of_integration_(calculus)
Fubini's_theorem states that if[4]
          &#x222C;  A &#x00D7; B    |  f ( x , y )  |   d ( x , y ) < &#x221E;
      ,   {\displaystyle \iint _{A\times B}\left|f(x,y)\right|\,d(x,y)<\infty
      ,}  [{\displaystyle \iint _{A\times B}\left|f(x,y)\right|\,d(x,y)<\infty
      ,}]
that is, if the integral is absolutely convergent, then the multiple integral
will give the same result as either of the two iterated integrals:
          &#x222C;  A &#x00D7; B   f ( x , y )  d ( x , y ) =  &#x222B;  A
      (   &#x222B;  B   f ( x , y )  d y  )   d x =  &#x222B;  B
      (   &#x222B;  A   f ( x , y )  d x  )   d y .   {\displaystyle \iint _
      {A\times B}f(x,y)\,d(x,y)=\int _{A}\left(\int _{B}f
      (x,y)\,dy\right)\,dx=\int _{B}\left(\int _{A}f(x,y)\,dx\right)\,dy.}
      [\iint _{A\times B}f(x,y)\,d(x,y)=\int _{A}\left(\int _{B}f
      (x,y)\,dy\right)\,dx=\int _{B}\left(\int _{A}f(x,y)\,dx\right)\,dy.]
In particular this will occur if |f(x, y)| is a bounded_function and A and B
are bounded_sets.
If the integral is not absolutely convergent, care is needed not to confuse the
concepts of multiple integral and iterated integral, especially since the same
notation is often used for either concept. The notation
          &#x222B;  0   1    &#x222B;  0   1   f ( x , y )  d y  d x
      {\displaystyle \int _{0}^{1}\int _{0}^{1}f(x,y)\,dy\,dx}  [\int _{0}^
      {1}\int _{0}^{1}f(x,y)\,dy\,dx]
means, in some cases, an iterated integral rather than a true double integral.
In an iterated integral, the outer integral
          &#x222B;  0   1   &#x22EF;  d x   {\displaystyle \int _{0}^{1}\cdots
      \,dx}  [\int _{0}^{1}\cdots \,dx]
is the integral with respect to x of the following function of x:
         g ( x ) =  &#x222B;  0   1   f ( x , y )  d y .   {\displaystyle g
      (x)=\int _{0}^{1}f(x,y)\,dy.}  [g(x)=\int _{0}^{1}f(x,y)\,dy.]
A double integral, on the other hand, is defined with respect to area in the
xy-plane. If the double integral exists, then it is equal to each of the two
iterated integrals (either "dy dx" or "dx dy") and one often computes it by
computing either of the iterated integrals. But sometimes the two iterated
integrals exist when the double integral does not, and in some such cases the
two iterated integrals are different numbers, i.e., one has
          &#x222B;  0   1    &#x222B;  0   1   f ( x , y )  d y  d x &#x2260;
      &#x222B;  0   1    &#x222B;  0   1   f ( x , y )  d x  d y .
      {\displaystyle \int _{0}^{1}\int _{0}^{1}f(x,y)\,dy\,dx\neq \int _{0}^
      {1}\int _{0}^{1}f(x,y)\,dx\,dy.}  [\int _{0}^{1}\int _{0}^{1}f
      (x,y)\,dy\,dx\neq \int _{0}^{1}\int _{0}^{1}f(x,y)\,dx\,dy.]
This is an instance of rearrangement of a conditionally_convergent integral.
On the other hand, some conditions ensure that the two iterated integrals are
equal even though the double integral need not exist. By the
FichtenholzâLichtenstein theorem, if f is bounded on [0, 1] Ã [0, 1] and
both iterated integrals exist, then they are equal. Moreover, existence of the
inner integrals ensures existence of the outer integrals.[6][7][8] The double
integral need not exist in this case even as Lebesgue_integral, according to
SierpiÅski.[9]
The notation
          &#x222B;  [ 0 , 1 ] &#x00D7; [ 0 , 1 ]   f ( x , y )  d x  d y
      {\displaystyle \int _{[0,1]\times [0,1]}f(x,y)\,dx\,dy}  [\int _{
      [0,1]\times [0,1]}f(x,y)\,dx\,dy]
may be used if one wishes to be emphatic about intending a double integral
rather than an iterated integral.
***** Some practical applications[edit] *****
Quite generally, just as in one variable, one can use the multiple integral to
find the average of a function over a given set. Given a set D â Rn and an
integrable function f over D, the average value of f over its domain is given
by
            f &#x00AF;    =   1  m ( D )     &#x222B;  D   f ( x )  d x ,
      {\displaystyle {\bar {f}}={\frac {1}{m(D)}}\int _{D}f(x)\,dx,}  [{\bar
      {f}}={\frac {1}{m(D)}}\int _{D}f(x)\,dx,]
where m(D) is the measure of D.
Additionally, multiple integrals are used in many applications in physics. The
examples below also show some variations in the notation.
In mechanics, the moment_of_inertia is calculated as the volume integral
(triple integral) of the density weighed with the square of the distance from
the axis:
          I  z   =  &#x222D;  V   &#x03C1;  r  2    d V .   {\displaystyle I_
      {z}=\iiint _{V}\rho r^{2}\,dV.}  [I_{z}=\iiint _{V}\rho r^{2}\,dV.]
The gravitational_potential associated with a mass_distribution given by a mass
measure dm on three-dimensional Euclidean_space R3 is[10]
         V (  x  ) = &#x2212;  &#x222D;    R   3       G   |   x  &#x2212;  y
      |      d m (  y  ) .   {\displaystyle V(\mathbf {x} )=-\iiint _{\mathbf
      {R} ^{3}}{\frac {G}{|\mathbf {x} -\mathbf {y} |}}\,dm(\mathbf {y} ).}  [V
      (\mathbf {x} )=-\iiint _{\mathbf {R} ^{3}}{\frac {G}{|\mathbf {x} -
      \mathbf {y} |}}\,dm(\mathbf {y} ).]
If there is a continuous function Ï(x) representing the density of the
distribution at x, so that dm(x) = Ï(x)d3x, where d3x is the Euclidean volume
element, then the gravitational potential is
         V (  x  ) = &#x2212;  &#x222D;    R   3       G   |   x  &#x2212;  y
      |      &#x03C1; (  y  )   d  3    y  .   {\displaystyle V(\mathbf {x} )=-
      \iiint _{\mathbf {R} ^{3}}{\frac {G}{|\mathbf {x} -\mathbf {y} |}}\,\rho
      (\mathbf {y} )\,d^{3}\mathbf {y} .}  [V(\mathbf {x} )=-\iiint _{\mathbf
      {R} ^{3}}{\frac {G}{|\mathbf {x} -\mathbf {y} |}}\,\rho (\mathbf {y}
      )\,d^{3}\mathbf {y} .]
In electromagnetism, Maxwell's_equations can be written using multiple
integrals to calculate the total magnetic and electric fields.[11] In the
following example, the electric_field produced by a distribution of charges
given by the volume charge_density Ï( râ ) is obtained by a triple integral
of a vector function:
            E &#x2192;    =   1  4 &#x03C0;  &#x03B5;  0      &#x222D;       r
      &#x2192;    &#x2212;     r &#x2192;    &#x2032;     &#x2016;     r
      &#x2192;    &#x2212;     r &#x2192;    &#x2032;   &#x2016;   3
      &#x03C1; (     r &#x2192;    &#x2032;  )   d  3    r &#x2032;  .
      {\displaystyle {\vec {E}}={\frac {1}{4\pi \varepsilon _{0}}}\iiint {\frac
      {{\vec {r}}-{\vec {r}}'}{\left\|{\vec {r}}-{\vec {r}}'\right\|^{3}}}\rho
      ({\vec {r}}')\,d^{3}r'.}  [{\displaystyle {\vec {E}}={\frac {1}{4\pi
      \varepsilon _{0}}}\iiint {\frac {{\vec {r}}-{\vec {r}}'}{\left\|{\vec
      {r}}-{\vec {r}}'\right\|^{3}}}\rho ({\vec {r}}')\,d^{3}r'.}]
This can also be written as an integral with respect to a signed_measure
representing the charge distribution.
***** See also[edit] *****
    * Main analysis theorems that relate multiple integrals:
          o Divergence_theorem
          o Stokes'_theorem
          o Green's_theorem
***** References[edit] *****
   1. ^ a b cStewart,_James (2008). Calculus: Early Transcendentals (6th ed.).
      Brooks Cole Cengage Learning. ISBN 978-0-495-01166-8.
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
   3. ^Larson; Edwards (2014). Multivariable Calculus (10th ed.). Cengage
      Learning. ISBN 978-1-285-08575-3.
   4. ^Rudin,_Walter. Principles of Mathematical Analysis. Walter Rudin Student
      Series in Advanced Mathematics (3rd ed.). McGrawâHill. ISBN 978-0-07-
      054235-8.
   5. ^ a bJones, Frank (2001). Lebesgue Integration on Euclidean Space. Jones
      and Bartlett. pp. 527â529.
   6. [ISBN missing]
   7. ^Stewart, James (2015-05-07). Calculus, 8th Edition. Cengage Learning.
      ISBN 978-1285740621.
   8. ^Lewin, Jonathan (2003). An Interactive Introduction to Mathematical
      Analysis. Cambridge. Sect. 16.6. ISBN 978-1107694040.
   9. ^Lewin, Jonathan (1987). "Some_applications_of_the_bounded_convergence
      theorem_for_an_introductory_course_in_analysis". The American
      Mathematical Monthly. AMS. 94 (10): 988â993. doi:10.2307/2322609.
      JSTOR 2322609.
  10. ^Sinclair, George Edward (1974). "A finitely additive generalization of
      the FichtenholzâLichtenstein theorem". Transactions of the American
      Mathematical Society. AMS. 193: 359â374. doi:10.2307/1996919.
      JSTOR 1996919.
  11. ^Bogachev, Vladimir I. (2006). Measure Theory. 1. Springer. Item 3.10.49.
  12. [ISBN missing]
  13. ^Kibble, Tom W. B.; Berkshire,_Frank_H. (2004). Classical_Mechanics (5th
      ed.). Imperial_College_Press. ISBN 978-1-86094-424-6.
  14. ^Jackson,_John_D. (1998). Classical Electrodynamics (3rd ed.). Wiley.
      ISBN 0-471-30932-X.
***** Further reading[edit] *****
    * Adams, Robert A. (2003). Calculus: A Complete Course (5th ed.). ISBN 0-
      201-79131-5.
Jain, R. K.; Iyengar, S. R. K. (2009). Advanced Engineering Mathematics (3rd
ed.). Narosa Publishing House. ISBN 978-81-7319-730-7.
***** External links[edit] *****
    * Weisstein,_Eric_W. "Multiple_Integral". MathWorld.
L.D. Kudryavtsev (2001) [1994], "Multiple_integral", in Hazewinkel,_Michiel
(ed.), Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Mathematical_Assistant_on_Web online evaluation of double integrals in
Cartesian_coordinates and polar_coordinates (includes intermediate steps in the
solution, powered by Maxima_(software))

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Multiple_integral&oldid=905269485"
Categories:
    * Integral_calculus
    * Multivariable_calculus
Hidden categories:
    * Pages_with_missing_ISBNs
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
    * Bosanski
    * CatalÃ 
    * Ð§ÓÐ²Ð°ÑÐ»Ð°
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 8 July 2019, at 01:18 (UTC).
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
