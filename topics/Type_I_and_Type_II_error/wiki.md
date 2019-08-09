The following text has been accessed from https://en.wikipedia.org/wiki/Type_I_and_type_II_errors at Fri Aug 9 04:01:09 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Type I and type II errors ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Concepts from statistical hypothesis testing
This article is about erroneous outcomes of statistical tests. For closely
related concepts in binary classification and testing generally, see false
positives_and_false_negatives.
 This article may be too technical for most readers to understand. Please help
 improve_it to make_it_understandable_to_non-experts, without removing the
 technical details. (April 2019)(Learn_how_and_when_to_remove_this_template
 message)
In statistical_hypothesis_testing a type I error is the rejection of a true
null hypothesis (also known as a "false positive" finding or conclusion), while
a type II error is the non-rejection of a false null hypothesis (also known as
a "false negative" finding or conclusion).[1] Much of statistical theory
revolves around the minimization of one or both of these errors, though the
complete elimination of either is treated as a statistical impossibility.
[citation_needed]
⁰
***** Contents *****
    * 1_Definition
    * 2_Statistical_test_theory
          o 2.1_Type_I_error
          o 2.2_Type_II_error
          o 2.3_Table_of_error_types
    * 3_Examples
          o 3.1_Example_1
          o 3.2_Example_2
          o 3.3_Example_3
          o 3.4_Example_4
    * 4_Etymology
    * 5_Related_terms
          o 5.1_Null_hypothesis
          o 5.2_Statistical_significance
    * 6_Application_domains
          o 6.1_Inventory_control
          o 6.2_Computers
                # 6.2.1_Computer_security
                # 6.2.2_Spam_filtering
                # 6.2.3_Malware
                # 6.2.4_Optical_character_recognition
          o 6.3_Security_screening
          o 6.4_Biometrics
          o 6.5_Medicine
                # 6.5.1_Medical_screening
                # 6.5.2_Medical_testing
    * 7_See_also
    * 8_Footnotes
    * 9_References
    * 10_External_links
***** Definition[edit] *****
In statistics, a null_hypothesis is a statement that one seeks to nullify (that
is, to conclude is incorrect) with evidence to the contrary. Most commonly, it
is presented as a statement that the phenomenon being studied produces no
effect or makes no difference. An example of such a null hypothesis might be
the statement, "A diet low in carbohydrates has no effect on people's weight."
An experimenter usually frames a null hypothesis with the intent of rejecting
it: that is, intending to run an experiment which produces data that shows that
the phenomenon under study does indeed make a difference (in this case, that a
diet low in carbohydrates over some specific time frame does in fact tend to
lower the body weight of people who adhere to it).[2] In some cases there is a
specific alternative_hypothesis that is opposed to the null hypothesis, in
other cases the alternative hypothesis is not explicitly stated, or is simply
"the null hypothesis is false" â in either event, this is a binary judgment,
but the interpretation differs and is a matter of significant dispute in
statistics.
    * A type I error (or error of the first kind) is the incorrect rejection of
      a true null hypothesis. Usually a type I error leads to the conclusion
      that a supposed effect or relationship exists when in fact it does not.
      Examples of type I errors include a test that shows a patient to have a
      disease when in fact the patient does not have the disease, a fire alarm
      going on indicating a fire when in fact there is no fire, or an
      experiment indicating that a medical treatment should cure a disease when
      in fact it does not.
    * A type II error (or error of the second kind) is the failure to reject a
      false null hypothesis. Some examples of type II errors are a blood test
      failing to detect the disease it was designed to detect, in a patient who
      really has the disease; a fire breaking out and the fire alarm does not
      ring; or a clinical trial of a medical treatment failing to show that the
      treatment works when really it does.
