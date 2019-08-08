The following text has been accessed from https://en.wikipedia.org/wiki/Triangle_inequality at Thu Aug 8 23:10:50 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Triangle inequality ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the basic inequality     z &#x2264; x + y
{\displaystyle z\leq x+y}  [{\displaystyle z\leq x+y}]. For other inequalities
associated with triangles, see List_of_triangle_inequalities.
Three examples of the triangle inequality for triangles with sides of lengths
x, y, z. The top example shows a case where z is much less than the sum x + y
of the other two sides, and the bottom example shows a case where the side z is
only slightly less than x + y.
In mathematics, the triangle inequality states that for any triangle, the sum
of the lengths of any two sides must be greater than or equal to the length of
the remaining side.[1][2] This statement permits the inclusion of degenerate
triangles, but some authors, especially those writing about elementary
geometry, will exclude this possibility, thus leaving out the possibility of
equality.[3] If x, y, and z are the lengths of the sides of the triangle, with
no side being greater than z, then the triangle inequality states that
         z &#x2264; x + y ,   {\displaystyle z\leq x+y,}  [z\leq x+y,]
with equality only in the degenerate case of a triangle with zero area. In
Euclidean_geometry and some other geometries, the triangle inequality is a
theorem about distances, and it is written using vectors and vector lengths
(norms):
         &#x2016;  x  +  y  &#x2016; &#x2264; &#x2016;  x  &#x2016; + &#x2016;
      y  &#x2016; ,   {\displaystyle \|\mathbf {x} +\mathbf {y} \|\leq
      \|\mathbf {x} \|+\|\mathbf {y} \|,}  [\|\mathbf {x} +\mathbf {y} \|\leq
      \|\mathbf {x} \|+\|\mathbf {y} \|,]
where the length z of the third side has been replaced by the vector sum x + y.
When x and y are real_numbers, they can be viewed as vectors in â1, and the
triangle inequality expresses a relationship between absolute_values.
In Euclidean geometry, for right_triangles the triangle inequality is a
consequence of the Pythagorean_theorem, and for general triangles, a
consequence of the law_of_cosines, although it may be proven without these
theorems. The inequality can be viewed intuitively in either â2 or â3. The
figure at the right shows three examples beginning with clear inequality (top)
and approaching equality (bottom). In the Euclidean case, equality occurs only
if the triangle has a 180Â° angle and two 0Â° angles, making the three vertices
collinear, as shown in the bottom example. Thus, in Euclidean geometry, the
shortest distance between two points is a straight line.
In spherical_geometry, the shortest distance between two points is an arc of a
great_circle, but the triangle inequality holds provided the restriction is
made that the distance between two points on a sphere is the length of a minor
spherical line segment (that is, one with central angle in [0, Ï]) with those
endpoints.[4][5]
The triangle inequality is a defining property of norms and measures of
distance. This property must be established as a theorem for any function
proposed for such purposes for each particular space: for example, spaces such
as the real_numbers, Euclidean_spaces, the Lp_spaces (p â¥ 1), and inner
product_spaces.
⁰
***** Contents *****
    * 1_Euclidean_geometry
          o 1.1_Mathematical_expression_of_the_constraint_on_the_sides_of_a
            triangle
          o 1.2_Right_triangle
          o 1.3_Examples_of_use
          o 1.4_Generalization_to_any_polygon
                # 1.4.1_Example_of_the_generalized_polygon_inequality_for_a
                  quadrilateral
                # 1.4.2_Relationship_with_shortest_paths
          o 1.5_Converse
          o 1.6_Generalization_to_higher_dimensions
    * 2_Normed_vector_space
          o 2.1_Example_norms
    * 3_Metric_space
    * 4_Reverse_triangle_inequality
    * 5_Reversal_in_Minkowski_space
    * 6_See_also
    * 7_Notes
    * 8_References
    * 9_External_links
***** Euclidean geometry[edit] *****
Euclid's construction for proof of the triangle inequality for plane geometry.
Euclid proved the triangle inequality for distances in plane_geometry using the
construction in the figure.[6] Beginning with triangle ABC, an isosceles
triangle is constructed with one side taken as BC and the other equal leg BD
along the extension of side AB. It then is argued that angle Î² > Î±, so side
AD > AC. But AD = AB + BD = AB + BC so the sum of sides AB + BC > AC. This
proof appears in Euclid's_Elements, Book 1, Proposition 20.[7]
**** Mathematical expression of the constraint on the sides of a triangle[edit]
****
For a proper triangle, the triangle inequality, as stated in words, literally
translates into three inequalities (given that a proper triangle has side
lengths a, b, c that are all positive and excludes the degenerate case of zero
area):
         a + b > c ,  b + c > a ,  c + a > b .   {\displaystyle a+b>c,\quad
      b+c>a,\quad c+a>b.}  [a+b>c,\quad b+c>a,\quad c+a>b.]
A more succinct form of this inequality system can be shown to be
          |  a &#x2212; b  |  < c < a + b .   {\displaystyle |a-b|<c<a+b.}
      [|a-b|<c<a+b.]
Another way to state it is
         max ( a ,  &#xA0;  b ,  &#xA0;  c ) < a + b + c &#x2212; max ( a ,
      &#xA0;  b ,  &#xA0;  c )   {\displaystyle \max(a,{\text{ }}b,{\text
      { }}c)<a+b+c-\max(a,{\text{ }}b,{\text{ }}c)}  [{\displaystyle \max(a,
      {\text{ }}b,{\text{ }}c)<a+b+c-\max(a,{\text{ }}b,{\text{ }}c)}]
