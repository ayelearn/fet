The following text has been accessed from https://en.wikipedia.org/wiki/Independence_(probability_theory)#Independent_random_variables at Fri Aug 9 02:50:50 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Independence (probability theory) ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Part of a series on statistics
Probability_theory
[Nuvola_apps_atlantik.png]
    * Probability_axioms
    * Probability_space
    * Sample_space
    * Elementary_event
    * Event
    * Random_variable
    * Probability_measure
    * Complementary_event
    * Joint_probability
    * Marginal_probability
    * Conditional_probability
    * Independence
    * Conditional_independence
    * Law_of_total_probability
    * Law_of_large_numbers
    * Bayes'_theorem
    * Boole's_inequality
    * Venn_diagram
    * Tree_diagram
    * v
    * t
    * e
In probability_theory, two events are independent, statistically independent,
or stochastically independent[1] if the occurrence of one does not affect the
probability of occurrence of the other (equivalently, does not affect the
odds). Similarly, two random_variables are independent if the realization of
one does not affect the probability_distribution of the other.
The concept of independence extends to dealing with collections of more than
two events or random variables, in which case the events are pairwise
independent if each pair are independent of each other, and the events are
mutually independent if each event is independent of each other combination of
events.
⁰
***** Contents *****
    * 1_Definition
          o 1.1_For_events
                # 1.1.1_Two_events
                # 1.1.2_Log_probability_and_information_content
                # 1.1.3_Odds
                # 1.1.4_More_than_two_events
          o 1.2_For_real_valued_random_variables
                # 1.2.1_Two_random_variables
                # 1.2.2_More_than_two_random_variables
          o 1.3_For_real_valued_random_vectors
          o 1.4_For_stochastic_processes
                # 1.4.1_For_one_stochastic_process
                # 1.4.2_For_two_stochastic_processes
          o 1.5_Independent_σ-algebras
    * 2_Properties
          o 2.1_Self-independence
          o 2.2_Expectation_and_covariance
          o 2.3_Characteristic_function
    * 3_Examples
          o 3.1_Rolling_dice
          o 3.2_Drawing_cards
          o 3.3_Pairwise_and_mutual_independence
          o 3.4_Mutual_independence
    * 4_Conditional_independence
          o 4.1_For_events
          o 4.2_For_random_variables
    * 5_See_also
    * 6_References
    * 7_External_links
