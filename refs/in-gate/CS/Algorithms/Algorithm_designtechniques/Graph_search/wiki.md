The following text has been accessed from https://en.wikipedia.org/wiki/Graph_traversal at Fri Aug 9 01:09:50 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Graph traversal ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Graph search" redirects here. It is not to be confused with Facebook_Graph
Search.
 This article needs additional citations for verification. Please help improve_this_article by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and removed.
 Find sources: "Graph_traversal" â news Â· newspapers Â· books Â· scholar Â· JSTOR (October
 2014)(Learn_how_and_when_to_remove_this_template_message)
Graph and tree
search_algorithms
    * Î±âÎ²
    * A*
    * B*
    * Backtracking
    * Beam
    * BellmanâFord
    * Best-first
    * Bidirectional
    * BorÅ¯vka
    * Branch_&_bound
    * BFS
    * British_Museum
    * D*
    * DFS
    * Dijkstra
    * Edmonds
    * FloydâWarshall
    * Fringe_search
    * Hill_climbing
    * IDA*
    * Iterative_deepening
    * Johnson
    * Jump_point
    * Kruskal
    * Lexicographic_BFS
    * LPA*
    * Prim
    * SMA*
    * SPFA
Listings
    * Graph_algorithms
    * Search_algorithms
    * List_of_graph_algorithms
Related topics
    * Dynamic_programming
    * Graph traversal
    * Tree_traversal
    * Search_games
    * v
    * t
    * e
In computer_science, graph traversal (also known as graph search) refers to the
process of visiting (checking and/or updating) each vertex in a graph. Such
traversals are classified by the order in which the vertices are visited. Tree
traversal is a special case of graph traversal.
⁰
***** Contents *****
    * 1_Redundancy
    * 2_Graph_traversal_algorithms
          o 2.1_Depth-first_search
                # 2.1.1_Pseudocode
          o 2.2_Breadth-first_search
                # 2.2.1_Pseudocode
    * 3_Applications
    * 4_Graph_exploration
    * 5_Universal_traversal_sequences
    * 6_References
    * 7_See_also
