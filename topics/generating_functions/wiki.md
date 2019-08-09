The following text has been accessed from https://en.wikipedia.org/wiki/Generating_function at Fri Aug 9 01:08:51 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Generating function ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about generating functions in mathematics. For generating
functions in classical mechanics, see Generating_function_(physics). For
signalling molecule, see Epidermal_growth_factor. For generators in computer
programming, see Generator_(computer_programming). For the moment generating
function in statistics, see Moment_generating_function.
 This article has multiple issues. Please help improve_it or discuss these
 issues on the talk_page. (Learn_how_and_when_to_remove_these_template
 messages)
  This article may be too technical for most readers to understand. Please help
  improve_it to make_it_understandable_to_non-experts, without removing the
  technical details. (March 2018)(Learn_how_and_when_to_remove_this_template
  message)
  This article may be too_long to read and navigate comfortably. The readable
  prose_size is 76 kilobytes. Please consider splitting content into sub-
  articles, condensing it, or adding subheadings. (March 2018)
 (Learn_how_and_when_to_remove_this_template_message)
In mathematics, a generating function is a way of encoding an infinite_sequence
of numbers (an) by treating them as the coefficients of a power_series. This
formal power series is the generating function. Unlike an ordinary series, this
formal_series is allowed to diverge, meaning that the generating function is
not always a true function and the "variable" is actually an indeterminate.
Generating functions were first introduced by Abraham_de_Moivre in 1730, in
order to solve the general linear recurrence problem.[1] One can generalize to
formal series in more than one indeterminate, to encode information about
arrays of numbers indexed by several natural numbers.
There are various types of generating functions, including ordinary generating
functions, exponential generating functions, Lambert series, Bell series, and
Dirichlet series; definitions and examples are given below. Every sequence in
principle has a generating function of each type (except that Lambert and
Dirichlet series require indices to start at 1 rather than 0), but the ease
with which they can be handled may differ considerably. The particular
generating function, if any, that is most useful in a given context will depend
upon the nature of the sequence and the details of the problem being addressed.
Generating functions are often expressed in closed_form (rather than as a
series), by some expression involving operations defined for formal series.
These expressions in terms of the indeterminate x may involve arithmetic
operations, differentiation with respect to x and composition with (i.e.,
substitution into) other generating functions; since these operations are also
defined for functions, the result looks like a function of x. Indeed, the
closed form expression can often be interpreted as a function that can be
evaluated at (sufficiently small) concrete values of x, and which has the
formal series as its series_expansion; this explains the designation
"generating functions". However such interpretation is not required to be
possible, because formal series are not required to give a convergent_series
when a nonzero numeric value is substituted for x. Also, not all expressions
that are meaningful as functions of x are meaningful as expressions designating
formal series; for example, negative and fractional powers of x are examples of
functions that do not have a corresponding formal power series.
Generating functions are not functions in the formal sense of a mapping from a
domain to a codomain. Generating functions are sometimes called generating
series,[2] in that a series of terms can be said to be the generator of its
sequence of term coefficients.
⁰
***** Contents *****
    * 1_Definitions
          o 1.1_Ordinary_generating_function_(OGF)
          o 1.2_Exponential_generating_function_(EGF)
          o 1.3_Poisson_generating_function
          o 1.4_Lambert_series
          o 1.5_Bell_series
          o 1.6_Dirichlet_series_generating_functions_(DGFs)
          o 1.7_Polynomial_sequence_generating_functions
    * 2_Ordinary_generating_functions
          o 2.1_Examples_of_generating_functions_for_simple_sequences
          o 2.2_Rational_functions
          o 2.3_Operations_on_generating_functions
                # 2.3.1_Multiplication_yields_convolution
                # 2.3.2_Shifting_sequence_indices
                # 2.3.3_Differentiation_and_integration_of_generating_functions
                # 2.3.4_Enumerating_arithmetic_progressions_of_sequences
          o 2.4_P-recursive_sequences_and_holonomic_generating_functions
                # 2.4.1_Definitions
                # 2.4.2_Examples
                # 2.4.3_Software_for_working_with_P-recursive_sequences_and
                  holonomic_generating_functions
          o 2.5_Relation_to_discrete-time_Fourier_transform
          o 2.6_Asymptotic_growth_of_a_sequence
                # 2.6.1_Asymptotic_growth_of_the_sequence_of_squares
                # 2.6.2_Asymptotic_growth_of_the_Catalan_numbers
          o 2.7_Bivariate_and_multivariate_generating_functions
          o 2.8_Representation_by_continued_fractions_(Jacobi-type_J-fractions)
                # 2.8.1_Definitions
                # 2.8.2_Properties_of_the_hth_convergent_functions
                # 2.8.3_Examples
    * 3_Examples
          o 3.1_Ordinary_generating_function
          o 3.2_Exponential_generating_function
          o 3.3_Lambert_series
          o 3.4_Bell_series
          o 3.5_Dirichlet_series_generating_function
          o 3.6_Multivariate_generating_functions
    * 4_Applications
          o 4.1_Various_techniques:_Evaluating_sums_and_tackling_other_problems
            with_generating_functions
                # 4.1.1_Example_1:_A_formula_for_sums_of_harmonic_numbers
                # 4.1.2_Example_2:_Modified_binomial_coefficient_sums_and_the
                  binomial_transform
                # 4.1.3_Example_3:_Generating_functions_for_mutually_recursive
                  sequences
          o 4.2_Convolution_(Cauchy_products)
                # 4.2.1_Example:_The_generating_function_for_the_Catalan
                  numbers
                # 4.2.2_Example:_Spanning_trees_of_fans_and_convolutions_of
                  convolutions
          o 4.3_Implicit_generating_functions_and_the_Lagrange_inversion
            formula
          o 4.4_Introducing_a_free_parameter_(snake_oil_method)
          o 4.5_Generating_functions_prove_congruences
                # 4.5.1_The_Stirling_numbers_modulo_small_integers
                # 4.5.2_Congruences_for_the_partition_function
          o 4.6_Transformations_of_generating_functions
          o 4.7_Other_applications
    * 5_Other_generating_functions
          o 5.1_Examples
          o 5.2_Convolution_polynomials
          o 5.3_Tables_of_special_generating_functions
    * 6_History
    * 7_See_also
    * 8_Notes
    * 9_References
    * 10_External_links
***** Definitions[edit] *****
      A generating function is a device somewhat similar to a bag. Instead of
      carrying many little objects detachedly, which could be embarrassing, we
      put them all in a bag, and then we have only one object to carry, the
      bag.
      âGeorge_PÃ³lya, Mathematics_and_plausible_reasoning (1954)
      A generating function is a clothesline on which we hang up a sequence of
      numbers for display.
      âHerbert_Wilf, Generatingfunctionology (1994)
**** Ordinary generating function (OGF)[edit] ****
The ordinary generating function of a sequence an is
         G (  a  n   ; x ) =  &#x2211;  n = 0   &#x221E;    a  n    x  n   .
      {\displaystyle G(a_{n};x)=\sum _{n=0}^{\infty }a_{n}x^{n}.}  [G
      (a_n;x)=\sum_{n=0}^\infty a_nx^n.]
When the term generating function is used without qualification, it is usually
taken to mean an ordinary generating function.
If an is the probability_mass_function of a discrete_random_variable, then its
ordinary generating function is called a probability-generating_function.
The ordinary generating function can be generalized to arrays with multiple
indices. For example, the ordinary generating function of a two-dimensional
array am, n (where n and m are natural numbers) is
         G (  a  m , n   ; x , y ) =  &#x2211;  m , n = 0   &#x221E;    a  m ,
      n    x  m    y  n   .   {\displaystyle G(a_{m,n};x,y)=\sum _{m,n=0}^
      {\infty }a_{m,n}x^{m}y^{n}.}  [G(a_{m,n};x,y)=\sum_{m,n=0}^\infty a_
      {m,n}x^my^n.]
**** Exponential generating function (EGF)[edit] ****
The exponential generating function of a sequence an is
         EG &#x2061; (  a  n   ; x ) =  &#x2211;  n = 0   &#x221E;    a  n
      x  n    n !    .   {\displaystyle \operatorname {EG} (a_{n};x)=\sum _
      {n=0}^{\infty }a_{n}{\frac {x^{n}}{n!}}.}  [{\displaystyle \operatorname
      {EG} (a_{n};x)=\sum _{n=0}^{\infty }a_{n}{\frac {x^{n}}{n!}}.}]
Exponential generating functions are generally more convenient than ordinary
generating functions for combinatorial_enumeration problems that involve
labelled objects.[3]
**** Poisson generating function[edit] ****
The Poisson generating function of a sequence an is
         PG &#x2061; (  a  n   ; x ) =  &#x2211;  n = 0   &#x221E;    a  n    e
      &#x2212; x      x  n    n !    =  e  &#x2212; x    EG &#x2061; (  a  n
      ; x ) .   {\displaystyle \operatorname {PG} (a_{n};x)=\sum _{n=0}^{\infty
      }a_{n}e^{-x}{\frac {x^{n}}{n!}}=e^{-x}\,\operatorname {EG} (a_{n};x).}  [
      {\displaystyle \operatorname {PG} (a_{n};x)=\sum _{n=0}^{\infty }a_{n}e^
      {-x}{\frac {x^{n}}{n!}}=e^{-x}\,\operatorname {EG} (a_{n};x).}]
**** Lambert series[edit] ****
The Lambert_series of a sequence an is
         LG &#x2061; (  a  n   ; x ) =  &#x2211;  n = 1   &#x221E;    a  n
      x  n    1 &#x2212;  x  n      .   {\displaystyle \operatorname {LG} (a_
      {n};x)=\sum _{n=1}^{\infty }a_{n}{\frac {x^{n}}{1-x^{n}}}.}  [
      {\displaystyle \operatorname {LG} (a_{n};x)=\sum _{n=1}^{\infty }a_{n}
      {\frac {x^{n}}{1-x^{n}}}.}]
The Lambert series coefficients in the power series expansions      b  n   :=
[  x  n   ] LG &#x2061; (  a  n   ; x )   {\displaystyle b_{n}:=[x^
{n}]\operatorname {LG} (a_{n};x)}  [{\displaystyle b_{n}:=[x^{n}]\operatorname
{LG} (a_{n};x)}] for integers     n &#x2265; 1   {\displaystyle n\geq 1}
[n\geq 1] are related by the divisor_sum      b  n   =  &#x2211;  d  |  n    a
d     {\displaystyle b_{n}=\sum _{d|n}a_{d}}  [{\displaystyle b_{n}=\sum _
{d|n}a_{d}}]. The main article provides several more classical, or at least
well-known examples related to special arithmetic_functions in number_theory.
Note that in a Lambert series the index n starts at 1, not at 0, as the first
term would otherwise be undefined.
**** Bell series[edit] ****
The Bell_series of a sequence an is an expression in terms of both an
indeterminate x and a prime p and is given by[4]
          BG  p   &#x2061; (  a  n   ; x ) =  &#x2211;  n = 0   &#x221E;    a
      p  n      x  n   .   {\displaystyle \operatorname {BG} _{p}(a_{n};x)=\sum
      _{n=0}^{\infty }a_{p^{n}}x^{n}.}  [\operatorname{BG}_p(a_n;x)=\sum_
      {n=0}^\infty a_{p^n}x^n.]
**** Dirichlet series generating functions (DGFs)[edit] ****
Formal_Dirichlet_series are often classified as generating functions, although
they are not strictly formal power series. The Dirichlet series generating
function of a sequence an is[5]
         DG &#x2061; (  a  n   ; s ) =  &#x2211;  n = 1   &#x221E;      a  n
      n  s     .   {\displaystyle \operatorname {DG} (a_{n};s)=\sum _{n=1}^
      {\infty }{\frac {a_{n}}{n^{s}}}.}  [{\displaystyle \operatorname {DG} (a_
      {n};s)=\sum _{n=1}^{\infty }{\frac {a_{n}}{n^{s}}}.}]
The Dirichlet series generating function is especially useful when an is a
multiplicative_function, in which case it has an Euler_product expression[6] in
terms of the function's Bell series
         DG &#x2061; (  a  n   ; s ) =  &#x220F;  p    BG  p   &#x2061; (  a  n
      ;  p  &#x2212; s   )  .   {\displaystyle \operatorname {DG} (a_
      {n};s)=\prod _{p}\operatorname {BG} _{p}(a_{n};p^{-s})\,.}
      [\operatorname{DG}(a_n;s)=\prod_{p} \operatorname{BG}_p(a_n;p^{-s})\,.]
If an is a Dirichlet_character then its Dirichlet series generating function is
called a Dirichlet_L-series. We also have a relation between the pair of
coefficients in the Lambert_series expansions above and their DGFs. Namely, we
can prove that     [  x  n   ] LG &#x2061; (  a  n   ; x ) =  b  n
{\displaystyle [x^{n}]\operatorname {LG} (a_{n};x)=b_{n}}  [{\displaystyle [x^
{n}]\operatorname {LG} (a_{n};x)=b_{n}}] if and only if     DG &#x2061; (  a  n
; s ) &#x03B6; ( s ) = DG &#x2061; (  b  n   ; s )   {\displaystyle
\operatorname {DG} (a_{n};s)\zeta (s)=\operatorname {DG} (b_{n};s)}  [
{\displaystyle \operatorname {DG} (a_{n};s)\zeta (s)=\operatorname {DG} (b_
{n};s)}] where     &#x03B6; ( s )   {\displaystyle \zeta (s)}  [\zeta (s)] is
the Riemann_zeta_function.[7]
**** Polynomial sequence generating functions[edit] ****
The idea of generating functions can be extended to sequences of other objects.
Thus, for example, polynomial sequences of binomial_type are generated by
          e  x f ( t )   =  &#x2211;  n = 0   &#x221E;       p  n   ( x )   n !
      t  n     {\displaystyle e^{xf(t)}=\sum _{n=0}^{\infty }{\frac {p_{n}(x)}
      {n!}}t^{n}}  [e^{xf(t)}=\sum_{n=0}^\infty \frac{p_n(x)}{n!} t^n]
where pn(x) is a sequence of polynomials and f(t) is a function of a certain
form. Sheffer_sequences are generated in a similar way. See the main article
generalized_Appell_polynomials for more information.
***** Ordinary generating functions[edit] *****
**** Examples of generating functions for simple sequences[edit] ****
Polynomials are a special case of ordinary generating functions, corresponding
to finite sequences, or equivalently sequences that vanish after a certain
point. These are important in that many finite sequences can usefully be
interpreted as generating functions, such as the PoincarÃ©_polynomial and
others.
A key generating function is that of the constant sequence
1, 1, 1, 1, 1, 1, 1, 1, 1, ..., whose ordinary generating function is the
geometric_series
          &#x2211;  n = 0   &#x221E;    x  n   =   1  1 &#x2212; x    .
      {\displaystyle \sum _{n=0}^{\infty }x^{n}={\frac {1}{1-x}}.}  [
      {\displaystyle \sum _{n=0}^{\infty }x^{n}={\frac {1}{1-x}}.}]
The left-hand side is the Maclaurin_series expansion of the right-hand side.
Alternatively, the equality can be justified by multiplying the power series on
the left by 1 − x, and checking that the result is the constant power series 1
(in other words, that all coefficients except the one of x0 are equal to 0).
Moreover, there can be no other power series with this property. The left-hand
side therefore designates the multiplicative_inverse of 1 − x in the ring of
power series.
Expressions for the ordinary generating function of other sequences are easily
derived from this one. For instance, the substitution x â ax gives the
generating function for the geometric_sequence 1, a, a2, a3, ... for any
constant a:
          &#x2211;  n = 0   &#x221E;   ( a x  )  n   =   1  1 &#x2212; a x    .
      {\displaystyle \sum _{n=0}^{\infty }(ax)^{n}={\frac {1}{1-ax}}.}  [
      {\displaystyle \sum _{n=0}^{\infty }(ax)^{n}={\frac {1}{1-ax}}.}]
(The equality also follows directly from the fact that the left-hand side is
the Maclaurin series expansion of the right-hand side.) In particular,
          &#x2211;  n = 0   &#x221E;   ( &#x2212; 1  )  n    x  n   =   1  1 +
      x    .   {\displaystyle \sum _{n=0}^{\infty }(-1)^{n}x^{n}={\frac {1}
      {1+x}}.}  [{\displaystyle \sum _{n=0}^{\infty }(-1)^{n}x^{n}={\frac {1}
      {1+x}}.}]
One can also introduce regular "gaps" in the sequence by replacing x by some
power of x, so for instance for the sequence 1, 0, 1, 0, 1, 0, 1, 0, .... one
gets the generating function
          &#x2211;  n = 0   &#x221E;    x  2 n   =   1  1 &#x2212;  x  2      .
      {\displaystyle \sum _{n=0}^{\infty }x^{2n}={\frac {1}{1-x^{2}}}.}  [
      {\displaystyle \sum _{n=0}^{\infty }x^{2n}={\frac {1}{1-x^{2}}}.}]
By squaring the initial generating function, or by finding the derivative of
both sides with respect to x and making a change of running variable
n â n + 1, one sees that the coefficients form the sequence
1, 2, 3, 4, 5, ..., so one has
          &#x2211;  n = 0   &#x221E;   ( n + 1 )  x  n   =   1  ( 1 &#x2212; x
      )  2      ,   {\displaystyle \sum _{n=0}^{\infty }(n+1)x^{n}={\frac {1}{
      (1-x)^{2}}},}  [{\displaystyle \sum _{n=0}^{\infty }(n+1)x^{n}={\frac {1}
      {(1-x)^{2}}},}]
and the third power has as coefficients the triangular_numbers
1, 3, 6, 10, 15, 21, ... whose term n is the binomial_coefficient
(    n + 2  2   )       {\displaystyle {\tbinom {n+2}{2}}}  [\tbinom{n+2}2], so
that
          &#x2211;  n = 0   &#x221E;      (    n + 2  2   )     x  n   =   1
      ( 1 &#x2212; x  )  3      .   {\displaystyle \sum _{n=0}^{\infty }{\binom
      {n+2}{2}}x^{n}={\frac {1}{(1-x)^{3}}}.}  [{\displaystyle \sum _{n=0}^
      {\infty }{\binom {n+2}{2}}x^{n}={\frac {1}{(1-x)^{3}}}.}]
More generally, for any non-negative integer k and non-zero real value a, it is
true that
          &#x2211;  n = 0   &#x221E;    a  n      (    n + k  k   )     x  n
      =   1  ( 1 &#x2212; a x  )  k + 1       .   {\displaystyle \sum _{n=0}^
      {\infty }a^{n}{\binom {n+k}{k}}x^{n}={\frac {1}{(1-ax)^{k+1}}}\,.}  [
      {\displaystyle \sum _{n=0}^{\infty }a^{n}{\binom {n+k}{k}}x^{n}={\frac
      {1}{(1-ax)^{k+1}}}\,.}]
Note that, since
         2    (    n + 2  2   )    &#x2212; 3    (    n + 1  1   )    +
      (   n 0   )    = 2    ( n + 1 ) ( n + 2 )  2   &#x2212; 3 ( n + 1 ) + 1 =
      n  2   ,   {\displaystyle 2{\binom {n+2}{2}}-3{\binom {n+1}{1}}+{\binom
      {n}{0}}=2{\frac {(n+1)(n+2)}{2}}-3(n+1)+1=n^{2},}  [{\displaystyle 2
      {\binom {n+2}{2}}-3{\binom {n+1}{1}}+{\binom {n}{0}}=2{\frac {(n+1)(n+2)}
      {2}}-3(n+1)+1=n^{2},}]
one can find the ordinary generating function for the sequence
0, 1, 4, 9, 16, ... of square_numbers by linear combination of binomial-
coefficient generating sequences:
         G (  n  2   ; x ) =  &#x2211;  n = 0   &#x221E;    n  2    x  n   =
      2  ( 1 &#x2212; x  )  3      &#x2212;   3  ( 1 &#x2212; x  )  2      +
      1  1 &#x2212; x    =    x ( x + 1 )   ( 1 &#x2212; x  )  3      .
      {\displaystyle G(n^{2};x)=\sum _{n=0}^{\infty }n^{2}x^{n}={\frac {2}{(1-
      x)^{3}}}-{\frac {3}{(1-x)^{2}}}+{\frac {1}{1-x}}={\frac {x(x+1)}{(1-x)^
      {3}}}.}  [{\displaystyle G(n^{2};x)=\sum _{n=0}^{\infty }n^{2}x^{n}=
      {\frac {2}{(1-x)^{3}}}-{\frac {3}{(1-x)^{2}}}+{\frac {1}{1-x}}={\frac {x
      (x+1)}{(1-x)^{3}}}.}]
We may also expand alternately to generate this same sequence of squares as a
sum of derivatives of the geometric_series in the following form:
             G (  n  2   ; x )    =  &#x2211;  n = 0   &#x221E;    n  2    x  n
      =  &#x2211;  n = 0   &#x221E;   n ( n &#x2212; 1 )  x  n   +  &#x2211;  n
      = 0   &#x221E;   n  x  n         =  x  2    D  2    [   1  1 &#x2212; x
      ]  + x D  [   1  1 &#x2212; x    ]        =    2  x  2     ( 1 &#x2212; x
      )  3      +   x  ( 1 &#x2212; x  )  2      =    x ( x + 1 )   ( 1
      &#x2212; x  )  3      .       {\displaystyle {\begin{aligned}G(n^
      {2};x)&=\sum _{n=0}^{\infty }n^{2}x^{n}=\sum _{n=0}^{\infty }n(n-1)x^
      {n}+\sum _{n=0}^{\infty }nx^{n}\\&=x^{2}D^{2}\left[{\frac {1}{1-
      x}}\right]+xD\left[{\frac {1}{1-x}}\right]\\&={\frac {2x^{2}}{(1-x)^
      {3}}}+{\frac {x}{(1-x)^{2}}}={\frac {x(x+1)}{(1-x)^{3}}}.\end{aligned}}}
      [{\displaystyle {\begin{aligned}G(n^{2};x)&=\sum _{n=0}^{\infty }n^{2}x^
      {n}=\sum _{n=0}^{\infty }n(n-1)x^{n}+\sum _{n=0}^{\infty }nx^{n}\\&=x^
      {2}D^{2}\left[{\frac {1}{1-x}}\right]+xD\left[{\frac {1}{1-x}}\right]\\&=
      {\frac {2x^{2}}{(1-x)^{3}}}+{\frac {x}{(1-x)^{2}}}={\frac {x(x+1)}{(1-x)^
      {3}}}.\end{aligned}}}]
By induction, we can similarly show for positive integers     m &#x2265; 1
{\displaystyle m\geq 1}  [{\displaystyle m\geq 1}] that [8][9]
          n  m   =  &#x2211;  j = 0   m    {     m     j     }     n !   ( n
      &#x2212; j ) !    ,   {\displaystyle n^{m}=\sum _{j=0}^{m}\left\{{\begin
      {matrix}m\\j\end{matrix}}\right\}{\frac {n!}{(n-j)!}},}  [{\displaystyle
      n^{m}=\sum _{j=0}^{m}\left\{{\begin{matrix}m\\j\end{matrix}}\right\}
      {\frac {n!}{(n-j)!}},}]
