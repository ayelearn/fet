The following text has been accessed from https://en.wikipedia.org/wiki/Inference at Fri Aug 9 02:53:30 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Inference ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For the 1992 album by pianist Marilyn Crispell and saxophonist Tim Berne, see
Inference_(album).
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (April 2010)(Learn_how_and_when
 to_remove_this_template_message)
Inferences are steps in reasoning, moving from premises to logical
consequences; etymologically, the word infer means to "carry forward".
Inference is theoretically traditionally divided into deduction and induction,
a distinction that in Europe dates at least to Aristotle (300s BCE). Deduction
is inference deriving logical_conclusions from premises known or assumed to be
true, with the laws_of_valid_inference being studied in logic. Induction is
inference from particular premises to a universal conclusion. A third type of
inference is sometimes distinguished, notably by Charles_Sanders_Peirce,
distinguishing abduction from induction, where abduction is inference to the
best explanation.
Various fields study how inference is done in practice. Human inference (i.e.
how humans draw conclusions) is traditionally studied within the field of
cognitive_psychology; artificial_intelligence researchers develop automated
inference systems to emulate human inference. Statistical_inference uses
mathematics to draw conclusions in the presence of uncertainty.This generalizes
deterministic reasoning, with the absence of uncertainty as a special case.
Statistical inference uses quantitative or qualitative (categorical) data which
may be subject to random variations.
⁰
***** Contents *****
    * 1_Definition
    * 2_Examples
          o 2.1_Example_for_definition_#1
          o 2.2_Example_for_definition_#2
    * 3_Incorrect_inference
    * 4_Applications
          o 4.1_Inference_engines
                # 4.1.1_Prolog_engine
          o 4.2_Semantic_web
          o 4.3_Bayesian_statistics_and_probability_logic
          o 4.4_Fuzzy_logic
          o 4.5_Non-monotonic_logic
    * 5_See_also
    * 6_References
    * 7_Further_reading
    * 8_External_links
