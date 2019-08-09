The following text has been accessed from https://en.wikipedia.org/wiki/Contour_integration at Fri Aug 9 02:37:17 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Contour integration ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the line integral in the complex plane. For the general
line integral, see Line_integral.
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
    * Contour integration
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
    * Multiple_integral
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
In the mathematical field of complex_analysis, contour integration is a method
of evaluating certain integrals along paths in the complex plane.[1][2][3]
Contour integration is closely related to the calculus of residues,[4] a method
of complex_analysis.
One use for contour integrals is the evaluation of integrals along the real
line that are not readily found by using only real variable methods.[5]
Contour integration methods include
    * direct integration of a complex-valued function along a curve in the
      complex plane (a contour)
    * application of the Cauchy_integral_formula
    * application of the residue_theorem
One method can be used, or a combination of these methods, or various limiting
processes, for the purpose of finding these integrals or sums.
⁰
***** Contents *****
    * 1_Curves_in_the_complex_plane
          o 1.1_Directed_smooth_curves
          o 1.2_Contours
    * 2_Contour_integrals
          o 2.1_For_continuous_functions
          o 2.2_As_a_generalization_of_the_Riemann_integral
    * 3_Direct_methods
          o 3.1_Example
    * 4_Applications_of_integral_theorems
          o 4.1_Example_1
                # 4.1.1_Using_the_Cauchy_integral_formula
                # 4.1.2_Using_the_method_of_residues
                # 4.1.3_Contour_note
          o 4.2_Example_2_â_Cauchy_distribution
          o 4.3_Example_3_â_trigonometric_integrals
          o 4.4_Example_3a_â_trigonometric_integrals,_the_general_procedure
          o 4.5_Example_4_â_branch_cuts
          o 4.6_Example_5_â_the_square_of_the_logarithm
          o 4.7_Example_6_â_logarithms_and_the_residue_at_infinity
    * 5_Evaluation_with_residue_theorem
    * 6_Multivariable_Contour_Integrals
          o 6.1_Example_1
          o 6.2_Example_2
    * 7_Integral_representation
    * 8_See_also
    * 9_References
    * 10_Further_reading
    * 11_External_links
***** Curves in the complex plane[edit] *****
In complex_analysis a contour is a type of curve in the complex_plane. In
contour integration, contours provide a precise definition of the curves on
which an integral may be suitably defined. A curve in the complex plane is
defined as a continuous_function from a closed_interval of the real_line to the
complex plane: z : [a, b] â C.
This definition of a curve coincides with the intuitive notion of a curve, but
includes a parametrization by a continuous function from a closed interval.
This more precise definition allows us to consider what properties a curve must
have for it to be useful for integration. In the following subsections we
narrow down the set of curves that we can integrate to include only those that
can be built up out of a finite number of continuous curves that can be given a
direction. Moreover, we will restrict the "pieces" from crossing over
themselves, and we require that each piece have a finite (non-vanishing)
continuous derivative. These requirements correspond to requiring that we
consider only curves that can be traced, such as by a pen, in a sequence of
even, steady strokes, which only stop to start a new piece of the curve, all
without picking up the pen.[6]
**** Directed smooth curves[edit] ****
Contours are often defined in terms of directed smooth curves.[6] These provide
a precise definition of a "piece" of a smooth curve, of which a contour is
made.
A smooth curve is a curve z : [a, b] â C with a non-vanishing, continuous
derivative such that each point is traversed only once (z is one-to-one), with
the possible exception of a curve such that the endpoints match (z(a) = z(b)).
In the case where the endpoints match the curve is called closed, and the
function is required to be one-to-one everywhere else and the derivative must
be continuous at the identified point (zâ²(a) = zâ²(b)). A smooth curve that
is not closed is often referred to as a smooth arc.[6]
The parametrization of a curve provides a natural ordering of points on the
curve: z(x) comes before z(y) if x < y. This leads to the notion of a directed
smooth curve. It is most useful to consider curves independent of the specific
parametrization. This can be done by considering equivalence_classes of smooth
curves with the same direction. A directed smooth curve can then be defined as
an ordered set of points in the complex plane that is the image of some smooth
curve in their natural order (according to the parametrization). Note that not
all orderings of the points are the natural ordering of a smooth curve. In
fact, a given smooth curve has only two such orderings. Also, a single closed
curve can have any point as its endpoint, while a smooth arc has only two
choices for its endpoints.
**** Contours[edit] ****
Contours are the class of curves on which we define contour integration. A
contour is a directed curve which is made up of a finite sequence of directed
smooth curves whose endpoints are matched to give a single direction. This
requires that the sequence of curves Î³1,â¦,Î³n be such that the terminal
point of Î³i coincides with the initial point of Î³i+1, â i, 1 â¤ i < n.
This includes all directed smooth curves. Also, a single point in the complex
plane is considered a contour. The symbol + is often used to denote the piecing
of curves together to form a new curve. Thus we could write a contour Î that
is made up of n curves as
         &#x0393; =  &#x03B3;  1   +  &#x03B3;  2   + &#x22EF; +  &#x03B3;  n
      .   {\displaystyle \Gamma =\gamma _{1}+\gamma _{2}+\cdots +\gamma _{n}.}
      [\Gamma =\gamma _{1}+\gamma _{2}+\cdots +\gamma _{n}.]
***** Contour integrals[edit] *****
The contour integral of a complex_function f : C â C is a generalization of
the integral for real-valued functions. For continuous_functions in the complex
plane, the contour integral can be defined in analogy to the line_integral by
first defining the integral along a directed smooth curve in terms of an
integral over a real valued parameter. A more general definition can be given
in terms of partitions of the contour in analogy with the partition_of_an
interval and the Riemann_integral. In both cases the integral over a contour is
defined as the sum of the integrals over the directed smooth curves that make
up the contour.
**** For continuous functions[edit] ****
To define the contour integral in this way one must first consider the
integral, over a real variable, of a complex-valued function. Let f : R â C
be a complex-valued function of a real variable, t. The real and imaginary
parts of f are often denoted as u(t) and v(t), respectively, so that
         f ( t ) = u ( t ) + i v ( t ) .   {\displaystyle f(t)=u(t)+iv(t).}  [f
      (t)=u(t)+iv(t).]
Then the integral of the complex-valued function f over the interval [a, b] is
given by
              &#x222B;  a   b   f ( t )  d t    =  &#x222B;  a   b     (   u
      ( t ) + i v ( t )   )    d t       =  &#x222B;  a   b   u ( t )  d t + i
      &#x222B;  a   b   v ( t )  d t .       {\displaystyle {\begin
      {aligned}\int _{a}^{b}f(t)\,dt&=\int _{a}^{b}{\big (}u(t)+iv(t){\big
      )}\,dt\\&=\int _{a}^{b}u(t)\,dt+i\int _{a}^{b}v(t)\,dt.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\int _{a}^{b}f(t)\,dt&=\int _{a}^{b}{\big
      (}u(t)+iv(t){\big )}\,dt\\&=\int _{a}^{b}u(t)\,dt+i\int _{a}^{b}v
      (t)\,dt.\end{aligned}}}]
Let f : C â C be a continuous_function on the directed_smooth_curve Î³. Let
z : R â C be any parametrization of Î³ that is consistent with its order
(direction). Then the integral along Î³ is denoted
          &#x222B;  &#x03B3;   f ( z )  d z    {\displaystyle \int _{\gamma }f
      (z)\,dz\,}  [\int _{\gamma }f(z)\,dz\,]
and is given by[6]
          &#x222B;  &#x03B3;   f ( z )  d z =  &#x222B;  a   b   f
      (   &#x03B3; ( t )   )    &#x03B3; &#x2032;  ( t )  d t .
      {\displaystyle \int _{\gamma }f(z)\,dz=\int _{a}^{b}f{\big (}\gamma (t)
      {\big )}\gamma '(t)\,dt.}  [{\displaystyle \int _{\gamma }f(z)\,dz=\int _
      {a}^{b}f{\big (}\gamma (t){\big )}\gamma '(t)\,dt.}]
This definition is well defined. That is, the result is independent of the
parametrization chosen.[6] In the case where the real integral on the right
side does not exist the integral along Î³ is said not to exist.
**** As a generalization of the Riemann integral[edit] ****
The generalization of the Riemann_integral to functions of a complex variable
is done in complete analogy to its definition for functions from the real
numbers. The partition of a directed smooth curve Î³ is defined as a finite,
ordered set of points on Î³. The integral over the curve is the limit of finite
sums of function values, taken at the points on the partition, in the limit
that the maximum distance between any two successive points on the partition
(in the two-dimensional complex plane), also known as the mesh, goes to zero.
***** Direct methods[edit] *****
Direct methods involve the calculation of the integral by means of methods
similar to those in calculating line integrals in several-variable calculus.
This means that we use the following method:
    * parametrizing the contour
            The contour is parametrized by a differentiable complex-valued
            function of real variables, or the contour is broken up into pieces
            and parametrized separately.
    * substitution of the parametrization into the integrand
            Substituting the parametrization into the integrand transforms the
            integral into an integral of one real variable.
    * direct evaluation
            The integral is evaluated in a method akin to a real-variable
            integral.
**** Example[edit] ****
A fundamental result in complex analysis is that the contour integral of 1/z is
2Ïi, where the path of the contour is taken to be the unit circle traversed
counterclockwise (or any positively oriented Jordan_curve about 0). In the case
of the unit circle there is a direct method to evaluate the integral
             &#x222E;       C   &#x2061;   1 z    d z .   {\displaystyle \oint
      _{C}{\frac {1}{z}}\,dz.}  [{\displaystyle \oint _{C}{\frac {1}{z}}\,dz.}]
In evaluating this integral, use the unit circle |z| = 1 as a contour,
parametrized by z(t) = eit, with t â [0, 2Ï], then dz/dt = ieit and
             &#x222E;       C   &#x2061;   1 z    d z =  &#x222B;  0   2
      &#x03C0;     1  e  i t     i  e  i t    d t = i  &#x222B;  0   2 &#x03C0;
      1  d t =   [    t     ]    0   2 &#x03C0;   i = ( 2 &#x03C0; &#x2212; 0 )
      i = 2 &#x03C0; i .   {\displaystyle \oint _{C}{\frac {1}{z}}\,dz=\int _
      {0}^{2\pi }{\frac {1}{e^{it}}}ie^{it}\,dt=i\int _{0}^{2\pi }1\,dt={\Big
      [}\;t\;{\Big ]}_{0}^{2\pi }i=(2\pi -0)i=2\pi i.}  [{\displaystyle \oint _
      {C}{\frac {1}{z}}\,dz=\int _{0}^{2\pi }{\frac {1}{e^{it}}}ie^
      {it}\,dt=i\int _{0}^{2\pi }1\,dt={\Big [}\;t\;{\Big ]}_{0}^{2\pi }i=(2\pi
      -0)i=2\pi i.}]
which is the value of the integral.
***** Applications of integral theorems[edit] *****
Applications of integral theorems are also often used to evaluate the contour
integral along a contour, which means that the real-valued integral is
calculated simultaneously along with calculating the contour integral.
Integral theorems such as the Cauchy_integral_formula or residue_theorem are
generally used in the following method:
    * a specific contour is chosen:
            The contour is chosen so that the contour follows the part of the
            complex plane that describes the real-valued integral, and also
            encloses singularities of the integrand so application of the
            Cauchy_integral_formula or residue_theorem is possible
    * application of Cauchy's_integral_theorem
            The integral is reduced to only an integration around a small
            circle about each pole.
    * application of the Cauchy_integral_formula or residue_theorem
            Application of these integral formulae gives us a value for the
            integral around the whole of the contour.
    * division of the contour into a contour along the real part and imaginary
      part
            The whole of the contour can be divided into the contour that
            follows the part of the complex plane that describes the real-
            valued integral as chosen before (call it R), and the integral that
            crosses the complex plane (call it I). The integral over the whole
            of the contour is the sum of the integral over each of these
            contours.
    * demonstration that the integral that crosses the complex plane plays no
      part in the sum
            If the integral I can be shown to be zero, or if the real-valued
            integral that is sought is improper, then if we demonstrate that
            the integral I as described above tends to 0, the integral along R
            will tend to the integral around the contour R + I.
    * conclusion
            If we can show the above step, then we can directly calculate R,
            the real-valued integral.
**** Example 1[edit] ****
Consider the integral
          &#x222B;  &#x2212; &#x221E;   &#x221E;     1   (   x  2   + 1  )   2
      d x ,   {\displaystyle \int _{-\infty }^{\infty }{\frac {1}{\left(x^
      {2}+1\right)^{2}}}\,dx,}  [{\displaystyle \int _{-\infty }^{\infty }
      {\frac {1}{\left(x^{2}+1\right)^{2}}}\,dx,}]
To evaluate this integral, we look at the complex-valued function
         f ( z ) =   1   (   z  2   + 1  )   2       {\displaystyle f(z)={\frac
      {1}{\left(z^{2}+1\right)^{2}}}}  [{\displaystyle f(z)={\frac {1}{\left(z^
      {2}+1\right)^{2}}}}]
which has singularities at i and âi. We choose a contour that will enclose
the real-valued integral, here a semicircle with boundary diameter on the real
line (going from, say, âa to a) will be convenient. Call this contour C.
There are two ways of proceeding, using the Cauchy_integral_formula or by the
method of residues:
*** Using the Cauchy integral formula[edit] ***
Note that:
             &#x222E;       C   &#x2061; f ( z )  d z =  &#x222B;  &#x2212; a
      a   f ( z )  d z +  &#x222B;  Arc   f ( z )  d z   {\displaystyle \oint _
      {C}f(z)\,dz=\int _{-a}^{a}f(z)\,dz+\int _{\text{Arc}}f(z)\,dz}  [
      {\displaystyle \oint _{C}f(z)\,dz=\int _{-a}^{a}f(z)\,dz+\int _{\text
      {Arc}}f(z)\,dz}]
thus
          &#x222B;  &#x2212; a   a   f ( z )  d z =     &#x222E;       C
      &#x2061; f ( z )  d z &#x2212;  &#x222B;  Arc   f ( z )  d z
      {\displaystyle \int _{-a}^{a}f(z)\,dz=\oint _{C}f(z)\,dz-\int _{\text
      {Arc}}f(z)\,dz}  [\int _{-a}^{a}f(z)\,dz=\oint _{C}f(z)\,dz-\int _{\text
      {Arc}}f(z)\,dz]
