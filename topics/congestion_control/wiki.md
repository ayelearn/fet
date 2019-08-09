The following text has been accessed from https://en.wikipedia.org/wiki/Network_congestion#Congestion_control at Fri Aug 9 01:10:27 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Network congestion ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Network congestion in data_networking and queueing_theory is the reduced
quality_of_service that occurs when a network node or link is carrying more
data than it can handle. Typical effects include queueing_delay, packet_loss or
the blocking of new connections. A consequence of congestion is that an
incremental increase in offered_load leads either only to a small increase or
even a decrease in network throughput.[1]
Network_protocols that use aggressive retransmissions to compensate for packet
loss due to congestion can increase congestion, even after the initial load has
been reduced to a level that would not normally have induced network
congestion. Such networks exhibit two stable states under the same level of
load. The stable state with low throughput is known as congestive collapse.
Networks use congestion control and congestion avoidance techniques to try to
avoid collapse. These include: exponential_backoff in protocols such as CSMA/CA
in 802.11 and the similar CSMA/CD in the original Ethernet, window reduction in
TCP, and fair_queueing in devices such as routers and network_switches. Other
techniques that address congestion include priority schemes which transmit some
packets with higher priority ahead of others and the explicit allocation of
network resources to specific flows through the use of admission_control.
⁰
***** Contents *****
    * 1_Network_capacity
    * 2_Congestive_collapse
    * 3_Congestion_control
          o 3.1_Theory_of_congestion_control
          o 3.2_Classification_of_congestion_control_algorithms
    * 4_Mitigation
          o 4.1_Practical_network_congestion_avoidance
          o 4.2_TCP/IP_congestion_avoidance
          o 4.3_Active_queue_management
                # 4.3.1_Random_early_detection
                # 4.3.2_Robust_random_early_detection_(RRED)
                # 4.3.3_Flowbased-RED/WRED
                # 4.3.4_Explicit_Congestion_Notification
                # 4.3.5_Cisco_AQM:_Dynamic_buffer_limiting
                # 4.3.6_TCP_window_shaping
                # 4.3.7_Backward_ECN
    * 5_Side_effects_of_congestive_collapse_avoidance
          o 5.1_Radio_links
          o 5.2_Short-lived_connections
    * 6_Admission_control
    * 7_See_also
    * 8_References
    * 9_Books
    * 10_External_links
***** Network capacity[edit] *****
Network resources are limited, including router processing time and link
throughput. Resource_contention may occur on networks in a number of common
circumstances. A wireless_LAN is easily filled by a single personal computer.
Even on fast computer networks, the backbone can easily be congested by a few
servers and client PCs. Denial-of-service_attacks by botnets are capable of
filling even the largest Internet_backbone network links, generating large-
scale network congestion. In telephone networks, a mass_call_event can
overwhelm digital telephone circuits.
***** Congestive collapse[edit] *****
Congestive collapse (or congestion collapse) is the condition in which
congestion prevents or limits useful communication. Congestion collapse
generally occurs at choke points in the network, where incoming traffic exceeds
outgoing bandwidth. Connection points between a local_area_network and a wide
area_network are common choke points. When a network is in this condition, it
settles into a stable state where traffic demand is high but little useful
throughput is available, packet_delay and loss occur and quality_of_service is
extremely poor.
Congestive collapse was identified as a possible problem by 1984.[2] It was
first observed on the early Internet in October 1986, when the NSFnet phase-
I backbone dropped three orders of magnitude from its capacity of 32 kbit/s to
40 bit/s, which continued until end nodes started implementing Van_Jacobson's
congestion_control between 1987 and 1988.[3] When more packets were sent than
could be handled by intermediate routers, the intermediate routers discarded
many packets, expecting the end points of the network to retransmit the
information. However, early TCP implementations had poor retransmission
behavior. When this packet loss occurred, the endpoints sent extra packets that
repeated the information lost, doubling the incoming rate.
***** Congestion control[edit] *****
Congestion control modulates traffic entry into a telecommunications network in
order to avoid congestive collapse resulting from oversubscription. This is
typically accomplished by reducing the rate of packets. Whereas congestion
control prevents senders from overwhelming the network, flow_control prevents
the sender from overwhelming the receiver.
**** Theory of congestion control[edit] ****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (May 2013)(Learn_how_and_when_to_remove_this_template_message)
The theory on congestion control was pioneered by Frank_Kelly, who applied
microeconomic_theory and convex_optimization theory to describe how individuals
controlling their own rates can interact to achieve an optimal network-wide
rate allocation. Examples of optimal rate allocation are max-min_fair
allocation and Kelly's suggestion of proportionally_fair allocation, although
many others are possible.
Let      x  i     {\displaystyle x_{i}}  [x_{i}] be the rate of flow     i
{\displaystyle i}  [i],      c  l     {\displaystyle c_{l}}  [c_{l}] be the
capacity of link     l   {\displaystyle l}  [l], and      r  l i
{\displaystyle r_{li}}  [r_{{li}}] be 1 if flow     i   {\displaystyle i}  [i]
uses link     l   {\displaystyle l}  [l] and 0 otherwise. Let     x
{\displaystyle x}  [x],     c   {\displaystyle c}  [c] and     R
{\displaystyle R}  [R] be the corresponding vectors and matrix. Let     U ( x )
{\displaystyle U(x)}  [U(x)] be an increasing, strictly concave function,
called the utility, which measures how much benefit a user obtains by
transmitting at rate     x   {\displaystyle x}  [x]. The optimal rate
allocation then satisfies
          max  x    &#x2211;  i   U (  x  i   )   {\displaystyle \max \limits _
      {x}\sum _{i}U(x_{i})}  [\max \limits _{x}\sum _{i}U(x_{i})]
      such that     R x &#x2264; c   {\displaystyle Rx\leq c}  [Rx\leq c]
