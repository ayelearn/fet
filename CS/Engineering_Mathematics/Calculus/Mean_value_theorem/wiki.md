The following text has been accessed from https://en.wikipedia.org/wiki/Mean_value_theorem at Fri Aug 9 01:09:33 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Mean value theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For the theorem in harmonic function theory, see Harmonic_function_Â§ The_mean
value_property.
Not to be confused with the Intermediate_value_theorem.
Part of a series of articles about
Calculus
    * Fundamental_theorem
    * Limits_of_functions
    * Continuity
    * Mean value theorem
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
For any function that is continuous on     [ a , b ]   {\displaystyle [a,b]}  [
[a,b]] and differentiable on     ( a , b )   {\displaystyle (a,b)}  [(a,b)]
there exists some     c   {\displaystyle c}  [c] in the interval     ( a , b )
{\displaystyle (a,b)}  [(a,b)] such that the secant joining the endpoints of
the interval     [ a , b ]   {\displaystyle [a,b]}  [[a,b]] is parallel to the
tangent at     c   {\displaystyle c}  [c] .
In mathematics, the mean value theorem states, roughly, that for a given planar
arc between two endpoints, there is at least one point at which the tangent to
the arc is parallel to the secant through its endpoints.
This theorem is used to prove statements about a function on an interval
starting from local hypotheses about derivatives at points of the interval.
More precisely, if     f   {\displaystyle f}  [f] is a continuous_function on
the closed_interval     [ a , b ]   {\displaystyle [a,b]}  [[a,b]], and
differentiable on the open_interval     ( a , b )   {\displaystyle (a,b)}  [
(a,b)], then there exists a point     c   {\displaystyle c}  [c] in     ( a , b
)   {\displaystyle (a,b)}  [(a,b)] such that:[1]
          f &#x2032;  ( c ) =    f ( b ) &#x2212; f ( a )   b &#x2212; a    .
      {\displaystyle f'(c)={\frac {f(b)-f(a)}{b-a}}.}  [{\displaystyle f'(c)=
      {\frac {f(b)-f(a)}{b-a}}.}]
It is one of the most important results in real_analysis.
⁰
***** Contents *****
    * 1_History
    * 2_Formal_statement
    * 3_Proof
    * 4_A_simple_application
    * 5_Cauchy's_mean_value_theorem
          o 5.1_Proof_of_Cauchy's_mean_value_theorem
    * 6_Generalization_for_determinants
    * 7_Mean_value_theorem_in_several_variables
    * 8_Mean_value_theorem_for_vector-valued_functions
    * 9_Mean_value_theorems_for_definite_integrals
          o 9.1_First_mean_value_theorem_for_definite_integrals
          o 9.2_Proof_of_the_first_mean_value_theorem_for_definite_integrals
          o 9.3_Second_mean_value_theorem_for_definite_integrals
          o 9.4_Mean_value_theorem_for_integration_fails_for_vector-valued
            functions
    * 10_A_probabilistic_analogue_of_the_mean_value_theorem
    * 11_Generalization_in_complex_analysis
    * 12_See_also
    * 13_Notes
    * 14_External_links
***** History[edit] *****
A special case of this theorem was first described by Parameshvara
(1370â1460), from the Kerala_School_of_Astronomy_and_Mathematics in India, in
his commentaries on GovindasvÄmi and BhÄskara_II.[2] A restricted form of the
theorem was proved by Michel_Rolle in 1691; the result was what is now known as
Rolle's_theorem, and was proved only for polynomials, without the techniques of
calculus. The mean value theorem in its modern form was stated and proved by
Augustin_Louis_Cauchy in 1823.[3]
***** Formal statement[edit] *****
The function     f   {\displaystyle f}  [f] attains the slope of the secant
between     a   {\displaystyle a}  [a] and     b   {\displaystyle b}  [b] as
the derivative at the point     &#x03BE; &#x2208; ( a , b )   {\displaystyle
\xi \in (a,b)}  [{\displaystyle \xi \in (a,b)}].
It is also possible that there are multiple tangents parallel to the secant.
Let     f : [ a , b ] &#x2192;  R    {\displaystyle f:[a,b]\to \mathbb {R} }  [
{\displaystyle f:[a,b]\to \mathbb {R} }] be a continuous_function on the closed
interval     [ a , b ]   {\displaystyle [a,b]}  [[a,b]] , and differentiable on
the open interval     ( a , b )   {\displaystyle (a,b)}  [(a,b)], where     a <
b   {\displaystyle a<b}  [a<b] . Then there exists some     c   {\displaystyle
c}  [c] in     ( a , b )   {\displaystyle (a,b)}  [(a,b)] such that
          f &#x2032;  ( c ) =    f ( b ) &#x2212; f ( a )   b &#x2212; a    .
      {\displaystyle f'(c)={\frac {f(b)-f(a)}{b-a}}.}  [{\displaystyle f'(c)=
      {\frac {f(b)-f(a)}{b-a}}.}]
The mean value theorem is a generalization of Rolle's_theorem, which assumes
f ( a ) = f ( b )   {\displaystyle f(a)=f(b)}  [{\displaystyle f(a)=f(b)}], so
that the right-hand side above is zero.
The mean value theorem is still valid in a slightly more general setting. One
only needs to assume that     f : [ a , b ] &#x2192;  R    {\displaystyle f:
[a,b]\to \mathbb {R} }  [{\displaystyle f:[a,b]\to \mathbb {R} }] is continuous
on     [ a , b ]   {\displaystyle [a,b]}  [[a,b]] , and that for every     x
{\displaystyle x}  [x] in     ( a , b )   {\displaystyle (a,b)}  [(a,b)] the
limit
          lim  h &#x2192; 0      f ( x + h ) &#x2212; f ( x )  h
      {\displaystyle \lim _{h\to 0}{\frac {f(x+h)-f(x)}{h}}}  [\lim _{h\to 0}
      {\frac {f(x+h)-f(x)}{h}}]