where      {     n     k     }    {\displaystyle \left\{{\begin{matrix}n\\k\end
{matrix}}\right\}}  [\left\{{\begin{matrix}n\\k\end{matrix}}\right\}] denote
the Stirling_numbers_of_the_second_kind and where the generating function
&#x2211;  n &#x2265; 0   n !  /  ( n &#x2212; j ) !   z  n   = j ! &#x22C5;  z
j    /  ( 1 &#x2212; z  )  j + 1     {\displaystyle \sum _{n\geq 0}n!/(n-
j)!\,z^{n}=j!\cdot z^{j}/(1-z)^{j+1}}  [{\displaystyle \sum _{n\geq 0}n!/(n-
j)!\,z^{n}=j!\cdot z^{j}/(1-z)^{j+1}}], so that we can form the analogous
generating functions over the integral     m   {\displaystyle m}  [m]-th powers
generalizing the result in the square case above. In particular, since we can
write        z  k    ( 1 &#x2212; z  )  k + 1      =  &#x2211;  i = 0   k
(   k i   )       ( &#x2212; 1  )  k &#x2212; i     ( 1 &#x2212; z  )  i + 1
{\displaystyle {\frac {z^{k}}{(1-z)^{k+1}}}=\sum _{i=0}^{k}{\binom {k}{i}}
{\frac {(-1)^{k-i}}{(1-z)^{i+1}}}}  [{\displaystyle {\frac {z^{k}}{(1-z)^
{k+1}}}=\sum _{i=0}^{k}{\binom {k}{i}}{\frac {(-1)^{k-i}}{(1-z)^{i+1}}}}], we
can apply a well-known finite sum identity involving the Stirling_numbers to
obtain that[10]
          &#x2211;  n &#x2265; 0    n  m    z  n   =  &#x2211;  j = 0   m
      {     m + 1     j + 1     }     ( &#x2212; 1  )  m &#x2212; j   j !   ( 1
      &#x2212; z  )  j + 1      .   {\displaystyle \sum _{n\geq 0}n^{m}z^
      {n}=\sum _{j=0}^{m}\left\{{\begin{matrix}m+1\\j+1\end{matrix}}\right\}
      {\frac {(-1)^{m-j}j!}{(1-z)^{j+1}}}.}  [{\displaystyle \sum _{n\geq 0}n^
      {m}z^{n}=\sum _{j=0}^{m}\left\{{\begin{matrix}m+1\\j+1\end
      {matrix}}\right\}{\frac {(-1)^{m-j}j!}{(1-z)^{j+1}}}.}]
**** Rational functions[edit] ****
Main article: Linear_recursive_sequence
The ordinary generating function of a sequence can be expressed as a rational
function (the ratio of two finite-degree polynomials) if and only if the
sequence is a linear_recursive_sequence with constant coefficients; this
generalizes the examples above. Conversely, every sequence generated by a
fraction of polynomials satisfies a linear recurrence with constant
coefficients; these coefficients are identical to the coefficients of the
fraction denominator polynomial (so they can be directly read off). This
observation shows it is easy to solve for generating functions of sequences
defined by a linear finite_difference_equation with constant coefficients, and
then hence, for explicit closed-form formulas for the coefficients of these
generating functions. The prototypical example here is to derive Binet's
formula for the Fibonacci_numbers via generating function techniques.
We also notice that the class of rational generating functions precisely
corresponds to the generating functions that enumerate quasi-polynomial
sequences of the form [11]
          f  n   =  p  1   ( n )  &#x03C1;  1   n   + &#x22EF; +  p  &#x2113;
      ( n )  &#x03C1;  &#x2113;   n   ,   {\displaystyle f_{n}=p_{1}(n)\rho _
      {1}^{n}+\cdots +p_{\ell }(n)\rho _{\ell }^{n},}  [{\displaystyle f_{n}=p_
      {1}(n)\rho _{1}^{n}+\cdots +p_{\ell }(n)\rho _{\ell }^{n},}]
where the reciprocal roots,      &#x03C1;  i   &#x2208;  C    {\displaystyle
\rho _{i}\in \mathbb {C} }  [{\displaystyle \rho _{i}\in \mathbb {C} }], are
fixed scalars and where      p  i   ( n )   {\displaystyle p_{i}(n)}  [
{\displaystyle p_{i}(n)}] is a polynomial in     n   {\displaystyle n}  [n] for
all     1 &#x2264; i &#x2264; &#x2113;   {\displaystyle 1\leq i\leq \ell }
[1\leq i\leq \ell ].
In general, Hadamard_products of rational functions produce rational generating
functions. Similarly, if     F ( s , t ) :=  &#x2211;  m , n &#x2265; 0   f ( m
, n )  w  m    z  n     {\displaystyle F(s,t):=\sum _{m,n\geq 0}f(m,n)w^{m}z^
{n}}  [{\displaystyle F(s,t):=\sum _{m,n\geq 0}f(m,n)w^{m}z^{n}}] is a
bivariate rational generating function, then its corresponding diagonal
generating function,     diag &#x2061; ( F ) :=  &#x2211;  n &#x2265; 0   f ( n
, n )  z  n     {\displaystyle \operatorname {diag} (F):=\sum _{n\geq 0}f
(n,n)z^{n}}  [{\displaystyle \operatorname {diag} (F):=\sum _{n\geq 0}f(n,n)z^
{n}}], is algebraic. For example, if we let [12]
         F ( s , t ) :=  &#x2211;  i , j &#x2265; 0      (    i + j  i   )
      s  i    t  j   =   1  1 &#x2212; s &#x2212; t    ,   {\displaystyle F
      (s,t):=\sum _{i,j\geq 0}{\binom {i+j}{i}}s^{i}t^{j}={\frac {1}{1-s-t}},}
      [{\displaystyle F(s,t):=\sum _{i,j\geq 0}{\binom {i+j}{i}}s^{i}t^{j}=
      {\frac {1}{1-s-t}},}]
then this generating function's diagonal coefficient generating function is
given by the well-known OGF formula
         diag &#x2061; ( F ) =  &#x2211;  n &#x2265; 0      (    2 n  n   )
      z  n   =   1  1 &#x2212; 4 z    .   {\displaystyle \operatorname {diag}
      (F)=\sum _{n\geq 0}{\binom {2n}{n}}z^{n}={\frac {1}{\sqrt {1-4z}}}.}  [
      {\displaystyle \operatorname {diag} (F)=\sum _{n\geq 0}{\binom {2n}{n}}z^
      {n}={\frac {1}{\sqrt {1-4z}}}.}]
This result is computed in many ways, including Cauchy's_integral_formula or
contour_integration, taking complex residues, or by direct manipulations of
formal_power_series in two variables.
**** Operations on generating functions[edit] ****
*** Multiplication yields convolution[edit] ***
Main article: Cauchy_product
Multiplication of ordinary generating functions yields a discrete convolution
(the Cauchy_product) of the sequences. For example, the sequence of cumulative
sums (compare to the slightly more general EulerâMaclaurin_formula)
         (  a  0   ,  a  0   +  a  1   ,  a  0   +  a  1   +  a  2   , &#x2026;
      )   {\displaystyle (a_{0},a_{0}+a_{1},a_{0}+a_{1}+a_{2},\ldots )}  [
      {\displaystyle (a_{0},a_{0}+a_{1},a_{0}+a_{1}+a_{2},\ldots )}]
of a sequence with ordinary generating function G(an; x) has the generating
function
         G (  a  n   ; x ) &#x22C5;   1  1 &#x2212; x      {\displaystyle G(a_
      {n};x)\cdot {\frac {1}{1-x}}}  [G(a_n; x) \cdot \frac{1}{1-x}]
because 1/(1 â x) is the ordinary generating function for the sequence (1, 1,
...). See also the section_on_convolutions in the applications section of this
article below for further examples of problem solving with convolutions of
generating functions and interpretations.
*** Shifting sequence indices[edit] ***
For integers     m &#x2265; 1   {\displaystyle m\geq 1}  [{\displaystyle m\geq
1}], we have the following two analogous identities for the modified generating
functions enumerating the shifted sequence variants of     &#x27E8;  g  n
&#x2212; m   &#x27E9;   {\displaystyle \langle g_{n-m}\rangle }  [
{\displaystyle \langle g_{n-m}\rangle }] and     &#x27E8;  g  n + m   &#x27E9;
{\displaystyle \langle g_{n+m}\rangle }  [{\displaystyle \langle g_{n+m}\rangle
}], respectively:
              z  m   G ( z )    =  &#x2211;  n &#x2265; m    g  n &#x2212; m
      z  n          G ( z ) &#x2212;  g  0   &#x2212;  g  1   z &#x2212;
      &#x22EF; &#x2212;  g  m &#x2212; 1    z  m &#x2212; 1     z  m        =
      &#x2211;  n &#x2265; 0    g  n + m    z  n   .       {\displaystyle
      {\begin{aligned}z^{m}G(z)&=\sum _{n\geq m}g_{n-m}z^{n}\\{\frac {G(z)-g_
      {0}-g_{1}z-\cdots -g_{m-1}z^{m-1}}{z^{m}}}&=\sum _{n\geq 0}g_{n+m}z^
      {n}.\end{aligned}}}  [{\displaystyle {\begin{aligned}z^{m}G(z)&=\sum _
      {n\geq m}g_{n-m}z^{n}\\{\frac {G(z)-g_{0}-g_{1}z-\cdots -g_{m-1}z^{m-1}}
      {z^{m}}}&=\sum _{n\geq 0}g_{n+m}z^{n}.\end{aligned}}}]
*** Differentiation and integration of generating functions[edit] ***
We have the following respective power series expansions for the first
derivative of a generating function and its integral:
              G  &#x2032;   ( z )    =  &#x2211;  n &#x2265; 0   ( n + 1 )  g
      n + 1    z  n       z &#x22C5;  G  &#x2032;   ( z )    =  &#x2211;  n
      &#x2265; 0   n  g  n    z  n        &#x222B;  0   z   G ( t )  d t    =
      &#x2211;  n &#x2265; 1      g  n &#x2212; 1   n    z  n   .
      {\displaystyle {\begin{aligned}G^{\prime }(z)&=\sum _{n\geq 0}(n+1)g_
      {n+1}z^{n}\\z\cdot G^{\prime }(z)&=\sum _{n\geq 0}ng_{n}z^{n}\\\int _{0}^
      {z}G(t)\,dt&=\sum _{n\geq 1}{\frac {g_{n-1}}{n}}z^{n}.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}G^{\prime }(z)&=\sum _{n\geq 0}(n+1)g_
      {n+1}z^{n}\\z\cdot G^{\prime }(z)&=\sum _{n\geq 0}ng_{n}z^{n}\\\int _{0}^
      {z}G(t)\,dt&=\sum _{n\geq 1}{\frac {g_{n-1}}{n}}z^{n}.\end{aligned}}}]
The differentiationâmultiplication operation of the second identity can be
repeated     k   {\displaystyle k}  [k] times to multiply the sequence by
n  k     {\displaystyle n^{k}}  [n^{k}], but that requires alternating between
differentiation and multiplication. If instead doing     k   {\displaystyle k}
[k] differentiations in sequence, the effect is to multiply by the     k
{\displaystyle k}  [k]th falling_factorial:
          z  k    G  ( k )   ( z ) =  &#x2211;  n &#x2265; 0    n   k &#x005F;
      g  n    z  n   =  &#x2211;  n &#x2265; 0   n ( n &#x2212; 1 ) &#x22EF;
      ( n &#x2212; k + 1 )  g  n    z  n    &#xA0;for all&#xA0;  k &#x2208;  N
      .   {\displaystyle z^{k}G^{(k)}(z)=\sum _{n\geq 0}n^{\underline {k}}g_
      {n}z^{n}=\sum _{n\geq 0}n(n-1)\dotsb (n-k+1)g_{n}z^{n}{\text{ for all
      }}k\in \mathbb {N} .}  [{\displaystyle z^{k}G^{(k)}(z)=\sum _{n\geq 0}n^
      {\underline {k}}g_{n}z^{n}=\sum _{n\geq 0}n(n-1)\dotsb (n-k+1)g_{n}z^{n}
      {\text{ for all }}k\in \mathbb {N} .}]
Using the Stirling_numbers_of_the_second_kind, that can be turned into another
formula for multiplying by      n  k     {\displaystyle n^{k}}  [n^{k}] as
follows (see the main article on generating_function_transformations):
          &#x2211;  j = 0   k    {     k     j     }   z  j    F  ( j )   ( z )
      =  &#x2211;  n &#x2265; 0    n  k    f  n    z  n    &#xA0;for all&#xA0;
      k &#x2208;  N  .   {\displaystyle \sum _{j=0}^{k}\left\{{\begin
      {matrix}k\\j\end{matrix}}\right\}z^{j}F^{(j)}(z)=\sum _{n\geq 0}n^{k}f_
      {n}z^{n}{\text{ for all }}k\in \mathbb {N} .}  [{\displaystyle \sum _
      {j=0}^{k}\left\{{\begin{matrix}k\\j\end{matrix}}\right\}z^{j}F^{(j)}
      (z)=\sum _{n\geq 0}n^{k}f_{n}z^{n}{\text{ for all }}k\in \mathbb {N} .}]
A negative-order reversal of this sequence powers formula corresponding to the
operation of repeated integration is defined by the zeta_series_transformation
and its generalizations defined as a derivative-based transformation_of
generating_functions, or alternately termwise by an performing an integral
transformation on the sequence generating function. Related operations of
performing fractional_integration on a sequence generating function are
discussed here.
*** Enumerating arithmetic progressions of sequences[edit] ***
In this section we give formulas for generating functions enumerating the
sequence     {  f  a n + b   }   {\displaystyle \{f_{an+b}\}}  [{\displaystyle
\{f_{an+b}\}}] given an ordinary generating function     F ( z )
{\displaystyle F(z)}  [{\displaystyle F(z)}] where     a , b &#x2208;  N
{\displaystyle a,b\in \mathbb {N} }  [{\displaystyle a,b\in \mathbb {N} }],
a &#x2265; 2   {\displaystyle a\geq 2}  [{\displaystyle a\geq 2}], and     0
&#x2264; b < a   {\displaystyle 0\leq b<a}  [{\displaystyle 0\leq b<a}] (see
the main_article_on_transformations). For     a = 2   {\displaystyle a=2}  [
{\displaystyle a=2}], this is simply the familiar decomposition of a function
into even_and_odd_parts (i.e., even and odd powers):
          &#x2211;  n &#x2265; 0    f  2 n    z  2 n   =   1 2    (  F ( z ) +
      F ( &#x2212; z )  )    {\displaystyle \sum _{n\geq 0}f_{2n}z^{2n}={\frac
      {1}{2}}\left(F(z)+F(-z)\right)}  [{\displaystyle \sum _{n\geq 0}f_{2n}z^
      {2n}={\frac {1}{2}}\left(F(z)+F(-z)\right)}]
          &#x2211;  n &#x2265; 0    f  2 n + 1    z  2 n + 1   =   1 2    (  F
      ( z ) &#x2212; F ( &#x2212; z )  )  .   {\displaystyle \sum _{n\geq 0}f_
      {2n+1}z^{2n+1}={\frac {1}{2}}\left(F(z)-F(-z)\right).}  [{\displaystyle
      \sum _{n\geq 0}f_{2n+1}z^{2n+1}={\frac {1}{2}}\left(F(z)-F(-z)\right).}]
More generally, suppose that     a &#x2265; 3   {\displaystyle a\geq 3}  [
{\displaystyle a\geq 3}] and that      &#x03C9;  a   = exp &#x2061;  (  2
&#x03C0; &#x0131;  /  a  )    {\displaystyle \omega _{a}=\exp \left(2\pi \imath
/a\right)}  [{\displaystyle \omega _{a}=\exp \left(2\pi \imath /a\right)}]
denotes the     a   {\displaystyle a}  [a]th primitive_root_of_unity. Then, as
an application of the discrete_Fourier_transform, we have the formula[13]
          &#x2211;  n &#x2265; 0    f  a n + b    z  a n + b   =   1 a
      &#x2211;  m = 0   a &#x2212; 1    &#x03C9;  a   &#x2212; m b   F
      (   &#x03C9;  a   m   z  )  .   {\displaystyle \sum _{n\geq 0}f_{an+b}z^
      {an+b}={\frac {1}{a}}\sum _{m=0}^{a-1}\omega _{a}^{-mb}F\left(\omega _
      {a}^{m}z\right).}  [{\displaystyle \sum _{n\geq 0}f_{an+b}z^{an+b}={\frac
      {1}{a}}\sum _{m=0}^{a-1}\omega _{a}^{-mb}F\left(\omega _{a}^
      {m}z\right).}]
For integers     m &#x2265; 1   {\displaystyle m\geq 1}  [{\displaystyle m\geq
1}], another useful formula providing somewhat reversed floored arithmetic
progressions â effectively repeating each coefficient     m   {\displaystyle
m}  [m] times â are generated by the identity[14]
          &#x2211;  n &#x2265; 0    f  &#x230A;   n m   &#x230B;    z  n   =
      1 &#x2212;  z  m     1 &#x2212; z    F (  z  m   ) =  (  1 + z + &#x22EF;
      +  z  m &#x2212; 2   +  z  m &#x2212; 1    )  F (  z  m   ) .
      {\displaystyle \sum _{n\geq 0}f_{\lfloor {\frac {n}{m}}\rfloor }z^{n}=
      {\frac {1-z^{m}}{1-z}}F(z^{m})=\left(1+z+\cdots +z^{m-2}+z^{m-1}\right)F
      (z^{m}).}  [{\displaystyle \sum _{n\geq 0}f_{\lfloor {\frac {n}
      {m}}\rfloor }z^{n}={\frac {1-z^{m}}{1-z}}F(z^{m})=\left(1+z+\cdots +z^{m-
      2}+z^{m-1}\right)F(z^{m}).}]
**** P-recursive sequences and holonomic generating functions[edit] ****
*** Definitions[edit] ***
A formal power series (or function)     F ( z )   {\displaystyle F(z)}  [
{\displaystyle F(z)}] is said to be holonomic if it satisfies a linear
differential equation of the form [15]
          c  0   ( z )  F  ( r )   ( z ) +  c  1   ( z )  F  ( r &#x2212; 1 )
      ( z ) + &#x22EF; +  c  r   ( z ) F ( z ) = 0 ,   {\displaystyle c_{0}
      (z)F^{(r)}(z)+c_{1}(z)F^{(r-1)}(z)+\cdots +c_{r}(z)F(z)=0,}  [
      {\displaystyle c_{0}(z)F^{(r)}(z)+c_{1}(z)F^{(r-1)}(z)+\cdots +c_{r}(z)F
      (z)=0,}]
where the coefficients      c  i   ( z )   {\displaystyle c_{i}(z)}  [
{\displaystyle c_{i}(z)}] are in the field of rational functions,      C  ( z )
{\displaystyle \mathbb {C} (z)}  [{\displaystyle \mathbb {C} (z)}].
Equivalently,     F ( z )   {\displaystyle F(z)}  [{\displaystyle F(z)}] is
holonomic if the vector space over      C  ( z )   {\displaystyle \mathbb {C}
(z)}  [{\displaystyle \mathbb {C} (z)}] spanned by the set of all of its
derivatives is finite dimensional.
Since we can clear denominators if need be in the previous equation, we may
assume that the functions,      c  i   ( z )   {\displaystyle c_{i}(z)}  [
{\displaystyle c_{i}(z)}] are polynomials in     z   {\displaystyle z}  [z].
Thus we can see an equivalent condition that a generating function is holonomic
if its coefficients satisfy a P-recurrence of the form
             c &#x005E;     s   ( n )  f  n + s   +     c &#x005E;     s
      &#x2212; 1   ( n )  f  n + s &#x2212; 1   + &#x22EF; +     c &#x005E;
      0   ( n )  f  n   = 0 ,   {\displaystyle {\widehat {c}}_{s}(n)f_{n+s}+
      {\widehat {c}}_{s-1}(n)f_{n+s-1}+\cdots +{\widehat {c}}_{0}(n)f_{n}=0,}
      [{\displaystyle {\widehat {c}}_{s}(n)f_{n+s}+{\widehat {c}}_{s-1}(n)f_
      {n+s-1}+\cdots +{\widehat {c}}_{0}(n)f_{n}=0,}]
for all large enough     n &#x2265;  n  0     {\displaystyle n\geq n_{0}}  [n
\geq n_0] and where the         c &#x005E;     i   ( n )   {\displaystyle
{\widehat {c}}_{i}(n)}  [{\displaystyle {\widehat {c}}_{i}(n)}] are fixed
finite-degree polynomials in     n   {\displaystyle n}  [n]. In other words,
the properties that a sequence be P-recursive and have a holonomic generating
function are equivalent. Holonomic functions are closed under the Hadamard
product operation     &#x2299;   {\displaystyle \odot }  [\odot ] on generating
functions.
*** Examples[edit] ***
The functions      e  z     {\displaystyle e^{z}}  [e^{z}],     log &#x2061;
( z )   {\displaystyle \log(z)}  [\log(z)],     cos &#x2061; ( z )
{\displaystyle \cos(z)}  [{\displaystyle \cos(z)}],     arcsin &#x2061; ( z )
{\displaystyle \arcsin(z)}  [\arcsin(z)],       1 + z     {\displaystyle {\sqrt
{1+z}}}  [{\displaystyle {\sqrt {1+z}}}], the dilogarithm function      Li  2
&#x2061; ( z )   {\displaystyle \operatorname {Li} _{2}(z)}  [{\displaystyle
\operatorname {Li} _{2}(z)}], the generalized_hypergeometric_functions        p
F  q   ( . . . ; . . . ; z )   {\displaystyle _{p}F_{q}(...;...;z)}  [
{\displaystyle _{p}F_{q}(...;...;z)}] and the functions defined by the power
series      &#x2211;  n &#x2265; 0    z  n    /  ( n !  )  2     {\displaystyle
\sum _{n\geq 0}z^{n}/(n!)^{2}}  [{\displaystyle \sum _{n\geq 0}z^{n}/(n!)^{2}}]
and the non-convergent      &#x2211;  n &#x2265; 0   n ! &#x22C5;  z  n
{\displaystyle \sum _{n\geq 0}n!\cdot z^{n}}  [{\displaystyle \sum _{n\geq
0}n!\cdot z^{n}}] are all holonomic. Examples of P-recursive sequences with
holonomic generating functions include      f  n   :=   1  n + 1       (    2 n
n   )      {\displaystyle f_{n}:={\frac {1}{n+1}}{\binom {2n}{n}}}  [
{\displaystyle f_{n}:={\frac {1}{n+1}}{\binom {2n}{n}}}] and      f  n   :=  2
n    /  (  n  2   + 1 )   {\displaystyle f_{n}:=2^{n}/(n^{2}+1)}  [
{\displaystyle f_{n}:=2^{n}/(n^{2}+1)}], where sequences such as       n
{\displaystyle {\sqrt {n}}}  [{\sqrt {n}}] and     log &#x2061; ( n )
{\displaystyle \log(n)}  [\log(n)] are not P-recursive due to the nature of
singularities in their corresponding generating functions. Similarly, functions
with infinitely-many singularities such as     tan &#x2061; ( z )
{\displaystyle \tan(z)}  [\tan(z)],     sec &#x2061; ( z )   {\displaystyle
\sec(z)}  [{\displaystyle \sec(z)}], and     &#x0393; ( z )   {\displaystyle
\Gamma (z)}  [\Gamma (z)] are not holonomic functions.
*** Software for working with P-recursive sequences and holonomic generating
functions[edit] ***
Tools for processing and working with P-recursive sequences in Mathematica
include the software packages provided for non-commercial use on the RISC
Combinatorics_Group_algorithmic_combinatorics_software site. Despite being
mostly closed-source, particularly powerful tools in this software suite are
provided by the Guess package for guessing P-recurrences for arbitrary input
sequences (useful for experimental_mathematics and exploration) and the Sigma
package which is able to find P-recurrences for many sums and solve for closed-
form solutions to P-recurrences involving generalized harmonic_numbers.[16]
Other packages listed on this particular RISC site are targeted at working with
holonomic generating functions specifically. (Depending on how in depth this
article gets on the topic, there are many, many other examples of useful
software tools that can be listed here or on this page in another section.)
**** Relation to discrete-time Fourier transform[edit] ****
Main article: Discrete-time_Fourier_transform
When the series converges_absolutely,
         G  (   a  n   ;  e  &#x2212; i &#x03C9;    )  =  &#x2211;  n = 0
      &#x221E;    a  n    e  &#x2212; i &#x03C9; n     {\displaystyle G\left(a_
      {n};e^{-i\omega }\right)=\sum _{n=0}^{\infty }a_{n}e^{-i\omega n}}  [G
      \left ( a_n; e^{-i \omega} \right) = \sum_{n=0}^\infty a_n e^{-i \omega
      n}]
