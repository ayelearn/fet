The following text has been accessed from https://en.wikipedia.org/wiki/Lebesgue_integration at Fri Aug 9 02:34:00 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Lebesgue integration ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The integral of a positive function can be interpreted as the area under a
curve.
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
    * Lebesgue integration
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
In mathematics, the integral of a non-negative function of a single variable
can be regarded, in the simplest case, as the area between the graph of that
function and the x-axis. The Lebesgue integral extends the integral to a larger
class of functions. It also extends the domains on which these functions can be
defined.
Long before the 20th century, mathematicians already understood that for non-
negative functions with a smooth enough graphâsuch as continuous_functions on
closed bounded intervalsâthe area under the curve could be defined as the
integral, and computed using approximation techniques on the region by
polygons. However, as the need to consider more irregular functions
aroseâe.g., as a result of the limiting processes of mathematical_analysis
and the mathematical theory_of_probabilityâit became clear that more careful
approximation techniques were needed to define a suitable integral. Also, one
might wish to integrate on spaces more general than the real line. The Lebesgue
integral provides abstractions needed to do this important job.
The Lebesgue integral plays an important role in probability theory, real
analysis, and many other fields in the mathematical sciences. It is named after
Henri_Lebesgue (1875â1941), who introduced the integral (Lebesgue_1904). It
is also a pivotal part of the axiomatic_theory_of_probability.
The term Lebesgue integration can mean either the general theory of integration
of a function with respect to a general measure, as introduced by Lebesgue, or
the specific case of integration of a function defined on a sub-domain of the
real_line with respect to the Lebesgue_measure.
⁰
***** Contents *****
    * 1_Introduction
          o 1.1_Intuitive_interpretation
          o 1.2_Towards_a_formal_definition
    * 2_Construction
          o 2.1_Measure_theory
          o 2.2_Measurable_functions
          o 2.3_Constructing_the_integral
                # 2.3.1_Indicator_functions
                # 2.3.2_Simple_functions
                # 2.3.3_Non-negative_functions
                # 2.3.4_Signed_functions
                # 2.3.5_Complex_valued_functions
          o 2.4_Example
          o 2.5_Domain_of_integration
    * 3_Limitations_of_the_Riemann_integral
    * 4_Basic_theorems_of_the_Lebesgue_integral
    * 5_Proof_techniques
    * 6_Alternative_formulations
    * 7_Limitations_of_Lebesgue_integral
    * 8_See_also
    * 9_Notes
    * 10_References
***** Introduction[edit] *****
The integral of a positive function f between limits a and b can be interpreted
as the area under the graph of f. This is easy to understand for familiar
functions such as polynomials, but what does it mean for more exotic functions?
In general, for which class of functions does "area under the curve" make
sense? The answer to this question has great theoretical and practical
importance.
As part of a general movement toward rigor in mathematics in the nineteenth
century, mathematicians attempted to put integral calculus on a firm
foundation. The Riemann_integralâproposed by Bernhard_Riemann
(1826â1866)âis a broadly successful attempt to provide such a foundation.
Riemann's definition starts with the construction of a sequence of easily
calculated areas that converge to the integral of a given function. This
definition is successful in the sense that it gives the expected answer for
many already-solved problems, and gives useful results for many other problems.
However, Riemann integration does not interact well with taking limits of
sequences of functions, making such limiting processes difficult to analyze.
This is important, for instance, in the study of Fourier_series, Fourier
transforms, and other topics. The Lebesgue integral is better able to describe
how and when it is possible to take limits under the integral sign (via the
powerful monotone_convergence_theorem and dominated_convergence_theorem).
While the Riemann integral considers the area under a curve as made out of
vertical rectangles, the Lebesgue definition considers horizontal slabs that
are not necessarily just rectangles, and so it is more flexible. For this
reason, the Lebesgue definition makes it possible to calculate integrals for a
broader class of functions. For example, the Dirichlet_function, which is 0
where its argument is irrational and 1 otherwise, has a Lebesgue integral, but
does not have a Riemann integral. Furthermore, the Lebesgue integral of this
function is zero, which agrees with the intuition that when picking a real
number uniformly at random from the unit interval, the probability of picking a
rational number should be zero.
Lebesgue summarized his approach to integration in a letter to Paul_Montel:
     I have to pay a certain sum, which I have collected in my pocket. I
     take the bills and coins out of my pocket and give them to the
     creditor in the order I find them until I have reached the total sum.
     This is the Riemann integral. But I can proceed differently. After I
     have taken all the money out of my pocket I order the bills and coins
     according to identical values and then I pay the several heaps one
     after the other to the creditor. This is my integral.
     â Source: (Siegmund-Schultze_2008)
The insight is that one should be able to rearrange the values of a function
freely, while preserving the value of the integral. This process of
rearrangement can convert a very pathological_function into one that is "nice"
from the point of view of integration, and thus let such pathological functions
be integrated.
**** Intuitive interpretation[edit] ****
Riemann-Darboux's integration (in blue) and Lebesgue integration (in red).
To get some intuition about the different approaches to integration, let us
imagine that we want to find a mountain's volume (above sea level).
  The RiemannâDarboux approach
      Divide the base of the mountain into a grid of 1 meter squares. Measure
      the altitude of the mountain at the center of each square. The volume on
      a single grid square is approximately 1 m2 Ã (that square's altitude),
      so the total volume is 1 m2 times the sum of the altitudes.
  The Lebesgue approach
      Draw a contour_map of the mountain, where adjacent contours are 1 meter
      of altitude apart. The volume of earth a single contour contains is
      approximately 1 m Ã (that contour's area), so the total volume is the
      sum of these areas times 1 m.
Folland summarizes the difference between the Riemann and Lebesgue approaches
thus: "to compute the Riemann integral of f, one partitions the domain [a, b]
into subintervals", while in the Lebesgue integral, "one is in effect
partitioning the range of f ."[1]
**** Towards a formal definition[edit] ****
A measurable function is shown, together with the set     { x  |  f ( x ) > t }
{\displaystyle \{x|f(x)>t\}}  [{\displaystyle \{x|f(x)>t\}}] (on the x-axis).
The Lebesgue integral is obtained by slicing along the y-axis, using the 1-
dimensional Lebesgue measure to measure the "width" of the slices.
To define the Lebesgue integral requires the formal notion of a measure that,
roughly, associates to each set A of real numbers a nonnegative number Î¼(A)
representing the "size" of A. This notion of "size" should agree with the usual
length of an interval or disjoint union of intervals. Suppose that f : â â
â+ is a non-negative real-valued function. Using the "partitioning the range
of f " philosophy, the integral of f should be the sum over t of the elementary
area contained in the thin horizontal strip between y = t and y = t − dt. This
elementary area is just
         &#x03BC;  (  { x &#x2223; f ( x ) > t }  )   d t .   {\displaystyle
      \mu \left(\{x\mid f(x)>t\}\right)\,dt.}  [\mu \left(\{x\mid f
      (x)>t\}\right)\,dt.]
Let
          f  &#x2217;   ( t ) = &#x03BC;  (  { x &#x2223; f ( x ) > t }  )  .
      {\displaystyle f^{*}(t)=\mu \left(\{x\mid f(x)>t\}\right).}  [f^{*}
      (t)=\mu \left(\{x\mid f(x)>t\}\right).]
The Lebesgue integral of f is then defined by[2]
         &#x222B; f  d &#x03BC; =  &#x222B;  0   &#x221E;    f  &#x2217;   ( t
      )  d t   {\displaystyle \int f\,d\mu =\int _{0}^{\infty }f^{*}(t)\,dt}
      [\int f\,d\mu =\int _{0}^{\infty }f^{*}(t)\,dt]