In terms of false_positives_and_false_negatives, a positive result corresponds
to rejecting the null hypothesis, while a negative result corresponds to
failing to reject the null hypothesis; "false" means the conclusion drawn is
incorrect. Thus a type I error is a false positive, and a type II error is a
false negative.
When comparing two means, concluding the means were different when in reality
they were not different is a type I error; concluding the means were not
different when in reality they were different is a type II error. Various
extensions have been suggested as "type_III_errors", though none have wide use
[according_to_whom?].
All statistical_hypothesis_tests have a probability of making type I and type
II errors. For example, all blood tests for a disease will falsely detect the
disease in some proportion of people who do not have it, and will fail to
detect the disease in some proportion of people who do have it. A test's
probability of making a type I error is denoted by Î±. A test's probability of
making a type II error is denoted by Î². These error rates are traded off
against each other: for any given sample set, the effort to reduce one type of
error generally results in increasing the other type of error. For a given
test, the only way to reduce both error rates is to increase the sample size,
and this may not be feasible. A test statistic is robust if the Type I error
rate is controlled.[3][why?]
These terms are also used in a more general way by social scientists and others
to refer to flaws in reasoning.[4]
***** Statistical test theory[edit] *****
In statistical_test theory, the notion of a statistical error is an integral
part of hypothesis_testing. The test requires an unambiguous statement of a
null hypothesis, which usually corresponds to a default "state of nature", for
example "this person is healthy", "this accused is not guilty" or "this product
is not broken". An alternative hypothesis is the negation of null hypothesis,
for example, "this person is not healthy", "this accused is guilty" or "this
product is broken". The result of the test may be negative, relative to the
null hypothesis (not healthy, guilty, broken) or positive (healthy, not guilty,
not broken). If the result of the test corresponds with reality, then a correct
decision has been made. However, if the result of the test does not correspond
with reality, then an error has occurred. Due to the statistical nature of a
test, the result is never, except in very rare cases, free of error. Two types
of error are distinguished: type I error and type II error.
**** Type I error[edit] ****
A type I error occurs when the null_hypothesis (H0) is true, but is rejected.
It is asserting something that is absent, a false hit. A type I error may be
likened to a so-called false_positive (a result that indicates that a given
condition is present when it actually is not present).
In terms of folk tales, an investigator may see the wolf when there is none
("raising a false alarm"). Where the null hypothesis (H0) comprises the
statement: "There is no wolf".
The type I error rate or significance level is the probability of rejecting the
null hypothesis given that it is true.[5][6] It is denoted by the Greek letter
Î± (alpha) and is also called the alpha level. Often, the significance level is
set to 0.05 (5%), implying that it is acceptable to have a 5% probability of
incorrectly rejecting the null hypothesis.[5]
**** Type II error[edit] ****
A type II error occurs when the null hypothesis is false, but erroneously fails
to be rejected. It is failing to assert what is present, a miss. A type II
error may be compared with a so-called false_negative (where an actual hit was
disregarded by the test and is seen as a miss) in a test checking for a single
condition with a definitive result of true or false. A type II error is
committed when a true alternative hypothesis is not believed.[4]
In terms of folk tales, an investigator may fail to detect the metaphoric
"wolf" when in fact a wolf is present ( and therefore fail to raise an alarm).
Again, H0, the null hypothesis, comprises the statement: "There is no wolf",
which, if a wolf is indeed present, is a type II error on the part of the
investigator (the wolf either exists or does not exist within a given
contextâ the only question is if it is correctly detected or not, either
failing to detect it when it is present, or detecting it when it is not
present).
The rate of the type II error is denoted by the Greek letter Î² (beta) and
related to the power of a test (which equals 1âÎ²).
**** Table of error types[edit] ****
Tabularised relations between truth/falseness of the null hypothesis and
outcomes of the test:[2]

 Table of error types  Null hypothesis (H0) is
                         
                        True                     False
                                                 Type II error
                Fail to Correct inference        (false negative)
                reject  (true negative)          (probability = Î²) 
Decision                (probability = 1 - Î±)
about null
hypothesis (H0)         Type I error             Correct inference
                Reject  (false positive)         (true positive)
                        (probability = Î±)     (probability = 1 - Î²)
                                                  
