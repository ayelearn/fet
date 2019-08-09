The following text has been accessed from https://en.wikipedia.org/wiki/Routing at Fri Aug 9 03:45:45 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Routing ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about routing in packet_switching networks. For other uses, see
Routing_(disambiguation).
Routing is the process of selecting a path for traffic in a network or between
or across multiple networks. Broadly, routing is performed in many types of
networks, including circuit-switched_networks, such as the public_switched
telephone_network (PSTN), and computer_networks, such as the Internet.
In packet switching networks, routing is the higher-level decision making that
directs network_packets from their source toward their destination through
intermediate network_nodes by specific packet forwarding mechanisms. Packet
forwarding is the transit of network packets from one network_interface to
another. Intermediate nodes are typically network_hardware devices such as
routers, gateways, firewalls, or switches. General-purpose computers also
forward packets and perform routing, although they have no specially optimized
hardware for the task.
The routing process usually directs forwarding on the basis of routing_tables,
which maintain a record of the routes to various network destinations. Routing
tables may be specified by an administrator, learned by observing network
traffic or built with the assistance of routing_protocols.
Routing, in a narrower sense of the term, often refers to IP_routing and is
contrasted with bridging. IP routing assumes that network_addresses are
structured and that similar addresses imply proximity within the network.
Structured addresses allow a single routing table entry to represent the route
to a group of devices. In large networks, structured addressing (routing, in
the narrow sense) outperforms unstructured addressing (bridging). Routing has
become the dominant form of addressing on the Internet. Bridging is still
widely used within local_area_networks.
⁰
***** Contents *****
    * 1_Delivery_schemes
    * 2_Topology_distribution
          o 2.1_Distance_vector_algorithms
          o 2.2_Link-state_algorithms
          o 2.3_Optimized_Link_State_Routing_algorithm
          o 2.4_Path_vector_protocol
    * 3_Path_selection
    * 4_Multiple_agents
    * 5_Route_analytics
    * 6_Centralized_routing
    * 7_See_also
    * 8_References
    * 9_Further_reading
    * 10_External_links
***** Delivery schemes[edit] *****
Routing_schemes
Unicast
[Unicast.svg]
Broadcast
[Broadcast.svg]
Multicast
[Multicast.svg]
Anycast
[Anycast-BM.svg]
Geocast
[Geocast.svg]
    * v
    * t
    * e
Routing schemes differ in how they deliver messages:
    * unicast delivers a message to a single specific node
    * broadcast delivers a message to all nodes in the network
    * multicast delivers a message to a group of nodes that have expressed
      interest in receiving the message
    * anycast delivers a message to any one out of a group of nodes, typically
      the one nearest to the source
    * geocast delivers a message to a group of nodes based on geographic
      location