where the integral on the right is an ordinary improper_Riemann_integral. Note
that fâ is a non-negative decreasing function, and therefore has a well-
defined improper Riemann integral with value in the interval [0,∞]. For a
suitable class of functions (the measurable_functions), this defines the
Lebesgue integral.
A general (not necessarily positive) measurable function f is Lebesgue
integrable if the area between the graph of f and the x-axis is finite:
         &#x222B;  |  f  |   d &#x03BC; < + &#x221E; .   {\displaystyle \int
      |f|\,d\mu <+\infty .}  [\int |f|\,d\mu <+\infty .]
In that case, as in the Riemannian case, the integral is the difference between
the area above the x-axis and the area below the x-axis:
         &#x222B; f  d &#x03BC; = &#x222B;  f  +    d &#x03BC; &#x2212;
      &#x222B;  f  &#x2212;    d &#x03BC;   {\displaystyle \int f\,d\mu =\int
      f^{+}\,d\mu -\int f^{-}\,d\mu }  [\int f\,d\mu =\int f^{+}\,d\mu -\int f^
      {-}\,d\mu ]
where     f =  f  +   &#x2212;  f  &#x2212;     {\displaystyle f=f^{+}-f^{-}}
[f=f^{+}-f^{-}] is the decomposition of f into the difference of two non-
negative functions given by
              f  +   ( x )    = max { f ( x ) , 0 }   =     {    f ( x ) ,
      if&#xA0;  f ( x ) > 0 ,     0 ,    otherwise             f  &#x2212;
      ( x )    = max { &#x2212; f ( x ) , 0 }   =     {    &#x2212; f ( x ) ,
      if&#xA0;  f ( x ) < 0 ,     0 ,    otherwise.              {\displaystyle
      {\begin{aligned}f^{+}(x)&=\max\{f(x),0\}&=&{\begin{cases}f(x),&{\text{if
      }}f(x)>0,\\0,&{\text{otherwise}}\end{cases}}\\f^{-}(x)&=\max\{-f
      (x),0\}&=&{\begin{cases}-f(x),&{\text{if }}f(x)<0,\\0,&{\text
      {otherwise.}}\end{cases}}\end{aligned}}}  [{\begin{aligned}f^{+}
      (x)&=\max\{f(x),0\}&=&{\begin{cases}f(x),&{\text{if }}f(x)>0,\\0,&{\text
      {otherwise}}\end{cases}}\\f^{-}(x)&=\max\{-f(x),0\}&=&{\begin{cases}-f
      (x),&{\text{if }}f(x)<0,\\0,&{\text{otherwise.}}\end{cases}}\end
      {aligned}}]
***** Construction[edit] *****
The theory of the Lebesgue integral requires a theory of measurable sets and
measures on these sets, as well as a theory of measurable functions and
integrals on these functions.
**** Measure theory[edit] ****
Further information: Measure_(mathematics)
Measure_theory was initially created to provide a useful abstraction of the
notion of length of subsets of the real lineâand, more generally, area and
volume of subsets of Euclidean spaces. In particular, it provided a systematic
answer to the question of which subsets of â have a length. As later set
theory developments showed (see non-measurable_set), it is actually impossible
to assign a length to all subsets of â in a way that preserves some natural
additivity and translation invariance properties. This suggests that picking
out a suitable class of measurable subsets is an essential prerequisite.
The Riemann integral uses the notion of length explicitly. Indeed, the element
of calculation for the Riemann integral is the rectangle [a, b] Ã [c, d],
whose area is calculated to be (b â a)(d â c). The quantity b â a is the
length of the base of the rectangle and d â c is the height of the rectangle.
Riemann could only use planar rectangles to approximate the area under the
curve, because there was no adequate theory for measuring more general sets.
In the development of the theory in most modern textbooks (after 1950), the
approach to measure and integration is axiomatic. This means that a measure is
any function Î¼ defined on a certain class Xâ of subsets of a set E, which
satisfies a certain list of properties. These properties can be shown to hold
in many different cases.
**** Measurable functions[edit] ****
We start with a measure_space (E, X, Î¼) where E is a set, X is a Ï-algebra of
subsets of E, and Î¼ is a (non-negative) measure on E defined on the sets of X.
For example, E can be Euclidean_n-space ân or some Lebesgue_measurable subset
of it, X is the Ï-algebra of all Lebesgue measurable subsets of E, and Î¼ is
the Lebesgue measure. In the mathematical theory of probability, we confine our
study to a probability measure Î¼, which satisfies Î¼(E) = 1.
Lebesgue's theory defines integrals for a class of functions called measurable
functions. A real-valued function f on E is measurable if the pre-image of
every interval of the form (t, â) is in X:
         { x  &#x2223;  f ( x ) > t } &#x2208; X  &#x2200; t &#x2208;  R  .
      {\displaystyle \{x\,\mid \,f(x)>t\}\in X\quad \forall t\in \mathbb {R} .}
      [{\displaystyle \{x\,\mid \,f(x)>t\}\in X\quad \forall t\in \mathbb {R}
      .}]
We can show that this is equivalent to requiring that the pre-image of any
Borel subset of â be in X. The set of measurable functions is closed under
algebraic operations, but more importantly it is closed under various kinds of
point-wise_sequential_limits:
          sup  k &#x2208;  N     f  k   ,   lim&#x2006;inf  k &#x2208;  N     f
      k   ,   lim&#x2006;sup  k &#x2208;  N     f  k     {\displaystyle \sup _
      {k\in \mathbb {N} }f_{k},\quad \liminf _{k\in \mathbb {N} }f_{k},\quad
      \limsup _{k\in \mathbb {N} }f_{k}}  [\sup _{k\in \mathbb {N} }f_{k},\quad
      \liminf _{k\in \mathbb {N} }f_{k},\quad \limsup _{k\in \mathbb {N} }f_
      {k}]
are measurable if the original sequence (fk)k, where k â â, consists of
measurable functions.
There are several approaches for defining an integral:
          &#x222B;  E   f  d &#x03BC; =  &#x222B;  E   f  ( x )   d &#x03BC;
      ( x )    {\displaystyle \int _{E}f\,d\mu =\int _{E}f\left(x\right)\,d\mu
      \left(x\right)}  [{\displaystyle \int _{E}f\,d\mu =\int _{E}f\left
      (x\right)\,d\mu \left(x\right)}]
for measurable real-valued functions f defined on E.
**** Constructing the integral[edit] ****
Approximating a function by simple functions.
One approach to constructing the Lebesgue integral is to make use of so-called
simple functions: finite real-linear combinations of indicator functions.
Simple functions can be used to approximate a measurable function, by
partitioning the range into layers. The integral of a simple function is equal
to the measure of a given layer, times the height of that layer. The integral
of a non-negative general measurable function is then defined as an appropriate
supremum of approximations by simple functions, and the integral of a (not
necessarily positive) measurable function is the difference of two integrals of
non-negative measurable functions, as mentioned earlier.
*** Indicator functions[edit] ***
To assign a value to the integral of the indicator_function 1S of a measurable
set S consistent with the given measure Î¼, the only reasonable choice is to
set:
         &#x222B;  1  S    d &#x03BC; = &#x03BC; ( S ) .   {\displaystyle \int
      1_{S}\,d\mu =\mu (S).}  [{\displaystyle \int 1_{S}\,d\mu =\mu (S).}]
