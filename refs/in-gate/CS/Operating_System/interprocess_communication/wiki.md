The following text has been accessed from https://en.wikipedia.org/wiki/Inter-process_communication at Fri Aug 9 01:12:04 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Inter-process communication ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other uses, see IPC.
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (August 2015)(Learn_how_and
 when_to_remove_this_template_message)
An example showing a grid_computing system connecting many personal computers
over the Internet using inter-process network communication
In computer_science, inter-process communication or interprocess communication
(IPC) refers specifically to the mechanisms an operating_system provides to
allow the processes to manage shared data. Typically, applications can use IPC,
categorized as clients_and_servers, where the client requests data and the
server responds to client requests.[1] Many applications are both clients and
servers, as commonly seen in distributed_computing. Methods for doing IPC are
divided into categories which vary based on software_requirements, such as
performance and modularity requirements, and system circumstances, such as
network_bandwidth and latency.[1]
IPC is very important to the design process for microkernels and nanokernels.
Microkernels reduce the number of functionalities provided by the kernel. Those
functionalities are then obtained by communicating with servers via IPC,
increasing drastically the number of IPC compared to a regular monolithic
kernel.
⁰
***** Contents *****
    * 1_Approaches
    * 2_Synchronization
    * 3_Applications
          o 3.1_Remote_procedure_call_interfaces
          o 3.2_Platform_communication_stack
          o 3.3_Operating_system_communication_stack
          o 3.4_Distributed_object_models
    * 4_See_also
    * 5_References
    * 6_External_links
***** Approaches[edit] *****
                                                     Provided by (operating
Method                    Short Description          systems or other
                                                     environments)
                          A record stored on disk,
                          or a record synthesized on
File                      demand by a file server,   Most operating systems
                          which can be accessed by
                          multiple processes.
                          A unique, late-1960's form
                          of inter-process           Dartmouth_Time-Sharing
Communications file       communication, most        System
                          closely resembling Plan
                          9's 9P_protocol
                          A system message sent from
                          one process to another,
Signal; also Asynchronous not usually used to        Most operating systems
System_Trap               transfer data but instead
                          used to remotely command
                          the partnered process.
                          Data sent over a network
                          interface, either to a
                          different process on the
                          same computer or to
                          another computer on the
Socket                    network. Stream-oriented   Most operating systems
                          (TCP; data written through
                          a socket requires
                          formatting to preserve
                          message boundaries) or
                          more rarely message-
                          oriented (UDP, SCTP).
                          Similar to an internet
                          socket but all
                          communication occurs
                          within the kernel. Domain
                          sockets use the file       All POSIX operating
Unix_domain_socket        system as their address    systems and Windows 10[2]
                          space. Processes reference
                          a domain socket as an
                          inode, and multiple
                          processes can communicate
                          with one socket
                          A data stream similar to a
                          socket, but which usually
                          preserves message
                          boundaries. Typically
                          implemented by the
Message_queue             operating system, they     Most operating systems
                          allow multiple processes
                          to read and write to the
                          message queue without
                          being directly connected
                          to each other.
                          A unidirectional data
                          channel. Data written to
                          the write end of the pipe
                          is buffered by the
                          operating system until it
Pipe                      is read from the read end  All POSIX systems, Windows
                          of the pipe. Two-way data
                          streams between processes
                          can be achieved by
                          creating two pipes
                          utilizing standard_input
                          and_output.
                          A pipe implemented through
                          a file on the file system
                          instead of standard_input  All POSIX systems,
Named_pipe                and_output. Multiple       Windows, AmigaOS 2.0+
                          processes can read and
                          write to the file as a
                          buffer for IPC data.
                          Multiple processes are
                          given access to the same
                          block of memory which
Shared_memory             creates a shared buffer    All POSIX systems, Windows
                          for the processes to
                          communicate with each
                          other.
                          Allows multiple programs
                          to communicate using       Used in RPC, RMI, and MPI
Message_passing           message queues and/or non- paradigms, Java_RMI,
                          OS managed channels,       CORBA, DDS, MSMQ,
                          commonly used in           MailSlots, QNX, others
                          concurrency models.
                          A file mapped to RAM and
                          can be modified by
                          changing memory addresses
Memory-mapped_file        directly instead of        All POSIX systems, Windows
                          outputting to a stream.
                          This shares the same
                          benefits as a standard
                          file.
