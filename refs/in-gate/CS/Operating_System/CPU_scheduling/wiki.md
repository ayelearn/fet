The following text has been accessed from https://en.wikipedia.org/wiki/Scheduling_(computing)#SHORT-TERM at Fri Aug 9 01:12:14 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Scheduling (computing) ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about scheduling in operating systems generally. For networks,
see Network_scheduler. For other uses, see Scheduling_(disambiguation).
 This article needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be challenged
 and removed.
 Find sources: "Scheduling" computing â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (December 2013)(Learn_how_and_when_to_remove_this_template_message)
In computing, scheduling is the method by which work is assigned to resources
that complete the work. The work may be virtual computation elements such as
threads, processes or data flows, which are in turn scheduled onto hardware
resources such as processors, network_links or expansion_cards.
A scheduler is what carries out the scheduling activity. Schedulers are often
implemented so they keep all computer resources busy (as in load_balancing),
allow multiple users to share system resources effectively, or to achieve a
target quality_of_service. Scheduling is fundamental to computation itself, and
an intrinsic part of the execution_model of a computer system; the concept of
scheduling makes it possible to have computer_multitasking with a single
central_processing_unit (CPU).
⁰
***** Contents *****
    * 1_Goals
    * 2_Types_of_operating_system_schedulers
          o 2.1_Process_scheduler
                # 2.1.1_Long-term_scheduling
                # 2.1.2_Medium-term_scheduling
                # 2.1.3_Short-term_scheduling
                # 2.1.4_Dispatcher
    * 3_Scheduling_disciplines
          o 3.1_First_come,_first_served
          o 3.2_Priority_scheduling
          o 3.3_Shortest_remaining_time_first
          o 3.4_Fixed_priority_pre-emptive_scheduling
          o 3.5_Round-robin_scheduling
          o 3.6_Multilevel_queue_scheduling
          o 3.7_Work-conserving_schedulers
          o 3.8_Scheduling_optimization_problems
          o 3.9_Manual_scheduling
          o 3.10_Choosing_a_scheduling_algorithm
    * 4_Operating_system_process_scheduler_implementations
          o 4.1_OS/360_and_successors
          o 4.2_Windows
          o 4.3_Classic_Mac_OS_and_macOS
          o 4.4_AIX
          o 4.5_Linux
                # 4.5.1_Linux_2.4
                # 4.5.2_Linux_2.6.0_to_Linux_2.6.22
                # 4.5.3_Since_Linux_2.6.23
          o 4.6_FreeBSD
          o 4.7_NetBSD
          o 4.8_Solaris
          o 4.9_Summary
    * 5_See_also
    * 6_Notes
    * 7_References
    * 8_Further_reading
