The following text has been accessed from https://en.wikipedia.org/wiki/Operating_system at Fri Aug 9 01:11:57 IST 2019
Creative_Commons_Attribution-ShareAlike_License



















[Page_semi-protected]
****** Operating system ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Operating systems
[Operating system placement.svg]
[About_this_image]
Common features
    * Process_management
    * Interrupts
    * Memory_management
    * File_system
    * Device_drivers
    * Networking
    * Security
    * I/O
    * v
    * t
    * e
An operating system (OS) is system_software that manages computer_hardware and
software resources and provides common services for computer_programs.
Time-sharing operating systems schedule_tasks for efficient use of the system
and may also include accounting software for cost allocation of processor_time,
mass_storage, printing, and other resources.
For hardware functions such as input_and_output and memory_allocation, the
operating system acts as an intermediary between programs and the computer
hardware,[1][2] although the application code is usually executed directly by
the hardware and frequently makes system_calls to an OS function or is
interrupted by it. Operating systems are found on many devices that contain a
computer – from cellular_phones and video_game_consoles to web_servers and
supercomputers.
The dominant desktop operating system is Microsoft_Windows with a market share
of around 82.74%. macOS by Apple_Inc. is in second place (13.23%), and the
varieties of Linux are collectively in third place (1.57%).[3] In the mobile
(smartphone and tablet combined) sector, use in 2017 is up to 70% of Google's
Android[4] and according to third quarter 2016 data, Android on smartphones is
dominant with 87.5 percent and a growth rate 10.3 percent per year, followed by
Apple's iOS with 12.1 percent and a per year decrease in market share of 5.2
percent, while other operating systems amount to just 0.3 percent.[5] Linux
distributions are dominant in the server and supercomputing sectors. Other
specialized classes of operating systems, such as embedded and real-time
systems, exist for many applications.
⁰
***** Contents *****
    * 1_Types_of_operating_systems
          o 1.1_Single-_and_multi-tasking
          o 1.2_Single-_and_multi-user
          o 1.3_Distributed
          o 1.4_Templated
          o 1.5_Embedded
          o 1.6_Real-time
          o 1.7_Library
    * 2_History
          o 2.1_Mainframes
          o 2.2_Microcomputers
    * 3_Examples
          o 3.1_Unix_and_Unix-like_operating_systems
                # 3.1.1_BSD_and_its_descendants
                # 3.1.2_macOS
                # 3.1.3_Linux
          o 3.2_Microsoft_Windows
          o 3.3_Other
    * 4_Components
          o 4.1_Kernel
                # 4.1.1_Program_execution
                # 4.1.2_Interrupts
                # 4.1.3_Modes
                # 4.1.4_Memory_management
                # 4.1.5_Virtual_memory
                # 4.1.6_Multitasking
                # 4.1.7_Disk_access_and_file_systems
                # 4.1.8_Device_drivers
          o 4.2_Networking
          o 4.3_Security
          o 4.4_User_interface
                # 4.4.1_Graphical_user_interfaces
    * 5_Real-time_operating_systems
    * 6_Operating_system_development_as_a_hobby
    * 7_Diversity_of_operating_systems_and_portability
    * 8_Market_share
    * 9_See_also
    * 10_References
    * 11_Further_reading
    * 12_External_links
***** Types of operating systems *****
**** Single- and multi-tasking ****
A single-tasking system can only run one program at a time, while a multi-
tasking operating system allows more than one program to be running in
concurrency. This is achieved by time-sharing, where the available processor
time is divided between multiple processes. These processes are each
interrupted repeatedly in time_slices by a task-scheduling subsystem of the
operating system. Multi-tasking may be characterized in preemptive and co-
operative types. In preemptive multitasking, the operating system slices the
CPU time and dedicates a slot to each of the programs. Unix-like operating
systems, such as Solaris and Linuxâas well as non-Unix-like, such as
AmigaOSâsupport preemptive multitasking. Cooperative multitasking is achieved
by relying on each process to provide time to the other processes in a defined
manner. 16-bit versions of Microsoft Windows used cooperative multi-tasking.
32-bit versions of both Windows NT and Win9x, used preemptive multi-tasking.
**** Single- and multi-user ****
Single-user operating systems have no facilities to distinguish users, but may
allow multiple programs to run in tandem.[6] A multi-user operating system
extends the basic concept of multi-tasking with facilities that identify
processes and resources, such as disk space, belonging to multiple users, and
the system permits multiple users to interact with the system at the same time.
Time-sharing operating systems schedule tasks for efficient use of the system
and may also include accounting software for cost allocation of processor time,
mass storage, printing, and other resources to multiple users.
**** Distributed ****
A distributed_operating_system manages a group of distinct computers and makes
them appear to be a single computer. The development of networked computers
that could be linked and communicate with each other gave rise to distributed
computing. Distributed computations are carried out on more than one machine.
When computers in a group work in cooperation, they form a distributed system.
[7]
**** Templated ****
In an OS, distributed and cloud_computing context, templating refers to
creating a single virtual_machine_image as a guest operating system, then
saving it as a tool for multiple running virtual machines. The technique is
used both in virtualization and cloud computing management, and is common in
large server warehouses.[8]
**** Embedded ****
Embedded_operating_systems are designed to be used in embedded_computer
systems. They are designed to operate on small machines like PDAs with less
autonomy. They are able to operate with a limited number of resources. They are
very compact and extremely efficient by design. Windows_CE and Minix_3 are some
examples of embedded operating systems.
**** Real-time ****
A real-time_operating_system is an operating system that guarantees to process
events or data by a specific moment in time. A real-time operating system may
be single- or multi-tasking, but when multitasking, it uses specialized
scheduling algorithms so that a deterministic nature of behavior is achieved.
An event-driven system switches between tasks based on their priorities or
external events while time-sharing operating systems switch tasks based on
clock interrupts.
**** Library ****
A library operating system is one in which the services that a typical
operating system provides, such as networking, are provided in the form of
libraries and composed with the application and configuration code to construct
a unikernel: a specialized, single_address_space, machine image that can be
deployed to cloud or embedded environments.
***** History *****
Main article: History_of_operating_systems
See also: Resident_monitor
Early computers were built to perform a series of single tasks, like a
calculator. Basic operating system features were developed in the 1950s, such
as resident_monitor functions that could automatically run different programs
in succession to speed up processing. Operating systems did not exist in their
modern and more complex forms until the early 1960s.[9] Hardware features were
added, that enabled use of runtime_libraries, interrupts, and parallel
processing. When personal_computers became popular in the 1980s, operating
systems were made for them similar in concept to those used on larger
computers.
In the 1940s, the earliest electronic digital systems had no operating systems.
Electronic systems of this time were programmed on rows of mechanical switches
or by jumper wires on plug boards. These were special-purpose systems that, for
example, generated ballistics tables for the military or controlled the
printing of payroll checks from data on punched paper cards. After programmable
general purpose computers were invented, machine languages (consisting of
strings of the binary digits 0 and 1 on punched paper tape) were introduced
that sped up the programming process (Stern, 1981).[full_citation_needed]
OS/360 was used on most IBM mainframe computers beginning in 1966, including
computers used by the Apollo_program.
In the early 1950s, a computer could execute only one program at a time. Each
user had sole use of the computer for a limited period of time and would arrive
at a scheduled time with program and data on punched paper cards or punched
tape. The program would be loaded into the machine, and the machine would be
set to work until the program completed or crashed. Programs could generally be
debugged via a front panel using toggle switches and panel lights. It is said
that Alan_Turing was a master of this on the early Manchester_Mark_1 machine,
and he was already deriving the primitive conception of an operating system
from the principles of the universal_Turing_machine.[9]
Later machines came with libraries of programs, which would be linked to a
user's program to assist in operations such as input and output and generating
computer_code from human-readable symbolic_code. This was the genesis of the
modern-day operating system. However, machines still ran a single job at a
time. At Cambridge University in England the job queue was at one time a
washing line (clothes_line) from which tapes were hung with different colored
clothes-pegs to indicate job-priority.[citation_needed]
An improvement was the Atlas_Supervisor introduced with the Manchester Atlas
commissioned in 1962, "considered by many to be the first recognisable modern
operating system".[10] Brinch_Hansen described it as "the most significant
breakthrough in the history of operating systems."[11]
**** Mainframes ****
Main article: History_of_IBM_mainframe_operating_systems
Through the 1950s, many major features were pioneered in the field of operating
systems on mainframe_computers, including batch_processing, input/output
interrupt, buffering, multitasking, spooling, runtime_libraries, link-loading,
and programs for sorting_records in files. These features were included or not
included in application software at the option of application programmers,
rather than in a separate operating system used by all applications. In 1959,
the SHARE_Operating_System was released as an integrated utility for the IBM
704, and later in the 709 and 7090 mainframes, although it was quickly
supplanted by IBSYS/IBJOB on the 709, 7090 and 7094.
During the 1960s, IBM's OS/360 introduced the concept of a single OS spanning
an entire product line, which was crucial for the success of the System/360
machines. IBM's current mainframe operating systems are distant_descendants of
this original system and applications written for OS/360 can still be run on
modern machines.[citation_needed]
OS/360 also pioneered the concept that the operating system keeps track of all
of the system resources that are used, including program and data space
allocation in main memory and file space in secondary storage, and file_locking
during update. When the process is terminated for any reason, all of these
resources are re-claimed by the operating system.
The alternative CP-67 system for the S/360-67 started a whole line of IBM
operating systems focused on the concept of virtual_machines. Other operating
systems used on IBM S/360 series mainframes included systems developed by IBM:
COS/360 (Compatibility Operating System), DOS/360 (Disk Operating System), TSS/
360 (Time Sharing System), TOS/360 (Tape Operating System), BOS/360 (Basic
Operating System), and ACP (Airline Control Program), as well as a few non-IBM
systems: MTS (Michigan Terminal System), MUSIC (Multi-User System for
Interactive Computing), and ORVYL (Stanford Timesharing System).
Control_Data_Corporation developed the SCOPE operating system in the 1960s, for
batch_processing. In cooperation with the University of Minnesota, the Kronos
and later the NOS operating systems were developed during the 1970s, which
supported simultaneous batch and timesharing use. Like many commercial
timesharing systems, its interface was an extension of the Dartmouth BASIC
operating systems, one of the pioneering efforts in timesharing and programming
languages. In the late 1970s, Control Data and the University of Illinois
developed the PLATO operating system, which used plasma panel displays and
long-distance time sharing networks. Plato was remarkably innovative for its
time, featuring real-time chat, and multi-user graphical games.
In 1961, Burroughs_Corporation introduced the B5000 with the MCP, (Master
Control_Program) operating system. The B5000 was a stack_machine designed to
exclusively support high-level languages with no machine language or assembler,
and indeed the MCP was the first OS to be written exclusively in a high-level
language – ESPOL, a dialect of ALGOL. MCP also introduced many other ground-
breaking innovations, such as being the first commercial implementation of
virtual_memory. During development of the AS/400, IBM made an approach to
Burroughs to license MCP to run on the AS/400 hardware. This proposal was
declined by Burroughs management to protect its existing hardware production.
MCP is still in use today in the Unisys ClearPath/MCP line of computers.
UNIVAC, the first commercial computer manufacturer, produced a series of EXEC
operating systems[citation_needed]. Like all early main-frame systems, this
batch-oriented system managed magnetic drums, disks, card readers and line
printers. In the 1970s, UNIVAC produced the Real-Time Basic (RTB) system to
support large-scale time sharing, also patterned after the Dartmouth BC system.
General_Electric and MIT developed General Electric Comprehensive Operating
Supervisor (GECOS), which introduced the concept of ringed security privilege
levels. After acquisition by Honeywell it was renamed General_Comprehensive
Operating_System (GCOS).
Digital Equipment Corporation developed many operating systems for its various
computer lines, including TOPS-10 and TOPS-20 time sharing systems for the 36-
bit PDP-10 class systems. Before the widespread use of UNIX, TOPS-10 was a
particularly popular system in universities, and in the early ARPANET
community. RT-11 was a single-user real-time OS for the PDP-11 class
minicomputer, and RSX-11 was the corresponding multi-user OS.
From the late 1960s through the late 1970s, several hardware capabilities
evolved that allowed similar or ported software to run on more than one system.
Early systems had utilized microprogramming to implement features on their
systems in order to permit different underlying computer_architectures to
appear to be the same as others in a series. In fact, most 360s after the 360/
40 (except the 360/165 and 360/168) were microprogrammed implementations.
The enormous investment in software for these systems made since the 1960s
caused most of the original computer manufacturers to continue to develop
compatible operating systems along with the hardware. Notable supported
mainframe operating systems include:
    * Burroughs_MCP – B5000, 1961 to Unisys Clearpath/MCP, present
    * IBM OS/360 – IBM_System/360, 1966 to IBM z/OS, present
    * IBM CP-67 – IBM_System/360, 1967 to IBM z/VM
    * UNIVAC EXEC_8 – UNIVAC_1108, 1967, to OS_2200 Unisys Clearpath Dorado,
      present
