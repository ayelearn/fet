The following text has been accessed from https://en.wikipedia.org/wiki/Runtime_system at Fri Aug 9 01:12:21 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Runtime system ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the infrastructure required to run programs. For the
execution phase of software applications, see Run_time_(program_lifecycle
phase).
Program_execution
General concepts
    * Code
    * Translation
          o Compiler
                # Compile-time
          o Optimizing_compiler
    * Intermediate_representation (IR)
    * Execution
          o Runtime system
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
A runtime system, also called run-time system, runtime environment or run-time
environment, primarily implements portions of an execution_model. This is not
to be confused with the runtime lifecycle phase of a program, during which the
runtime system is in operation. Most languages have some form of runtime system
that provides an environment in which programs run. This environment may
address a number of issues including the layout of application memory, how the
program accesses variables, mechanisms for passing parameters between
procedures, interfacing with the operating system, and otherwise. The compiler
makes assumptions depending on the specific runtime system to generate correct
code. Typically the runtime system will have some responsibility for setting up
and managing the stack and heap, and may include features such as garbage
collection, threads or other dynamic features built into the language.[1]
⁰
***** Contents *****
    * 1_Overview
    * 2_Examples
    * 3_Advanced_features
    * 4_History
    * 5_See_also
    * 6_References
***** Overview[edit] *****
Every programming language specifies an execution model, and many implement at
least part of that model in a runtime system. One possible definition of
runtime system behavior is, among others, any behavior not directly
attributable to the program itself. This definition includes, as part of the
runtime system, things such as putting parameters onto the stack before a
function call, the behavior of disk I/O, and parallel execution of related
behaviors.
By this definition, essentially every language has a runtime system, including
compiled_languages, interpreted_languages, and embedded_domain-specific
languages. Even API invoked stand alone execution models such as Pthreads have
a runtime system that is the implementation of execution model's behavior.
Most scholarly papers on runtime systems focus on the implementation details of
parallel runtime systems. A notable example of a parallel runtime system is
that of Cilk, a popular parallel programming model.[2] In addition, the proto-
runtime toolkit was created to simplify the creation of parallel runtime
systems.[3]
In addition to the execution model behavior, a runtime system may also perform
support services such as type_checking, debugging, or code_generation and
optimization.[4]
The runtime system is also the gateway by which a running program interacts
with the runtime environment, which contains not only state values that are
accessible during program execution, but also active entities that can be
interacted with during program execution like disk drives and people via
keyboards. For example, environment_variables are features of many operating
systems, and are part of the runtime environment; a running program can access
them via the runtime system. Likewise, hardware devices such as a DVD drive are
active entities that a program can interact with via a runtime system.
A unique application of a runtime environment (RTE) is within an operating
system (OS) that only allows that RTE to run, meaning from boot until power-
down the entire OS is dedicated to only the application(s) running within that
RTE. Any other code that tries to run or any failures in the application(s)
break the RTE which breaks the OS which stops all processing and requires a re-
boot. If the boot is from read-only memory, an extremely secure, simple,
single-mission system is created.
***** Examples[edit] *****
As a simple example of a basic runtime system, the runtime system of the C
language is a particular set of instructions inserted into the executable image
by the compiler. Among other things, these instructions manage the processor
stack, create space for local variables, and copy function-call parameters onto
the top of the stack. There are often no clear criteria for deciding which
language behavior is considered inside the runtime system versus which behavior
is part of the source program. For C, the setup of the stack is part of the
runtime system, as opposed to part of the semantics of an individual program,
because it maintains a global invariant that holds over all executions. This
systematic behavior implements the execution_model of the language, as opposed
to implementing semantics of the particular program text which is directly
translated into code that computes results.
One way to observe this separation between the semantics of a particular
program and the runtime environment is to compile a program into an object_file
containing all the functions versus compiling an entire program to an
executable binary. The object file will only contain assembly code relevant to
those functions, while the executable binary will contain additional code used
to implement the runtime environment. The object file, on one hand, may be
missing information from the runtime environment that will be resolved by
linking. On the other hand, the code in the object file still depends on
assumptions in the runtime system; for example, a function may read parameters
from a particular register or stack location, depending on the calling
convention used by the runtime environment.
Another example is the case of using an application_programming_interface (API)
to interact with a runtime system. The calls to that API look the same as calls
to a regular software_library, however at some point during the call the
execution model changes. The runtime system implements an execution model
different from that of the language the library is written in terms of. A
person reading the code of a normal library would be able to understand the
library's behavior by just knowing the language the library was written in.
However, a person reading the code of the API that invokes a runtime system
would not be able to understand the behavior of the API call just by knowing
the language the call was written in. At some point, via some mechanism, the
execution model stops being that of the language the call is written in and
switches over to being the execution model implemented by the runtime system.
For example, the trap instruction is one method of switching execution models.
This difference is what distinguishes an API-invoked execution model, such as
POSIX threads, from a usual software library. Both POSIX threads calls and
software library calls are invoked via an API, but POSIX threads behavior
cannot be understood in terms of the language of the call. Rather, POSIX
threads calls bring into play an outside execution model, which is implemented
by the POSIX threads runtime system (this runtime system is often the OS
kernel).
As an extreme example, the physical CPU itself can be viewed as an
implementation of the runtime system of a specific assembly language. In this
view, the execution model is implemented by the physical CPU and memory
systems. As an analogy, runtime systems for higher-level languages are
themselves implemented using some other languages. This creates a hierarchy of
runtime systems, with the CPU itselfâor actually its logic at the microcode
layer or belowâacting as the lowest-level runtime system.
***** Advanced features[edit] *****
Some compiled or interpreted languages provide an interface that allows
application code to interact directly with the runtime system. An example is
the Thread class in the Java_language. The class allows code (that is animated
by one thread) to do things such as start and stop other threads. Normally,
core aspects of a language's behavior such as task_scheduling and resource
management are not accessible in this fashion.
Higher-level behaviors implemented by a runtime system may include tasks such
as drawing text on the screen or making an Internet connection. It is often the
case that operating_systems provide these kinds of behaviors as well, and when
available, the runtime system is implemented as an abstraction_layer that
translates the invocation of the runtime system into an invocation of the
operating system. This hides the complexity or variations in the services
offered by different operating systems. This also implies that the OS kernel
can itself be viewed as a runtime system, and that the set of OS calls that
invoke OS behaviors may be viewed as interactions with a runtime system.
In the limit, the runtime system may provide services such as a P-code_machine
or virtual_machine, that hide even the processor's instruction_set. This is the
approach followed by many interpreted_languages such as AWK, and some languages
like Java, which are meant to be compiled into some machine-independent
intermediate_representation code (such as bytecode). This arrangement
simplifies the task of language implementation and its adaptation to different
machines, and improves efficiency of sophisticated language features such as
reflection. It also allows the same program to be executed on any machine
without an explicit recompiling step, a feature that has become very important
since the proliferation of the World_Wide_Web. To speed up execution, some
runtime systems feature just-in-time_compilation to machine code.
A modern aspect of runtime systems is parallel execution behaviors, such as the
behaviors exhibited by mutex constructs in Pthreads and parallel section
constructs in OpenMP. A runtime system with such parallel execution behaviors
may be modularized according to the proto-runtime approach.
***** History[edit] *****
Notable early examples of runtime systems are the interpreters for BASIC and
Lisp. These environments also included a garbage_collector. Forth is an early
example of a language designed to be compiled into intermediate representation
code; its runtime system was a virtual machine that interpreted that code.
Another popular, if theoretical, example is Donald_Knuth's MIX computer.
In C and later languages that supported dynamic memory allocation, the runtime
system also included a library that managed the program's memory pool.
In the object-oriented_programming_languages, the runtime system was often also
responsible for dynamic type checking and resolving method references.
***** See also[edit] *****
 Look up run-time in Wiktionary, the free dictionary.
    * Run_time_(program_lifecycle_phase)
    * Execution_model
    * Programming_model
***** References[edit] *****
   1. ^Aho, Alfred V.; Lam, Monica S.; Sethi, Ravi; Ullman, Jeffrey D. (2007).
      Compilers: Principles, Techniques and Tools (2nd ed.). Boston, MA:
      Pearson Education. p. 427. ISBN 978-0-321-48681-3.
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
   3. ^Blumofe, Robert D.; et al. (1995). "Cilk:_An_efficient_multithreaded
      runtime_system". ACM.
   4. ^Open Source Research Institute; et al. (2011). "The_Proto-Runtime
      Toolkit".
   5. ^Andrew W. Appel (May 1989). "A_Runtime_System" (PDF). Princeton
      University. Archived from the_original (PDF) on 2013-12-30. Retrieved
      2013-12-30.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Runtime_system&oldid=902042345"
Categories:
    * Computing_platforms
    * Run-time_systems
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
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * Italiano
    * Magyar
    * æ¥æ¬èª
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * TÃ¼rkÃ§e
    * ä¸­æ
Edit_links
    * This page was last edited on 16 June 2019, at 03:41 (UTC).
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