***** Definition[edit] *****
The process by which a conclusion is inferred from multiple observations is
called inductive_reasoning. The conclusion may be correct or incorrect, or
correct to within a certain degree of accuracy, or correct in certain
situations. Conclusions inferred from multiple observations may be tested by
additional observations.
This definition is disputable (due to its lack of clarity. Ref: Oxford English
dictionary: "induction ... 3. Logic the inference of a general law from
particular instances."[clarification_needed]) The definition given thus applies
only when the "conclusion" is general.
Two possible definitions of "inference" are:
   1. A conclusion reached on the basis of evidence and reasoning.
   2. The process of reaching such a conclusion.
***** Examples[edit] *****
**** Example for definition #1[edit] ****
Ancient_Greek_philosophers defined a number of syllogisms, correct three part
inferences, that can be used as building blocks for more complex reasoning. We
begin with a famous example:
   1. All humans are mortal.
   2. All Greeks are humans.
   3. All Greeks are mortal.
The reader can check that the premises and conclusion are true, but logic is
concerned with inference: does the truth of the conclusion follow from that of
the premises?
The validity of an inference depends on the form of the inference. That is, the
word "valid" does not refer to the truth of the premises or the conclusion, but
rather to the form of the inference. An inference can be valid even if the
parts are false, and can be invalid even if some parts are true. But a valid
form with true premises will always have a true conclusion.
For example, consider the form of the following symbological track:
   1. All meat comes from animals.
   2. All beef is meat.
   3. Therefore, all beef comes from animals.
If the premises are true, then the conclusion is necessarily true, too.
Now we turn to an invalid form.
   1. All A are B.
   2. All C are B.
   3. Therefore, all C are A.
To show that this form is invalid, we demonstrate how it can lead from true
premises to a false conclusion.
   1. All apples are fruit. (True)
   2. All bananas are fruit. (True)
   3. Therefore, all bananas are apples. (False)
A valid argument with a false premise may lead to a false conclusion, (this and
the following examples do not follow the Greek syllogism):
   1. All tall people are French. (False)
   2. John Lennon was tall. (True)
   3. Therefore, John Lennon was French. (False)
When a valid argument is used to derive a false conclusion from a false
premise, the inference is valid because it follows the form of a correct
inference.
A valid argument can also be used to derive a true conclusion from a false
premise:
   1. All tall people are musicians. (Valid, False)
   2. John Lennon was tall. (Valid, True)
   3. Therefore, John Lennon was a musician. (Valid, True)
In this case we have one false premise and one true premise where a true
conclusion has been inferred.
**** Example for definition #2[edit] ****
Evidence: It is the early 1950s and you are an American stationed in the Soviet
Union. You read in the Moscow newspaper that a soccer team from a small city in
Siberia starts winning game after game. The team even defeats the Moscow team.
Inference: The small city in Siberia is not a small city anymore. The Soviets
are working on their own nuclear or high-value secret weapons program.
Knowns: The Soviet Union is a command_economy: people and material are told
where to go and what to do. The small city was remote and historically had
never distinguished itself; its soccer season was typically short because of
the weather.
Explanation: In a command_economy, people and material are moved where they are
needed. Large cities might field good teams due to the greater availability of
high quality players; and teams that can practice longer (weather, facilities)
can reasonably be expected to be better. In addition, you put your best and
brightest in places where they can do the most goodâsuch as on high-value
weapons programs. It is an anomaly for a small city to field such a good team.
The anomaly (i.e. the soccer scores and great soccer team) indirectly described
a condition by which the observer inferred a new meaningful patternâthat the
small city was no longer small. Why would you put a large city of your best and
brightest in the middle of nowhere? To hide them, of course.
***** Incorrect inference[edit] *****
An incorrect inference is known as a fallacy. Philosophers who study informal
logic have compiled large lists of them, and cognitive psychologists have
documented many biases_in_human_reasoning that favor incorrect reasoning.
***** Applications[edit] *****
**** Inference engines[edit] ****
Main articles: Reasoning_system, Inference_engine, expert_system, and business
rule_engine
AI systems first provided automated logical inference and these were once
extremely popular research topics, leading to industrial applications under the
form of expert_systems and later business_rule_engines. More recent work on
automated_theorem_proving has had a stronger basis in formal logic.
An inference system's job is to extend a knowledge base automatically. The
knowledge base (KB) is a set of propositions that represent what the system
knows about the world. Several techniques can be used by that system to extend
KB by means of valid inferences. An additional requirement is that the
conclusions the system arrives at are relevant to its task.
*** Prolog engine[edit] ***
Prolog (for "Programming in Logic") is a programming_language based on a subset
of predicate_calculus. Its main job is to check whether a certain proposition
can be inferred from a KB (knowledge base) using an algorithm called backward
chaining.
Let us return to our Socrates syllogism. We enter into our Knowledge Base the
following piece of code:
mortal(X) :- 	man(X).
man(socrates).
( Here :- can be read as "if". Generally, if P     &#x2192;   {\displaystyle
\to }  [\to ] Q (if P then Q) then in Prolog we would code Q:-P (Q if P).)
This states that all men are mortal and that Socrates is a man. Now we can ask
the Prolog system about Socrates:
?- mortal(socrates).
(where ?- signifies a query: Can mortal(socrates). be deduced from the KB using
the rules) gives the answer "Yes".
On the other hand, asking the Prolog system the following:
?- mortal(plato).
gives the answer "No".
This is because Prolog does not know anything about Plato, and hence defaults
to any property about Plato being false (the so-called closed_world
assumption). Finally ?- mortal(X) (Is anything mortal) would result in "Yes"
(and in some implementations: "Yes": X=socrates)
Prolog can be used for vastly more complicated inference tasks. See the
corresponding article for further examples.
**** Semantic web[edit] ****
Recently automatic reasoners found in semantic_web a new field of application.
Being based upon description_logic, knowledge expressed using one variant of
OWL can be logically processed, i.e., inferences can be made upon it.
**** Bayesian statistics and probability logic[edit] ****
Main article: Bayesian_inference
Philosophers and scientists who follow the Bayesian_framework for inference use
the mathematical rules of probability to find this best explanation. The
Bayesian view has a number of desirable featuresâone of them is that it
embeds deductive (certain) logic as a subset (this prompts some writers to call
Bayesian probability "probability logic", following E._T._Jaynes).
Bayesians identify probabilities with degrees of beliefs, with certainly true
propositions having probability 1, and certainly false propositions having
probability 0. To say that "it's going to rain tomorrow" has a 0.9 probability
is to say that you consider the possibility of rain tomorrow as extremely
likely.
Through the rules of probability, the probability of a conclusion and of
alternatives can be calculated. The best explanation is most often identified
with the most probable (see Bayesian_decision_theory). A central rule of
Bayesian inference is Bayes'_theorem.
**** Fuzzy logic[edit] ****
Main article: Fuzzy_logic
[[icon]] This section needs expansion. You can help by adding_to_it. (October
         2016)