**** Microcomputers ****
PC DOS was an early personal computer OS that featured a command line
interface.
Mac OS by Apple_Computer became the first widespread OS to feature a graphical
user_interface. Many of its features such as windows and icons would later
become commonplace in GUIs.
The first microcomputers did not have the capacity or need for the elaborate
operating systems that had been developed for mainframes and minis;
minimalistic operating systems were developed, often loaded from ROM and known
as monitors. One notable early disk_operating_system was CP/M, which was
supported on many early microcomputers and was closely imitated by Microsoft's
MS-DOS, which became widely popular as the operating system chosen for the IBM
PC (IBM's version of it was called IBM DOS or PC_DOS). In the 1980s, Apple
Computer Inc. (now Apple_Inc.) abandoned its popular Apple_II series of
microcomputers to introduce the Apple_Macintosh computer with an innovative
graphical_user_interface (GUI) to the Mac_OS.
The introduction of the Intel_80386 CPU chip in October 1985,[12] with 32-bit
architecture and paging capabilities, provided personal computers with the
ability to run multitasking operating systems like those of earlier
minicomputers and mainframes. Microsoft responded to this progress by hiring
Dave_Cutler, who had developed the VMS operating system for Digital_Equipment
Corporation. He would lead the development of the Windows_NT operating system,
which continues to serve as the basis for Microsoft's operating systems line.
Steve_Jobs, a co-founder of Apple_Inc., started NeXT Computer Inc., which
developed the NEXTSTEP operating system. NEXTSTEP would later be acquired by
Apple_Inc. and used, along with code from FreeBSD as the core of Mac_OS_X
(macOS after latest name change).
The GNU_Project was started by activist and programmer Richard_Stallman with
the goal of creating a complete free_software replacement to the proprietary
UNIX operating system. While the project was highly successful in duplicating
the functionality of various parts of UNIX, development of the GNU_Hurd kernel
proved to be unproductive. In 1991, Finnish computer science student Linus
Torvalds, with cooperation from volunteers collaborating over the Internet,
released the first version of the Linux_kernel. It was soon merged with the GNU
user_space components and system_software to form a complete operating system.
Since then, the combination of the two major components has usually been
referred to as simply "Linux" by the software industry, a naming convention
that Stallman and the Free_Software_Foundation remain opposed to, preferring
the name GNU/Linux. The Berkeley Software Distribution, known as BSD, is the
UNIX derivative distributed by the University of California, Berkeley, starting
in the 1970s. Freely distributed and ported to many minicomputers, it
eventually also gained a following for use on PCs, mainly as FreeBSD, NetBSD
and OpenBSD.
***** Examples *****
**** Unix and Unix-like operating systems ****
Main article: Unix
Evolution of Unix systems
Unix was originally written in assembly_language.[13] Ken_Thompson wrote B,
mainly based on BCPL, based on his experience in the MULTICS project. B was
replaced by C, and Unix, rewritten in C, developed into a large, complex family
of inter-related operating systems which have been influential in every modern
operating system (see History).
The Unix-like family is a diverse group of operating systems, with several
major sub-categories including System_V, BSD, and Linux. The name "UNIX" is a
trademark of The_Open_Group which licenses it for use with any operating system
that has been shown to conform to their definitions. "UNIX-like" is commonly
used to refer to the large set of operating systems which resemble the original
UNIX.
Unix-like systems run on a wide variety of computer_architectures. They are
used heavily for servers in business, as well as workstations in academic and
engineering environments. Free UNIX variants, such as Linux and BSD, are
popular in these areas.
Four operating systems are certified by The_Open_Group (holder of the Unix
trademark) as Unix. HP's HP-UX and IBM's AIX are both descendants of the
original System V Unix and are designed to run only on their respective
vendor's hardware. In contrast, Sun_Microsystems's Solaris can run on multiple
types of hardware, including x86 and Sparc servers, and PCs. Apple's macOS, a
replacement for Apple's earlier (non-Unix) Mac OS, is a hybrid_kernel-based BSD
variant derived from NeXTSTEP, Mach, and FreeBSD.
Unix interoperability was sought by establishing the POSIX standard. The POSIX
standard can be applied to any operating system, although it was originally
created for various Unix variants.
*** BSD and its descendants ***
Main article: Berkeley_Software_Distribution
The first_server for the World_Wide_Web ran on NeXTSTEP, based on BSD.
A subgroup of the Unix family is the Berkeley_Software_Distribution family,
which includes FreeBSD, NetBSD, and OpenBSD. These operating systems are most
commonly found on webservers, although they can also function as a personal
computer OS. The Internet owes much of its existence to BSD, as many of the
protocols now commonly used by computers to connect, send and receive data over
a network were widely implemented and refined in BSD. The World_Wide_Web was
also first demonstrated on a number of computers running an OS based on BSD
called NeXTSTEP.
In 1974, University_of_California,_Berkeley installed its first Unix system.
Over time, students and staff in the computer science department there began
adding new programs to make things easier, such as text editors. When Berkeley
received new VAX computers in 1978 with Unix installed, the school's
undergraduates modified Unix even more in order to take advantage of the
computer's hardware possibilities. The Defense_Advanced_Research_Projects
Agency of the US Department_of_Defense took interest, and decided to fund the
project. Many schools, corporations, and government organizations took notice
and started to use Berkeley's version of Unix instead of the official one
distributed by AT&T.
Steve_Jobs, upon leaving Apple Inc. in 1985, formed NeXT_Inc., a company that
manufactured high-end computers running on a variation of BSD called NeXTSTEP.
One of these computers was used by Tim_Berners-Lee as the first webserver to
create the World Wide Web.
Developers like Keith_Bostic encouraged the project to replace any non-free
code that originated with Bell Labs. Once this was done, however, AT&T sued.
After two years of legal disputes, the BSD project spawned a number of free
derivatives, such as NetBSD and FreeBSD (both in 1993), and OpenBSD (from
NetBSD in 1995).
*** macOS ***
Main article: macOS
macOS (formerly "Mac OS X" and later "OS X") is a line of open_core graphical
operating systems developed, marketed, and sold by Apple_Inc., the latest of
which is pre-loaded on all currently shipping Macintosh computers. macOS is the
successor to the original classic_Mac_OS, which had been Apple's primary
operating system since 1984. Unlike its predecessor, macOS is a UNIX operating
system built on technology that had been developed at NeXT through the second
half of the 1980s and up until Apple purchased the company in early 1997. The
operating system was first released in 1999 as Mac_OS_X_Server_1.0, followed in
March 2001 by a client version (Mac_OS_X_v10.0_"Cheetah"). Since then, six more
distinct "client" and "server" editions of macOS have been released, until the
two were merged in OS_X_10.7_"Lion".
Prior to its merging with macOS, the server edition – macOS_Server – was
architecturally identical to its desktop counterpart and usually ran on Apple's
line of Macintosh server hardware. macOS Server included work group management
and administration software tools that provide simplified access to key network
services, including a mail_transfer_agent, a Samba_server, an LDAP server, a
domain_name_server, and others. With Mac_OS_X_v10.7_Lion, all server aspects of
Mac OS X Server have been integrated into the client version and the product
re-branded as "OS X" (dropping "Mac" from the name). The server tools are now
offered as an application.[14]
*** Linux ***
Main articles: Linux and Linux_kernel
Ubuntu, desktop Linux_distribution
The Linux kernel originated in 1991, as a project of Linus_Torvalds, while a
university student in Finland. He posted information about his project on a
newsgroup for computer students and programmers, and received support and
assistance from volunteers who succeeded in creating a complete and functional
kernel.
Linux is Unix-like, but was developed without any Unix code, unlike BSD and its
variants. Because of its open license model, the Linux_kernel code is available
for study and modification, which resulted in its use on a wide range of
computing machinery from supercomputers to smart-watches. Although estimates
suggest that Linux is used_on only 1.82% of all "desktop" (or laptop) PCs,[15]
it has been widely adopted for use in servers[16] and embedded systems[17] such
as cell phones. Linux has superseded Unix on many platforms and is used on most
supercomputers including the top 385.[18] Many of the same computers are also
on Green500 (but in different order), and Linux runs on the top 10. Linux is
also commonly used on other small energy-efficient computers, such as
smartphones and smartwatches. The Linux kernel is used in some popular
distributions, such as Red_Hat, Debian, Ubuntu, Linux_Mint and Google's
Android, Chrome_OS, and Chromium_OS.
**** Microsoft Windows ****
Main article: Microsoft_Windows
Microsoft Windows is a family of proprietary operating systems designed by
Microsoft_Corporation and primarily targeted to Intel architecture based
computers, with an estimated 88.9 percent total usage share on Web connected
computers.[15][19][20][21] The latest version is Windows_10.
In 2011, Windows 7 overtook Windows XP as most common version in use.[22][23]
[24]
Microsoft Windows was first released in 1985, as an operating_environment
running on top of MS-DOS, which was the standard operating system shipped on
most Intel architecture personal computers at the time. In 1995, Windows_95 was
released which only used MS-DOS as a bootstrap. For backwards compatibility,
Win9x could run real-mode MS-DOS[25][26] and 16-bit Windows_3.x[27] drivers.
Windows_ME, released in 2000, was the last version in the Win9x family. Later
versions have all been based on the Windows_NT kernel. Current client versions
of Windows run on IA-32, x86-64 and 32-bit ARM microprocessors.[28] In addition
Itanium is still supported in older server version Windows_Server_2008_R2. In
the past, Windows NT supported additional architectures.
Server editions of Windows are widely used. In recent years, Microsoft has
expended significant capital in an effort to promote the use of Windows as a
server_operating_system. However, Windows' usage on servers is not as
widespread as on personal computers as Windows competes against Linux and BSD
for server market share.[29][30]
ReactOS is a Windows-alternative operating system, which is being developed on
the principles of Windows – without using any of Microsoft's code.
**** Other ****
There have been many operating systems that were significant in their day but
are no longer so, such as AmigaOS; OS/2 from IBM and Microsoft; classic_Mac_OS,
the non-Unix precursor to Apple's macOS; BeOS; XTS-300; RISC_OS; MorphOS;
Haiku; BareMetal and FreeMint. Some are still used in niche markets and
continue to be developed as minority platforms for enthusiast communities and
specialist applications. OpenVMS, formerly from DEC, is still under active
development by Hewlett-Packard. Yet other operating systems are used almost
exclusively in academia, for operating systems education or to do research on
operating system concepts. A typical example of a system that fulfills both
roles is MINIX, while for example Singularity is used purely for research.
Another example is the Oberon_System designed at ETH_ZÃ¼rich by Niklaus_Wirth,
JÃ¼rg_Gutknecht and a group of students at the former Computer Systems
Institute in the 1980s. It was used mainly for research, teaching, and daily
work in Wirth's group.
Other operating systems have failed to win significant market share, but have
introduced innovations that have influenced mainstream operating systems, not
least Bell Labs' Plan_9.
***** Components *****
The components of an operating system all exist in order to make the different
parts of a computer work together. All user software needs to go through the
operating system in order to use any of the hardware, whether it be as simple
as a mouse or keyboard or as complex as an Internet component.
**** Kernel ****
Main article: Kernel_(computing)
A kernel connects the application software to the hardware of a computer.
With the aid of the firmware and device_drivers, the kernel provides the most
basic level of control over all of the computer's hardware devices. It manages
memory access for programs in the RAM, it determines which programs get access
to which hardware resources, it sets up or resets the CPU's operating states
for optimal operation at all times, and it organizes the data for long-term
non-volatile_storage with file_systems on such media as disks, tapes, flash
memory, etc.
*** Program execution ***
Main article: Process_(computing)
The operating system provides an interface between an application program and
the computer hardware, so that an application program can interact with the
hardware only by obeying rules and procedures programmed into the operating
system. The operating system is also a set of services which simplify
development and execution of application programs. Executing an application
program involves the creation of a process by the operating system kernel which
assigns memory space and other resources, establishes a priority for the
process in multi-tasking systems, loads program binary code into memory, and
initiates execution of the application program which then interacts with the
user and with hardware devices.
*** Interrupts ***
Main article: Interrupt
Interrupts are central to operating systems, as they provide an efficient way
for the operating system to interact with and react to its environment. The
alternative – having the operating system "watch" the various sources of input
for events (polling) that require action – can be found in older systems with
very small stacks (50 or 60 bytes) but is unusual in modern systems with large
stacks. Interrupt-based programming is directly supported by most modern CPUs.
Interrupts provide a computer with a way of automatically saving local register
contexts, and running specific code in response to events. Even very basic
computers support hardware interrupts, and allow the programmer to specify code
which may be run when that event takes place.
When an interrupt is received, the computer's hardware automatically suspends
whatever program is currently running, saves its status, and runs computer code
previously associated with the interrupt; this is analogous to placing a
bookmark in a book in response to a phone call. In modern operating systems,
interrupts are handled by the operating system's kernel. Interrupts may come
from either the computer's hardware or the running program.
When a hardware device triggers an interrupt, the operating system's kernel
decides how to deal with this event, generally by running some processing code.
The amount of code being run depends on the priority of the interrupt (for
example: a person usually responds to a smoke detector alarm before answering
the phone). The processing of hardware interrupts is a task that is usually
delegated to software called a device_driver, which may be part of the
operating system's kernel, part of another program, or both. Device drivers may
then relay information to a running program by various means.
A program may also trigger an interrupt to the operating system. If a program
wishes to access hardware, for example, it may interrupt the operating system's
kernel, which causes control to be passed back to the kernel. The kernel then
processes the request. If a program wishes additional resources (or wishes to
shed resources) such as memory, it triggers an interrupt to get the kernel's
attention.
*** Modes ***
Main articles: User_mode and Supervisor_mode
Privilege rings for the x86 microprocessor architecture available in protected
mode. Operating systems determine which processes run in each mode.
Modern microprocessors (CPU or MPU) support multiple modes of operation. CPUs
with this capability offer at least two modes: user_mode and supervisor_mode.
In general terms, supervisor mode operation allows unrestricted access to all
machine resources, including all MPU instructions. User mode operation sets
limits on instruction use and typically disallows direct access to machine
resources. CPUs might have other modes similar to user mode as well, such as
the virtual modes in order to emulate older processor types, such as 16-bit
processors on a 32-bit one, or 32-bit processors on a 64-bit one.
At power-on or reset, the system begins in supervisor mode. Once an operating
system kernel has been loaded and started, the boundary between user mode and
supervisor mode (also known as kernel mode) can be established.
Supervisor mode is used by the kernel for low level tasks that need
unrestricted access to hardware, such as controlling how memory is accessed,
and communicating with devices such as disk drives and video display devices.
User mode, in contrast, is used for almost everything else. Application
programs, such as word processors and database managers, operate within user
mode, and can only access machine resources by turning control over to the
kernel, a process which causes a switch to supervisor mode. Typically, the
transfer of control to the kernel is achieved by executing a software_interrupt
instruction, such as the Motorola 68000 TRAP instruction. The software
interrupt causes the microprocessor to switch from user mode to supervisor mode
and begin executing code that allows the kernel to take control.
In user mode, programs usually have access to a restricted set of
microprocessor instructions, and generally cannot execute any instructions that
could potentially cause disruption to the system's operation. In supervisor
mode, instruction execution restrictions are typically removed, allowing the
kernel unrestricted access to all machine resources.
The term "user mode resource" generally refers to one or more CPU registers,
which contain information that the running program isn't allowed to alter.
Attempts to alter these resources generally causes a switch to supervisor mode,
where the operating system can deal with the illegal operation the program was
attempting, for example, by forcibly terminating ("killing") the program).
*** Memory management ***
Main article: Memory_management
Among other things, a multiprogramming operating system kernel must be
responsible for managing all system memory which is currently in use by
programs. This ensures that a program does not interfere with memory already in
use by another program. Since programs time share, each program must have
independent access to memory.
Cooperative memory management, used by many early operating systems, assumes
that all programs make voluntary use of the kernel's memory manager, and do not
exceed their allocated memory. This system of memory management is almost never
seen any more, since programs often contain bugs which can cause them to exceed
their allocated memory. If a program fails, it may cause memory used by one or
more other programs to be affected or overwritten. Malicious programs or
viruses may purposefully alter another program's memory, or may affect the
operation of the operating system itself. With cooperative memory management,
it takes only one misbehaved program to crash the system.
Memory_protection enables the kernel to limit a process' access to the
computer's memory. Various methods of memory protection exist, including memory
segmentation and paging. All methods require some level of hardware support
(such as the 80286 MMU), which doesn't exist in all computers.
In both segmentation and paging, certain protected_mode registers specify to
the CPU what memory address it should allow a running program to access.
Attempts to access other addresses trigger an interrupt which cause the CPU to
re-enter supervisor_mode, placing the kernel in charge. This is called a
segmentation_violation or Seg-V for short, and since it is both difficult to
assign a meaningful result to such an operation, and because it is usually a
sign of a misbehaving program, the kernel generally resorts to terminating the
offending program, and reports the error.
Windows versions 3.1 through ME had some level of memory protection, but
programs could easily circumvent the need to use it. A general_protection_fault
would be produced, indicating a segmentation violation had occurred; however,
the system would often crash anyway.
*** Virtual memory ***
Main article: Virtual_memory
Further information: Page_fault
Many operating systems can "trick" programs into using memory scattered around
the hard disk and RAM as if it is one continuous chunk of memory, called
virtual memory.
The use of virtual memory addressing (such as paging or segmentation) means
that the kernel can choose what memory each program may use at any given time,
allowing the operating system to use the same memory locations for multiple
tasks.
If a program tries to access memory that isn't in its current range of
accessible memory, but nonetheless has been allocated to it, the kernel is
interrupted in the same way as it would if the program were to exceed its
allocated memory. (See section on memory management.) Under UNIX this kind of
interrupt is referred to as a page_fault.
When the kernel detects a page fault it generally adjusts the virtual memory
range of the program which triggered it, granting it access to the memory
requested. This gives the kernel discretionary power over where a particular
application's memory is stored, or even whether or not it has actually been
allocated yet.
In modern operating systems, memory which is accessed less frequently can be
temporarily stored on disk or other media to make that space available for use
by other programs. This is called swapping, as an area of memory can be used by
multiple programs, and what that memory area contains can be swapped or
exchanged on demand.
"Virtual memory" provides the programmer or the user with the perception that
there is a much larger amount of RAM in the computer than is really there.[31]
*** Multitasking ***
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (December 2018)(Learn_how_and_when_to_remove_this_template_message)
Main articles: Computer_multitasking and Process_management_(computing)
Further information: Context_switch, Preemptive_multitasking, and Cooperative
multitasking
Multitasking refers to the running of multiple independent computer programs on
the same computer; giving the appearance that it is performing the tasks at the
same time. Since most computers can do at most one or two things at one time,
this is generally done via time-sharing, which means that each program uses a
share of the computer's time to execute.
An operating system kernel contains a scheduling program which determines how
much time each process spends executing, and in which order execution control
should be passed to programs. Control is passed to a process by the kernel,
which allows the program access to the CPU and memory. Later, control is
returned to the kernel through some mechanism, so that another program may be
allowed to use the CPU. This so-called passing of control between the kernel
and applications is called a context_switch.
An early model which governed the allocation of time to programs was called
cooperative_multitasking. In this model, when control is passed to a program by
the kernel, it may execute for as long as it wants before explicitly returning
control to the kernel. This means that a malicious or malfunctioning program
may not only prevent any other programs from using the CPU, but it can hang the
entire system if it enters an infinite_loop.
Modern operating systems extend the concepts of application preemption to
device drivers and kernel code, so that the operating system has preemptive
control over internal run-times as well.
The philosophy governing preemptive_multitasking is that of ensuring that all
programs are given regular time on the CPU. This implies that all programs must
be limited in how much time they are allowed to spend on the CPU without being
interrupted. To accomplish this, modern operating system kernels make use of a
timed interrupt. A protected_mode timer is set by the kernel which triggers a
return to supervisor mode after the specified time has elapsed. (See above
sections on Interrupts and Dual Mode Operation.)
On many single user operating systems cooperative multitasking is perfectly
adequate, as home computers generally run a small number of well tested
programs. The AmigaOS is an exception, having preemptive multitasking from its
very first version. Windows_NT was the first version of Microsoft_Windows which
enforced preemptive multitasking, but it didn't reach the home user market
until Windows_XP (since Windows_NT was targeted at professionals).
*** Disk access and file systems ***
Main article: Virtual_file_system
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (December 2018)(Learn_how_and_when_to_remove_this_template_message)
File systems allow users and programs to organize and sort files on a computer,
often through the use of directories (or "folders").
Access to data stored on disks is a central feature of all operating systems.
Computers store data on disks using files, which are structured in specific
ways in order to allow for faster access, higher reliability, and to make
better use of the drive's available space. The specific way in which files are
stored on a disk is called a file_system, and enables files to have names and
attributes. It also allows them to be stored in a hierarchy of directories or
folders arranged in a directory_tree.
Early operating systems generally supported a single type of disk drive and
only one kind of file system. Early file systems were limited in their
capacity, speed, and in the kinds of file names and directory structures they
could use. These limitations often reflected limitations in the operating
systems they were designed for, making it very difficult for an operating
system to support more than one file system.
While many simpler operating systems support a limited range of options for
accessing storage systems, operating systems like UNIX and Linux support a
technology known as a virtual_file_system or VFS. An operating system such as
UNIX supports a wide array of storage devices, regardless of their design or
file_systems, allowing them to be accessed through a common application
programming_interface (API). This makes it unnecessary for programs to have any
knowledge about the device they are accessing. A VFS allows the operating
system to provide programs with access to an unlimited number of devices with
an infinite variety of file systems installed on them, through the use of
specific device_drivers and file system drivers.
A connected storage_device, such as a hard_drive, is accessed through a device
driver. The device driver understands the specific language of the drive and is
able to translate that language into a standard language used by the operating
system to access all disk drives. On UNIX, this is the language of block
devices.
When the kernel has an appropriate device driver in place, it can then access
the contents of the disk drive in raw format, which may contain one or more
file systems. A file system driver is used to translate the commands used to
access each specific file system into a standard set of commands that the
operating system can use to talk to all file systems. Programs can then deal
with these file systems on the basis of filenames, and directories/folders,
contained within a hierarchical structure. They can create, delete, open, and
close files, as well as gather various information about them, including access
permissions, size, free space, and creation and modification dates.
Various differences between file systems make supporting all file systems
difficult. Allowed characters in file names, case_sensitivity, and the presence
of various kinds of file_attributes makes the implementation of a single
interface for every file system a daunting task. Operating systems tend to
recommend using (and so support natively) file systems specifically designed
for them; for example, NTFS in Windows and ext3 and ReiserFS in Linux. However,
in practice, third party drivers are usually available to give support for the
most widely used file systems in most general-purpose operating systems (for
example, NTFS is available in Linux through NTFS-3g, and ext2/3 and ReiserFS
are available in Windows through third-party software).
Support for file systems is highly varied among modern operating systems,
although there are several common file systems which almost all operating
systems include support and drivers for. Operating systems vary on file system
support and on the disk formats they may be installed on. Under Windows, each
file system is usually limited in application to certain media; for example,
CDs must use ISO_9660 or UDF, and as of Windows_Vista, NTFS is the only file
system which the operating system can be installed on. It is possible to
install Linux onto many types of file systems. Unlike other operating systems,
Linux and UNIX allow any file system to be used regardless of the media it is
stored in, whether it is a hard drive, a disc (CD, DVD...), a USB flash drive,
or even contained within a file located on another file system.
*** Device drivers ***
Main article: Device_driver
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (December 2018)(Learn_how_and_when_to_remove_this_template_message)
A device_driver is a specific type of computer software developed to allow
interaction with hardware devices. Typically this constitutes an interface for
communicating with the device, through the specific computer bus or
communications subsystem that the hardware is connected to, providing commands
to and/or receiving data from the device, and on the other end, the requisite
interfaces to the operating system and software applications. It is a
specialized hardware-dependent computer program which is also operating system
specific that enables another program, typically an operating system or
applications software package or computer program running under the operating
system kernel, to interact transparently with a hardware device, and usually
provides the requisite interrupt handling necessary for any necessary
asynchronous time-dependent hardware interfacing needs.
The key design goal of device drivers is abstraction. Every model of hardware
(even within the same class of device) is different. Newer models also are
released by manufacturers that provide more reliable or better performance and
these newer models are often controlled differently. Computers and their
operating systems cannot be expected to know how to control every device, both
now and in the future. To solve this problem, operating systems essentially
dictate how every type of device should be controlled. The function of the
device driver is then to translate these operating system mandated function
calls into device specific calls. In theory a new device, which is controlled
in a new manner, should function correctly if a suitable driver is available.
This new driver ensures that the device appears to operate as usual from the
operating system's point of view.
Under versions of Windows before Vista and versions of Linux before 2.6, all
driver execution was co-operative, meaning that if a driver entered an infinite
loop it would freeze the system. More recent revisions of these operating
systems incorporate kernel preemption, where the kernel interrupts the driver
to give it tasks, and then separates itself from the process until it receives
a response from the device driver, or gives it more tasks to do.
**** Networking ****
Main article: Computer_network
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (December 2018)(Learn_how_and_when_to_remove_this_template_message)
Currently most operating systems support a variety of networking protocols,
hardware, and applications for using them. This means that computers running
dissimilar operating systems can participate in a common network for sharing
resources such as computing, files, printers, and scanners using either wired
or wireless connections. Networks can essentially allow a computer's operating
system to access the resources of a remote computer to support the same
functions as it could if those resources were connected directly to the local
computer. This includes everything from simple communication, to using
networked file systems or even sharing another computer's graphics or sound
hardware. Some network services allow the resources of a computer to be
accessed transparently, such as SSH which allows networked users direct access
to a computer's command line interface.
Client/server networking allows a program on a computer, called a client, to
connect via a network to another computer, called a server. Servers offer (or
host) various services to other network computers and users. These services are
usually provided through ports or numbered access points beyond the server's IP
address. Each port number is usually associated with a maximum of one running
program, which is responsible for handling requests to that port. A daemon,
being a user program, can in turn access the local hardware resources of that
computer by passing requests to the operating system kernel.
Many operating systems support one or more vendor-specific or open networking
protocols as well, for example, SNA on IBM systems, DECnet on systems from
Digital_Equipment_Corporation, and Microsoft-specific protocols (SMB) on
Windows. Specific protocols for specific tasks may also be supported such as
NFS for file access. Protocols like ESound, or esd can be easily extended over
the network to provide sound from local applications, on a remote system's
sound hardware.
**** Security ****
Main article: Computer_security
A computer being secure depends on a number of technologies working properly. A
modern operating system provides access to a number of resources, which are
available to software running on the system, and to external devices like
networks via the kernel.[citation_needed]
The operating system must be capable of distinguishing between requests which
should be allowed to be processed, and others which should not be processed.
While some systems may simply distinguish between "privileged" and "non-
privileged", systems commonly have a form of requester identity, such as a user
name. To establish identity there may be a process of authentication. Often a
username must be quoted, and each username may have a password. Other methods
of authentication, such as magnetic cards or biometric data, might be used
instead. In some cases, especially connections from the network, resources may
be accessed with no authentication at all (such as reading files over a network
share). Also covered by the concept of requester identity is authorization; the
particular services and resources accessible by the requester once logged into
a system are tied to either the requester's user account or to the variously
configured groups of users to which the requester belongs.[citation_needed]
In addition to the allow or disallow model of security, a system with a high
level of security also offers auditing options. These would allow tracking of
requests for access to resources (such as, "who has been reading this file?").
Internal security, or security from an already running program is only possible
if all possibly harmful requests must be carried out through interrupts to the
operating system kernel. If programs can directly access hardware and
resources, they cannot be secured.[citation_needed]
External security involves a request from outside the computer, such as a login
at a connected console or some kind of network connection. External requests
are often passed through device drivers to the operating system's kernel, where
they can be passed onto applications, or carried out directly. Security of
operating systems has long been a concern because of highly sensitive data held
on computers, both of a commercial and military nature. The United States
Government Department_of_Defense (DoD) created the Trusted_Computer_System
Evaluation_Criteria (TCSEC) which is a standard that sets basic requirements
for assessing the effectiveness of security. This became of vital importance to
operating system makers, because the TCSEC was used to evaluate, classify and
select trusted_operating_systems being considered for the processing, storage
and retrieval of sensitive or classified_information.
Network services include offerings such as file sharing, print services, email,
web sites, and file_transfer_protocols (FTP), most of which can have
compromised security. At the front line of security are hardware devices known
as firewalls or intrusion detection/prevention systems. At the operating system
level, there are a number of software firewalls available, as well as intrusion
detection/prevention systems. Most modern operating systems include a software
firewall, which is enabled by default. A software firewall can be configured to
allow or deny network traffic to or from a service or application running on
the operating system. Therefore, one can install and be running an insecure
service, such as Telnet or FTP, and not have to be threatened by a security
breach because the firewall would deny all traffic trying to connect to the
service on that port.
An alternative strategy, and the only sandbox strategy available in systems
that do not meet the Popek_and_Goldberg_virtualization_requirements, is where
the operating system is not running user programs as native code, but instead
either emulates a processor or provides a host for a p-code based system such
as Java.
Internal security is especially relevant for multi-user systems; it allows each
user of the system to have private files that the other users cannot tamper
with or read. Internal security is also vital if auditing is to be of any use,
since a program can potentially bypass the operating system, inclusive of
bypassing auditing.
**** User interface ****
Main article: Operating_system_user_interface
A screenshot of the Bash command line. Each command is typed out after the
'prompt', and then its output appears below, working its way down the screen.
The current command prompt is at the bottom.
Every computer that is to be operated by an individual requires a user
interface. The user interface is usually referred to as a shell and is
essential if human interaction is to be supported. The user interface views the
directory_structure and requests services from the operating system that will
acquire data from input_hardware_devices, such as a keyboard, mouse or credit
card_reader, and requests operating system services to display prompts, status
messages and such on output_hardware_devices, such as a video_monitor or
printer. The two most common forms of a user interface have historically been
the command-line_interface, where computer commands are typed out line-by-line,
and the graphical_user_interface, where a visual environment (most commonly a
WIMP) is present.
*** Graphical user interfaces ***
A screenshot of the KDE_Plasma_5 graphical user interface. Programs take the
form of images on the screen, and the files, folders (directories), and
applications take the form of icons and symbols. A mouse is used to navigate
the computer.
Most of the modern computer systems support graphical_user_interfaces (GUI),
and often include them. In some computer systems, such as the original
implementation of the classic_Mac_OS, the GUI is integrated into the kernel.
While technically a graphical user interface is not an operating system
service, incorporating support for one into the operating system kernel can
allow the GUI to be more responsive by reducing the number of context_switches
required for the GUI to perform its output functions. Other operating systems
are modular, separating the graphics subsystem from the kernel and the
Operating System. In the 1980s UNIX, VMS and many others had operating systems
that were built this way. Linux and macOS are also built this way. Modern
releases of Microsoft Windows such as Windows_Vista implement a graphics
subsystem that is mostly in user-space; however the graphics drawing routines
of versions between Windows_NT_4.0 and Windows_Server_2003 exist mostly in
kernel space. Windows_9x had very little distinction between the interface and
the kernel.
Many computer operating systems allow the user to install or create any user
interface they desire. The X Window_System in conjunction with GNOME or KDE
Plasma_5 is a commonly found setup on most Unix and Unix-like (BSD, Linux,
Solaris) systems. A number of Windows_shell_replacements have been released for
Microsoft Windows, which offer alternatives to the included Windows_shell, but
the shell itself cannot be separated from Windows.
Numerous Unix-based GUIs have existed over time, most derived from X11.
Competition among the various vendors of Unix (HP, IBM, Sun) led to much
fragmentation, though an effort to standardize in the 1990s to COSE and CDE
failed for various reasons, and were eventually eclipsed by the widespread
adoption of GNOME and K_Desktop_Environment. Prior to free_software-based
toolkits and desktop environments, Motif was the prevalent toolkit/desktop
combination (and was the basis upon which CDE was developed).
Graphical user interfaces evolve over time. For example, Windows has modified
its user interface almost every time a new major version of Windows is
released, and the Mac OS GUI changed dramatically with the introduction of
Mac OS X in 1999.[32]
***** Real-time operating systems *****
Main article: Real-time_operating_system
A real-time operating system (RTOS) is an operating system intended for
applications with fixed deadlines (real-time_computing). Such applications
include some small embedded_systems, automobile engine controllers, industrial
robots, spacecraft, industrial control, and some large-scale computing systems.
An early example of a large-scale real-time operating system was Transaction
Processing_Facility developed by American_Airlines and IBM for the Sabre
Airline_Reservations_System.
Embedded systems that have fixed deadlines use a real-time_operating_system
such as VxWorks, PikeOS, eCos, QNX, MontaVista_Linux and RTLinux. Windows_CE is
a real-time_operating_system that shares similar APIs to desktop Windows but
shares none of desktop Windows' codebase.[33] Symbian_OS also has an RTOS
kernel (EKA2) starting with version 8.0b.
Some embedded systems use operating systems such as Palm_OS, BSD, and Linux,
although such operating systems do not support real-time computing.
***** Operating system development as a hobby *****
See also: Hobbyist_operating_system_development
Operating system development is one of the most complicated activities in which
a computing hobbyist may engage.[citation_needed] A hobby operating system may
be classified as one whose code has not been directly derived from an existing
operating system, and has few users and active_developers.[34]
In some cases, hobby development is in support of a "homebrew" computing
device, for example, a simple single-board_computer powered by a 6502
microprocessor. Or, development may be for an architecture already in
widespread use. Operating system development may come from entirely new
concepts, or may commence by modeling an existing operating system. In either
case, the hobbyist is his/her own developer, or may interact with a small and
sometimes unstructured group of individuals who have like interests.
Examples of a hobby operating system include Syllable and TempleOS.
***** Diversity of operating systems and portability *****
Application software is generally written for use on a specific operating
system, and sometimes even for specific hardware.[citation_needed] When porting
the application to run on another OS, the functionality required by that
application may be implemented differently by that OS (the names of functions,
meaning of arguments, etc.) requiring the application to be adapted, changed,
or otherwise maintained.
Unix was the first operating system not written in assembly language, making it
very portable to systems different from its native PDP-11.[35]
This cost in supporting operating systems diversity can be avoided by instead
writing applications against software_platforms such as Java or Qt. These
abstractions have already borne the cost of adaptation to specific operating
systems and their system_libraries.
Another approach is for operating system vendors to adopt standards. For
example, POSIX and OS_abstraction_layers provide commonalities that reduce
porting costs.
***** Market share *****
Further information: Usage_share_of_operating_systems
***** See also *****
    * [icon]Computer_Science_portal
    * Comparison_of_operating_systems
    * Crash_(computing)
    * Hypervisor
    * Interruptible_operating_system
    * List_of_important_publications_in_operating_systems
    * List_of_operating_systems
    * List_of_pioneers_in_computer_science
    * Live_CD
    * Glossary_of_operating_systems_terms
    * Microcontroller
    * Mobile_device
    * Mobile_operating_system
    * Network_operating_system
    * Object-oriented_operating_system
    * Operating_System_Projects
    * System_Commander
    * System_image
    * Timeline_of_operating_systems
