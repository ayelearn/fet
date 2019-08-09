The following text has been accessed from https://en.wikipedia.org/wiki/Sequence at Fri Aug 9 00:01:54 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Sequence ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Sequential" redirects here. For the manual transmission, see Sequential_manual
transmission. For other uses, see Sequence_(disambiguation).
In mathematics, a sequence is an enumerated collection of objects in which
repetitions are allowed. Like a set, it contains members (also called elements,
or terms). The number of elements (possibly infinite) is called the length of
the sequence. Unlike a set, the same elements can appear multiple times at
different positions in a sequence, and order matters. Formally, a sequence can
be defined as a function whose domain is either the set of the natural_numbers
(for infinite sequences) or the set of the first n natural numbers (for a
sequence of finite length n). The position of an element in a sequence is its
rank or index; it is the natural number from which the element is the image. It
depends on the context or a specific convention, if the first element has index
0 or 1. When a symbol has been chosen for denoting a sequence, the nth element
of the sequence is denoted by this symbol with n as subscript; for example, the
nth element of the Fibonacci_sequence is generally denoted Fn.
For example, (M, A, R, Y) is a sequence of letters with the letter 'M' first
and 'Y' last. This sequence differs from (A, R, M, Y). Also, the sequence (1,
1, 2, 3, 5, 8), which contains the number 1 at two different positions, is a
valid sequence. Sequences can be finite, as in these examples, or infinite,
such as the sequence of all even positive_integers (2, 4, 6, ...). In computing
and computer_science, finite sequences are sometimes called strings, words or
lists, the different names commonly corresponding to different ways to
represent them in computer_memory; infinite sequences are called streams. The
empty sequence ( ) is included in most notions of sequence, but may be excluded
depending on the context.
An infinite sequence of real_numbers (in blue). This sequence is neither
increasing, decreasing, convergent, nor Cauchy. It is, however, bounded.
⁰
***** Contents *****
    * 1_Examples_and_notation
          o 1.1_Examples
          o 1.2_Indexing
          o 1.3_Defining_a_sequence_by_recursion
    * 2_Formal_definition_and_basic_properties
          o 2.1_Definition
          o 2.2_Finite_and_infinite
          o 2.3_Increasing_and_decreasing
          o 2.4_Bounded
          o 2.5_Subsequences
          o 2.6_Other_types_of_sequences
    * 3_Limits_and_convergence
          o 3.1_Formal_definition_of_convergence
          o 3.2_Applications_and_important_results
          o 3.3_Cauchy_sequences
          o 3.4_Infinite_limits
    * 4_Series
    * 5_Use_in_other_fields_of_mathematics
          o 5.1_Topology
                # 5.1.1_Product_topology
          o 5.2_Analysis
                # 5.2.1_Sequence_spaces
          o 5.3_Linear_algebra
          o 5.4_Abstract_algebra
                # 5.4.1_Free_monoid
                # 5.4.2_Exact_sequences
                # 5.4.3_Spectral_sequences
          o 5.5_Set_theory
          o 5.6_Computing
          o 5.7_Streams
    * 6_See_also
    * 7_Notes
    * 8_References
    * 9_External_links
***** Examples and notation[edit] *****
A sequence can be thought of as a list of elements with a particular order.
Sequences are useful in a number of mathematical disciplines for studying
functions, spaces, and other mathematical structures using the convergence
properties of sequences. In particular, sequences are the basis for series,
which are important in differential_equations and analysis. Sequences are also
of interest in their own right and can be studied as patterns or puzzles, such
as in the study of prime_numbers.
There are a number of ways to denote a sequence, some of which are more useful
for specific types of sequences. One way to specify a sequence is to list the
elements. For example, the first four odd numbers form the sequence (1, 3, 5,
7). This notation can be used for infinite sequences as well. For instance, the
infinite sequence of positive odd integers can be written (1, 3, 5, 7, ...).
Listing is most useful for infinite sequences with a pattern that can be easily
discerned from the first few elements. Other ways to denote a sequence are
discussed after the examples.
**** Examples[edit] ****
A tiling with squares whose sides are successive Fibonacci numbers in length.
The prime_numbers are the natural_numbers bigger than 1 that have no divisors
but 1 and themselves. Taking these in their natural order gives the sequence
(2, 3, 5, 7, 11, 13, 17, ...). The prime numbers are widely used in mathematics
and specifically in number_theory.
The Fibonacci_numbers are the integer sequence whose elements are the sum of
the previous two elements. The first two elements are either 0 and 1 or 1 and 1
so that the sequence is (0, 1, 1, 2, 3, 5, 8, 13, 21, 34, ...).
For a large list of examples of integer sequences, see On-Line_Encyclopedia_of
Integer_Sequences.
Other examples of sequences include ones made up of rational_numbers, real
numbers, and complex_numbers. The sequence (.9, .99, .999, .9999, ...)
approaches the number 1. In fact, every real number can be written as the limit
of a sequence of rational numbers, e.g. via its decimal_expansion. For
instance, Ï is the limit of the sequence (3, 3.1, 3.14, 3.141, 3.1415, ...). A
related sequence is the sequence of decimal digits of Ï, i.e. (3, 1, 4, 1, 5,
9, ...). This sequence does not have any pattern that is easily discernible by
eye, unlike the preceding sequence, which is increasing.
**** Indexing[edit] ****
Other notations can be useful for sequences whose pattern cannot be easily
guessed, or for sequences that do not have a pattern such as the digits of Ï.
One such notation is to write down a general formula for computing the nth term
as a function of n, enclose it in parentheses, and include a subscript
indicating the range of values that n can take. For example, in this notation
the sequence of even numbers could be written as     ( 2 n  )  n &#x2208;  N
{\displaystyle (2n)_{n\in \mathbb {N} }}  [{\displaystyle (2n)_{n\in \mathbb
{N} }}]. The sequence of squares could be written as     (  n  2    )  n
&#x2208;  N      {\displaystyle (n^{2})_{n\in \mathbb {N} }}  [{\displaystyle
(n^{2})_{n\in \mathbb {N} }}]. The variable n is called an index, and the set
of values that it can take is called the index_set.
It is often useful to combine this notation with the technique of treating the
elements of a sequence as variables. This yields expressions like     (  a  n
)  n &#x2208;  N      {\displaystyle (a_{n})_{n\in \mathbb {N} }}  [
{\displaystyle (a_{n})_{n\in \mathbb {N} }}], which denotes a sequence whose
nth element is given by the variable      a  n     {\displaystyle a_{n}}  [a_
{n}]. For example:
              a  1      = 1  st element of&#xA0;  (  a  n    )  n &#x2208;  N
      a  2      = 2  nd element&#xA0;       a  3      = 3  rd element&#xA0;
      &#x22EE;      a  n &#x2212; 1      = ( n &#x2212; 1 )  th element       a
      n      = n  th element       a  n + 1      = ( n + 1 )  th element
      &#x22EE;       {\displaystyle {\begin{aligned}a_{1}&=1{\text{st element
      of }}(a_{n})_{n\in \mathbb {N} }\\a_{2}&=2{\text{nd element }}\\a_{3}&=3
      {\text{rd element }}\\&\vdots \\a_{n-1}&=(n-1){\text{th element}}\\a_
      {n}&=n{\text{th element}}\\a_{n+1}&=(n+1){\text{th element}}\\&\vdots
      \end{aligned}}}  [{\displaystyle {\begin{aligned}a_{1}&=1{\text{st
      element of }}(a_{n})_{n\in \mathbb {N} }\\a_{2}&=2{\text{nd element
      }}\\a_{3}&=3{\text{rd element }}\\&\vdots \\a_{n-1}&=(n-1){\text{th
      element}}\\a_{n}&=n{\text{th element}}\\a_{n+1}&=(n+1){\text{th
      element}}\\&\vdots \end{aligned}}}]
