The following text has been accessed from https://en.wikipedia.org/wiki/Riemann_integral at Fri Aug 9 02:35:37 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Riemann integral ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Basic type of integral in elementary calculus
The integral as the area of a region under a curve.
A sequence of Riemann sums over a regular partition of an interval. The number
on top is the total area of the rectangles, which converges to the integral of
the function.
The partition does not need to be regular, as shown here. The approximation
works as long as the width of each subdivision tends to zero.
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
    * Riemann integral
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
In the branch of mathematics known as real_analysis, the Riemann integral,
created by Bernhard_Riemann, was the first rigorous definition of the integral
of a function on an interval. It was presented to the faculty at the University
of_GÃ¶ttingen in 1854, but not published in a journal until 1868.[1] For many
functions and practical applications, the Riemann integral can be evaluated by
the fundamental_theorem_of_calculus or approximated by numerical_integration.
The Riemann integral is unsuitable for many theoretical purposes. Some of the
technical deficiencies in Riemann integration can be remedied with the
RiemannâStieltjes_integral, and most disappear with the Lebesgue_integral.
⁰
***** Contents *****
    * 1_Overview
    * 2_Definition
          o 2.1_Partitions_of_an_interval
          o 2.2_Riemann_sums
          o 2.3_Riemann_integral
    * 3_Examples
    * 4_Similar_concepts
    * 5_Properties
          o 5.1_Linearity
    * 6_Integrability
    * 7_Generalizations
    * 8_See_also
    * 9_Notes
    * 10_References
    * 11_External_links
***** Overview[edit] *****
Let f be a non-negative real-valued function on the interval [a, b], and let
         S =  {  ( x , y )  : &#xA0; a &#x2264; x &#x2264; b , 0 < y < f ( x )
      }    {\displaystyle S=\left\{(x,y)\,:\ a\leq x\leq b,0<y<f(x)\right\}}
      [S = \left \{ (x, y) \, : \ a \leq x \leq b, 0 < y < f(x) \right \}]
be the region of the plane under the graph of the function f and above the
interval [a, b] (see the figure on the top right). We are interested in
measuring the area of S. Once we have measured it, we will denote the area by:
          &#x222B;  a   b   f ( x )  d x .   {\displaystyle \int _{a}^{b}f
      (x)\,dx.}  [\int_{a}^{b}f(x)\,dx.]
The basic idea of the Riemann integral is to use very simple approximations for
the area of S. By taking better and better approximations, we can say that "in
the limit" we get exactly the area of S under the curve.
Note that where f can be both positive and negative, the definition of S is
modified so that the integral corresponds to the signed area under the graph of
f: that is, the area above the x-axis minus the area below the x-axis.
***** Definition[edit] *****
**** Partitions of an interval[edit] ****
A partition_of_an_interval [a, b] is a finite sequence of numbers of the form
         a =  x  0   <  x  1   <  x  2   < &#x22EF; <  x  n   = b
      {\displaystyle a=x_{0}<x_{1}<x_{2}<\dots <x_{n}=b}  [{\displaystyle a=x_
      {0}<x_{1}<x_{2}<\dots <x_{n}=b}]
Each [xi, xi + 1] is called a sub-interval of the partition. The mesh or norm
of a partition is defined to be the length of the longest sub-interval, that
is,
         max  (   x  i + 1   &#x2212;  x  i    )  ,  i &#x2208; [ 0 , n
      &#x2212; 1 ] .   {\displaystyle \max \left(x_{i+1}-x_{i}\right),\quad
      i\in [0,n-1].}  [{\displaystyle \max \left(x_{i+1}-x_{i}\right),\quad
      i\in [0,n-1].}]
A tagged partition P(x, t) of an interval [a, b] is a partition together with a
finite sequence of numbers t0, ..., tn â 1 subject to the conditions that for
each i, ti â [xi, xi + 1]. In other words, it is a partition together with a
distinguished point of every sub-interval. The mesh of a tagged partition is
the same as that of an ordinary partition.
Suppose that two partitions P(x, t) and Q(y, s) are both partitions of the
interval [a, b]. We say that Q(y, s) is a refinement of P(x, t) if for each
integer i, with i â [0, n], there exists an integer r(i) such that xi = yr(i)
and such that ti = sj for some j with j â [r(i), r(i + 1)). Said more simply,
a refinement of a tagged partition breaks up some of the sub-intervals and adds
tags to the partition where necessary, thus it "refines" the accuracy of the
partition.
We can define a partial_order on the set of all tagged partitions by saying
that one tagged partition is greater or equal to another if the former is a
refinement of the latter.
**** Riemann sums[edit] ****
Let f be a real-valued function defined on the interval [a, b]. The Riemann_sum
of f with respect to the tagged partition x0, ..., xn together with t0, ..., tn
â 1 is[2]
          &#x2211;  i = 0   n &#x2212; 1   f (  t  i   )  (   x  i + 1
      &#x2212;  x  i    )  .   {\displaystyle \sum _{i=0}^{n-1}f(t_{i})\left(x_
      {i+1}-x_{i}\right).}  [{\displaystyle \sum _{i=0}^{n-1}f(t_{i})\left(x_
      {i+1}-x_{i}\right).}]
