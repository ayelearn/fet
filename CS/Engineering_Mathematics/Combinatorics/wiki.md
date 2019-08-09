The following text has been accessed from https://en.wikipedia.org/wiki/Combinatorics at Fri Aug 9 01:08:48 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Combinatorics ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with Combinatoriality.
Combinatorics is an area of mathematics primarily concerned with counting, both
as a means and an end in obtaining results, and certain properties of finite
structures. It is closely related to many other areas of mathematics and has
many applications ranging from logic to statistical_physics, from evolutionary
biology to computer_science, etc.
To fully understand the scope of combinatorics requires a great deal of further
amplification, the details of which are not universally agreed upon.[1]
According to H.J._Ryser, a definition of the subject is difficult because it
crosses so many mathematical subdivisions.[2] Insofar as an area can be
described by the types of problems it addresses, combinatorics is involved with
    * the enumeration (counting) of specified structures, sometimes referred to
      as arrangements or configurations in a very general sense, associated
      with finite systems,
    * the existence of such structures that satisfy certain given criteria,
    * the construction of these structures, perhaps in many ways, and
    * optimization, finding the "best" structure or solution among several
      possibilities, be it the "largest", "smallest" or satisfying some other
      optimality criterion.
Leon_Mirsky has said: "combinatorics is a range of linked studies which have
something in common and yet diverge widely in their objectives, their methods,
and the degree of coherence they have attained."[3] One way to define
combinatorics is, perhaps, to describe its subdivisions with their problems and
techniques. This is the approach that is used below. However, there are also
purely historical reasons for including or not including some topics under the
combinatorics umbrella.[4] Although primarily concerned with finite systems,
some combinatorial questions and techniques can be extended to an infinite
(specifically, countable) but discrete setting.
Combinatorics is well known for the breadth of the problems it tackles.
Combinatorial problems arise in many areas of pure_mathematics, notably in
algebra, probability_theory, topology, and geometry,[5] as well as in its many
application areas. Many combinatorial questions have historically been
considered in isolation, giving an ad hoc solution to a problem arising in some
mathematical context. In the later twentieth century, however, powerful and
general theoretical methods were developed, making combinatorics into an
independent branch of mathematics in its own right.[6] One of the oldest and
most accessible parts of combinatorics is graph_theory, which by itself has
numerous natural connections to other areas. Combinatorics is used frequently
in computer science to obtain formulas and estimates in the analysis_of
algorithms.
A mathematician who studies combinatorics is called a combinatorialist.
⁰
***** Contents *****
    * 1_History
    * 2_Approaches_and_subfields_of_combinatorics
          o 2.1_Enumerative_combinatorics
          o 2.2_Analytic_combinatorics
          o 2.3_Partition_theory
          o 2.4_Graph_theory
          o 2.5_Design_theory
          o 2.6_Finite_geometry
          o 2.7_Order_theory
          o 2.8_Matroid_theory
          o 2.9_Extremal_combinatorics
          o 2.10_Probabilistic_combinatorics
          o 2.11_Algebraic_combinatorics
          o 2.12_Combinatorics_on_words
          o 2.13_Geometric_combinatorics
          o 2.14_Topological_combinatorics
          o 2.15_Arithmetic_combinatorics
          o 2.16_Infinitary_combinatorics
    * 3_Related_fields
          o 3.1_Combinatorial_optimization
          o 3.2_Coding_theory
          o 3.3_Discrete_and_computational_geometry
          o 3.4_Combinatorics_and_dynamical_systems
          o 3.5_Combinatorics_and_physics
    * 4_See_also
    * 5_Notes
    * 6_References
    * 7_External_links