is the discrete-time Fourier transform of the sequence a0, a1, ....
**** Asymptotic growth of a sequence[edit] ****
In calculus, often the growth rate of the coefficients of a power series can be
used to deduce a radius_of_convergence for the power series. The reverse can
also hold; often the radius of convergence for a generating function can be
used to deduce the asymptotic_growth of the underlying sequence.
For instance, if an ordinary generating function G(an; x) that has a finite
radius of convergence of r can be written as
         G (  a  n   ; x ) =    A ( x ) + B ( x )   (  1 &#x2212;   x r    )
      &#x2212; &#x03B2;     x  &#x03B1;       {\displaystyle G(a_{n};x)={\frac
      {A(x)+B(x)\left(1-{\frac {x}{r}}\right)^{-\beta }}{x^{\alpha }}}}  [G
      (a_n; x) = \frac{A(x) + B(x) \left (1- \frac{x}{r} \right )^{-\beta}}{x^
      {\alpha}}]
where each of A(x) and B(x) is a function that is analytic to a radius of
convergence greater than r (or is entire), and where B(r) â  0 then
          a  n   &#x223C;    B ( r )    r  &#x03B1;   &#x0393; ( &#x03B2; )
      n  &#x03B2; &#x2212; 1   ( 1  /  r  )  n   &#x223C;    B ( r )   r
      &#x03B1;        (    n + &#x03B2; &#x2212; 1  n   )    ( 1  /  r  )  n
      =    B ( r )   r  &#x03B1;      (       (   &#x03B2; n   )       )  ( 1
      /  r  )  n    ,   {\displaystyle a_{n}\sim {\frac {B(r)}{r^{\alpha
      }\Gamma (\beta )}}\,n^{\beta -1}(1/r)^{n}\sim {\frac {B(r)}{r^{\alpha }}}
      {\binom {n+\beta -1}{n}}(1/r)^{n}={\frac {B(r)}{r^{\alpha }}}\left(\!\!
      {\binom {\beta }{n}}\!\!\right)(1/r)^{n}\,,}  [{\displaystyle a_{n}\sim
      {\frac {B(r)}{r^{\alpha }\Gamma (\beta )}}\,n^{\beta -1}(1/r)^{n}\sim
      {\frac {B(r)}{r^{\alpha }}}{\binom {n+\beta -1}{n}}(1/r)^{n}={\frac {B
      (r)}{r^{\alpha }}}\left(\!\!{\binom {\beta }{n}}\!\!\right)(1/r)^{n}\,,}]
using the Gamma_function, a binomial_coefficient, or a multiset_coefficient.
Often this approach can be iterated to generate several terms in an asymptotic
series for an. In particular,
         G  (   a  n   &#x2212;    B ( r )   r  &#x03B1;        (    n +
      &#x03B2; &#x2212; 1  n   )    ( 1  /  r  )  n   ; x  )  = G (  a  n   ; x
      ) &#x2212;    B ( r )   r  &#x03B1;       (  1 &#x2212;   x r    )
      &#x2212; &#x03B2;    .   {\displaystyle G\left(a_{n}-{\frac {B(r)}{r^
      {\alpha }}}{\binom {n+\beta -1}{n}}(1/r)^{n};x\right)=G(a_{n};x)-{\frac
      {B(r)}{r^{\alpha }}}\left(1-{\frac {x}{r}}\right)^{-\beta }\,.}  [
      {\displaystyle G\left(a_{n}-{\frac {B(r)}{r^{\alpha }}}{\binom {n+\beta -
      1}{n}}(1/r)^{n};x\right)=G(a_{n};x)-{\frac {B(r)}{r^{\alpha }}}\left(1-
      {\frac {x}{r}}\right)^{-\beta }\,.}]
The asymptotic growth of the coefficients of this generating function can then
be sought via the finding of A, B, Î±, Î², and r to describe the generating
function, as above.
Similar asymptotic analysis is possible for exponential generating functions.
With an exponential generating function, it is an/n! that grows according to
these asymptotic formulae.
*** Asymptotic growth of the sequence of squares[edit] ***
As derived above, the ordinary generating function for the sequence of squares
is
            x ( x + 1 )   ( 1 &#x2212; x  )  3      .   {\displaystyle {\frac
      {x(x+1)}{(1-x)^{3}}}.}  [\frac{x(x+1)}{(1-x)^3}.]
With r = 1, Î± = 0, Î² = 3, A(x) = 0, and B(x) = x(x+1), we can verify that the
squares grow as expected, like the squares:
          a  n   &#x223C;    B ( r )    r  &#x03B1;   &#x0393; ( &#x03B2; )
      n  &#x03B2; &#x2212; 1     (   1 r   )   n   =    1 ( 1 + 1 )    1  0
      &#x0393; ( 3 )      n  3 &#x2212; 1   ( 1  /  1  )  n   =  n  2   .
      {\displaystyle a_{n}\sim {\frac {B(r)}{r^{\alpha }\Gamma (\beta )}}\,n^
      {\beta -1}\left({\frac {1}{r}}\right)^{n}={\frac {1(1+1)}{1^{0}\,\Gamma
      (3)}}\,n^{3-1}(1/1)^{n}=n^{2}.}  [a_n \sim \frac{B(r)}{r^{\alpha} \Gamma
      (\beta)} \, n^{\beta-1} \left (\frac{1}{r} \right )^{n} = \frac{1(1+1)}
      {1^0\,\Gamma(3)}\,n^{3-1} (1/1)^n = n^2.]
*** Asymptotic growth of the Catalan numbers[edit] ***
Main article: Catalan_number
The ordinary generating function for the Catalan numbers is
            1 &#x2212;   1 &#x2212; 4 x     2 x    .   {\displaystyle {\frac
      {1-{\sqrt {1-4x}}}{2x}}.}  [\frac{1-\sqrt{1-4x}}{2x}.]
With r = 1/4, Î± = 1, Î² = â1/2, A(x) = 1/2, and B(x) = â1/2, we can
conclude that, for the Catalan numbers,
          a  n   &#x223C;    B ( r )    r  &#x03B1;   &#x0393; ( &#x03B2; )
      n  &#x03B2; &#x2212; 1     (   1 r   )   n   =    &#x2212;   1 2
      (   1 4    )  1   &#x0393; ( &#x2212;   1 2   )      n  &#x2212;   1 2
      &#x2212; 1     (   1  1 4    )   n   =   1  &#x03C0;     n  &#x2212;   3
      2       4  n   .   {\displaystyle a_{n}\sim {\frac {B(r)}{r^{\alpha
      }\Gamma (\beta )}}\,n^{\beta -1}\left({\frac {1}{r}}\right)^{n}={\frac {-
      {\frac {1}{2}}}{({\frac {1}{4}})^{1}\Gamma (-{\frac {1}{2}})}}\,n^{-
      {\frac {1}{2}}-1}\left({\frac {1}{\frac {1}{4}}}\right)^{n}={\frac {1}
      {\sqrt {\pi }}}n^{-{\frac {3}{2}}}\,4^{n}.}  [a_{n}\sim {\frac  {B(r)}{r^
      {{\alpha }}\Gamma (\beta )}}\,n^{{\beta -1}}\left({\frac  {1}{r}}\right)^
      {{n}}={\frac  {-{\frac  {1}{2}}}{({\frac  {1}{4}})^{1}\Gamma (-{\frac
      {1}{2}})}}\,n^{{-{\frac  {1}{2}}-1}}\left({\frac  {1}{{\frac  {1}
      {4}}}}\right)^{n}={\frac  {1}{{\sqrt  {\pi }}}}n^{{-{\frac  {3}{2}}}}\,4^
      {n}.]
**** Bivariate and multivariate generating functions[edit] ****
One can define generating functions in several variables for arrays with
several indices. These are called multivariate generating functions or,
sometimes, super generating functions. For two variables, these are often
called bivariate generating functions.
For instance, since     ( 1 + x  )  n     {\displaystyle (1+x)^{n}}  [(1+x)^n]
is the ordinary generating function for binomial_coefficients for a fixed n,
one may ask for a bivariate generating function that generates the binomial
coefficients        (   n k   )      {\displaystyle {\binom {n}{k}}}  [{\binom
{n}{k}}] for all k and n. To do this, consider     ( 1 + x  )  n
{\displaystyle (1+x)^{n}}  [(1+x)^n] as itself a series, in n, and find the
generating function in y that has these as coefficients. Since the generating
function for      a  n     {\displaystyle a^{n}}  [a^{n}] is
           1  1 &#x2212; a y    ,   {\displaystyle {\frac {1}{1-ay}},}  [\frac
      {1}{1-ay},]
the generating function for the binomial coefficients is:
          &#x2211;  n , k      (   n k   )     x  k    y  n   =   1  1 &#x2212;
      ( 1 + x ) y    =   1  1 &#x2212; y &#x2212; x y    .   {\displaystyle
      \sum _{n,k}{\binom {n}{k}}x^{k}y^{n}={\frac {1}{1-(1+x)y}}={\frac {1}{1-
      y-xy}}.}  [\sum_{n,k} \binom{n}{k} x^k y^n = \frac{1}{1-(1+x)y}=\frac{1}
      {1-y-xy}.]
**** Representation by continued fractions (Jacobi-type J-fractions)[edit] ****
*** Definitions[edit] ***
Expansions of (formal) Jacobi-type and Stieltjes-type continued_fractions (J-
fractions and S-fractions, respectively) whose      h  t h     {\displaystyle
h^{th}}  [{\displaystyle h^{th}}] rational convergents represent ___2_h___
{\displaystyle_2h}__[2h]-order_accurate power series are another way to express
the typically divergent ordinary generating functions for many special one and
two-variate sequences. The particular form of the Jacobi-type_continued
fractions (J-fractions) are expanded as in the following equation and have the
next corresponding power series expansions with respect to     z
{\displaystyle z}  [z] for some specific, application-dependent component
sequences,     {   ab   i   }   {\displaystyle \{{\text{ab}}_{i}\}}  [
{\displaystyle \{{\text{ab}}_{i}\}}] and     {  c  i   }   {\displaystyle \{c_
{i}\}}  [{\displaystyle \{c_{i}\}}], where     z &#x2260; 0   {\displaystyle
z\neq 0}  [{\displaystyle z\neq 0}] denotes the formal variable in the second
power series expansion given below:[17]
              J  [ &#x221E; ]   ( z )    =         1          1 &#x2212;  c  1
      z &#x2212;           ab   2    z  2            1 &#x2212;  c  2   z
      &#x2212;           ab   3    z  2            &#x22F1;
      = 1 +  c  1   z +  (    ab   2   +  c  1   2    )   z  2   +  (  2   ab
      2    c  1   +  c  1   3   +   ab   2    c  2    )   z  3   + &#x22EF; .
      {\displaystyle {\begin{aligned}J^{[\infty ]}(z)&={\cfrac {1}{1-c_{1}z-
      {\cfrac {{\text{ab}}_{2}z^{2}}{1-c_{2}z-{\cfrac {{\text{ab}}_{3}z^{2}}
      {\ddots }}}}}}\\&=1+c_{1}z+\left({\text{ab}}_{2}+c_{1}^{2}\right)z^
      {2}+\left(2{\text{ab}}_{2}c_{1}+c_{1}^{3}+{\text{ab}}_{2}c_{2}\right)z^
      {3}+\cdots .\end{aligned}}}  [{\displaystyle {\begin{aligned}J^{[\infty
      ]}(z)&={\cfrac {1}{1-c_{1}z-{\cfrac {{\text{ab}}_{2}z^{2}}{1-c_{2}z-
      {\cfrac {{\text{ab}}_{3}z^{2}}{\ddots }}}}}}\\&=1+c_{1}z+\left({\text
      {ab}}_{2}+c_{1}^{2}\right)z^{2}+\left(2{\text{ab}}_{2}c_{1}+c_{1}^{3}+
      {\text{ab}}_{2}c_{2}\right)z^{3}+\cdots .\end{aligned}}}]
The coefficients of      z  n     {\displaystyle z^{n}}  [z^n], denoted in
shorthand by      j  n   := [  z  n   ]  J  [ &#x221E; ]   ( z )
{\displaystyle j_{n}:=[z^{n}]J^{[\infty ]}(z)}  [{\displaystyle j_{n}:=[z^
{n}]J^{[\infty ]}(z)}], in the previous equations correspond to matrix
solutions of the equations
           [     k  0 , 1      k  1 , 1     0   0   &#x22EF;      k  0 , 2
      k  1 , 2      k  2 , 2     0   &#x22EF;      k  0 , 3      k  1 , 3
      k  2 , 3      k  3 , 3     &#x22EF;     &#x22EE;   &#x22EE;   &#x22EE;
      &#x22EE;    ]   =   [     k  0 , 0     0   0   0   &#x22EF;      k  0 , 1
      k  1 , 1     0   0   &#x22EF;      k  0 , 2      k  1 , 2      k  2 , 2
      0   &#x22EF;     &#x22EE;   &#x22EE;   &#x22EE;   &#x22EE;    ]
      &#x22C5;   [     c  1     1   0   0   &#x22EF;       ab   2      c  2
      1   0   &#x22EF;     0     ab   3      c  3     1   &#x22EF;     &#x22EE;
      &#x22EE;   &#x22EE;   &#x22EE;    ]   ,   {\displaystyle {\begin
      {bmatrix}k_{0,1}&k_{1,1}&0&0&\cdots \\k_{0,2}&k_{1,2}&k_{2,2}&0&\cdots
      \\k_{0,3}&k_{1,3}&k_{2,3}&k_{3,3}&\cdots \\\vdots &\vdots &\vdots &\vdots
      \end{bmatrix}}={\begin{bmatrix}k_{0,0}&0&0&0&\cdots \\k_{0,1}&k_
      {1,1}&0&0&\cdots \\k_{0,2}&k_{1,2}&k_{2,2}&0&\cdots \\\vdots &\vdots
      &\vdots &\vdots \end{bmatrix}}\cdot {\begin{bmatrix}c_{1}&1&0&0&\cdots \\
      {\text{ab}}_{2}&c_{2}&1&0&\cdots \\0&{\text{ab}}_{3}&c_{3}&1&\cdots
      \\\vdots &\vdots &\vdots &\vdots \end{bmatrix}},}  [{\displaystyle
      {\begin{bmatrix}k_{0,1}&k_{1,1}&0&0&\cdots \\k_{0,2}&k_{1,2}&k_
      {2,2}&0&\cdots \\k_{0,3}&k_{1,3}&k_{2,3}&k_{3,3}&\cdots \\\vdots &\vdots
      &\vdots &\vdots \end{bmatrix}}={\begin{bmatrix}k_{0,0}&0&0&0&\cdots \\k_
      {0,1}&k_{1,1}&0&0&\cdots \\k_{0,2}&k_{1,2}&k_{2,2}&0&\cdots \\\vdots
      &\vdots &\vdots &\vdots \end{bmatrix}}\cdot {\begin{bmatrix}c_
      {1}&1&0&0&\cdots \\{\text{ab}}_{2}&c_{2}&1&0&\cdots \\0&{\text{ab}}_
      {3}&c_{3}&1&\cdots \\\vdots &\vdots &\vdots &\vdots \end{bmatrix}},}]
where      j  0   &#x2261;  k  0 , 0   = 1   {\displaystyle j_{0}\equiv k_
{0,0}=1}  [{\displaystyle j_{0}\equiv k_{0,0}=1}],      j  n   =  k  0 , n
{\displaystyle j_{n}=k_{0,n}}  [{\displaystyle j_{n}=k_{0,n}}] for     n
&#x2265; 1   {\displaystyle n\geq 1}  [n\geq 1],      k  r , s   = 0
{\displaystyle k_{r,s}=0}  [{\displaystyle k_{r,s}=0}] if     r > s
{\displaystyle r>s}  [{\displaystyle r>s}], and where for all integers     p ,
q &#x2265; 0   {\displaystyle p,q\geq 0}  [{\displaystyle p,q\geq 0}], we have
an addition formula relation given by
          j  p + q   =  k  0 , p   &#x22C5;  k  0 , q   +  &#x2211;  i = 1
      min ( p , q )     ab   2   &#x22EF;   ab   i + 1   &#x00D7;  k  i , p
      &#x22C5;  k  i , q   .   {\displaystyle j_{p+q}=k_{0,p}\cdot k_{0,q}+\sum
      _{i=1}^{\min(p,q)}{\text{ab}}_{2}\cdots {\text{ab}}_{i+1}\times k_
      {i,p}\cdot k_{i,q}.}  [{\displaystyle j_{p+q}=k_{0,p}\cdot k_{0,q}+\sum _
      {i=1}^{\min(p,q)}{\text{ab}}_{2}\cdots {\text{ab}}_{i+1}\times k_
      {i,p}\cdot k_{i,q}.}]
*** Properties of the hth convergent functions[edit] ***
For     h &#x2265; 0   {\displaystyle h\geq 0}  [{\displaystyle h\geq 0}]
(though in practice when     h &#x2265; 2   {\displaystyle h\geq 2}  [
{\displaystyle h\geq 2}]), we can define the rational      h  th
{\displaystyle h^{\text{th}}}  [{\displaystyle h^{\text{th}}}] convergents to
the infinite J-fraction,      J  [ &#x221E; ]   ( z )   {\displaystyle J^{
[\infty ]}(z)}  [{\displaystyle J^{[\infty ]}(z)}], expanded by
          Conv  h   &#x2061; ( z ) :=     P  h   ( z )    Q  h   ( z )    =  j
      0   +  j  1   z + &#x22EF; +  j  2 h &#x2212; 1    z  2 h &#x2212; 1   +
      &#x2211;  n &#x2265; 2 h       j &#x007E;     h , n    z  n   ,
      {\displaystyle \operatorname {Conv} _{h}(z):={\frac {P_{h}(z)}{Q_{h}
      (z)}}=j_{0}+j_{1}z+\cdots +j_{2h-1}z^{2h-1}+\sum _{n\geq 2h}{\widetilde
      {j}}_{h,n}z^{n},}  [{\displaystyle \operatorname {Conv} _{h}(z):={\frac
      {P_{h}(z)}{Q_{h}(z)}}=j_{0}+j_{1}z+\cdots +j_{2h-1}z^{2h-1}+\sum _{n\geq
      2h}{\widetilde {j}}_{h,n}z^{n},}]
component-wise through the sequences,      P  h   ( z )   {\displaystyle P_{h}
(z)}  [{\displaystyle P_{h}(z)}] and      Q  h   ( z )   {\displaystyle Q_{h}
(z)}  [{\displaystyle Q_{h}(z)}], defined recursively by
              P  h   ( z )    = ( 1 &#x2212;  c  h   z )  P  h &#x2212; 1   ( z
      ) &#x2212;   ab   h    z  2    P  h &#x2212; 2   ( z ) +  &#x03B4;  h , 1
      Q  h   ( z )    = ( 1 &#x2212;  c  h   z )  Q  h &#x2212; 1   ( z )
      &#x2212;   ab   h    z  2    Q  h &#x2212; 2   ( z ) + ( 1 &#x2212;  c  1
      z )  &#x03B4;  h , 1   +  &#x03B4;  0 , 1   .       {\displaystyle
      {\begin{aligned}P_{h}(z)&=(1-c_{h}z)P_{h-1}(z)-{\text{ab}}_{h}z^{2}P_{h-
      2}(z)+\delta _{h,1}\\Q_{h}(z)&=(1-c_{h}z)Q_{h-1}(z)-{\text{ab}}_{h}z^
      {2}Q_{h-2}(z)+(1-c_{1}z)\delta _{h,1}+\delta _{0,1}.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}P_{h}(z)&=(1-c_{h}z)P_{h-1}(z)-{\text
      {ab}}_{h}z^{2}P_{h-2}(z)+\delta _{h,1}\\Q_{h}(z)&=(1-c_{h}z)Q_{h-1}(z)-
      {\text{ab}}_{h}z^{2}Q_{h-2}(z)+(1-c_{1}z)\delta _{h,1}+\delta _{0,1}.\end
      {aligned}}}]
Moreover, the rationality of the convergent function,       Conv   h   ( z )
{\displaystyle {\text{Conv}}_{h}(z)}  [{\displaystyle {\text{Conv}}_{h}(z)}]
for all     h &#x2265; 2   {\displaystyle h\geq 2}  [{\displaystyle h\geq 2}]
implies additional finite difference equations and congruence properties
satisfied by the sequence of      j  n     {\displaystyle j_{n}}  [
{\displaystyle j_{n}}], and for      M  h   :=   ab   2   &#x22EF;   ab   h + 1
{\displaystyle M_{h}:={\text{ab}}_{2}\cdots {\text{ab}}_{h+1}}  [{\displaystyle
M_{h}:={\text{ab}}_{2}\cdots {\text{ab}}_{h+1}}] if     h  |  &#x2223;  M  h
{\displaystyle h|\mid M_{h}}  [{\displaystyle h|\mid M_{h}}] then we have the
congruence
          j  n   &#x2261; [  z  n   ]  Conv  h   &#x2061; ( z )   ( mod  h )  ,
      {\displaystyle j_{n}\equiv [z^{n}]\operatorname {Conv} _{h}(z){\pmod
      {h}},}  [{\displaystyle j_{n}\equiv [z^{n}]\operatorname {Conv} _{h}(z)
      {\pmod {h}},}]