**** Non-monotonic logic[edit] ****
Main article: Non-monotonic_logic
[1]
A relation of inference is monotonic if the addition of premises does not
undermine previously reached conclusions; otherwise the relation is non-
monotonic. Deductive inference is monotonic: if a conclusion is reached on the
basis of a certain set of premises, then that conclusion still holds if more
premises are added.
By contrast, everyday reasoning is mostly non-monotonic because it involves
risk: we jump to conclusions from deductively insufficient premises. We know
when it is worth or even necessary (e.g. in medical diagnosis) to take the
risk. Yet we are also aware that such inference is defeasibleâthat new
information may undermine old conclusions. Various kinds of defeasible but
remarkably successful inference have traditionally captured the attention of
philosophers (theories of induction, Peirce's theory of abduction, inference to
the best explanation, etc.). More recently logicians have begun to approach the
phenomenon from a formal point of view. The result is a large body of theories
at the interface of philosophy, logic and artificial intelligence.
***** See also[edit] *****
    * A_priori_and_a_posteriori
    * Abductive_reasoning
    * Deductive_reasoning
          o Inductive_reasoning
    * Entailment
    * Epilogism
    * Analogy
    * Axiom_system
          o Axiom
    * Immediate_inference
    * Inferential_programming
    * Inquiry
    * Logic
    * Logic_of_information
    * Logical_assertion
    * Logical_graph
    * Rule_of_inference
    * List_of_rules_of_inference
    * Theorem
    * Transduction_(machine_learning)
    * [icon]Logic_portal
    * [icon]Thinking_portal
***** References[edit] *****
   1. ^Fuhrmann, AndrÃ©. Nonmonotonic_Logic (PDF). Archived from the_original
      (PDF) on 9 December 2003.
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
***** Further reading[edit] *****
    * Hacking, Ian (2011). An Introduction to Probability and Inductive Logic.
      Cambridge University Press. ISBN 978-0-521-77501-4.
Jaynes, Edwin Thompson (2003). Probability_Theory:_The_Logic_of_Science.
Cambridge University Press. ISBN 978-0-521-59271-0.
McKay,_David_J.C. (2003). Information_Theory,_Inference,_and_Learning
Algorithms. Cambridge University Press. ISBN 978-0-521-64298-9.
Russell,_Stuart_J.; Norvig,_Peter (2003), Artificial_Intelligence:_A_Modern
Approach (2nd ed.), Upper Saddle River, New Jersey: Prentice Hall, ISBN 0-13-
790395-2
Tijms,_Henk (2004). Understanding Probability. Cambridge University Press.
ISBN 978-0-521-70172-3.
Inductive inference:
    * Carnap, Rudolf; Jeffrey, Richard C., eds. (1971). Studies in Inductive
      Logic and Probability. 1. The University of California Press.