***** History[edit] *****
An example of change_ringing (with six bells), one of the earliest nontrivial
results in graph_theory.
Main article: History_of_combinatorics
Basic combinatorial concepts and enumerative results appeared throughout the
ancient_world. In the 6th century BCE, ancient_Indian physician Sushruta
asserts in Sushruta_Samhita that 63 combinations can be made out of 6 different
tastes, taken one at a time, two at a time, etc., thus computing all 26 â 1
possibilities. Greek historian Plutarch discusses an argument between
Chrysippus (3rd century BCE) and Hipparchus (2nd century BCE) of a rather
delicate enumerative problem, which was later shown to be related to
SchrÃ¶derâHipparchus_numbers.[7][8] In the Ostomachion, Archimedes (3rd
century BCE) considers a tiling_puzzle.
In the Middle_Ages, combinatorics continued to be studied, largely outside of
the European_civilization. The Indian mathematician MahÄvÄ«ra (c. 850)
provided formulae for the number of permutations and combinations,[9][10] and
these formulas may have been familiar to Indian mathematicians as early as the
6th century CE.[11] The philosopher and astronomer Rabbi Abraham_ibn_Ezra (c.
1140) established the symmetry of binomial_coefficients, while a closed formula
was obtained later by the talmudist and mathematician Levi_ben_Gerson (better
known as Gersonides), in 1321.[12] The arithmetical triangleâ a graphical
diagram showing relationships among the binomial coefficientsâ was presented
by mathematicians in treatises dating as far back as the 10th century, and
would eventually become known as Pascal's_triangle. Later, in Medieval_England,
campanology provided examples of what is now known as Hamiltonian_cycles in
certain Cayley_graphs on permutations.[13]
During the Renaissance, together with the rest of mathematics and the sciences,
combinatorics enjoyed a rebirth. Works of Pascal, Newton, Jacob_Bernoulli and
Euler became foundational in the emerging field. In modern times, the works of
J.J._Sylvester (late 19th century) and Percy_MacMahon (early 20th century)
helped lay the foundation for enumerative and algebraic_combinatorics. Graph
theory also enjoyed an explosion of interest at the same time, especially in
connection with the four_color_problem.
In the second half of the 20th century, combinatorics enjoyed a rapid growth,
which led to establishment of dozens of new journals and conferences in the
subject.[14] In part, the growth was spurred by new connections and
applications to other fields, ranging from algebra to probability, from
functional_analysis to number_theory, etc. These connections shed the
boundaries between combinatorics and parts of mathematics and theoretical
computer science, but at the same time led to a partial fragmentation of the
field.
***** Approaches and subfields of combinatorics[edit] *****
**** Enumerative combinatorics[edit] ****
Five binary_trees on three vertices, an example of Catalan_numbers.
Main article: Enumerative_combinatorics
Enumerative combinatorics is the most classical area of combinatorics and
concentrates on counting the number of certain combinatorial objects. Although
counting the number of elements in a set is a rather broad mathematical
problem, many of the problems that arise in applications have a relatively
simple combinatorial description. Fibonacci_numbers is the basic example of a
problem in enumerative combinatorics. The twelvefold_way provides a unified
framework for counting permutations, combinations and partitions.
**** Analytic combinatorics[edit] ****
Main article: Analytic_combinatorics
Analytic_combinatorics concerns the enumeration of combinatorial structures
using tools from complex_analysis and probability_theory. In contrast with
enumerative combinatorics, which uses explicit combinatorial formulae and
generating_functions to describe the results, analytic combinatorics aims at
obtaining asymptotic_formulae.
**** Partition theory[edit] ****
A plane_partition.
Main article: Partition_theory
Partition theory studies various enumeration and asymptotic problems related to
integer_partitions, and is closely related to q-series, special_functions and
orthogonal_polynomials. Originally a part of number_theory and analysis, it is
now considered a part of combinatorics or an independent field. It incorporates
the bijective_approach and various tools in analysis and analytic_number
theory, and has connections with statistical_mechanics.
**** Graph theory[edit] ****
Petersen_graph.
Main article: Graph_theory
Graphs are basic objects in combinatorics. The questions range from counting
(e.g., the number of graphs on n vertices with k edges) to structural (e.g.,
which graphs contain Hamiltonian cycles) to algebraic questions (e.g., given a
graph G and two numbers x and y, does the Tutte_polynomial TG(x,y) have a
combinatorial interpretation?). Although there are very strong connections
between graph theory and combinatorics, these two are sometimes thought of as
separate subjects.[15] This is due to the fact that while combinatorial methods
apply to many graph theory problems, the two are generally used to seek
solutions to different problems.
**** Design theory[edit] ****
Main article: Combinatorial_design
Design theory is a study of combinatorial_designs, which are collections of
subsets with certain intersection properties. Block_designs are combinatorial
designs of a special type. This area is one of the oldest parts of
combinatorics, such as in Kirkman's_schoolgirl_problem proposed in 1850. The
solution of the problem is a special case of a Steiner_system, which systems
play an important role in the classification_of_finite_simple_groups. The area
has further connections to coding_theory and geometric combinatorics.
**** Finite geometry[edit] ****
Main article: Finite_geometry
Finite geometry is the study of geometric_systems having only a finite number
of points. Structures analogous to those found in continuous geometries
(Euclidean_plane, real_projective_space, etc.) but defined combinatorially are
the main items studied. This area provides a rich source of examples for design
theory. It should not be confused with discrete geometry (combinatorial
geometry).
**** Order theory[edit] ****
Hasse_diagram of the powerset of {x,y,z} ordered by inclusion.
Main article: Order_theory
Order theory is the study of partially_ordered_sets, both finite and infinite.
Various examples of partial orders appear in algebra, geometry, number theory
and throughout combinatorics and graph theory. Notable classes and examples of
partial orders include lattices and Boolean_algebras.
**** Matroid theory[edit] ****
Main article: Matroid_theory
Matroid theory abstracts part of geometry. It studies the properties of sets
(usually, finite sets) of vectors in a vector_space that do not depend on the
particular coefficients in a linear_dependence relation. Not only the structure
but also enumerative properties belong to matroid theory. Matroid theory was
introduced by Hassler_Whitney and studied as a part of order theory. It is now
an independent field of study with a number of connections with other parts of
combinatorics.
**** Extremal combinatorics[edit] ****
Main article: Extremal_combinatorics
Extremal combinatorics studies extremal questions on set_systems. The types of
questions addressed in this case are about the largest possible graph which
satisfies certain properties. For example, the largest triangle-free_graph on
2n vertices is a complete_bipartite_graph Kn,n. Often it is too hard even to
find the extremal answer f(n) exactly and one can only give an asymptotic
estimate.
Ramsey_theory is another part of extremal combinatorics. It states that any
sufficiently_large configuration will contain some sort of order. It is an
advanced generalization of the pigeonhole_principle.
**** Probabilistic combinatorics[edit] ****
Self-avoiding_walk in a square_grid_graph.
Main article: Probabilistic_method
In probabilistic combinatorics, the questions are of the following type: what
is the probability of a certain property for a random discrete object, such as
a random_graph? For instance, what is the average number of triangles in a
random graph? Probabilistic methods are also used to determine the existence of
combinatorial objects with certain prescribed properties (for which explicit
examples might be difficult to find), simply by observing that the probability
of randomly selecting an object with those properties is greater than 0. This
approach (often referred to as the probabilistic_method) proved highly
effective in applications to extremal combinatorics and graph theory. A closely
related area is the study of finite Markov_chains, especially on combinatorial
objects. Here again probabilistic tools are used to estimate the mixing_time.
Often associated with Paul_ErdÅs, who did the pioneering work on the subject,
probabilistic combinatorics was traditionally viewed as a set of tools to study
problems in other parts of combinatorics. However, with the growth of
applications to analysis_of_algorithms in computer_science, as well as
classical probability, additive and probabilistic_number_theory, the area
recently grew to become an independent field of combinatorics.
**** Algebraic combinatorics[edit] ****
Young_diagram of a partition (5,4,1).
Main article: Algebraic_combinatorics
Algebraic combinatorics is an area of mathematics that employs methods of
abstract_algebra, notably group_theory and representation_theory, in various
combinatorial contexts and, conversely, applies combinatorial techniques to
problems in algebra. Algebraic combinatorics is continuously expanding its
scope, in both topics and techniques, and can be seen as the area of
mathematics where the interaction of combinatorial and algebraic methods is
particularly strong and significant.
**** Combinatorics on words[edit] ****
Construction of a ThueâMorse_infinite_word.
Main article: Combinatorics_on_words
Combinatorics on words deals with formal_languages. It arose independently
within several branches of mathematics, including number_theory, group_theory
and probability. It has applications to enumerative combinatorics, fractal
analysis, theoretical_computer_science, automata_theory and linguistics. While
many applications are new, the classical ChomskyâSchÃ¼tzenberger_hierarchy of
classes of formal_grammars is perhaps the best-known result in the field.
**** Geometric combinatorics[edit] ****
An icosahedron.
Main article: Geometric_combinatorics
Geometric combinatorics is related to convex and discrete_geometry, in
particular polyhedral_combinatorics. It asks, for example, how many faces of
each dimension a convex_polytope can have. Metric properties of polytopes play
an important role as well, e.g. the Cauchy_theorem on the rigidity of convex
polytopes. Special polytopes are also considered, such as permutohedra,
associahedra and Birkhoff_polytopes. We should note that combinatorial_geometry
is an old fashioned name for discrete geometry.
**** Topological combinatorics[edit] ****
Splitting_a_necklace with two cuts.
Main article: Topological_combinatorics
Combinatorial analogs of concepts and methods in topology are used to study
graph_coloring, fair_division, partitions, partially_ordered_sets, decision
trees, necklace_problems and discrete_Morse_theory. It should not be confused
with combinatorial_topology which is an older name for algebraic_topology.
**** Arithmetic combinatorics[edit] ****
Main article: Arithmetic_combinatorics
Arithmetic combinatorics arose out of the interplay between number_theory,
combinatorics, ergodic_theory and harmonic_analysis. It is about combinatorial
estimates associated with arithmetic operations (addition, subtraction,
multiplication, and division). Additive_number_theory (sometimes also called
additive combinatorics) refers to the special case when only the operations of
addition and subtraction are involved. One important technique in arithmetic
combinatorics is the ergodic_theory of dynamical_systems.
**** Infinitary combinatorics[edit] ****
Main article: Infinitary_combinatorics
Infinitary combinatorics, or combinatorial set theory, is an extension of ideas
in combinatorics to infinite sets. It is a part of set_theory, an area of
mathematical_logic, but uses tools and ideas from both set theory and extremal
combinatorics.
Gian-Carlo_Rota used the name continuous combinatorics[16] to describe
geometric_probability, since there are many analogies between counting and
measure.
***** Related fields[edit] *****
Kissing_spheres are connected to both coding_theory and discrete_geometry.
**** Combinatorial optimization[edit] ****
Combinatorial_optimization is the study of optimization on discrete and
combinatorial objects. It started as a part of combinatorics and graph theory,
but is now viewed as a branch of applied mathematics and computer science,
related to operations_research, algorithm_theory and computational_complexity
theory.
**** Coding theory[edit] ****
Coding_theory started as a part of design theory with early combinatorial
constructions of error-correcting_codes. The main idea of the subject is to
design efficient and reliable methods of data transmission. It is now a large
field of study, part of information_theory.
**** Discrete and computational geometry[edit] ****
Discrete_geometry (also called combinatorial geometry) also began as a part of
combinatorics, with early results on convex_polytopes and kissing_numbers. With
the emergence of applications of discrete geometry to computational_geometry,
these two fields partially merged and became a separate field of study. There
remain many connections with geometric and topological combinatorics, which
themselves can be viewed as outgrowths of the early discrete geometry.
**** Combinatorics and dynamical systems[edit] ****
Combinatorial_aspects_of_dynamical_systems is another emerging field. Here
dynamical systems can be defined on combinatorial objects. See for example
graph_dynamical_system.
**** Combinatorics and physics[edit] ****
There are increasing interactions between combinatorics_and_physics,
particularly statistical_physics. Examples include an exact solution of the
Ising_model, and a connection between the Potts_model on one hand, and the
chromatic and Tutte_polynomials on the other hand.
***** See also[edit] *****
    * [icon]Discrete_mathematics_portal
    * Combinatorial_biology
    * Combinatorial_chemistry
    * Combinatorial_data_analysis
    * Combinatorial_game_theory
    * Combinatorial_group_theory
    * List_of_combinatorics_topics
    * Phylogenetics