exists as a finite number or equals     &#x221E;   {\displaystyle \infty }
[\infty ] or     &#x2212; &#x221E;   {\displaystyle -\infty }  [-\infty ] . If
finite, that limit equals      f &#x2032;  ( x )   {\displaystyle f'(x)}  [f'
(x)] . An example where this version of the theorem applies is given by the
real-valued cube_root function mapping     x &#x2192;  x   1 3
{\displaystyle x\to x^{\frac {1}{3}}}  [{\displaystyle x\to x^{\frac {1}{3}}}]
, whose derivative tends to infinity at the origin.
Note that the theorem, as stated, is false if a differentiable function is
complex-valued instead of real-valued. For example, define     f ( x ) =  e  x
i     {\displaystyle f(x)=e^{xi}}  [{\displaystyle f(x)=e^{xi}}] for all real
x   {\displaystyle x}  [x] . Then
         f ( 2 &#x03C0; ) &#x2212; f ( 0 ) = 0 = 0 ( 2 &#x03C0; &#x2212; 0 )
      {\displaystyle f(2\pi )-f(0)=0=0(2\pi -0)}  [{\displaystyle f(2\pi )-f
      (0)=0=0(2\pi -0)}]
while      f &#x2032;  ( x ) &#x2260; 0   {\displaystyle f'(x)\neq 0}  [
{\displaystyle f'(x)\neq 0}] for any real     x   {\displaystyle x}  [x] .
These formal statements are also known as Lagrange's Mean Value Theorem.[4]
***** Proof[edit] *****
The expression        f ( b ) &#x2212; f ( a )   b &#x2212; a
{\displaystyle {\frac {f(b)-f(a)}{b-a}}}  [{\displaystyle {\frac {f(b)-f(a)}{b-
a}}}] gives the slope of the line joining the points     ( a , f ( a ) )
{\displaystyle (a,f(a))}  [(a,f(a))] and     ( b , f ( b ) )   {\displaystyle
(b,f(b))}  [{\displaystyle (b,f(b))}] , which is a chord of the graph of     f
{\displaystyle f}  [f] , while      f &#x2032;  ( x )   {\displaystyle f'(x)}
[f'(x)] gives the slope of the tangent to the curve at the point     ( x , f
( x ) )   {\displaystyle (x,f(x))}  [(x,f(x))] . Thus the mean value theorem
says that given any chord of a smooth curve, we can find a point lying between
the end-points of the chord such that the tangent at that point is parallel to
the chord. The following proof illustrates this idea.
Define     g ( x ) = f ( x ) &#x2212; r x   {\displaystyle g(x)=f(x)-rx}  [
{\displaystyle g(x)=f(x)-rx}] , where     r   {\displaystyle r}  [r] is a
constant. Since     f   {\displaystyle f}  [f] is continuous on     [ a , b ]
{\displaystyle [a,b]}  [[a,b]] and differentiable on     ( a , b )
{\displaystyle (a,b)}  [(a,b)] , the same is true for     g   {\displaystyle g}
[g] . We now want to choose     r   {\displaystyle r}  [r] so that     g
{\displaystyle g}  [g] satisfies the conditions of Rolle's_theorem. Namely
             g ( a ) = g ( b )     &#x27FA;  f ( a ) &#x2212; r a = f ( b )
      &#x2212; r b        &#x27FA;  r ( b &#x2212; a ) = f ( b ) &#x2212; f ( a
      )        &#x27FA;  r =    f ( b ) &#x2212; f ( a )   b &#x2212; a
      &#x22C5;       {\displaystyle {\begin{aligned}g(a)=g(b)&\iff f(a)-ra=f
      (b)-rb\\&\iff r(b-a)=f(b)-f(a)\\&\iff r={\frac {f(b)-f(a)}{b-a}}\cdot
      \end{aligned}}}  [{\begin{aligned}g(a)=g(b)&\iff f(a)-ra=f(b)-rb\\&\iff r
      (b-a)=f(b)-f(a)\\&\iff r={\frac {f(b)-f(a)}{b-a}}\cdot \end{aligned}}]
By Rolle's_theorem, since     g   {\displaystyle g}  [g] is differentiable and
g ( a ) = g ( b )   {\displaystyle g(a)=g(b)}  [{\displaystyle g(a)=g(b)}] ,
there is some     c   {\displaystyle c}  [c] in     ( a , b )   {\displaystyle
(a,b)}  [(a,b)] for which      g &#x2032;  ( c ) = 0   {\displaystyle g'(c)=0}
[{\displaystyle g'(c)=0}] , and it follows from the equality     g ( x ) = f
( x ) &#x2212; r x   {\displaystyle g(x)=f(x)-rx}  [{\displaystyle g(x)=f(x)-
rx}] that,
               g &#x2032;  ( x ) =  f &#x2032;  ( x ) &#x2212; r       g
      &#x2032;  ( c ) = 0       g &#x2032;  ( c ) =  f &#x2032;  ( c ) &#x2212;
      r = 0       &#x21D2;  f &#x2032;  ( c ) = r =    f ( b ) &#x2212; f ( a )
      b &#x2212; a          {\displaystyle {\begin{aligned}&g'(x)=f'(x)-r\\&g'
      (c)=0\\&g'(c)=f'(c)-r=0\\&\Rightarrow f'(c)=r={\frac {f(b)-f(a)}{b-
      a}}\end{aligned}}}  [{\displaystyle {\begin{aligned}&g'(x)=f'(x)-r\\&g'
      (c)=0\\&g'(c)=f'(c)-r=0\\&\Rightarrow f'(c)=r={\frac {f(b)-f(a)}{b-
      a}}\end{aligned}}}]
***** A simple application[edit] *****
Assume that f is a continuous, real-valued function, defined on an arbitrary
interval I of the real line. If the derivative of f at every interior_point of
the interval I exists and is zero, then f is constant in the interior.
Proof: Assume the derivative of f at every interior_point of the interval I
exists and is zero. Let (a, b) be an arbitrary open interval in I. By the mean
value theorem, there exists a point c in (a,b) such that
         0 =  f &#x2032;  ( c ) =    f ( b ) &#x2212; f ( a )   b &#x2212; a
      .   {\displaystyle 0=f'(c)={\frac {f(b)-f(a)}{b-a}}.}  [{\displaystyle
      0=f'(c)={\frac {f(b)-f(a)}{b-a}}.}]
This implies that f(a) = f(b). Thus, f is constant on the interior of I and
thus is constant on I by continuity. (See below for a multivariable version of
this result.)
Remarks:
    * Only continuity of f, not differentiability, is needed at the endpoints
      of the interval I. No hypothesis of continuity needs to be stated if I is
      an open_interval, since the existence of a derivative at a point implies
      the continuity at this point. (See the section continuity_and
      differentiability of the article derivative.)
    * The differentiability of f can be relaxed to one-sided_differentiability,
      a proof given in the article on semi-differentiability.
***** Cauchy's mean value theorem[edit] *****
Cauchy's mean value theorem, also known as the extended mean value theorem,[5]
is a generalization of the mean value theorem. It states: If functions f and g
are both continuous on the closed interval [a, b], and differentiable on the
open interval (a, b), then there exists some c â (a, b), such that[4]
Geometrical meaning of Cauchy's theorem
         ( f ( b ) &#x2212; f ( a ) )  g &#x2032;  ( c ) = ( g ( b ) &#x2212; g
      ( a ) )  f &#x2032;  ( c ) .   {\displaystyle (f(b)-f(a))g'(c)=(g(b)-g
      (a))f'(c).}  [{\displaystyle (f(b)-f(a))g'(c)=(g(b)-g(a))f'(c).}]
Of course, if g(a) â  g(b) and if gâ²(c) â  0, this is equivalent to:
             f &#x2032;  ( c )    g &#x2032;  ( c )    =    f ( b ) &#x2212; f
      ( a )   g ( b ) &#x2212; g ( a )    .   {\displaystyle {\frac {f'(c)}{g'
      (c)}}={\frac {f(b)-f(a)}{g(b)-g(a)}}.}  [{\displaystyle {\frac {f'(c)}{g'
      (c)}}={\frac {f(b)-f(a)}{g(b)-g(a)}}.}]
Geometrically, this means that there is some tangent to the graph of the curve
[6]
           {    [ a , b ] &#x2192;   R   2       t &#x21A6; ( f ( t ) , g ( t )
      )         {\displaystyle {\begin{cases}[a,b]\to \mathbf {R} ^
      {2}\\t\mapsto (f(t),g(t))\end{cases}}}  [{\displaystyle {\begin{cases}
      [a,b]\to \mathbf {R} ^{2}\\t\mapsto (f(t),g(t))\end{cases}}}]
