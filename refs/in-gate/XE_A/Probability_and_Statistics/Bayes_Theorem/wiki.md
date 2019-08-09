The following text has been accessed from https://en.wikipedia.org/wiki/Bayes%27_theorem at Fri Aug 9 00:03:03 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Bayes' theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Bayes rule" redirects here. For the concept in decision theory, see Bayes
estimator.
Probability based on prior knowledge
A blue neon_sign showing the simple statement of Bayesâ theorem at the
offices of HP_Autonomy
Part of a series on Statistics
Bayesian_statistics
[Bayes_icon.svg]
Theory
    * Admissible_decision_rule
    * Bayesian_efficiency
    * Bayesian_probability
    * Probability_interpretations
    * Bayes' theorem
    * Bayes_factor
    * Bayesian_inference
    * Bayesian_network
    * Prior
    * Posterior
    * Likelihood
    * Conjugate_prior
    * Posterior_predictive
    * Hyperparameter
    * Hyperprior
    * Principle_of_indifference
    * Principle_of_maximum_entropy
    * Empirical_Bayes_method
    * Cromwell's_rule
    * Bernsteinâvon_Mises_theorem
    * Schwarz_criterion
    * Credible_interval
    * Maximum_a_posteriori_estimation
    * Radical_probabilism
Techniques
    * Bayesian_linear_regression
    * Bayesian_estimator
    * Approximate_Bayesian_computation
    * Markov_chain_Monte_Carlo
    * [Fisher_iris_versicolor_sepalwidth.svg] Statistics_portal
    * v
    * t
    * e
In probability_theory and statistics, Bayesâ theorem (alternatively Bayesâ
law or Bayesâ rule) describes the probability of an event, based on prior
knowledge of conditions that might be related to the event. For example, if
cancer is related to age, then, using Bayesâ theorem, a person's age can be
used to more accurately assess the probability that they have cancer, compared
to the assessment of the probability of cancer made without knowledge of the
personâs age.
One of the many applications of Bayesâ theorem is Bayesian_inference, a
particular approach to statistical_inference. When applied, the probabilities
involved in Bayesâ theorem may have different probability_interpretations.
With the Bayesian_probability interpretation the theorem expresses how a degree
of belief, expressed as a probability, should rationally change to account for
availability of related evidence. Bayesian inference is fundamental to Bayesian
statistics.
Bayesâ theorem is named after Reverend Thomas_Bayes (/beÉªz/; 1701?â1761),
who first used conditional probability to provide an algorithm (his Proposition
9) that uses evidence to calculate limits on an unknown parameter, published as
 An_Essay_towards_solving_a_Problem_in_the_Doctrine_of_Chances (1763). In what
he called a scholium, Bayes extended his algorithm to any unknown prior cause.
Independently of Bayes, Pierre-Simon_Laplace in 1774, and later in his 1812
âThÃ©orie_analytique_des_probabilitÃ©sâ used conditional probability to
formulate the relation of an updated posterior probability from a prior
probability, given evidence. Sir_Harold_Jeffreys put Bayes's algorithm and
Laplaceâs formulation on an axiomatic basis. Jeffreys wrote that Bayesâ
theorem âis to the theory of probability what the Pythagorean_theorem is to
geometry.â[1]
⁰
***** Contents *****
    * 1_Statement_of_theorem
    * 2_Examples
          o 2.1_Drug_testing
          o 2.2_A_more_complicated_example
    * 3_Interpretations
          o 3.1_Bayesian_interpretation
          o 3.2_Frequentist_interpretation
                # 3.2.1_Example
    * 4_Forms
          o 4.1_Events
                # 4.1.1_Simple_form
                # 4.1.2_Alternative_form
                # 4.1.3_Extended_form
          o 4.2_Random_variables
                # 4.2.1_Simple_form
                # 4.2.2_Extended_form
          o 4.3_Bayesâ_rule
    * 5_Derivation
          o 5.1_For_events
          o 5.2_For_random_variables
    * 6_Correspondence_to_other_mathematical_frameworks
          o 6.1_Propositional_logic
          o 6.2_Subjective_logic
    * 7_History
    * 8_See_also
    * 9_Notes
    * 10_References
    * 11_Further_reading
    * 12_External_links
***** Statement of theorem[edit] *****
Visualization of Bayesâ theorem by superposition of two event tree_diagrams.
Bayesâ theorem is stated mathematically as the following equation:[2]
   P ( A &#x2223; B ) =    P ( B &#x2223; A ) P ( A )   P ( B )
{\displaystyle P(A\mid B)={\frac {P(B\mid A)P(A)}{P(B)}}}  [{\displaystyle P
(A\mid B)={\frac {P(B\mid A)P(A)}{P(B)}}}]
where     A   {\displaystyle A}  [A] and     B   {\displaystyle B}  [B] are
events and     P ( B ) &#x2260; 0   {\displaystyle P(B)\neq 0}  [{\displaystyle
P(B)\neq 0}].
    *    P ( A &#x2223; B )   {\displaystyle P(A\mid B)}  [P(A\mid B)] is a
      conditional_probability: the likelihood of event     A   {\displaystyle
      A}  [A] occurring given that     B   {\displaystyle B}  [B] is true.
    *    P ( B &#x2223; A )   {\displaystyle P(B\mid A)}  [{\displaystyle P
      (B\mid A)}] is also a conditional probability: the likelihood of event
      B   {\displaystyle B}  [B] occurring given that     A   {\displaystyle A}
      [A] is true.
    *    P ( A )   {\displaystyle P(A)}  [P(A)] and     P ( B )
      {\displaystyle P(B)}  [P(B)] are the probabilities of observing     A
      {\displaystyle A}  [A] and     B   {\displaystyle B}  [B] independently
      of each other; this is known as the marginal_probability.