The Lagrange_dual of this problem decouples, so that each flow sets its own
rate, based only on a price signalled by the network. Each link capacity
imposes a constraint, which gives rise to a Lagrange_multiplier,      p  l
{\displaystyle p_{l}}  [p_{l}]. The sum of these multipliers,      y  i   =
&#x2211;  l    p  l    r  l i   ,   {\displaystyle y_{i}=\sum _{l}p_{l}r_{li},}
[y_{i}=\sum _{l}p_{l}r_{{li}},] is the price to which the flow responds.
Congestion control then becomes a distributed optimisation algorithm. Many
current congestion control algorithms can be modelled in this framework, with
p  l     {\displaystyle p_{l}}  [p_{l}] being either the loss probability or
the queueing delay at link     l   {\displaystyle l}  [l]. A major weakness is
that it assigns the same price to all flows, while sliding window flow control
causes burstiness that causes different flows to observe different loss or
delay at a given link.
**** Classification of congestion control algorithms[edit] ****
See also: TCP_congestion_control
Among the ways to classify congestion control algorithms are:
    * By type and amount of feedback received from the network: Loss; delay;
      single-bit or multi-bit explicit signals
    * By incremental deployability: Only sender needs modification; sender and
      receiver need modification; only router needs modification; sender,
      receiver and routers need modification.
    * By performance aspect: high bandwidth-delay product networks; lossy
      links; fairness; advantage to short flows; variable-rate links
    * By fairness criterion: Max-min fairness; proportionally fair; controlled
      delay
***** Mitigation[edit] *****
Mechanisms have been invented to prevent network congestion or to deal with a
network collapse:
    * Network_scheduler – active_queue_management which reorders or selectively
      drops network packets in the presence of congestion
    * Explicit_Congestion_Notification – an extension to IP and TCP
      communications protocols that adds a flow control mechanism
    * TCP_congestion_control – various implementations of efforts to deal with
      network congestion
