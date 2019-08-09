The following text has been accessed from https://en.wikipedia.org/wiki/Real_analysis at Fri Aug 9 02:34:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Real analysis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The first four partial sums of the Fourier_series for a square_wave. Fourier
series are an important tool in real analysis.
In mathematics, real analysis is the branch of mathematical_analysis that
studies the behavior of real_numbers, sequences and series of real numbers, and
real-valued_functions.[1] Some particular properties of real-valued sequences
and functions that real analysis studies include convergence, limits,
continuity, smoothness, differentiability and integrability.
Real analysis is distinguished from complex_analysis, which deals with the
study of complex_numbers and their functions.
⁰
***** Contents *****
    * 1_Scope
          o 1.1_Construction_of_the_real_numbers
          o 1.2_Order_properties_of_the_real_numbers
          o 1.3_Topological_properties_of_the_real_numbers
          o 1.4_Sequences
          o 1.5_Limits_and_convergence
                # 1.5.1_Uniform_and_pointwise_convergence_for_sequences_of
                  functions
          o 1.6_Compactness
          o 1.7_Continuity
                # 1.7.1_Uniform_continuity
                # 1.7.2_Absolute_continuity
          o 1.8_Differentiation
          o 1.9_Series
                # 1.9.1_Taylor_series
                # 1.9.2_Fourier_series
          o 1.10_Integration
                # 1.10.1_Riemann_integration
                # 1.10.2_Lebesgue_integration_and_measure
          o 1.11_Distributions
          o 1.12_Relation_to_complex_analysis
    * 2_Important_results
    * 3_Generalizations_and_related_areas_of_mathematics
    * 4_See_also
    * 5_References
    * 6_Bibliography
    * 7_External_links
***** Scope[edit] *****
 This article may require cleanup to meet Wikipedia's quality_standards. The
 specific problem is: This section goes too heavily into detail about each
 concept. It should just portray a brief overview in relation to the field of
 real analysis Please help improve_this_article if you can. (June 2019)(Learn
 how_and_when_to_remove_this_template_message)
**** Construction of the real numbers[edit] ****
Main article: Construction_of_the_real_numbers
The theorems of real analysis rely intimately upon the structure of the real
number line. The real number system consists of a set (     R    {\displaystyle
\mathbb {R} }  [\mathbb {R} ]), together with two binary_operations denoted +
and â, and an order denoted <. The operations make the real numbers a field,
and, along with the order, an ordered_field. The real number system is the
unique complete ordered field, in the sense that any other complete ordered
field is isomorphic to it. Intuitively, completeness means that there are no
'gaps' in the real numbers. In particular, this property distinguishes the real
numbers from other ordered fields (e.g., the rational numbers      Q
{\displaystyle \mathbb {Q} }  [\mathbb {Q} ]) and is critical to the proof of
several key properties of functions of the real numbers. The completeness of
the reals is often conveniently expressed as the least upper bound property
(see below).
There are several ways of formalizing the definition of the real_numbers.
Modern approaches consist of providing a list of axioms, and a proof of the
existence of a model for them, which has above properties. Moreover, one may
show that any two models are isomorphic, which means that all models have
exactly the same properties, and that one may forget how the model is
constructed for using real numbers. Some of these constructions are described
in the main article.
**** Order properties of the real numbers[edit] ****
The real numbers have several important lattice-theoretic properties that are
absent in the complex numbers. Most importantly, the real numbers form an
ordered_field, in which sums and products of positive numbers are also
positive. Moreover, the ordering of the real numbers is total, and the real
numbers have the least_upper_bound_property:
     Every nonempty subset of      R    {\displaystyle \mathbb {R} }
     [\mathbb {R} ] that has an upper bound has a least_upper_bound that
     is also a real number.
These order-theoretic properties lead to a number of important results in real
analysis, such as the monotone_convergence_theorem, the intermediate_value
theorem and the mean_value_theorem.
However, while the results in real analysis are stated for real numbers, many
of these results can be generalized to other mathematical objects. In
particular, many ideas in functional_analysis and operator_theory generalize
properties of the real numbers â such generalizations include the theories of
Riesz_spaces and positive_operators. Also, mathematicians consider real and
imaginary_parts of complex sequences, or by pointwise_evaluation of operator
sequences.
**** Topological properties of the real numbers[edit] ****
Many of the theorems of real analysis are consequences of the topological
properties of the real number line. The order properties of the real numbers
described above are closely related to these topological properties. As a
topological_space, the real numbers has a standard topology, which is the order
topology induced by order     <   {\displaystyle <}  [<]. Alternatively, by
defining the metric or distance function     d :  R  &#x00D7;  R  &#x2192;   R
&#x2265; 0     {\displaystyle d:\mathbb {R} \times \mathbb {R} \to \mathbb {R}
_{\geq 0}}  [{\displaystyle d:\mathbb {R} \times \mathbb {R} \to \mathbb {R} _
{\geq 0}}] using the absolute_value function as     d ( x , y ) =  |  x
&#x2212; y  |    {\displaystyle d(x,y)=|x-y|}  [d(x,y)=|x-y|], the real numbers
become the prototypical example of a metric_space. The topology induced by
metric     d   {\displaystyle d}  [d] turns out to be identical to the standard
topology induced by order     <   {\displaystyle <}  [<]. Theorems like the
intermediate_value_theorem that are essentially topological in nature can often
be proved in the more general setting of metric or topological spaces rather
than in      R    {\displaystyle \mathbb {R} }  [\mathbb {R} ] only. Often,
such proofs tend to be shorter or simpler compared to classical proofs that
apply direct methods.
**** Sequences[edit] ****
Main article: Sequence
A sequence is a function whose domain is a countable, totally_ordered set. The
domain is usually taken to be the natural_numbers[2], although it is
occasionally convenient to also consider bidirectional sequences indexed by the
set of all integers, including negative indices.
Of interest in real analysis, a real-valued sequence, here indexed by the
natural numbers, is a map     a :  N  &#x2192;  R  , &#xA0; n &#x21A6;  a  n
{\displaystyle a:\mathbb {N} \to \mathbb {R} ,\ n\mapsto a_{n}}  [
{\displaystyle a:\mathbb {N} \to \mathbb {R} ,\ n\mapsto a_{n}}]. Each     a
( n ) =  a  n     {\displaystyle a(n)=a_{n}}  [a(n)=a_{n}] is referred to as a
term (or, less commonly, an element) of the sequence. A sequence is rarely
denoted explicitly as a function; instead, by convention, it is almost always
notated as if it were an ordered â-tuple, with individual terms or a general
term enclosed in parentheses:
        (  a  n   ) = (  a  n    )  n &#x2208;  N    = (  a  1   ,  a  2
     ,  a  3   , &#x22EF; )   {\displaystyle (a_{n})=(a_{n})_{n\in \mathbb
     {N} }=(a_{1},a_{2},a_{3},\cdots )}  [{\displaystyle (a_{n})=(a_{n})_
     {n\in \mathbb {N} }=(a_{1},a_{2},a_{3},\cdots )}].[3]
A sequence that tends to a limit (i.e.,      lim  n &#x2192; &#x221E;    a  n
{\textstyle \lim _{n\to \infty }a_{n}}  [{\textstyle \lim _{n\to \infty }a_
{n}}] exists) is said to be convergent; otherwise it is divergent. (See the
section on limits and convergence for details.) A real-valued sequence     (  a
n   )   {\displaystyle (a_{n})}  [(a_{n})] is bounded if there exists     M
&#x2208;  R    {\displaystyle M\in \mathbb {R} }  [{\displaystyle M\in \mathbb
{R} }] such that      |   a  n    |  < M   {\displaystyle |a_{n}|<M}  [
{\displaystyle |a_{n}|<M}] for all     n &#x2208;  N    {\displaystyle n\in
\mathbb {N} }  [n\in \mathbb {N} ]. A real-valued sequence     (  a  n   )
{\displaystyle (a_{n})}  [(a_{n})] is monotonically increasing or decreasing if
         a  1   &#x2264;  a  2   &#x2264;  a  3   &#x2264; &#x2026;
     {\displaystyle a_{1}\leq a_{2}\leq a_{3}\leq \ldots }  [
     {\displaystyle a_{1}\leq a_{2}\leq a_{3}\leq \ldots }] or      a  1
     &#x2265;  a  2   &#x2265;  a  3   &#x2265; &#x2026;   {\displaystyle
     a_{1}\geq a_{2}\geq a_{3}\geq \ldots }  [{\displaystyle a_{1}\geq a_
     {2}\geq a_{3}\geq \ldots }]