implying
         2 max ( a ,  &#xA0;  b ,  &#xA0;  c ) < a + b + c   {\displaystyle
      2\max(a,{\text{ }}b,{\text{ }}c)<a+b+c}  [{\displaystyle 2\max(a,{\text
      { }}b,{\text{ }}c)<a+b+c}]
and thus that the longest side length is less than the semiperimeter.
A mathematically equivalent formulation is that the area of a triangle with
sides a, b, c must be a real number greater than zero. Heron's_formula for the
area is
             4 &#x22C5;  area     =   ( a + b + c ) ( &#x2212; a + b + c ) ( a
      &#x2212; b + c ) ( a + b &#x2212; c )         =   &#x2212;  a  4
      &#x2212;  b  4   &#x2212;  c  4   + 2  a  2    b  2   + 2  a  2    c  2
      + 2  b  2    c  2     .       {\displaystyle {\begin{aligned}4\cdot
      {\text{area}}&={\sqrt {(a+b+c)(-a+b+c)(a-b+c)(a+b-c)}}\\&={\sqrt {-a^{4}-
      b^{4}-c^{4}+2a^{2}b^{2}+2a^{2}c^{2}+2b^{2}c^{2}}}.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}4\cdot {\text{area}}&={\sqrt {(a+b+c)(-
      a+b+c)(a-b+c)(a+b-c)}}\\&={\sqrt {-a^{4}-b^{4}-c^{4}+2a^{2}b^{2}+2a^{2}c^
      {2}+2b^{2}c^{2}}}.\end{aligned}}}]
In terms of either area expression, the triangle inequality imposed on all
sides is equivalent to the condition that the expression under the square root
sign be real and greater than zero (so the area expression is real and greater
than zero).
The triangle inequality provides two more interesting constraints for triangles
whose sides are a, b, c, where a ≥ b ≥ c and    &#x03D5;   {\displaystyle \phi
}  [\phi ] is the golden_ratio, as
         1 <    a + c  b   < 3   {\displaystyle 1<{\frac {a+c}{b}}<3}  [
      {\displaystyle 1<{\frac {a+c}{b}}<3}]
         1 &#x2264; min (   a b   ,  &#xA0;    b c   ) < &#x03D5; .
      {\displaystyle 1\leq \min({\frac {a}{b}},{\text{ }}{\frac {b}{c}})<\phi
      .}  [{\displaystyle 1\leq \min({\frac {a}{b}},{\text{ }}{\frac {b}
      {c}})<\phi .}][8]
**** Right triangle[edit] ****
Isosceles triangle with equal sides AB = AC divided into two right triangles by
an altitude drawn from one of the two base angles.
In the case of right triangles, the triangle inequality specializes to the
statement that the hypotenuse is greater than either of the two sides and less
than their sum.[9]
The second part of this theorem is already established above for any side of
any triangle. The first part is established using the lower figure. In the
figure, consider the right triangle ADC. An isosceles triangle ABC is
constructed with equal sides AB = AC. From the triangle_postulate, the angles
in the right triangle ADC satisfy:
         &#x03B1; + &#x03B3; = &#x03C0;  /  2 &#xA0; .   {\displaystyle \alpha
      +\gamma =\pi /2\ .}  [\alpha +\gamma =\pi /2\ .]
Likewise, in the isosceles triangle ABC, the angles satisfy:
         2 &#x03B2; + &#x03B3; = &#x03C0; &#xA0; .   {\displaystyle 2\beta
      +\gamma =\pi \ .}  [2\beta +\gamma =\pi \ .]
Therefore,
         &#x03B1; = &#x03C0;  /  2 &#x2212; &#x03B3; , &#xA0;  w h i l e
      &#xA0; &#x03B2; = &#x03C0;  /  2 &#x2212; &#x03B3;  /  2 &#xA0; ,
      {\displaystyle \alpha =\pi /2-\gamma ,\ \mathrm {while} \ \beta =\pi /2-
      \gamma /2\ ,}  [\alpha =\pi /2-\gamma ,\ \mathrm {while} \ \beta =\pi /2-
      \gamma /2\ ,]
and so, in particular,
         &#x03B1; < &#x03B2; &#xA0; .   {\displaystyle \alpha <\beta \ .}
      [\alpha <\beta \ .]
That means side AD opposite angle Î± is shorter than side AB opposite the
larger angle Î². But AB = AC. Hence:
            A C  &#x00AF;   >    A D  &#x00AF;   &#xA0; .   {\displaystyle
      {\overline {\mathrm {AC} }}>{\overline {\mathrm {AD} }}\ .}  [{\overline
      {\mathrm {AC} }}>{\overline {\mathrm {AD} }}\ .]