***** Goals[edit] *****
A scheduler may aim at one or more of many goals, for example: maximizing
throughput (the total amount of work completed per time unit); minimizing wait
time (time from work becoming ready until the first point it begins execution);
minimizing latency or response_time (time from work becoming ready until it is
finished in case of batch activity,[1][2][3] or until the system responds and
hands the first output to the user in case of interactive activity);[4] or
maximizing fairness (equal CPU time to each process, or more generally
appropriate times according to the priority and workload of each process). In
practice, these goals often conflict (e.g. throughput versus latency), thus a
scheduler will implement a suitable compromise. Preference is measured by any
one of the concerns mentioned above, depending upon the user's needs and
objectives.
In real-time environments, such as embedded_systems for automatic_control in
industry (for example robotics), the scheduler also must ensure that processes
can meet deadlines; this is crucial for keeping the system stable. Scheduled
tasks can also be distributed to remote devices across a network and managed
through an administrative back end.
***** Types of operating system schedulers[edit] *****
See also: Network_scheduler, I/O_scheduling, and Job_scheduler
The scheduler is an operating system module that selects the next jobs to be
admitted into the system and the next process to run. Operating systems may
feature up to three distinct scheduler types: a long-term scheduler (also known
as an admission scheduler or high-level scheduler), a mid-term or medium-term
scheduler, and a short-term scheduler. The names suggest the relative frequency
with which their functions are performed.
**** Process scheduler[edit] ****
The process scheduler is a part of the operating system that decides which
process runs at a certain point in time. It usually has the ability to pause a
running process, move it to the back of the running queue and start a new
process; such a scheduler is known as preemptive scheduler, otherwise it is a
cooperative scheduler.[5]
*** Long-term scheduling[edit] ***
The long-term scheduler, or admission scheduler, decides which jobs or
processes are to be admitted to the ready queue (in main memory); that is, when
an attempt is made to execute a program, its admission to the set of currently
executing processes is either authorized or delayed by the long-term scheduler.
Thus, this scheduler dictates what processes are to run on a system, and the
degree of concurrency to be supported at any one time – whether many or few
processes are to be executed concurrently, and how the split between I/O-
intensive and CPU-intensive processes is to be handled. The long-term scheduler
is responsible for controlling the degree of multiprogramming.
In general, most processes can be described as either I/O-bound or CPU-bound.
An I/O-bound process is one that spends more of its time doing I/O than it
spends doing computations. A CPU-bound process, in contrast, generates I/
O requests infrequently, using more of its time doing computations. It is
important that a long-term scheduler selects a good process mix of I/O-bound
and CPU-bound processes. If all processes are I/O-bound, the ready queue will
almost always be empty, and the short-term scheduler will have little to do. On
the other hand, if all processes are CPU-bound, the I/O waiting queue will
almost always be empty, devices will go unused, and again the system will be
unbalanced. The system with the best performance will thus have a combination
of CPU-bound and I/O-bound processes. In modern operating systems, this is used
to make sure that real-time processes get enough CPU time to finish their
tasks.[6]
Long-term scheduling is also important in large-scale systems such as batch
processing systems, computer_clusters, supercomputers, and render_farms. For
example, in concurrent_systems, coscheduling of interacting processes is often
required to prevent them from blocking due to waiting on each other. In these
cases, special-purpose job_scheduler software is typically used to assist these
functions, in addition to any underlying admission scheduling support in the
operating system.
*** Medium-term scheduling[edit] ***
The medium-term scheduler temporarily removes processes from main memory and
places them in secondary memory (such as a hard_disk_drive) or vice versa,
which is commonly referred to as "swapping out" or "swapping in" (also
incorrectly as "paging out" or "paging in"). The medium-term scheduler may
decide to swap out a process which has not been active for some time, or a
process which has a low priority, or a process which is page_faulting
frequently, or a process which is taking up a large amount of memory in order
to free up main memory for other processes, swapping the process back in later
when more memory is available, or when the process has been unblocked and is no
longer waiting for a resource. [Stallings, 396] [Stallings, 370]
In many systems today (those that support mapping virtual address space to
secondary storage other than the swap file), the medium-term scheduler may
actually perform the role of the long-term scheduler, by treating binaries as
"swapped out processes" upon their execution. In this way, when a segment of
the binary is required it can be swapped in on demand, or "lazy loaded".
[Stallings, 394]
*** Short-term scheduling[edit] ***
The short-term scheduler (also known as the CPU scheduler) decides which of the
ready, in-memory processes is to be executed (allocated a CPU) after a clock
interrupt, an I/O interrupt, an operating system_call or another form of
signal. Thus the short-term scheduler makes scheduling decisions much more
frequently than the long-term or mid-term schedulers – a scheduling decision
will at a minimum have to be made after every time slice, and these are very
short. This scheduler can be preemptive, implying that it is capable of
forcibly removing processes from a CPU when it decides to allocate that CPU to
another process, or non-preemptive (also known as "voluntary" or "co-
operative"), in which case the scheduler is unable to "force" processes off the
CPU.
A preemptive scheduler relies upon a programmable_interval_timer which invokes
an interrupt_handler that runs in kernel_mode and implements the scheduling
function.
*** Dispatcher[edit] ***
Another component that is involved in the CPU-scheduling function is the
dispatcher, which is the module that gives control of the CPU to the process
selected by the short-term scheduler. It receives control in kernel mode as the
result of an interrupt or system call. The functions of a dispatcher mop the
following:
    * Context_switches, in which the dispatcher saves the state (also known as
      context) of the process or thread that was previously running; the
      dispatcher then loads the initial or previously saved state of the new
      process.
    * Switching to user mode.
    * Jumping to the proper location in the user program to restart that
      program indicated by its new state.
The dispatcher should be as fast as possible, since it is invoked during every
process switch. During the context switches, the processor is virtually idle
for a fraction of time, thus unnecessary context switches should be avoided.
The time it takes for the dispatcher to stop one process and start another is
known as the dispatch latency.[6]:155
***** Scheduling disciplines[edit] *****
Scheduling disciplines are algorithms used for distributing resources among
parties which simultaneously and asynchronously request them. Scheduling
disciplines are used in routers (to handle packet traffic) as well as in
operating_systems (to share CPU_time among both threads and processes), disk
drives (I/O_scheduling), printers (print_spooler), most embedded systems, etc.
The main purposes of scheduling algorithms are to minimize resource_starvation
and to ensure fairness amongst the parties utilizing the resources. Scheduling
deals with the problem of deciding which of the outstanding requests is to be
allocated resources. There are many different scheduling algorithms. In this
section, we introduce several of them.
In packet-switched computer_networks and other statistical_multiplexing, the
notion of a scheduling algorithm is used as an alternative to first-come_first-
served queuing of data packets.
The simplest best-effort scheduling algorithms are round-robin, fair_queuing (a
max-min_fair scheduling algorithm), proportionally_fair scheduling and maximum
throughput. If differentiated or guaranteed quality_of_service is offered, as
opposed to best-effort communication, weighted_fair_queuing may be utilized.
In advanced packet radio wireless networks such as HSDPA (High-Speed Downlink
Packet Access) 3.5G cellular system, channel-dependent scheduling may be used
to take advantage of channel_state_information. If the channel conditions are
favourable, the throughput and system_spectral_efficiency may be increased. In
even more advanced systems such as LTE, the scheduling is combined by channel-
dependent packet-by-packet dynamic_channel_allocation, or by assigning OFDMA
multi-carriers or other frequency-domain_equalization components to the users
that best can utilize them.[7]
**** First come, first served[edit] ****
Main article: FIFO_(computing_and_electronics)
A sample thread_pool (green boxes) with a queue (FIFO) of waiting tasks (blue)
and a queue of completed tasks (yellow)
First in, first out (FIFO), also known as first come, first served (FCFS), is
the simplest scheduling algorithm. FIFO simply queues processes in the order
that they arrive in the ready queue. This is commonly used for a task queue,
for example as illustrated in this section.
    * Since context switches only occur upon process termination, and no
      reorganization of the process queue is required, scheduling overhead is
      minimal.
    * Throughput can be low, because long processes can be holding the CPU,
      causing the short processes to wait for a long time (known as the convoy
      effect).
    * No starvation, because each process gets chance to be executed after a
      definite time.
    * Turnaround_time, waiting time and response time depends on the order of
      their arrival and can be high for the same reasons above.
    * No prioritization occurs, thus this system has trouble meeting process
      deadlines.
    * The lack of prioritization means that as long as every process eventually
      completes, there is no starvation. In an environment where some processes
      might not complete, there can be starvation.
    * It is based on queuing.
**** Priority scheduling[edit] ****
Main article: Earliest_deadline_first_scheduling
See also: Deadline-monotonic_scheduling
Earliest deadline first (EDF) or least time to go is a dynamic scheduling
algorithm used in real-time operating systems to place processes in a priority
queue. Whenever a scheduling event occurs (a task finishes, new task is
released, etc.), the queue will be searched for the process closest to its
deadline, which will be the next to be scheduled for execution.
**** Shortest remaining time first[edit] ****
Main article: Shortest_remaining_time
Similar to shortest_job_first (SJF). With this strategy the scheduler arranges
processes with the least estimated processing time remaining to be next in the
queue. This requires advanced knowledge or estimations about the time required
for a process to complete.
    * If a shorter process arrives during another process' execution, the
      currently running process is interrupted (known as preemption), dividing
      that process into two separate computing blocks. This creates excess
      overhead through additional context switching. The scheduler must also
      place each incoming process into a specific place in the queue, creating
      additional overhead.
    * This algorithm is designed for maximum throughput in most scenarios.
    * Waiting time and response time increase as the process's computational
      requirements increase. Since turnaround time is based on waiting time
      plus processing time, longer processes are significantly affected by
      this. Overall waiting time is smaller than FIFO, however since no process
      has to wait for the termination of the longest process.
    * No particular attention is given to deadlines, the programmer can only
      attempt to make processes with deadlines as short as possible.
    * Starvation is possible, especially in a busy system with many small
      processes being run.
    * To use this policy we should have at least two processes of different
      priority
**** Fixed priority pre-emptive scheduling[edit] ****
Main article: Fixed_priority_pre-emptive_scheduling
The operating system assigns a fixed priority rank to every process, and the
scheduler arranges the processes in the ready queue in order of their priority.
Lower-priority processes get interrupted by incoming higher-priority processes.
    * Overhead is not minimal, nor is it significant.
    * FPPS has no particular advantage in terms of throughput over FIFO
      scheduling.
    * If the number of rankings is limited, it can be characterized as a
      collection of FIFO queues, one for each priority ranking. Processes in
      lower-priority queues are selected only when all of the higher-priority
      queues are empty.
    * Waiting time and response time depend on the priority of the process.
      Higher-priority processes have smaller waiting and response times.
    * Deadlines can be met by giving processes with deadlines a higher
      priority.
    * Starvation of lower-priority processes is possible with large numbers of
      high-priority processes queuing for CPU time.
**** Round-robin scheduling[edit] ****
Main article: Round-robin_scheduling
The scheduler assigns a fixed time unit per process, and cycles through them.
If process completes within that time-slice it gets terminated otherwise it is
rescheduled after giving a chance to all other processes.
    * RR scheduling involves extensive overhead, especially with a small time
      unit.
    * Balanced throughput between FCFS/ FIFO and SJF/SRTF, shorter jobs are
      completed faster than in FIFO and longer processes are completed faster
      than in SJF.
    * Good average response time, waiting time is dependent on number of
      processes, and not average process length.
    * Because of high waiting times, deadlines are rarely met in a pure RR
      system.
    * Starvation can never occur, since no priority is given. Order of time
      unit allocation is based upon process arrival time, similar to FIFO.
    * If Time-Slice is large it becomes FCFS /FIFO or if it is short then it
      becomes SJF/SRTF.
**** Multilevel queue scheduling[edit] ****
Main article: Multilevel_queue
This is used for situations in which processes are easily divided into
different groups. For example, a common division is made between foreground
(interactive) processes and background (batch) processes. These two types of
processes have different response-time requirements and so may have different
scheduling needs. It is very useful for shared memory problems.
**** Work-conserving schedulers[edit] ****
Main article: Work-conserving_scheduler
A work-conserving_scheduler is a scheduler that always tries to keep the
scheduled resources busy, if there are submitted jobs ready to be scheduled. In
contrast, a non-work conserving scheduler is a scheduler that, in some cases,
may leave the scheduled resources idle despite the presence of jobs ready to be
scheduled.
**** Scheduling optimization problems[edit] ****
There are several scheduling problems in which the goal is to decide which job
goes to which station at what time, such that the total makespan is minimized:
    * Job_shop_scheduling – there are n jobs and m identical stations. Each job
      should be executed on a single machine. This is usually regarded as an
      online problem.
    * Open-shop_scheduling – there are n jobs and m different stations. Each
      job should spend some time at each station, in a free order.
    * Flow_shop_scheduling – there are n jobs and m different stations. Each
      job should spend some time at each station, in a pre-determined order.
**** Manual scheduling[edit] ****
A very common method in embedded systems is to schedule jobs manually. This can
for example be done in a time-multiplexed fashion. Sometimes the kernel is
divided in three or more parts: Manual scheduling, preemptive and interrupt
level. Exact methods for scheduling jobs are often proprietary.
    * No resource starvation problems
    * Very high predictability; allows implementation of hard real-time systems
    * Almost no overhead
    * May not be optimal for all applications
    * Effectiveness is completely dependent on the implementation
**** Choosing a scheduling algorithm[edit] ****
When designing an operating system, a programmer must consider which scheduling
algorithm will perform best for the use the system is going to see. There is no
universal âbestâ scheduling algorithm, and many operating systems use
extended or combinations of the scheduling algorithms above.
For example, Windows_NT/XP/Vista uses a multilevel_feedback_queue, a
combination of fixed-priority preemptive scheduling, round-robin, and first in,
first out algorithms. In this system, threads can dynamically increase or
decrease in priority depending on if it has been serviced already, or if it has
been waiting extensively. Every priority level is represented by its own queue,
with round-robin_scheduling among the high-priority threads and FIFO among the
lower-priority ones. In this sense, response time is short for most threads,
and short but critical system threads get completed very quickly. Since threads
can only use one time unit of the round-robin in the highest-priority queue,
starvation can be a problem for longer high-priority threads.
***** Operating system process scheduler implementations[edit] *****
The algorithm used may be as simple as round-robin in which each process is
given equal time (for instance 1 ms, usually between 1 ms and 100 ms) in a
cycling list. So, process A executes for 1 ms, then process B, then process C,
then back to process A.
More advanced algorithms take into account process priority, or the importance
of the process. This allows some processes to use more time than other
processes. The kernel always uses whatever resources it needs to ensure proper
functioning of the system, and so can be said to have infinite priority. In SMP
systems, processor_affinity is considered to increase overall system
performance, even if it may cause a process itself to run more slowly. This
generally improves performance by reducing cache_thrashing.
**** OS/360 and successors[edit] ****
IBM OS/360 was available with three different schedulers. The differences were
such that the variants were often considered three different operating systems:
    * The Single Sequential Scheduler option, also known as the Primary Control
      Program (PCP) provided sequential execution of a single stream of jobs.
    * The Multiple Sequential Scheduler option, known as Multiprogramming with
      a Fixed Number of Tasks (MFT) provided execution of multiple concurrent
      jobs. Execution was governed by a priority which had a default for each
      stream or could be requested separately for each job. MFT version II
      added subtasks (threads), which executed at a priority based on that of
      the parent job. Each job stream defined the maximum amount of memory
      which could be used by any job in that stream.
    * The Multiple Priority Schedulers option, or Multiprogramming with a
      Variable Number of Tasks (MVT), featured subtasks from the start; each
      job requested the priority and memory it required before execution.
Later virtual storage versions of MVS added a Workload_Manager feature to the
scheduler, which schedules processor resources according to an elaborate scheme
defined by the installation.
**** Windows[edit] ****
Very early MS-DOS and Microsoft Windows systems were non-multitasking, and as
such did not feature a scheduler. Windows_3.1x used a non-preemptive scheduler,
meaning that it did not interrupt programs. It relied on the program to end or
tell the OS that it didn't need the processor so that it could move on to
another process. This is usually called cooperative multitasking. Windows 95
introduced a rudimentary preemptive scheduler; however, for legacy support
opted to let 16 bit applications run without preemption.[8]
Windows_NT-based operating systems use a multilevel feedback queue. 32 priority
levels are defined, 0 through to 31, with priorities 0 through 15 being
"normal" priorities and priorities 16 through 31 being soft real-time
priorities, requiring privileges to assign. 0 is reserved for the Operating
System. Users can select 5 of these priorities to assign to a running
application from the Task Manager application, or through thread management
APIs. The kernel may change the priority level of a thread depending on its I/
O and CPU usage and whether it is interactive (i.e. accepts and responds to
input from humans), raising the priority of interactive and I/O bounded
processes and lowering that of CPU bound processes, to increase the
responsiveness of interactive applications.[9] The scheduler was modified in
Windows_Vista to use the cycle_counter_register of modern processors to keep
track of exactly how many CPU cycles a thread has executed, rather than just
using an interval-timer interrupt routine.[10] Vista also uses a priority
scheduler for the I/O queue so that disk defragmenters and other such programs
do not interfere with foreground operations.[11]
**** Classic Mac OS and macOS[edit] ****
Mac OS 9 uses cooperative scheduling for threads, where one process controls
multiple cooperative threads, and also provides preemptive scheduling for
multiprocessing tasks. The kernel schedules multiprocessing tasks using a
preemptive scheduling algorithm. All Process Manager processes run within a
special multiprocessing task, called the "blue task". Those processes are
scheduled cooperatively, using a round-robin_scheduling algorithm; a process
yields control of the processor to another process by explicitly calling a
blocking_function such as WaitNextEvent. Each process has its own copy of the
Thread_Manager that schedules that process's threads cooperatively; a thread
yields control of the processor to another thread by calling YieldToAnyThread
or YieldToThread.[12]
macOS uses a multilevel feedback queue, with four priority bands for threads –
normal, system high priority, kernel mode only, and real-time.[13] Threads are
scheduled preemptively; macOS also supports cooperatively scheduled threads in
its implementation of the Thread Manager in Carbon.[12]
**** AIX[edit] ****
In AIX Version 4 there are three possible values for thread scheduling policy:
    * First In, First Out: Once a thread with this policy is scheduled, it runs
      to completion unless it is blocked, it voluntarily yields control of the
      CPU, or a higher-priority thread becomes dispatchable. Only fixed-
      priority threads can have a FIFO scheduling policy.
    * Round Robin: This is similar to the AIX Version 3 scheduler round-robin
      scheme based on 10ms time slices. When a RR thread has control at the end
      of the time slice, it moves to the tail of the queue of dispatchable
      threads of its priority. Only fixed-priority threads can have a Round
      Robin scheduling policy.
    * OTHER: This policy is defined by POSIX1003.4a as implementation-defined.
      In AIX Version 4, this policy is defined to be equivalent to RR, except
      that it applies to threads with non-fixed priority. The recalculation of
      the running thread's priority value at each clock interrupt means that a
      thread may lose control because its priority value has risen above that
      of another dispatchable thread. This is the AIX Version 3 behavior.
Threads are primarily of interest for applications that currently consist of
several asynchronous processes. These applications might impose a lighter load
on the system if converted to a multithreaded structure.
AIX 5 implements the following scheduling policies: FIFO, round robin, and a
fair round robin. The FIFO policy has three different implementations: FIFO,
FIFO2, and FIFO3. The round robin policy is named SCHED_RR in AIX, and the fair
round robin is called SCHED_OTHER.[14]
**** Linux[edit] ****
A highly simplified structure of the Linux kernel, which includes process
schedulers, I/O schedulers, and packet_schedulers
*** Linux 2.4[edit] ***
In Linux 2.4, an O(n)_scheduler with a multilevel_feedback_queue with priority
levels ranging from 0 to 140 was used; 0–99 are reserved for real-time tasks
and 100–140 are considered nice task levels. For real-time tasks, the time
quantum for switching processes was approximately 200 ms, and for nice tasks
approximately 10 ms.[citation_needed] The scheduler ran through the run_queue
of all ready processes, letting the highest priority processes go first and run
through their time slices, after which they will be placed in an expired queue.
When the active queue is empty the expired queue will become the active queue
and vice versa.
However, some enterprise Linux_distributions such as SUSE_Linux_Enterprise
Server replaced this scheduler with a backport of the O(1)_scheduler (which was
maintained by Alan_Cox in his Linux 2.4-ac Kernel series) to the Linux 2.4
kernel used by the distribution.
*** Linux 2.6.0 to Linux 2.6.22[edit] ***
In versions 2.6.0 to 2.6.22, the kernel used an O(1)_scheduler developed by
Ingo_Molnar and many other kernel developers during the Linux 2.5 development.
For many kernel in time frame, Con_Kolivas developed patch sets which improved
interactivity with this scheduler or even replaced it with his own schedulers.
*** Since Linux 2.6.23[edit] ***
Con Kolivas' work, most significantly his implementation of "fair_scheduling"
named "Rotating Staircase Deadline", inspired Ingo MolnÃ¡r to develop the
Completely_Fair_Scheduler as a replacement for the earlier O(1)_scheduler,
crediting Kolivas in his announcement.[15] CFS is the first implementation of a
fair queuing process_scheduler widely used in a general-purpose operating
system.[16]
The Completely_Fair_Scheduler (CFS) uses a well-studied, classic scheduling
algorithm called fair_queuing originally invented for packet_networks. Fair
queuing had been previously applied to CPU scheduling under the name stride
scheduling. The fair queuing CFS scheduler has a scheduling complexity of O(log
N), where N is the number of tasks in the runqueue. Choosing a task can be done
in constant time, but reinserting a task after it has run requires O(log N)
operations, because the run_queue is implemented as a red-black_tree.
The Brain_Fuck_Scheduler (BFS), also created by Con Kolivas, is an alternative
to the CFS.
**** FreeBSD[edit] ****
FreeBSD uses a multilevel feedback queue with priorities ranging from 0â255.
0â63 are reserved for interrupts, 64â127 for the top half of the kernel,
128â159 for real-time user threads, 160â223 for time-shared user threads,
and 224â255 for idle user threads. Also, like Linux, it uses the active queue
setup, but it also has an idle queue.[17]
**** NetBSD[edit] ****
NetBSD uses a multilevel feedback queue with priorities ranging from 0â223.
0â63 are reserved for time-shared threads (default, SCHED_OTHER policy),
64â95 for user threads which entered kernel_space, 96-128 for kernel threads,
128â191 for user real-time threads (SCHED_FIFO and SCHED_RR policies), and
192â223 for software_interrupts.
**** Solaris[edit] ****
Solaris uses a multilevel feedback queue with priorities ranging between 0 and
169. Priorities 0–59 are reserved for time-shared threads, 60–99 for system
threads, 100–159 for real-time threads, and 160–169 for low priority
interrupts. Unlike Linux,[17] when a process is done using its time quantum, it
is given a new priority and put back in the queue. Solaris 9 introduced two new
scheduling classes, namely fixed priority class and fair share class. The
threads with fixed priority have the same priority range as that of the time-
sharing class, but their priorities are not dynamically adjusted. The fair
scheduling class uses CPU shares to prioritize threads for scheduling
decisions. CPU shares indicate the entitlement to CPU resources. They are
allocated to a set of processes, which are collectively known as a project.[6]
**** Summary[edit] ****
Operating System                Preemption Algorithm
Amiga_OS                        Yes        Prioritized round-robin_scheduling
FreeBSD                         Yes        Multilevel_feedback_queue
Linux_kernel before 2.6.0       Yes        Multilevel_feedback_queue
Linux kernel 2.6.0–2.6.23     Yes        O(1)_scheduler
Linux kernel after 2.6.23       Yes        Completely_Fair_Scheduler
classic_Mac_OS pre-9            None       Cooperative_scheduler
                                           Preemptive scheduler for MP tasks,
Mac_OS_9                        Some       and cooperative for processes and
                                           threads
macOS                           Yes        Multilevel_feedback_queue
NetBSD                          Yes        Multilevel_feedback_queue
Solaris                         Yes        Multilevel_feedback_queue
Windows_3.1x                    None       Cooperative_scheduler
                                           Preemptive scheduler for 32-bit
Windows_95, 98, Me              Half       processes, and cooperative for 16-
                                           bit processes
Windows_NT (including 2000, XP, Yes        Multilevel_feedback_queue
Vista, 7, and Server)
***** See also[edit] *****
    * Activity_selection_problem
    * Aging_(scheduling)
    * Atropos_scheduler
    * Automated_planning_and_scheduling
    * Cyclic_executive
    * Dynamic_priority_scheduling
    * Foreground-background
    * Interruptible_operating_system
    * Least_slack_time_scheduling
    * Lottery_scheduling
    * Priority_inversion
    * Process_states
    * Queuing_Theory
    * Rate-monotonic_scheduling
    * Resource-Task_Network
    * Scheduling_(production_processes)
    * Stochastic_scheduling
    * Time-utility_function
***** Notes[edit] *****
   1. ^C. L., Liu; James W., Layland (January 1973). "Scheduling Algorithms for
      Multiprogramming in a Hard-Real-Time Environment". Journal of the ACM.
      ACM. 20 (1): 46â61. doi:10.1145/321738.321743. We define the response
      time of a request for a certain task to be the time span between the
      request and the end of the response to that request.
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
   3. ^Kleinrock, Leonard (1976). Queueing_Systems,_Vol._2:_Computer
      Applications (1 ed.). Wiley-Interscience. p. 171. ISBN 047149111X. For a
      customer requiring x sec of service, his response time will equal his
      service time x plus his waiting time.
   4. ^Feitelson, Dror G. (2015). Workload_Modeling_for_Computer_Systems
      Performance_Evaluation. Cambridge University Press. Section 8.4 (Page
      422) in Version 1.03 of the freely available manuscript.
      ISBN 9781107078239. Retrieved 2015-10-17. if we denote the time that a
      job waits in the queue by tw, and the time it actually runs by tr, then
      the response time is r = tw + tr.
   5. ^Silberschatz, Abraham; Galvin, Peter Baer; Gagne, Greg (2012). Operating
      System_Concepts (9 ed.). Wiley Publishing. p. 187. ISBN 0470128720. In an
      interactive system, turnaround time may not be the best criterion. Often,
      a process can produce some output fairly early and can continue computing
      new results while previous results are being output to the user. Thus,
      another measure is the time from the submission of a request until the
      first response is produced. This measure, called response time, is the
      time it takes to start responding, not the time it takes to output the
      response.
   6. ^Paul Krzyzanowski (2014-02-19). "Process_Scheduling:_Who_gets_to_run
      next?". cs.rutgers.edu. Retrieved 2015-01-11.
   7. ^ a b cAbraham_Silberschatz, Peter Baer Galvin and Greg Gagne (2013).
      Operating System Concepts. 9. John Wiley & Sons, Inc. ISBN 978-1-118-
      06333-0.CS1 maint: Uses authors parameter (link)
   8. ^Guowang_Miao; Jens Zander; Ki Won Sung; Ben Slimane (2016). Fundamentals
      of Mobile Data Networks. Cambridge_University_Press. ISBN 1107143217.
   9. ^ Early_Windows at the Wayback_Machine (archive index)
  10. ^Sriram Krishnan. "A_Tale_of_Two_Schedulers_Windows_NT_and_Windows_CE".
      Archived from the_original on July 22, 2012.
  11. ^"Windows_Administration:_Inside_the_Windows_Vista_Kernel:_Part_1".
      Technet.microsoft.com. 2016-11-14. Retrieved 2016-12-09.
  12. ^ [1]
  13. ^ a b"Technical_Notes". Developer.apple.com. Retrieved 2016-12-09.
  14. ^"Guides_and_Sample_Code". Developer.apple.com. Retrieved 2016-12-09.
  15. ^ [2] Archived 2011-08-11 at the Wayback_Machine
  16. ^MolnÃ¡r,_Ingo (2007-04-13). "&#x5b;patch&#x5d;_Modular_Scheduler_Core
      and_Completely_Fair_Scheduler_&#x5b;CFS&#x5d;". linux-kernel (Mailing
      list).
  17. ^Tong Li; Dan Baumberger; Scott Hahn. "Efficient_and_Scalable
      Multiprocessor_Fair_Scheduling_Using_Distributed_Weighted_Round-Robin"
      (PDF). Happyli.org. Retrieved 2016-12-09.
  18. ^ a b"Comparison_of_Solaris,_Linux,_and_FreeBSD_Kernels" (PDF). Archived
      from the_original (PDF) on August 7, 2008.