***** Synchronization[edit] *****
Main article: Synchronization_(computer_science)
Depending on the solution, an IPC mechanism may provide synchronization or
leave it up to processes and threads to communicate amongst themselves (e.g.
via shared memory).
While synchronization will include some information (e.g. whether or not the
lock is enabled, a count of processes waiting, etc.) it is not primarily an
information-passing communication mechanism per se.
Examples of synchronization primitives are:
    * Semaphore
    * Spinlock
    * Barrier
    * Mutual_exclusion
***** Applications[edit] *****
 This article is in list format, but may read better as prose. You can help by
 converting_this_article, if appropriate. Editing_help is available. (November
 2016)
**** Remote procedure call interfaces[edit] ****
Main article: remote_procedure_call
    * Java's Remote_Method_Invocation (RMI)
    * ONC_RPC
    * XML-RPC or SOAP
    * JSON-RPC
    * Message Bus (Mbus) (specified in RFC_3259)
    * .NET_Remoting
**** Platform communication stack[edit] ****
The following are messaging and information systems that utilize IPC
mechanisms, but don't implement IPC themselves:
    * KDE's Desktop_Communications_Protocol (DCOP) – deprecated by D-Bus
    * D-Bus
    * OpenWrt uses ubus micro bus architecture
    * MCAPI Multicore Communications API
    * SIMPL The Synchronous Interprocess Messaging Project for Linux (SIMPL)
    * 9P (Plan 9 Filesystem Protocol)
    * Distributed_Computing_Environment (DCE)
    * Thrift
    * TIPC
    * ZeroC's Internet_Communications_Engine (ICE)
    * ÃMQ
    * Enduro/X Middleware
    * YAMI4
**** Operating system communication stack[edit] ****
The following are platform or programming language-specific APIs:
    * Apple_Computer's Apple_events (previously known as Interapplication
      Communications (IAC)).
    * Enea's LINX for Linux (open source) and various DSP and general purpose
      processors under OSE
    * The Mach_kernel's Mach Ports
    * Microsoft's ActiveX, Component_Object_Model (COM), Microsoft_Transaction
      Server (COM+), Distributed_Component_Object_Model (DCOM), Dynamic_Data
      Exchange (DDE), Object_Linking_and_Embedding (OLE), anonymous_pipes,
      named_pipes, Local_Procedure_Call, MailSlots, Message_loop, MSRPC, .NET
      Remoting, and Windows_Communication_Foundation (WCF)
    * Novell's SPX
    * POSIX mmap, message_queues, semaphores,[3] and shared_memory
    * RISC_OS's messages
    * Solaris Doors
    * System_V's message queues, semaphores, and shared memory
    * OpenBinder Open binder
    * QNX's PPS (Persistent Publish/Subscribe) service
**** Distributed object models[edit] ****
The following are platform or programming language specific-APIs that use IPC,
but do not themselves implement it:
    * Libt2n for C++ under Linux only, handles complex objects and exceptions
    * PHP's sessions
    * Distributed_Ruby
    * Common_Object_Request_Broker_Architecture (CORBA)
***** See also[edit] *****
    * [icon]Computer_programming_portal
    * Computer_network_programming
    * Communicating_Sequential_Processes (CSP paradigm)
    * Data_Distribution_Service
    * Protected_procedure_call
***** References[edit] *****
   1. ^ a b"Interprocess_Communications". Microsoft.
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
   3. ^"Windows/WSL_Interop_with_AF_UNIX". Microsoft Corporation. Retrieved 25
      May 2018.
   4. ^ Concurrent programming - communication between processes http://
      www.tldp.org/pub/Linux/docs/ldp-archived/linuxfocus/English/Archives/lf-
      2003_01-0281.pdf
    * Stevens,_Richard. UNIX Network Programming, Volume 2, Second Edition:
      Interprocess Communications. Prentice Hall, 1999.
ISBN 0-13-081081-9
U. Ramachandran, M. Solomon, M. Vernon Hardware_support_for_interprocess
communication Proceedings of the 14th annual international symposium on
Computer architecture. Pittsburgh, Pennsylvania, United States. Pages: 178 -
188. Year of Publication: 1987
ISBN 0-8186-0776-9
Crovella, M. Bianchini, R. LeBlanc, T. Markatos, E. Wisniewski, R. Using
communication-to-computation_ratio_in_parallel_program_designand_performance
prediction 1â4 December 1992. pp. 238â245
ISBN 0-8186-3200-3
***** External links[edit] *****
    * Linux_IPC_with_sub-microsecond_latencies
    * Linux_ipc(5)_man_page describing System V IPC
    * Windows_IPC
    * Unix_Network_Programming_(Vol_2:_Interprocess_Communications) by W.
      Richard Stevens
    * Interprocess_Communication_and_Pipes_in_C
    * DIPC,_Distributed_System_V_IPC
    * v
    * t
    * e
