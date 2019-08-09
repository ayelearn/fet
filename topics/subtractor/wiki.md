The following text has been accessed from https://en.wikipedia.org/wiki/Subtractor at Fri Aug 9 01:27:12 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Subtractor ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article needs additional citations for verification. Please help improve_this_article by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and removed.
 Find sources: "Subtractor" â news Â· newspapers Â· books Â· scholar Â· JSTOR (December 2009)
 (Learn_how_and_when_to_remove_this_template_message)
Part of a series on the
ALU
[ALU_block]
Quick navigation
Theory
    * Binary_number
    * Boolean_algebra
    * Logic_gate
    * Ones'_complement
    * Two's_complement
    * Signed_number_representations
Components
    * Adder (+)
          o Adder
          o Half_adder
          o Full_adder
          o Ripple-carry_adder
          o Carry-lookahead_adder
          o BrentâKung_adder
          o KoggeâStone_adder
          o Carry-save_adder
          o Carry-select_adder
          o Carry-skip_adder
      Adderâsubtractor (Â±)
          o Adderâsubtractor
      Subtractor (â)
          o Subtractor
          o Full_subtractor
          o Half_subtractor
      Multiplier (Ã)
          o Binary_multiplier
          o Multiplication_algorithm
          o Booth's_multiplication_algorithm
          o Wallace_tree
          o Dadda_multiplier
      Divider (Ã·)
          o Binary_Divider
          o Division_algorithm
      Bitwise ops (0b00)
          o Bitwise_operation
          o NOT
          o AND
          o OR
          o Bit_shifts
          o Bit_manipulation
      See also
          o Kochanski_multiplication (exponentiation)
Categories
    * Category:Binary_arithmetic
    * Category:Computer_arithmetic
See also
    * FPU
    * GPU
    * AGU
    * Mechanical_calculator
    * v
    * t
    * e
In electronics, a subtractor can be designed using the same approach as that of
an adder. The binary subtraction process is summarized below. As with an adder,
in the general case of calculations on multi-bit numbers, three bits are
involved in performing the subtraction for each bit of the difference: the
minuend (     X  i     {\displaystyle X_{i}}  [X_{i}]), subtrahend (     Y  i
{\displaystyle Y_{i}}  [Y_{i}]), and a borrow in from the previous (less
significant) bit order position (     B  i     {\displaystyle B_{i}}  [B_{
{i}}]). The outputs are the difference bit (     D  i     {\displaystyle D_{i}}
[D_{{i}}]) and borrow bit      B  i + 1     {\displaystyle B_{i+1}}  [B_{
{i+1}}]. The subtractor is best understood by considering that the subtrahend
and both borrow bits have negative weights, whereas the X and D bits are
positive. The operation performed by the subtractor is to rewrite      X  i
&#x2212;  Y  i   &#x2212;  B  i     {\displaystyle X_{i}-Y_{i}-B_{i}}  [X_{
{i}}-Y_{{i}}-B_{{i}}] (which can take the values -2, -1, 0, or 1) as the sum
&#x2212; 2  B  i + 1   +  D  i     {\displaystyle -2B_{i+1}+D_{i}}  [-2B_{
{i+1}}+D_{{i}}].
          D  i   =  X    &#x2295;  Y  i   &#x2295;  B  i     {\displaystyle D_
      {i}=X_{}\oplus Y_{i}\oplus B_{i}}  [{\displaystyle D_{i}=X_{}\oplus Y_
      {i}\oplus B_{i}}]
          B  i + 1   =  X  i   < (  Y  i   +  B  i   )   {\displaystyle B_
      {i+1}=X_{i}<(Y_{i}+B_{i})}  [B_{i+1}=X_{i}<(Y_{i}+B_{i})]
Subtractors are usually implemented within a binary adder for only a small cost
when using the standard two's_complement notation, by providing an addition/
subtraction selector to the carry-in and to invert the second operand.
         &#x2212; B =    B &#x00AF;    + 1   {\displaystyle -B={\bar {B}}+1}
      [-B={\bar {B}}+1] (definition of two's complement notation)
             A &#x2212; B    = A + ( &#x2212; B )       = A +    B &#x00AF;
      + 1       {\displaystyle {\begin{alignedat}{2}A-B&=A+(-B)\\&=A+{\bar
      {B}}+1\\\end{alignedat}}}  [{\begin{alignedat}{2}A-B&=A+(-B)\\&=A+{\bar
      {B}}+1\\\end{alignedat}}]
⁰
***** Contents *****
    * 1_Half_subtractor
    * 2_Full_subtractor
    * 3_See_also
    * 4_References
    * 5_External_links
***** Half subtractor[edit] *****
Logic diagram for a half subtractor
The half subtractor is a combinational_circuit which is used to perform
subtraction of two bits. It has two inputs, the minuend     X   {\displaystyle
X}  [X] and subtrahend     Y   {\displaystyle Y}  [Y] and two outputs the
difference     D   {\displaystyle D}  [D] and borrow out      B  out
{\displaystyle B_{\text{out}}}  [B_{\text{out}}]. The borrow out signal is set
when the subtractor needs to borrow from the next digit in a multi-digit
subtraction. That is,      B  out   = 1   {\displaystyle B_{\text{out}}=1}  [B_
{\text{out}}=1] when     X < Y   {\displaystyle X<Y}  [X<Y]. Since     X
{\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y] are bits,      B  out
= 1   {\displaystyle B_{\text{out}}=1}  [B_{\text{out}}=1] if and only if     X
= 0   {\displaystyle X=0}  [X=0] and     Y = 1   {\displaystyle Y=1}  [Y=1]. An
important point worth mentioning is that the half subtractor diagram aside
implements     X &#x2212; Y   {\displaystyle X-Y}  [X-Y] and not     Y &#x2212;
X   {\displaystyle Y-X}  [Y-X] since      B  out     {\displaystyle B_{\text
{out}}}  [B_{\text{out}}] on the diagram is given by
          B  out   =   X &#x00AF;   &#x22C5; Y   {\displaystyle B_{\text{out}}=
      {\overline {X}}\cdot Y}  [{\displaystyle B_{\text{out}}={\overline
      {X}}\cdot Y}].