***** Notes[edit] *****
   1. ^Pak, Igor. "What_is_Combinatorics?". Retrieved 1 November 2017.
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
   3. ^ Ryser_1963, p. 2
   4. ^Mirsky, Leon (1979), "Book_Review" (PDF), Bulletin (New Series) of the
      American Mathematical Society, 1: 380â388
   5. ^Rota, Gian Carlo (1969). Discrete Thoughts. BirkhaÃ¼ser. p. 50. ...
      combinatorial theory has been the mother of several of the more active
      branches of today's mathematics, which have become independent ... . The
      typical ... case of this is algebraic topology (formerly known as
      combinatorial topology)
   6. ^ BjÃ¶rner and Stanley, p. 2
   7. ^LovÃ¡sz, LÃ¡szlÃ³ (1979). Combinatorial_Problems_and_Exercises. North-
      Holland. In my opinion, combinatorics is now growing out of this early
      stage.
   8. ^ Stanley,_Richard_P.; "Hipparchus, Plutarch, SchrÃ¶der, and Hough",
      American Mathematical Monthly 104 (1997), no. 4, 344â350.
   9. ^ Habsieger, Laurent; Kazarian, Maxim; and Lando, Sergei; "On_the_Second
      Number_of_Plutarch", American Mathematical Monthly 105 (1998), no. 5,
      446.
  10. ^O'Connor,_John_J.; Robertson,_Edmund_F., "Combinatorics", MacTutor
      History_of_Mathematics_archive, University_of_St_Andrews
  11. .
  12. ^Puttaswamy, Tumkur K. (2000), "The Mathematical Accomplishments of
      Ancient Indian Mathematicians", in Selin, Helaine (ed.), Mathematics
      Across_Cultures:_The_History_of_Non-Western_Mathematics, Netherlands:
      Kluwer Academic Publishers, p. 417, ISBN 978-1-4020-0260-1
  13. ^Biggs, Norman L. (1979). "The Roots of Combinatorics". Historia
      Mathematica. 6 (2): 109â136. doi:10.1016/0315-0860(79)90074-0.
  14. ^Maistrov, L.E. (1974), Probability_Theory:_A_Historical_Sketch, Academic
      Press, p. 35, ISBN 978-1-4832-1863-2
  15. . (Translation from 1967 Russian ed.)
  16. ^  White, Arthur T.; "Ringing the Cosets", American Mathematical Monthly,
      94 (1987), no. 8, 721â746; White, Arthur T.; "Fabian Stedman: The First
      Group Theorist?", American Mathematical Monthly, 103 (1996), no. 9,
      771â778.
  17. ^ See Journals_in_Combinatorics_and_Graph_Theory
  18. ^ Sanders, Daniel P.; 2-Digit_MSC_Comparison Archived 2008-12-31 at the
      Wayback_Machine
  19. ^ Continuous_and_profinite_combinatorics