Furthermore, observe that
         f ( z ) =   1   (   z  2   + 1  )   2     =   1  ( z + i  )  2   ( z
      &#x2212; i  )  2      .   {\displaystyle f(z)={\frac {1}{\left(z^
      {2}+1\right)^{2}}}={\frac {1}{(z+i)^{2}(z-i)^{2}}}.}  [{\displaystyle f
      (z)={\frac {1}{\left(z^{2}+1\right)^{2}}}={\frac {1}{(z+i)^{2}(z-i)^
      {2}}}.}]
Since the only singularity in the contour is the one at i, then we can write
         f ( z ) =    1  ( z + i  )  2      ( z &#x2212; i  )  2      ,
      {\displaystyle f(z)={\frac {\frac {1}{(z+i)^{2}}}{(z-i)^{2}}},}  [
      {\displaystyle f(z)={\frac {\frac {1}{(z+i)^{2}}}{(z-i)^{2}}},}]
which puts the function in the form for direct application of the formula.
Then, by using Cauchy's integral formula,
             &#x222E;       C   &#x2061; f ( z )  d z =     &#x222E;       C
      &#x2061;    1  ( z + i  )  2      ( z &#x2212; i  )  2       d z = 2
      &#x03C0; i   d  d z     (   1  ( z + i  )  2      )     |    z = i   = 2
      &#x03C0; i  (    &#x2212; 2   ( z + i  )  3      )     |    z = i   =
      &#x03C0; 2     {\displaystyle \oint _{C}f(z)\,dz=\oint _{C}{\frac {\frac
      {1}{(z+i)^{2}}}{(z-i)^{2}}}\,dz=2\pi i{\frac {d}{dz}}\left({\frac {1}{
      (z+i)^{2}}}\right){\Bigg |}_{z=i}=2\pi i\left({\frac {-2}{(z+i)^
      {3}}}\right){\Bigg |}_{z=i}={\frac {\pi }{2}}}  [{\displaystyle \oint _
      {C}f(z)\,dz=\oint _{C}{\frac {\frac {1}{(z+i)^{2}}}{(z-i)^{2}}}\,dz=2\pi
      i{\frac {d}{dz}}\left({\frac {1}{(z+i)^{2}}}\right){\Bigg |}_{z=i}=2\pi
      i\left({\frac {-2}{(z+i)^{3}}}\right){\Bigg |}_{z=i}={\frac {\pi }{2}}}]
We take the first derivative, in the above steps, because the pole is a second-
order pole. That is, (z â i) is taken to the second power, so we employ the
first derivative of f(z). If it were (z â i) taken to the third power, we
would use the second derivative and divide by 2!, etc. The case of (z â i) to
the first power corresponds to a zero order derivativeâjust f(z) itself.
We need to show that the integral over the arc of the semicircle tends to zero
as a â â, using the estimation_lemma
          |   &#x222B;  Arc   f ( z )  d z  |  &#x2264; M L   {\displaystyle
      \left|\int _{\text{Arc}}f(z)\,dz\right|\leq ML}  [\left|\int _{\text
      {Arc}}f(z)\,dz\right|\leq ML]
where M is an upper bound on |f(z)| along the arc and L the length of the arc.
Now,
          |   &#x222B;  Arc   f ( z )  d z  |  &#x2264;    a &#x03C0;    (   a
      2   &#x2212; 1  )   2     &#x2192; 0   &#xA0;as&#xA0;   a &#x2192;
      &#x221E; .   {\displaystyle \left|\int _{\text{Arc}}f(z)\,dz\right|\leq
      {\frac {a\pi }{\left(a^{2}-1\right)^{2}}}\rightarrow 0{\mbox{ as
      }}a\rightarrow \infty .}  [{\displaystyle \left|\int _{\text{Arc}}f
      (z)\,dz\right|\leq {\frac {a\pi }{\left(a^{2}-1\right)^{2}}}\rightarrow 0
      {\mbox{ as }}a\rightarrow \infty .}]
So
          &#x222B;  &#x2212; &#x221E;   &#x221E;     1   (   x  2   + 1  )   2
      d x =  &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( z )  d z =  lim  a
      &#x2192; + &#x221E;    &#x222B;  &#x2212; a   a   f ( z )  d z =
      &#x03C0; 2   .  &#x25FB;   {\displaystyle \int _{-\infty }^{\infty }
      {\frac {1}{\left(x^{2}+1\right)^{2}}}\,dx=\int _{-\infty }^{\infty }f
      (z)\,dz=\lim _{a\to +\infty }\int _{-a}^{a}f(z)\,dz={\frac {\pi }
      {2}}.\quad \square }  [{\displaystyle \int _{-\infty }^{\infty }{\frac
      {1}{\left(x^{2}+1\right)^{2}}}\,dx=\int _{-\infty }^{\infty }f
      (z)\,dz=\lim _{a\to +\infty }\int _{-a}^{a}f(z)\,dz={\frac {\pi }
      {2}}.\quad \square }]
*** Using the method of residues[edit] ***
Consider the Laurent_series of f(z) about i, the only singularity we need to
consider. We then have
         f ( z ) =    &#x2212; 1   4 ( z &#x2212; i  )  2      +    &#x2212; i
      4 ( z &#x2212; i )    +   3 16   +   i 8   ( z &#x2212; i ) +    &#x2212;
      5  64   ( z &#x2212; i  )  2   + &#x22EF;   {\displaystyle f(z)={\frac {-
      1}{4(z-i)^{2}}}+{\frac {-i}{4(z-i)}}+{\frac {3}{16}}+{\frac {i}{8}}(z-i)+
      {\frac {-5}{64}}(z-i)^{2}+\cdots }  [{\displaystyle f(z)={\frac {-1}{4(z-
      i)^{2}}}+{\frac {-i}{4(z-i)}}+{\frac {3}{16}}+{\frac {i}{8}}(z-i)+{\frac
      {-5}{64}}(z-i)^{2}+\cdots }]
(See the sample Laurent calculation from Laurent_series for the derivation of
this series.)
It is clear by inspection that the residue is âi/4, so, by the residue
theorem, we have
             &#x222E;       C   &#x2061; f ( z )  d z =     &#x222E;       C
      &#x2061;   1   (   z  2   + 1  )   2      d z = 2 &#x03C0; i   Res  z = i
      &#x2061; f = 2 &#x03C0; i  (  &#x2212;   i 4    )  =   &#x03C0; 2
      &#x25FB;   {\displaystyle \oint _{C}f(z)\,dz=\oint _{C}{\frac {1}{\left
      (z^{2}+1\right)^{2}}}\,dz=2\pi i\,\operatorname {Res} _{z=i}f=2\pi i\left
      (-{\frac {i}{4}}\right)={\frac {\pi }{2}}\quad \square }  [{\displaystyle
      \oint _{C}f(z)\,dz=\oint _{C}{\frac {1}{\left(z^{2}+1\right)^
      {2}}}\,dz=2\pi i\,\operatorname {Res} _{z=i}f=2\pi i\left(-{\frac {i}
      {4}}\right)={\frac {\pi }{2}}\quad \square }]
Thus we get the same result as before.
*** Contour note[edit] ***
As an aside, a question can arise whether we do not take the semicircle to
include the other singularity, enclosing âi. To have the integral along the
real axis moving in the correct direction, the contour must travel clockwise,
i.e., in a negative direction, reversing the sign of the integral overall.
This does not affect the use of the method of residues by series.
**** Example 2 â Cauchy distribution[edit] ****
The integral
          &#x222B;  &#x2212; &#x221E;   &#x221E;      e  i t x     x  2   + 1
      d x   {\displaystyle \int _{-\infty }^{\infty }{\frac {e^{itx}}{x^
      {2}+1}}\,dx}  [{\displaystyle \int _{-\infty }^{\infty }{\frac {e^{itx}}
      {x^{2}+1}}\,dx}]
[the_contour]
(which arises in probability_theory as a scalar multiple of the characteristic
function of the Cauchy_distribution) resists the techniques of elementary
calculus. We will evaluate it by expressing it as a limit of contour integrals
along the contour C that goes along the real line from âa to a and then
counterclockwise along a semicircle centered at 0 from a to âa. Take a to be
greater than 1, so that the imaginary unit i is enclosed within the curve. The
contour integral is
          &#x222B;  C      e  i t z     z  2   + 1     d z .   {\displaystyle
      \int _{C}{\frac {e^{itz}}{z^{2}+1}}\,dz.}  [{\displaystyle \int _{C}
      {\frac {e^{itz}}{z^{2}+1}}\,dz.}]
Since eitz is an entire_function (having no singularities at any point in the
complex plane), this function has singularities only where the denominator z2 +
1 is zero. Since z2 + 1 = (z + i)(z â i), that happens only where z = i or z
= âi. Only one of those points is in the region bounded by this contour. The
residue of f(z) at z = i is
          lim  z &#x2192; i   ( z &#x2212; i ) f ( z ) =  lim  z &#x2192; i
      ( z &#x2212; i )    e  i t z     z  2   + 1    =  lim  z &#x2192; i   ( z
      &#x2212; i )    e  i t z    ( z &#x2212; i ) ( z + i )    =  lim  z
      &#x2192; i      e  i t z    z + i    =    e  &#x2212; t    2 i    .
      {\displaystyle \lim _{z\to i}(z-i)f(z)=\lim _{z\to i}(z-i){\frac {e^
      {itz}}{z^{2}+1}}=\lim _{z\to i}(z-i){\frac {e^{itz}}{(z-i)(z+i)}}=\lim _
      {z\to i}{\frac {e^{itz}}{z+i}}={\frac {e^{-t}}{2i}}.}  [{\displaystyle
      \lim _{z\to i}(z-i)f(z)=\lim _{z\to i}(z-i){\frac {e^{itz}}{z^
      {2}+1}}=\lim _{z\to i}(z-i){\frac {e^{itz}}{(z-i)(z+i)}}=\lim _{z\to i}
      {\frac {e^{itz}}{z+i}}={\frac {e^{-t}}{2i}}.}]
According to the residue_theorem, then, we have
          &#x222B;  C   f ( z )  d z = 2 &#x03C0; i  Res  z = i   &#x2061; f
      ( z ) = 2 &#x03C0; i    e  &#x2212; t    2 i    = &#x03C0;  e  &#x2212; t
      .   {\displaystyle \int _{C}f(z)\,dz=2\pi i\operatorname {Res} _{z=i}f
      (z)=2\pi i{\frac {e^{-t}}{2i}}=\pi e^{-t}.}  [{\displaystyle \int _{C}f
      (z)\,dz=2\pi i\operatorname {Res} _{z=i}f(z)=2\pi i{\frac {e^{-t}}
      {2i}}=\pi e^{-t}.}]
The contour C may be split into a "straight" part and a curved arc, so that
          &#x222B;  straight   +  &#x222B;  arc   = &#x03C0;  e  &#x2212; t   ,
      {\displaystyle \int _{\text{straight}}+\int _{\text{arc}}=\pi e^{-t},}  [
      {\displaystyle \int _{\text{straight}}+\int _{\text{arc}}=\pi e^{-t},}]
and thus
          &#x222B;  &#x2212; a   a   = &#x03C0;  e  &#x2212; t   &#x2212;
      &#x222B;  arc   .   {\displaystyle \int _{-a}^{a}=\pi e^{-t}-\int _{\text
      {arc}}.}  [{\displaystyle \int _{-a}^{a}=\pi e^{-t}-\int _{\text{arc}}.}]
It can be shown that if t > 0 then
          &#x222B;  arc      e  i t z     z  2   + 1     d z &#x2192; 0
      &#xA0;as&#xA0;   a &#x2192; &#x221E; .   {\displaystyle \int _{\text
      {arc}}{\frac {e^{itz}}{z^{2}+1}}\,dz\rightarrow 0{\mbox{ as
      }}a\rightarrow \infty .}  [{\displaystyle \int _{\text{arc}}{\frac {e^
      {itz}}{z^{2}+1}}\,dz\rightarrow 0{\mbox{ as }}a\rightarrow \infty .}]
Therefore, if t > 0 then
          &#x222B;  &#x2212; &#x221E;   &#x221E;      e  i t x     x  2   + 1
      d x = &#x03C0;  e  &#x2212; t   .   {\displaystyle \int _{-\infty }^
      {\infty }{\frac {e^{itx}}{x^{2}+1}}\,dx=\pi e^{-t}.}  [{\displaystyle
      \int _{-\infty }^{\infty }{\frac {e^{itx}}{x^{2}+1}}\,dx=\pi e^{-t}.}]
A similar argument with an arc that winds around âi rather than i shows that
if t < 0 then
          &#x222B;  &#x2212; &#x221E;   &#x221E;      e  i t x     x  2   + 1
      d x = &#x03C0;  e  t   ,   {\displaystyle \int _{-\infty }^{\infty }
      {\frac {e^{itx}}{x^{2}+1}}\,dx=\pi e^{t},}  [{\displaystyle \int _{-
      \infty }^{\infty }{\frac {e^{itx}}{x^{2}+1}}\,dx=\pi e^{t},}]
and finally we have this:
          &#x222B;  &#x2212; &#x221E;   &#x221E;      e  i t x     x  2   + 1
      d x = &#x03C0;  e  &#x2212;  |  t  |    .  &#x25FB;   {\displaystyle \int
      _{-\infty }^{\infty }{\frac {e^{itx}}{x^{2}+1}}\,dx=\pi e^{-|t|}.\quad
      \square }  [{\displaystyle \int _{-\infty }^{\infty }{\frac {e^{itx}}{x^
      {2}+1}}\,dx=\pi e^{-|t|}.\quad \square }]
(If t = 0 then the integral yields immediately to real-valued calculus methods
and its value is Ï.)
**** Example 3 â trigonometric integrals[edit] ****
Certain substitutions can be made to integrals involving trigonometric
functions, so the integral is transformed into a rational function of a complex
variable and then the above methods can be used in order to evaluate the
integral.
As an example, consider
          &#x222B;  &#x2212; &#x03C0;   &#x03C0;     1  1 + 3 ( cos &#x2061; t
      )  2       d t .   {\displaystyle \int _{-\pi }^{\pi }{\frac {1}{1+3(\cos
      t)^{2}}}\,dt.}  [{\displaystyle \int _{-\pi }^{\pi }{\frac {1}{1+3(\cos
      t)^{2}}}\,dt.}]
