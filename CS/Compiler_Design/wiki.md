The following text has been accessed from https://en.wikipedia.org/wiki/Compiler#Compiler_construction at Fri Aug 9 01:12:19 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Compiler ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about software to translate computer languages. For the anime,
see Compiler_(anime).
"Compile" and "compiling" redirect here. For the software company, see Compile_
(company). For other uses, see compilation.
Program_execution
General concepts
    * Code
    * Translation
          o Compiler
                # Compile-time
          o Optimizing_compiler
    * Intermediate_representation (IR)
    * Execution
          o Runtime_system
                # Runtime
          o Executable
          o Interpreter
          o Virtual_machine
Types of code
    * Source_code
    * Object_code
    * Bytecode
    * Machine_code
    * Microcode
Compilation strategies
    * Just-in-time (JIT)
          o Tracing_just-in-time
    * Ahead-of-time (AOT)
    * Transcompilation
    * Recompilation
Notable runtimes
    * Android_Runtime (ART)
    * Common_Language_Runtime (CLR) & Mono
    * crt0
    * HHVM
    * Java_virtual_machine (JVM)
    * Objective-C
    * V8
          o Node.js
    * PyPy
    * Zend_Engine
Notable compilers & toolchains
    * GNU_Compiler_Collection (GCC)
    * LLVM
          o Clang
    * v
    * t
    * e
A compiler is a computer_program that translates computer code written in one
programming_language (the source language) into another programming language
(the target language). The name compiler is primarily used for programs that
translate source_code from a high-level_programming_language to a lower_level
language (e.g., assembly_language, object_code, or machine_code) to create an
executable program.[1][2]:p1
However, there are many different types of compilers. If the compiled program
can run on a computer whose CPU or operating_system is different from the one
on which the compiler runs, the compiler is a cross-compiler. A bootstrap
compiler is written in the language that it intends to compile. A program that
translates from a low-level_language to a higher level one is a decompiler. A
program that translates between high-level languages is usually called a
source-to-source_compiler or transpiler. A language rewriter is usually a
program that translates the form of expressions without a change of language.
The term compiler-compiler refers to tools used to create parsers that perform
syntax analysis.
A compiler is likely to perform many or all of the following operations:
preprocessing, lexical_analysis, parsing, semantic_analysis (syntax-directed
translation), conversion of input programs to an intermediate_representation,
code_optimization and code_generation. Compilers implement these operations in
phases that promote efficient design and correct transformations of source
input to target output. Program faults caused by incorrect compiler behavior
can be very difficult to track down and work around; therefore, compiler
implementers invest significant effort to ensure compiler_correctness.[3]
Compilers are not the only language processor used to transform source
programs. An interpreter is computer software that transforms and then executes
the indicated operations.[2]:p2 The translation process influences the design
of computer languages which leads to a preference of compilation or
interpretation. In practice, an interpreter can be implemented for compiled
languages and compilers can be implemented for interpreted languages.
⁰
***** Contents *****
    * 1_History
    * 2_Compiler_construction
          o 2.1_One-pass_versus_multi-pass_compilers
          o 2.2_Three-stage_compiler_structure
                # 2.2.1_Front_end
                # 2.2.2_Middle_end
                # 2.2.3_Back_end
          o 2.3_Compiler_correctness
    * 3_Compiled_versus_interpreted_languages
    * 4_Types
    * 5_See_also
    * 6_Notes
    * 7_References
    * 8_External_links
***** History[edit] *****
Main article: History_of_compiler_construction
A diagram of the operation of a typical multi-language, multi-target compiler
Theoretical computing concepts developed by scientists, mathematicians, and
engineers formed the basis of digital modern computing development during World
War II. Primitive binary languages evolved because digital devices only
understand ones and zeros and the circuit patterns in the underlying machine
architecture. In the late 1940s, assembly languages were created to offer a
more workable abstraction of the computer architectures. Limited memory
capacity of early computers led to substantial technical challenges when the
first compilers were designed. Therefore, the compilation process needed to be
divided into several small programs. The front end programs produce the
analysis products used by the back end programs to generate target code. As
computer technology provided more resources, compiler designs could align
better with the compilation process.
It is usually more productive for a programmer to use a high-level language, so
the development of high-level languages followed naturally from the
capabilities offered by digital computers. High-level languages are formal
languages that are strictly defined by their syntax and semantics which form
the high-level language architecture. Elements of these formal languages
include:
    * Alphabet, any finite set of symbols;
    * String, a finite sequence of symbols;
    * Language, any set of strings on an alphabet.
The sentences in a language may be defined by a set of rules called a grammar.
[4]
BackusâNaur_form (BNF) describes the syntax of "sentences" of a language and
was used for the syntax of Algol 60 by John_Backus.[5] The ideas derive from
the context-free_grammar concepts by Noam_Chomsky, a linguist.[6] "BNF and its
extensions have become standard tools for describing the syntax of programming
notations, and in many cases parts of compilers are generated automatically
from a BNF description."[7]
In the 1940s, Konrad_Zuse designed an algorithmic programming language called
PlankalkÃ¼l ("Plan Calculus"). While no actual implementation occurred until
the 1970s, it presented concepts later seen in APL designed by Ken Iverson in
the late 1950s.[8] APL is a language for mathematical computations.
High-level language design during the formative years of digital computing
provided useful programming tools for a variety of applications:
    * FORTRAN (Formula Translation) for engineering and science applications is
      considered to be the first high-level language.[9]
    * COBOL (Common Business-Oriented Language) evolved from A-0 and FLOW-MATIC
      to become the dominant high-level language for business applications.[10]
    * LISP (List Processor) for symbolic computation.[11]
