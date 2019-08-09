The following text has been accessed from https://en.wikipedia.org/wiki/Conditional_probability at Fri Aug 9 02:44:01 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Conditional probability ******
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
    * Conditional probability
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
In probability_theory, conditional probability is a measure of the probability
of an event occurring given that another event has occurred.[1] If the event of
interest is A and the event B is known or assumed to have occurred, "the
conditional probability of A given B", or "the probability of A under the
condition B", is usually written as P(A | B), or sometimes PB(A) or P(A / B).
For example, the probability that any given person has a cough on any given day
may be only 5%. But if we know or assume that the person has a cold, then they
are much more likely to be coughing. The conditional probability of coughing by
the unwell might be 75%, then: P(Cough) = 5%; P(Cough | Sick) = 75%
The concept of conditional probability is one of the most fundamental and one
of the most important in probability theory.[2] But conditional probabilities
can be quite slippery and require careful interpretation.[3] For example, there
need not be a causal relationship between A and B, and they don't have to occur
simultaneously.
P(A | B) may or may not be equal to P(A) (the unconditional probability of A).
If P(A | B) = P(A), then events A and B are said to be "independent": in such a
case, knowledge about either event does not give information on the other. P
(A | B) (the conditional probability of A given B) typically differs from P
(B | A). For example, if a person has dengue, they might have a 90% chance of
testing positive for dengue. In this case what is being measured is that if
event B ("having dengue") has occurred, the probability of A (test is positive)
given that B (having dengue) occurred is 90%: that is, P(A | B) = 90%.
Alternatively, if a person tests positive for dengue they may have only a 15%
chance of actually having this rare disease because the false_positive rate for
the test may be high. In this case what is being measured is the probability of
the event B (having dengue) given that the event A (test is positive) has
occurred: P(B | A) = 15%. Falsely equating the two probabilities causes various
errors of reasoning such as the base_rate_fallacy. Conditional probabilities
can be reversed using Bayes'_theorem.
Conditional probabilities can be displayed in a conditional_probability_table.
⁰
***** Contents *****
    * 1_Definition
          o 1.1_Conditioning_on_an_event
                # 1.1.1_Kolmogorov_definition
                # 1.1.2_As_an_axiom_of_probability
                # 1.1.3_As_the_probability_of_a_conditional_event
          o 1.2_Measure-theoretic_definition
          o 1.3_Conditioning_on_a_random_variable
          o 1.4_Partial_conditional_probability
    * 2_Example
    * 3_Use_in_inference
    * 4_Statistical_independence
    * 5_Common_fallacies
          o 5.1_Assuming_conditional_probability_is_of_similar_size_to_its
            inverse
          o 5.2_Assuming_marginal_and_conditional_probabilities_are_of_similar
            size
          o 5.3_Over-_or_under-weighting_priors
    * 6_Formal_derivation
    * 7_See_also
    * 8_References
    * 9_External_links