Note that we can consider multiple sequences at the same time by using
different variables; e.g.     (  b  n    )  n &#x2208;  N      {\displaystyle
(b_{n})_{n\in \mathbb {N} }}  [{\displaystyle (b_{n})_{n\in \mathbb {N} }}]
could be a different sequence than     (  a  n    )  n &#x2208;  N
{\displaystyle (a_{n})_{n\in \mathbb {N} }}  [{\displaystyle (a_{n})_{n\in
\mathbb {N} }}]. We can even consider a sequence of sequences:     ( (  a  m ,
n    )  n &#x2208;  N     )  m &#x2208;  N      {\displaystyle ((a_{m,n})_{n\in
\mathbb {N} })_{m\in \mathbb {N} }}  [{\displaystyle ((a_{m,n})_{n\in \mathbb
{N} })_{m\in \mathbb {N} }}] denotes a sequence whose mth term is the sequence
(  a  m , n    )  n &#x2208;  N      {\displaystyle (a_{m,n})_{n\in \mathbb {N}
}}  [{\displaystyle (a_{m,n})_{n\in \mathbb {N} }}].
An alternative to writing the domain of a sequence in the subscript is to
indicate the range of values that the index can take by listing its highest and
lowest legal values. For example, the notation     (  k  2    )  k = 1   10
{\displaystyle (k^{2})_{k=1}^{10}}  [{\displaystyle (k^{2})_{k=1}^{10}}]
denotes the ten-term sequence of squares     ( 1 , 4 , 9 , . . . , 100 )
{\displaystyle (1,4,9,...,100)}  [{\displaystyle (1,4,9,...,100)}]. The limits
&#x221E;   {\displaystyle \infty }  [\infty ] and     &#x2212; &#x221E;
{\displaystyle -\infty }  [-\infty ] are allowed, but they do not represent
valid values for the index, only the supremum or infimum of such values,
respectively. For example, the sequence     (  a  n    )  n = 1   &#x221E;
{\displaystyle (a_{n})_{n=1}^{\infty }}  [{\displaystyle (a_{n})_{n=1}^{\infty
}}] is the same as the sequence     (  a  n    )  n &#x2208;  N
{\displaystyle (a_{n})_{n\in \mathbb {N} }}  [{\displaystyle (a_{n})_{n\in
\mathbb {N} }}], and does not contain an additional term "at infinity". The
sequence     (  a  n    )  n = &#x2212; &#x221E;   &#x221E;     {\displaystyle
(a_{n})_{n=-\infty }^{\infty }}  [{\displaystyle (a_{n})_{n=-\infty }^{\infty
}}] is a bi-infinite sequence, and can also be written as     ( . . . ,  a
&#x2212; 1   ,  a  0   ,  a  1   ,  a  2   , . . . )   {\displaystyle (...,a_{-
1},a_{0},a_{1},a_{2},...)}  [{\displaystyle (...,a_{-1},a_{0},a_{1},a_
{2},...)}].
In cases where the set of indexing numbers is understood, the subscripts and
superscripts are often left off. That is, one simply writes     (  a  k   )
{\displaystyle (a_{k})}  [(a_{k})] for an arbitrary sequence. Often, the index
k is understood to run from 1 to â. However, sequences are frequently indexed
starting from zero, as in
         (  a  k    )  k = 0   &#x221E;   = (  a  0   ,  a  1   ,  a  2   , . .
      . ) .   {\displaystyle (a_{k})_{k=0}^{\infty }=(a_{0},a_{1},a_{2},...).}
      [{\displaystyle (a_{k})_{k=0}^{\infty }=(a_{0},a_{1},a_{2},...).}]
In some cases the elements of the sequence are related naturally to a sequence
of integers whose pattern can be easily inferred. In these cases the index set
may be implied by a listing of the first few abstract elements. For instance,
the sequence of squares of odd_numbers could be denoted in any of the following
ways.
    *    ( 1 , 9 , 25 , . . . )   {\displaystyle (1,9,25,...)}  [{\displaystyle
      (1,9,25,...)}]
    *    (  a  1   ,  a  3   ,  a  5   , . . . ) ,   a  k   =  k  2
      {\displaystyle (a_{1},a_{3},a_{5},...),\qquad a_{k}=k^{2}}  [
      {\displaystyle (a_{1},a_{3},a_{5},...),\qquad a_{k}=k^{2}}]
    *    (  a  2 k &#x2212; 1    )  k = 1   &#x221E;   ,   a  k   =  k  2
      {\displaystyle (a_{2k-1})_{k=1}^{\infty },\qquad a_{k}=k^{2}}  [(a_{2k-
      1})_{k=1}^\infty, \qquad a_k = k^2]
    *    (  a  k    )  k = 1   &#x221E;   ,   a  k   = ( 2 k &#x2212; 1  )  2
      {\displaystyle (a_{k})_{k=1}^{\infty },\qquad a_{k}=(2k-1)^{2}}  [(a_
      {k})_{k=1}^\infty, \qquad a_k = (2k-1)^2]
    *    ( ( 2 k &#x2212; 1  )  2    )  k = 1   &#x221E;     {\displaystyle (
      (2k-1)^{2})_{k=1}^{\infty }}  [((2k-1)^2)_{k=1}^\infty]
Moreover, the subscripts and superscripts could have been left off in the
third, fourth, and fifth notations, if the indexing set was understood to be
the natural_numbers. Note that in the second and third bullets, there is a
well-defined sequence     (  a  k    )  k = 1   &#x221E;     {\displaystyle (a_
{k})_{k=1}^{\infty }}  [{\displaystyle (a_{k})_{k=1}^{\infty }}], but it is not
the same as the sequence denoted by the expression.
**** Defining a sequence by recursion[edit] ****
Main article: Recurrence_relation
Sequences whose elements are related to the previous elements in a
straightforward way are often defined using recursion. This is in contrast to
the definition of sequences of elements as functions of their positions.
To define a sequence by recursion, one needs a rule, called recurrence relation
to construct each element in terms of the ones before it. In addition, enough
initial elements must be provided so that all subsequent elements of the
sequence can be computed by successive applications of the recurrence relation.
The Fibonacci_sequence is a simple classical example, defined by the recurrence
relation
          a  n   =  a  n &#x2212; 1   +  a  n &#x2212; 2   ,   {\displaystyle
      a_{n}=a_{n-1}+a_{n-2},}  [{\displaystyle a_{n}=a_{n-1}+a_{n-2},}]