***** Definition[edit] *****
**** For events[edit] ****
*** Two events[edit] ***
Two events     A   {\displaystyle A}  [A] and     B   {\displaystyle B}  [B]
are independent (often written as     A &#x22A5; B   {\displaystyle A\perp B}
[A\perp B] or     A &#x22A5;    &#x22A5; B   {\displaystyle A\perp \!\!\!\perp
B}  [A\perp \!\!\!\perp B]) if and only if their joint_probability equals the
product of their probabilities:[2]:p. 29[3]:p. 10
    P  ( A &#x2229; B ) =  P  ( A )  P  ( B )   {\displaystyle        
\mathrm {P} (A\cap B)=\mathrm {P} (A)\mathrm {P} (B)}  [\mathrm{P}      (Eq.1)
(A \cap B) = \mathrm{P}(A)\mathrm{P}(B)]
Why this defines independence is made clear by rewriting with conditional
probabilities:
          P  ( A &#x2229; B ) =  P  ( A )  P  ( B )  &#x27FA;   P  ( A ) =
      P  ( A &#x2229; B )    P  ( B )    =  P  ( A &#x2223; B )
      {\displaystyle \mathrm {P} (A\cap B)=\mathrm {P} (A)\mathrm {P} (B)\iff
      \mathrm {P} (A)={\frac {\mathrm {P} (A\cap B)}{\mathrm {P} (B)}}=\mathrm
      {P} (A\mid B)}  [{\displaystyle \mathrm {P} (A\cap B)=\mathrm {P}
      (A)\mathrm {P} (B)\iff \mathrm {P} (A)={\frac {\mathrm {P} (A\cap B)}
      {\mathrm {P} (B)}}=\mathrm {P} (A\mid B)}].
and similarly
          P  ( A &#x2229; B ) =  P  ( A )  P  ( B )  &#x27FA;   P  ( B ) =  P
      ( B &#x2223; A )   {\displaystyle \mathrm {P} (A\cap B)=\mathrm {P}
      (A)\mathrm {P} (B)\iff \mathrm {P} (B)=\mathrm {P} (B\mid A)}  [
      {\displaystyle \mathrm {P} (A\cap B)=\mathrm {P} (A)\mathrm {P} (B)\iff
      \mathrm {P} (B)=\mathrm {P} (B\mid A)}].
Thus, the occurrence of     B   {\displaystyle B}  [B] does not affect the
probability of     A   {\displaystyle A}  [A], and vice versa. Although the
derived expressions may seem more intuitive, they are not the preferred
definition, as the conditional probabilities may be undefined if      P  ( A )
{\displaystyle \mathrm {P} (A)}  [{\displaystyle \mathrm {P} (A)}] or      P
( B )   {\displaystyle \mathrm {P} (B)}  [{\displaystyle \mathrm {P} (B)}] are
0. Furthermore, the preferred definition makes clear by symmetry that when
A   {\displaystyle A}  [A] is independent of     B   {\displaystyle B}  [B],
B   {\displaystyle B}  [B] is also independent of     A   {\displaystyle A}
[A].
*** Log probability and information content[edit] ***
Stated in terms of log_probability, two events are independent if and only if
the log probability of the joint event is the sum of the log probability of the
individual events:
         log &#x2061;  P  ( A &#x2229; B ) = log &#x2061;  P  ( A ) + log
      &#x2061;  P  ( B )   {\displaystyle \log \mathrm {P} (A\cap B)=\log
      \mathrm {P} (A)+\log \mathrm {P} (B)}  [{\displaystyle \log \mathrm {P}
      (A\cap B)=\log \mathrm {P} (A)+\log \mathrm {P} (B)}]
In information_theory, negative log probability is interpreted as information
content, and thus two events are independent if and only if the information
content of the combined event equals the sum of information content of the
individual events:
          I  ( A &#x2229; B ) =  I  ( A ) +  I  ( B )   {\displaystyle \mathrm
      {I} (A\cap B)=\mathrm {I} (A)+\mathrm {I} (B)}  [{\displaystyle \mathrm
      {I} (A\cap B)=\mathrm {I} (A)+\mathrm {I} (B)}]
See Information_content_Â§ Additivity_of_independent_events for details.
*** Odds[edit] ***
Stated in terms of odds, two events are independent if and only if the odds
ratio of     A   {\displaystyle A}  [A] and     B   {\displaystyle B}  [B] is
unity (1). Analogously with probability, this is equivalent to the conditional
odds being equal to the unconditional odds:
         O ( A &#x2223; B ) = O ( A )  &#xA0;and&#xA0;  O ( B &#x2223; A ) = O
      ( B ) ,   {\displaystyle O(A\mid B)=O(A){\text{ and }}O(B\mid A)=O(B),}
      [{\displaystyle O(A\mid B)=O(A){\text{ and }}O(B\mid A)=O(B),}]
or to the odds of one event, given the other event, being the same as the odds
of the event, given the other event not occurring:
         O ( A &#x2223; B ) = O ( A &#x2223; &#x00AC; B )  &#xA0;and&#xA0;  O
      ( B &#x2223; A ) = O ( B &#x2223; &#x00AC; A ) .   {\displaystyle O(A\mid
      B)=O(A\mid \neg B){\text{ and }}O(B\mid A)=O(B\mid \neg A).}  [
      {\displaystyle O(A\mid B)=O(A\mid \neg B){\text{ and }}O(B\mid A)=O(B\mid
      \neg A).}]
The odds ratio can be defined as
         O ( A &#x2223; B ) : O ( A &#x2223; &#x00AC; B ) ,   {\displaystyle O
      (A\mid B):O(A\mid \neg B),}  [{\displaystyle O(A\mid B):O(A\mid \neg
      B),}]
or symmetrically for odds of     B   {\displaystyle B}  [B] given     A
{\displaystyle A}  [A], and thus is 1 if and only if the events are
independent.
*** More than two events[edit] ***
A finite set of events     {  A  i    }  i = 1   n     {\displaystyle \{A_
{i}\}_{i=1}^{n}}  [{\displaystyle \{A_{i}\}_{i=1}^{n}}] is pairwise independent
if every pair of events is independent[4]—that is, if and only if for all
distinct pairs of indices     m , k   {\displaystyle m,k}  [{\displaystyle
m,k}],
    P  (  A  m   &#x2229;  A  k   ) =  P  (  A  m   )  P  (  A  k
)   {\displaystyle \mathrm {P} (A_{m}\cap A_{k})=\mathrm {P} (A_     (Eq.2)
{m})\mathrm {P} (A_{k})}  [{\displaystyle \mathrm {P} (A_{m}\cap     
A_{k})=\mathrm {P} (A_{m})\mathrm {P} (A_{k})}]
A finite set of events is mutually independent if every event is independent of
any intersection of the other events[4][3]:p. 11—that is, if and only if for
every     k &#x2264; n   {\displaystyle k\leq n}  [k\leq n] and for every     k
{\displaystyle k}  [k]-element subset of events     {  B  i    }  i = 1   k
{\displaystyle \{B_{i}\}_{i=1}^{k}}  [{\displaystyle \{B_{i}\}_{i=1}^{k}}] of
{  A  i    }  i = 1   n     {\displaystyle \{A_{i}\}_{i=1}^{n}}  [
{\displaystyle \{A_{i}\}_{i=1}^{n}}],
    P   (   &#x22C2;  i = 1   k    B  i    )  =  &#x220F;  i = 1
k    P  (  B  i   )   {\displaystyle \mathrm {P} \left(\bigcap _    
{i=1}^{k}B_{i}\right)=\prod _{i=1}^{k}\mathrm {P} (B_{i})}  [         (Eq.3)
{\displaystyle \mathrm {P} \left(\bigcap _{i=1}^{k}B_
{i}\right)=\prod _{i=1}^{k}\mathrm {P} (B_{i})}]
This is called the multiplication rule for independent events. Note that it is
not a single condition involving only the product of all the probabilities of
all single events (see below for a counterexample); it must hold true for all
subsets of events.
For more than two events, a mutually independent set of events is (by
definition) pairwise independent; but the converse is not necessarily true (see
below for a counterexample).[2]:p. 30
**** For real valued random variables[edit] ****
*** Two random variables[edit] ***
Two random variables     X   {\displaystyle X}  [X] and     Y   {\displaystyle
Y}  [Y] are independent if_and_only_if (iff) the elements of the Ï-system
generated by them are independent; that is to say, for every     x
{\displaystyle x}  [x] and     y   {\displaystyle y}  [y], the events     { X
&#x2264; x }   {\displaystyle \{X\leq x\}}  [{\displaystyle \{X\leq x\}}] and
{ Y &#x2264; y }   {\displaystyle \{Y\leq y\}}  [{\displaystyle \{Y\leq y\}}]
are independent events (as defined above in Eq.1). That is,     X
{\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y] with cumulative
distribution_functions      F  X   ( x )   {\displaystyle F_{X}(x)}  [F_X(x)]
and      F  Y   ( y )   {\displaystyle F_{Y}(y)}  [F_Y(y)], are independent iff
the combined random variable     ( X , Y )   {\displaystyle (X,Y)}  [(X,Y)] has
a joint cumulative distribution function[3]:p. 15
    F  X , Y   ( x , y ) =  F  X   ( x )  F  Y   ( y )   for
all&#xA0;  x , y   {\displaystyle F_{X,Y}(x,y)=F_{X}(x)F_{Y}          (Eq.4)
(y)\quad {\text{for all }}x,y}  [{\displaystyle F_{X,Y}(x,y)=F_{X}    
(x)F_{Y}(y)\quad {\text{for all }}x,y}]
or equivalently, if the probability_densities      f  X   ( x )
{\displaystyle f_{X}(x)}  [f_{X}(x)] and      f  Y   ( y )   {\displaystyle f_
{Y}(y)}  [f_Y(y)] and the joint probability density      f  X , Y   ( x , y )
{\displaystyle f_{X,Y}(x,y)}  [f_{{X,Y}}(x,y)] exist,
          f  X , Y   ( x , y ) =  f  X   ( x )  f  Y   ( y )   for all&#xA0;  x
      , y   {\displaystyle f_{X,Y}(x,y)=f_{X}(x)f_{Y}(y)\quad {\text{for all
      }}x,y}  [{\displaystyle f_{X,Y}(x,y)=f_{X}(x)f_{Y}(y)\quad {\text{for all
      }}x,y}].
*** More than two random variables[edit] ***
A finite set of     n   {\displaystyle n}  [n] random variables     {  X  1   ,
&#x2026; ,  X  n   }   {\displaystyle \{X_{1},\ldots ,X_{n}\}}  [{\displaystyle
\{X_{1},\ldots ,X_{n}\}}] is pairwise_independent if and only if every pair of
random variables is independent. Even if the set of random variables is
pairwise independent, it is not necessarily mutually independent as defined
next.
A finite set of     n   {\displaystyle n}  [n] random variables     {  X  1   ,
&#x2026; ,  X  n   }   {\displaystyle \{X_{1},\ldots ,X_{n}\}}  [{\displaystyle
\{X_{1},\ldots ,X_{n}\}}] is mutually independent if and only if for any
sequence of numbers     {  x  1   , &#x2026; ,  x  n   }   {\displaystyle \{x_
{1},\ldots ,x_{n}\}}  [{\displaystyle \{x_{1},\ldots ,x_{n}\}}], the events
{  X  1   &#x2264;  x  1   } , &#x2026; , {  X  n   &#x2264;  x  n   }
{\displaystyle \{X_{1}\leq x_{1}\},\ldots ,\{X_{n}\leq x_{n}\}}  [
{\displaystyle \{X_{1}\leq x_{1}\},\ldots ,\{X_{n}\leq x_{n}\}}] are mutually
independent events (as defined above in Eq.3). This is equivalent to the
following condition on the joint cumulative distribution function      F   X  1
, &#x2026; ,  X  n     (  x  1   , &#x2026; ,  x  n   )   {\displaystyle F_{X_
{1},\ldots ,X_{n}}(x_{1},\ldots ,x_{n})}  [{\displaystyle F_{X_{1},\ldots ,X_
{n}}(x_{1},\ldots ,x_{n})}]. A finite set of     n   {\displaystyle n}  [n]
random variables     {  X  1   , &#x2026; ,  X  n   }   {\displaystyle \{X_
{1},\ldots ,X_{n}\}}  [{\displaystyle \{X_{1},\ldots ,X_{n}\}}] is mutually
independent if and only if[3]:p. 16
    F   X  1   , &#x2026; ,  X  n     (  x  1   , &#x2026; ,  x  n
) =  F   X  1     (  x  1   ) &#x22C5; &#x2026; &#x22C5;  F   X  n
(  x  n   )   for all&#xA0;   x  1   , &#x2026; ,  x  n
{\displaystyle F_{X_{1},\ldots ,X_{n}}(x_{1},\ldots ,x_{n})=F_{X_     (Eq.5)
{1}}(x_{1})\cdot \ldots \cdot F_{X_{n}}(x_{n})\quad {\text{for all    
}}x_{1},\ldots ,x_{n}}  [{\displaystyle F_{X_{1},\ldots ,X_{n}}(x_
{1},\ldots ,x_{n})=F_{X_{1}}(x_{1})\cdot \ldots \cdot F_{X_{n}}(x_
{n})\quad {\text{for all }}x_{1},\ldots ,x_{n}}]
Notice that is not necessary here to require that the probability distribution
factorizes for all possible     k &#x2212;   {\displaystyle k-}  [
{\displaystyle k-}]element subsets as in the case for     n   {\displaystyle n}
[n] events. This is not required because e.g.      F   X  1   ,  X  2   ,  X  3
(  x  1   ,  x  2   ,  x  3   ) =  F   X  1     (  x  1   ) &#x22C5;  F   X  2
(  x  2   ) &#x22C5;  F   X  3     (  x  3   )   {\displaystyle F_{X_{1},X_
{2},X_{3}}(x_{1},x_{2},x_{3})=F_{X_{1}}(x_{1})\cdot F_{X_{2}}(x_{2})\cdot F_{X_
{3}}(x_{3})}  [{\displaystyle F_{X_{1},X_{2},X_{3}}(x_{1},x_{2},x_{3})=F_{X_
{1}}(x_{1})\cdot F_{X_{2}}(x_{2})\cdot F_{X_{3}}(x_{3})}] implies      F   X  1
,  X  3     (  x  1   ,  x  3   ) =  F   X  1     (  x  1   ) &#x22C5;  F   X
3     (  x  3   )   {\displaystyle F_{X_{1},X_{3}}(x_{1},x_{3})=F_{X_{1}}(x_
{1})\cdot F_{X_{3}}(x_{3})}  [{\displaystyle F_{X_{1},X_{3}}(x_{1},x_{3})=F_{X_
{1}}(x_{1})\cdot F_{X_{3}}(x_{3})}].
The measure-theoretically inclined may prefer to substitute events     { X
&#x2208; A }   {\displaystyle \{X\in A\}}  [{\displaystyle \{X\in A\}}] for
events     { X &#x2264; x }   {\displaystyle \{X\leq x\}}  [\{X\leq x\}] in the
above definition, where     A   {\displaystyle A}  [A] is any Borel_set. That
definition is exactly equivalent to the one above when the values of the random
variables are real_numbers. It has the advantage of working also for complex-
valued random variables or for random variables taking values in any measurable
space (which includes topological_spaces endowed by appropriate Ï-algebras).
**** For real valued random vectors[edit] ****
Two random vectors      X  = (  X  1   , . . . ,  X  m    )  T
{\displaystyle \mathbf {X} =(X_{1},...,X_{m})^{T}}  [{\displaystyle \mathbf {X}
=(X_{1},...,X_{m})^{T}}] and      Y  = (  Y  1   , . . . ,  Y  n    )  T
{\displaystyle \mathbf {Y} =(Y_{1},...,Y_{n})^{T}}  [{\displaystyle \mathbf {Y}
=(Y_{1},...,Y_{n})^{T}}] are called independent if[5]:p. 187
    F   X , Y    (  x , y  ) =  F   X    (  x  ) &#x22C5;  F   Y
(  y  )   for all&#xA0;   x  ,  y    {\displaystyle F_{\mathbf
{X,Y} }(\mathbf {x,y} )=F_{\mathbf {X} }(\mathbf {x} )\cdot F_        
{\mathbf {Y} }(\mathbf {y} )\quad {\text{for all }}\mathbf {x}          (Eq.6)
,\mathbf {y} }  [{\displaystyle F_{\mathbf {X,Y} }(\mathbf {x,y}
)=F_{\mathbf {X} }(\mathbf {x} )\cdot F_{\mathbf {Y} }(\mathbf {y}
)\quad {\text{for all }}\mathbf {x} ,\mathbf {y} }]
where      F   X    (  x  )   {\displaystyle F_{\mathbf {X} }(\mathbf {x} )}  [
{\displaystyle F_{\mathbf {X} }(\mathbf {x} )}] and      F   Y    (  y  )
{\displaystyle F_{\mathbf {Y} }(\mathbf {y} )}  [{\displaystyle F_{\mathbf {Y}
}(\mathbf {y} )}] denote the cumulative distribution functions of      X
{\displaystyle \mathbf {X} }  [\mathbf {X} ] and      Y    {\displaystyle
\mathbf {Y} }  [\mathbf {Y} ] and      F   X , Y    (  x , y  )
{\displaystyle F_{\mathbf {X,Y} }(\mathbf {x,y} )}  [{\displaystyle F_{\mathbf
{X,Y} }(\mathbf {x,y} )}] denotes their joint cumulative distribution function.
Independence of      X    {\displaystyle \mathbf {X} }  [\mathbf {X} ] and
Y    {\displaystyle \mathbf {Y} }  [\mathbf {Y} ] is often denoted by      X
&#x22A5;    &#x22A5;  Y    {\displaystyle \mathbf {X} \perp \!\!\!\perp \mathbf
{Y} }  [{\displaystyle \mathbf {X} \perp \!\!\!\perp \mathbf {Y} }]. Written
component-wise,      X    {\displaystyle \mathbf {X} }  [\mathbf {X} ] and
Y    {\displaystyle \mathbf {Y} }  [\mathbf {Y} ] are called independent if
          F   X  1   , &#x2026; ,  X  m   ,  Y  1   , &#x2026; ,  Y  n     (  x
      1   , &#x2026; ,  x  m   ,  y  1   , &#x2026; ,  y  n   ) =  F   X  1   ,
      &#x2026; ,  X  m     (  x  1   , &#x2026; ,  x  m   ) &#x22C5;  F   Y  1
      , &#x2026; ,  Y  n     (  y  1   , &#x2026; ,  y  n   )   for all&#xA0;
      x  1   , &#x2026; ,  x  m   ,  y  1   , &#x2026; ,  y  n
      {\displaystyle F_{X_{1},\ldots ,X_{m},Y_{1},\ldots ,Y_{n}}(x_{1},\ldots
      ,x_{m},y_{1},\ldots ,y_{n})=F_{X_{1},\ldots ,X_{m}}(x_{1},\ldots ,x_
      {m})\cdot F_{Y_{1},\ldots ,Y_{n}}(y_{1},\ldots ,y_{n})\quad {\text{for
      all }}x_{1},\ldots ,x_{m},y_{1},\ldots ,y_{n}}  [{\displaystyle F_{X_
      {1},\ldots ,X_{m},Y_{1},\ldots ,Y_{n}}(x_{1},\ldots ,x_{m},y_{1},\ldots
      ,y_{n})=F_{X_{1},\ldots ,X_{m}}(x_{1},\ldots ,x_{m})\cdot F_{Y_{1},\ldots
      ,Y_{n}}(y_{1},\ldots ,y_{n})\quad {\text{for all }}x_{1},\ldots ,x_{m},y_
      {1},\ldots ,y_{n}}].