holds, respectively. If either holds, the sequence is said to be monotonic. The
monotonicity is strict if the chained inequalities still hold with     &#x2264;
{\displaystyle \leq }  [\leq ] or     &#x2265;   {\displaystyle \geq }  [\geq ]
replaced by < or >.
Given a sequence     (  a  n   )   {\displaystyle (a_{n})}  [(a_{n})], another
sequence     (  b  k   )   {\displaystyle (b_{k})}  [{\displaystyle (b_{k})}]
is a subsequence of     (  a  n   )   {\displaystyle (a_{n})}  [(a_{n})] if
b  k   =  a   n  k       {\displaystyle b_{k}=a_{n_{k}}}  [{\displaystyle b_
{k}=a_{n_{k}}}] for all positive integers     k   {\displaystyle k}  [k] and
(  n  k   )   {\displaystyle (n_{k})}  [{\displaystyle (n_{k})}] is a strictly
increasing sequence of natural numbers.
**** Limits and convergence[edit] ****
Main article: Limit_(mathematics)
Roughly speaking, a limit is the value that a function or a sequence
"approaches" as the input or index approaches some value.[4] (This value can
include the symbols     &#x00B1; &#x221E;   {\displaystyle \pm \infty }  [\pm
\infty ] when addressing the behavior of a function or sequence as the variable
increases or decreases without bound.) The idea of a limit is fundamental to
calculus (and mathematical_analysis in general) and its formal definition is
used in turn to define notions like continuity, derivatives, and integrals. (In
fact, the study of limiting behavior has been used as a characteristic that
distinguishes calculus and mathematical analysis from other branches of
mathematics.)
The concept of limit was informally introduced for functions by Newton and
Leibniz, at the end of 17th century, for building infinitesimal_calculus. For
sequences, the concept was introduced by Cauchy, and made rigorous, at the end
of 19th century by Bolzano and Weierstrass, who gave the modern Îµ-Î´
definition, which follows.
Definition. Let     f   {\displaystyle f}  [f] be a real-valued function
defined on     E &#x2282;  R    {\displaystyle E\subset \mathbb {R} }
[E\subset\mathbb{R}]. We say that    f ( x )   {\displaystyle f(x)}  [f(x)]
tends to     L   {\displaystyle L}  [L] as     x   {\displaystyle x}  [x]
approaches      x  0     {\displaystyle x_{0}}  [x_{0}], or that the limit of
f ( x )   {\displaystyle f(x)}  [f(x)] as     x   {\displaystyle x}  [x]
approaches      x  0     {\displaystyle x_{0}}  [x_{0}] is     L
{\displaystyle L}  [L] if, for any     &#x03F5; > 0   {\displaystyle \epsilon
>0}  [\epsilon >0], there exists     &#x03B4; > 0   {\displaystyle \delta >0}
[\delta >0] such that for all     x &#x2208; E   {\displaystyle x\in E}  [x\in
E],     0 <  |  x &#x2212;  x  0    |  < &#x03B4;   {\displaystyle 0<|x-x_
{0}|<\delta }  [{\displaystyle 0<|x-x_{0}|<\delta }] implies that      |  f ( x
) &#x2212; L  |  < &#x03F5;   {\displaystyle |f(x)-L|<\epsilon }  [
{\displaystyle |f(x)-L|<\epsilon }]. We write this symbolically as
        f ( x ) &#x2192; L &#xA0; &#xA0;  as  &#xA0; &#xA0; x &#x2192;  x
     0     {\displaystyle f(x)\to L\ \ {\text{as}}\ \ x\to x_{0}}  [
     {\displaystyle f(x)\to L\ \ {\text{as}}\ \ x\to x_{0}}], or      lim
     x &#x2192;  x  0     f ( x ) = L   {\displaystyle \lim _{x\to x_{0}}f
     (x)=L}  [{\displaystyle \lim _{x\to x_{0}}f(x)=L}].
Intuitively, this definition can be thought of in the following way: We say
that     f ( x ) &#x2192; L   {\displaystyle f(x)\to L}  [{\displaystyle f
(x)\to L}] as     x &#x2192;  x  0     {\displaystyle x\to x_{0}}  [
{\displaystyle x\to x_{0}}], when, given any positive number     &#x03F5;
{\displaystyle \epsilon }  [\epsilon ], no matter how small, we can always find
a     &#x03B4;   {\displaystyle \delta }  [\delta ], such that we can guarantee
that     f ( x )   {\displaystyle f(x)}  [f(x)] and     L   {\displaystyle L}
[L] are less than     &#x03F5;   {\displaystyle \epsilon }  [\epsilon ] apart,
as long as     x   {\displaystyle x}  [x] (in the domain of     f
{\displaystyle f}  [f]) is a real number that is less than     &#x03B4;
{\displaystyle \delta }  [\delta ] away from      x  0     {\displaystyle x_
{0}}  [x_{0}] but distinct from      x  0     {\displaystyle x_{0}}  [x_{0}].
The purpose of the last stipulation, which corresponds to the condition     0 <
|  x &#x2212;  x  0    |    {\displaystyle 0<|x-x_{0}|}  [{\displaystyle 0<|x-
x_{0}|}] in the definition, is to ensure that      lim  x &#x2192;  x  0     f
( x ) = L   {\displaystyle \lim _{x\to x_{0}}f(x)=L}  [{\displaystyle \lim _
{x\to x_{0}}f(x)=L}] does not imply anything about the value of     f (  x  0
)   {\displaystyle f(x_{0})}  [f(x_{0})] itself. Actually,      x  0
{\displaystyle x_{0}}  [x_{0}] does not even need to be in the domain of     f
{\displaystyle f}  [f] in order for      lim  x &#x2192;  x  0     f ( x )
{\displaystyle \lim _{x\to x_{0}}f(x)}  [{\displaystyle \lim _{x\to x_{0}}f
(x)}] to exist.
In a slightly different but related context, the concept of a limit applies to
the behavior of a sequence     (  a  n   )   {\displaystyle (a_{n})}  [(a_{n})]
when     n   {\displaystyle n}  [n] becomes large.
Definition. Let     (  a  n   )   {\displaystyle (a_{n})}  [(a_{n})] be a real-
valued sequence. We say that     (  a  n   )   {\displaystyle (a_{n})}  [(a_
{n})] converges to     a   {\displaystyle a}  [a] if, for any     &#x03F5; > 0
{\displaystyle \epsilon >0}  [\epsilon >0], there exists a natural number     N
{\displaystyle N}  [N] such that     n &#x2265; N   {\displaystyle n\geq N}
[n\geq N] implies that      |  a &#x2212;  a  n    |  < &#x03F5;
{\displaystyle |a-a_{n}|<\epsilon }  [{\displaystyle |a-a_{n}|<\epsilon }]. We
write this symbolically as
         a  n   &#x2192; a &#xA0; &#xA0;  as  &#xA0; &#xA0; n &#x2192;
     &#x221E;   {\displaystyle a_{n}\to a\ \ {\text{as}}\ \ n\to \infty }
     [{\displaystyle a_{n}\to a\ \ {\text{as}}\ \ n\to \infty }], or
     lim  n &#x2192; &#x221E;    a  n   = a   {\displaystyle \lim _{n\to
     \infty }a_{n}=a}  [{\displaystyle \lim _{n\to \infty }a_{n}=a}];