We seek to make a substitution of z = eit. Now, recall
         cos &#x2061; t =   1 2    (   e  i t   +  e  &#x2212; i t    )  =   1
      2    (  z +   1 z    )    {\displaystyle \cos t={\frac {1}{2}}\left(e^
      {it}+e^{-it}\right)={\frac {1}{2}}\left(z+{\frac {1}{z}}\right)}  [
      {\displaystyle \cos t={\frac {1}{2}}\left(e^{it}+e^{-it}\right)={\frac
      {1}{2}}\left(z+{\frac {1}{z}}\right)}]
and
            d z   d t    = i z , &#xA0; d t =    d z   i z    .
      {\displaystyle {\frac {dz}{dt}}=iz,\ dt={\frac {dz}{iz}}.}  [
      {\displaystyle {\frac {dz}{dt}}=iz,\ dt={\frac {dz}{iz}}.}]
Taking C to be the unit circle, we substitute to get:
                 &#x222E;       C   &#x2061;   1  1 + 3   (    1 2    (  z +
      1 z    )   )   2          d z   i z       =     &#x222E;       C
      &#x2061;   1  1 +   3 4     (  z +   1 z    )   2        1  i z     d z
      =     &#x222E;       C   &#x2061;    &#x2212; i   z +   3 4   z   (  z +
      1 z    )   2       d z       = &#x2212; i     &#x222E;       C   &#x2061;
      1  z +   3 4   z  (   z  2   + 2 +   1  z  2      )      d z       =
      &#x2212; i     &#x222E;       C   &#x2061;   1  z +   3 4    (   z  3   +
      2 z +   1 z    )      d z       = &#x2212; i     &#x222E;       C
      &#x2061;   1    3 4    z  3   +   5 2   z +   3  4 z        d z       =
      &#x2212; i     &#x222E;       C   &#x2061;   4  3  z  3   + 10 z +   3 z
      d z       = &#x2212; 4 i     &#x222E;       C   &#x2061;   1  3  z  3   +
      10 z +   3 z       d z       = &#x2212; 4 i     &#x222E;       C
      &#x2061;   z  3  z  4   + 10  z  2   + 3     d z       = &#x2212; 4 i
      &#x222E;       C   &#x2061;   z  3  (  z +   3   i  )   (  z &#x2212;   3
      i  )   (  z +   i  3     )   (  z &#x2212;   i  3     )      d z       =
      &#x2212;    4 i  3       &#x222E;       C   &#x2061;   z   (  z +   3   i
      )   (  z &#x2212;   3   i  )   (  z +   i  3     )   (  z &#x2212;   i  3
      )      d z .       {\displaystyle {\begin{aligned}\oint _{C}{\frac {1}
      {1+3\left({\frac {1}{2}}\left(z+{\frac {1}{z}}\right)\right)^{2}}}\,
      {\frac {dz}{iz}}&=\oint _{C}{\frac {1}{1+{\frac {3}{4}}\left(z+{\frac {1}
      {z}}\right)^{2}}}{\frac {1}{iz}}\,dz\\&=\oint _{C}{\frac {-i}{z+{\frac
      {3}{4}}z\left(z+{\frac {1}{z}}\right)^{2}}}\,dz\\&=-i\oint _{C}{\frac {1}
      {z+{\frac {3}{4}}z\left(z^{2}+2+{\frac {1}{z^{2}}}\right)}}\,dz\\&=-
      i\oint _{C}{\frac {1}{z+{\frac {3}{4}}\left(z^{3}+2z+{\frac {1}
      {z}}\right)}}\,dz\\&=-i\oint _{C}{\frac {1}{{\frac {3}{4}}z^{3}+{\frac
      {5}{2}}z+{\frac {3}{4z}}}}\,dz\\&=-i\oint _{C}{\frac {4}{3z^{3}+10z+
      {\frac {3}{z}}}}\,dz\\&=-4i\oint _{C}{\frac {1}{3z^{3}+10z+{\frac {3}
      {z}}}}\,dz\\&=-4i\oint _{C}{\frac {z}{3z^{4}+10z^{2}+3}}\,dz\\&=-4i\oint
      _{C}{\frac {z}{3\left(z+{\sqrt {3}}i\right)\left(z-{\sqrt
      {3}}i\right)\left(z+{\frac {i}{\sqrt {3}}}\right)\left(z-{\frac {i}{\sqrt
      {3}}}\right)}}\,dz\\&=-{\frac {4i}{3}}\oint _{C}{\frac {z}{\left(z+{\sqrt
      {3}}i\right)\left(z-{\sqrt {3}}i\right)\left(z+{\frac {i}{\sqrt
      {3}}}\right)\left(z-{\frac {i}{\sqrt {3}}}\right)}}\,dz.\end{aligned}}}
      [{\displaystyle {\begin{aligned}\oint _{C}{\frac {1}{1+3\left({\frac {1}
      {2}}\left(z+{\frac {1}{z}}\right)\right)^{2}}}\,{\frac {dz}{iz}}&=\oint _
      {C}{\frac {1}{1+{\frac {3}{4}}\left(z+{\frac {1}{z}}\right)^{2}}}{\frac
      {1}{iz}}\,dz\\&=\oint _{C}{\frac {-i}{z+{\frac {3}{4}}z\left(z+{\frac {1}
      {z}}\right)^{2}}}\,dz\\&=-i\oint _{C}{\frac {1}{z+{\frac {3}{4}}z\left(z^
      {2}+2+{\frac {1}{z^{2}}}\right)}}\,dz\\&=-i\oint _{C}{\frac {1}{z+{\frac
      {3}{4}}\left(z^{3}+2z+{\frac {1}{z}}\right)}}\,dz\\&=-i\oint _{C}{\frac
      {1}{{\frac {3}{4}}z^{3}+{\frac {5}{2}}z+{\frac {3}{4z}}}}\,dz\\&=-i\oint
      _{C}{\frac {4}{3z^{3}+10z+{\frac {3}{z}}}}\,dz\\&=-4i\oint _{C}{\frac {1}
      {3z^{3}+10z+{\frac {3}{z}}}}\,dz\\&=-4i\oint _{C}{\frac {z}{3z^{4}+10z^
      {2}+3}}\,dz\\&=-4i\oint _{C}{\frac {z}{3\left(z+{\sqrt {3}}i\right)\left
      (z-{\sqrt {3}}i\right)\left(z+{\frac {i}{\sqrt {3}}}\right)\left(z-{\frac
      {i}{\sqrt {3}}}\right)}}\,dz\\&=-{\frac {4i}{3}}\oint _{C}{\frac {z}
      {\left(z+{\sqrt {3}}i\right)\left(z-{\sqrt {3}}i\right)\left(z+{\frac {i}
      {\sqrt {3}}}\right)\left(z-{\frac {i}{\sqrt {3}}}\right)}}\,dz.\end
      {aligned}}}]
The singularities to be considered are at         &#x00B1; i   3     .
{\displaystyle {\tfrac {\pm i}{\sqrt {3}}}.}  [{\displaystyle {\tfrac {\pm i}
{\sqrt {3}}}.}] Let C1 be a small circle about        i  3     ,
{\displaystyle {\tfrac {i}{\sqrt {3}}},}  [{\displaystyle {\tfrac {i}{\sqrt
{3}}},}] and C2 be a small circle about         &#x2212; i   3     .
{\displaystyle {\tfrac {-i}{\sqrt {3}}}.}  [{\displaystyle {\tfrac {-i}{\sqrt
{3}}}.}] Then we arrive at the following:
             &#x2212;    4 i  3      [      &#x222E;        C  1     &#x2061;
      z   (  z +   3   i  )   (  z &#x2212;   3   i  )   (  z +   i  3     )
      z &#x2212;   i  3        d z +     &#x222E;        C  2     &#x2061;    z
      (  z +   3   i  )   (  z &#x2212;   3   i  )   (  z &#x2212;   i  3     )
      z +   i  3        d z  ]        = &#x2212;    4 i  3    [  2 &#x03C0; i
      (   z   (  z +   3   i  )   (  z &#x2212;   3   i  )   (  z +   i  3
      )     )  |   z =   i  3      + 2 &#x03C0; i     (   z   (  z +   3   i  )
      (  z &#x2212;   3   i  )   (  z &#x2212;   i  3     )     )  |   z =
      &#x2212;   i  3       ]        =    8 &#x03C0;  3    [     i  3
      (    i  3    +   3   i  )   (    i  3    &#x2212;   3   i  )   (    i  3
      +   i  3     )     +    &#x2212;   i  3       (  &#x2212;   i  3    +   3
      i  )   (  &#x2212;   i  3    &#x2212;   3   i  )   (  &#x2212;   i  3
      &#x2212;   i  3     )      ]        =    8 &#x03C0;  3    [     i  3
      (    4  3    i  )   (  &#x2212;   2  i   3       )   (   2    3   i    )
      +    &#x2212;   i  3       (    2  3    i  )   (  &#x2212;   4  3    i  )
      (  &#x2212;   2  3    i  )      ]        =    8 &#x03C0;  3    [     i  3
      i  (   4  3    )   (   2  3    )   (   2  3    )     +    &#x2212;   i  3
      &#x2212; i  (   2  3    )   (   4  3    )   (   2  3    )      ]        =
      8 &#x03C0;  3    [     1  3     (   4  3    )   (   2  3    )   (   2  3
      )     +    1  3     (   2  3    )   (   4  3    )   (   2  3    )      ]
      =    8 &#x03C0;  3    [     1  3    16  3   3       +    1  3    16  3
      3        ]        =    8 &#x03C0;  3    [    3 16   +   3 16    ]
      = &#x03C0; .       {\displaystyle {\begin{aligned}-{\frac {4i}{3}}&\left
      [\oint _{C_{1}}{\frac {\frac {z}{\left(z+{\sqrt {3}}i\right)\left(z-
      {\sqrt {3}}i\right)\left(z+{\frac {i}{\sqrt {3}}}\right)}}{z-{\frac {i}
      {\sqrt {3}}}}}\,dz+\oint _{C_{2}}{\frac {\frac {z}{\left(z+{\sqrt
      {3}}i\right)\left(z-{\sqrt {3}}i\right)\left(z-{\frac {i}{\sqrt
      {3}}}\right)}}{z+{\frac {i}{\sqrt {3}}}}}\,dz\right]\\&=-{\frac {4i}
      {3}}\left[2\pi i\left.\left({\frac {z}{\left(z+{\sqrt {3}}i\right)\left
      (z-{\sqrt {3}}i\right)\left(z+{\frac {i}{\sqrt
      {3}}}\right)}}\right)\right|_{z={\frac {i}{\sqrt {3}}}}+2\pi i\left.\left
      ({\frac {z}{\left(z+{\sqrt {3}}i\right)\left(z-{\sqrt {3}}i\right)\left
      (z-{\frac {i}{\sqrt {3}}}\right)}}\right)\right|_{z=-{\frac {i}{\sqrt
      {3}}}}\right]\\&={\frac {8\pi }{3}}\left[{\frac {\frac {i}{\sqrt {3}}}
      {\left({\frac {i}{\sqrt {3}}}+{\sqrt {3}}i\right)\left({\frac {i}{\sqrt
      {3}}}-{\sqrt {3}}i\right)\left({\frac {i}{\sqrt {3}}}+{\frac {i}{\sqrt
      {3}}}\right)}}+{\frac {-{\frac {i}{\sqrt {3}}}}{\left(-{\frac {i}{\sqrt
      {3}}}+{\sqrt {3}}i\right)\left(-{\frac {i}{\sqrt {3}}}-{\sqrt
      {3}}i\right)\left(-{\frac {i}{\sqrt {3}}}-{\frac {i}{\sqrt
      {3}}}\right)}}\right]\\&={\frac {8\pi }{3}}\left[{\frac {\frac {i}{\sqrt
      {3}}}{\left({\frac {4}{\sqrt {3}}}i\right)\left(-{\frac {2}{i{\sqrt
      {3}}}}\right)\left({\frac {2}{{\sqrt {3}}i}}\right)}}+{\frac {-{\frac {i}
      {\sqrt {3}}}}{\left({\frac {2}{\sqrt {3}}}i\right)\left(-{\frac {4}{\sqrt
      {3}}}i\right)\left(-{\frac {2}{\sqrt {3}}}i\right)}}\right]\\&={\frac
      {8\pi }{3}}\left[{\frac {\frac {i}{\sqrt {3}}}{i\left({\frac {4}{\sqrt
      {3}}}\right)\left({\frac {2}{\sqrt {3}}}\right)\left({\frac {2}{\sqrt
      {3}}}\right)}}+{\frac {-{\frac {i}{\sqrt {3}}}}{-i\left({\frac {2}{\sqrt
      {3}}}\right)\left({\frac {4}{\sqrt {3}}}\right)\left({\frac {2}{\sqrt
      {3}}}\right)}}\right]\\&={\frac {8\pi }{3}}\left[{\frac {\frac {1}{\sqrt
      {3}}}{\left({\frac {4}{\sqrt {3}}}\right)\left({\frac {2}{\sqrt
      {3}}}\right)\left({\frac {2}{\sqrt {3}}}\right)}}+{\frac {\frac {1}{\sqrt
      {3}}}{\left({\frac {2}{\sqrt {3}}}\right)\left({\frac {4}{\sqrt
      {3}}}\right)\left({\frac {2}{\sqrt {3}}}\right)}}\right]\\&={\frac {8\pi
      }{3}}\left[{\frac {\frac {1}{\sqrt {3}}}{\frac {16}{3{\sqrt {3}}}}}+
      {\frac {\frac {1}{\sqrt {3}}}{\frac {16}{3{\sqrt {3}}}}}\right]\\&={\frac
      {8\pi }{3}}\left[{\frac {3}{16}}+{\frac {3}{16}}\right]\\&=\pi .\end
      {aligned}}}  [{\displaystyle {\begin{aligned}-{\frac {4i}{3}}&\left[\oint
      _{C_{1}}{\frac {\frac {z}{\left(z+{\sqrt {3}}i\right)\left(z-{\sqrt
      {3}}i\right)\left(z+{\frac {i}{\sqrt {3}}}\right)}}{z-{\frac {i}{\sqrt
      {3}}}}}\,dz+\oint _{C_{2}}{\frac {\frac {z}{\left(z+{\sqrt
      {3}}i\right)\left(z-{\sqrt {3}}i\right)\left(z-{\frac {i}{\sqrt
      {3}}}\right)}}{z+{\frac {i}{\sqrt {3}}}}}\,dz\right]\\&=-{\frac {4i}
      {3}}\left[2\pi i\left.\left({\frac {z}{\left(z+{\sqrt {3}}i\right)\left
      (z-{\sqrt {3}}i\right)\left(z+{\frac {i}{\sqrt
      {3}}}\right)}}\right)\right|_{z={\frac {i}{\sqrt {3}}}}+2\pi i\left.\left
      ({\frac {z}{\left(z+{\sqrt {3}}i\right)\left(z-{\sqrt {3}}i\right)\left
      (z-{\frac {i}{\sqrt {3}}}\right)}}\right)\right|_{z=-{\frac {i}{\sqrt
      {3}}}}\right]\\&={\frac {8\pi }{3}}\left[{\frac {\frac {i}{\sqrt {3}}}
      {\left({\frac {i}{\sqrt {3}}}+{\sqrt {3}}i\right)\left({\frac {i}{\sqrt
      {3}}}-{\sqrt {3}}i\right)\left({\frac {i}{\sqrt {3}}}+{\frac {i}{\sqrt
      {3}}}\right)}}+{\frac {-{\frac {i}{\sqrt {3}}}}{\left(-{\frac {i}{\sqrt
      {3}}}+{\sqrt {3}}i\right)\left(-{\frac {i}{\sqrt {3}}}-{\sqrt
      {3}}i\right)\left(-{\frac {i}{\sqrt {3}}}-{\frac {i}{\sqrt
      {3}}}\right)}}\right]\\&={\frac {8\pi }{3}}\left[{\frac {\frac {i}{\sqrt
      {3}}}{\left({\frac {4}{\sqrt {3}}}i\right)\left(-{\frac {2}{i{\sqrt
      {3}}}}\right)\left({\frac {2}{{\sqrt {3}}i}}\right)}}+{\frac {-{\frac {i}
      {\sqrt {3}}}}{\left({\frac {2}{\sqrt {3}}}i\right)\left(-{\frac {4}{\sqrt
      {3}}}i\right)\left(-{\frac {2}{\sqrt {3}}}i\right)}}\right]\\&={\frac
      {8\pi }{3}}\left[{\frac {\frac {i}{\sqrt {3}}}{i\left({\frac {4}{\sqrt
      {3}}}\right)\left({\frac {2}{\sqrt {3}}}\right)\left({\frac {2}{\sqrt
      {3}}}\right)}}+{\frac {-{\frac {i}{\sqrt {3}}}}{-i\left({\frac {2}{\sqrt
      {3}}}\right)\left({\frac {4}{\sqrt {3}}}\right)\left({\frac {2}{\sqrt
      {3}}}\right)}}\right]\\&={\frac {8\pi }{3}}\left[{\frac {\frac {1}{\sqrt
      {3}}}{\left({\frac {4}{\sqrt {3}}}\right)\left({\frac {2}{\sqrt
      {3}}}\right)\left({\frac {2}{\sqrt {3}}}\right)}}+{\frac {\frac {1}{\sqrt
      {3}}}{\left({\frac {2}{\sqrt {3}}}\right)\left({\frac {4}{\sqrt
      {3}}}\right)\left({\frac {2}{\sqrt {3}}}\right)}}\right]\\&={\frac {8\pi
      }{3}}\left[{\frac {\frac {1}{\sqrt {3}}}{\frac {16}{3{\sqrt {3}}}}}+
      {\frac {\frac {1}{\sqrt {3}}}{\frac {16}{3{\sqrt {3}}}}}\right]\\&={\frac
      {8\pi }{3}}\left[{\frac {3}{16}}+{\frac {3}{16}}\right]\\&=\pi .\end
      {aligned}}}]