**** For stochastic processes[edit] ****
*** For one stochastic process[edit] ***
The definition of independence may be extended from random vectors to a
stochastic_process. Thereby it is required for an independent stochastic
process that the random variables obtained by sampling the process at any     n
{\displaystyle n}  [n] times      t  1   , &#x2026; ,  t  n     {\displaystyle
t_{1},\ldots ,t_{n}}  [t_{1},\ldots ,t_{n}] are independent random variables
for any     n   {\displaystyle n}  [n].[6]:p. 163
Formally, a stochastic process       {  X  t   }   t &#x2208;   T
{\displaystyle \left\{X_{t}\right\}_{t\in {\mathcal {T}}}}  [{\displaystyle
\left\{X_{t}\right\}_{t\in {\mathcal {T}}}}] is called independent, if and only
if for all     n &#x2208;  N    {\displaystyle n\in \mathbb {N} }  [n\in
\mathbb{N}] and for all      t  1   , &#x2026; ,  t  n   &#x2208;   T
{\displaystyle t_{1},\ldots ,t_{n}\in {\mathcal {T}}}  [{\displaystyle t_
{1},\ldots ,t_{n}\in {\mathcal {T}}}]
    F   X   t  1     , &#x2026; ,  X   t  n       (  x  1   ,
&#x2026; ,  x  n   ) =  F   X   t  1       (  x  1   ) &#x22C5;
&#x2026; &#x22C5;  F   X   t  n       (  x  n   )   for all&#xA0;
x  1   , &#x2026; ,  x  n     {\displaystyle F_{X_{t_{1}},\ldots      
,X_{t_{n}}}(x_{1},\ldots ,x_{n})=F_{X_{t_{1}}}(x_{1})\cdot \ldots       (Eq.7)
\cdot F_{X_{t_{n}}}(x_{n})\quad {\text{for all }}x_{1},\ldots ,x_
{n}}  [{\displaystyle F_{X_{t_{1}},\ldots ,X_{t_{n}}}(x_{1},\ldots
,x_{n})=F_{X_{t_{1}}}(x_{1})\cdot \ldots \cdot F_{X_{t_{n}}}(x_
{n})\quad {\text{for all }}x_{1},\ldots ,x_{n}}]
where      F   X   t  1     , &#x2026; ,  X   t  n       (  x  1   , &#x2026; ,
x  n   ) =  P  ( X (  t  1   ) &#x2264;  x  1   , &#x2026; , X (  t  n   )
&#x2264;  x  n   )   {\displaystyle F_{X_{t_{1}},\ldots ,X_{t_{n}}}(x_
{1},\ldots ,x_{n})=\mathrm {P} (X(t_{1})\leq x_{1},\ldots ,X(t_{n})\leq x_{n})}
[{\displaystyle F_{X_{t_{1}},\ldots ,X_{t_{n}}}(x_{1},\ldots ,x_{n})=\mathrm
{P} (X(t_{1})\leq x_{1},\ldots ,X(t_{n})\leq x_{n})}]. Notice that independence
of a stochastic process is a property within a stochastic process, not between
two stochastic processes.
*** For two stochastic processes[edit] ***
Independence of two stochastic processes is a property between two stochastic
processes       {  X  t   }   t &#x2208;   T       {\displaystyle \left\{X_
{t}\right\}_{t\in {\mathcal {T}}}}  [{\displaystyle \left\{X_{t}\right\}_{t\in
{\mathcal {T}}}}] and       {  Y  t   }   t &#x2208;   T       {\displaystyle
\left\{Y_{t}\right\}_{t\in {\mathcal {T}}}}  [{\displaystyle \left\{Y_
{t}\right\}_{t\in {\mathcal {T}}}}] that are defined on the same probability
space     ( &#x03A9; ,   F   , P )   {\displaystyle (\Omega ,{\mathcal {F}},P)}
[(\Omega ,{\mathcal {F}},P)]. Formally, two stochastic processes       {  X  t
}   t &#x2208;   T       {\displaystyle \left\{X_{t}\right\}_{t\in {\mathcal
{T}}}}  [{\displaystyle \left\{X_{t}\right\}_{t\in {\mathcal {T}}}}] and
{  Y  t   }   t &#x2208;   T       {\displaystyle \left\{Y_{t}\right\}_{t\in
{\mathcal {T}}}}  [{\displaystyle \left\{Y_{t}\right\}_{t\in {\mathcal {T}}}}]
are said to be independent if for all     n &#x2208;  N    {\displaystyle n\in
\mathbb {N} }  [n\in \mathbb{N}] and for all      t  1   , &#x2026; ,  t  n
&#x2208;   T     {\displaystyle t_{1},\ldots ,t_{n}\in {\mathcal {T}}}  [
{\displaystyle t_{1},\ldots ,t_{n}\in {\mathcal {T}}}], the random vectors
( X (  t  1   ) , &#x2026; , X (  t  n   ) )   {\displaystyle (X(t_{1}),\ldots
,X(t_{n}))}  [{\displaystyle (X(t_{1}),\ldots ,X(t_{n}))}] and     ( Y (  t  1
) , &#x2026; , Y (  t  n   ) )   {\displaystyle (Y(t_{1}),\ldots ,Y(t_{n}))}  [
{\displaystyle (Y(t_{1}),\ldots ,Y(t_{n}))}] are independent,[7]:p. 515 i.e. if
    F   X   t  1     , &#x2026; ,  X   t  n     ,  Y   t  1     ,