***** Definition[edit] *****
Illustration of conditional probabilities with an Euler_diagram. The
unconditional probability P(A) = 0.30 + 0.10 + 0.12 = 0.52. However, the
conditional probability P(A|B1) = 1, P(A|B2) = 0.12 Ã· (0.12 + 0.04) = 0.75,
and P(A|B3) = 0.
On a tree_diagram, branch probabilities are conditional on the event associated
with the parent node. (Here the overbars indicate that the event does not
occur.)
Venn Pie Chart describing conditional probabilities
**** Conditioning on an event[edit] ****
*** Kolmogorov definition[edit] ***
Given two events A and B, from the sigma-field of a probability space, with the
unconditional_probability of B (that is, of the event B occurring ) being
greater than zero, P(B) > 0, the conditional probability of A given B is
defined as the quotient of the probability of the joint of events A and B, and
the probability of B:[4]
         P ( A &#x2223; B ) =    P ( A &#x2229; B )   P ( B )    ,
      {\displaystyle P(A\mid B)={\frac {P(A\cap B)}{P(B)}},}  [{\displaystyle P
      (A\mid B)={\frac {P(A\cap B)}{P(B)}},}]
where     P ( A &#x2229; B )   {\displaystyle P(A\cap B)}  [P(A\cap B)] is the
probability that both events A and B occur. This may be visualized as
restricting the sample space to situations in which B occurs. The logic behind
this equation is that if the possible outcomes for A and B are restricted to
those in which B occurs, this set serves as the new sample space.
Note that this is a definition but not a theoretical result. We just denote the
quantity        P ( A &#x2229; B )   P ( B )      {\displaystyle {\frac {P
(A\cap B)}{P(B)}}}  [{\displaystyle {\frac {P(A\cap B)}{P(B)}}}] as     P ( A
&#x2223; B )   {\displaystyle P(A\mid B)}  [P(A\mid B)] and call it the
conditional probability of A given B.
*** As an axiom of probability[edit] ***
Some authors, such as de_Finetti, prefer to introduce conditional probability
as an axiom_of_probability:
         P ( A &#x2229; B ) = P ( A &#x2223; B ) P ( B )   {\displaystyle P
      (A\cap B)=P(A\mid B)P(B)}  [{\displaystyle P(A\cap B)=P(A\mid B)P(B)}]
Although mathematically equivalent, this may be preferred philosophically;
under major probability_interpretations such as the subjective_theory,
conditional probability is considered a primitive entity. Further, this
"multiplication axiom" introduces a symmetry with the summation axiom for
mutually_exclusive_events:[5]
         P ( A &#x222A; B ) = P ( A ) + P ( B ) &#x2212;    P ( A &#x2229; B )
      0      {\displaystyle P(A\cup B)=P(A)+P(B)-{\cancelto {0}{P(A\cap B)}}}
      [P(A\cup B)=P(A)+P(B)-{\cancelto {0}{P(A\cap B)}}]
*** As the probability of a conditional event[edit] ***
Conditional probability can be defined as the probability of a conditional
event      A  B     {\displaystyle A_{B}}  [A_B].[6] Assuming that the
experiment underlying the events     A   {\displaystyle A}  [A] and     B
{\displaystyle B}  [B] is repeated, the GoodmanâNguyenâvan_Fraassen
conditional event can be defined as
          A  B   =  &#x22C3;  i &#x2265; 1    (   &#x22C2;  j < i      B
      &#x00AF;    j   ,  A  i    B  i    )  .   {\displaystyle A_{B}=\bigcup _
      {i\geq 1}\left(\bigcap _{j<i}{\overline {B}}_{j},A_{i}B_{i}\right).}  [
      {\displaystyle A_{B}=\bigcup _{i\geq 1}\left(\bigcap _{j<i}{\overline
      {B}}_{j},A_{i}B_{i}\right).}]
It can be shown that
         P (  A  B   ) =    P ( A &#x2229; B )   P ( B )      {\displaystyle P
      (A_{B})={\frac {P(A\cap B)}{P(B)}}}  [{\displaystyle P(A_{B})={\frac {P
      (A\cap B)}{P(B)}}}]
which meets the Kolmogorov definition of conditional probability. Note that the
equation     P (  A  B   ) = P ( A &#x2229; B )  /  P ( B )   {\displaystyle P
(A_{B})=P(A\cap B)/P(B)}  [{\displaystyle P(A_{B})=P(A\cap B)/P(B)}] is a
theoretical result and not a definition. The definition via conditional events
can be understood directly in terms of the Kolmogorov_axioms and is
particularly close to the Kolmogorov interpretation_of_probability in terms of
experimental data. For example, conditional events can be repeated themselves
leading to a generalized notion of conditional event      A  B ( n )
{\displaystyle A_{B(n)}}  [{\displaystyle A_{B(n)}}]. It can be shown[6] that
the sequence     (  A  B ( n )    )  n &#x2265; 1     {\displaystyle (A_{B
(n)})_{n\geq 1}}  [{\displaystyle (A_{B(n)})_{n\geq 1}}] is i.i.d., which
yields a strong_law_of_large_numbers for conditional probability:
         P  (   lim  n &#x2192; &#x221E;      A &#x00AF;    B   n   = P ( A
      &#x2223; B )  )  = 100 &#x0025;   {\displaystyle P\left(\lim _{n\to
      \infty }{\overline {A}}_{B}^{n}=P(A\mid B)\right)=100\%}  [{\displaystyle
      P\left(\lim _{n\to \infty }{\overline {A}}_{B}^{n}=P(A\mid
      B)\right)=100\%}]