Jeffrey, Richard C., ed. (1980). Studies_in_Inductive_Logic_and_Probability. 2.
The University of California Press. ISBN 9780520038264.
Angluin, Dana (1976). An Application of the Theory of Computational Complexity
to the Study of Inductive Inference (Ph.D.). University of California at
Berkeley.
Angluin, Dana (1980). "Inductive_Inference_of_Formal_Languages_from_Positive
Data" (PDF). Information and Control. 45 (2): 117â135. doi:10.1016/s0019-9958
(80)90285-5.
Angluin, Dana; Smith, Carl H. (Sep 1983). "Inductive_Inference:_Theory_and
Methods" (PDF). Computing Surveys. 15 (3): 237â269. doi:10.1145/
356914.356918.
Gabbay, Dov M.; Hartmann, Stephan; Woods, John, eds. (2009). Inductive Logic.
Handbook of the History of Logic. 10. Elsevier.
Goodman, Nelson (1983). Fact,_Fiction,_and_Forecast. Harvard University Press.
ISBN 9780674290716.
Abductive inference:
    * O'Rourke, P.; Josephson, J., eds. (1997). Automated abduction: Inference
      to the best explanation. AAAI Press.
Psillos, Stathis (2009). Gabbay, Dov M.; Hartmann, Stephan; Woods, John (eds.).
An_Explorer_upon_Untrodden_Ground:_Peirce_on_Abduction (PDF). Handbook of the
History of Logic. 10. Elsevier. pp. 117â152.
Ray, Oliver (Dec 2005). Hybrid_Abductive_Inductive_Learning (Ph.D.). University
of London, Imperial College. CiteSeerX 10.1.1.66.1877.
Psychological investigations about human reasoning:
    * deductive:
          o Johnson-Laird,_Philip_Nicholas; Byrne, Ruth M. J. (1992).
            Deduction. Erlbaum.
Byrne, Ruth M. J.; Johnson-Laird,_P._N. (2009). ""If"_and_the_Problems_of
Conditional_Reasoning" (PDF). Trends in Cognitive Sciences. 13 (7): 282â287.
doi:10.1016/j.tics.2009.04.003. Archived from the_original (PDF) on 2014-04-07.
Retrieved 2013-08-09.
Knauff, Markus; Fangmeier, Thomas; Ruff, Christian C.; Johnson-Laird,_P._N.
(2003). "Reasoning,_Models,_and_Images:_Behavioral_Measures_and_Cortical
Activity" (PDF). Journal of Cognitive Neuroscience. 15 (4): 559â573.
CiteSeerX 10.1.1.318.6615. doi:10.1162/089892903321662949. PMID 12803967.
Johnson-Laird,_Philip_N. (1995). Gazzaniga, M. S. (ed.). Mental_Models,
Deductive_Reasoning,_and_the_Brain (PDF). MIT Press. pp. 999â1008.
Khemlani, Sangeet; Johnson-Laird,_P._N. (2008). "Illusory_Inferences_about
Embedded_Disjunctions" (PDF). Proceedings of the 30th Annual Conference of the
Cognitive Science Society. Washington/DC. pp. 2128â2133.
statistical:
    * McCloy, Rachel; Byrne, Ruth M. J.; Johnson-Laird,_Philip_N. (2009).
      "Understanding_Cumulative_Risk" (PDF). The Quarterly Journal of
      Experimental Psychology. 63 (3): 499â515. doi:10.1080/
      17470210903024784. Archived from the_original (PDF) on 2015-05-18.
      Retrieved 2013-08-09.
Johnson-Laird,_Philip_N. (1994). "Mental_Models_and_Probabilistic_Thinking"
(PDF). Cognition. 50 (1â3): 189â209. doi:10.1016/0010-0277(94)90028-0.
,
analogical:
    * Burns, B. D. (1996). "Meta-Analogical Transfer: Transfer Between Episodes
      of Analogical Reasoning". Journal of Experimental Psychology: Learning,
      Memory, and Cognition. 22 (4): 1032â1048. doi:10.1037/0278-
      7393.22.4.1032.