***** References[edit] *****
    * BÅaÅ¼ewicz, Jacek; Ecker, K.H.; Pesch, E.; Schmidt, G.; Weglarz, J.
      (2001). Scheduling computer and manufacturing processes (2 ed.). Berlin
      [u.a.]: Springer. ISBN 3-540-41931-4.
Stallings, William (2004). Operating Systems Internals and Design Principles
(fourth edition). Prentice Hall. ISBN 0-13-031999-6.
Information_on_the_Linux_2.6_O(1)-scheduler
***** Further reading[edit] *****
    * Operating_Systems:_Three_Easy_Pieces by Remzi H. Arpaci-Dusseau and
      Andrea C. Arpaci-Dusseau. Arpaci-Dusseau Books, 2014. Relevant chapters:
      Scheduling:_Introduction Multi-level_Feedback_Queue Proportional-share
      Scheduling Multiprocessor_Scheduling
    * Brief_discussion_of_Job_Scheduling_algorithms
    * Understanding_the_Linux_Kernel:_Chapter_10_Process_Scheduling
    * Kerneltrap:_Linux_kernel_scheduler_articles
    * AIX_CPU_monitoring_and_tuning
    * Josh_Aas'_introduction_to_the_Linux_2.6.8.1_CPU_scheduler_implementation
    * Peter Brucker, Sigrid Knust. Complexity results for scheduling problems
      [3]
    * TORSCHE_Scheduling_Toolbox_for_Matlab is a toolbox of scheduling and
      graph algorithms.
    * A_survey_on_cellular_networks_packet_scheduling
    * Large-scale_cluster_management_at_Google_with_Borg
    * v
    * t
    * e