which is parallel to the line defined by the points (f(a), g(a)) and (f(b), g
(b)). However Cauchy's theorem does not claim the existence of such a tangent
in all cases where (f(a), g(a)) and (f(b), g(b)) are distinct points, since it
might be satisfied only for some value c with fâ²(c) = gâ²(c) = 0, in other
words a value for which the mentioned curve is stationary; in such points no
tangent to the curve is likely to be defined at all. An example of this
situation is the curve given by
         t &#x21A6; (  t  3   , 1 &#x2212;  t  2   ) ,   {\displaystyle
      t\mapsto (t^{3},1-t^{2}),}  [t\mapsto (t^{3},1-t^{2}),]
which on the interval [â1, 1] goes from the point (â1, 0) to (1, 0), yet
never has a horizontal tangent; however it has a stationary point (in fact a
cusp) at t = 0.
Cauchy's mean value theorem can be used to prove l'HÃ´pital's_rule. The mean
value theorem is the special case of Cauchy's mean value theorem when g(t) = t.
**** Proof of Cauchy's mean value theorem[edit] ****
The proof of Cauchy's mean value theorem is based on the same idea as the proof
of the mean value theorem.
    * Suppose g(a) â  g(b). Define h(x) = f(x) â rg(x), where r is fixed in
      such a way that h(a) = h(b), namely
                   h ( a ) = h ( b )     &#x27FA;  f ( a ) &#x2212; r g ( a ) =
            f ( b ) &#x2212; r g ( b )        &#x27FA;  r ( g ( b ) &#x2212; g
            ( a ) ) = f ( b ) &#x2212; f ( a )        &#x27FA;  r =    f ( b )
            &#x2212; f ( a )   g ( b ) &#x2212; g ( a )    .
            {\displaystyle {\begin{aligned}h(a)=h(b)&\iff f(a)-rg(a)=f(b)-rg
            (b)\\&\iff r(g(b)-g(a))=f(b)-f(a)\\&\iff r={\frac {f(b)-f(a)}{g(b)-
            g(a)}}.\end{aligned}}}  [{\displaystyle {\begin{aligned}h(a)=h
            (b)&\iff f(a)-rg(a)=f(b)-rg(b)\\&\iff r(g(b)-g(a))=f(b)-f(a)\\&\iff
            r={\frac {f(b)-f(a)}{g(b)-g(a)}}.\end{aligned}}}]
      Since f and g are continuous on [a, b] and differentiable on (a, b), the
      same is true for h. All in all, h satisfies the conditions of Rolle's
      theorem: consequently, there is some c in (a, b) for which hâ²(c) = 0.
      Now using the definition of h we have:
               0 =  h &#x2032;  ( c ) =  f &#x2032;  ( c ) &#x2212; r  g
            &#x2032;  ( c ) =  f &#x2032;  ( c ) &#x2212;  (    f ( b )
            &#x2212; f ( a )   g ( b ) &#x2212; g ( a )    )   g &#x2032;  ( c
            ) .   {\displaystyle 0=h'(c)=f'(c)-rg'(c)=f'(c)-\left({\frac {f(b)-
            f(a)}{g(b)-g(a)}}\right)g'(c).}  [{\displaystyle 0=h'(c)=f'(c)-rg'
            (c)=f'(c)-\left({\frac {f(b)-f(a)}{g(b)-g(a)}}\right)g'(c).}]
      Therefore:
                f &#x2032;  ( c ) =    f ( b ) &#x2212; f ( a )   g ( b )
            &#x2212; g ( a )     g &#x2032;  ( c ) ,   {\displaystyle f'(c)=
            {\frac {f(b)-f(a)}{g(b)-g(a)}}g'(c),}  [{\displaystyle f'(c)={\frac
            {f(b)-f(a)}{g(b)-g(a)}}g'(c),}]
      which implies the result.[4]
    * If g(a) = g(b), then, applying Rolle's_theorem to g, it follows that
      there exists c in (a, b) for which gâ²(c) = 0. Using this choice of c,
      Cauchy's mean value theorem (trivially) holds.
***** Generalization for determinants[edit] *****
Assume that     f , g ,   {\displaystyle f,g,}  [{\displaystyle f,g,}] and
h   {\displaystyle h}  [h] are differentiable functions on     ( a , b )
{\displaystyle (a,b)}  [(a,b)] that are continuous on     [ a , b ]
{\displaystyle [a,b]}  [[a,b]]. Define
         D ( x ) =  |     f ( x )   g ( x )   h ( x )     f ( a )   g ( a )   h
      ( a )     f ( b )   g ( b )   h ( b )     |    {\displaystyle D(x)=\left|
      {\begin{array}{ccc}f(x)&g(x)&h(x)\\f(a)&g(a)&h(a)\\f(b)&g(b)&h(b)\end
      {array}}\right|}  [{\displaystyle D(x)=\left|{\begin{array}{ccc}f(x)&g
      (x)&h(x)\\f(a)&g(a)&h(a)\\f(b)&g(b)&h(b)\end{array}}\right|}]
There exists     c &#x2208; ( a , b )   {\displaystyle c\in (a,b)}  [c\in
(a,b)] such that      D &#x2032;  ( c ) = 0   {\displaystyle D'(c)=0}  [D'
(c)=0].
Notice that
          D &#x2032;  ( x ) =  |      f &#x2032;  ( x )    g &#x2032;  ( x )
      h &#x2032;  ( x )     f ( a )   g ( a )   h ( a )     f ( b )   g ( b )
      h ( b )     |    {\displaystyle D'(x)=\left|{\begin{array}{ccc}f'(x)&g'
      (x)&h'(x)\\f(a)&g(a)&h(a)\\f(b)&g(b)&h(b)\end{array}}\right|}  [
      {\displaystyle D'(x)=\left|{\begin{array}{ccc}f'(x)&g'(x)&h'(x)\\f(a)&g
      (a)&h(a)\\f(b)&g(b)&h(b)\end{array}}\right|}]
and if we place     h ( x ) = 1   {\displaystyle h(x)=1}  [h(x)=1], we get
Cauchy's mean value theorem. If we place     h ( x ) = 1   {\displaystyle h
(x)=1}  [h(x)=1] and     g ( x ) = x   {\displaystyle g(x)=x}  [g(x)=x] we get
Lagrange's mean value theorem.
The proof of the generalization is quite simple: each of     D ( a )
{\displaystyle D(a)}  [D(a)] and     D ( b )   {\displaystyle D(b)}  [D(b)] are
determinants with two identical rows, hence     D ( a ) = D ( b ) = 0
{\displaystyle D(a)=D(b)=0}  [D(a)=D(b)=0]. The Rolle's theorem implies that
there exists     c &#x2208; ( a , b )   {\displaystyle c\in (a,b)}  [c\in
(a,b)] such that      D &#x2032;  ( c ) = 0   {\displaystyle D'(c)=0}  [D'
(c)=0].
***** Mean value theorem in several variables[edit] *****
The mean value theorem generalizes to real functions of multiple variables. The
trick is to use parametrization to create a real function of one variable, and
then apply the one-variable theorem.
Let     G   {\displaystyle G}  [G] be an open convex subset of       R   n
{\displaystyle \mathbb {R} ^{n}}  [\mathbb {R} ^{n}] , and let     f : G
&#x2192;  R    {\displaystyle f:G\to \mathbb {R} }  [{\displaystyle f:G\to
\mathbb {R} }] be a differentiable function. Fix points     x , y &#x2208; G
{\displaystyle x,y\in G}  [x,y\in G] , and define     g ( t ) = f   (   ( 1
&#x2212; t ) x + t y   )     {\displaystyle g(t)=f{\Big (}(1-t)x+ty{\Big )}}  [
{\displaystyle g(t)=f{\Big (}(1-t)x+ty{\Big )}}] . Since     g   {\displaystyle
g}  [g] is a differentiable function in one variable, the mean value theorem
gives:
         g ( 1 ) &#x2212; g ( 0 ) =  g &#x2032;  ( c )   {\displaystyle g(1)-g
      (0)=g'(c)}  [{\displaystyle g(1)-g(0)=g'(c)}]
