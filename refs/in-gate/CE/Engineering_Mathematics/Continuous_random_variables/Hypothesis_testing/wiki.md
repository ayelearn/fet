The following text has been accessed from https://en.wikipedia.org/wiki/Statistical_hypothesis_testing at Thu Aug 8 23:42:57 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Statistical hypothesis testing ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Critical region" redirects here. For the computer science notion of a
"critical section", sometimes called a "critical region", see critical_section.
A statistical hypothesis, sometimes called confirmatory data analysis, is a
hypothesis that is testable on the basis of observing a process that is modeled
via a set of random_variables.[1] A statistical hypothesis test is a method of
statistical_inference. Commonly, two statistical data sets are compared, or a
data set obtained by sampling is compared against a synthetic data set from an
idealized model. A hypothesis is proposed for the statistical relationship
between the two data sets, and this is compared as an alternative to an
idealized null hypothesis that proposes no relationship between two data sets.
The comparison is deemed statistically_significant if the relationship between
the data sets would be an unlikely realization of the null_hypothesis according
to a threshold probability—the significance level. Hypothesis tests are used
when determining what outcomes of a study would lead to a rejection of the null
hypothesis for a pre-specified level of significance.
The process of distinguishing between the null hypothesis and the alternative
hypothesis is aided by considering two conceptual types of errors. The first
type of error occurs when the null hypothesis is wrongly rejected. The second
type of error occurs when the null hypothesis is wrongly not rejected. (The two
types are known as type_1_and_type_2_errors.)
Hypothesis tests based on statistical significance are another way of
expressing confidence_intervals (more precisely, confidence sets). In other
words, every hypothesis test based on significance can be obtained via a
confidence interval, and every confidence interval can be obtained via a
hypothesis test based on significance.[2]
Significance-based hypothesis testing is the most common framework for
statistical hypothesis testing. An alternative framework for statistical
hypothesis testing is to specify a set of statistical_models, one for each
candidate hypothesis, and then use model_selection techniques to choose the
most appropriate model.[3] The most common selection techniques are based on
either Akaike_information_criterion or Bayes_factor.
⁰
***** Contents *****
    * 1_The_testing_process
          o 1.1_Interpretation
          o 1.2_Use_and_importance
          o 1.3_Cautions
    * 2_Examples
          o 2.1_Human_sex_ratio
          o 2.2_Lady_tasting_tea
          o 2.3_Courtroom_trial
          o 2.4_Philosopher's_beans
          o 2.5_Clairvoyant_card_game
          o 2.6_Radioactive_suitcase
    * 3_Definition_of_terms
    * 4_Common_test_statistics
    * 5_Variations_and_sub-classes
    * 6_History
          o 6.1_Early_use
          o 6.2_Modern_origins_and_early_controversy
          o 6.3_Early_choices_of_null_hypothesis
    * 7_Null_hypothesis_statistical_significance_testing
    * 8_Criticism
    * 9_Alternatives
    * 10_Philosophy
    * 11_Education
    * 12_See_also
    * 13_References
    * 14_Further_reading
    * 15_External_links
          o 15.1_Online_calculators
***** The testing process[edit] *****
In the statistics literature, statistical hypothesis testing plays a
fundamental role.[4] The usual line of reasoning is as follows:
   1. There is an initial research hypothesis of which the truth is unknown.
   2. The first step is to state the relevant null and alternative hypotheses.
      This is important, as mis-stating the hypotheses will muddy the rest of
      the process.
   3. The second step is to consider the statistical_assumptions being made
      about the sample in doing the test; for example, assumptions about the
      statistical_independence or about the form of the distributions of the
      observations. This is equally important as invalid assumptions will mean
      that the results of the test are invalid.
   4. Decide which test is appropriate, and state the relevant test_statistic
      T.
   5. Derive the distribution of the test statistic under the null hypothesis
      from the assumptions. In standard cases this will be a well-known result.
      For example, the test statistic might follow a Student's_t_distribution
      or a normal_distribution.
   6. Select a significance level (Î±), a probability threshold below which the
      null hypothesis will be rejected. Common values are 5% and 1%.
   7. The distribution of the test statistic under the null hypothesis
      partitions the possible values of T into those for which the null
      hypothesis is rejected—the so-called critical region—and those for which
      it is not. The probability of the critical region is Î±.
   8. Compute from the observations the observed value tobs of the test
      statistic T.
   9. Decide to either reject the null hypothesis in favor of the alternative
      or not reject it. The decision rule is to reject the null hypothesis H0
      if the observed value tobs is in the critical region, and to accept or
      "fail to reject" the hypothesis otherwise.
An alternative process is commonly used:
   1. Compute from the observations the observed value tobs of the test
      statistic T.
   2. Calculate the p-value. This is the probability, under the null
      hypothesis, of sampling a test statistic at least as extreme as that
      which was observed.
   3. Reject the null hypothesis, in favor of the alternative hypothesis, if
      and only if the p-value is less than the significance level (the selected
      probability) threshold.
The two processes are equivalent.[5] The former process was advantageous in the
past when only tables of test statistics at common probability thresholds were
available. It allowed a decision to be made without the calculation of a
probability. It was adequate for classwork and for operational use, but it was
deficient for reporting results.
The latter process relied on extensive tables or on computational support not
always available. The explicit calculation of a probability is useful for
reporting. The calculations are now trivially performed with appropriate
software.
The difference in the two processes applied to the Radioactive suitcase example
(below):
    * "The Geiger-counter reading is 10. The limit is 9. Check the suitcase."
    * "The Geiger-counter reading is high; 97% of safe suitcases have lower
      readings. The limit is 95%. Check the suitcase."
The former report is adequate, the latter gives a more detailed explanation of
the data and the reason why the suitcase is being checked.
It is important to note the difference between accepting the null hypothesis
and simply failing to reject it. The "fail to reject" terminology highlights
the fact that the null hypothesis is assumed to be true from the start of the
test; if there is a lack of evidence against it, it simply continues to be
assumed true. The phrase "accept the null hypothesis" may suggest it has been
proved simply because it has not been disproved, a logical fallacy known as the
argument_from_ignorance. Unless a test with particularly high power is used,
the idea of "accepting" the null hypothesis may be dangerous. Nonetheless the
terminology is prevalent throughout statistics, where the meaning actually
intended is well understood.
The processes described here are perfectly adequate for computation. They
seriously neglect the design_of_experiments considerations.[6][7]
It is particularly critical that appropriate sample sizes be estimated before
conducting the experiment.
The phrase "test of significance" was coined by statistician Ronald_Fisher.[8]
**** Interpretation[edit] ****
The p-value is the probability that a given result (or a more significant
result) would occur under the null hypothesis. For example, say that a fair
coin is tested for fairness (the null hypothesis). At a significance level of
0.05, the fair coin would be expected to (incorrectly) reject the null
hypothesis in about 1 out of every 20 tests. The p-value does not provide the
probability that either hypothesis is correct (a common source of confusion).
[9]
If the p-value is less than the chosen significance threshold (equivalently, if
the observed test statistic is in the critical region), then we say the null
hypothesis is rejected at the chosen level of significance. Rejection of the
null hypothesis is a conclusion. This is like a "guilty" verdict in a criminal
trial: the evidence is sufficient to reject innocence, thus proving guilt. We
might accept the alternative hypothesis (and the research hypothesis).
If the p-value is not less than the chosen significance threshold
(equivalently, if the observed test statistic is outside the critical region),
then the evidence is insufficient to support a conclusion. (This is similar to
a "not guilty" verdict.) The researcher typically gives extra consideration to
those cases where the p-value is close to the significance level.
Some people find it helpful to think of the hypothesis testing framework as
analogous to a mathematical proof_by_contradiction.[10]
In the Lady tasting tea example (below), Fisher required the Lady to properly
categorize all of the cups of tea to justify the conclusion that the result was
unlikely to result from chance. His test revealed that if the lady was
effectively guessing at random (the null hypothesis), there was a 1.4% chance
that the observed results (perfectly ordered tea) would occur.
Whether rejection of the null hypothesis truly justifies acceptance of the
research hypothesis depends on the structure of the hypotheses. Rejecting the
hypothesis that a large paw print originated from a bear does not immediately
prove the existence of Bigfoot. Hypothesis testing emphasizes the rejection,
which is based on a probability, rather than the acceptance, which requires
extra steps of logic.
"The probability of rejecting the null hypothesis is a function of five
factors: whether the test is one- or two tailed, the level of significance, the
standard deviation, the amount of deviation from the null hypothesis, and the
number of observations."[11] These factors are a source of criticism; factors
under the control of the experimenter/analyst give the results an appearance of
subjectivity.
**** Use and importance[edit] ****
Statistics are helpful in analyzing most collections of data. This is equally
true of hypothesis testing which can justify conclusions even when no
scientific theory exists. In the Lady tasting tea example, it was "obvious"
that no difference existed between (milk poured into tea) and (tea poured into
milk). The data contradicted the "obvious".
Real world applications of hypothesis testing include:[12]
    * Testing whether more men than women suffer from nightmares
    * Establishing authorship of documents
    * Evaluating the effect of the full moon on behavior
    * Determining the range at which a bat can detect an insect by echo
    * Deciding whether hospital carpeting results in more infections
    * Selecting the best means to stop smoking
    * Checking whether bumper stickers reflect car owner behavior
    * Testing the claims of handwriting analysts
Statistical hypothesis testing plays an important role in the whole of
statistics and in statistical_inference. For example, Lehmann (1992) in a
review of the fundamental paper by Neyman and Pearson (1933) says:
"Nevertheless, despite their shortcomings, the new paradigm formulated in the
1933 paper, and the many developments carried out within its framework continue
to play a central role in both the theory and practice of statistics and can be
expected to do so in the foreseeable future".
Significance testing has been the favored statistical tool in some experimental
social sciences (over 90% of articles in the Journal of Applied Psychology
during the early 1990s).[13] Other fields have favored the estimation of
parameters (e.g. effect_size). Significance testing is used as a substitute for
the traditional comparison of predicted value and experimental result at the
core of the scientific_method. When theory is only capable of predicting the
sign of a relationship, a directional (one-sided) hypothesis test can be
configured so that only a statistically significant result supports theory.
This form of theory appraisal is the most heavily criticized application of
hypothesis testing.
**** Cautions[edit] ****
"If the government required statistical procedures to carry warning labels like
those on drugs, most inference methods would have long labels indeed."[14] This
caution applies to hypothesis tests and alternatives to them.
The successful hypothesis test is associated with a probability and a type-
I error rate. The conclusion might be wrong.
The conclusion of the test is only as solid as the sample upon which it is
based. The design of the experiment is critical. A number of unexpected effects
have been observed including:
    * The clever_Hans_effect. A horse appeared to be capable of doing simple
      arithmetic.
    * The Hawthorne_effect. Industrial workers were more productive in better
      illumination, and most productive in worse.
    * The placebo_effect. Pills with no medically active ingredients were
      remarkably effective.