Notice that the result may be equal to +â, unless Î¼ is a finite measure.
*** Simple functions[edit] ***
A finite linear_combination of indicator functions
          &#x2211;  k    a  k    1   S  k       {\displaystyle \sum _{k}a_{k}1_
      {S_{k}}}  [\sum _{k}a_{k}1_{S_{k}}]
where the coefficients ak are real numbers and the sets Sk are measurable, is
called a measurable simple_function. We extend the integral by linearity to
non-negative measurable simple functions. When the coefficients ak are non-
negative, we set
         &#x222B;  (   &#x2211;  k    a  k    1   S  k      )   d &#x03BC; =
      &#x2211;  k    a  k   &#x222B;  1   S  k      d &#x03BC; =  &#x2211;  k
      a  k    &#x03BC; (  S  k   ) .   {\displaystyle \int \left(\sum _{k}a_
      {k}1_{S_{k}}\right)\,d\mu =\sum _{k}a_{k}\int 1_{S_{k}}\,d\mu =\sum _
      {k}a_{k}\,\mu (S_{k}).}  [\int \left(\sum _{k}a_{k}1_{S_{k}}\right)\,d\mu
      =\sum _{k}a_{k}\int 1_{S_{k}}\,d\mu =\sum _{k}a_{k}\,\mu (S_{k}).]
The convention 0 Ã â = 0 must be used, and the result may be infinite. Even
if a simple function can be written in many ways as a linear combination of
indicator functions, the integral is always the same. This can be shown using
the additivity property of measures.
Some care is needed when defining the integral of a real-valued simple
function, to avoid the undefined expression â â â: one assumes that the
representation
         f =  &#x2211;  k    a  k    1   S  k       {\displaystyle f=\sum _
      {k}a_{k}1_{S_{k}}}  [f=\sum _{k}a_{k}1_{S_{k}}]
is such that Î¼(Sk) < â whenever ak â  0. Then the above formula for the
integral of f makes sense, and the result does not depend upon the particular
representation of f satisfying the assumptions.
If B is a measurable subset of E and s is a measurable simple function one
defines
          &#x222B;  B   s  d &#x03BC; = &#x222B;  1  B    s  d &#x03BC; =
      &#x2211;  k    a  k    &#x03BC; (  S  k   &#x2229; B ) .   {\displaystyle
      \int _{B}s\,d\mu =\int 1_{B}\,s\,d\mu =\sum _{k}a_{k}\,\mu (S_{k}\cap
      B).}  [\int _{B}s\,d\mu =\int 1_{B}\,s\,d\mu =\sum _{k}a_{k}\,\mu (S_
      {k}\cap B).]
*** Non-negative functions[edit] ***
Let f be a non-negative measurable function on E, which we allow to attain the
value +â, in other words, f takes non-negative values in the extended_real
number_line. We define
          &#x222B;  E   f  d &#x03BC; = sup  {    &#x222B;  E   s  d &#x03BC; :
      0 &#x2264; s &#x2264; f , &#xA0; s &#xA0;  simple    }  .
      {\displaystyle \int _{E}f\,d\mu =\sup \left\{\,\int _{E}s\,d\mu :0\leq
      s\leq f,\ s\ {\text{simple}}\,\right\}.}  [\int _{E}f\,d\mu =\sup \left\
      {\,\int _{E}s\,d\mu :0\leq s\leq f,\ s\ {\text{simple}}\,\right\}.]