spatial:
    * Jahn, Georg; Knauff, Markus; Johnson-Laird,_P._N. (2007). "Preferred
      mental_models_in_reasoning_about_spatial_relations" (PDF). Memory &
      Cognition. 35 (8): 2075â2087. doi:10.3758/bf03192939.
Knauff, Markus; Johnson-Laird,_P._N. (2002). "Visual_imagery_can_impede
reasoning" (PDF). Memory & Cognition. 30 (3): 363â371. doi:10.3758/
bf03194937.
Waltz, James A.; Knowlton, Barbara J.; Holyoak, Keith J.; Boone, Kyle B.;
Mishkin, Fred S.; de Menezes Santos, Marcia; Thomas, Carmen R.; Miller, Bruce
L. (Mar 1999). "A_System_for_Relational_Reasoning_in_Human_Prefrontal_Cortex".
Psychological Science. 10 (2): 119â125. doi:10.1111/1467-9280.00118.
moral:
    * Bucciarelli, Monica; Khemlani, Sangeet; Johnson-Laird,_P._N. (Feb 2008).
      "The_Psychology_of_Moral_Reasoning" (PDF). Judgment and Decision Making.
      3 (2): 121â139.
***** External links[edit] *****
 Look up inference or infer in Wiktionary, the free dictionary.
    * Inference at PhilPapers
    * Inference_example_and_definition
    * Inference at the Indiana_Philosophy_Ontology_Project
    * v
    * t
    * e
Logic
    * Outline
    * History
                * Computer_science
                * Inference
                * Philosophy_of_logic
                * Proof
                * Semantics
                * Syntax
                         * Classical
                         * Informal
Fields                         o Critical_thinking
            Logics             o Reason
                         * Mathematical
                         * Non-classical
                         * Philosophical
                         * Argumentation
            Theories     * Metalogic
                         * Metamathematics
                         * Set
                * Abduction
                * Analytic_and_synthetic_propositions
                * Contradiction
                      o Paradox
                      o Antinomy
                * Deduction
                * Deductive_closure
                * Definition
                * Description
                * Entailment
Foundations           o Linguistic
                * Form
                * Induction
                * Logical_truth
                * Name
                * Necessity_and_sufficiency
                * Probability
                * Reference
                * Statement
                * Substitution
                * Truth
                * Validity
                       * Mathematical_logic
            topics     * Boolean_algebra
                       * Set_theory
Lists                  * Logicians
                       * Rules_of_inference
            other      * Paradoxes
                       * Fallacies
                       * Logic_symbols
    * Portal
    * Category
    * WikiProject (talk)
    * changes
    * v
    * t
    * e
Philosophy
Branches
                  * Metaphysics
                        o Ontology
Traditional       * Epistemology
                  * Logic
                  * Ethics
                  * Aesthetics
                  * Action
                  * Art
                        o Culture
                        o Design
                        o Music
                        o Film
                  * Business
                  * Color
                  * Cosmos
                  * Dialogue
                  * Education
                  * Environment
                  * Futility
                  * Happiness
                  * Healthcare
                  * History
                  * Human_nature
                  * Humor
                  * Feminism
                  * Language
                  * Life
                  * Literature
                  * Mathematics
                  * Mind
                        o Pain
Philosophy of           o Psychology
                  * Philosophy_of_psychiatry
                  * Philosophy_of_perception
                  * Philosophy
                  * Religion
                  * Science
                        o Physics
                        o Chemistry
                        o Biology
                        o Geography
                  * Sexuality
                  * Social_science
                        o Culture
                        o Economics
                        o Justice
                        o Law
                        o Politics
                        o Society
                  * Space_and_time
                  * Sport
                  * Technology
                        o Artificial_intelligence
                        o Computer_science
                        o Engineering
                        o Information
                  * War