for some     c   {\displaystyle c}  [c] between 0 and 1. But since     g ( 1 )
= f ( y )   {\displaystyle g(1)=f(y)}  [{\displaystyle g(1)=f(y)}] and     g
( 0 ) = f ( x )   {\displaystyle g(0)=f(x)}  [{\displaystyle g(0)=f(x)}] ,
computing      g &#x2032;  ( c )   {\displaystyle g'(c)}  [{\displaystyle g'
(c)}] explicitly we have:
         f ( y ) &#x2212; f ( x ) = &#x2207; f   (   ( 1 &#x2212; c ) x + c y
      )   &#x22C5; ( y &#x2212; x )   {\displaystyle f(y)-f(x)=\nabla f{\Big (}
      (1-c)x+cy{\Big )}\cdot (y-x)}  [{\displaystyle f(y)-f(x)=\nabla f{\Big (}
      (1-c)x+cy{\Big )}\cdot (y-x)}]
where     &#x2207;   {\displaystyle \nabla }  [\nabla ] denotes a gradient and
&#x22C5;   {\displaystyle \cdot }  [\cdot ] a dot_product. Note that this is an
exact analog of the theorem in one variable (in the case     n = 1
{\displaystyle n=1}  [n=1] this is the theorem in one variable). By the
CauchyâSchwarz_inequality, the equation gives the estimate:
           |   f ( y ) &#x2212; f ( x )   |   &#x2264;   |   &#x2207; f   (
      ( 1 &#x2212; c ) x + c y   )     |   &#xA0;   |   y &#x2212; x   |   .
      {\displaystyle {\Bigg |}f(y)-f(x){\Bigg |}\leq {\Bigg |}\nabla f{\Big (}
      (1-c)x+cy{\Big )}{\Bigg |}\ {\Big |}y-x{\Big |}.}  [{\displaystyle {\Bigg
      |}f(y)-f(x){\Bigg |}\leq {\Bigg |}\nabla f{\Big (}(1-c)x+cy{\Big )}{\Bigg
      |}\ {\Big |}y-x{\Big |}.}]
In particular, when the partial derivatives of     f   {\displaystyle f}  [f]
are bounded,     f   {\displaystyle f}  [f] is Lipschitz_continuous (and
therefore uniformly_continuous). Note that     f   {\displaystyle f}  [f] is
not assumed to be continuously differentiable or continuous on the closure of
G   {\displaystyle G}  [G] . However, in order to use the chain rule to compute
g &#x2032;    {\displaystyle g'}  [{\displaystyle g'}], we really do need to
know that     f   {\displaystyle f}  [f] is differentiable on     G
{\displaystyle G}  [G]; the existence of the     x   {\displaystyle x}  [x] and
y   {\displaystyle y}  [y] partial derivatives by itself is not sufficient for
the theorem to be true[clarification_needed].
As an application of the above, we prove that     f   {\displaystyle f}  [f] is
constant if     G   {\displaystyle G}  [G] is open and connected and every
partial derivative of     f   {\displaystyle f}  [f] is 0. Pick some point
x  0   &#x2208; G   {\displaystyle x_{0}\in G}  [{\displaystyle x_{0}\in G}] ,
and let     g ( x ) = f ( x ) &#x2212; f (  x  0   )   {\displaystyle g(x)=f
(x)-f(x_{0})}  [{\displaystyle g(x)=f(x)-f(x_{0})}] . We want to show     g ( x
) = 0   {\displaystyle g(x)=0}  [g(x)=0] for every     x &#x2208; G
{\displaystyle x\in G}  [x\in G] . For that, let     E = { x &#x2208; G : g ( x
) = 0 }   {\displaystyle E=\{x\in G:g(x)=0\}}  [{\displaystyle E=\{x\in G:g
(x)=0\}}] . Then E is closed and nonempty. It is open too: for every     x
&#x2208; E   {\displaystyle x\in E}  [x\in E] ,
           |   g ( y )   |   =   |   g ( y ) &#x2212; g ( x )   |   &#x2264;
      ( 0 )   |   y &#x2212; x   |   = 0   {\displaystyle {\Big |}g(y){\Big |}=
      {\Bigg |}g(y)-g(x){\Bigg |}\leq (0){\Big |}y-x{\Big |}=0}  [
      {\displaystyle {\Big |}g(y){\Big |}={\Bigg |}g(y)-g(x){\Bigg |}\leq (0)
      {\Big |}y-x{\Big |}=0}]
for every     y   {\displaystyle y}  [y] in some neighborhood of     x
{\displaystyle x}  [x] . (Here, it is crucial that     x   {\displaystyle x}
[x] and     y   {\displaystyle y}  [y] are sufficiently close to each other.)
Since     G   {\displaystyle G}  [G] is connected, we conclude     E = G
{\displaystyle E=G}  [{\displaystyle E=G}] .
The above arguments are made in a coordinate-free manner; hence, they
generalize to the case when     G   {\displaystyle G}  [G] is a subset of a
Banach space.
***** Mean value theorem for vector-valued functions[edit] *****
There is no exact analog of the mean value theorem for vector-valued functions.
In Principles of Mathematical Analysis, Rudin gives an inequality which can be
applied to many of the same situations to which the mean value theorem is
applicable in the one dimensional case:[7]
Theorem. For a continuous vector-valued function      f  : [ a , b ] &#x2192;
R   k     {\displaystyle \mathbf {f} :[a,b]\to \mathbb {R} ^{k}}  [
{\displaystyle \mathbf {f} :[a,b]\to \mathbb {R} ^{k}}] differentiable on
( a , b )   {\displaystyle (a,b)}  [(a,b)], there exists     x &#x2208; ( a , b
)   {\displaystyle x\in (a,b)}  [x\in (a,b)] such that      |    f  &#x2032;
( x )  |  &#x2265;   1  b &#x2212; a     |   f  ( b ) &#x2212;  f  ( a )  |
{\displaystyle |\mathbf {f} '(x)|\geq {\frac {1}{b-a}}|\mathbf {f} (b)-\mathbf
{f} (a)|}  [{\displaystyle |\mathbf {f} '(x)|\geq {\frac {1}{b-a}}|\mathbf {f}
(b)-\mathbf {f} (a)|}].
Jean_DieudonnÃ© in his classic treatise Foundations of Modern Analysis discards
the mean value theorem and replaces it by mean inequality as the proof is not
constructive and one cannot find the mean value and in applications one only
needs mean inequality. Serge_Lang in Analysis Iuses the mean value theorem, in
integral form, as an instant reflex but this use requires the continuity of the
derivative. If one uses the HenstockâKurzweil_integral one can have the mean
value theorem in integral form without the additional assumption that
derivative should be continuous as every derivative is HenstockâKurzweil
integrable. The problem is roughly speaking the following: If f : U â Rm is a
differentiable function (where U â Rn is open) and if x + th, x, h â Rn, t
â [0, 1] is the line segment in question (lying inside U), then one can apply
the above parametrization procedure to each of the component functions fi (i =
1, ..., m) of f (in the above notation set y = x + h). In doing so one finds
points x + tih on the line segment satisfying
          f  i   ( x + h ) &#x2212;  f  i   ( x ) = &#x2207;  f  i   ( x +  t
      i   h ) &#x22C5; h .   {\displaystyle f_{i}(x+h)-f_{i}(x)=\nabla f_{i}
      (x+t_{i}h)\cdot h.}  [{\displaystyle f_{i}(x+h)-f_{i}(x)=\nabla f_{i}
      (x+t_{i}h)\cdot h.}]