for non-symbolic, determinate choices of the parameter sequences,     {   ab
i   }   {\displaystyle \{{\text{ab}}_{i}\}}  [{\displaystyle \{{\text{ab}}_
{i}\}}] and     {  c  i   }   {\displaystyle \{c_{i}\}}  [{\displaystyle \{c_
{i}\}}], when     h &#x2265; 2   {\displaystyle h\geq 2}  [{\displaystyle h\geq
2}], i.e., when these sequences do not implicitly depend on an auxiliary
parameter such as     q   {\displaystyle q}  [q],     x   {\displaystyle x}
[x], or     R   {\displaystyle R}  [R] as in the examples contained in the
table below.
*** Examples[edit] ***
The next table provides examples of closed-form formulas for the component
sequences found computationally (and subsequently proved correct in the cited
references [18]) in several special cases of the prescribed sequences,      j
n     {\displaystyle j_{n}}  [{\displaystyle j_{n}}], generated by the general
expansions of the J-fractions defined in the first subsection. Here we define
0 <  |  a  |  ,  |  b  |  ,  |  q  |  < 1   {\displaystyle 0<|a|,|b|,|q|<1}  [
{\displaystyle 0<|a|,|b|,|q|<1}] and the parameters     R   {\displaystyle R}
[R],     &#x03B1; &#x2208;   Z   +     {\displaystyle \alpha \in \mathbb {Z} ^
{+}}  [{\displaystyle \alpha \in \mathbb {Z} ^{+}}] and     x   {\displaystyle
x}  [x] to be indeterminates with respect to these expansions, where the
prescribed sequences enumerated by the expansions of these J-fractions are
defined in terms of the q-Pochhammer_symbol, Pochhammer_symbol, and the
binomial_coefficients.
                                                                 ab   i   ( i
    j  n                                    c  i   ( i      &#x2265; 2 )
{\displaystyle j_       c  1            &#x2265; 2 )        {\displaystyle
{n}}  [             {\displaystyle c_   {\displaystyle c_   {\text{ab}}_{i}
{\displaystyle j_   {1}}  [c_{1}]       {i}(i\geq 2)}  [    (i\geq 2)}  [
{n}}]                                   {\displaystyle c_   {\displaystyle
                                        {i}(i\geq 2)}]      {\text{ab}}_{i}
                                                            (i\geq 2)}]
                                            q  2 h &#x2212;
                                        3    (   q  2 h   +     q  6 h &#x2212;
                                        q  2 h &#x2212; 2   10    (   q  2 h
    q   n  2                            &#x2212; 1  )       &#x2212; 2
{\displaystyle q^      q                {\displaystyle q^   &#x2212; 1  )
{n^{2}}}  [         {\displaystyle q}   {2h-3}\left(q^      {\displaystyle q^
{\displaystyle q^   [q]                 {2h}+q^{2h-2}-      {6h-10}\left(q^{2h-
{n^{2}}}]                               1\right)}  [        2}-1\right)}  [
                                        {\displaystyle q^   {\displaystyle q^
                                        {2h-3}\left(q^      {6h-10}\left(q^{2h-
                                        {2h}+q^{2h-2}-      2}-1\right)}]
                                        1\right)}]
                                            q  h &#x2212; 1
                                        &#x2212; a  q  h       a  q  2 h
                                        &#x2212; 2    (   q &#x2212; 4   ( a  q
                                        h   +  q  h         h &#x2212; 2
   ( a ; q  )  n                        &#x2212; 1          &#x2212; 1 ) (  q
{\displaystyle         1 &#x2212; a     &#x2212; 1  )       h &#x2212; 1
(a;q)_{n}}  [       {\displaystyle 1-a} {\displaystyle q^   &#x2212; 1 )
{\displaystyle      [1-a]               {h-1}-aq^{h-2}\left {\displaystyle aq^
(a;q)_{n}}]                             (q^{h}+q^{h-1}-     {2h-4}(aq^{h-2}-1)
                                        1\right)}  [        (q^{h-1}-1)}  [
                                        {\displaystyle q^   {\displaystyle aq^
                                        {h-1}-aq^{h-2}\left {2h-4}(aq^{h-2}-1)
                                        (q^{h}+q^{h-1}-     (q^{h-1}-1)}]
                                        1\right)}]
                                                                  (  q  h
                                               q  h         &#x2212; 1
                                        &#x2212; z &#x2212; &#x2212; 1 ) (  q
     (  z  q                            q z +  q  h   z   q h &#x2212; 1
&#x2212; n   ; q  )       q &#x2212; z  2 h &#x2212; 1      &#x2212; z )
n                   q                   {\displaystyle      &#x22C5; z   q  4 h
{\displaystyle      {\displaystyle      {\frac {q^{h}-z-    &#x2212; 5
\left(zq^{-         {\frac {q-z}{q}}}   qz+q^{h}z}{q^{2h-   {\displaystyle
n};q\right)_{n}}  [ [{\displaystyle     1}}}}  [            {\frac {(q^{h-1}-1)
{\displaystyle      {\frac {q-z}{q}}}]  {\displaystyle      (q^{h-1}-z)\cdot z}
\left(zq^{-                             {\frac {q^{h}-z-    {q^{4h-5}}}}  [
n};q\right)_{n}}]                       qz+q^{h}z}{q^{2h-   {\displaystyle
                                        1}}}}]              {\frac {(q^{h-1}-1)
                                                            (q^{h-1}-z)\cdot z}
                                                            {q^{4h-5}}}}]
                                                                   q  2 i
                                               q  i         &#x2212; 4   ( 1
                                        &#x2212; 2    (  q  &#x2212; b  q  i
                                        + a b  q  2 i       &#x2212; 3   ) ( 1
                                        &#x2212; 3   + a    &#x2212; a  q  i
                                        ( 1 &#x2212;  q  i  &#x2212; 2   ) ( a
                                        &#x2212; 1          &#x2212; b  q  i
                                        &#x2212;  q  i   )  &#x2212; 2   ) ( 1
                                        + b (  q  i         &#x2212;  q  i
                                        &#x2212; q &#x2212; &#x2212; 1   )
                                        1 )  )    ( 1       ( 1 &#x2212; b  q
                                        &#x2212; b  q  2 i  2 i &#x2212; 5   )
      ( a ; q  )  n                     &#x2212; 4   ) ( 1  ( 1 &#x2212; b  q
( b ; q  )  n             1 &#x2212; a  &#x2212; b  q  2 i  2 i &#x2212; 4    )
{\displaystyle      1 &#x2212; b        &#x2212; 2   )      2   ( 1 &#x2212; b
{\frac {(a;q)_{n}}{ {\displaystyle      {\displaystyle      q  2 i &#x2212; 3
(b;q)_{n}}}}  [     {\frac {1-a}{1-b}}} {\frac {q^{i-       )
{\displaystyle      [{\displaystyle     2}\left(q+abq^{2i-  {\displaystyle
{\frac {(a;q)_{n}}{ {\frac {1-a}{1-     3}+a(1-q^{i-1}-q^   {\frac {q^{2i-4}(1-
(b;q)_{n}}}}]       b}}}]               {i})+b(q^{i}-q-     bq^{i-3})(1-aq^{i-
                                        1)\right)}{(1-bq^   2})(a-bq^{i-2})(1-
                                        {2i-4})(1-bq^{2i-   q^{i-1})}{(1-bq^
                                        2})}}}  [           {2i-5})(1-bq^{2i-
                                        {\displaystyle      4})^{2}(1-bq^{2i-
                                        {\frac {q^{i-       3})}}}  [
                                        2}\left(q+abq^{2i-  {\displaystyle
                                        3}+a(1-q^{i-1}-q^   {\frac {q^{2i-4}(1-
                                        {i})+b(q^{i}-q-     bq^{i-3})(1-aq^{i-
                                        1)\right)}{(1-bq^   2})(a-bq^{i-2})(1-
                                        {2i-4})(1-bq^{2i-   q^{i-1})}{(1-bq^
                                        2})}}}]             {2i-5})(1-bq^{2i-
                                                            4})^{2}(1-bq^{2i-
                                                            3})}}}]
    &#x03B1;  n
&#x22C5;   (   R                                               ( i &#x2212; 1 )
&#x03B1;   )   n                                            &#x03B1; ( R + ( i
{\displaystyle                             R + 2 &#x03B1;   &#x2212; 2 )
\alpha ^{n}\cdot                        ( i &#x2212; 1 )    &#x03B1; )
\left({\frac {R}       R                {\displaystyle      {\displaystyle (i-
{\alpha }}\right)_  {\displaystyle R}   R+2\alpha (i-1)}  [ 1)\alpha (R+(i-
{n}}  [             [R]                 {\displaystyle      2)\alpha )}  [
{\displaystyle                          R+2\alpha (i-1)}]   {\displaystyle (i-
\alpha ^{n}\cdot                                            1)\alpha (R+(i-
\left({\frac {R}                                            2)\alpha )}]
{\alpha }}\right)_
{n}}]






                                                                        {




                                                            &#x2212;






                                                            (

                                                            x

                                                            &#x2212;

                                                            i

                                                            +

                                                            2

                                                            )

                                                            (

                                                            x

                                                            +

                                                            i

                                                            &#x2212;

                                                            1

                                                            )





                                                            4

                                                            &#x22C5;

                                                            (

                                                            2

                                                            i

                                                            &#x2212;

                                                            3
                                           &#x2212;    ( x
                                        + 2 ( i &#x2212; 1
                                        )  2   )   ( 2 i
   ( &#x2212; 1  )                      &#x2212; 1 ) ( 2 i  )
n      (   x n   )                      &#x2212; 3 )
{\displaystyle (-      &#x2212; x       {\displaystyle -
1)^{n}{\binom {x}   {\displaystyle -x}  {\frac {(x+2(i-1)^
{n}}}  [            [-x]                {2})}{(2i-1)(2i-    2
{\displaystyle (-                       3)}}}  [
1)^{n}{\binom {x}                       {\displaystyle -
{n}}}]                                  {\frac {(x+2(i-1)^
                                        {2})}{(2i-1)(2i-
                                        3)}}}]






                                                                              i

                                                            &#x2265;
                                                                              3
                                                                              ;





                                                            &#x2212;




                                                            1

                                                            2



                                                                              x
                                                                              (
                                                                              x
                                                                              +
                                                                              1
                                                                              )


                                                                              i
                                                                              =

                                                            2.








                                                                {\displaystyle
                                                            {\begin{cases}-
                                                            {\frac {(x-i+2)
                                                            (x+i-1)}{4\cdot
                                                            (2i-3)^{2}}}&i\geq
                                                            3;\\-{\frac {1}
                                                            {2}}x(x+1)&i=2.\end
                                                            {cases}}}

                                                            [{\displaystyle
                                                            {\begin{cases}-
                                                            {\frac {(x-i+2)
                                                            (x+i-1)}{4\cdot
                                                            (2i-3)^{2}}}&i\geq
                                                            3;\\-{\frac {1}
                                                            {2}}x(x+1)&i=2.\end
                                                            {cases}}}]






                                                                        {




                                                            &#x2212;






                                                            (

                                                            x

                                                            &#x2212;

                                                            i

                                                            +

                                                            2

                                                            )

                                                            (

                                                            x

                                                            +

                                                            i

                                                            &#x2212;

                                                            1

                                                            )





                                                            4

                                                            &#x22C5;

                                                            (

                                                            2

                                                            i

                                                            &#x2212;

                                                            3

                                              ( x &#x2212;
   ( &#x2212; 1  )                      2 i ( i &#x2212; 2
n      (    x + n                       ) &#x2212; 1 )      )
n   )                  &#x2212; ( x + 1 ( 2 i &#x2212; 1 )
{\displaystyle (-   )   {\displaystyle  ( 2 i &#x2212; 3 )
1)^{n}{\binom {x+n} -(x+1)}  [          {\displaystyle
{n}}}  [            {\displaystyle -    {\frac {(x-2i(i-2)- 2
{\displaystyle (-   (x+1)}]             1)}{(2i-1)(2i-3)}}}
1)^{n}{\binom {x+n}                     [{\displaystyle
{n}}}]                                  {\frac {(x-2i(i-2)-
                                        1)}{(2i-1)(2i-
                                        3)}}}]






                                                                              i

                                                            &#x2265;
                                                                              3
                                                                              ;





                                                            &#x2212;




                                                            1

                                                            2



                                                                              x
                                                                              (
                                                                              x
                                                                              +
                                                                              1
                                                                              )


                                                                              i
                                                                              =

                                                            2.








                                                                {\displaystyle
                                                            {\begin{cases}-
                                                            {\frac {(x-i+2)
                                                            (x+i-1)}{4\cdot
                                                            (2i-3)^{2}}}&i\geq
                                                            3;\\-{\frac {1}
                                                            {2}}x(x+1)&i=2.\end
                                                            {cases}}}

                                                            [{\displaystyle
                                                            {\begin{cases}-
                                                            {\frac {(x-i+2)
                                                            (x+i-1)}{4\cdot
                                                            (2i-3)^{2}}}&i\geq
                                                            3;\\-{\frac {1}
                                                            {2}}x(x+1)&i=2.\end
                                                            {cases}}}]
Note that the radii of convergence of these series corresponding to the
definition of the Jacobi-type J-fractions given above are in general different
from that of the corresponding power series expansions defining the ordinary
generating functions of these sequences.
***** Examples[edit] *****
Main article: Examples_of_generating_functions
Generating functions for the sequence of square_numbers an = n2 are:
**** Ordinary generating function[edit] ****
         G (  n  2   ; x ) =  &#x2211;  n = 0   &#x221E;    n  2    x  n   =
      x ( x + 1 )   ( 1 &#x2212; x  )  3        {\displaystyle G(n^{2};x)=\sum
      _{n=0}^{\infty }n^{2}x^{n}={\frac {x(x+1)}{(1-x)^{3}}}}  [{\displaystyle
      G(n^{2};x)=\sum _{n=0}^{\infty }n^{2}x^{n}={\frac {x(x+1)}{(1-x)^{3}}}}]
**** Exponential generating function[edit] ****
         EG &#x2061; (  n  2   ; x ) =  &#x2211;  n = 0   &#x221E;       n  2
      x  n     n !    = x ( x + 1 )  e  x     {\displaystyle \operatorname {EG}
      (n^{2};x)=\sum _{n=0}^{\infty }{\frac {n^{2}x^{n}}{n!}}=x(x+1)e^{x}}  [
      {\displaystyle \operatorname {EG} (n^{2};x)=\sum _{n=0}^{\infty }{\frac
      {n^{2}x^{n}}{n!}}=x(x+1)e^{x}}]
**** Lambert series[edit] ****
As an example of a Lambert series identity not given in the main_article, we
can show that for      |  x  |  ,  |  x q  |  < 1   {\displaystyle |x|,|xq|<1}
[{\displaystyle |x|,|xq|<1}] we have that [19]
          &#x2211;  n &#x2265; 1       q  n    x  n     1 &#x2212;  x  n      =
      &#x2211;  n &#x2265; 1       q  n    x   n  2       1 &#x2212; q  x  n
      +  &#x2211;  n &#x2265; 1       q  n    x  n ( n + 1 )     1 &#x2212;  x
      n      ,   {\displaystyle \sum _{n\geq 1}{\frac {q^{n}x^{n}}{1-x^
      {n}}}=\sum _{n\geq 1}{\frac {q^{n}x^{n^{2}}}{1-qx^{n}}}+\sum _{n\geq 1}
      {\frac {q^{n}x^{n(n+1)}}{1-x^{n}}},}  [{\displaystyle \sum _{n\geq 1}
      {\frac {q^{n}x^{n}}{1-x^{n}}}=\sum _{n\geq 1}{\frac {q^{n}x^{n^{2}}}{1-
      qx^{n}}}+\sum _{n\geq 1}{\frac {q^{n}x^{n(n+1)}}{1-x^{n}}},}]
where we have the special case identity for the generating function of the
divisor_function,     d ( n ) &#x2261;  &#x03C3;  0   ( n )   {\displaystyle d
(n)\equiv \sigma _{0}(n)}  [{\displaystyle d(n)\equiv \sigma _{0}(n)}], given
by
          &#x2211;  n &#x2265; 1      x  n    1 &#x2212;  x  n      =  &#x2211;
      n &#x2265; 1       x   n  2     ( 1 +  x  n   )   1 &#x2212;  x  n      .
      {\displaystyle \sum _{n\geq 1}{\frac {x^{n}}{1-x^{n}}}=\sum _{n\geq 1}
      {\frac {x^{n^{2}}(1+x^{n})}{1-x^{n}}}.}  [{\displaystyle \sum _{n\geq 1}
      {\frac {x^{n}}{1-x^{n}}}=\sum _{n\geq 1}{\frac {x^{n^{2}}(1+x^{n})}{1-x^
      {n}}}.}]
**** Bell series[edit] ****
          BG  p   &#x2061; (  n  2   ; x ) =  &#x2211;  n = 0   &#x221E;   (  p
      n    )  2    x  n   =   1  1 &#x2212;  p  2   x      {\displaystyle
      \operatorname {BG} _{p}(n^{2};x)=\sum _{n=0}^{\infty }(p^{n})^{2}x^{n}=
      {\frac {1}{1-p^{2}x}}}  [\operatorname{BG}_p(n^2;x)=\sum_{n=0}^\infty (p^
      {n})^2x^n=\frac{1}{1-p^2x}]
**** Dirichlet series generating function[edit] ****
         DG &#x2061; (  n  2   ; s ) =  &#x2211;  n = 1   &#x221E;      n  2
      n  s     = &#x03B6; ( s &#x2212; 2 ) ,   {\displaystyle \operatorname
      {DG} (n^{2};s)=\sum _{n=1}^{\infty }{\frac {n^{2}}{n^{s}}}=\zeta (s-2),}
      [{\displaystyle \operatorname {DG} (n^{2};s)=\sum _{n=1}^{\infty }{\frac
      {n^{2}}{n^{s}}}=\zeta (s-2),}]
using the Riemann_zeta_function.
The sequence ak generated by a Dirichlet_series generating function (DGF)
corresponding to:
         DG &#x2061; (  a  k   ; s ) = &#x03B6; ( s  )  m     {\displaystyle
      \operatorname {DG} (a_{k};s)=\zeta (s)^{m}}  [{\displaystyle
      \operatorname {DG} (a_{k};s)=\zeta (s)^{m}}]
where     &#x03B6; ( s )   {\displaystyle \zeta (s)}  [\zeta (s)] is the
Riemann_zeta_function, has the ordinary generating function:
          &#x2211;  k = 1   k = n    a  k    x  k   = x +    (   m 1   )
      &#x2211;  2 &#x2264; a &#x2264; n    x  a   +    (   m 2   )
      &#x2211;  a &#x2265; 2    &#x2211;  b &#x2265; 2     a b &#x2264; n     x
      a b   +    (   m 3   )        &#x2211;  a &#x2265; 2    &#x2211;  c
      &#x2265; 2    &#x2211;  b &#x2265; 2     a b c &#x2264; n     x  a b c
      +    (   m 4   )        &#x2211;  a &#x2265; 2    &#x2211;  b &#x2265; 2
      &#x2211;  c &#x2265; 2    &#x2211;  d &#x2265; 2     a b c d &#x2264; n
      x  a b c d   + &#x22EF;   {\displaystyle \sum _{k=1}^{k=n}a_{k}x^{k}=x+{m
      \choose 1}\sum _{2\leq a\leq n}x^{a}+{m \choose 2}{\underset {ab\leq n}
      {\sum _{a\geq 2}\sum _{b\geq 2}}}x^{ab}+{m \choose 3}{\underset {abc\leq
      n}{\sum _{a\geq 2}\sum _{c\geq 2}\sum _{b\geq 2}}}x^{abc}+{m \choose 4}
      {\underset {abcd\leq n}{\sum _{a\geq 2}\sum _{b\geq 2}\sum _{c\geq 2}\sum
      _{d\geq 2}}}x^{abcd}+\cdots }  [{\displaystyle \sum _{k=1}^{k=n}a_{k}x^
      {k}=x+{m \choose 1}\sum _{2\leq a\leq n}x^{a}+{m \choose 2}{\underset
      {ab\leq n}{\sum _{a\geq 2}\sum _{b\geq 2}}}x^{ab}+{m \choose 3}{\underset
      {abc\leq n}{\sum _{a\geq 2}\sum _{c\geq 2}\sum _{b\geq 2}}}x^{abc}+{m
      \choose 4}{\underset {abcd\leq n}{\sum _{a\geq 2}\sum _{b\geq 2}\sum _
      {c\geq 2}\sum _{d\geq 2}}}x^{abcd}+\cdots }]
**** Multivariate generating functions[edit] ****
Multivariate generating functions arise in practice when calculating the number
of contingency_tables of non-negative integers with specified row and column
totals. Suppose the table has r rows and c columns; the row sums are      t  1
, &#x2026;  t  r     {\displaystyle t_{1},\ldots t_{r}}  [t_1,\ldots t_r] and
the column sums are      s  1   , &#x2026;  s  c     {\displaystyle s_
{1},\ldots s_{c}}  [s_1,\ldots s_c]. Then, according to I._J._Good,[20] the
number of such tables is the coefficient of
          x  1    t  1     &#x2026;  x  r    t  r      y  1    s  1
      &#x2026;  y  c    s  c       {\displaystyle x_{1}^{t_{1}}\ldots x_{r}^{t_
      {r}}y_{1}^{s_{1}}\ldots y_{c}^{s_{c}}}  [x_1^{t_1}\ldots x_r^{t_r}y_1^
      {s_1}\ldots y_c^{s_c}]
in
          &#x220F;  i = 1   r    &#x220F;  j = 1   c     1  1 &#x2212;  x  i
      y  j      .   {\displaystyle \prod _{i=1}^{r}\prod _{j=1}^{c}{\frac {1}
      {1-x_{i}y_{j}}}.}  [\prod_{i=1}^{r}\prod_{j=1}^c\frac{1}{1-x_iy_j}.]
In the bivariate case, non-polynomial double sum examples of so-termed "double"
or "super" generating functions of the form     G ( w , z ) :=  &#x2211;  m , n
&#x2265; 0    g  m , n    w  m    z  n     {\displaystyle G(w,z):=\sum _
{m,n\geq 0}g_{m,n}w^{m}z^{n}}  [{\displaystyle G(w,z):=\sum _{m,n\geq 0}g_
{m,n}w^{m}z^{n}}] include the following two-variable generating functions for
the binomial_coefficients, the Stirling_numbers, and the Eulerian_numbers:[21]
              e  z + w z      =  &#x2211;  m , n &#x2265; 0      (   n m   )
      w  m      z  n    n !         e  w (  e  z   &#x2212; 1 )      =
      &#x2211;  m , n &#x2265; 0    {     n     m     }   w  m      z  n    n !
      1  ( 1 &#x2212; z  )  w         =  &#x2211;  m , n &#x2265; 0    [     n
      m     ]   w  m      z  n    n !           1 &#x2212; w    e  ( w &#x2212;
      1 ) z   &#x2212; w       =  &#x2211;  m , n &#x2265; 0    &#x27E8;     n
      m     &#x27E9;   w  m      z  n    n !            e  w   &#x2212;  e  z
      w  e  z   &#x2212; z  e  w         =  &#x2211;  m , n &#x2265; 0
      &#x27E8;     m + n + 1     m     &#x27E9;      w  m    z  n     ( m + n +
      1 ) !    .       {\displaystyle {\begin{aligned}e^{z+wz}&=\sum _{m,n\geq
      0}{\binom {n}{m}}w^{m}{\frac {z^{n}}{n!}}\\e^{w(e^{z}-1)}&=\sum _{m,n\geq
      0}\left\{{\begin{matrix}n\\m\end{matrix}}\right\}w^{m}{\frac {z^{n}}
      {n!}}\\{\frac {1}{(1-z)^{w}}}&=\sum _{m,n\geq 0}\left[{\begin
      {matrix}n\\m\end{matrix}}\right]w^{m}{\frac {z^{n}}{n!}}\\{\frac {1-w}{e^
      {(w-1)z}-w}}&=\sum _{m,n\geq 0}\left\langle {\begin{matrix}n\\m\end
      {matrix}}\right\rangle w^{m}{\frac {z^{n}}{n!}}\\{\frac {e^{w}-e^{z}}{we^
      {z}-ze^{w}}}&=\sum _{m,n\geq 0}\left\langle {\begin{matrix}m+n+1\\m\end
      {matrix}}\right\rangle {\frac {w^{m}z^{n}}{(m+n+1)!}}.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}e^{z+wz}&=\sum _{m,n\geq 0}{\binom {n}
      {m}}w^{m}{\frac {z^{n}}{n!}}\\e^{w(e^{z}-1)}&=\sum _{m,n\geq 0}\left\{
      {\begin{matrix}n\\m\end{matrix}}\right\}w^{m}{\frac {z^{n}}{n!}}\\{\frac
      {1}{(1-z)^{w}}}&=\sum _{m,n\geq 0}\left[{\begin{matrix}n\\m\end
      {matrix}}\right]w^{m}{\frac {z^{n}}{n!}}\\{\frac {1-w}{e^{(w-1)z}-
      w}}&=\sum _{m,n\geq 0}\left\langle {\begin{matrix}n\\m\end
      {matrix}}\right\rangle w^{m}{\frac {z^{n}}{n!}}\\{\frac {e^{w}-e^{z}}{we^
      {z}-ze^{w}}}&=\sum _{m,n\geq 0}\left\langle {\begin{matrix}m+n+1\\m\end
      {matrix}}\right\rangle {\frac {w^{m}z^{n}}{(m+n+1)!}}.\end{aligned}}}]
***** Applications[edit] *****
**** Various techniques: Evaluating sums and tackling other problems with
generating functions[edit] ****
*** Example 1: A formula for sums of harmonic numbers[edit] ***
Generating functions give us several methods to manipulate sums and to
establish identities between sums.
The simplest case occurs when      s  n   =  &#x2211;  k = 0   n     a  k
{\displaystyle s_{n}=\sum _{k=0}^{n}{a_{k}}}  [s_{n}=\sum _{{k=0}}^{{n}}{a_
{k}}]. We then know that     S ( z ) =    A ( z )   1 &#x2212; z
{\displaystyle S(z)={\frac {A(z)}{1-z}}}  [S(z)={\frac  {A(z)}{1-z}}] for the
corresponding ordinary generating functions.
For example, we can manipulate      s  n   =  &#x2211;  k = 1   n    H  k
{\displaystyle s_{n}=\sum _{k=1}^{n}H_{k}}  [s_{n}=\sum _{{k=1}}^{{n}}H_{{k}}],
where      H  k   = 1 +   1 2   + &#x22EF; +   1 k     {\displaystyle H_{k}=1+
{\frac {1}{2}}+\cdots +{\frac {1}{k}}}  [H_{k}=1+{\frac  {1}{2}}+\cdots +{\frac
{1}{k}}] are the harmonic_numbers. Let     H ( z ) =  &#x2211;  n &#x2265; 1
H  n    z  n      {\displaystyle H(z)=\sum _{n\geq 1}{H_{n}z^{n}}}  [
{\displaystyle H(z)=\sum _{n\geq 1}{H_{n}z^{n}}}] be the ordinary generating
function of the harmonic numbers. Then
         H ( z ) =      &#x2211;  n &#x2265; 1      1 n    z  n      1 &#x2212;
      z      ,   {\displaystyle H(z)={\dfrac {\sum _{n\geq 1}{{\frac {1}{n}}z^
      {n}}}{1-z}}\,,}  [H(z)={\dfrac  {\sum _{{n\geq 1}}{{\frac  {1}{n}}z^{n}}}
      {1-z}}\,,]