Processor scheduling
               * Deadline-monotonic
               * Earliest_deadline
               * Fair-share
               * Fixed-priority_pre-emptive
               * Foreground-background
               * Gang
               * Generalized_foreground-background
               * Highest_response_ratio_next
               * Lottery
               * Multilevel_feedback_queue
Algorithms     * Process_Contention_Scope
               * Proportional_share
               * Rate-monotonic
               * Round-robin
               * Shortest_job_next
               * Shortest_remaining_time
               * Statistical_time-division_multiplexing
               * Stride
               * Two-level
               * Windows_NT
               * YDS_algorithm
               * Brain_Fuck
               * Completely_Fair
               * O(1)
Linux          * O(n)
               * SCHED_DEADLINE
               * SCHED_FIFO
               * SCHED_NORMAL
Other          * Processor_affinity
               * Starvation
    * v
    * t
    * e
Operating_systems
                           * Advocacy
                           * Comparison
                           * Forensic_engineering
General                    * History
                           * Hobbyist_development
                           * List
                           * Timeline
                           * Usage_share
                                         * Exokernel
                                         * Hybrid
                                         * Microkernel
                       Architectures     * Monolithic
                                         * vkernel
Kernel                                   * Rump_kernel
                                         * Unikernel
                                         * Device_driver
                       Components        * Loadable_kernel_module
                                         * Microkernel
                                         * User_space
                                      * Context_switch
                                      * Interrupt
                                      * IPC
                       Concepts       * Process
                                      * Process_control_block
                                      * Real-time
