The following text has been accessed from https://en.wikipedia.org/wiki/Theory_of_computation at Fri Aug 9 01:07:21 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Theory of computation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with computational_theory_of_mind.
For the journal, see Theory_of_Computing.
An artistic representation of a Turing_machine. Turing machines are frequently
used as theoretical models for computing.
In theoretical_computer_science and mathematics, the theory of computation is
the branch that deals with how efficiently problems can be solved on a model_of
computation, using an algorithm. The field is divided into three major
branches: automata_theory and languages, computability_theory, and
computational_complexity_theory, which are linked by the question: "What are
the fundamental capabilities and limitations of computers?".[1]
In order to perform a rigorous study of computation, computer scientists work
with a mathematical abstraction of computers called a model_of_computation.
There are several models in use, but the most commonly examined is the Turing
machine.[2] Computer scientists study the Turing machine because it is simple
to formulate, can be analyzed and used to prove results, and because it
represents what many consider the most powerful possible "reasonable" model of
computation (see ChurchâTuring_thesis).[3] It might seem that the potentially
infinite memory capacity is an unrealizable attribute, but any decidable
problem[4] solved by a Turing machine will always require only a finite amount
of memory. So in principle, any problem that can be solved (decided) by a
Turing machine can be solved by a computer that has a finite amount of memory.
⁰
***** Contents *****
    * 1_History
    * 2_Branches
          o 2.1_Automata_theory
                # 2.1.1_Formal_Language_theory
          o 2.2_Computability_theory
          o 2.3_Computational_complexity_theory
    * 3_Models_of_computation
    * 4_References
    * 5_Further_reading
    * 6_External_links
***** History[edit] *****
The theory of computation can be considered the creation of models of all kinds
in the field of computer science. Therefore, mathematics_and_logic are used. In
the last century it became an independent academic discipline and was separated
from mathematics.
Some pioneers of the theory of computation were Ramon_Llull, Alonzo_Church,
Kurt_GÃ¶del, Alan_Turing, Stephen_Kleene, RÃ³zsa_PÃ©ter, John_von_Neumann and
Claude_Shannon.
***** Branches[edit] *****
**** Automata theory[edit] ****
Main article: Automata_theory
Grammar Languages              Automaton              Production rules
                                                      (constraints)
                                                         &#x03B1; &#x2192;
                                                      &#x03B2;   {\displaystyle
Type-0  Recursively_enumerable Turing_machine         \alpha \rightarrow \beta
                                                      }  [\alpha \rightarrow
                                                      \beta ] (no restrictions)
                                                         &#x03B1; A &#x03B2;
                                                      &#x2192; &#x03B1;
                               Linear-bounded_non-    &#x03B3; &#x03B2;
Type-1  Context-sensitive      deterministic_Turing   {\displaystyle \alpha
                               machine                A\beta \rightarrow \alpha
                                                      \gamma \beta }  [\alpha A
                                                      \beta \rightarrow \alpha
                                                      \gamma \beta]
                                                         A &#x2192; &#x03B3;
Type-2  Context-free           Non-deterministic      {\displaystyle
                               pushdown_automaton     A\rightarrow \gamma }  [A
                                                      \rightarrow \gamma]
                                                         A &#x2192; a
                                                      {\displaystyle
                                                      A\rightarrow a}  [A
                                                      \rightarrow a]
Type-3  Regular                Finite_state_automaton and
                                                         A &#x2192; a B
                                                      {\displaystyle
                                                      A\rightarrow aB}  [A
                                                      \rightarrow aB]