Each term in the sum is the product of the value of the function at a given
point and the length of an interval. Consequently, each term represents the
(signed) area of a rectangle with height f(ti) and width xi + 1 â xi. The
Riemann sum is the (signed) area of all the rectangles.
A closely related concept are the lower and upper Darboux sums. These are
similar to Riemann sums, but the tags are replaced by the infimum_and_supremum
(respectively) of f on each sub-interval:
             L ( f , P )    =  &#x2211;  i = 0   n &#x2212; 1    inf  t
      &#x2208; [  x  i   ,  x  i + 1   ]   f ( t ) (  x  i + 1   &#x2212;  x  i
      ) ,     U ( f , P )    =  &#x2211;  i = 0   n &#x2212; 1    sup  t
      &#x2208; [  x  i   ,  x  i + 1   ]   f ( t ) (  x  i + 1   &#x2212;  x  i
      ) .       {\displaystyle {\begin{aligned}L(f,P)&=\sum _{i=0}^{n-1}\inf _
      {t\in [x_{i},x_{i+1}]}f(t)(x_{i+1}-x_{i}),\\U(f,P)&=\sum _{i=0}^{n-1}\sup
      _{t\in [x_{i},x_{i+1}]}f(t)(x_{i+1}-x_{i}).\end{aligned}}}  [
      {\displaystyle {\begin{aligned}L(f,P)&=\sum _{i=0}^{n-1}\inf _{t\in [x_
      {i},x_{i+1}]}f(t)(x_{i+1}-x_{i}),\\U(f,P)&=\sum _{i=0}^{n-1}\sup _{t\in
      [x_{i},x_{i+1}]}f(t)(x_{i+1}-x_{i}).\end{aligned}}}]
If f is continuous, then the lower and upper Darboux sums for an untagged
partition are equal to the Riemann sum for that partition, where the tags are
chosen to be the minimum or maximum (respectively) of f on each subinterval.
(When f is discontinuous on a subinterval, there may not be a tag that achieves
the infimum or supremum on that subinterval.) The Darboux_integral, which is
similar to the Riemann integral but based on Darboux sums, is equivalent to the
Riemann integral.
**** Riemann integral[edit] ****
Loosely speaking, the Riemann integral is the limit of the Riemann sums of a
function as the partitions get finer. If the limit exists then the function is
said to be integrable (or more specifically Riemann-integrable). The Riemann
sum can be made as close as desired to the Riemann integral by making the
partition fine enough.[3]
One important requirement is that the mesh of the partitions must become
smaller and smaller, so that in the limit, it is zero. If this were not so,
then we would not be getting a good approximation to the function on certain
subintervals. In fact, this is enough to define an integral. To be specific, we
say that the Riemann integral of f equals s if the following condition holds:
     For all Îµ > 0, there exists Î´ > 0 such that for any tagged
     partition x0, ..., xn and t0, ..., tn â 1 whose mesh is less than
     Î´, we have
               |   &#x2211;  i = 0   n &#x2212; 1   f (  t  i   ) (  x  i
           + 1   &#x2212;  x  i   ) &#x2212; s  |  < &#x03B5; .
           {\displaystyle \left|\sum _{i=0}^{n-1}f(t_{i})(x_{i+1}-x_{i})-
           s\right|<\varepsilon .}  [\left|\sum_{i=0}^{n-1} f(t_i) (x_
           {i+1}-x_i) - s\right| < \varepsilon.]
Unfortunately, this definition is very difficult to use. It would help to
develop an equivalent definition of the Riemann integral which is easier to
work with. We develop this definition now, with a proof of equivalence
following. Our new definition says that the Riemann integral of f equals s if
the following condition holds:
     For all Îµ > 0, there exists a tagged partition y0, ..., ym and r0,
     ..., rm â 1 such that for any tagged partition x0, ..., xn and t0,
     ..., tn â 1 which is a refinement of y0, ..., ym and r0, ..., rm
     â 1, we have
               |   &#x2211;  i = 0   n &#x2212; 1   f (  t  i   ) (  x  i
           + 1   &#x2212;  x  i   ) &#x2212; s  |  < &#x03B5; .
           {\displaystyle \left|\sum _{i=0}^{n-1}f(t_{i})(x_{i+1}-x_{i})-
           s\right|<\varepsilon .}  [\left|\sum_{i=0}^{n-1} f(t_i) (x_
           {i+1}-x_i) - s\right| < \varepsilon.]
Both of these mean that eventually, the Riemann sum of f with respect to any
partition gets trapped close to s. Since this is true no matter how close we
demand the sums be trapped, we say that the Riemann sums converge to s. These
definitions are actually a special case of a more general concept, a net.
As we stated earlier, these two definitions are equivalent. In other words, s
works in the first definition if and only if s works in the second definition.
To show that the first definition implies the second, start with an Îµ, and
choose a Î´ that satisfies the condition. Choose any tagged partition whose
mesh is less than Î´. Its Riemann sum is within Îµ of s, and any refinement of
this partition will also have mesh less than Î´, so the Riemann sum of the
refinement will also be within Îµ of s.
To show that the second definition implies the first, it is easiest to use the
Darboux_integral. First, one shows that the second definition is equivalent to
the definition of the Darboux integral; for this see the article on Darboux
integration. Now we will show that a Darboux integrable function satisfies the
first definition. Fix Îµ, and choose a partition y0, ..., ym such that the
lower and upper Darboux sums with respect to this partition are within Îµ/2 of
the value s of the Darboux integral. Let
         r = 2  sup  x &#x2208; [ a , b ]    |  f ( x )  |  .   {\displaystyle
      r=2\sup _{x\in [a,b]}|f(x)|.}  [{\displaystyle r=2\sup _{x\in [a,b]}|f
      (x)|.}]