Process_management                    * Thread
                                      * Time-sharing
                                      * Computer_multitasking
                                      * Fixed-priority_preemptive
                       Scheduling     * Multilevel_feedback_queue
                       algorithms     * Preemptive
                                      * Round-robin
                                      * Shortest_job_next
                           * Bus_error
                           * General_protection_fault
Memory_management and      * Memory_protection
resource protection        * Paging
                           * Protection_ring
                           * Segmentation_fault
                           * Virtual_memory
                           * Boot_loader
                           * Defragmentation
                           * Device_file
Storage access and         * File_attribute
file_systems               * Inode
                           * Journal
                           * Partition
                           * Virtual_file_system
                           * Virtual_tape_library
                           * AmigaOS
                           * Android
                           * BeOS
                           * BSD
                           * Chrome_OS
                           * Cosmos
                           * CP/M
                           * Darwin
                           * DOS
                           * Genode
                           * GNU
                           * Haiku
                           * illumos
                           * IncludeOS
                           * iOS
                                 o audioOS
                                 o iPadOS
                                 o tvOS
                                 o watchOS
                           * ITS
                           * Linux
                           * Macintosh
                                 o Classic_Mac_OS
                                 o macOS
                           * MINIX
                           * MorphOS
List                       * MUSIC/SP
                           * Nemesis
                           * NeXTSTEP
                           * NOS
                           * OpenVMS
                           * ORVYL
                           * OS/2
                           * OS-9
                           * OSv
                           * Pick
                           * QNX
                           * ReactOS
                           * RISC_OS
                           * RSTS/E
                           * RSX-11
                           * RT-11
                           * Solaris
                           * TOPS-10/TOPS-20
                           * TPF
                           * TRIPOS
                           * Unix
                           * Visi_On
                           * VM/CMS
                           * VS/9
                           * webOS
                           * Windows
                           * Xinu
                           * z/OS
                           * API
                           * Computer_network
                           * HAL
                           * Live_CD
                           * Live_USB
                           * OS_shell