**** Measure-theoretic definition[edit] ****
If P(B) = 0, then according to the simple definition, P(A|B) is undefined.
However, it is possible to define a conditional probability with respect to a
Ï-algebra of such events (such as those arising from a continuous_random
variable).
For example, if X and Y are non-degenerate and jointly continuous random
variables with density ÆX,Y(x, y) then, if B has positive measure,
         P ( X &#x2208; A &#x2223; Y &#x2208; B ) =     &#x222B;  y &#x2208; B
      &#x222B;  x &#x2208; A    f  X , Y   ( x , y )  d x  d y    &#x222B;  y
      &#x2208; B    &#x222B;  x &#x2208;  R     f  X , Y   ( x , y )  d x  d y
      .   {\displaystyle P(X\in A\mid Y\in B)={\frac {\int _{y\in B}\int _{x\in
      A}f_{X,Y}(x,y)\,dx\,dy}{\int _{y\in B}\int _{x\in \mathbb {R} }f_{X,Y}
      (x,y)\,dx\,dy}}.}  [{\displaystyle P(X\in A\mid Y\in B)={\frac {\int _
      {y\in B}\int _{x\in A}f_{X,Y}(x,y)\,dx\,dy}{\int _{y\in B}\int _{x\in
      \mathbb {R} }f_{X,Y}(x,y)\,dx\,dy}}.}]
The case where B has zero measure is problematic. For the case that B = {y0},
representing a single point, the conditional probability could be defined as
         P ( X &#x2208; A &#x2223; Y =  y  0   ) =     &#x222B;  x &#x2208; A
      f  X , Y   ( x ,  y  0   )  d x    &#x222B;  x &#x2208;  R     f  X , Y
      ( x ,  y  0   )  d x    ,   {\displaystyle P(X\in A\mid Y=y_{0})={\frac
      {\int _{x\in A}f_{X,Y}(x,y_{0})\,dx}{\int _{x\in \mathbb {R} }f_{X,Y}
      (x,y_{0})\,dx}},}  [{\displaystyle P(X\in A\mid Y=y_{0})={\frac {\int _
      {x\in A}f_{X,Y}(x,y_{0})\,dx}{\int _{x\in \mathbb {R} }f_{X,Y}(x,y_
      {0})\,dx}},}]
however this approach leads to the BorelâKolmogorov_paradox. The more general
case of zero measure is even more problematic, as can be seen by noting that
the limit, as all Î´yi approach zero, of
         P ( X &#x2208; A &#x2223; Y &#x2208;  &#x22C3;  i   [  y  i   ,  y  i
      + &#x03B4;  y  i   ] ) &#x224A;     &#x2211;  i    &#x222B;  x &#x2208; A
      f  X , Y   ( x ,  y  i   )  d x  &#x03B4;  y  i      &#x2211;  i
      &#x222B;  x &#x2208;  R     f  X , Y   ( x ,  y  i   )  d x  &#x03B4;  y
      i      ,   {\displaystyle P(X\in A\mid Y\in \bigcup _{i}[y_{i},y_
      {i}+\delta y_{i}])\approxeq {\frac {\sum _{i}\int _{x\in A}f_{X,Y}(x,y_
      {i})\,dx\,\delta y_{i}}{\sum _{i}\int _{x\in \mathbb {R} }f_{X,Y}(x,y_
      {i})\,dx\,\delta y_{i}}},}  [{\displaystyle P(X\in A\mid Y\in \bigcup _
      {i}[y_{i},y_{i}+\delta y_{i}])\approxeq {\frac {\sum _{i}\int _{x\in A}f_
      {X,Y}(x,y_{i})\,dx\,\delta y_{i}}{\sum _{i}\int _{x\in \mathbb {R} }f_
      {X,Y}(x,y_{i})\,dx\,\delta y_{i}}},}]
depends on their relationship as they approach zero. See conditional
expectation for more information.
**** Conditioning on a random variable[edit] ****
Let X be a random variable; we assume for the sake of presentation that X is
discrete, that is, X takes on only finitely many values x. Let A be an event.
The conditional probability of A given X is defined as the random variable,
written P(A|X), that takes on the value
         P ( A &#x2223; X = x )   {\displaystyle P(A\mid X=x)}  [P(A\mid X=x)]
whenever
         X = x .   {\displaystyle X=x.}  [X=x.]
More formally,
         P ( A &#x2223; X ) ( &#x03C9; ) = P ( A &#x2223; X = X ( &#x03C9; ) )
      .   {\displaystyle P(A\mid X)(\omega )=P(A\mid X=X(\omega )).}  [
      {\displaystyle P(A\mid X)(\omega )=P(A\mid X=X(\omega )).}]
The conditional probability P(A|X) is a function of X: e.g., if the function g
is defined as
         g ( x ) = P ( A &#x2223; X = x ) ,   {\displaystyle g(x)=P(A\mid
      X=x),}  [{\displaystyle g(x)=P(A\mid X=x),}]
then
         P ( A &#x2223; X ) = g &#x2218; X .   {\displaystyle P(A\mid X)=g\circ
      X.}  [{\displaystyle P(A\mid X)=g\circ X.}]
Note that P(A|X) and X are now both random_variables. From the law_of_total
probability, the expected_value of P(A|X) is equal to the unconditional
probability of A.
**** Partial conditional probability[edit] ****
The partial conditional probability     P ( A &#x2223;  B  1   &#x2261;  b  1
, &#x2026; ,  B  m   &#x2261;  b  m   )   {\displaystyle P(A\mid B_{1}\equiv b_
{1},\ldots ,B_{m}\equiv b_{m})}  [{\displaystyle P(A\mid B_{1}\equiv b_
{1},\ldots ,B_{m}\equiv b_{m})}] is about the probability of event     A
{\displaystyle A}  [A] given that each of the condition events      B  i
{\displaystyle B_{i}}  [B_{i}] has occurred to a degree      b  i
{\displaystyle b_{i}}  [b_{i}] (degree of belief, degree of experience) that
might be different from 100%. Frequentistically, partial conditional
probability makes sense, if the conditions are tested in experiment repetitions
of appropriate length     n   {\displaystyle n}  [n] .[7] Such     n
{\displaystyle n}  [n]-bounded partial conditional probability can be defined
as the conditionally_expected average occurrence of event     A
{\displaystyle A}  [A] in testbeds of length     n   {\displaystyle n}  [n]
that adhere to all of the probability specifications      B  i   &#x2261;  b  i
{\displaystyle B_{i}\equiv b_{i}}  [{\displaystyle B_{i}\equiv b_{i}}], i.e.:
          P  n   ( A &#x2223;  B  1   &#x2261;  b  1   , &#x2026; ,  B  m
      &#x2261;  b  m   ) = E &#x2061; (    A &#x00AF;    n   &#x2223;    B
      &#x00AF;    1   n   =  b  1   , &#x2026; ,    B &#x00AF;    m   n   =  b
      m   )   {\displaystyle P^{n}(A\mid B_{1}\equiv b_{1},\ldots ,B_{m}\equiv
      b_{m})=\operatorname {E} ({\overline {A}}^{n}\mid {\overline {B}}_{1}^
      {n}=b_{1},\ldots ,{\overline {B}}_{m}^{n}=b_{m})}  [{\displaystyle P^{n}
      (A\mid B_{1}\equiv b_{1},\ldots ,B_{m}\equiv b_{m})=\operatorname {E} (
      {\overline {A}}^{n}\mid {\overline {B}}_{1}^{n}=b_{1},\ldots ,{\overline
      {B}}_{m}^{n}=b_{m})}][7]
Based on that, partial conditional probability can be defined as
         P ( A &#x2223;  B  1   &#x2261;  b  1   , &#x2026; ,  B  m   &#x2261;
      b  m   ) =  lim  n &#x2192; &#x221E;    P  n   ( A &#x2223;  B  1
      &#x2261;  b  1   , &#x2026; ,  B  m   &#x2261;  b  m   ) ,
      {\displaystyle P(A\mid B_{1}\equiv b_{1},\ldots ,B_{m}\equiv b_{m})=\lim
      _{n\to \infty }P^{n}(A\mid B_{1}\equiv b_{1},\ldots ,B_{m}\equiv b_{m}),}
      [{\displaystyle P(A\mid B_{1}\equiv b_{1},\ldots ,B_{m}\equiv b_{m})=\lim
      _{n\to \infty }P^{n}(A\mid B_{1}\equiv b_{1},\ldots ,B_{m}\equiv b_
      {m}),}]
where      b  i   n &#x2208;  N    {\displaystyle b_{i}n\in \mathbb {N} }  [
{\displaystyle b_{i}n\in \mathbb {N} }] [7]
Jeffrey_conditionalization [8] [9] is a special case of partial conditional
probability in which the condition events must form a partition:
         P ( A &#x2223;  B  1   &#x2261;  b  1   , &#x2026; ,  B  m   &#x2261;
      b  m   ) =  &#x2211;  i = 1   m    b  i   P ( A &#x2223;  B  i   )
      {\displaystyle P(A\mid B_{1}\equiv b_{1},\ldots ,B_{m}\equiv b_{m})=\sum
      _{i=1}^{m}b_{i}P(A\mid B_{i})}  [{\displaystyle P(A\mid B_{1}\equiv b_
      {1},\ldots ,B_{m}\equiv b_{m})=\sum _{i=1}^{m}b_{i}P(A\mid B_{i})}]
***** Example[edit] *****
Suppose that somebody secretly rolls two fair six-sided dice, and we wish to
compute the probability that the face-up value of the first one is 2, given the
information that their sum is no greater than 5.
    * Let D1 be the value rolled on die 1.
    * Let D2 be the value rolled on die 2.
Probability that D1 = 2
Table 1 shows the sample_space of 36 combinations of rolled values of the two
dice, each of which occurs with probability 1/36, with the numbers displayed in
the red and dark gray cells being D1 + D2.
D1 = 2 in exactly 6 of the 36 outcomes; thus P(D1 =
2) = &#x200b;6⁄36 = &#x200b;1⁄6:
       ______Table_1______
      |+   |D2____________|
      |____|1|2|3|4_|5_|6_|
      |  |1|2|3|4|5_|6_|7_|
      |  |2|3|4|5|6_|7_|8_|
      |D1|3|4|5|6|7_|8_|9_|
      |  |4|5|6|7|8_|9_|10|
      |  |5|6|7|8|9_|10|11|
      |__|6|7|8|9|10|11|12|
Probability that D1 + D2 â¤ 5
Table 2 shows that D1 + D2 â¤ 5 for exactly 10 of the 36 outcomes, thus P
(D1 + D2 â¤ 5) = &#x200b;10⁄36:
       ______Table_2______
      |+   |D2____________|
      |____|1|2|3|4_|5_|6_|
      |  |1|2|3|4|5_|6_|7_|
      |  |2|3|4|5|6_|7_|8_|
      |D1|3|4|5|6|7_|8_|9_|
      |  |4|5|6|7|8_|9_|10|
      |  |5|6|7|8|9_|10|11|
      |__|6|7|8|9|10|11|12|
Probability that D1 = 2 given that D1 + D2 â¤ 5
Table 3 shows that for 3 of these 10 outcomes, D1 = 2.
Thus, the conditional probability P(D1 = 2 | D1+D2 â¤ 5) = &#x200b;3⁄10 = 0.3:
       ______Table_3______
      |+   |D2____________|
      |____|1|2|3|4_|5_|6_|
      |  |1|2|3|4|5_|6_|7_|
      |  |2|3|4|5|6_|7_|8_|
      |D1|3|4|5|6|7_|8_|9_|
      |  |4|5|6|7|8_|9_|10|
      |  |5|6|7|8|9_|10|11|
      |__|6|7|8|9|10|11|12|
Here, in the earlier notation for the definition of conditional probability,
the conditioning event B is that D1 + D2 â¤ 5, and the event A is D1 = 2. We
have     P ( A &#x2223; B ) =     P ( A &#x2229; B )   P ( B )     =     3  /
36   10  /  36     =    3 10    ,   {\displaystyle P(A\mid B)={\tfrac {P(A\cap
B)}{P(B)}}={\tfrac {3/36}{10/36}}={\tfrac {3}{10}},}  [{\displaystyle P(A\mid
B)={\tfrac {P(A\cap B)}{P(B)}}={\tfrac {3/36}{10/36}}={\tfrac {3}{10}},}] as
seen in the table.
***** Use in inference[edit] *****
In statistical_inference, the conditional probability is an update of the
probability of an event based on new information.[3] Incorporating the new
information can be done as follows:[1]
    * Let A, the event of interest, be in the sample_space, say (X,P).
    * The occurrence of the event A knowing that event B has or will have
      occurred, means the occurrence of A as it is restricted to B, i.e.     A
      &#x2229; B   {\displaystyle A\cap B}  [A\cap B].
    * Without the knowledge of the occurrence of B, the information about the
      occurrence of A would simply be P(A)
    * The probability of A knowing that event B has or will have occurred, will
      be the probability of     A &#x2229; B   {\displaystyle A\cap B}  [A\cap
      B] relative to P(B), the probability that B has occurred.
    * This results in     P ( A  |  B ) = P ( A &#x2229; B )  /  P ( B )
      {\textstyle P(A|B)=P(A\cap B)/P(B)}  [{\textstyle P(A|B)=P(A\cap B)/P
      (B)}] whenever P(B) > 0 and 0 otherwise.
This approach results in a probability measure that is consistent with the
original probability measure and satisfies all the Kolmogorov_axioms. This
conditional probability measure also could have resulted by assuming that the
relative magnitude of the probability of A with respect to X will be preserved
with respect to B (cf. a_Formal_Derivation below).
The wording "evidence" or "information" is generally used in the Bayesian
interpretation_of_probability. The conditioning event is interpreted as
evidence for the conditioned event. That is, P(A) is the probability of A
before accounting for evidence E, and P(A|E) is the probability of A after
having accounted for evidence E or after having updated P(A). This is
consistent with the frequentist interpretation, which is the first definition
given above.
***** Statistical independence[edit] *****
Main article: Independence_(probability_theory)
Events A and B are defined to be statistically_independent if
         P ( A &#x2229; B ) = P ( A ) P ( B ) .   {\displaystyle P(A\cap B)=P
      (A)P(B).}  [{\displaystyle P(A\cap B)=P(A)P(B).}]
If P(B) is not zero, then this is equivalent to the statement that
         P ( A &#x2223; B ) = P ( A ) .   {\displaystyle P(A\mid B)=P(A).}  [
      {\displaystyle P(A\mid B)=P(A).}]
Similarly, if P(A) is not zero, then
         P ( B &#x2223; A ) = P ( B )   {\displaystyle P(B\mid A)=P(B)}  [
      {\displaystyle P(B\mid A)=P(B)}]
is also equivalent. Although the derived forms may seem more intuitive, they
are not the preferred definition as the conditional probabilities may be
undefined, and the preferred definition is symmetrical in A and B.
Independent events vs. mutually exclusive events
The concepts of mutually independent events and mutually_exclusive_events are
separate and distinct. The following table contrasts results for the two cases
(provided the probability of the conditioning event is not zero).
                            If statistically independent  If mutually exclusive
   P ( A &#x2223; B ) =
{\displaystyle P(A\mid B)=}    P ( A )   {\displaystyle P 0
[{\displaystyle P(A\mid     (A)}  [P(A)]
B)=}]
   P ( B &#x2223; A ) =
{\displaystyle P(B\mid A)=}    P ( B )   {\displaystyle P 0
[{\displaystyle P(B\mid     (B)}  [P(B)]
A)=}]
   P ( A &#x2229; B ) =        P ( A ) P ( B )
{\displaystyle P(A\cap B)=} {\displaystyle P(A)P(B)}  [   0
[{\displaystyle P(A\cap     {\displaystyle P(A)P(B)}]
B)=}]
In fact, mutually exclusive events cannot be statistically independent (unless
they both are impossible), since knowing that one occurs gives information
about the other (specifically, that it certainly does not occur).
***** Common fallacies[edit] *****
      These fallacies should not be confused with Robert K. Shope's 1978
      "conditional_fallacy", which deals with counterfactual examples that beg
      the_question.
**** Assuming conditional probability is of similar size to its inverse[edit]
****
Main article: Confusion_of_the_inverse
A geometric visualisation of Bayes' theorem. In the table, the values 2, 3, 6
and 9 give the relative weights of each corresponding condition and case. The
figures denote the cells of the table involved in each metric, the probability
being the fraction of each figure that is shaded. This shows that P(A|B) P(B) =
P(B|A) P(A) i.e. P(A|B) = P(B|A) P(A)/P(B) . Similar reasoning can be used to
show that P(Ä|B) = P(B|Ä) P(Ä)/P(B) etc.
In general, it cannot be assumed that P(A|B) â P(B|A). This can be an
insidious error, even for those who are highly conversant with statistics.[10]
The relationship between P(A|B) and P(B|A) is given by Bayes'_theorem:
             P ( B &#x2223; A )    =    P ( A &#x2223; B ) P ( B )   P ( A )
      &#x21D4;    P ( B &#x2223; A )   P ( A &#x2223; B )       =    P ( B )
      P ( A )          {\displaystyle {\begin{aligned}P(B\mid A)&={\frac {P
      (A\mid B)P(B)}{P(A)}}\\\Leftrightarrow {\frac {P(B\mid A)}{P(A\mid B)}}&=
      {\frac {P(B)}{P(A)}}\end{aligned}}}  [{\displaystyle {\begin{aligned}P
      (B\mid A)&={\frac {P(A\mid B)P(B)}{P(A)}}\\\Leftrightarrow {\frac {P
      (B\mid A)}{P(A\mid B)}}&={\frac {P(B)}{P(A)}}\end{aligned}}}]
That is, P(A|B) â P(B|A) only if P(B)/P(A) â 1, or equivalently, P(A) â P
(B).
**** Assuming marginal and conditional probabilities are of similar size[edit]
****
In general, it cannot be assumed that P(A) â P(A|B). These probabilities are
linked through the law_of_total_probability:
         P ( A ) =  &#x2211;  n   P ( A &#x2229;  B  n   ) =  &#x2211;  n   P
      ( A &#x2223;  B  n   ) P (  B  n   ) .   {\displaystyle P(A)=\sum _{n}P
      (A\cap B_{n})=\sum _{n}P(A\mid B_{n})P(B_{n}).}  [{\displaystyle P
      (A)=\sum _{n}P(A\cap B_{n})=\sum _{n}P(A\mid B_{n})P(B_{n}).}]
where the events     (  B  n   )   {\displaystyle (B_{n})}  [(B_{n})] form a
countable partition of     &#x03A9;   {\displaystyle \Omega }  [\Omega ].
This fallacy may arise through selection_bias.[11] For example, in the context
of a medical claim, let SC be the event that a sequela (chronic disease) S
occurs as a consequence of circumstance (acute condition) C. Let H be the event
that an individual seeks medical help. Suppose that in most cases, C does not
cause S so P(SC) is low. Suppose also that medical attention is only sought if
S has occurred due to C. From experience of patients, a doctor may therefore
erroneously conclude that P(SC) is high. The actual probability observed by the
doctor is P(SC|H).
**** Over- or under-weighting priors[edit] ****
Not taking prior probability into account partially or completely is called
base_rate_neglect. The reverse, insufficient adjustment from the prior
probability is conservatism.
***** Formal derivation[edit] *****
Formally, P(A | B) is defined as the probability of A according to a new
probability function on the sample space, such that outcomes not in B have
probability 0 and that it is consistent with all original probability_measures.
[12][13]
Let Î© be a sample_space with elementary_events {Ï}. Suppose we are told the
event B â Î© has occurred. A new probability distribution (denoted by the
conditional notation) is to be assigned on {Ï} to reflect this. For events in
B, it is reasonable to assume that the relative magnitudes of the probabilities
will be preserved. For some constant scale factor Î±, the new distribution will
therefore satisfy:
               1.&#xA0;  &#x03C9; &#x2208; B : P ( &#x03C9; &#x2223; B ) =
      &#x03B1; P ( &#x03C9; )       2.&#xA0;  &#x03C9; &#x2209; B : P
      ( &#x03C9; &#x2223; B ) = 0       3.&#xA0;   &#x2211;  &#x03C9; &#x2208;
      &#x03A9;    P ( &#x03C9; &#x2223; B )  = 1.       {\displaystyle {\begin
      {aligned}&{\text{1. }}\omega \in B:P(\omega \mid B)=\alpha P(\omega )\\&
      {\text{2. }}\omega \notin B:P(\omega \mid B)=0\\&{\text{3. }}\sum _
      {\omega \in \Omega }{P(\omega \mid B)}=1.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}&{\text{1. }}\omega \in B:P(\omega \mid B)=\alpha P
      (\omega )\\&{\text{2. }}\omega \notin B:P(\omega \mid B)=0\\&{\text{3.
      }}\sum _{\omega \in \Omega }{P(\omega \mid B)}=1.\end{aligned}}}]
Substituting 1 and 2 into 3 to select Î±:
             1    =  &#x2211;  &#x03C9; &#x2208; &#x03A9;    P ( &#x03C9;
      &#x2223; B )        =  &#x2211;  &#x03C9; &#x2208; B    P ( &#x03C9;
      &#x2223; B )  +     &#x2211;  &#x03C9; &#x2209; B   P ( &#x03C9; &#x2223;
      B )   0          = &#x03B1;  &#x2211;  &#x03C9; &#x2208; B    P
      ( &#x03C9; )        = &#x03B1; &#x22C5; P ( B )     &#x21D2; &#x03B1;
      =   1  P ( B )          {\displaystyle {\begin{aligned}1&=\sum _{\omega
      \in \Omega }{P(\omega \mid B)}\\&=\sum _{\omega \in B}{P(\omega \mid B)}+
      {\cancelto {0}{\sum _{\omega \notin B}P(\omega \mid B)}}\\&=\alpha \sum _
      {\omega \in B}{P(\omega )}\\[5pt]&=\alpha \cdot P(B)\\[5pt]\Rightarrow
      \alpha &={\frac {1}{P(B)}}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}1&=\sum _{\omega \in \Omega }{P(\omega \mid B)}\\&=\sum _{\omega
      \in B}{P(\omega \mid B)}+{\cancelto {0}{\sum _{\omega \notin B}P(\omega
      \mid B)}}\\&=\alpha \sum _{\omega \in B}{P(\omega )}\\[5pt]&=\alpha \cdot
      P(B)\\[5pt]\Rightarrow \alpha &={\frac {1}{P(B)}}\end{aligned}}}]
So the new probability distribution is
              1.&#xA0;  &#x03C9; &#x2208; B    : P ( &#x03C9; &#x2223; B ) =
      P ( &#x03C9; )   P ( B )         2.&#xA0;  &#x03C9; &#x2209; B    : P
      ( &#x03C9; &#x2223; B ) = 0       {\displaystyle {\begin{aligned}{\text
      {1. }}\omega \in B&:P(\omega \mid B)={\frac {P(\omega )}{P(B)}}\\{\text
      {2. }}\omega \notin B&:P(\omega \mid B)=0\end{aligned}}}  [{\displaystyle
      {\begin{aligned}{\text{1. }}\omega \in B&:P(\omega \mid B)={\frac {P
      (\omega )}{P(B)}}\\{\text{2. }}\omega \notin B&:P(\omega \mid B)=0\end
      {aligned}}}]
Now for a general event A,
             P ( A &#x2223; B )    =  &#x2211;  &#x03C9; &#x2208; A &#x2229; B
      P ( &#x03C9; &#x2223; B )  +     &#x2211;  &#x03C9; &#x2208; A &#x2229;
      B  c     P ( &#x03C9; &#x2223; B )   0          =  &#x2211;  &#x03C9;
      &#x2208; A &#x2229; B      P ( &#x03C9; )   P ( B )          =    P ( A
      &#x2229; B )   P ( B )          {\displaystyle {\begin{aligned}P(A\mid
      B)&=\sum _{\omega \in A\cap B}{P(\omega \mid B)}+{\cancelto {0}{\sum _
      {\omega \in A\cap B^{c}}P(\omega \mid B)}}\\&=\sum _{\omega \in A\cap B}
      {\frac {P(\omega )}{P(B)}}\\[5pt]&={\frac {P(A\cap B)}{P(B)}}\end
      {aligned}}}  [{\displaystyle {\begin{aligned}P(A\mid B)&=\sum _{\omega
      \in A\cap B}{P(\omega \mid B)}+{\cancelto {0}{\sum _{\omega \in A\cap B^
      {c}}P(\omega \mid B)}}\\&=\sum _{\omega \in A\cap B}{\frac {P(\omega )}{P
      (B)}}\\[5pt]&={\frac {P(A\cap B)}{P(B)}}\end{aligned}}}]
***** See also[edit] *****
    * [icon]Mathematics_portal
    * BorelâKolmogorov_paradox
    * Chain_rule_(probability)
    * Class_membership_probabilities
    * Conditional_probability_distribution
    * Conditioning_(probability)
    * Joint_probability_distribution
    * Monty_Hall_problem
    * Posterior_probability
    * Bayes'_theorem
***** References[edit] *****
   1. ^ a bGut, Allan (2013). Probability: A Graduate Course (Second ed.). New
      York, NY: Springer. ISBN 978-1-4614-4707-8.
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
   3. ^Ross, Sheldon (2010). A First Course in Probability (8th ed.). Pearson
      Prentice Hall. ISBN 978-0-13-603313-4.
   4. ^ a bCasella, George; Berger, Roger L. (2002). Statistical Inference.
      Duxbury Press. ISBN 0-534-24312-6.
   5. ^Kolmogorov, Andrey (1956), Foundations of the Theory of Probability,
      Chelsea
   6. ^ Gillies, Donald (2000); "Philosophical Theories of Probability";
      Routledge; Chapter 4 "The subjective theory"
   7. ^ a bDraheim, Dirk (2017). "An_Operational_Semantics_of_Conditional
      Probabilities_that_Fully_Adheres_to_Kolmogorov's_Explication_of
      Probability_Theory". doi:10.13140/RG.2.2.10050.48323/3.
   8. ^ a b cDraheim, Dirk (2017). "Generalized_Jeffrey_Conditionalization_(A
      Frequentist_Semantics_of_Partial_Conditionalization)". Springer.
      Retrieved December 19, 2017.
   9. ^Jeffrey, Richard C. (1983), The_Logic_of_Decision,_2nd_edition,
      University of Chicago Press
  10. ^"Bayesian_Epistemology". Stanford Encyclopedia of Philosophy. 2017.
      Retrieved December 29, 2017.
  11. ^ Paulos, J.A. (1988) Innumeracy: Mathematical Illiteracy and its
      Consequences, Hill and Wang.
  12. ISBN 0-8090-7447-8 (p. 63 et seq.)
  13. ^ Thomas Bruss, F; Der Wyatt Earp Effekt; Spektrum der Wissenschaft;
      March 2007
  14. ^ George Casella and Roger L. Berger (1990), Statistical Inference,
      Duxbury Press,
  15. ISBN 0-534-11958-1 (p. 18 et seq.)
  16. ^ Grinstead_and_Snell's_Introduction_to_Probability, p. 134
***** External links[edit] *****
 Wikimedia Commons has media related to Conditional_probability.
    * Weisstein,_Eric_W. "Conditional_Probability". MathWorld.
F._Thomas_Bruss Der Wyatt-Earp-Effekt oder die betÃ¶rende Macht kleiner
Wahrscheinlichkeiten (in German), Spektrum der Wissenschaft (German Edition of
Scientific American), Vol 2, 110â113, (2007).
Visual_explanation_of_conditional_probability

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Conditional_probability&oldid=908157342"
Categories:
    * Conditional_probability
    * Invalid_proofs
    * Statistical_ratios
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * Cymraeg
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 27 July 2019, at 21:01 (UTC).
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