If r = 0, then f is the zero function, which is clearly both Darboux and
Riemann integrable with integral zero. Therefore, we will assume that r > 0. If
m > 1, then we choose Î´ such that
         &#x03B4; < min  {    &#x03B5;  2 r ( m &#x2212; 1 )    ,  (   y  1
      &#x2212;  y  0    )  ,  (   y  2   &#x2212;  y  1    )  , &#x22EF; ,
      (   y  m   &#x2212;  y  m &#x2212; 1    )   }    {\displaystyle \delta
      <\min \left\{{\frac {\varepsilon }{2r(m-1)}},\left(y_{1}-y_
      {0}\right),\left(y_{2}-y_{1}\right),\cdots ,\left(y_{m}-y_{m-
      1}\right)\right\}}  [{\displaystyle \delta <\min \left\{{\frac
      {\varepsilon }{2r(m-1)}},\left(y_{1}-y_{0}\right),\left(y_{2}-y_
      {1}\right),\cdots ,\left(y_{m}-y_{m-1}\right)\right\}}]
If m = 1, then we choose Î´ to be less than one. Choose a tagged partition x0,
..., xn and t0, ..., tn â 1 with mesh smaller than Î´. We must show that the
Riemann sum is within Îµ of s.
To see this, choose an interval [xi, xi + 1]. If this interval is contained
within some [yj, yj + 1], then
          m  j   < f (  t  i   ) <  M  j     {\displaystyle m_{j}<f(t_{i})<M_
      {j}}  [ m_j < f(t_i) < M_j]
where mj and Mj are respectively, the infimum and the supremum of f on [yj, yj
+ 1]. If all intervals had this property, then this would conclude the proof,
because each term in the Riemann sum would be bounded by a corresponding term
in the Darboux sums, and we chose the Darboux sums to be near s. This is the
case when m = 1, so the proof is finished in that case.
Therefore, we may assume that m > 1. In this case, it is possible that one of
the [xi, xi + 1] is not contained in any [yj, yj + 1]. Instead, it may stretch
across two of the intervals determined by y0, ..., ym. (It cannot meet three
intervals because Î´ is assumed to be smaller than the length of any one
interval.) In symbols, it may happen that
          y  j   <  x  i   <  y  j + 1   <  x  i + 1   <  y  j + 2   .
      {\displaystyle y_{j}<x_{i}<y_{j+1}<x_{i+1}<y_{j+2}.}  [y_j < x_i < y_
      {j+1} < x_{i+1} < y_{j+2}.]
(We may assume that all the inequalities are strict because otherwise we are in
the previous case by our assumption on the length of Î´.) This can happen at
most m â 1 times.
To handle this case, we will estimate the difference between the Riemann sum
and the Darboux sum by subdividing the partition x0, ..., xn at yj + 1. The
term f(ti)(xi + 1 â xi) in the Riemann sum splits into two terms:
         f  (  t  i   )   (   x  i + 1   &#x2212;  x  i    )  = f  (  t  i   )
      (   x  i + 1   &#x2212;  y  j + 1    )  + f  (  t  i   )   (   y  j + 1
      &#x2212;  x  i    )  .   {\displaystyle f\left(t_{i}\right)\left(x_{i+1}-
      x_{i}\right)=f\left(t_{i}\right)\left(x_{i+1}-y_{j+1}\right)+f\left(t_
      {i}\right)\left(y_{j+1}-x_{i}\right).}  [{\displaystyle f\left(t_
      {i}\right)\left(x_{i+1}-x_{i}\right)=f\left(t_{i}\right)\left(x_{i+1}-y_
      {j+1}\right)+f\left(t_{i}\right)\left(y_{j+1}-x_{i}\right).}]
Suppose, without loss of generality, that ti â [yj, yj + 1]. Then
          m  j   < f (  t  i   ) <  M  j   ,   {\displaystyle m_{j}<f(t_{i})<M_
      {j},}  [m_j < f(t_i) < M_j,]
so this term is bounded by the corresponding term in the Darboux sum for yj. To
bound the other term, notice that
          x  i + 1   &#x2212;  y  j + 1   < &#x03B4; <   &#x03B5;  2 r ( m
      &#x2212; 1 )    ,   {\displaystyle x_{i+1}-y_{j+1}<\delta <{\frac
      {\varepsilon }{2r(m-1)}},}  [x_{i+1}-y_{j+1} < \delta < \frac
      {\varepsilon}{2r(m-1)},]
It follows that, for some (indeed any) t*
i â [yj + 1, xi + 1],
          |  f  (  t  i   )  &#x2212; f  (  t  i   &#x2217;   )   |   (   x  i
      + 1   &#x2212;  y  j + 1    )  <   &#x03B5;  2 ( m &#x2212; 1 )    .
      {\displaystyle \left|f\left(t_{i}\right)-f\left(t_{i}^
      {*}\right)\right|\left(x_{i+1}-y_{j+1}\right)<{\frac {\varepsilon }{2(m-
      1)}}.}  [{\displaystyle \left|f\left(t_{i}\right)-f\left(t_{i}^
      {*}\right)\right|\left(x_{i+1}-y_{j+1}\right)<{\frac {\varepsilon }{2(m-
      1)}}.}]