Miscellaneous concepts           o CLI
                                 o GUI
                                 o NUI
                                 o TUI
                                 o VUI
                                 o ZUI
                           * PXE
    * v
    * t
    * e
Software_design_patterns
                  * Abstract_factory
                  * Builder
                  * Dependency_injection
                  * Factory_method
Creational        * Lazy_initialization
                  * Multiton
                  * Object_pool
                  * Prototype
                  * RAII
                  * Singleton
                  * Adapter
                  * Bridge
                  * Composite
                  * Decorator
                  * Delegation
Structural        * Facade
                  * Flyweight
                  * Front_controller
                  * Marker_interface
                  * Module
                  * Proxy
                  * Twin
                  * Blackboard
                  * Chain_of_responsibility
                  * Command
                  * Interpreter
                  * Iterator
                  * Mediator
                  * Memento
Behavioral        * Null_object
                  * Observer
                  * Servant
                  * Specification
                  * State
                  * Strategy
                  * Template_method
                  * Visitor
                  * Closure
                  * Currying
Functional        * Function_composition
                  * Functor
                  * Monad
                  * Generator
                  * Active_object
                  * Actor
                  * Balking
                  * Barrier
                  * Binding_properties
                  * Coroutine
                  * Compute_kernel
                  * Double-checked_locking
                  * Event-based_asynchronous
                  * Fiber
                  * Futex
                  * Futures_and_promises