Unicast is the dominant form of message delivery on the Internet. This article
focuses on unicast routing algorithms.
***** Topology distribution[edit] *****
With static_routing, small networks may use manually configured routing tables.
Larger networks have complex topologies that can change rapidly, making the
manual construction of routing tables unfeasible. Nevertheless, most of the
public_switched_telephone_network (PSTN) uses pre-computed routing tables, with
fallback routes if the most direct route becomes blocked (see routing_in_the
PSTN).
Dynamic_routing attempts to solve this problem by constructing routing tables
automatically, based on information carried by routing_protocols, allowing the
network to act nearly autonomously in avoiding network failures and blockages.
Dynamic routing dominates the Internet. Examples of dynamic-routing protocols
and algorithms include Routing_Information_Protocol (RIP), Open_Shortest_Path
First (OSPF) and Enhanced_Interior_Gateway_Routing_Protocol (EIGRP).
**** Distance vector algorithms[edit] ****
Main article: Distance-vector_routing_protocol
Distance vector algorithms use the BellmanâFord_algorithm. This approach
assigns a cost number to each of the links between each node in the network.
Nodes send information from point A to point B via the path that results in the
lowest total cost (i.e. the sum of the costs of the links between the nodes
used).
When a node first starts, it only knows of its immediate neighbours, and the
direct cost involved in reaching them. (This information â the list of
destinations, the total cost to each, and the next hop to send data to get
there â makes up the routing table, or distance table.) Each node, on a
regular basis, sends to each neighbour node its own current assessment of the
total cost to get to all the destinations it knows of. The neighbouring nodes
examine this information and compare it to what they already know; anything
that represents an improvement on what they already have, they insert in their
own table. Over time, all the nodes in the network discover the best next hop
and total cost for all destinations.
When a network node goes down, any nodes that used it as their next hop discard
the entry and convey the updated routing information to all adjacent nodes,
which in turn repeat the process. Eventually all the nodes in the network
receive the updates, and discover new paths to all the destinations that don't
involve the down node.
**** Link-state algorithms[edit] ****
Main article: Link-state_routing_protocol
When applying link-state algorithms, a graphical_map of the network is the
fundamental data used for each node. To produce its map, each node floods the
entire network with information about the other nodes it can connect to. Each
node then independently assembles this information into a map. Using this map,
each router independently determines the least-cost path from itself to every
other node using a standard shortest_paths algorithm such as Dijkstra's
algorithm. The result is a tree_graph rooted at the current node, such that the
path through the tree from the root to any other node is the least-cost path to
that node. This tree then serves to construct the routing table, which
specifies the best next hop to get from the current node to any other node.
**** Optimized Link State Routing algorithm[edit] ****
Main article: Optimized_Link_State_Routing_Protocol
A link-state routing algorithm optimized for mobile_ad_hoc_networks is the
optimized Link State Routing Protocol (OLSR).[1] OLSR is proactive; it uses
Hello and Topology Control (TC) messages to discover and disseminate link state
information through the mobile_ad_hoc_network. Using Hello messages, each node
discovers 2-hop neighbor information and elects a set of multipoint_relays
(MPRs). MPRs distinguish OLSR from other link state routing protocols.
**** Path vector protocol[edit] ****
Main article: Path_vector_protocol
Distance vector and link state routing are both intra-domain routing protocols.
They are used inside an autonomous_system, but not between autonomous systems.
Both of these routing protocols become intractable in large networks and cannot
be used in Inter-domain routing. Distance vector routing is subject to
instability if there are more than a few hops in the domain. Link state routing
needs huge amount of resources to calculate routing tables. It also creates
heavy traffic due to flooding.
Path vector routing is used for inter-domain routing. It is similar to distance
vector routing. Path vector routing assumes that one node (there can be many)
in each autonomous system acts on behalf of the entire autonomous system. This
node is called the speaker node. The speaker node creates a routing table and
advertises it to neighboring speaker nodes in neighboring autonomous systems.
The idea is the same as distance vector routing except that only speaker nodes
in each autonomous system can communicate with each other. The speaker node
advertises the path, not the metric, of the nodes in its autonomous system or
other autonomous systems. Path vector routing is discussed in RFC_1322; the
path vector routing algorithm is somewhat similar to the distance vector
algorithm in the sense that each border router advertises the destinations it
can reach to its neighboring router. However, instead of advertising networks
in terms of a destination and the distance to that destination, networks are
advertised as destination addresses and path descriptions to reach those
destinations. A route is defined as a pairing between a destination and the
attributes of the path to that destination, thus the name, path vector routing,
where the routers receive a vector that contains paths to a set of
destinations. The path, expressed in terms of the domains (or confederations)
traversed so far, is carried in a special path attribute that records the
sequence of routing domains through which the reachability information has
passed.
***** Path selection[edit] *****
Path selection involves applying a routing_metric to multiple routes to select
(or predict) the best route. Most routing algorithms use only one network path
at a time. Multipath_routing techniques enable the use of multiple alternative
paths.
In computer networking, the metric is computed by a routing algorithm, and can
cover information such as bandwidth, network_delay, hop_count, path cost, load,
MTU (maximum transmission unit), reliability, and communication cost (see e.g.
this_survey for a list of proposed routing metrics). The routing table stores
only the best possible routes, while link-state or topological databases may
store all other information as well.
In case of overlapping or equal routes, algorithms consider the following
elements to decide which routes to install into the routing table (sorted by
priority):
   1. Prefix-Length: where longer subnet masks are preferred (independent of
      whether it is within a routing protocol or over different routing
      protocol)
   2. Metric: where a lower metric/cost is preferred (only valid within one and
      the same routing protocol)
   3. Administrative_distance: where a route learned from a more reliable
      routing protocol is preferred (only valid between different routing
      protocols)
