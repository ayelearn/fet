The following text has been accessed from https://en.wikipedia.org/wiki/Link-state_routing_protocol at Fri Aug 9 01:10:46 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Link-state routing protocol ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Link-state routing protocols are one of the two main classes of routing
protocols used in packet_switching networks for computer_communications, the
other being distance-vector_routing_protocols. Examples of link-state routing
protocols include Open_Shortest_Path_First (OSPF) and Intermediate_System_to
Intermediate_System (IS-IS).
The link-state protocol is performed by every switching node in the network
(i.e., nodes that are prepared to forward packets; in the Internet, these are
called routers). The basic concept of link-state routing is that every node
constructs a map of the connectivity to the network, in the form of a graph,
showing which nodes are connected to which other nodes. Each node then
independently calculates the next best logical path from it to every possible
destination in the network. Each collection of best paths will then form each
node's routing_table.
This contrasts with distance-vector_routing_protocols, which work by having
each node share its routing table with its neighbours, in a link-state protocol
the only information passed between nodes is connectivity related. Link-state
algorithms are sometimes characterized informally as each router, "telling the
world about its neighbours."
⁰
***** Contents *****
    * 1_History
    * 2_Distributing_maps
          o 2.1_Determining_the_neighbours_of_each_node
          o 2.2_Distributing_the_information_for_the_map
          o 2.3_Creating_the_map
          o 2.4_Notes_about_this_stage
    * 3_Calculating_the_routing_table
          o 3.1_Calculating_the_shortest_paths
          o 3.2_Filling_the_routing_table
    * 4_Optimizations_to_the_algorithm
          o 4.1_Partial_Recomputation
          o 4.2_Topology_Reduction
          o 4.3_Fisheye_State_Routing
    * 5_Failure_modes
    * 6_The_Optimized_Link_State_Routing_Protocol_for_mobile_ad_hoc_networks
    * 7_See_also
    * 8_References
    * 9_Further_reading
***** History[edit] *****
What is believed to be the first adaptive routing network of computers, using
link-state routing as its heart, was designed and implemented during 1976-77 by
a team from Plessey_Radar led by Bernard J Harris; the project was for "Wavell"
- a system of computer command and control for the British Army.[citation
needed]
The first link-state routing concept was published in 1979 by John_M._McQuillan
(then at Bolt,_Beranek_and_Newman) as a mechanism that would calculate routes
more quickly when network conditions changed, and thus lead to more stable
routing.[1][2]
Later work at BBN_Technologies showed how to use the link-state technique in a
hierarchical system (i.e., one in which the network was divided into areas) so
that each switching node does not need a map of the entire network, only the
area(s) in which it is included.[citation_needed]
The technique was later adapted for use in the contemporary link-state routing
protocols IS-IS and OSPF. Cisco literature refers to enhanced_interior_gateway
routing_protocol (EIGRP) as a "hybrid" protocol,[citation_needed] despite the
fact it distributes routing tables instead of topology maps. However, it does
synchronize routing tables at start up as OSPF does, and sends specific updates
only when topology changes occur.
In 2004, Radia_Perlman proposed using link-state routing for layer_2 frame
forwarding with devices called routing_bridges or Rbridges. The Internet
Engineering_Task_Force has standardized the transparent_interconnection_of_lots
of_links (TRILL) protocol to accomplish this.[3]
More recently, this hierarchical technique was applied to wireless_mesh
networks using the optimized_link_state_routing_protocol (OLSR). Where a
connection can have varying quality, the quality of a connection can be used to
select better connections. This is used in some routing_protocols that use
radio frequency transmission.
In 2012, the IEEE completed and approved the standardization of the use of IS-
IS to control Ethernet forwarding with IEEE_802.1aq shortest path bridging
(SPB).
***** Distributing maps[edit] *****
This description covers only the simplest configuration; i.e., one with no
areas, so that all nodes have a map of the entire network. The hierarchical
case is somewhat more complex; see the various protocol specifications.
As previously mentioned, the first main stage in the link-state algorithm is to
give a map of the network to every node. This is done with several subsidiary
steps.
**** Determining the neighbours of each node[edit] ****
First, each node needs to determine what other ports it is connected to, over
fully working links; it does this using a reachability protocol which it runs
periodically and separately with each of its directly connected neighbours.
**** Distributing the information for the map[edit] ****
Next, each node periodically (and in case of connectivity changes) sends a
short message, the link-state_advertisement, which:
    * Identifies the node which is producing it.
    * Identifies all the other nodes (either routers or networks) to which it
      is directly connected.
    * Includes a 'sequence number', which increases every time the source node
      makes up a new version of the message.