if     (  a  n   )   {\displaystyle (a_{n})}  [(a_{n})] fails to converge, we
say that     (  a  n   )   {\displaystyle (a_{n})}  [(a_{n})] diverges.
Generalizing to a real-valued function of a real variable, a slight
modification of this definition (replacement of sequence     (  a  n   )
{\displaystyle (a_{n})}  [(a_{n})] and term      a  n     {\displaystyle a_{n}}
[a_{n}] by function     f   {\displaystyle f}  [f] and value     f ( x )
{\displaystyle f(x)}  [f(x)] and natural numbers     N   {\displaystyle N}  [N]
and     n   {\displaystyle n}  [n] by real numbers     M   {\displaystyle M}
[M] and     x   {\displaystyle x}  [x], respectively) yields the definition of
the limit of     f ( x )   {\displaystyle f(x)}  [f(x)] as     x
{\displaystyle x}  [x] increases without bound, notated      lim  x &#x2192;
&#x221E;   f ( x )   {\displaystyle \lim _{x\to \infty }f(x)}  [{\displaystyle
\lim _{x\to \infty }f(x)}]. Reversing the inequality     x &#x2265; M
{\displaystyle x\geq M}  [{\displaystyle x\geq M}] to     x &#x2264; M
{\displaystyle x\leq M}  [{\displaystyle x\leq M}] gives the corresponding
definition of the limit of     f ( x )   {\displaystyle f(x)}  [f(x)] as     x
{\displaystyle x}  [x] decreases without bound,      lim  x &#x2192; &#x2212;
&#x221E;   f ( x )   {\displaystyle \lim _{x\to -\infty }f(x)}  [{\displaystyle
\lim _{x\to -\infty }f(x)}].
Sometimes, it is useful to conclude that a sequence converges, even though the
value to which it converges is unknown or irrelevant. In these cases, the
concept of a Cauchy sequence is useful.
Definition. Let     (  a  n   )   {\displaystyle (a_{n})}  [(a_{n})] be a real-
valued sequence. We say that     (  a  n   )   {\displaystyle (a_{n})}  [(a_
{n})] is a Cauchy sequence if, for any     &#x03F5; > 0   {\displaystyle
\epsilon >0}  [\epsilon >0], there exists a natural number     N
{\displaystyle N}  [N] such that     m , n &#x2265; N   {\displaystyle m,n\geq
N}  [{\displaystyle m,n\geq N}] implies that      |   a  m   &#x2212;  a  n
|  < &#x03F5;   {\displaystyle |a_{m}-a_{n}|<\epsilon }  [{\displaystyle |a_
{m}-a_{n}|<\epsilon }].
It can be shown that a real-valued sequence is Cauchy if and only if it is
convergent. This property of the real numbers is expressed by saying that the
real numbers endowed with the standard metric,     (  R  ,  |  &#x22C5;  |  )
{\displaystyle (\mathbb {R} ,|\cdot |)}  [{\displaystyle (\mathbb {R} ,|\cdot
|)}], is a complete_metric_space. In a general metric space, however, a Cauchy
sequence need not converge.
In addition, for real-valued sequences that are monotonic, it can be shown that
the sequence is bounded if and only if it is convergent.
*** Uniform and pointwise convergence for sequences of functions[edit] ***
Main article: Uniform_convergence
In addition to sequences of numbers, one may also speak of sequences of
functions on     E &#x2282;  R    {\displaystyle E\subset \mathbb {R} }  [
{\displaystyle E\subset \mathbb {R} }], that is, infinite, ordered families of
functions      f  n   : E &#x2192;  R    {\displaystyle f_{n}:E\to \mathbb {R}
}  [{\displaystyle f_{n}:E\to \mathbb {R} }], denoted     (  f  n    )  n = 1
&#x221E;     {\displaystyle (f_{n})_{n=1}^{\infty }}  [(f_{n})_{n=1}^{\infty
}], and their convergence properties. However, in the case of sequences of
functions, there are two kinds of convergence, known as pointwise convergence
and uniform convergence, that need to be distinguished.
Roughly speaking, pointwise convergence of functions      f  n
{\displaystyle f_{n}}  [f_{n}] to a limiting function     f : E &#x2192;  R
{\displaystyle f:E\to \mathbb {R} }  [{\displaystyle f:E\to \mathbb {R} }],
denoted      f  n   &#x2192; f   {\displaystyle f_{n}\rightarrow f}  [
{\displaystyle f_{n}\rightarrow f}], simply means that given any     x &#x2208;
E   {\displaystyle x\in E}  [x\in E],      f  n   ( x ) &#x2192; f ( x )
{\displaystyle f_{n}(x)\to f(x)}  [f_n(x)\to f(x)] as     n &#x2192; &#x221E;
{\displaystyle n\to \infty }  [n\to \infty ]. In contrast, uniform convergence
is a stronger type of convergence, in the sense that a uniformly convergent
sequence of functions also converges pointwise, but not conversely. Uniform
convergence requires members of the family of functions,      f  n
{\displaystyle f_{n}}  [f_{n}], to fall within some error     &#x03F5; > 0
{\displaystyle \epsilon >0}  [\epsilon >0] of     f   {\displaystyle f}  [f]
for every value of     x &#x2208; E   {\displaystyle x\in E}  [x\in E],
whenever     n &#x2265; N   {\displaystyle n\geq N}  [n\geq N], for some
integer     N   {\displaystyle N}  [N]. For a family of functions to uniformly
converge, sometimes denoted      f  n   &#x21C9; f   {\displaystyle f_
{n}\rightrightarrows f}  [{\displaystyle f_{n}\rightrightarrows f}], such a
value of     N   {\displaystyle N}  [N] must exist for any     &#x03F5; > 0
{\displaystyle \epsilon >0}  [\epsilon >0] given, no matter how small.
Intuitively, we can visualize this situation by imagining that, for a large
enough     N   {\displaystyle N}  [N], the functions      f  N   ,  f  N + 1
,  f  N + 2   , &#x2026;   {\displaystyle f_{N},f_{N+1},f_{N+2},\ldots }  [
{\displaystyle f_{N},f_{N+1},f_{N+2},\ldots }] are all confined within a 'tube'
of width     2 &#x03F5;   {\displaystyle 2\epsilon }  [2\epsilon] about     f
{\displaystyle f}  [f] (i.e., between     f &#x2212; &#x03F5;   {\displaystyle
f-\epsilon }  [{\displaystyle f-\epsilon }] and     f + &#x03F5;
{\displaystyle f+\epsilon }  [{\displaystyle f+\epsilon }]) for every value in
their domain     E   {\displaystyle E}  [E].
The distinction between pointwise and uniform convergence is important when
exchanging the order of two limiting operations (e.g., taking a limit, a
derivative, or integral) is desired: in order for the exchange to be well-
behaved, many theorems of real analysis call for uniform convergence. For
example, a sequence of continuous functions (see below) is guaranteed to
converge to a continuous limiting function if the convergence is uniform, while
the limiting function may not be continuous if convergence is only pointwise.
Karl_Weierstrass is generally credited for clearly defining the concept of
uniform convergence and fully investigating its implications.
**** Compactness[edit] ****
Main article: Compactness
Compactness is a concept from general_topology that plays an important role in
many of the theorems of real analysis. The property of compactness is a
generalization of the notion of a set being closed and bounded. (In the context
of real analysis, these notions are equivalent: a set in Euclidean space is
compact if and only if it is closed and bounded.) Briefly, a closed_set
contains all of its boundary_points, while a set is bounded if there exists a
real number such that the distance between any two points of the set is less
than that number. In      R    {\displaystyle \mathbb {R} }  [\mathbb {R} ],
sets that are closed and bounded, and therefore compact, include the empty set,
any finite number of points, closed_intervals, and their finite unions.
However, this list is not exhaustive; for instance, the set      { 1  /  n : n
&#x2208;  N  } &#x222A; { 0   }  {\displaystyle \{1/n:n\in \mathbb {N} \}\cup \
{0}\}  [{\displaystyle \{1/n:n\in \mathbb {N} \}\cup \{0}\}] is another example
of a compact set. On the other hand, the set     { 1  /  n : n &#x2208;  N  }
{\displaystyle \{1/n:n\in \mathbb {N} \}}  [{\displaystyle \{1/n:n\in \mathbb
{N} \}}] is not compact because it is bounded but not closed, as the boundary
point 0 is not a member of the set. The set     [ 0 , &#x221E; )
{\displaystyle [0,\infty )}  [[0,\infty )] is also not compact because it is
closed but not bounded.
For subsets of the real numbers, there are several equivalent definitions of
compactness.
Definition. A set     E &#x2282;  R    {\displaystyle E\subset \mathbb {R} }
[E\subset\mathbb{R}] is compact if it is closed and bounded.
This definition also holds for Euclidean space of any finite dimension,       R
n     {\displaystyle \mathbb {R} ^{n}}  [\mathbb {R} ^{n}], but it is not valid
for metric spaces in general. The equivalence of the definition with the
definition of compactness based on subcovers, given later in this section, is
known as the Heine-Borel_theorem.
A more general definition that applies to all metric spaces uses the notion of
a subsequence (see above).
Definition. A set     E   {\displaystyle E}  [E] in a metric space is compact
if every sequence in     E   {\displaystyle E}  [E] has a convergent
subsequence.
This particular property is known as subsequential compactness. In      R
{\displaystyle \mathbb {R} }  [\mathbb {R} ], a set is subsequentially compact
if and only if it is closed and bounded, making this definition equivalent to
the one given above. Subsequential compactness is equivalent to the definition
of compactness based on subcovers for metric spaces, but not for topological
spaces in general.
The most general definition of compactness relies on the notion of open covers
and subcovers, which is applicable to topological spaces (and thus to metric
spaces and      R    {\displaystyle \mathbb {R} }  [\mathbb {R} ] as special
cases). In brief, a collection of open sets      U  &#x03B1;     {\displaystyle
U_{\alpha }}  [U_{\alpha }] is said to be an open cover of set     X
{\displaystyle X}  [X] if the union of these sets is a superset of     X
{\displaystyle X}  [X]. This open cover is said to have a finite subcover if a
finite subcollection of the      U  &#x03B1;     {\displaystyle U_{\alpha }}
[U_{\alpha }] could be found that also covers     X   {\displaystyle X}  [X].
Definition. A set     X   {\displaystyle X}  [X] in a topological space is
compact if every open cover of     X   {\displaystyle X}  [X] has a finite
subcover.
Compact sets are well-behaved with respect to properties like convergence and
continuity. For instance, any Cauchy sequence in a compact metric space is
convergent. As another example, the image of a compact metric space under a
continuous map is also compact.
**** Continuity[edit] ****
Main article: Continuous_function
A function from the set of real_numbers to the real numbers can be represented
by a graph in the Cartesian_plane; such a function is continuous if, roughly
speaking, the graph is a single unbroken curve with no "holes" or "jumps".
There are several ways to make this intuition mathematically rigorous. Several
definitions of varying levels of generality can be given. In cases where two or
more definitions are applicable, they are readily shown to be equivalent to one
another, so the most convenient definition can be used to determine whether a
given function is continuous or not. In the first definition given below,     f
: I &#x2192;  R    {\displaystyle f:I\to \mathbb {R} }  [{\displaystyle f:I\to
\mathbb {R} }] is a function defined on a non-degenerate interval     I
{\displaystyle I}  [I] of the set of real numbers as its domain. Some
possibilities include     I =  R    {\displaystyle I=\mathbb {R} }  [
{\displaystyle I=\mathbb {R} }], the whole set of real numbers, an open
interval     I = ( a , b ) = { x &#x2208;  R    |   a < x < b } ,
{\displaystyle I=(a,b)=\{x\in \mathbb {R} \,|\,a<x<b\},}  [{\displaystyle I=
(a,b)=\{x\in \mathbb {R} \,|\,a<x<b\},}] or a closed_interval     I = [ a , b ]
= { x &#x2208;  R    |   a &#x2264; x &#x2264; b } .   {\displaystyle I=[a,b]=\
{x\in \mathbb {R} \,|\,a\leq x\leq b\}.}  [{\displaystyle I=[a,b]=\{x\in
\mathbb {R} \,|\,a\leq x\leq b\}.}] Here,     a   {\displaystyle a}  [a] and
b   {\displaystyle b}  [b] are distinct real numbers, and we exclude the case
of     I   {\displaystyle I}  [I] being empty or consisting of only one point,
in particular.
Definition. If     I &#x2282;  R    {\displaystyle I\subset \mathbb {R} }
[I\subset \mathbb{R}] is a non-degenerate interval, we say that     f : I
&#x2192;  R    {\displaystyle f:I\to \mathbb {R} }  [{\displaystyle f:I\to
\mathbb {R} }] is continuous at     p &#x2208; E   {\displaystyle p\in E}  [
{\displaystyle p\in E}] if      lim  x &#x2192; p   f ( x ) = f ( p )
{\displaystyle \lim _{x\to p}f(x)=f(p)}  [{\displaystyle \lim _{x\to p}f(x)=f
(p)}]. We say that     f   {\displaystyle f}  [f] is a continuous map if     f
{\displaystyle f}  [f] is continuous at every     p &#x2208; I   {\displaystyle
p\in I}  [{\displaystyle p\in I}].
In contrast to the requirements for     f   {\displaystyle f}  [f] to have a
limit at a point     p   {\displaystyle p}  [p], which do not constrain the
behavior of     f   {\displaystyle f}  [f] at     p   {\displaystyle p}  [p]
itself, the following two conditions, in addition to the existence of      lim
x &#x2192; p   f ( x )   {\textstyle \lim _{x\to p}f(x)}  [{\textstyle \lim _
{x\to p}f(x)}], must also hold in order for     f   {\displaystyle f}  [f] to
be continuous at     p   {\displaystyle p}  [p]: (i)     f   {\displaystyle f}
[f] must be defined at     p   {\displaystyle p}  [p], i.e.,     p
{\displaystyle p}  [p] is in the domain of     f   {\displaystyle f}  [f]; and
(ii)     f ( x ) &#x2192; f ( p )   {\displaystyle f(x)\to f(p)}  [
{\displaystyle f(x)\to f(p)}] as     x &#x2192; p   {\displaystyle x\to p}  [
{\displaystyle x\to p}]. The definition above actually applies to any domain
E   {\displaystyle E}  [E] that does not contain an isolated_point, or
equivalently,     E   {\displaystyle E}  [E] where every     p &#x2208; E
{\displaystyle p\in E}  [{\displaystyle p\in E}] is a limit_point of     E
{\displaystyle E}  [E]. A more general definition applying to     f : X
&#x2192;  R    {\displaystyle f:X\to \mathbb {R} }  [f:X\to\mathbb{R}] with a
general domain     X &#x2282;  R    {\displaystyle X\subset \mathbb {R} }
[X\subset {\mathbb  {R}}] is the following:
Definition. If     X   {\displaystyle X}  [X] is an arbitrary subset of      R
{\displaystyle \mathbb {R} }  [\mathbb {R} ], we say that     f : X &#x2192;  R
{\displaystyle f:X\to \mathbb {R} }  [f:X\to\mathbb{R}] is continuous at     p
&#x2208; X   {\displaystyle p\in X}  [p\in X] if, for any     &#x03F5; > 0
{\displaystyle \epsilon >0}  [\epsilon >0], there exists     &#x03B4; > 0
{\displaystyle \delta >0}  [\delta >0] such that for all     x &#x2208; X
{\displaystyle x\in X}  [x\in X],      |  x &#x2212; p  |  < &#x03B4;
{\displaystyle |x-p|<\delta }  [|x-p|<\delta] implies that      |  f ( x )
&#x2212; f ( p )  |  < &#x03F5;   {\displaystyle |f(x)-f(p)|<\epsilon }  [|f
(x)-f(p)|<\epsilon]. We say that     f   {\displaystyle f}  [f] is a continuous
map if     f   {\displaystyle f}  [f] is continuous at every     p &#x2208; X
{\displaystyle p\in X}  [p\in X].
A consequence of this definition is that     f   {\displaystyle f}  [f] is
trivially continuous at any isolated point     p &#x2208; X   {\displaystyle
p\in X}  [p\in X]. This somewhat unintuitive treatment of isolated points is
necessary to ensure that our definition of continuity for functions on the real
line is consistent with the most general definition of continuity for maps
between topological_spaces (which includes metric_spaces and      R
{\displaystyle \mathbb {R} }  [\mathbb {R} ] in particular as special cases).
This definition, which extends beyond the scope of our discussion of real
analysis, is given below for completeness.
Definition. If     X   {\displaystyle X}  [X] and     Y   {\displaystyle Y}
[Y] are topological spaces, we say that     f : X &#x2192; Y   {\displaystyle
f:X\to Y}  [f:X\to Y] is continuous at     p &#x2208; X   {\displaystyle p\in
X}  [p\in X] if      f  &#x2212; 1   ( V )   {\displaystyle f^{-1}(V)}  [
{\displaystyle f^{-1}(V)}] is a neighborhood of     p   {\displaystyle p}  [p]
in     X   {\displaystyle X}  [X] for every neighborhood     V   {\displaystyle
V}  [V] of     f ( p )   {\displaystyle f(p)}  [f(p)] in     Y   {\displaystyle
Y}  [Y]. We say that     f   {\displaystyle f}  [f] is a continuous map if
f  &#x2212; 1   ( U )   {\displaystyle f^{-1}(U)}  [f^{-1}(U)] is open in     X
{\displaystyle X}  [X] for every     U   {\displaystyle U}  [U] open in     Y
{\displaystyle Y}  [Y].
(Here,      f  &#x2212; 1   ( S )   {\displaystyle f^{-1}(S)}  [f^{-1}(S)]
refers to the preimage of     S &#x2282; Y   {\displaystyle S\subset Y}  [
{\displaystyle S\subset Y}] under     f   {\displaystyle f}  [f].)
*** Uniform continuity[edit] ***
Main article: Uniform_continuity
Definition. If     X   {\displaystyle X}  [X] is a subset of the real_numbers,
we say a function     f : X &#x2192;  R    {\displaystyle f:X\to \mathbb {R} }
[f:X\to\mathbb{R}] is uniformly continuous on     X   {\displaystyle X}  [X]
if, for any     &#x03F5; > 0   {\displaystyle \epsilon >0}  [\epsilon >0],
there exists a     &#x03B4; > 0   {\displaystyle \delta >0}  [\delta >0] such
that for all     x , y &#x2208; X   {\displaystyle x,y\in X}  [x,y\in X],
|  x &#x2212; y  |  < &#x03B4;   {\displaystyle |x-y|<\delta }  [{\displaystyle
|x-y|<\delta }] implies that      |  f ( x ) &#x2212; f ( y )  |  < &#x03F5;
{\displaystyle |f(x)-f(y)|<\epsilon }  [{\displaystyle |f(x)-f(y)|<\epsilon }].
Explicitly, when a function is uniformly continuous on     X   {\displaystyle
X}  [X], the choice of     &#x03B4;   {\displaystyle \delta }  [\delta ] needed
to fulfill the definition must work for all of     X   {\displaystyle X}  [X]
for a given     &#x03F5;   {\displaystyle \epsilon }  [\epsilon ]. In contrast,
when a function is continuous at every point     p &#x2208; X   {\displaystyle
p\in X}  [p\in X] (or said to be continuous on     X   {\displaystyle X}  [X]),
the choice of     &#x03B4;   {\displaystyle \delta }  [\delta ] may depend on
both     &#x03F5;   {\displaystyle \epsilon }  [\epsilon ] and     p
{\displaystyle p}  [p]. Importantly, in contrast to simple continuity, uniform
continuity is a property of a function that only makes sense with a specified
domain; to speak of uniform continuity at a single point     p   {\displaystyle
p}  [p] is meaningless.
On a compact set, it is easily shown that all continuous functions are
uniformly continuous. If     E   {\displaystyle E}  [E] is a bounded noncompact
subset of      R    {\displaystyle \mathbb {R} }  [\mathbb {R} ], then there
exists     f : E &#x2192;  R    {\displaystyle f:E\to \mathbb {R} }  [
{\displaystyle f:E\to \mathbb {R} }] that is continuous but not uniformly
continuous. As a simple example, consider     f : ( 0 , 1 ) &#x2192;  R
{\displaystyle f:(0,1)\to \mathbb {R} }  [{\displaystyle f:(0,1)\to \mathbb {R}
}] defined by     f ( x ) = 1  /  x   {\displaystyle f(x)=1/x}  [f(x)=1/x]. By
choosing points close to 0, we can always make      |  f ( x ) &#x2212; f ( y )
|  > &#x03F5;   {\displaystyle |f(x)-f(y)|>\epsilon }  [{\displaystyle |f(x)-f
(y)|>\epsilon }] for any single choice of     &#x03B4; > 0   {\displaystyle
\delta >0}  [\delta >0], for a given     &#x03F5; > 0   {\displaystyle \epsilon
>0}  [\epsilon >0].
*** Absolute continuity[edit] ***
Main article: Absolute_continuity
Definition. Let     I &#x2282;  R    {\displaystyle I\subset \mathbb {R} }  [
{\displaystyle I\subset \mathbb {R} }] be an interval on the real_line. A
function     f : I &#x2192;  R    {\displaystyle f:I\to \mathbb {R} }  [
{\displaystyle f:I\to \mathbb {R} }] is said to be absolutely continuous on
I   {\displaystyle I}  [I] if for every positive number     &#x03F5;
{\displaystyle \epsilon }  [\epsilon ], there is a positive number     &#x03B4;
{\displaystyle \delta }  [\delta ] such that whenever a finite sequence of
pairwise_disjoint sub-intervals     (  x  1   ,  y  1   ) , (  x  2   ,  y  2
) , &#x2026; , (  x  n   ,  y  n   )   {\displaystyle (x_{1},y_{1}),(x_{2},y_
{2}),\ldots ,(x_{n},y_{n})}  [{\displaystyle (x_{1},y_{1}),(x_{2},y_{2}),\ldots
,(x_{n},y_{n})}] of     I   {\displaystyle I}  [I] satisfies[5]
          &#x2211;  k = 1   n   (  y  k   &#x2212;  x  k   ) < &#x03B4;
      {\displaystyle \sum _{k=1}^{n}(y_{k}-x_{k})<\delta }  [{\displaystyle
      \sum _{k=1}^{n}(y_{k}-x_{k})<\delta }]
