The following text has been accessed from https://en.wikipedia.org/wiki/Design_of_experiments at Fri Aug 9 02:53:15 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Design of experiments ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For the book, see The_Design_of_Experiments.
 This article has multiple issues. Please help improve_it or discuss these issues on the talk_page.
 (Learn_how_and_when_to_remove_these_template_messages)
  This article needs additional citations for verification. Please help improve_this_article by adding_citations_to
  reliable_sources. Unsourced material may be challenged and removed.
  Find sources: "Design_of_experiments" â news Â· newspapers Â· books Â· scholar Â· JSTOR (September 2015)(Learn_how
  and_when_to_remove_this_template_message)
  This article possibly contains original_research. Please improve_it by verifying the claims made and
  adding inline_citations. Statements consisting only of original research should be removed.
  (September 2015)(Learn_how_and_when_to_remove_this_template_message)
 (Learn_how_and_when_to_remove_this_template_message)
Design of experiments with full factorial_design (left), response_surface with
second-degree polynomial (right)
The design of experiments (DOE, DOX, or experimental design) is the design of
any task that aims to describe or explain the variation of information under
conditions that are hypothesized to reflect the variation. The term is
generally associated with experiments in which the design introduces conditions
that directly affect the variation, but may also refer to the design of quasi-
experiments, in which natural conditions that influence the variation are
selected for observation.
In its simplest form, an experiment aims at predicting the outcome by
introducing a change of the preconditions, which is represented by one or more
independent_variables, also referred to as "input variables" or "predictor
variables." The change in one or more independent variables is generally
hypothesized to result in a change in one or more dependent_variables, also
referred to as "output variables" or "response variables." The experimental
design may also identify control_variables that must be held constant to
prevent external factors from affecting the results. Experimental design
involves not only the selection of suitable independent, dependent, and control
variables, but planning the delivery of the experiment under statistically
optimal conditions given the constraints of available resources. There are
multiple approaches for determining the set of design points (unique
combinations of the settings of the independent variables) to be used in the
experiment.
Main concerns in experimental design include the establishment of validity,
reliability, and replicability. For example, these concerns can be partially
addressed by carefully choosing the independent variable, reducing the risk of
measurement error, and ensuring that the documentation of the method is
sufficiently detailed. Related concerns include achieving appropriate levels of
statistical_power and sensitivity.
Correctly designed experiments advance knowledge in the natural and social
sciences and engineering. Other applications include marketing and policy
making. The study of the design of experiments is an important topic in
metascience.
⁰
***** Contents *****
    * 1_History
          o 1.1_Systematic_clinical_trials
          o 1.2_Statistical_experiments,_following_Charles_S._Peirce
                # 1.2.1_Randomized_experiments
                # 1.2.2_Optimal_designs_for_regression_models
          o 1.3_Sequences_of_experiments
    * 2_Fisher's_principles
    * 3_Example
    * 4_Avoiding_false_positives
    * 5_Discussion_topics_when_setting_up_an_experimental_design
    * 6_Causal_attributions
    * 7_Statistical_control
    * 8_Experimental_designs_after_Fisher
    * 9_Human_participant_constraints
    * 10_See_also
    * 11_References
          o 11.1_Sources
    * 12_External_links
***** History[edit] *****
**** Systematic clinical trials[edit] ****
 This section possibly contains original_research. Please improve_it by
 verifying the claims made and adding inline_citations. Statements consisting
 only of original research should be removed. (September 2015)(Learn_how_and
 when_to_remove_this_template_message)
                        This section relies too much on references to primary
[Question_book-new.svg] sources. Please improve this section by adding
                        secondary_or_tertiary_sources. (September 2015)(Learn
                        how_and_when_to_remove_this_template_message)
In 1747, while serving as surgeon on HMS_Salisbury, James_Lind carried out a
systematic clinical trial to compare remedies for scurvy.[1] This systematic
clinical trial constitutes a type of DOE.[citation_needed][dubious  – discuss]
Lind selected 12 men from the ship, all suffering from scurvy. Lind limited his
subjects to men who "were as similar as I could have them," that is, he
provided strict entry requirements to reduce extraneous variation. He divided
them into six pairs, giving each pair different supplements to their basic diet
for two weeks. The treatments were all remedies that had been proposed:
    * A quart of cider every day.
    * Twenty five gutts (drops) of vitriol (sulphuric acid) three times a day
      upon an empty stomach.
    * One half-pint of seawater every day.
    * A mixture of garlic, mustard, and horseradish in a lump the size of a
      nutmeg.
    * Two spoonfuls of vinegar three times a day.
    * Two oranges and one lemon every day.