This message is sent to all the nodes on a network. As a necessary precursor,
each node in the network remembers, for every one of its neighbors, the
sequence number of the last link-state message which it received from that
node. When a link-state advertisement is received at a node, the node looks up
the sequence number it has stored for the source of that link-state message: if
this message is newer (i.e., has a higher sequence number), it is saved, and a
copy is sent in turn to each of that node's neighbors. This procedure rapidly
gets a copy of the latest version of each node's link-state advertisement to
every node in the network.
Networks running link state algorithms can also be segmented into hierarchies
which limit the scope of route changes. These features mean that link state
algorithms scale better to larger networks.
**** Creating the map[edit] ****
Finally, with the complete set of link-state advertisements (one from each node
in the network) in hand, each node produces the graph for the map of the
network. The algorithm iterates over the collection of link-state
advertisements; for each one, it makes links on the map of the network, from
the node which sent that message, to all the nodes which that message indicates
are neighbors of the sending node.
No link is considered to have been correctly reported unless the two ends
agree; i.e., if one node reports that it is connected to another, but the other
node does not report that it is connected to the first, there is a problem, and
the link is not included on the map.
**** Notes about this stage[edit] ****
The link-state message giving information about the neighbors is recomputed,
and then flooded throughout the network, whenever there is a change in the
connectivity between the node and its neighbors; e.g., when a link fails. Any
such change will be detected by the reachability protocol which each node runs
with its neighbors.
***** Calculating the routing table[edit] *****
As initially mentioned, the second main stage in the link-state algorithm is to
produce routing tables, by inspecting the maps. This is again done with several
steps.
**** Calculating the shortest paths[edit] ****
Each node independently runs an algorithm over the map to determine the
shortest_path from itself to every other node in the network; generally some
variant of Dijkstra's_algorithm is used. This is based around a link cost
across each path which includes available bandwidth among other things.
A node maintains two data structures: a tree containing nodes which are "done",
and a list of candidates. The algorithm starts with both structures empty; it
then adds to the first one the node itself. The variant of a Greedy_Algorithm
then repetitively does the following:
    * All neighbour nodes which are directly connected to the node are just
      added to the tree (excepting any nodes which are already in either the
      tree or the candidate list). The rest are added to the second (candidate)
      list.
    * Each node in the candidate list is compared to each of the nodes already
      in the tree. The candidate node which is closest to any of the nodes
      already in the tree is itself moved into the tree and attached to the
      appropriate neighbor node. When a node is moved from the candidate list
      into the tree, it is removed from the candidate list and is not
      considered in subsequent iterations of the algorithm.
The above two steps are repeated as long as there are any nodes left in the
candidate list. (When there are none, all the nodes in the network will have
been added to the tree.) This procedure ends with the tree containing all the
nodes in the network, with the node on which the algorithm is running as the
root of the tree. The shortest path from that node to any other node is
indicated by the list of nodes one traverses to get from the root of the tree,
to the desired node in the tree..!
**** Filling the routing table[edit] ****
With the shortest paths in hand, the next step is to fill in the routing table.
For any given destination node, the best path for that destination is the node
which is the first step from the root node, down the branch in the shortest-
path tree which leads toward the desired destination node. To create the
routing table, it is only necessary to walk the tree, remembering the identity
of the node at the head of each branch, and filling in the routing table entry
for each node one comes across with that identity.
***** Optimizations to the algorithm[edit] *****
The algorithm described above was made as simple as possible, to aid in ease of
understanding. In practice, there are a number of optimizations which are used.
**** Partial Recomputation[edit] ****
Whenever a change in the connectivity map happens, it is necessary to recompute
the shortest-path tree, and then recreate the routing table. Work by BBN
Technologies[citation_needed] discovered how to recompute only that part of the
tree which could have been affected by a given change in the map. Also, the
routing table would normally be filled in as the shortest-path tree is
computed, instead of making it a separate operation.
**** Topology Reduction[edit] ****
In some cases it is reasonable to reduce the number of nodes that generate LSA
messages. For instance, a node that has only one connection to the network
graph does not need to send LSA messages, as the information on its existence
could be already included in the LSA message of its only neighbor. For this
reason a topology reduction strategy can be applied, in which only a subset of
the network nodes generate LSA messages. Two widely studied approaches for
topology reduction are:
   1. MultiPoint_Relays that are at the base of the OLSR protocol but have also
      been proposed for OSPF[4]
   2. Connected_Dominating_Sets that again have been proposed for OSPF[5]