Because a routing metric is specific to a given routing protocol, multi-
protocol routers must use some external heuristic to select between routes
learned from different routing protocols. Cisco routers, for example, attribute
a value known as the administrative_distance to each route, where smaller
administrative distances indicate routes learned from a supposedly more
reliable protocol.
A local network administrator, in special cases, can set up host-specific
routes to a particular device that provides more control over network usage,
permits testing, and better overall security. This is useful for debugging
network connections or routing tables.
In some small systems, a single central device decides ahead of time the
complete path of every packet. In some other small systems, whichever edge
device injects a packet into the network decides ahead of time the complete
path of that particular packet. In both of these systems, that route-planning
device needs to know a lot of information about what devices are connected to
the network and how they are connected to each other. Once it has this
information, it can use an algorithm such as A*_search_algorithm to find the
best path.
In high-speed systems, there are so many packets transmitted every second that
it is infeasible for a single device to calculate the complete path for each
and every packet. Early high-speed systems dealt with this by setting up a
circuit_switching relay_channel once for the first packet between some source
and some destination; later packets between that same source and that same
destination continue to follow the same path without recalculating until the
channel teardown. Later high-speed systems inject packets into the network
without any one device ever calculating a complete path for that
packetâmultiple agents.
In large systems, there are so many connections between devices, and those
connections change so frequently, that it is infeasible for any one device to
even know how all the devices are connected to each other, much less calculate
a complete path through them. Such systems generally use next-hop routing.
Most systems use a deterministic dynamic_routing algorithm: When a device
chooses a path to a particular final destination, that device always chooses
the same path to that destination until it receives information that makes it
think some other path is better. A few routing algorithms do not use a
deterministic algorithm to find the "best" link for a packet to get from its
original source to its final destination. Instead, to avoid congestion in
switched systems or network hot spots in packet systems, a few algorithms use a
randomized algorithmâValiant's paradigmâthat routes a path to a randomly
picked intermediate destination, and from there to its true final destination.
[2][3] In many early telephone switches, a randomizer was often used to select
the start of a path through a multistage_switching_fabric.
Depending on the application for which path selection is performed, different
metrics can be used. For example, for web requests one can use minimum latency
paths to minimize web page load time, or for bulk data transfers one can choose
the least utilized path to balance load across the network and increase
throughput. A popular path selection objective is to reduce the average
completion times of traffic flows and the total network bandwidth consumption
which basically lead to better use of network capacity. Recently, a path
selection metric was proposed that computes the total number of bytes scheduled
on the edges per path as selection metric.[4] An empirical analysis of several
path selection metrics, including this new proposal, has been made available.
[5]
***** Multiple agents[edit] *****
In some networks, routing is complicated by the fact that no single entity is
responsible for selecting paths; instead, multiple entities are involved in
selecting paths or even parts of a single path. Complications or inefficiency
can result if these entities choose paths to optimize their own objectives,
which may conflict with the objectives of other participants.
A classic example involves traffic in a road system, in which each driver picks
a path that minimizes their travel time. With such routing, the equilibrium
routes can be longer than optimal for all drivers. In particular, Braess'
paradox shows that adding a new road can lengthen travel times for all drivers.
In another model, for example, used for routing automated_guided_vehicles
(AGVs) on a terminal, reservations are made for each vehicle to prevent
simultaneous use of the same part of an infrastructure. This approach is also
referred to as context-aware routing.[6]
The Internet is partitioned into autonomous_systems (ASs) such as internet
service_providers (ISPs), each of which controls routes involving its network,
at multiple levels. First, AS-level paths are selected via the BGP protocol,
which produces a sequence of ASs through which packets flow. Each AS may have
multiple paths, offered by neighboring ASs, from which to choose. Its decision
often involves business relationships with these neighboring ASs,[7] which may
be unrelated to path quality or latency. Second, once an AS-level path has been
selected, there are often multiple corresponding router-level paths, in part
because two ISPs may be connected in multiple locations. In choosing the single
router-level path, it is common practice for each ISP to employ hot-potato
routing: sending traffic along the path that minimizes the distance through the
ISP's own networkâeven if that path lengthens the total distance to the
destination.
Consider two ISPs, A and B. Each has a presence in New_York, connected by a
fast link with latency 5 msâand each has a presence in London connected by a
5 ms link. Suppose both ISPs have trans-Atlantic links that connect their two
networks, but A's link has latency 100 ms and B's has latency 120 ms. When
routing a message from a source in A 's London network to a destination in B 's
New York network, A may choose to immediately send the message to B in London.
This saves A the work of sending it along an expensive trans-Atlantic link, but
causes the message to experience latency 125 ms when the other route would have
been 20 ms faster.
A 2003 measurement study of Internet routes found that, between pairs of
neighboring ISPs, more than 30% of paths have inflated latency due to hot-
potato routing, with 5% of paths being delayed by at least 12 ms. Inflation due
to AS-level path selection, while substantial, was attributed primarily to
BGP's lack of a mechanism to directly optimize for latency, rather than to
selfish routing policies. It was also suggested that, were an appropriate
mechanism in place, ISPs would be willing to cooperate to reduce latency rather
than use hot-potato routing.[8]
Such a mechanism was later published by the same authors, first for the case of
two ISPs[9] and then for the global case.[10]
***** Route analytics[edit] *****
As the Internet and IP networks become mission_critical business tools, there
has been increased interest in techniques and methods to monitor the routing
posture of networks. Incorrect routing or routing issues cause undesirable
performance degradation, flapping and/or downtime. Monitoring routing in a
network is achieved using route_analytics tools and techniques.
***** Centralized routing[edit] *****
In networks where a logically centralized control is available over the
forwarding state, for example using Software-defined_networking, routing
techniques can be used that aim to optimize global and network-wide performance
metrics. This has been used by large internet companies that operate many data
centers in different geographical locations attached using private optical
links examples of which includes Microsoft's Global WAN,[11] Facebook's Express
Backbone,[12] and Google's B4.[13] Global performance metrics to optimize
include maximizing network utilization, minimizing traffic flow completion
times, and maximizing the traffic delivered prior to specific deadlines.
Minimizing flow completion times over private WAN, particularly, has not
received much attention from the research community. However, with the
increasing number of businesses that operate globally distributed data centers
connected using private inter-data center networks, it is likely to see
increasing research effort in this realm.[14] A very recent work on reducing
the completion times of flows over private WAN discusses modeling routing as a
graph optimization problem by pushing all the queuing to the end-points.
Authors also propose a heuristic to solve the problem efficiently while
sacrificing negligible performance.[15]
***** See also[edit] *****
    * Collective_routing
    * Deflection_routing
    * Edge_Disjoint_Shortest_Pair_Algorithm
    * Flood_search_routing
    * Fuzzy_routing
    * Geographic_routing
    * Heuristic_routing
    * Path_computation_element (PCE)
    * Policy-based_routing
    * Wormhole_routing
    * Small_world_routing
    * Turn_restriction_routing