The citrus treatment stopped after six days when they ran out of fruit, but by
that time one sailor was fit for duty while the other had almost recovered.
Apart from that, only group one (cider) showed some effect of its treatment.
The remainder of the crew presumably served as a control, but Lind did not
report results from any control (untreated) group.[citation_needed]
**** Statistical experiments, following Charles S. Peirce[edit] ****
Main article: Frequentist_statistics
See also: Randomization
A theory of statistical inference was developed by Charles_S._Peirce in
"Illustrations_of_the_Logic_of_Science" (1877â1878) and "A_Theory_of_Probable
Inference" (1883), two publications that emphasized the importance of
randomization-based inference in statistics.[citation_needed]
*** Randomized experiments[edit] ***
Main article: Random_assignment
See also: Repeated_measures_design
Charles S. Peirce randomly assigned volunteers to a blinded, repeated-measures
design to evaluate their ability to discriminate weights.[2][3][4][5] Peirce's
experiment inspired other researchers in psychology and education, which
developed a research tradition of randomized experiments in laboratories and
specialized textbooks in the 1800s.[2][3][4][5]
*** Optimal designs for regression models[edit] ***
Main article: Response_surface_methodology
See also: Optimal_design
Charles_S._Peirce also contributed the first English-language publication on an
optimal_design for regression models in 1876.[6] A pioneering optimal_design
for polynomial_regression was suggested by Gergonne in 1815. In 1918, Kirstine
Smith published optimal designs for polynomials of degree six (and less).
[citation_needed]
**** Sequences of experiments[edit] ****
Main article: Sequential_analysis
See also: Multi-armed_bandit_problem, Gittins_index, and Optimal_design
The use of a sequence of experiments, where the design of each may depend on
the results of previous experiments, including the possible decision to stop
experimenting, is within the scope of Sequential_analysis, a field that was
pioneered[7] by Abraham_Wald in the context of sequential tests of statistical
hypotheses.[8] Herman_Chernoff wrote an overview of optimal sequential designs,
[9] while adaptive_designs have been surveyed by S. Zacks.[10] One specific
type of sequential design is the "two-armed bandit", generalized to the multi-
armed_bandit, on which early work was done by Herbert_Robbins in 1952.[11]
***** Fisher's principles[edit] *****
A methodology for designing experiments was proposed by Ronald_Fisher, in his
innovative books: The Arrangement of Field Experiments (1926) and The_Design_of
Experiments (1935). Much of his pioneering work dealt with agricultural
applications of statistical methods. As a mundane example, he described how to
test the lady_tasting_tea hypothesis, that a certain lady could distinguish by
flavour alone whether the milk or the tea was first placed in the cup. These
methods have been broadly adapted in the physical and social sciences, are
still used in agricultural_engineering and differ from the design and analysis
of computer_experiments.[citation_needed]
  Comparison
      In some fields of study it is not possible to have independent
      measurements to a traceable metrology_standard. Comparisons between
      treatments are much more valuable and are usually preferable, and often
      compared against a scientific_control or traditional treatment that acts
      as baseline.
  Randomization
      Random assignment is the process of assigning individuals at random to
      groups or to different groups in an experiment, so that each individual
      of the population has the same chance of becoming a participant in the
      study. The random assignment of individuals to groups (or conditions
      within a group) distinguishes a rigorous, "true" experiment from an
      observational study or "quasi-experiment".[12] There is an extensive body
      of mathematical theory that explores the consequences of making the
      allocation of units to treatments by means of some random mechanism (such
      as tables of random numbers, or the use of randomization devices such as
      playing cards or dice). Assigning units to treatments at random tends to
      mitigate confounding, which makes effects due to factors other than the
      treatment to appear to result from the treatment.
      The risks associated with random allocation (such as having a serious
      imbalance in a key characteristic between a treatment group and a control
      group) are calculable and hence can be managed down to an acceptable
      level by using enough experimental units. However, if the population is
      divided into several subpopulations that somehow differ, and the research
      requires each subpopulation to be equal in size, stratified sampling can
      be used. In that way, the units in each subpopulation are randomized, but
      not the whole sample. The results of an experiment can be generalized
      reliably from the experimental units to a larger statistical_population
      of units only if the experimental units are a random_sample from the
      larger population; the probable error of such an extrapolation depends on
      the sample size, among other things.
  Statistical_replication
      Measurements are usually subject to variation and measurement
      uncertainty; thus they are repeated and full experiments are replicated
      to help identify the sources of variation, to better estimate the true
      effects of treatments, to further strengthen the experiment's reliability
      and validity, and to add to the existing knowledge of the topic.[13]
      However, certain conditions must be met before the replication of the
      experiment is commenced: the original research question has been
      published in a peer-reviewed journal or widely cited, the researcher is
      independent of the original experiment, the researcher must first try to
      replicate the original findings using the original data, and the write-up
      should state that the study conducted is a replication study that tried
      to follow the original study as strictly as possible.[14]
  Blocking
      Blocking is the non-random arrangement of experimental units into groups
      (blocks/lots) consisting of units that are similar to one another.
      Blocking reduces known but irrelevant sources of variation between units
      and thus allows greater precision in the estimation of the source of
      variation under study.
  Orthogonality
Example of orthogonal factorial design
      Orthogonality concerns the forms of comparison (contrasts) that can be
      legitimately and efficiently carried out. Contrasts can be represented by
      vectors and sets of orthogonal contrasts are uncorrelated and
      independently distributed if the data are normal. Because of this
      independence, each orthogonal treatment provides different information to
      the others. If there are T treatments and T â 1 orthogonal contrasts,
      all the information that can be captured from the experiment is
      obtainable from the set of contrasts.
  Factorial_experiments
      Use of factorial experiments instead of the one-factor-at-a-time method.
      These are efficient at evaluating the effects and possible interactions
      of several factors (independent variables). Analysis of experiment design
      is built on the foundation of the analysis_of_variance, a collection of
      models that partition the observed variance into components, according to
      what factors the experiment must estimate or test.
***** Example[edit] *****
[Balance_Ã _tabac_1850.JPG]
This example is attributed to Harold_Hotelling.[9] It conveys some of the
flavor of those aspects of the subject that involve combinatorial designs.
[citation_needed]
Weights of eight objects are measured using a pan_balance and set of standard
weights. Each weighing measures the weight difference between objects in the
left pan vs. any objects in the right pan by adding calibrated weights to the
lighter pan until the balance is in equilibrium. Each measurement has a random
error. The average error is zero; the standard_deviations of the probability
distribution of the errors is the same number Ï on different weighings; errors
on different weighings are independent. Denote the true weights by
          &#x03B8;  1   , &#x2026; ,  &#x03B8;  8   .    {\displaystyle \theta
      _{1},\dots ,\theta _{8}.\,}  [\theta_1, \dots, \theta_8.\,]