**** Fisheye State Routing[edit] ****
With FSR the LSA are sent with different TTL values in order to restrict their
diffusion and limit the overhead due to control messages. The same concept is
used also in the Hazy_Sighted_Link_State_Routing_Protocol.
***** Failure modes[edit] *****
If all the nodes are not working from exactly the same map, routing loops can
form. These are situations in which, in the simplest form, two neighboring
nodes each think the other is the best path to a given destination. Any packet
headed to that destination arriving at either node will loop between the two,
hence the name. Routing loops involving more than two nodes are also possible.
This can occur since each node computes its shortest-path tree and its routing
table without interacting in any way with any other nodes. If two nodes start
with different maps, it is possible to have scenarios in which routing loops
are created.
***** The Optimized Link State Routing Protocol for mobile ad hoc networks
[edit] *****
The Optimized_Link_State_Routing_Protocol (OLSR) is a link-state routing
protocol optimized for mobile_ad_hoc_networks (which can also be used on other
wireless_ad_hoc_networks).[6] OLSR is proactive, it uses Hello and Topology
Control (TC) messages to discover and disseminate link state information into
the mobile_ad_hoc_network. Using Hello messages each node discovers 2-hop
neighbor information and elects a set of multipoint_relays (MPRs). MPRs makes
OLSR unique from other link state routing protocols. Individual nodes use the
topology information to compute next hop paths regard to all nodes in the
network using shortest hop forwarding paths.
***** See also[edit] *****
    * 802.1aq_Shortest_Path_Bridging
***** References[edit] *****
   1. ^ John_M._McQuillan, Isaac Richer and Eric C. Rosen, ARPANet Routing
      Algorithm Improvements, BBN Report No. 3803, Cambridge, April 1978
   2. ^ John_M._McQuillan, Isaac Richer and Eric C. Rosen, The New Routing
      Algorithm for the ARPANet, IEEE Trans. on Comm., 28(5), pp. 711â719,
      1980
   3. ^Transparent Interconnection of Lots of Links (TRILL) Use of IS-IS,
      RFC 7176
   4. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   5. ^ https://tools.ietf.org/html/rfc5449
   6. ^ https://tools.ietf.org/html/rfc5614
   7. ^ RFC_3626
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (September 2010)(Learn_how_and
 when_to_remove_this_template_message)
    * Josh Seeger and Atul Khanna, Reducing Routing Overhead in a Growing DDN,
      MILCOMM '86, IEEE, 1986
    * Radia_Perlman âRbridges:_Transparent_Routingâ, Infocom 2004.
***** Further reading[edit] *****
    * Section_"Link-State_Versus_Distance_Vector" in the Chapter "Routing
      Basics" in the Cisco "Internetworking Technology Handbook"

Retrieved from "https://en.wikipedia.org/w/index.php?title=Link-
state_routing_protocol&oldid=895901629"
Categories:
    * Routing_protocols
    * Routing_algorithms
Hidden categories:
    * Pages_using_RFC_magic_links
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2016
    * Articles_with_unsourced_statements_from_February_2013
    * Articles_with_unsourced_statements_from_March_2013
    * Articles_lacking_in-text_citations_from_September_2010
    * All_articles_lacking_in-text_citations
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
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Italiano
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
Edit_links
    * This page was last edited on 7 May 2019, at 05:58 (UTC).
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