Since this happens at most m â 1 times, the distance between the Riemann sum
and a Darboux sum is at most Îµ/2. Therefore, the distance between the Riemann
sum and s is at most Îµ.
***** Examples[edit] *****
Let f : [0, 1] â R be the function which takes the value 1 at every point.
Any Riemann sum of f on [0, 1] will have the value 1, therefore the Riemann
integral of f on [0, 1] is 1.
Let IQ : [0, 1] â R be the indicator_function of the rational numbers in [0,
1]; that is, IQ takes the value 1 on rational numbers and 0 on irrational
numbers. This function does not have a Riemann integral. To prove this, we will
show how to construct tagged partitions whose Riemann sums get arbitrarily
close to both zero and one.
To start, let x0, ..., xn and t0, ..., tn â 1 be a tagged partition (each ti
is between xi and xi + 1). Choose Îµ > 0. The ti have already been chosen, and
we can't change the value of f at those points. But if we cut the partition
into tiny pieces around each ti, we can minimize the effect of the ti. Then, by
carefully choosing the new tags, we can make the value of the Riemann sum turn
out to be within Îµ of either zero or one.
Our first step is to cut up the partition. There are n of the ti, and we want
their total effect to be less than Îµ. If we confine each of them to an
interval of length less than Îµ/n, then the contribution of each ti to the
Riemann sum will be at least 0 Â· Îµ/n and at most 1 Â· Îµ/n. This makes the
total sum at least zero and at most Îµ. So let Î´ be a positive number less
than Îµ/n. If it happens that two of the ti are within Î´ of each other, choose
Î´ smaller. If it happens that some ti is within Î´ of some xj, and ti is not
equal to xj, choose Î´ smaller. Since there are only finitely many ti and xj,
we can always choose Î´ sufficiently small.
Now we add two cuts to the partition for each ti. One of the cuts will be at ti
â Î´/2, and the other will be at ti + Î´/2. If one of these leaves the
interval [0, 1], then we leave it out. ti will be the tag corresponding to the
subinterval
          [   t  i   &#x2212;   &#x03B4; 2   ,  t  i   +   &#x03B4; 2    ]  .
      {\displaystyle \left[t_{i}-{\frac {\delta }{2}},t_{i}+{\frac {\delta }
      {2}}\right].}  [{\displaystyle \left[t_{i}-{\frac {\delta }{2}},t_{i}+
      {\frac {\delta }{2}}\right].}]
If ti is directly on top of one of the xj, then we let ti be the tag for both
intervals:
          [   t  i   &#x2212;   &#x03B4; 2   ,  x  j    ]  ,   and    [   x  j
      ,  t  i   +   &#x03B4; 2    ]  .   {\displaystyle \left[t_{i}-{\frac
      {\delta }{2}},x_{j}\right],\quad {\text{and}}\quad \left[x_{j},t_{i}+
      {\frac {\delta }{2}}\right].}  [{\displaystyle \left[t_{i}-{\frac {\delta
      }{2}},x_{j}\right],\quad {\text{and}}\quad \left[x_{j},t_{i}+{\frac
      {\delta }{2}}\right].}]
We still have to choose tags for the other subintervals. We will choose them in
two different ways. The first way is to always choose a rational_point, so that
the Riemann sum is as large as possible. This will make the value of the
Riemann sum at least 1 â Îµ. The second way is to always choose an irrational
point, so that the Riemann sum is as small as possible. This will make the
value of the Riemann sum at most Îµ.
Since we started from an arbitrary partition and ended up as close as we wanted
to either zero or one, it is false to say that we are eventually trapped near
some number s, so this function is not Riemann integrable. However, it is
Lebesgue_integrable. In the Lebesgue sense its integral is zero, since the
function is zero almost_everywhere. But this is a fact that is beyond the reach
of the Riemann integral.
There are even worse examples. IQ is equivalent (that is, equal almost
everywhere) to a Riemann integrable function, but there are non-Riemann
integrable bounded functions which are not equivalent to any Riemann integrable
function. For example, let C be the SmithâVolterraâCantor_set, and let IC
be its indicator function. Because C is not Jordan_measurable, IC is not
Riemann integrable. Moreover, no function g equivalent to IC is Riemann
integrable: g, like IC, must be zero on a dense set, so as in the previous
example, any Riemann sum of g has a refinement which is within Îµ of 0 for any
positive number Îµ. But if the Riemann integral of g exists, then it must equal
the Lebesgue integral of IC, which is 1/2. Therefore, g is not Riemann
integrable.
***** Similar concepts[edit] *****
It is popular to define the Riemann integral as the Darboux_integral. This is
because the Darboux integral is technically simpler and because a function is
Riemann-integrable if and only if it is Darboux-integrable.
Some calculus books do not use general tagged partitions, but limit themselves
to specific types of tagged partitions. If the type of partition is limited too
much, some non-integrable functions may appear to be integrable.
One popular restriction is the use of "left-hand" and "right-hand" Riemann
sums. In a left-hand Riemann sum, ti = xi for all i, and in a right-hand
Riemann sum, ti = xi + 1 for all i. Alone this restriction does not impose a
problem: we can refine any partition in a way that makes it a left-hand or
right-hand sum by subdividing it at each ti. In more formal language, the set
of all left-hand Riemann sums and the set of all right-hand Riemann sums is
cofinal in the set of all tagged partitions.
Another popular restriction is the use of regular subdivisions of an interval.
For example, the nth regular subdivision of [0, 1] consists of the intervals
          [  0 ,   1 n    ]  ,  [    1 n   ,   2 n    ]  , &#x2026; ,  [     n
      &#x2212; 1  n   , 1  ]  .   {\displaystyle \left[0,{\frac {1}
      {n}}\right],\left[{\frac {1}{n}},{\frac {2}{n}}\right],\ldots ,\left[
      {\frac {n-1}{n}},1\right].}  [{\displaystyle \left[0,{\frac {1}
      {n}}\right],\left[{\frac {1}{n}},{\frac {2}{n}}\right],\ldots ,\left[
      {\frac {n-1}{n}},1\right].}]