We consider two different experiments:
   1. Weigh each object in one pan, with the other pan empty. Let Xi be the
      measured weight of the object, for i = 1, ..., 8.
   2. Do the eight weighings according to the following schedule and let Yi be
      the measured difference for i = 1, ..., 8:
                     left pan     right pan       1st weighing:    1 &#xA0; 2
            &#xA0; 3 &#xA0; 4 &#xA0; 5 &#xA0; 6 &#xA0; 7 &#xA0; 8    (empty)
            2nd:    1 &#xA0; 2 &#xA0; 3 &#xA0; 8 &#xA0;   4 &#xA0; 5 &#xA0; 6
            &#xA0; 7      3rd:    1 &#xA0; 4 &#xA0; 5 &#xA0; 8 &#xA0;   2
            &#xA0; 3 &#xA0; 6 &#xA0; 7      4th:    1 &#xA0; 6 &#xA0; 7 &#xA0;
            8 &#xA0;   2 &#xA0; 3 &#xA0; 4 &#xA0; 5      5th:    2 &#xA0; 4
            &#xA0; 6 &#xA0; 8 &#xA0;   1 &#xA0; 3 &#xA0; 5 &#xA0; 7      6th:
            2 &#xA0; 5 &#xA0; 7 &#xA0; 8 &#xA0;   1 &#xA0; 3 &#xA0; 4 &#xA0; 6
            7th:    3 &#xA0; 4 &#xA0; 7 &#xA0; 8 &#xA0;   1 &#xA0; 2 &#xA0; 5
            &#xA0; 6      8th:    3 &#xA0; 5 &#xA0; 6 &#xA0; 8 &#xA0;   1
            &#xA0; 2 &#xA0; 4 &#xA0; 7       {\displaystyle {\begin{array}
            {lcc}&{\text{left pan}}&{\text{right pan}}\\\hline {\text{1st
            weighing:}}&1\ 2\ 3\ 4\ 5\ 6\ 7\ 8&{\text{(empty)}}\\{\text{2nd:
            }}&1\ 2\ 3\ 8\ &4\ 5\ 6\ 7\\{\text{3rd:}}&1\ 4\ 5\ 8\ &2\ 3\ 6\ 7\\
            {\text{4th:}}&1\ 6\ 7\ 8\ &2\ 3\ 4\ 5\\{\text{5th:}}&2\ 4\ 6\ 8\
            &1\ 3\ 5\ 7\\{\text{6th:}}&2\ 5\ 7\ 8\ &1\ 3\ 4\ 6\\{\text{7th:
            }}&3\ 4\ 7\ 8\ &1\ 2\ 5\ 6\\{\text{8th:}}&3\ 5\ 6\ 8\ &1\ 2\ 4\
            7\end{array}}}  [{\displaystyle {\begin{array}{lcc}&{\text{left
            pan}}&{\text{right pan}}\\\hline {\text{1st weighing:}}&1\ 2\ 3\ 4\
            5\ 6\ 7\ 8&{\text{(empty)}}\\{\text{2nd:}}&1\ 2\ 3\ 8\ &4\ 5\ 6\
            7\\{\text{3rd:}}&1\ 4\ 5\ 8\ &2\ 3\ 6\ 7\\{\text{4th:}}&1\ 6\ 7\ 8\
            &2\ 3\ 4\ 5\\{\text{5th:}}&2\ 4\ 6\ 8\ &1\ 3\ 5\ 7\\{\text{6th:
            }}&2\ 5\ 7\ 8\ &1\ 3\ 4\ 6\\{\text{7th:}}&3\ 4\ 7\ 8\ &1\ 2\ 5\ 6\\
            {\text{8th:}}&3\ 5\ 6\ 8\ &1\ 2\ 4\ 7\end{array}}}]
      Then the estimated value of the weight θ1 is
                   &#x03B8; &#x005E;     1   =     Y  1   +  Y  2   +  Y  3   +
            Y  4   &#x2212;  Y  5   &#x2212;  Y  6   &#x2212;  Y  7   &#x2212;
            Y  8    8   .   {\displaystyle {\widehat {\theta }}_{1}={\frac {Y_
            {1}+Y_{2}+Y_{3}+Y_{4}-Y_{5}-Y_{6}-Y_{7}-Y_{8}}{8}}.}  [\widehat
            {\theta}_1 = \frac{Y_1 + Y_2 + Y_3 + Y_4 - Y_5 - Y_6 - Y_7 - Y_8}
            {8}. ]
      Similar estimates can be found for the weights of the other items. For
      example
                       &#x03B8; &#x005E;     2      =     Y  1   +  Y  2
            &#x2212;  Y  3   &#x2212;  Y  4   +  Y  5   +  Y  6   &#x2212;  Y
            7   &#x2212;  Y  8    8   .         &#x03B8; &#x005E;     3      =
            Y  1   +  Y  2   &#x2212;  Y  3   &#x2212;  Y  4   &#x2212;  Y  5
            &#x2212;  Y  6   +  Y  7   +  Y  8    8   .         &#x03B8;
            &#x005E;     4      =     Y  1   &#x2212;  Y  2   +  Y  3
            &#x2212;  Y  4   +  Y  5   &#x2212;  Y  6   +  Y  7   &#x2212;  Y
            8    8   .         &#x03B8; &#x005E;     5      =     Y  1
            &#x2212;  Y  2   +  Y  3   &#x2212;  Y  4   &#x2212;  Y  5   +  Y
            6   &#x2212;  Y  7   +  Y  8    8   .         &#x03B8; &#x005E;
            6      =     Y  1   &#x2212;  Y  2   &#x2212;  Y  3   +  Y  4   +
            Y  5   &#x2212;  Y  6   &#x2212;  Y  7   +  Y  8    8   .
            &#x03B8; &#x005E;     7      =     Y  1   &#x2212;  Y  2   &#x2212;
            Y  3   +  Y  4   &#x2212;  Y  5   +  Y  6   +  Y  7   &#x2212;  Y
            8    8   .         &#x03B8; &#x005E;     8      =     Y  1   +  Y
            2   +  Y  3   +  Y  4   +  Y  5   +  Y  6   +  Y  7   +  Y  8    8
            .       {\displaystyle {\begin{aligned}{\widehat {\theta }}_{2}&=
            {\frac {Y_{1}+Y_{2}-Y_{3}-Y_{4}+Y_{5}+Y_{6}-Y_{7}-Y_{8}}{8}}.\\
            [5pt]{\widehat {\theta }}_{3}&={\frac {Y_{1}+Y_{2}-Y_{3}-Y_{4}-Y_
            {5}-Y_{6}+Y_{7}+Y_{8}}{8}}.\\[5pt]{\widehat {\theta }}_{4}&={\frac
            {Y_{1}-Y_{2}+Y_{3}-Y_{4}+Y_{5}-Y_{6}+Y_{7}-Y_{8}}{8}}.\\[5pt]
            {\widehat {\theta }}_{5}&={\frac {Y_{1}-Y_{2}+Y_{3}-Y_{4}-Y_{5}+Y_
            {6}-Y_{7}+Y_{8}}{8}}.\\[5pt]{\widehat {\theta }}_{6}&={\frac {Y_
            {1}-Y_{2}-Y_{3}+Y_{4}+Y_{5}-Y_{6}-Y_{7}+Y_{8}}{8}}.\\[5pt]{\widehat
            {\theta }}_{7}&={\frac {Y_{1}-Y_{2}-Y_{3}+Y_{4}-Y_{5}+Y_{6}+Y_{7}-
            Y_{8}}{8}}.\\[5pt]{\widehat {\theta }}_{8}&={\frac {Y_{1}+Y_{2}+Y_
            {3}+Y_{4}+Y_{5}+Y_{6}+Y_{7}+Y_{8}}{8}}.\end{aligned}}}  [
            {\displaystyle {\begin{aligned}{\widehat {\theta }}_{2}&={\frac {Y_
            {1}+Y_{2}-Y_{3}-Y_{4}+Y_{5}+Y_{6}-Y_{7}-Y_{8}}{8}}.\\[5pt]{\widehat
            {\theta }}_{3}&={\frac {Y_{1}+Y_{2}-Y_{3}-Y_{4}-Y_{5}-Y_{6}+Y_
            {7}+Y_{8}}{8}}.\\[5pt]{\widehat {\theta }}_{4}&={\frac {Y_{1}-Y_
            {2}+Y_{3}-Y_{4}+Y_{5}-Y_{6}+Y_{7}-Y_{8}}{8}}.\\[5pt]{\widehat
            {\theta }}_{5}&={\frac {Y_{1}-Y_{2}+Y_{3}-Y_{4}-Y_{5}+Y_{6}-Y_
            {7}+Y_{8}}{8}}.\\[5pt]{\widehat {\theta }}_{6}&={\frac {Y_{1}-Y_
            {2}-Y_{3}+Y_{4}+Y_{5}-Y_{6}-Y_{7}+Y_{8}}{8}}.\\[5pt]{\widehat
            {\theta }}_{7}&={\frac {Y_{1}-Y_{2}-Y_{3}+Y_{4}-Y_{5}+Y_{6}+Y_{7}-
            Y_{8}}{8}}.\\[5pt]{\widehat {\theta }}_{8}&={\frac {Y_{1}+Y_{2}+Y_
            {3}+Y_{4}+Y_{5}+Y_{6}+Y_{7}+Y_{8}}{8}}.\end{aligned}}}]