Compiler technology evolved from the need for a strictly defined transformation
of the high-level source program into a low-level target program for the
digital computer. The compiler could be viewed as a front end to deal with the
analysis of the source code and a back end to synthesize the analysis into the
target code. Optimization between the front end and back end could produce more
efficient target code.[12]
Some early milestones in the development of compiler technology:
    * 1952 â An Autocode compiler developed by Alick_Glennie for the
      Manchester_Mark_I computer at the University of Manchester is considered
      by some to be the first compiled programming language.
    * 1952 â Grace_Hopper's team at Remington_Rand wrote the compiler for the
      A-0 programming language (and coined the term compiler to describe it),
      [13][14] although the A-0 compiler functioned more as a loader or linker
      than the modern notion of a full compiler.
    * 1954-1957 â A team led by John_Backus at IBM developed FORTRAN which is
      usually considered the first high-level language. In 1957, they completed
      a FORTRAN compiler that is generally credited as having introduced the
      first unambiguously complete compiler.
    * 1959 â The Conference on Data Systems Language (CODASYL) initiated
      development of COBOL. The COBOL design drew on A-0 and FLOW-MATIC. By the
      early 1960s COBOL was compiled on multiple architectures.
    * 1958-1962 â John_McCarthy at MIT designed LISP.[15] The symbol
      processing capabilities provided useful features for artificial
      intelligence research. In 1962, LISP 1.5 release noted some tools: an
      interpreter written by Stephen Russell and Daniel J. Edwards, a compiler
      and assembler written by Tim Hart and Mike Levin.[16]