***** Examples[edit] *****
**** Drug testing[edit] ****
Tree diagram illustrating drug testing example. U, Åª, â+â and âââ
are the events representing user, non-user, positive result and negative
result. Percentages in parentheses are calculated.
Suppose that a test for using a particular drug is 99% sensitive and 99%
specific. That is, the test will produce 99% true positive results for drug
users and 99% true negative results for non-drug users. Suppose that 0.5% of
people are users of the drug. What is the probability that a randomly selected
individual with a positive test is a drug user?
             P (  User  &#x2223;  +  )    =    P (  +  &#x2223;  User  ) P
      (  User  )   P ( + )          =    P (  +  &#x2223;  User  ) P (  User  )
      P (  +  &#x2223;  User  ) P (  User  ) + P (  +  &#x2223;  Non-user  ) P
      (  Non-user  )          =    0.99 &#x00D7; 0.005   0.99 &#x00D7; 0.005 +
      0.01 &#x00D7; 0.995          &#x2248; 33.2 &#x0025;       {\displaystyle
      {\begin{aligned}P({\text{User}}\mid {\text{+}})&={\frac {P({\text{+}}\mid
      {\text{User}})P({\text{User}})}{P(+)}}\\&={\frac {P({\text{+}}\mid {\text
      {User}})P({\text{User}})}{P({\text{+}}\mid {\text{User}})P({\text
      {User}})+P({\text{+}}\mid {\text{Non-user}})P({\text{Non-user}})}}\\
      [8pt]&={\frac {0.99\times 0.005}{0.99\times 0.005+0.01\times 0.995}}\\
      [8pt]&\approx 33.2\%\end{aligned}}}  [{\displaystyle {\begin{aligned}P(
      {\text{User}}\mid {\text{+}})&={\frac {P({\text{+}}\mid {\text{User}})P(
      {\text{User}})}{P(+)}}\\&={\frac {P({\text{+}}\mid {\text{User}})P({\text
      {User}})}{P({\text{+}}\mid {\text{User}})P({\text{User}})+P({\text
      {+}}\mid {\text{Non-user}})P({\text{Non-user}})}}\\[8pt]&={\frac
      {0.99\times 0.005}{0.99\times 0.005+0.01\times 0.995}}\\[8pt]&\approx
      33.2\%\end{aligned}}}]
Even if an individual tests positive, it is more likely that they do not use
the drug than that they do. This is because the number of non-users is large
compared to the number of users. The number of false positives outweighs the
number of true positives. For example, if 1000 individuals are tested, there
are expected to be 995 non-users and 5 users. From the 995 non-users,
0.01 Ã 995 â 10 false positives are expected. From the 5 users,
0.99 Ã 5 â 5 true positives are expected. Out of 15 positive results, only 5
are genuine.
The importance of specificity in this example can be seen by calculating that
even if sensitivity is raised to 100% and specificity remains at 99% then the
probability of the person being a drug user only rises from 33.2% to 33.4%, but
if the sensitivity is held at 99% and the specificity is increased to 99.5%
then the probability of the person being a drug user rises to about 49.9%.
**** A more complicated example[edit] ****
The entire output of a factory is produced on three machines. The three
machines account for 20%, 30%, and 50% of the factory output. The fraction of
defective items produced is 5% for the first machine; 3% for the second
machine; and 1% for the third machine. If an item is chosen at random from the
total output and is found to be defective, what is the probability that it was
produced by the third machine?
Once again, the answer can be reached without recourse to the formula by
applying the conditions to any hypothetical number of cases. For example, if
100,000 items are produced by the factory, 20,000 will be produced by Machine
A, 30,000 by Machine B, and 50,000 by Machine C. Machine A will produce 1000
defective items, Machine B 900, and Machine C 500. Of the total 2400 defective
items, only 500, or 5/24 were produced by Machine C.
A solution is as follows. Let Xi denote the event that a randomly chosen item
was made by the i th machine (for i = A,B,C). Let Y denote the event that a
randomly chosen item is defective. Then, we are given the following
information:
         P (  X  A   ) = 0.2 ,  P (  X  B   ) = 0.3 ,  P (  X  C   ) = 0.5.
      {\displaystyle P(X_{A})=0.2,\quad P(X_{B})=0.3,\quad P(X_{C})=0.5.}  [
      {\displaystyle P(X_{A})=0.2,\quad P(X_{B})=0.3,\quad P(X_{C})=0.5.}]
If the item was made by the first machine, then the probability that it is
defective is 0.05; that is, P(Y | XA) = 0.05. Overall, we have
         P ( Y &#x2223;  X  A   ) = 0.05 ,  P ( Y &#x2223;  X  B   ) = 0.03 ,
      P ( Y &#x2223;  X  C   ) = 0.01.   {\displaystyle P(Y\mid X_
      {A})=0.05,\quad P(Y\mid X_{B})=0.03,\quad P(Y\mid X_{C})=0.01.}  [
      {\displaystyle P(Y\mid X_{A})=0.05,\quad P(Y\mid X_{B})=0.03,\quad P
      (Y\mid X_{C})=0.01.}]
To answer the original question, we first find P(Y). That can be done in the
following way:
         P ( Y ) =  &#x2211;  i   P ( Y &#x2223;  X  i   ) P (  X  i   ) =
      ( 0.05 ) ( 0.2 ) + ( 0.03 ) ( 0.3 ) + ( 0.01 ) ( 0.5 ) = 0.024.
      {\displaystyle P(Y)=\sum _{i}P(Y\mid X_{i})P(X_{i})=(0.05)(0.2)+(0.03)
      (0.3)+(0.01)(0.5)=0.024.}  [{\displaystyle P(Y)=\sum _{i}P(Y\mid X_{i})P
      (X_{i})=(0.05)(0.2)+(0.03)(0.3)+(0.01)(0.5)=0.024.}]
Hence 2.4% of the total output of the factory is defective.
We are given that Y has occurred, and we want to calculate the conditional
probability of XC. By Bayesâ theorem,
         P (  X  C   &#x2223; Y ) =    P ( Y &#x2223;  X  C   ) P (  X  C   )
      P ( Y )    =    0.01 &#x22C5; 0.50  0.024   =   5 24     {\displaystyle P
      (X_{C}\mid Y)={\frac {P(Y\mid X_{C})P(X_{C})}{P(Y)}}={\frac {0.01\cdot
      0.50}{0.024}}={\frac {5}{24}}}  [{\displaystyle P(X_{C}\mid Y)={\frac {P
      (Y\mid X_{C})P(X_{C})}{P(Y)}}={\frac {0.01\cdot 0.50}{0.024}}={\frac {5}
      {24}}}]
Given that the item is defective, the probability that it was made by the third
machine is only 5/24. Although machine C produces half of the total output, it
produces a much smaller fraction of the defective items. Hence the knowledge
that the item selected was defective enables us to replace the prior
probability P(XC) = 1/2 by the smaller posterior probability P(XC | Y) = 5/24.
***** Interpretations[edit] *****
A geometric visualisation of Bayesâ theorem. The figures denote the cells of
the table involved in each metric, the probability being the fraction of each
figure that is shaded. Similar reasoning shows that          P (    A &#x00AF;
&#x2223; B ) =    P ( B &#x2223;    A &#x00AF;    ) P (    A &#x00AF;    )   P
( B )           {\displaystyle {\begin{smallmatrix}P({\bar {A}}\mid B)={\frac
{P(B\mid {\bar {A}})P({\bar {A}})}{P(B)}}\end{smallmatrix}}}  [{\displaystyle
{\begin{smallmatrix}P({\bar {A}}\mid B)={\frac {P(B\mid {\bar {A}})P({\bar
{A}})}{P(B)}}\end{smallmatrix}}}] and so on.
The interpretation of Bayesâ theorem depends on the interpretation_of
probability ascribed to the terms. The two main interpretations are described
below.
**** Bayesian interpretation[edit] ****
In the Bayesian_(or_epistemological)_interpretation, probability measures a
âdegree of belief.â Bayesâ theorem then links the degree of belief in a
proposition before and after accounting for evidence. For example, suppose it
is believed with 50% certainty that a coin is twice as likely to land heads
than tails. If the coin is flipped a number of times and the outcomes observed,
that degree of belief may rise, fall or remain the same depending on the
results.
For proposition A and evidence B,
          * Pâ(A), the prior, is the initial degree of belief in A.
          * Pâ(A | B), the posterior is the degree of belief having accounted
            for B.
          * the quotient P(B | A)/P(B) represents the support B provides for A.
For more on the application of Bayes' theorem under the Bayesian interpretation
of probability, see Bayesian_inference.
**** Frequentist interpretation[edit] ****
Illustration of frequentist interpretation with tree_diagrams. Bayesâ theorem
connects conditional probabilities to their inverses.
In the frequentist_interpretation, probability measures a âproportion of
outcomes.â For example, suppose an experiment is performed many times. P(A)
is the proportion of outcomes with property A, and P(B) that with property B. P
(B | A) is the proportion of outcomes with property B out of outcomes with
property A, and P(A | B) the proportion of those with A out of those with B.
The role of Bayesâ theorem is best visualized with tree diagrams, as shown to
the right. The two diagrams partition the same outcomes by A and B in opposite
orders, to obtain the inverse probabilities. Bayes' theorem serves as the link
between these different partitionings.
*** Example[edit] ***
Tree diagram illustrating frequentist example. R, C, P and P bar are the events
representing rare, common, pattern and no pattern. Percentages in parentheses
are calculated. Note that three independent values are given, so it is possible
to calculate the inverse tree (see figure above).
An entomologist spots what might be a rare subspecies of beetle, due to the
pattern on its back. In the rare subspecies, 98% have the pattern, or P
(Pattern | Rare) = 98%. In the common subspecies, 5% have the pattern. The rare
subspecies accounts for only 0.1% of the population. How likely is the beetle
having the pattern to be rare, or what is P(Rare | Pattern)?
From the extended form of Bayesâ theorem (since any beetle can be only rare
or common),
             P (  Rare  &#x2223;  Pattern  )    =    P (  Pattern  &#x2223;
      Rare  ) P (  Rare  )   P (  Pattern  )          =    P (  Pattern
      &#x2223;  Rare  ) P (  Rare  )   P (  Pattern  &#x2223;  Rare  ) P
      (  Rare  ) + P (  Pattern  &#x2223;  Common  ) P (  Common  )          =
      0.98 &#x00D7; 0.001   0.98 &#x00D7; 0.001 + 0.05 &#x00D7; 0.999
      &#x2248; 1.9 &#x0025;       {\displaystyle {\begin{aligned}P({\text
      {Rare}}\mid {\text{Pattern}})&={\frac {P({\text{Pattern}}\mid {\text
      {Rare}})P({\text{Rare}})}{P({\text{Pattern}})}}\\[8pt]&={\frac {P({\text
      {Pattern}}\mid {\text{Rare}})P({\text{Rare}})}{P({\text{Pattern}}\mid
      {\text{Rare}})P({\text{Rare}})+P({\text{Pattern}}\mid {\text{Common}})P(
      {\text{Common}})}}\\[8pt]&={\frac {0.98\times 0.001}{0.98\times
      0.001+0.05\times 0.999}}\\[8pt]&\approx 1.9\%\end{aligned}}}  [
      {\displaystyle {\begin{aligned}P({\text{Rare}}\mid {\text{Pattern}})&=
      {\frac {P({\text{Pattern}}\mid {\text{Rare}})P({\text{Rare}})}{P({\text
      {Pattern}})}}\\[8pt]&={\frac {P({\text{Pattern}}\mid {\text{Rare}})P(
      {\text{Rare}})}{P({\text{Pattern}}\mid {\text{Rare}})P({\text{Rare}})+P(
      {\text{Pattern}}\mid {\text{Common}})P({\text{Common}})}}\\[8pt]&={\frac
      {0.98\times 0.001}{0.98\times 0.001+0.05\times 0.999}}\\[8pt]&\approx
      1.9\%\end{aligned}}}]
***** Forms[edit] *****
**** Events[edit] ****
*** Simple form[edit] ***
For events A and B, provided that P(B) â  0,
         P ( A &#x2223; B ) =    P ( B &#x2223; A ) P ( A )   P ( B )
      &#x22C5;   {\displaystyle P(A\mid B)={\frac {P(B\mid A)P(A)}{P(B)}}\cdot
      }  [{\displaystyle P(A\mid B)={\frac {P(B\mid A)P(A)}{P(B)}}\cdot }]
In many applications, for instance in Bayesian_inference, the event B is fixed
in the discussion, and we wish to consider the impact of its having been
observed on our belief in various possible events A. In such a situation the
denominator of the last expression, the probability of the given evidence B, is
fixed; what we want to vary is A. Bayesâ theorem then shows that the
posterior probabilities are proportional to the numerator:
         P ( A &#x2223; B ) &#x221D; P ( A ) &#x22C5; P ( B &#x2223; A )
      {\displaystyle P(A\mid B)\propto P(A)\cdot P(B\mid A)}  [{\displaystyle P
      (A\mid B)\propto P(A)\cdot P(B\mid A)}] (proportionality over A for given
      B).
The posterior is proportional to the prior times the likelihood.[3]
If events A1, A2, ..., are mutually exclusive and exhaustive, i.e., one of them
is certain to occur but no two can occur together, and we know their
probabilities up to proportionality, then we can determine the proportionality
constant by using the fact that their probabilities must add up to one. For
instance, for a given event A, the event A itself and its complement Â¬A are
exclusive and exhaustive. Denoting the constant of proportionality by c we have
         P ( A &#x2223; B ) = c &#x22C5; P ( A ) &#x22C5; P ( B &#x2223; A )
      &#xA0;and&#xA0;  P ( &#x00AC; A &#x2223; B ) = c &#x22C5; P ( &#x00AC; A
      ) &#x22C5; P ( B &#x2223; &#x00AC; A ) .   {\displaystyle P(A\mid
      B)=c\cdot P(A)\cdot P(B\mid A){\text{ and }}P(\neg A\mid B)=c\cdot P(\neg
      A)\cdot P(B\mid \neg A).}  [{\displaystyle P(A\mid B)=c\cdot P(A)\cdot P
      (B\mid A){\text{ and }}P(\neg A\mid B)=c\cdot P(\neg A)\cdot P(B\mid \neg
      A).}]