The question of design of experiments is: which experiment is better?
The variance of the estimate X1 of Î¸1 is Ï2 if we use the first experiment.
But if we use the second experiment, the variance of the estimate given above
is Ï2/8. Thus the second experiment gives us 8 times as much precision for the
estimate of a single item, and estimates all items simultaneously, with the
same precision. What the second experiment achieves with eight would require 64
weighings if the items are weighed separately. However, note that the estimates
for the items obtained in the second experiment have errors that correlate with
each other.
Many problems of the design of experiments involve combinatorial_designs, as in
this example and others.[15]
***** Avoiding false positives[edit] *****
See also: Metascience
False_positive conclusions, often resulting from the pressure_to_publish or the
author's own confirmation_bias, are an inherent hazard in many fields. A good
way to prevent biases potentially leading to false positives in the data
collection phase is to use a double-blind design. When a double-blind design is
used, participants are randomly assigned to experimental groups but the
researcher is unaware of what participants belong to which group. Therefore,
the researcher can not affect the participants' response to the intervention.
Experimental designs with undisclosed degrees of freedom are a problem.[16]
This can lead to conscious or unconscious "p-hacking": trying multiple things
until you get the desired result. It typically involves the manipulation -
perhaps unconsciously - of the process of statistical_analysis and the degrees
of freedom until they return a figure below the p<.05 level of statistical
significance.[17][18] So the design of the experiment should include a clear
statement proposing the analyses to be undertaken. P-hacking can be prevented
by preregistering researches, in which researchers have to send their data
analysis plan to the journal they wish to publish their paper in before they
even start their data collection, so no data manipulation is possible (https://
osf.io). Another way to prevent this is taking the double-blind design to the
data-analysis phase, where the data are sent to a data-analyst unrelated to the
research who scrambles up the data so there is no way to know which
participants belong to before they are potentially taken away as outliers.
Clear and complete documentation of the experimental methodology is also
important in order to support replication of results.[19]
***** Discussion topics when setting up an experimental design[edit] *****
An experimental design or randomized clinical trial requires careful
consideration of several factors before actually doing the experiment.[20] An
experimental design is the laying out of a detailed experimental plan in
advance of doing the experiment. Some of the following topics have already been
discussed in the principles of experimental design section:
   1. How many factors does the design have, and are the levels of these
      factors fixed or random?
   2. Are control conditions needed, and what should they be?
   3. Manipulation checks; did the manipulation really work?
   4. What are the background variables?
   5. What is the sample size. How many units must be collected for the
      experiment to be generalisable and have enough power?
   6. What is the relevance of interactions between factors?
   7. What is the influence of delayed effects of substantive factors on
      outcomes?
   8. How do response shifts affect self-report measures?
   9. How feasible is repeated administration of the same measurement
      instruments to the same units at different occasions, with a post-test
      and follow-up tests?
  10. What about using a proxy pretest?
  11. Are there lurking variables?
  12. Should the client/patient, researcher or even the analyst of the data be
      blind to conditions?
  13. What is the feasibility of subsequent application of different conditions
      to the same units?
  14. How many of each control and noise factors should be taken into account?