Again, alone this restriction does not impose a problem, but the reasoning
required to see this fact is more difficult than in the case of left-hand and
right-hand Riemann sums.
However, combining these restrictions, so that one uses only left-hand or
right-hand Riemann sums on regularly divided intervals, is dangerous. If a
function is known in advance to be Riemann integrable, then this technique will
give the correct value of the integral. But under these conditions the
indicator_function IQ will appear to be integrable on [0, 1] with integral
equal to one: Every endpoint of every subinterval will be a rational number, so
the function will always be evaluated at rational numbers, and hence it will
appear to always equal one. The problem with this definition becomes apparent
when we try to split the integral into two pieces. The following equation ought
to hold:
          &#x222B;  0     2   &#x2212; 1     I   Q    ( x )  d x +  &#x222B;
      2   &#x2212; 1   1     I   Q    ( x )  d x =  &#x222B;  0   1     I   Q
      ( x )  d x .   {\displaystyle \int _{0}^{{\sqrt {2}}-1}\!I_{\mathbb {Q} }
      (x)\,dx+\int _{{\sqrt {2}}-1}^{1}\!I_{\mathbb {Q} }(x)\,dx=\int _{0}^
      {1}\!I_{\mathbb {Q} }(x)\,dx.}  [{\displaystyle \int _{0}^{{\sqrt {2}}-
      1}\!I_{\mathbb {Q} }(x)\,dx+\int _{{\sqrt {2}}-1}^{1}\!I_{\mathbb {Q} }
      (x)\,dx=\int _{0}^{1}\!I_{\mathbb {Q} }(x)\,dx.}]
If we use regular subdivisions and left-hand or right-hand Riemann sums, then
the two terms on the left are equal to zero, since every endpoint except 0 and
1 will be irrational, but as we have seen the term on the right will equal 1.
As defined above, the Riemann integral avoids this problem by refusing to
integrate IQ. The Lebesgue integral is defined in such a way that all these
integrals are 0.
***** Properties[edit] *****
**** Linearity[edit] ****
The Riemann integral is a linear transformation; that is, if f and g are
Riemann-integrable on [a, b] and Î± and Î² are constants, then
          &#x222B;  a   b     (   &#x03B1; f ( x ) + &#x03B2; g ( x )   )    d
      x = &#x03B1;  &#x222B;  a   b   f ( x )  d x + &#x03B2;  &#x222B;  a   b
      g ( x )  d x .   {\displaystyle \int _{a}^{b}{\bigl (}\alpha f(x)+\beta g
      (x){\bigr )}\,dx=\alpha \int _{a}^{b}f(x)\,dx+\beta \int _{a}^{b}g
      (x)\,dx.}  [{\displaystyle \int _{a}^{b}{\bigl (}\alpha f(x)+\beta g(x)
      {\bigr )}\,dx=\alpha \int _{a}^{b}f(x)\,dx+\beta \int _{a}^{b}g(x)\,dx.}]
