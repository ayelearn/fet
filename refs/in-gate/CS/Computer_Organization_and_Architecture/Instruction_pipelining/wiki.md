The following text has been accessed from https://en.wikipedia.org/wiki/Instruction_pipelining at Fri Aug 9 01:11:03 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Instruction pipelining ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
method of improving instruction-level parallelism
 It has been suggested that Simultaneous_multithreading be merged into this
 article. (Discuss)Proposed since January 2019.
 This article needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be challenged
 and removed.
 Find sources: "Instruction_pipelining" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (May 2016)(Learn_how_and_when_to_remove_this_template_message)
                      Basic_five-stage_pipeline
Clock cycle 1  2  3  4   5   6   7
Instr. No.
1           IF ID EX MEM WB
2              IF ID EX  MEM WB
3                 IF ID  EX  MEM WB
4                    IF  ID  EX  MEM
5                        IF  ID  EX
(IF = Instruction Fetch, ID = Instruction Decode, EX = Execute, MEM =
Memory access, WB = Register write back).
In the fourth clock cycle (the green column), the earliest instruction
is in MEM stage, and the latest instruction has not yet entered the
pipeline.
In computer_science, instruction pipelining is a technique for implementing
instruction-level_parallelism within a single processor. Pipelining attempts to
keep every part of the processor busy with some instruction by dividing
incoming instructions into a series of sequential steps (the eponymous
"pipeline") performed by different processor_units with different parts of
instructions processed in parallel. It allows faster CPU throughput than would
otherwise be possible at a given clock_rate, but may increase latency due to
the added overhead of the pipelining process itself.
⁰
***** Contents *****
    * 1_Concept_and_motivation
          o 1.1_Number_of_steps
    * 2_History
          o 2.1_Hazards
                # 2.1.1_Workarounds
                # 2.1.2_Solutions
          o 2.2_Branches
          o 2.3_Special_situations
    * 3_Design_considerations
    * 4_Illustrated_example
          o 4.1_Pipeline_bubble
    * 5_See_also
    * 6_Notes
    * 7_References
    * 8_External_links
***** Concept and motivation[edit] *****
Central_processing_units (CPUs) are driven by a clock. Each clock pulse need
not do the same thing; rather, logic in the CPU directs successive pulses to
different places to perform a useful sequence. There are many reasons that the
entire execution of a machine instruction cannot happen at once; in pipelining,
effects that cannot happen at the same time are made into dependent steps of
the instruction.
For example, if one clock pulse latches a value into a register or begins a
calculation, it will take some time for the value to be stable at the outputs
of the register or for the calculation to complete. As another example, reading
an instruction out of a memory unit cannot be done at the same time that an
instruction writes a result to the same memory unit.
**** Number of steps[edit] ****
The number of dependent steps varies with the machine architecture. For
example:
    * The 1956â1961 IBM_Stretch project proposed the terms Fetch, Decode, and
      Execute that have become common.
    * The classic_RISC_pipeline comprises:
         1. Instruction fetch
         2. Instruction decode and register fetch
         3. Execute
         4. Memory access
         5. Register write back
    * The Atmel_AVR and the PIC_microcontroller each have a two-stage pipeline.
    * Many designs include pipelines as long as 7, 10 and even 20 stages (as in
      the Intel Pentium_4).
    * The later "Prescott" and "Cedar Mill" Netburst cores from Intel, used in
      the last Pentium 4 models and their Pentium_D and Xeon derivatives, have
      a long 31-stage pipeline.
    * The Xelerated X10q Network Processor has a pipeline more than a thousand
      stages long, although in this case 200 of these stages represent
      independent CPUs with individually programmed instructions. The remaining
      stages are used to coordinate accesses to memory and on-chip function
      units.[1]
As the pipeline is made "deeper" (with a greater number of dependent steps), a
given step can be implemented with simpler circuitry, which may let the
processor clock run faster.[2] Such pipelines may be called superpipelines.[3]
A processor is said to be fully pipelined if it can fetch an instruction on
every cycle. Thus, if some instructions or conditions require delays that
inhibit fetching new instructions, the processor is not fully pipelined.
***** History[edit] *****
 This section needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be challenged
 and removed.
 Find sources: "Instruction_pipelining" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (March 2019)(Learn_how_and_when_to_remove_this_template_message)