&#x2026; ,  Y   t  n       (  x  1   , &#x2026; ,  x  n   ,  y  1
, &#x2026; ,  y  n   ) =  F   X   t  1     , &#x2026; ,  X   t  n
(  x  1   , &#x2026; ,  x  n   ) &#x22C5;  F   Y   t  1     ,
&#x2026; ,  Y   t  n       (  y  1   , &#x2026; ,  y  n   )   for
all&#xA0;   x  1   , &#x2026; ,  x  n     {\displaystyle F_{X_{t_
{1}},\ldots ,X_{t_{n}},Y_{t_{1}},\ldots ,Y_{t_{n}}}(x_{1},\ldots      
,x_{n},y_{1},\ldots ,y_{n})=F_{X_{t_{1}},\ldots ,X_{t_{n}}}(x_          (Eq.8)
{1},\ldots ,x_{n})\cdot F_{Y_{t_{1}},\ldots ,Y_{t_{n}}}(y_
{1},\ldots ,y_{n})\quad {\text{for all }}x_{1},\ldots ,x_{n}}  [
{\displaystyle F_{X_{t_{1}},\ldots ,X_{t_{n}},Y_{t_{1}},\ldots ,Y_
{t_{n}}}(x_{1},\ldots ,x_{n},y_{1},\ldots ,y_{n})=F_{X_{t_
{1}},\ldots ,X_{t_{n}}}(x_{1},\ldots ,x_{n})\cdot F_{Y_{t_
{1}},\ldots ,Y_{t_{n}}}(y_{1},\ldots ,y_{n})\quad {\text{for all
}}x_{1},\ldots ,x_{n}}]
**** Independent σ-algebras[edit] ****
The definitions above (Eq.1 and Eq.2) are both generalized by the following
definition of independence for σ-algebras. Let     ( &#x03A9; , &#x03A3; ,  P
)   {\displaystyle (\Omega ,\Sigma ,\mathrm {P} )}  [{\displaystyle (\Omega
,\Sigma ,\mathrm {P} )}] be a probability space and let       A
{\displaystyle {\mathcal {A}}}  [{\mathcal {A}}] and       B     {\displaystyle
{\mathcal {B}}}  [{\mathcal {B}}] be two sub-Ï-algebras of     &#x03A3;
{\displaystyle \Sigma }  [\Sigma ].       A     {\displaystyle {\mathcal {A}}}
[{\mathcal {A}}] and       B     {\displaystyle {\mathcal {B}}}  [{\mathcal
{B}}] are said to be independent if, whenever     A &#x2208;   A
{\displaystyle A\in {\mathcal {A}}}  [A\in {\mathcal {A}}] and     B &#x2208;
B     {\displaystyle B\in {\mathcal {B}}}  [B\in {\mathcal {B}}],
          P  ( A &#x2229; B ) =  P  ( A )  P  ( B ) .   {\displaystyle \mathrm
      {P} (A\cap B)=\mathrm {P} (A)\mathrm {P} (B).}  [\mathrm{P}(A \cap B) =
      \mathrm{P}(A) \mathrm{P}(B).]