We need to show this integral coincides with the preceding one, defined on the
set of simple functions, when Eâ is a segment [a, b]. There is also the
question of whether this corresponds in any way to a Riemann notion of
integration. It is possible to prove that the answer to both questions is yes.
We have defined the integral of f for any non-negative extended real-valued
measurable function on E. For some functions, this integralâ â«E f dÎ¼â is
infinite.
It is often useful to have a particular sequence of simple functions that
approximates the Lebesgue integral well (analogously to a Riemann sum). For a
non-negative measurable function f, let      s  n   ( x )   {\displaystyle s_
{n}(x)}  [{\displaystyle s_{n}(x)}] be the simple function whose value is     k
/   2  n     {\displaystyle k/2^{n}}  [{\displaystyle k/2^{n}}] whenever     k
/   2  n   &#x2264; f ( x ) < ( k + 1 )  /   2  n     {\displaystyle k/2^
{n}\leq f(x)<(k+1)/2^{n}}  [{\displaystyle k/2^{n}\leq f(x)<(k+1)/2^{n}}], for
k a non-negative integer less than (say)      4  n     {\displaystyle 4^{n}}
[4^{n}]. Then it can be proven directly that
         &#x222B; f  d &#x03BC; =  lim  n &#x2192; &#x221E;   &#x222B;  s  n
      d &#x03BC;   {\displaystyle \int f\,d\mu =\lim _{n\to \infty }\int s_
      {n}\,d\mu }  [{\displaystyle \int f\,d\mu =\lim _{n\to \infty }\int s_
      {n}\,d\mu }]
and that the limit on the right hand side exists as an extended real number.
This bridges the connection between the approach to the Lebesgue integral using
simple functions, and the motivation for the Lebesgue integral using a
partition of the range.
*** Signed functions[edit] ***
To handle signed functions, we need a few more definitions. If f is a
measurable function of the set E to the reals (including Â±â), then we can
write
         f =  f  +   &#x2212;  f  &#x2212;   ,    {\displaystyle f=f^{+}-f^{-
      },\quad }  [f=f^{+}-f^{-},\quad ]
where
          f  +   ( x ) =  {     f ( x )    if&#xA0;  f ( x ) > 0     0
      otherwise          {\displaystyle f^{+}(x)=\left\{{\begin{matrix}f(x)&
      {\text{if }}f(x)>0\\0&{\text{otherwise}}\end{matrix}}\right.}  [f^{+}
      (x)=\left\{{\begin{matrix}f(x)&{\text{if }}f(x)>0\\0&{\text
      {otherwise}}\end{matrix}}\right.]
          f  &#x2212;   ( x ) =  {     &#x2212; f ( x )    if&#xA0;  f ( x ) <
      0     0    otherwise          {\displaystyle f^{-}(x)=\left\{{\begin
      {matrix}-f(x)&{\text{if }}f(x)<0\\0&{\text{otherwise}}\end
      {matrix}}\right.}  [f^{-}(x)=\left\{{\begin{matrix}-f(x)&{\text{if }}f
      (x)<0\\0&{\text{otherwise}}\end{matrix}}\right.]
Note that both f+ and fâ are non-negative measurable functions. Also note
that
          |  f  |  =  f  +   +  f  &#x2212;   .    {\displaystyle |f|=f^{+}+f^
      {-}.\quad }  [|f|=f^{+}+f^{-}.\quad ]
We say that the Lebesgue integral of the measurable function f exists, or is
defined if at least one of     &#x222B;  f  +    d &#x03BC;   {\displaystyle
\int f^{+}\,d\mu }  [\int f^{+}\,d\mu ] and     &#x222B;  f  &#x2212;    d
&#x03BC;   {\displaystyle \int f^{-}\,d\mu }  [\int f^{-}\,d\mu ] is finite:
         min  (  &#x222B;  f  +    d &#x03BC; , &#x222B;  f  &#x2212;    d
      &#x03BC;  )  < &#x221E; .   {\displaystyle \min \left(\int f^{+}\,d\mu
      ,\int f^{-}\,d\mu \right)<\infty .}  [\min \left(\int f^{+}\,d\mu ,\int
      f^{-}\,d\mu \right)<\infty .]
In this case we define
         &#x222B; f  d &#x03BC; = &#x222B;  f  +    d &#x03BC; &#x2212;
      &#x222B;  f  &#x2212;    d &#x03BC; .   {\displaystyle \int f\,d\mu =\int
      f^{+}\,d\mu -\int f^{-}\,d\mu .}  [{\displaystyle \int f\,d\mu =\int f^
      {+}\,d\mu -\int f^{-}\,d\mu .}]
If
         &#x222B;  |  f  |   d &#x03BC; < &#x221E; ,   {\displaystyle \int
      |f|\,d\mu <\infty ,}  [\int |f|\,d\mu <\infty ,]
we say that f is Lebesgue integrable.
It turns out that this definition gives the desirable properties of the
integral.
*** Complex valued functions[edit] ***
Complex valued functions can be similarly integrated, by considering the real
part and the imaginary part separately.
If h=f+ig for real-valued integrable functions f, g, then the integral of h is
defined by
         &#x222B; h  d &#x03BC; = &#x222B; f  d &#x03BC; + i &#x222B; g  d
      &#x03BC; .   {\displaystyle \int h\,d\mu =\int f\,d\mu +i\int g\,d\mu .}
      [\int h\,d\mu =\int f\,d\mu +i\int g\,d\mu .]
The function is Lebesgue integrable if and only if its absolute_value is
Lebesgue integrable (see Absolutely_integrable_function).
**** Example[edit] ****
Consider the indicator_function of the rational numbers, 1Q. This function is
nowhere_continuous.
    *     1   Q      {\displaystyle 1_{\mathbf {Q} }}  [1_{\mathbf {Q} }] is
      not Riemann-integrable on [0, 1]: No matter how the set [0, 1] is
      partitioned into subintervals, each partition contains at least one
      rational and at least one irrational number, because rationals and
      irrationals are both dense in the reals. Thus the upper Darboux_sums are
      all one, and the lower Darboux sums are all zero.
    *     1   Q      {\displaystyle 1_{\mathbf {Q} }}  [1_{\mathbf {Q} }] is
      Lebesgue-integrable on [0, 1] using the Lebesgue_measure: Indeed, it is
      the indicator function of the rationals so by definition
                &#x222B;  [ 0 , 1 ]    1   Q     d &#x03BC; = &#x03BC; (  Q
            &#x2229; [ 0 , 1 ] ) = 0 ,   {\displaystyle \int _{[0,1]}1_{\mathbf
            {Q} }\,d\mu =\mu (\mathbf {Q} \cap [0,1])=0,}  [\int _{[0,1]}1_
            {\mathbf {Q} }\,d\mu =\mu (\mathbf {Q} \cap [0,1])=0,]
      because Q is countable.