***** Examples[edit] *****
**** Example 1[edit] ****
Hypothesis: "Adding water to toothpaste protects against cavities."
Null hypothesis (H0): "Adding water does not make toothpaste more effective in
fighting cavities."
This null hypothesis is tested against experimental data with a view to
nullifying it with evidence to the contrary.
A type I error occurs when detecting an effect (adding water to toothpaste
protects against cavities) that is not present. The null hypothesis is true
(i.e., it is true that adding water to toothpaste does not make it more
effective in protecting against cavities), but this null hypothesis is rejected
based on bad experimental data or an extreme outcome of chance alone.
**** Example 2[edit] ****
Hypothesis: "Adding fluoride to toothpaste protects against cavities."
Null hypothesis (H0): "Adding fluoride to toothpaste has no effect on
cavities."
This null hypothesis is tested against experimental data with a view to
nullifying it with evidence to the contrary.
A type II error occurs when failing to detect an effect (adding fluoride to
toothpaste protects against cavities) that is present. The null hypothesis is
false (i.e., adding fluoride is actually effective against cavities), but data
from the given experiment are such that the null hypothesis cannot be rejected.
**** Example 3[edit] ****
Hypothesis: "The evidence produced before the court proves that this man is
guilty."
Null hypothesis (H0): "This man is innocent."
A type I error occurs when convicting an innocent person (a miscarriage_of
justice). A type II error occurs when letting a guilty person go free (an error
of_impunity).
A positive correct outcome occurs when convicting a guilty person. A negative
correct outcome occurs when letting an innocent person go free.
**** Example 4[edit] ****
Hypothesis: "A patient's symptoms improve after treatment A more rapidly than
after a placebo treatment."
Null hypothesis (H0): "A patient's symptoms after treatment A are
indistinguishable from a placebo."
A Type I error would falsely indicate that treatment A is more effective than
the placebo, whereas a Type II error would be a failure to demonstrate that
treatment A is more effective than placebo even though it actually is more
effective.
***** Etymology[edit] *****
In 1928, Jerzy_Neyman (1894â1981) and Egon_Pearson (1895â1980), both
eminent statisticians, discussed the problems associated with "deciding whether
or not a particular sample may be judged as likely to have been randomly drawn
from a certain population"[7]p. 1: and, as Florence_Nightingale_David remarked,
"it is necessary to remember the adjective 'random' [in the term 'random
sample'] should apply to the method of drawing the sample and not to the sample
itself".[8]
They identified "two sources of error", namely:
      (a) the error of rejecting a hypothesis that should have not been
      rejected, and
      (b) the error of failing to reject a hypothesis that should have been
      rejected.[7]p.31
In 1930, they elaborated on these two sources of error, remarking that:
            ...in testing hypotheses two considerations must be kept in view,
            (1) we must be able to reduce the chance of rejecting a true
            hypothesis to as low a value as desired; (2) the test must be so
            devised that it will reject the hypothesis tested when it is likely
            to be false.[9]
In 1933, they observed that these "problems are rarely presented in such a form
that we can discriminate with certainty between the true and false hypothesis"
(p. 187). They also noted that, in deciding whether to fail to reject, or
reject a particular hypothesis amongst a "set of alternative hypotheses"
(p. 201), H1, H2, . . ., it was easy to make an error:
      ...[and] these errors will be of two kinds:
            (I) we reject H0 [i.e., the hypothesis to be tested] when it is
            true,
            (II) we fail to reject H0 when some alternative hypothesis HA or H1
            is true.[10]p.187 (There are various notations for the
            alternative).