**** Example 3a â trigonometric integrals, the general procedure[edit] ****
The above method may be applied to all integrals of the type
          &#x222B;  0   2 &#x03C0;      P   (   sin &#x2061; ( t ) , sin
      &#x2061; ( 2 t ) , &#x2026; , cos &#x2061; ( t ) , cos &#x2061; ( 2 t ) ,
      &#x2026;   )     Q   (   sin &#x2061; ( t ) , sin &#x2061; ( 2 t ) ,
      &#x2026; , cos &#x2061; ( t ) , cos &#x2061; ( 2 t ) , &#x2026;   )
      d t   {\displaystyle \int _{0}^{2\pi }{\frac {P{\big (}\sin(t),\sin
      (2t),\ldots ,\cos(t),\cos(2t),\ldots {\big )}}{Q{\big (}\sin(t),\sin
      (2t),\ldots ,\cos(t),\cos(2t),\ldots {\big )}}}\,dt}  [{\displaystyle
      \int _{0}^{2\pi }{\frac {P{\big (}\sin(t),\sin(2t),\ldots ,\cos(t),\cos
      (2t),\ldots {\big )}}{Q{\big (}\sin(t),\sin(2t),\ldots ,\cos(t),\cos
      (2t),\ldots {\big )}}}\,dt}]
where P and Q are polynomials, i.e. a rational function in trigonometric terms
is being integrated. Note that the bounds of integration may as well be Ï and
âÏ, as in the previous example, or any other pair of endpoints 2Ï apart.
The trick is to use the substitution z = eit where dz = ieit dt and hence
           1  i z     d z = d t .   {\displaystyle {\frac {1}{iz}}\,dz=dt.}  [
      {\frac {1}{iz}}\,dz=dt.]
This substitution maps the interval [0, 2Ï] to the unit circle. Furthermore,
         sin &#x2061; ( k t ) =     e  i k t   &#x2212;  e  &#x2212; i k t
      2 i    =     z  k   &#x2212;  z  &#x2212; k     2 i      {\displaystyle
      \sin(kt)={\frac {e^{ikt}-e^{-ikt}}{2i}}={\frac {z^{k}-z^{-k}}{2i}}}  [
      {\displaystyle \sin(kt)={\frac {e^{ikt}-e^{-ikt}}{2i}}={\frac {z^{k}-z^{-
      k}}{2i}}}]
and
         cos &#x2061; ( k t ) =     e  i k t   +  e  &#x2212; i k t    2   =
      z  k   +  z  &#x2212; k    2     {\displaystyle \cos(kt)={\frac {e^
      {ikt}+e^{-ikt}}{2}}={\frac {z^{k}+z^{-k}}{2}}}  [{\displaystyle \cos(kt)=
      {\frac {e^{ikt}+e^{-ikt}}{2}}={\frac {z^{k}+z^{-k}}{2}}}]
so that a rational function f(z) in z results from the substitution, and the
integral becomes
             &#x222E;        |  z  |  = 1   &#x2061; f ( z )   1  i z     d z
      {\displaystyle \oint _{|z|=1}f(z){\frac {1}{iz}}\,dz}  [\oint _{|z|=1}f
      (z){\frac {1}{iz}}\,dz]
which is in turn computed by summing the residues of f(z)1/iz inside the unit
circle.
[TrigonometricToComplex.png]
The image at right illustrates this for
         I =  &#x222B;  0    &#x03C0; 2      1  1 + ( sin &#x2061; t  )  2
      d t ,   {\displaystyle I=\int _{0}^{\frac {\pi }{2}}{\frac {1}{1+(\sin
      t)^{2}}}\,dt,}  [{\displaystyle I=\int _{0}^{\frac {\pi }{2}}{\frac {1}
      {1+(\sin t)^{2}}}\,dt,}]
which we now compute. The first step is to recognize that
         I =   1 4    &#x222B;  0   2 &#x03C0;     1  1 + ( sin &#x2061; t  )
      2       d t .   {\displaystyle I={\frac {1}{4}}\int _{0}^{2\pi }{\frac
      {1}{1+(\sin t)^{2}}}\,dt.}  [{\displaystyle I={\frac {1}{4}}\int _{0}^
      {2\pi }{\frac {1}{1+(\sin t)^{2}}}\,dt.}]
The substitution yields
           1 4       &#x222E;        |  z  |  = 1   &#x2061;    4 i z    z  4
      &#x2212; 6  z  2   + 1     d z =     &#x222E;        |  z  |  = 1
      &#x2061;    i z    z  4   &#x2212; 6  z  2   + 1     d z .
      {\displaystyle {\frac {1}{4}}\oint _{|z|=1}{\frac {4iz}{z^{4}-6z^
      {2}+1}}\,dz=\oint _{|z|=1}{\frac {iz}{z^{4}-6z^{2}+1}}\,dz.}  [{\frac {1}
      {4}}\oint _{|z|=1}{\frac {4iz}{z^{4}-6z^{2}+1}}\,dz=\oint _{|z|=1}{\frac
      {iz}{z^{4}-6z^{2}+1}}\,dz.]
The poles of this function are at 1 Â± √2 and â1 Â± √2. Of these, 1 + √2 and
â1 â √2 are outside the unit circle (shown in red, not to scale), whereas 1
â √2 and â1 + √2 are inside the unit circle (shown in blue). The
corresponding residues are both equal to âi√2/16, so that the value of the
integral is
         I = 2 &#x03C0; i  2  (  &#x2212;    2  16   i  )  = &#x03C0;    2  4
      .   {\displaystyle I=2\pi i\;2\left(-{\frac {\sqrt {2}}{16}}i\right)=\pi
      {\frac {\sqrt {2}}{4}}.}  [I=2\pi i\;2\left(-{\frac {\sqrt {2}}
      {16}}i\right)=\pi {\frac {\sqrt {2}}{4}}.]
**** Example 4 â branch cuts[edit] ****
Consider the real integral
          &#x222B;  0   &#x221E;      x    x  2   + 6 x + 8     d x .
      {\displaystyle \int _{0}^{\infty }{\frac {\sqrt {x}}{x^{2}+6x+8}}\,dx.}
      [{\displaystyle \int _{0}^{\infty }{\frac {\sqrt {x}}{x^{2}+6x+8}}\,dx.}]
We can begin by formulating the complex integral
          &#x222B;  C      z    z  2   + 6 z + 8     d z = I .   {\displaystyle
      \int _{C}{\frac {\sqrt {z}}{z^{2}+6z+8}}\,dz=I.}  [{\displaystyle \int _
      {C}{\frac {\sqrt {z}}{z^{2}+6z+8}}\,dz=I.}]
[Keyhole_contour.svg]
We can use the Cauchy integral formula or residue theorem again to obtain the
relevant residues. However, the important thing to note is that z&#x200b;1⁄2 =
e&#x200b;1⁄2Log z, so z&#x200b;1⁄2 has a branch_cut. This affects our choice of
the contour C. Normally the logarithm branch cut is defined as the negative
real axis, however, this makes the calculation of the integral slightly more
complicated, so we define it to be the positive real axis.
Then, we use the so-called keyhole contour, which consists of a small circle
about the origin of radius Îµ say, extending to a line segment parallel and
close to the positive real axis but not touching it, to an almost full circle,
returning to a line segment parallel, close, and below the positive real axis
in the negative sense, returning to the small circle in the middle.
Note that z = â2 and z = â4 are inside the big circle. These are the two
remaining poles, derivable by factoring the denominator of the integrand. The
branch point at z = 0 was avoided by detouring around the origin.
Let Î³ be the small circle of radius Îµ, Î the larger, with radius R, then
          &#x222B;  C   =  &#x222B;  &#x03B5;   R   +  &#x222B;  &#x0393;   +
      &#x222B;  R   &#x03B5;   +  &#x222B;  &#x03B3;   .   {\displaystyle \int
      _{C}=\int _{\varepsilon }^{R}+\int _{\Gamma }+\int _{R}^{\varepsilon
      }+\int _{\gamma }.}  [\int _{C}=\int _{\varepsilon }^{R}+\int _{\Gamma
      }+\int _{R}^{\varepsilon }+\int _{\gamma }.]
It can be shown that the integrals over Î and Î³ both tend to zero as Îµ â 0
and R â â, by an estimation argument above, that leaves two terms. Now
since z&#x200b;1⁄2 = e&#x200b;1⁄2Log z, on the contour outside the branch cut,
we have gained 2Ï in argument along Î³. (By Euler's_identity, eiÏ represents
the unit vector, which therefore has Ï as its log. This Ï is what is meant by
the argument of z. The coefficient of 1/2 forces us to use 2Ï.) So
              &#x222B;  R   &#x03B5;      z    z  2   + 6 z + 8     d z    =
      &#x222B;  R   &#x03B5;      e    1 2   Log &#x2061; z     z  2   + 6 z +
      8     d z       =  &#x222B;  R   &#x03B5;      e    1 2   ( log &#x2061;
      |  z  |  + i arg &#x2061;  z  )     z  2   + 6 z + 8     d z       =
      &#x222B;  R   &#x03B5;       e    1 2   log &#x2061;  |  z  |     e    1
      2   ( 2 &#x03C0; i )      z  2   + 6 z + 8     d z       =  &#x222B;  R
      &#x03B5;       e    1 2   log &#x2061;  |  z  |     e  &#x03C0; i      z
      2   + 6 z + 8     d z       =  &#x222B;  R   &#x03B5;      &#x2212;   z
      z  2   + 6 z + 8     d z       =  &#x222B;  &#x03B5;   R      z    z  2
      + 6 z + 8     d z .       {\displaystyle {\begin{aligned}\int _{R}^
      {\varepsilon }{\frac {\sqrt {z}}{z^{2}+6z+8}}\,dz&=\int _{R}^{\varepsilon
      }{\frac {e^{{\frac {1}{2}}\operatorname {Log} z}}{z^
      {2}+6z+8}}\,dz\\&=\int _{R}^{\varepsilon }{\frac {e^{{\frac {1}{2}}(\log
      |z|+i\arg {z})}}{z^{2}+6z+8}}\,dz\\&=\int _{R}^{\varepsilon }{\frac {e^{
      {\frac {1}{2}}\log |z|}e^{{\frac {1}{2}}(2\pi i)}}{z^
      {2}+6z+8}}\,dz\\&=\int _{R}^{\varepsilon }{\frac {e^{{\frac {1}{2}}\log
      |z|}e^{\pi i}}{z^{2}+6z+8}}\,dz\\&=\int _{R}^{\varepsilon }{\frac {-
      {\sqrt {z}}}{z^{2}+6z+8}}\,dz\\&=\int _{\varepsilon }^{R}{\frac {\sqrt
      {z}}{z^{2}+6z+8}}\,dz.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}\int _{R}^{\varepsilon }{\frac {\sqrt {z}}{z^
      {2}+6z+8}}\,dz&=\int _{R}^{\varepsilon }{\frac {e^{{\frac {1}
      {2}}\operatorname {Log} z}}{z^{2}+6z+8}}\,dz\\&=\int _{R}^{\varepsilon }
      {\frac {e^{{\frac {1}{2}}(\log |z|+i\arg {z})}}{z^{2}+6z+8}}\,dz\\&=\int
      _{R}^{\varepsilon }{\frac {e^{{\frac {1}{2}}\log |z|}e^{{\frac {1}{2}}
      (2\pi i)}}{z^{2}+6z+8}}\,dz\\&=\int _{R}^{\varepsilon }{\frac {e^{{\frac
      {1}{2}}\log |z|}e^{\pi i}}{z^{2}+6z+8}}\,dz\\&=\int _{R}^{\varepsilon }
      {\frac {-{\sqrt {z}}}{z^{2}+6z+8}}\,dz\\&=\int _{\varepsilon }^{R}{\frac
      {\sqrt {z}}{z^{2}+6z+8}}\,dz.\end{aligned}}}]