But generally there will not be a single point x + t*h on the line segment
satisfying
          f  i   ( x + h ) &#x2212;  f  i   ( x ) = &#x2207;  f  i   ( x +  t
      &#x2217;   h ) &#x22C5; h .   {\displaystyle f_{i}(x+h)-f_{i}(x)=\nabla
      f_{i}(x+t^{*}h)\cdot h.}  [{\displaystyle f_{i}(x+h)-f_{i}(x)=\nabla f_
      {i}(x+t^{*}h)\cdot h.}]
for all i simultaneously. For example, define:
           {    f : [ 0 , 2 &#x03C0; ] &#x2192;   R   2       f ( x ) = ( cos
      &#x2061; ( x ) , sin &#x2061; ( x ) )         {\displaystyle {\begin
      {cases}f:[0,2\pi ]\to \mathbf {R} ^{2}\\f(x)=(\cos(x),\sin(x))\end
      {cases}}}  [{\displaystyle {\begin{cases}f:[0,2\pi ]\to \mathbf {R} ^
      {2}\\f(x)=(\cos(x),\sin(x))\end{cases}}}]
Then     f ( 2 &#x03C0; ) &#x2212; f ( 0 ) =  0  &#x2208;   R   2
{\displaystyle f(2\pi )-f(0)=\mathbf {0} \in \mathbf {R} ^{2}}  [{\displaystyle
f(2\pi )-f(0)=\mathbf {0} \in \mathbf {R} ^{2}}], but      f  1  &#x2032;  ( x
) = &#x2212; sin &#x2061; ( x )   {\displaystyle f_{1}'(x)=-\sin(x)}  [
{\displaystyle f_{1}'(x)=-\sin(x)}] and      f  2  &#x2032;  ( x ) = cos
&#x2061; ( x )   {\displaystyle f_{2}'(x)=\cos(x)}  [{\displaystyle f_{2}'
(x)=\cos(x)}] are never simultaneously zero as     x   {\displaystyle x}  [x]
ranges over      [  0 , 2 &#x03C0;  ]    {\displaystyle \left[0,2\pi \right]}
[{\displaystyle \left[0,2\pi \right]}].
However a certain type of generalization of the mean value theorem to vector-
valued functions is obtained as follows: Let f be a continuously differentiable
real-valued function defined on an open interval I, and let x as well as x + h
be points of I. The mean value theorem in one variable tells us that there
exists some t* between 0 and 1 such that
         f ( x + h ) &#x2212; f ( x ) =  f &#x2032;  ( x +  t  &#x2217;   h )
      &#x22C5; h .   {\displaystyle f(x+h)-f(x)=f'(x+t^{*}h)\cdot h.}  [
      {\displaystyle f(x+h)-f(x)=f'(x+t^{*}h)\cdot h.}]
On the other hand, we have, by the fundamental_theorem_of_calculus followed by
a change of variables,
         f ( x + h ) &#x2212; f ( x ) =  &#x222B;  x   x + h    f &#x2032;  ( u
      )  d u =  (   &#x222B;  0   1    f &#x2032;  ( x + t h )  d t  )
      &#x22C5; h .   {\displaystyle f(x+h)-f(x)=\int _{x}^{x+h}f'(u)\,du=\left
      (\int _{0}^{1}f'(x+th)\,dt\right)\cdot h.}  [{\displaystyle f(x+h)-f
      (x)=\int _{x}^{x+h}f'(u)\,du=\left(\int _{0}^{1}f'(x+th)\,dt\right)\cdot
      h.}]
Thus, the value fâ²(x + t*h) at the particular point t* has been replaced by
the mean value
          &#x222B;  0   1    f &#x2032;  ( x + t h )  d t .   {\displaystyle
      \int _{0}^{1}f'(x+th)\,dt.}  [\int _{0}^{1}f'(x+th)\,dt.]
This last version can be generalized to vector valued functions:
      Lemma 1. Let U â Rn be open, f : U â Rm continuously differentiable,
      and x â U, h â Rn vectors such that the line segment x + th, 0 â¤ t
      â¤ 1 remains in U. Then we have:
               f ( x + h ) &#x2212; f ( x ) =  (   &#x222B;  0   1   D f ( x +
            t h )  d t  )  &#x22C5; h ,   {\displaystyle f(x+h)-f(x)=\left(\int
            _{0}^{1}Df(x+th)\,dt\right)\cdot h,}  [{\displaystyle f(x+h)-f
            (x)=\left(\int _{0}^{1}Df(x+th)\,dt\right)\cdot h,}]
      where Df denotes the Jacobian_matrix of f and the integral of a matrix is
      to be understood componentwise.
Proof. Let f1, ..., fm denote the components of f and define:
           {     g  i   : [ 0 , 1 ] &#x2192;  R       g  i   ( t ) =  f  i
      ( x + t h )         {\displaystyle {\begin{cases}g_{i}:[0,1]\to \mathbf
      {R} \\g_{i}(t)=f_{i}(x+th)\end{cases}}}  [{\displaystyle {\begin{cases}g_
      {i}:[0,1]\to \mathbf {R} \\g_{i}(t)=f_{i}(x+th)\end{cases}}}]
Then we have
               f  i   ( x + h ) &#x2212;  f  i   ( x ) =  g  i   ( 1 ) &#x2212;
      g  i   ( 0 ) =  &#x222B;  0   1    g  i  &#x2032;  ( t )  d t     =
      &#x222B;  0   1    (   &#x2211;  j = 1   n      &#x2202;  f  i
      &#x2202;  x  j      ( x + t h )  h  j    )   d t =  &#x2211;  j = 1   n
      (   &#x222B;  0   1      &#x2202;  f  i     &#x2202;  x  j      ( x + t h
      )  d t  )   h  j   .       {\displaystyle {\begin{aligned}&f_{i}(x+h)-f_
      {i}(x)=g_{i}(1)-g_{i}(0)=\int _{0}^{1}g_{i}'(t)\,dt\\={}&\int _{0}^
      {1}\left(\sum _{j=1}^{n}{\frac {\partial f_{i}}{\partial x_{j}}}(x+th)h_
      {j}\right)\,dt=\sum _{j=1}^{n}\left(\int _{0}^{1}{\frac {\partial f_{i}}
      {\partial x_{j}}}(x+th)\,dt\right)h_{j}.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}&f_{i}(x+h)-f_{i}(x)=g_{i}(1)-g_{i}(0)=\int _{0}^{1}g_
      {i}'(t)\,dt\\={}&\int _{0}^{1}\left(\sum _{j=1}^{n}{\frac {\partial f_
      {i}}{\partial x_{j}}}(x+th)h_{j}\right)\,dt=\sum _{j=1}^{n}\left(\int _
      {0}^{1}{\frac {\partial f_{i}}{\partial x_{j}}}(x+th)\,dt\right)h_
      {j}.\end{aligned}}}]