and thus
         S ( z ) =  &#x2211;  n &#x2265; 1     s  n    z  n    =      &#x2211;
      n &#x2265; 1      1 n    z  n      ( 1 &#x2212; z  )  2        .
      {\displaystyle S(z)=\sum _{n\geq 1}{s_{n}z^{n}}={\dfrac {\sum _{n\geq 1}{
      {\frac {1}{n}}z^{n}}}{(1-z)^{2}}}\,.}  [S(z)=\sum _{{n\geq 1}}{s_{n}z^
      {n}}={\dfrac  {\sum _{{n\geq 1}}{{\frac  {1}{n}}z^{n}}}{(1-z)^{2}}}\,.]
Using       1  ( 1 &#x2212; z  )  2      =  &#x2211;  n &#x2265; 0    ( n + 1 )
z  n      {\displaystyle {\frac {1}{(1-z)^{2}}}=\sum _{n\geq 0}{(n+1)z^{n}}}  [
{\frac  {1}{(1-z)^{2}}}=\sum _{{n\geq 0}}{(n+1)z^{n}}], convolution with the
numerator yields
          s  n   =  &#x2211;  k = 1   n      1 k   ( n + 1 &#x2212; k )  = ( n
      + 1 )  H  n   &#x2212; n  ,   {\displaystyle s_{n}=\sum _{k=1}^{n}{{\frac
      {1}{k}}(n+1-k)}=(n+1)H_{n}-n\,,}  [s_{n}=\sum _{{k=1}}^{{n}}{{\frac  {1}
      {k}}(n+1-k)}=(n+1)H_{n}-n\,,]
which can also be written as
          &#x2211;  k = 1   n     H  k    = ( n + 1 ) (  H  n + 1   &#x2212; 1
      )  .   {\displaystyle \sum _{k=1}^{n}{H_{k}}=(n+1)(H_{n+1}-1)\,.}  [\sum
      _{{k=1}}^{{n}}{H_{k}}=(n+1)(H_{{n+1}}-1)\,.]
*** Example 2: Modified binomial coefficient sums and the binomial transform
[edit] ***
As another example of using generating functions to relate sequences and
manipulate sums, for an arbitrary sequence     &#x27E8;  f  n   &#x27E9;
{\displaystyle \langle f_{n}\rangle }  [{\displaystyle \langle f_{n}\rangle }]
we define the two sequences of sums
          s  n   :=  &#x2211;  m = 0   n      (   n m   )     f  m    3  n
      &#x2212; m     {\displaystyle s_{n}:=\sum _{m=0}^{n}{\binom {n}{m}}f_
      {m}3^{n-m}}  [{\displaystyle s_{n}:=\sum _{m=0}^{n}{\binom {n}{m}}f_{m}3^
      {n-m}}]
             s &#x007E;     n   :=  &#x2211;  m = 0   n      (   n m   )    ( m
      + 1 ) ( m + 2 ) ( m + 3 )  f  m    3  n &#x2212; m   ,   {\displaystyle
      {\widetilde {s}}_{n}:=\sum _{m=0}^{n}{\binom {n}{m}}(m+1)(m+2)(m+3)f_
      {m}3^{n-m},}  [{\displaystyle {\widetilde {s}}_{n}:=\sum _{m=0}^{n}
      {\binom {n}{m}}(m+1)(m+2)(m+3)f_{m}3^{n-m},}]
for all     n &#x2265; 0   {\displaystyle n\geq 0}  [n\geq 0], and seek to
express the second sums in terms of the first. We suggest an approach by
generating functions.
First, we use the binomial_transform to write the generating function for the
first sum as
         S ( z ) =   1  ( 1 &#x2212; 3 z )    F  (   z  1 &#x2212; 3 z    )  .
      {\displaystyle S(z)={\frac {1}{(1-3z)}}F\left({\frac {z}{1-3z}}\right).}
      [{\displaystyle S(z)={\frac {1}{(1-3z)}}F\left({\frac {z}{1-
      3z}}\right).}]
Since the generating function for the sequence     &#x27E8; ( n + 1 ) ( n + 2 )
( n + 3 )  f  n   &#x27E9;   {\displaystyle \langle (n+1)(n+2)(n+3)f_{n}\rangle
}  [{\displaystyle \langle (n+1)(n+2)(n+3)f_{n}\rangle }] is given by     6 F
( z ) + 18 z  F  &#x2032;   ( z ) + 9  z  2    F  &#x2032; &#x2032;   ( z ) +
z  3    F  ( 3 )   ( z )   {\displaystyle 6F(z)+18zF^{\prime }(z)+9z^{2}F^
{\prime \prime }(z)+z^{3}F^{(3)}(z)}  [{\displaystyle 6F(z)+18zF^{\prime }
(z)+9z^{2}F^{\prime \prime }(z)+z^{3}F^{(3)}(z)}], we may write the generating
function for the second sum defined above in the form
            S &#x007E;    ( z ) =   6  ( 1 &#x2212; 3 z )    F  (   z  1
      &#x2212; 3 z    )  +    18 z   ( 1 &#x2212; 3 z  )  2       F  &#x2032;
      (   z  1 &#x2212; 3 z    )  +    9  z  2     ( 1 &#x2212; 3 z  )  3
      F  &#x2032; &#x2032;    (   z  1 &#x2212; 3 z    )  +    z  3    ( 1
      &#x2212; 3 z  )  4       F  ( 3 )    (   z  1 &#x2212; 3 z    )  .
      {\displaystyle {\widetilde {S}}(z)={\frac {6}{(1-3z)}}F\left({\frac {z}
      {1-3z}}\right)+{\frac {18z}{(1-3z)^{2}}}F^{\prime }\left({\frac {z}{1-
      3z}}\right)+{\frac {9z^{2}}{(1-3z)^{3}}}F^{\prime \prime }\left({\frac
      {z}{1-3z}}\right)+{\frac {z^{3}}{(1-3z)^{4}}}F^{(3)}\left({\frac {z}{1-
      3z}}\right).}  [{\displaystyle {\widetilde {S}}(z)={\frac {6}{(1-
      3z)}}F\left({\frac {z}{1-3z}}\right)+{\frac {18z}{(1-3z)^{2}}}F^{\prime
      }\left({\frac {z}{1-3z}}\right)+{\frac {9z^{2}}{(1-3z)^{3}}}F^{\prime
      \prime }\left({\frac {z}{1-3z}}\right)+{\frac {z^{3}}{(1-3z)^{4}}}F^{
      (3)}\left({\frac {z}{1-3z}}\right).}]
In particular, we may write this modified sum generating function in the form
of
         a ( z ) &#x22C5; S ( z ) + b ( z ) &#x22C5; z  S  &#x2032;   ( z ) + c
      ( z ) &#x22C5;  z  2    S  &#x2032; &#x2032;   ( z ) + d ( z ) &#x22C5;
      z  3    S  ( 3 )   ( z ) ,   {\displaystyle a(z)\cdot S(z)+b(z)\cdot zS^
      {\prime }(z)+c(z)\cdot z^{2}S^{\prime \prime }(z)+d(z)\cdot z^{3}S^{(3)}
      (z),}  [{\displaystyle a(z)\cdot S(z)+b(z)\cdot zS^{\prime }(z)+c(z)\cdot
      z^{2}S^{\prime \prime }(z)+d(z)\cdot z^{3}S^{(3)}(z),}]
for     a ( z ) = 6 ( 1 &#x2212; 3 z  )  3     {\displaystyle a(z)=6(1-3z)^{3}}
[{\displaystyle a(z)=6(1-3z)^{3}}],     b ( z ) = 18 ( 1 &#x2212; 3 z  )  3
{\displaystyle b(z)=18(1-3z)^{3}}  [{\displaystyle b(z)=18(1-3z)^{3}}],     c
( z ) = 9 ( 1 &#x2212; 3 z  )  3     {\displaystyle c(z)=9(1-3z)^{3}}  [
{\displaystyle c(z)=9(1-3z)^{3}}], and     d ( z ) = ( 1 &#x2212; 3 z  )  3
{\displaystyle d(z)=(1-3z)^{3}}  [{\displaystyle d(z)=(1-3z)^{3}}] where
( 1 &#x2212; 3 z  )  3   = 1 &#x2212; 9 z + 27  z  2   &#x2212; 27  z  3
{\displaystyle (1-3z)^{3}=1-9z+27z^{2}-27z^{3}}  [{\displaystyle (1-3z)^{3}=1-
9z+27z^{2}-27z^{3}}].
Finally, it follows that we may express the second sums through the first sums
in the following form:
                 s &#x007E;     n      = [  z  n   ]  (  6 ( 1 &#x2212; 3 z  )
      3    &#x2211;  n &#x2265; 0    s  n    z  n   + 18 ( 1 &#x2212; 3 z  )  3
      &#x2211;  n &#x2265; 0   n  s  n    z  n   + 9 ( 1 &#x2212; 3 z  )  3
      &#x2211;  n &#x2265; 0   n ( n &#x2212; 1 )  s  n    z  n   + ( 1
      &#x2212; 3 z  )  3    &#x2211;  n &#x2265; 0   n ( n &#x2212; 1 ) ( n
      &#x2212; 2 )  s  n    z  n    )        = ( n + 1 ) ( n + 2 ) ( n + 3 )  s
      n   &#x2212; 9 n ( n + 1 ) ( n + 2 )  s  n &#x2212; 1   + 27 ( n &#x2212;
      1 ) n ( n + 1 )  s  n &#x2212; 2   &#x2212; ( n &#x2212; 2 ) ( n &#x2212;
      1 ) n  s  n &#x2212; 3   .       {\displaystyle {\begin{aligned}
      {\widetilde {s}}_{n}&=[z^{n}]\left(6(1-3z)^{3}\sum _{n\geq 0}s_{n}z^
      {n}+18(1-3z)^{3}\sum _{n\geq 0}ns_{n}z^{n}+9(1-3z)^{3}\sum _{n\geq 0}n(n-
      1)s_{n}z^{n}+(1-3z)^{3}\sum _{n\geq 0}n(n-1)(n-2)s_{n}z^{n}\right)\\&=
      (n+1)(n+2)(n+3)s_{n}-9n(n+1)(n+2)s_{n-1}+27(n-1)n(n+1)s_{n-2}-(n-2)(n-
      1)ns_{n-3}.\end{aligned}}}  [{\displaystyle {\begin{aligned}{\widetilde
      {s}}_{n}&=[z^{n}]\left(6(1-3z)^{3}\sum _{n\geq 0}s_{n}z^{n}+18(1-3z)^
      {3}\sum _{n\geq 0}ns_{n}z^{n}+9(1-3z)^{3}\sum _{n\geq 0}n(n-1)s_{n}z^{n}+
      (1-3z)^{3}\sum _{n\geq 0}n(n-1)(n-2)s_{n}z^{n}\right)\\&=(n+1)(n+2)
      (n+3)s_{n}-9n(n+1)(n+2)s_{n-1}+27(n-1)n(n+1)s_{n-2}-(n-2)(n-1)ns_{n-
      3}.\end{aligned}}}]
*** Example 3: Generating functions for mutually recursive sequences[edit] ***
In this example, we re-formulate a generating function example given in Section
7.3 of Concrete Mathematics (see also Section 7.1 of the same reference for
pretty pictures of generating function series). In particular, suppose that we
seek the total number of ways (denoted      U  n     {\displaystyle U_{n}}  [U_
{n}]) to tile a     3 &#x00D7; n   {\displaystyle 3\times n}  [{\displaystyle
3\times n}] rectangle with unmarked     2 &#x00D7; 1   {\displaystyle 2\times
1}  [2\times 1] domino pieces. Let the auxiliary sequence,      V  n
{\displaystyle V_{n}}  [V_{n}], be defined as the number of ways to cover a
3 &#x00D7; n   {\displaystyle 3\times n}  [{\displaystyle 3\times n}]
rectangle-minus-corner section of the full rectangle. We seek to use these
definitions to give a closed_form formula for      U  n     {\displaystyle U_
{n}}  [U_{n}] without breaking down this definition further to handle the cases
of vertical versus horizontal dominoes. Notice that the ordinary generating
functions for our two sequences correspond to the series
         U ( z ) = 1 + 3  z  2   + 11  z  4   + 41  z  6   + &#x22EF;
      {\displaystyle U(z)=1+3z^{2}+11z^{4}+41z^{6}+\cdots }  [{\displaystyle U
      (z)=1+3z^{2}+11z^{4}+41z^{6}+\cdots }]
         V ( z ) = z + 4  z  3   + 15  z  5   + 56  z  7   + &#x22EF; .
      {\displaystyle V(z)=z+4z^{3}+15z^{5}+56z^{7}+\cdots .}  [{\displaystyle V
      (z)=z+4z^{3}+15z^{5}+56z^{7}+\cdots .}]
If we consider the possible configurations that can be given starting from the
left edge of the     3 &#x00D7; n   {\displaystyle 3\times n}  [{\displaystyle
3\times n}] rectangle, we are able to express the following mutually dependent,
or mutually recursive, recurrence relations for our two sequences when     n
&#x2265; 2   {\displaystyle n\geq 2}  [n\geq 2] defined as above where      U
0   = 1   {\displaystyle U_{0}=1}  [{\displaystyle U_{0}=1}],      U  1   = 0
{\displaystyle U_{1}=0}  [{\displaystyle U_{1}=0}],      V  0   = 0
{\displaystyle V_{0}=0}  [V_{0}=0], and      V  1   = 1   {\displaystyle V_
{1}=1}  [{\displaystyle V_{1}=1}]:
              U  n      = 2  V  n &#x2212; 1   +  U  n &#x2212; 2        V  n
      =  U  n &#x2212; 1   +  V  n &#x2212; 2   .       {\displaystyle {\begin
      {aligned}U_{n}&=2V_{n-1}+U_{n-2}\\V_{n}&=U_{n-1}+V_{n-2}.\end{aligned}}}
      [{\displaystyle {\begin{aligned}U_{n}&=2V_{n-1}+U_{n-2}\\V_{n}&=U_{n-
      1}+V_{n-2}.\end{aligned}}}]
Since we have that for all integers     m &#x2265; 0   {\displaystyle m\geq 0}
[m\geq 0], the index-shifted generating functions satisfy      z  m   G ( z ) =
&#x2211;  n &#x2265; m    g  n &#x2212; m    z  n     {\displaystyle z^{m}G
(z)=\sum _{n\geq m}g_{n-m}z^{n}}  [{\displaystyle z^{m}G(z)=\sum _{n\geq m}g_
{n-m}z^{n}}] (incidentally, we also have a corresponding formula when     m < 0
{\displaystyle m<0}  [m<0] given by      &#x2211;  n &#x2265; 0    g  n + m
z  n   =    G ( z ) &#x2212;  g  0   &#x2212;  g  1   z &#x2212; &#x22EF;
&#x2212;  g  m &#x2212; 1    z  m &#x2212; 1     z  m       {\displaystyle \sum
_{n\geq 0}g_{n+m}z^{n}={\frac {G(z)-g_{0}-g_{1}z-\cdots -g_{m-1}z^{m-1}}{z^
{m}}}}  [{\displaystyle \sum _{n\geq 0}g_{n+m}z^{n}={\frac {G(z)-g_{0}-g_{1}z-
\cdots -g_{m-1}z^{m-1}}{z^{m}}}}]), we can use the initial conditions specified
above and the previous two recurrence relations to see that we have the next
two equations relating the generating functions for these sequences given by
             U ( z )    = 2 z V ( z ) +  z  2   U ( z ) + 1     V ( z )    = z
      U ( z ) +  z  2   V ( z )       =   z  1 &#x2212;  z  2      U ( z ) ,
      {\displaystyle {\begin{aligned}U(z)&=2zV(z)+z^{2}U(z)+1\\V(z)&=zU(z)+z^
      {2}V(z)\\&={\frac {z}{1-z^{2}}}U(z),\end{aligned}}}  [{\displaystyle
      {\begin{aligned}U(z)&=2zV(z)+z^{2}U(z)+1\\V(z)&=zU(z)+z^{2}V(z)\\&={\frac
      {z}{1-z^{2}}}U(z),\end{aligned}}}]
which then implies by solving the system of equations (and this is the
particular trick to our method here) that
         U ( z ) =    1 &#x2212;  z  2     1 &#x2212; 4  z  2   +  z  4      =
      1  3 &#x2212;   3      &#x22C5;   1  1 &#x2212; ( 2 +   3   )  z  2
      +   1  3 +   3      &#x22C5;   1  1 &#x2212; ( 2 &#x2212;   3   )  z  2
      .   {\displaystyle U(z)={\frac {1-z^{2}}{1-4z^{2}+z^{4}}}={\frac {1}{3-
      {\sqrt {3}}}}\cdot {\frac {1}{1-(2+{\sqrt {3}})z^{2}}}+{\frac {1}{3+
      {\sqrt {3}}}}\cdot {\frac {1}{1-(2-{\sqrt {3}})z^{2}}}.}  [{\displaystyle
      U(z)={\frac {1-z^{2}}{1-4z^{2}+z^{4}}}={\frac {1}{3-{\sqrt {3}}}}\cdot
      {\frac {1}{1-(2+{\sqrt {3}})z^{2}}}+{\frac {1}{3+{\sqrt {3}}}}\cdot
      {\frac {1}{1-(2-{\sqrt {3}})z^{2}}}.}]
Thus by performing algebraic simplifications to the sequence resulting from the
second partial fractions expansions of the generating function in the previous
equation, we find that      U  2 n + 1   &#x2261; 0   {\displaystyle U_
{2n+1}\equiv 0}  [{\displaystyle U_{2n+1}\equiv 0}] and that
          U  2 n   =  &#x2308;    ( 2 +   3    )  n     3 &#x2212;   3
      &#x2309;  ,   {\displaystyle U_{2n}=\left\lceil {\frac {(2+{\sqrt {3}})^
      {n}}{3-{\sqrt {3}}}}\right\rceil ,}  [{\displaystyle U_{2n}=\left\lceil
      {\frac {(2+{\sqrt {3}})^{n}}{3-{\sqrt {3}}}}\right\rceil ,}]
for all integers     n &#x2265; 0   {\displaystyle n\geq 0}  [n\geq 0]. We also
note that the same shifted generating function technique applied to the second-
order recurrence for the Fibonacci_numbers is the prototypical example of using
generating functions to solve recurrence relations in one variable already
covered, or at least hinted at, in the subsection on rational_functions given
above.
**** Convolution (Cauchy products)[edit] ****
A discrete convolution of the terms in two formal power series turns a product
of generating functions into a generating function enumerating a convolved sum
of the original sequence terms (see Cauchy_product).
      1.Consider A(z) and B(z) are ordinary generating functions.
               C ( z ) = A ( z ) B ( z ) &#x21D4; [  z  n   ] C ( z ) =
            &#x2211;  k = 0   n     a  k    b  n &#x2212; k      {\displaystyle
            C(z)=A(z)B(z)\Leftrightarrow [z^{n}]C(z)=\sum _{k=0}^{n}{a_{k}b_{n-
            k}}}  [{\displaystyle C(z)=A(z)B(z)\Leftrightarrow [z^{n}]C(z)=\sum
            _{k=0}^{n}{a_{k}b_{n-k}}}]
      2.Consider A(z) and B(z) are exponential generating functions.
               C ( z ) = A ( z ) B ( z ) &#x21D4; [  z  n    /  n ! ] C ( z ) =
            &#x2211;  k = 0   n      (   n k   )     a  k    b  n &#x2212; k
            {\displaystyle C(z)=A(z)B(z)\Leftrightarrow [z^{n}/n!]C(z)=\sum _
            {k=0}^{n}{\binom {n}{k}}a_{k}b_{n-k}}  [{\displaystyle C(z)=A(z)B
            (z)\Leftrightarrow [z^{n}/n!]C(z)=\sum _{k=0}^{n}{\binom {n}{k}}a_
            {k}b_{n-k}}]
      3.Consider the triply convolved sequence resulting from the product of
      three ordinary generating functions
               C ( z ) = F ( z ) G ( z ) H ( z ) &#x21D4; [  z  n   ] C ( z ) =
            &#x2211;  j + k + &#x2113; = n    f  j    g  k    h  &#x2113;
            {\displaystyle C(z)=F(z)G(z)H(z)\Leftrightarrow [z^{n}]C(z)=\sum _
            {j+k+\ell =n}f_{j}g_{k}h_{\ell }}  [{\displaystyle C(z)=F(z)G(z)H
            (z)\Leftrightarrow [z^{n}]C(z)=\sum _{j+k+\ell =n}f_{j}g_{k}h_{\ell
            }}]
      4.Consider the     m   {\displaystyle m}  [m]-fold convolution of a
      sequence with itself for some positive integer     m &#x2265; 1
      {\displaystyle m\geq 1}  [{\displaystyle m\geq 1}] (see the example below
      for an application)
               C ( z ) = G ( z  )  m   &#x21D4; [  z  n   ] C ( z ) =  &#x2211;
            k  1   +  k  2   + &#x22EF; +  k  m   = n    g   k  1      g   k  2
            &#x22EF;  g   k  m       {\displaystyle C(z)=G(z)^
            {m}\Leftrightarrow [z^{n}]C(z)=\sum _{k_{1}+k_{2}+\cdots +k_
            {m}=n}g_{k_{1}}g_{k_{2}}\cdots g_{k_{m}}}  [{\displaystyle C(z)=G
            (z)^{m}\Leftrightarrow [z^{n}]C(z)=\sum _{k_{1}+k_{2}+\cdots +k_
            {m}=n}g_{k_{1}}g_{k_{2}}\cdots g_{k_{m}}}]
Multiplication of generating functions, or convolution of their underlying
sequences, can correspond to a notion of independent events in certain counting
and probability scenarios. For example, if we adopt the notational convention
that the probability_generating_function, or pgf, of a random variable     Z
{\displaystyle Z}  [Z] is denoted by      G  Z   ( z )   {\displaystyle G_{Z}
(z)}  [{\displaystyle G_{Z}(z)}], then we can show that for any two random
variables [22]
          G  X + Y   ( z ) =  G  X   ( z )  G  Y   ( z ) ,   {\displaystyle G_
      {X+Y}(z)=G_{X}(z)G_{Y}(z),}  [{\displaystyle G_{X+Y}(z)=G_{X}(z)G_{Y}
      (z),}]
if     X   {\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y] are
independent. Similarly, the number of ways to pay     n &#x2265; 0
{\displaystyle n\geq 0}  [n\geq 0] cents in coin denominations of values in the
set     { 1 , 5 , 10 , 25 , 50 }   {\displaystyle \{1,5,10,25,50\}}  [
{\displaystyle \{1,5,10,25,50\}}] (i.e., in pennies, nickels, dimes, quarters,
and half dollars, respectively) is generated by the product
         C ( z ) =   1  1 &#x2212; z      1  1 &#x2212;  z  5        1  1
      &#x2212;  z  10        1  1 &#x2212;  z  25        1  1 &#x2212;  z  50
      ,   {\displaystyle C(z)={\frac {1}{1-z}}{\frac {1}{1-z^{5}}}{\frac {1}{1-
      z^{10}}}{\frac {1}{1-z^{25}}}{\frac {1}{1-z^{50}}},}  [{\displaystyle C
      (z)={\frac {1}{1-z}}{\frac {1}{1-z^{5}}}{\frac {1}{1-z^{10}}}{\frac {1}
      {1-z^{25}}}{\frac {1}{1-z^{50}}},}]