Concurrency       * Guarded_suspension
                  * Immutable_object
                  * Join
                  * Lock
                  * Messaging
                  * Monitor
                  * Nuclear
                  * Proactor
                  * Reactor
                  * Read_write_lock
                  * Scheduler
                  * Thread_pool
                  * Thread-local_storage
                  * ADR
                  * Active_record
                  * Broker
                  * Clientâserver
                  * CBD
                  * DAO
                  * DTO
                  * DDD
                  * ECS
                  * EDA
                  * Front_controller
                  * Identity_map
                  * Interceptor
                  * Implicit_invocation
                  * Inversion_of_control
                  * Model_2
                  * MOM
Architectural     * Microservices
                  * MVA
                  * MVC
                  * MVP
                  * MVVM
                  * Monolithic
                  * Multitier
                  * Naked_objects
                  * ORB
                  * P2P
                  * Publishâsubscribe
                  * PAC
                  * REST
                  * SOA
                  * Service_locator
                  * SN
                  * SBA
                  * Specification
                  * Ambassador
                  * Anti-Corruption_Layer
                  * Bulkhead
                  * Cache-Aside
                  * Circuit_Breaker
                  * CQRS
                  * Compensating_Transaction
                  * Competing_Consumers
                  * Compute_Resource_Consolidation
                  * Event_Sourcing
                  * External_Configuration_Store
                  * Federated_Identity
                  * Gatekeeper
