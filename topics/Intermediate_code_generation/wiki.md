The following text has been accessed from https://en.wikipedia.org/wiki/Code_generation_(compiler) at Fri Aug 9 01:12:28 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Code generation (compiler) ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article needs additional citations for verification. Please help improve_this_article
 by adding_citations_to_reliable_sources. Unsourced material may be challenged and removed.
 Find sources: "Code_generation" compiler â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (November 2006)(Learn_how_and_when_to_remove_this_template_message)
In computing, code generation is the process by which a compiler's code
generator converts some intermediate_representation of source_code into a form
(e.g., machine_code) that can be readily executed by a machine.
Sophisticated compilers typically perform multiple passes over various
intermediate forms. This multi-stage process is used because many algorithms
for code_optimization are easier to apply one at a time, or because the input
to one optimization relies on the completed processing performed by another
optimization. This organization also facilitates the creation of a single
compiler that can target multiple architectures, as only the last of the code
generation stages (the backend) needs to change from target to target. (For
more information on compiler design, see Compiler.)
The input to the code generator typically consists of a parse_tree or an
abstract_syntax_tree. The tree is converted into a linear sequence of
instructions, usually in an intermediate_language such as three-address_code.
Further stages of compilation may or may not be referred to as "code
generation", depending on whether they involve a significant change in the
representation of the program. (For example, a peephole_optimization pass would
not likely be called "code generation", although a code generator might
incorporate a peephole optimization pass.)
⁰
***** Contents *****
    * 1_Major_tasks_in_code_generation
    * 2_Runtime_code_generation
    * 3_Related_concepts
          o 3.1_Reflection
    * 4_See_also
    * 5_References
***** Major tasks in code generation[edit] *****
In addition to the basic conversion from an intermediate representation into a
linear sequence of machine instructions, a typical code generator tries to
optimize the generated code in some way.
Tasks which are typically part of a sophisticated compiler's "code generation"
phase include:
    * Instruction_selection: which instructions to use.
    * Instruction_scheduling: in which order to put those instructions.
      Scheduling is a speed optimization that can have a critical effect on
      pipelined machines.
    * Register_allocation: the allocation of variables to processor_registers
      [1]
    * Debug_data generation if required so the code can be debugged.
Instruction selection is typically carried out by doing a recursive postorder
traversal on the abstract syntax tree, matching particular tree configurations
against templates; for example, the tree W := ADD(X,MUL(Y,Z)) might be
transformed into a linear sequence of instructions by recursively generating
the sequences for t1 := X and t2 := MUL(Y,Z), and then emitting the instruction
ADD W, t1, t2.
In a compiler that uses an intermediate language, there may be two instruction
selection stages — one to convert the parse tree into intermediate code, and a
second phase much later to convert the intermediate code into instructions from
the instruction_set of the target machine. This second phase does not require a
tree traversal; it can be done linearly, and typically involves a simple
replacement of intermediate-language operations with their corresponding
opcodes. However, if the compiler is actually a language_translator (for
example, one that converts Eiffel to C), then the second code-generation phase
may involve building a tree from the linear intermediate code.
***** Runtime code generation[edit] *****
When code generation occurs at runtime, as in just-in-time_compilation (JIT),
it is important that the entire process be efficient with respect to space and
time. For example, when regular_expressions are interpreted and used to
generate code at runtime, a non-deterministic finite_state_machine is often
generated instead of a deterministic one, because usually the former can be
created more quickly and occupies less memory space than the latter. Despite
its generally generating less efficient code, JIT code generation can take
advantage of profiling information that is available only at runtime.
***** Related concepts[edit] *****
The fundamental task of taking input in one language and producing output in a
non-trivially different language can be understood in terms of the core
transformational operations of formal_language_theory. Consequently, some
techniques that were originally developed for use in compilers have come to be
employed in other ways as well. For example, YACC (Yet Another Compiler
Compiler) takes input in Backus-Naur_form and converts it to a parser in C.
Though it was originally created for automatic generation of a parser for a
compiler, yacc is also often used to automate writing code that needs to be
modified each time specifications are changed.[2]
Many integrated_development_environments (IDEs) support some form of automatic
source_code_generation, often using algorithms in common with compiler code
generators, although commonly less complicated. (See also: Program
transformation, Data_transformation.)
**** Reflection[edit] ****
In general, a syntax and semantic analyzer tries to retrieve the structure of
the program from the source code, while a code generator uses this structural
information (e.g., data_types) to produce code. In other words, the former adds
information while the latter loses some of the information. One consequence of
this information loss is that reflection becomes difficult or even impossible.
To counter this problem, code generators often embed syntactic and semantic
information in addition to the code necessary for execution.
***** See also[edit] *****
    * Automatic_programming
    * Comparison_of_code_generation_tools
    * Source_to_source_compilation: automatic translation of a computer program
      from one programming language to another
***** References[edit] *****
   1. ^Aho, Alfred V.; Ravi Sethi; Jeffrey D. Ullman (1987). Compilers:
      Principles, Techniques, and Tools. Addison-Wesley. p. 15. ISBN 0-201-
      10088-6.
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
   3. ^ Code_Generation:_The_Real_Lesson_of_Rails. Artima.com (2006-03-16).
      Retrieved on 2013-08-10.
Authority_control [Edit_this_at_Wikidata]     * GND: 4010346-8
                                              * LCCN: sh85027644

Retrieved from "https://en.wikipedia.org/w/index.php?title=Code_generation_
(compiler)&oldid=900211450"
Categories:
    * Machine_code
    * Compiler_construction
Hidden categories:
    * Articles_needing_additional_references_from_November_2006
    * All_articles_needing_additional_references
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
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
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 4 June 2019, at 04:38 (UTC).
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