Likewise, a finite family of Ï-algebras     (  &#x03C4;  i    )  i &#x2208; I
{\displaystyle (\tau _{i})_{i\in I}}  [(\tau_i)_{i\in I}], where     I
{\displaystyle I}  [I] is an index_set, is said to be independent if and only
if
         &#x2200;   (  A  i   )   i &#x2208; I   &#x2208;  &#x220F;  i &#x2208;
      I    &#x03C4;  i   &#xA0; : &#xA0;  P   (   &#x22C2;  i &#x2208; I    A
      i    )  =  &#x220F;  i &#x2208; I    P   (  A  i   )    {\displaystyle
      \forall \left(A_{i}\right)_{i\in I}\in \prod \nolimits _{i\in I}\tau _
      {i}\ :\ \mathrm {P} \left(\bigcap \nolimits _{i\in I}A_{i}\right)=\prod
      \nolimits _{i\in I}\mathrm {P} \left(A_{i}\right)}  [\forall \left
      (A_i\right)_{i\in I} \in \prod\nolimits_{i\in I}\tau_i \ : \ \mathrm
      {P}\left(\bigcap\nolimits_{i\in I}A_i\right) = \prod\nolimits_{i\in
      I}\mathrm{P}\left(A_i\right)]
and an infinite family of σ-algebras is said to be independent if all its
finite subfamilies are independent.
The new definition relates to the previous ones very directly:
    * Two events are independent (in the old sense) if_and_only_if the Ï-
      algebras that they generate are independent (in the new sense). The Ï-
      algebra generated by an event     E &#x2208; &#x03A3;   {\displaystyle
      E\in \Sigma }  [E\in \Sigma ] is, by definition,
               &#x03C3; ( { E } ) = { &#x2205; , E , &#x03A9; &#x2216; E ,
            &#x03A9; } .   {\displaystyle \sigma (\{E\})=\{\emptyset ,E,\Omega
            \setminus E,\Omega \}.}  [\sigma (\{E\})=\{\emptyset ,E,\Omega
            \setminus E,\Omega \}.]
    * Two random variables     X   {\displaystyle X}  [X] and     Y
      {\displaystyle Y}  [Y] defined over     &#x03A9;   {\displaystyle \Omega
      }  [\Omega ] are independent (in the old sense) if and only if the Ï-
      algebras that they generate are independent (in the new sense). The Ï-
      algebra generated by a random variable     X   {\displaystyle X}  [X]
      taking values in some measurable_space     S   {\displaystyle S}  [S]
      consists, by definition, of all subsets of     &#x03A9;   {\displaystyle
      \Omega }  [\Omega ] of the form      X  &#x2212; 1   ( U )
      {\displaystyle X^{-1}(U)}  [{\displaystyle X^{-1}(U)}], where     U
      {\displaystyle U}  [U] is any measurable subset of     S   {\displaystyle
      S}  [S].
