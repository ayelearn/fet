The following text has been accessed from https://en.wikipedia.org/wiki/Deadlock at Fri Aug 9 01:12:17 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Deadlock ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with Deathlok.
This article is about the computer science concept. For other uses, see
Deadlock_(disambiguation).
"Livelock" redirects here. For the video game, see Livelock_(video_game).
Both processes need resources to continue execution. P1 requires additional
resource R1 and is in possession of resource R2, P2 requires additional
resource R2 and is in possession of R1; neither process can continue.
Four processes (blue lines) compete for one resource (grey circle), following a
right-before-left policy. A deadlock occurs when all processes lock the
resource simultaneously (black lines). The deadlock can be resolved by breaking
the symmetry.
In concurrent_computing, a deadlock is a state in which each member of a group
is waiting for another member, including itself, to take action, such as
sending a message or more commonly releasing a lock.[1] Deadlock is a common
problem in multiprocessing systems, parallel_computing, and distributed
systems, where software and hardware locks are used to arbitrate shared
resources and implement process_synchronization.[2]
In an operating_system, a deadlock occurs when a process or thread enters a
waiting state because a requested system_resource is held by another waiting
process, which in turn is waiting for another resource held by another waiting
process. If a process is unable to change its state indefinitely because the
resources requested by it are being used by another waiting process, then the
system is said to be in a deadlock.[3]
In a communications_system, deadlocks occur mainly due to lost or corrupt
signals rather than resource contention.[4]
Two processes competing for two resources in opposite order.
   1. A single process goes through.
   2. The later process has to wait.
   3. A deadlock occurs when the first process locks the first resource at the
      same time as the second process locks the second resource.
   4. The deadlock can be resolved by cancelling and restarting the first
      process.
⁰
***** Contents *****
    * 1_Necessary_conditions
    * 2_Deadlock_handling
          o 2.1_Ignoring_deadlock
          o 2.2_Detection
          o 2.3_Prevention
    * 3_Livelock
    * 4_Distributed_deadlock
    * 5_See_also
    * 6_References
    * 7_Further_reading
    * 8_External_links
***** Necessary conditions[edit] *****
A deadlock situation on a resource can arise if and only if all of the
following conditions hold simultaneously in a system:[5]
   1. Mutual_exclusion: At least one resource must be held in a non-shareable
      mode. Otherwise, the processes would not be prevented from using the
      resource when necessary. Only one process can use the resource at any
      given instant of time.[6]
   2. Hold and wait or resource holding: a process is currently holding at
      least one resource and requesting additional resources which are being
      held by other processes.
   3. No preemption: a resource can be released only voluntarily by the process
      holding it.
   4. Circular wait: each process must be waiting for a resource which is being
      held by another process, which in turn is waiting for the first process
      to release the resource. In general, there is a set of waiting processes,
      P = {P1, P2, â¦, PN}, such that P1 is waiting for a resource held by P2,
      P2 is waiting for a resource held by P3 and so on until PN is waiting for
      a resource held by P1.[3][7]