Adding these two formulas we deduce that
         1 = c &#x22C5; ( P ( B &#x2223; A ) &#x22C5; P ( A ) + P ( B &#x2223;
      &#x00AC; A ) &#x22C5; P ( &#x00AC; A ) ) ,   {\displaystyle 1=c\cdot (P
      (B\mid A)\cdot P(A)+P(B\mid \neg A)\cdot P(\neg A)),}  [{\displaystyle
      1=c\cdot (P(B\mid A)\cdot P(A)+P(B\mid \neg A)\cdot P(\neg A)),}]
or
         c =   1  P ( B &#x2223; A ) &#x22C5; P ( A ) + P ( B &#x2223; &#x00AC;
      A ) &#x22C5; P ( &#x00AC; A )    =   1  P ( B )    .   {\displaystyle c=
      {\frac {1}{P(B\mid A)\cdot P(A)+P(B\mid \neg A)\cdot P(\neg A)}}={\frac
      {1}{P(B)}}.}  [{\displaystyle c={\frac {1}{P(B\mid A)\cdot P(A)+P(B\mid
      \neg A)\cdot P(\neg A)}}={\frac {1}{P(B)}}.}]
*** Alternative form[edit] ***
Another form of Bayesâ theorem that is generally encountered when looking at
two competing statements or hypotheses is:
         P ( A &#x2223; B ) =    P ( B &#x2223; A ) P ( A )   P ( B &#x2223; A
      ) P ( A ) + P ( B &#x2223; &#x00AC; A ) P ( &#x00AC; A )    .
      {\displaystyle P(A\mid B)={\frac {P(B\mid A)P(A)}{P(B\mid A)P(A)+P(B\mid
      \neg A)P(\neg A)}}.}  [{\displaystyle P(A\mid B)={\frac {P(B\mid A)P(A)}
      {P(B\mid A)P(A)+P(B\mid \neg A)P(\neg A)}}.}]
For an epistemological interpretation:
For proposition A and evidence or background B,[4]
    *    P ( A )   {\displaystyle P(A)}  [P(A)] is the prior_probability, is
      the initial degree of belief in A.
    *    P ( &#x00AC; A )   {\displaystyle P(\neg A)}  [{\displaystyle P(\neg
      A)}] is the corresponding probability of the initial degree of belief
      against A, where     1 &#x2212; P ( A ) = P ( &#x00AC; A )
      {\displaystyle 1-P(A)=P(\neg A)}  [{\displaystyle 1-P(A)=P(\neg A)}]
    *    P ( B &#x2223; A )   {\displaystyle P(B\mid A)}  [{\displaystyle P
      (B\mid A)}] is the conditional_probability or likelihood, is the degree
      of belief in B, given that the proposition A is true.
    *    P ( B &#x2223; &#x00AC; A )   {\displaystyle P(B\mid \neg A)}  [
      {\displaystyle P(B\mid \neg A)}] is the conditional_probability or
      likelihood, is the degree of belief in B, given that the proposition A is
      false.
    *    P ( A &#x2223; B )   {\displaystyle P(A\mid B)}  [P(A\mid B)] is the
      posterior_probability, is the probability for A after taking into account
      B for and against A.
*** Extended form[edit] ***
Often, for some partition {Aj} of the sample_space, the event_space is given or
conceptualized in terms of P(Aj) and P(B | Aj). It is then useful to compute P
(B) using the law_of_total_probability:
         P ( B ) =   &#x2211;  j   P ( B &#x2223;  A  j   ) P (  A  j   )  ,
      {\displaystyle P(B)={\sum _{j}P(B\mid A_{j})P(A_{j})},}  [P(B)={\sum _
      {j}P(B\mid A_{j})P(A_{j})},]
         &#x21D2; P (  A  i   &#x2223; B ) =    P ( B &#x2223;  A  i   ) P (  A
      i   )    &#x2211;  j   P ( B &#x2223;  A  j   ) P (  A  j   )    &#x22C5;
      {\displaystyle \Rightarrow P(A_{i}\mid B)={\frac {P(B\mid A_{i})P(A_{i})}
      {\sum \limits _{j}P(B\mid A_{j})P(A_{j})}}\cdot }  [{\displaystyle
      \Rightarrow P(A_{i}\mid B)={\frac {P(B\mid A_{i})P(A_{i})}{\sum \limits _
      {j}P(B\mid A_{j})P(A_{j})}}\cdot }]