Seminal uses of pipelining were in the ILLIAC_II project and the IBM_Stretch
project, though a simple version was used earlier in the Z1 in 1939 and the Z3
in 1941.[4]
Pipelining began in earnest in the late 1970s in supercomputers such as vector
processors and array processors.[citation_needed] One of the early
supercomputers was the Cyber series built by Control Data Corporation. Its main
architect, Seymour_Cray, later headed Cray Research. Cray developed the XMP
line of supercomputers, using pipelining for both multiply and add/subtract
functions. Later, Star Technologies added parallelism (several pipelined
functions working in parallel), developed by Roger Chen. In 1984, Star
Technologies added the pipelined divide circuit developed by James Bradley. By
the mid-1980s, pipelining was used by many different companies around the
world.[citation_needed]
Pipelining was not limited to supercomputers. In 1976, the Amdahl_Corporation's
470 series general purpose mainframe had a 7-step pipeline, and a patented
branch prediction circuit.[citation_needed]
Today, pipelining and most of the above innovations are implemented by the
instruction_unit of most microprocessors.[citation_needed]
**** Hazards[edit] ****
Main article: Hazard_(computer_architecture)
The model of sequential execution assumes that each instruction completes
before the next one begins; this assumption is not true on a pipelined
processor. A situation where the expected result is problematic is known as a
hazard. Imagine the following two register instructions to a hypothetical
processor:
1: add 1 to R5
2: copy R5 to R6
If the processor has the 5 steps listed in the initial illustration,
instruction 1 would be fetched at time t1 and its execution would be complete
at t5. Instruction 2 would be fetched at t2 and would be complete at t6. The
first instruction might deposit the incremented number into R5 as its fifth
step (register write back) at t5. But the second instruction might get the
number from R5 (to copy to R6) in its second step (instruction decode and
register fetch) at time t3. It seems that the first instruction would not have
incremented the value by then. The above code invokes a hazard.
Writing computer programs in a compiled language might not raise these
concerns, as the compiler could be designed to generate machine code that
avoids hazards.
*** Workarounds[edit] ***
In some early DSP and RISC processors, the documentation advises programmers to
avoid such dependencies in adjacent and nearly adjacent instructions (called
delay_slots), or declares that the second instruction uses an old value rather
than the desired value (in the example above, the processor might counter-
intuitively copy the unincremented value), or declares that the value it uses
is undefined. The programmer may have unrelated work that the processor can do
in the meantime; or, to ensure correct results, the programmer may insert NOPs
into the code, partly negating the advantages of pipelining.
*** Solutions[edit] ***
Pipelined processors commonly use three techniques to work as expected when the
programmer assumes that each instruction completes before the next one begins:
    * Processors that can compute the presence of a hazard may stall[definition
      needed], delaying processing of the second instruction (and subsequent
      instructions) until the values it requires as input are ready. This
      creates a bubble[definition_needed] in the pipeline, also partly negating
      the advantages of pipelining.
    * Some processors can not only compute the presence of a hazard but can
      compensate by having additional data paths that provide needed inputs to
      a computation step before a subsequent instruction would otherwise
      compute them, an attribute called operand_forwarding.[5][6]
    * Some processors can determine that instructions other than the next
      sequential one are not dependent on the current ones and can be executed
      without hazards. Such processors may perform out-of-order_execution.
**** Branches[edit] ****
A branch out of the normal instruction sequence often involves a hazard. Unless
the processor can give effect to the branch in a single time cycle, the
pipeline will continue fetching instructions sequentially. Such instructions
cannot be allowed to take effect because the programmer has diverted control to
another part of the program.
A conditional branch is even more problematic. The processor may or may not
branch, depending on a calculation that has not yet occurred. Various
processors may stall, may attempt branch_prediction, and may be able to begin
to execute two different program sequences (eager_execution), both assuming the
branch is and is not taken, discarding all work that pertains to the incorrect
guess.[a]
A processor with an implementation of branch prediction that usually makes
correct predictions can minimize the performance penalty from branching.
However, if branches are predicted poorly, it may create more work for the
processor, such as flushing_from_the_pipeline the incorrect code path that has
begun execution before resuming execution at the correct location.
Programs written for a pipelined processor deliberately avoid branching to
minimize possible loss of speed. For example, the programmer can handle the
usual case with sequential execution and branch only on detecting unusual
cases. Using programs such as gcov to analyze code_coverage lets the programmer
measure how often particular branches are actually executed and gain insight
with which to optimize the code.
**** Special situations[edit] ****
  Self-modifying programs
      The technique of self-modifying_code can be problematic on a pipelined
      processor. In this technique, one of the effects of a program is to
      modify its own upcoming instructions. If the processor has an instruction
      cache, the original instruction may already have been copied into a
      prefetch_input_queue and the modification will not take effect. Some
      processors such as the Zilog_Z280 can configure their on-chip cache
      memories for data-only fetches, or as part of their ordinary memory
      address space, and avoid such difficulties with self-modifying
      instructions.
  Uninterruptible instructions
      An instruction may be uninterruptible to ensure its atomicity, such as
      when it swaps two items. A sequential processor permits interrupts
      between instructions, but a pipelining processor overlaps instructions,
      so executing an uninterruptible instruction renders portions of ordinary
      instructions uninterruptible too. The Cyrix_coma_bug would hang a single-
      core system using an infinite loop in which an uninterruptible
      instruction was always in the pipeline.