The claim follows since Df is the matrix consisting of the components
&#x2202;  f  i     &#x2202;  x  j       .   {\displaystyle {\tfrac {\partial f_
{i}}{\partial x_{j}}}.}  [{\displaystyle {\tfrac {\partial f_{i}}{\partial x_
{j}}}.}]
      Lemma 2. Let v : [a, b] â Rm be a continuous function defined on the
      interval [a, b] â R. Then we have
                &#x2016;   &#x222B;  a   b   v ( t )  d t  &#x2016;  &#x2A7D;
            &#x222B;  a   b   &#x2016; v ( t ) &#x2016;  d t .   {\displaystyle
            \left\|\int _{a}^{b}v(t)\,dt\right\|\leqslant \int _{a}^{b}\|v
            (t)\|\,dt.}  [{\displaystyle \left\|\int _{a}^{b}v
            (t)\,dt\right\|\leqslant \int _{a}^{b}\|v(t)\|\,dt.}]
Proof. Let u in Rm denote the value of the integral
         u :=  &#x222B;  a   b   v ( t )  d t .   {\displaystyle u:=\int _{a}^
      {b}v(t)\,dt.}  [u:=\int _{a}^{b}v(t)\,dt.]
Now we have (using the CauchyâSchwarz_inequality):
         &#x2016; u  &#x2016;  2   = &#x27E8; u , u &#x27E9; =  &#x27E8;
      &#x222B;  a   b   v ( t )  d t , u  &#x27E9;  =  &#x222B;  a   b
      &#x27E8; v ( t ) , u &#x27E9;  d t &#x2A7D;  &#x222B;  a   b   &#x2016; v
      ( t ) &#x2016; &#x22C5; &#x2016; u &#x2016;  d t = &#x2016; u &#x2016;
      &#x222B;  a   b   &#x2016; v ( t ) &#x2016;  d t   {\displaystyle \|u\|^
      {2}=\langle u,u\rangle =\left\langle \int _{a}^{b}v(t)\,dt,u\right\rangle
      =\int _{a}^{b}\langle v(t),u\rangle \,dt\leqslant \int _{a}^{b}\|v
      (t)\|\cdot \|u\|\,dt=\|u\|\int _{a}^{b}\|v(t)\|\,dt}  [{\displaystyle
      \|u\|^{2}=\langle u,u\rangle =\left\langle \int _{a}^{b}v
      (t)\,dt,u\right\rangle =\int _{a}^{b}\langle v(t),u\rangle \,dt\leqslant
      \int _{a}^{b}\|v(t)\|\cdot \|u\|\,dt=\|u\|\int _{a}^{b}\|v(t)\|\,dt}]
Now cancelling the norm of u from both ends gives us the desired inequality.
      Mean Value Inequality. If the norm of Df(x + th) is bounded by some
      constant M for t in [0, 1], then
               &#x2016; f ( x + h ) &#x2212; f ( x ) &#x2016; &#x2A7D; M
            &#x2016; h &#x2016; .   {\displaystyle \|f(x+h)-f(x)\|\leqslant
            M\|h\|.}  [{\displaystyle \|f(x+h)-f(x)\|\leqslant M\|h\|.}]
Proof. From Lemma 1 and 2 it follows that
         &#x2016; f ( x + h ) &#x2212; f ( x ) &#x2016; =  &#x2016;   &#x222B;
      0   1   ( D f ( x + t h ) &#x22C5; h )  d t  &#x2016;  &#x2A7D;  &#x222B;
      0   1   &#x2016; D f ( x + t h ) &#x2016; &#x22C5; &#x2016; h &#x2016;  d
      t &#x2A7D; M &#x2016; h &#x2016; .   {\displaystyle \|f(x+h)-f
      (x)\|=\left\|\int _{0}^{1}(Df(x+th)\cdot h)\,dt\right\|\leqslant \int _
      {0}^{1}\|Df(x+th)\|\cdot \|h\|\,dt\leqslant M\|h\|.}  [{\displaystyle \|f
      (x+h)-f(x)\|=\left\|\int _{0}^{1}(Df(x+th)\cdot h)\,dt\right\|\leqslant
      \int _{0}^{1}\|Df(x+th)\|\cdot \|h\|\,dt\leqslant M\|h\|.}]
***** Mean value theorems for definite integrals[edit] *****
**** First mean value theorem for definite integrals[edit] ****
Geometrically: interpreting f(c) as the height of a rectangle and bâa as the
width, this rectangle has the same area as the region below the curve from a to
b[8]
Let f : [a, b] â R be a continuous function. Then there exists c in (a, b)
such that
          &#x222B;  a   b   f ( x )  d x = f ( c ) ( b &#x2212; a ) .
      {\displaystyle \int _{a}^{b}f(x)\,dx=f(c)(b-a).}  [\int _{a}^{b}f
      (x)\,dx=f(c)(b-a).]
Since the mean value of f on [a, b] is defined as
           1  b &#x2212; a     &#x222B;  a   b   f ( x )  d x ,
      {\displaystyle {\frac {1}{b-a}}\int _{a}^{b}f(x)\,dx,}  [{\frac {1}{b-
      a}}\int _{a}^{b}f(x)\,dx,]
we can interpret the conclusion as f achieves its mean value at some c in (a,
b).[9]
In general, if f : [a, b] â R is continuous and g is an integrable function
that does not change sign on [a, b], then there exists c in (a, b) such that
          &#x222B;  a   b   f ( x ) g ( x )  d x = f ( c )  &#x222B;  a   b   g
      ( x )  d x .   {\displaystyle \int _{a}^{b}f(x)g(x)\,dx=f(c)\int _{a}^
      {b}g(x)\,dx.}  [\int _{a}^{b}f(x)g(x)\,dx=f(c)\int _{a}^{b}g(x)\,dx.]