This is an important distinction to make since subtraction itself is not
commutative, but the difference bit     D   {\displaystyle D}  [D] is
calculated using an XOR_gate which is commutative.
[Half-subtractor_using_NAND_gate_only.]
Half-subtractor using NAND gate only.
The truth_table for the half subtractor is:
Inputs Outputs
X Y    D Bout
0 0    0 0
0 1    1 1
1 0    1 0
1 1    0 0
Using the table above and a Karnaugh_map, we find the following logic equations
for     D   {\displaystyle D}  [D] and      B  out     {\displaystyle B_{\text
{out}}}  [B_{\text{out}}]:
         D = X &#x2295; Y   {\displaystyle D=X\oplus Y}  [D=X\oplus Y]
          B  out   =   X &#x00AF;   &#x22C5; Y   {\displaystyle B_{\text{out}}=
      {\overline {X}}\cdot Y}  [B_{\text{out}}={\overline {X}}\cdot Y].
Consequently, a simplified half-subtract circuit, advantageously avoiding
crossed traces in particular as well as a negate gate is:
      X ââ XOR ââ¬âââââââ |X-Y|,  is 0 if X equals Y, 1
otherwise
         ââââ   ââââ
      Y ââ´âââââââ AND ââ borrow, is 1 if Y > X, 0
otherwise
where lines to the right are outputs and others (from the top, bottom or left)
are inputs.
***** Full subtractor[edit] *****
The full subtractor is a combinational_circuit which is used to perform
subtraction of three input bits: the minuend     X   {\displaystyle X}  [X],
subtrahend     Y   {\displaystyle Y}  [Y], and borrow in      B  in
{\displaystyle B_{\text{in}}}  [B_{\text{in}}]. The full subtractor generates
two output bits: the difference     D   {\displaystyle D}  [D] and borrow out
B  out     {\displaystyle B_{\text{out}}}  [B_{\text{out}}].      B  in
{\displaystyle B_{\text{in}}}  [B_{\text{in}}] is set when the previous digit
is borrowed from     X   {\displaystyle X}  [X]. Thus,      B  in
{\displaystyle B_{\text{in}}}  [B_{\text{in}}] is also subtracted from     X
{\displaystyle X}  [X] as well as the subtrahend     Y   {\displaystyle Y}
[Y]. Or in symbols:     X &#x2212; Y &#x2212;  B  in     {\displaystyle X-Y-B_
{\text{in}}}  [X-Y-B_{\text{in}}]. Like the half subtractor, the full
subtractor generates a borrow out when it needs to borrow from the next digit.
Since we are subtracting     Y   {\displaystyle Y}  [Y] and      B  in
{\displaystyle B_{\text{in}}}  [B_{\text{in}}] from     X   {\displaystyle X}
[X], a borrow out needs to be generated when     X < Y +  B  in
{\displaystyle X<Y+B_{\text{in}}}  [X<Y+B_{\text{in}}]. When a borrow out is
generated, 2 is added in the current digit. (This is similar to the subtraction
algorithm in decimal. Instead of adding 2, we add 10 when we borrow.)
Therefore,     D = X &#x2212; Y &#x2212;  B  in   + 2  B  out
{\displaystyle D=X-Y-B_{\text{in}}+2B_{\text{out}}}  [D=X-Y-B_{\text{in}}+2B_
{\text{out}}].
[Full_subtractor_circuit]
Full subtractor circuit
The truth table for the full subtractor is:
Inputs  Outputs
X Y Bin D Bout
0 0 0   0 0
0 0 1   1 1
0 1 0   1 1
0 1 1   0 1
1 0 0   1 0
1 0 1   0 0
1 1 0   0 0
1 1 1   1 1
Therefore the equation is D=XâYâBin and Bout=X'Bin+X'Y+YBin
***** See also[edit] *****
    * Adder_(electronics)
    * Carry-lookahead_adder
    * Carry-save_adder
    * Adding_machine
    * Adder-subtractor
***** References[edit] *****
    * Foundations Of Digital Electronics by Elijah Mwangi
***** External links[edit] *****
    * N_bit_Binary_addition_or_subtraction_using_single_circuit.
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
                Instruction_pipelining Operand_forwarding
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
index.php?title=Subtractor&oldid=900084679"
Categories:
    * Computer_arithmetic
    * Binary_logic
    * Adders_(electronics)
    * Subtraction
Hidden categories:
    * Articles_needing_additional_references_from_December_2009
    * All_articles_needing_additional_references
    * Pages_using_collapsible_list_with_both_background_and_text-align_in
      titlestyle
    * Pages_using_sidebar_with_the_child_parameter
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
    * íêµ­ì´
    * Bahasa_Indonesia
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * à¹à¸à¸¢
Edit_links
    * This page was last edited on 3 June 2019, at 09:50 (UTC).
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