with initial terms      a  0   = 0   {\displaystyle a_{0}=0}  [a_{0}=0] and
a  1   = 1   {\displaystyle a_{1}=1}  [a_{1}=1]. From this, a simple
computation shows that the first ten terms of this sequence are 0, 1, 1, 2, 3,
5, 8, 13, 21, and 34.
A complicated example of a sequence defined by a recurrence relation is
Recaman's sequence,[1] defined by the recurrence relation
           {     a  n   =  a  n &#x2212; 1   &#x2212; n ,   if the result is
      positive and not already in the previous terms,       a  n   =  a  n
      &#x2212; 1   + n ,   otherwise  ,         {\displaystyle {\begin{cases}a_
      {n}=a_{n-1}-n,\quad {\text{if the result is positive and not already in
      the previous terms,}}\\a_{n}=a_{n-1}+n,\quad {\text{otherwise}},\end
      {cases}}}  [{\displaystyle {\begin{cases}a_{n}=a_{n-1}-n,\quad {\text{if
      the result is positive and not already in the previous terms,}}\\a_{n}=a_
      {n-1}+n,\quad {\text{otherwise}},\end{cases}}}]
with initial term      a  0   = 0.   {\displaystyle a_{0}=0.}  [{\displaystyle
a_{0}=0.}]
A linear recurrence with constant coefficients is a recurrence relation of the
form
          a  n   =  c  0   +  c  1    a  n &#x2212; 1   + &#x22EF; +  c  k    a
      n &#x2212; k   ,   {\displaystyle a_{n}=c_{0}+c_{1}a_{n-1}+\dots +c_{k}a_
      {n-k},}  [{\displaystyle a_{n}=c_{0}+c_{1}a_{n-1}+\dots +c_{k}a_{n-k},}]
where      c  0   , &#x2026; ,  c  k     {\displaystyle c_{0},\dots ,c_{k}}  [
{\displaystyle c_{0},\dots ,c_{k}}] are constants. There is a general method
for expressing the general term      a  n     {\displaystyle a_{n}}  [a_{n}] of
such a sequence as a function of n; see Linear_recurrence. In the case of the
Fibonacci sequence, one has      c  0   = 0 ,  c  1   =  c  2   = 1 ,
{\displaystyle c_{0}=0,c_{1}=c_{2}=1,}  [{\displaystyle c_{0}=0,c_{1}=c_
{2}=1,}] and the resulting function of n is given by Binet's_formula.
A holonomic_sequence is a sequence defined by a recurrence relation of the form
          a  n   =  c  1    a  n &#x2212; 1   + &#x22EF; +  c  k    a  n
      &#x2212; k   ,   {\displaystyle a_{n}=c_{1}a_{n-1}+\dots +c_{k}a_{n-k},}
      [{\displaystyle a_{n}=c_{1}a_{n-1}+\dots +c_{k}a_{n-k},}]