Schools_of_thought
                 * Ancient
                 * Western
                       o Medieval
By_era                 o Renaissance
                       o Early_modern
                       o Modern
                       o Contemporary
                             * Agriculturalism
                             * Confucianism
                             * Legalism
                             * Logicians
             Chinese         * Mohism
                             * Chinese_naturalism
                             * Neotaoism
                             * Taoism
                             * Yangism
                             * Zen
                             * Aristotelianism
                             * Atomism
                             * Cynicism
                             * Cyrenaics
                             * Eleatics
                             * Eretrian_school
                             * Epicureanism
                             * Hermeneutics
                             * Ionian
                                   o Ephesian
             Greco-Roman           o Milesian
                             * Megarian_school
                             * Neoplatonism
                             * Peripatetic
                             * Platonism
                             * Pluralism
Ancient                      * Presocratic
                             * Pyrrhonism
                             * Pythagoreanism
                             * Neopythagoreanism
                             * Sophistic
                             * Stoicism
                             * Hindu
                             * Samkhya
                             * Nyaya
                             * Vaisheshika
                             * Yoga
                             * MÄ«mÄá¹sÄ
                             * ÄjÄ«vika
                             * AjÃ±ana
             Indian          * CÄrvÄka
                             * Jain
                                   o Anekantavada
                                   o SyÄdvÄda
                             * Buddhist
                                   o ÅÅ«nyatÄ
                                   o Madhyamaka
                                   o Yogacara
                                   o SautrÄntika
                                   o Svatantrika
                             * Mazdakism
             Persian         * Zoroastrianism
                             * Zurvanism
                            * Christian
                            * Augustinianism
                        Scholasticism
             European   Thomism
                        Scotism
                        Occamism
                        Renaissance_humanism
                            * Korean_Confucianism
             East Asian     * Edo_neo-Confucianism
                            * Neo-Confucianism
                            * Vedanta
                                  o Acintya_bheda_abheda
Medieval                          o Advaita
                                  o Bhedabheda
             Indian               o Dvaita
                                  o Nimbarka_Sampradaya
                                  o Shuddhadvaita
                                  o Vishishtadvaita
                            * Navya-NyÄya
                            * Averroism
                            * Avicennism
             Islamic        * Illuminationism
                            * Ê¿Ilm_al-KalÄm
                            * Sufi
             Jewish         * Judeo-Islamic
                        * Cartesianism
                        * Kantianism
             People     * Neo-Kantianism
                        * Hegelianism
                        * Marxism
                        * Spinozism
                        * Anarchism
                        * Classical_Realism
                        * Liberalism
                        * Collectivism
                        * Conservatism
                        * Determinism
                        * Dualism
                        * Empiricism
                        * Existentialism
                        * Foundationalism
                        * Historicism
                        * Holism
                        * Humanism
                              o Anti-
                        * Idealism
                              o Absolute
Modern                        o British
                              o German
                              o Objective
             0                o Subjective
                              o Transcendental
                        * Individualism
                        * Kokugaku
                        * Materialism
                        * Modernism
                        * Monism
                        * Naturalism
                        * Natural_law
                        * Nihilism
                        * New_Confucianism
                        * Neo-scholasticism
                        * Pragmatism
                        * Phenomenology
                        * Positivism
                        * Reductionism
                        * Rationalism
                        * Social_contract
                        * Socialism
                        * Transcendentalism
                        * Utilitarianism
                             * Applied_ethics
                             * Analytic_feminism
                             * Analytical_Marxism
                             * Communitarianism
                             * Consequentialism
                             * Critical_rationalism
                             * Experimental_philosophy
                             * Falsificationism
                             * Foundationalism / Coherentism
                             * Generative_linguistics
                             * Internalism_and_Externalism
                             * Logical_positivism
                             * Legal_positivism
                             * Normative_ethics
             Analytic        * Meta-ethics
                             * Moral_realism
                             * Quinean_naturalism
                             * Ordinary_language_philosophy
                             * Postanalytic_philosophy
                             * Quietism
                             * Rawlsian
                             * Reformed_epistemology
                             * Systemics
                             * Scientism
