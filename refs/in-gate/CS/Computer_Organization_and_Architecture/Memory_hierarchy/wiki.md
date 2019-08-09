The following text has been accessed from https://en.wikipedia.org/wiki/Memory_hierarchy at Fri Aug 9 01:11:05 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Memory hierarchy ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Diagram of the computer memory hierarchy
In computer_architecture, the memory hierarchy separates computer_storage into
a hierarchy based on response time. Since response time, complexity, and
capacity are related, the levels may also be distinguished by their performance
and controlling technologies.[1] Memory hierarchy affects performance in
computer architectural design, algorithm predictions, and lower level
programming constructs involving locality_of_reference.
Designing for high performance requires considering the restrictions of the
memory hierarchy, i.e. the size and capabilities of each component. Each of the
various components can be viewed as part of a hierarchy of memories
(m1,m2,...,mn) in which each member mi is typically smaller and faster than the
next highest member mi+1 of the hierarchy. To limit waiting by higher levels, a
lower level will respond by filling a buffer and then signaling for activating
the transfer.
There are four major storage levels.[1]
   1. Internal – Processor_registers and cache.
   2. Main – the system RAM and controller cards.
   3. On-line mass storage – Secondary storage.
   4. Off-line bulk storage – Tertiary and Off-line storage.
This is a general memory hierarchy structuring. Many other structures are
useful. For example, a paging algorithm may be considered as a level for
virtual_memory when designing a computer_architecture, and one can include a
level of nearline_storage between online and offline storage.
⁰
***** Contents *****
    * 1_Properties_of_the_technologies_in_the_memory_hierarchy
    * 2_Examples
    * 3_See_also
    * 4_References
***** Properties of the technologies in the memory hierarchy[edit] *****
    * Adding complexity slows down the memory hierarchy.[2]
    * CMOx memory technology stretches the Flash space in the memory hierarchy
      [3]
    * One of the main ways to increase system performance is minimising how far
      down the memory hierarchy one has to go to manipulate data.[4]
    * Latency and bandwidth are two metrics associated with caches and. Neither
      of them is uniform, but is specific to a particular component of the
      memory hierarchy.[5]
    * Predicting where in the memory hierarchy the data resides is difficult.
      [5]
    * ...the location in the memory hierarchy dictates the time required for
      the prefetch to occur.[5]
***** Examples[edit] *****
Memory hierarchy of an AMD Bulldozer server.
The number of levels in the memory hierarchy and the performance at each level
has increased over time. The type of memory or storage components also change
historically [6]. For example, the memory hierarchy of an Intel Haswell Mobile
[7] processor circa 2013 is:
    * Processor_registers – the fastest possible access (usually 1 CPU cycle).
      A few thousand bytes in size
    * Cache
          o Level 0 (L0) Micro_operations cache – 6 KiB [8] in size
          o Level 1 (L1) Instruction cache – 128 KiB in size
          o Level 1 (L1) Data cache – 128 KiB in size. Best access speed is
            around 700 GiB/second[9]
          o Level 2 (L2) Instruction and data (shared) – 1 MiB in size. Best
            access speed is around 200 GiB/second[9]
          o Level 3 (L3) Shared cache – 6 MiB in size. Best access speed is
            around 100 GB/second[9]
          o Level 4 (L4) Shared cache – 128 MiB in size. Best access speed is
            around 40 GB/second[9]
    * Main_memory (Primary_storage) – Gigabytes in size. Best access speed is
      around 10 GB/second.[9] In the case of a NUMA machine, access times may
      not be uniform
    * Disk_storage (Secondary_storage) – Terabytes in size. As of 2017, best
      access speed is from a consumer solid_state_drive is about 2000 MB/second
      [10]
    * Nearline_storage (Tertiary_storage) – Up to exabytes in size. As of 2013,
      best access speed is about 160 MB/second[11]
    * Offline_storage
The lower levels of the hierarchy â from disks downwards â are also known
as tiered_storage. The formal distinction between online, nearline, and offline
storage is:[12]
    * Online storage is immediately available for I/O.
    * Nearline storage is not immediately available, but can be made online
      quickly without human intervention.
    * Offline storage is not immediately available, and requires some human
      intervention to bring online.