where      c  1   , &#x2026; ,  c  k     {\displaystyle c_{1},\dots ,c_{k}}  [
{\displaystyle c_{1},\dots ,c_{k}}] are polynomials in n. For most holonomic
sequences, there is no explicit formula for expressing explicitly      a  n
{\displaystyle a_{n}}  [a_{n}] as a function of n. Nevertheless holonomic
sequences play an important role in various areas of mathematics. For example,
many special_functions have a Taylor_series whose sequence of coefficients is
holonomic. The use of the recurrence relation allows a fast computation of
values of such special functions.
Not all sequences can be specified by a recurrence relation. An example is the
sequence of prime_numbers in their natural order (2, 3, 5, 7, 11, 13, 17, ...).
***** Formal definition and basic properties[edit] *****
There are many different notions of sequences in mathematics, some of which
(e.g., exact_sequence) are not covered by the definitions and notations
introduced below.
**** Definition[edit] ****
In this article, a sequence is formally defined as a function whose domain is
an interval of integers. This definition covers several different uses of the
word "sequence", including one-sided infinite sequences, bi-infinite sequences,
and finite sequences (see below for definitions of these kinds of sequences).
However, many authors use a narrower definition by requiring the domain of a
sequence to be the set of natural_numbers. This narrower definition has the
disadvantage that it rules out finite sequences and bi-infinite sequences, both
of which are usually called sequences in standard mathematical practice.
Another disadvantage is that, if one removes the first terms of a sequence, one
needs reindexing the remainder terms for fitting this definition. In some
contexts, to shorten exposition, the codomain of the sequence is fixed by
context, for example by requiring it to be the set R of real numbers,[2] the
set C of complex numbers,[3] or a topological_space.[4]
Although sequences are a type of function, they are usually distinguished
notationally from functions in that the input is written as a subscript rather
than in parentheses, that is, an rather than a(n). There are terminological
differences as well: the value of a sequence at the lowest input (often 1) is
called the "first element" of the sequence, the value at the second smallest
input (often 2) is called the "second element", etc. Also, while a function
abstracted from its input is usually denoted by a single letter, e.g. f, a
sequence abstracted from its input is usually written by a notation such as
(  a  n    )  n &#x2208; A     {\displaystyle (a_{n})_{n\in A}}  [
{\displaystyle (a_{n})_{n\in A}}], or just as     (  a  n   ) .
{\displaystyle (a_{n}).}  [{\displaystyle (a_{n}).}] Here A is the domain, or
index set, of the sequence.
Sequences and their limits (see below) are important concepts for studying
topological spaces. An important generalization of sequences is the concept of
nets. A net is a function from a (possibly uncountable) directed_set to a
topological space. The notational conventions for sequences normally apply to
nets as well.
**** Finite and infinite[edit] ****
See also: Ï-language
The length of a sequence is defined as the number of terms in the sequence.
A sequence of a finite length n is also called an n-tuple. Finite sequences
include the empty sequence ( ) that has no elements.
Normally, the term infinite sequence refers to a sequence that is infinite in
one direction, and finite in the otherâthe sequence has a first element, but
no final element. Such a sequence is called a singly infinite sequence or a
one-sided infinite sequence when disambiguation is necessary. In contrast, a
sequence that is infinite in both directionsâi.e. that has neither a first
nor a final elementâis called a bi-infinite sequence, two-way infinite
sequence, or doubly infinite sequence. A function from the set Z of all
integers into a set, such as for instance the sequence of all even integers
( ..., â4, â2, 0, 2, 4, 6, 8... ), is bi-infinite. This sequence could be
denoted     ( 2 n  )  n = &#x2212; &#x221E;   &#x221E;     {\displaystyle (2n)_
{n=-\infty }^{\infty }}  [(2n)_{n=-\infty}^{\infty}].
**** Increasing and decreasing[edit] ****
A sequence is said to be monotonically_increasing, if each term is greater than
or equal to the one before it. For example, the sequence     (  a  n    )  n =
1   &#x221E;     {\displaystyle (a_{n})_{n=1}^{\infty }}  [(a_n)_{n=1}^{\infty}
] is monotonically increasing if and only if an+1     &#x2265;   {\displaystyle
\geq }  [\geq ] an for all n â N. If each consecutive term is strictly
greater than (>) the previous term then the sequence is called strictly
monotonically increasing. A sequence is monotonically decreasing, if each
consecutive term is less than or equal to the previous one, and strictly
monotonically decreasing, if each is strictly less than the previous. If a
sequence is either increasing or decreasing it is called a monotone sequence.
This is a special case of the more general notion of a monotonic_function.
The terms nondecreasing and nonincreasing are often used in place of increasing
and decreasing in order to avoid any possible confusion with strictly
increasing and strictly decreasing, respectively.
**** Bounded[edit] ****
If the sequence of real numbers (an) is such that all the terms are less than
some real number M, then the sequence is said to be bounded from above. In
other words, this means that there exists M such that for all n, an â¤ M. Any
such M is called an upper bound. Likewise, if, for some real m, an â¥ m for
all n greater than some N, then the sequence is bounded from below and any such
m is called a lower bound. If a sequence is both bounded from above and bounded
from below, then the sequence is said to be bounded.
**** Subsequences[edit] ****
A subsequence of a given sequence is a sequence formed from the given sequence
by deleting some of the elements without disturbing the relative positions of
the remaining elements. For instance, the sequence of positive even integers
(2, 4, 6, ...) is a subsequence of the positive integers (1, 2, 3, ...). The
positions of some elements change when other elements are deleted. However, the
relative positions are preserved.
Formally, a subsequence of the sequence     (  a  n    )  n &#x2208;  N
{\displaystyle (a_{n})_{n\in \mathbb {N} }}  [{\displaystyle (a_{n})_{n\in
\mathbb {N} }}] is any sequence of the form     (  a   n  k      )  k &#x2208;
N      {\displaystyle (a_{n_{k}})_{k\in \mathbb {N} }}  [{\displaystyle (a_{n_
{k}})_{k\in \mathbb {N} }}], where     (  n  k    )  k &#x2208;  N
{\displaystyle (n_{k})_{k\in \mathbb {N} }}  [{\displaystyle (n_{k})_{k\in
\mathbb {N} }}] is a strictly increasing sequence of positive integers.
**** Other types of sequences[edit] ****
Some other types of sequences that are easy to define include:
    * An integer_sequence is a sequence whose terms are integers.
    * A polynomial_sequence is a sequence whose terms are polynomials.
    * A positive integer sequence is sometimes called multiplicative, if anm =
      an am for all pairs n, m such that n and m are coprime.[5] In other
      instances, sequences are often called multiplicative, if an = na1 for all
      n. Moreover, a multiplicative Fibonacci sequence[6] satisfies the
      recursion relation an = anâ1 anâ2.
    * A binary_sequence is a sequence whose terms have one of two discrete
      values, e.g. base_2 values (0,1,1,0, ...), a series of coin tosses
      (Heads/Tails) H,T,H,H,T, ..., the answers to a set of True or False
      questions (T, F, T, T, ...), and so on.
***** Limits and convergence[edit] *****
Main article: Limit_of_a_sequence
The plot of a convergent sequence (an) is shown in blue. From the graph we can
see that the sequence is converging to the limit zero as n increases.
An important property of a sequence is convergence. If a sequence converges, it
converges to a particular value known as the limit. If a sequence converges to
some limit, then it is convergent. A sequence that does not converge is
divergent.
Informally, a sequence has a limit if the elements of the sequence become
closer and closer to some value     L   {\displaystyle L}  [L] (called the
limit of the sequence), and they become and remain arbitrarily close to     L
{\displaystyle L}  [L], meaning that given a real number     d   {\displaystyle
d}  [d] greater than zero, all but a finite number of the elements of the
sequence have a distance from     L   {\displaystyle L}  [L] less than     d
{\displaystyle d}  [d].
For example, the sequence      a  n   =    n + 1   2  n  2
{\displaystyle a_{n}={\frac {n+1}{2n^{2}}}}  [{\displaystyle a_{n}={\frac {n+1}
{2n^{2}}}}] shown to the right converges to the value 0. On the other hand, the
sequences      b  n   =  n  3     {\displaystyle b_{n}=n^{3}}  [{\displaystyle
b_{n}=n^{3}}] (which begins 1, 8, 27, …) and      c  n   = ( &#x2212; 1  )  n
{\displaystyle c_{n}=(-1)^{n}}  [{\displaystyle c_{n}=(-1)^{n}}] (which begins
-1, 1, -1, 1, …) are both divergent.
If a sequence converges, then the value it converges to is unique. This value
is called the limit of the sequence. The limit of a convergent sequence
(  a  n   )   {\displaystyle (a_{n})}  [(a_{n})] is normally denoted      lim
n &#x2192; &#x221E;    a  n     {\displaystyle \lim _{n\to \infty }a_{n}}  [
{\displaystyle \lim _{n\to \infty }a_{n}}]. If     (  a  n   )   {\displaystyle
(a_{n})}  [(a_{n})] is a divergent sequence, then the expression      lim  n
&#x2192; &#x221E;    a  n     {\displaystyle \lim _{n\to \infty }a_{n}}  [
{\displaystyle \lim _{n\to \infty }a_{n}}] is meaningless.
**** Formal definition of convergence[edit] ****
A sequence of real numbers     (  a  n   )   {\displaystyle (a_{n})}  [(a_{n})]
converges to a real number     L   {\displaystyle L}  [L] if, for all
&#x03B5; > 0   {\displaystyle \varepsilon >0}  [\varepsilon >0], there exists a
natural number     N   {\displaystyle N}  [N] such that for all     n &#x2265;
N   {\displaystyle n\geq N}  [n\geq N] we have[2]
         |   a  n   &#x2212; L  |  < &#x03B5; .   {\displaystyle |a_{n}-
     L|<\varepsilon .}  [{\displaystyle |a_{n}-L|<\varepsilon .}]