Because the Riemann integral of a function is a number, this makes the Riemann
integral a linear_functional on the vector_space of Riemann-integrable
functions.
***** Integrability[edit] *****
A bounded_function on a compact_interval [a, b] is Riemann integrable if and
only if it is continuous almost_everywhere (the set of its points of
discontinuity has measure_zero, in the sense of Lebesgue_measure). This is
known as the Lebesgue's integrability condition or Lebesgue's criterion for
Riemann integrability or the RiemannâLebesgue theorem.[4] The criterion has
nothing to do with the Lebesgue_integral. It is due to Lebesgue and uses his
measure_zero, but makes use of neither Lebesgue's general measure or integral.
The integrability condition can be proven in various ways,[4][5][6][7] one of
which is sketched below.
      Proof
      The proof is easiest using the Darboux_integral definition of integrability (formally,
      the Riemann condition for integrability) â a function is Riemann integrable if and
      only if the upper and lower sums can be made arbitrarily close by choosing an
      appropriate partition.
      One direction can be proven using the oscillation definition of continuity:[8] For
      every positive Îµ, Let XÎµ be the set of points in [a, b] with oscillation of at least
      Îµ. Since every point where f is discontinuous has a positive oscillation and vice
      versa, the set of points in [a, b], where f is discontinuous is equal to the union over
      {X1/n} for all natural numbers n.
      If this set does not have a zero Lebesgue_measure, then by countable_additivity of the
      measure there is at least one such n so that X1/n does not have a zero measure. Thus
      there is some positive number c such that every countable collection of open intervals
      covering X1/n has a total length of at least c. In particular this is also true for
      every such finite collection of intervals. Note that this remains true also for X1/
      n less a finite number of points (as a finite number of points can always be covered by
      a finite collection of intervals with arbitrarily small total length).
      For every partition_of_[a,_b], consider the set of intervals whose interiors include
      points from X1/n. These interiors consist of a finite open cover of X1/n, possibly up
      to a finite number of points (which may fall on interval edges). Thus these intervals
      have a total length of at least c. Since in these points f has oscillation of at least
      1/n, the infimum_and_supremum of f in each of these intervals differ by at least 1/n.
      Thus the upper and lower sums of f differ by at least c/n. Since this is true for every
      partition, f is not Riemann integrable.
      We now prove the converse direction using the sets XÎµ defined above.[9] Note that for
      every Îµ, XÎµ is compact, as it is bounded (by a and b) and closed:
          * For every series of points in XÎµ that is converging in [a, b], its limit is in
            XÎµ as well. This is because every neighborhood of the limit point is also a
            neighborhood of some point in XÎµ, and thus f has an oscillation of at least Îµ
            on it. Hence the limit point is in XÎµ.
      Now, suppose that f is continuous almost_everywhere. Then for every Îµ, XÎµ has zero
      Lebesgue_measure. Therefore, there is a countable collections of open intervals in [a,
      b] which is an open_cover of XÎµ, such that the sum over all their lengths is
      arbitrarily small. Since_XÎµ_is_compact, there is a finite subcover â a finite
      collections of open intervals in [a, b] with arbitrarily small total length that
      together contain all points in XÎµ. We denote these intervals {I(Îµ)i}, for 1 â¤ i â¤
      k, for some natural k.
      The complement of the union of these intervals is itself a union of a finite number of
      intervals, which we denote {J(Îµ)i} (for 1 â¤ i â¤ k â 1 and possibly for i = k, k
      + 1 as well).
      We now show that for every Îµ > 0, there are upper_and_lower_sums whose difference is
      less than Îµ, from which Riemann integrability follows. To this end, we construct a
      partition_of_[a,_b] as follows:
      Denote Îµ1 = Îµ / 2(b â a) and Îµ2 = Îµ / 2(M â m), where m and M are the infimum
      and_supremum of f on [a, b]. Since we may choose intervals {I(Îµ1)i} with arbitrarily
      small total length, we choose them to have total length smaller than Îµ2.
      Each of the intervals {J(Îµ1)i} has an empty intersection with XÎµ1, so each point in
      it has a neighborhood with oscillation smaller than Îµ1. These neighborhoods consist of
      an open_cover of the interval, and since the interval is compact there is a finite
      subcover of them. This subcover is a finite collection of open intervals, which are
      subintervals of J(Îµ1)i (except for those that include an edge point, for which we only
      take their intersection with J(Îµ1)i). We take the edge points of the subintervals for
      all J(Îµ1)i â s, including the edge points of the intervals themselves, as our
      partition.
      Thus the partition divides [a, b] to two kinds of intervals:
          * Intervals of the latter kind (themselves subintervals of some J(Îµ1)i). In each
            of these, f oscillates by less than Îµ1. Since the total length of these is not
            larger than b â a, they together contribute at most Îµâ
            1(b â a) = Îµ/2 to the difference between the upper and lower sums of the
            partition.
          * The intervals {I(Îµ)i}. These have total length smaller than Îµ2, and f
            oscillates on them by no more than M â m. Thus together they contribute less
            than Îµâ
            2(M â m) = Îµ/2 to the difference between the upper and lower sums of the
            partition.
      In total, the difference between the upper and lower sums of the partition is smaller
      than Îµ, as required.
In particular, any set that is at most countable has Lebesgue_measure zero, and
thus a bounded function (on a compact interval) with only finitely or countably
many discontinuities is Riemann integrable.
An indicator_function of a bounded set is Riemann-integrable if and only if the
set is Jordan_measurable.[10] The Riemann integral can be interpreted measure-
theoretically as the integral with respect to the Jordan measure.
If a real-valued function is monotone on the interval [a, b] it is Riemann-
integrable, since its set of discontinuities is at most countable, and
therefore of Lebesgue measure zero.
If a real-valued function on [a, b] is Riemann-integrable, it is Lebesgue-
integrable. That is, Riemann-integrability is a stronger (meaning more
difficult to satisfy) condition than Lebesgue-integrability.
If fn is a uniformly_convergent sequence on [a, b] with limit f, then Riemann
integrability of all fn implies Riemann integrability of f, and
          &#x222B;  a   b   f  d x =  &#x222B;  a   b     lim  n &#x2192;
      &#x221E;     f  n     d x  =  lim  n &#x2192; &#x221E;    &#x222B;  a   b
      f  n    d x .   {\displaystyle \int _{a}^{b}f\,dx=\int _{a}^{b}{\lim _
      {n\to \infty }{f_{n}}\,dx}=\lim _{n\to \infty }\int _{a}^{b}f_{n}\,dx.}
      [ \int_{a}^{b} f\, dx = \int_a^b{\lim_{n \to \infty}{f_n}\, dx} = \lim_{n
      \to \infty} \int_{a}^{b} f_n\, dx.]