A statistical analysis of misleading data produces misleading conclusions. The
issue of data quality can be more subtle. In forecasting for example, there is
no agreement on a measure of forecast accuracy. In the absence of a consensus
measurement, no decision based on measurements will be without controversy.
The book How_to_Lie_with_Statistics[15][16] is the most popular book on
statistics ever published.[17] It does not much consider hypothesis testing,
but its cautions are applicable, including: Many claims are made on the basis
of samples too small to convince. If a report does not mention sample size, be
doubtful.
Hypothesis testing acts as a filter of statistical conclusions; only those
results meeting a probability threshold are publishable. Economics also acts as
a publication filter; only those results favorable to the author and funding
source may be submitted for publication. The impact of filtering on publication
is termed publication_bias. A related problem is that of multiple_testing
(sometimes linked to data_mining), in which a variety of tests for a variety of
possible effects are applied to a single data set and only those yielding a
significant result are reported. These are often dealt with by using
multiplicity correction procedures that control the family_wise_error_rate
(FWER) or the false_discovery_rate (FDR).
Those making critical decisions based on the results of a hypothesis test are
prudent to look at the details rather than the conclusion alone. In the
physical sciences most results are fully accepted only when independently
confirmed. The general advice concerning statistics is, "Figures never lie, but
liars figure" (anonymous).
***** Examples[edit] *****
**** Human sex ratio[edit] ****
Main article: Human_sex_ratio
The earliest use of statistical hypothesis testing is generally credited to the
question of whether male and female births are equally likely (null
hypothesis), which was addressed in the 1700s by John_Arbuthnot (1710),[18] and
later by Pierre-Simon_Laplace (1770s).[19]
Arbuthnot examined birth records in London for each of the 82 years from 1629
to 1710, and applied the sign_test, a simple non-parametric_test.[20][21][22]
In every year, the number of males born in London exceeded the number of
females. Considering more male or more female births as equally likely, the
probability of the observed outcome is 0.582, or about 1 in
4,8360,0000,0000,0000,0000,0000; in modern terms, this is the p-value. This is
vanishingly small, leading Arbuthnot that this was not due to chance, but to
divine providence: "From whence it follows, that it is Art, not Chance, that
governs." In modern terms, he rejected the null hypothesis of equally likely
male and female births at the p = 1/282 significance level.
Laplace considered the statistics of almost half a million births. The
statistics showed an excess of boys compared to girls.[23][24] He concluded by
calculation of a p-value that the excess was a real, but unexplained, effect.
[25]
**** Lady tasting tea[edit] ****
Main article: Lady_tasting_tea
In a famous example of hypothesis testing, known as the Lady tasting tea,[26]
Dr. Muriel_Bristol, a female colleague of Fisher claimed to be able to tell
whether the tea or the milk was added first to a cup. Fisher proposed to give
her eight cups, four of each variety, in random order. One could then ask what
the probability was for her getting the number she got correct, but just by
chance. The null hypothesis was that the Lady had no such ability. The test
statistic was a simple count of the number of successes in selecting the 4
cups. The critical region was the single case of 4 successes of 4 possible
based on a conventional probability criterion (< 5%). A pattern of 4 successes
corresponds to 1 out of 70 possible combinations (pâ 1.4%). Fisher asserted
that no alternative hypothesis was (ever) required. The lady correctly
identified every cup,[27] which would be considered a statistically significant
result.
**** Courtroom trial[edit] ****
A statistical test procedure is comparable to a criminal trial; a defendant is
considered not guilty as long as his or her guilt is not proven. The prosecutor
tries to prove the guilt of the defendant. Only when there is enough evidence
for the prosecution is the defendant convicted.
In the start of the procedure, there are two hypotheses      H  0
{\displaystyle H_{0}}  [H_{0}]: "the defendant is not guilty", and      H  1
{\displaystyle H_{1}}  [H_{1}]: "the defendant is guilty". The first one,
H  0     {\displaystyle H_{0}}  [H_{0}], is called the null_hypothesis, and is
for the time being accepted. The second one,      H  1     {\displaystyle H_
{1}}  [H_{1}], is called the alternative hypothesis. It is the alternative
hypothesis that one hopes to support.
The hypothesis of innocence is only rejected when an error is very unlikely,
because one doesn't want to convict an innocent defendant. Such an error is
called error_of_the_first_kind (i.e., the conviction of an innocent person),
and the occurrence of this error is controlled to be rare. As a consequence of
this asymmetric behaviour, an error_of_the_second_kind (acquitting a person who
committed the crime), is more common.
                        H0 is true       H1 is true
                        Truly not guilty Truly guilty
Accept null hypothesis   Right decision  Wrong decision
       Acquittal                          Type II Error
Reject null hypothesis  Wrong decision   Right decision
      Conviction          Type I Error
A criminal trial can be regarded as either or both of two decision processes:
guilty vs not guilty or evidence vs a threshold ("beyond a reasonable doubt").
In one view, the defendant is judged; in the other view the performance of the
prosecution (which bears the burden of proof) is judged. A hypothesis test can
be regarded as either a judgment of a hypothesis or as a judgment of evidence.
**** Philosopher's beans[edit] ****
The following example was produced by a philosopher describing scientific
methods generations before hypothesis testing was formalized and popularized.
[28]
     Few beans of this handful are white.
     Most beans in this bag are white.
     Therefore: Probably, these beans were taken from another bag.
     This is an hypothetical inference.
The beans in the bag are the population. The handful are the sample. The null
hypothesis is that the sample originated from the population. The criterion for
rejecting the null-hypothesis is the "obvious" difference in appearance (an
informal difference in the mean). The interesting result is that consideration
of a real population and a real sample produced an imaginary bag. The
philosopher was considering logic rather than probability. To be a real
statistical hypothesis test, this example requires the formalities of a
probability calculation and a comparison of that probability to a standard.
A simple generalization of the example considers a mixed bag of beans and a
handful that contain either very few or very many white beans. The
generalization considers both extremes. It requires more calculations and more
comparisons to arrive at a formal answer, but the core philosophy is unchanged;
If the composition of the handful is greatly different from that of the bag,
then the sample probably originated from another bag. The original example is
termed a one-sided or a one-tailed test while the generalization is termed a
two-sided or two-tailed test.
The statement also relies on the inference that the sampling was random. If
someone had been picking through the bag to find white beans, then it would
explain why the handful had so many white beans, and also explain why the
number of white beans in the bag was depleted (although the bag is probably
intended to be assumed much larger than one's hand).
**** Clairvoyant card game[edit] ****
A person (the subject) is tested for clairvoyance. They are shown the reverse
of a randomly chosen playing card 25 times and asked which of the four suits it
belongs to. The number of hits, or correct answers, is called X.
As we try to find evidence of their clairvoyance, for the time being the null
hypothesis is that the person is not clairvoyant.[29] The alternative is: the
person is (more or less) clairvoyant.
If the null hypothesis is valid, the only thing the test person can do is
guess. For every card, the probability (relative frequency) of any single suit
appearing is 1/4. If the alternative is valid, the test subject will predict
the suit correctly with probability greater than 1/4. We will call the
probability of guessing correctly p. The hypotheses, then, are:
    * null hypothesis      :    H  0   : p =    1 4      {\displaystyle {\text
      {:}}\qquad H_{0}:p={\tfrac {1}{4}}}  [\text{:} \qquad H_0: p = \tfrac 14]
          (just guessing)
and
    * alternative hypothesis      :   H  1   : p >    1 4      {\displaystyle
      {\text{:}}H_{1}:p>{\tfrac {1}{4}}}  [\text{:} H_1: p > \tfrac 14]    
      (true clairvoyant).
When the test subject correctly predicts all 25 cards, we will consider them
clairvoyant, and reject the null hypothesis. Thus also with 24 or 23 hits. With
only 5 or 6 hits, on the other hand, there is no cause to consider them so. But
what about 12 hits, or 17 hits? What is the critical number, c, of hits, at
which point we consider the subject to be clairvoyant? How do we determine the
critical value c? With the choice c=25 (i.e. we only accept clairvoyance when
all cards are predicted correctly) we're more critical than with c=10. In the
first case almost no test subjects will be recognized to be clairvoyant, in the
second case, a certain number will pass the test. In practice, one decides how
critical one will be. That is, one decides how often one accepts an error of
the first kind â a false_positive, or Type I error. With c = 25 the
probability of such an error is:
         P (  reject&#xA0;   H  0   &#x2223;  H  0    &#xA0;is valid  ) = P ( X
      = 25 &#x2223; p =    1 4    ) =   (    1 4    )   25   &#x2248;  10
      &#x2212; 15   ,   {\displaystyle P({\text{reject }}H_{0}\mid H_{0}{\text
      { is valid}})=P(X=25\mid p={\tfrac {1}{4}})=\left({\tfrac {1}{4}}\right)^
      {25}\approx 10^{-15},}  [P(\text{reject }H_0 \mid H_0 \text{ is valid}) =
      P(X = 25\mid p=\tfrac 14)=\left(\tfrac 14\right)^{25}\approx10^{-15},]