Early operating systems and software were written in assembly language. In the
60s and early 70s, the use of high-level languages for system programming was
still controversial due to resource limitations. However, several research and
industry efforts began the shift toward high-level systems programming
languages, for example, BCPL, BLISS, B, and C.
BCPL (Basic Combined Programming Language) designed in 1966 by Martin_Richards
at the University of Cambridge was originally developed as a compiler writing
tool.[17] Several compilers have been implemented, Richards' book provides
insights to the language and its compiler.[18] BCPL was not only an influential
systems programming language that is still used in research[19] but also
provided a basis for the design of B and C languages.
BLISS (Basic Language for Implementation of System Software) was developed for
a Digital Equipment Corporation (DEC) PDP-10 computer by W.A. Wulf's Carnegie
Mellon University (CMU) research team. The CMU team went on to develop BLISS-11
compiler one year later in 1970.
Multics (Multiplexed Information and Computing Service), a time-sharing
operating system project, involved MIT, Bell_Labs, General_Electric (later
Honeywell) and was led by Fernando_CorbatÃ³ from MIT.[20] Multics was written
in the PL/I language developed by IBM and IBM User Group.[21] IBM's goal was to
satisfy business, scientific, and systems programming requirements. There were
other languages that could have been considered but PL/I offered the most
complete solution even though it had not been implemented.[22] For the first
few years of the Mulitics project, a subset of the language could be compiled
to assembly language with the Early PL/I (EPL) compiler by Doug McIlory and Bob
Morris from Bell Labs.[23] EPL supported the project until a boot-strapping
compiler for the full PL/I could be developed.[24]
Bell Labs left the Multics project in 1969: "Over time, hope was replaced by
frustration as the group effort initially failed to produce an economically
useful system."[25] Continued participation would drive up project support
costs. So researchers turned to other development efforts. A system programming
language B based on BCPL concepts was written by Dennis_Ritchie and Ken
Thompson. Ritchie created a boot-strapping compiler for B and wrote Unics
(Uniplexed Information and Computing Service) operating system for a PDP-7 in
B. Unics eventually became spelled Unix.
Bell Labs started development and expansion of C based on B and BCPL. The BCPL
compiler had been transported to Multics by Bell Labs and BCPL was a preferred
language at Bell Labs.[26] Initially, a front-end program to Bell Labs' B
compiler was used while a C compiler was developed. In 1971, a new PDP-11
provided the resource to define extensions to B and rewrite the compiler. By
1973 the design of C language was essentially complete and the Unix kernel for
a PDP-11 was rewritten in C. Steve Johnson started development of Portable C
Compiler (PCC) to support retargeting of C compilers to new machines.[27][28]
Object-oriented_programming (OOP) offered some interesting possibilities for
application development and maintenance. OOP concepts go further back but were
part of LISP and Simula language science.[29] At Bell Labs, the development of
C++ became interested in OOP.[30] C++ was first used in 1980 for systems
programming. The initial design leveraged C language systems programming
capabilities with Simula concepts. Object-oriented facilities were added in
1983.[31] The Cfront program implemented a C++ front-end for C84 language
compiler. In subsequent years several C++ compilers were developed as C++
popularity grew.
In many application domains, the idea of using a higher-level language quickly
caught on. Because of the expanding functionality supported by newer
programming_languages and the increasing complexity of computer architectures,
compilers became more complex.
DARPA (Defense Advanced Research Projects Agency) sponsored a compiler project
with Wulf's CMU research team in 1970. The Production Quality Compiler-Compiler
PQCC design would produce a Production Quality Compiler (PQC) from formal
definitions of source language and the target.[32] PQCC tried to extend the
term compiler-compiler beyond the traditional meaning as a parser generator
(e.g., Yacc) without much success. PQCC might more properly be referred to as a
compiler generator.
PQCC research into code generation process sought to build a truly automatic
compiler-writing system. The effort discovered and designed the phase structure
of the PQC. The BLISS-11 compiler provided the initial structure.[33] The
phases included analyses (front end), intermediate translation to virtual
machine (middle end), and translation to the target (back end). TCOL was
developed for the PQCC research to handle language specific constructs in the
intermediate representation.[34] Variations of TCOL supported various
languages. The PQCC project investigated techniques of automated compiler
construction. The design concepts proved useful in optimizing compilers and
compilers for the object-oriented programming language Ada.
The Ada Stoneman Document formalized the program support environment (APSE)
along with the kernel (KAPSE) and minimal (MAPSE). An Ada interpreter NYU/ED
supported development and standardization efforts with the American National
Standards Institute (ANSI) and the International Standards Organization (ISO).
Initial Ada compiler development by the U.S. Military Services included the
compilers in a complete integrated design environment along the lines of the
Stoneman Document. Army and Navy worked on the Ada Language System (ALS)
project targeted to DEC/VAX architecture while the Air Force started on the Ada
Integrated Environment (AIE) targeted to IBM 370 series. While the projects did
not provide the desired results, they did contribute to the overal effort on
Ada development.[35]
Other Ada compiler efforts got underway in Britain at the University of York
and in Germany at the University of Karlsruhe. In the U. S., Verdix (later
acquired by Rational) delivered the Verdix Ada Development System (VADS) to the
Army. VADS provided a set of development tools including a compiler. Unix/VADS
could be hosted on a variety of Unix platforms such as DEC Ultrix and the Sun
3/60 Solaris targeted to Motorola 68020 in an Army CECOM evaluation.[36] There
were soon many Ada compilers available that passed the Ada Validation tests.
The Free Software Foundation GNU project developed the GNU_Compiler_Collection
(GCC) which provides a core capability to support multiple languages and
targets. The Ada version GNAT is one of the most widely used Ada compilers.
GNAT is free but there is also commercial support, for example, AdaCore, was
founded in 1994 to provide commercial software solutions for Ada. GNAT Pro
includes the GNU GCC based GNAT with a tool suite to provide an integrated
development_environment.
High-level languages continued to drive compiler research and development.
Focus areas included optimization and automatic code generation. Trends in
programming languages and development environments influenced compiler
technology. More compilers became included in language distributions (PERL,
Java Development Kit) and as a component of an IDE (VADS, Eclipse, Ada Pro).
The interrelationship and interdependence of technologies grew. The advent of
web services promoted growth of web languages and scripting languages. Scripts
trace back to the early days of Command Line Interfaces (CLI) where the user
could enter commands to be executed by the system. User Shell concepts
developed with languages to write shell programs. Early Windows designs offered
a simple batch programming capability. The conventional transformation of these
language used an interpreter. While not widely used, Bash and Batch compilers
have been written. More recently sophisticated interpreted languages became
part of the developers tool kit. Modern scripting languages include PHP,
Python, Ruby and Lua. (Lua is widely used in game development.) All of these
have interpreter and compiler support.[37]
"When the field of compiling began in the late 50s, its focus was limited to
the translation of high-level language programs into machine code ... The
compiler field is increasingly intertwined with other disciplines including
computer architecture, programming languages, formal methods, software
engineering, and computer security."[38] The "Compiler Research: The Next 50
Years" article noted the importance of object-oriented languages and Java.
Security and parallel computing were cited among the future research targets.
***** Compiler construction[edit] *****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (September 2010)(Learn_how_and_when_to_remove_this_template_message)
A compiler implements a formal transformation from a high-level source program
to a low-level target program. Compiler design can define an end to end
solution or tackle a defined subset that interfaces with other compilation
tools e.g. preprocessors, assemblers, linkers. Design requirements include
rigorously defined interfaces both internally between compiler components and
externally between supporting toolsets.
In the early days, the approach taken to compiler design was directly affected
by the complexity of the computer language to be processed, the experience of
the person(s) designing it, and the resources available. Resource limitations
led to the need to pass through the source code more than once.
A compiler for a relatively simple language written by one person might be a
single, monolithic piece of software. However, as the source language grows in
complexity the design may be split into a number of interdependent phases.
Separate phases provide design improvements that focus development on the
functions in the compilation process.
**** One-pass versus multi-pass compilers[edit] ****
Classifying compilers by number of passes has its background in the hardware
resource limitations of computers. Compiling involves performing lots of work
and early computers did not have enough memory to contain one program that did
all of this work. So compilers were split up into smaller programs which each
made a pass over the source (or some representation of it) performing some of
the required analysis and translations.
The ability to compile in a single_pass has classically been seen as a benefit
because it simplifies the job of writing a compiler and one-pass compilers
generally perform compilations faster than multi-pass_compilers. Thus, partly
driven by the resource limitations of early systems, many early languages were
specifically designed so that they could be compiled in a single pass (e.g.,
Pascal).
In some cases the design of a language feature may require a compiler to
perform more than one pass over the source. For instance, consider a
declaration appearing on line 20 of the source which affects the translation of
a statement appearing on line 10. In this case, the first pass needs to gather
information about declarations appearing after statements that they affect,
with the actual translation happening during a subsequent pass.
The disadvantage of compiling in a single pass is that it is not possible to
perform many of the sophisticated optimizations needed to generate high quality
code. It can be difficult to count exactly how many passes an optimizing
compiler makes. For instance, different phases of optimization may analyse one
expression many times but only analyse another expression once.
Splitting a compiler up into small programs is a technique used by researchers
interested in producing provably correct compilers. Proving the correctness of
a set of small programs often requires less effort than proving the correctness
of a larger, single, equivalent program.
**** Three-stage compiler structure[edit] ****
Compiler design
Regardless of the exact number of phases in the compiler design, the phases can
be assigned to one of three stages. The stages include a front end, a middle
end, and a back end.
    * The front end verifies syntax and semantics according to a specific
      source language. For statically_typed_languages it performs type_checking
      by collecting type information. If the input program is syntactically
      incorrect or has a type error, it generates error and/or warning
      messages, usually identifying the location in the source code where the
      problem was detected; in some cases the actual error may be (much)
      earlier in the program. Aspects of the front end include lexical
      analysis, syntax analysis, and semantic analysis. The front end
      transforms the input program into an intermediate_representation (IR) for
      further processing by the middle end. This IR is usually a lower-level
      representation of the program with respect to the source code.
    * The middle end performs optimizations on the IR that are independent of
      the CPU architecture being targeted. This source code/machine code
      independence is intended to enable generic optimizations to be shared
      between versions of the compiler supporting different languages and
      target processors. Examples of middle end optimizations are removal of
      useless (dead_code_elimination) or unreachable code (reachability
      analysis), discovery and propagation of constant values (constant
      propagation), relocation of computation to a less frequently executed
      place (e.g., out of a loop), or specialization of computation based on
      the context. Eventually producing the "optimized" IR that is used by the
      back end.
    * The back end takes the optimized IR from the middle end. It may perform
      more analysis, transformations and optimizations that are specific for
      the target CPU architecture. The back end generates the target-dependent
      assembly code, performing register_allocation in the process. The back
      end performs instruction_scheduling, which re-orders instructions to keep
      parallel execution_units busy by filling delay_slots. Although most
      algorithms for optimization are NP-hard, heuristic techniques are well-
      developed and currently implemented in production-quality compilers.
      Typically the output of a back end is machine code specialized for a
      particular processor and operating system.