Therefore:
          &#x222B;  C      z    z  2   + 6 z + 8     d z = 2  &#x222B;  0
      &#x221E;      x    x  2   + 6 x + 8     d x .   {\displaystyle \int _{C}
      {\frac {\sqrt {z}}{z^{2}+6z+8}}\,dz=2\int _{0}^{\infty }{\frac {\sqrt
      {x}}{x^{2}+6x+8}}\,dx.}  [{\displaystyle \int _{C}{\frac {\sqrt {z}}{z^
      {2}+6z+8}}\,dz=2\int _{0}^{\infty }{\frac {\sqrt {x}}{x^{2}+6x+8}}\,dx.}]
By using the residue theorem or the Cauchy integral formula (first employing
the partial fractions method to derive a sum of two simple contour integrals)
one obtains
         &#x03C0; i  (    i  2    &#x2212; i  )  =  &#x222B;  0   &#x221E;
      x    x  2   + 6 x + 8     d x = &#x03C0;  (  1 &#x2212;   1  2     )  .
      &#x25FB;   {\displaystyle \pi i\left({\frac {i}{\sqrt {2}}}-i\right)=\int
      _{0}^{\infty }{\frac {\sqrt {x}}{x^{2}+6x+8}}\,dx=\pi \left(1-{\frac {1}
      {\sqrt {2}}}\right).\quad \square }  [{\displaystyle \pi i\left({\frac
      {i}{\sqrt {2}}}-i\right)=\int _{0}^{\infty }{\frac {\sqrt {x}}{x^
      {2}+6x+8}}\,dx=\pi \left(1-{\frac {1}{\sqrt {2}}}\right).\quad \square }]
**** Example 5 â the square of the logarithm[edit] ****
[KeyholeContourLeft.png]
This section treats a type of integral of which
          &#x222B;  0   &#x221E;      log &#x2061; x    (  1 +  x  2    )   2
      d x   {\displaystyle \int _{0}^{\infty }{\frac {\log x}{\left(1+x^
      {2}\right)^{2}}}\,dx}  [{\displaystyle \int _{0}^{\infty }{\frac {\log x}
      {\left(1+x^{2}\right)^{2}}}\,dx}]
is an example.
To calculate this integral, one uses the function
         f ( z ) =   (    log &#x2061; z   1 +  z  2      )   2
      {\displaystyle f(z)=\left({\frac {\log z}{1+z^{2}}}\right)^{2}}  [
      {\displaystyle f(z)=\left({\frac {\log z}{1+z^{2}}}\right)^{2}}]
and the branch of the logarithm corresponding to âÏ < arg z â¤ Ï.
We will calculate the integral of f(z) along the keyhole contour shown at
right. As it turns out this integral is a multiple of the initial integral that
we wish to calculate and by the Cauchy residue theorem we have
              (   &#x222B;  R   +  &#x222B;  M   +  &#x222B;  N   +  &#x222B;
      r    )  f ( z )  d z    = 2 &#x03C0; i   (    Res  z = i   &#x2061; f ( z
      ) +  Res  z = &#x2212; i   &#x2061; f ( z )   )         = 2 &#x03C0; i
      (  &#x2212;   &#x03C0; 4   +   1 16   i  &#x03C0;  2   &#x2212;
      &#x03C0; 4   &#x2212;   1 16   i  &#x03C0;  2    )        = &#x2212; i
      &#x03C0;  2   .       {\displaystyle {\begin{aligned}\left(\int _{R}+\int
      _{M}+\int _{N}+\int _{r}\right)f(z)\,dz&=2\pi i{\big (}\operatorname
      {Res} _{z=i}f(z)+\operatorname {Res} _{z=-i}f(z){\big )}\\&=2\pi i\left(-
      {\frac {\pi }{4}}+{\frac {1}{16}}i\pi ^{2}-{\frac {\pi }{4}}-{\frac {1}
      {16}}i\pi ^{2}\right)\\&=-i\pi ^{2}.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}\left(\int _{R}+\int _{M}+\int _{N}+\int _{r}\right)f
      (z)\,dz&=2\pi i{\big (}\operatorname {Res} _{z=i}f(z)+\operatorname {Res}
      _{z=-i}f(z){\big )}\\&=2\pi i\left(-{\frac {\pi }{4}}+{\frac {1}{16}}i\pi
      ^{2}-{\frac {\pi }{4}}-{\frac {1}{16}}i\pi ^{2}\right)\\&=-i\pi ^{2}.\end
      {aligned}}}]
Let R be the radius of the large circle, and r the radius of the small one. We
will denote the upper line by M, and the lower line by N. As before we take the
limit when R â â and r â 0. The contributions from the two circles
vanish. For example, one has the following upper bound with the ML_lemma:
          |   &#x222B;  R   f ( z )  d z  |  &#x2264; 2 &#x03C0; R    ( log
      &#x2061; R  )  2   +  &#x03C0;  2      (   R  2   &#x2212; 1  )   2
      &#x2192; 0.   {\displaystyle \left|\int _{R}f(z)\,dz\right|\leq 2\pi R
      {\frac {(\log R)^{2}+\pi ^{2}}{\left(R^{2}-1\right)^{2}}}\to 0.}  [
      {\displaystyle \left|\int _{R}f(z)\,dz\right|\leq 2\pi R{\frac {(\log R)^
      {2}+\pi ^{2}}{\left(R^{2}-1\right)^{2}}}\to 0.}]
In order to compute the contributions of M and N we set z = âx + iÎµ on M and
z = âx â iÎµ on N, with 0 < x < â:
             &#x2212; i  &#x03C0;  2      =  (   &#x222B;  R   +  &#x222B;  M
      +  &#x222B;  N   +  &#x222B;  r    )  f ( z )  d z       =  (   &#x222B;
      M   +  &#x222B;  N    )  f ( z )  d z      &#x222B;  R   ,  &#x222B;  r
      &#xA0;vanish         = &#x2212;  &#x222B;  &#x221E;   0     (    log
      &#x2061; ( &#x2212; x + i &#x03B5; )   1 + ( &#x2212; x + i &#x03B5;  )
      2      )   2    d x &#x2212;  &#x222B;  0   &#x221E;     (    log
      &#x2061; ( &#x2212; x &#x2212; i &#x03B5; )   1 + ( &#x2212; x &#x2212; i
      &#x03B5;  )  2      )   2    d x       =  &#x222B;  0   &#x221E;
      (    log &#x2061; ( &#x2212; x + i &#x03B5; )   1 + ( &#x2212; x + i
      &#x03B5;  )  2      )   2    d x &#x2212;  &#x222B;  0   &#x221E;
      (    log &#x2061; ( &#x2212; x &#x2212; i &#x03B5; )   1 + ( &#x2212; x
      &#x2212; i &#x03B5;  )  2      )   2    d x       =  &#x222B;  0
      &#x221E;     (    log &#x2061; x + i &#x03C0;   1 +  x  2      )   2    d
      x &#x2212;  &#x222B;  0   &#x221E;     (    log &#x2061; x &#x2212; i
      &#x03C0;   1 +  x  2      )   2    d x    &#x03B5; &#x2192; 0       =
      &#x222B;  0   &#x221E;      ( log &#x2061; x + i &#x03C0;  )  2
      &#x2212; ( log &#x2061; x &#x2212; i &#x03C0;  )  2      (  1 +  x  2
      )   2      d x       =  &#x222B;  0   &#x221E;      4 &#x03C0; i log
      &#x2061; x    (  1 +  x  2    )   2      d x       = 4 &#x03C0; i
      &#x222B;  0   &#x221E;      log &#x2061; x    (  1 +  x  2    )   2
      d x       {\displaystyle {\begin{aligned}-i\pi ^{2}&=\left(\int _{R}+\int
      _{M}+\int _{N}+\int _{r}\right)f(z)\,dz\\&=\left(\int _{M}+\int _
      {N}\right)f(z)\,dz&&\int _{R},\int _{r}{\mbox{ vanish}}\\&=-\int _{\infty
      }^{0}\left({\frac {\log(-x+i\varepsilon )}{1+(-x+i\varepsilon )^
      {2}}}\right)^{2}\,dx-\int _{0}^{\infty }\left({\frac {\log(-x-
      i\varepsilon )}{1+(-x-i\varepsilon )^{2}}}\right)^{2}\,dx\\&=\int _{0}^
      {\infty }\left({\frac {\log(-x+i\varepsilon )}{1+(-x+i\varepsilon )^
      {2}}}\right)^{2}\,dx-\int _{0}^{\infty }\left({\frac {\log(-x-
      i\varepsilon )}{1+(-x-i\varepsilon )^{2}}}\right)^{2}\,dx\\&=\int _{0}^
      {\infty }\left({\frac {\log x+i\pi }{1+x^{2}}}\right)^{2}\,dx-\int _{0}^
      {\infty }\left({\frac {\log x-i\pi }{1+x^{2}}}\right)^
      {2}\,dx&&\varepsilon \to 0\\&=\int _{0}^{\infty }{\frac {(\log x+i\pi )^
      {2}-(\log x-i\pi )^{2}}{\left(1+x^{2}\right)^{2}}}\,dx\\&=\int _{0}^
      {\infty }{\frac {4\pi i\log x}{\left(1+x^{2}\right)^{2}}}\,dx\\&=4\pi
      i\int _{0}^{\infty }{\frac {\log x}{\left(1+x^{2}\right)^{2}}}\,dx\end
      {aligned}}}  [{\displaystyle {\begin{aligned}-i\pi ^{2}&=\left(\int _
      {R}+\int _{M}+\int _{N}+\int _{r}\right)f(z)\,dz\\&=\left(\int _{M}+\int
      _{N}\right)f(z)\,dz&&\int _{R},\int _{r}{\mbox{ vanish}}\\&=-\int _
      {\infty }^{0}\left({\frac {\log(-x+i\varepsilon )}{1+(-x+i\varepsilon )^
      {2}}}\right)^{2}\,dx-\int _{0}^{\infty }\left({\frac {\log(-x-
      i\varepsilon )}{1+(-x-i\varepsilon )^{2}}}\right)^{2}\,dx\\&=\int _{0}^
      {\infty }\left({\frac {\log(-x+i\varepsilon )}{1+(-x+i\varepsilon )^
      {2}}}\right)^{2}\,dx-\int _{0}^{\infty }\left({\frac {\log(-x-
      i\varepsilon )}{1+(-x-i\varepsilon )^{2}}}\right)^{2}\,dx\\&=\int _{0}^
      {\infty }\left({\frac {\log x+i\pi }{1+x^{2}}}\right)^{2}\,dx-\int _{0}^
      {\infty }\left({\frac {\log x-i\pi }{1+x^{2}}}\right)^
      {2}\,dx&&\varepsilon \to 0\\&=\int _{0}^{\infty }{\frac {(\log x+i\pi )^
      {2}-(\log x-i\pi )^{2}}{\left(1+x^{2}\right)^{2}}}\,dx\\&=\int _{0}^
      {\infty }{\frac {4\pi i\log x}{\left(1+x^{2}\right)^{2}}}\,dx\\&=4\pi
      i\int _{0}^{\infty }{\frac {\log x}{\left(1+x^{2}\right)^{2}}}\,dx\end
      {aligned}}}]
which gives
          &#x222B;  0   &#x221E;      log &#x2061; x    (  1 +  x  2    )   2
      d x = &#x2212;   &#x03C0; 4   .   {\displaystyle \int _{0}^{\infty }
      {\frac {\log x}{\left(1+x^{2}\right)^{2}}}\,dx=-{\frac {\pi }{4}}.}  [
      {\displaystyle \int _{0}^{\infty }{\frac {\log x}{\left(1+x^{2}\right)^
      {2}}}\,dx=-{\frac {\pi }{4}}.}]
**** Example 6 â logarithms and the residue at infinity[edit] ****
[ContourLogs.png]
We seek to evaluate
         I =  &#x222B;  0   3       x   3 4    ( 3 &#x2212; x  )   1 4      5
      &#x2212; x     d x .   {\displaystyle I=\int _{0}^{3}{\frac {x^{\frac {3}
      {4}}(3-x)^{\frac {1}{4}}}{5-x}}\,dx.}  [{\displaystyle I=\int _{0}^{3}
      {\frac {x^{\frac {3}{4}}(3-x)^{\frac {1}{4}}}{5-x}}\,dx.}]