***** References[edit] *****
    * BjÃ¶rner, Anders; and Stanley, Richard P.; (2010); A_Combinatorial
      Miscellany
    * BÃ³na, MiklÃ³s; (2011); A_Walk_Through_Combinatorics_(3rd_Edition).
ISBN 978-981-4335-23-2, 978-981-4460-00-2
Graham, Ronald L.; Groetschel, Martin; and LovÃ¡sz, LÃ¡szlÃ³; eds. (1996);
Handbook of Combinatorics, Volumes 1 and 2. Amsterdam, NL, and Cambridge, MA:
Elsevier (North-Holland) and MIT Press.
ISBN 0-262-07169-X
Lindner, Charles C.; and Rodger, Christopher A.; eds. (1997); Design Theory,
CRC-Press; 1st. edition (1997).
ISBN 0-8493-3986-3.
Riordan,_John (2002) [1958], An Introduction to Combinatorial Analysis, Dover,
ISBN 978-0-486-42536-8
Ryser, Herbert John (1963), Combinatorial Mathematics, The Carus Mathematical
Monographs(#14), The Mathematical Association of America
Stanley,_Richard_P. (1997, 1999); Enumerative_Combinatorics,_Volumes_1_and_2,
Cambridge_University_Press.
ISBN 0-521-55309-1, 0-521-56069-1
van Lint, Jacobus H.; and Wilson, Richard M.; (2001); A Course in
Combinatorics, 2nd Edition, Cambridge University Press.
ISBN 0-521-80340-3
***** External links[edit] *****
Combinatoricsat Wikipedia's sister_projects
    * Definitions from Wiktionary
    * Media from Wikimedia Commons
    * Quotations from Wikiquote
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Combinatorial_analysis",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Combinatorial_Analysis â an article in EncyclopÃ¦dia_Britannica_Eleventh
Edition
Combinatorics, a MathWorld article with many references.
Combinatorics, from a MathPages.com portal.
The_Hyperbook_of_Combinatorics, a collection of math articles links.
The_Two_Cultures_of_Mathematics by W.T. Gowers, article on problem solving vs
theory building.
"Glossary_of_Terms_in_Combinatorics"
List_of_Combinatorics_Software_and_Databases
    * v
    * t
    * e
Areas_of_mathematics
                  * Category_theory
                  * Information_theory
Foundations       * Mathematical_logic
                  * Philosophy_of_mathematics
                  * Set_theory
                  * Abstract
Algebra           * Elementary
                  * Linear
                  * Multilinear
                  * Calculus
                  * Real_analysis
Analysis          * Complex_analysis
                  * Differential_equations
                  * Functional_analysis
                  * Combinatorics
Discrete          * Graph_theory
                  * Order_theory
                  * Game_theory
                  * Algebraic
                  * Analytic
Geometry          * Differential
                  * Discrete
                  * Euclidean
                  * Finite
                  * Arithmetic
Number_theory     * Algebraic_number_theory
                  * Analytic_number_theory
                  * Diophantine_geometry
                  * Algebraic
Topology          * Differential
                  * Geometric
                  * Control_theory
                  * Mathematical_economics
                  * Mathematical_finance
Applied           * Mathematical_physics
                  * Mathematical_statistics
                  * Probability
                  * Statistics
                  * Computer_science
                  * Theory_of_computation
Computational     * Numerical_analysis
                  * Optimization
                  * Computer_algebra
                  * History_of_mathematics
Others            * Recreational_mathematics
                  * Mathematics_and_art
                  * Mathematics_education
    * [Category] Category
    * [Portal] Portal
    * [Commons page]Commons
    * [WikiProject]WikiProject
    * v
    * t
    * e
Computer_science
Note: This template roughly follows the 2012 ACM_Computing_Classification
System.
                          * Printed_circuit_board
                          * Peripheral
                          * Integrated_circuit
Hardware                  * Very_Large_Scale_Integration
                          * Systems_on_Chip_(SoCs)
                          * Energy_consumption_(Green_computing)
                          * Electronic_design_automation
                          * Hardware_acceleration
                          * Computer_architecture
Computer systems          * Embedded_system
organization              * Real-time_computing
                          * Dependability
                          * Network_architecture
                          * Network_protocol
Networks                  * Network_components
                          * Network_scheduler
                          * Network_performance_evaluation
                          * Network_service
                          * Interpreter
                          * Middleware
Software organization     * Virtual_machine
                          * Operating_system
                          * Software_quality
                          * Programming_paradigm
                          * Programming_language
                          * Compiler
                          * Domain-specific_language
Software_notations        * Modeling_language
and tools                 * Software_framework
                          * Integrated_development_environment
                          * Software_configuration_management
                          * Software_library
                          * Software_repository
                          * Software_development_process
                          * Requirements_analysis
                          * Software_design
Software_development      * Software_construction
                          * Software_deployment
                          * Software_maintenance
                          * Programming_team
                          * Open-source_model
                          * Model_of_computation
                          * Formal_language
Theory_of_computation     * Automata_theory
                          * Computational_complexity_theory
                          * Logic
                          * Semantics
                          * Algorithm_design
                          * Analysis_of_algorithms
Algorithms                * Algorithmic_efficiency
                          * Randomized_algorithm
                          * Computational_geometry
                          * Discrete_mathematics
                          * Probability
Mathematics               * Statistics
of computing              * Mathematical_software
                          * Information_theory
                          * Mathematical_analysis
                          * Numerical_analysis
                          * Database_management_system
                          * Information_storage_systems
                          * Enterprise_information_system
                          * Social_information_systems
                          * Geographic_information_system
                          * Decision_support_system
Information               * Process_control_system
systems                   * Multimedia_information_system
                          * Data_mining
                          * Digital_library
                          * Computing_platform
                          * Digital_marketing
                          * World_Wide_Web
                          * Information_retrieval
                          * Cryptography
                          * Formal_methods
                          * Security_services
Security                  * Intrusion_detection_system
                          * Hardware_security
                          * Network_security
                          * Information_security
                          * Application_security
                          * Interaction_design
Humanâcomputer       * Social_computing
interaction               * Ubiquitous_computing
                          * Visualization
                          * Accessibility
                          * Concurrent_computing
                          * Parallel_computing
Concurrency               * Distributed_computing
                          * Multithreading
                          * Multiprocessing
                          * Natural_language_processing
                          * Knowledge_representation_and_reasoning
                          * Computer_vision
Artificial                * Automated_planning_and_scheduling
intelligence              * Search_methodology
                          * Control_method
                          * Philosophy_of_artificial_intelligence
                          * Distributed_artificial_intelligence
                          * Supervised_learning
                          * Unsupervised_learning
Machine_learning          * Reinforcement_learning
                          * Multi-task_learning
                          * Cross-validation
                          * Animation
                          * Rendering
                          * Image_manipulation
Graphics                  * Graphics_processing_unit
                          * Mixed_reality
                          * Virtual_reality
                          * Image_compression
                          * Solid_modeling
                          * E-commerce
                          * Enterprise_software
                          * Computational_mathematics
                          * Computational_physics
                          * Computational_chemistry
                          * Computational_biology
                          * Computational_social_science
                          * Computational_engineering
Applied                   * Computational_healthcare
computing                 * Digital_art
                          * Electronic_publishing
                          * Cyberwarfare
                          * Electronic_voting
                          * Video_games
                          * Word_processing
                          * Operations_research
                          * Educational_technology
                          * Document_management
    * [Wikipedia book] Book
    * [Category] Category
    * [Portal] Portal
    * [Outline] Outline
    * [WikiProject]WikiProject
    * [Commons page] Commons

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Combinatorics&oldid=901616898"
Categories:
    * Combinatorics
Hidden categories:
    * Webarchive_template_wayback_links
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
    * Wikibooks
    * Wikiquote
    * Wikiversity
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * á áá­á
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * Ð§ÓÐ²Ð°ÑÐ»Ð°
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * è´èª
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Ido
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Latina
    * LatvieÅ¡u
    * LietuviÅ³
    * Lingua_Franca_Nova
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * áá¼ááºáá¬áá¬áá¬
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Patois
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡Ð°ÑÐ°_ÑÑÐ»Ð°
    * Scots
    * Shqip
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ××Ö´×××©
    * ç²µèª
    * Å½emaitÄÅ¡ka
    * ä¸­æ
Edit_links
    * This page was last edited on 13 June 2019, at 04:02 (UTC).
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