then
           &#x2211;  k = 1   n    |  f (  y  k   ) &#x2212; f (  x  k   )  |  <
      &#x03F5; .    {\displaystyle \displaystyle \sum _{k=1}^{n}|f(y_{k})-f(x_
      {k})|<\epsilon .}  [{\displaystyle \displaystyle \sum _{k=1}^{n}|f(y_
      {k})-f(x_{k})|<\epsilon .}]
Absolutely continuous functions are continuous: consider the case n = 1 in this
definition. The collection of all absolutely continuous functions on I is
denoted AC(I). Absolute continuity is an important concept in the Lebesgue
theory of integration, allowing the formulation of a generalized version of the
fundamental theorem of calculus that applies to the Lebesgue integral.
**** Differentiation[edit] ****
Main articles: Derivative and Differential_calculus
The notion of the derivative of a function or differentiability originates from
the concept of approximating a function near a given point using the "best"
linear approximation. This approximation, if it exists, is unique and is given
by the line that is tangent to the function at the given point     a
{\displaystyle a}  [a], and the slope of the line is the derivative of the
function at     a   {\displaystyle a}  [a].
A function     f :  R  &#x2192;  R    {\displaystyle f:\mathbb {R} \to \mathbb
{R} }  [{\displaystyle f:\mathbb {R} \to \mathbb {R} }] is differentiable at
a   {\displaystyle a}  [a] if the limit
          f &#x2032;  ( a ) =  lim  h &#x2192; 0      f ( a + h ) &#x2212; f
      ( a )  h     {\displaystyle f'(a)=\lim _{h\to 0}{\frac {f(a+h)-f(a)}{h}}}
      [f'(a)=\lim _{h\to 0}{\frac {f(a+h)-f(a)}{h}}]
exists. This limit is known as the derivative of     f   {\displaystyle f}  [f]
at     a   {\displaystyle a}  [a], and the function      f &#x2032;
{\displaystyle f'}  [f'], possibly defined on only a subset of      R
{\displaystyle \mathbb {R} }  [\mathbb {R} ], is the derivative (or derivative
function) of    f   {\displaystyle f}  [f]. If the derivative exists
everywhere, the function is said to be differentiable.
As a simple consequence of the definition,     f   {\displaystyle f}  [f] is
continuous at    a   {\displaystyle a}  [a] if it is differentiable there.
Differentiability is therefore a stronger regularity condition (condition
describing the "smoothness" of a function) than continuity, and it is possible
for a function to be continuous on the entire real line but not differentiable
anywhere (see Weierstrass's_nowhere_differentiable_continuous_function). It is
possible to discuss the existence of higher-order derivatives as well, by
finding the derivative of a derivative function, and so on.
One can classify functions by their differentiability class. The class      C
0     {\displaystyle C^{0}}  [C^0] (sometimes      C  0   ( [ a , b ] )
{\displaystyle C^{0}([a,b])}  [{\displaystyle C^{0}([a,b])}] to indicate the
interval of applicability) consists of all continuous functions. The class
C  1     {\displaystyle C^{1}}  [C^{1}] consists of all differentiable
functions whose derivative is continuous; such functions are called
continuously differentiable. Thus, a      C  1     {\displaystyle C^{1}}  [C^
{1}] function is exactly a function whose derivative exists and is of class
C  0     {\displaystyle C^{0}}  [C^0]. In general, the classes     C  k
{\displaystyle C^{k}}  [C^{k}] can be defined recursively by declaring      C
0     {\displaystyle C^{0}}  [C^0] to be the set of all continuous functions
and declaring     C  k     {\displaystyle C^{k}}  [C^{k}] for any positive
integer     k   {\displaystyle k}  [k] to be the set of all differentiable
functions whose derivative is in      C  k &#x2212; 1     {\displaystyle C^{k-
1}}  [{\displaystyle C^{k-1}}]. In particular,     C  k     {\displaystyle C^
{k}}  [C^{k}] is contained in      C  k &#x2212; 1     {\displaystyle C^{k-1}}
[{\displaystyle C^{k-1}}] for every     k   {\displaystyle k}  [k], and there
are examples to show that this containment is strict. Class      C  &#x221E;
{\displaystyle C^{\infty }}  [C^{\infty }] is the intersection of the sets
C  k     {\displaystyle C^{k}}  [C^{k}] as    k   {\displaystyle k}  [k] varies
over the non-negative integers, and the members of this class are known as the
smooth functions. Class      C  &#x03C9;     {\displaystyle C^{\omega }}  [C^
{\omega }] consists of all analytic_functions, and is strictly contained in
C  &#x221E;     {\displaystyle C^{\infty }}  [C^{\infty }] (see bump_function
for a smooth function that is not analytic).
The chain_rule, mean_value_theorem, l'Hospital's_rule, and Taylor's_theorem are
important results in the elementary theory of the derivative.
**** Series[edit] ****
Main article: series_(mathematics)
A series formalizes the imprecise notion of taking the sum of an endless
sequence of numbers. The idea that taking the sum of an "infinite" number of
terms can lead to a finite result was counterintuitive to the ancient Greeks
and led to the formulation of a number of paradoxes by Zeno and other
philosophers. The modern notion of assigning a value to a series avoids dealing
with the ill-defined notion of adding an "infinite" number of terms. Instead,
the finite sum of the first     n   {\displaystyle n}  [n] terms of the
sequence, known as a partial sum, is considered, and the concept of a limit is
applied to the sequence of partial sums as     n   {\displaystyle n}  [n] grows
without bound. The series is assigned the value of this limit, if it exists.
Given an (infinite) sequence     (  a  n   )   {\displaystyle (a_{n})}  [(a_
{n})], we can define an associated series as the formal mathematical object
a  1   +  a  2   +  a  3   + &#x22EF; =  &#x2211;  n = 1   &#x221E;    a  n
{\textstyle a_{1}+a_{2}+a_{3}+\cdots =\sum _{n=1}^{\infty }a_{n}}  [{\textstyle
a_{1}+a_{2}+a_{3}+\cdots =\sum _{n=1}^{\infty }a_{n}}], sometimes simply
written as     &#x2211;  a  n     {\textstyle \sum a_{n}}  [{\textstyle \sum a_
{n}}]. The partial sums of a series     &#x2211;  a  n     {\textstyle \sum a_
{n}}  [{\textstyle \sum a_{n}}] are the numbers      s  n   =  &#x2211;  j = 1
n    a  j     {\textstyle s_{n}=\sum _{j=1}^{n}a_{j}}  [{\textstyle s_{n}=\sum
_{j=1}^{n}a_{j}}]. A series     &#x2211;  a  n     {\textstyle \sum a_{n}}  [
{\textstyle \sum a_{n}}] is said to be convergent if the sequence consisting of
its partial sums,     (  s  n   )   {\displaystyle (s_{n})}  [(s_n)], is
convergent; otherwise it is divergent. The sum of a convergent series is
defined as the number     s =  lim  n &#x2192; &#x221E;    s  n     {\textstyle
s=\lim _{n\to \infty }s_{n}}  [{\textstyle s=\lim _{n\to \infty }s_{n}}].
It is to be emphasized that the word "sum" is used here in a metaphorical sense
as a shorthand for taking the limit of a sequence of partial sums and should
not be interpreted as simply "adding" an infinite number of terms. For
instance, in contrast to the behavior of finite sums, rearranging the terms of
an infinite series may result in convergence to a different number (see the
article on the Riemann_rearrangement_theorem for further discussion).
An example of a convergent series is a geometric_series which forms the basis
of one of Zeno's famous paradoxes:
          &#x2211;  n = 1   &#x221E;     1  2  n     =   1 2   +   1 4   +   1
      8   + &#x22EF; = 1   {\displaystyle \sum _{n=1}^{\infty }{\frac {1}{2^
      {n}}}={\frac {1}{2}}+{\frac {1}{4}}+{\frac {1}{8}}+\cdots =1}  [
      {\displaystyle \sum _{n=1}^{\infty }{\frac {1}{2^{n}}}={\frac {1}{2}}+
      {\frac {1}{4}}+{\frac {1}{8}}+\cdots =1}].