The independent variable of a study often has many levels or different groups.
In a true experiment, researchers can have an experimental group, which is
where their intervention testing the hypothesis is implemented, and a control
group, which has all the same element as the experimental group, without the
interventional element. Thus, when everything else except for one intervention
is held constant, researchers can certify with some certainty that this one
element is what caused the observed change. In some instances, having a control
group is not ethical. This is sometimes solved using two different experimental
groups. In some cases, independent variables cannot be manipulated, for example
when testing the difference between two groups who have a different disease, or
testing the difference between genders (obviously variables that would be hard
or unethical to assign participants to). In these cases, a quasi-experimental
design may be used.
***** Causal attributions[edit] *****
In the pure experimental design, the independent (predictor) variable is
manipulated by the researcher - that is - every participant of the research is
chosen randomly from the population, and each participant chosen is assigned
randomly to conditions of the independent variable. Only when this is done is
it possible to certify with high probability that the reason for the
differences in the outcome variables are caused by the different conditions.
Therefore, researchers should choose the experimental design over other design
types whenever possible. However, the nature of the independent variable does
not always allow for manipulation. In those cases, researchers must be aware of
not certifying about causal attribution when their design doesn't allow for it.
For example, in observational designs, participants are not assigned randomly
to conditions, and so if there are differences found in outcome variables
between conditions, it is likely that there is something other than the
differences between the conditions that causes the differences in outcomes,
that is - a third variable. The same goes for studies with correlational
design. (AdÃ©r & Mellenbergh, 2008).
***** Statistical control[edit] *****
It is best that a process be in reasonable statistical control prior to
conducting designed experiments. When this is not possible, proper blocking,
replication, and randomization allow for the careful conduct of designed
experiments.[21] To control for nuisance variables, researchers institute
control checks as additional measures. Investigators should ensure that
uncontrolled influences (e.g., source credibility perception) do not skew the
findings of the study. A manipulation_check is one example of a control check.
Manipulation checks allow investigators to isolate the chief variables to
strengthen support that these variables are operating as planned.
One of the most important requirements of experimental research designs is the
necessity of eliminating the effects of spurious, intervening, and antecedent
variables. In the most basic model, cause (X) leads to effect (Y). But there
could be a third variable (Z) that influences (Y), and X might not be the true
cause at all. Z is said to be a spurious variable and must be controlled for.
The same is true for intervening_variables (a variable in between the supposed
cause (X) and the effect (Y)), and anteceding variables (a variable prior to
the supposed cause (X) that is the true cause). When a third variable is
involved and has not been controlled for, the relation is said to be a zero
order relationship. In most practical applications of experimental research
designs there are several causes (X1, X2, X3). In most designs, only one of
these causes is manipulated at a time.
***** Experimental designs after Fisher[edit] *****
Some efficient designs for estimating several main effects were found
independently and in near succession by Raj_Chandra_Bose and K. Kishen in 1940
at the Indian_Statistical_Institute, but remained little known until the
PlackettâBurman_designs were published in Biometrika in 1946. About the same
time, C._R._Rao introduced the concepts of orthogonal_arrays as experimental
designs. This concept played a central role in the development of Taguchi
methods by Genichi_Taguchi, which took place during his visit to Indian
Statistical Institute in early 1950s. His methods were successfully applied and
adopted by Japanese and Indian industries and subsequently were also embraced
by US industry albeit with some reservations.
In 1950, Gertrude_Mary_Cox and William_Gemmell_Cochran published the book
Experimental Designs, which became the major reference work on the design of
experiments for statisticians for years afterwards.
Developments of the theory of linear_models have encompassed and surpassed the
cases that concerned early writers. Today, the theory rests on advanced topics
in linear_algebra, algebra and combinatorics.
As with other branches of statistics, experimental design is pursued using both
frequentist and Bayesian approaches: In evaluating statistical procedures like
experimental designs, frequentist_statistics studies the sampling_distribution
while Bayesian_statistics updates a probability_distribution on the parameter
space.
Some important contributors to the field of experimental designs are C._S.
Peirce, R._A._Fisher, F._Yates, C._R._Rao, R._C._Bose, J._N._Srivastava,
Shrikhande_S._S., D._Raghavarao, W._G._Cochran, O._Kempthorne, W. T. Federer,
V. V. Fedorov, A. S. Hedayat, J._A._Nelder, R._A._Bailey, J._Kiefer, W. J.
Studden, A. PÃ¡zman, F. Pukelsheim, D._R._Cox, H. P. Wynn, A. C. Atkinson, G.
E._P._Box and G._Taguchi.[citation_needed] The textbooks of D. Montgomery, R.
Myers, and G. Box/W. Hunter/J.S. Hunter have reached generations of students
and practitioners. [22] [23] [24] [25] [26]
Some discussion of experimental design in the context of system_identification
(model building for static or dynamic models) is given in [27] and [28].
***** Human participant constraints[edit] *****
Laws and ethical considerations preclude some carefully designed experiments
with human subjects. Legal constraints are dependent on jurisdiction.
Constraints may involve institutional_review_boards, informed_consent and
confidentiality affecting both clinical (medical) trials and behavioral and
social science experiments.[29] In the field of toxicology, for example,
experimentation is performed on laboratory animals with the goal of defining
safe exposure limits for humans.[30] Balancing the constraints are views from
the medical field.[31] Regarding the randomization of patients, "... if no one
knows which therapy is better, there is no ethical imperative to use one
therapy or another." (p 380) Regarding experimental design, "...it is clearly
not ethical to place subjects at risk to collect data in a poorly designed
study when this situation can be easily avoided...". (p 393)
***** See also[edit] *****
    * [icon]Statistics_portal
    * Adversarial_collaboration
    * Bayesian_experimental_design
    * Block_design
    * BoxâBehnken_design
    * Central_composite_design
    * Clinical_trial
    * Clinical_study_design
    * Computer_experiment
    * Control_variable
    * Controlling_for_a_variable
    * Experimetrics (econometrics-related experiments)
    * Factor_analysis
    * Fractional_factorial_design
    * Glossary_of_experimental_design
    * Grey_box_model
    * Industrial_engineering
    * Instrument_effect
    * Law_of_large_numbers
    * Manipulation_checks
    * Multifactor_design_of_experiments_software
    * One-factor-at-a-time_method
    * Optimal_design
    * Plackett-Burman_design
    * Probabilistic_design
    * Protocol_(natural_sciences)
    * Quasi-experimental_design
    * Randomized_block_design
    * Randomized_controlled_trial
    * Research_design
    * Robust_parameter_design
    * Sample_size_determination
    * Supersaturated design
    * Survey_sampling
    * System_identification
    * Taguchi_methods