A similar construction shows AC > DC, establishing the theorem.
An alternative proof (also based upon the triangle postulate) proceeds by
considering three positions for point B:[10] (i) as depicted (which is to be
proven), or (ii) B coincident with D (which would mean the isosceles triangle
had two right angles as base angles plus the vertex angle Î³, which would
violate the triangle_postulate), or lastly, (iii) B interior to the right
triangle between points A and D (in which case angle ABC is an exterior angle
of a right triangle BDC and therefore larger than Ï/2, meaning the other base
angle of the isosceles triangle also is greater than Ï/2 and their sum exceeds
Ï in violation of the triangle postulate).
This theorem establishing inequalities is sharpened by Pythagoras'_theorem to
the equality that the square of the length of the hypotenuse equals the sum of
the squares of the other two sides.
**** Examples of use[edit] ****
Consider a triangle whose sides are in an arithmetic_progression and let the
sides be a, a + d, a + 2d. Then the triangle inequality requires that
         0 < a < 2 a + 3 d   {\displaystyle 0<a<2a+3d}  [{\displaystyle
      0<a<2a+3d}]
         0 < a + d < 2 a + 2 d   {\displaystyle 0<a+d<2a+2d}  [{\displaystyle
      0<a+d<2a+2d}]
         0 < a + 2 d < 2 a + d .   {\displaystyle 0<a+2d<2a+d.}  [
      {\displaystyle 0<a+2d<2a+d.}]
To satisfy all these inequalities requires
         a > 0  &#xA0;and&#xA0;  &#x2212;   a 3   < d < a .   {\displaystyle
      a>0{\text{ and }}-{\frac {a}{3}}<d<a.}  [a>0{\text{ and }}-{\frac {a}
      {3}}<d<a.][11]
When d is chosen such that d = a/3, it generates a right triangle that is
always similar to the Pythagorean_triple with sides 3, 4, 5.
Now consider a triangle whose sides are in a geometric_progression and let the
sides be a, ar, ar2. Then the triangle inequality requires that
         0 < a < a r + a  r  2     {\displaystyle 0<a<ar+ar^{2}}  [
      {\displaystyle 0<a<ar+ar^{2}}]
         0 < a r < a + a  r  2     {\displaystyle 0<ar<a+ar^{2}}  [
      {\displaystyle 0<ar<a+ar^{2}}]
         0 < a  r  2   < a + a r .   {\displaystyle 0<ar^{2}<a+ar.}  [
      {\displaystyle 0<ar^{2}<a+ar.}]
The first inequality requires a > 0; consequently it can be divided through and
eliminated. With a > 0, the middle inequality only requires r > 0. This now
leaves the first and third inequalities needing to satisfy
              r  2   + r &#x2212; 1      > 0      r  2   &#x2212; r &#x2212; 1
      < 0.       {\displaystyle {\begin{aligned}r^{2}+r-1&{}>0\\r^{2}-r-1&
      {}<0.\end{aligned}}}  [{\displaystyle {\begin{aligned}r^{2}+r-1&{}>0\\r^
      {2}-r-1&{}<0.\end{aligned}}}]
The first of these quadratic inequalities requires r to range in the region
beyond the value of the positive root of the quadratic equation r2 + r â 1 =
0, i.e. r > Ï â 1 where Ï is the golden_ratio. The second quadratic
inequality requires r to range between 0 and the positive root of the quadratic
equation r2 â r â 1 = 0, i.e. 0 < r < Ï. The combined requirements result
in r being confined to the range
         &#x03C6; &#x2212; 1 < r < &#x03C6;   &#xA0;and&#xA0;  a > 0.
      {\displaystyle \varphi -1<r<\varphi \,{\text{ and }}a>0.}  [
      {\displaystyle \varphi -1<r<\varphi \,{\text{ and }}a>0.}][12]
When r the common ratio is chosen such that r = √Ï it generates a right
triangle that is always similar to the Kepler_triangle.
**** Generalization to any polygon[edit] ****
The triangle inequality can be extended by mathematical_induction to arbitrary
polygonal paths, showing that the total length of such a path is no less than
the length of the straight line between its endpoints. Consequently, the length
of any polygon side is always less than the sum of the other polygon side
lengths.
*** Example of the generalized polygon inequality for a quadrilateral[edit] ***
Consider a quadrilateral whose sides are in a geometric_progression and let the
sides be a, ar, ar2, ar3. Then the generalized polygon inequality requires that
         0 < a < a r + a  r  2   + a  r  3     {\displaystyle 0<a<ar+ar^{2}+ar^
      {3}}  [{\displaystyle 0<a<ar+ar^{2}+ar^{3}}]
         0 < a r < a + a  r  2   + a  r  3     {\displaystyle 0<ar<a+ar^{2}+ar^
      {3}}  [{\displaystyle 0<ar<a+ar^{2}+ar^{3}}]
         0 < a  r  2   < a + a r + a  r  3     {\displaystyle 0<ar^{2}<a+ar+ar^
      {3}}  [{\displaystyle 0<ar^{2}<a+ar+ar^{3}}]
         0 < a  r  3   < a + a r + a  r  2   .   {\displaystyle 0<ar^
      {3}<a+ar+ar^{2}.}  [{\displaystyle 0<ar^{3}<a+ar+ar^{2}.}]
These inequalities for a > 0 reduce to the following
          r  3   +  r  2   + r &#x2212; 1 > 0   {\displaystyle r^{3}+r^{2}+r-
      1>0}  [{\displaystyle r^{3}+r^{2}+r-1>0}]
          r  3   &#x2212;  r  2   &#x2212; r &#x2212; 1 < 0.   {\displaystyle
      r^{3}-r^{2}-r-1<0.}  [{\displaystyle r^{3}-r^{2}-r-1<0.}][13]