**** Domain of integration[edit] ****
A technical issue in Lebesgue integration is that the domain of integration is
defined as a set (a subset of a measure space), with no notion of orientation.
In elementary calculus, one defines integration with respect to an orientation:
          &#x222B;  b   a   f := &#x2212;  &#x222B;  a   b   f .
      {\displaystyle \int _{b}^{a}f:=-\int _{a}^{b}f.}  [\int _{b}^{a}f:=-\int
      _{a}^{b}f.]
Generalizing this to higher dimensions yields integration of differential
forms. By contrast, Lebesgue integration provides an alternative
generalization, integrating over subsets with respect to a measure; this can be
notated as
          &#x222B;  A   f  d &#x03BC; =  &#x222B;  [ a , b ]   f  d &#x03BC;
      {\displaystyle \int _{A}f\,d\mu =\int _{[a,b]}f\,d\mu }  [\int _
      {A}f\,d\mu =\int _{[a,b]}f\,d\mu ]
to indicate integration over a subset A. For details on the relation between
these generalizations, see Differential_form_Â§ Relation_with_measures.
***** Limitations of the Riemann integral[edit] *****
Here we discuss the limitations of the Riemann integral and the greater scope
offered by the Lebesgue integral. This discussion presumes a working
understanding of the Riemann_integral.
With the advent of Fourier_series, many analytical problems involving integrals
came up whose satisfactory solution required interchanging limit processes and
integral signs. However, the conditions under which the integrals
          &#x2211;  k   &#x222B;  f  k   ( x ) d x ,  &#x222B;  [   &#x2211;  k
      f  k   ( x )  ]  d x   {\displaystyle \sum _{k}\int f_{k}(x)dx,\quad \int
      \left[\sum _{k}f_{k}(x)\right]dx}  [\sum _{k}\int f_{k}(x)dx,\quad \int
      \left[\sum _{k}f_{k}(x)\right]dx]
are equal proved quite elusive in the Riemann framework. There are some other
technical difficulties with the Riemann integral. These are linked with the
limit-taking difficulty discussed above.
Failure of monotone convergence. As shown above, the indicator_function 1Q on
the rationals is not Riemann integrable. In particular, the Monotone
convergence_theorem fails. To see why, let {ak} be an enumeration of all the
rational numbers in [0, 1] (they are countable so this can be done.) Then let
          g  k   ( x ) =  {     1    if&#xA0;  x =  a  j   , j &#x2264; k     0
      otherwise          {\displaystyle g_{k}(x)=\left\{{\begin{matrix}1&{\text
      {if }}x=a_{j},j\leq k\\0&{\text{otherwise}}\end{matrix}}\right.}  [g_{k}
      (x)=\left\{{\begin{matrix}1&{\text{if }}x=a_{j},j\leq k\\0&{\text
      {otherwise}}\end{matrix}}\right.]
The function gk is zero everywhere, except on a finite set of points. Hence its
Riemann integral is zero. Each gk is non-negative, and this sequence of
functions is monotonically increasing, but its limit as k â â is 1Q, which
is not Riemann integrable.
Unsuitability for unbounded intervals. The Riemann integral can only integrate
functions on a bounded interval. It can however be extended to unbounded
intervals by taking limits, so long as this doesn't yield an answer such as â
â â.
Integrating on structures other than Euclidean space. The Riemann integral is
inextricably linked to the order structure of the real line.
***** Basic theorems of the Lebesgue integral[edit] *****
The Lebesgue integral has the following properties:
Equivalence_relation of equality almost-everywhere: The Lebesgue integral does
not distinguish between functions that differ only on a set of Î¼-measure zero.
To make this precise, functions f and g are said to be equal almost everywhere
(a.e.) if
         &#x03BC; ( { x &#x2208; E : f ( x ) &#x2260; g ( x ) } ) = 0.
      {\displaystyle \mu (\{x\in E:f(x)\neq g(x)\})=0.}  [\mu (\{x\in E:f
      (x)\neq g(x)\})=0.]
    * If f, g are non-negative measurable functions (possibly assuming the
      value +â) such that f = g almost everywhere, then
         &#x222B; f  d &#x03BC; = &#x222B; g  d &#x03BC; .   {\displaystyle
      \int f\,d\mu =\int g\,d\mu .}  [\int f\,d\mu =\int g\,d\mu .]
To wit, the integral respects the equivalence relation of almost-everywhere
equality.
    * If f, g are functions such that f = g almost everywhere, then f is
      Lebesgue integrable if and only if g is Lebesgue integrable, and the
      integrals of f and g are the same if they exist.
Linearity: If f and g are Lebesgue integrable functions and a and b are real
numbers, then af + bg is Lebesgue integrable and
         &#x222B; ( a f + b g )  d &#x03BC; = a &#x222B; f  d &#x03BC; + b
      &#x222B; g  d &#x03BC; .   {\displaystyle \int (af+bg)\,d\mu =a\int
      f\,d\mu +b\int g\,d\mu .}  [\int (af+bg)\,d\mu =a\int f\,d\mu +b\int
      g\,d\mu .]
Monotonicity: If f â¤ g, then
         &#x222B; f  d &#x03BC; &#x2264; &#x222B; g  d &#x03BC; .
      {\displaystyle \int f\,d\mu \leq \int g\,d\mu .}  [\int f\,d\mu \leq \int
      g\,d\mu .]
Monotone_convergence_theorem: Suppose { fk}k â â is a sequence of non-
negative measurable functions such that
          f  k   ( x ) &#x2264;  f  k + 1   ( x )  &#x2200; k &#x2208;  N  ,
      &#x2200; x &#x2208; E .   {\displaystyle f_{k}(x)\leq f_{k+1}(x)\quad
      \forall k\in \mathbb {N} ,\,\forall x\in E.}  [f_{k}(x)\leq f_{k+1}
      (x)\quad \forall k\in \mathbb {N} ,\,\forall x\in E.]
Then, the pointwise limit f of fk is Lebesgue measurable and
          lim  k   &#x222B;  f  k    d &#x03BC; = &#x222B; f  d &#x03BC; .
      {\displaystyle \lim _{k}\int f_{k}\,d\mu =\int f\,d\mu .}  [
      {\displaystyle \lim _{k}\int f_{k}\,d\mu =\int f\,d\mu .}]
