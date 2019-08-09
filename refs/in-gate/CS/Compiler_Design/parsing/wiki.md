The following text has been accessed from https://en.wikipedia.org/wiki/Parsing at Fri Aug 9 01:12:23 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Parsing ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Parsing, syntax analysis, or syntactic analysis is the process of analysing a
string of symbols, either in natural_language, computer_languages or data
structures, conforming to the rules of a formal_grammar. The term parsing comes
from Latin pars (orationis), meaning part_(of_speech).[1]
The term has slightly different meanings in different branches of linguistics
and computer_science. Traditional sentence parsing is often performed as a
method of understanding the exact meaning of a sentence or word, sometimes with
the aid of devices such as sentence_diagrams. It usually emphasizes the
importance of grammatical divisions such as subject and predicate.
Within computational_linguistics the term is used to refer to the formal
analysis by a computer of a sentence or other string of words into its
constituents, resulting in a parse_tree showing their syntactic relation to
each other, which may also contain semantic and other information.
The term is also used in psycholinguistics when describing language
comprehension. In this context, parsing refers to the way that human beings
analyze a sentence or phrase (in spoken language or text) "in terms of
grammatical constituents, identifying the parts of speech, syntactic relations,
etc."[1] This term is especially common when discussing what linguistic cues
help speakers to interpret garden-path_sentences.
Within computer science, the term is used in the analysis of computer
languages, referring to the syntactic analysis of the input code into its
component parts in order to facilitate the writing of compilers and
interpreters. The term may also be used to describe a split or separation.
⁰
***** Contents *****
    * 1_Human_languages
          o 1.1_Traditional_methods
          o 1.2_Computational_methods
          o 1.3_Psycholinguistics
          o 1.4_Discourse_Analysis
    * 2_Computer_languages
          o 2.1_Parser
          o 2.2_Overview_of_process
    * 3_Types_of_parsers
    * 4_Parser_development_software
    * 5_Lookahead
    * 6_See_also
    * 7_References
    * 8_Further_reading
    * 9_External_links
***** Human languages[edit] *****
Main category: Natural_language_parsing
**** Traditional methods[edit] ****
The traditional grammatical exercise of parsing, sometimes known as clause
analysis, involves breaking down a text into its component parts of speech with
an explanation of the form, function, and syntactic relationship of each part.
[2] This is determined in large part from study of the language's conjugations
and declensions, which can be quite intricate for heavily inflected languages.
To parse a phrase such as 'man bites dog' involves noting that the singular
noun 'man' is the subject of the sentence, the verb 'bites' is the third person
singular of the present tense of the verb 'to bite', and the singular noun
'dog' is the object of the sentence. Techniques such as sentence_diagrams are
sometimes used to indicate relation between elements in the sentence.
Parsing was formerly central to the teaching of grammar throughout the English-
speaking world, and widely regarded as basic to the use and understanding of
written language. However, the general teaching of such techniques is no longer
current.
**** Computational methods[edit] ****
 This section needs additional citations for verification. Please help improve_this_article by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and removed.
 Find sources: "Parsing" â news Â· newspapers Â· books Â· scholar Â· JSTOR (February 2013)
 (Learn_how_and_when_to_remove_this_template_message)