If     (  a  n   )   {\displaystyle (a_{n})}  [(a_{n})] is a sequence of
complex numbers rather than a sequence of real numbers, this last formula can
still be used to define convergence, with the provision that      |  &#x22C5;
|    {\displaystyle |\cdot |}  [|\cdot |] denotes the complex modulus, i.e.
|  z  |  =    z  &#x2217;   z     {\displaystyle |z|={\sqrt {z^{*}z}}}  [
{\displaystyle |z|={\sqrt {z^{*}z}}}]. If     (  a  n   )   {\displaystyle (a_
{n})}  [(a_{n})] is a sequence of points in a metric_space, then the formula
can be used to define convergence, if the expression      |   a  n   &#x2212; L
|    {\displaystyle |a_{n}-L|}  [{\displaystyle |a_{n}-L|}] is replaced by the
expression      dist  (  a  n   , L )   {\displaystyle {\text{dist}}(a_{n},L)}
[{\displaystyle {\text{dist}}(a_{n},L)}], which denotes the distance between
a  n     {\displaystyle a_{n}}  [a_{n}] and     L   {\displaystyle L}  [L].
**** Applications and important results[edit] ****
If     (  a  n   )   {\displaystyle (a_{n})}  [(a_{n})] and     (  b  n   )
{\displaystyle (b_{n})}  [(b_{n})] are convergent sequences, then the following
limits exist, and can be computed as follows:[2][7]
    *     lim  n &#x2192; &#x221E;   (  a  n   &#x00B1;  b  n   ) =  lim  n
      &#x2192; &#x221E;    a  n   &#x00B1;  lim  n &#x2192; &#x221E;    b  n
      {\displaystyle \lim _{n\to \infty }(a_{n}\pm b_{n})=\lim _{n\to \infty
      }a_{n}\pm \lim _{n\to \infty }b_{n}}  [{\displaystyle \lim _{n\to \infty
      }(a_{n}\pm b_{n})=\lim _{n\to \infty }a_{n}\pm \lim _{n\to \infty }b_
      {n}}]
    *     lim  n &#x2192; &#x221E;   c  a  n   = c  lim  n &#x2192; &#x221E;
      a  n     {\displaystyle \lim _{n\to \infty }ca_{n}=c\lim _{n\to \infty
      }a_{n}}  [{\displaystyle \lim _{n\to \infty }ca_{n}=c\lim _{n\to \infty
      }a_{n}}] for all     c   {\displaystyle c}  [c]
    *     lim  n &#x2192; &#x221E;   (  a  n    b  n   ) =  (   lim  n &#x2192;
      &#x221E;    a  n    )   (   lim  n &#x2192; &#x221E;    b  n    )
      {\displaystyle \lim _{n\to \infty }(a_{n}b_{n})=\left(\lim _{n\to \infty
      }a_{n}\right)\left(\lim _{n\to \infty }b_{n}\right)}  [{\displaystyle
      \lim _{n\to \infty }(a_{n}b_{n})=\left(\lim _{n\to \infty }a_
      {n}\right)\left(\lim _{n\to \infty }b_{n}\right)}]
    *     lim  n &#x2192; &#x221E;      a  n    b  n     =     lim  n &#x2192;
      &#x221E;    a  n      lim  n &#x2192; &#x221E;    b  n
      {\displaystyle \lim _{n\to \infty }{\frac {a_{n}}{b_{n}}}={\frac {\lim
      \limits _{n\to \infty }a_{n}}{\lim \limits _{n\to \infty }b_{n}}}}  [
      {\displaystyle \lim _{n\to \infty }{\frac {a_{n}}{b_{n}}}={\frac {\lim
      \limits _{n\to \infty }a_{n}}{\lim \limits _{n\to \infty }b_{n}}}}],
      provided that      lim  n &#x2192; &#x221E;    b  n   &#x2260; 0
      {\displaystyle \lim _{n\to \infty }b_{n}\neq 0}  [\lim _{n\to \infty }b_
      {n}\neq 0]
    *     lim  n &#x2192; &#x221E;    a  n   p   =   (   lim  n &#x2192;
      &#x221E;    a  n    )   p     {\displaystyle \lim _{n\to \infty }a_{n}^
      {p}=\left(\lim _{n\to \infty }a_{n}\right)^{p}}  [{\displaystyle \lim _
      {n\to \infty }a_{n}^{p}=\left(\lim _{n\to \infty }a_{n}\right)^{p}}] for
      all     p > 0   {\displaystyle p>0}  [p>0]
Moreover:
    * If      a  n   &#x2264;  b  n     {\displaystyle a_{n}\leq b_{n}}  [a_
      {n}\leq b_{n}] for all     n   {\displaystyle n}  [n] greater than some
      N   {\displaystyle N}  [N], then      lim  n &#x2192; &#x221E;    a  n
      &#x2264;  lim  n &#x2192; &#x221E;    b  n     {\displaystyle \lim _{n\to
      \infty }a_{n}\leq \lim _{n\to \infty }b_{n}}  [\lim _{n\to \infty }a_
      {n}\leq \lim _{n\to \infty }b_{n}].[a]
    * (Squeeze_Theorem)
      If     (  c  n   )   {\displaystyle (c_{n})}  [{\displaystyle (c_{n})}]
      is a sequence such that      a  n   &#x2264;  c  n   &#x2264;  b  n
      {\displaystyle a_{n}\leq c_{n}\leq b_{n}}  [a_{n}\leq c_{n}\leq b_{n}]
      for all     n > N   {\displaystyle n>N}  [n>N] and      lim  n &#x2192;
      &#x221E;    a  n   =  lim  n &#x2192; &#x221E;    b  n   = L
      {\displaystyle \lim _{n\to \infty }a_{n}=\lim _{n\to \infty }b_{n}=L}
      [\lim _{n\to \infty }a_{n}=\lim _{n\to \infty }b_{n}=L],
      then     (  c  n   )   {\displaystyle (c_{n})}  [{\displaystyle (c_{n})}]
      is convergent, and      lim  n &#x2192; &#x221E;    c  n   = L
      {\displaystyle \lim _{n\to \infty }c_{n}=L}  [\lim _{n\to \infty }c_
      {n}=L].
    * If a sequence is bounded and monotonic then it is convergent.
    * A sequence is convergent if and only if all of its subsequences are
      convergent.