This requires a close study of
         f ( z ) =  z   3 4    ( 3 &#x2212; z  )   1 4    .   {\displaystyle f
      (z)=z^{\frac {3}{4}}(3-z)^{\frac {1}{4}}.}  [{\displaystyle f(z)=z^{\frac
      {3}{4}}(3-z)^{\frac {1}{4}}.}]
We will construct f(z) so that it has a branch cut on [0, 3], shown in red in
the diagram. To do this, we choose two branches of the logarithm, setting
          z   3 4    = exp &#x2061;  (    3 4   log &#x2061; z  )
      where&#xA0;   &#x2212; &#x03C0; &#x2264; arg &#x2061; z < &#x03C0;
      {\displaystyle z^{\frac {3}{4}}=\exp \left({\frac {3}{4}}\log
      z\right)\quad {\mbox{where }}-\pi \leq \arg z<\pi }  [{\displaystyle z^
      {\frac {3}{4}}=\exp \left({\frac {3}{4}}\log z\right)\quad {\mbox{where
      }}-\pi \leq \arg z<\pi }]
and
         ( 3 &#x2212; z  )   1 4    = exp &#x2061;  (    1 4   log &#x2061; ( 3
      &#x2212; z )  )     where&#xA0;   0 &#x2264; arg &#x2061; ( 3 &#x2212; z
      ) < 2 &#x03C0; .   {\displaystyle (3-z)^{\frac {1}{4}}=\exp \left({\frac
      {1}{4}}\log(3-z)\right)\quad {\mbox{where }}0\leq \arg(3-z)<2\pi .}  [
      {\displaystyle (3-z)^{\frac {1}{4}}=\exp \left({\frac {1}{4}}\log(3-
      z)\right)\quad {\mbox{where }}0\leq \arg(3-z)<2\pi .}]
The cut of z&#x200b;3⁄4 is therefore (ââ, 0] and the cut of (3 â
z)&#x200b;1⁄4 is (ââ, 3]. It is easy to see that the cut of the product of
the two, i.e. f(z), is [0, 3], because f(z) is actually continuous across
(ââ, 0). This is because when z = âr < 0 and we approach the cut from
above, f(z) has the value
          r   3 4     e    3 4   &#x03C0; i   ( 3 + r  )   1 4     e    2 4
      &#x03C0; i   =  r   3 4    ( 3 + r  )   1 4     e    5 4   &#x03C0; i   .
      {\displaystyle r^{\frac {3}{4}}e^{{\frac {3}{4}}\pi i}(3+r)^{\frac {1}
      {4}}e^{{\frac {2}{4}}\pi i}=r^{\frac {3}{4}}(3+r)^{\frac {1}{4}}e^{{\frac
      {5}{4}}\pi i}.}  [{\displaystyle r^{\frac {3}{4}}e^{{\frac {3}{4}}\pi i}
      (3+r)^{\frac {1}{4}}e^{{\frac {2}{4}}\pi i}=r^{\frac {3}{4}}(3+r)^{\frac
      {1}{4}}e^{{\frac {5}{4}}\pi i}.}]
When we approach from below, f(z) has the value
          r   3 4     e  &#x2212;   3 4   &#x03C0; i   ( 3 + r  )   1 4     e
      0 4   &#x03C0; i   =  r   3 4    ( 3 + r  )   1 4     e  &#x2212;   3 4
      &#x03C0; i   .   {\displaystyle r^{\frac {3}{4}}e^{-{\frac {3}{4}}\pi i}
      (3+r)^{\frac {1}{4}}e^{{\frac {0}{4}}\pi i}=r^{\frac {3}{4}}(3+r)^{\frac
      {1}{4}}e^{-{\frac {3}{4}}\pi i}.}  [{\displaystyle r^{\frac {3}{4}}e^{-
      {\frac {3}{4}}\pi i}(3+r)^{\frac {1}{4}}e^{{\frac {0}{4}}\pi i}=r^{\frac
      {3}{4}}(3+r)^{\frac {1}{4}}e^{-{\frac {3}{4}}\pi i}.}]
But
          e  &#x2212;   3 4   &#x03C0; i   =  e    5 4   &#x03C0; i   ,
      {\displaystyle e^{-{\frac {3}{4}}\pi i}=e^{{\frac {5}{4}}\pi i},}  [
      {\displaystyle e^{-{\frac {3}{4}}\pi i}=e^{{\frac {5}{4}}\pi i},}]
so that we have continuity across the cut. This is illustrated in the diagram,
where the two black oriented circles are labelled with the corresponding value
of the argument of the logarithm used in z&#x200b;3⁄4 and (3 â z)&#x200b;1⁄4.
We will use the contour shown in green in the diagram. To do this we must
compute the value of f(z) along the line segments just above and just below the
cut.
Let z = r (in the limit, i.e. as the two green circles shrink to radius zero),
where 0 â¤ r â¤ 3. Along the upper segment, we find that f(z) has the value
          r   3 4     e    0 4   &#x03C0; i   ( 3 &#x2212; r  )   1 4     e
      2 4   &#x03C0; i   = i  r   3 4    ( 3 &#x2212; r  )   1 4
      {\displaystyle r^{\frac {3}{4}}e^{{\frac {0}{4}}\pi i}(3-r)^{\frac {1}
      {4}}e^{{\frac {2}{4}}\pi i}=ir^{\frac {3}{4}}(3-r)^{\frac {1}{4}}}  [
      {\displaystyle r^{\frac {3}{4}}e^{{\frac {0}{4}}\pi i}(3-r)^{\frac {1}
      {4}}e^{{\frac {2}{4}}\pi i}=ir^{\frac {3}{4}}(3-r)^{\frac {1}{4}}}]
and along the lower segment,
          r   3 4     e    0 4   &#x03C0; i   ( 3 &#x2212; r  )   1 4     e
      0 4   &#x03C0; i   =  r   3 4    ( 3 &#x2212; r  )   1 4    .
      {\displaystyle r^{\frac {3}{4}}e^{{\frac {0}{4}}\pi i}(3-r)^{\frac {1}
      {4}}e^{{\frac {0}{4}}\pi i}=r^{\frac {3}{4}}(3-r)^{\frac {1}{4}}.}  [
      {\displaystyle r^{\frac {3}{4}}e^{{\frac {0}{4}}\pi i}(3-r)^{\frac {1}
      {4}}e^{{\frac {0}{4}}\pi i}=r^{\frac {3}{4}}(3-r)^{\frac {1}{4}}.}]
It follows that the integral of f(z)/5 â z along the upper segment is âiI
in the limit, and along the lower segment, I.
If we can show that the integrals along the two green circles vanish in the
limit, then we also have the value of I, by the Cauchy_residue_theorem. Let the
radius of the green circles be Ï, where Ï < 0.001 and Ï â 0, and apply the
ML_inequality. For the circle CL on the left, we find
          |   &#x222B;   C   L         f ( z )   5 &#x2212; z    d z  |
      &#x2264; 2 &#x03C0; &#x03C1;     &#x03C1;   3 4     3.001   1 4     4.999
      &#x2208;   O    (  &#x03C1;   7 4    )  &#x2192; 0.   {\displaystyle
      \left|\int _{C_{\mathrm {L} }}{\frac {f(z)}{5-z}}dz\right|\leq 2\pi \rho
      {\frac {\rho ^{\frac {3}{4}}3.001^{\frac {1}{4}}}{4.999}}\in {\mathcal
      {O}}\left(\rho ^{\frac {7}{4}}\right)\to 0.}  [{\displaystyle \left|\int
      _{C_{\mathrm {L} }}{\frac {f(z)}{5-z}}dz\right|\leq 2\pi \rho {\frac
      {\rho ^{\frac {3}{4}}3.001^{\frac {1}{4}}}{4.999}}\in {\mathcal {O}}\left
      (\rho ^{\frac {7}{4}}\right)\to 0.}]
Similarly, for the circle CR on the right, we have
          |   &#x222B;   C   R         f ( z )   5 &#x2212; z    d z  |
      &#x2264; 2 &#x03C0; &#x03C1;     3.001   3 4     &#x03C1;   1 4     1.999
      &#x2208;   O    (  &#x03C1;   5 4    )  &#x2192; 0.   {\displaystyle
      \left|\int _{C_{\mathrm {R} }}{\frac {f(z)}{5-z}}dz\right|\leq 2\pi \rho
      {\frac {3.001^{\frac {3}{4}}\rho ^{\frac {1}{4}}}{1.999}}\in {\mathcal
      {O}}\left(\rho ^{\frac {5}{4}}\right)\to 0.}  [{\displaystyle \left|\int
      _{C_{\mathrm {R} }}{\frac {f(z)}{5-z}}dz\right|\leq 2\pi \rho {\frac
      {3.001^{\frac {3}{4}}\rho ^{\frac {1}{4}}}{1.999}}\in {\mathcal {O}}\left
      (\rho ^{\frac {5}{4}}\right)\to 0.}]
Now using the Cauchy_residue_theorem, we have
         ( &#x2212; i + 1 ) I = &#x2212; 2 &#x03C0; i  (   Res  z = 5
      &#x2061;    f ( z )   5 &#x2212; z    +  Res  z = &#x221E;   &#x2061;
      f ( z )   5 &#x2212; z     )  .   {\displaystyle (-i+1)I=-2\pi i\left
      (\operatorname {Res} _{z=5}{\frac {f(z)}{5-z}}+\operatorname {Res} _
      {z=\infty }{\frac {f(z)}{5-z}}\right).}  [{\displaystyle (-i+1)I=-2\pi
      i\left(\operatorname {Res} _{z=5}{\frac {f(z)}{5-z}}+\operatorname {Res}
      _{z=\infty }{\frac {f(z)}{5-z}}\right).}]
where the minus sign is due to the clockwise direction around the residues.
Using the branch of the logarithm from before, clearly
          Res  z = 5   &#x2061;    f ( z )   5 &#x2212; z    = &#x2212;  5   3
      4     e    1 4   log &#x2061; ( &#x2212; 2 )   .   {\displaystyle
      \operatorname {Res} _{z=5}{\frac {f(z)}{5-z}}=-5^{\frac {3}{4}}e^{{\frac
      {1}{4}}\log(-2)}.}  [{\displaystyle \operatorname {Res} _{z=5}{\frac {f
      (z)}{5-z}}=-5^{\frac {3}{4}}e^{{\frac {1}{4}}\log(-2)}.}]
The pole is shown in blue in the diagram. The value simplifies to
         &#x2212;  5   3 4     e    1 4   ( log &#x2061; 2 + &#x03C0; i )   =
      &#x2212;  e    1 4   &#x03C0; i    5   3 4     2   1 4    .
      {\displaystyle -5^{\frac {3}{4}}e^{{\frac {1}{4}}(\log 2+\pi i)}=-e^{
      {\frac {1}{4}}\pi i}5^{\frac {3}{4}}2^{\frac {1}{4}}.}  [{\displaystyle -
      5^{\frac {3}{4}}e^{{\frac {1}{4}}(\log 2+\pi i)}=-e^{{\frac {1}{4}}\pi
      i}5^{\frac {3}{4}}2^{\frac {1}{4}}.}]
We use the following formula for the residue at infinity:
          Res  z = &#x221E;   &#x2061; h ( z ) =  Res  z = 0   &#x2061;
      (  &#x2212;   1  z  2     h  (   1 z   )   )  .   {\displaystyle
      \operatorname {Res} _{z=\infty }h(z)=\operatorname {Res} _{z=0}\left(-
      {\frac {1}{z^{2}}}h\left({\frac {1}{z}}\right)\right).}  [{\displaystyle
      \operatorname {Res} _{z=\infty }h(z)=\operatorname {Res} _{z=0}\left(-
      {\frac {1}{z^{2}}}h\left({\frac {1}{z}}\right)\right).}]
Substituting, we find
           1  5 &#x2212;   1 z      = &#x2212; z  (  1 + 5 z +  5  2    z  2
      +  5  3    z  3   + &#x22EF;  )    {\displaystyle {\frac {1}{5-{\frac {1}
      {z}}}}=-z\left(1+5z+5^{2}z^{2}+5^{3}z^{3}+\cdots \right)}  [{\frac {1}{5-
      {\frac {1}{z}}}}=-z\left(1+5z+5^{2}z^{2}+5^{3}z^{3}+\cdots \right)]
and
           (    1  z  3      (  3 &#x2212;   1 z    )   )    1 4    =   1 z
      ( 3 z &#x2212; 1  )   1 4    =   1 z    e    1 4   &#x03C0; i   ( 1
      &#x2212; 3 z  )   1 4    ,   {\displaystyle \left({\frac {1}{z^{3}}}\left
      (3-{\frac {1}{z}}\right)\right)^{\frac {1}{4}}={\frac {1}{z}}(3z-1)^
      {\frac {1}{4}}={\frac {1}{z}}e^{{\frac {1}{4}}\pi i}(1-3z)^{\frac {1}
      {4}},}  [{\displaystyle \left({\frac {1}{z^{3}}}\left(3-{\frac {1}
      {z}}\right)\right)^{\frac {1}{4}}={\frac {1}{z}}(3z-1)^{\frac {1}{4}}=
      {\frac {1}{z}}e^{{\frac {1}{4}}\pi i}(1-3z)^{\frac {1}{4}},}]
where we have used the fact that â1 = eÏi for the second branch of the
logarithm. Next we apply the binomial expansion, obtaining
           1 z    e    1 4   &#x03C0; i    (  1 &#x2212;    (     1 4   1   )
      3 z +    (     1 4   2   )     3  2    z  2   &#x2212;    (     1 4   3
      )     3  3    z  3   + &#x22EF;  )  .   {\displaystyle {\frac {1}{z}}e^{
      {\frac {1}{4}}\pi i}\left(1-{{\frac {1}{4}} \choose 1}3z+{{\frac {1}{4}}
      \choose 2}3^{2}z^{2}-{{\frac {1}{4}} \choose 3}3^{3}z^{3}+\cdots
      \right).}  [{\displaystyle {\frac {1}{z}}e^{{\frac {1}{4}}\pi i}\left(1-{
      {\frac {1}{4}} \choose 1}3z+{{\frac {1}{4}} \choose 2}3^{2}z^{2}-{{\frac
      {1}{4}} \choose 3}3^{3}z^{3}+\cdots \right).}]