These four conditions are known as the Coffman conditions from their first
description in a 1971 article by Edward_G._Coffman,_Jr.[7]
***** Deadlock handling[edit] *****
Most current operating systems cannot prevent deadlocks.[8] When a deadlock
occurs, different operating systems respond to them in different non-standard
manners. Most approaches work by preventing one of the four Coffman conditions
from occurring, especially the fourth one.[9] Major approaches are as follows.
**** Ignoring deadlock[edit] ****
In this approach, it is assumed that a deadlock will never occur. This is also
an application of the Ostrich_algorithm.[9][10] This approach was initially
used by MINIX and UNIX.[7] This is used when the time intervals between
occurrences of deadlocks are large and the data loss incurred each time is
tolerable.
**** Detection[edit] ****
Under the deadlock detection, deadlocks are allowed to occur. Then the state of
the system is examined to detect that a deadlock has occurred and subsequently
it is corrected. An algorithm is employed that tracks resource allocation and
process states, it rolls back and restarts one or more of the processes in
order to remove the detected deadlock. Detecting a deadlock that has already
occurred is easily possible since the resources that each process has locked
and/or currently requested are known to the resource scheduler of the operating
system.[10]
After a deadlock is detected, it can be corrected by using one of the following
methods:[citation_needed]
   1. Process termination: one or more processes involved in the deadlock may
      be aborted. One could choose to abort all competing processes involved in
      the deadlock. This ensures that deadlock is resolved with certainty and
      speed.[citation_needed] But the expense is high as partial computations
      will be lost. Or, one could choose to abort one process at a time until
      the deadlock is resolved. This approach has high overhead because after
      each abort an algorithm must determine whether the system is still in
      deadlock.[citation_needed] Several factors must be considered while
      choosing a candidate for termination, such as priority and age of the
      process.[citation_needed]
   2. Resource preemption: resources allocated to various processes may be
      successively preempted and allocated to other processes until the
      deadlock is broken.[11]
**** Prevention[edit] ****
Main article: Deadlock_prevention_algorithms
(A) Two processes competing for one resource, following a first-come, first-
served policy. (B) Deadlock occurs when both processes lock the resource
simultaneously. (C) The deadlock can be resolved by breaking the symmetry of
the locks. (D) The deadlock can be prevented by breaking the symmetry of the
locking mechanism.
Deadlock prevention works by preventing one of the four Coffman conditions from
occurring.
    * Removing the mutual exclusion condition means that no process will have
      exclusive access to a resource. This proves impossible for resources that
      cannot be spooled. But even with spooled resources, deadlock could still
      occur. Algorithms that avoid mutual exclusion are called non-blocking
      synchronization algorithms.
    * The hold and wait or resource holding conditions may be removed by
      requiring processes to request all the resources they will need before
      starting up (or before embarking upon a particular set of operations).
      This advance knowledge is frequently difficult to satisfy and, in any
      case, is an inefficient use of resources. Another way is to require
      processes to request resources only when it has none. Thus, first they
      must release all their currently held resources before requesting all the
      resources they will need from scratch. This too is often impractical. It
      is so because resources may be allocated and remain unused for long
      periods. Also, a process requiring a popular resource may have to wait
      indefinitely, as such a resource may always be allocated to some process,
      resulting in resource_starvation.[12] (These algorithms, such as
      serializing_tokens, are known as the all-or-none algorithms.)
    * The no preemption condition may also be difficult or impossible to avoid
      as a process has to be able to have a resource for a certain amount of
      time, or the processing outcome may be inconsistent or thrashing may
      occur. However, inability to enforce preemption may interfere with a
      priority algorithm. Preemption of a "locked out" resource generally
      implies a rollback, and is to be avoided, since it is very costly in
      overhead. Algorithms that allow preemption include lock-free_and_wait-
      free_algorithms and optimistic_concurrency_control. If a process holding
      some resources and requests for some another resource(s) that cannot be
      immediately allocated to it, the condition may be removed by releasing
      all the currently being held resources of that process.
    * The final condition is the circular wait condition. Approaches that avoid
      circular waits include disabling interrupts during critical sections and
      using a hierarchy to determine a partial_ordering of resources. If no
      obvious hierarchy exists, even the memory address of resources has been
      used to determine ordering and resources are requested in the increasing
      order of the enumeration.[3] Dijkstra's_solution can also be used.