Automata theory is the study of abstract machines (or more appropriately,
abstract 'mathematical' machines or systems) and the computational problems
that can be solved using these machines. These abstract machines are called
automata. Automata comes from the Greek word (ÎÏÏÏÎ¼Î±ÏÎ±) which means
that something is doing something by itself. Automata theory is also closely
related to formal_language theory,[5] as the automata are often classified by
the class of formal languages they are able to recognize. An automaton can be a
finite representation of a formal language that may be an infinite set.
Automata are used as theoretical models for computing machines, and are used
for proofs about computability.
*** Formal Language theory[edit] ***
Main article: Formal_language
[The_Chomsky_hierarchy]
Set inclusions described by the Chomsky hierarchy
Language theory is a branch of mathematics concerned with describing languages
as a set of operations over an alphabet. It is closely linked with automata
theory, as automata are used to generate and recognize formal languages. There
are several classes of formal languages, each allowing more complex language
specification than the one before it, i.e. Chomsky_hierarchy,[6] and each
corresponding to a class of automata which recognizes it. Because automata are
used as models for computation, formal languages are the preferred mode of
specification for any problem that must be computed.
**** Computability theory[edit] ****
Main article: Computability_theory
Computability theory deals primarily with the question of the extent to which a
problem is solvable on a computer. The statement that the halting_problem
cannot be solved by a Turing machine[7] is one of the most important results in
computability theory, as it is an example of a concrete problem that is both
easy to formulate and impossible to solve using a Turing machine. Much of
computability theory builds on the halting problem result.
Another important step in computability theory was Rice's_theorem, which states
that for all non-trivial properties of partial functions, it is undecidable
whether a Turing machine computes a partial function with that property.[8]
Computability theory is closely related to the branch of mathematical_logic
called recursion_theory, which removes the restriction of studying only models
of computation which are reducible to the Turing model.[9] Many mathematicians
and computational theorists who study recursion theory will refer to it as
computability theory.
**** Computational complexity theory[edit] ****
Main article: Computational_complexity_theory
A representation of the relation among complexity classes
Complexity_theory considers not only whether a problem can be solved at all on
a computer, but also how efficiently the problem can be solved. Two major
aspects are considered: time complexity and space complexity, which are
respectively how many steps does it take to perform a computation, and how much
memory is required to perform that computation.
In order to analyze how much time and space a given algorithm requires,
computer scientists express the time or space required to solve the problem as
a function of the size of the input problem. For example, finding a particular
number in a long list of numbers becomes harder as the list of numbers grows
larger. If we say there are n numbers in the list, then if the list is not
sorted or indexed in any way we may have to look at every number in order to
find the number we're seeking. We thus say that in order to solve this problem,
the computer needs to perform a number of steps that grows linearly in the size
of the problem.
To simplify this problem, computer scientists have adopted Big_O_notation,
which allows functions to be compared in a way that ensures that particular
aspects of a machine's construction do not need to be considered, but rather
only the asymptotic_behavior as problems become large. So in our previous
example we might say that the problem requires     O ( n )   {\displaystyle O
(n)}  [O(n)] steps to solve.
Perhaps the most important open problem in all of computer_science is the
question of whether a certain broad class of problems denoted NP can be solved
efficiently. This is discussed further at Complexity_classes_P_and_NP, and P
versus_NP_problem is one of the seven Millennium_Prize_Problems stated by the
Clay_Mathematics_Institute in 2000. The Official_Problem_Description was given
by Turing_Award winner Stephen_Cook.
***** Models of computation[edit] *****
Main article: Model_of_computation
Aside from a Turing_machine, other equivalent (See: ChurchâTuring_thesis)
models of computation are in use.
  Lambda_calculus
      A computation consists of an initial lambda expression (or two if you
      want to separate the function and its input) plus a finite sequence of
      lambda terms, each deduced from the preceding term by one application of
      Beta_reduction.
  Combinatory_logic
      is a concept which has many similarities to     &#x03BB;   {\displaystyle
      \lambda }  [\lambda ]-calculus, but also important differences exist
      (e.g. fixed point combinator Y has normal form in combinatory logic but
      not in     &#x03BB;   {\displaystyle \lambda }  [\lambda ]-calculus).
      Combinatory logic was developed with great ambitions: understanding the
      nature of paradoxes, making foundations of mathematics more economic
      (conceptually), eliminating the notion of variables (thus clarifying
      their role in mathematics).
  Î¼-recursive_functions
      a computation consists of a mu-recursive function, i.e. its defining
      sequence, any input value(s) and a sequence of recursive functions
      appearing in the defining sequence with inputs and outputs. Thus, if in
      the defining sequence of a recursive function     f ( x )
      {\displaystyle f(x)}  [f(x)] the functions     g ( x )   {\displaystyle g
      (x)}  [g(x)] and     h ( x , y )   {\displaystyle h(x,y)}  [h(x,y)]
      appear, then terms of the form 'g(5)=7' or 'h(3,2)=10' might appear. Each
      entry in this sequence needs to be an application of a basic function or
      follow from the entries above by using composition, primitive_recursion
      or Î¼_recursion. For instance if     f ( x ) = h ( x , g ( x ) )
      {\displaystyle f(x)=h(x,g(x))}  [f(x)=h(x,g(x))], then for 'f(5)=3' to
      appear, terms like 'g(5)=6' and 'h(5,6)=3' must occur above. The
      computation terminates only if the final term gives the value of the
      recursive function applied to the inputs.
  Markov_algorithm
      a string_rewriting_system that uses grammar-like rules to operate on
      strings of symbols.
  Register_machine
      is a theoretically interesting idealization of a computer. There are
      several variants. In most of them, each register can hold a natural
      number (of unlimited size), and the instructions are simple (and few in
      number), e.g. only decrementation (combined with conditional jump) and
      incrementation exist (and halting). The lack of the infinite (or
      dynamically growing) external store (seen at Turing machines) can be
      understood by replacing its role with GÃ¶del_numbering techniques: the
      fact that each register holds a natural number allows the possibility of
      representing a complicated thing (e.g. a sequence, or a matrix etc.) by
      an appropriate huge natural number â unambiguity of both representation
      and interpretation can be established by number_theoretical foundations
      of these techniques.
In addition to the general computational models, some simpler computational
models are useful for special, restricted applications. Regular_expressions,
for example, specify string patterns in many contexts, from office productivity
software to programming_languages. Another formalism mathematically equivalent
to regular expressions, Finite_automata are used in circuit design and in some
kinds of problem-solving. Context-free_grammars specify programming language
syntax. Non-deterministic pushdown_automata are another formalism equivalent to
context-free grammars. Primitive_recursive_functions are a defined subclass of
the recursive functions.
Different models of computation have the ability to do different tasks. One way
to measure the power of a computational model is to study the class of formal
languages that the model can generate; in such a way to the Chomsky_hierarchy
of languages is obtained.
***** References[edit] *****
   1. ^Michael_Sipser (2013). Introduction to the Theory of Computation 3rd.
      Cengage Learning. ISBN 978-1-133-18779-0. central areas of the theory of
      computation: automata, computability, and complexity. (Page 1)
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
   3. ^Hodges,_Andrew (2012). Alan Turing: The Enigma (The Centenary Edition).
      Princeton_University_Press. ISBN 978-0-691-15564-7.
   4. ^Rabin,_Michael_O. (June 2012). Turing,_Church,_GÃ¶del,_Computability,
      Complexity_and_Randomization:_A_Personal_View.
   5. ^Donald Monk (1976). Mathematical Logic. Springer-Verlag.
      ISBN 9780387901701.
   6. ^Hopcroft,_John_E. and Jeffrey_D._Ullman (2006). Introduction_to_Automata
      Theory,_Languages,_and_Computation._3rd_ed. Reading, MA: Addison-Wesley.
      ISBN 978-0-321-45536-9.
   7. ^Chomsky_hierarchy (1956). "Three models for the description of
      language". Information Theory, IRE Transactions on. IEEE. 2 (3):
      113â124. doi:10.1109/TIT.1956.1056813.
   8. ^Alan_Turing (1937). "On_computable_numbers,_with_an_application_to_the
      Entscheidungsproblem". Proceedings of the London Mathematical Society.
      IEEE. 2 (42): 230â265. doi:10.1112/plms/s2-42.1.230. Retrieved 6
      January 2015.
   9. ^Henry Gordon Rice (1953). "Classes of Recursively Enumerable Sets and
      Their Decision Problems". Transactions of the American Mathematical
      Society. American Mathematical Society. 74 (2): 358â366. doi:10.2307/
      1990888. JSTOR 1990888.
  10. ^Martin_Davis (2004). The undecidable: Basic papers on undecidable
      propositions, unsolvable problems and computable functions (Dover Ed).
      Dover Publications. ISBN 978-0486432281.
***** Further reading[edit] *****
  Textbooks aimed at computer scientists
(There are many textbooks in this area; this list is by necessity incomplete.)
    * Hopcroft,_John_E., and Jeffrey_D._Ullman (2006). Introduction_to_Automata
      Theory,_Languages,_and_Computation. 3rd ed Reading, MA: Addison-Wesley.
ISBN 978-0-321-45536-9 One of the standard references in the field.
Linz_P. An introduction to formal language and automata. Narosa Publishing.
ISBN 9788173197819.
Michael_Sipser (2013). Introduction to the Theory of Computation (3rd ed.).
Cengage Learning. ISBN 978-1-133-18779-0.
Eitan_Gurari (1989). An_Introduction_to_the_Theory_of_Computation. Computer
Science Press. ISBN 0-7167-8182-4. Archived from the_original on 2007-01-07.
Hein, James L. (1996) Theory of Computation. Sudbury, MA: Jones & Bartlett.
ISBN 978-0-86720-497-1 A gentle introduction to the field, appropriate for
second-year undergraduate computer science students.
Taylor, R. Gregory (1998). Models of Computation and Formal Languages. New
York: Oxford University Press.
ISBN 978-0-19-510983-2 An unusually readable textbook, appropriate for upper-
level undergraduates or beginning graduate students.
Lewis, F. D. (2007). Essentials_of_theoretical_computer_science A textbook
covering the topics of formal languages, automata and grammars. The emphasis
appears to be on presenting an overview of the results and their applications
rather than providing proofs of the results.
Martin_Davis, Ron Sigal, Elaine J. Weyuker, Computability, complexity, and
languages: fundamentals of theoretical computer science, 2nd ed., Academic
Press, 1994,
ISBN 0-12-206382-1. Covers a wider range of topics than most other introductory
books, including program_semantics and quantification_theory. Aimed at graduate
students.
  Books on computability theory from the (wider) mathematical perspective
    * Hartley_Rogers,_Jr (1987). Theory of Recursive Functions and Effective
      Computability, MIT Press.
ISBN 0-262-68052-1
S._Barry_Cooper (2004). Computability Theory. Chapman and Hall/CRC. ISBN 1-
58488-237-9.
.
Carl_H._Smith, A recursive introduction to the theory of computation, Springer,
1994,
ISBN 0-387-94332-3. A shorter textbook suitable for graduate students in
Computer Science.
  Historical perspective
    * Richard_L._Epstein and Walter_A._Carnielli (2000). Computability:
      Computable Functions, Logic, and the Foundations of Mathematics, with
      Computability: A Timeline (2nd ed.). Wadsworth/Thomson Learning. ISBN 0-
      534-54644-7.
.
***** External links[edit] *****
    * Theory_of_Computation at MIT
    * Theory_of_Computation at Harvard
    * Computability_Logic - A theory of interactive computation. The main web
      source on this subject.
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
                  * Theory of computation
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

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Theory_of_computation&oldid=906460507"
Categories:
    * Theory_of_computation
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
    * Bosanski
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * Galego
    * GÄ©kÅ©yÅ©
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * Bahasa_Melayu
    * MirandÃ©s
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Tagalog
    * à¹à¸à¸¢
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * ä¸­æ
Edit_links
    * This page was last edited on 16 July 2019, at 00:10 (UTC).
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