***** References *****
   1. ^Stallings (2005). Operating Systems, Internals and Design Principles.
      Pearson: Prentice Hall. p. 6.
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
   3. ^Dhotre, I.A. (2009). Operating Systems. Technical Publications. p. 1.
   4. ^"Desktop_Operating_System_Market_Share_Worldwide_|_StatCounter_Global
      Stats". StatCounter Global Stats. Retrieved 18 December 2017.
   5. ^"Mobile_&_Tablet_Operating_System_Market_Share_Worldwide_|_StatCounter
      Global_Stats". StatCounter Global Stats. Retrieved 18 December 2017.
   6. ^"Strategy_Analytics:_Android_Captures_Record_88_Percent_Share_of_Global
      Smartphone_Shipments_in_Q3_2016". 2 November 2016. Archived from the
      original on 5 November 2016.
   7. ^ Lorch, Jacob R., and Alan Jay Smith. "Reducing processor power
      consumption by improving processor time management in a single-user
      operating system." Proceedings of the 2nd annual international conference
      on Mobile computing and networking. ACM, 1996.
   8. ^Mishra, B.; Singh, N.; Singh, R. (2014). "Master-slave group based model
      for co-ordinator selection, an improvement of bully algorithm".
      International Conference on Parallel, Distributed and Grid Computing
      (PDGC). pp. 457â460. doi:10.1109/PDGC.2014.7030789. ISBN 978-1-4799-
      7682-9.
   9. ^Gagne, Silberschatz Galvin (2012). Operating Systems Concepts. New York:
      Wiley. p. 716. ISBN 978-1118063330.
  10. ^ a bHansen, Per Brinch, ed. (2001). Classic_Operating_Systems. Springer.
      pp. 4â7. ISBN 0-387-95113-X.
  11. ^Lavington, Simon (1998). A History of Manchester Computers (2nd ed.).
      Swindon: The British Computer Society. pp. 50â52. ISBN 978-1-902505-01-
      5.
  12. ^Brinch Hansen, Per (2000). Classic Operating Systems: From Batch
      Processing to Distributed Systems. Springer-Verlag.
  13. ^"IntelÂ®_Microprocessor_Quick_Reference_Guide_-_Year". www.intel.com.
      Archived from the original on 25 April 2016. Retrieved 24 April 2016.
  14. ^Ritchie, Dennis. "Unix_Manual,_first_edition". Lucent Technologies.
      Archived from the_original on 18 May 2008. Retrieved 22 November 2012.
  15. ^"OS_X_Mountain_Lion_â_Move_your_Mac_even_further_ahead". Apple.
      Archived from the original on 23 May 2011. Retrieved 7 August 2012.
  16. ^ a b"Top_5_Operating_Systems_from_January_to_April_2011". StatCounter.
      October 2009. Archived from the original on 26 May 2012. Retrieved 5
      November 2009.
  17. ^"IDC_report_into_Server_market_share". Idc.com. Archived from the
      original on 27 September 2012. Retrieved 7 August 2012.
  18. ^LinuxDevices Staff (23 April 2008). "Linux_still_top_embedded_OS".
      LinuxGizmos.com. Archived from the_original on 19 April 2016. Retrieved 5
      April 2016.
  19. ^"Sublist_Generator". Top500.org. Retrieved 6 February 2017.
  20. ^"Global_Web_Stats". Net Market Share, Net Applications. May 2011.
      Archived from the original on 25 January 2010. Retrieved 7 May 2011.
  21. ^"Global_Web_Stats". W3Counter, Awio Web Services. September 2009.
      Archived from the original on 28 June 2012. Retrieved 24 October 2009.
  22. ^"Operating_System_Market_Share". Net Applications. October 2009.
      Archived from the original on 25 January 2010. Retrieved 5 November 2009.
  23. ^"w3schools.com_OS_Platform_Statistics". Archived from the original on 5
      August 2011. Retrieved 30 October 2011.
  24. ^"Stats_Count_Global_Stats_Top_Five_Operating_Systems". Archived from the
      original on 26 May 2012. Retrieved 30 October 2011.
  25. ^"Global_statistics_at_w3counter.com". Archived from the original on 28
      June 2012. Retrieved 23 January 2012.
  26. ^"Troubleshooting_MS-DOS_Compatibility_Mode_on_Hard_Disks".
      Support.microsoft.com. Archived from the original on 10 August 2012.
      Retrieved 7 August 2012.
  27. ^"Using_NDIS_2_PCMCIA_Network_Card_Drivers_in_Windows_95".
      Support.microsoft.com. Archived from the original on 17 February 2013.
      Retrieved 7 August 2012.
  28. ^"INFO:_Windows_95_Multimedia_Wave_Device_Drivers_Must_be_16_bit".
      Support.microsoft.com. Archived from the original on 17 February 2013.
      Retrieved 7 August 2012.
  29. ^Arthur, Charles. "Windows_8_will_run_on_ARM_chips_-_but_third-party_apps
      will_need_rewrite". The Guardian. Archived from the original on 12
      October 2016.
  30. ^"Operating_System_Share_by_Groups_for_Sites_in_All_Locations_January
      2009". Archived from the original on 6 July 2009.
  31. ^"Behind_the_IDC_data:_Windows_still_No._1_in_server_operating_systems".
      ZDNet. 26 February 2010. Archived from the original on 1 March 2010.
  32. ^Stallings, William (2008). Computer Organization & Architecture. New
      Delhi: Prentice-Hall of India Private Limited. p. 267. ISBN 978-81-203-
      2962-1.
  33. ^ Poisson, Ken. "Chronology_of_Personal_Computer_Software" Archived 14
      May 2008 at the Wayback_Machine. Retrieved on 2008-05-07. Last checked on
      2009-03-30.
  34. ^"Reading:_Operating_System". Lumen. Retrieved 5 January 2019.
  35. ^"My_OS_is_less_hobby_than_yours". Osnews. 21 December 2009. Archived
      from the original on 24 December 2009. Retrieved 21 December 2009.
  36. ^"The_History_of_Unix". BYTE. August 1983. p. 188. Retrieved 31 January
      2015.