The value of any of the integrals is allowed to be infinite.
Fatou's_lemma: If { fk}k â N is a sequence of non-negative measurable
functions, then
         &#x222B;  lim&#x2006;inf  k    f  k    d &#x03BC; &#x2264;
      lim&#x2006;inf  k   &#x222B;  f  k    d &#x03BC; .   {\displaystyle \int
      \liminf _{k}f_{k}\,d\mu \leq \liminf _{k}\int f_{k}\,d\mu .}  [\int
      \liminf _{k}f_{k}\,d\mu \leq \liminf _{k}\int f_{k}\,d\mu .]
Again, the value of any of the integrals may be infinite.
Dominated_convergence_theorem: Suppose { fk}k â N is a sequence of complex
measurable functions with pointwise limit f, and there is a Lebesgue integrable
function g (i.e., g belongs to the space_L1) such that | fk | â¤ g for all k.
Then, f is Lebesgue integrable and
          lim  k   &#x222B;  f  k    d &#x03BC; = &#x222B; f  d &#x03BC; .
      {\displaystyle \lim _{k}\int f_{k}\,d\mu =\int f\,d\mu .}  [\lim _{k}\int
      f_{k}\,d\mu =\int f\,d\mu .]
***** Proof techniques[edit] *****
To illustrate some of the proof techniques used in Lebesgue integration theory,
we sketch a proof of the above-mentioned Lebesgue monotone convergence theorem.
Let { fk}k â N be a non-decreasing sequence of non-negative measurable
functions and put
         f =  sup  k &#x2208;  N     f  k   =  lim  k &#x2208;  N     f  k   .
      {\displaystyle f=\sup _{k\in \mathbb {N} }f_{k}=\lim _{k\in \mathbb {N}
      }f_{k}.}  [f=\sup _{k\in \mathbb {N} }f_{k}=\lim _{k\in \mathbb {N} }f_
      {k}.]
By the monotonicity property of the integral, it is immediate that:
         &#x222B; f  d &#x03BC; &#x2265;  lim  k   &#x222B;  f  k    d &#x03BC;
      {\displaystyle \int f\,d\mu \geq \lim _{k}\int f_{k}\,d\mu }  [
      {\displaystyle \int f\,d\mu \geq \lim _{k}\int f_{k}\,d\mu }]
and the limit on the right exists, because the sequence is monotonic. We now
prove the inequality in the other direction. It follows from the definition of
integral that there is a non-decreasing sequence (gn) of non-negative simple
functions such that gn â¤ fâ and
          lim  n   &#x222B;  g  n    d &#x03BC; = &#x222B; f  d &#x03BC; .
      {\displaystyle \lim _{n}\int g_{n}\,d\mu =\int f\,d\mu .}  [
      {\displaystyle \lim _{n}\int g_{n}\,d\mu =\int f\,d\mu .}]
Therefore, it suffices to prove that for each n â â,
         &#x222B;  g  n    d &#x03BC; &#x2264;  lim  k   &#x222B;  f  k    d
      &#x03BC; .   {\displaystyle \int g_{n}\,d\mu \leq \lim _{k}\int f_
      {k}\,d\mu .}  [{\displaystyle \int g_{n}\,d\mu \leq \lim _{k}\int f_
      {k}\,d\mu .}]
We will show that if g is a simple function and
          lim  k    f  k   ( x ) &#x2265; g ( x )   {\displaystyle \lim _{k}f_
      {k}(x)\geq g(x)}  [\lim _{k}f_{k}(x)\geq g(x)]
almost everywhere, then
          lim  k   &#x222B;  f  k    d &#x03BC; &#x2265; &#x222B; g  d &#x03BC;
      .   {\displaystyle \lim _{k}\int f_{k}\,d\mu \geq \int g\,d\mu .}  [
      {\displaystyle \lim _{k}\int f_{k}\,d\mu \geq \int g\,d\mu .}]
By breaking up the function g into its constant value parts, this reduces to
the case in which g is the indicator function of a set. The result we have to
prove is then
     Suppose A is a measurable set and { fk}k â â is a nondecreasing
     sequence of non-negative measurable functions on E such that
               lim  k    f  k   ( x ) &#x2265; 1   {\displaystyle \lim _
           {k}f_{k}(x)\geq 1}  [\lim _{k}f_{k}(x)\geq 1]
     for almost all x â A. Then
               lim  k   &#x222B;  f  k    d &#x03BC; &#x2265; &#x03BC; ( A
           ) .   {\displaystyle \lim _{k}\int f_{k}\,d\mu \geq \mu (A).}
           [\lim _{k}\int f_{k}\,d\mu \geq \mu (A).]
To prove this result, fix Îµ > 0 and define the sequence of measurable sets
          B  k   = { x &#x2208; A :  f  k   ( x ) &#x2265; 1 &#x2212; &#x03B5;
      } .   {\displaystyle B_{k}=\{x\in A:f_{k}(x)\geq 1-\varepsilon \}.}  [B_
      {k}=\{x\in A:f_{k}(x)\geq 1-\varepsilon \}.]
By monotonicity of the integral, it follows that for any k â â,
         ( 1 &#x2212; &#x03B5; ) &#x03BC; (  B  k   ) = &#x222B; ( 1 &#x2212;
      &#x03B5; )  1   B  k      d &#x03BC; &#x2264; &#x222B;  f  k    d
      &#x03BC;   {\displaystyle (1-\varepsilon )\mu (B_{k})=\int (1-\varepsilon
      )1_{B_{k}}\,d\mu \leq \int f_{k}\,d\mu }  [{\displaystyle (1-\varepsilon
      )\mu (B_{k})=\int (1-\varepsilon )1_{B_{k}}\,d\mu \leq \int f_{k}\,d\mu
      }]
Because almost every x is in Bk for large enough k, we have
          &#x22C3;  k    B  k   = A ,   {\displaystyle \bigcup _{k}B_{k}=A,}
      [\bigcup _{k}B_{k}=A,]
up to a set of measure 0. Thus by countable additivity of Î¼, and because Bk
increases with k,
         &#x03BC; ( A ) =  lim  k   &#x03BC; (  B  k   ) &#x2264;  lim  k   ( 1
      &#x2212; &#x03B5;  )  &#x2212; 1   &#x222B;  f  k    d &#x03BC; .
      {\displaystyle \mu (A)=\lim _{k}\mu (B_{k})\leq \lim _{k}(1-\varepsilon
      )^{-1}\int f_{k}\,d\mu .}  [{\displaystyle \mu (A)=\lim _{k}\mu (B_
      {k})\leq \lim _{k}(1-\varepsilon )^{-1}\int f_{k}\,d\mu .}]