However, the Lebesgue_monotone_convergence_theorem (on a monotone pointwise
limit) does not hold. In Riemann integration, taking limits under the integral
sign is far more difficult to logically justify than in Lebesgue integration.
[11]
***** Generalizations[edit] *****
It is easy to extend the Riemann integral to functions with values in the
Euclidean vector space Rn for any n. The integral is defined component-wise; in
other words, if f = (f1, ..., fn) then
         &#x222B;  f  =  (  &#x222B;  f  1   ,  &#x2026; , &#x222B;  f  n    )
      .   {\displaystyle \int \mathbf {f} =\left(\int f_{1},\,\dots ,\int f_
      {n}\right).}  [\int\mathbf{f} = \left(\int f_1,\,\dots, \int f_n\right).]
In particular, since the complex numbers are a real vector_space, this allows
the integration of complex valued functions.
The Riemann integral is only defined on bounded intervals, and it does not
extend well to unbounded intervals. The simplest possible extension is to
define such an integral as a limit, in other words, as an improper_integral:
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x )  d x =  lim    a
      &#x2192; &#x2212; &#x221E;   b &#x2192; &#x221E;      &#x222B;  a   b   f
      ( x )  d x .   {\displaystyle \int _{-\infty }^{\infty }f(x)\,dx=\lim _
      {a\to -\infty \atop b\to \infty }\int _{a}^{b}f(x)\,dx.}  [{\displaystyle
      \int _{-\infty }^{\infty }f(x)\,dx=\lim _{a\to -\infty  \atop b\to \infty
      }\int _{a}^{b}f(x)\,dx.}]
This definition carries with it some subtleties, such as the fact that it is
not always equivalent to compute the Cauchy_principal_value
          lim  a &#x2192; &#x221E;    &#x222B;  &#x2212; a   a   f ( x )  d x .
      {\displaystyle \lim _{a\to \infty }\int _{-a}^{a}f(x)\,dx.}  [
      {\displaystyle \lim _{a\to \infty }\int _{-a}^{a}f(x)\,dx.}]
For example, consider the function f(x) which is 0 at x = 0, 1 for x > 0, and
â1 for x < 0. By symmetry,
          &#x222B;  &#x2212; a   a   f ( x )  d x = 0   {\displaystyle \int _{-
      a}^{a}f(x)\,dx=0}  [{\displaystyle \int _{-a}^{a}f(x)\,dx=0}]
always, regardless of a. But there are many ways for the interval of
integration to expand to fill the real line, and other ways can produce
different results; in other words, the multivariate limit does not always
exist. We can compute
              &#x222B;  &#x2212; a   2 a   f ( x )  d x    = a ,      &#x222B;
      &#x2212; 2 a   a   f ( x )  d x    = &#x2212; a .       {\displaystyle
      {\begin{aligned}\int _{-a}^{2a}f(x)\,dx&=a,\\\int _{-2a}^{a}f(x)\,dx&=-
      a.\end{aligned}}}  [{\displaystyle {\begin{aligned}\int _{-a}^{2a}f
      (x)\,dx&=a,\\\int _{-2a}^{a}f(x)\,dx&=-a.\end{aligned}}}]
In general, this improper Riemann integral is undefined. Even standardizing a
way for the interval to approach the real line does not work because it leads
to disturbingly counterintuitive results. If we agree (for instance) that the
improper integral should always be
          lim  a &#x2192; &#x221E;    &#x222B;  &#x2212; a   a   f ( x )  d x ,
      {\displaystyle \lim _{a\to \infty }\int _{-a}^{a}f(x)\,dx,}  [
      {\displaystyle \lim _{a\to \infty }\int _{-a}^{a}f(x)\,dx,}]
then the integral of the translation f(x â 1) is â2, so this definition is
not invariant under shifts, a highly undesirable property. In fact, not only
does this function not have an improper Riemann integral, its Lebesgue integral
is also undefined (it equals â â â).
Unfortunately, the improper Riemann integral is not powerful enough. The most
severe problem is that there are no widely applicable theorems for commuting
improper Riemann integrals with limits of functions. In applications such as
Fourier_series it is important to be able to approximate the integral of a
function using integrals of approximations to the function. For proper Riemann
integrals, a standard theorem states that if fn is a sequence of functions that
converge_uniformly to f on a compact set [a, b], then
          lim  n &#x2192; &#x221E;    &#x222B;  a   b    f  n   ( x )  d x =
      &#x222B;  a   b   f ( x )  d x .   {\displaystyle \lim _{n\to \infty
      }\int _{a}^{b}f_{n}(x)\,dx=\int _{a}^{b}f(x)\,dx.}  [{\displaystyle \lim
      _{n\to \infty }\int _{a}^{b}f_{n}(x)\,dx=\int _{a}^{b}f(x)\,dx.}]
On non-compact intervals such as the real line, this is false. For example,
take fn(x) to be nâ1 on [0, n] and zero elsewhere. For all n we have:
          &#x222B;  &#x2212; &#x221E;   &#x221E;    f  n    d x = 1.
      {\displaystyle \int _{-\infty }^{\infty }f_{n}\,dx=1.}  [\int_{-
      \infty}^\infty f_n\,dx = 1.]