***** Further reading *****
    * Auslander, Marc A.; Larkin, David C.; Scherr, Allan L. (1981). "The
      evolution_of_the_MVS_Operating_System" (PDF). IBM J. Research &
      Development.
Deitel, Harvey M.; Deitel, Paul; Choffnes, David. Operating Systems. Pearson/
Prentice Hall. ISBN 978-0-13-092641-8.
Bic, Lubomur F.; Shaw, Alan C. (2003). Operating Systems. Pearson: Prentice
Hall.
Silberschatz, Avi; Galvin, Peter; Gagne, Greg (2008). Operating Systems
Concepts. John_Wiley_&_Sons. ISBN 0-470-12872-0.
O'Brien, J. A., & Marakas, G. M.(2011). Management Information Systems. 10e.
McGraw-Hill Irwin.
Leva, Alberto; Maggio, Martina; Papadopoulos, Alessandro Vittorio; Terraneo,
Federico (2013). Control-based Operating System Design. IET. ISBN 978-1-84919-
609-3.
Arpaci-Dusseau, Remzi; Arpaci-Dusseau, Andrea (2015). Operating_Systems:_Three
Easy_Pieces.
***** External links *****
 Look up operating_system in Wiktionary, the free dictionary.
 Wikimedia Commons has media related to Screenshots_of_operating_systems.
 Wikiversity has learning resources about Operating_Systems
    * Operating_Systems at Curlie
    * Multics_History and the history of operating systems
    * v
    * t
    * e