The left-hand side polynomials of these two inequalities have roots that are
the tribonacci_constant and its reciprocal. Consequently, r is limited to the
range 1/t < r < t where t is the tribonacci constant.
*** Relationship with shortest paths[edit] ***
The arc length of a curve is defined as the least upper bound of the lengths of
polygonal approximations.
This generalization can be used to prove that the shortest curve between two
points in Euclidean geometry is a straight line.
No polygonal path between two points is shorter than the line between them.
This implies that no curve can have an arc_length less than the distance
between its endpoints. By definition, the arc length of a curve is the least
upper_bound of the lengths of all polygonal approximations of the curve. The
result for polygonal paths shows that the straight line between the endpoints
is the shortest of all the polygonal approximations. Because the arc length of
the curve is greater than or equal to the length of every polygonal
approximation, the curve itself cannot be shorter than the straight line path.
[14]
**** Converse[edit] ****
The converse of the triangle inequality theorem is also true: if three real
numbers are such that each is less than the sum of the others, then there
exists a triangle with these numbers as its side lengths and with positive
area; and if one number equals the sum of the other two, there exists a
degenerate triangle (that is, with zero area) with these numbers as its side
lengths.
In either case, if the side lengths are a, b, c we can attempt to place a
triangle in the Euclidean_plane as shown in the diagram. We need to prove that
there exists a real number h consistent with the values a, b, and c, in which
case this triangle exists.
Triangle with altitude h cutting base c into d + (c â d).
By the Pythagorean_theorem we have b2 = h2 + d2 and a2 = h2 + (c â d)2
according to the figure at the right. Subtracting these yields a2 â b2 = c2
â 2cd. This equation allows us to express d in terms of the sides of the
triangle:
         d =    &#x2212;  a  2   +  b  2   +  c  2     2 c    .
      {\displaystyle d={\frac {-a^{2}+b^{2}+c^{2}}{2c}}.}  [d=\frac{-
      a^2+b^2+c^2}{2c}.]
For the height of the triangle we have that h2 = b2 â d2. By replacing d with
the formula given above, we have
          h  2   =  b  2   &#x2212;   (    &#x2212;  a  2   +  b  2   +  c  2
      2 c    )   2   .   {\displaystyle h^{2}=b^{2}-\left({\frac {-a^{2}+b^
      {2}+c^{2}}{2c}}\right)^{2}.}  [{\displaystyle h^{2}=b^{2}-\left({\frac {-
      a^{2}+b^{2}+c^{2}}{2c}}\right)^{2}.}]
For a real number h to satisfy this,      h  2     {\displaystyle h^{2}}  [h^
{2}] must be non-negative:
          b  2   &#x2212;   (    &#x2212;  a  2   +  b  2   +  c  2     2 c
      )   2   &#x2265; 0 ,   {\displaystyle b^{2}-\left({\frac {-a^{2}+b^{2}+c^
      {2}}{2c}}\right)^{2}\geq 0,}  [{\displaystyle b^{2}-\left({\frac {-a^
      {2}+b^{2}+c^{2}}{2c}}\right)^{2}\geq 0,}]
          (  b &#x2212;    &#x2212;  a  2   +  b  2   +  c  2     2 c     )
      (  b +    &#x2212;  a  2   +  b  2   +  c  2     2 c     )  &#x2265; 0 ,
      {\displaystyle \left(b-{\frac {-a^{2}+b^{2}+c^{2}}{2c}}\right)\left(b+
      {\frac {-a^{2}+b^{2}+c^{2}}{2c}}\right)\geq 0,}  [{\displaystyle \left(b-
      {\frac {-a^{2}+b^{2}+c^{2}}{2c}}\right)\left(b+{\frac {-a^{2}+b^{2}+c^
      {2}}{2c}}\right)\geq 0,}]
          (   a  2   &#x2212; ( b &#x2212; c  )  2   ) ( ( b + c  )  2
      &#x2212;  a  2    )  &#x2265; 0 ,   {\displaystyle \left(a^{2}-(b-c)^{2})
      ((b+c)^{2}-a^{2}\right)\geq 0,}  [{\displaystyle \left(a^{2}-(b-c)^{2})(
      (b+c)^{2}-a^{2}\right)\geq 0,}]
         ( a + b &#x2212; c ) ( a &#x2212; b + c ) ( b + c + a ) ( b + c
      &#x2212; a ) &#x2265; 0 ,   {\displaystyle (a+b-c)(a-b+c)(b+c+a)(b+c-
      a)\geq 0,}  [{\displaystyle (a+b-c)(a-b+c)(b+c+a)(b+c-a)\geq 0,}]
         ( a + b &#x2212; c ) ( a + c &#x2212; b ) ( b + c &#x2212; a )
      &#x2265; 0 ,   {\displaystyle (a+b-c)(a+c-b)(b+c-a)\geq 0,}  [
      {\displaystyle (a+b-c)(a+c-b)(b+c-a)\geq 0,}]
which holds if the triangle inequality is satisfied for all sides. Therefore
there does exist a real number h consistent with the sides a, b, c, and the
triangle exists. If each triangle inequality holds strictly, h > 0 and the
triangle is non-degenerate (has positive area); but if one of the inequalities
holds with equality, so h = 0, the triangle is degenerate.
**** Generalization to higher dimensions[edit] ****
In Euclidean space, the hypervolume of an (n â 1)-facet of an n-simplex is
less than or equal to the sum of the hypervolumes of the other n facets. In
particular, the area of a triangular face of a tetrahedron is less than or
equal to the sum of the areas of the other three sides.
***** Normed vector space[edit] *****
Triangle inequality for norms of vectors.
In a normed_vector_space V, one of the defining properties of the norm is the
triangle inequality:
          &#x2016; x + y &#x2016; &#x2264; &#x2016; x &#x2016; + &#x2016; y
      &#x2016;  &#x2200;  x , y &#x2208; V    {\displaystyle \displaystyle
      \|x+y\|\leq \|x\|+\|y\|\quad \forall \,x,y\in V}  [\displaystyle
      \|x+y\|\leq \|x\|+\|y\|\quad \forall \,x,y\in V]