Cloud             * Index_Table
Distributed       * Leader_Election
                  * MapReduce
                  * Materialized_View
                  * Pipes
                  * Filters
                  * Priority_Queue
                  * Publisher-Subscriber
                  * Queue-Based_Load_Leveling
                  * Retry
                  * Scheduler_Agent_Supervisor
                  * Sharding
                  * Sidecar
                  * Strangler
                  * Throttling
                  * Valet_Key
                  * Business_delegate
                  * Composite_entity
                  * Intercepting_filter
Other             * Lazy_loading
                  * Mangler
                  * Mock_object
                  * Type_tunnel
                  * Method_chaining
Books             * Design_Patterns
                  * Enterprise_Integration_Patterns
                  * Christopher_Alexander
                  * Erich_Gamma
                  * Ralph_Johnson
                  * John_Vlissides
                  * Grady_Booch
People            * Kent_Beck
                  * Ward_Cunningham
                  * Martin_Fowler
                  * Robert_Martin
                  * Jim_Coplien
                  * Douglas_Schmidt
                  * Linda_Rising
Communities       * The_Hillside_Group
                  * The_Portland_Pattern_Repository

Retrieved from "https://en.wikipedia.org/w/index.php?title=Scheduling_
(computing)&oldid=908388602"
Categories:
    * Software_design_patterns
    * Operations_research
    * Planning
    * Scheduling_(computing)
    * Scheduling_algorithms
Hidden categories:
    * CS1_maint:_Uses_authors_parameter
    * Webarchive_template_wayback_links
    * Articles_needing_additional_references_from_December_2013
    * All_articles_needing_additional_references
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_December_2011
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
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 29 July 2019, at 11:57 (UTC).
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