In all of the papers co-written by Neyman and Pearson the expression H0 always
signifies "the hypothesis to be tested".
In the same paper[10]p. 190 they call these two sources of error, errors of
type I and errors of type II respectively.
***** Related terms[edit] *****
See also: Coverage_probability
**** Null hypothesis[edit] ****
Main article: Null_hypothesis
It is standard practice for statisticians to conduct tests in order to
determine whether or not a "speculative hypothesis" concerning the observed
phenomena of the world (or its inhabitants) can be supported. The results of
such testing determine whether a particular set of results agrees reasonably
(or does not agree) with the speculated hypothesis.
On the basis that it is always assumed, by statistical convention, that the
speculated hypothesis is wrong, and the so-called "null hypothesis" that the
observed phenomena simply occur by chance (and that, as a consequence, the
speculated agent has no effect) â the test will determine whether this
hypothesis is right or wrong. This is why the hypothesis under test is often
called the null hypothesis (most likely, coined by Fisher (1935, p. 19)),
because it is this hypothesis that is to be either nullified or not nullified
by the test. When the null hypothesis is nullified, it is possible to conclude
that data support the "alternative hypothesis" (which is the original
speculated one).
The consistent application by statisticians of Neyman and Pearson's convention
of representing "the hypothesis to be tested" (or "the hypothesis to be
nullified") with the expression H0 has led to circumstances where many
understand the term "the null hypothesis" as meaning "the nil hypothesis" â a
statement that the results in question have arisen through chance. This is not
necessarily the case â the key restriction, as per Fisher (1966), is that
"the null hypothesis must be exact, that is free from vagueness and ambiguity,
because it must supply the basis of the 'problem of distribution,' of which the
test of significance is the solution."[11] As a consequence of this, in
experimental science the null hypothesis is generally a statement that a
particular treatment has no effect; in observational science, it is that there
is no difference between the value of a particular measured variable, and that
of an experimental prediction.
**** Statistical significance[edit] ****
If the probability of obtaining a result as extreme as the one obtained,
supposing that the null hypothesis were true, is lower than a pre-specified
cut-off probability (for example, 5%), then the result is said to be
statistically_significant and the null hypothesis is rejected.
British statistician Sir_Ronald_Aylmer_Fisher (1890â1962) stressed that the
"null hypothesis":
     ... is never proved or established, but is possibly disproved, in the
     course of experimentation. Every experiment may be said to exist only
     in order to give the facts a chance of disproving the null
     hypothesis.
     â Fisher, 1935, p.19
***** Application domains[edit] *****
Statistical tests always involve a trade-off between:
   1. the acceptable level of false positives (in which a non-match is declared
      to be a match) and
   2. the acceptable level of false negatives (in which an actual match is not
      detected).
A threshold value can be varied to make the test more restrictive or more
sensitive, with the more restrictive tests increasing the risk of rejecting
true positives, and the more sensitive_tests increasing the risk of accepting
false positives.
**** Inventory control[edit] ****
An automated inventory control system that rejects high-quality goods of a
consignment commits a type I error, while a system that accepts low-quality
goods commits a type II error.
**** Computers[edit] ****
The notions of false positives and false negatives have a wide currency in the
realm of computers and computer applications, as follows.
*** Computer security[edit] ***
Main articles: computer_security and computer_insecurity
Security vulnerabilities are an important consideration in the task of keeping
computer data safe, while maintaining access to that data for appropriate
users. Moulton (1983), stresses the importance of:
    * avoiding the type I errors (or false positives) that classify authorized
      users as imposters.
    * avoiding the type II errors (or false negatives) that classify imposters
      as authorized users.
*** Spam filtering[edit] ***
A false positive occurs when spam_filtering or spam blocking techniques wrongly
classify a legitimate email message as spam and, as a result, interferes with
its delivery. While most anti-spam tactics can block or filter a high
percentage of unwanted emails, doing so without creating significant false-
positive results is a much more demanding task.
A false negative occurs when a spam email is not detected as spam, but is
classified as non-spam. A low number of false negatives is an indicator of the
efficiency of spam filtering.
*** Malware[edit] ***
The term "false positive" is also used when antivirus_software wrongly
classifies a harmless file as a virus. The incorrect detection may be due to
heuristics or to an incorrect virus_signature in a database. Similar problems
can occur with antitrojan or antispyware software.
*** Optical character recognition[edit] ***
Detection algorithms of all kinds often create false positives. Optical
character_recognition (OCR) software may detect an "a" where there are only
some dots that appear to be an "a" to the algorithm being used.
**** Security screening[edit] ****
Main articles: explosive_detection and metal_detector
False positives are routinely found every day in airport_security_screening,
which are ultimately visual_inspection systems. The installed security alarms
are intended to prevent weapons being brought onto aircraft; yet they are often
set to such high sensitivity that they alarm many times a day for minor items,
such as keys, belt buckles, loose change, mobile phones, and tacks in shoes.
The ratio of false positives (identifying an innocent traveller as a terrorist)
to true positives (detecting a would-be terrorist) is, therefore, very high;
and because almost every alarm is a false positive, the positive_predictive
value of these screening tests is very low.
The relative cost of false results determines the likelihood that test creators
allow these events to occur. As the cost of a false negative in this scenario
is extremely high (not detecting a bomb being brought onto a plane could result
in hundreds of deaths) whilst the cost of a false positive is relatively low (a
reasonably simple further inspection) the most appropriate test is one with a
low statistical specificity but high statistical sensitivity (one that allows a
high rate of false positives in return for minimal false negatives).
**** Biometrics[edit] ****
Biometric matching, such as for fingerprint_recognition, facial_recognition or
iris_recognition, is susceptible to type I and type II errors. The null
hypothesis is that the input does identify someone in the searched list of
people, so:
    * the probability of type I errors is called the "false reject rate" (FRR)
      or false non-match rate (FNMR),
    * while the probability of type II errors is called the "false accept rate"
      (FAR) or false match rate (FMR).[12]
If the system is designed to rarely match suspects then the probability of type
II errors can be called the "false_alarm rate". On the other hand, if the
system is used for validation (and acceptance is the norm) then the FAR is a
measure of system security, while the FRR measures user inconvenience level.
**** Medicine[edit] ****
Further information: False_positives_and_false_negatives
*** Medical screening[edit] ***
In the practice of medicine, there is a significant difference between the
applications of screening and testing.
    * Screening involves relatively cheap tests that are given to large
      populations, none of whom manifest any clinical indication of disease
      (e.g., Pap_smears).
    * Testing involves far more expensive, often invasive, procedures that are
      given only to those who manifest some clinical indication of disease, and
      are most often applied to confirm a suspected diagnosis.
For example, most states in the USA require newborns to be screened for
phenylketonuria and hypothyroidism, among other congenital_disorders. Although
they display a high rate of false positives, the screening tests are considered
valuable because they greatly increase the likelihood of detecting these
disorders at a far earlier stage.[13]
The simple blood tests used to screen possible blood_donors for HIV and
hepatitis have a significant rate of false positives; however, physicians use
much more expensive and far more precise tests to determine whether a person is
actually infected with either of these viruses.
Perhaps the most widely discussed false positives in medical screening come
from the breast cancer screening procedure mammography. The US rate of false
positive mammograms is up to 15%, the highest in world. One consequence of the
high false positive rate in the US is that, in any 10-year period, half of the
American women screened receive a false positive mammogram. False positive
mammograms are costly, with over $100 million spent annually in the U.S. on
follow-up testing and treatment. They also cause women unneeded anxiety. As a
result of the high false positive rate in the US, as many as 90â95% of women
who get a positive mammogram do not have the condition. The lowest rate in the
world is in the Netherlands, 1%. The lowest rates are generally in Northern
Europe where mammography films are read twice and a high threshold for
additional testing is set (the high threshold decreases the power of the test).
The ideal population screening test would be cheap, easy to administer, and
produce zero false-negatives, if possible. Such tests usually produce more
false-positives, which can subsequently be sorted out by more sophisticated
(and expensive) testing.
*** Medical testing[edit] ***
False negatives and false positives are significant issues in medical_testing.
False negatives may provide a falsely reassuring message to patients and
physicians that disease is absent, when it is actually present. This sometimes
leads to inappropriate or inadequate treatment of both the patient and their
disease. A common example is relying on cardiac_stress_tests to detect coronary
atherosclerosis, even though cardiac stress tests are known to only detect
limitations of coronary_artery blood flow due to advanced stenosis.
False negatives produce serious and counter-intuitive problems, especially when
the condition being searched for is common. If a test with a false negative
rate of only 10%, is used to test a population with a true occurrence rate of
70%, many of the negatives detected by the test will be false.
False positives can also produce serious and counter-intuitive problems when
the condition being searched for is rare, as in screening. If a test has a
false positive rate of one in ten thousand, but only one in a million samples
(or people) is a true positive, most of the positives detected by that test
will be false. The probability that an observed positive result is a false
positive may be calculated using Bayes'_theorem.
***** See also[edit] *****
    * [icon]Statistics_portal
    * Binary_classification
    * Detection_theory
    * Egon_Pearson
    * Ethics_in_mathematics
    * False_positive_paradox
    * Family-wise_error_rate
    * Information_retrieval_performance_measures
    * NeymanâPearson_lemma
    * Null_hypothesis
    * Probability_of_a_hypothesis for Bayesian inference
    * Precision_and_recall
    * Prosecutor's_fallacy
    * Prozone_phenomenon
    * Receiver_operating_characteristic
    * Sensitivity_and_specificity
    * Statisticians'_and_engineers'_cross-reference_of_statistical_terms
    * Testing_hypotheses_suggested_by_the_data
    * Type_III_error
***** Footnotes[edit] *****
   1. ^"Type_I_Error_and_Type_II_Error_-_Experimental_Errors". explorable.com.
      Retrieved 30 May 2016.
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
   3. ^ a bSheskin, David (2004). Handbook of Parametric and Nonparametric
      Statistical Procedures. CRC Press. p. 54. ISBN 1584884401.
   4. ^Derrick, B; Toher, D; White, P (2016). "Why_Welchs_test_is_Type_I_error
      robust" (PDF). The Quantitative Methods for Psychology. 12 (1): 30â38.
      doi:10.20982/tqmp.12.1.p030.
   5. ^ a bShermer, Michael (2002). The_Skeptic_Encyclopedia_of_Pseudoscience_2
      volume_set. ABC-CLIO. p. 455. ISBN 1-57607-653-9. Retrieved 10 January
      2011.
   6. ^ a bLindenmayer, David; Burgman, Mark A. (2005). "Monitoring, assessment
      and indicators". Practical Conservation Biology (PAP/CDR ed.).
      Collingwood, Victoria, Australia: CSIRO Publishing. pp. 401â424.
      ISBN 0-643-09089-4.
   7. ^Schlotzhauer, Sandra (2007). Elementary Statistics Using JMP (SAS Press)
      (1 ed.). Cary, NC: SAS Institute. pp. 166â423. ISBN 1-599-94375-1.
   8. ^ a bNeyman, J.; Pearson, E.S. (1967) [1928]. "On the Use and
      Interpretation of Certain Test Criteria for Purposes of Statistical
      Inference, Part I". Joint Statistical Papers. Cambridge University Press.
      pp. 1â66.
   9. ^David, F.N. (1949). Probability_Theory_for_Statistical_Methods.
      Cambridge University Press. p. 28.
  10. ^Pearson, E.S.; Neyman, J. (1967) [1930]. "On the Problem of Two
      Samples". Joint Statistical Papers. Cambridge University Press. p. 100.
  11. ^ a bNeyman, J.; Pearson, E.S. (1967) [1933]. "The testing of statistical
      hypotheses in relation to probabilities a priori". Joint Statistical
      Papers. Cambridge University Press. pp. 186â202.
  12. ^ Fisher, R.A. (1966). The design of experiments. 8th edition. Hafner:
      Edinburgh.
  13. ^Williams, G.O. (1996). "Iris_Recognition_Technology" (PDF).
      debut.cis.nctu.edu.tw. p. 56. Archived from the_original (PDF) on 26
      April 2011. Retrieved 23 May 2010. crossover error rate (that point where
      the probabilities of False Reject (Type I error) and False Fail to reject
      (Type II error) are approximately equal) is .00076%
  14. ^ In relation to this newborn screening, recent studies have shown that
      there are more than 12 times more false positives than correct screens
      (Gambrill, 2006. [1])
***** References[edit] *****
    * Betz, M.A. & Gabriel,_K.R., "Type IV Errors and Analysis of Simple
      Effects", Journal of Educational Statistics, Vol.3, No.2, (Summer 1978),
      pp. 121â144.
    * David, F.N., "A Power Function for Tests of Randomness in a Sequence of
      Alternatives", Biometrika, Vol.34, Nos.3/4, (December 1947),
      pp. 335â339.
    * Fisher, R.A., The Design of Experiments, Oliver & Boyd (Edinburgh), 1935.
    * Gambrill, W., "False Positives on Newborns' Disease Tests Worry Parents",
      Health Day, (5 June 2006). [2]
    * Kaiser, H.F., "Directional Statistical Decisions", Psychological Review,
      Vol.67, No.3, (May 1960), pp. 160â167.
    * Kimball, A.W., "Errors of the Third Kind in Statistical Consulting",
      Journal of the American Statistical Association, Vol.52, No.278, (June
      1957), pp. 133â142.
    * Lubin, A., "The Interpretation of Significant Interaction", Educational
      and Psychological Measurement, Vol.21, No.4, (Winter 1961),
      pp. 807â817.
    * Marascuilo, L.A. & Levin, J.R., "Appropriate Post Hoc Comparisons for
      Interaction and nested Hypotheses in Analysis of Variance Designs: The
      Elimination of Type-IV Errors", American Educational Research Journal,
      Vol.7., No.3, (May 1970), pp. 397â421.
    * Mitroff, I.I. & Featheringham, T.R., "On Systemic Problem Solving and the
      Error of the Third Kind", Behavioral Science, Vol.19, No.6, (November
      1974), pp. 383â393.
    * Mosteller, F., "A k-Sample Slippage Test for an Extreme Population", The
      Annals of Mathematical Statistics, Vol.19, No.1, (March 1948),
      pp. 58â65.
    * Moulton, R.T., âNetwork Securityâ, Datamation, Vol.29, No.7, (July
      1983), pp. 121â127.
    * Raiffa, H., Decision Analysis: Introductory Lectures on Choices Under
      Uncertainty, AddisonâWesley, (Reading), 1968.
***** External links[edit] *****
    * Bias_and_Confounding â presentation by Nigel Paneth, Graduate School of
      Public Health, University of Pittsburgh
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
            Testing_hypotheses            o Uniformly_most_powerful_test
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

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Type_I_and_type_II_errors&oldid=906551687"
Categories:
    * Design_of_experiments
    * Error
    * Statistical_hypothesis_testing
    * Spam_filtering
Hidden categories:
    * Articles_with_short_description
    * Wikipedia_articles_that_are_too_technical_from_April_2019
    * All_articles_that_are_too_technical
    * Articles_needing_expert_attention_from_April_2019
    * All_articles_needing_expert_attention
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_June_2019
    * All_articles_with_specifically_marked_weasel-worded_phrases
    * Articles_with_specifically_marked_weasel-worded_phrases_from_June_2019
    * Wikipedia_articles_needing_clarification_from_June_2019
    * Use_dmy_dates_from_October_2012
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * Galego
    * íêµ­ì´
    * Ãslenska
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 16 July 2019, at 15:59 (UTC).
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