that is, the norm of the sum_of_two_vectors is at most as large as the sum of
the norms of the two vectors. This is also referred to as subadditivity. For
any proposed function to behave as a norm, it must satisfy this requirement.
[15]
If the normed space is euclidean, or, more generally, strictly_convex, then
&#x2016; x + y &#x2016; = &#x2016; x &#x2016; + &#x2016; y &#x2016;
{\displaystyle \|x+y\|=\|x\|+\|y\|}  [\|x+y\|=\|x\|+\|y\|] if and only if the
triangle formed by x, y, and x + y, is degenerate, that is, x and y are on the
same ray, i.e., x = 0 or y = 0, or x = Î± y for some Î± > 0. This property
characterizes strictly convex normed spaces such as the âp spaces with 1 < p
< â. However, there are normed spaces in which this is not true. For
instance, consider the plane with the â1 norm (the Manhattan_distance) and
denote x = (1, 0) and y = (0, 1). Then the triangle formed by x, y, and x + y,
is non-degenerate but
         &#x2016; x + y &#x2016; = &#x2016; ( 1 , 1 ) &#x2016; =  |  1  |  +  |
      1  |  = 2 = &#x2016; x &#x2016; + &#x2016; y &#x2016; .   {\displaystyle
      \|x+y\|=\|(1,1)\|=|1|+|1|=2=\|x\|+\|y\|.}  [\|x+y\|=\|
      (1,1)\|=|1|+|1|=2=\|x\|+\|y\|.]
**** Example norms[edit] ****
    * Absolute value as norm for the real_line. To be a norm, the triangle
      inequality requires that the absolute_value satisfy for any real numbers
      x and y:
                |  x + y  |  &#x2264;  |  x  |  +  |  y  |  ,   {\displaystyle
            |x+y|\leq |x|+|y|,}  [|x+y|\leq |x|+|y|,]
      which it does.
Proof:[16]
         &#x2212;  | x |  &#x2264; x &#x2264;  | x |    {\displaystyle -
      \left\vert x\right\vert \leq x\leq \left\vert x\right\vert }  [
      {\displaystyle -\left\vert x\right\vert \leq x\leq \left\vert
      x\right\vert }]
         &#x2212;  | y |  &#x2264; y &#x2264;  | y |    {\displaystyle -
      \left\vert y\right\vert \leq y\leq \left\vert y\right\vert }  [
      {\displaystyle -\left\vert y\right\vert \leq y\leq \left\vert
      y\right\vert }]
After adding,
         &#x2212; (  | x |  +  | y |  ) &#x2264; x + y &#x2264;  | x |  +  | y
      |    {\displaystyle -(\left\vert x\right\vert +\left\vert y\right\vert
      )\leq x+y\leq \left\vert x\right\vert +\left\vert y\right\vert }  [
      {\displaystyle -(\left\vert x\right\vert +\left\vert y\right\vert )\leq
      x+y\leq \left\vert x\right\vert +\left\vert y\right\vert }]
Use the fact that      | b |  &#x2264; a &#x21D4; &#x2212; a &#x2264; b
&#x2264; a   {\displaystyle \left\vert b\right\vert \leq a\Leftrightarrow -
a\leq b\leq a}  [{\displaystyle \left\vert b\right\vert \leq a\Leftrightarrow -
a\leq b\leq a}] (with b replaced by x+y and a by      | x |  +  | y |
{\displaystyle \left\vert x\right\vert +\left\vert y\right\vert }  [
{\displaystyle \left\vert x\right\vert +\left\vert y\right\vert }]), we have
          |  x + y  |  &#x2264;  |  x  |  +  |  y  |    {\displaystyle
      |x+y|\leq |x|+|y|}  [{\displaystyle |x+y|\leq |x|+|y|}]