Using this definition, it is easy to show that if     X   {\displaystyle X}
[X] and     Y   {\displaystyle Y}  [Y] are random variables and     Y
{\displaystyle Y}  [Y] is constant, then     X   {\displaystyle X}  [X] and
Y   {\displaystyle Y}  [Y] are independent, since the Ï-algebra generated by a
constant random variable is the trivial Ï-algebra     { &#x2205; , &#x03A9; }
{\displaystyle \{\varnothing ,\Omega \}}  [{\displaystyle \{\varnothing ,\Omega
\}}]. Probability zero events cannot affect independence so independence also
holds if     Y   {\displaystyle Y}  [Y] is only Pr-almost_surely constant.
***** Properties[edit] *****
**** Self-independence[edit] ****
Note that an event is independent of itself if and only if
          P  ( A ) =  P  ( A &#x2229; A ) =  P  ( A ) &#x22C5;  P  ( A )
      &#x21D4;  P  ( A ) = 0  &#xA0;or&#xA0;   P  ( A ) = 1   {\displaystyle
      \mathrm {P} (A)=\mathrm {P} (A\cap A)=\mathrm {P} (A)\cdot \mathrm {P}
      (A)\Leftrightarrow \mathrm {P} (A)=0{\text{ or }}\mathrm {P} (A)=1}  [
      {\displaystyle \mathrm {P} (A)=\mathrm {P} (A\cap A)=\mathrm {P} (A)\cdot
      \mathrm {P} (A)\Leftrightarrow \mathrm {P} (A)=0{\text{ or }}\mathrm {P}
      (A)=1}].
Thus an event is independent of itself if and only if it almost_surely occurs
or its complement almost surely occurs; this fact is useful when proving
zeroâone_laws.[8]
**** Expectation and covariance[edit] ****
Main article: Correlation_and_dependence
If     X   {\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y] are
independent random variables, then the expectation_operator     E
{\displaystyle \operatorname {E} }  [\operatorname {E} ] has the property
         E &#x2061; [ X Y ] = E &#x2061; [ X ] E &#x2061; [ Y ] ,
      {\displaystyle \operatorname {E} [XY]=\operatorname {E} [X]\operatorname
      {E} [Y],}  [{\displaystyle \operatorname {E} [XY]=\operatorname {E}
      [X]\operatorname {E} [Y],}]
and the covariance     cov &#x2061; [ X , Y ]   {\displaystyle \operatorname
{cov} [X,Y]}  [{\displaystyle \operatorname {cov} [X,Y]}] is zero, since we
have
         cov &#x2061; [ X , Y ] = E &#x2061; [ X Y ] &#x2212; E &#x2061; [ X ]
      E &#x2061; [ Y ]   {\displaystyle \operatorname {cov} [X,Y]=\operatorname
      {E} [XY]-\operatorname {E} [X]\operatorname {E} [Y]}  [{\displaystyle
      \operatorname {cov} [X,Y]=\operatorname {E} [XY]-\operatorname {E}
      [X]\operatorname {E} [Y]}].
(The converse of these, i.e. the proposition that if two random variables have
a covariance of 0 they must be independent, is not true. See uncorrelated.)
Similarly for two stochastic processes       {  X  t   }   t &#x2208;   T
{\displaystyle \left\{X_{t}\right\}_{t\in {\mathcal {T}}}}  [{\displaystyle
\left\{X_{t}\right\}_{t\in {\mathcal {T}}}}] and       {  Y  t   }   t &#x2208;
T       {\displaystyle \left\{Y_{t}\right\}_{t\in {\mathcal {T}}}}  [
{\displaystyle \left\{Y_{t}\right\}_{t\in {\mathcal {T}}}}]: If they are
independent, then they are uncorrelated.[9]:p. 151
**** Characteristic function[edit] ****
Two random variables     X   {\displaystyle X}  [X] and     Y   {\displaystyle
Y}  [Y] are independent if and only if the characteristic_function of the
random vector     ( X , Y )   {\displaystyle (X,Y)}  [(X,Y)] satisfies
          &#x03C6;  ( X , Y )   ( t , s ) =  &#x03C6;  X   ( t ) &#x22C5;
      &#x03C6;  Y   ( s )   {\displaystyle \varphi _{(X,Y)}(t,s)=\varphi _{X}
      (t)\cdot \varphi _{Y}(s)}  [{\displaystyle \varphi _{(X,Y)}(t,s)=\varphi
      _{X}(t)\cdot \varphi _{Y}(s)}].
In particular the characteristic function of their sum is the product of their
marginal characteristic functions:
          &#x03C6;  X + Y   ( t ) =  &#x03C6;  X   ( t ) &#x22C5;  &#x03C6;  Y
      ( t ) ,   {\displaystyle \varphi _{X+Y}(t)=\varphi _{X}(t)\cdot \varphi _
      {Y}(t),}  [\varphi_{X+Y}(t) = \varphi_X(t)\cdot\varphi_Y(t),]