In the special case where A is a binary_variable:
         P ( A &#x2223; B ) =    P ( B &#x2223; A ) P ( A )   P ( B &#x2223; A
      ) P ( A ) + P ( B &#x2223; &#x00AC; A ) P ( &#x00AC; A )    &#x22C5;
      {\displaystyle P(A\mid B)={\frac {P(B\mid A)P(A)}{P(B\mid A)P(A)+P(B\mid
      \neg A)P(\neg A)}}\cdot }  [{\displaystyle P(A\mid B)={\frac {P(B\mid A)P
      (A)}{P(B\mid A)P(A)+P(B\mid \neg A)P(\neg A)}}\cdot }]
**** Random variables[edit] ****
Diagram illustrating the meaning of Bayesâ theorem as applied to an event
space generated by continuous random variables X and Y. Note that there exists
an instance of Bayesâ theorem for each point in the domain. In practice,
these instances might be parametrized by writing the specified probability
densities as a function of x and y.
Consider a sample_space Î© generated by two random_variables X and Y. In
principle, Bayesâ theorem applies to the events A = {X = x} and B = {Y = y}.
         P ( X = x &#x2223; Y = y ) =    P ( Y = y &#x2223; X = x ) P ( X = x )
      P ( Y = y )      {\displaystyle P(X=x\mid Y=y)={\frac {P(Y=y\mid X=x)P
      (X=x)}{P(Y=y)}}}  [{\displaystyle P(X=x\mid Y=y)={\frac {P(Y=y\mid X=x)P
      (X=x)}{P(Y=y)}}}]
However, terms become 0 at points where either variable has finite probability
density. To remain useful, Bayesâ theorem may be formulated in terms of the
relevant densities (see Derivation).
*** Simple form[edit] ***
If X is continuous and Y is discrete,
          f  X &#x2223; Y = y   ( x ) =    P ( Y = y &#x2223; X = x )  f  X
      ( x )   P ( Y = y )      {\displaystyle f_{X\mid Y=y}(x)={\frac {P
      (Y=y\mid X=x)f_{X}(x)}{P(Y=y)}}}  [{\displaystyle f_{X\mid Y=y}(x)={\frac
      {P(Y=y\mid X=x)f_{X}(x)}{P(Y=y)}}}]
where each     f   {\displaystyle f}  [f] is a density function.
If X is discrete and Y is continuous,
         P ( X = x &#x2223; Y = y ) =     f  Y &#x2223; X = x   ( y ) P ( X = x
      )    f  Y   ( y )    .   {\displaystyle P(X=x\mid Y=y)={\frac {f_{Y\mid
      X=x}(y)P(X=x)}{f_{Y}(y)}}.}  [{\displaystyle P(X=x\mid Y=y)={\frac {f_
      {Y\mid X=x}(y)P(X=x)}{f_{Y}(y)}}.}]
If both X and Y are continuous,
          f  X &#x2223; Y = y   ( x ) =     f  Y &#x2223; X = x   ( y )  f  X
      ( x )    f  Y   ( y )    .   {\displaystyle f_{X\mid Y=y}(x)={\frac {f_
      {Y\mid X=x}(y)f_{X}(x)}{f_{Y}(y)}}.}  [{\displaystyle f_{X\mid Y=y}(x)=
      {\frac {f_{Y\mid X=x}(y)f_{X}(x)}{f_{Y}(y)}}.}]
*** Extended form[edit] ***
Diagram illustrating how an event space generated by continuous random
variables X and Y is often conceptualized.
A continuous event space is often conceptualized in terms of the numerator
terms. It is then useful to eliminate the denominator using the law_of_total
probability. For fY(y), this becomes an integral:
          f  Y   ( y ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;    f  Y   ( y
      &#x2223; X = &#x03BE; )  f  X   ( &#x03BE; )  d &#x03BE; .
      {\displaystyle f_{Y}(y)=\int _{-\infty }^{\infty }f_{Y}(y\mid X=\xi )f_
      {X}(\xi )\,d\xi .}  [{\displaystyle f_{Y}(y)=\int _{-\infty }^{\infty }f_
      {Y}(y\mid X=\xi )f_{X}(\xi )\,d\xi .}]
**** Bayesâ rule[edit] ****
Bayesâ theorem in odds_form is:
         O (  A  1   :  A  2   &#x2223; B ) = O (  A  1   :  A  2   ) &#x22C5;
      &#x039B; (  A  1   :  A  2   &#x2223; B )   {\displaystyle O(A_{1}:A_
      {2}\mid B)=O(A_{1}:A_{2})\cdot \Lambda (A_{1}:A_{2}\mid B)}  [O(A_{1}:A_
      {2}\mid B)=O(A_{1}:A_{2})\cdot \Lambda (A_{1}:A_{2}\mid B)]
where
         &#x039B; (  A  1   :  A  2   &#x2223; B ) =    P ( B &#x2223;  A  1
      )   P ( B &#x2223;  A  2   )      {\displaystyle \Lambda (A_{1}:A_{2}\mid
      B)={\frac {P(B\mid A_{1})}{P(B\mid A_{2})}}}  [\Lambda (A_{1}:A_{2}\mid
      B)={\frac {P(B\mid A_{1})}{P(B\mid A_{2})}}]
is called the Bayes_factor or likelihood_ratio and the odds between two events
is simply the ratio of the probabilities of the two events. Thus
         O (  A  1   :  A  2   ) =    P (  A  1   )   P (  A  2   )    ,
      {\displaystyle O(A_{1}:A_{2})={\frac {P(A_{1})}{P(A_{2})}},}  [O(A_{1}:A_
      {2})={\frac {P(A_{1})}{P(A_{2})}},]
         O (  A  1   :  A  2   &#x2223; B ) =    P (  A  1   &#x2223; B )   P
      (  A  2   &#x2223; B )    ,   {\displaystyle O(A_{1}:A_{2}\mid B)={\frac
      {P(A_{1}\mid B)}{P(A_{2}\mid B)}},}  [O(A_{1}:A_{2}\mid B)={\frac {P(A_
      {1}\mid B)}{P(A_{2}\mid B)}},]
So the rule says that the posterior odds are the prior odds times the Bayes
factor, or in other words, posterior is proportional to prior times likelihood.
In the special case that      A  1   = A   {\displaystyle A_{1}=A}  [A_{1}=A]
and      A  2   = &#x00AC; A   {\displaystyle A_{2}=\neg A}  [A_{2}=\neg A],
one writes     O ( A ) = O ( A : &#x00AC; A ) = P ( A )  /  ( 1 &#x2212; P ( A
) )   {\displaystyle O(A)=O(A:\neg A)=P(A)/(1-P(A))}  [{\displaystyle O(A)=O(A:
\neg A)=P(A)/(1-P(A))}], and uses a similar abbreviation for the Bayes factor
and for the conditional odds. The odds on     A   {\displaystyle A}  [A] is by
definition the odds for and against     A   {\displaystyle A}  [A]. Bayesâ
rule can then be written in the abbreviated form
         O ( A  |  B ) = O ( A ) &#x22C5; &#x039B; ( A  |  B ) ,
      {\displaystyle O(A|B)=O(A)\cdot \Lambda (A|B),}  [O(A|B)=O(A)\cdot
      \Lambda (A|B),]