This front/middle/back-end approach makes it possible to combine front ends for
different languages with back ends for different CPUs while sharing the
optimizations of the middle end.[39] Practical examples of this approach are
the GNU_Compiler_Collection, LLVM,[40] and the Amsterdam_Compiler_Kit, which
have multiple front-ends, shared optimizations and multiple back-ends.
*** Front end[edit] ***
Lexer and parser example for C. Starting from the sequence of characters "if
(net>0.0)total+=net*(1.0+tax/100.0);", the scanner composes a sequence of
tokens, and categorizes each of them, for example as identifier, reserved word,
number literal, or operator. The latter sequence is transformed by the parser
into a syntax_tree, which is then treated by the remaining compiler phases. The
scanner and parser handles the regular and properly context-free parts of the
grammar_for_C, respectively.
The front end analyzes the source code to build an internal representation of
the program, called the intermediate_representation (IR). It also manages the
symbol_table, a data structure mapping each symbol in the source code to
associated information such as location, type and scope.
While the frontend can be a single monolithic function or program, as in a
scannerless_parser, it is more commonly implemented and analyzed as several
phases, which may execute sequentially or concurrently. This method is favored
due to its modularity and separation_of_concerns. Most commonly today, the
frontend is broken into three phases: lexical_analysis (also known as lexing),
syntax_analysis (also known as scanning or parsing), and semantic_analysis.
Lexing and parsing comprise the syntactic analysis (word syntax and phrase
syntax, respectively), and in simple cases these modules (the lexer and parser)
can be automatically generated from a grammar for the language, though in more
complex cases these require manual modification. The lexical grammar and phrase
grammar are usually context-free_grammars, which simplifies analysis
significantly, with context-sensitivity handled at the semantic analysis phase.
The semantic analysis phase is generally more complex and written by hand, but
can be partially or fully automated using attribute_grammars. These phases
themselves can be further broken down: lexing as scanning and evaluating, and
parsing as building a concrete_syntax_tree (CST, parse tree) and then
transforming it into an abstract_syntax_tree (AST, syntax tree). In some cases
additional phases are used, notably line reconstruction and preprocessing, but
these are rare.
The main phases of the front end include the following:
    * Line reconstruction converts the input character sequence to a canonical
      form ready for the parser. Languages which strop their keywords or allow
      arbitrary spaces within identifiers require this phase. The top-down,
      recursive-descent, table-driven parsers used in the 1960s typically read
      the source one character at a time and did not require a separate
      tokenizing phase. Atlas_Autocode and Imp (and some implementations of
      ALGOL and Coral_66) are examples of stropped languages whose compilers
      would have a Line Reconstruction phase.
    * Preprocessing supports macro substitution and conditional compilation.
      Typically the preprocessing phase occurs before syntactic or semantic
      analysis; e.g. in the case of C, the preprocessor manipulates lexical
      tokens rather than syntactic forms. However, some languages such as
      Scheme support macro substitutions based on syntactic forms.
    * Lexical_analysis (also known as lexing or tokenization) breaks the source
      code text into a sequence of small pieces called lexical tokens.[41] This
      phase can be divided into two stages: the scanning, which segments the
      input text into syntactic units called lexemes and assign them a
      category; and the evaluating, which converts lexemes into a processed
      value. A token is a pair consisting of a token name and an optional token
      value.[42] Common token categories may include identifiers, keywords,
      separators, operators, literals and comments, although the set of token
      categories varies in different programming_languages. The lexeme syntax
      is typically a regular_language, so a finite_state_automaton constructed
      from a regular_expression can be used to recognize it. The software doing
      lexical analysis is called a lexical_analyzer. This may not be a separate
      stepâit can be combined with the parsing step in scannerless_parsing,
      in which case parsing is done at the character level, not the token
      level.
    * Syntax_analysis (also known as parsing) involves parsing the token
      sequence to identify the syntactic structure of the program. This phase
      typically builds a parse_tree, which replaces the linear sequence of
      tokens with a tree structure built according to the rules of a formal
      grammar which define the language's syntax. The parse tree is often
      analyzed, augmented, and transformed by later phases in the compiler.[43]
    * Semantic_analysis adds semantic information to the parse_tree and builds
      the symbol_table. This phase performs semantic checks such as type
      checking (checking for type errors), or object_binding (associating
      variable and function references with their definitions), or definite
      assignment (requiring all local variables to be initialized before use),
      rejecting incorrect programs or issuing warnings. Semantic analysis
      usually requires a complete parse tree, meaning that this phase logically
      follows the parsing phase, and logically precedes the code_generation
      phase, though it is often possible to fold multiple phases into one pass
      over the code in a compiler implementation.