The correct endpoint behavior is usually to repeat dropped information, but
progressively slow the repetition rate. Provided all endpoints do this, the
congestion lifts and the network resumes normal behavior.[citation_needed]
Other strategies such as slow-start ensure that new connections don't overwhelm
the router before congestion detection initiates.
Common router congestion avoidance mechanisms include fair_queuing and other
scheduling_algorithms, and random_early_detection (RED) where packets are
randomly dropped as congestion is detected. This proactively triggers the
endpoints to slow transmission before congestion collapse occurs. Fair queuing
is most useful in routers at choke points with a small number of connections
passing through them. Larger routers must rely on RED.[citation_needed]
Some end-to-end protocols are designed behave well under congested conditions;
TCP is a well known example. The first TCP implementations to handle congestion
were described in 1984,[4] but Van_Jacobson's inclusion of an open source
solution in the Berkeley Standard Distribution UNIX ("BSD") in 1988 first
provided good behavior.
UDP does not control congestion. Protocols built atop UDP must handle
congestion independently. Protocols that transmit at a fixed rate, independent
of congestion, can be problematic. Real-time streaming protocols, including
many Voice_over_IP protocols, have this property. Thus, special measures, such
as quality_of_service, must be taken to keep packets from being dropped in the
presence of congestion.
In general, congestion in pure datagram networks must be kept at the periphery
of the network, where the above mechanisms can handle it. Congestion in the
Internet_backbone is problematic. Cheap fiber-optic lines have reduced costs in
the Internet backbone allowing it to be provisioned with enough bandwidth to
keep congestion at the periphery.[citation_needed]
**** Practical network congestion avoidance[edit] ****
Connection-oriented protocols, such as the widely used TCP protocol, generally
watch for packet errors, losses, or delays (see Quality_of_Service) to adjust
the transmit speed. Various network congestion avoidance processes, support
different trade-offs.[5]
**** TCP/IP congestion avoidance[edit] ****
The TCP_congestion_avoidance_algorithm is the primary basis for congestion
control in the Internet.[6][7][8][9][10]
Problems occur when concurrent TCP flows experience port_queue_buffer tail-
drops, defeating TCP's automatic congestion avoidance. All flows that
experience port queue buffer tail-drop begin a TCP retrain at the same moment
â this is called TCP_global_synchronization.
**** Active queue management[edit] ****
Active_queue_management (AQM) is the reorder or drop of network packets inside
a transmit buffer that is associated with a network_interface_controller (NIC).
This task is performed by the network_scheduler.
*** Random early detection[edit] ***
One solution is to use random_early_detection (RED) on the network equipment's
port_queue_buffer.[11][12] On network_equipment ports with more than one queue
buffer, weighted_random_early_detection (WRED) could be used if available.
RED indirectly signals to sender and receiver by deleting some packets, e.g.
when the average queue buffer lengths are more than a threshold (e.g. 50%) and
deletes linearly or cubically more packets,[13] up to e.g. 100%. The average
queue buffer lengths are computed over 1 second intervals.
*** Robust random early detection (RRED)[edit] ***
The robust_random_early_detection (RRED) algorithm was proposed to improve the
TCP throughput against denial-of-service (DoS) attacks, particularly low-rate
denial-of-service (LDoS) attacks. Experiments confirmed that RED-like
algorithms were vulnerable under Low-rate Denial-of-Service (LDoS) attacks due
to the oscillating TCP queue size caused by the attacks.[14]
*** Flowbased-RED/WRED[edit] ***
Some network equipment is equipped with ports that can follow and measure each
flow (flowbased-RED/WRED) and are thereby able to signal a too big bandwidth
flow according to some quality of service policy. A policy could then divide
the bandwidth among all flows by some criteria.
*** Explicit Congestion Notification[edit] ***
Another approach is to use IP Explicit_Congestion_Notification (ECN).[15] ECN
is used only when two hosts signal that they want to use it. With this method,
a protocol bit is used to signal explicit congestion. This is better than the
indirect packet delete congestion notification performed by the RED/WRED
algorithms, but it requires explicit support by both hosts.[16] ECN coauthor
Sally_Floyd published detailed information on ECN, including the version
required for Cisco_IOS.[11]
When a router receives a packet marked as ECN-capable and anticipates (using
RED) congestion, it sets the ECN flag, notifying the sender of congestion. The
sender should respond by decreasing its transmission bandwidth, e.g., by
decreasing the TCP window size (sending rate) or by other means.
*** Cisco AQM: Dynamic buffer limiting[edit] ***
Cisco_Systems (Engine IV and V) has the capability to classify flows as
aggressive (bad) or adaptive (good). It ensures that no flows fill the port
queues. DBL can utilize IP ECN instead of packet-delete-signalling.[17][18]
*** TCP window shaping[edit] ***
See also: TCP_window_scale_option
Congestion avoidance can be achieved efficiently by reducing traffic. When an
application requests a large file, graphic or web page, it usually advertises a
"window" of between 32K and 64K. This results in the server sending a full
window of data (assuming the file is larger than the window). When many
applications simultaneously request downloads, this data creates a congestion
point at an upstream provider by flooding the queue. By using a device to
reduce the window advertisement, the remote servers send less data, thus
reducing the congestion. This technique can reduce network congestion by a
factor of 40.[citation_needed]
*** Backward ECN[edit] ***
Backward ECN (BECN) is another proposed congestion mechanism. It uses ICMP
source_quench messages as an IP signalling mechanism to implement a basic ECN
mechanism for IP networks, keeping congestion notifications at the IP level and
requiring no negotiation between network endpoints. Effective congestion
notifications can be propagated to transport layer protocols, such as TCP and
UDP, for the appropriate adjustments.[19]
***** Side effects of congestive collapse avoidance[edit] *****
**** Radio links[edit] ****
The protocols that avoid congestive collapse are often based on the idea that
data loss is caused by congestion. This is true in nearly all cases; errors
during transmission are rare. However, this causes WiFi, 3G or other networks
with a radio layer to have poor throughput in some cases since wireless
networks are susceptible to data loss due to interference. The TCP connections
running over a radio based physical_layer see the data loss and tend to
erroneously believe that congestion is occurring.
**** Short-lived connections[edit] ****
The slow-start protocol performs badly for short connections. Older web
browsers created many short-lived connections and opened and closed the
connection for each file. This kept most connections in the slow start mode,
which slowed response times.
To avoid this problem, modern browsers either open multiple connections
simultaneously or reuse_one_connection for all files requested from a
particular server. Initial performance can be poor, and many connections never
get out of the slow-start regime, significantly increasing latency.
***** Admission control[edit] *****
Admission_control requires devices to receive permission before establishing
new network connections. If the new connection risks creating congestion,
permission can be denied. One example of this is the use of Contention-Free
Transmission Opportunities (CFTXOPs) in the ITU-T G.hn standard, which provides
high-speed (up to 1 Gbit/s) local_area_networking over varying wires (power
lines, phone lines and coaxial cables).
***** See also[edit] *****
    * Bandwidth_management
    * Bufferbloat
    * Cascading_failure
    * Choke_exchange
    * Erlang_(unit)
    * Max-min_fairness
    * Sorcerer's_Apprentice_Syndrome
    * TCP_congestion-avoidance_algorithm
    * Teletraffic_engineering
    * Thrashing
    * Traffic_shaping
    * Reliability_(computer_networking)