The conclusion is that
          Res  z = &#x221E;   &#x2061;    f ( z )   5 &#x2212; z    =  e    1 4
      &#x03C0; i    (  5 &#x2212;   3 4    )  =  e    1 4   &#x03C0; i     17 4
      .   {\displaystyle \operatorname {Res} _{z=\infty }{\frac {f(z)}{5-z}}=e^
      {{\frac {1}{4}}\pi i}\left(5-{\frac {3}{4}}\right)=e^{{\frac {1}{4}}\pi
      i}{\frac {17}{4}}.}  [{\displaystyle \operatorname {Res} _{z=\infty }
      {\frac {f(z)}{5-z}}=e^{{\frac {1}{4}}\pi i}\left(5-{\frac {3}
      {4}}\right)=e^{{\frac {1}{4}}\pi i}{\frac {17}{4}}.}]
Finally, it follows that the value of I is
         I = 2 &#x03C0; i    e    1 4   &#x03C0; i    &#x2212; 1 + i
      (    17 4   &#x2212;  5   3 4     2   1 4     )  = 2 &#x03C0;  2
      &#x2212;   1 2      (    17 4   &#x2212;  5   3 4     2   1 4     )
      {\displaystyle I=2\pi i{\frac {e^{{\frac {1}{4}}\pi i}}{-1+i}}\left(
      {\frac {17}{4}}-5^{\frac {3}{4}}2^{\frac {1}{4}}\right)=2\pi 2^{-{\frac
      {1}{2}}}\left({\frac {17}{4}}-5^{\frac {3}{4}}2^{\frac {1}{4}}\right)}  [
      {\displaystyle I=2\pi i{\frac {e^{{\frac {1}{4}}\pi i}}{-1+i}}\left(
      {\frac {17}{4}}-5^{\frac {3}{4}}2^{\frac {1}{4}}\right)=2\pi 2^{-{\frac
      {1}{2}}}\left({\frac {17}{4}}-5^{\frac {3}{4}}2^{\frac {1}{4}}\right)}]
which yields
         I =   &#x03C0;  2   2       (  17 &#x2212;  5   3 4     2   9 4     )
      =   &#x03C0;  2   2       (  17 &#x2212;  40   3 4     )  .
      {\displaystyle I={\frac {\pi }{2{\sqrt {2}}}}\left(17-5^{\frac {3}{4}}2^
      {\frac {9}{4}}\right)={\frac {\pi }{2{\sqrt {2}}}}\left(17-40^{\frac {3}
      {4}}\right).}  [{\displaystyle I={\frac {\pi }{2{\sqrt {2}}}}\left(17-5^
      {\frac {3}{4}}2^{\frac {9}{4}}\right)={\frac {\pi }{2{\sqrt {2}}}}\left
      (17-40^{\frac {3}{4}}\right).}]
***** Evaluation with residue theorem[edit] *****
Using the residue_theorem, we can evaluate closed contour integrals. The
following are examples on evaluating contour integrals with the residue
theorem.
Using the residue theorem, let's evaluate this contour integral.
             &#x222E;       C   &#x2061;    e  z    z  3      d z
      {\displaystyle \oint _{C}{\frac {e^{z}}{z^{3}}}\,dz}  [{\displaystyle
      \oint _{C}{\frac {e^{z}}{z^{3}}}\,dz}]
As a refresher, the residue theorem states
             &#x222E;       C   &#x2061; f ( z ) = 2 &#x03C0; i &#x22C5;
      &#x2211; Res &#x2061; ( f ,  a  k   ) ,   {\displaystyle \oint _{C}f
      (z)=2\pi i\cdot \sum \operatorname {Res} (f,a_{k}),}  [{\displaystyle
      \oint _{C}f(z)=2\pi i\cdot \sum \operatorname {Res} (f,a_{k}),}]
where     Res   {\displaystyle \operatorname {Res} }  [\operatorname {Res}] is
the residue of     f ( z )   {\displaystyle f(z)}  [f(z)].
   f ( z )   {\displaystyle f(z)}  [f(z)] has only one pole,     0
{\displaystyle 0}  [{\displaystyle 0}]. From that, we can determine the residue
of     f ( z )   {\displaystyle f(z)}  [f(z)] to be        1 2
{\displaystyle {\tfrac {1}{2}}}  [{\tfrac {1}{2}}]
                 &#x222E;       C   &#x2061; f ( z )    =     &#x222E;       C
      &#x2061;    e  z    z  3           = 2 &#x03C0; i &#x22C5;  Res  z = 0
      &#x2061; f ( z )       = 2 &#x03C0; i  Res  z = 0   &#x2061;    e  z    z
      3           = 2 &#x03C0; i &#x22C5;   1 2         = &#x03C0; i
      {\displaystyle {\begin{aligned}\oint _{C}f(z)&=\oint _{C}{\frac {e^{z}}
      {z^{3}}}\\&=2\pi i\cdot \operatorname {Res} _{z=0}f(z)\\&=2\pi
      i\operatorname {Res} _{z=0}{\frac {e^{z}}{z^{3}}}\\&=2\pi i\cdot {\frac
      {1}{2}}\\&=\pi i\end{aligned}}}  [{\displaystyle {\begin{aligned}\oint _
      {C}f(z)&=\oint _{C}{\frac {e^{z}}{z^{3}}}\\&=2\pi i\cdot \operatorname
      {Res} _{z=0}f(z)\\&=2\pi i\operatorname {Res} _{z=0}{\frac {e^{z}}{z^
      {3}}}\\&=2\pi i\cdot {\frac {1}{2}}\\&=\pi i\end{aligned}}}]
Thus, using the residue_theorem, we can determine:
             &#x222E;       C   &#x2061;    e  z    z  3     = &#x03C0; i .
      {\displaystyle \oint _{C}{\frac {e^{z}}{z^{3}}}=\pi i.}  [{\displaystyle
      \oint _{C}{\frac {e^{z}}{z^{3}}}=\pi i.}]
***** Multivariable Contour Integrals[edit] *****
To solve multivariable contour integrals (i.e. surface_integrals, complex
volume_integrals, and higher order integrals), we must use the divergence
theorem. For right now, let     &#x2207;   {\displaystyle \nabla }  [\nabla ]
be interchangeable with     Div   {\displaystyle \operatorname {Div} }
[\operatorname{Div}]. These will both serve as the divergence of the vector
field denoted as      F    {\displaystyle \mathbf {F} }  [\mathbf {F} ]. This
theorem states:
             &#x222B; &#x22EF;  &#x222B;  U    &#x23DF;    n   Div &#x2061;
      (  F  )  d V =        &#x222E;      &#x2061; &#x22EF;     &#x222E;
      &#x2202; U    &#x23DF;    n &#x2212; 1    F  &#x22C5;  n   d S
      {\displaystyle \underbrace {\int \cdots \int _{U}} _{n}\operatorname
      {Div} (\mathbf {F} )\,dV=\underbrace {\oint \cdots \oint _{\partial U}} _
      {n-1}\mathbf {F} \cdot \mathbf {n} \,dS}  [{\displaystyle \underbrace
      {\int \cdots \int _{U}} _{n}\operatorname {Div} (\mathbf {F}
      )\,dV=\underbrace {\oint \cdots \oint _{\partial U}} _{n-1}\mathbf {F}
      \cdot \mathbf {n} \,dS}]
In addition, we also need to evaluate     &#x2207; &#x22C5;  F
{\displaystyle \nabla \cdot \mathbf {F} }  [{\displaystyle \nabla \cdot \mathbf
{F} }] where     &#x2207; &#x22C5;  F    {\displaystyle \nabla \cdot \mathbf
{F} }  [\nabla \cdot \mathbf{F}] is an alternate notation of     Div &#x2061;
(  F  )   {\displaystyle \operatorname {Div} (\mathbf {F} )}  [{\displaystyle
\operatorname {Div} (\mathbf {F} )}]. The Divergence of any dimension can be
described as
             Div &#x2061; (  F  )    = &#x2207; &#x22C5;  F        =
      (    &#x2202;  &#x2202; u    ,   &#x2202;  &#x2202; x    ,   &#x2202;
      &#x2202; y    ,   &#x2202;  &#x2202; z    , &#x22EF;  )  &#x22C5; (  F  u
      ,  F  x   ,  F  y   ,  F  z   &#x22EF; )       =  (     &#x2202;  F  u
      &#x2202; u    +    &#x2202;  F  x     &#x2202; x    +    &#x2202;  F  y
      &#x2202; y    +    &#x2202;  F  z     &#x2202; z    &#x22EF;  )
      {\displaystyle {\begin{aligned}\operatorname {Div} (\mathbf {F} )&=\nabla
      \cdot \mathbf {F} \\&=\left({\frac {\partial }{\partial u}},{\frac
      {\partial }{\partial x}},{\frac {\partial }{\partial y}},{\frac {\partial
      }{\partial z}},\cdots \right)\cdot (F_{u},F_{x},F_{y},F_{z}\cdots
      )\\&=\left({\frac {\partial F_{u}}{\partial u}}+{\frac {\partial F_{x}}
      {\partial x}}+{\frac {\partial F_{y}}{\partial y}}+{\frac {\partial F_
      {z}}{\partial z}}\cdots \right)\end{aligned}}}  [{\displaystyle {\begin
      {aligned}\operatorname {Div} (\mathbf {F} )&=\nabla \cdot \mathbf {F}
      \\&=\left({\frac {\partial }{\partial u}},{\frac {\partial }{\partial
      x}},{\frac {\partial }{\partial y}},{\frac {\partial }{\partial
      z}},\cdots \right)\cdot (F_{u},F_{x},F_{y},F_{z}\cdots )\\&=\left({\frac
      {\partial F_{u}}{\partial u}}+{\frac {\partial F_{x}}{\partial x}}+{\frac
      {\partial F_{y}}{\partial y}}+{\frac {\partial F_{z}}{\partial z}}\cdots
      \right)\end{aligned}}}]
**** Example 1[edit] ****
Let the vector_field      F  = sin &#x2061; ( 2 x ) + sin &#x2061; ( 2 y ) +
sin &#x2061; ( 2 z )   {\displaystyle \mathbf {F} =\sin(2x)+\sin(2y)+\sin(2z)}
[{\displaystyle \mathbf {F} =\sin(2x)+\sin(2y)+\sin(2z)}] and be bounded by the
following
          0 &#x2264; x &#x2264; 1    0 &#x2264; y &#x2264; 3 &#x03C0;
      &#x2212; 1 &#x2264; z &#x2264; 4    {\displaystyle {0\leq x\leq 1}\quad
      {0\leq y\leq 3\pi }\quad {-1\leq z\leq 4}}  [{\displaystyle {0\leq x\leq
      1}\quad {0\leq y\leq 3\pi }\quad {-1\leq z\leq 4}}]
The corresponding double contour integral would be set up as such:
      [\oiint]      S     {\displaystyle {\scriptstyle S}}  [{\scriptstyle S}]
      F  &#x22C5;  n   d S   {\displaystyle \mathbf {F} \cdot \mathbf {n} \,dS}
      [{\displaystyle \mathbf {F} \cdot \mathbf {n} \,dS}]
We now evaluate     &#x2207; &#x22C5;  F    {\displaystyle \nabla \cdot \mathbf
{F} }  [\nabla \cdot \mathbf {F} ]. While we're at it, let's set up the
corresponding triple integral:
               =  &#x222D;  V    (     &#x2202;  F  x     &#x2202; x    +
      &#x2202;  F  y     &#x2202; y    +    &#x2202;  F  z     &#x2202; z     )
      d V       =  &#x222D;  V    (     &#x2202; sin &#x2061; ( 2 x )
      &#x2202; x    +    &#x2202; sin &#x2061; ( 2 y )   &#x2202; y    +
      &#x2202; sin &#x2061; ( 2 z )   &#x2202; z     )   d V       =  &#x222D;
      V   2 ( cos &#x2061; ( 2 x ) + cos &#x2061; ( 2 y ) + cos &#x2061; ( 2 z
      ) )  d V       =  &#x222B;  0   1    &#x222B;  0   3    &#x222B;
      &#x2212; 1   4   2 ( cos &#x2061; ( 2 x ) + cos &#x2061; ( 2 y ) + cos
      &#x2061; ( 2 z ) )  d x  d y  d z       =  &#x222B;  0   1    &#x222B;  0
      3   ( 10 cos &#x2061; ( 2 y ) + sin &#x2061; ( 8 ) + sin &#x2061; ( 2 ) +
      10 cos &#x2061; ( z ) )  d y  d z       =  &#x222B;  0   1   ( 30 cos
      &#x2061; ( 2 z ) + 3 sin &#x2061; ( 2 ) + 3 sin &#x2061; ( 8 ) + 5 sin
      &#x2061; ( 6 ) )  d z       = 18 sin &#x2061; ( 2 ) + 3 sin &#x2061; ( 8
      ) + 5 sin &#x2061; ( 6 )       {\displaystyle {\begin{aligned}&=\iiint _
      {V}\left({\frac {\partial F_{x}}{\partial x}}+{\frac {\partial F_{y}}
      {\partial y}}+{\frac {\partial F_{z}}{\partial z}}\right)\,dV\\&=\iiint _
      {V}\left({\frac {\partial \sin(2x)}{\partial x}}+{\frac {\partial \sin
      (2y)}{\partial y}}+{\frac {\partial \sin(2z)}{\partial
      z}}\right)\,dV\\&=\iiint _{V}2(\cos(2x)+\cos(2y)+\cos(2z))\,dV\\&=\int _
      {0}^{1}\int _{0}^{3}\int _{-1}^{4}2(\cos(2x)+\cos(2y)+\cos
      (2z))\,dx\,dy\,dz\\&=\int _{0}^{1}\int _{0}^{3}(10\cos(2y)+\sin(8)+\sin
      (2)+10\cos(z))\,dy\,dz\\&=\int _{0}^{1}(30\cos(2z)+3\sin(2)+3\sin
      (8)+5\sin(6))\,dz\\&=18\sin(2)+3\sin(8)+5\sin(6)\end{aligned}}}  [
      {\displaystyle {\begin{aligned}&=\iiint _{V}\left({\frac {\partial F_{x}}
      {\partial x}}+{\frac {\partial F_{y}}{\partial y}}+{\frac {\partial F_
      {z}}{\partial z}}\right)\,dV\\&=\iiint _{V}\left({\frac {\partial \sin
      (2x)}{\partial x}}+{\frac {\partial \sin(2y)}{\partial y}}+{\frac
      {\partial \sin(2z)}{\partial z}}\right)\,dV\\&=\iiint _{V}2(\cos(2x)+\cos
      (2y)+\cos(2z))\,dV\\&=\int _{0}^{1}\int _{0}^{3}\int _{-1}^{4}2(\cos
      (2x)+\cos(2y)+\cos(2z))\,dx\,dy\,dz\\&=\int _{0}^{1}\int _{0}^{3}(10\cos
      (2y)+\sin(8)+\sin(2)+10\cos(z))\,dy\,dz\\&=\int _{0}^{1}(30\cos(2z)+3\sin
      (2)+3\sin(8)+5\sin(6))\,dz\\&=18\sin(2)+3\sin(8)+5\sin(6)\end{aligned}}}]