though the reverse implication is not true. Random variables that satisfy the
latter condition are called subindependent.
***** Examples[edit] *****
**** Rolling dice[edit] ****
The event of getting a 6 the first time a die is rolled and the event of
getting a 6 the second time are independent. By contrast, the event of getting
a 6 the first time a die is rolled and the event that the sum of the numbers
seen on the first and second trial is 8 are not independent.
**** Drawing cards[edit] ****
If two cards are drawn with replacement from a deck of cards, the event of
drawing a red card on the first trial and that of drawing a red card on the
second trial are independent. By contrast, if two cards are drawn without
replacement from a deck of cards, the event of drawing a red card on the first
trial and that of drawing a red card on the second trial are not independent,
because a deck that has had a red card removed has proportionately fewer red
cards.
**** Pairwise and mutual independence[edit] ****
Pairwise independent, but not mutually independent, events.
Mutually independent events.
Consider the two probability spaces shown. In both cases,      P  ( A ) =  P
( B ) = 1  /  2   {\displaystyle \mathrm {P} (A)=\mathrm {P} (B)=1/2}  [
{\displaystyle \mathrm {P} (A)=\mathrm {P} (B)=1/2}] and      P  ( C ) = 1  /
4   {\displaystyle \mathrm {P} (C)=1/4}  [{\displaystyle \mathrm {P} (C)=1/4}].
The random variables in the first space are pairwise independent because      P
( A  |  B ) =  P  ( A  |  C ) = 1  /  2 =  P  ( A )   {\displaystyle \mathrm
{P} (A|B)=\mathrm {P} (A|C)=1/2=\mathrm {P} (A)}  [{\displaystyle \mathrm {P}
(A|B)=\mathrm {P} (A|C)=1/2=\mathrm {P} (A)}],      P  ( B  |  A ) =  P  ( B  |
C ) = 1  /  2 =  P  ( B )   {\displaystyle \mathrm {P} (B|A)=\mathrm {P}
(B|C)=1/2=\mathrm {P} (B)}  [{\displaystyle \mathrm {P} (B|A)=\mathrm {P}
(B|C)=1/2=\mathrm {P} (B)}], and      P  ( C  |  A ) =  P  ( C  |  B ) = 1  /
4 =  P  ( C )   {\displaystyle \mathrm {P} (C|A)=\mathrm {P} (C|B)=1/4=\mathrm
{P} (C)}  [{\displaystyle \mathrm {P} (C|A)=\mathrm {P} (C|B)=1/4=\mathrm {P}
(C)}]; but the three random variables are not mutually independent. The random
variables in the second space are both pairwise independent and mutually
independent. To illustrate the difference, consider conditioning on two events.
In the pairwise independent case, although any one event is independent of each
of the other two individually, it is not independent of the intersection of the
other two:
          P  ( A  |  B C ) =    4 40     4 40   +   1 40      =    4 5
      &#x2260;  P  ( A )   {\displaystyle \mathrm {P} (A|BC)={\frac {\frac {4}
      {40}}{{\frac {4}{40}}+{\frac {1}{40}}}}={\tfrac {4}{5}}\neq \mathrm {P}
      (A)}  [\mathrm{P}(A|BC) = \frac{\frac{4}{40}}{\frac{4}{40} + \frac{1}
      {40}} = \tfrac{4}{5} \ne \mathrm{P}(A)]
          P  ( B  |  A C ) =    4 40     4 40   +   1 40      =    4 5
      &#x2260;  P  ( B )   {\displaystyle \mathrm {P} (B|AC)={\frac {\frac {4}
      {40}}{{\frac {4}{40}}+{\frac {1}{40}}}}={\tfrac {4}{5}}\neq \mathrm {P}
      (B)}  [\mathrm{P}(B|AC) = \frac{\frac{4}{40}}{\frac{4}{40} + \frac{1}
      {40}} = \tfrac{4}{5} \ne \mathrm{P}(B)]
          P  ( C  |  A B ) =    4 40     4 40   +   6 40      =    2 5
      &#x2260;  P  ( C )   {\displaystyle \mathrm {P} (C|AB)={\frac {\frac {4}
      {40}}{{\frac {4}{40}}+{\frac {6}{40}}}}={\tfrac {2}{5}}\neq \mathrm {P}
      (C)}  [\mathrm{P}(C|AB) = \frac{\frac{4}{40}}{\frac{4}{40} + \frac{6}
      {40}} = \tfrac{2}{5} \ne \mathrm{P}(C)]
In the mutually independent case, however,
          P  ( A  |  B C ) =    1 16     1 16   +   1 16      =    1 2    =  P
      ( A )   {\displaystyle \mathrm {P} (A|BC)={\frac {\frac {1}{16}}{{\frac
      {1}{16}}+{\frac {1}{16}}}}={\tfrac {1}{2}}=\mathrm {P} (A)}  [\mathrm{P}
      (A|BC) = \frac{\frac{1}{16}}{\frac{1}{16} + \frac{1}{16}} = \tfrac{1}{2}
      = \mathrm{P}(A)]
          P  ( B  |  A C ) =    1 16     1 16   +   1 16      =    1 2    =  P
      ( B )   {\displaystyle \mathrm {P} (B|AC)={\frac {\frac {1}{16}}{{\frac
      {1}{16}}+{\frac {1}{16}}}}={\tfrac {1}{2}}=\mathrm {P} (B)}  [\mathrm{P}
      (B|AC) = \frac{\frac{1}{16}}{\frac{1}{16} + \frac{1}{16}} = \tfrac{1}{2}
      = \mathrm{P}(B)]
          P  ( C  |  A B ) =    1 16     1 16   +   3 16      =    1 4    =  P
      ( C )   {\displaystyle \mathrm {P} (C|AB)={\frac {\frac {1}{16}}{{\frac
      {1}{16}}+{\frac {3}{16}}}}={\tfrac {1}{4}}=\mathrm {P} (C)}  [\mathrm{P}
      (C|AB) = \frac{\frac{1}{16}}{\frac{1}{16} + \frac{3}{16}} = \tfrac{1}{4}
      = \mathrm{P}(C)]
**** Mutual independence[edit] ****
It is possible to create a three-event example in which
          P  ( A &#x2229; B &#x2229; C ) =  P  ( A )  P  ( B )  P  ( C ) ,
      {\displaystyle \mathrm {P} (A\cap B\cap C)=\mathrm {P} (A)\mathrm {P}
      (B)\mathrm {P} (C),}  [\mathrm{P}(A \cap B \cap C) = \mathrm{P}(A)\mathrm
      {P}(B)\mathrm{P}(C),]
and yet no two of the three events are pairwise independent (and hence the set
of events are not mutually independent).[10] This example shows that mutual
independence involves requirements on the products of probabilities of all
combinations of events, not just the single events as in this example. For
another example, take     A   {\displaystyle A}  [A] to be empty and     B
{\displaystyle B}  [B] and     C   {\displaystyle C}  [C ] to be identical
events with non-zero probability. Then, since     B   {\displaystyle B}  [B]
and     C   {\displaystyle C}  [C ] are the same event, they are not
independent, but the probability of the intersection of the events is zero, the
product of the probabilities.
***** Conditional independence[edit] *****
Main article: Conditional_independence
**** For events[edit] ****
The events     A   {\displaystyle A}  [A] and     B   {\displaystyle B}  [B]
are conditionally independent given an event     C   {\displaystyle C}  [C]
when
    P  ( A &#x2229; B &#x2223; C ) =  P  ( A &#x2223; C ) &#x22C5;  P  ( B
&#x2223; C )   {\displaystyle \mathrm {P} (A\cap B\mid C)=\mathrm {P} (A\mid
C)\cdot \mathrm {P} (B\mid C)}  [{\displaystyle \mathrm {P} (A\cap B\mid
C)=\mathrm {P} (A\mid C)\cdot \mathrm {P} (B\mid C)}].
**** For random variables[edit] ****
Intuitively, two random variables     X   {\displaystyle X}  [X] and     Y
{\displaystyle Y}  [Y] are conditionally independent given     Z
{\displaystyle Z}  [Z] if, once     Z   {\displaystyle Z}  [Z] is known, the
value of     Y   {\displaystyle Y}  [Y] does not add any additional information
about     X   {\displaystyle X}  [X]. For instance, two measurements     X
{\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y] of the same
underlying quantity     Z   {\displaystyle Z}  [Z] are not independent, but
they are conditionally independent given     Z   {\displaystyle Z}  [Z] (unless
the errors in the two measurements are somehow connected).
The formal definition of conditional independence is based on the idea of
conditional_distributions. If     X   {\displaystyle X}  [X],     Y
{\displaystyle Y}  [Y], and     Z   {\displaystyle Z}  [Z] are discrete_random
variables, then we define     X   {\displaystyle X}  [X] and     Y
{\displaystyle Y}  [Y] to be conditionally independent given     Z
{\displaystyle Z}  [Z] if
          P  ( X &#x2264; x , Y &#x2264; y   |   Z = z ) =  P  ( X &#x2264; x
      |   Z = z ) &#x22C5;  P  ( Y &#x2264; y   |   Z = z )   {\displaystyle
      \mathrm {P} (X\leq x,Y\leq y\;|\;Z=z)=\mathrm {P} (X\leq x\;|\;Z=z)\cdot
      \mathrm {P} (Y\leq y\;|\;Z=z)}  [\mathrm{P}(X \le x, Y \le y\;|\;Z = z) =
      \mathrm{P}(X \le x\;|\;Z = z) \cdot \mathrm{P}(Y \le y\;|\;Z = z)]