*** Middle end[edit] ***
The middle end, also known as optimizer, performs optimizations on the
intermediate representation in order to improve the performance and the quality
of the produced machine code.[44] The middle end contains those optimizations
that are independent of the CPU architecture being targeted.
The main phases of the middle end include the following:
    * Analysis: This is the gathering of program information from the
      intermediate representation derived from the input; data-flow_analysis is
      used to build use-define_chains, together with dependence_analysis, alias
      analysis, pointer_analysis, escape_analysis, etc. Accurate analysis is
      the basis for any compiler optimization. The control_flow_graph of every
      compiled function and the call_graph of the program are usually also
      built during the analysis phase.
    * Optimization: the intermediate language representation is transformed
      into functionally equivalent but faster (or smaller) forms. Popular
      optimizations are inline_expansion, dead_code_elimination, constant
      propagation, loop_transformation and even automatic_parallelization.
Compiler analysis is the prerequisite for any compiler optimization, and they
tightly work together. For example, dependence_analysis is crucial for loop
transformation.
The scope of compiler analysis and optimizations vary greatly; their scope may
range from operating within a basic_block, to whole procedures, or even the
whole program. There is a trade-off between the granularity of the
optimizations and the cost of compilation. For example, peephole_optimizations
are fast to perform during compilation but only affect a small local fragment
of the code, and can be performed independently of the context in which the
code fragment appears. In contrast, interprocedural_optimization requires more
compilation time and memory space, but enable optimizations which are only
possible by considering the behavior of multiple functions simultaneously.
Interprocedural analysis and optimizations are common in modern commercial
compilers from HP, IBM, SGI, Intel, Microsoft, and Sun_Microsystems. The free
software GCC was criticized for a long time for lacking powerful
interprocedural optimizations, but it is changing in this respect. Another open
source compiler with full analysis and optimization infrastructure is Open64,
which is used by many organizations for research and commercial purposes.
Due to the extra time and space needed for compiler analysis and optimizations,
some compilers skip them by default. Users have to use compilation options to
explicitly tell the compiler which optimizations should be enabled.
*** Back end[edit] ***
The back end is responsible for the CPU architecture specific optimizations and
for code_generation[44].
The main phases of the back end include the following:
    * Machine dependent optimizations: optimizations that depend on the details
      of the CPU architecture that the compiler targets.[45] A prominent
      example is peephole_optimizations, which rewrites short sequences of
      assembler instructions into more efficient instructions.
    * Code_generation: the transformed intermediate language is translated into
      the output language, usually the native machine_language of the system.
      This involves resource and storage decisions, such as deciding which
      variables to fit into registers and memory and the selection and
      scheduling of appropriate machine instructions along with their
      associated addressing_modes (see also Sethi-Ullman_algorithm). Debug data
      may also need to be generated to facilitate debugging.