In contrast, the harmonic_series has been known since the Middle Ages to be a
divergent series:
          &#x2211;  n = 1   &#x221E;     1 n   = 1 +   1 2   +   1 3   +
      &#x22EF; = &#x221E;   {\displaystyle \sum _{n=1}^{\infty }{\frac {1}
      {n}}=1+{\frac {1}{2}}+{\frac {1}{3}}+\cdots =\infty }  [{\displaystyle
      \sum _{n=1}^{\infty }{\frac {1}{n}}=1+{\frac {1}{2}}+{\frac {1}
      {3}}+\cdots =\infty }].
(Here, "    = &#x221E;   {\displaystyle =\infty }  [=\infty ]" is merely a
notational convention to indicate that the partial sums of the series grow
without bound.)
A series     &#x2211;  a  n     {\textstyle \sum a_{n}}  [{\textstyle \sum a_
{n}}] is said to converge_absolutely if     &#x2211;  |   a  n    |
{\textstyle \sum |a_{n}|}  [{\textstyle \sum |a_{n}|}] is convergent. A
convergent series     &#x2211;  a  n     {\textstyle \sum a_{n}}  [{\textstyle
\sum a_{n}}] for which     &#x2211;  |   a  n    |    {\textstyle \sum |a_{n}|}
[{\textstyle \sum |a_{n}|}] diverges is said to converge conditionally (or
nonabsolutely). It is easily shown that absolute convergence of a series
implies its convergence. On the other hand, an example of a conditionally
convergent series is
          &#x2211;  n = 1   &#x221E;      ( &#x2212; 1  )  n &#x2212; 1    n
      = 1 &#x2212;   1 2   +   1 3   &#x2212;   1 4   + &#x22EF; = log &#x2061;
      2   {\displaystyle \sum _{n=1}^{\infty }{\frac {(-1)^{n-1}}{n}}=1-{\frac
      {1}{2}}+{\frac {1}{3}}-{\frac {1}{4}}+\cdots =\log 2}  [{\displaystyle
      \sum _{n=1}^{\infty }{\frac {(-1)^{n-1}}{n}}=1-{\frac {1}{2}}+{\frac {1}
      {3}}-{\frac {1}{4}}+\cdots =\log 2}].