***** Design considerations[edit] *****
  Speed
      Pipelining keeps all portions of the processor occupied and increases the
      amount of useful work the processor can do in a given time. Pipelining
      typically reduces the processor's cycle time and increases the throughput
      of instructions. The speed advantage is diminished to the extent that
      execution encounters hazards that require execution to slow below its
      ideal rate. A non-pipelined processor executes only a single instruction
      at a time. The start of the next instruction is delayed not based on
      hazards but unconditionally.
      A pipelined processor's need to organize all its work into modular steps
      may require the duplication of registers, which increases the latency of
      some instructions.
  Economy
      By making each dependent step simpler, pipelining can enable complex
      operations more economically than adding complex circuitry, such as for
      numerical calculations. However, a processor that declines to pursue
      increased speed with pipelining may be simpler and cheaper to
      manufacture.
  Predictability
      Compared to environments where the programmer needs to avoid or work
      around hazards, use of a non-pipelined processor may make it easier to
      program and to train programmers. The non-pipelined processor also makes
      it easier to predict the exact timing of a given sequence of
      instructions.
***** Illustrated example[edit] *****
To the right is a generic pipeline with four stages: fetch, decode, execute and
write-back. The top gray box is the list of instructions waiting to be
executed, the bottom gray box is the list of instructions that have had their
execution completed, and the middle white box is the pipeline.
The execution is as follows:
Generic 4-stage pipeline; the colored boxes represent instructions independent
of each other
Clock Execution
0         * Four instructions are waiting to be executed
1         * The green instruction is fetched from memory
2         * The green instruction is decoded
          * The purple instruction is fetched from memory
          * The green instruction is executed (actual operation is performed)
3         * The purple instruction is decoded
          * The blue instruction is fetched
          * The green instruction's results are written back to the register
            file or memory
4         * The purple instruction is executed
          * The blue instruction is decoded
          * The red instruction is fetched
          * The execution of green instruction is completed
5         * The purple instruction is written back
          * The blue instruction is executed
          * The red instruction is decoded
          * The execution of purple instruction is completed
6         * The blue instruction is written back
          * The red instruction is executed
7         * The execution of blue instruction is completed
          * The red instruction is written back
8         * The execution of red instruction is completed
9         * The execution of all four instructions is completed
**** Pipeline bubble[edit] ****
Main article: Bubble_(computing)
A bubble in cycle 3 delays execution.
A pipelined processor may deal with hazards by stalling and creating a bubble
in the pipeline, resulting in one or more cycles in which nothing useful
happens.
In the illustration at right, in cycle 3, the processor cannot decode the
purple instruction, perhaps because the processor determines that decoding
depends on results produced by the execution of the green instruction. The
green instruction can proceed to the Execute stage and then to the Write-back
stage as scheduled, but the purple instruction is stalled for one cycle at the
Fetch stage. The blue instruction, which was due to be fetched during cycle 3,
is stalled for one cycle, as is the red instruction after it.
Because of the bubble (the blue ovals in the illustration), the processor's
Decode circuitry is idle during cycle 3. Its Execute circuitry is idle during
cycle 4 and its Write-back circuitry is idle during cycle 5.
When the bubble moves out of the pipeline (at cycle 6), normal execution
resumes. But everything now is one cycle late. It will take 8 cycles (cycle 1
through 8) rather than 7 to completely execute the four instructions shown in
colors.

***** See also[edit] *****
    * Wait_state
    * Classic_RISC_pipeline