The triangle inequality is useful in mathematical_analysis for determining the
best upper estimate on the size of the sum of two numbers, in terms of the
sizes of the individual numbers.
There is also a lower estimate, which can be found using the reverse triangle
inequality which states that for any real numbers x and y:
          |  x &#x2212; y  |  &#x2265;   |    |  x  |  &#x2212;  |  y  |    |
      .   {\displaystyle |x-y|\geq {\bigg |}|x|-|y|{\bigg |}.}  [|x-y|\geq
      {\bigg |}|x|-|y|{\bigg |}.]
    * Inner product as norm in an inner_product_space. If the norm arises from
      an inner product (as is the case for Euclidean spaces), then the triangle
      inequality follows from the CauchyâSchwarz_inequality as follows: Given
      vectors     x   {\displaystyle x}  [x] and     y   {\displaystyle y}
      [y], and denoting the inner product as     &#x27E8; x , y &#x27E9;
      {\displaystyle \langle x,y\rangle }  [{\displaystyle \langle x,y\rangle
      }]:[17]
         &#x2016; x
      + y  &#x2016;
      2                 = &#x27E8; x + y , x + y &#x27E9;   {\displaystyle =\langle
      {\displaystyle x+y,x+y\rangle }  [=\langle x+y,x+y\rangle ]
      \|x+y\|^{2}}
      [\|x+y\|^{2}]
                        = &#x2016; x  &#x2016;  2   + &#x27E8; x , y &#x27E9; +
                     &#x27E8; y , x &#x27E9; + &#x2016; y  &#x2016;  2
                     {\displaystyle =\|x\|^{2}+\langle x,y\rangle +\langle y,x\rangle
                     +\|y\|^{2}}  [=\|x\|^{2}+\langle x,y\rangle +\langle y,x\rangle
                     +\|y\|^{2}]
                        &#x2264; &#x2016; x  &#x2016;  2   + 2  |  &#x27E8; x , y
                     &#x27E9;  |  + &#x2016; y  &#x2016;  2     {\displaystyle \leq
                     \|x\|^{2}+2|\langle x,y\rangle |+\|y\|^{2}}  [\leq \|x\|^
                     {2}+2|\langle x,y\rangle |+\|y\|^{2}]
                        &#x2264; &#x2016; x  &#x2016;  2   + 2 &#x2016; x &#x2016;
                     &#x2016; y &#x2016; + &#x2016; y  &#x2016;  2     {\displaystyle
                     \leq \|x\|^{2}+2\|x\|\|y\|+\|y\|^{2}}  [\leq \|x\|^
                     {2}+2\|x\|\|y\|+\|y\|^{2}] (by the CauchyâSchwarz inequality)
                        =   (  &#x2016; x &#x2016; + &#x2016; y &#x2016;  )   2
                     {\displaystyle =\left(\|x\|+\|y\|\right)^{2}}  [=\left
                     (\|x\|+\|y\|\right)^{2}]
      where the last form is a consequence of:
               &#x2016; x  &#x2016;  2   + 2 &#x2016; x &#x2016; &#x2016; y
            &#x2016; + &#x2016; y  &#x2016;  2   =   (  &#x2016; x &#x2016; +
            &#x2016; y &#x2016;  )   2   &#xA0; .   {\displaystyle \|x\|^
            {2}+2\|x\|\|y\|+\|y\|^{2}=\left(\|x\|+\|y\|\right)^{2}\ .}  [\|x\|^
            {2}+2\|x\|\|y\|+\|y\|^{2}=\left(\|x\|+\|y\|\right)^{2}\ .]
The CauchyâSchwarz inequality turns into an equality if and only if x and y
are linearly dependent. The inequality     &#x27E8; x , y &#x27E9; + &#x27E8; y
, x &#x27E9; &#x2264; 2  |  &#x27E8; x , y &#x27E9;  |    {\displaystyle
\langle x,y\rangle +\langle y,x\rangle \leq 2|\langle x,y\rangle |}  [\langle
x,y\rangle +\langle y,x\rangle \leq 2|\langle x,y\rangle |] turns into an
equality for linearly dependent     x   {\displaystyle x}  [x] and     y
{\displaystyle y}  [y] if and only if one of the vectors x or y is a
nonnegative scalar of the other.
      Taking the square root of the final result gives the triangle inequality.
    * p-norm: a commonly used norm is the p-norm:
               &#x2016; x  &#x2016;  p   =   (   &#x2211;  i = 1   n    |   x
            i     |   p    )   1  /  p   &#xA0; ,   {\displaystyle \|x\|_
            {p}=\left(\sum _{i=1}^{n}|x_{i}|^{p}\right)^{1/p}\ ,}  [\|x\|_
            {p}=\left(\sum _{i=1}^{n}|x_{i}|^{p}\right)^{1/p}\ ,]
      where the xi are the components of vector x. For p = 2 the p-norm becomes
      the Euclidean norm:
               &#x2016; x  &#x2016;  2   =   (   &#x2211;  i = 1   n    |   x
            i     |   2    )   1  /  2   =   (   &#x2211;  i = 1   n    x  i
            2    )   1  /  2   &#xA0; ,   {\displaystyle \|x\|_{2}=\left(\sum _
            {i=1}^{n}|x_{i}|^{2}\right)^{1/2}=\left(\sum _{i=1}^{n}x_{i}^
            {2}\right)^{1/2}\ ,}  [\|x\|_{2}=\left(\sum _{i=1}^{n}|x_{i}|^
            {2}\right)^{1/2}=\left(\sum _{i=1}^{n}x_{i}^{2}\right)^{1/2}\ ,]
      which is Pythagoras'_theorem in n-dimensions, a very special case
      corresponding to an inner product norm. Except for the case p = 2, the p-
      norm is not an inner product norm, because it does not satisfy the
      parallelogram_law. The triangle inequality for general values of p is
      called Minkowski's_inequality.[18] It takes the form:
               &#x2016; x + y  &#x2016;  p   &#x2264; &#x2016; x  &#x2016;  p
            + &#x2016; y  &#x2016;  p   &#xA0; .   {\displaystyle \|x+y\|_
            {p}\leq \|x\|_{p}+\|y\|_{p}\ .}  [\|x+y\|_{p}\leq \|x\|_{p}+\|y\|_
            {p}\ .]
***** Metric space[edit] *****
In a metric_space M with metric d, the triangle inequality is a requirement
upon distance:
         d ( x , &#xA0; z ) &#x2264; d ( x , &#xA0; y ) + d ( y , &#xA0; z )
      &#xA0; ,   {\displaystyle d(x,\ z)\leq d(x,\ y)+d(y,\ z)\ ,}  [d(x,\
      z)\leq d(x,\ y)+d(y,\ z)\ ,]