**** Example 2[edit] ****
For example, let the vector_field      F  =  u  4   +  x  5   +  y  6   +  z
&#x2212; 3     {\displaystyle \mathbf {F} =u^{4}+x^{5}+y^{6}+z^{-3}}  [
{\displaystyle \mathbf {F} =u^{4}+x^{5}+y^{6}+z^{-3}}], and     n
{\displaystyle n}  [n] is the fourth dimension. Let this vector_field be
bounded by the following:
          0 &#x2264; x &#x2264; 1    &#x2212; 10 &#x2264; y &#x2264; 2 &#x03C0;
      4 &#x2264; z &#x2264; 5    &#x2212; 1 &#x2264; u &#x2264; 3
      {\displaystyle {0\leq x\leq 1}\quad {-10\leq y\leq 2\pi }\quad {4\leq
      z\leq 5}\quad {-1\leq u\leq 3}}  [{\displaystyle {0\leq x\leq 1}\quad {-
      10\leq y\leq 2\pi }\quad {4\leq z\leq 5}\quad {-1\leq u\leq 3}}]
To evaluate this, we must utilize the divergence_theorem as stated before, and
we must evaluate     &#x2207; &#x22C5;  F    {\displaystyle \nabla \cdot
\mathbf {F} }  [\nabla \cdot \mathbf {F} ]. For right now, let     d V = d x d
y d z d u   {\displaystyle dV=dxdydzdu}  [{\displaystyle dV=dxdydzdu}]
      [\oiiint]      S     {\displaystyle {\scriptstyle S}}  [{\scriptstyle S}]
      F  &#x22C5;  n   d S   {\displaystyle \mathbf {F} \cdot \mathbf {n} \,dS}
      [{\displaystyle \mathbf {F} \cdot \mathbf {n} \,dS}]
               =  &#x2A0C;  V    (     &#x2202;  F  u     &#x2202; u    +
      &#x2202;  F  x     &#x2202; x    +    &#x2202;  F  y     &#x2202; y    +
      &#x2202;  F  z     &#x2202; z     )   d V       =  &#x2A0C;  V
      (     &#x2202;  u  4     &#x2202; u    +    &#x2202;  x  5     &#x2202; x
      +    &#x2202;  y  6     &#x2202; y    +    &#x2202;  z  &#x2212; 3
      &#x2202; z     )   d V       =  &#x2A0C;  V      4  u  3    z  4   + 5  x
      4    z  4   + 5  y  4    z  4   &#x2212; 3   z  4      d V       =
      &#x2A0C;  V      4  u  3    z  4   + 5  x  4    z  4   + 5  y  4    z  4
      &#x2212; 3   z  4      d V       =  &#x222B;  0   1    &#x222B;  &#x2212;
      10   2 &#x03C0;    &#x222B;  4   5    &#x222B;  &#x2212; 1   3      4  u
      3    z  4   + 5  x  4    z  4   + 5  y  4    z  4   &#x2212; 3   z  4
      d V       =  &#x222B;  0   1    &#x222B;  &#x2212; 10   2 &#x03C0;
      &#x222B;  4   5    (    4 ( 3  u  4    z  3   + 3  y  6   + 91  z  3   +
      3 )   3  z  3      )   d y  d z  d u       =  &#x222B;  0   1    &#x222B;
      &#x2212; 10   2 &#x03C0;    (  4  u  4   +   743440 21   +   4  z  3
      )   d z  d u       =  &#x222B;  0   1    (  &#x2212;   1  2  &#x03C0;  2
      +    1486880 &#x03C0;  21   + 8 &#x03C0;  u  4   + 40  u  4   +
      371720021 1050    )   d u       =   371728421 1050   +    14869136
      &#x03C0;  3   &#x2212; 105   210  &#x03C0;  2            &#x2248;
      576468.77        {\displaystyle {\begin{aligned}&=\iiiint _{V}\left(
      {\frac {\partial F_{u}}{\partial u}}+{\frac {\partial F_{x}}{\partial
      x}}+{\frac {\partial F_{y}}{\partial y}}+{\frac {\partial F_{z}}{\partial
      z}}\right)\,dV\\&=\iiiint _{V}\left({\frac {\partial u^{4}}{\partial u}}+
      {\frac {\partial x^{5}}{\partial x}}+{\frac {\partial y^{6}}{\partial
      y}}+{\frac {\partial z^{-3}}{\partial z}}\right)\,dV\\&=\iiiint _{V}
      {\frac {4u^{3}z^{4}+5x^{4}z^{4}+5y^{4}z^{4}-3}{z^{4}}}\,dV\\&=\iiiint _
      {V}{\frac {4u^{3}z^{4}+5x^{4}z^{4}+5y^{4}z^{4}-3}{z^{4}}}\,dV\\&=\int _
      {0}^{1}\int _{-10}^{2\pi }\int _{4}^{5}\int _{-1}^{3}{\frac {4u^{3}z^
      {4}+5x^{4}z^{4}+5y^{4}z^{4}-3}{z^{4}}}\,dV\\&=\int _{0}^{1}\int _{-10}^
      {2\pi }\int _{4}^{5}\left({\frac {4(3u^{4}z^{3}+3y^{6}+91z^{3}+3)}{3z^
      {3}}}\right)\,dy\,dz\,du\\&=\int _{0}^{1}\int _{-10}^{2\pi }\left(4u^{4}+
      {\frac {743440}{21}}+{\frac {4}{z^{3}}}\right)\,dz\,du\\&=\int _{0}^
      {1}\left(-{\frac {1}{2\pi ^{2}}}+{\frac {1486880\pi }{21}}+8\pi u^
      {4}+40u^{4}+{\frac {371720021}{1050}}\right)\,du\\&={\frac {371728421}
      {1050}}+{\frac {14869136\pi ^{3}-105}{210\pi ^{2}}}\\&\approx
      {576468.77}\end{aligned}}}  [{\displaystyle {\begin{aligned}&=\iiiint _
      {V}\left({\frac {\partial F_{u}}{\partial u}}+{\frac {\partial F_{x}}
      {\partial x}}+{\frac {\partial F_{y}}{\partial y}}+{\frac {\partial F_
      {z}}{\partial z}}\right)\,dV\\&=\iiiint _{V}\left({\frac {\partial u^{4}}
      {\partial u}}+{\frac {\partial x^{5}}{\partial x}}+{\frac {\partial y^
      {6}}{\partial y}}+{\frac {\partial z^{-3}}{\partial
      z}}\right)\,dV\\&=\iiiint _{V}{\frac {4u^{3}z^{4}+5x^{4}z^{4}+5y^{4}z^
      {4}-3}{z^{4}}}\,dV\\&=\iiiint _{V}{\frac {4u^{3}z^{4}+5x^{4}z^{4}+5y^
      {4}z^{4}-3}{z^{4}}}\,dV\\&=\int _{0}^{1}\int _{-10}^{2\pi }\int _{4}^
      {5}\int _{-1}^{3}{\frac {4u^{3}z^{4}+5x^{4}z^{4}+5y^{4}z^{4}-3}{z^
      {4}}}\,dV\\&=\int _{0}^{1}\int _{-10}^{2\pi }\int _{4}^{5}\left({\frac {4
      (3u^{4}z^{3}+3y^{6}+91z^{3}+3)}{3z^{3}}}\right)\,dy\,dz\,du\\&=\int _{0}^
      {1}\int _{-10}^{2\pi }\left(4u^{4}+{\frac {743440}{21}}+{\frac {4}{z^
      {3}}}\right)\,dz\,du\\&=\int _{0}^{1}\left(-{\frac {1}{2\pi ^{2}}}+{\frac
      {1486880\pi }{21}}+8\pi u^{4}+40u^{4}+{\frac {371720021}
      {1050}}\right)\,du\\&={\frac {371728421}{1050}}+{\frac {14869136\pi ^{3}-
      105}{210\pi ^{2}}}\\&\approx {576468.77}\end{aligned}}}]
Thus, we can evaluate a contour integral of the fourth dimension.
***** Integral representation[edit] *****
[[icon]] This section needs expansion. You can help by adding_to_it. (November
         2013)
An integral representation of a function is an expression of the function
involving a contour integral. Various integral representations are known for
many special_functions. Integral representations can be important for
theoretical reasons, e.g. giving analytic_continuation or functional_equations,
or sometimes for numerical_evaluations.
Hankel's contour
For example, the original definition of the Riemann_zeta_function Î¶(s) via a
Dirichlet_series,
         &#x03B6; ( s ) =  &#x2211;  n = 1   &#x221E;     1  n  s     ,
      {\displaystyle \zeta (s)=\sum _{n=1}^{\infty }{\frac {1}{n^{s}}},}  [
      {\displaystyle \zeta (s)=\sum _{n=1}^{\infty }{\frac {1}{n^{s}}},}]
is valid only for Re(s) > 1. But
         &#x03B6; ( s ) = &#x2212;    &#x0393; ( 1 &#x2212; s )   2 &#x03C0; i
      &#x222B;  H      ( &#x2212; t  )  s &#x2212; 1      e  t   &#x2212; 1
      d t ,   {\displaystyle \zeta (s)=-{\frac {\Gamma (1-s)}{2\pi i}}\int _{H}
      {\frac {(-t)^{s-1}}{e^{t}-1}}dt,}  [{\displaystyle \zeta (s)=-{\frac
      {\Gamma (1-s)}{2\pi i}}\int _{H}{\frac {(-t)^{s-1}}{e^{t}-1}}dt,}]
where the integration is done over the Hankel_contour H, is valid for all
complex s not equal to 1.
***** See also[edit] *****
    * Residue_(complex_analysis)
    * Cauchy_principal_value
    * Poisson_integral
    * Pochhammer_contour
***** References[edit] *****
   1. ^Stalker, John (1998). Complex_Analysis:_Fundamentals_of_the_Classical
      Theory_of_Functions. Springer. p. 77. ISBN 0-8176-4038-X.
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
   3. ^Bak, Joseph; Newman, Donald J. (1997). "Chapters 11 & 12". Complex
      Analysis. Springer. pp. 130â156. ISBN 0-387-94756-6.
   4. ^Krantz, Steven George (1999). "Chapter 2". Handbook_of_Complex
      Variables. Springer. ISBN 0-8176-4011-8.
   5. ^MitrinoviÄ, Dragoslav S.; KeÄkiÄ, Jovan D. (1984). "Chapter 2". The
      Cauchy_Method_of_Residues:_Theory_and_Applications. Springer. ISBN 90-
      277-1623-4.
   6. ^MitrinoviÄ, Dragoslav S.; KeÄkiÄ, Jovan D. (1984). "Chapter 5". The
      Cauchy_Method_of_Residues:_Theory_and_Applications. ISBN 90-277-1623-4.
   7. ^ a b c d eSaff, Edward B.; Snider, Arthur David (2003). "Chapter 4".
      Fundamentals_of_Complex_Analysis_with_Applications_to_Engineering,
      Science,_and_Mathematics (3rd ed.). ISBN 0-1390-7874-6.
***** Further reading[edit] *****
    * Titchmarsh,_E._C. (1939), The Theory of Functions (2nd ed.), Oxford
      University Press, ISBN 0-19-853349-7
Jean Jacquelin, Marko Riedel, Branche_univalente[permanent_dead_link], Les-
Mathematiques.net, in French.
Marko Riedel et al., ProblÃ¨me_d'intÃ©grale, Les-Mathematiques.net, in French.
Marko Riedel et al., Integral_by_residue, math.stackexchange.com.
W W L Chen, Introduction_to_Complex_Analysis
Various authors, sin_lÃ­mites_ni_cotas, es.ciencia.matematicas, in Spanish.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Complex_integration,_method_of",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
    * v
    * t
    * e
Integrals
                          * Riemann_integral
                          * Lebesgue_integral
                          * Burkill_integral
                          * Bochner_integral
                          * Daniell_integral
                          * Darboux_integral
                          * HenstockâKurzweil_integral
Numerical_integration     * Haar_integral
                          * Hellinger_integral
                          * Khinchin_integral
                          * Kolmogorov_integral
                          * LebesgueâStieltjes_integral
                          * Pettis_integral
                          * Pfeffer_integral
                          * RiemannâStieltjes_integral
                          * Regulated_integral
                          * Integration_by_parts
                          * Integration_by_substitution
                          * Inverse_function_integration
                          * Order_of_integration_(calculus)
                          * trigonometric_substitution
Methods                   * Integration_by_partial_fractions
                          * Integration_by_reduction_formulae
                          * Integration_using_parametric_derivatives
                          * Integration_using_Euler's_formula
                          * Differentiation_under_the_integral_sign
                          * Contour integration
Improper Integrals        * Improper_integral
                          * Gaussian_integral
                          * ItÃ´_integral
Stochastic integrals      * RussoâVallois_integral
                          * Stratonovich_integral
                          * Skorokhod_integral

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Contour_integration&oldid=909275647"
Categories:
    * Complex_analysis
Hidden categories:
    * Articles_to_be_expanded_from_November_2013
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_August_2017
    * Articles_with_permanently_dead_external_links
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
    * ÙØ§Ø±Ø³Û
    * íêµ­ì´
    * Italiano
    * æ¥æ¬èª
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Svenska
    * TÃ¼rkÃ§e
Edit_links
    * This page was last edited on 4 August 2019, at 10:17 (UTC).
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