or in words: the posterior odds on     A   {\displaystyle A}  [A] equals the
prior odds on     A   {\displaystyle A}  [A] times the likelihood ratio for
A   {\displaystyle A}  [A] given information     B   {\displaystyle B}  [B]. In
short, posterior odds equals prior odds times likelihood ratio.
***** Derivation[edit] *****
**** For events[edit] ****
Bayesâ theorem may be derived from the definition of conditional_probability:
         P ( A &#x2223; B ) =    P ( A &#x2229; B )   P ( B )    ,
      &#xA0;if&#xA0;  P ( B ) &#x2260; 0 ,   {\displaystyle P(A\mid B)={\frac
      {P(A\cap B)}{P(B)}},{\text{ if }}P(B)\neq 0,}  [{\displaystyle P(A\mid
      B)={\frac {P(A\cap B)}{P(B)}},{\text{ if }}P(B)\neq 0,}]
         P ( B &#x2223; A ) =    P ( B &#x2229; A )   P ( A )    ,
      &#xA0;if&#xA0;  P ( A ) &#x2260; 0 ,   {\displaystyle P(B\mid A)={\frac
      {P(B\cap A)}{P(A)}},{\text{ if }}P(A)\neq 0,}  [{\displaystyle P(B\mid
      A)={\frac {P(B\cap A)}{P(A)}},{\text{ if }}P(A)\neq 0,}]
where     P ( A &#x2229; B )   {\displaystyle P(A\cap B)}  [P(A\cap B)] is the
joint_probability of both A and B being true, because
         P ( B &#x2229; A ) = P ( A &#x2229; B )   {\displaystyle P(B\cap A)=P
      (A\cap B)}  [{\displaystyle P(B\cap A)=P(A\cap B)}]
         &#x21D2; P ( A &#x2229; B ) = P ( A &#x2223; B ) P ( B ) = P ( B
      &#x2223; A ) P ( A )   {\displaystyle \Rightarrow P(A\cap B)=P(A\mid B)P
      (B)=P(B\mid A)P(A)}  [{\displaystyle \Rightarrow P(A\cap B)=P(A\mid B)P
      (B)=P(B\mid A)P(A)}]
         &#x21D2; P ( A &#x2223; B ) =    P ( B &#x2223; A ) P ( A )   P ( B )
      ,  &#xA0;if&#xA0;  P ( B ) &#x2260; 0.   {\displaystyle \Rightarrow P
      (A\mid B)={\frac {P(B\mid A)P(A)}{P(B)}},{\text{ if }}P(B)\neq 0.}  [
      {\displaystyle \Rightarrow P(A\mid B)={\frac {P(B\mid A)P(A)}{P(B)}},
      {\text{ if }}P(B)\neq 0.}]