for all x, y, z in M. That is, the distance from x to z is at most as large as
the sum of the distance from x to y and the distance from y to z.
The triangle inequality is responsible for most of the interesting structure on
a metric space, namely, convergence. This is because the remaining requirements
for a metric are rather simplistic in comparison. For example, the fact that
any convergent_sequence in a metric space is a Cauchy_sequence is a direct
consequence of the triangle inequality, because if we choose any xn and xm such
that d(xn, x) < Îµ/2 and d(xm, x) < Îµ/2, where Îµ > 0 is given and arbitrary
(as in the definition of a limit in a metric space), then by the triangle
inequality, d(xn, xm) â¤ d(xn, x) + d(xm, x) < Îµ/2 + Îµ/2 = Îµ, so that the
sequence {xn} is a Cauchy sequence, by definition.
This version of the triangle inequality reduces to the one stated above in case
of normed vector spaces where a metric is induced via d(x, y) â âx â
yâ, with x â y being the vector pointing from point y to x.
***** Reverse triangle inequality[edit] *****
The reverse triangle inequality is an elementary consequence of the triangle
inequality that gives lower bounds instead of upper bounds. For plane geometry,
the statement is:[19]
      Any side of a triangle is greater than the difference between the other
      two sides.
In the case of a normed vector space, the statement is:
           |   &#x2016; x &#x2016; &#x2212; &#x2016; y &#x2016;   |   &#x2264;
      &#x2016; x &#x2212; y &#x2016; ,   {\displaystyle {\bigg |}\|x\|-\|y\|
      {\bigg |}\leq \|x-y\|,}  [{\bigg |}\|x\|-\|y\|{\bigg |}\leq \|x-y\|,]
or for metric spaces, |d(y, x) â d(x, z)| â¤ d(y, z). This implies that the
norm     &#x2016; &#x22C5; &#x2016;   {\displaystyle \|\cdot \|}  [\|\cdot \|]
as well as the distance function     d ( x , &#x22C5; )   {\displaystyle d
(x,\cdot )}  [{\displaystyle d(x,\cdot )}] are Lipschitz_continuous with
Lipschitz constant 1, and therefore are in particular uniformly_continuous.
The proof for the reverse triangle uses the regular triangle inequality, and
&#x2016; y &#x2212; x &#x2016; = &#x2016;  &#x2212;  1 ( x &#x2212; y )
&#x2016; =  |   &#x2212;  1  |  &#x22C5; &#x2016; x &#x2212; y &#x2016; =
&#x2016; x &#x2212; y &#x2016;   {\displaystyle \|y-x\|=\|{-}1(x-y)\|=|{-
}1|\cdot \|x-y\|=\|x-y\|}  [{\displaystyle \|y-x\|=\|{-}1(x-y)\|=|{-}1|\cdot
\|x-y\|=\|x-y\|}]:
         &#x2016; x &#x2016; = &#x2016; ( x &#x2212; y ) + y &#x2016; &#x2264;
      &#x2016; x &#x2212; y &#x2016; + &#x2016; y &#x2016; &#x21D2; &#x2016; x
      &#x2016; &#x2212; &#x2016; y &#x2016; &#x2264; &#x2016; x &#x2212; y
      &#x2016; ,   {\displaystyle \|x\|=\|(x-y)+y\|\leq \|x-
      y\|+\|y\|\Rightarrow \|x\|-\|y\|\leq \|x-y\|,}  [\|x\|=\|(x-y)+y\|\leq
      \|x-y\|+\|y\|\Rightarrow \|x\|-\|y\|\leq \|x-y\|,]
         &#x2016; y &#x2016; = &#x2016; ( y &#x2212; x ) + x &#x2016; &#x2264;
      &#x2016; y &#x2212; x &#x2016; + &#x2016; x &#x2016; &#x21D2; &#x2016; x
      &#x2016; &#x2212; &#x2016; y &#x2016; &#x2265; &#x2212; &#x2016; x
      &#x2212; y &#x2016; ,   {\displaystyle \|y\|=\|(y-x)+x\|\leq \|y-
      x\|+\|x\|\Rightarrow \|x\|-\|y\|\geq -\|x-y\|,}  [\|y\|=\|(y-x)+x\|\leq
      \|y-x\|+\|x\|\Rightarrow \|x\|-\|y\|\geq -\|x-y\|,]
Combining these two statements gives:
         &#x2212; &#x2016; x &#x2212; y &#x2016; &#x2264; &#x2016; x &#x2016;
      &#x2212; &#x2016; y &#x2016; &#x2264; &#x2016; x &#x2212; y &#x2016;
      &#x21D2;   |   &#x2016; x &#x2016; &#x2212; &#x2016; y &#x2016;   |
      &#x2264; &#x2016; x &#x2212; y &#x2016; .   {\displaystyle -\|x-y\|\leq
      \|x\|-\|y\|\leq \|x-y\|\Rightarrow {\bigg |}\|x\|-\|y\|{\bigg |}\leq \|x-
      y\|.}  [-\|x-y\|\leq \|x\|-\|y\|\leq \|x-y\|\Rightarrow {\bigg |}\|x\|-
      \|y\|{\bigg |}\leq \|x-y\|.]