Inter-process communication
Data exchange among threads in computer_programs
                       * File
                       * Memory-mapped_file
                       * Message_passing
                       * Message_queue_and_mailbox
                       * Named_pipe
                       * Anonymous_pipe
Methods                * Pipe
                       * Semaphore
                       * Shared_memory
                       * Signal
                       * Sockets
                             o Network
                             o Unix
                       * Apple_events
                       * COM+
                       * CORBA
                       * D-Bus
                       * DDS
                       * DCE
Protocols              * ICE
and standards          * OpenBinder
                       * ONC_RPC
                       * POSIX (various methods)
                       * SOAP
                       * REST
                       * Thrift
                       * TIPC
                       * XML-RPC
                       * D-Bus
Software_libraries     * libevent
and frameworks         * SIMPL
                       * LINX
    * v
    * t
    * e
Web_syndication
  History
      Blogging
      Podcasting
      Vlog|Video_blogging
      Web_syndication_technology
               * Art
               * Bloggernacle
               * Classical_music
               * Corporate
               * Dream_diary
               * Edublog
               * Electronic_journal
               * Fake
               * Family
               * Fashion
               * Food
               * Health
Types          * Law
               * Lifelog
               * Litblog
               * MP3
               * News
               * Photoblog
               * Police
               * Political
               * Prayer
               * Project
               * Reverse
               * Travel
               * Warblog
           General       * BitTorrent
                         * Feed_URI_scheme
                         * Linkback
                         * Permalink
                         * Ping
           Features      * Pingback
                         * Reblogging
                         * Refback
                         * Rollback
                         * Trackback
                         * Conversation_threading
           Mechanism     * Geotagging
                         * RSS_enclosure
                         * Synchronization
                         * Atom_feed
                         * Data_feed
           Memetics      * Photofeed
                         * Product_feed
Technology               * RDF_feed
                         * Web_feed
                         * GeoRSS
           RSS           * MRSS
                         * RSS_TV
                         * Inter-process communication
                         * Livemark
                         * Mashup
           Social        * Referencing
                         * RSS_editor
                         * RSS_tracking
                         * Streaming_media
                         * OML
                         * OPML
                         * RSS_Advisory_Board
           Standard      * Usenet
                         * World_Wide_Web
                         * XBEL
                         * XOXO
               * Audio_podcast
               * Enhanced_podcast
               * Mobilecast
               * Narrowcasting
               * Peercasting
               * Screencast
               * Slidecasting
               * Videocast
               * Webcomic
               * Webtoon
Form           * Web_series
               * Anonymous_blogging
               * Collaborative_blog
               * Columnist
               * Instant_messaging
               * Liveblogging
               * Microblog
               * Mobile_blogging
               * Roblog
               * Spam_blog
               * Video_blogging
               * Motovlogging
                                 * Carnivals
                                 * Fiction
                                 * Journalism
                                       o Citizen
           Alternative_media           o Database
                                 * Online_diary
                                 * Search_engines
                                 * Sideblog
                                 * Software
                                 * Web_directory
                                 * Aggregation
                                       o News
                                       o Poll
                                       o Review
                                       o Search
                                       o Video
Media                            * Atom
           Micromedia            * AtomPub
                                 * Broadcatching
                                 * Hashtag
                                 * NewsML
                                       o 1
                                       o G2
                                 * Social_communication
                                 * Social_software
                                 * Web_Slice
                                 * Blogosphere
                                 * Escribitionist
                                 * Glossary_of_blogging
           Related               * Pay_per_click
                                 * Posting_style
                                 * Slashdot_effect
                                 * Spam_in_blogs
                                 * Uses_of_podcasting

Retrieved from "https://en.wikipedia.org/w/index.php?title=Inter-
process_communication&oldid=909076794"
Categories:
    * Inter-process_communication
Hidden categories:
    * Articles_lacking_in-text_citations_from_August_2015
    * All_articles_lacking_in-text_citations
    * Articles_needing_cleanup_from_November_2016
    * All_pages_needing_cleanup
    * Articles_with_sections_that_need_to_be_turned_into_prose_from_November
      2016
    * Pages_using_RFC_magic_links
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
    * AzÉrbaycanca
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 2 August 2019, at 22:34 (UTC).
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