**** For random variables[edit] ****
For two continuous random_variables X and Y, Bayesâ theorem may be
analogously derived from the definition of conditional_density:
          f  X &#x2223; Y = y   ( x ) =     f  X , Y   ( x , y )    f  Y   ( y
      )      {\displaystyle f_{X\mid Y=y}(x)={\frac {f_{X,Y}(x,y)}{f_{Y}(y)}}}
      [{\displaystyle f_{X\mid Y=y}(x)={\frac {f_{X,Y}(x,y)}{f_{Y}(y)}}}]
          f  Y &#x2223; X = x   ( y ) =     f  X , Y   ( x , y )    f  X   ( x
      )      {\displaystyle f_{Y\mid X=x}(y)={\frac {f_{X,Y}(x,y)}{f_{X}(x)}}}
      [{\displaystyle f_{Y\mid X=x}(y)={\frac {f_{X,Y}(x,y)}{f_{X}(x)}}}]
Therefore,
          f  X &#x2223; Y = y   ( x ) =     f  Y &#x2223; X = x   ( y )  f  X
      ( x )    f  Y   ( y )    .   {\displaystyle f_{X\mid Y=y}(x)={\frac {f_
      {Y\mid X=x}(y)f_{X}(x)}{f_{Y}(y)}}.}  [{\displaystyle f_{X\mid Y=y}(x)=
      {\frac {f_{Y\mid X=x}(y)f_{X}(x)}{f_{Y}(y)}}.}]