***** References[edit] *****
   1. ^ RFC_3626
   2. ^  Michael Mitzenmacher; AndrÃ©a W. Richa; Ramesh Sitaraman. "The_Power
      of_Two_Random_Choices:_A_Survey_of_Techniques_and_Results". Section
      "Randomized Protocols for Circuit Routing". p. 34.
   3. ^  Stefan Haas. "The_IEEE_1355_Standard:_Developments,_Performance_and
      Application_in_High_Energy_Physics". 1998. p. 15. quote: "To eliminate
      network hot spots, ... a two phase routing algorithm. This involves every
      packet being first sent to a randomly chosen intermediate destination;
      from the intermediate destination it is forwarded to its final
      destination. This algorithm, referred to as Universal Routing, is
      designed to maximize capacity and minimize delay under conditions of
      heavy load."
   4. ^M. Noormohammadpour; C. S. Raghavendra. (2018). "Poster_Abstract:
      Minimizing_Flow_Completion_Times_using_Adaptive_Routing_over_Inter-
      Datacenter_Wide_Area_Networks".
   5. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   6. ^M. Noormohammadpour; C. S. Raghavendra. (2018). "Minimizing_Flow
      Completion_Times_using_Adaptive_Routing_over_Inter-Datacenter_Wide_Area
      Networks".
   7. ^  Jonne Zutt, Arjan J.C. van Gemund, Mathijs M. de Weerdt, and Cees
      Witteveen (2010). Dealing_with_Uncertainty_in_Operational_Transport
      Planning. In R.R. Negenborn and Z. Lukszo and H. Hellendoorn (Eds.)
      Intelligent Infrastructures, Ch. 14, pp. 355â382. Springer.
   8. ^ Matthew Caesar and Jennifer_Rexford. BGP_routing_policies_in_ISP
      networks. IEEE Network Magazine, special issue on Interdomain Routing,
      Nov/Dec 2005.
   9. ^ Neil Spring, Ratul Mahajan, and Thomas Anderson. Quantifying_the_Causes
      of_Path_Inflation. Proc. SIGCOMM 2003.
  10. ^ Ratul Mahajan, David Wetherall, and Thomas Anderson. Negotiation-Based
      Routing_Between_Neighboring_ISPs. Proc. NSDI 2005.
  11. ^ Ratul Mahajan, David Wetherall, and Thomas Anderson. Mutually
      Controlled_Routing_with_Independent_ISPs. Proc. NSDI 2007.
  12. ^Khalidi, Yousef (March 15, 2017). "How_Microsoft_builds_its_fast_and
      reliable_global_network".
  13. ^"Building_Express_Backbone:_Facebook's_new_long-haul_network". May 1,
      2017.
  14. ^"Inside_Google's_Software-Defined_Network". May 14, 2017.
  15. ^Noormohammadpour, Mohammad; Raghavendra, Cauligi (16 July 2018).
      "Datacenter_Traffic_Control:_Understanding_Techniques_and_Tradeoffs".
      IEEE Communications Surveys and Tutorials. 20 (2): 1492â1525. arXiv:
      1712.03530. doi:10.1109/COMST.2017.2782753.
  16. ^Noormohammadpour, Mohammad; Srivastava, Ajitesh; Raghavendra, Cauligi
      (2018). "On_Minimizing_the_Completion_Times_of_Long_Flows_over_Inter-
      Datacenter_WAN". IEEE Communications Letters.