*** Taylor series[edit] ***
Main article: Taylor_series
The Taylor series of a real or complex-valued_function Æ(x) that is infinitely
differentiable at a real or complex_number a is the power_series
         f ( a ) +     f &#x2032;  ( a )   1 !    ( x &#x2212; a ) +     f
      &#x2033;  ( a )   2 !    ( x &#x2212; a  )  2   +     f  ( 3 )   ( a )
      3 !    ( x &#x2212; a  )  3   + &#x22EF; .   {\displaystyle f(a)+{\frac
      {f'(a)}{1!}}(x-a)+{\frac {f''(a)}{2!}}(x-a)^{2}+{\frac {f^{(3)}(a)}{3!}}
      (x-a)^{3}+\cdots .}  [f(a)+{\frac {f'(a)}{1!}}(x-a)+{\frac {f''(a)}{2!}}
      (x-a)^{2}+{\frac {f^{(3)}(a)}{3!}}(x-a)^{3}+\cdots .]
which can be written in the more compact sigma_notation as
          &#x2211;  n = 0   &#x221E;       f  ( n )   ( a )   n !     ( x
      &#x2212; a  )  n     {\displaystyle \sum _{n=0}^{\infty }{\frac {f^{(n)}
      (a)}{n!}}\,(x-a)^{n}}  [\sum _{n=0}^{\infty }{\frac {f^{(n)}(a)}{n!}}\,
      (x-a)^{n}]