***** References[edit] *****
   1. ^ (Al-Bahadili, 2012, p. 282) Al-Bahadili, H. (2012). Simulation_in
      computer_network_design_and_modeling:_Use_and_analysis. Hershey, PA: IGI
      Global.
   2. ^
   3. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   4. RFC 896
   5. ^Fall, K.R.; Stevens, W.R. (2011). TCP/IP_Illustrated,_Volume_1:_The
      Protocols (2 ed.). Pearson Education. p. 739. ISBN 9780132808187.
   6. ^Vinton G. Cerf; Robert E. Kahn (May 1974). "A Protocol for Packet
      Network Intercommunication". IEEE Transactions on Communications. 22 (5):
      637â648. doi:10.1109/tcom.1974.1092259. Archived from the
      original|archive-url= requires |url= (help) on March 4, 2016.
   7. ^ TCP_Tunnels:_Avoiding_Congestion_Collapse_(2000)
   8. ^ Van_Jacobson, Michael_J._Karels. Congestion_Avoidance_and_Control
      (1988). Proceedings of the Sigcomm '88 Symposium, vol.18(4): pp.314–329.
      Stanford, CA. August, 1988. This paper originated many of the congestion
      avoidance algorithms used in TCP/IP.
   9. ^ RFC_2001 - TCP Slow Start, Congestion Avoidance, Fast Retransmit, and
      Fast Recovery Algorithms
  10. ^ RFC_2581 - TCP Congestion Control
  11. ^ RFC_3390 - TCP Increasing TCP's Initial Window
  12. ^ TCP_Congestion_Avoidance_Explained_via_a_Sequence_Diagram
  13. ^ a b Sally_Floyd:_RED_(Random_Early_Detection)_Queue_Management
  14. ^ Sally Floyd, Van Jacobson. Random_Early_Detection_Gateways_for
      Congestion_Avoidance (1993). IEEE/ACM Transactions on Networking, vol.1
      (4): pp.397–413. Invented Random Early Detection (RED) gateways.
  15. ^ An_Analytical_RED_Function_Design_Guaranteeing_Stable_System_Behavior
      Quote: "...The advantage of this function lies not only in avoiding heavy
      oscillations but also in avoiding link under-utilization at low loads.
      The applicability of the derived function is independent of the load
      range, no parameters are to be adjusted. Compared to the original linear
      drop function applicability is extended by far...Our example with
      realistic system parameters gives an approximation function of the cubic
      of the queue size..."
  16. ^Zhang, Changwang; Yin, Jianping; Cai, Zhiping; Chen, Weifeng (2010).
      "RRED:_Robust_RED_Algorithm_to_Counter_Low-rate_Denial-of-Service
      Attacks" (PDF). IEEE Communications Letters. IEEE. 14: 489â491.
  17. ^ RFC_3168 - The Addition of Explicit Congestion Notification (ECN) to IP
  18. ^ Comparative_study_of_RED,_ECN_and_TCP_Rate_Control_(1999)
  19. ^"Active_Queue_Management". Archived from the_original on 2008-08-21.
      Retrieved 2010-11-26.
  20. ^ Enabling_Dynamic_Buffer_Limiting
  21. ^ A_proposal_for_Backward_ECN_for_the_Internet_Protocol
    * "Deploying IP and MPLS QoS for Multiservice Networks: Theory and
      Practice" by John Evans, Clarence Filsfils (Morgan Kaufmann, 2007,