and moreover, if we allow the     n   {\displaystyle n}  [n] cents to be paid
in coins of any positive integer denomination, we arrive at the generating for
the number of such combinations of change being generated by the partition
function generating function expanded by the infinite q-Pochhammer_symbol
product of      &#x220F;  n &#x2265; 1   ( 1 &#x2212;  z  n    )  &#x2212; 1
{\displaystyle \prod _{n\geq 1}(1-z^{n})^{-1}}  [{\displaystyle \prod _{n\geq
1}(1-z^{n})^{-1}}].
*** Example: The generating function for the Catalan numbers[edit] ***
An example where convolutions of generating functions are useful allows us to
solve for a specific closed-form function representing the ordinary generating
function for the Catalan_numbers,      C  n     {\displaystyle C_{n}}  [C_{n}].
In particular, this sequence has the combinatorial interpretation as being the
number of ways to insert parentheses into the product      x  0   &#x22C5;  x
1   &#x22EF;  x  n     {\displaystyle x_{0}\cdot x_{1}\cdots x_{n}}  [
{\displaystyle x_{0}\cdot x_{1}\cdots x_{n}}] so that the order of
multiplication is completely specified. For example,      C  2   = 2
{\displaystyle C_{2}=2}  [{\displaystyle C_{2}=2}] which corresponds to the two
expressions      x  0   &#x22C5; (  x  1   &#x22C5;  x  2   )   {\displaystyle
x_{0}\cdot (x_{1}\cdot x_{2})}  [{\displaystyle x_{0}\cdot (x_{1}\cdot x_{2})}]
and     (  x  0   &#x22C5;  x  1   ) &#x22C5;  x  2     {\displaystyle (x_
{0}\cdot x_{1})\cdot x_{2}}  [{\displaystyle (x_{0}\cdot x_{1})\cdot x_{2}}].
It follows that the sequence satisfies a recurrence relation given by
          C  n   =  &#x2211;  k = 0   n &#x2212; 1    C  k    C  n &#x2212; 1
      &#x2212; k   +  &#x03B4;  n , 0   =  C  0    C  n &#x2212; 1   +  C  1
      C  n &#x2212; 2   + &#x22EF; +  C  n &#x2212; 1    C  0   +  &#x03B4;  n
      , 0   , &#xA0; n &#x2265; 0 ,   {\displaystyle C_{n}=\sum _{k=0}^{n-1}C_
      {k}C_{n-1-k}+\delta _{n,0}=C_{0}C_{n-1}+C_{1}C_{n-2}+\cdots +C_{n-1}C_
      {0}+\delta _{n,0},\ n\geq 0,}  [{\displaystyle C_{n}=\sum _{k=0}^{n-1}C_
      {k}C_{n-1-k}+\delta _{n,0}=C_{0}C_{n-1}+C_{1}C_{n-2}+\cdots +C_{n-1}C_
      {0}+\delta _{n,0},\ n\geq 0,}]
and so has a corresponding convolved generating function,     C ( z )
{\displaystyle C(z)}  [C(z)], satisfying
         C ( z ) = z &#x22C5; C ( z  )  2   + 1.   {\displaystyle C(z)=z\cdot C
      (z)^{2}+1.}  [{\displaystyle C(z)=z\cdot C(z)^{2}+1.}]
Since     C ( 0 ) = 1 &#x2260; &#x221E;   {\displaystyle C(0)=1\neq \infty }  [
{\displaystyle C(0)=1\neq \infty }], we then arrive at a formula for this
generating function given by
             C ( z )    =    1 &#x2212;   1 &#x2212; 4 z     2 z          =
      &#x2211;  n &#x2265; 0     1  n + 1       (    2 n  n   )     z  n   .
      {\displaystyle {\begin{aligned}C(z)&={\frac {1-{\sqrt {1-4z}}}
      {2z}}\\&=\sum _{n\geq 0}{\frac {1}{n+1}}{\binom {2n}{n}}z^{n}.\end
      {aligned}}}  [{\displaystyle {\begin{aligned}C(z)&={\frac {1-{\sqrt {1-
      4z}}}{2z}}\\&=\sum _{n\geq 0}{\frac {1}{n+1}}{\binom {2n}{n}}z^{n}.\end
      {aligned}}}]
Note that the first equation implicitly defining     C ( z )   {\displaystyle C
(z)}  [C(z)] above implies that
         C ( z ) =   1  1 &#x2212; z &#x22C5; C ( z )    ,   {\displaystyle C
      (z)={\frac {1}{1-z\cdot C(z)}},}  [{\displaystyle C(z)={\frac {1}{1-
      z\cdot C(z)}},}]
which then leads to another "simple" (as in of form) continued fraction
expansion of this generating function.
*** Example: Spanning trees of fans and convolutions of convolutions[edit] ***
A fan of order     n   {\displaystyle n}  [n] is defined to be a graph on the
vertices     { 0 , 1 , &#x2026; , n }   {\displaystyle \{0,1,\ldots ,n\}}  [
{\displaystyle \{0,1,\ldots ,n\}}] with     2 n &#x2212; 1   {\displaystyle 2n-
1}  [2n-1] edges connected according to the following rules: Vertex     0
{\displaystyle 0}  [{\displaystyle 0}] is connected by a single edge to each of
the other     n   {\displaystyle n}  [n] vertices, and vertex     k
{\displaystyle k}  [k] is connected by a single edge to the next vertex     k +
1   {\displaystyle k+1}  [k+1] for all     1 &#x2264; k < n   {\displaystyle
1\leq k<n}  [1 \leq k < n].[23] There is one fan of order one, three fans of
order two, eight fans of order three, and so on. A spanning_tree is a subgraph
of a graph which contains all of the original vertices and which contains
enough edges to make this subgraph connected, but not so many edges that there
is a cycle in the subgraph. We ask how many spanning trees      f  n
{\displaystyle f_{n}}  [f_{n}] of a fan of order     n   {\displaystyle n}  [n]
are possible for each     n &#x2265; 1   {\displaystyle n\geq 1}  [n\geq 1].
As an observation, we may approach the question by counting the number of ways
to join adjacent sets of vertices. For example, when     n = 4   {\displaystyle
n=4}  [n=4], we have that      f  4   = 4 + 3 &#x22C5; 1 + 2 &#x22C5; 2 + 1
&#x22C5; 3 + 2 &#x22C5; 1 &#x22C5; 1 + 1 &#x22C5; 2 &#x22C5; 1 + 1 &#x22C5; 1
&#x22C5; 2 + 1 &#x22C5; 1 &#x22C5; 1 &#x22C5; 1 &#x22C5; 1 = 21
{\displaystyle f_{4}=4+3\cdot 1+2\cdot 2+1\cdot 3+2\cdot 1\cdot 1+1\cdot 2\cdot
1+1\cdot 1\cdot 2+1\cdot 1\cdot 1\cdot 1\cdot 1=21}  [{\displaystyle f_
{4}=4+3\cdot 1+2\cdot 2+1\cdot 3+2\cdot 1\cdot 1+1\cdot 2\cdot 1+1\cdot 1\cdot
2+1\cdot 1\cdot 1\cdot 1\cdot 1=21}], which is a sum over the     m
{\displaystyle m}  [m]-fold convolutions of the sequence      g  n   = n = [  z
n   ] z  /  ( 1 &#x2212; z  )  2     {\displaystyle g_{n}=n=[z^{n}]z/(1-z)^{2}}
[{\displaystyle g_{n}=n=[z^{n}]z/(1-z)^{2}}] for     m := 1 , 2 , 3 , 4
{\displaystyle m:=1,2,3,4}  [{\displaystyle m:=1,2,3,4}]. More generally, we
may write a formula for this sequence as
          f  n   =  &#x2211;  m > 0    &#x2211;     k  1   +  k  2   + &#x22EF;
      +  k  m   = n    k  1   ,  k  2   , &#x2026; ,  k  m   > 0      g   k  1
      g   k  2     &#x22EF;  g   k  m     ,   {\displaystyle f_{n}=\sum _
      {m>0}\sum _{\scriptstyle k_{1}+k_{2}+\cdots +k_{m}=n \atop \scriptstyle
      k_{1},k_{2},\ldots ,k_{m}>0}g_{k_{1}}g_{k_{2}}\cdots g_{k_{m}},}  [
      {\displaystyle f_{n}=\sum _{m>0}\sum _{\scriptstyle k_{1}+k_{2}+\cdots
      +k_{m}=n \atop \scriptstyle k_{1},k_{2},\ldots ,k_{m}>0}g_{k_{1}}g_{k_
      {2}}\cdots g_{k_{m}},}]
from which we see that the ordinary generating function for this sequence is
given by the next sum of convolutions as
             F ( z )    = G ( z ) + G ( z  )  2   + G ( z  )  3   + &#x22EF;
      =    G ( z )   1 &#x2212; G ( z )          =   z  ( 1 &#x2212; z  )  2
      &#x2212; z    =   z  1 &#x2212; 3 z +  z  2      ,       {\displaystyle
      {\begin{aligned}F(z)&=G(z)+G(z)^{2}+G(z)^{3}+\cdots \\[6pt]&={\frac {G
      (z)}{1-G(z)}}\\[6pt]&={\frac {z}{(1-z)^{2}-z}}={\frac {z}{1-3z+z^
      {2}}},\end{aligned}}}  [{\displaystyle {\begin{aligned}F(z)&=G(z)+G(z)^
      {2}+G(z)^{3}+\cdots \\[6pt]&={\frac {G(z)}{1-G(z)}}\\[6pt]&={\frac {z}{
      (1-z)^{2}-z}}={\frac {z}{1-3z+z^{2}}},\end{aligned}}}]
from which we are able to extract an exact formula for the sequence by taking
the partial_fraction_expansion of the last generating function.
**** Implicit generating functions and the Lagrange inversion formula[edit]
****
         This section needs expansion with: This section needs to be added to
[[icon]] the list of techniques with generating functions. You can help by
         adding_to_it. (April 2017)
**** Introducing a free parameter (snake oil method)[edit] ****
Sometimes the sum      s  n     {\displaystyle s_{n}}  [s_{n}] is complicated,
and it is not always easy to evaluate. The "Free Parameter" method is another
method (called "snake oil" by H. Wilf) to evaluate these sums.
Both methods discussed so far have     n   {\displaystyle n}  [n] as limit in
the summation. When n does not appear explicitly in the summation, we may
consider     n   {\displaystyle n}  [n] as a âfreeâ parameter and treat
s  n     {\displaystyle s_{n}}  [s_{n}] as a coefficient of     F ( z ) =
&#x2211;   s  n    z  n      {\displaystyle F(z)=\sum {s_{n}z^{n}}}  [F(z)=\sum
{s_{n}z^{n}}], change the order of the summations on     n   {\displaystyle n}
[n] and     k   {\displaystyle k}  [k], and try to compute the inner sum.
For example, if we want to compute
          s  n   =  &#x2211;  k &#x2265; 0       (    n + k   m + 2 k    )
      (    2 k  k   )       ( &#x2212; 1  )  k     k + 1      ( m , n &#x2208;
      N   0   )   {\displaystyle s_{n}=\sum _{k\geq 0}{{\binom {n+k}{m+2k}}
      {\binom {2k}{k}}{\frac {(-1)^{k}}{k+1}}}\quad (m,n\in \mathbb {N} _{0})}
      [s_{n}=\sum _{{k\geq 0}}{{\binom  {n+k}{m+2k}}{\binom  {2k}{k}}{\frac  {
      (-1)^{k}}{k+1}}}\quad (m,n\in {\mathbb  {N}}_{0})]
we can treat     n   {\displaystyle n}  [n] as a "free" parameter, and set
         F ( z ) =  &#x2211;  n &#x2265; 0     [   &#x2211;  k &#x2265; 0
      (    n + k   m + 2 k    )       (    2 k  k   )       ( &#x2212; 1  )  k
      k + 1      ]    z  n     {\displaystyle F(z)=\sum _{n\geq 0}{\left[\sum _
      {k\geq 0}{{\binom {n+k}{m+2k}}{\binom {2k}{k}}{\frac {(-1)^{k}}
      {k+1}}}\right]}z^{n}}  [F(z)=\sum _{{n\geq 0}}{\left[\sum _{{k\geq 0}}{
      {\binom  {n+k}{m+2k}}{\binom  {2k}{k}}{\frac  {(-1)^{k}}{k+1}}}\right]}z^
      {n}]
Interchanging summation (âsnake oilâ) gives
         F ( z ) =  &#x2211;  k &#x2265; 0       (    2 k  k   )
      ( &#x2212; 1  )  k     k + 1     z  &#x2212; k     &#x2211;  n &#x2265; 0
      (    n + k   m + 2 k    )     z  n + k      {\displaystyle F(z)=\sum _
      {k\geq 0}{{\binom {2k}{k}}{\frac {(-1)^{k}}{k+1}}z^{-k}}\sum _{n\geq 0}{
      {\binom {n+k}{m+2k}}z^{n+k}}}  [F(z)=\sum _{{k\geq 0}}{{\binom  {2k}{k}}
      {\frac  {(-1)^{k}}{k+1}}z^{{-k}}}\sum _{{n\geq 0}}{{\binom  {n+k}
      {m+2k}}z^{{n+k}}}]
Now the inner sum is        z  m + 2 k    ( 1 &#x2212; z  )  m + 2 k + 1
{\displaystyle {\frac {z^{m+2k}}{(1-z)^{m+2k+1}}}}  [{\frac  {z^{{m+2k}}}{(1-
z)^{{m+2k+1}}}}]. Thus
             F ( z )    =    z  m    ( 1 &#x2212; z  )  m + 1       &#x2211;  k
      &#x2265; 0      1  k + 1       (    2 k  k   )    (    &#x2212; z   ( 1
      &#x2212; z  )  2       )  k          =    z  m    ( 1 &#x2212; z  )  m +
      1       &#x2211;  k &#x2265; 0     C  k   (    &#x2212; z   ( 1 &#x2212;
      z  )  2       )  k      (where&#xA0;   C  k   =  k  th    &#xA0;Catalan
      number)        =    z  m    ( 1 &#x2212; z  )  m + 1         1 &#x2212;
      1 +    4 z   ( 1 &#x2212; z  )  2           &#x2212; 2 z   ( 1 &#x2212; z
      )  2             =    &#x2212;  z  m &#x2212; 1     2 ( 1 &#x2212; z  )
      m &#x2212; 1      ( 1 &#x2212;    1 + z   1 &#x2212; z    )       =    z
      m    ( 1 &#x2212; z  )  m      = z    z  m &#x2212; 1    ( 1 &#x2212; z
      )  m      .       {\displaystyle {\begin{aligned}F(z)&={\frac {z^{m}}{(1-
      z)^{m+1}}}\sum _{k\geq 0}{{\frac {1}{k+1}}{\binom {2k}{k}}({\frac {-z}{
      (1-z)^{2}}})^{k}}\\&={\frac {z^{m}}{(1-z)^{m+1}}}\sum _{k\geq 0}{C_{k}(
      {\frac {-z}{(1-z)^{2}}})^{k}}\quad {\text{(where }}C_{k}=k^{\text{th}}
      {\text{ Catalan number)}}\\&={\frac {z^{m}}{(1-z)^{m+1}}}{\frac {1-{\sqrt
      {1+{\frac {4z}{(1-z)^{2}}}}}}{\frac {-2z}{(1-z)^{2}}}}\\&={\frac {-z^{m-
      1}}{2(1-z)^{m-1}}}(1-{\frac {1+z}{1-z}})\\&={\frac {z^{m}}{(1-z)^{m}}}=z
      {\frac {z^{m-1}}{(1-z)^{m}}}.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}F(z)&={\frac {z^{m}}{(1-z)^{m+1}}}\sum _{k\geq 0}{{\frac {1}
      {k+1}}{\binom {2k}{k}}({\frac {-z}{(1-z)^{2}}})^{k}}\\&={\frac {z^{m}}{
      (1-z)^{m+1}}}\sum _{k\geq 0}{C_{k}({\frac {-z}{(1-z)^{2}}})^{k}}\quad
      {\text{(where }}C_{k}=k^{\text{th}}{\text{ Catalan number)}}\\&={\frac
      {z^{m}}{(1-z)^{m+1}}}{\frac {1-{\sqrt {1+{\frac {4z}{(1-z)^{2}}}}}}{\frac
      {-2z}{(1-z)^{2}}}}\\&={\frac {-z^{m-1}}{2(1-z)^{m-1}}}(1-{\frac {1+z}{1-
      z}})\\&={\frac {z^{m}}{(1-z)^{m}}}=z{\frac {z^{m-1}}{(1-z)^{m}}}.\end
      {aligned}}}]
Then we obtain
          s  n   =    (    n &#x2212; 1   m &#x2212; 1    )
      &#xA0;for&#xA0;   m &#x2265; 1  ,   s  n   = [ n = 0 ]   &#xA0;for&#xA0;
      m = 0.   {\displaystyle s_{n}={\binom {n-1}{m-1}}\quad {\text{ for
      }}\quad m\geq 1\quad ,\quad s_{n}=[n=0]\quad {\text{ for }}\quad m=0.}  [
      {\displaystyle s_{n}={\binom {n-1}{m-1}}\quad {\text{ for }}\quad m\geq
      1\quad ,\quad s_{n}=[n=0]\quad {\text{ for }}\quad m=0.}]
**** Generating functions prove congruences[edit] ****
We say that two generating functions (power series) are congruent modulo     m
{\displaystyle m}  [m], written     A ( z ) &#x2261; B ( z )   ( mod  m )
{\displaystyle A(z)\equiv B(z){\pmod {m}}}  [{\displaystyle A(z)\equiv B(z)
{\pmod {m}}}] if their coefficients are congruent modulo     m   {\displaystyle
m}  [m] for all     n &#x2265; 0   {\displaystyle n\geq 0}  [n\geq 0], i.e.,
a  n   &#x2261;  b  n     ( mod  m )    {\displaystyle a_{n}\equiv b_{n}{\pmod
{m}}}  [{\displaystyle a_{n}\equiv b_{n}{\pmod {m}}}] for all relevant cases of
the integers     n   {\displaystyle n}  [n] (note that we need not assume that
m   {\displaystyle m}  [m] is an integer hereâit may very well be polynomial-
valued in some indeterminate     x   {\displaystyle x}  [x], for example). If
the "simpler" right-hand-side generating function,     B ( z )   {\displaystyle
B(z)}  [B(z)], is a rational function of     z   {\displaystyle z}  [z], then
the form of this sequences suggests that the sequence is eventually_periodic
modulo fixed particular cases of integer-valued     m &#x2265; 2
{\displaystyle m\geq 2}  [m \geq 2]. For example, we can prove that the Euler
numbers,     &#x27E8;  E  n   &#x27E9; = &#x27E8; 1 , 1 , 5 , 61 , 1385 ,
&#x2026; &#x27E9; &#x27FC; &#x27E8; 1 , 1 , 2 , 1 , 2 , 1 , 2 , &#x2026;
&#x27E9;   ( mod  3 )    {\displaystyle \langle E_{n}\rangle =\langle
1,1,5,61,1385,\ldots \rangle \longmapsto \langle 1,1,2,1,2,1,2,\ldots \rangle
{\pmod {3}}}  [{\displaystyle \langle E_{n}\rangle =\langle
1,1,5,61,1385,\ldots \rangle \longmapsto \langle 1,1,2,1,2,1,2,\ldots \rangle
{\pmod {3}}}], satisfy the following congruence modulo     3   {\displaystyle
3}  [3]:[24]
          &#x2211;  n &#x2265; 0    E  n    z  n   =    1 &#x2212;  z  2     1
      +  z  2        ( mod  3 )  .   {\displaystyle \sum _{n\geq 0}E_{n}z^{n}=
      {\frac {1-z^{2}}{1+z^{2}}}{\pmod {3}}.}  [{\displaystyle \sum _{n\geq
      0}E_{n}z^{n}={\frac {1-z^{2}}{1+z^{2}}}{\pmod {3}}.}]
One of the most useful, if not downright powerful, methods of obtaining
congruences for sequences enumerated by special generating functions modulo any
integers (i.e., not only prime powers      p  k     {\displaystyle p^{k}}  [p^
{k}]) is given in the section on continued fraction representations of (even
non-convergent) ordinary generating functions by J-fractions above. We cite one
particular result related to generating series expanded through a
representation by continued fraction from Lando's Lectures on Generating
Functions as follows:
            Theorem: (Congruences for Series Generated by Expansions of
            Continued Fractions) Suppose that the generating function     A ( z
            )   {\displaystyle A(z)}  [A(z)] is represented by an infinite
            continued_fraction of the form
               A ( z ) =   1  1 &#x2212;  c  1   z        p  1    z  2     1
            &#x2212;  c  2   z        p  2    z  2     1 &#x2212;  c  3   z
            &#x22EF; ,   {\displaystyle A(z)={\frac {1}{1-c_{1}z}}{\frac {p_
            {1}z^{2}}{1-c_{2}z}}{\frac {p_{2}z^{2}}{1-c_{3}z}}\cdots ,}  [
            {\displaystyle A(z)={\frac {1}{1-c_{1}z}}{\frac {p_{1}z^{2}}{1-c_
            {2}z}}{\frac {p_{2}z^{2}}{1-c_{3}z}}\cdots ,}]
            and that      A  p   ( z )   {\displaystyle A_{p}(z)}  [
            {\displaystyle A_{p}(z)}] denotes the      p  t h
            {\displaystyle p^{th}}  [p^{{th}}] convergent to this continued
            fraction expansion defined such that      a  n   = [  z  n   ]  A
            p   ( z )   {\displaystyle a_{n}=[z^{n}]A_{p}(z)}  [{\displaystyle
            a_{n}=[z^{n}]A_{p}(z)}] for all     0 &#x2264; n < 2 p
            {\displaystyle 0\leq n<2p}  [{\displaystyle 0\leq n<2p}]. Then 1)
            the function      A  p   ( z )   {\displaystyle A_{p}(z)}  [
            {\displaystyle A_{p}(z)}] is rational for all     p &#x2265; 2
            {\displaystyle p\geq 2}  [{\displaystyle p\geq 2}] where we assume
            that one of divisibility criteria of     p  |   p  1   ,  p  1    p
            2   ,  p  1    p  2    p  3   &#x22EF;   {\displaystyle p|p_{1},p_
            {1}p_{2},p_{1}p_{2}p_{3}\cdots }  [{\displaystyle p|p_{1},p_{1}p_
            {2},p_{1}p_{2}p_{3}\cdots }] is met, i.e.,     p  |   p  1    p  2
            &#x22EF;  p  k     {\displaystyle p|p_{1}p_{2}\cdots p_{k}}  [
            {\displaystyle p|p_{1}p_{2}\cdots p_{k}}] for some     k &#x2265; 1
            {\displaystyle k\geq 1}  [k\geq 1]; and 2) If the integer     p
            {\displaystyle p}  [p] divides the product      p  1    p  2
            &#x22EF;  p  k     {\displaystyle p_{1}p_{2}\cdots p_{k}}  [
            {\displaystyle p_{1}p_{2}\cdots p_{k}}], then we have that     A
            ( z ) &#x2261;  A  k   ( z )   ( mod  p )    {\displaystyle A
            (z)\equiv A_{k}(z){\pmod {p}}}  [{\displaystyle A(z)\equiv A_{k}(z)
            {\pmod {p}}}].
Generating functions also have other uses in proving congruences for their
coefficients. We cite the next two specific examples deriving special case
congruences for the Stirling_numbers_of_the_first_kind and for the partition
function_(mathematics)     p ( n )   {\displaystyle p(n)}  [p(n)] which show
the versatility of generating functions in tackling problems involving integer
sequences.
*** The Stirling numbers modulo small integers[edit] ***
The main_article on the Stirling numbers generated by the finite products
          S  n   ( x ) :=  &#x2211;  k = 0   n    [     n     k     ]   x  k
      = x ( x + 1 ) ( x + 2 ) &#x22EF; ( x + n &#x2212; 1 ) , &#xA0; n &#x2265;
      1 ,   {\displaystyle S_{n}(x):=\sum _{k=0}^{n}\left[{\begin
      {matrix}n\\k\end{matrix}}\right]x^{k}=x(x+1)(x+2)\cdots (x+n-1),\ n\geq
      1,}  [{\displaystyle S_{n}(x):=\sum _{k=0}^{n}\left[{\begin
      {matrix}n\\k\end{matrix}}\right]x^{k}=x(x+1)(x+2)\cdots (x+n-1),\ n\geq
      1,}]