For example, always-on spinning disks are online, while spinning disks that
spin-down, such as massive array of idle disk (MAID), are nearline. Removable
media such as tape cartridges that can be automatically loaded, as in a tape
library, are nearline, while cartridges that must be manually loaded are
offline.
Most modern CPUs are so fast that for most program workloads, the bottleneck is
the locality_of_reference of memory accesses and the efficiency of the caching
and memory transfer between different levels of the hierarchy[citation_needed].
As a result, the CPU spends much of its time idling, waiting for memory I/O to
complete. This is sometimes called the space cost, as a larger memory object is
more likely to overflow a small/fast level and require use of a larger/slower
level. The resulting load on memory use is known as pressure (respectively
register pressure, cache pressure, and (main) memory pressure). Terms for data
being missing from a higher level and needing to be fetched from a lower level
are, respectively: register_spilling (due to register_pressure: register to
cache), cache_miss (cache to main memory), and (hard) page_fault (main memory
to disk).
Modern programming_languages mainly assume two levels of memory, main memory
and disk storage, though in assembly_language and inline_assemblers in
languages such as C, registers can be directly accessed. Taking optimal
advantage of the memory hierarchy requires the cooperation of programmers,
hardware, and compilers (as well as underlying support from the operating
system):
    * Programmers are responsible for moving data between disk and memory
      through file I/O.
    * Hardware is responsible for moving data between memory and caches.
    * Optimizing_compilers are responsible for generating code that, when
      executed, will cause the hardware to use caches and registers
      efficiently.
Many programmers assume one level of memory. This works fine until the
application hits a performance wall. Then the memory hierarchy will be assessed
during code_refactoring.
***** See also[edit] *****
    * Memory_characteristics
    * Cache_Hierarchy
    * Use_of_spatial_and_temporal_locality:_hierarchical_memory
    * Buffer_vs._cache
    * Cache_hierarchy_in_a_modern_processor
    * Memory_wall
    * Computer_memory
    * Hierarchical_storage_management
    * Cloud_storage
    * Memory_access_pattern
***** References[edit] *****
   1. ^ a bToy, Wing; Zee, Benjamin (1986). Computer Hardware/Software
      Architecture. Prentice Hall. p. 30. ISBN 0-13-163502-6.
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
   3. ^ Write-combining
   4. ^"Memory_Hierarchy". Unitity Semiconductor Corporation. Archived from the
      original on 5 August 2009. Retrieved 16 September 2009.
   5. ^PÃ¡draig Brady. "Multi-Core". Retrieved 16 September 2009.
   6. ^ a b cvan der Pas, Ruud (2002). Santa Clara, California: Sun
      Microsystems: 26. 817-0742-10 http://www.sun.com/.Missing or empty
      |title= (help); |contribution= ignored (help)
   7. ^"Memory_&_Storage_-_Timeline_of_Computer_History_-_Computer_History
      Museum". www.computerhistory.org.
   8. ^Crothers, Brooke. "Dissecting_Intel's_top_graphics_in_Apple's_15-inch
      MacBook_Pro_-_CNET". News.cnet.com. Retrieved 2014-07-31.
   9. ^"Intel's_Haswell_Architecture_Analyzed:_Building_a_New_PC_and_a_New
      Intel". AnandTech. Retrieved 2014-07-31.
  10. ^ a b c d e"SiSoftware_Zone". Sisoftware.co.uk. Retrieved 2014-07-31.
  11. ^"Samsung_960_Pro_M.2_NVMe_SSD_Review". storagereview.com. Retrieved
      2017-04-13.
  12. ^"Ultrium_-_LTO_Technology_-_Ultrium_GenerationsLTO". Lto.org. Archived
      from the_original on 2011-07-27. Retrieved 2014-07-31.
  13. ^Pearson, Tony (2010). "Correct_use_of_the_term_Nearline". IBM
      Developerworks, Inside System Storage. Retrieved 2015-08-16.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Memory_hierarchy&oldid=872104906"
Categories:
    * Computer_architecture
    * Computer_data_storage
    * Hierarchy
Hidden categories:
    * Pages_with_citations_lacking_titles
    * CS1_errors:_chapter_ignored
    * Pages_with_citations_having_bare_URLs
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2009
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
    * CatalÃ 
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Bahasa_Indonesia
    * ×¢××¨××ª
    * Nederlands
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 5 December 2018, at 05:05 (UTC).
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