***** References[edit] *****
   1. ^Dunn, Peter (January 1997). "James_Lind_(1716-94)_of_Edinburgh_and_the
      treatment_of_scurvy". Archives of Disease in Childhood: Fetal and
      Neonatal Edition. 76 (1): 64â65. doi:10.1136/fn.76.1.F64. PMC 1720613.
      PMID 9059193. Retrieved 17 January 2009.
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
   3. ^ a bPeirce,_Charles_Sanders; Jastrow,_Joseph (1885). "On_Small
      Differences_in_Sensation". Memoirs of the National Academy of Sciences.
      3: 73â83.
   4. ^ a b Hacking,_Ian (September 1988). "Telepathy: Origins of Randomization
      in Experimental Design". Isis. 79 (3): 427â451. doi:10.1086/354775.
      JSTOR 234674. MR 1013489.
   5. ^ a b Stephen_M._Stigler (November 1992). "A Historical View of
      Statistical Concepts in Psychology and Educational Research". American
      Journal of Education. 101 (1): 60â70. doi:10.1086/444032.
      JSTOR 1085417.
   6. ^ a b Trudy Dehue (December 1997). "Deception, Efficiency, and Random
      Groups: Psychology and the Gradual Origination of the Random Group
      Design". Isis. 88 (4): 653â673. doi:10.1086/383850. PMID 9519574.
   7. ^Peirce,_C._S. (1876). "Note on the Theory of the Economy of Research".
      Coast Survey Report: 197â201.
   8. , actually published 1879, NOAA PDF_Eprint.
      Reprinted in Collected_Papers 7, paragraphs 139â157, also in Writings
      4, pp. 72â78, and inPeirce,_C._S. (July â August 1967). "Note on the
      Theory of the Economy of Research". Operations Research. 15 (4):
      643â648. doi:10.1287/opre.15.4.643. JSTOR 168276.
   9. ^ Johnson, N.L. (1961). "Sequential analysis: a survey." Journal_of_the
      Royal_Statistical_Society, Series A. Vol. 124 (3), 372–411. (pages
      375–376)
  10. ^ Wald, A. (1945) "Sequential Tests of Statistical Hypotheses", Annals_of
      Mathematical_Statistics, 16 (2), 117–186.
  11. ^ a b Herman_Chernoff, Sequential Analysis and Optimal Design, SIAM
      Monograph, 1972.
  12. ^ Zacks, S. (1996) "Adaptive Designs for Parametric Models". In: Ghosh,
      S. and Rao, C. R., (Eds) (1996). "Design and Analysis of Experiments,"
      Handbook of Statistics, Volume 13. North-Holland.
  13. ISBN 0-444-82061-2. (pages 151–180)
  14. ^Robbins, H. (1952). "Some Aspects of the Sequential Design of
      Experiments". Bulletin of the American Mathematical Society. 58 (5):
      527â535. doi:10.1090/S0002-9904-1952-09620-8.
  15. ^ Creswell, J.W. (2008), Educational research: Planning, conducting, and
      evaluating quantitative and qualitative research (3rd edition), Upper
      Saddle River, NJ: Prentice Hall. 2008, p. 300.
  16. ISBN 0-13-613550-1
  17. ^Dr. Hani (2009). "Replication_study". Retrieved 27 October 2011.
  18. ^Burman, Leonard E.; Robert W. Reed; James Alm (2010), "A_call_for
      replication_studies", Public_Finance_Review, 38 (6): 787â793, doi:
      10.1177/1091142110385210, retrieved 27 October 2011
  19. ^Jack Sifri (8 December 2014). "How_to_Use_Design_of_Experiments_to
      Create_Robust_Designs_With_High_Yield". youtube.com. Retrieved 11
      February 2015.
  20. ^Simmons, Joseph; Leif Nelson; Uri Simonsohn (November 2011). "False-
      Positive_Psychology:_Undisclosed_Flexibility_in_Data_Collection_and
      Analysis_Allows_Presenting_Anything_as_Significant". Psychological
      Science. 22 (11): 1359â1366. doi:10.1177/0956797611417632. ISSN 0956-
      7976. PMID 22006061. Retrieved 29 January 2012.
  21. ^"Science,_Trust_And_Psychology_In_Crisis". KPLU. 2 June 2014. Retrieved
      12 June 2014.
  22. ^"Why_Statistically_Significant_Studies_Can_Be_Insignificant". Pacific
      Standard. 4 June 2014. Retrieved 12 June 2014.
  23. ^Chris Chambers (10 June 2014). "Physics_envy:_Do_'hard'_sciences_hold
      the_solution_to_the_replication_crisis_in_psychology?". theguardian.com.
      Retrieved 12 June 2014.
  24. ^ Ader, Mellenberg & Hand (2008) "Advising on Research Methods: A
      consultant's companion"
  25. ^ Bisgaard, S (2008) "Must a Process be in Statistical Control before
      Conducting Designed Experiments?", Quality Engineering, ASQ, 20 (2), pp
      143 - 176
  26. ^Montgomery, Douglas (2013). Design and analysis of experiments (8th
      ed.). Hoboken, NJ: John Wiley & Sons, Inc. ISBN 9781118146927.
  27. ^ Walpole, Ronald E.; Myers, Raymond H.; Myers, Sharon L.; Ye, Keying
      (2007). Probability & statistics for engineers & scientists (8 ed.).
      Upper Saddle River, NJ: Pearson Prentice Hall. ISBN 978-0131877115.
  28. ^ Myers, Raymond H.; Montgomery, Douglas C.; Vining, G. Geoffrey;
      Robinson, Timothy J. (2010). Generalized linear models : with
      applications in engineering and the sciences (2 ed.). Hoboken, N.J.:
      Wiley. ISBN 978-0470454633.
  29. ^ Box, George E.P.; Hunter, William G.; Hunter, J. Stuart (1978).
      Statistics_for_Experimenters :_An_Introduction_to_Design,_Data_Analysis,
      and_Model_Building. New York: Wiley. ISBN 978-0-471-09315-2.
  30. ^ Box, George E.P.; Hunter, William G.; Hunter, J. Stuart (2005).
      Statistics for Experimenters : Design, Innovation, and Discovery (2 ed.).
      Hoboken, N.J.: Wiley. ISBN 978-0471718130.
  31. ^Spall, J. C. (2010). "Factorial Design for Efficient Experimentation:
      Generating Informative Data for System Identification". IEEE Control
      Systems Magazine. 30 (5): 38â53. doi:10.1109/MCS.2010.937677.
  32. ^Pronzato, L (2008). "Optimal experimental design and some related
      control problems". Automatica. 44 (2): 303â325. arXiv:0802.4381. doi:
      10.1016/j.automatica.2007.05.016.
  33. ^ Moore, David S.; Notz, William I. (2006). Statistics : concepts and
      controversies (6th ed.). New York: W.H. Freeman. pp. Chapter 7: Data
      ethics. ISBN 9780716786368.
  34. ^ Ottoboni, M. Alice (1991). The_dose_makes_the_poison :_a_plain-language
      guide_to_toxicology (2nd ed.). New York, N.Y: Van Nostrand Reinhold.
      ISBN 978-0442006600.
  35. ^Glantz, Stanton A. (1992). Primer_of_biostatistics (3rd ed.). ISBN 978-
      0-07-023511-3.