***** Further reading[edit] *****
    * Ash, Gerald (1997). Dynamic Routing in Telecommunication Networks.
      McGrawâHill. ISBN 978-0-07-006414-0.
Doyle, Jeff & Carroll, Jennifer (2005). Routing TCP/IP, Volume I, Second Ed.
Cisco Press. ISBN 978-1-58705-202-6.
Ciscopress
ISBN 1-58705-202-4
Doyle, Jeff & Carroll, Jennifer (2001). Routing TCP/IP, Volume II. Cisco Press.
ISBN 978-1-57870-089-9.
Ciscopress
ISBN 1-57870-089-2
Huitema, Christian (2000). Routing in the Internet, Second Ed. PrenticeâHall.
ISBN 978-0-321-22735-5.
Kurose, James E. & Ross, Keith W. (2004). Computer Networking, Third Ed.
Benjamin/Cummings. ISBN 978-0-321-22735-5.
Medhi, Deepankar & Ramasamy, Karthikeyan (2007). Network Routing: Algorithms,
Protocols, and Architectures. Morgan Kaufmann. ISBN 978-0-12-088588-6.
***** External links[edit] *****
 Wikiversity has learning resources about Routing
 Wikimedia Commons has media related to Routing.
    * Count-To-Infinity_Problem
    * "Stability_Features" are ways of avoiding the "count to infinity"
      problem.
    * Cisco_IT_Case_Studies about Routing and Switching
    * "IP_Routing_and_Subnets". www.eventhelix.com. Retrieved 2018-04-28.
    * v
    * t
    * e
Routing_protocols
                    * Babel
                    * B.A.T.M.A.N.
                    * BGP
General             * IS-IS
                    * OLSR
                    * OSPF
                    * RIP
Vendor-driven       * (Cisco) IGRP / EIGRP
                    * (Nortel) SMLT / R-SMLT / DSMLT
                    * CTP
Special-purpose     * CSPF
                    * DVMRP
Defunct             * BGMP
                    * EGP

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Routing&oldid=906401444"
Categories:
    * Internet_architecture
    * Routing
Hidden categories:
    * Pages_using_RFC_magic_links
    * Commons_category_link_from_Wikidata
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * íêµ­ì´
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * æ¥æ¬èª
    * PÃ¤lzisch
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ú©ÙØ±Ø¯Û
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 15 July 2019, at 16:19 (UTC).
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