As this is true for any positive Îµ the result follows.
For another Proof of the Monotone Convergence Theorem, we follow:[1]
Let (X, M, Î¼) be a measure space.
{ fn} is an increasing sequence of numbers, therefore its limit exists, even if
it is equal to â. We know that
         &#x222B;  f  n   &#x2264; &#x222B; f   {\displaystyle \int f_{n}\leq
      \int f}  [\int f_{n}\leq \int f]
for all n, so that
          lim  n &#x2192; &#x221E;   &#x222B;  f  n   &#x2264; &#x222B; f
      {\displaystyle \lim \limits _{n\rightarrow \infty }\int f_{n}\leq \int f}
      [\lim \limits _{n\rightarrow \infty }\int f_{n}\leq \int f].
Now we need to establish the reverse inequality. Fix Î± â (0, 1), let Ï be a
simple function with 0 â¤ Ï â¤ f and let
          E  n   = { x :  f  n   ( x ) &#x2265; &#x03B1; &#x03D5; ( x ) }
      {\displaystyle E_{n}=\{x:f_{n}(x)\geq \alpha \phi (x)\}}  [E_{n}=\{x:f_
      {n}(x)\geq \alpha \phi (x)\}].
Then {En} is an increasing sequence of measurable sets with      &#x22C3;
&#x221E;    E  n   = X   {\displaystyle \bigcup \limits ^{\infty }E_{n}=X}
[\bigcup \limits ^{\infty }E_{n}=X]. We know that
         &#x222B;  f  n   &#x2265;  &#x222B;   E  n      f  n   &#x2265;
      &#x03B1;  &#x222B;   E  n     &#x03D5;   {\displaystyle \int f_{n}\geq
      \int \limits _{E_{n}}f_{n}\geq \alpha \int \limits _{E_{n}}\phi }  [\int
      f_{n}\geq \int \limits _{E_{n}}f_{n}\geq \alpha \int \limits _{E_{n}}\phi
      ].
This is true for all n, including the limit:
         lim  &#x222B;   E  n     &#x03D5; = &#x222B; &#x03D5;   {\displaystyle
      \lim \int \limits _{E_{n}}\phi =\int \phi }  [\lim \int \limits _{E_
      {n}}\phi =\int \phi ].
Hence,
         lim &#x222B;  f  n   &#x2265; &#x03B1; &#x222B; &#x03D5;
      {\displaystyle \lim \int f_{n}\geq \alpha \int \phi }  [\lim \int f_
      {n}\geq \alpha \int \phi ].
This was true for all Î± â (0, 1), so it remains true for Î± = 1, and taking
the supremum over simple Ï â¤ f by the definition of integration in L+,
         lim &#x222B;  f  n   &#x2265; &#x222B; f   {\displaystyle \lim \int f_
      {n}\geq \int f}  [\lim \int f_{n}\geq \int f].
Now we have both inequalities, so we've shown the Monotone Convergence theorem:
         lim &#x222B;  f  n   = &#x222B; f   {\displaystyle \lim \int f_
      {n}=\int f}  [\lim \int f_{n}=\int f]
for f{n+1} â¥ fn, and fn â f pointwise, {fn} â L+, the set of positive
measurable functions from X â [0, â].
***** Alternative formulations[edit] *****
It is possible to develop the integral with respect to the Lebesgue measure
without relying on the full machinery of measure theory. One such approach is
provided by the Daniell_integral.
There is also an alternative approach to developing the theory of integration
via methods of functional_analysis. The Riemann integral exists for any
continuous function f of compact support defined on ân (or a fixed open
subset). Integrals of more general functions can be built starting from these
integrals.
Let Cc be the space of all real-valued compactly supported continuous functions
of â. Define a norm on Cc by
          &#x2016; f &#x2016;  = &#x222B;  |  f ( x )  |   d x .
      {\displaystyle \left\|f\right\|=\int |f(x)|\,dx.}  [{\displaystyle
      \left\|f\right\|=\int |f(x)|\,dx.}]
Then Cc is a normed vector space (and in particular, it is a metric space.) All
metric spaces have Hausdorff_completions, so let L1 be its completion. This
space is isomorphic to the space of Lebesgue integrable functions modulo the
subspace of functions with integral zero. Furthermore, the Riemann integral â«
is a uniformly_continuous functional with respect to the norm on Cc, which is
dense in L1. Hence â« has a unique extension to all of L1. This integral is
precisely the Lebesgue integral.
More generally, when the measure space on which the functions are defined is
also a locally_compact topological_space (as is the case with the real numbers
â), measures compatible with the topology in a suitable sense (Radon
measures, of which the Lebesgue measure is an example) an integral with respect
to them can be defined in the same manner, starting from the integrals of
continuous_functions with compact_support. More precisely, the compactly
supported functions form a vector_space that carries a natural topology, and a
(Radon) measure is defined as a continuous linear functional on this space. The
value of a measure at a compactly supported function is then also by definition
the integral of the function. One then proceeds to expand the measure (the
integral) to more general functions by continuity, and defines the measure of a
set as the integral of its indicator function. This is the approach taken by
Bourbaki_(2004) and a certain number of other authors. For details see Radon
measures.
***** Limitations of Lebesgue integral[edit] *****
The main purpose of the Lebesgue integral is to provide an integral notion
where limits of integrals hold under mild assumptions. There is no guarantee
that every function is Lebesgue integrable. But it may happen that improper
integrals exist for functions that are not Lebesgue integrable. One example
would be
      ______sin_&#x2061;_(_x_)__x_____{\displaystyle_{\frac_{\sin(x)}{x}}}__[
      {\frac_{\sin(x)}{x}}]
over the entire real line. This function is not Lebesgue integrable, as
          &#x222B;  &#x2212; &#x221E;   &#x221E;    |    sin &#x2061; ( x )  x
      |  d x = &#x221E; .   {\displaystyle \int _{-\infty }^{\infty }\left|
      {\frac {\sin(x)}{x}}\right|dx=\infty .}  [{\displaystyle \int _{-\infty
      }^{\infty }\left|{\frac {\sin(x)}{x}}\right|dx=\infty .}]