Operating systems
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
Systems_science
                       * Anatomical
                       * Art
                       * Biological
                       * Complex
                       * Complex_adaptive
                       * Conceptual
                       * Coupled_humanâenvironment
                       * Database
                       * Dynamical
                       * Ecological
                       * Economic
                       * Energy
                       * Formal
                       * Holarchic
Systems types          * Information
                       * Legal
                       * Measurement
                       * Metric
                       * Multi-agent
                       * Nervous
                       * Nonlinear
                       * Operating
                       * Physical
                       * Planetary
                       * Political
                       * Sensory
                       * Social
                       * Star
                       * Writing
                       * Doubling_time
                       * Leverage_points
Concepts               * Limiting_factor
                       * Negative_feedback
                       * Positive_feedback
                       * Chaos_theory
                       * Complex_systems
                       * Control_theory
                       * Cybernetics
                       * Earth_system_science
                       * Living_systems
                       * Sociotechnical_system
                       * Systemics
                       * Urban_metabolism
Theoretical fields     * World-systems_theory
                       * Analysis
                       * Biology
                       * Dynamics
                       * Ecology
                       * Engineering
                       * Neuroscience
                       * Pharmacology
                       * Psychology
                       * Theory
                       * Thinking
                       * Alexander_Bogdanov
                       * Russell_L._Ackoff
                       * William_Ross_Ashby
                       * Ruzena_Bajcsy
                       * BÃ©la_H._BÃ¡nÃ¡thy
                       * Gregory_Bateson
                       * Anthony_Stafford_Beer
                       * Richard_E._Bellman
                       * Ludwig_von_Bertalanffy
                       * Margaret_Boden
                       * Kenneth_E._Boulding
                       * Murray_Bowen
                       * Kathleen_Carley
                       * Mary_Cartwright
                       * C._West_Churchman
                       * Manfred_Clynes
                       * George_Dantzig
                       * Edsger_W._Dijkstra
                       * Fred_Emery
                       * Heinz_von_Foerster
                       * Stephanie_Forrest
                       * Jay_Wright_Forrester
                       * Barbara_Grosz
                       * Charles_A. S._Hall
                       * Lydia_Kavraki