ISBN 0-12-370549-5)
RFC_2914 - Congestion Control Principles, Sally Floyd, September, 2000
RFC_896 - "Congestion Control in IP/TCP", John Nagle, 6 January 1984
Introduction to Congestion_Avoidance_and_Control, Van Jacobson and Michael J.
Karels, November, 1988
***** Books[edit] *****
    * "Deploying IP and MPLS QoS for Multiservice Networks: Theory and
      Practice" by John Evans, Clarence Filsfils (Morgan Kaufmann, 2007,
ISBN 0-12-370549-5)
***** External links[edit] *****
    * Nagle, J. RFC_896: Congestion control in IP/TCP internetworks (1984)
    * Floyd, S. RFC_2914: Congestion control principles (2000)
    * Floyd, S. and K. Fall, Promoting_the_Use_of_End-to-End_Congestion_Control
      in_the_Internet (IEEE/ACM Transactions on Networking, August 1999)
    * Sally Floyd, On_the_Evolution_of_End-to-end_Congestion_Control_in_the
      Internet:_An_Idiosyncratic_View (IMA Workshop on Scaling Phenomena in
      Communication Networks, October 1999) (pdf format)
    * Linktionary_term:_Queuing
    * Pierre-Francois_Quet,_Sriram_Chellappan,_Arjan_Durresi,_Mukundan
      Sridharan,_Hitay_Ozbay,_Raj_Jain,_"_Guidelines_for_optimizing_Multi-Level
      ECN,_using_fluid_flow_based_TCP_model"
    * Sally_Floyd,_Ratul_Mahajan,_David_Wetherall:_RED-PD:_RED_with
      Preferential_Dropping
    * A_Generic_Simple_RED_Simulator_for_educational_purposes_by_Mehmet_Suzen
    * Approaches_to_Congestion_Control_in_Packet_Networks
    * Papers_in_Congestion_Control
    * Random_Early_Detection_Homepage
    * Explicit_Congestion_Notification_Homepage
    * TFRC_Homepage
    * AIMD-FC_Homepage
    * [
      permanent_dead_link] TCP congestion control simulation: Fast recovery
    * Recent_Publications_in_low-rate_denial-of-service_(DoS)_attacks

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Network_congestion&oldid=907586520"
Categories:
    * Network_performance
    * Teletraffic
    * Transport_layer_protocols
    * Technological_failures
    * Packets_(information_technology)
Hidden categories:
    * Pages_with_archiveurl_citation_errors
    * Pages_using_RFC_magic_links
    * Articles_needing_additional_references_from_May_2013
    * All_articles_needing_additional_references
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_February_2019
    * Articles_with_unsourced_statements_from_July_2010
    * Articles_with_unsourced_statements_from_January_2011
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_September_2018
    * Articles_with_permanently_dead_external_links
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
    * Dansk
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * ä¸­æ
Edit_links
    * This page was last edited on 23 July 2019, at 22:17 (UTC).
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