Contemporary                 * Scientific_realism
                             * Scientific_skepticism
                             * Transactionalism
                             * Contemporary_utilitarianism
                             * Vienna_Circle
                             * Wittgensteinian
                             * Critical_theory
                             * Deconstruction
                             * Existentialism
                             * Feminist
                             * Frankfurt_School
                             * New_Historicism
                             * Hermeneutics
             Continental     * Neo-Marxism
                             * Phenomenology
                             * Posthumanism
                             * Postmodernism
                             * Post-structuralism
                             * Social_constructionism
                             * Structuralism
                             * Western_Marxism
                             * Kyoto_School
                             * Objectivism
             Other           * Postcritique
                             * Russian_cosmism
                             * more...
Positions
                 * Formalism
Aesthetics       * Institutionalism
                 * Aesthetic_response
                 * Consequentialism
Ethics           * Deontology
                 * Virtue
                 * Compatibilism
                 * Determinism
Free_will              o Hard
                 * Incompatibilism
                       o Hard
                 * Libertarianism
                 * Atomism
Metaphysics      * Dualism
                 * Monism
                 * Naturalism
                 * Constructivism
                 * Empiricism
                 * Idealism
Epistemology     * Particularism
                 * Fideism
                 * Rationalism / Reasonism
                 * Skepticism
                 * Solipsism
                 * Behaviorism
                 * Emergentism
                 * Eliminativism
Mind             * Epiphenomenalism
                 * Functionalism
                 * Objectivism
                 * Subjectivism
                 * Absolutism
                 * Particularism
Normativity      * Relativism
                 * Nihilism
                 * Skepticism
                 * Universalism
                 * Action
Ontology         * Event
                 * Process
                 * Anti-realism
                 * Conceptualism
                 * Idealism
Reality          * Materialism
                 * Naturalism
                 * Nominalism
                 * Physicalism
                 * Realism
    * By region
    * Related lists
    * Miscellaneous
                  * African
                  * Ethiopian
                  * Amerindian
                  * Aztec
                  * Eastern
                  * Chinese
                  * Egyptian
                  * Indian
                  * Indonesian
                  * Iranian
                  * Japanese
                  * Korean
                  * Pakistani
                  * Vietnamese
By region         * Western
                  * American
                  * Australian
                  * British
                  * Czech
                  * Danish
                  * French
                  * German
                  * Greek
                  * Italian
                  * Polish
                  * Romanian
                  * Russian
                  * Slovene
                  * Spanish
                  * Turkish
                  * Outline
                  * Index
                  * Years
                  * Problems
Lists             * Schools
                  * Glossary
                  * Philosophers
                  * Movements
                  * Publications
                  * Natural_law
Miscellaneous     * Women_in_philosophy
                  * Sage_(philosophy)
    * [Portal] Portal
    * [Category] Category
    * [Wikipedia book] Book
                                              * BNF: cb11935348h (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4139983-3
                                              * LCCN: sh85066082
                                              * NDL: 00571577

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Inference&oldid=909609733"
Categories:
    * Logic_and_statistics
    * Sources_of_knowledge
    * Reasoning
    * Concepts_in_logic
    * Logical_consequence
Hidden categories:
    * Articles_lacking_in-text_citations_from_April_2010
    * All_articles_lacking_in-text_citations
    * Wikipedia_articles_needing_clarification_from_August_2013
    * Articles_to_be_expanded_from_October_2016
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
    * Wikipedia_articles_with_BNF_identifiers
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
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Italiano
    * ×¢××¨××ª
    * La_.lojban.
    * Nederlands
    * æ¥æ¬èª
    * à¨ªà©°à¨à¨¾à¨¬à©
    * PlattdÃ¼Ã¼tsch
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 6 August 2019, at 13:32 (UTC).
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