***** Notes[edit] *****
   1. ^ Early pipelined processors without any of these heuristics, such as the
      PA-RISC processor of Hewlett-Packard, dealt with hazards by simply
      warning the programmer; in this case, that one or more instructions
      following the branch would be executed whether or not the branch was
      taken. This could be useful; for instance, after computing a number in a
      register, a conditional branch could be followed by loading into the
      register a value more useful to subsequent computations in both the
      branch and the non-branch case.
***** References[edit] *****
   1. ^Glaskowsky, Peter (Aug 18, 2003). "Xelerated's_Xtraordinary_NPU_â
      World's_First_40Gb/s_Packet_Processor_Has_200_CPUs". Microprocessor
      Report. 18 (8): 12â14. Retrieved 20 March 2017.
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
   3. ^John Paul Shen, Mikko H. Lipasti (2004). Modern_Processor_Design.
      McGraw-Hill_Professional.
   4. ^Sunggu Lee (2000). Design_of_Computers_and_Other_Complex_Digital
      Devices. Prentice_Hall.
   5. ^Raul Rojas (1997). "Konrad Zuse's Legacy: The Architecture of the Z1 and
      Z3". IEEE Annals of the History of Computing. 19 (2).
   6. ^"CMSC_411_Lecture_19,_Pipelining_Data_Forwarding". Csee.umbc.edu.
      Retrieved 2014-02-08.
   7. ^"High_performance_computing,_Notes_of_class_11". hpc.serc.iisc.ernet.in.
      September 2000. Archived from the_original on 2013-12-27. Retrieved 2014-
      02-08.
***** External links[edit] *****
 Wikimedia Commons has media related to Pipeline_(computer_hardware).
 Wikibooks has a book on the topic of: Microprocessor_Design/Pipelined
 Processors
    * Branch_Prediction_in_the_Pentium_Family (Archive.org_copy)
    * ArsTechnica_article_on_pipelining
    * Counterflow_Pipeline_Processor_Architecture
    * v
    * t
    * e
Processor_technologies
                    * Turing_machine
                          o Universal
                          o PostâTuring
                          o Quantum
                    * Belt_machine
                    * Stack_machine
                    * Finite-state_machine
Models                    o with_datapath
                          o Hierarchical
                          o Queue_automaton
                    * Register_machines
                          o Counter
                          o Pointer
                          o Random-access
                          o Random-access_stored_program
                    * Von_Neumann
                    * Harvard
                          o modified
                    * Dataflow
                    * Transport-triggered
                    * Cellular
                    * Endianness
                    * Memory_access
                          o NUMA
                          o HUMA
Architecture              o Load/store
                          o Register/memory
                    * Cache_hierarchy
                    * Memory_hierarchy
                          o Virtual_memory
                          o Secondary_storage
                    * Heterogeneous
                    * Fabric
                    * Multiprocessing
                    * Cognitive
                    * Neuromorphic
                          * CISC
                          * RISC
                          * Application-specific
                          * EDGE
                                o TRIPS
                          * VLIW
                Types           o EPIC
                          * MISC
                          * OISC
                          * NISC
Instruction_set           * ZISC
architectures             * comparison
                                o addressing_modes
                    * x86
                    * ARM
                    * MIPS
                    * Power_ISA
                    * SPARC
                    * Itanium
                    * Unicore
                    * MicroBlaze
                    * RISC-V
                    * others
                                       Pipeline_stall
                Instruction pipelining Operand_forwarding
                                       Classic_RISC_pipeline
                                           * Data_dependency
                Hazards                    * Structural
                                           * Control
Execution                                  * False_sharing
                                           * Tomasulo_algorithm
                Out-of-order                     o Reservation_station
                                                 o Re-order_buffer
                                           * Register_renaming
                Speculative                * Branch_prediction
                                           * Memory_dependence_prediction
                                     * Bit
                                           o Bit-serial
                                           o Word
                                     * Instruction
                                     * Pipelining
                                           o Scalar
                Level                      o Superscalar
                                     * Task
                                           o Thread
                                           o Process
                                     * Data
                                           o Vector
                                     * Memory
Parallelism                          * Distributed
                                     * Temporal
                                     * Simultaneous
                Multithreading             o Hyperthreading
                                     * Speculative
                                     * Preemptive
                                     * Cooperative
                                     * SISD
                                     * SIMD
                                           o SWAR
                Flynn's_taxonomy     * SIMT
                                     * MISD
                                     * MIMD
                                           o SPMD
                    * Transistor_count
                    * Instructions_per_cycle (IPC)
                          o Cycles_per_instruction (CPI)
                    * Instructions_per_second (IPS)