**** Compiler correctness[edit] ****
Main article: Compiler_correctness
Compiler_correctness is the branch of software engineering that deals with
trying to show that a compiler behaves according to its language_specification.
[46][self-published_source?][non-primary_source_needed] Techniques include
developing the compiler using formal_methods and using rigorous testing (often
called compiler validation) on an existing compiler.
***** Compiled versus interpreted languages[edit] *****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (October 2018)(Learn_how_and_when_to_remove_this_template_message)
Higher-level programming languages usually appear with a type of translation in
mind: either designed as compiled_language or interpreted_language. However, in
practice there is rarely anything about a language that requires it to be
exclusively compiled or exclusively interpreted, although it is possible to
design languages that rely on re-interpretation at run time. The categorization
usually reflects the most popular or widespread implementations of a language
â for instance, BASIC is sometimes called an interpreted language, and C a
compiled one, despite the existence of BASIC compilers and C interpreters.
Interpretation does not replace compilation completely. It only hides it from
the user and makes it gradual. Even though an interpreter can itself be
interpreted, a directly executed program is needed somewhere at the bottom of
the stack (see machine_language).
Further, compilers can contain interpreters for optimization reasons. For
example, where an expression can be executed during compilation and the results
inserted into the output program, then it prevents it having to be recalculated
each time the program runs, which can greatly speed up the final program.
Modern trends toward just-in-time_compilation and bytecode_interpretation at
times blur the traditional categorizations of compilers and interpreters even
further.
Some language specifications spell out that implementations must include a
compilation facility; for example, Common_Lisp. However, there is nothing
inherent in the definition of Common Lisp that stops it from being interpreted.
Other languages have features that are very easy to implement in an
interpreter, but make writing a compiler much harder; for example, APL,
SNOBOL4, and many scripting languages allow programs to construct arbitrary
source code at runtime with regular string operations, and then execute that
code by passing it to a special evaluation_function. To implement these
features in a compiled language, programs must usually be shipped with a
runtime_library that includes a version of the compiler itself.
***** Types[edit] *****
One classification of compilers is by the platform on which their generated
code executes. This is known as the target platform.
A native or hosted compiler is one whose output is intended to directly run on
the same type of computer and operating system that the compiler itself runs
on. The output of a cross_compiler is designed to run on a different platform.
Cross compilers are often used when developing software for embedded_systems
that are not intended to support a software development environment.
The output of a compiler that produces code for a virtual_machine (VM) may or
may not be executed on the same platform as the compiler that produced it. For
this reason such compilers are not usually classified as native or cross
compilers.
The lower level language that is the target of a compiler may itself be a high-
level_programming_language. C, viewed by some as a sort of portable assembly
language, is frequently the target language of such compilers. For example,
Cfront, the original compiler for C++, used C as its target language. The C
code generated by such a compiler is usually not intended to be readable and
maintained by humans, so indent_style and creating pretty C intermediate code
are ignored. Some of the features of C that make it a good target language
include the #line directive, which can be generated by the compiler to support
debugging of the original source, and the wide platform support available with
C compilers.
While a common compiler type outputs machine code, there are many other types:
    * Source-to-source_compilers are a type of compiler that takes a high-level
      language as its input and outputs a high-level language. For example, an
      automatic_parallelizing compiler will frequently take in a high-level
      language program as an input and then transform the code and annotate it
      with parallel code annotations (e.g. OpenMP) or language constructs (e.g.
      Fortran's DOALL statements).
    * Bytecode compilers that compile to assembly language of a theoretical
      machine, like some Prolog implementations
          o This Prolog machine is also known as the Warren_Abstract_Machine
            (or WAM).
          o Bytecode compilers for Java, Python are also examples of this
            category.
    * Just-in-time_compilers (JIT compiler) defer compilation until runtime.
      JIT compilers exist for many modern languages including Python,
      JavaScript, Smalltalk, Java, Microsoft .NET's Common_Intermediate
      Language (CIL) and others. A JIT compiler generally runs inside an
      interpreter. When the interpreter detects that a code path is "hot",
      meaning it is executed frequently, the JIT compiler will be invoked and
      compile the "hot" code for increased performance.
          o For some languages, such as Java, applications are first compiled
            using a bytecode compiler and delivered in a machine-independent
            intermediate_representation. A bytecode interpreter executes the
            bytecode, but the JIT compiler will translate the bytecode to
            machine code when increased performance is necessary.[47][non-
            primary_source_needed]
    * Hardware_compilers (also known as syntheses tools) are compilers whose
      output is a description of the hardware configuration instead of a
      sequence of instructions.
          o The output of these compilers target computer_hardware at a very
            low level, for example a field-programmable_gate_array (FPGA) or
            structured application-specific_integrated_circuit (ASIC).[48][non-
            primary_source_needed] Such compilers are said to be hardware
            compilers, because the source code they compile effectively
            controls the final configuration of the hardware and how it
            operates. The output of the compilation is only an interconnection
            of transistors or lookup_tables.
          o An example of hardware compiler is XST, the Xilinx Synthesis Tool
            used for configuring FPGAs.[49][non-primary_source_needed] Similar
            tools are available from Altera,[50][non-primary_source_needed]
            Synplicity, Synopsys and other hardware vendors.[citation_needed]
    * An assembler is a program that compiles human readable assembly_language
      to machine_code, the actual instructions executed by hardware. The
      inverse program that translates machine code to assembly language is
      called a disassembler.
    * A program that translates from a low-level language to a higher level one
      is a decompiler.[citation_needed]
    * A program that translates between high-level languages is usually called
      a language translator, source-to-source_compiler, language converter, or
      language rewriter.[citation_needed] The last term is usually applied to
      translations that do not involve a change of language.[51]
    * A program that translates into an object code format that is not
      supported on the compilation machine is called a cross_compiler and is
      commonly used to prepare code for embedded applications.[citation_needed]
      [clarification_needed]
    * A program that rewrites object code back into the same type of object
      code while applying optimisations and transformations is a binary
      recompiler.
***** See also[edit] *****
    * [icon]Computer_programming_portal
[icon]     * Book:_Compiler_construction
    * Abstract_interpretation
    * Bottom-up_parsing
    * Compile_and_go_loader
    * Compile_farm
    * List_of_compilers
    * List_of_important_publications_in_computer_science_Â§ Compilers
    * Metacompilation
***** Notes[edit] *****
   1. ^PC Mag Staff (28 February 2017). "Encyclopedia:_Definition_of_Compiler".
      PCMag.com. Retrieved 28 February 2017.
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
   3. ^ a b Compilers:_Principles,_Techniques,_and_Tools by Alfred V. Aho, Ravi
      Sethi, Jeffrey D. Ullman - Second Edition, 2007
   4. ^Sun, Chengnian; Le, Vu; Zhang, Qirun; Su, Zhendong (2016). "Toward
      Understanding_Compiler_Bugs_in_GCC_and_LLVM". ACM.
   5. ^ lecture notes Compilers: Principles, Techniques, and Tools Jing-Shin
      Chang Department of Computer Science & Information Engineering National
      Chi-Nan University
   6. ^ Naur, P. et al. "Report on ALGOL 60". Communications of the ACM 3 (May
      1960), 299â314.
   7. ^Chomsky, Noam; Lightfoot, David W. (2002). Syntactic Structures. Walter
      de Gruyter. ISBN 978-3-11-017279-9.
   8. ^Gries, David (2012). "Appendix_1:_Backus-Naur_Form". The Science of
      Programming. Springer Science & Business Media. p. 304. ISBN 978-
      1461259831.
   9. ^Iverson, Kenneth E. (1962). A Programming Language. John Wiley & Sons.
      ISBN 978-0-471430-14-8.
  10. ^Backus, John. "The_history_of_FORTRAN_I,_II_and_III" (PDF). History of
      Programming Languages. Softwarepreservation.org.
  11. ^ Porter Adams, Vicki (5 October 1981). "Captain Grace M. Hopper: the
      Mother of COBOL". InfoWorld. 3 (20): 33. ISSN 0199-6649.
  12. ^ McCarthy, J.; Brayton, R.; Edwards, D.; Fox, P.; Hodes, L.; Luckham,
      D.; Maling, K.; Park, D.; Russell, S. (March 1960). "LISP I Programmers
      Manual" (PDF). Boston, Massachusetts: Artificial Intelligence Group,
      M.I.T. Computation Center and Research Laboratory.
  13. ^ Compilers Principles, Techniques, & Tools 2nd edition by Aho, Lam,
      Sethi, Ullman
  14. ISBN 0-321-48681-1
  15. ^Hopper, Grace Murray (1952). "The Education of a Computer". Proceedings
      of the 1952 ACM National Meeting (Pittsburgh): 243â249. doi:10.1145/
      609784.609818.
  16. ^Ridgway, Richard K. (1952). "Compiling routines". Proceedings of the
      1952 ACM National Meeting (Toronto): 1â5. doi:10.1145/800259.808980.
  17. ^ "Recursive_Functions_of_Symbolic_Expressions_and_Their_Computation_by
      Machine", Communications of the ACM, April 1960
  18. ^McCarthy, John; Abrahams, Paul W.; Edwards, Daniel J.; Hart, Timothy P.;
      Levin, Michael I. (1965). Lisp_1.5_Programmers_Manual. The MIT Press.
      ISBN 9780262130110.
  19. ^ "BCPL:_A_tool_for_compiler_writing_and_system_programming" M. Richards,
      University Mathematical Laboratory Cambridge, England 1969
  20. ^ BCPL: The Language and Its Compiler, M Richards, Cambridge University
      Press (first published 31 December 1981)
  21. ^ The BCPL Cintsys and Cintpos User Guide, M. Richards, 2017
  22. ^CorbatÃ³, F. J.; Vyssotsky, V. A. "Introduction_and_Overview_of_the
      MULTICS_System". 1965 Fall Joint Computer Conference. Multicians.org.
  23. ^ Report II of the SHARE Advanced Language Development Committee, 25 June
      1964
  24. ^ Multicians.org "The Choice of PL/I" article, Editor /tom Van Vleck
  25. ^ "PL/I As a Tool for System Programming", F.J. Corbato, Datamation May
      6, 1969 issue
  26. ^ "The_Multics_PL/1_Compiler", R. A. Freiburghouse, GE, Fall Joint
      Computer Conference 1969
  27. ^ Datamation column, 1969
  28. ^ Dennis M. Ritchie, "The_Development_of_the_C_Language", ACM Second
      History of Programming Languages Conference, April 1993
  29. ^ S.C. Johnson, "a Portable C Compiler: Theory and Practice", 5th ACM
      POPL Symposium, January 1978
  30. ^ A. Snyder, A_Portable_Compiler_for_the_Language_C, MIT, 1974.
  31. ^ K. Nygarard, University of Oslo, Norway, "Basic_Concepts_in_Object
      Oriented_Programming", SIGPLAN Notices V21, 1986
  32. ^ B. Stroustrup: "What is Object-Oriented Programming?" Proceedings 14th
      ASU Conference, 1986.
  33. ^ Bjarne Stroustrup, "An Overview of the C++ Programming Language",
      Handbook of Object Technology (Editor: Saba Zamir,
  34. ISBN 0-8493-3135-8)
  35. ^ Leverett, Cattell, Hobbs, Newcomer, Reiner, Schatz, Wulf: "An Overview
      of the Production Quality Compiler-Compiler Project", CMU-CS-89-105, 1979
  36. ^ W. Wulf, K. Nori, "Delayed_binding_in_PQCC_generated_compilers", CMU
      Research Showcase Report, CMU-CS-82-138, 1982
  37. ^ Joseph M. Newcomer, David Alex Lamb, Bruce W. Leverett, Michael Tighe,
      William A. Wulf - Carnegie-Mellon University and David Levine, Andrew H.
      Reinerit - Intermetrics: "TCOL Ada: Revised Report on An Intermediate
      Representation for the DOD Standard Programming Language", 1979
  38. ^ William A. Whitaker, "Ada - the project: the DoD High Order Working
      Group", ACM SIGPLAN Notices (Volume 28, No. 3, March 1991)
  39. ^ CECOM Center for Software Engineering Advanced Software Technology,
      "Final Report - Evaluation of the ACEC Benchmark Suite for Real-Time
      Applications", AD-A231 968, 1990
  40. ^ P.Biggar, E. de Vries, D. Gregg, "A Practical Solution for Scripting
      Language Compilers", submission to Science of Computer Programming, 2009
  41. ^ M.Hall, D. Padua, K. Pingali, "Compiler Research: The Next 50 Years",
      ACM Communications 2009 Vol 54 #2
  42. ^ Cooper and Torczon 2012, p. 8
  43. ^Lattner, Chris (2017). "LLVM". In Brown, Amy; Wilson, Greg (eds.). The
      Architecture of Open Source Applications. Archived from the original on 2
      December 2016. Retrieved 28 February 2017.
  44. ^ Aho, Lam, Sethi, Ullman 2007, p. 5-6, 109-189
  45. ^ Aho, Lam, Sethi, Ullman 2007, p. 111
  46. ^ Aho, Lam, Sethi, Ullman 2007, p. 8, 191-300
  47. ^ a bBlindell, Gabriel Hjort (3 June 2016). Instruction selection :
      principles, methods, and applications. Switzerland. ISBN 9783319340197.
      OCLC 951745657.
  48. ^ Cooper and Toczon (2012), p. 540
  49. ^Chlipala, Adam. "Syntactic_Proofs_of_Compositional_Compiler_Correctness"
      (manuscript draft, publication date unknown). Archived (PDF) from the
      original on 29 August 2017. Retrieved 28 February 2017 – via
      Adam.Chlipala.net.
  50. [self-published_source?][non-primary_source_needed]
  51. ^Aycock, John (2003). "A Brief History of Just-in-Time". ACM Comput.
      Surv. 35 (2, June): 93â113. doi:10.1145/857076.857077.
  52. [non-primary_source_needed]
  53. ^Swartz, Jordan S.; Betz, Vaugh; Rose, Jonathan (22â25 February 1998).
      "A_Fast_Routability-Driven_Router_for_FPGAs" (PDF). FPGA '98 Proceedings
      of the 1998 ACM/SIGDA Sixth International Symposium on Field Programmable
      Gate Arrays. Monterey, CA: ACM: 140â149. doi:10.1145/275107.275134.
      ISBN 978-0897919784. Archived (PDF) from the original on 9 August 2017.
  54. ^Xilinx Staff (2009). "XST_Synthesis_Overview". Xilinx, Inc. Archived
      from the original on 2 November 2016. Retrieved 28 February 2017.
  55. [non-primary_source_needed]
  56. ^Altera Staff (2017). "Spectra-Qâ¢_Engine". Altera.com. Archived from
      the_original on 10 October 2016. Retrieved 28 February 2017.
  57. [non-primary_source_needed]
  58. ^"Language_Translator_Tutorial" (PDF). Washington University.
***** References[edit] *****
    * LLVM community. "The_LLVM_Target-Independent_Code_Generator". LLVM
      Documentation. Retrieved 17 June 2016.
Compiler_textbook_references A collection of references to mainstream Compiler
Construction Textbooks
Aho,_Alfred_V.; Sethi,_Ravi; Ullman,_Jeffrey_D. (1986). Compilers:_Principles,
Techniques,_and_Tools (1st ed.). Addison-Wesley. ISBN 9780201100884.
Allen,_Frances_E. (September 1981). "A History of Language Processor Technology
in IBM". IBM Journal of Research and Development. IBM. 25 (5): 535â548. doi:
10.1147/rd.255.0535.
Allen, Randy; Kennedy,_Ken (2001). Optimizing Compilers for Modern
Architectures. Morgan_Kaufmann_Publishers. ISBN 978-1-55860-286-1.
Appel,_Andrew_Wilson (2002). Modern Compiler Implementation in Java (2nd ed.).
Cambridge_University_Press. ISBN 978-0-521-82060-8.
Appel,_Andrew_Wilson (1998). Modern_Compiler_Implementation_in_ML. Cambridge
University_Press. ISBN 978-0-521-58274-2.
Bornat,_Richard (1979). Understanding_and_Writing_Compilers:_A_Do_It_Yourself
Guide (PDF). Macmillan_Publishing. ISBN 978-0-333-21732-0.
Cooper, Keith Daniel; Torczon, Linda (2012). Engineering a compiler (2nd ed.).
Amsterdam: Elsevier/Morgan Kaufmann. p. 8. ISBN 9780120884780. OCLC 714113472.
McKeeman,_William_Marshall; Horning,_James_J.; Wortman, David B. (1970). A
Compiler_Generator. Englewood_Cliffs,_NJ: Prentice-Hall. ISBN 978-0-13-155077-
3.
Muchnick,_Steven (1997). Advanced_Compiler_Design_and_Implementation. Morgan
Kaufmann_Publishers. ISBN 978-1-55860-320-2.
Scott,_Michael_Lee (2005). Programming_Language_Pragmatics (2nd ed.). Morgan
Kaufmann. ISBN 978-0-12-633951-2.
Srikant, Y. N.; Shankar, Priti (2003). The_Compiler_Design_Handbook:
Optimizations_and_Machine_Code_Generation. CRC_Press. ISBN 978-0-8493-1240-3.
Terry, Patrick D. (1997). Compilers_and_Compiler_Generators:_An_Introduction
with_C++. International Thomson Computer Press. ISBN 978-1-85032-298-6.
Wirth,_Niklaus (1996). Compiler_Construction (PDF). Addison-Wesley. ISBN 978-0-
201-40353-4.
***** External links[edit] *****
 Look up compiler in Wiktionary, the free dictionary.
 Wikibooks has a book on the topic of: Compiler_Construction
 Wikimedia Commons has media related to Compilers.
    * Compilers at Curlie
    * Incremental_Approach_to_Compiler_Construction – a PDF tutorial
    * Compile-Howto
    * Basics_of_Compiler_Design at the Wayback_Machine (archived 2018-05-15)
    * Short_animation on YouTube explaining the key conceptual difference
      between compilers and interpreters
    * Syntax_Analysis_&_LL1_Parsing on YouTube
    * Let's_Build_a_Compiler, by Jack Crenshaw
    * Forum_about_compiler_development at the Wayback_Machine (archived 2014-
      10-10)
    * Difference_Between_Compiler_and_Interpreter
                                              * BNE: XX532454
                                              * BNF: cb120631538 (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4148248-7
                                              * LCCN: sh86007588
                                              * NDL: 01191219

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Compiler&oldid=907829368"
Categories:
    * American_inventions
    * Compilers
    * Compiler_construction
    * Computer_libraries
    * Programming_language_implementation
    * Utility_software_types
Hidden categories:
    * All_articles_with_self-published_sources
    * Articles_with_self-published_sources_from_March_2017
    * All_pages_needing_factual_verification
    * Wikipedia_articles_needing_factual_verification_from_March_2017
    * Use_dmy_dates_from_July_2012
    * Articles_needing_additional_references_from_September_2010
    * All_articles_needing_additional_references
    * Articles_needing_additional_references_from_October_2018
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_March_2017
    * Wikipedia_articles_needing_clarification_from_February_2017
    * Commons_category_link_is_on_Wikidata
    * Articles_with_Curlie_links
    * Webarchive_template_wayback_links
    * Wikipedia_articles_with_BNE_identifiers
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
    * AzÉrbaycanca
    * ØªÛØ±Ú©Ø¬Ù
    * à¦¬à¦¾à¦à¦²à¦¾
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
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
    * Gaeilge
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hornjoserbsce
    * Hrvatski
    * Ilokano
    * Bahasa_Indonesia
    * Interlingua
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * Latina
    * LatvieÅ¡u
    * LÃ«tzebuergesch
    * LietuviÅ³
    * Lingua_Franca_Nova
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * MirandÃ©s
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * áá¼ááºáá¬áá¬áá¬
    * Nederlands
    * à¤¨à¥à¤ªà¤¾à¤²à¥
    * æ¥æ¬èª
    * Norsk
    * ÐÐ»ÑÐº_Ð¼Ð°ÑÐ¸Ð¹
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Ù¾ÙØ¬Ø§Ø¨Û
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * à°¤à±à°²à±à°à±
    * à¹à¸à¸¢
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * Winaray
    * å´è¯­
    * ××Ö´×××©
    * ç²µèª
    * Zazaki
    * ä¸­æ
Edit_links
    * This page was last edited on 25 July 2019, at 15:07 (UTC).
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