***** Redundancy[edit] *****
Unlike tree traversal, graph traversal may require that some vertices be
visited more than once, since it is not necessarily known before transitioning
to a vertex that it has already been explored. As graphs become more dense,
this redundancy becomes more prevalent, causing computation time to increase;
as graphs become more sparse, the opposite holds true.
Thus, it is usually necessary to remember which vertices have already been
explored by the algorithm, so that vertices are revisited as infrequently as
possible (or in the worst case, to prevent the traversal from continuing
indefinitely). This may be accomplished by associating each vertex of the graph
with a "color" or "visitation" state during the traversal, which is then
checked and updated as the algorithm visits each vertex. If the vertex has
already been visited, it is ignored and the path is pursued no further;
otherwise, the algorithm checks/updates the vertex and continues down its
current path.
Several special cases of graphs imply the visitation of other vertices in their
structure, and thus do not require that visitation be explicitly recorded
during the traversal. An important example of this is a tree: during a
traversal it may be assumed that all "ancestor" vertices of the current vertex
(and others depending on the algorithm) have already been visited. Both the
depth-first and breadth-first_graph_searches are adaptations of tree-based
algorithms, distinguished primarily by the lack of a structurally determined
"root" vertex and the addition of a data structure to record the traversal's
visitation state.
***** Graph traversal algorithms[edit] *****
Note. â If each vertex in a graph is to be traversed by a tree-based
algorithm (such as DFS or BFS), then the algorithm must be called at least once
for each connected_component of the graph. This is easily accomplished by
iterating through all the vertices of the graph, performing the algorithm on
each vertex that is still unvisited when examined.
A non-verbal description of three graph traversal algorithms: randomly, depth-
first search, and breadth-first search.
**** Depth-first search[edit] ****
Main article: Depth-first_search
A depth-first search (DFS) is an algorithm for traversing a finite graph. DFS
visits the child vertices before visiting the sibling vertices; that is, it
traverses the depth of any particular path before exploring its breadth. A
stack (often the program's call_stack via recursion) is generally used when
implementing the algorithm.
The algorithm begins with a chosen "root" vertex; it then iteratively
transitions from the current vertex to an adjacent, unvisited vertex, until it
can no longer find an unexplored vertex to transition to from its current
location. The algorithm then backtracks along previously visited vertices,
until it finds a vertex connected to yet more uncharted territory. It will then
proceed down the new path as it had before, backtracking as it encounters dead-
ends, and ending only when the algorithm has backtracked past the original
"root" vertex from the very first step.
DFS is the basis for many graph-related algorithms, including topological_sorts
and planarity_testing.
*** Pseudocode[edit] ***
    * Input: A graph G and a vertex v of G.
    * Output: A labeling of the edges in the connected component of v as
      discovery edges and back edges.
1 procedure DFS(G, v):
2     label v as explored
3     for all edges e in G.incidentEdges(v) do
4         if edge e is unexplored then
5             w â G.adjacentVertex(v, e)
6             if vertex w is unexplored then
7                 label e as a discovered edge
8                 recursively call DFS(G, w)
9             else
10               label e as a back edge
**** Breadth-first search[edit] ****
Main article: Breadth-first_search
[[icon]] This section needs expansion. You can help by adding_to_it. (October
         2012)
A breadth-first search (BFS) is another technique for traversing a finite
graph. BFS visits the sibling vertices before visiting the child vertices, and
a queue is used in the search process. This algorithm is often used to find the
shortest path from one vertex to another.
*** Pseudocode[edit] ***
    * Input: A graph G and a vertex v of G.
    * Output: The closest vertex to v satisfying some conditions, or null if no
      such vertex exists.
1 procedure BFS(G, v):
2     create a queue Q
3     enqueue v onto Q
4     mark v
5     while Q is not empty do
6         w â Q.dequeue()
7         if w is what we are looking for then
8             return w
9         for all edges e in G.adjacentEdges(w) do
12            x â G.adjacentVertex(w, e)
13            if x is not marked then
14                mark x
15                enqueue x onto Q
16     return null
***** Applications[edit] *****
Breadth-first search can be used to solve many problems in graph theory, for
example:
    * finding all vertices within one connected_component;
    * Cheney's_algorithm;
    * finding the shortest_path between two vertices;
    * testing a graph for bipartiteness;
    * CuthillâMcKee_algorithm mesh numbering;
    * FordâFulkerson_algorithm for computing the maximum_flow in a flow
      network;
    * serialization/deserialization of a binary tree vs serialization in sorted
      order (allows the tree to be re-constructed in an efficient manner);
    * maze_generation_algorithms;
    * flood_fill algorithm for marking contiguous regions of a two dimensional
      image or n-dimensional array;
    * analysis of networks and relationships.
***** Graph exploration[edit] *****
The problem of graph exploration can be seen as a variant of graph traversal.
It is an online problem, meaning that the information about the graph is only
revealed during the runtime of the algorithm. A common model is as follows:
given a connected graph G = (V, E) with non-negative edge weights. The
algorithm starts at some vertex, and knows all incident outgoing edges and the
vertices at the end of these edgesâbut not more. When a new vertex is
visited, then again all incident outgoing edges and the vertices at the end are
known. The goal is to visit all n vertices and return to the starting vertex,
but the sum of the weights of the tour should be as small as possible. The
problem can also be understood as a specific version of the travelling_salesman
problem, where the salesman has to discover the graph on the go.
For general graphs, the best known algorithms for both undirected and directed
graphs is a simple greedy algorithm:
    * In the undirected case, the greedy tour is at most O(ln n)-times longer
      than an optimal tour.[1] The best lower bound known for any deterministic
      online algorithm is 2.5 â Îµ;[2]
    * In the directed case, the greedy tour is at most (n â 1)-times longer
      than an optimal tour. This matches the lower bound of n â 1.[3] An
      analogous competitive lower bound of Î©(n) also holds for randomized
      algorithms that know the coordinates of each node in a geometric
      embedding. If instead of visiting all nodes just a single "treasure" node
      has to be found, the competitive bounds are Î(n2) on unit weight
      directed graphs, for both deterministic and randomized algorithms.
***** Universal traversal sequences[edit] *****
[[icon]] This section needs expansion. You can help by adding_to_it. (December
         2016)
A universal traversal sequence is a sequence of instructions comprising a graph
traversal for any regular_graph with a set number of vertices and for any
starting vertex. A probabilistic proof was used by Aleliunas et al. to show
that there exists a universal traversal sequence with number of instructions
proportional to O(n5) for any regular graph with n vertices.[4] The steps
specified in the sequence are relative to the current node, not absolute. For
example, if the current node is vj, and vj has d neighbors, then the traversal
sequence will specify the next node to visit, vj+1, as the ith neighbor of vj,
where 1 â¤ i â¤ d.
***** References[edit] *****
   1. ^Rosenkrantz, Daniel J.; Stearns, Richard E.; Lewis, II, Philip M.
      (1977). "An Analysis of Several Heuristics for the Traveling Salesman
      Problem". SIAM Journal on Computing. 6 (3): 563â581. doi:10.1137/
      0206041.
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
   3. ^Dobrev, Stefan; KrÃ¡lovic, Rastislav; Markou, Euripides (2012). "Online
      Graph Exploration with Advice". Proc. Of the 19th International
      Colloquium on Structural Information and Communication Complexity
      (SIROCCO). Lecture Notes in Computer Science. 7355: 267â278. doi:
      10.1007/978-3-642-31104-8_23. ISBN 978-3-642-31103-1.
   4. ^Foerster, Klaus-Tycho; Wattenhofer, Roger (December 2016). "Lower_and
      upper_competitive_bounds_for_online_directed_graph_exploration".
      Theoretical Computer Science. 655: 15â29. doi:10.1016/
      j.tcs.2015.11.017.
   5. ^Aleliunas, R.; Karp, R.; Lipton, R.; LovÃ¡sz, L.; Rackoff, C. (1979).
      "Random walks, universal traversal sequences, and the complexity of maze
      problems". 20th Annual Symposium on Foundations of Computer Science (SFCS
      1979): 218â223. doi:10.1109/SFCS.1979.34.
***** See also[edit] *****
    * External_memory_graph_traversal

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Graph_traversal&oldid=908932053"
Categories:
    * Graph_algorithms
Hidden categories:
    * Articles_needing_additional_references_from_October_2014
    * All_articles_needing_additional_references
    * Articles_to_be_expanded_from_October_2012
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
    * Articles_to_be_expanded_from_December_2016
    * Articles_with_example_pseudocode
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
    * Deutsch
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Polski
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 1 August 2019, at 23:08 (UTC).
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