and hence, very small. The probability of a false positive is the probability
of randomly guessing correctly all 25 times.
Being less critical, with c=10, gives:
         P (  reject&#xA0;   H  0   &#x2223;  H  0    &#xA0;is valid  ) = P ( X
      &#x2265; 10 &#x2228; X &#x2264; 2 &#x2223; p =    1 4    ) =  &#x2211;  k
      = 0   2   P ( X = k &#x2223; p =    1 4    ) +  &#x2211;  k = 10   25   P
      ( X = k &#x2223; p =    1 4    ) &#x2248; 0  .  103.   {\displaystyle P(
      {\text{reject }}H_{0}\mid H_{0}{\text{ is valid}})=P(X\geq 10\lor X\leq
      2\mid p={\tfrac {1}{4}})=\sum _{k=0}^{2}P(X=k\mid p={\tfrac {1}{4}})+\sum
      _{k=10}^{25}P(X=k\mid p={\tfrac {1}{4}})\approx 0{.}103.}  [
      {\displaystyle P({\text{reject }}H_{0}\mid H_{0}{\text{ is valid}})=P
      (X\geq 10\lor X\leq 2\mid p={\tfrac {1}{4}})=\sum _{k=0}^{2}P(X=k\mid p=
      {\tfrac {1}{4}})+\sum _{k=10}^{25}P(X=k\mid p={\tfrac {1}{4}})\approx 0
      {.}103.}]
Thus, c = 10 yields a much greater probability of false positive.
Before the test is actually performed, the maximum acceptable probability of a
Type I error (Î±) is determined. Typically, values in the range of 1% to 5% are
selected. (If the maximum acceptable error rate is zero, an infinite number of
correct guesses is required.) Depending on this Type 1 error rate, the critical
value c is calculated. For example, if we select an error rate of 1%, c is
calculated thus:
         P (  reject&#xA0;   H  0   &#x2223;  H  0    &#xA0;is valid  ) = P ( X
      &#x2265; c &#x2223; p =    1 4    ) &#x2264; 0  .  01.   {\displaystyle P
      ({\text{reject }}H_{0}\mid H_{0}{\text{ is valid}})=P(X\geq c\mid p=
      {\tfrac {1}{4}})\leq 0{.}01.}  [P(\text{reject }H_0 \mid H_0 \text{ is
      valid}) = P(X \ge c\mid p=\tfrac 14) \le 0{.}01.]
From all the numbers c, with this property, we choose the smallest, in order to
minimize the probability of a Type II error, a false_negative. For the above
example, we select:     c = 13   {\displaystyle c=13}  [c=13].
**** Radioactive suitcase[edit] ****
As an example, consider determining whether a suitcase contains some
radioactive material. Placed under a Geiger_counter, it produces 10 counts per
minute. The null hypothesis is that no radioactive material is in the suitcase
and that all measured counts are due to ambient radioactivity typical of the
surrounding air and harmless objects. We can then calculate how likely it is
that we would observe 10 counts per minute if the null hypothesis were true. If
the null hypothesis predicts (say) on average 9 counts per minute, then
according to the Poisson_distribution typical for radioactive_decay there is
about 41% chance of recording 10 or more counts. Thus we can say that the
suitcase is compatible with the null hypothesis (this does not guarantee that
there is no radioactive material, just that we don't have enough evidence to
suggest there is). On the other hand, if the null hypothesis predicts 3 counts
per minute (for which the Poisson distribution predicts only 0.1% chance of
recording 10 or more counts) then the suitcase is not compatible with the null
hypothesis, and there are likely other factors responsible to produce the
measurements.
The test does not directly assert the presence of radioactive material. A
successful test asserts that the claim of no radioactive material present is
unlikely given the reading (and therefore ...). The double negative (disproving
the null hypothesis) of the method is confusing, but using a counter-example to
disprove is standard mathematical practice. The attraction of the method is its
practicality. We know (from experience) the expected range of counts with only
ambient radioactivity present, so we can say that a measurement is unusually
large. Statistics just formalizes the intuitive by using numbers instead of
adjectives. We probably do not know the characteristics of the radioactive
suitcases; We just assume that they produce larger readings.
To slightly formalize intuition: radioactivity is suspected if the Geiger-count
with the suitcase is among or exceeds the greatest (5% or 1%) of the Geiger-
counts made with ambient radiation alone. This makes no assumptions about the
distribution of counts. Many ambient radiation observations are required to
obtain good probability estimates for rare events.
The test described here is more fully the null-hypothesis statistical
significance test. The null hypothesis represents what we would believe by
default, before seeing any evidence. Statistical_significance is a possible
finding of the test, declared when the observed sample is unlikely to have
occurred by chance if the null hypothesis were true. The name of the test
describes its formulation and its possible outcome. One characteristic of the
test is its crisp decision: to reject or not reject the null hypothesis. A
calculated value is compared to a threshold, which is determined from the
tolerable risk of error.
***** Definition of terms[edit] *****
The following definitions are mainly based on the exposition in the book by
Lehmann and Romano:[4]
  Statistical hypothesis 
      A statement about the parameters describing a population (not a sample).
  Statistic 
      A value calculated from a sample without any unknown parameters, often to
      summarize the sample for comparison purposes.
  Simple hypothesis 
      Any hypothesis which specifies the population distribution completely.
  Composite hypothesis 
      Any hypothesis which does not specify the population distribution
      completely.
  Null_hypothesis (H0) 
      A hypothesis associated with a contradiction to a theory one would like
      to prove.
  Positive data 
      Data that enable the investigator to reject a null hypothesis.
  Alternative_hypothesis (H1) 
      A hypothesis (often composite) associated with a theory one would like to
      prove.
  Statistical test 
      A procedure whose inputs are samples and whose result is a hypothesis.
  Region of acceptance 
      The set of values of the test statistic for which we fail to reject the
      null hypothesis.
  Region of rejection / Critical region
      The set of values of the test statistic for which the null hypothesis is
      rejected.
  Critical_value
      The threshold value delimiting the regions of acceptance and rejection
      for the test statistic.
  Power_of_a_test (1 â Î²)
      The test's probability of correctly rejecting the null hypothesis. The
      complement of the false_negative rate, Î². Power is termed sensitivity in
      biostatistics. ("This is a sensitive test. Because the result is
      negative, we can confidently say that the patient does not have the
      condition.") See sensitivity_and_specificity and Type_I_and_type_II
      errors for exhaustive definitions.
  Size
      For simple hypotheses, this is the test's probability of incorrectly
      rejecting the null hypothesis. The false_positive rate. For composite
      hypotheses this is the supremum of the probability of rejecting the null
      hypothesis over all cases covered by the null hypothesis. The complement
      of the false positive rate is termed specificity in biostatistics. ("This
      is a specific test. Because the result is positive, we can confidently
      say that the patient has the condition.") See sensitivity_and_specificity
      and Type_I_and_type_II_errors for exhaustive definitions.
  Significance level of a test (Î±)
      It is the upper bound imposed on the size of a test. Its value is chosen
      by the statistician prior to looking at the data or choosing any
      particular test to be used. It is the maximum exposure to erroneously
      rejecting H0 he/she is ready to accept. Testing H0 at significance level
      Î± means testing H0 with a test whose size does not exceed Î±. In most
      cases, one uses tests whose size is equal to the significance level.
  p-value
      The probability, assuming the null hypothesis is true, of observing a
      result at least as extreme as the test statistic. In case of a composite
      null hypothesis, the worst case probability.
  Statistical_significance test 
      A predecessor to the statistical hypothesis test (see the Origins
      section). An experimental result was said to be statistically significant
      if a sample was sufficiently inconsistent with the (null) hypothesis.
      This was variously considered common sense, a pragmatic heuristic for
      identifying meaningful experimental results, a convention establishing a
      threshold of statistical evidence or a method for drawing conclusions
      from data. The statistical hypothesis test added mathematical rigor and
      philosophical consistency to the concept by making the alternative
      hypothesis explicit. The term is loosely used to describe the modern
      version which is now part of statistical hypothesis testing.
  Conservative test 
      A test is conservative if, when constructed for a given nominal
      significance level, the true probability of incorrectly rejecting the
      null hypothesis is never greater than the nominal level.
  Exact_test
      A test in which the significance level or critical value can be computed
      exactly, i.e., without any approximation. In some contexts this term is
      restricted to tests applied to categorical_data and to permutation_tests,
      in which computations are carried out by complete enumeration of all
      possible outcomes and their probabilities.
A statistical hypothesis test compares a test statistic (z or t for examples)
to a threshold. The test statistic (the formula found in the table below) is
based on optimality. For a fixed level of Type I error rate, use of these
statistics minimizes Type II error rates (equivalent to maximizing power). The
following terms describe tests in terms of such optimality:
  Most powerful test
      For a given size or significance level, the test with the greatest power
      (probability of rejection) for a given value of the parameter(s) being
      tested, contained in the alternative hypothesis.
  Uniformly_most_powerful_test (UMP)
      A test with the greatest power for all values of the parameter(s) being
      tested, contained in the alternative hypothesis.
***** Common test statistics[edit] *****
Main article: Test_statistic
***** Variations and sub-classes[edit] *****
Statistical hypothesis testing is a key technique of both frequentist_inference
and Bayesian_inference, although the two types of inference have notable
differences. Statistical hypothesis tests define a procedure that controls
(fixes) the probability of incorrectly deciding that a default position (null
hypothesis) is incorrect. The procedure is based on how likely it would be for
a set of observations to occur if the null hypothesis were true. Note that this
probability of making an incorrect decision is not the probability that the
null hypothesis is true, nor whether any specific alternative hypothesis is
true. This contrasts with other possible techniques of decision_theory in which
the null and alternative_hypothesis are treated on a more equal basis.
One naÃ¯ve Bayesian approach to hypothesis testing is to base decisions on the
posterior_probability,[30][31] but this fails when comparing point and
continuous hypotheses. Other approaches to decision making, such as Bayesian
decision_theory, attempt to balance the consequences of incorrect decisions
across all possibilities, rather than concentrating on a single null
hypothesis. A number of other approaches to reaching a decision based on data
are available via decision_theory and optimal_decisions, some of which have
desirable properties. Hypothesis testing, though, is a dominant approach to
data analysis in many fields of science. Extensions to the theory of hypothesis
testing include the study of the power of tests, i.e. the probability of
correctly rejecting the null hypothesis given that it is false. Such
considerations can be used for the purpose of sample_size_determination prior
to the collection of data.
***** History[edit] *****
**** Early use[edit] ****
While hypothesis testing was popularized early in the 20th century, early forms
were used in the 1700s. The first use is credited to John_Arbuthnot (1710),[32]
followed by Pierre-Simon_Laplace (1770s), in analyzing the human_sex_ratio at
birth; see Â§ Human_sex_ratio.
**** Modern origins and early controversy[edit] ****
Modern significance testing is largely the product of Karl_Pearson (p-value,
Pearson's_chi-squared_test), William_Sealy_Gosset (Student's_t-distribution),
and Ronald_Fisher ("null_hypothesis", analysis_of_variance, "significance
test"), while hypothesis testing was developed by Jerzy_Neyman and Egon_Pearson
(son of Karl). Ronald Fisher began his life in statistics as a Bayesian (Zabell
1992), but Fisher soon grew disenchanted with the subjectivity involved (namely
use of the principle_of_indifference when determining prior probabilities), and
sought to provide a more "objective" approach to inductive inference.[33]
Fisher was an agricultural statistician who emphasized rigorous experimental
design and methods to extract a result from few samples assuming Gaussian
distributions. Neyman (who teamed with the younger Pearson) emphasized
mathematical rigor and methods to obtain more results from many samples and a
wider range of distributions. Modern hypothesis testing is an inconsistent
hybrid of the Fisher vs Neyman/Pearson formulation, methods and terminology
developed in the early 20th century.
Fisher popularized the "significance test". He required a null-hypothesis
(corresponding to a population frequency distribution) and a sample. His (now
familiar) calculations determined whether to reject the null-hypothesis or not.
Significance testing did not utilize an alternative hypothesis so there was no
concept of a Type II error.
The p-value was devised as an informal, but objective, index meant to help a
researcher determine (based on other knowledge) whether to modify future
experiments or strengthen one's faith in the null hypothesis.[34] Hypothesis
testing (and Type I/II errors) was devised by Neyman and Pearson as a more
objective alternative to Fisher's p-value, also meant to determine researcher
behaviour, but without requiring any inductive inference by the researcher.[35]
[36]
Neyman & Pearson considered a different problem (which they called "hypothesis
testing"). They initially considered two simple hypotheses (both with frequency
distributions). They calculated two probabilities and typically selected the
hypothesis associated with the higher probability (the hypothesis more likely
to have generated the sample). Their method always selected a hypothesis. It
also allowed the calculation of both types of error probabilities.
Fisher and Neyman/Pearson clashed bitterly. Neyman/Pearson considered their
formulation to be an improved generalization of significance testing.(The
defining paper[35] was abstract. Mathematicians have generalized and refined
the theory for decades.[37]) Fisher thought that it was not applicable to
scientific research because often, during the course of the experiment, it is
discovered that the initial assumptions about the null hypothesis are
questionable due to unexpected sources of error. He believed that the use of
rigid reject/accept decisions based on models formulated before data is
collected was incompatible with this common scenario faced by scientists and
attempts to apply this method to scientific research would lead to mass
confusion.[38]
The dispute between Fisher and NeymanâPearson was waged on philosophical
grounds, characterized by a philosopher as a dispute over the proper role of
models in statistical inference.[39]
Events intervened: Neyman accepted a position in the western hemisphere,
breaking his partnership with Pearson and separating disputants (who had
occupied the same building) by much of the planetary diameter. World War II
provided an intermission in the debate. The dispute between Fisher and Neyman
terminated (unresolved after 27 years) with Fisher's death in 1962. Neyman
wrote a well-regarded eulogy.[40] Some of Neyman's later publications reported
p-values and significance levels.[41]
The modern version of hypothesis testing is a hybrid of the two approaches that
resulted from confusion by writers of statistical textbooks (as predicted by
Fisher) beginning in the 1940s.[42] (But signal_detection, for example, still
uses the Neyman/Pearson formulation.) Great conceptual differences and many
caveats in addition to those mentioned above were ignored. Neyman and Pearson
provided the stronger terminology, the more rigorous mathematics and the more
consistent philosophy, but the subject taught today in introductory statistics
has more similarities with Fisher's method than theirs.[43] This history
explains the inconsistent terminology (example: the null hypothesis is never
accepted, but there is a region of acceptance).
Sometime around 1940,[42] in an apparent effort to provide researchers with a
"non-controversial"[44] way to have_their_cake_and_eat_it_too, the authors of
statistical text books began anonymously combining these two strategies by
using the p-value in place of the test_statistic (or data) to test against the
NeymanâPearson "significance level".[42] Thus, researchers were encouraged to
infer the strength of their data against some null_hypothesis using p-values,
while also thinking they are retaining the post-data collection objectivity
provided by hypothesis testing. It then became customary for the null
hypothesis, which was originally some realistic research hypothesis, to be used
almost solely as a strawman "nil" hypothesis (one where a treatment has no
effect, regardless of the context).[45]
                A comparison between Fisherian, frequentist (NeymanâPearson)
  Fisher's null
# hypothesis    NeymanâPearson decision theory
  testing
  Set up a
  statistical
  null
  hypothesis.   Set up two statistical hypotheses, H1 and H2, and decide about Î±, Î², and
1 The null need sample size before the experiment, based on subjective cost-benefit
  not be a nil  considerations. These define a rejection region for each hypothesis.
  hypothesis
  (i.e., zero
  difference).
  Report the
  exact level
  of
  significance
  (e.g. p =
  0.051 or p =
  0.049). Do
  not use a
  conventional
  5% level, and
  do not talk
  about
  accepting or  If the data falls into the rejection region of H1, accept H2; otherwise accept
2 rejecting     H1. Note that accepting a hypothesis does not mean that you believe in it, but
  hypotheses.   only that you act as if it were true.
  If the result
  is "not
  significant",
  draw no
  conclusions
  and make no
  decisions,
  but suspend
  judgement
  until further
  data is
  available.
  Use this
  procedure
  only if
  little is
  known about
  the problem
  at hand, and  The usefulness of the procedure is limited among others to situations where
  only to draw  you have a disjunction of hypotheses (e.g. either Î¼1 = 8 or Î¼2 = 10 is true)
3 provisional   and where you can make meaningful cost-benefit trade-offs for choosing alpha
  conclusions   and beta.
  in the
  context of an
  attempt to
  understand
  the
  experimental
  situation.
**** Early choices of null hypothesis[edit] ****
Paul_Meehl has argued that the epistemological importance of the choice of null
hypothesis has gone largely unacknowledged. When the null hypothesis is
predicted by theory, a more precise experiment will be a more severe test of
the underlying theory. When the null hypothesis defaults to "no difference" or
"no effect", a more precise experiment is a less severe test of the theory that
motivated performing the experiment.[46] An examination of the origins of the
latter practice may therefore be useful:
1778: Pierre_Laplace compares the birthrates of boys and girls in multiple
European cities. He states: "it is natural to conclude that these possibilities
are very nearly in the same ratio". Thus Laplace's null hypothesis that the
birthrates of boys and girls should be equal given "conventional wisdom".[23]
1900: Karl_Pearson develops the chi_squared_test to determine "whether a given
form of frequency curve will effectively describe the samples drawn from a
given population." Thus the null hypothesis is that a population is described
by some distribution predicted by theory. He uses as an example the numbers of
five and sixes in the Weldon_dice_throw_data.[47]
1904: Karl_Pearson develops the concept of "contingency" in order to determine
whether outcomes are independent of a given categorical factor. Here the null
hypothesis is by default that two things are unrelated (e.g. scar formation and
death rates from smallpox).[48] The null hypothesis in this case is no longer
predicted by theory or conventional wisdom, but is instead the principle_of
indifference that led Fisher and others to dismiss the use of "inverse
probabilities".[49]
***** Null hypothesis statistical significance testing[edit] *****
An example of NeymanâPearson hypothesis testing can be made by a change to
the radioactive suitcase example. If the "suitcase" is actually a shielded
container for the transportation of radioactive material, then a test might be
used to select among three hypotheses: no radioactive source present, one
present, two (all) present. The test could be required for safety, with actions
required in each case. The NeymanâPearson_lemma of hypothesis testing says
that a good criterion for the selection of hypotheses is the ratio of their
probabilities (a likelihood_ratio). A simple method of solution is to select
the hypothesis with the highest probability for the Geiger counts observed. The
typical result matches intuition: few counts imply no source, many counts imply
two sources and intermediate counts imply one source. Notice also that usually
there are problems for proving_a_negative. Null hypotheses should be at least
falsifiable.
NeymanâPearson theory can accommodate both prior probabilities and the costs
of actions resulting from decisions.[50] The former allows each test to
consider the results of earlier tests (unlike Fisher's significance tests). The
latter allows the consideration of economic issues (for example) as well as
probabilities. A likelihood ratio remains a good criterion for selecting among
hypotheses.
The two forms of hypothesis testing are based on different problem
formulations. The original test is analogous to a true/false question; the
NeymanâPearson test is more like multiple choice. In the view of Tukey[51]
the former produces a conclusion on the basis of only strong evidence while the
latter produces a decision on the basis of available evidence. While the two
tests seem quite different both mathematically and philosophically, later
developments lead to the opposite claim. Consider many tiny radioactive
sources. The hypotheses become 0,1,2,3... grains of radioactive sand. There is
little distinction between none or some radiation (Fisher) and 0 grains of
radioactive sand versus all of the alternatives (NeymanâPearson). The major
NeymanâPearson paper of 1933[35] also considered composite hypotheses (ones
whose distribution includes an unknown parameter). An example proved the
optimality of the (Student's) t-test, "there can be no better test for the
hypothesis under consideration" (p 321). NeymanâPearson theory was proving
the optimality of Fisherian methods from its inception.
Fisher's significance testing has proven a popular flexible statistical tool in
application with little mathematical growth potential. NeymanâPearson
hypothesis testing is claimed as a pillar of mathematical statistics,[52]
creating a new paradigm for the field. It also stimulated new applications in
statistical_process_control, detection_theory, decision_theory and game_theory.
Both formulations have been successful, but the successes have been of a
different character.
The dispute over formulations is unresolved. Science primarily uses Fisher's
(slightly modified) formulation as taught in introductory statistics.
Statisticians study NeymanâPearson theory in graduate school. Mathematicians
are proud of uniting the formulations. Philosophers consider them separately.
Learned opinions deem the formulations variously competitive (Fisher vs
Neyman), incompatible[33] or complementary.[37] The dispute has become more
complex since Bayesian inference has achieved respectability.
The terminology is inconsistent. Hypothesis testing can mean any mixture of two
formulations that both changed with time. Any discussion of significance
testing vs hypothesis testing is doubly vulnerable to confusion.
Fisher thought that hypothesis testing was a useful strategy for performing
industrial quality control, however, he strongly disagreed that hypothesis
testing could be useful for scientists.[34] Hypothesis testing provides a means
of finding test statistics used in significance testing.[37] The concept of
power is useful in explaining the consequences of adjusting the significance
level and is heavily used in sample_size_determination. The two methods remain
philosophically distinct.[39] They usually (but not always) produce the same
mathematical answer. The preferred answer is context dependent.[37] While the
existing merger of Fisher and NeymanâPearson theories has been heavily
criticized, modifying the merger to achieve Bayesian goals has been considered.
[53]
***** Criticism[edit] *****
See also: p-value_Â§ Misconceptions
Criticism of statistical hypothesis testing fills volumes[54][55][56][57][58]
[59] citing 300â400 primary references[citation_needed]. Much of the
criticism can be summarized by the following issues:
    * The interpretation of a p-value is dependent upon stopping rule and
      definition of multiple comparison. The former often changes during the
      course of a study and the latter is unavoidably ambiguous. (i.e. "p
      values depend on both the (data) observed and on the other possible
      (data) that might have been observed but weren't").[60]
    * Confusion resulting (in part) from combining the methods of Fisher and
      NeymanâPearson which are conceptually distinct.[51]
    * Emphasis on statistical significance to the exclusion of estimation and
      confirmation by repeated experiments.[61]
    * Rigidly requiring statistical significance as a criterion for
      publication, resulting in publication_bias.[62] Most of the criticism is
      indirect. Rather than being wrong, statistical hypothesis testing is
      misunderstood, overused and misused.
    * When used to detect whether a difference exists between groups, a paradox
      arises. As improvements are made to experimental design (e.g. increased
      precision of measurement and sample size), the test becomes more lenient.
      Unless one accepts the absurd assumption that all sources of noise in the
      data cancel out completely, the chance of finding statistical
      significance in either direction approaches 100%.[63]
    * Layers of philosophical concerns. The probability of statistical
      significance is a function of decisions made by experimenters/analysts.
      [11] If the decisions are based on convention they are termed arbitrary
      or mindless[44] while those not so based may be termed subjective. To
      minimize type II errors, large samples are recommended. In psychology
      practically all null hypotheses are claimed to be false for sufficiently
      large samples so "...it is usually nonsensical to perform an experiment
      with the sole aim of rejecting the null hypothesis.".[64] "Statistically
      significant findings are often misleading" in psychology.[65] Statistical
      significance does not imply practical significance and correlation_does
      not_imply_causation. Casting doubt on the null hypothesis is thus far
      from directly supporting the research hypothesis.
    * "[I]t does not tell us what we want to know".[66] Lists of dozens of
      complaints are available.[58][67][68]
Critics and supporters are largely in factual agreement regarding the
characteristics of null hypothesis significance testing (NHST): While it can
provide critical information, it is inadequate as the sole tool for statistical
analysis. Successfully rejecting the null hypothesis may offer no support for
the research hypothesis. The continuing controversy concerns the selection of
the best statistical practices for the near-term future given the (often poor)
existing practices. Critics would prefer to ban NHST completely, forcing a
complete departure from those practices, while supporters suggest a less
absolute change.[citation_needed]
Controversy over significance testing, and its effects on publication bias in
particular, has produced several results. The American Psychological
Association has strengthened its statistical reporting requirements after
review,[69] medical journal publishers have recognized the obligation to
publish some results that are not statistically significant to combat
publication bias[70] and a journal (Journal of Articles in Support of the Null
Hypothesis) has been created to publish such results exclusively.[71] Textbooks
have added some cautions[72] and increased coverage of the tools necessary to
estimate the size of the sample required to produce significant results. Major
organizations have not abandoned use of significance tests although some have
discussed doing so.[69]
***** Alternatives[edit] *****
Main article: Estimation_statistics
See also: Confidence_interval_Â§ Statistical_hypothesis_testing
The numerous criticisms of significance testing do not lead to a single
alternative. A unifying position of critics is that statistics should not lead
to a conclusion or a decision but to a probability or to an estimated value
with an interval_estimate rather than to an accept-reject decision regarding a
particular hypothesis. It is unlikely that the controversy surrounding
significance testing will be resolved in the near future. Its supposed flaws
and unpopularity do not eliminate the need for an objective and transparent
means of reaching conclusions regarding studies that produce statistical
results. Critics have not unified around an alternative. Other forms of
reporting confidence or uncertainty could probably grow in popularity. One
strong critic of significance testing suggested a list of reporting
alternatives:[73] effect sizes for importance, prediction intervals for
confidence, replications and extensions for replicability, meta-analyses for
generality. None of these suggested alternatives produces a conclusion/
decision. Lehmann said that hypothesis testing theory can be presented in terms
of conclusions/decisions, probabilities, or confidence intervals. "The
distinction between the ... approaches is largely one of reporting and
interpretation."[74]
On one "alternative" there is no disagreement: Fisher himself said,[26] "In
relation to the test of significance, we may say that a phenomenon is
experimentally demonstrable when we know how to conduct an experiment which
will rarely fail to give us a statistically significant result." Cohen, an
influential critic of significance testing, concurred,[66] "... don't look for
a magic alternative to NHST [null hypothesis significance testing] ... It
doesn't exist." "... given the problems of statistical induction, we must
finally rely, as have the older sciences, on replication." The "alternative" to
significance testing is repeated testing. The easiest way to decrease
statistical uncertainty is by obtaining more data, whether by increased sample
size or by repeated tests. Nickerson claimed to have never seen the publication
of a literally replicated experiment in psychology.[67] An indirect approach to
replication is meta-analysis.
Bayesian_inference is one proposed alternative to significance testing.
(Nickerson cited 10 sources suggesting it, including Rozeboom (1960)).[67] For
example, Bayesian parameter_estimation can provide rich information about the
data from which researchers can draw inferences, while using uncertain priors
that exert only minimal influence on the results when enough data is available.
Psychologist John K. Kruschke has suggested Bayesian estimation as an
alternative for the t-test.[75] Alternatively two competing models/hypothesis
can be compared using Bayes_factors.[76] Bayesian methods could be criticized
for requiring information that is seldom available in the cases where
significance testing is most heavily used. Neither the prior probabilities nor
the probability distribution of the test statistic under the alternative
hypothesis are often available in the social sciences.[67]
Advocates of a Bayesian approach sometimes claim that the goal of a researcher
is most often to objectively assess the probability that a hypothesis is true
based on the data they have collected.[77][78] Neither Fisher's significance
testing, nor NeymanâPearson hypothesis testing can provide this information,
and do not claim to. The probability a hypothesis is true can only be derived
from use of Bayes'_Theorem, which was unsatisfactory to both the Fisher and
NeymanâPearson camps due to the explicit use of subjectivity in the form of
the prior_probability.[35][79] Fisher's strategy is to sidestep this with the
p-value (an objective index based on the data alone) followed by inductive
inference, while NeymanâPearson devised their approach of inductive
behaviour.
***** Philosophy[edit] *****
Hypothesis testing and philosophy intersect. Inferential_statistics, which
includes hypothesis testing, is applied probability. Both probability and its
application are intertwined with philosophy. Philosopher David_Hume wrote, "All
knowledge degenerates into probability." Competing practical definitions of
probability reflect philosophical differences. The most common application of
hypothesis testing is in the scientific interpretation of experimental data,
which is naturally studied by the philosophy_of_science.
Fisher and Neyman opposed the subjectivity of probability. Their views
contributed to the objective definitions. The core of their historical
disagreement was philosophical.
Many of the philosophical criticisms of hypothesis testing are discussed by
statisticians in other contexts, particularly correlation_does_not_imply
causation and the design_of_experiments. Hypothesis testing is of continuing
interest to philosophers.[39][80]
***** Education[edit] *****
Main article: Statistics_education
Statistics is increasingly being taught in schools with hypothesis testing
being one of the elements taught.[81][82] Many conclusions reported in the
popular press (political opinion polls to medical studies) are based on
statistics. Some writers have stated that statistical analysis of this kind
allows for thinking clearly about problems involving mass data, as well as the
effective reporting of trends and inferences from said data, but caution that
writers for a broad public should have a solid understanding of the field in
order to use the terms and concepts correctly.[83][84][citation_needed][83][84]
[citation_needed] An introductory college statistics class places much emphasis
on hypothesis testing â perhaps half of the course. Such fields as literature
and divinity now include findings based on statistical analysis (see the Bible
Analyzer). An introductory statistics class teaches hypothesis testing as a
cookbook process. Hypothesis testing is also taught at the postgraduate level.
Statisticians learn how to create good statistical test procedures (like z,
Student's t, F and chi-squared). Statistical hypothesis testing is considered a
mature area within statistics,[74] but a limited amount of development
continues.
An academic study states that the cookbook method of teaching introductory
statistics leaves no time for history, philosophy or controversy. Hypothesis
testing has been taught as received unified method. Surveys showed that
graduates of the class were filled with philosophical misconceptions (on all
aspects of statistical inference) that persisted among instructors.[85] While
the problem was addressed more than a decade ago,[86] and calls for educational
reform continue,[87] students still graduate from statistics classes holding
fundamental misconceptions about hypothesis testing.[88] Ideas for improving
the teaching of hypothesis testing include encouraging students to search for
statistical errors in published papers, teaching the history of statistics and
emphasizing the controversy in a generally dry subject.[89]
***** See also[edit] *****
    * [icon]Statistics_portal
    * Statistics
    * BehrensâFisher_problem
    * Bootstrapping_(statistics)
    * Checking_if_a_coin_is_fair
    * Comparing_means test decision tree
    * Complete_spatial_randomness
    * Counternull
    * Falsifiability
    * Fisher's_method for combining independent tests_of_significance
    * Granger_causality
    * Look-elsewhere_effect
    * Modifiable_areal_unit_problem
    * Omnibus_test
    * Dichotomous_thinking
    * Almost_sure_hypothesis_testing
***** References[edit] *****
   1. ^ Stuart A., Ord K., Arnold S. (1999), Kendall's Advanced Theory of
      Statistics: Volume 2A—Classical Inference & the Linear Model (Arnold)
      §20.2.
   2. ^Rice, John A. (2007). Mathematical Statistics and Data Analysis (3rd
      ed.). Thomson_Brooks/Cole. Â§9.3.
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
   4. ^Burnham, K. P.; Anderson, D. R. (2002). Model Selection and Multimodel
      Inference: A practical information-theoretic approach (2nd ed.).
      Springer-Verlag. ISBN 978-0-387-95364-9.
   5. ^ a bLehmann, E. L.; Romano, Joseph P. (2005). Testing Statistical
      Hypotheses (3E ed.). New York: Springer. ISBN 978-0-387-98864-1.
   6. ^Triola, Mario (2001). Elementary_statistics (8 ed.). Boston: Addison-
      Wesley. p. 388. ISBN 978-0-201-61477-0.
   7. ^Hinkelmann, Klaus and Kempthorne,_Oscar (2008). Design and Analysis of
      Experiments. I and II (Second ed.). Wiley. ISBN 978-0-470-38551-7.CS1
      maint: Multiple names: authors list (link)
   8. ^Montgomery, Douglas (2009). Design and analysis of experiments. Hoboken,
      N.J.: Wiley. ISBN 978-0-470-12866-4.
   9. ^ R. A. Fisher (1925).Statistical Methods for Research Workers,
      Edinburgh: Oliver and Boyd, 1925, p.43.
  10. ^Nuzzo, Regina (2014). "Scientific method: Statistical errors". Nature.
      506.
  11. ^Siegrist, Kyle. "Hypothesis_Testing_-_Introduction".
      www.randomservices.org. Retrieved March 8, 2018.
  12. ^ a b Bakan, David (1966). "The test of significance in psychological
      research". Psychological Bulletin. 66 (6): 423â437. doi:10.1037/
      h0020412.
  13. ^Richard J. Larsen; Donna Fox Stroup (1976). Statistics in the Real
      World: a book of examples. Macmillan. ISBN 978-0023677205.
  14. ^Hubbard, R.; Parsa, A. R.; Luthy, M. R. (1997). "The Spread of
      Statistical Significance Testing in Psychology: The Case of the Journal
      of Applied Psychology". Theory and Psychology. 7 (4): 545â554. doi:
      10.1177/0959354397074006.
  15. ^Moore, David (2003). Introduction to the Practice of Statistics. New
      York: W.H. Freeman and Co. p. 426. ISBN 9780716796572.
  16. ^Huff, Darrell (1993). How_to_lie_with_statistics. New York: Norton.
      ISBN 978-0-393-31072-6.
  17. ^Huff, Darrell (1991). How to Lie with Statistics. London: Penguin Books.
      ISBN 978-0-14-013629-6.
  18. ^ "Over the last fifty years, How to Lie with Statistics has sold more
      copies than any other statistical text." J. M. Steele. ""Darrell_Huff_and
      Fifty_Years_of_How_to_Lie_with_Statistics". Statistical Science, 20 (3),
      2005, 205â209.
  19. ^John Arbuthnot (1710). "An_argument_for_Divine_Providence,_taken_from
      the_constant_regularity_observed_in_the_births_of_both_sexes" (PDF).
      Philosophical_Transactions_of_the_Royal_Society_of_London. 27
      (325â336): 186â190. doi:10.1098/rstl.1710.0011.
  20. ^Brian, Ãric; Jaisson, Marie (2007). "Physico-Theology and Mathematics
      (1710â1794)". The Descent of Human Sex Ratio at Birth. Springer Science
      & Business Media. pp. 1â25. ISBN 978-1-4020-6036-6.
  21. ^Conover, W.J. (1999), "Chapter 3.4: The Sign Test", Practical
      Nonparametric Statistics (Third ed.), Wiley, pp. 157â176, ISBN 978-0-
      471-16068-7
  22. ^Sprent, P. (1989), Applied Nonparametric Statistical Methods (Second
      ed.), Chapman & Hall, ISBN 978-0-412-44980-2
  23. ^Stigler, Stephen M. (1986). The History of Statistics: The Measurement
      of Uncertainty Before 1900. Harvard University Press. pp. 225â226.
      ISBN 978-0-67440341-3.
  24. ^ a bLaplace, P. (1778). "MÃ©moire_sur_les_probabilitÃ©s" (PDF).
      MÃ©moires de l'AcadÃ©mie Royale des Sciences de Paris. 9: 227â332.
  25. ^Laplace, P. (1778). "MÃ©moire_sur_les_probabilitÃ©s_(XIX,_XX)". Oeuvres
      complÃ¨tes de Laplace. MÃ©moires de l'AcadÃ©mie Royale des Sciences de
      Paris. 9. pp. 429â438.
  26. ^Stigler, Stephen M. (1986). The_History_of_Statistics:_The_Measurement
      of_Uncertainty_before_1900. Cambridge, Mass: Belknap Press of Harvard
      University Press. p. 134. ISBN 978-0-674-40340-6.
  27. ^ a bFisher,_Sir_Ronald_A. (1956) [1935]. "Mathematics_of_a_Lady_Tasting
      Tea". In James Roy Newman (ed.). The World of Mathematics, volume 3
      [Design of Experiments]. Courier Dover Publications. ISBN 978-0-486-
      41151-4.
  28.  Originally from Fisher's book Design of Experiments.
  29. ^Box, Joan Fisher (1978). R.A. Fisher, The Life of a Scientist. New York:
      Wiley. p. 134. ISBN 978-0-471-09300-8.
  30. ^C. S. Peirce (August 1878). "Illustrations_of_the_Logic_of_Science_VI:
      Deduction,_Induction,_and_Hypothesis". Popular Science Monthly. 13.
      Retrieved March 30, 2012.
  31. ^Jaynes, E. T. (2007). Probability theory : the logic of science (5.
      print. ed.). Cambridge [u.a.]: Cambridge Univ. Press. ISBN 978-0-521-
      59271-0.
  32. ^ Schervish, M (1996) Theory of Statistics, p. 218. Springer
  33. ISBN 0-387-94546-6
  34. ^Kaye, David H.; Freedman, David A. (2011). "Reference_Guide_on
      Statistics". Reference Manual on Scientific Evidence (3rd ed.). Eagan, MN
      Washington, D.C: West National Academies Press. p. 259. ISBN 978-0-309-
      21421-6.
  35. ^Bellhouse, P. (2001), "John Arbuthnot", in Statisticians of the
      Centuries by C.C. Heyde and E. Seneta, Springer, pp. 39â42, ISBN 978-0-
      387-95329-8
  36. ^ a b Raymond Hubbard, M._J._Bayarri, P_Values_are_not_Error
      Probabilities Archived September 4, 2013, at the Wayback_Machine. A
      working paper that explains the difference between Fisher's evidential p-
      value and the NeymanâPearson Type I error rate     &#x03B1;
      {\displaystyle \alpha }  [\alpha ].
  37. ^ a bFisher, R (1955). "Statistical_Methods_and_Scientific_Induction"
      (PDF). Journal of the Royal Statistical Society, Series B. 17 (1):
      69â78.
  38. ^ a b c dNeyman, J; Pearson, E. S. (January 1, 1933). "On the Problem of
      the most Efficient Tests of Statistical Hypotheses". Philosophical
      Transactions_of_the_Royal_Society_A. 231 (694â706): 289â337. doi:
      10.1098/rsta.1933.0009.
  39. ^Goodman, S N (June 15, 1999). "Toward evidence-based medical statistics.
      1: The P Value Fallacy". Ann Intern Med. 130 (12): 995â1004. doi:
      10.7326/0003-4819-130-12-199906150-00008. PMID 10383371.
  40. ^ a b c dLehmann, E. L. (December 1993). "The Fisher, NeymanâPearson
      Theories of Testing Hypotheses: One Theory or Two?". Journal of the
      American Statistical Association. 88 (424): 1242â1249. doi:10.1080/
      01621459.1993.10476404.
  41. ^Fisher, R N (1958). "The_Nature_of_Probability" (PDF). Centennial
      Review. 2: 261â274.
  42. "We are quite in danger of sending highly trained and highly intelligent
      young men out into the world with tables of erroneous numbers under their
      arms, and with a dense fog in the place where their brains ought to be.
      In this century, of course, they will be working on guided missiles and
      advising the medical profession on the control of disease, and there is
      no limit to the extent to which they could impede every sort of national
      effort."
  43. ^ a b cLenhard, Johannes (2006). "Models and Statistical Inference: The
      Controversy between Fisher and NeymanâPearson". Br. J. Philos. Sci. 57:
      69â91. doi:10.1093/bjps/axi152.
  44. ^Neyman, Jerzy (1967). "RA Fisher (1890â1962): An Appreciation".
      Science. 156.3781 (3781): 1456â1460. doi:10.1126/science.156.3781.1456.
      PMID 17741062.
  45. ^Losavich, J. L.; Neyman, J.; Scott, E. L.; Wells, M. A. (1971).
      "Hypothetical_explanations_of_the_negative_apparent_effects_of_cloud
      seeding_in_the_Whitetop_Experiment". Proceedings of the National Academy
      of Sciences of the United States of America. 68 (11): 2643â2646. doi:
      10.1073/pnas.68.11.2643. PMC 389491. PMID 16591951.
  46. ^ a b cHalpin, P F; Stam, HJ (Winter 2006). "Inductive Inference or
      Inductive Behavior: Fisher and Neyman: Pearson Approaches to Statistical
      Testing in Psychological Research (1940â1960)". The American Journal of
      Psychology. 119 (4): 625â653. doi:10.2307/20445367. JSTOR 20445367.
      PMID 17286092.
  47. ^Gigerenzer, Gerd; Zeno Swijtink; Theodore Porter; Lorraine Daston; John
      Beatty; Lorenz Kruger (1989). "Part 3: The Inference Experts". The Empire
      of Chance: How Probability Changed Science and Everyday Life. Cambridge
      University Press. pp. 70â122. ISBN 978-0-521-39838-1.
  48. ^ a bGigerenzer, G (November 2004). "Mindless statistics". The Journal of
      Socio-Economics. 33 (5): 587â606. doi:10.1016/j.socec.2004.09.033.
  49. ^Loftus, G R (1991). "On_the_Tyranny_of_Hypothesis_Testing_in_the_Social
      Sciences" (PDF). Contemporary Psychology. 36 (2): 102â105. doi:10.1037/
      029395.
  50. ^Meehl, P (1990). "Appraising_and_Amending_Theories:_The_Strategy_of
      Lakatosian_Defense_and_Two_Principles_That_Warrant_It" (PDF).
      Psychological Inquiry. 1 (2): 108â141. doi:10.1207/s15327965pli0102_1.
  51. ^Pearson, K (1900). "On_the_criterion_that_a_given_system_of_deviations
      from_the_probable_in_the_case_of_a_correlated_system_of_variables_is_such
      that_it_can_be_reasonably_supposed_to_have_arisen_from_random_sampling"
      (PDF). Philosophical Magazine Series. 5 (50): 157â175. doi:10.1080/
      14786440009463897.
  52. ^Pearson, K (1904). "On_the_Theory_of_Contingency_and_Its_Relation_to
      Association_and_Normal_Correlation". Drapers' Company Research Memoirs
      Biometric Series. 1: 1â35.
  53. ^Zabell, S (1989). "R. A. Fisher on the History of Inverse Probability".
      Statistical Science. 4 (3): 247â256. doi:10.1214/ss/1177012488.
      JSTOR 2245634.
  54. ^Ash, Robert (1970). Basic probability theory. New York: Wiley. ISBN 978-
      0471034506.
  55. Section 8.2
  56. ^ a bTukey, John W. (1960). "Conclusions vs decisions". Technometrics. 26
      (4): 423â433. doi:10.1080/00401706.1960.10489909.
  57.  "Until we go through the accounts of testing hypotheses, separating
      [NeymanâPearson] decision elements from [Fisher] conclusion elements,
      the intimate mixture of disparate elements will be a continual source of
      confusion." ... "There is a place for both "doing one's best" and "saying
      only what is certain," but it is important to know, in each instance,
      both which one is being done, and which one ought to be done."
  58. ^Stigler, Stephen M. (August 1996). "The History of Statistics in 1933".
      Statistical Science. 11 (3): 244â252. doi:10.1214/ss/1032280216.
      JSTOR 2246117.
  59. ^Berger, James O. (2003). "Could Fisher, Jeffreys and Neyman Have Agreed
      on Testing?". Statistical Science. 18 (1): 1â32. doi:10.1214/ss/
      1056397485.
  60. ^Morrison, Denton; Henkel, Ramon, eds. (2006) [1970]. The Significance
      Test Controversy. AldineTransaction. ISBN 978-0-202-30879-1.
  61. ^Oakes, Michael (1986). Statistical Inference: A Commentary for the
      Social and Behavioural Sciences. Chichester New York: Wiley. ISBN 978-
      0471104438.
  62. ^Chow, Siu L. (1997). Statistical Significance: Rationale, Validity and
      Utility. ISBN 978-0-7619-5205-3.
  63. ^Harlow, Lisa Lavoie; Stanley A. Mulaik; James H. Steiger, eds. (1997).
      What If There Were No Significance Tests?. Lawrence Erlbaum Associates.
      ISBN 978-0-8058-2634-0.
  64. ^ a bKline, Rex (2004). Beyond Significance Testing: Reforming Data
      Analysis Methods in Behavioral Research. Washington, D.C.: American
      Psychological Association. ISBN 9781591471189.
  65. ^McCloskey, Deirdre N.; Stephen T. Ziliak (2008). The Cult of Statistical
      Significance: How the Standard Error Costs Us Jobs, Justice, and Lives.
      University of Michigan Press. ISBN 978-0-472-05007-9.
  66. ^Cornfield, Jerome (1976). "Recent_Methodological_Contributions_to
      Clinical_Trials" (PDF). American Journal of Epidemiology. 104 (4):
      408â421. doi:10.1093/oxfordjournals.aje.a112313.
  67. ^Yates, Frank (1951). "The Influence of Statistical Methods for Research
      Workers on the Development of the Science of Statistics". Journal of the
      American Statistical Association. 46 (253): 19â34. doi:10.1080/
      01621459.1951.10500764.
  68.  "The emphasis given to formal tests of significance throughout [R.A.
      Fisher's] Statistical Methods ... has caused scientific research workers
      to pay undue attention to the results of the tests of significance they
      perform on their data, particularly data derived from experiments, and
      too little to the estimates of the magnitude of the effects they are
      investigating." ... "The emphasis on tests of significance and the
      consideration of the results of each experiment in isolation, have had
      the unfortunate consequence that scientific workers have often regarded
      the execution of a test of significance on an experiment as the ultimate
      objective."
  69. ^Begg, Colin B.; Berlin, Jesse A. (1988). "Publication bias: a problem in
      interpreting medical data". Journal of the Royal Statistical Society,
      Series A. 151 (3): 419â463. doi:10.2307/2982993. JSTOR 2982993.
  70. ^Meehl, Paul E. (1967). "Theory-Testing_in_Psychology_and_Physics:_A
      Methodological_Paradox" (PDF). Philosophy of Science. 34 (2): 103â115.
      doi:10.1086/288135. Archived from the_original (PDF) on December 3, 2013.
  71.  Thirty years later, Meehl acknowledged statistical significance theory
      to be mathematically sound while continuing to question the default
      choice of null hypothesis, blaming instead the "social scientists' poor
      understanding of the logical relation between theory and fact" in "The
      Problem Is Epistemology, Not Statistics: Replace Significance Tests by
      Confidence Intervals and Quantify Accuracy of Risky Numerical
      Predictions" (Chapter 14 in Harlow (1997)).
  72. ^Nunnally, Jum (1960). "The place of statistics in psychology".
      Educational and Psychological Measurement. 20 (4): 641â650. doi:
      10.1177/001316446002000401.
  73. ^Lykken, David T. (1991). "What's wrong with psychology, anyway?".
      Thinking Clearly About Psychology. 1: 3â39.
  74. ^ a bJacob Cohen (December 1994). "The Earth Is Round (p < .05)".
      American Psychologist. 49 (12): 997â1003. doi:10.1037/0003-
      066X.49.12.997.
  75.  This paper lead to the review of statistical practices by the APA. Cohen
      was a member of the Task Force that did the review.
  76. ^ a b c dNickerson, Raymond S. (2000). "Null Hypothesis Significance
      Tests: A Review of an Old and Continuing Controversy". Psychological
      Methods. 5 (2): 241â301. doi:10.1037/1082-989X.5.2.241. PMID 10937333.
  77. ^Branch, Mark (2014). "Malignant side effects of null hypothesis
      significance testing". Theory & Psychology. 24 (2): 256â277. doi:
      10.1177/0959354314525282.
  78. ^ a bWilkinson, Leland (1999). "Statistical Methods in Psychology
      Journals; Guidelines and Explanations". American Psychologist. 54 (8):
      594â604. doi:10.1037/0003-066X.54.8.594.
  79.  "Hypothesis tests. It is hard to imagine a situation in which a
      dichotomous accept-reject decision is better than reporting an actual p
      value or, better still, a confidence interval." (p 599). The committee
      used the cautionary term "forbearance" in describing its decision against
      a ban of hypothesis testing in psychology reporting. (p 603)
  80. ^"ICMJE:_Obligation_to_Publish_Negative_Studies". Archived from the
      original on July 16, 2012. Retrieved September 3, 2012. Editors should
      seriously consider for publication any carefully done study of an
      important question, relevant to their readers, whether the results for
      the primary or any additional outcome are statistically significant.
      Failure to submit or publish findings because of lack of statistical
      significance is an important cause of publication bias.
  81. ^ Journal of Articles in Support of the Null Hypothesis website: JASNH
      homepage. Volume 1 number 1 was published in 2002, and all articles are
      on psychology-related subjects.
  82. ^Howell, David (2002). Statistical Methods for Psychology (5 ed.).
      Duxbury. p. 94. ISBN 978-0-534-37770-0.
  83. ^Armstrong, J. Scott (2007). "Significance_tests_harm_progress_in
      forecasting". International Journal of Forecasting. 23 (2): 321â327.
      CiteSeerX 10.1.1.343.9516. doi:10.1016/j.ijforecast.2007.03.004.
  84. ^ a bE. L. Lehmann (1997). "Testing Statistical Hypotheses: The Story of
      a Book". Statistical Science. 12 (1): 48â52. doi:10.1214/ss/1029963261.
  85. ^Kruschke, J K (July 9, 2012). "Bayesian_Estimation_Supersedes_the_T
      Test" (PDF). Journal of Experimental Psychology: General. 142 (2):
      573â603. doi:10.1037/a0029146.
  86. ^Kass, R. E. (1993). "Bayes_factors_and_model_uncertainty" (PDF).
      Department of Statistics, University of Washington.
  87. ^Rozeboom, William W (1960). "The_fallacy_of_the_null-hypothesis
      significance_test" (PDF). Psychological Bulletin. 57 (5): 416â428.
      CiteSeerX 10.1.1.398.9002. doi:10.1037/h0042040.
  88.  "...the proper application of statistics to scientific inference is
      irrevocably committed to extensive consideration of inverse [AKA
      Bayesian] probabilities..." It was acknowledged, with regret, that a
      priori probability distributions were available "only as a subjective
      feel, differing from one person to the next" "in the more immediate
      future, at least".
  89. ^Berger, James (2006). "The Case for Objective Bayesian Analysis".
      Bayesian Analysis. 1 (3): 385â402. doi:10.1214/06-ba115.
  90.  In listing the competing definitions of "objective" Bayesian analysis,
      "A major goal of statistics (indeed science) is to find a completely
      coherent objective Bayesian methodology for learning from data." The
      author expressed the view that this goal "is not attainable".
  91. ^Aldrich, J (2008). "R._A._Fisher_on_Bayes_and_Bayes'_theorem" (PDF).
      Bayesian Analysis. 3 (1): 161â170. doi:10.1214/08-BA306. Archived from
      the_original (PDF) on September 6, 2014.
  92. ^ Mayo, D. G.; Spanos, A. (2006). "Severe Testing as a Basic Concept in a
      NeymanâPearson Philosophy of Induction". The British Journal for the
      Philosophy of Science. 57 (2): 323â357. CiteSeerX 10.1.1.130.8131. doi:
      10.1093/bjps/axl003.
  93. ^ Mathematics_>_High_School:_Statistics_&_Probability_>_Introduction
      Archived July 28, 2012, at Archive.today Common Core State Standards
      Initiative (relates to USA students)
  94. ^ College_Board_Tests_>_AP:_Subjects_>_Statistics The College Board
      (relates to USA students)
  95. ^ a bHuff, Darrell (1993). How_to_lie_with_statistics. New York: Norton.
      p. 8. ISBN 978-0-393-31072-6.
  96. 'Statistical methods and statistical terms are necessary in reporting the
      mass data of social and economic trends, business conditions, "opinion"
      polls, the census. But without writers who use the words with honesty and
      readers who know what they mean, the result can only be semantic
      nonsense.'
  97. ^ a bSnedecor, George W.; Cochran, William G. (1967). Statistical Methods
      (6 ed.). Ames, Iowa: Iowa State University Press. p. 3.
  98.  "...the basic ideas in statistics assist us in thinking clearly about
      the problem, provide some guidance about the conditions that must be
      satisfied if sound inferences are to be made, and enable us to detect
      many inferences that have no good logical foundation."
  99. ^Sotos, Ana Elisa Castro; Vanhoof, Stijn; Noortgate, Wim Van den;
      Onghena, Patrick (2007). "Students'_Misconceptions_of_Statistical
      Inference:_A_Review_of_the_Empirical_Evidence_from_Research_on_Statistics
      Education" (PDF). Educational Research Review. 2 (2): 98â113. doi:
      10.1016/j.edurev.2007.04.001.
 100. ^Moore, David S. (1997). "New_Pedagogy_and_New_Content:_The_Case_of
      Statistics" (PDF). International Statistical Review. 65 (2): 123â165.
      doi:10.2307/1403333. JSTOR 1403333.
 101. ^Hubbard, Raymond; Armstrong,_J._Scott (2006). "Why_We_Don't_Really_Know
      What_Statistical_Significance_Means:_Implications_for_Educators" (PDF).
      Journal of Marketing Education. 28 (2): 114â120. doi:10.1177/
      0273475306288399. Archived from the original on May 18, 2006.CS1 maint:
      Unfit url (link)
 102.  Preprint
 103. ^Sotos, Ana Elisa Castro; Vanhoof, Stijn; Noortgate, Wim Van den;
      Onghena, Patrick (2009). "How Confident Are Students in Their
      Misconceptions about Hypothesis Tests?". Journal of Statistics Education.
      17 (2). doi:10.1080/10691898.2009.11889514.
 104. ^Gigerenzer, G. (2004). "The_Null_Ritual_What_You_Always_Wanted_to_Know
      About_Significant_Testing_but_Were_Afraid_to_Ask" (PDF). The SAGE
      Handbook of Quantitative Methodology for the Social Sciences.
      pp. 391â408. doi:10.4135/9781412986311. ISBN 9780761923596.
***** Further reading[edit] *****
    * Lehmann E.L. (1992) "Introduction to Neyman and Pearson (1933) On the
      Problem of the Most Efficient Tests of Statistical Hypotheses". In:
      Breakthroughs in Statistics, Volume 1, (Eds Kotz, S., Johnson, N.L.),
      Springer-Verlag.
ISBN 0-387-94037-5 (followed by reprinting of the paper)
Neyman, J.; Pearson, E.S. (1933). "On the Problem of the Most Efficient Tests
of Statistical Hypotheses". Philosophical_Transactions_of_the_Royal_Society_A.
231 (694â706): 289â337. doi:10.1098/rsta.1933.0009.
***** External links[edit] *****
 Wikimedia Commons has media related to Hypothesis_testing.
 Wikiversity has learning resources about Statistical_hypothesis_testing at
 Introduction_to_Statistical_Analysis/Unit_5_Content
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Statistical_hypotheses,
      verification_of", Encyclopedia_of_Mathematics, Springer Science+Business
      Media B.V. / Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Wilson GonzÃ¡lez, Georgina; Kay Sankaran (September 10, 1997). "Hypothesis
Testing". Environmental Sampling & Monitoring Primer. Virginia Tech.
Bayesian_critique_of_classical_hypothesis_testing
Critique_of_classical_hypothesis_testing_highlighting_long-standing_qualms_of
statisticians
Dallal GE (2007) The_Little_Handbook_of_Statistical_Practice (A good tutorial)
References_for_arguments_for_and_against_hypothesis_testing
Statistical_Tests_Overview: How to choose the correct statistical test
**** Online calculators[edit] ****
    * MBAStats_confidence_interval_and_hypothesis_test_calculators
    * Some p-value_and_hypothesis_test_calculators.
    * v
    * t
    * e
Statistics
    * Outline
    * Index
Descriptive_statistics
                               * Mean
                                     o arithmetic
                Center               o geometric
                                     o harmonic
                               * Median
                               * Mode
                               * Variance
                               * Standard_deviation
Continuous_data Dispersion     * Coefficient_of_variation
                               * Percentile
                               * Range
                               * Interquartile_range
                               * Central_limit_theorem
                               * Moments
                Shape                o Skewness
                                     o Kurtosis
                                     o L-moments
Count_data          * Index_of_dispersion
                    * Grouped_data
Summary tables      * Frequency_distribution
                    * Contingency_table
                    * Pearson_product-moment_correlation
                    * Rank_correlation
Dependence                o Spearman's_rho
                          o Kendall's_tau
                    * Partial_correlation
                    * Scatter_plot
                    * Bar_chart
                    * Biplot
                    * Box_plot
                    * Control_chart
                    * Correlogram
                    * Fan_chart
Graphics            * Forest_plot
                    * Histogram
                    * Pie_chart
                    * QâQ_plot
                    * Run_chart
                    * Scatter_plot
                    * Stem-and-leaf_display
                    * Radar_chart
Data_collection
                           * Population
                           * Statistic
                           * Effect_size
Study_design               * Statistical_power
                           * Optimal_design
                           * Sample_size_determination
                           * Replication
                           * Missing_data
                           * Sampling
                                 o stratified
Survey_methodology               o cluster
                           * Standard_error
                           * Opinion_poll
                           * Questionnaire
                           * Scientific_control
                           * Randomized_experiment
                           * Randomized_controlled_trial
Controlled_experiments     * Random_assignment
                           * Blocking
                           * Interaction
                           * Factorial_experiment
                           * Adaptive_clinical_trial
Adaptive Designs           * Up-and-Down_Designs
                           * Stochastic_approximation
                           * Cross-sectional_study
Observational_Studies      * Cohort_study
                           * Natural_experiment
                           * Quasi-experiment
Statistical_inference
                * Population
                * Statistic
                * Probability_distribution
                * Sampling_distribution
                      o Order_statistic
                * Empirical_distribution
                      o Density_estimation
                * Statistical_model
                      o Model_specification
                      o Lp_space
                * Parameter
                      o location
                      o scale
                      o shape
Statistical     * Parametric_family
theory                o Likelihood (monotone)
                      o Locationâscale_family
                      o Exponential_family
                * Completeness
                * Sufficiency
                * Statistical_functional
                      o Bootstrap
                      o U
                      o V
                * Optimal_decision
                      o loss_function
                * Efficiency
                * Statistical_distance
                      o divergence
                * Asymptotics
                * Robustness
                                    * Estimating_equations
                                          o Maximum_likelihood
                                          o Method_of_moments
                                          o M-estimator
                                          o Minimum_distance
            Point_estimation        * Unbiased_estimators
                                          o Mean-unbiased_minimum-variance
                                                # RaoâBlackwellization
                                                # LehmannâScheffÃ©_theorem
                                          o Median_unbiased
                                    * Plug-in
                                    * Confidence_interval
                                    * Pivot
Frequentist                         * Likelihood_interval
inference   Interval_estimation     * Prediction_interval
                                    * Tolerance_interval
                                    * Resampling
                                          o Bootstrap
                                          o Jackknife
                                    * 1-_&_2-tails
                                    * Power
            Testing hypotheses            o Uniformly_most_powerful_test
                                    * Permutation_test
                                          o Randomization_test
                                    * Multiple_comparisons
                                    * Likelihood-ratio
            Parametric_tests        * Score/Lagrange_multiplier
                                    * Wald
                * Z-test_(normal)
                * Student's_t-test
                * F-test
                           * Chi-squared
                           * G-test
                           * KolmogorovâSmirnov
                           * AndersonâDarling
                           * Lilliefors
            Goodness       * JarqueâBera
            of_fit         * Normality_(ShapiroâWilk)
                           * Likelihood-ratio_test
Specific                   * Model_selection
tests                            o Cross_validation
                                 o AIC
                                 o BIC
                           * Sign
                                 o Sample_median
                           * Signed_rank_(Wilcoxon)
            Rank                 o HodgesâLehmann_estimator
            statistics     * Rank_sum_(MannâWhitney)
                           * Nonparametric anova
                                 o 1-way_(KruskalâWallis)
                                 o 2-way_(Friedman)
                                 o Ordered_alternative_(JonckheereâTerpstra)
                * Bayesian_probability
                      o prior
Bayesian              o posterior
inference       * Credible_interval
                * Bayes_factor
                * Bayesian_estimator
                      o Maximum_posterior_estimator
    * Correlation
    * Regression_analysis
                       * Pearson_product-moment
Correlation            * Partial_correlation
                       * Confounding_variable
                       * Coefficient_of_determination
                       * Errors_and_residuals
Regression             * Regression_validation
analysis               * Mixed_effects_models
                       * Simultaneous_equations_models
                       * Multivariate_adaptive_regression_splines_(MARS)
                       * Simple_linear_regression
Linear_regression      * Ordinary_least_squares
                       * General_linear_model
                       * Bayesian_regression
                       * Nonlinear_regression
                       * Nonparametric
Non-standard           * Semiparametric
predictors             * Isotonic
                       * Robust
                       * Heteroscedasticity
                       * Homoscedasticity
Generalized_linear     * Exponential_families
model                  * Logistic_(Bernoulli) / Binomial / Poisson_regressions
                       * Analysis_of_variance_(ANOVA,_anova)
Partition_of           * Analysis_of_covariance
variance               * Multivariate_ANOVA
                       * Degrees_of_freedom
Categorical / Multivariate / Time-series / Survival_analysis
                 * Cohen's_kappa
                 * Contingency_table
Categorical      * Graphical_model
                 * Log-linear_model
                 * McNemar's_test
                 * Regression
                 * Manova
                 * Principal_components
                 * Canonical_correlation
                 * Discriminant_analysis
Multivariate     * Cluster_analysis
                 * Classification
                 * Structural_equation_model
                       o Factor_analysis
                 * Multivariate_distributions
                       o Elliptical_distributions
                             # Normal
                                  * Decomposition
                                  * Trend
                                  * Stationarity
             General              * Seasonal_adjustment
                                  * Exponential_smoothing
                                  * Cointegration
                                  * Structural_break
                                  * Granger_causality
                                  * DickeyâFuller
                                  * Johansen
             Specific tests       * Q-statistic_(LjungâBox)
                                  * DurbinâWatson
Time-series                       * BreuschâGodfrey
                                  * Autocorrelation_(ACF)
                                        o partial_(PACF)
                                  * Cross-correlation_(XCF)
             Time_domain          * ARMA_model
                                  * ARIMA_model_(BoxâJenkins)
                                  * Autoregressive_conditional
                                    heteroskedasticity_(ARCH)
                                  * Vector_autoregression_(VAR)
                                  * Spectral_density_estimation
             Frequency_domain     * Fourier_analysis
                                  * Wavelet
                                  * Whittle_likelihood
                                   * KaplanâMeier_estimator_(product_limit)
             Survival_function     * Proportional_hazards_models
Survival                           * Accelerated_failure_time_(AFT)_model
                                   * First_hitting_time
             Hazard_function       * NelsonâAalen_estimator
             Test                  * Log-rank_test
Applications
                           * Bioinformatics
Biostatistics              * Clinical_trials / studies
                           * Epidemiology
                           * Medical_statistics
                           * Chemometrics
                           * Methods_engineering
Engineering_statistics     * Probabilistic_design
                           * Process / quality_control
                           * Reliability
                           * System_identification
                           * Actuarial_science
                           * Census
                           * Crime_statistics
                           * Demography
Social_statistics          * Econometrics
                           * National_accounts
                           * Official_statistics
                           * Population_statistics
                           * Psychometrics
                           * Cartography
                           * Environmental_statistics
Spatial_statistics         * Geographic_information_system
                           * Geostatistics
                           * Kriging
    * [Category]Category
    * [Portal]Portal
    * [Commons page]Commons
    * [WikiProject] WikiProject
    * v
    * t
    * e
Public_health
                               * Auxology
                               * Biological_hazard
                               * Chief_Medical_Officer
                               * Cultural_competence
                               * Deviance
                               * Environmental_health
                               * Euthenics
                               * Genomics
                               * Globalization_and_disease
                               * Health_economics
                               * Health_literacy
                               * Health_policy
General                              o Health_system
                                     o Health_care_reform
                                     o Public_health_law
                               * Maternal_health
                               * Medical_anthropology
                               * Medical_sociology
                               * Mental_health
                               * Pharmaceutical_policy
                               * Public_health_intervention
                               * Public_health_laboratory
                               * Reproductive_health
                               * Social_psychology
                               * Sociology_of_health_and_illness
                               * Behavior_change
                                     o Theories
                               * Family_planning
                               * Health_promotion
                               * Human_nutrition
                               * Preventive_nutrition
                               * Hygiene
                                     o Food_safety
                                     o Hand_washing
                                     o Infection_control
                                     o Oral_hygiene
                               * Occupational_safety_and_health
                                     o Human_factors_and_ergonomics
                                     o Hygiene
Preventive_healthcare                o Injury_prevention
                                     o Medicine
                                     o Nursing
                               * Patient_safety
                                     o Organization
                               * Pharmacovigilance
                               * Safe_sex
                               * Sanitation
                                     o Emergency
                                     o Fecalâoral_transmission
                                     o Open_defecation
                                     o Sanitary_sewer
                                     o Waterborne_diseases
                               * Smoking_cessation
                               * Vaccination
                               * Vector_control
                               * Biostatistics
                               * Child_mortality
                               * Community_health
                               * Epidemiology
                               * Global_health
                               * Health_impact_assessment
Population_health              * Health_system
                               * Infant_mortality
                               * Open-source_healthcare_software
                               * Public_health_informatics
                               * Social_determinants_of_health
                                     o Health_equity
                                     o Race_and_health
                               * Social_medicine
                               * Caseâcontrol_study
                               * Randomized_controlled_trial
                               * Relative_risk
                               * Statistical hypothesis testing
Biological and                       o Analysis_of_variance_(ANOVA)
epidemiological statistics           o Regression_analysis
                                     o ROC_curve
                                     o Student's_t-test
                                     o Z-test
                               * Statistical_software
                               * Asymptomatic_carrier
                               * Epidemics
                                     o List
                               * Notifiable_diseases
Infectious and epidemic              o List
disease prevention             * Public_health_surveillance
                                     o Disease_surveillance
                               * Quarantine
                               * Sexually_transmitted_infection
                               * Tropical_disease
                               * Vaccine_trial
                               * Food
                                     o Additive
                                     o Chemistry
                                     o Engineering
                                     o Microbiology
Food hygiene and                     o Processing
safety management                    o Safety
                                     o Safety_scandals
                               * Genetically_modified_food
                               * Good_agricultural_practice
                               * Good_manufacturing_practice
                                     o HACCP
                                     o ISO_22000
                               * Diffusion_of_innovations
                               * Health_belief_model
                               * Health_communication
                               * Health_psychology
Health behavioral              * Positive_deviance
sciences                       * PRECEDE-PROCEED_model
                               * Social_cognitive_theory
                               * Social_norms_approach
                               * Theory_of_planned_behavior
                               * Transtheoretical_model
                                             * Europe
                                                   o Centre_for_Disease
                                                     Prevention_and_Control
                                                   o Committee_on_the
                                                     Environment,_Public_Health
                                                     and_Food_Safety
                                             * India
                                                   o Ministry_of_Health_and
                                                     Family_Welfare
                           Organizations     * U.S.
                                                   o Centers_for_Disease
                                                     Control_and_Prevention
                                                   o City_and_county_health
                                                     departments
                                                   o Council_on_Education_for
                                                     Public_Health
Organizations,                                     o Public_Health_Service
education                                    * World_Health_Organization
and history                                  * World_Toilet_Organization
                                             * Health_education
                                             * Higher education
                                                   o Bachelor_of_Science_in
                           Education                 Public_Health
                                                   o Doctor_of_Public_Health
                                                   o Professional_degrees_of
                                                     public_health
                                                   o Schools_of_public_health
                                             * Sara_Josephine_Baker
                                             * Samuel_Jay_Crumbine
                                             * Carl_Rogers_Darnall
                                             * Joseph_Lister
                           History           * Margaret_Sanger
                                             * John_Snow
                                             * Typhoid_Mary
                                             * Germ_theory_of_disease
                                             * Social_hygiene_movement
    * [Category] Category
    * [Commons page] Commons
    * [WikiProject] WikiProject

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Statistical_hypothesis_testing&oldid=909688699"
Categories:
    * Design_of_experiments
    * Statistical_hypothesis_testing
    * Psychometrics
    * Logic_and_statistics
    * Mathematical_and_quantitative_methods_(economics)
Hidden categories:
    * CS1_maint:_Multiple_names:_authors_list
    * CS1:_long_volume_value
    * Webarchive_template_wayback_links
    * Webarchive_template_archiveis_links
    * CS1_maint:_Unfit_url
    * Use_mdy_dates_from_November_2016
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_December_2015
    * Articles_with_unsourced_statements_from_April_2012
    * Commons_category_link_is_on_Wikidata
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Jawa
    * àº¥àº²àº§
    * LietuviÅ³
    * à´®à´²à´¯à´¾à´³à´
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 00:01 (UTC).
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