**** Sources[edit] ****
    * Peirce,_C._S. (1877â1878), "Illustrations of the Logic of Science"
      (series), Popular Science Monthly, vols. 12-13. Relevant individual
      papers:
          o (1878 March), "The Doctrine of Chances", Popular Science Monthly,
            v. 12, March issue, pp. 604â615. Internet Archive Eprint.
          o (1878 April), "The Probability of Induction", Popular Science
            Monthly, v. 12, pp. 705â718. Internet Archive Eprint.
          o (1878 June), "The Order of Nature", Popular Science Monthly, v. 13,
            pp. 203â217.Internet Archive Eprint.
          o (1878 August), "Deduction, Induction, and Hypothesis", Popular
            Science Monthly, v. 13, pp. 470â482. Internet Archive Eprint.
          o Peirce,_C._S. (1883), "A Theory of Probable Inference", Studies in
            Logic, pp. 126-181, Little, Brown, and Company. (Reprinted 1983,
            John Benjamins Publishing Company,
ISBN 90-272-3271-7)
***** External links[edit] *****
 Wikimedia Commons has media related to Design_of_experiments.
Library_resources about
Experimental design
===============================================================================
    * Resources_in_your_library
    * A chapter from a "NIST/SEMATECH_Handbook_on_Engineering_Statistics" at
      NIST
    * BoxâBehnken_designs from a "NIST/SEMATECH_Handbook_on_Engineering
      Statistics" at NIST
    * Detailed_mathematical_developments_of_most_common_DoE in the Opera
      Magistris v3.6 online reference Chapter 15, section 7.4,