**** Cauchy sequences[edit] ****
Main article: Cauchy_sequence
The plot of a Cauchy sequence (Xn), shown in blue, as Xn versus n. In the graph
the sequence appears to be converging to a limit as the distance between
consecutive terms in the sequence gets smaller as n increases. In the real
numbers every Cauchy sequence converges to some limit.
A Cauchy sequence is a sequence whose terms become arbitrarily close together
as n gets very large. The notion of a Cauchy sequence is important in the study
of sequences in metric_spaces, and, in particular, in real_analysis. One
particularly important result in real analysis is Cauchy characterization of
convergence for sequences:
      A sequence of real numbers is convergent (in the reals) if and only if it
      is Cauchy.
In contrast, there are Cauchy sequences of rational_numbers that are not
convergent in the rationals, e.g. the sequence defined by x1 = 1 and xn+1 = xn
+ 2/xn/2 is Cauchy, but has no rational limit, cf. here. More generally, any
sequence of rational numbers that converges to an irrational_number is Cauchy,
but not convergent when interpreted as a sequence in the set of rational
numbers.
Metric spaces that satisfy the Cauchy characterization of convergence for
sequences are called complete_metric_spaces and are particularly nice for
analysis.
**** Infinite limits[edit] ****
In calculus, it is common to define notation for sequences which do not
converge in the sense discussed above, but which instead become and remain
arbitrarily large, or become and remain arbitrarily negative. If      a  n
{\displaystyle a_{n}}  [a_{n}] becomes arbitrarily large as     n &#x2192;
&#x221E;   {\displaystyle n\to \infty }  [n\to \infty ], we write
          lim  n &#x2192; &#x221E;    a  n   = &#x221E; .   {\displaystyle \lim
      _{n\to \infty }a_{n}=\infty .}  [\lim_{n\to\infty}a_n = \infty.]
In this case we say that the sequence diverges, or that it converges to
infinity. An example of such a sequence is an = n.
If      a  n     {\displaystyle a_{n}}  [a_{n}] becomes arbitrarily negative
(i.e. negative and large in magnitude) as     n &#x2192; &#x221E;
{\displaystyle n\to \infty }  [n\to \infty ], we write
          lim  n &#x2192; &#x221E;    a  n   = &#x2212; &#x221E;
      {\displaystyle \lim _{n\to \infty }a_{n}=-\infty }  [\lim_{n\to\infty}a_n
      = -\infty]
and say that the sequence diverges or converges to negative infinity.
***** Series[edit] *****
Main article: Series_(mathematics)
A series is, informally speaking, the sum of the terms of a sequence. That is,
it is an expression of the form      &#x2211;  n = 1   &#x221E;    a  n
{\displaystyle \sum _{n=1}^{\infty }a_{n}}  [{\displaystyle \sum _{n=1}^{\infty
}a_{n}}] or      a  1   +  a  2   + &#x22EF;   {\displaystyle a_{1}+a_
{2}+\cdots }  [{\displaystyle a_{1}+a_{2}+\cdots }], where     (  a  n   )
{\displaystyle (a_{n})}  [(a_{n})] is a sequence of real or complex numbers.
The partial sums of a series are the expressions resulting from replacing the
infinity symbol with a finite number, i.e. the Nth partial sum of the series
&#x2211;  n = 1   &#x221E;    a  n     {\displaystyle \sum _{n=1}^{\infty }a_
{n}}  [{\displaystyle \sum _{n=1}^{\infty }a_{n}}] is the number
          S  N   =  &#x2211;  n = 1   N    a  n   =  a  1   +  a  2   +
      &#x22EF; +  a  N   .   {\displaystyle S_{N}=\sum _{n=1}^{N}a_{n}=a_{1}+a_
      {2}+\cdots +a_{N}.}  [{\displaystyle S_{N}=\sum _{n=1}^{N}a_{n}=a_{1}+a_
      {2}+\cdots +a_{N}.}]
The partial sums themselves form a sequence     (  S  N    )  N &#x2208;  N
{\displaystyle (S_{N})_{N\in \mathbb {N} }}  [{\displaystyle (S_{N})_{N\in
\mathbb {N} }}], which is called the sequence of partial sums of the series
&#x2211;  n = 1   &#x221E;    a  n     {\displaystyle \sum _{n=1}^{\infty }a_
{n}}  [{\displaystyle \sum _{n=1}^{\infty }a_{n}}]. If the sequence of partial
sums converges, then we say that the series      &#x2211;  n = 1   &#x221E;
a  n     {\displaystyle \sum _{n=1}^{\infty }a_{n}}  [{\displaystyle \sum _
{n=1}^{\infty }a_{n}}] is convergent, and the limit      lim  N &#x2192;
&#x221E;    S  N     {\displaystyle \lim _{N\to \infty }S_{N}}  [{\displaystyle
\lim _{N\to \infty }S_{N}}] is called the value of the series. The same
notation is used to denote a series and its value, i.e. we write      &#x2211;
n = 1   &#x221E;    a  n   =  lim  N &#x2192; &#x221E;    S  N
{\displaystyle \sum _{n=1}^{\infty }a_{n}=\lim _{N\to \infty }S_{N}}  [
{\displaystyle \sum _{n=1}^{\infty }a_{n}=\lim _{N\to \infty }S_{N}}].
***** Use in other fields of mathematics[edit] *****
**** Topology[edit] ****
Sequences play an important role in topology, especially in the study of metric
spaces. For instance:
    * A metric_space is compact exactly when it is sequentially_compact.
    * A function from a metric space to another metric space is continuous
      exactly when it takes convergent sequences to convergent sequences.
    * A metric space is a connected_space if and only if, whenever the space is
      partitioned into two sets, one of the two sets contains a sequence
      converging to a point in the other set.
    * A topological_space is separable exactly when there is a dense sequence
      of points.
Sequences can be generalized to nets or filters. These generalizations allow
one to extend some of the above theorems to spaces without metrics.
*** Product topology[edit] ***
The topological_product of a sequence of topological spaces is the cartesian
product of those spaces, equipped with a natural_topology called the product
topology.
More formally, given a sequence of spaces     (  X  i    )  i &#x2208;  N
{\displaystyle (X_{i})_{i\in \mathbb {N} }}  [{\displaystyle (X_{i})_{i\in
\mathbb {N} }}], the product space
         X :=  &#x220F;  i &#x2208;  N     X  i   ,   {\displaystyle X:=\prod _
      {i\in \mathbb {N} }X_{i},}  [{\displaystyle X:=\prod _{i\in \mathbb {N}
      }X_{i},}]