for all     x   {\displaystyle x}  [x],     y   {\displaystyle y}  [y] and
z   {\displaystyle z}  [z] such that      P  ( Z = z ) > 0   {\displaystyle
\mathrm {P} (Z=z)>0}  [{\displaystyle \mathrm {P} (Z=z)>0}]. On the other hand,
if the random variables are continuous and have a joint probability_density
function      f  X Y Z   ( x , y , z )   {\displaystyle f_{XYZ}(x,y,z)}  [
{\displaystyle f_{XYZ}(x,y,z)}], then     X   {\displaystyle X}  [X] and     Y
{\displaystyle Y}  [Y] are conditionally_independent given     Z
{\displaystyle Z}  [Z] if
          f  X Y  |  Z   ( x , y  |  z ) =  f  X  |  Z   ( x  |  z ) &#x22C5;
      f  Y  |  Z   ( y  |  z )   {\displaystyle f_{XY|Z}(x,y|z)=f_{X|Z}
      (x|z)\cdot f_{Y|Z}(y|z)}  [{\displaystyle f_{XY|Z}(x,y|z)=f_{X|Z}
      (x|z)\cdot f_{Y|Z}(y|z)}]
for all real numbers     x   {\displaystyle x}  [x],     y   {\displaystyle y}
[y] and     z   {\displaystyle z}  [z] such that      f  Z   ( z ) > 0
{\displaystyle f_{Z}(z)>0}  [{\displaystyle f_{Z}(z)>0}].
If discrete     X   {\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y]
are conditionally independent given     Z   {\displaystyle Z}  [Z], then
          P  ( X = x  |  Y = y , Z = z ) =  P  ( X = x  |  Z = z )
      {\displaystyle \mathrm {P} (X=x|Y=y,Z=z)=\mathrm {P} (X=x|Z=z)}  [\mathrm
      {P}(X = x | Y = y , Z = z) = \mathrm{P}(X = x | Z = z)]
for any     x   {\displaystyle x}  [x],     y   {\displaystyle y}  [y] and
z   {\displaystyle z}  [z] with      P  ( Z = z ) > 0   {\displaystyle \mathrm
{P} (Z=z)>0}  [{\displaystyle \mathrm {P} (Z=z)>0}]. That is, the conditional
distribution for     X   {\displaystyle X}  [X] given     Y   {\displaystyle Y}
[Y] and     Z   {\displaystyle Z}  [Z] is the same as that given     Z
{\displaystyle Z}  [Z] alone. A similar equation holds for the conditional
probability density functions in the continuous case.
Independence can be seen as a special kind of conditional independence, since
probability can be seen as a kind of conditional probability given no events.
***** See also[edit] *****
    * Copula_(statistics)
    * Independent_and_identically_distributed_random_variables
    * Mutually_exclusive_events
    * Subindependence
    * Conditional_independence
    * Normally_distributed_and_uncorrelated_does_not_imply_independent
    * Mean_dependence
***** References[edit] *****
   1. ^Russell, Stuart; Norvig, Peter (2002). Artificial Intelligence: A Modern
      Approach. Prentice_Hall. p. 478. ISBN 0-13-790395-2.
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
   3. ^ a bFlorescu, Ionut (2014). Probability and Stochastic Processes. Wiley.
      ISBN 978-0-470-62455-5.
   4. ^ a b c dGallager, Robert G. (2013). Stochastic Processes Theory for
      Applications. Cambridge University Press. ISBN 978-1-107-03975-9.
   5. ^ a bFeller, W (1971). "Stochastic Independence". An Introduction to
      Probability Theory and Its Applications. Wiley.
   6. ^Papoulis, Athanasios (1991). Probability, Random Variables and
      Stochastic Porcesses. MCGraw Hill. ISBN 0-07-048477-5.
   7. ^Hwei, Piao (1997). Theory and Problems of Probability, Random Variables,
      and Random Processes. McGraw-Hill. ISBN 0-07-030644-3.
   8. ^Amos Lapidoth (8 February 2017). A_Foundation_in_Digital_Communication.
      Cambridge University Press. ISBN 978-1-107-17732-1.
   9. ^Durrett,_Richard (1996). Probability: theory and examples (Second ed.).
  10.  page 62
  11. ^Park,Kun Il (2018). Fundamentals of Probability and Stochastic Processes
      with Applications to Communications. Springer. ISBN 978-3-319-68074-3.
  12. ^ George, Glyn, "Testing for the independence of three events,"
      Mathematical Gazette 88, November 2004, 568. PDF
***** External links[edit] *****
    *  Media related to Statistical_dependence at Wikimedia Commons

Retrieved from "https://en.wikipedia.org/w/index.php?title=Independence_
(probability_theory)&oldid=889300352"
Categories:
    * Experiment_(probability_theory)
    * Independence_(probability_theory)
Hidden categories:
    * Commons_category_link_from_Wikidata
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
    * CatalÃ 
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÅ¡Äina
    * Basa_Sunda
    * Suomi
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 24 March 2019, at 20:34 (UTC).
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