***** Livelock[edit] *****
A livelock is similar to a deadlock, except that the states of the processes
involved in the livelock constantly change with regard to one another, none
progressing.
The term was coined by Edward_A._Ashcroft in a 1975 paper[13] in connection
with an examination of airline booking systems.[14] Livelock is a special case
of resource_starvation; the general definition only states that a specific
process is not progressing.[15]
Livelock is a risk with some algorithms that detect and recover from deadlock.
If more than one process takes action, the deadlock_detection_algorithm can be
repeatedly triggered. This can be avoided by ensuring that only one process
(chosen arbitrarily or by priority) takes action.[16]
***** Distributed deadlock[edit] *****
Distributed deadlocks can occur in distributed_systems when distributed
transactions or concurrency_control is being used.
Distributed deadlocks can be detected either by constructing a global wait-for
graph from local wait-for graphs at a deadlock detector or by a distributed
algorithm like edge_chasing.
Phantom deadlocks are deadlocks that are falsely detected in a distributed
system due to system internal delays but do not actually exist.
For example, if a process releases a resource R1 and issues a request for R2,
and the first message is lost or delayed, a coordinator (detector of deadlocks)
could falsely conclude a deadlock (if the request for R2 while having R1 would
cause a deadlock).
***** See also[edit] *****
    * Aporia
    * Banker's_algorithm
    * Catch-22_(logic)
    * Circular_reference
    * Dining_philosophers_problem
    * File_locking
    * Gridlock (in vehicular traffic)
    * Hang_(computing)
    * Impasse
    * Infinite_loop
    * Linearizability
    * Model_checker can be used to formally verify that a system will never
      enter a deadlock
    * Ostrich_algorithm
    * Priority_inversion
    * Race_condition
    * Readers-writer_lock
    * Sleeping_barber_problem
    * Stalemate
    * Synchronization_(computer_science)
    * Turn_restriction_routing
***** References[edit] *****
   1. ^Coulouris, George (2012). Distributed Systems Concepts and Design.
      Pearson. p. 716. ISBN 978-0-273-76059-7.
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
   3. ^Padua, David (2011). Encyclopedia_of_Parallel_Computing. Springer.
      p. 524. ISBN 9780387097657. Retrieved 28 January 2012.
   4. ^ a b cSilberschatz, Abraham (2006). Operating_System_Principles (7th
      ed.). Wiley-India. p. 237. ISBN 9788126509621. Retrieved 29 January 2012.
   5. ^Schneider, G. Michael (2009). Invitation_to_Computer_Science. Cengage
      Learning. p. 271. ISBN 978-0324788594. Retrieved 28 January 2012.
   6. ^Silberschatz, Abraham (2006). Operating_System_Principles (7 ed.).
      Wiley-India. p. 239. ISBN 9788126509621. Retrieved 29 January 2012.
   7. ^"ECS_150_Spring_1999:_Four_Necessary_and_Sufficient_Conditions_for
      Deadlock". nob.cs.ucdavis.edu. Archived from the original on 29 April
      2018. Retrieved 29 April 2018.
   8. ^ a b cShibu, K. (2009). Intro_To_Embedded_Systems (1st ed.). Tata
      McGraw-Hill Education. p. 446. ISBN 9780070145894. Retrieved 28 January
      2012.
   9. ^Silberschatz, Abraham (2006). Operating_System_Principles (7 ed.).
      Wiley-India. p. 237. ISBN 9788126509621. Retrieved 29 January 2012.
  10. ^ a bStuart, Brian L. (2008). Principles_of_operating_systems (1st ed.).
      Cengage Learning. p. 446. ISBN 9781418837693. Retrieved 28 January 2012.
  11. ^ a bTanenbaum, Andrew S. (1995). Distributed_Operating_Systems (1st
      ed.). Pearson Education. p. 117. ISBN 9788177581799. Retrieved 28 January
      2012.
  12. ^"IBM_Knowledge_Center". www.ibm.com. Archived from the original on 19
      March 2017. Retrieved 29 April 2018.
  13. ^Silberschatz, Abraham (2006). Operating_System_Principles (7 ed.).
      Wiley-India. p. 244. ISBN 9788126509621. Retrieved 29 January 2012.
  14. ^Ashcroft, E.A. (1975). "Proving assertions about parallel programs".
      Journal of Computer and System Sciences. 10: 110â135. doi:10.1016/
      S0022-0000(75)80018-3.
  15. ^Kwong, Y. S. (1979). "On the absence of livelocks in parallel programs".
      Semantics of Concurrent Computation. Lecture Notes in Computer Science.
      70. pp. 172â190. doi:10.1007/BFb0022469. ISBN 3-540-09511-X.
  16. ^Anderson, James H.; Yong-jik Kim (2001). "Shared-memory_mutual
      exclusion:_Major_research_trends_since_1986". Archived from the original
      on 25 May 2006.
  17. ^ZÃ¶bel, Dieter (October 1983). "The Deadlock problem: a classifying
      bibliography". ACM SIGOPS Operating Systems Review. 17 (4): 6â15. doi:
      10.1145/850752.850753. ISSN 0163-5980.