is defined as the set of all sequences     (  x  i    )  i &#x2208;  N
{\displaystyle (x_{i})_{i\in \mathbb {N} }}  [{\displaystyle (x_{i})_{i\in
\mathbb {N} }}] such that for each i,      x  i     {\displaystyle x_{i}}  [x_
{i}] is an element of      X  i     {\displaystyle X_{i}}  [X_{i}]. The
canonical_projections are the maps pi : X → Xi defined by the equation      p
i   ( (  x  j    )  j &#x2208;  N    ) =  x  i     {\displaystyle p_{i}((x_
{j})_{j\in \mathbb {N} })=x_{i}}  [{\displaystyle p_{i}((x_{j})_{j\in \mathbb
{N} })=x_{i}}]. Then the product topology on X is defined to be the coarsest
topology (i.e. the topology with the fewest open sets) for which all the
projections pi are continuous. The product topology is sometimes called the
Tychonoff topology.
**** Analysis[edit] ****
In analysis, when talking about sequences, one will generally consider
sequences of the form
         (  x  1   ,  x  2   ,  x  3   , &#x2026; )  &#xA0;or&#xA0;  (  x  0
      ,  x  1   ,  x  2   , &#x2026; )   {\displaystyle (x_{1},x_{2},x_
      {3},\dots ){\text{ or }}(x_{0},x_{1},x_{2},\dots )}  [{\displaystyle (x_
      {1},x_{2},x_{3},\dots ){\text{ or }}(x_{0},x_{1},x_{2},\dots )}]
which is to say, infinite sequences of elements indexed by natural_numbers.
It may be convenient to have the sequence start with an index different from 1
or 0. For example, the sequence defined by xn = 1/log(n) would be defined only
for n â¥ 2. When talking about such infinite sequences, it is usually
sufficient (and does not change much for most considerations) to assume that
the members of the sequence are defined at least for all indices large_enough,
that is, greater than some given N.
The most elementary type of sequences are numerical ones, that is, sequences of
real or complex numbers. This type can be generalized to sequences of elements
of some vector_space. In analysis, the vector spaces considered are often
function_spaces. Even more generally, one can study sequences with elements in
some topological_space.
*** Sequence spaces[edit] ***
Main article: Sequence_space
A sequence_space is a vector_space whose elements are infinite sequences of
real or complex numbers. Equivalently, it is a function_space whose elements
are functions from the natural_numbers to the field K, where K is either the
field of real numbers or the field of complex numbers. The set of all such
functions is naturally identified with the set of all possible infinite
sequences with elements in K, and can be turned into a vector_space under the
operations of pointwise_addition of functions and pointwise scalar
multiplication. All sequence spaces are linear_subspaces of this space.
Sequence spaces are typically equipped with a norm, or at least the structure
of a topological_vector_space.
The most important sequences spaces in analysis are the âp spaces, consisting
of the p-power summable sequences, with the p-norm. These are special cases of
Lp_spaces for the counting_measure on the set of natural numbers. Other
important classes of sequences like convergent sequences or null_sequences form
sequence spaces, respectively denoted c and c0, with the sup norm. Any sequence
space can also be equipped with the topology of pointwise_convergence, under
which it becomes a special kind of FrÃ©chet_space called an FK-space.
**** Linear algebra[edit] ****
Sequences over a field may also be viewed as vectors in a vector_space.
Specifically, the set of F-valued sequences (where F is a field) is a function
space (in fact, a product_space) of F-valued functions over the set of natural
numbers.
**** Abstract algebra[edit] ****
Abstract algebra employs several types of sequences, including sequences of
mathematical objects such as groups or rings.
*** Free monoid[edit] ***
Main article: Free_monoid
If A is a set, the free_monoid over A (denoted A*, also called Kleene_star of
A) is a monoid containing all the finite sequences (or strings) of zero or more
elements of A, with the binary operation of concatenation. The free_semigroup
A+ is the subsemigroup of A* containing all elements except the empty sequence.
*** Exact sequences[edit] ***
Main article: Exact_sequence
In the context of group_theory, a sequence
          G  0      &#x2192;   f  1        G  1      &#x2192;   f  2        G
      2      &#x2192;   f  3       &#x22EF;    &#x2192;   f  n        G  n
      {\displaystyle G_{0}\;{\xrightarrow {f_{1}}}\;G_{1}\;{\xrightarrow {f_
      {2}}}\;G_{2}\;{\xrightarrow {f_{3}}}\;\cdots \;{\xrightarrow {f_{n}}}\;G_
      {n}}  [G_{0}\;{\xrightarrow {f_{1}}}\;G_{1}\;{\xrightarrow {f_{2}}}\;G_
      {2}\;{\xrightarrow {f_{3}}}\;\cdots \;{\xrightarrow {f_{n}}}\;G_{n}]
of groups and group_homomorphisms is called exact, if the image (or range) of
each homomorphism is equal to the kernel of the next:
          i m  (  f  k   ) =  k e r  (  f  k + 1   )   {\displaystyle \mathrm
      {im} (f_{k})=\mathrm {ker} (f_{k+1})}  [\mathrm {im} (f_{k})=\mathrm
      {ker} (f_{k+1})]
Note that the sequence of groups and homomorphisms may be either finite or
infinite.
A similar definition can be made for certain other algebraic_structures. For
example, one could have an exact sequence of vector_spaces and linear_maps, or
of modules and module_homomorphisms.
*** Spectral sequences[edit] ***
Main article: Spectral_sequence
In homological_algebra and algebraic_topology, a spectral sequence is a means
of computing homology groups by taking successive approximations. Spectral
sequences are a generalization of exact_sequences, and since their introduction
by Jean_Leray (1946), they have become an important research tool, particularly
in homotopy_theory.
**** Set theory[edit] ****
An ordinal-indexed_sequence is a generalization of a sequence. If Î± is a limit
ordinal and X is a set, an Î±-indexed sequence of elements of X is a function
from Î± to X. In this terminology an Ï-indexed sequence is an ordinary
sequence.
**** Computing[edit] ****
In computer_science, finite sequences are called lists. Potentially infinite
sequences are called streams. Finite sequences of characters or digits are
called strings.
**** Streams[edit] ****
Infinite sequences of digits (or characters) drawn from a finite alphabet are
of particular interest in theoretical_computer_science. They are often referred
to simply as sequences or streams, as opposed to finite strings. Infinite
binary sequences, for instance, are infinite sequences of bits (characters
drawn from the alphabet {0, 1}). The set C = {0, 1}â of all infinite binary
sequences is sometimes called the Cantor_space.
An infinite binary sequence can represent a formal_language (a set of strings)
by setting the n th bit of the sequence to 1 if and only if the n th string (in
shortlex_order) is in the language. This representation is useful in the
diagonalization_method for proofs.[8]
***** See also[edit] *****
    * Enumeration
    * On-Line_Encyclopedia_of_Integer_Sequences
    * Recurrence_relation
    * Sequence_space
  Operations
    * Cauchy_product
  Examples
    * Discrete-time_signal
    * Farey_sequence
    * Fibonacci_sequence
    * Look-and-say_sequence
    * ThueâMorse_sequence
  Types
    * Â±1-sequence
    * Arithmetic_progression
    * Automatic_sequence
    * Cauchy_sequence
    * Constant-recursive_sequence
    * Geometric_progression
    * Holonomic_sequence
    * Regular_sequence
    * Pseudorandom_binary_sequence
    * Random_sequence
  Related concepts
    * List_(computing)
    * Net_(topology) (a generalization of sequences)
    * Ordinal-indexed_sequence
    * Recursion_(computer_science)
    * Set_(mathematics)
    * Tuple