***** Reversal in Minkowski space[edit] *****
The Minkowski_space metric      &#x03B7;  &#x03BC; &#x03BD;     {\displaystyle
\eta _{\mu \nu }}  [\eta _{\mu \nu }] is not positive-definite, which means
that     &#x2016; x  &#x2016;  2   =  &#x03B7;  &#x03BC; &#x03BD;    x
&#x03BC;    x  &#x03BD;     {\displaystyle \|x\|^{2}=\eta _{\mu \nu }x^{\mu }x^
{\nu }}  [{\displaystyle \|x\|^{2}=\eta _{\mu \nu }x^{\mu }x^{\nu }}] can have
either sign or vanish, even if the vector x is non-zero. Moreover, if x and y
are both timelike vectors lying in the future light cone, the triangle
inequality is reversed:
         &#x2016; x + y &#x2016; &#x2265; &#x2016; x &#x2016; + &#x2016; y
      &#x2016; .   {\displaystyle \|x+y\|\geq \|x\|+\|y\|.}  [{\displaystyle
      \|x+y\|\geq \|x\|+\|y\|.}]
A physical example of this inequality is the twin_paradox in special
relativity. The same reversed form of the inequality holds if both vectors lie
in the past light cone, and if one or both are null vectors. The result holds
in n + 1 dimensions for any n â¥ 1. If the plane defined by x and y is
spacelike (and therefore a Euclidean subspace) then the usual triangle
inequality holds.
***** See also[edit] *****
    * Subadditivity
    * Minkowski_inequality
    * Ptolemy's_inequality
***** Notes[edit] *****
   1. ^ Wolfram MathWorld â http://mathworld.wolfram.com/
      TriangleInequality.html
   2. ^ Mohamed A. Khamsi; William A. Kirk (2001). "Â§1.4 The triangle
      inequality in ân". An_introduction_to_metric_spaces_and_fixed_point
      theory. Wiley-IEEE. ISBN 0-471-41825-0.
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
   4. ^ for instance,Jacobs, Harold R. (1974), Geometry, W. H. Freeman & Co.,
      p. 246, ISBN 0-7167-0456-0
   5. ^ Oliver Brock; Jeff Trinkle; Fabio Ramos (2009). Robotics:_Science_and
      Systems_IV. MIT Press. p. 195. ISBN 0-262-51309-9.
   6. ^ Arlan Ramsay; Robert D. Richtmyer (1995). Introduction_to_hyperbolic
      geometry. Springer. p. 17. ISBN 0-387-94339-0.
   7. ^ Harold R. Jacobs (2003). Geometry:_seeing,_doing,_understanding (3rd
      ed.). Macmillan. p. 201. ISBN 0-7167-4361-2.
   8. ^ David E. Joyce (1997). "Euclid's_elements,_Book_1,_Proposition_20".
      Euclid's elements. Dept. Math and Computer Science, Clark University.
      Retrieved 2010-06-25.
   9. ^ American_Mathematical_Monthly, pp. 49-50, 1954.
  10. ^ Claude Irwin Palmer (1919). Practical_mathematics_for_home_study:_being
      the_essentials_of_arithmetic,_geometry,_algebra_and_trigonometry. McGraw-
      Hill. p. 422.
  11. ^ Alexander Zawaira; Gavin Hitchcock (2009). "Lemma 1: In a right-angled
      triangle the hypotenuse is greater than either of the other two sides". A
      primer_for_mathematics_competitions. Oxford University Press. ISBN 0-19-
      953988-X.
  12. ^Wolfram|Alpha. "input:_solve_0<a<2a+3d,_0<a+d<2a+2d,_0<a+2d<2a+d,".
      Wolfram Research. Retrieved 2010-09-07.
  13. ^Wolfram|Alpha. "input:_solve_0<a<ar+ar2,_0<ar<a+ar2,_0<ar2<a+ar".
      Wolfram Research. Retrieved 2010-09-07.
  14. ^Wolfram|Alpha. "input:_solve_0<a<ar+ar2+ar3,_0<ar3<a+ar+ar2". Wolfram
      Research. Retrieved 2012-07-29.
  15. ^John_Stillwell (1997). Numbers_and_Geometry. Springer. ISBN 978-0-387-
      98289-2.
  16.  p. 95.
  17. ^ Rainer Kress (1988). "Â§3.1: Normed spaces". Numerical_analysis.
      Springer. p. 26. ISBN 0-387-98408-9.
  18. ^ James Stewart (2008). Essential Calculus. Thomson Brooks/Cole. p. A10.
      ISBN 978-0-495-10860-3.
  19. ^ John Stillwell (2005). The_four_pillars_of_geometry. Springer. p. 80.
      ISBN 0-387-25530-3.
  20. ^ Karen_Saxe (2002). Beginning_functional_analysis. Springer. p. 61.
      ISBN 0-387-95224-1.
  21. ^ Anonymous (1854). "Exercise I. to proposition XIX". The_popular
      educator;_fourth_volume. Ludgate Hill, London: John Cassell. p. 196.
***** References[edit] *****
    * Pedoe,_Daniel (1988). Geometry: A comprehensive course. Dover. ISBN 0-
      486-65812-0.
.
Rudin,_Walter (1976). Principles of Mathematical Analysis. New York: McGraw-
Hill. ISBN 0-07-054235-X.
.
***** External links[edit] *****
    * Triangle_inequality at ProofWiki

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Triangle_inequality&oldid=902847676"
Categories:
    * Geometric_inequalities
    * Linear_algebra
    * Metric_geometry
    * Theorems_in_geometry
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
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
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ú©ÙØ±Ø¯Û
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 21 June 2019, at 17:50 (UTC).
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