where n! denotes the factorial of n and Æ (n)(a) denotes the nth derivative of
Æ evaluated at the point a. The derivative of order zero Æ is defined to be
Æ itself and (x â a)0 and 0! are both defined to be 1. In the case that a =
0, the series is also called a Maclaurin series.
A Taylor series of f about point a may diverge, converge at only the point a,
converge for all x such that      |  x &#x2212; a  |  < R   {\displaystyle |x-
a|<R}  [{\displaystyle |x-a|<R}] (the largest such R for which convergence is
guaranteed is called the radius of convergence), or converge on the entire real
line. Even a converging Taylor series may converge to a value different from
the value of the function at that point. If the Taylor series at a point has a
nonzero radius_of_convergence, and sums to the function in the disc_of
convergence, then the function is analytic. The analytic functions have many
fundamental properties. In particular, an analytic function of a real variable
extends naturally to a function of a complex variable. It is in this way that
the exponential_function, the logarithm, the trigonometric_functions and their
inverses are extended to functions of a complex variable.
*** Fourier series[edit] ***
Main article: Fourier_series
Fourier series decomposes periodic_functions or periodic signals into the sum
of a (possibly infinite) set of simple oscillating functions, namely sines_and
cosines (or complex_exponentials). The study of Fourier series typically occurs
and is handled within the branch mathematics > mathematical_analysis > Fourier
analysis.
**** Integration[edit] ****
Integration is a formalization of the problem of finding the area bound by a
curve and the related problems of determining the length of a curve or volume
enclosed by a surface. The basic strategy to solving problems of this type was
known to the ancient Greeks and Chinese, and was known as the method_of
exhaustion. Generally speaking, the desired area is bounded from above and
below, respectively, by increasingly accurate circumscribing and inscribing
polygonal approximations whose exact areas can be computed. By considering
approximations consisting of a larger and larger ("infinite") number of smaller
and smaller ("infinitesimal") pieces, the area bound by the curve can be
deduced, as the upper and lower bounds defined by the approximations converge
around a common value.
The spirit of this basic strategy can easily be seen in the definition of the
Riemann integral, in which the integral is said to exist if upper and lower
Riemann (or Darboux) sums converge to a common value as thinner and thinner
rectangular slices ("refinements") are considered. Though the machinery used to
define it is much more elaborate compared to the Riemann integral, the Lebesgue
integral was defined with similar basic ideas in mind. Compared to the Riemann
integral, the more sophisticated Lebesgue integral allows area (or length,
volume, etc.; termed a "measure" in general) to be defined and computed for
much more complicated and irregular subsets of Euclidean space, although there
still exist "non-measurable" subsets for which an area cannot be assigned.
*** Riemann integration[edit] ***
Main article: Riemann_integral
The Riemann integral is defined in terms of Riemann_sums of functions with
respect to tagged partitions of an interval. Let     [ a , b ]   {\displaystyle
[a,b]}  [[a,b]] be a closed_interval of the real line; then a tagged partition
P     {\displaystyle {\cal {P}}}  [{\displaystyle {\cal {P}}}] of     [ a , b ]
{\displaystyle [a,b]}  [[a,b]] is a finite sequence
         a =  x  0   &#x2264;  t  1   &#x2264;  x  1   &#x2264;  t  2
      &#x2264;  x  2   &#x2264; &#x22EF; &#x2264;  x  n &#x2212; 1   &#x2264;
      t  n   &#x2264;  x  n   = b .     {\displaystyle a=x_{0}\leq t_{1}\leq x_
      {1}\leq t_{2}\leq x_{2}\leq \cdots \leq x_{n-1}\leq t_{n}\leq x_
      {n}=b.\,\!}  [a=x_{0}\leq t_{1}\leq x_{1}\leq t_{2}\leq x_{2}\leq \cdots
      \leq x_{n-1}\leq t_{n}\leq x_{n}=b.\,\!]
This partitions the interval     [ a , b ]   {\displaystyle [a,b]}  [[a,b]]
into     n   {\displaystyle n}  [n] sub-intervals     [  x  i &#x2212; 1   ,  x
i   ]   {\displaystyle [x_{i-1},x_{i}]}  [[x_{i-1},x_{i}]] indexed by     i = 1
, &#x2026; , n   {\displaystyle i=1,\ldots ,n}  [i=1,\ldots, n], each of which
is "tagged" with a distinguished point      t  i   &#x2208; [  x  i &#x2212; 1
,  x  i   ]   {\displaystyle t_{i}\in [x_{i-1},x_{i}]}  [{\displaystyle t_
{i}\in [x_{i-1},x_{i}]}]. For a function     f   {\displaystyle f}  [f] bounded
on     [ a , b ]   {\displaystyle [a,b]}  [[a,b]], we define the Riemann sum of
f   {\displaystyle f}  [f] with respect to tagged partition       P
{\displaystyle {\cal {P}}}  [{\displaystyle {\cal {P}}}] as
          &#x2211;  i = 1   n   f (  t  i   )  &#x0394;  i   ,   {\displaystyle
      \sum _{i=1}^{n}f(t_{i})\Delta _{i},}  [{\displaystyle \sum _{i=1}^{n}f(t_
      {i})\Delta _{i},}]
where      &#x0394;  i   =  x  i   &#x2212;  x  i &#x2212; 1     {\displaystyle
\Delta _{i}=x_{i}-x_{i-1}}  [{\displaystyle \Delta _{i}=x_{i}-x_{i-1}}] is the
width of sub-interval     i   {\displaystyle i}  [i]. Thus, each term of the
sum is the area of a rectangle with height equal to the function value at the
distinguished point of the given sub-interval, and width the same as the sub-
interval width. The mesh of such a tagged partition is the width of the largest
sub-interval formed by the partition,      |   |   &#x0394;  i    |   |  =  max
i = 1 , &#x2026; , n    &#x0394;  i     {\displaystyle ||\Delta _{i}||=\max _
{i=1,\ldots ,n}\Delta _{i}}  [{\displaystyle ||\Delta _{i}||=\max _{i=1,\ldots
,n}\Delta _{i}}]. We say that the Riemann integral of     f   {\displaystyle f}
[f] on     [ a , b ]   {\displaystyle [a,b]}  [[a,b]] is     S   {\displaystyle
S}  [S] if for any     &#x03F5; > 0   {\displaystyle \epsilon >0}  [\epsilon
>0] there exists     &#x03B4; > 0   {\displaystyle \delta >0}  [\delta >0] such
that, for any tagged partition       P     {\displaystyle {\cal {P}}}  [
{\displaystyle {\cal {P}}}] with mesh      |   |   &#x0394;  i    |   |  <
&#x03B4;   {\displaystyle ||\Delta _{i}||<\delta }  [{\displaystyle ||\Delta _
{i}||<\delta }], we have
                |  S &#x2212;  &#x2211;  i = 1   n   f (  t  i   )  &#x0394;  i
            |  < &#x03F5; .   {\displaystyle \left|S-\sum _{i=1}^{n}f(t_
            {i})\Delta _{i}\right|<\epsilon .}  [{\displaystyle \left|S-\sum _
            {i=1}^{n}f(t_{i})\Delta _{i}\right|<\epsilon .}]