Processor           * Floating-point_operations_per_second (FLOPS)
performance         * Transactions_per_second (TPS)
                    * Synaptic_updates_per_second (SUPS)
                    * Performance_per_watt (PPW)
                    * Cache_performance_metrics
                    * Computer_performance_by_orders_of_magnitude
                    * Central_processing_unit (CPU)
                    * Graphics_processing_unit (GPU)
                          o GPGPU
                    * Vector
                    * Barrel
                    * Stream
                    * Coprocessor
                    * ASIC
                    * FPGA
                    * CPLD
                    * Multi-chip_module (MCM)
                    * System_in_package (SiP)
                                   * Microprocessor
                                   * Microcontroller
Types           By application     * Mobile
                                   * Notebook
                                   * Ultra-low-voltage
                                   * ASIP
                                   * System_on_a_chip (SoC)
                Systems            * Multiprocessor (MPSoC)
                on chip            * Programmable (PSoC)
                                   * Network_on_a_chip (NoC)
                                   * AI_accelerator
                                   * Vision_processing_unit (VPU)
                                   * Physics_processing_unit (PPU)
                Hardware           * Digital_signal_processor (DSP)
                accelerators       * Tensor_processing_unit (TPU)
                                   * Secure_cryptoprocessor
                                   * Network_processor
                                   * Baseband_processor
                    * 1-bit
                    * 2-bit
                    * 4-bit
                    * 8-bit
                    * 16-bit
                    * 32-bit
Word_size           * 48-bit
                    * 64-bit
                    * 128-bit
                    * 256-bit
                    * 512-bit
                    * others
                          o variable
                    * Single-core
Core count          * Multi-core
                    * Manycore
                    * Heterogeneous_architecture
                    * Core
                    * Cache
                          o CPU_cache
                          o replacement_policies
                          o coherence
                    * Bus
                    * Clock_rate
                    * Clock_signal
                    * FIFO
                                     * Arithmetic_logic_unit (ALU)
                                     * Address_generation_unit (AGU)
                                     * Floating-point_unit (FPU)
                Functional_units     * Memory_management_unit (MMU)
                                           o Loadâstore_unit
                                           o Translation_lookaside_buffer (TLB)
                                     * Integrated_memory_controller (IMC)
                                     * Combinational
                                     * Sequential
                Logic                * Glue
                                     * Logic_gate
                                           o Quantum
                                           o Array
                                     * Processor_register
                                     * Status_register
                Registers            * Stack_register
Components                           * Register_file
                                     * Memory_buffer
                                     * Program_counter
                                     * Instruction_unit
                                     * Data_buffer
                Control unit         * Write_buffer
                                     * Microcode ROM
                                     * Counter
                                     * Multiplexer
                                     * Demultiplexer
                                     * Adder
                                     * Multiplier
                Datapath                   o CPU
                                     * Binary_decoder
                                           o Address_decoder
                                           o Sum_addressed_decoder
                                     * Barrel_shifter
                                     * Integrated_circuit
                                           o 3D
                                           o Mixed-signal
                                           o Power_management
                Circuitry            * Boolean
                                     * Digital
                                     * Analog
                                     * Quantum
                                     * Switch
                    * PMU
                    * APM
Power               * ACPI
management          * Dynamic_frequency_scaling
                    * Dynamic_voltage_scaling
                    * Clock_gating
                    * Performance_per_watt (PPW)
                    * History_of_general-purpose_CPUs
                    * Microprocessor_chronology
Related             * Processor_design
                    * Digital_electronics
                    * Hardware_security_module
                    * Semiconductor_device_fabrication

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Instruction_pipelining&oldid=902552671"
Categories:
    * Superscalar_microprocessors
    * Instruction_processing
Hidden categories:
    * Articles_with_short_description
    * Use_American_English_from_March_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_to_be_merged_from_January_2019
    * All_articles_to_be_merged
    * Articles_needing_additional_references_from_May_2016
    * All_articles_needing_additional_references
    * Articles_needing_additional_references_from_March_2019
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_March_2019
    * Wikipedia_articles_needing_clarification_from_January_2018
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
    * ÄeÅ¡tina
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Hrvatski
    * Italiano
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 19 June 2019, at 16:18 (UTC).
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