In some machine_translation and natural_language_processing systems, written
texts in human languages are parsed by computer programs.[3] Human sentences
are not easily parsed by programs, as there is substantial ambiguity in the
structure of human language, whose usage is to convey meaning (or semantics)
amongst a potentially unlimited range of possibilities but only some of which
are germane to the particular case.[4] So an utterance "Man bites dog" versus
"Dog bites man" is definite on one detail but in another language might appear
as "Man dog bites" with a reliance on the larger context to distinguish between
those two possibilities, if indeed that difference was of concern. It is
difficult to prepare formal rules to describe informal behaviour even though it
is clear that some rules are being followed.[citation_needed]
In order to parse natural language data, researchers must first agree on the
grammar to be used. The choice of syntax is affected by both linguistic and
computational concerns; for instance some parsing systems use lexical
functional_grammar, but in general, parsing for grammars of this type is known
to be NP-complete. Head-driven_phrase_structure_grammar is another linguistic
formalism which has been popular in the parsing community, but other research
efforts have focused on less complex formalisms such as the one used in the
Penn Treebank. Shallow_parsing aims to find only the boundaries of major
constituents such as noun phrases. Another popular strategy for avoiding
linguistic controversy is dependency_grammar parsing.
Most modern parsers are at least partly statistical; that is, they rely on a
corpus of training data which has already been annotated (parsed by hand). This
approach allows the system to gather information about the frequency with which
various constructions occur in specific contexts. (See machine_learning.)
Approaches which have been used include straightforward PCFGs (probabilistic
context-free grammars),[5] maximum_entropy,[6] and neural_nets.[7] Most of the
more successful systems use lexical statistics (that is, they consider the
identities of the words involved, as well as their part_of_speech). However
such systems are vulnerable to overfitting and require some kind of smoothing
to be effective.[citation_needed]
Parsing algorithms for natural language cannot rely on the grammar having
'nice' properties as with manually designed grammars for programming languages.
As mentioned earlier some grammar formalisms are very difficult to parse
computationally; in general, even if the desired structure is not context-free,
some kind of context-free approximation to the grammar is used to perform a
first pass. Algorithms which use context-free grammars often rely on some
variant of the CYK_algorithm, usually with some heuristic to prune away
unlikely analyses to save time. (See chart_parsing.) However some systems trade
speed for accuracy using, e.g., linear-time versions of the shift-reduce
algorithm. A somewhat recent development has been parse_reranking in which the
parser proposes some large number of analyses, and a more complex system
selects the best option.[citation_needed] Semantic_parsers convert texts into
representations of their meanings.[8]
**** Psycholinguistics[edit] ****
In psycholinguistics, parsing involves not just the assignment of words to
categories (formation of ontological insights), but the evaluation of the
meaning of a sentence according to the rules of syntax drawn by inferences made
from each word in the sentence (known as connotation. This normally occurs as
words are being heard or read. Consequently, psycholinguistic models of parsing
are of necessity incremental, meaning that they build up an interpretation as
the sentence is being processed, which is normally expressed in terms of a
partial syntactic structure. Creation of initially wrong structures occurs when
interpreting garden_path_sentences.
**** Discourse Analysis[edit] ****
Discourse_Analysis examines ways to analyze language use and semiotic events.
Persuasive language may be called rhetoric.
***** Computer languages[edit] *****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (February 2013)(Learn_how_and_when_to_remove_this_template_message)
**** Parser[edit] ****
A parser is a software component that takes input data (frequently text) and
builds a data_structure â often some kind of parse_tree, abstract_syntax_tree
or other hierarchical structure, giving a structural representation of the
input while checking for correct syntax. The parsing may be preceded or
followed by other steps, or these may be combined into a single step. The
parser is often preceded by a separate lexical_analyser, which creates tokens
from the sequence of input characters; alternatively, these can be combined in
scannerless_parsing. Parsers may be programmed by hand or may be automatically
or semi-automatically generated by a parser_generator. Parsing is complementary
to templating, which produces formatted output. These may be applied to
different domains, but often appear together, such as the scanf/printf pair, or
the input (front end parsing) and output (back end code generation) stages of a
compiler.
The input to a parser is often text in some computer_language, but may also be
text in a natural language or less structured textual data, in which case
generally only certain parts of the text are extracted, rather than a parse
tree being constructed. Parsers range from very simple functions such as scanf,
to complex programs such as the frontend of a C++_compiler or the HTML parser
of a web_browser. An important class of simple parsing is done using regular
expressions, in which a group of regular expressions defines a regular_language
and a regular expression engine automatically generating a parser for that
language, allowing pattern matching and extraction of text. In other contexts
regular expressions are instead used prior to parsing, as the lexing step whose
output is then used by the parser.
The use of parsers varies by input. In the case of data languages, a parser is
often found as the file reading facility of a program, such as reading in HTML
or XML text; these examples are markup_languages. In the case of programming
languages, a parser is a component of a compiler or interpreter, which parses
the source_code of a computer_programming_language to create some form of
internal representation; the parser is a key step in the compiler_frontend.
Programming languages tend to be specified in terms of a deterministic_context-
free_grammar because fast and efficient parsers can be written for them. For
compilers, the parsing itself can be done in one pass or multiple passes â
see one-pass_compiler and multi-pass_compiler.
The implied disadvantages of a one-pass compiler can largely be overcome by
adding fix-ups, where provision is made for code relocation during the forward
pass, and the fix-ups are applied backwards when the current program segment
has been recognized as having been completed. An example where such a fix-up
mechanism would be useful would be a forward GOTO statement, where the target
of the GOTO is unknown until the program segment is completed. In this case,
the application of the fix-up would be delayed until the target of the GOTO was
recognized. Conversely, a backward GOTO does not require a fix-up, as the
location will already be known.
Context-free grammars are limited in the extent to which they can express all
of the requirements of a language. Informally, the reason is that the memory of
such a language is limited. The grammar cannot remember the presence of a
construct over an arbitrarily long input; this is necessary for a language in
which, for example, a name must be declared before it may be referenced. More
powerful grammars that can express this constraint, however, cannot be parsed
efficiently. Thus, it is a common strategy to create a relaxed parser for a
context-free grammar which accepts a superset of the desired language
constructs (that is, it accepts some invalid constructs); later, the unwanted
constructs can be filtered out at the semantic_analysis (contextual analysis)
step.
For example, in Python the following is syntactically valid code:
x = 1
print(x)
The following code, however, is syntactically valid in terms of the context-
free grammar, yielding a syntax tree with the same structure as the previous,
but is syntactically invalid in terms of the context-sensitive_grammar, which
requires that variables be initialized before use:
x = 1
print(y)
Rather than being analyzed at the parsing stage, this is caught by checking the
values in the syntax tree, hence as part of semantic analysis: context-
sensitive syntax is in practice often more easily analyzed as semantics.
**** Overview of process[edit] ****
[Flow_of_data_in_a_typical_parser]
The following example demonstrates the common case of parsing a computer
language with two levels of grammar: lexical and syntactic.
The first stage is the token generation, or lexical_analysis, by which the
input character stream is split into meaningful symbols defined by a grammar of
regular_expressions. For example, a calculator program would look at an input
such as "12 * (3 + 4)^2" and split it into the tokens 12, *, (, 3, +, 4, ), ^,
2, each of which is a meaningful symbol in the context of an arithmetic
expression. The lexer would contain rules to tell it that the characters *, +,
^, ( and ) mark the start of a new token, so meaningless tokens like "12*" or "
(3" will not be generated.
The next stage is parsing or syntactic analysis, which is checking that the
tokens form an allowable expression. This is usually done with reference to a
context-free_grammar which recursively defines components that can make up an
expression and the order in which they must appear. However, not all rules
defining programming languages can be expressed by context-free grammars alone,
for example type validity and proper declaration of identifiers. These rules
can be formally expressed with attribute_grammars.
The final phase is semantic_parsing or analysis, which is working out the
implications of the expression just validated and taking the appropriate
action. In the case of a calculator or interpreter, the action is to evaluate
the expression or program; a compiler, on the other hand, would generate some
kind of code. Attribute grammars can also be used to define these actions.
***** Types of parsers[edit] *****
The task of the parser is essentially to determine if and how the input can be
derived from the start symbol of the grammar. This can be done in essentially
two ways:
    * Top-down_parsing - Top-down parsing can be viewed as an attempt to find
      left-most derivations of an input-stream by searching for parse_trees
      using a top-down expansion of the given formal_grammar rules. Tokens are
      consumed from left to right. Inclusive choice is used to accommodate
      ambiguity by expanding all alternative right-hand-sides of grammar rules.
      [9]
    * Bottom-up_parsing - A parser can start with the input and attempt to
      rewrite it to the start symbol. Intuitively, the parser attempts to
      locate the most basic elements, then the elements containing these, and
      so on. LR_parsers are examples of bottom-up parsers. Another term used
      for this type of parser is Shift-Reduce parsing.
LL_parsers and recursive-descent_parser are examples of top-down parsers which
cannot accommodate left_recursive production_rules. Although it has been
believed that simple implementations of top-down parsing cannot accommodate
direct and indirect left-recursion and may require exponential time and space
complexity while parsing ambiguous context-free_grammars, more sophisticated
algorithms for top-down parsing have been created by Frost, Hafiz, and
Callaghan[10][11] which accommodate ambiguity and left_recursion in polynomial
time and which generate polynomial-size representations of the potentially
exponential number of parse trees. Their algorithm is able to produce both
left-most and right-most derivations of an input with regard to a given
context-free_grammar.
An important distinction with regard to parsers is whether a parser generates a
leftmost derivation or a rightmost derivation (see context-free_grammar). LL
parsers will generate a leftmost derivation and LR parsers will generate a
rightmost derivation (although usually in reverse).[9]
Some graphical parsing algorithms have been designed for visual_programming
languages.[12][13] Parsers for visual languages are sometimes based on graph
grammars.[14]
Adaptive_parsing algorithms have been used to construct "self-extending"
natural_language_user_interfaces.[15]
***** Parser development software[edit] *****
 This article is in list format, but may read better as prose. You can help by
 converting_this_article, if appropriate. Editing_help is available. (January
 2017)
Some of the well known parser development tools include the following. Also see
comparison_of_parser_generators.
    * ANTLR
    * Bison
    * Coco/R
    * Definite_clause_grammar
    * GOLD
    * JavaCC
    * Lemon
    * Lex
    * LuZc
    * Parboiled
    * Parsec
    * Ragel
    * Spirit_Parser_Framework
    * Syntax_Definition_Formalism
    * SYNTAX
    * XPL
    * Yacc
    * PackCC
***** Lookahead[edit] *****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (April 2012)(Learn_how_and_when_to_remove_this_template_message)
C program that cannot be parsed with less than 2 token lookahead. Top: C
grammar excerpt[16]. Bottom: a parser has digested the tokens "int v;main(){"
and is about choose a rule to derive Stmt. Looking only at the first lookahead
token "v", it cannot decide which of both alternatives for Stmt to choose; the
latter requires peeking at the second token.
Lookahead establishes the maximum incoming tokens that a parser can use to
decide which rule it should use. Lookahead is especially relevant to LL, LR,
and LALR_parsers, where it is often explicitly indicated by affixing the
lookahead to the algorithm name in parentheses, such as LALR(1).
Most programming_languages, the primary target of parsers, are carefully
defined in such a way that a parser with limited lookahead, typically one, can
parse them, because parsers with limited lookahead are often more efficient.
One important change[citation_needed] to this trend came in 1990 when Terence
Parr created ANTLR for his Ph.D. thesis, a parser_generator for efficient LL(k)
parsers, where k is any fixed value.
LR parsers typically have only a few actions after seeing each token. They are
shift (add this token to the stack for later reduction), reduce (pop tokens
from the stack and form a syntactic construct), end, error (no known rule
applies) or conflict (does not know whether to shift or reduce).
Lookahead has two advantages.[clarification_needed]
    * It helps the parser take the correct action in case of conflicts. For
      example, parsing the if statement in the case of an else clause.
    * It eliminates many duplicate states and eases the burden of an extra
      stack. A C language non-lookahead parser will have around 10,000 states.
      A lookahead parser will have around 300 states.
Example: Parsing the Expression 1 + 2 * 3[dubious  – discuss]
Set of expression parsing rules (called grammar) is as follows,
Rule1: E â E + Expression is the sum of two expressions.
Rule2: E â E * Expression is the product of two expressions.
Rule3: E â numbExpression is a simple number
Rule4: + has less precedence than *
Most programming languages (except for a few such as APL and Smalltalk) and
algebraic formulas give higher precedence to multiplication than addition, in
which case the correct interpretation of the example above is 1 + (2 * 3). Note
that Rule4 above is a semantic rule. It is possible to rewrite the grammar to
incorporate this into the syntax. However, not all such rules can be translated
into syntax.
  Simple non-lookahead parser actions
Initially Input = [1, +, 2, *, 3]
   1. Shift "1" onto stack from input (in anticipation of rule3). Input = [+,
      2, *, 3] Stack = [1]
   2. Reduces "1" to expression "E" based on rule3. Stack = [E]
   3. Shift "+" onto stack from input (in anticipation of rule1). Input = [2,
      *, 3] Stack = [E, +]
   4. Shift "2" onto stack from input (in anticipation of rule3). Input = [*,
      3] Stack = [E, +, 2]
   5. Reduce stack element "2" to Expression "E" based on rule3. Stack = [E, +,
      E]
   6. Reduce stack items [E, +, E] and new input "E" to "E" based on rule1.
      Stack = [E]
   7. Shift "*" onto stack from input (in anticipation of rule2). Input = [3]
      Stack = [E,*]
   8. Shift "3" onto stack from input (in anticipation of rule3). Input = []
      (empty) Stack = [E, *, 3]
   9. Reduce stack element "3" to expression "E" based on rule3. Stack = [E, *,
      E]
  10. Reduce stack items [E, *, E] and new input "E" to "E" based on rule2.
      Stack = [E]
The parse tree and resulting code from it is not correct according to language
semantics.
To correctly parse without lookahead, there are three solutions:
    * The user has to enclose expressions within parentheses. This often is not
      a viable solution.
    * The parser needs to have more logic to backtrack and retry whenever a
      rule is violated or not complete. The similar method is followed in LL
      parsers.
    * Alternatively, the parser or grammar needs to have extra logic to delay
      reduction and reduce only when it is absolutely sure which rule to reduce
      first. This method is used in LR parsers. This correctly parses the
      expression but with many more states and increased stack depth.
  Lookahead parser actions[clarification_needed]
   1. Shift 1 onto stack on input 1 in anticipation of rule3. It does not
      reduce immediately.
   2. Reduce stack item 1 to simple Expression on input + based on rule3. The
      lookahead is +, so we are on path to E +, so we can reduce the stack to
      E.
   3. Shift + onto stack on input + in anticipation of rule1.
   4. Shift 2 onto stack on input 2 in anticipation of rule3.
   5. Reduce stack item 2 to Expression on input * based on rule3. The
      lookahead * expects only E before it.
   6. Now stack has E + E and still the input is *. It has two choices now,
      either to shift based on rule2 or reduction based on rule1. Since * has
      higher precedence than + based on rule4, we shift * onto stack in
      anticipation of rule2.
   7. Shift 3 onto stack on input 3 in anticipation of rule3.
   8. Reduce stack item 3 to Expression after seeing end of input based on
      rule3.
   9. Reduce stack items E * E to E based on rule2.
  10. Reduce stack items E + E to E based on rule1.
The parse tree generated is correct and simply more efficient[clarify][citation
needed] than non-lookahead parsers. This is the strategy followed in LALR
parsers.
***** See also[edit] *****
 This article is in list format, but may read better as prose. You can help by
 converting_this_article, if appropriate. Editing_help is available. (January
 2017)
    * Backtracking
    * Chart_parser
    * Compiler-compiler
    * Deterministic_parsing
    * Generating_strings
    * Grammar_checker
    * LALR_parser
    * Lexical_analysis
    * Pratt_parser
    * Shallow_parsing
    * Left_corner_parser
    * Parsing_expression_grammar
    * ASF+SDF_Meta_Environment
    * DMS_Software_Reengineering_Toolkit
    * Program_transformation
    * Source_code_generation
***** References[edit] *****
   1. ^ a b"Parse". dictionary.reference.com. Retrieved 27 November 2010.
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
   3. ^"Grammar_and_Composition".
   4. ^Christopher D.. Manning; Christopher D. Manning; Hinrich SchÃ¼tze
      (1999). Foundations_of_Statistical_Natural_Language_Processing. MIT
      Press. ISBN 978-0-262-13360-9.
   5. ^Jurafsky, Daniel (1996). "A Probabilistic Model of Lexical and Syntactic
      Access and Disambiguation". Cognitive Science. 20 (2): 137â194.
      CiteSeerX 10.1.1.150.5711. doi:10.1207/s15516709cog2002_1.
   6. ^ Klein, Dan, and Christopher D. Manning. "Accurate_unlexicalized
      parsing." Proceedings of the 41st Annual Meeting on Association for
      Computational Linguistics-Volume 1. Association for Computational
      Linguistics, 2003.
   7. ^ Charniak, Eugene. "A_maximum-entropy-inspired_parser." Proceedings of
      the 1st North American chapter of the Association for Computational
      Linguistics conference. Association for Computational Linguistics, 2000.
   8. ^ Chen, Danqi, and Christopher Manning. "A_fast_and_accurate_dependency
      parser_using_neural_networks." Proceedings of the 2014 conference on
      empirical methods in natural language processing (EMNLP). 2014.
   9. ^Jia, Robin; Liang, Percy (2016-06-11). "Data Recombination for Neural
      Semantic Parsing". arXiv:1606.03622 [cs.CL].
  10. ^ a b Aho, A.V., Sethi, R. and Ullman ,J.D. (1986) " Compilers:
      principles, techniques, and tools." Addison-Wesley_Longman Publishing
      Co., Inc. Boston, MA, USA.
  11. ^ Frost, R., Hafiz, R. and Callaghan, P. (2007) " Modular_and_Efficient
      Top-Down_Parsing_for_Ambiguous_Left-Recursive_Grammars ." 10th
      International Workshop on Parsing Technologies (IWPT), ACL-SIGPARSE,
      Pages: 109 - 120, June 2007, Prague.
  12. ^ Frost, R., Hafiz, R. and Callaghan, P. (2008) " Parser_Combinators_for
      Ambiguous_Left-Recursive_Grammars." 10th International Symposium on
      Practical Aspects of Declarative Languages (PADL), ACM-SIGPLAN, Volume
      4902/2008, Pages: 167 - 181, January 2008, San Francisco.
  13. ^ Rekers, Jan, and Andy SchÃ¼rr. "Defining_and_parsing_visual_languages
      with_layered_graph_grammars." Journal of Visual Languages & Computing 8.1
      (1997): 27-55.
  14. ^ Rekers, Jan, and A. Schurr. "A_graph_grammar_approach_to_graphical
      parsing." Visual Languages, Proceedings., 11th IEEE International
      Symposium on. IEEE, 1995.
  15. ^ Zhang, Da-Qian, Kang Zhang, and Jiannong Cao. "A_context-sensitive
      graph_grammar_formalism_for_the_specification_of_visual_languages." The
      Computer Journal 44.3 (2001): 186-200.
  16. ^Jill Fain Lehman (6 December 2012). Adaptive_Parsing:_Self-Extending
      Natural_Language_Interfaces. Springer Science & Business Media. ISBN 978-
      1-4615-3622-2.
  17. ^ taken fromBrian W. Kernighan and Dennis M. Ritchie (Apr 1988). The C
      Programming Language. Prentice Hall Software Series (2nd ed.). Englewood
      Cliffs/NJ: Prentice Hall. ISBN 0131103628.
  18.  (Appendix A.13 "Grammar", p.193 ff)
***** Further reading[edit] *****
    * Chapman, Nigel P., LR_Parsing:_Theory_and_Practice, Cambridge_University
      Press, 1987.
ISBN 0-521-30413-X
Grune, Dick; Jacobs, Ceriel J.H., Parsing_Techniques_-_A_Practical_Guide, Vrije
Universiteit_Amsterdam, Amsterdam, The Netherlands. Originally published by
Ellis Horwood, Chichester, England, 1990;
ISBN 0-13-651431-6
***** External links[edit] *****
 Look up parse or parsing in Wiktionary, the free dictionary.
    * The_Lemon_LALR_Parser_Generator
    * Stanford_Parser The Stanford Parser
    * Turin_University_Parser Natural language parser for the Italian, open
      source, developed in Common Lisp by Leonardo Lesmo, University of Torino,
      Italy.
    * Short_history_of_parser_construction
    * Spoon: A library to analyze, transform, rewrite, and transpile Java
      source code. It parses source files to build a well-designed AST with
      powerful analysis and transformation API.
    * v
    * t
    * e
Parsing algorithms
                   * LL
Top-down           * Recursive_descent
                         o Tail_recursive
                         o Pratt_parser
                   * Precedence
                         o Simple
                         o Operator
                               # Shunting-yard
                   * Bounded-context
                   * LR
Bottom-up                o Simple
                         o Look-ahead
                         o Canonical
                         o Generalized
                   * CYK
                   * Recursive_ascent
                   * Shift-reduce
                   * Combinator
Mixed/Other        * Chart
                   * Earley
                   * PEG
                   * Definite_clause_grammar
                   * Dynamic_programming
                   * Memoization
                   * Parser_generator
Related topics           o LALR
                   * Metacompiler
                   * Parse_tree
                   * AST
                   * Scannerless_parsing
                   * History_of_compiler_construction
                   * Comparison_of_parser_generators

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Parsing&oldid=897166408"
Categories:
    * Algorithms_on_strings
    * Compiler_construction
    * Parsing
Hidden categories:
    * Articles_needing_additional_references_from_February_2013
    * All_articles_needing_additional_references
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_February_2018
    * Articles_with_unsourced_statements_from_May_2008
    * Articles_with_unsourced_statements_from_January_2019
    * Articles_needing_cleanup_from_January_2017
    * All_pages_needing_cleanup
    * Articles_with_sections_that_need_to_be_turned_into_prose_from_January
      2017
    * Articles_needing_additional_references_from_April_2012
    * Articles_with_unsourced_statements_from_December_2008
    * Wikipedia_articles_needing_clarification_from_April_2019
    * All_accuracy_disputes
    * Articles_with_disputed_statements_from_April_2019
    * All_Wikipedia_articles_needing_clarification
    * Articles_with_unsourced_statements_from_April_2011
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
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 15 May 2019, at 06:20 (UTC).
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