The sequence {fn} converges uniformly to the zero function, and clearly the
integral of the zero function is zero. Consequently,
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f  d x &#x2260;  lim  n
      &#x2192; &#x221E;    &#x222B;  &#x2212; &#x221E;   &#x221E;    f  n    d
      x .   {\displaystyle \int _{-\infty }^{\infty }f\,dx\neq \lim _{n\to
      \infty }\int _{-\infty }^{\infty }f_{n}\,dx.}  [{\displaystyle \int _{-
      \infty }^{\infty }f\,dx\neq \lim _{n\to \infty }\int _{-\infty }^{\infty
      }f_{n}\,dx.}]
This demonstrates that for integrals on unbounded intervals, uniform
convergence of a function is not strong enough to allow passing a limit through
an integral sign. This makes the Riemann integral unworkable in applications
(even though the Riemann integral assigns both sides the correct value),
because there is no other general criterion for exchanging a limit and a
Riemann integral, and without such a criterion it is difficult to approximate
integrals by approximating their integrands.
A better route is to abandon the Riemann integral for the Lebesgue_integral.
The definition of the Lebesgue integral is not obviously a generalization of
the Riemann integral, but it is not hard to prove that every Riemann-integrable
function is Lebesgue-integrable and that the values of the two integrals agree
whenever they are both defined. Moreover, a function f defined on a bounded
interval is Riemann-integrable if and only if it is bounded and the set of
points where f is discontinuous has Lebesgue measure zero.
An integral which is in fact a direct generalization of the Riemann integral is
the HenstockâKurzweil_integral.
Another way of generalizing the Riemann integral is to replace the factors xk +
1 â xk in the definition of a Riemann sum by something else; roughly
speaking, this gives the interval of integration a different notion of length.
This is the approach taken by the RiemannâStieltjes_integral.
In multivariable_calculus, the Riemann integrals for functions from Rn â R
are multiple_integrals.
***** See also[edit] *****
    * Area
    * Antiderivative
    * Lebesgue_integration
***** Notes[edit] *****
   1. ^ The Riemann integral was introduced in Bernhard Riemann's paper "Ãber
      die Darstellbarkeit einer Function durch eine trigonometrische Reihe" (On
      the representability of a function by a trigonometric series; i.e., when
      can a function be represented by a trigonometric series). This paper was
      submitted to the University of GÃ¶ttingen in 1854 as Riemann's
      Habilitationsschrift (qualification to become an instructor). It was
      published in 1868 in Abhandlungen der KÃ¶niglichen Gesellschaft der
      Wissenschaften zu GÃ¶ttingen (Proceedings of the Royal Philosophical
      Society at GÃ¶ttingen), vol. 13, pages 87-132. (Available online here.)
      For Riemann's definition of his integral, see section 4, "Ãber den
      Begriff eines bestimmten Integrals und den Umfang seiner GÃ¼ltigkeit" (On
      the concept of a definite integral and the extent of its validity), pages
      101â103.
   2. ^Krantz,_Steven_G. (1991). Real_Analysis_and_Foundations. CRC Press.
      p. 173.
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
   4. ;2005 edition. ISBN 9781584884835.
   5. ^Taylor,_Michael_E. (2006). Measure_Theory_and_Integration. American
      Mathematical Society. p. 1. ISBN 9780821872468.
   6. ^ a b Apostol_1974, pp. 169â172
   7. ^Brown, A. B. (September 1936). "A Proof of the Lebesgue Condition for
      Riemann Integrability". The American Mathematical Monthly. 43 (7):
      396â398. doi:10.2307/2301737. ISSN 0002-9890. JSTOR 2301737.
   8. ^ Basic real analysis, by Houshang H. Sohrab, section 7.3, Sets of
      Measure Zero and Lebesgueâs Integrability Condition, pp._264â271
   9. ^ Introduction_to_Real_Analysis, updated April 2010, William F. Trench,
      3.5 "A More Advanced Look at the Existence of the Proper Riemann
      Integral", pp. 171â177
  10. ^ Lebesgueâs_Condition, John Armstrong, December 15, 2009, The
      Unapologetic Mathematician
  11. ^ Jordan_Content_Integrability_Condition, John Armstrong, December 9,
      2009, The Unapologetic Mathematician
  12. ^ PlanetMath_Volume
  13. ^Cunningham, Frederick, Jr. (1967). "Taking_limits_under_the_integral
      sign". Mathematics Magazine. 40: 179â186. doi:10.2307/2688673.
***** References[edit] *****
    * Shilov, G. E., and Gurevich, B. L., 1978. Integral, Measure, and
      Derivative: A Unified Approach, Richard A. Silverman, trans. Dover
      Publications.
ISBN 0-486-63519-8.
Apostol,_Tom (1974), Mathematical Analysis, Addison-Wesley
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Riemann_integral", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
    * v
    * t
    * e
Integrals
                          * Riemann integral
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
                          * Contour_integration
Improper Integrals        * Improper_integral
                          * Gaussian_integral
                          * ItÃ´_integral
Stochastic integrals      * RussoâVallois_integral
                          * Stratonovich_integral
                          * Skorokhod_integral

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Riemann_integral&oldid=897361989"
Categories:
    * Definitions_of_mathematical_integration
    * Bernhard_Riemann
Hidden categories:
    * Articles_with_short_description
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AzÉrbaycanca
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Bahasa_Indonesia
    * Italiano
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Sicilianu
    * SlovenÄina
    * Ú©ÙØ±Ø¯Û
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 16 May 2019, at 14:46 (UTC).
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