***** Notes[edit] *****
   1. ^ Note that if the inequalities are replaced by strict inequalities then
      this is false: There are sequences such that      a  n   <  b  n
      {\displaystyle a_{n}<b_{n}}  [a_{n}<b_{n}] for all     n   {\displaystyle
      n}  [n], but      lim  n &#x2192; &#x221E;    a  n   =  lim  n &#x2192;
      &#x221E;    b  n     {\displaystyle \lim _{n\to \infty }a_{n}=\lim _{n\to
      \infty }b_{n}}  [{\displaystyle \lim _{n\to \infty }a_{n}=\lim _{n\to
      \infty }b_{n}}].
***** References[edit] *****
   1. ^Sloane,_N. J. A. (ed.). "Sequence&#x20;A005132&#x20;(RecamÃ¡n's
      sequence)". The On-Line_Encyclopedia_of_Integer_Sequences. OEIS
      Foundation. Retrieved 26 January 2018.
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
   3. ^ a b cGaughan, Edward (2009). "1.1 Sequences and Convergence".
      Introduction to Analysis. AMS (2009). ISBN 978-0-8218-4787-9.
   4. ^Edward B. Saff & Arthur David Snider (2003). "Chapter_2.1". Fundamentals
      of Complex Analysis. ISBN 978-01-390-7874-3.
   5. ^James R. Munkres (2000). "Chapters_1&2". Topology. ISBN 978-01-318-1629-
      9.
   6. ^Lando, Sergei K. (2003-10-21). "7.4 Multiplicative sequences". Lectures
      on generating functions. AMS. ISBN 978-0-8218-3481-7.
   7. ^Falcon, Sergio (2003). "Fibonacci's multiplicative sequence".
      International Journal of Mathematical Education in Science and
      Technology. 34 (2): 310â315. doi:10.1080/0020739031000158362.
   8. ^Dawikins, Paul. "Series_and_Sequences". Paul's Online Math Notes/Calc II
      (notes). Retrieved 18 December 2012.
   9. ^Oflazer, Kemal. "FORMAL_LANGUAGES,_AUTOMATA_AND_COMPUTATION:
      DECIDABILITY" (PDF). cmu.edu. Carnegie-Mellon University. Retrieved 24
      April 2015.
***** External links[edit] *****
 Look up sequence in Wiktionary, the free dictionary.
 Look up enumerate or collection in Wiktionary, the free dictionary.
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Sequence", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
The_On-Line_Encyclopedia_of_Integer_Sequences
Journal_of_Integer_Sequences (free)
"Sequence". PlanetMath.
    * v
    * t
    * e
Sequences and series
                            * Arithmetic_progression
                            * Geometric_progression
                            * Harmonic_progression
               Basic        * Square_number
                            * Cubic_number
                            * Factorial
                            * Powers_of_two
                            * Powers_of_10
Integer                     * Complete_sequence
sequences                   * Fibonacci_numbers
                            * Figurate_number
                            * Heptagonal_number
               Advanced     * Hexagonal_number
               (list)       * Lucas_number
                            * Pell_number
                            * Pentagonal_number
                            * Polygonal_number
                            * Triangular_number
Properties of      * Cauchy_sequence
sequences          * Monotone_sequence
                   * Periodic_sequence
                   * Convergent_series
                   * Divergent_series
Properties of      * Conditional_convergence
series             * Absolute_convergence
                   * Uniform_convergence                                                                  [Fibonacci
                   * Alternating_series                                                                   spiral
                   * Telescoping_series                                                                   with
                              * 1/2_â_1/4_+_1/8_â_1/16_+_â¯                                 square
               Convergent     * 1/2_+_1/4_+_1/8_+_1/16_+_â¯                                           sizes_up
                              * 1/4_+_1/16_+_1/64_+_1/256_+_â¯                                        to_34.]
                              * 1_+_1/2s+_1/3s_+_..._(Riemann_zeta_function)
                              * 1_+_1_+_1_+_1_+_â¯
                              * 1_+_2_+_3_+_4_+_â¯
Explicit                      * 1_+_2_+_4_+_8_+_â¯
series                        * 1_â_1_+_1_â_1_+_â¯_(Grandi's_series)
               Divergent      * Infinite_arithmetic_series
                              * 1_â_2_+_3_â_4_+_â¯
                              * 1_â_2_+_4_â_8_+_â¯
                              * 1_+_1/2_+_1/3_+_1/4_+_â¯_(harmonic_series)
                              * 1_â_1_+_2_â_6_+_24_â_120_+_â¯_(alternating_factorials)
                              * 1/2_+_1/3_+_1/5_+_1/7_+_1/11_+_â¯_(inverses_of_primes)
                   * Taylor_series
                   * Power_series
                   * Formal_power_series
Kinds of           * Laurent_series
series             * Puiseux_series
                   * Dirichlet_series
                   * Trigonometric_series
                   * Fourier_series
                   * Generating_series
                   * Generalized_hypergeometric_series
                   * Hypergeometric_function_of_a_matrix_argument
Hypergeometric     * Lauricella_hypergeometric_series
series             * Modular_hypergeometric_series
                   * Riemann's_differential_equation
                   * Theta_hypergeometric_series
    * [Wikipedia book] Book
    * [Category] Category

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Sequence&oldid=905326260"
Categories:
    * Elementary_mathematics
    * Sequences_and_series
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
    * Asturianu
    * AzÉrbaycanca
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
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
    * Gaeilge
    * Galego
    * Ð¥Ð°Ð»ÑÐ¼Ð³
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Ido
    * Bahasa_Indonesia
    * Interlingua
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Latina
    * LatvieÅ¡u
    * LÃ«tzebuergesch
    * LietuviÅ³
    * Lumbaart
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * MirandÃ©s
    * Nederlands
    * à¤¨à¥à¤ªà¤¾à¤²à¥
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
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
    * ÅlÅ¯nski
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 8 July 2019, at 12:21 (UTC).
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