provides an overview of the congruences for these numbers derived strictly from
properties of their generating function as in Section 4.6 of Wilf's stock
reference Generatingfunctionology. We repeat the basic argument and notice that
when reduces modulo     2   {\displaystyle 2}  [2], these finite product
generating functions each satisfy
          S  n   ( x ) = [ x ( x + 1 ) ] &#x22C5; [ x ( x + 1 ) ] &#x22EF; =  x
      &#x2308; n  /  2 &#x2309;   ( x + 1  )  &#x230A; n  /  2 &#x230B;   ,
      {\displaystyle S_{n}(x)=[x(x+1)]\cdot [x(x+1)]\cdots =x^{\lceil n/2\rceil
      }(x+1)^{\lfloor n/2\rfloor },}  [{\displaystyle S_{n}(x)=[x(x+1)]\cdot [x
      (x+1)]\cdots =x^{\lceil n/2\rceil }(x+1)^{\lfloor n/2\rfloor },}]
which implies that the parity of these Stirling_numbers matches that of the
binomial coefficient
          [     n     k     ]  &#x2261;    (    &#x230A; n  /  2 &#x230B;   k
      &#x2212; &#x2308; n  /  2 &#x2309;    )      ( mod  2 )  ,
      {\displaystyle \left[{\begin{matrix}n\\k\end{matrix}}\right]\equiv
      {\binom {\lfloor n/2\rfloor }{k-\lceil n/2\rceil }}{\pmod {2}},}  [
      {\displaystyle \left[{\begin{matrix}n\\k\end{matrix}}\right]\equiv
      {\binom {\lfloor n/2\rfloor }{k-\lceil n/2\rceil }}{\pmod {2}},}]
and consequently shows that      [     n     k     ]    {\displaystyle \left[
{\begin{matrix}n\\k\end{matrix}}\right]}  [{\displaystyle \left[{\begin
{matrix}n\\k\end{matrix}}\right]}] is even whenever     k <  &#x2308;   n 2
&#x2309;    {\displaystyle k<\left\lceil {\frac {n}{2}}\right\rceil }  [
{\displaystyle k<\left\lceil {\frac {n}{2}}\right\rceil }].
Similarly, we can reduce the right-hand-side products defining the Stirling
number generating functions modulo     3   {\displaystyle 3}  [3] to obtain
slightly more complicated expressions providing that
              [     n     m     ]     &#x2261; [  x  m   ]  (   x  &#x2308; n
      /  3 &#x2309;   ( x + 1  )  &#x2308; ( n &#x2212; 1 )  /  3 &#x2309;
      ( x + 2  )  &#x230A; n  /  3 &#x230B;    )       ( mod  3 )
      &#x2261;  &#x2211;  k = 0   m      (    &#x2308; ( n &#x2212; 1 )  /  3
      &#x2309;  k   )       (    &#x230A; n  /  3 &#x230B;   m &#x2212; k
      &#x2212; &#x2308; n  /  3 &#x2309;    )    &#x00D7;  2  &#x2308; n  /  3
      &#x2309; + &#x230A; n  /  3 &#x230B; &#x2212; ( m &#x2212; k )
      ( mod  3 )  .       {\displaystyle {\begin{aligned}\left[{\begin
      {matrix}n\\m\end{matrix}}\right]&\equiv [x^{m}]\left(x^{\lceil n/3\rceil
      }(x+1)^{\lceil (n-1)/3\rceil }(x+2)^{\lfloor n/3\rfloor }\right)&&{\pmod
      {3}}\\&\equiv \sum _{k=0}^{m}{\binom {\lceil (n-1)/3\rceil }{k}}{\binom
      {\lfloor n/3\rfloor }{m-k-\lceil n/3\rceil }}\times 2^{\lceil n/3\rceil
      +\lfloor n/3\rfloor -(m-k)}&&{\pmod {3}}.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}\left[{\begin{matrix}n\\m\end{matrix}}\right]&\equiv [x^
      {m}]\left(x^{\lceil n/3\rceil }(x+1)^{\lceil (n-1)/3\rceil }(x+2)^
      {\lfloor n/3\rfloor }\right)&&{\pmod {3}}\\&\equiv \sum _{k=0}^{m}{\binom
      {\lceil (n-1)/3\rceil }{k}}{\binom {\lfloor n/3\rfloor }{m-k-\lceil n/
      3\rceil }}\times 2^{\lceil n/3\rceil +\lfloor n/3\rfloor -(m-k)}&&{\pmod
      {3}}.\end{aligned}}}]
*** Congruences for the partition function[edit] ***
In this example, we pull in some of the machinery of infinite products whose
power series expansions generate the expansions of many special functions and
enumerate partition functions. In particular, we recall that the partition
function     p ( n )   {\displaystyle p(n)}  [p(n)] is generated by the
reciprocal infinite q-Pochhammer_symbol product (or z-Pochhammer product as the
case may be) given by
              &#x2211;  n &#x2265; 1   p ( n )  z  n      =   1  ( 1 &#x2212; z
      ) ( 1 &#x2212;  z  2   ) ( 1 &#x2212;  z  3   ) &#x22EF;          = 1 + z
      + 2  z  2   + 3  z  3   + 5  z  4   + 7  z  5   + 11  z  6   + &#x22EF; .
      {\displaystyle {\begin{aligned}\sum _{n\geq 1}p(n)z^{n}&={\frac {1}{(1-z)
      (1-z^{2})(1-z^{3})\cdots }}\\[4pt]&=1+z+2z^{2}+3z^{3}+5z^{4}+7z^{5}+11z^
      {6}+\cdots .\end{aligned}}}  [{\displaystyle {\begin{aligned}\sum _{n\geq
      1}p(n)z^{n}&={\frac {1}{(1-z)(1-z^{2})(1-z^{3})\cdots }}\\[4pt]&=1+z+2z^
      {2}+3z^{3}+5z^{4}+7z^{5}+11z^{6}+\cdots .\end{aligned}}}]
This partition function satisfies many known congruence_properties, which
notably include the following results though there are still many open
questions about the forms of related integer congruences for the function:[25]
             p ( 5 m + 4 )    &#x2261; 0   ( mod  5 )      p ( 7 m + 5 )
      &#x2261; 0   ( mod  7 )      p ( 11 m + 4 )    &#x2261; 0   ( mod  11 )
      p ( 25 m + 24 )    &#x2261; 0   ( mod   5  2   )  .       {\displaystyle
      {\begin{aligned}p(5m+4)&\equiv 0{\pmod {5}}\\p(7m+5)&\equiv 0{\pmod
      {7}}\\p(11m+4)&\equiv 0{\pmod {11}}\\p(25m+24)&\equiv 0{\pmod {5^
      {2}}}.\end{aligned}}}  [{\displaystyle {\begin{aligned}p(5m+4)&\equiv 0
      {\pmod {5}}\\p(7m+5)&\equiv 0{\pmod {7}}\\p(11m+4)&\equiv 0{\pmod
      {11}}\\p(25m+24)&\equiv 0{\pmod {5^{2}}}.\end{aligned}}}]
We show how to use generating functions and manipulations of congruences for
formal power series to give a highly elementary proof of the first of these
congruences listed above.
First, we observe that the binomial coefficient generating function,     1  /
( 1 &#x2212; z  )  5     {\displaystyle 1/(1-z)^{5}}  [{\displaystyle 1/(1-z)^
{5}}], satisfies that each of its coefficients are divisible by     5
{\displaystyle 5}  [5] with the exception of those which correspond to the
powers of     1 ,  z  5   ,  z  10   , &#x2026;   {\displaystyle 1,z^{5},z^
{10},\ldots }  [{\displaystyle 1,z^{5},z^{10},\ldots }], all of which otherwise
have a remainder of     1   {\displaystyle 1}  [1] modulo     5
{\displaystyle 5}  [5]. Thus we may write
           1  ( 1 &#x2212; z  )  5      &#x2261;   1  1 &#x2212;  z  5
      ( mod  5 )    &#x27FA;      1 &#x2212;  z  5     ( 1 &#x2212; z  )  5
      &#x2261; 1   ( mod  5 )  ,   {\displaystyle {\frac {1}{(1-z)^{5}}}\equiv
      {\frac {1}{1-z^{5}}}{\pmod {5}}\qquad \iff \qquad {\frac {1-z^{5}}{(1-z)^
      {5}}}\equiv 1{\pmod {5}},}  [{\displaystyle {\frac {1}{(1-z)^{5}}}\equiv
      {\frac {1}{1-z^{5}}}{\pmod {5}}\qquad \iff \qquad {\frac {1-z^{5}}{(1-z)^
      {5}}}\equiv 1{\pmod {5}},}]
which in particular shows us that
            ( 1 &#x2212;  z  5   ) ( 1 &#x2212;  z  10   ) ( 1 &#x2212;  z  15
      ) &#x22EF;    {  ( 1 &#x2212; z ) ( 1 &#x2212;  z  2   ) ( 1 &#x2212;  z
      3   ) &#x22EF;  }   5     &#x2261; 1   ( mod  5 )  .   {\displaystyle
      {\frac {(1-z^{5})(1-z^{10})(1-z^{15})\cdots }{\left\{(1-z)(1-z^{2})(1-z^
      {3})\cdots \right\}^{5}}}\equiv 1{\pmod {5}}.}  [{\displaystyle {\frac {
      (1-z^{5})(1-z^{10})(1-z^{15})\cdots }{\left\{(1-z)(1-z^{2})(1-z^
      {3})\cdots \right\}^{5}}}\equiv 1{\pmod {5}}.}]
Hence, we easily see that     5   {\displaystyle 5}  [5] divides each
coefficient of      z  5 m + 1     {\displaystyle z^{5m+1}}  [{\displaystyle z^
{5m+1}}] in the infinite product expansions of
         z &#x22C5;    ( 1 &#x2212;  z  5   ) ( 1 &#x2212;  z  10   ) &#x22EF;
      ( 1 &#x2212; z ) ( 1 &#x2212;  z  2   ) &#x22EF;    = z &#x22C5;   {  ( 1
      &#x2212; z ) ( 1 &#x2212;  z  2   ) &#x22EF;  }   4   &#x00D7;    ( 1
      &#x2212;  z  5   ) ( 1 &#x2212;  z  10   ) &#x22EF;    {  ( 1 &#x2212; z
      ) ( 1 &#x2212;  z  2   ) &#x22EF;  }   5     .   {\displaystyle z\cdot
      {\frac {(1-z^{5})(1-z^{10})\cdots }{(1-z)(1-z^{2})\cdots }}=z\cdot \left\
      {(1-z)(1-z^{2})\cdots \right\}^{4}\times {\frac {(1-z^{5})(1-z^
      {10})\cdots }{\left\{(1-z)(1-z^{2})\cdots \right\}^{5}}}.}  [
      {\displaystyle z\cdot {\frac {(1-z^{5})(1-z^{10})\cdots }{(1-z)(1-z^
      {2})\cdots }}=z\cdot \left\{(1-z)(1-z^{2})\cdots \right\}^{4}\times
      {\frac {(1-z^{5})(1-z^{10})\cdots }{\left\{(1-z)(1-z^{2})\cdots \right\}^
      {5}}}.}]
Finally, since we may write the generating function for the partition function
as
                z  ( 1 &#x2212; z ) ( 1 &#x2212;  z  2   ) &#x22EF;        =
      z &#x22C5;    ( 1 &#x2212;  z  5   ) ( 1 &#x2212;  z  10   ) &#x22EF;
      ( 1 &#x2212; z ) ( 1 &#x2212;  z  2   ) &#x22EF;    &#x00D7; ( 1 +  z  5
      +  z  10   + &#x22EF; ) ( 1 +  z  10   +  z  20   + &#x22EF; ) &#x22EF;
      =     z +  &#x2211;  n &#x2265; 2   p ( n &#x2212; 1 )  z  n   ,
      {\displaystyle {\begin{aligned}&{\frac {z}{(1-z)(1-z^{2})\cdots }}\\
      [5pt]={}&z\cdot {\frac {(1-z^{5})(1-z^{10})\cdots }{(1-z)(1-z^{2})\cdots
      }}\times (1+z^{5}+z^{10}+\cdots )(1+z^{10}+z^{20}+\cdots )\cdots \\[5pt]=
      {}&z+\sum _{n\geq 2}p(n-1)z^{n},\end{aligned}}}  [{\displaystyle {\begin
      {aligned}&{\frac {z}{(1-z)(1-z^{2})\cdots }}\\[5pt]={}&z\cdot {\frac {(1-
      z^{5})(1-z^{10})\cdots }{(1-z)(1-z^{2})\cdots }}\times (1+z^{5}+z^
      {10}+\cdots )(1+z^{10}+z^{20}+\cdots )\cdots \\[5pt]={}&z+\sum _{n\geq
      2}p(n-1)z^{n},\end{aligned}}}]
we may equate the coefficients of      z  5 m + 5     {\displaystyle z^{5m+5}}
[{\displaystyle z^{5m+5}}] in the previous equations to prove our desired
congruence result, namely that,     p ( 5 m + 4 ) &#x2261; 0   ( mod  5 )
{\displaystyle p(5m+4)\equiv 0{\pmod {5}}}  [{\displaystyle p(5m+4)\equiv 0
{\pmod {5}}}] for all     m &#x2265; 0   {\displaystyle m\geq 0}  [m\geq 0].
**** Transformations of generating functions[edit] ****
There are a number of transformations of generating functions that provide
other applications (see the main_article). A transformation of a sequence's
ordinary generating function (OGF) provides a method of converting the
generating function for one sequence into a generating function enumerating
another. These transformations typically involve integral formulas involving a
sequence OGF (see integral_transformations) or weighted sums over the higher-
order derivatives of these functions (see derivative_transformations).
Generating function transformations can come into play when we seek to express
a generating function for the sums
          s  n   :=  &#x2211;  m = 0   n      (   n m   )     C  n , m    a  m
      ,   {\displaystyle s_{n}:=\sum _{m=0}^{n}{\binom {n}{m}}C_{n,m}a_{m},}  [
      {\displaystyle s_{n}:=\sum _{m=0}^{n}{\binom {n}{m}}C_{n,m}a_{m},}]
in the form of     S ( z ) = g ( z ) A ( f ( z ) )   {\displaystyle S(z)=g(z)A
(f(z))}  [{\displaystyle S(z)=g(z)A(f(z))}] involving the original sequence
generating function. For example, if the sums      s  n   :=  &#x2211;  k
&#x2265; 0      (    n + k   m + 2 k    )     a  k     {\displaystyle s_{n}:
=\sum _{k\geq 0}{\binom {n+k}{m+2k}}a_{k}}  [{\displaystyle s_{n}:=\sum _{k\geq
0}{\binom {n+k}{m+2k}}a_{k}}], then the generating function for the modified
sum expressions is given by     S ( z ) =    z  m    ( 1 &#x2212; z  )  m + 1
A  (   z  ( 1 &#x2212; z  )  2      )    {\displaystyle S(z)={\frac {z^{m}}{(1-
z)^{m+1}}}A\left({\frac {z}{(1-z)^{2}}}\right)}  [{\displaystyle S(z)={\frac
{z^{m}}{(1-z)^{m+1}}}A\left({\frac {z}{(1-z)^{2}}}\right)}] [26] (see also the
binomial_transform and the Stirling_transform).
There are also integral formulas for converting between a sequence's OGF,     F
( z )   {\displaystyle F(z)}  [{\displaystyle F(z)}], and its exponential
generating function, or EGF,        F &#x005E;    ( z )   {\displaystyle
{\widehat {F}}(z)}  [{\displaystyle {\widehat {F}}(z)}], and vice versa given
by
         F ( z ) =  &#x222B;  0   &#x221E;      F &#x005E;    ( t z )  e
      &#x2212; t    d t   {\displaystyle F(z)=\int _{0}^{\infty }{\widehat {F}}
      (tz)e^{-t}\,dt}  [{\displaystyle F(z)=\int _{0}^{\infty }{\widehat {F}}
      (tz)e^{-t}\,dt}]
            F &#x005E;    ( z ) =   1  2 &#x03C0;     &#x222B;  &#x2212;
      &#x03C0;   &#x03C0;   F  (  z  e  &#x2212; &#x0131; &#x03D1;    )   e   e
      &#x0131; &#x03D1;      d &#x03D1; ,   {\displaystyle {\widehat {F}}(z)=
      {\frac {1}{2\pi }}\int _{-\pi }^{\pi }F\left(ze^{-\imath \vartheta
      }\right)e^{e^{\imath \vartheta }}\,d\vartheta ,}  [{\displaystyle
      {\widehat {F}}(z)={\frac {1}{2\pi }}\int _{-\pi }^{\pi }F\left(ze^{-
      \imath \vartheta }\right)e^{e^{\imath \vartheta }}\,d\vartheta ,}]
provided that these integrals converge for appropriate values of     z
{\displaystyle z}  [z].
**** Other applications[edit] ****
Generating functions are used to:
    * Find a closed_formula for a sequence given in a recurrence relation. For
      example, consider Fibonacci_numbers.
    * Find recurrence_relations for sequencesâthe form of a generating
      function may suggest a recurrence formula.
    * Find relationships between sequencesâif the generating functions of two
      sequences have a similar form, then the sequences themselves may be
      related.
    * Explore the asymptotic behaviour of sequences.
    * Prove identities involving sequences.
    * Solve enumeration problems in combinatorics and encoding their solutions.
      Rook_polynomials are an example of an application in combinatorics.
    * Evaluate infinite sums.
***** Other generating functions[edit] *****
**** Examples[edit] ****
Examples of polynomial_sequences generated by more complex generating functions
include:
    * Appell_polynomials
    * Chebyshev_polynomials
    * Difference_polynomials
    * Generalized_Appell_polynomials
    * Q-difference_polynomials
Other sequences generated by more complex generating functions:
    * Double exponential generating functions. For example: Aitken's_Array:
      Triangle_of_Numbers
    * Hadamard products of generating functions / diagonal generating functions
      and their corresponding integral_transformations
**** Convolution polynomials[edit] ****
Knuth's article titled "Convolution Polynomials"[27] defines a generalized
class of convolution polynomial sequences by their special generating functions
of the form
         F ( z  )  x   = exp &#x2061;  (  x log &#x2061; F ( z )  )  =
      &#x2211;  n &#x2265; 0    f  n   ( x )  z  n   ,   {\displaystyle F(z)^
      {x}=\exp \left(x\log F(z)\right)=\sum _{n\geq 0}f_{n}(x)z^{n},}  [
      {\displaystyle F(z)^{x}=\exp \left(x\log F(z)\right)=\sum _{n\geq 0}f_{n}
      (x)z^{n},}]
for some analytic function     F   {\displaystyle F}  [F] with a power series
expansion such that     F ( 0 ) = 1   {\displaystyle F(0)=1}  [{\displaystyle F
(0)=1}]. We say that a family of polynomials,      f  0   ,  f  1   ,  f  2   ,
&#x2026;   {\displaystyle f_{0},f_{1},f_{2},\ldots }  [{\displaystyle f_{0},f_
{1},f_{2},\ldots }], forms a convolution family if     deg &#x2061; {  f  n   }
&#x2264; n   {\displaystyle \deg\{f_{n}\}\leq n}  [{\displaystyle \deg\{f_
{n}\}\leq n}] and if the following convolution condition holds for all     x ,
y   {\displaystyle x,y}  [x,y] and for all     n &#x2265; 0   {\displaystyle
n\geq 0}  [n\geq 0]:
          f  n   ( x + y ) =  f  n   ( x )  f  0   ( y ) +  f  n &#x2212; 1
      ( x )  f  1   ( y ) + &#x22EF; +  f  1   ( x )  f  n &#x2212; 1   ( y ) +
      f  0   ( x )  f  n   ( y ) .   {\displaystyle f_{n}(x+y)=f_{n}(x)f_{0}
      (y)+f_{n-1}(x)f_{1}(y)+\cdots +f_{1}(x)f_{n-1}(y)+f_{0}(x)f_{n}(y).}  [
      {\displaystyle f_{n}(x+y)=f_{n}(x)f_{0}(y)+f_{n-1}(x)f_{1}(y)+\cdots +f_
      {1}(x)f_{n-1}(y)+f_{0}(x)f_{n}(y).}]
We see that for non-identically zero convolution families, this definition is
equivalent to requiring that the sequence have an ordinary generating function
of the first form given above.
A sequence of convolution polynomials defined in the notation above has the
following properties:
    * The sequence     n ! &#x22C5;  f  n   ( x )   {\displaystyle n!\cdot f_
      {n}(x)}  [{\displaystyle n!\cdot f_{n}(x)}] is of binomial_type
    * Special values of the sequence include      f  n   ( 1 ) = [  z  n   ] F
      ( z )   {\displaystyle f_{n}(1)=[z^{n}]F(z)}  [{\displaystyle f_{n}(1)=
      [z^{n}]F(z)}] and      f  n   ( 0 ) =  &#x03B4;  n , 0     {\displaystyle
      f_{n}(0)=\delta _{n,0}}  [{\displaystyle f_{n}(0)=\delta _{n,0}}], and
    * For arbitrary (fixed)     x , y , t &#x2208;  C    {\displaystyle
      x,y,t\in \mathbb {C} }  [{\displaystyle x,y,t\in \mathbb {C} }], these
      polynomials satisfy convolution formulas of the form
              f  n   ( x + y )    =  &#x2211;  k = 0   n    f  k   ( x )  f  n
      &#x2212; k   ( y )      f  n   ( 2 x )    =  &#x2211;  k = 0   n    f  k
      ( x )  f  n &#x2212; k   ( x )     x n  f  n   ( x + y )    = ( x + y )
      &#x2211;  k = 0   n   k  f  k   ( x )  f  n &#x2212; k   ( y )        ( x
      + y )  f  n   ( x + y + t n )   x + y + t n       =  &#x2211;  k = 0   n
      x  f  k   ( x + t k )   x + t k       y  f  n &#x2212; k   ( y + t ( n
      &#x2212; k ) )   y + t ( n &#x2212; k )    .       {\displaystyle {\begin
      {aligned}f_{n}(x+y)&=\sum _{k=0}^{n}f_{k}(x)f_{n-k}(y)\\f_{n}(2x)&=\sum _
      {k=0}^{n}f_{k}(x)f_{n-k}(x)\\xnf_{n}(x+y)&=(x+y)\sum _{k=0}^{n}kf_{k}
      (x)f_{n-k}(y)\\{\frac {(x+y)f_{n}(x+y+tn)}{x+y+tn}}&=\sum _{k=0}^{n}
      {\frac {xf_{k}(x+tk)}{x+tk}}{\frac {yf_{n-k}(y+t(n-k))}{y+t(n-k)}}.\end
      {aligned}}}  [{\displaystyle {\begin{aligned}f_{n}(x+y)&=\sum _{k=0}^
      {n}f_{k}(x)f_{n-k}(y)\\f_{n}(2x)&=\sum _{k=0}^{n}f_{k}(x)f_{n-k}(x)\\xnf_
      {n}(x+y)&=(x+y)\sum _{k=0}^{n}kf_{k}(x)f_{n-k}(y)\\{\frac {(x+y)f_{n}
      (x+y+tn)}{x+y+tn}}&=\sum _{k=0}^{n}{\frac {xf_{k}(x+tk)}{x+tk}}{\frac
      {yf_{n-k}(y+t(n-k))}{y+t(n-k)}}.\end{aligned}}}]