ISBN 978-2-8399-0932-7.
    * v
    * t
    * e
Design of experiments
                  * Scientific_experiment
                  * Statistical design
                  * Control
                  * Internal and external validity
                  * Experimental_unit
Scientific        * Blinding
method            * Optimal_design: Bayesian
                  * Random_assignment
                  * Randomization
                  * Restricted_randomization
                  * Replication_versus_subsampling
                  * Sample_size
                  * Treatment
                  * Effect_size
                  * Contrast
Treatment         * Interaction
and blocking      * Confounding
                  * Orthogonality
                  * Blocking
                  * Covariate
                  * Nuisance_variable
                  * Linear_regression
                  * Ordinary_least_squares
                  * Bayesian
                  * Random_effect
                  * Mixed_model
Models            * Hierarchical_model: Bayesian
and inference     * Analysis_of_variance_(Anova)
                  * Cochran's_theorem
                  * Manova_(multivariate)
                  * Ancova_(covariance)
                  * Compare_means
                  * Multiple_comparison
                  * Factorial
                  * Fractional_factorial
                  * Plackett-Burman
                  * Taguchi
                  * Response_surface_methodology
                  * Polynomial_and_rational_modeling
                  * Box-Behnken
Designs           * Central_composite
                  * Block
Completely        * Generalized_randomized_block_design (GRBD)
randomized        * Latin_square
                  * Graeco-Latin_square
                  * Orthogonal_array
                  * Latin_hypercube
                    Repeated_measures_design
                  * Crossover_study
                  * Randomized_controlled_trial
                  * Sequential_analysis
                  * Sequential_probability_ratio_test
    * Glossary
    * Category
    * Statistics_portal
    * Statistical_outline
    * Statistical_topics
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
Study design               * Statistical_power
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
    * v
    * t
    * e
Clinical_research and experimental design
                     * Clinical_trial
                           o Trial_protocols
Overview                   o Adaptive_clinical_trial
                     * Academic_clinical_trials
                     * Clinical_study_design
Controlled_study     * Randomized_controlled_trial
(EBM_I_to_II-1;            o Scientific_experiment
A_to_B)                    o Blind_experiment
                           o Open-label_trial
                     * Cross-sectional_study vs. Longitudinal_study, Ecological
                       study
Observational        * Cohort_study
study                      o Retrospective
(EBM_II-2_to_II-           o Prospective
3;_B_to_C)           * Caseâcontrol_study (Nested_caseâcontrol_study)
                     * Case_series
                     * Case_study
                     * Case_report
                 Occurrence        Incidence, Cumulative_incidence, Prevalence,
                                   Point_prevalence, Period_prevalence
                                   Risk_difference, Number_needed_to_treat,
                 Association       Number_needed_to_harm, Risk_ratio, Relative
                                   risk_reduction, Odds_ratio, Hazard_ratio
                                   Attributable_fraction_among_the_exposed,
Measures         Population_impact Attributable_fraction_for_the_population,
                                   Preventable_fraction_among_the_unexposed,
                                   Preventable_fraction_for_the_population
                                   Clinical_endpoint, Virulence, Infectivity,
                                   Mortality_rate, Morbidity, Case_fatality
                 Other             rate, Specificity_and_sensitivity,
                                   Likelihood-ratios, Pre-_and_post-test
                                   probability
                     * In_vitro
                     * In_vivo
                     * Animal_testing
Trial/test types     * Animal_testing_on_non-human_primates
                     * First-in-man_study
                     * Multicenter_trial
                     * Seeding_trial
                     * Vaccine_trial
                     * Riskâbenefit_ratio
Analysis_of          * Systematic_review
clinical_trials      * Replication
                     * Meta-analysis
                     * Intention-to-treat_analysis
                     * Selection_bias
Interpretation       * Survivorship_bias
of results           * Correlation_does_not_imply_causation
                     * Null_result
    * Category
    * Glossary
    * List_of_topics
    * v
    * t
    * e
Six_Sigma tools
                  * Project_charter
Define phase      * Voice_of_the_customer
                  * Value_stream_mapping
                  * Business_process_mapping
Measure phase     * Process_capability
                  * Pareto_chart
                  * Root_cause_analysis
Analyse phase     * Failure_mode_and_effects_analysis
                  * Multi-vari_chart
Improve phase     * Design of experiments
                  * Kaizen
                  * Control_plan
Control phase     * Statistical_process_control
                  * 5S
                  * Poka-yoke
DMAIC
                                              * GND: 4078859-3
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85046441
                                              * NDL: 00574739

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Design_of_experiments&oldid=909693823"
Categories:
    * Design_of_experiments
    * Statistical_theory
    * Industrial_engineering
    * Systems_engineering
    * Statistical_process_control
    * Quantitative_research
    * Experiments
    * Metascience
Hidden categories:
    * Articles_needing_additional_references_from_September_2015
    * All_articles_needing_additional_references
    * Articles_that_may_contain_original_research_from_September_2015
    * All_articles_that_may_contain_original_research
    * Articles_with_multiple_maintenance_issues
    * Use_dmy_dates_from_July_2013
    * Articles_lacking_reliable_references_from_September_2015
    * All_articles_lacking_reliable_references
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2015
    * All_accuracy_disputes
    * Articles_with_disputed_statements_from_September_2015
    * Articles_with_unsourced_statements_from_December_2018
    * Articles_with_unsourced_statements_from_November_2011
    * Commons_category_link_from_Wikidata
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Bahasa_Indonesia
    * Nederlands
    * æ¥æ¬èª
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 00:30 (UTC).
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