Systems_scientists     * James_J._Kay
                       * Faina_M._Kirillova
                       * George_Klir
                       * Allenna_Leonard
                       * Edward_Norton_Lorenz
                       * Niklas_Luhmann
                       * Humberto_Maturana
                       * Margaret_Mead
                       * Donella_Meadows
                       * Mihajlo_D._Mesarovic
                       * James_Grier_Miller
                       * Radhika_Nagpal
                       * Howard_T._Odum
                       * Talcott_Parsons
                       * Ilya_Prigogine
                       * Qian_Xuesen
                       * Anatol_Rapoport
                       * Peter_Senge
                       * Claude_Shannon
                       * Katia_Sycara
                       * Eric_Trist
                       * Francisco_Varela
                       * Manuela_M._Veloso
                       * Kevin_Warwick
                       * Norbert_Wiener
                       * Jennifer_Wilby
                       * Anthony_Wilden
                       * Systems_theory_in_anthropology
Applications           * Systems_theory_in_archaeology
                       * Systems_theory_in_political_science
Organizations          * List
                       * Principia_Cybernetica
    * [Category] Category
    * [Portal] Portal
    * [Commons page] Commons
    * v
    * t
    * e
Computer_science
Note: This template roughly follows the 2012 ACM_Computing_Classification
System.
                          * Printed_circuit_board
                          * Peripheral
                          * Integrated_circuit