***** Correspondence to other mathematical frameworks[edit] *****
**** Propositional logic[edit] ****
Bayesâ theorem represents a generalisation of contraposition which in
propositional_logic can be expressed as:
         ( &#x00AC; A &#x2192; &#x00AC; B ) &#x2192; ( B &#x2192; A ) .
      {\displaystyle (\lnot A\to \lnot B)\to (B\to A).}  [{\displaystyle (\lnot
      A\to \lnot B)\to (B\to A).}]
The corresponding formula in terms of probability calculus is Bayes' theorem
which in its expanded form is expressed as:
         P ( A &#x2223; B ) =    P ( B &#x2223; A ) a ( A )   P ( B &#x2223; A
      ) a ( A ) + P ( B &#x2223; &#x00AC; A ) a ( &#x00AC; A )    .
      {\displaystyle P(A\mid B)={\frac {P(B\mid A)a(A)}{P(B\mid A)a(A)+P(B\mid
      \lnot A)a(\lnot A)}}.}  [{\displaystyle P(A\mid B)={\frac {P(B\mid A)a
      (A)}{P(B\mid A)a(A)+P(B\mid \lnot A)a(\lnot A)}}.}]
In the equation above the conditional_probability     P ( B &#x2223; A )
{\displaystyle P(B\mid A)}  [P(B\mid A)] generalizes the logical statement
( A &#x2192; B )   {\displaystyle (A\to B)}  [{\displaystyle (A\to B)}], i.e.
in addition to assigning TRUE or FALSE we can also assign any probability to
the statement. The term     a ( A )   {\displaystyle a(A)}  [{\displaystyle a
(A)}] denotes the prior_probability (aka. the base_rate) of     A
{\displaystyle A}  [A]. Assume that     P ( A &#x2223; B ) = 1   {\displaystyle
P(A\mid B)=1}  [{\displaystyle P(A\mid B)=1}] is equivalent to     ( B &#x2192;
A )   {\displaystyle (B\to A)}  [{\displaystyle (B\to A)}] being TRUE, and that
P ( A &#x2223; B ) = 0   {\displaystyle P(A\mid B)=0}  [{\displaystyle P(A\mid
B)=0}] is equivalent to     ( B &#x2192; A )   {\displaystyle (B\to A)}  [
{\displaystyle (B\to A)}] being FALSE. It is then easy to see that     P ( A
&#x2223; B ) = 1   {\displaystyle P(A\mid B)=1}  [{\displaystyle P(A\mid B)=1}]
when     P ( &#x00AC; B &#x2223; &#x00AC; A ) = 1   {\displaystyle P(\lnot
B\mid \lnot A)=1}  [{\displaystyle P(\lnot B\mid \lnot A)=1}] i.e. when
( &#x00AC; A &#x2192; &#x00AC; B )   {\displaystyle (\lnot A\to \lnot B)}  [
{\displaystyle (\lnot A\to \lnot B)}] is TRUE. This is because     P ( B
&#x2223; &#x00AC; A ) = 1 &#x2212; P ( &#x00AC; B &#x2223; &#x00AC; A ) = 0
{\displaystyle P(B\mid \lnot A)=1-P(\lnot B\mid \lnot A)=0}  [{\displaystyle P
(B\mid \lnot A)=1-P(\lnot B\mid \lnot A)=0}] so that the fraction on the right-
hand side of the equation above is equal to 1, and hence     P ( A &#x2223; B )
= 1   {\displaystyle P(A\mid B)=1}  [{\displaystyle P(A\mid B)=1}] which is
equivalent to     ( B &#x2192; A )   {\displaystyle (B\to A)}  [{\displaystyle
(B\to A)}] being TRUE. Hence, Bayesâ theorem represents a generalization of
contraposition.[5]
**** Subjective logic[edit] ****
Bayesâ theorem represents a special case of conditional inversion in
subjective_logic expressed as:
         (  &#x03C9;  A     |  &#x007E;    B   S   ,  &#x03C9;  A     |
      &#x007E;    &#x00AC; B   S   ) = (  &#x03C9;  B &#x2223; A   S   ,
      &#x03C9;  B &#x2223; &#x00AC; A   S   )    &#x03D5; &#x007E;     a  A   ,
      {\displaystyle (\omega _{A{\tilde {|}}B}^{S},\omega _{A{\tilde {|}}\lnot
      B}^{S})=(\omega _{B\mid A}^{S},\omega _{B\mid \lnot A}^{S}){\widetilde
      {\phi }}a_{A},}  [{\displaystyle (\omega _{A{\tilde {|}}B}^{S},\omega _{A
      {\tilde {|}}\lnot B}^{S})=(\omega _{B\mid A}^{S},\omega _{B\mid \lnot A}^
      {S}){\widetilde {\phi }}a_{A},}]
where        &#x03D5; &#x007E;      {\displaystyle {\widetilde {\phi }}}  [
{\displaystyle {\widetilde {\phi }}}] denotes the operator for conditional
inversion. The argument     (  &#x03C9;  B &#x2223; A   S   ,  &#x03C9;  B
&#x2223; &#x00AC; A   S   )   {\displaystyle (\omega _{B\mid A}^{S},\omega _
{B\mid \lnot A}^{S})}  [{\displaystyle (\omega _{B\mid A}^{S},\omega _{B\mid
\lnot A}^{S})}] denotes a pair of binomial conditional opinions given by source
S   {\displaystyle S}  [S], and the argument      a  A     {\displaystyle a_
{A}}  [a_{A}] denotes the prior_probability (aka. the base_rate) of     A
{\displaystyle A}  [A]. The pair of inverted conditional opinions is denoted
(  &#x03C9;  A     |  &#x007E;    B   S   ,  &#x03C9;  A     |  &#x007E;
&#x00AC; B   S   )   {\displaystyle (\omega _{A{\tilde {|}}B}^{S},\omega _{A
{\tilde {|}}\lnot B}^{S})}  [{\displaystyle (\omega _{A{\tilde {|}}B}^
{S},\omega _{A{\tilde {|}}\lnot B}^{S})}]. The conditional opinion
&#x03C9;  A &#x2223; B   S     {\displaystyle \omega _{A\mid B}^{S}}  [
{\displaystyle \omega _{A\mid B}^{S}}] generalizes the probabilistic
conditional     P ( A &#x2223; B )   {\displaystyle P(A\mid B)}  [P(A\mid B)],
i.e. in addition to assigning a probability the source     S   {\displaystyle
S}  [S] can assign any subjective opinion to the conditional statement     ( A
&#x2223; B )   {\displaystyle (A\mid B)}  [{\displaystyle (A\mid B)}]. A
binomial subjective opinion      &#x03C9;  A   S     {\displaystyle \omega _
{A}^{S}}  [{\displaystyle \omega _{A}^{S}}] is the belief in the truth of
statement     A   {\displaystyle A}  [A] with degrees of uncertainty, as
expressed by source     S   {\displaystyle S}  [S]. Every subjective opinion
has a corresponding projected probability     P (  &#x03C9;  A   S   )
{\displaystyle P(\omega _{A}^{S})}  [{\displaystyle P(\omega _{A}^{S})}]. The
projected probability of opinions applied to Bayesâ theorem produces a
homomorphism so that Bayesâ theorem can be expressed in terms of the
projected probabilities of opinions:
         P (  &#x03C9;  A     |  &#x007E;    B   S   ) =    P (  &#x03C9;  B
      &#x2223; A   S   ) a ( A )   P (  &#x03C9;  B &#x2223; A   S   ) a ( A )
      + P (  &#x03C9;  B &#x2223; &#x00AC; A   S   ) a ( &#x00AC; A )    .
      {\displaystyle P(\omega _{A{\tilde {|}}B}^{S})={\frac {P(\omega _{B\mid
      A}^{S})a(A)}{P(\omega _{B\mid A}^{S})a(A)+P(\omega _{B\mid \lnot A}^{S})a
      (\lnot A)}}.}  [{\displaystyle P(\omega _{A{\tilde {|}}B}^{S})={\frac {P
      (\omega _{B\mid A}^{S})a(A)}{P(\omega _{B\mid A}^{S})a(A)+P(\omega _
      {B\mid \lnot A}^{S})a(\lnot A)}}.}]
Hence, the subjective Bayesâ theorem represents a generalization of Bayesâ
theorem.[6]
***** History[edit] *****
Bayesâ theorem was named after Thomas_Bayes (1701â1761), who studied how to
compute a distribution for the probability parameter of a binomial_distribution
(in modern terminology). Bayesâs unpublished manuscript was significantly
edited by Richard_Price before it was posthumously read at the Royal_Society.
Price edited[7] Bayesâs major work âAn_Essay_towards_solving_a_Problem_in
the_Doctrine_of_Chancesâ (1763), which appeared in Philosophical
Transactions,[8] and contains Bayesâ theorem. Price wrote an introduction to
the paper which provides some of the philosophical basis of Bayesian
statistics. In 1765, he was elected a Fellow of the Royal Society in
recognition of his work on the legacy of Bayes.[9][10]
The French mathematician Pierre-Simon_Laplace reproduced and extended Bayes's
results in 1774, apparently unaware of Bayes's work.[note_1][11] The Bayesian
interpretation of probability was developed mainly by Laplace.[12]
Stephen_Stigler used a Bayesian argument to conclude that Bayesâ theorem was
discovered by Nicholas_Saunderson, a blind English mathematician, some time
before Bayes;[13][14] that interpretation, however, has been disputed.[15]
Martyn Hooper[16] and Sharon McGrayne[17] have argued that Richard_Price's
contribution was substantial:
     By modern standards, we should refer to the BayesâPrice rule. Price
     discovered Bayesâ work, recognized its importance, corrected it,
     contributed to the article, and found a use for it. The modern
     convention of employing Bayesâ name alone is unfair but so
     entrenched that anything else makes little sense.[17]
***** See also[edit] *****
    * [icon]Statistics_portal
    * Quantum_Bayesianism
    * Bayesian_inference
    * Bayesian_probability
    * Inductive_probability
***** Notes[edit] *****
   1. ^ Laplace refined Bayes' theorem over a period of decades:
          o Laplace announced his independent discovery of Bayes' theorem in:
            Laplace (1774) "MÃ©moire sur la probabilitÃ© des causes par les
            Ã©vÃ©nements," "MÃ©moires de l'AcadÃ©mie royale des Sciences de MI
            (Savants Ã©trangers)," 4: 621â656. Reprinted in: Laplace,
            "Oeuvres complÃ¨tes" (Paris, France: Gauthier-Villars et fils,
            1841), vol. 8, pp. 27â65. Available on-line at: Gallica. Bayes'
            theorem appears on p. 29.
          o Laplace presented a refinement of Bayes' theorem in: Laplace (read:
            1783 / published: 1785) "MÃ©moire sur les approximations des
            formules qui sont fonctions de trÃ¨s grands nombres," "MÃ©moires de
            l'AcadÃ©mie royale des Sciences de Paris," 423â467. Reprinted in:
            Laplace, "Oeuvres complÃ¨tes" (Paris, France: Gauthier-Villars et
            fils, 1844), vol. 10, pp. 295â338. Available on-line at: Gallica.
            Bayes' theorem is stated on page 301.
          o See also: Laplace, "Essai philosophique sur les probabilitÃ©s"
            (Paris, France: Mme. Ve. Courcier [Madame veuve (i.e., widow)
            Courcier], 1814), page_10. English translation: Pierre Simon,
            Marquis de Laplace with F. W. Truscott and F. L. Emory, trans., "A
            Philosophical Essay on Probabilities" (New York, New York: John
            Wiley & Sons, 1902), page_15.
***** References[edit] *****
   1. ^Jeffreys,_Harold (1973). Scientific Inference (3rd ed.). Cambridge
      University_Press. p. 31. ISBN 978-0-521-18078-8.
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
   3. ^Stuart, A.; Ord, K. (1994), Kendall's Advanced Theory of Statistics:
      Volume IâDistribution Theory, Edward_Arnold, Â§8.7
   4. ^ Lee, Peter M. (2012). "Chapter 1". Bayesian_Statistics. Wiley.
      ISBN 978-1-1183-3257-3.
   5. ^"Bayes'_Theorem:_Introduction". Trinity University. Archived from the
      original on 21 August 2004. Retrieved 5 August 2014.
   6. ^ Audun JÃ¸sang, 2016, Subjective Logic; A formalism for Reasoning Under
      Uncertainty. Springer, Cham,
   7. ISBN 978-3-319-42337-1
   8. ^ Audun JÃ¸sang, 2016, Generalising_Bayes'_Theorem_in_Subjective_Logic.
      IEEE International Conference on Multisensor Fusion and Integration for
      Intelligent Systems (MFI 2016), Baden-Baden, September 2016
   9. ^Allen, Richard (1999). David_Hartley_on_Human_Nature. SUNY Press.
      pp. 243â4. ISBN 978-0-7914-9451-6. Retrieved 16 June 2013.
  10. ^Bayes, Thomas & Price, Richard (1763). "An_Essay_towards_solving_a
      Problem_in_the_Doctrine_of_Chance._By_the_late_Rev._Mr._Bayes,
      communicated_by_Mr._Price,_in_a_letter_to_John_Canton,_A._M._F._R._S."
      (PDF). Philosophical Transactions of the Royal Society of London. 53 (0):
      370â418. doi:10.1098/rstl.1763.0053. Archived from the_original (PDF)
      on 2011-04-10. Retrieved 2003-12-27.
  11. ^ Holland, pp. 46â7.
  12. ^Price, Richard (1991). Price:_Political_Writings. Cambridge University
      Press. p. xxiii. ISBN 978-0-521-40969-8. Retrieved 16 June 2013.
  13. ^Daston, Lorraine (1988). Classical_Probability_in_the_Enlightenment.
      Princeton Univ Press. p. 268. ISBN 0-691-08497-1.
  14. ^ Stigler, Stephen M. (1986). The History of Statistics: The Measurement
      of Uncertainty before 1900. Harvard University Press, Chapter 3.
  15. ^Stigler, Stephen M. (1983). "Who Discovered Bayes' Theorem?". The
      American Statistician. 37 (4): 290â296. doi:10.1080/
      00031305.1983.10483122.
  16. ^de Vaux, Richard; Velleman, Paul; Bock, David (2016). Stats, Data and
      Models (4th ed.). Pearson. pp. 380â381. ISBN 978-0-321-98649-8.
  17. ^Edwards, A. W. F. (1986). "Is the Reference in Hartley (1749) to
      Bayesian Inference?". The American Statistician. 40 (2): 109â110. doi:
      10.1080/00031305.1986.10475370.
  18. ^Hooper, Martyn (2013). "Richard Price, Bayes' theorem, and God".
      Significance. 10 (1): 36â39. doi:10.1111/j.1740-9713.2013.00638.x.
  19. ^ a bMcGrayne, S. B. (2011). The Theory That Would Not Die: How Bayes'
      Rule Cracked the Enigma Code, Hunted Down Russian Submarines & Emerged
      Triumphant from Two Centuries of Controversy. Yale_University_Press.
      ISBN 978-0-300-18822-6.
***** Further reading[edit] *****
    * Bruss, F. Thomas (2013), â250 years of âAn Essay towards solving a
      Problem in the Doctrine of Chance. By the late Rev. Mr. Bayes,
      communicated by Mr. Price, in a letter to John Canton, A. M. F. R.
      S.â,â doi:10.1365/s13291-013-0077-z, Jahresbericht der Deutschen
      Mathematiker-Vereinigung, Springer Verlag, Vol. 115, Issue 3-4 (2013),
      129-133.
    * Gelman, A, Carlin, JB, Stern, HS, and Rubin, DB (2003), âBayesian Data
      Analysis,â Second Edition, CRC Press.
    * Grinstead, CM and Snell, JL (1997), âIntroduction to Probability (2nd
      edition),â American Mathematical Society (free pdf available) [1].
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Bayes_formula", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
McGrayne, SB (2011). The Theory That Would Not Die: How Bayes' Rule Cracked the
Enigma Code, Hunted Down Russian Submarines & Emerged Triumphant from Two
Centuries of Controversy. Yale_University_Press. ISBN 978-0-300-18822-6.
Laplace, P (1774/1986), âMemoir on the Probability of the Causes of
Events,â Statistical Science 1(3):364â378.
Lee, Peter M (2012), âBayesian Statistics: An Introduction,â 4th edition.
Wiley.
ISBN 978-1-118-33257-3.
Puga JL, Krzywinski M, Altman N (31 March 2015). "Bayes'_theorem". Nature
Methods. 12 (4): 277â278.
Rosenthal, Jeffrey S (2005), âStruck by Lightning: The Curious World of
Probabilities.â HarperCollins. (Granta, 2008.
ISBN 9781862079960).
Stigler, SM (1986). "Laplace's 1774 Memoir on Inverse Probability". Statistical
Science. 1 (3): 359â363. doi:10.1214/ss/1177013620.
Stone, JV (2013), download chapter 1 of âBayesâ_Rule:_A_Tutorial
Introduction_to_Bayesian_Analysisâ, Sebtel Press, England.
Bayesian_Reasoning_for_Intelligent_People, An introduction and tutorial to the
use of Bayesâ theorem in statistics and cognitive science.
Morris, Dan (2016), Read first 6 chapters for free of âBayesâ_Theorem
Examples:_A_Visual_Introduction_For_Beginnersâ Blue Windmill
ISBN 978-1549761744. A short tutorial on how to understand problem scenarios
and find P(B), P(A), and P(B|A).
***** External links[edit] *****
    * Bayes'_theorem at the EncyclopÃ¦dia_Britannica
    * The_Theory_That_Would_Not_Die_by_Sharon_Bertsch_McGrayne New York Times
      Book Review by John_Allen_Paulos on 5 August 2011
    * Visual_explanation_of_Bayes_using_trees (video)
    * Bayesâ_frequentist_interpretation_explained_visually (video)
    * Earliest_Known_Uses_of_Some_of_the_Words_of_Mathematics_(B). Contains
      origins of âBayesian,â âBayesâ Theorem,â âBayes Estimate/
      Risk/Solution,â âEmpirical Bayes,â and âBayes Factor.â
    * Weisstein,_Eric_W. "Bayes'_Theorem". MathWorld.
Bayes'_theorem at PlanetMath.org.
Bayes_Theorem_and_the_Folly_of_Prediction
A_tutorial_on_probability_and_Bayesâ_theorem_devised_for_Oxford_University
psychology_students
An_Intuitive_Explanation_of_Bayesâ_Theorem_by_Eliezer_S._Yudkowsky

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Bayes%27_theorem&oldid=909854417"
Categories:
    * Bayesian_statistics
    * Probability_theorems
    * Statistical_theorems
Hidden categories:
    * Articles_with_short_description
    * Articles_with_EncyclopÃ¦dia_Britannica_links
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AragonÃ©s
    * Asturianu
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Latina
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 8 August 2019, at 01:24 (UTC).
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