**** Proof of the first mean value theorem for definite integrals[edit] ****
Suppose f : [a, b] â R is continuous and g is a nonnegative integrable
function on [a, b]. By the extreme_value_theorem, there exists m and M such
that for each x in [a, b],     m &#x2A7D; f ( x ) &#x2A7D; M   {\displaystyle
m\leqslant f(x)\leqslant M}  [{\displaystyle m\leqslant f(x)\leqslant M}] and
f [ a , b ] = [ m , M ]   {\displaystyle f[a,b]=[m,M]}  [{\displaystyle f[a,b]=
[m,M]}]. Since g is nonnegative,
         m  &#x222B;  a   b   g ( x )  d x &#x2A7D;  &#x222B;  a   b   f ( x )
      g ( x )  d x &#x2A7D; M  &#x222B;  a   b   g ( x )  d x .
      {\displaystyle m\int _{a}^{b}g(x)\,dx\leqslant \int _{a}^{b}f(x)g
      (x)\,dx\leqslant M\int _{a}^{b}g(x)\,dx.}  [{\displaystyle m\int _{a}^
      {b}g(x)\,dx\leqslant \int _{a}^{b}f(x)g(x)\,dx\leqslant M\int _{a}^{b}g
      (x)\,dx.}]
Now let
         I =  &#x222B;  a   b   g ( x )  d x .   {\displaystyle I=\int _{a}^
      {b}g(x)\,dx.}  [I=\int _{a}^{b}g(x)\,dx.]
If     I = 0   {\displaystyle I=0}  [I=0], we're done since
         0 &#x2A7D;  &#x222B;  a   b   f ( x ) g ( x )  d x &#x2A7D; 0
      {\displaystyle 0\leqslant \int _{a}^{b}f(x)g(x)\,dx\leqslant 0}  [
      {\displaystyle 0\leqslant \int _{a}^{b}f(x)g(x)\,dx\leqslant 0}]
means
          &#x222B;  a   b   f ( x ) g ( x )  d x = 0 ,   {\displaystyle \int _
      {a}^{b}f(x)g(x)\,dx=0,}  [\int _{a}^{b}f(x)g(x)\,dx=0,]
so for any c in (a, b),
          &#x222B;  a   b   f ( x ) g ( x )  d x = f ( c ) I = 0.
      {\displaystyle \int _{a}^{b}f(x)g(x)\,dx=f(c)I=0.}  [{\displaystyle \int
      _{a}^{b}f(x)g(x)\,dx=f(c)I=0.}]
If I â  0, then
         m &#x2A7D;   1 I    &#x222B;  a   b   f ( x ) g ( x )  d x &#x2A7D; M
      .   {\displaystyle m\leqslant {\frac {1}{I}}\int _{a}^{b}f(x)g
      (x)\,dx\leqslant M.}  [{\displaystyle m\leqslant {\frac {1}{I}}\int _{a}^
      {b}f(x)g(x)\,dx\leqslant M.}]
By the intermediate_value_theorem, f attains every value of the interval [m,
M], so for some c in [a, b]
         f ( c ) =   1 I    &#x222B;  a   b   f ( x ) g ( x )  d x ,
      {\displaystyle f(c)={\frac {1}{I}}\int _{a}^{b}f(x)g(x)\,dx,}  [f(c)=
      {\frac {1}{I}}\int _{a}^{b}f(x)g(x)\,dx,]
that is,
          &#x222B;  a   b   f ( x ) g ( x )  d x = f ( c )  &#x222B;  a   b   g
      ( x )  d x .   {\displaystyle \int _{a}^{b}f(x)g(x)\,dx=f(c)\int _{a}^
      {b}g(x)\,dx.}  [\int _{a}^{b}f(x)g(x)\,dx=f(c)\int _{a}^{b}g(x)\,dx.]
Finally, if g is negative on [a, b], then
         M  &#x222B;  a   b   g ( x )  d x &#x2A7D;  &#x222B;  a   b   f ( x )
      g ( x )  d x &#x2A7D; m  &#x222B;  a   b   g ( x )  d x ,
      {\displaystyle M\int _{a}^{b}g(x)\,dx\leqslant \int _{a}^{b}f(x)g
      (x)\,dx\leqslant m\int _{a}^{b}g(x)\,dx,}  [{\displaystyle M\int _{a}^
      {b}g(x)\,dx\leqslant \int _{a}^{b}f(x)g(x)\,dx\leqslant m\int _{a}^{b}g
      (x)\,dx,}]
and we still get the same result as above.
QED
**** Second mean value theorem for definite integrals[edit] ****
There are various slightly different theorems called the second mean value
theorem for definite integrals. A commonly found version is as follows:
      If G : [a, b] â R is a positive monotonically_decreasing function and
      Ï : [a, b] â R is an integrable function, then there exists a number x
      in (a, b] such that
                &#x222B;  a   b   G ( t ) &#x03C6; ( t )  d t = G (  a  +   )
            &#x222B;  a   x   &#x03C6; ( t )  d t .   {\displaystyle \int _{a}^
            {b}G(t)\varphi (t)\,dt=G(a^{+})\int _{a}^{x}\varphi (t)\,dt.}
            [\int _{a}^{b}G(t)\varphi (t)\,dt=G(a^{+})\int _{a}^{x}\varphi
            (t)\,dt.]
Here     G (  a  +   )   {\displaystyle G(a^{+})}  [G(a^{+})] stands for
lim  x &#x2192;  a  +     G ( x )    {\displaystyle {\lim _{x\to a^{+}}G(x)}}
[{\lim _{x\to a^{+}}G(x)}], the existence of which follows from the conditions.
Note that it is essential that the interval (a, b] contains b. A variant not
having this requirement is:[10]
      If G : [a, b] â R is a monotonic (not necessarily decreasing and
      positive) function and Ï : [a, b] â R is an integrable function, then
      there exists a number x in (a, b) such that
                &#x222B;  a   b   G ( t ) &#x03C6; ( t )  d t = G (  a  +   )
            &#x222B;  a   x   &#x03C6; ( t )  d t + G (  b  &#x2212;   )
            &#x222B;  x   b   &#x03C6; ( t )  d t .   {\displaystyle \int _{a}^
            {b}G(t)\varphi (t)\,dt=G(a^{+})\int _{a}^{x}\varphi (t)\,dt+G(b^{-
            })\int _{x}^{b}\varphi (t)\,dt.}  [\int _{a}^{b}G(t)\varphi
            (t)\,dt=G(a^{+})\int _{a}^{x}\varphi (t)\,dt+G(b^{-})\int _{x}^
            {b}\varphi (t)\,dt.]
**** Mean value theorem for integration fails for vector-valued functions[edit]
****
If the function     G   {\displaystyle G}  [G] returns a multi-dimensional
vector, then the MVT for integration is not true, even if the domain of     G
{\displaystyle G}  [G] is also multi-dimensional.
For example, consider the following 2-dimensional function defined on an     n
{\displaystyle n}  [n]-dimensional cube:
           {    G : [ 0 , 2 &#x03C0;  ]  n   &#x2192;   R   2       G (  x  1
      , &#x22EF; ,  x  n   ) =  (  sin &#x2061; (  x  1   + &#x22EF; +  x  n
      ) , cos &#x2061; (  x  1   + &#x22EF; +  x  n   )  )
      {\displaystyle {\begin{cases}G:[0,2\pi ]^{n}\to \mathbb {R} ^{2}\\G(x_
      {1},\cdots ,x_{n})=\left(\sin(x_{1}+\cdots +x_{n}),\cos(x_{1}+\cdots +x_
      {n})\right)\end{cases}}}  [{\displaystyle {\begin{cases}G:[0,2\pi ]^
      {n}\to \mathbb {R} ^{2}\\G(x_{1},\cdots ,x_{n})=\left(\sin(x_{1}+\cdots
      +x_{n}),\cos(x_{1}+\cdots +x_{n})\right)\end{cases}}}]
Then, by symmetry it is easy to see that the mean value of     G
{\displaystyle G}  [G] over its domain is (0,0):
          &#x222B;  [ 0 , 2 &#x03C0;  ]  n     G (  x  1   , &#x22EF; ,  x  n
      ) d  x  1   &#x22EF; d  x  n   = ( 0 , 0 )   {\displaystyle \int _{
      [0,2\pi ]^{n}}G(x_{1},\cdots ,x_{n})dx_{1}\cdots dx_{n}=(0,0)}  [\int _{
      [0,2\pi ]^{n}}G(x_{1},\cdots ,x_{n})dx_{1}\cdots dx_{n}=(0,0)]