Hardware                  * Very_Large_Scale_Integration
                          * Systems_on_Chip_(SoCs)
                          * Energy_consumption_(Green_computing)
                          * Electronic_design_automation
                          * Hardware_acceleration
                          * Computer_architecture
Computer systems          * Embedded_system
organization              * Real-time_computing
                          * Dependability
                          * Network_architecture
                          * Network_protocol
Networks                  * Network_components
                          * Network_scheduler
                          * Network_performance_evaluation
                          * Network_service
                          * Interpreter
                          * Middleware
Software organization     * Virtual_machine
                          * Operating system
                          * Software_quality
                          * Programming_paradigm
                          * Programming_language
                          * Compiler
                          * Domain-specific_language
Software_notations        * Modeling_language
and tools                 * Software_framework
                          * Integrated_development_environment
                          * Software_configuration_management
                          * Software_library
                          * Software_repository
                          * Software_development_process
                          * Requirements_analysis
                          * Software_design
Software_development      * Software_construction
                          * Software_deployment
                          * Software_maintenance
                          * Programming_team
                          * Open-source_model
                          * Model_of_computation
                          * Formal_language
Theory_of_computation     * Automata_theory
                          * Computational_complexity_theory
                          * Logic
                          * Semantics
                          * Algorithm_design
                          * Analysis_of_algorithms