This is sometimes denoted       R    &#x222B;  a   b   f = S   {\displaystyle
{\mathcal {R}}\int _{a}^{b}f=S}  [{\displaystyle {\mathcal {R}}\int _{a}^
{b}f=S}]. When the chosen tags give the maximum (respectively, minimum) value
of each interval, the Riemann sum is known as the upper (respectively, lower)
Darboux sum. A function is Darboux integrable if the upper and lower Darboux
sums can be made to be arbitrarily close to each other for a sufficiently small
mesh. Although this definition gives the Darboux integral the appearance of
being a special case of the Riemann integral, they are, in fact, equivalent, in
the sense that a function is Darboux integrable if and only if it is Riemann
integrable, and the values of the integrals are equal. In fact, calculus and
real analysis textbooks often conflate the two, introducing the definition of
the Darboux integral as that of the Riemann integral, due to the slightly
easier to apply definition of the former.
The fundamental_theorem_of_calculus asserts that integration and
differentiation are inverse operations in a certain sense.
*** Lebesgue integration and measure[edit] ***
Main article: Lebesgue_integral
Lebesgue integration is a mathematical construction that extends the integral
to a larger class of functions; it also extends the domains on which these
functions can be defined. The concept of a measure, an abstraction of length,
area, or volume, is central to the definition of the Lebesgue integral and is
important to the study of probability_theory. (For a construction of the
Lebesgue integral, the main article on Lebesgue_integration should be
consulted.)
**** Distributions[edit] ****
Main article: Distribution_(mathematics)
Distributions (or generalized_functions) are objects that generalize functions.
Distributions make it possible to differentiate functions whose derivatives do
not exist in the classical sense. In particular, any locally_integrable
function has a distributional derivative.
**** Relation to complex analysis[edit] ****
Real analysis is an area of analysis that studies concepts such as sequences
and their limits, continuity, differentiation, integration and sequences of
functions. By definition, real analysis focuses on the real_numbers, often
including positive and negative infinity to form the extended_real_line. Real
analysis is closely related to complex_analysis, which studies broadly the same
properties of complex_numbers. In complex analysis, it is natural to define
differentiation via holomorphic_functions, which have a number of useful
properties, such as repeated differentiability, expressability as power_series,
and satisfying the Cauchy_integral_formula.
In real analysis, it is usually more natural to consider differentiable,
smooth, or harmonic_functions, which are more widely applicable, but may lack
some more powerful properties of holomorphic functions. However, results such
as the fundamental_theorem_of_algebra are simpler when expressed in terms of
complex numbers.
Techniques from the theory_of_analytic_functions of a complex variable are
often used in real analysis â such as evaluation of real integrals by residue
calculus.
***** Important results[edit] *****
Important results include the BolzanoâWeierstrass and HeineâBorel_theorems,
the intermediate_value_theorem and mean_value_theorem, Taylor's_theorem, the
fundamental_theorem_of_calculus, the ArzelÃ -Ascoli_theorem, the Stone-
Weierstrass_theorem, Fatou's_lemma, and the monotone_convergence and dominated
convergence_theorems.
***** Generalizations and related areas of mathematics[edit] *****
Various ideas from real analysis can be generalized from the real line to
broader or more abstract contexts. These generalizations link real analysis to
other disciplines and subdisciplines, in many cases playing an important role
in their development as distinct areas of mathematics. For instance,
generalization of ideas like continuous functions and compactness from real
analysis to metric_spaces and topological_spaces connects real analysis to the
field of general_topology, while generalization of finite-dimensional Euclidean
spaces to infinite-dimensional analogs led to the study of Banach_spaces, and
Hilbert_spaces as topics of importance in functional_analysis. Georg_Cantor's
investigation of sets and sequence of real numbers, mappings between them, and
the foundational issues of real analysis gave birth to naive_set_theory. The
study of issues of convergence for sequences of functions eventually gave rise
to Fourier_analysis as a subdiscipline of mathematical analysis. Investigation
of the consequences of generalizing differentiability from functions of a real
variable to ones of a complex variable gave rise to the concept of holomorphic
functions and the inception of complex_analysis as another distinct
subdiscipline of analysis. On the other hand, the generalization of integration
from the Riemann sense to that of Lebesgue led to the formulation of the
concept of abstract measure_spaces, a fundamental concept in measure_theory.
Finally, the generalization of integration from the real line to curves and
surfaces in higher dimensional space brought about the study of vector
calculus, whose further generalization and formalization played an important
role in the evolution of the concepts of differential_forms and smooth_
(differentiable)_manifolds in differential_geometry and other closely related
areas of geometry and topology.
***** See also[edit] *****
    * List_of_real_analysis_topics
    * Time-scale_calculus â a unification of real analysis with calculus of
      finite differences
    * Real_multivariable_function
    * Real_coordinate_space
    * Complex_analysis
    * Non-Newtonian_calculus, alternatives to the classical calculus of Newton
      and Leibniz.
***** References[edit] *****
   1. ^Tao, Terence (2003). "Lecture_notes_for_MATH_131AH" (PDF). Course
      Website for MATH 131AH, Department of Mathematics, UCLA.
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
   3. ^Gaughan, Edward. "1.1 Sequences and Convergence". Introduction to
      Analysis. AMS (2009). ISBN 0-8218-4787-2.
   4. ^ Some authors (e.g., Rudin 1976) use braces instead and write     {  a
      n   }   {\displaystyle \{a_{n}\}}  [\{a_{n}\}]. However, this notation
      conflicts with the usual notation for a set, which, in contrast to a
      sequence, disregards the order and the multiplicity of its elements.
   5. ^Stewart,_James (2008). Calculus: Early Transcendentals (6th ed.).
      Brooks/Cole. ISBN 0-495-01166-5.
   6. ^ Royden_1988, Sect. 5.4, page 108; Nielsen_1997, Definition 15.6 on page
      251; Athreya_&_Lahiri_2006, Definitions 4.4.1, 4.4.2 on pages 128,129.
      The interval I is assumed to be bounded and closed in the former two
      books but not the latter book.
***** Bibliography[edit] *****
    * Abbott, Stephen (2001). Understanding Analysis. Undergradutate Texts in
      Mathematics. New York: Springer-Verlag. ISBN 0-387-95060-5.
Aliprantis,_Charalambos_D.; Burkinshaw, Owen (1998). Principles of real
analysis (3rd ed.). Academic. ISBN 0-12-050257-7.
Bartle,_Robert_G.; Sherbert, Donald R. (2011). Introduction to Real Analysis
(4th ed.). New York: John Wiley and Sons. ISBN 978-0-471-43331-6.
Bressoud,_David (2007). A Radical Approach to Real Analysis. MAA. ISBN 0-88385-
747-2.
Browder, Andrew (1996). Mathematical Analysis: An Introduction. Undergraduate
Texts_in_Mathematics. New York: Springer-Verlag. ISBN 0-387-94614-4.
Carothers, Neal L. (2000). Real_Analysis. Cambridge: Cambridge University
Press. ISBN 978-0521497565.
Dangello, Frank; Seyfried, Michael (1999). Introductory Real Analysis. Brooks
Cole. ISBN 978-0-395-95933-6.
Kolmogorov,_A._N.; Fomin,_S._V. (1975). Introductory_Real_Analysis. Translated
by Richard A. Silverman. Dover Publications. ISBN 0486612260. Retrieved 2 April
2013.
Rudin,_Walter (1976). Principles_of_Mathematical_Analysis. Walter Rudin Student
Series in Advanced Mathematics (3rd ed.). New York: McGrawâHill. ISBN 978-0-
07-054235-8.
Rudin, Walter (1987). Real_and_Complex_Analysis (3rd ed.). New York: McGraw-
Hill. ISBN 978-0-07-054234-1.
Spivak,_Michael (1994). Calculus (3rd ed.). Houston, Texas: Publish or Perish,
Inc. ISBN 091409890X.
***** External links[edit] *****
    * How_We_Got_From_There_to_Here:_A_Story_of_Real_Analysis by Robert Rogers
      and Eugene Boman
    * A_First_Course_in_Analysis by Donald Yau
    * Analysis_WebNotes by John Lindsay Orr
    * Interactive_Real_Analysis by Bert G. Wachsmuth
    * A_First_Analysis_Course by John O'Connor
    * Mathematical_Analysis_I by Elias Zakon
    * Mathematical_Analysis_II by Elias Zakon
    * Trench, William F. (2003). Introduction_to_Real_Analysis (PDF). Prentice
      Hall. ISBN 978-0-13-045786-8.
Earliest_Known_Uses_of_Some_of_the_Words_of_Mathematics:_Calculus_&_Analysis
Basic_Analysis:_Introduction_to_Real_Analysis by Jiri Lebl
Topics_in_Real_and_Functional_Analysis by Gerald_Teschl, University of Vienna.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Real_analysis&oldid=906778823"
Categories:
    * Real_analysis
Hidden categories:
    * Articles_needing_cleanup_from_June_2019
    * All_pages_needing_cleanup
    * Cleanup_tagged_articles_with_a_reason_field_from_June_2019
    * Wikipedia_pages_needing_cleanup_from_June_2019
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
    * Wikibooks
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * Cymraeg
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Bahasa_Indonesia
    * ×¢××¨××ª
    * á¥áá áá£áá
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * æ¥æ¬èª
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à·à·à¶à·à¶½
    * Simple_English
    * SlovenÄina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ××Ö´×××©
    * ä¸­æ
Edit_links
    * This page was last edited on 18 July 2019, at 05:32 (UTC).
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