For a fixed non-zero parameter     t &#x2208;  C    {\displaystyle t\in \mathbb
{C} }  [{\displaystyle t\in \mathbb {C} }], we have modified generating
functions for these convolution polynomial sequences given by
            z  F  n   ( x + t n )   ( x + t n )    = [  z  n   ]    F    t
      ( z  )  x   ,   {\displaystyle {\frac {zF_{n}(x+tn)}{(x+tn)}}=[z^{n}]
      {\mathcal {F}}_{t}(z)^{x},}  [{\displaystyle {\frac {zF_{n}(x+tn)}{
      (x+tn)}}=[z^{n}]{\mathcal {F}}_{t}(z)^{x},}]
where        F    t   ( z )   {\displaystyle {\mathcal {F}}_{t}(z)}  [
{\displaystyle {\mathcal {F}}_{t}(z)}] is implicitly defined by a functional
equation of the form        F    t   ( z ) = F  (  x    F    t   ( z  )  t    )
{\displaystyle {\mathcal {F}}_{t}(z)=F\left(x{\mathcal {F}}_{t}(z)^{t}\right)}
[{\displaystyle {\mathcal {F}}_{t}(z)=F\left(x{\mathcal {F}}_{t}(z)^
{t}\right)}]. Moreover, we can use matrix methods (as in the reference) to
prove that given two convolution polynomial sequences,     &#x27E8;  f  n   ( x
) &#x27E9;   {\displaystyle \langle f_{n}(x)\rangle }  [{\displaystyle \langle
f_{n}(x)\rangle }] and     &#x27E8;  g  n   ( x ) &#x27E9;   {\displaystyle
\langle g_{n}(x)\rangle }  [{\displaystyle \langle g_{n}(x)\rangle }], with
respective corresponding generating functions,     F ( z  )  x
{\displaystyle F(z)^{x}}  [{\displaystyle F(z)^{x}}] and     G ( z  )  x
{\displaystyle G(z)^{x}}  [{\displaystyle G(z)^{x}}], then for arbitrary     t
{\displaystyle t}  [t] we have the identity
         [  z  n   ]   (  G ( z ) F  (  z G ( z  )  t    )   )   x   =
      &#x2211;  k = 0   n    F  k   ( x )  G  n &#x2212; k   ( x + t k ) .
      {\displaystyle [z^{n}]\left(G(z)F\left(zG(z)^{t}\right)\right)^{x}=\sum _
      {k=0}^{n}F_{k}(x)G_{n-k}(x+tk).}  [{\displaystyle [z^{n}]\left(G(z)F\left
      (zG(z)^{t}\right)\right)^{x}=\sum _{k=0}^{n}F_{k}(x)G_{n-k}(x+tk).}]
Examples of convolution polynomial sequences include the binomial power series,
B    t   ( z ) = 1 + z    B    t   ( z  )  t     {\displaystyle {\mathcal {B}}_
{t}(z)=1+z{\mathcal {B}}_{t}(z)^{t}}  [{\displaystyle {\mathcal {B}}_{t}(z)=1+z
{\mathcal {B}}_{t}(z)^{t}}], so-termed tree polynomials, the Bell_numbers,
B ( n )   {\displaystyle B(n)}  [{\displaystyle B(n)}], the Laguerre
polynomials, and the Stirling_convolution_polynomials.
**** Tables of special generating functions[edit] ****
An initial listing of special mathematical series is found here. A number of
useful and special sequence generating functions are found in Section 5.4 and
7.4 of Concrete Mathematics and in Section 2.5 of Wilf's
Generatingfunctionology. Other special generating functions of note include the
entries in the next table, which is by no means complete.[28]
         This section needs expansion with: Lists of special and special
[[icon]] sequence generating functions. The next table is a start. You can help
         by adding_to_it. (April 2017)
Formal power series       Generating-function        Notes
                          formula
    &#x2211;  n &#x2265;
0      (    m + n  n   )       1  ( 1 &#x2212; z  )
(   H  n + m   &#x2212;   m + 1      ln &#x2061;   1
H  m    )   z  n          1 &#x2212; z
{\displaystyle \sum _     {\displaystyle {\frac {1}{     H  n
{n\geq 0}{\binom {m+n}    (1-z)^{m+1}}}\ln {\frac    {\displaystyle H_{n}}  [H_
{n}}\left(H_{n+m}-H_      {1}{1-z}}}  [              {n}] is a first-order
{m}\right)z^{n}}  [       {\displaystyle {\frac {1}{ harmonic_number
{\displaystyle \sum _     (1-z)^{m+1}}}\ln {\frac
{n\geq 0}{\binom {m+n}    {1}{1-z}}}]
{n}}\left(H_{n+m}-H_
{m}\right)z^{n}}]
    &#x2211;  n &#x2265;
0    B  n      z  n    n       z   e  z   &#x2212; 1
!      {\displaystyle     {\displaystyle {\frac {z}      B  n
\sum _{n\geq 0}B_{n}      {e^{z}-1}}}  [             {\displaystyle B_{n}}  [B_
{\frac {z^{n}}{n!}}}  [   {\displaystyle {\frac {z}  {n}] is a Bernoulli_number
{\displaystyle \sum _     {e^{z}-1}}}]
{n\geq 0}B_{n}{\frac {z^
{n}}{n!}}}]
                                 F  m   z   1
                          &#x2212; (  F  m &#x2212;      F  n
    &#x2211;  n &#x2265;  1   +  F  m + 1   ) z +    {\displaystyle F_{n}}  [F_
0    F  m n    z  n       ( &#x2212; 1  )  m    z  2 {n}] is a Fibonacci_number
{\displaystyle \sum _     {\displaystyle {\frac {F_  and     m &#x2208;   Z   +
{n\geq 0}F_{mn}z^{n}}  [  {m}z}{1-(F_{m-1}+F_        {\displaystyle m\in
{\displaystyle \sum _     {m+1})z+(-1)^{m}z^{2}}}}   \mathbb {Z} ^{+}}  [
{n\geq 0}F_{mn}z^{n}}]    [{\displaystyle {\frac {F_ {\displaystyle m\in
                          {m}z}{1-(F_{m-1}+F_        \mathbb {Z} ^{+}}]
                          {m+1})z+(-1)^{m}z^{2}}}}]
                             (  z  &#x2212; 1    )
    &#x2211;  n &#x2265;  &#x2212; m  &#x00AF;    =
0    {     n     m     }  z  m    ( 1 &#x2212; z )       x   n &#x00AF;
z  n     {\displaystyle   ( 1 &#x2212; 2 z )         {\displaystyle x^
\sum _{n\geq 0}\left\{    &#x22EF; ( 1 &#x2212; m z  {\overline {n}}}  [x^
{\begin{matrix}n\\m\end   )      {\displaystyle (z^  {\overline{n}}] denotes
{matrix}}\right\}z^{n}}   {-1})^{\overline {-m}}=    the rising_factorial, or
[{\displaystyle \sum _    {\frac {z^{m}}{(1-z)(1-    Pochhammer_symbol and some
{n\geq 0}\left\{{\begin   2z)\cdots (1-mz)}}}  [     integer     m &#x2265; 0
{matrix}n\\m\end          {\displaystyle (z^{-1})^   {\displaystyle m\geq 0}
{matrix}}\right\}z^{n}}]  {\overline {-m}}={\frac    [m\geq 0]
                          {z^{m}}{(1-z)(1-2z)\cdots
                          (1-mz)}}}]
    &#x2211;  n &#x2265;      z   m &#x00AF;    = z
0    [     n     m     ]  ( z + 1 ) &#x22EF; ( z + m
z  n     {\displaystyle   &#x2212; 1 )
\sum _{n\geq 0}\left[     {\displaystyle z^
{\begin{matrix}n\\m\end   {\overline {m}}=z
{matrix}}\right]z^{n}}  [ (z+1)\cdots (z+m-1)}  [
{\displaystyle \sum _     {\displaystyle z^
{n\geq 0}\left[{\begin    {\overline {m}}=z
{matrix}n\\m\end          (z+1)\cdots (z+m-1)}]
{matrix}}\right]z^{n}}]
    &#x2211;  n &#x2265;
1      ( &#x2212; 1  )  n
&#x2212; 1    4  n   (  4
n   &#x2212; 2 )  B  2 n
z  2 n     ( 2 n )           ln &#x2061;    tan
&#x22C5; ( 2 n ) !        &#x2061; ( z )  z
{\displaystyle \sum _     {\displaystyle \ln {\frac
{n\geq 1}{\frac {(-1)^{n- {\tan(z)}{z}}}  [
1}4^{n}(4^{n}-2)B_{2n}z^  {\displaystyle \ln {\frac
{2n}}{(2n)\cdot (2n)!}}}  {\tan(z)}{z}}}]
[{\displaystyle \sum _
{n\geq 1}{\frac {(-1)^{n-
1}4^{n}(4^{n}-2)B_{2n}z^
{2n}}{(2n)\cdot (2n)!}}}]
    &#x2211;  n &#x2265;
0      ( 1  /  2  )   n
&#x00AF;     z  2 n
( 2 n + 1 ) &#x22C5; n !      z  &#x2212; 1   arcsin
{\displaystyle \sum _     &#x2061; ( z )
{n\geq 0}{\frac {(1/2)^   {\displaystyle z^{-
{\overline {n}}z^{2n}}{   1}\arcsin(z)}  [
(2n+1)\cdot n!}}}  [      {\displaystyle z^{-
{\displaystyle \sum _     1}\arcsin(z)}]
{n\geq 0}{\frac {(1/2)^
{\overline {n}}z^{2n}}{
(2n+1)\cdot n!}}}]
                                                         Li  s   &#x2061; ( z )
                                                     {\displaystyle
                                                     \operatorname {Li} _{s}
    &#x2211;  n &#x2265;         Li  s   &#x2061;    (z)}  [\operatorname {Li}
0    H  n   ( s )    z  n ( z )   1 &#x2212; z       _{s}(z)] is the
{\displaystyle \sum _     {\displaystyle {\frac      polylogarithm function and
{n\geq 0}H_{n}^{(s)}z^    {\operatorname {Li} _{s}   H  n   ( s )
{n}}  [{\displaystyle     (z)}{1-z}}}  [             {\displaystyle H_{n}^{
\sum _{n\geq 0}H_{n}^{    {\displaystyle {\frac      (s)}}  [{\displaystyle H_
(s)}z^{n}}]               {\operatorname {Li} _{s}   {n}^{(s)}}] is a
                          (z)}{1-z}}}]               generalized harmonic
                                                     number for     &#x211C;
                                                     ( s ) > 1   {\displaystyle
                                                     \Re (s)>1}  [\Re (s)>1]
                                                         {     n     m     }
                                                     {\displaystyle \left\{
                                                     {\begin{matrix}n\\m\end
                                                     {matrix}}\right\}}  [
                              &#x2211;  0 &#x2264; j {\displaystyle \left\{
                          &#x2264; m    {     m      {\begin{matrix}n\\m\end
                          j     }     j ! &#x22C5;   {matrix}}\right\}}] is a
                          z  j     ( 1 &#x2212; z  ) Stirling_number_of_the
                          j + 1                      second_kind and where the
                          {\displaystyle \sum _      individual terms in the
    &#x2211;  n &#x2265;  {0\leq j\leq m}\left\{     expansion satisfy        z
0    n  m    z  n         {\begin{matrix}m\\j\end    i    ( 1 &#x2212; z  )  i
{\displaystyle \sum _     {matrix}}\right\}{\frac    + 1      =  &#x2211;  k =
{n\geq 0}n^{m}z^{n}}  [   {j!\cdot z^{j}}{(1-z)^     0   i      (   i k   )
{\displaystyle \sum _     {j+1}}}}  [{\displaystyle  ( &#x2212; 1  )  k
{n\geq 0}n^{m}z^{n}}]     \sum _{0\leq j\leq         &#x2212; i     ( 1
                          m}\left\{{\begin           &#x2212; z  )  k + 1
                          {matrix}m\\j\end           {\displaystyle {\frac {z^
                          {matrix}}\right\}{\frac    {i}}{(1-z)^{i+1}}}=\sum _
                          {j!\cdot z^{j}}{(1-z)^     {k=0}^{i}{\binom {i}{k}}
                          {j+1}}}}]                  {\frac {(-1)^{k-i}}{(1-z)^
                                                     {k+1}}}}  [{\displaystyle
                                                     {\frac {z^{i}}{(1-z)^
                                                     {i+1}}}=\sum _{k=0}^{i}
                                                     {\binom {i}{k}}{\frac {(-
                                                     1)^{k-i}}{(1-z)^{k+1}}}}]
                               (    1 +   1 + 4 z
                          2   )   n   +   (    1
    &#x2211;  k < n       &#x2212;   1 + 4 z    2
(    n &#x2212; k  k   )  )   n     {\displaystyle
n  n &#x2212; k     z  k  \left({\frac {1+{\sqrt
{\displaystyle \sum _     {1+4z}}}{2}}\right)^
{k<n}{\binom {n-k}{k}}    {n}+\left({\frac {1-{\sqrt
{\frac {n}{n-k}}z^{k}}  [ {1+4z}}}{2}}\right)^{n}}
{\displaystyle \sum _     [{\displaystyle \left(
{k<n}{\binom {n-k}{k}}    {\frac {1+{\sqrt {1+4z}}}
{\frac {n}{n-k}}z^{k}}]   {2}}\right)^{n}+\left(
                          {\frac {1-{\sqrt {1+4z}}}
                          {2}}\right)^{n}}]
    &#x2211;   n  1   ,                              The two-variable case is
&#x2026; ,  n  m                 z  1   &#x22EF;  z  given by     M ( w , z ) :
&#x2265; 0   min (  n  1  m     ( 1 &#x2212;  z  1   =  &#x2211;  m , n
, &#x2026; ,  n  m   )  z ) &#x22EF; ( 1 &#x2212;  z &#x2265; 0   min ( m , n )
1    n  1     &#x22EF;  z m   ) ( 1 &#x2212;  z  1   w  m    z  n   =    w z
m    n  m                 &#x22EF;  z  m   )         ( 1 &#x2212; w ) ( 1
{\displaystyle \sum _{n_  {\displaystyle {\frac {z_  &#x2212; z ) ( 1 &#x2212;
{1},\ldots ,n_{m}\geq     {1}\cdots z_{m}}{(1-z_     w z )      {\displaystyle
0}\min(n_{1},\ldots ,n_   {1})\cdots (1-z_{m})(1-z_  M(w,z):=\sum _{m,n\geq
{m})z_{1}^{n_{1}}\cdots   {1}\cdots z_{m})}}}  [     0}\min(m,n)w^{m}z^{n}=
z_{m}^{n_{m}}}  [         {\displaystyle {\frac {z_  {\frac {wz}{(1-w)(1-z)(1-
{\displaystyle \sum _{n_  {1}\cdots z_{m}}{(1-z_     wz)}}}  [{\displaystyle M
{1},\ldots ,n_{m}\geq     {1})\cdots (1-z_{m})(1-z_  (w,z):=\sum _{m,n\geq
0}\min(n_{1},\ldots ,n_   {1}\cdots z_{m})}}}]       0}\min(m,n)w^{m}z^{n}=
{m})z_{1}^{n_{1}}\cdots                              {\frac {wz}{(1-w)(1-z)(1-
z_{m}^{n_{m}}}]                                      wz)}}}]
    &#x2211;  n &#x2265;
0      (   s n   )     z                                s &#x2208;  C
n     {\displaystyle \sum    ( 1 + z  )  s           {\displaystyle s\in
_{n\geq 0}{\binom {s}     {\displaystyle (1+z)^{s}}  \mathbb {C} }  [
{n}}z^{n}}  [             [{\displaystyle (1+z)^     {\displaystyle s\in
{\displaystyle \sum _     {s}}]                      \mathbb {C} }]
{n\geq 0}{\binom {s}
{n}}z^{n}}]
    &#x2211;  n &#x2265;
0      (   n k   )     z        z  k    ( 1 &#x2212;
n     {\displaystyle \sum z  )  k + 1                   k &#x2208;  N
_{n\geq 0}{\binom {n}     {\displaystyle {\frac {z^  {\displaystyle k\in
{k}}z^{n}}  [             {k}}{(1-z)^{k+1}}}}  [     \mathbb {N} }  [k\in
{\displaystyle \sum _     {\displaystyle {\frac {z^  \mathbb {N} ]
{n\geq 0}{\binom {n}      {k}}{(1-z)^{k+1}}}}]
{k}}z^{n}}]
                             &#x2212;   &#x2202;
    &#x2211;  n &#x2265;  &#x2202; s       L i   s
1   log &#x2061;  ( n )   ( z )  &#x2061;   |   s =
z  n     {\displaystyle   0     {\displaystyle -
\sum _{n\geq 1}\log {     {\partial \over \partial
(n)}z^{n}}  [             s}\operatorname {{Li}_{s}
{\displaystyle \sum _     (z)} |_{s=0}}  [
{n\geq 1}\log {(n)}z^     {\displaystyle -{\partial
{n}}]                     \over \partial
                          s}\operatorname {{Li}_{s}
                          (z)} |_{s=0}}]

***** History[edit] *****
George_PÃ³lya writes in Mathematics_and_plausible_reasoning:
      The name "generating function" is due to Laplace. Yet, without giving it
      a name, Euler used the device of generating functions long before Laplace
      [..]. He applied this mathematical tool to several problems in
      Combinatory Analysis and the Theory_of_Numbers.
***** See also[edit] *****
    * Moment-generating_function
    * Probability-generating_function
    * Generating_function_transformation
    * Stanley's_reciprocity_theorem
    * Applications to Partition_(number_theory)
    * Combinatorial_principles
    * Cyclic_sieving
    * Z-transform
***** Notes[edit] *****
   1. ^ Donald_E._Knuth, The_Art_of_Computer_Programming, Volume 1 Fundamental
      Algorithms (Third Edition) Addison-Wesley.
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
   3. ISBN 0-201-89683-4. Section 1.2.9: "Generating Functions".
   4. ^ This alternative term can already be found in E.N. Gilbert (1956),
      "Enumeration of Labeled graphs", Canadian_Journal_of_Mathematics 3,
      p. 405â411, but its use is rare before the year 2000; since then it
      appears to be increasing.
   5. ^ Flajolet & Sedgewick (2009) p.95
   6. ^Apostol,_Tom_M. (1976), Introduction to analytic number theory,
      Undergraduate Texts in Mathematics, New York-Heidelberg: Springer-Verlag,
      ISBN 978-0-387-90163-3, MR 0434929, Zbl 0335.10001
   7.  pp.42â43
   8. ^ Wilf (1994) p.56
   9. ^ Wilf (1994) p.59
  10. ^Hardy and Wright (2008). An Introduction to the Theory of Numbers (Sixth
      ed.). New York: Oxford University Press. p. 339.
  11. ^Spivey, Michael Z. (2007). "Combinatorial Sums and Finite Differences".
      Discrete Math. 307 (24): 3130â3146. doi:10.1016/j.disc.2007.03.052.
      MR 2370116.
  12. ^Mathar, R. J. (2012). "Yet another table of integrals". arXiv:1207.5845.
  13.  v4 eq. (0.4)
  14. ^ See Table 265 in Section 6.1 of Concrete Mathematics for finite sum
      identities involving the Stirling number triangles.
  15. ^ See section 2.4 in Lando's book Lectures on Generating Functions
      (2002).
  16. ^ Example from Section 6.3 of R. P. Stanley's Enumerative Combinatorics
      (Volume 2).
  17. ^ See Section 1.2.9 in Knuth's The Art of Computer Programming (Vol. 1).
  18. ^ Solution to exercise 7.36 on page 569 in Graham, Knuth and Patshnik.
  19. ^Flajolet and Sedgewick (2010). Analytic Combinatorics. New York:
      Cambridge University Press. ISBN 978-0-521-89806-5.
  20.  (Section B.4)
  21. ^Schneider, C. (2007). "Symbolic Summation Assists Combinatorics".
      Sem.Lothar.Combin. 56: 1â36.
  22. ^ See P. Flajolet's article Combinatorial_aspects_of_continued_fractions
      (1980) and also refer to H. S. Wall's Analytic theory of continued
      fractions (1948) for more complete information on the properties of J-
      fractions.
  23. ^ See the following articles:
          o Continued_Fractions_for_Square_Series_Generating_Functions (2016)
          o Jacobi_Type_Continued_Fractions_for_the_Ordinary_Generating
            Functions_of_Generalized_Factorial_Functions (2017)
          o Jacobi-Type_Continued_Fractions_and_Congruences_for_Binomial
            Coefficients_Modulo_Integers_____h_&#x2265;_2___{\displaystyle
            h\geq_2}__[{\displaystyle_h\geq_2}] (2017)
  24. ^"Lambert_series_identity". Math Overflow. 2017.
  25. ^Good, I. J. (1986). "On applications of symmetric Dirichlet
      distributions and their mixtures to contingency tables". Annals_of
      Statistics. 4 (6): 1159â1189. doi:10.1214/aos/1176343649.
  26. ^ See the usage of these terms in Section 7.4 of Concrete Mathematics on
      special sequence generating functions.
  27. ^ Section 8.3 in Concrete Mathematics.
  28. ^ See Example 6 in Section 7.3 of Concrete Mathematics for another method
      and the complete setup of this problem using generating functions. This
      more "convoluted" approach is given in Section 7.5 of the same reference.
  29. ^ See Section 5 of Lando's Lectures on Generating Functions.
  30. ^ See Section 19.12 of Hardy and Wright's classic book An introduction to
      the theory of numbers.
  31. ^ Solution to exercise 5.71 on page 535 in Concrete Mathematics by
      Graham, Knuth and Patashnik.
  32. ^Knuth, D. E. (1992). "Convolution_Polynomials" (PDF). Mathematica J. 2:
      67â78.
  33. ^ See also the 1031 Generating Functions found in the article referenced
      here.
***** References[edit] *****
    * Doubilet, Peter; Rota,_Gian-Carlo; Stanley,_Richard (1972). "On_the
      foundations_of_combinatorial_theory._VI._The_idea_of_generating
      function". Proceedings of the Sixth Berkeley Symposium on Mathematical
      Statistics and Probability. 2: 267â318. Zbl 0267.05002.
 Reprinted inRota,_Gian-Carlo (1975). "3. The idea of generating function".
Finite Operator Calculus. With the collaboration of P. Doubilet, C. Greene, D.
Kahaner, A._Odlyzko and R._Stanley. Academic Press. pp. 83â134. ISBN 0-12-
596650-4. Zbl 0328.05007.
Flajolet,_Philippe; Sedgewick,_Robert (2009). Analytic_Combinatorics (PDF).
Cambridge University Press. ISBN 978-0-521-89806-5. Zbl 1165.05001.
Goulden, Ian P.; Jackson,_David_M. (2004). Combinatorial Enumeration. Dover
Publications. ISBN 978-0486435978.
Ronald_L._Graham; Donald_E._Knuth; Oren_Patashnik (1994). "Chapter 7:
Generating Functions". Concrete_Mathematics._A_foundation_for_computer_science
(second ed.). Addison-Wesley. pp. 320â380. ISBN 0-201-55802-5.
Zbl 0836.00001.
Wilf,_Herbert_S. (1994). Generatingfunctionology (2nd ed.). Boston, MA:
Academic Press. ISBN 0-12-751956-4. Zbl 0831.05001.
Martin Aigner. A Course in Enumeration
***** External links[edit] *****
    * "Introduction_To_Ordinary_Generating_Functions" by Mike Zabrocki, York
      University, Mathematics and Statistics
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Generating_function",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Generating_Functions,_Power_Indices_and_Coin_Change at cut-the-knot
"Generating_Functions" by Ed_Pegg,_Jr., Wolfram_Demonstrations_Project, 2007.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Generating_function&oldid=907689625"
Categories:
    * Generating_functions
Hidden categories:
    * Wikipedia_articles_that_are_too_technical_from_March_2018
    * All_articles_that_are_too_technical
    * Articles_needing_expert_attention_from_March_2018
    * All_articles_needing_expert_attention
    * Articles_that_may_be_too_long_from_March_2018
    * Articles_with_multiple_maintenance_issues
    * Articles_to_be_expanded_from_April_2017
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * SlovenÄina
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * ä¸­æ
Edit_links
    * This page was last edited on 24 July 2019, at 16:13 (UTC).
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