However, there is no point in which     G = ( 0 , 0 )   {\displaystyle G=(0,0)}
[G=(0,0)], because      |  G  |  = 1   {\displaystyle |G|=1}  [|G|=1]
everywhere.
***** A probabilistic analogue of the mean value theorem[edit] *****
Let X and Y be non-negative random_variables such that E[X] < E[Y] < â and
X  &#x2A7D;  s t   Y   {\displaystyle X\leqslant _{st}Y}  [{\displaystyle
X\leqslant _{st}Y}] (i.e. X is smaller than Y in the usual_stochastic_order).
Then there exists an absolutely continuous non-negative random variable Z
having probability_density_function
          f  Z   ( x ) =    Pr ( Y > x ) &#x2212; Pr ( X > x )     E   [ Y ]
      &#x2212;   E   [ X ]     ,  x &#x2A7E; 0.   {\displaystyle f_{Z}(x)={\Pr
      (Y>x)-\Pr(X>x) \over {\rm {E}}[Y]-{\rm {E}}[X]}\,,\qquad x\geqslant 0.}
      [{\displaystyle f_{Z}(x)={\Pr(Y>x)-\Pr(X>x) \over {\rm {E}}[Y]-{\rm {E}}
      [X]}\,,\qquad x\geqslant 0.}]
Let g be a measurable and differentiable_function such that E[g(X)], E[g(Y)] <
â, and let its derivative gâ² be measurable and Riemann-integrable on the
interval [x, y] for all y â¥ x â¥ 0. Then, E[gâ²(Z)] is finite and[11]
           E   [ g ( Y ) ] &#x2212;   E   [ g ( X ) ] =   E   [  g &#x2032;
      ( Z ) ]  [   E   ( Y ) &#x2212;   E   ( X ) ] .   {\displaystyle {\rm
      {E}}[g(Y)]-{\rm {E}}[g(X)]={\rm {E}}[g'(Z)]\,[{\rm {E}}(Y)-{\rm {E}}
      (X)].}  [{\rm {E}}[g(Y)]-{\rm {E}}[g(X)]={\rm {E}}[g'(Z)]\,[{\rm {E}}(Y)-
      {\rm {E}}(X)].]
***** Generalization in complex analysis[edit] *****
As noted above, the theorem does not hold for differentiable complex-valued
functions. Instead, a generalization of the theorem is stated such:[12]
Let f : Î© â C be a holomorphic_function on the open convex set Î©, and let a
and b be distinct points in Î©. Then there exist points u, v on Lab (the line
segment from a to b) such that
          R e  (  f &#x2032;  ( u ) ) =  R e   (    f ( b ) &#x2212; f ( a )
      b &#x2212; a    )  ,   {\displaystyle \mathrm {Re} (f'(u))=\mathrm {Re}
      \left({\frac {f(b)-f(a)}{b-a}}\right),}  [{\displaystyle \mathrm {Re} (f'
      (u))=\mathrm {Re} \left({\frac {f(b)-f(a)}{b-a}}\right),}]
          I m  (  f &#x2032;  ( v ) ) =  I m   (    f ( b ) &#x2212; f ( a )
      b &#x2212; a    )  .   {\displaystyle \mathrm {Im} (f'(v))=\mathrm {Im}
      \left({\frac {f(b)-f(a)}{b-a}}\right).}  [{\displaystyle \mathrm {Im} (f'
      (v))=\mathrm {Im} \left({\frac {f(b)-f(a)}{b-a}}\right).}]
Where Re() is the Real part and Im() is the Imaginary part of a complex-valued
function.
***** See also[edit] *****
    * Newmark-beta_method
    * Mean_value_theorem_(divided_differences)
    * Racetrack_principle
    * Stolarsky_mean
***** Notes[edit] *****
   1. ^Weisstein, Eric. "Mean-Value_Theorem". MathWorld. Wolfram_Research.
      Retrieved 24 March 2011.
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
   3. ^ J. J. O'Connor and E. F. Robertson (2000). Paramesvara, MacTutor
      History_of_Mathematics_archive.
   4. ^ÃdÃ¡m Besenyei. "Historical_development_of_the_mean_value_theorem"
      (PDF).
   5. ^ a b cKirshna's_Real_Analysis:_(General). Krishna Prakashan Media.
   6. ^W., Weisstein, Eric. "Extended_Mean-Value_Theorem".
      mathworld.wolfram.com. Retrieved 2018-10-08.
   7. ^"Cauchy's_Mean_Value_Theorem". Math24. Retrieved 2018-10-08.
   8. ^Rudin, Walter (1976). Principles_of_Mathematical_Analysis_(3rd_ed.). New
      York: McGraw-Hill. p. 113. ISBN 978-0-07-054235-8.
   9. ^"Mathwords:_Mean_Value_Theorem_for_Integrals". www.mathwords.com.
  10. ^Michael Comenetz (2002). Calculus: The Elements. World Scientific.
      p. 159. ISBN 978-981-02-4904-5.
  11. ^Hobson, E. W. (1909). "On_the_Second_Mean-Value_Theorem_of_the_Integral
      Calculus". Proc._London_Math._Soc. S2â7 (1): 14â23. doi:10.1112/plms/
      s2-7.1.14. MR 1575669.
  12. ^Di Crescenzo, A. (1999). "A Probabilistic Analogue of the Mean Value
      Theorem and Its Applications to Reliability Theory". J._Appl._Probab. 36
      (3): 706â719. doi:10.1239/jap/1032374628. JSTOR 3215435.
  13. ^"Complex_Mean-Value_Theorem". PlanetMath. PlanetMath.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Cauchy_theorem", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
PlanetMath:_Mean-Value_Theorem
Weisstein,_Eric_W. "Mean_value_theorem". MathWorld.
Weisstein,_Eric_W. "Cauchy's_Mean-Value_Theorem". MathWorld.
"Mean_Value_Theorem:_Intuition_behind_the_Mean_Value_Theorem" at the Khan
Academy

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Mean_value_theorem&oldid=903310322"
Categories:
    * Theorems_in_calculus
    * Theorems_in_real_analysis
Hidden categories:
    * Wikipedia_articles_needing_clarification_from_March_2018
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
**** In other projects ****
    * Wikimedia_Commons
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * á áá­á
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AzÉrbaycanca
    * CatalÃ 
    * ÄeÅ¡tina
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
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 24 June 2019, at 23:10 (UTC).
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