On the other hand,      &#x222B;  &#x2212; &#x221E;   &#x221E;      sin
&#x2061; ( x )  x   d x   {\displaystyle \int _{-\infty }^{\infty }{\frac {\sin
(x)}{x}}dx}  [{\displaystyle \int _{-\infty }^{\infty }{\frac {\sin(x)}{x}}dx}]
exists as an improper integral and can be computed to be finite; it is twice
the Dirichlet_integral.
***** See also[edit] *****
    * Henri_Lebesgue, for a non-technical description of Lebesgue integration
    * Null_set
    * Integration
    * Measure
    * Sigma-algebra
    * Lebesgue_space
    * LebesgueâStieltjes_integration
    * HenstockâKurzweil_integral
***** Notes[edit] *****
   1. ^ a bFolland, Gerald B. (1984). Real_Analysis:_Modern_Techniques_and
      Their_Applications. Wiley. p. 56.
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
   3. ^ Lieb_&_Loss_2001
***** References[edit] *****
    * Bartle, Robert G. (1995). The elements of integration and Lebesgue
      measure. Wiley Classics Library. New York: John Wiley & Sons Inc.
      xii+179. ISBN 0-471-04222-6. MR 1312157.
    * Bauer, Heinz (2001). Measure and Integration Theory. De Gruyter Studies
      in Mathematics 26. Berlin: De Gruyter. 236. ISBN 978-3-11-016719-1.
    * Bourbaki,_Nicolas (2004). Integration. I. Chapters 1â6. Translated from
      the 1959, 1965 and 1967 French originals by Sterling K. Berberian.
      Elements of Mathematics (Berlin). Berlin: Springer-Verlag. xvi+472.
      ISBN 3-540-41129-1. MR 2018901.
    * Dudley, Richard M. (1989). Real analysis and probability. The Wadsworth &
      Brooks/Cole Mathematics Series. Pacific Grove, CA: Wadsworth & Brooks/
      Cole Advanced Books & Software. xii+436. ISBN 0-534-10050-3. MR 0982264.
 Very thorough treatment, particularly for probabilists with good notes and
historical references.
    * Folland, Gerald B. (1999). Real analysis: Modern techniques and their
      applications. Pure and Applied Mathematics (New York) (Second ed.). New
      York: John Wiley & Sons Inc. xvi+386. ISBN 0-471-31716-0. MR 1681462.
    * Halmos,_Paul_R. (1950). Measure Theory. New York, N. Y.: D. Van Nostrand
      Company, Inc. pp. xi+304. MR 0033869.
 A classic, though somewhat dated presentation.
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Lebesgue_integral", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Lebesgue,_Henri (1904). "LeÃ§ons sur l'intÃ©gration et la recherche des
fonctions primitives". Paris: Gauthier-Villars.
    * Lebesgue,_Henri (1972). Oeuvres scientifiques (en cinq volumes) (in
      French). Geneva: Institut de MathÃ©matiques de l'UniversitÃ© de GenÃ¨ve.
      p. 405. MR 0389523.
    * Lieb,_Elliott; Loss,_Michael (2001). Analysis. Graduate_Studies_in
      Mathematics. 14 (2nd ed.). American_Mathematical_Society. ISBN 978-
      0821827833.
Loomis, Lynn H. (1953). An introduction to abstract harmonic analysis. Toronto-
New York-London: D. Van Nostrand Company, Inc. pp. x+190. MR 0054173.
 Includes a presentation of the Daniell integral.
    * Munroe, M. E. (1953). Introduction to measure and integration. Cambridge,
      Mass.: Addison-Wesley Publishing Company Inc. pp. x+310. MR 0053186.
 Good treatment of the theory of outer measures.
    * Royden, H. L. (1988). Real analysis (Third ed.). New York: Macmillan
      Publishing Company. pp. xx+444. ISBN 0-02-404151-3. MR 1013117.
    * Rudin,_Walter (1976). Principles of mathematical analysis. International
      Series in Pure and Applied Mathematics (Third ed.). New York: McGraw-Hill
      Book Co. pp. x+342. MR 0385023.
 Known as Little Rudin, contains the basics of the Lebesgue theory, but does
not treat material such as Fubini's_theorem.
    * Rudin, Walter (1966). Real and complex analysis. New York: McGraw-Hill
      Book Co. pp. xi+412. MR 0210528.
 Known as Big Rudin. A complete and careful presentation of the theory. Good
presentation of the Riesz extension theorems. However, there is a minor flaw
(in the first edition) in the proof of one of the extension theorems, the
discovery of which constitutes exercise 21 of Chapter 2.
Saks,_StanisÅaw (1937). "Theory_of_the_Integral". Monografie_Matematyczne. 7
(2nd ed.). Warszawa-LwÃ³w: G.E. Stechert & Co.: VI+347. JFM 63.0183.05.
Zbl 0017.30004.
. English translation by Laurence_Chisholm_Young, with two additional notes by
Stefan_Banach.
    * Shilov, G. E.; Gurevich, B. L. (1977). Integral, measure and derivative:
      a unified approach. Translated from the Russian and edited by Richard A.
      Silverman. Dover Books on Advanced Mathematics. New York: Dover
      Publications Inc. xiv+233. ISBN 0-486-63519-8. MR 0466463.
 Emphasizes the Daniell_integral.
    * Siegmund-Schultze, Reinhard (2008), "Henri Lebesgue", in Timothy Gowers,
      June Barrow-Green, Imre Leader (eds.), Princeton Companion to
      Mathematics, Princeton University PressCS1 maint: Uses editors parameter
      (link)
.
Teschl,_Gerald. Topics_in_Real_and_Functional_Analysis. (lecture notes).
    * Yeh, James (2006). Real Analysis: Theory of Measure and Integral 2nd.
      Edition Paperback. Singapore: World Scientific Publishing Company Pte.
      Ltd. p. 760. ISBN 978-981-256-6.
    * v
    * t
    * e
Integrals
                          * Riemann_integral
                          * Lebesgue integral
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
                          * Contour_integration
Improper Integrals        * Improper_integral
                          * Gaussian_integral
                          * ItÃ´_integral
Stochastic integrals      * RussoâVallois_integral
                          * Stratonovich_integral
                          * Skorokhod_integral
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh94008345
                                              * NDL: 00567363

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Lebesgue_integration&oldid=892240081"
Categories:
    * Definitions_of_mathematical_integration
    * Measure_theory
Hidden categories:
    * CS1_French-language_sources_(fr)
    * CS1_maint:_Uses_editors_parameter
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Basa_Sunda
    * Suomi
    * Svenska
    * Tagalog
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 13 April 2019, at 04:01 (UTC).
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