Algorithms                * Algorithmic_efficiency
                          * Randomized_algorithm
                          * Computational_geometry
                          * Discrete_mathematics
                          * Probability
Mathematics               * Statistics
of computing              * Mathematical_software
                          * Information_theory
                          * Mathematical_analysis
                          * Numerical_analysis
                          * Database_management_system
                          * Information_storage_systems
                          * Enterprise_information_system
                          * Social_information_systems
                          * Geographic_information_system
                          * Decision_support_system
Information               * Process_control_system
systems                   * Multimedia_information_system
                          * Data_mining
                          * Digital_library
                          * Computing_platform
                          * Digital_marketing
                          * World_Wide_Web
                          * Information_retrieval
                          * Cryptography
                          * Formal_methods
                          * Security_services
Security                  * Intrusion_detection_system
                          * Hardware_security
                          * Network_security
                          * Information_security
                          * Application_security
                          * Interaction_design
Humanâcomputer       * Social_computing
interaction               * Ubiquitous_computing
                          * Visualization
                          * Accessibility
                          * Concurrent_computing
                          * Parallel_computing
Concurrency               * Distributed_computing
                          * Multithreading
                          * Multiprocessing
                          * Natural_language_processing
                          * Knowledge_representation_and_reasoning
                          * Computer_vision
Artificial                * Automated_planning_and_scheduling
intelligence              * Search_methodology
                          * Control_method
                          * Philosophy_of_artificial_intelligence
                          * Distributed_artificial_intelligence
                          * Supervised_learning
                          * Unsupervised_learning
Machine_learning          * Reinforcement_learning
                          * Multi-task_learning
                          * Cross-validation
                          * Animation
                          * Rendering
                          * Image_manipulation
Graphics                  * Graphics_processing_unit
                          * Mixed_reality
                          * Virtual_reality
                          * Image_compression
                          * Solid_modeling
                          * E-commerce
                          * Enterprise_software
                          * Computational_mathematics
                          * Computational_physics
                          * Computational_chemistry
                          * Computational_biology
                          * Computational_social_science
                          * Computational_engineering
Applied                   * Computational_healthcare
computing                 * Digital_art
                          * Electronic_publishing
                          * Cyberwarfare
                          * Electronic_voting
                          * Video_games
                          * Word_processing
                          * Operations_research
                          * Educational_technology
                          * Document_management
    * [Wikipedia book] Book
    * [Category] Category
    * [Portal] Portal
    * [Outline] Outline
    * [WikiProject]WikiProject
    * [Commons page] Commons
                                              * BNF: cb119333481 (data)
                                              * GND: 4006216-8
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85094982
                                              * NDL: 00865121
                                              * NKC: ph115593

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Operating_system&oldid=909771321"
Categories:
    * Operating_systems
Hidden categories:
    * Webarchive_template_wayback_links
    * Wikipedia_pages_semi-protected_against_vandalism
    * Wikipedia_indefinitely_move-protected_pages
    * Use_dmy_dates_from_July_2015
    * Articles_with_incomplete_citations_from_August_2014
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2010
    * Articles_with_unsourced_statements_from_June_2010
    * Articles_with_unsourced_statements_from_February_2015
    * Articles_needing_additional_references_from_December_2018
    * All_articles_needing_additional_references
    * Articles_with_unsourced_statements_from_December_2018
    * Articles_with_unsourced_statements_from_April_2015
    * Commons_category_link_is_locally_defined
    * Articles_with_Curlie_links
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
    * Wikipedia_articles_with_NKC_identifiers
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
    * View_source
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
    * Wikibooks
    * Wikinews
    * Wikiversity
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * AcÃ¨h
    * Afrikaans
    * Alemannisch
    * á áá­á
    * Ãnglisc
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AragonÃ©s
    * à¦à¦¸à¦®à§à¦¯à¦¼à¦¾
    * Asturianu
    * AzÉrbaycanca
    * ØªÛØ±Ú©Ø¬Ù
    * à¦¬à¦¾à¦à¦²à¦¾
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐ°ÑÒ¡Ð¾ÑÑÑÐ°
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * Brezhoneg
    * ÐÑÑÑÐ°Ð´
    * CatalÃ 
    * Ð§ÓÐ²Ð°ÑÐ»Ð°
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * DavvisÃ¡megiella
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Furlan
    * Gaeilge
    * Galego
    * å®¢å®¶èª/Hak-kÃ¢-ngÃ®
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hornjoserbsce
    * Hrvatski
    * Ido
    * Ilokano
    * Bahasa_Indonesia
    * Interlingua
    * Interlingue
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Jawa
    * à²à²¨à³à²¨à²¡
    * á¥áá áá£áá
    * KaszÃ«bsczi
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * KurdÃ®
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * àº¥àº²àº§
    * Latina
    * LatvieÅ¡u
    * LÃ«tzebuergesch
    * LietuviÅ³
    * Ligure
    * LingÃ¡la
    * Lingua_Franca_Nova
    * Lumbaart
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Malagasy
    * à´®à´²à´¯à´¾à´³à´
    * à¤®à¤°à¤¾à¤ à¥
    * ááá áááá£á á
    * ÙØµØ±Ù
    * Bahasa_Melayu
    * MÃ¬ng-dÄÌ¤ng-ngá¹³Ì
    * MirandÃ©s
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * áá¼ááºáá¬áá¬áá¬
    * Nederlands
    * à¤¨à¥à¤ªà¤¾à¤²_à¤­à¤¾à¤·à¤¾
    * æ¥æ¬èª
    * ÐÐ¾ÑÑÐ¸Ð¹Ð½
    * Norsk
    * Norsk_nynorsk
    * Occitan
    * ÐÐ»ÑÐº_Ð¼Ð°ÑÐ¸Ð¹
    * à¬à¬¡à¬¼à¬¿à¬
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * à¨ªà©°à¨à¨¾à¨¬à©
    * PÃ¤lzisch
    * Ù¾ÙØ¬Ø§Ø¨Û
    * PlattdÃ¼Ã¼tsch
    * Polski
    * PortuguÃªs
    * Qaraqalpaqsha
    * Ripoarisch
    * RomÃ¢nÄ
    * Runa_Simi
    * Ð ÑÑÐ¸Ð½ÑÑÐºÑÐ¹
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡Ð°ÑÐ°_ÑÑÐ»Ð°
    * Sardu
    * Scots
    * Shqip
    * à·à·à¶à·à¶½
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * ÅlÅ¯nski
    * Soomaaliga
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Basa_Sunda
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * Taqbaylit
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * à°¤à±à°²à±à°à±
    * à¹à¸à¸¢
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * VÃ¨neto
    * Tiáº¿ng_Viá»t
    * VÃµro
    * Walon
    * Winaray
    * Wolof
    * å´è¯­
    * ××Ö´×××©
    * YorÃ¹bÃ¡
    * ç²µèª
    * Zazaki
    * Å½emaitÄÅ¡ka
    * ä¸­æ
Edit_links
    * This page was last edited on 7 August 2019, at 14:15 (UTC).
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