***** Further reading[edit] *****
    * Kaveh, Nima; Emmerich, Wolfgang. "Deadlock_Detection_in_Distributed
      Object_Systems" (PDF). London: University College London.
Bensalem, Saddek; Fernandez, Jean-Claude; Havelund, Klaus; Mounier, Laurent
(2006). Confirmation of deadlock potentials detected by runtime analysis.
Proceedings of the 2006 Workshop on Parallel and Distributed Systems: Testing
and Debugging. ACM. pp. 41â50. CiteSeerX 10.1.1.431.3757. doi:10.1145/
1147403.1147412. ISBN 978-1595934147.
Coffman, Edward G., Jr.; Elphick, Michael J.; Shoshani, Arie (1971). "System
Deadlocks" (PDF). ACM Computing Surveys. 3 (2): 67â78. doi:10.1145/
356586.356588.
Mogul, Jeffrey C.; Ramakrishnan, K. K. (1997). "Eliminating receive livelock in
an interrupt-driven kernel". ACM Transactions on Computer Systems. 15 (3):
217â252. CiteSeerX 10.1.1.156.667. doi:10.1145/263326.263335. ISSN 0734-2071.
Havender, James W. (1968). "Avoiding_deadlock_in_multitasking_systems". IBM
Systems Journal. 7 (2): 74. doi:10.1147/sj.72.0074.
Holliday, JoAnne L.; El Abbadi, Amr. "Distributed_Deadlock_Detection".
Encyclopedia of Distributed Computing. Archived from the_original on 2 November
2015. Retrieved 29 December 2004.
Knapp, Edgar (1987). "Deadlock detection in distributed databases". ACM
Computing Surveys. 19 (4): 303â328. CiteSeerX 10.1.1.137.6874. doi:10.1145/
45075.46163. ISSN 0360-0300.
Ling, Yibei; Chen, Shigang; Chiang, Jason (2006). "On Optimal Deadlock
Detection Scheduling". IEEE Transactions on Computers. 55 (9): 1178â1187.
CiteSeerX 10.1.1.259.4311. doi:10.1109/tc.2006.151.
***** External links[edit] *****
    * "Advanced_Synchronization_in_Java_Threads" by Scott Oaks and Henry Wong
    * Deadlock_Detection_Agents
    * DeadLock at the Portland Pattern Repository
    * Etymology_of_"Deadlock"
    * v
    * t
    * e
Concurrent_computing
General              * Concurrency
                     * Concurrency_control
                     * CSP
                     * CCS
                     * ACP
                     * LOTOS
Process_calculi      * Ï-calculus
                     * Ambient_calculus
                     * API-Calculus
                     * PEPA
                     * Join-calculus
                     * ABA_problem
                     * Cigarette_smokers_problem
                     * Deadlock
Classic problems     * Dining_philosophers_problem
                     * Producerâconsumer_problem
                     * Race_condition
                     * Readersâwriters_problem
                     * Sleeping_barber_problem
    * [Category] Category:_Concurrent_computing

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Deadlock&oldid=908880825"
Categories:
    * Concurrency_(computer_science)
    * Software_bugs
    * Software_anomalies
    * Distributed_computing_problems
    * Edsger_W._Dijkstra
Hidden categories:
    * Use_dmy_dates_from_August_2012
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2016
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 1 August 2019, at 16:33 (UTC).
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
