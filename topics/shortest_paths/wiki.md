The following text has been accessed from https://en.wikipedia.org/wiki/Shortest_path_problem at Fri Aug 9 01:09:48 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Shortest path problem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (June 2009)(Learn_how_and_when
 to_remove_this_template_message)
Shortest path (A, C, E, D, F) between vertices A and F in the weighted directed
graph
In graph_theory, the shortest path problem is the problem of finding a path
between two vertices (or nodes) in a graph such that the sum of the weights of
its constituent edges is minimized.
The problem of finding the shortest path between two intersections on a road
map may be modeled as a special case of the shortest path problem in graphs,
where the vertices correspond to intersections and the edges correspond to road
segments, each weighted by the length of the segment.
⁰
***** Contents *****
    * 1_Definition
    * 2_Algorithms
    * 3_Single-source_shortest_paths
          o 3.1_Undirected_graphs
          o 3.2_Unweighted_graphs
          o 3.3_Directed_acyclic_graphs_(DAGs)
          o 3.4_Directed_graphs_with_nonnegative_weights
          o 3.5_Directed_graphs_with_arbitrary_weights_without_negative_cycles
          o 3.6_Planar_directed_graphs_with_arbitrary_weights
    * 4_All-pairs_shortest_paths
          o 4.1_Undirected_graph
          o 4.2_Directed_graph
    * 5_Applications
          o 5.1_Road_networks
    * 6_Related_problems
          o 6.1_Strategic_shortest-paths
    * 7_Linear_programming_formulation
    * 8_General_algebraic_framework_on_semirings:_the_algebraic_path_problem
    * 9_Shortest_path_in_stochastic_time-dependent_networks
    * 10_See_also
    * 11_References
          o 11.1_Notes
          o 11.2_Bibliography
    * 12_Further_reading
***** Definition[edit] *****
The shortest path problem can be defined for graphs whether undirected,
directed, or mixed. It is defined here for undirected graphs; for directed
graphs the definition of path requires that consecutive vertices be connected
by an appropriate directed edge.
Two vertices are adjacent when they are both incident to a common edge. A path
in an undirected graph is a sequence of vertices     P = (  v  1   ,  v  2   ,
&#x2026; ,  v  n   ) &#x2208; V &#x00D7; V &#x00D7; &#x22EF; &#x00D7; V
{\displaystyle P=(v_{1},v_{2},\ldots ,v_{n})\in V\times V\times \cdots \times
V}  [{\displaystyle P=(v_{1},v_{2},\ldots ,v_{n})\in V\times V\times \cdots
\times V}] such that      v  i     {\displaystyle v_{i}}  [v_{i}] is adjacent
to      v  i + 1     {\displaystyle v_{i+1}}  [v_{i+1}] for     1 &#x2264; i <
n   {\displaystyle 1\leq i<n}  [1\leq i<n]. Such a path     P   {\displaystyle
P}  [P] is called a path of length     n &#x2212; 1   {\displaystyle n-1}  [n-
1] from      v  1     {\displaystyle v_{1}}  [v_{1}] to      v  n
{\displaystyle v_{n}}  [v_{n}]. (The      v  i     {\displaystyle v_{i}}  [v_
{i}] are variables; their numbering here relates to their position in the
sequence and needs not to relate to any canonical labeling of the vertices.)
Let      e  i , j     {\displaystyle e_{i,j}}  [e_{i,j}] be the edge incident
to both      v  i     {\displaystyle v_{i}}  [v_{i}] and      v  j
{\displaystyle v_{j}}  [v_{j}]. Given a real-valued weight function     f : E
&#x2192;  R    {\displaystyle f:E\rightarrow \mathbb {R} }  [f:E\rightarrow
\mathbb {R} ], and an undirected (simple) graph     G   {\displaystyle G}  [G],
the shortest path from     v   {\displaystyle v}  [v] to      v &#x2032;
{\displaystyle v'}  [v'] is the path     P = (  v  1   ,  v  2   , &#x2026; ,
v  n   )   {\displaystyle P=(v_{1},v_{2},\ldots ,v_{n})}  [P=(v_{1},v_
{2},\ldots ,v_{n})] (where      v  1   = v   {\displaystyle v_{1}=v}  [v_{1}=v]
and      v  n   =  v &#x2032;    {\displaystyle v_{n}=v'}  [v_{n}=v']) that
over all possible     n   {\displaystyle n}  [n] minimizes the sum
&#x2211;  i = 1   n &#x2212; 1   f (  e  i , i + 1   ) .   {\displaystyle \sum
_{i=1}^{n-1}f(e_{i,i+1}).}  [\sum _{i=1}^{n-1}f(e_{i,i+1}).] When each edge in
the graph has unit weight or     f : E &#x2192; { 1 }   {\displaystyle f:
E\rightarrow \{1\}}  [f:E\rightarrow \{1\}], this is equivalent to finding the
path with fewest edges.
The problem is also sometimes called the single-pair shortest path problem, to
distinguish it from the following variations:
    * The single-source shortest path problem, in which we have to find
      shortest paths from a source vertex v to all other vertices in the graph.
    * The single-destination shortest path problem, in which we have to find
      shortest paths from all vertices in the directed graph to a single
      destination vertex v. This can be reduced to the single-source shortest
      path problem by reversing the arcs in the directed graph.
    * The all-pairs shortest path problem, in which we have to find shortest
      paths between every pair of vertices v, v' in the graph.
These generalizations have significantly more efficient algorithms than the
simplistic approach of running a single-pair shortest path algorithm on all
relevant pairs of vertices.
***** Algorithms[edit] *****
The most important algorithms for solving this problem are:
    * Dijkstra's_algorithm solves the single-source shortest path problem with
      non-negative edge weight.
    * BellmanâFord_algorithm solves the single-source problem if edge weights
      may be negative.
    * A*_search_algorithm solves for single pair shortest path using heuristics
      to try to speed up the search.
    * FloydâWarshall_algorithm solves all pairs shortest paths.
    * Johnson's_algorithm solves all pairs shortest paths, and may be faster
      than FloydâWarshall on sparse_graphs.
    * Viterbi_algorithm solves the shortest stochastic path problem with an
      additional probabilistic weight on each node.
Additional algorithms and associated evaluations may be found in Cherkassky,
Goldberg_&_Radzik_(1996).
***** Single-source shortest paths[edit] *****
**** Undirected graphs[edit] ****
Weights Time_complexity  Author
â+ O(V2)            Dijkstra_1959
â+ O((E + V) log�Johnson_1977 (binary_heap)
â+ O(E + V log VFredman_&_Tarjan_1984 (Fibonacci_heap)
â  O(E)             Thorup_1999 (requires constant-time multiplication).
**** Unweighted graphs[edit] ****
Algorithm            Time complexity Author
Breadth-first_search O(E + V)
**** Directed acyclic graphs (DAGs)[edit] ****
An algorithm using topological_sorting can solve the single-source shortest
path problem in linear time, Î(E + V), in weighted DAGs.
**** Directed graphs with nonnegative weights[edit] ****
The following table is taken from Schrijver_(2004), with some corrections and
additions. A green background indicates an asymptotically best bound in the
table; L is the maximum length (or weight) among all edges, assuming integer
edge weights.
Algorithm                 Time complexity    Author
                          O(V2EL)            Ford_1956
BellmanâFord_algorithO(VE)              Shimbel_1955, Bellman_1958,
                                             Moore_1959
                          O(V2 log V)      Dantzig_1960
                                             Leyzorek_et_al._1957, Dijkstra
Dijkstra's_algorithm with O(V2)              1959, Minty (see Pollack_&
list                                         Wiebenson_1960), Whiting_&
                                             Hillier_1960
Dijkstra's_algorithm with O((E + V) log VJohnson_1977
binary_heap
. . .                     . . .              . . .
Dijkstra's_algorithm with O(E + V log V) Fredman_&_Tarjan_1984, Fredman
Fibonacci_heap                               &_Tarjan_1987
                          O(E log log L)  Johnson_1981, Karlsson_&
                                             Poblete_1983
Gabow's_algorithm         O(E logE/V L)    Gabow_1983, Gabow_1985
                          O(E + V √log L)Ahuja_et_al._1990
Thorup                    O(E + V log logThorup_2004
This list is incomplete; you can help by expanding_it.
**** Directed graphs with arbitrary weights without negative cycles[edit] ****
Algorithm                Time complexity Author
                         O(V2EL)         Ford_1956
BellmanâFord_algoritO(VE)           Shimbel_1955, Bellman_1958, Moore_1959
This list is incomplete; you can help by expanding_it.
**** Planar directed graphs with arbitrary weights[edit] ****
***** All-pairs shortest paths[edit] *****
The all-pairs shortest path problem finds the shortest paths between every pair
of vertices v, v' in the graph. The all-pairs shortest paths problem for
unweighted directed graphs was introduced by Shimbel_(1953), who observed that
it could be solved by a linear number of matrix multiplications that takes a
total time of O(V4).
**** Undirected graph[edit] ****
Weights                 Time complexity            Algorithm
â+                 O(V3)                      FloydâWarshall_algorithm
   { + 1 , + &#x221E; }    O (  V  &#x03C9;   log
{\displaystyle \        &#x2061; V )               Seidel's_algorithm
{+1,+\infty \}}  [      {\displaystyle O(V^{\omega (expected running time).
{\displaystyle \        }\log V)}  [{\displaystyle
{+1,+\infty \}}]        O(V^{\omega }\log V)}]
                           O (  V  3    /   2
                        &#x03A9; ( log &#x2061; n
                        )  1  /  2     )
â                  {\displaystyle O(V^{3}/2^  Williams_2014
                        {\Omega (\log n)^{1/2}})}
                        [O(V^{3}/2^{\Omega (\log
                        n)^{1/2}})]
â+                 O(EV log Î±(E,V))      Pettie_&_Ramachandran_2002
                                                   Thorup_1999 (requires
â                  O(EV)                      constant-time
                                                   multiplication).
**** Directed graph[edit] ****
Weights                  Time complexity             Algorithm
â (no negative cycleO(V3)                       FloydâWarshall_algorithm
                            O (  V  3    /   2
                         &#x03A9; ( log &#x2061; n
                         )  1  /  2     )
â                   {\displaystyle O(V^{3}/2^   Williams_2014
                         {\Omega (\log n)^{1/2}})}
                         [O(V^{3}/2^{\Omega (\log
                         n)^{1/2}})]
â (no negative cycleO(EV + V2 log V)        JohnsonâDijkstra
â (no negative cycleO(EV + V2 log log V)   Pettie_2004
â                   O(EV + V2 log log V)   Hagerup_2000
***** Applications[edit] *****
Shortest path algorithms are applied to automatically find directions between
physical locations, such as driving directions on web_mapping websites like
MapQuest or Google_Maps. For this application fast specialized algorithms are
available.[1]
If one represents a nondeterministic abstract_machine as a graph where vertices
describe states and edges describe possible transitions, shortest path
algorithms can be used to find an optimal sequence of choices to reach a
certain goal state, or to establish lower bounds on the time needed to reach a
given state. For example, if vertices represent the states of a puzzle like a
Rubik's_Cube and each directed edge corresponds to a single move or turn,
shortest path algorithms can be used to find a solution that uses the minimum
possible number of moves.
In a networking or telecommunications mindset, this shortest path problem is
sometimes called the min-delay path problem and usually tied with a widest_path
problem. For example, the algorithm may seek the shortest (min-delay) widest
path, or widest shortest (min-delay) path.
A more lighthearted application is the games of "six_degrees_of_separation"
that try to find the shortest path in graphs like movie stars appearing in the
same film.
Other applications, often studied in operations_research, include plant and
facility layout, robotics, transportation, and VLSI design.[2]
**** Road networks[edit] ****
A road network can be considered as a graph with positive weights. The nodes
represent road junctions and each edge of the graph is associated with a road
segment between two junctions. The weight of an edge may correspond to the
length of the associated road segment, the time needed to traverse the segment,
or the cost of traversing the segment. Using directed edges it is also possible
to model one-way streets. Such graphs are special in the sense that some edges
are more important than others for long distance travel (e.g. highways). This
property has been formalized using the notion of highway dimension.[3] There
are a great number of algorithms that exploit this property and are therefore
able to compute the shortest path a lot quicker than would be possible on
general graphs.
All of these algorithms work in two phases. In the first phase, the graph is
preprocessed without knowing the source or target node. The second phase is the
query phase. In this phase, source and target node are known.The idea is that
the road network is static, so the preprocessing phase can be done once and
used for a large number of queries on the same road network.
The algorithm with the fastest known query time is called hub labeling and is
able to compute shortest path on the road networks of Europe or the USA in a
fraction of a microsecond.[4] Other techniques that have been used are:
    * ALT (A* search, landmarks, and triangle_inequality)
    * Arc flags
    * Contraction_hierarchies
    * Transit node routing
    * Reach-based pruning
    * Labeling
    * Hub_labels
***** Related problems[edit] *****
For shortest path problems in computational_geometry, see Euclidean_shortest
path.
The travelling_salesman_problem is the problem of finding the shortest path
that goes through every vertex exactly once, and returns to the start. Unlike
the shortest path problem, which can be solved in polynomial time in graphs
without negative cycles, the travelling salesman problem is NP-complete and, as
such, is believed not to be efficiently solvable for large sets of data (see P
=_NP_problem). The problem of finding_the_longest_path in a graph is also NP-
complete.
The Canadian_traveller_problem and the stochastic shortest path problem are
generalizations where either the graph isn't completely known to the mover,
changes over time, or where actions (traversals) are probabilistic.
The shortest multiple disconnected path [5] is a representation of the
primitive path network within the framework of Reptation_theory.
The widest_path_problem seeks a path so that the minimum label of any edge is
as large as possible.
**** Strategic shortest-paths[edit] ****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (December 2015)(Learn_how_and_when_to_remove_this_template_message)
Sometimes, the edges in a graph have personalities: each edge has its own
selfish interest. An example is a communication network, in which each edge is
a computer that possibly belongs to a different person. Different computers
have different transmission speeds, so every edge in the network has a numeric
weight equal to the number of milliseconds it takes to transmit a message. Our
goal is to send a message between two points in the network in the shortest
time possible. If we know the transmission-time of each computer (the weight of
each edge), then we can use a standard shortest-paths algorithm. If we do not
know the transmission times, then we have to ask each computer to tell us its
transmission-time. But, the computers may be selfish: a computer might tell us
that its transmission time is very long, so that we will not bother it with our
messages. A possible solution to this problem is to use a_variant_of_the_VCG
mechanism, which gives the computers an incentive to reveal their true weights.
***** Linear programming formulation[edit] *****
There is a natural linear_programming formulation for the shortest path
problem, given below. It is very simple compared to most other uses of linear
programs in discrete_optimization, however it illustrates connections to other
concepts.
Given a directed graph (V, A) with source node s, target node t, and cost wij
for each edge (i, j) in A, consider the program with variables xij
      minimize      &#x2211;  i j &#x2208; A    w  i j    x  i j
      {\displaystyle \sum _{ij\in A}w_{ij}x_{ij}}  [\sum _{ij\in A}w_{ij}x_
      {ij}] subject to     x &#x2265; 0   {\displaystyle x\geq 0}  [x\geq 0]
      and for all i,      &#x2211;  j    x  i j   &#x2212;  &#x2211;  j    x  j
      i   =   {    1 ,    if&#xA0;  i = s ;     &#x2212; 1 ,    if&#xA0;  i = t
      ;     0 ,    &#xA0;otherwise.          {\displaystyle \sum _{j}x_{ij}-
      \sum _{j}x_{ji}={\begin{cases}1,&{\text{if }}i=s;\\-1,&{\text{if
      }}i=t;\\0,&{\text{ otherwise.}}\end{cases}}}  [\sum _{j}x_{ij}-\sum _
      {j}x_{ji}={\begin{cases}1,&{\text{if }}i=s;\\-1,&{\text{if }}i=t;\\0,&
      {\text{ otherwise.}}\end{cases}}]
The intuition behind this is that      x  i j     {\displaystyle x_{ij}}  [x_
{ij}] is an indicator variable for whether edge (i, j) is part of the shortest
path: 1 when it is, and 0 if it is not. We wish to select the set of edges with
minimal weight, subject to the constraint that this set forms a path from s to
t (represented by the equality constraint: for all vertices except s and t the
number of incoming and outcoming edges that are part of the path must be the
same (i.e., that it should be a path from s to t).
This LP has the special property that it is integral; more specifically, every
basic_optimal_solution (when one exists) has all variables equal to 0 or 1, and
the set of edges whose variables equal 1 form an s-t dipath. See Ahuja et al.
[6] for one proof, although the origin of this approach dates back to mid-20th
century.
The dual for this linear program is
      maximize yt â ys subject to for all ij, yj â yi ≤ wij
and feasible duals correspond to the concept of a consistent_heuristic for the
A*_algorithm for shortest paths. For any feasible dual y the reduced_costs
w  i j  &#x2032;  =  w  i j   &#x2212;  y  j   +  y  i     {\displaystyle w'_
{ij}=w_{ij}-y_{j}+y_{i}}  [w'_{ij}=w_{ij}-y_{j}+y_{i}] are nonnegative and A*
essentially runs Dijkstra's_algorithm on these reduced costs.
***** General algebraic framework on semirings: the algebraic path problem
[edit] *****
[[icon]] This section needs expansion. You can help by adding_to_it. (August
         2014)
Many problems can be framed as a form of the shortest path for some suitably
substituted notions of addition along a path and taking the minimum. The
general approach to these is to consider the two operations to be those of a
semiring. Semiring multiplication is done along the path, and the addition is
between paths. This general framework is known as the algebraic_path_problem.
[7][8][9]
Most of the classic shortest-path algorithms (and new ones) can be formulated
as solving linear systems over such algebraic structures.[10]
More recently, an even more general framework for solving these (and much less
obviously related problems) has been developed under the banner of valuation
algebras.[11]
***** Shortest path in stochastic time-dependent networks[edit] *****
In real-life situations, the transportation network is usually stochastic and
time-dependent. In fact, a traveler traversing a link daily may experiences
different travel times on that link due not only to the fluctuations in travel
demand (origin-destination matrix) but also due to such incidents as work
zones, bad weather conditions, accidents and vehicle breakdowns. As a result, a
stochastic time-dependent (STD) network is a more realistic representation of
an actual road network compared with the deterministic one.[12][13]
Despite considerable progress during the course of the past decade, it remains
a controversial question how an optimal path should be defined and identified
in stochastic road networks. In other words, there is no unique definition of
an optimal path under uncertainty. One possible and common answer to this
question is to find a path with the minimum expected travel time. The main
advantage of using this approach is that efficient shortest path algorithms
introduced for the deterministic networks can be readily employed to identify
the path with the minimum expected travel time in a stochastic network.
However, the resulting optimal path identified by this approach may not be
reliable, because this approach fails to address travel time variability. To
tackle this issue some researchers use distribution of travel time instead of
expected value of it so they find the probability distribution of total
travelling time using different optimization methods such as dynamic
programming and Dijkstra's_algorithm .[14] These methods use stochastic
optimization, specifically stochastic dynamic programming to find the shortest
path in networks with probabilistic arc length.[15] The concept of travel time
reliability is used interchangeably with travel time variability in the
transportation research literature, so that, in general, one can say that the
higher the variability in travel time, the lower the reliability would be, and
vice versa.
In order to account for travel time reliability more accurately, two common
alternative definitions for an optimal path under uncertainty have been
suggested. Some have introduced the concept of the most reliable path, aiming
to maximize the probability of arriving on time or earlier than a given travel
time budget. Others, alternatively, have put forward the concept of an Î±-
reliable path based on which they intended to minimize the travel time budget
required to ensure a pre-specified on-time arrival probability.
***** See also[edit] *****
    * Pathfinding
    * IEEE_802.1aq
    * Flow_network
    * Shortest_path_tree
    * Euclidean_shortest_path
    * Min-plus_matrix_multiplication
    * Bidirectional_search, an algorithm that finds the shortest path between
      two vertices on a directed graph
***** References[edit] *****
**** Notes[edit] ****
   1. ^Sanders,_Peter (March 23, 2009). "Fast_route_planning". Google Tech
      Talk.
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
   3. ^Chen, Danny Z. (December 1996). "Developing algorithms and software for
      geometric path planning problems". ACM Computing Surveys. 28 (4es).
      Article 18. doi:10.1145/242224.242246.
   4. ^ Abraham, Ittai; Fiat, Amos; Goldberg,_Andrew_V.; Werneck, Renato F.
      "Highway_Dimension,_Shortest_Paths,_and_Provably_Efficient_Algorithms".
      ACM-SIAM Symposium on Discrete Algorithms, pages 782â793, 2010.
   5. ^ Abraham, Ittai; Delling, Daniel; Goldberg,_Andrew_V.; Werneck, Renato
      F. research.microsoft.com/pubs/142356/HL-TR.pdf_"A_Hub-Based_Labeling
      Algorithm_for_Shortest_Paths_on_Road_Networks". Symposium on Experimental
      Algorithms, pages 230â241, 2011.
   6. ^Kroger, Martin (2005). "Shortest multiple disconnected path for the
      analysis of entanglements in two- and three-dimensional polymeric
      systems". Computer Physics Communications. 168 (3): 209â232. Bibcode:
      2005CoPhC.168..209K. doi:10.1016/j.cpc.2005.01.020.
   7. ^Ahuja,_Ravindra_K.; Magnanti,_Thomas_L.; Orlin,_James_B. (1993). Network
      Flows: Theory, Algorithms and Applications. Prentice Hall. ISBN 978-0-13-
      617549-0.
   8. ^Pair, Claude (1967), "Sur des algorithmes pour des problÃ¨mes de
      cheminement dans les graphes finis (On algorithms for path problems in
      finite graphs)", in Rosentiehl (ed.), ThÃ©orie des graphes (journÃ©es
      internationales d'Ã©tudes) -- Theory of Graphs (international symposium),
      Rome (Italy), July 1966: Dunod (Paris) et Gordon and Breach (New York),
      p. 271
   9. ^ Derniame, Jean Claude; Pair, Claude (1971), ProblÃ¨mes de cheminement
      dans les graphes (Path Problems in Graphs), Dunod (Paris)
  10. ^Baras, John; Theodorakopoulos, George (4 April 2010). Path_Problems_in
      Networks. Morgan & Claypool Publishers. pp. 9â. ISBN 978-1-59829-924-3.
  11. ^Gondran, Michel; Minoux, Michel (2008). Graphs, Dioids and Semirings:
      New Models and Algorithms. Springer Science & Business Media. chapter 4.
      ISBN 978-0-387-75450-5.
  12. ^Pouly, Marc; Kohlas, JÃ¼rg (2011). Generic Inference: A Unifying Theory
      for Automated Reasoning. John Wiley & Sons. Chapter 6. Valuation Algebras
      for Path Problems. ISBN 978-1-118-01086-0.
  13. ^ Loui, R.P., 1983. Optimal paths in graphs with stochastic or
      multidimensional weights. Communications of the ACM, 26(9), pp.670-676.
  14. ^Rajabi-Bahaabadi, Mojtaba; Shariat-Mohaymany, Afshin; Babaei, Mohsen;
      Ahn, Chang Wook (2015). "Multi-objective path finding in stochastic time-
      dependent road networks using non-dominated sorting genetic algorithm".
      Expert Systems with Applications. 42 (12): 5056â5064. doi:10.1016/
      j.eswa.2015.02.046.
  15. ^Olya, Mohammad Hessam (2014). "Finding shortest path in a combined
      exponential â gamma probability distribution arc length". International
      Journal of Operational Research. 21 (1): 25â37. doi:10.1504/
      IJOR.2014.064020.
  16. ^Olya, Mohammad Hessam (2014). "Applying Dijkstra's algorithm for general
      shortest path problem with normal probability distribution arc length".
      International Journal of Operational Research. 21 (2): 143â154. doi:
      10.1504/IJOR.2014.064541.
**** Bibliography[edit] ****
    * Ahuja, Ravindra K.; Mehlhorn, Kurt; Orlin, James; Tarjan,_Robert_E.
      (April 1990). "Faster_algorithms_for_the_shortest_path_problem". Journal
      of the ACM. ACM. 37 (2): 213â223. doi:10.1145/77600.77615.
Bellman,_Richard (1958). "On a routing problem". Quarterly of Applied
Mathematics. 16: 87â90. doi:10.1090/qam/102435. MR 0102435.
Cherkassky, Boris V.; Goldberg,_Andrew_V.; Radzik, Tomasz (1996). "Shortest
paths_algorithms:_theory_and_experimental_evaluation". Mathematical
Programming. Ser. A. 73 (2): 129â174. doi:10.1016/0025-5610(95)00021-6.
MR 1392160.
Cormen,_Thomas_H.; Leiserson,_Charles_E.; Rivest,_Ronald_L.; Stein,_Clifford
(2001) [1990]. "Single-Source Shortest Paths and All-Pairs Shortest Paths".
Introduction_to_Algorithms (2nd ed.). MIT Press and McGraw-Hill. pp. 580â642.
ISBN 0-262-03293-7.
Dantzig, G. B. (January 1960). "On the Shortest Route through a Network".
Management Science. 6 (2): 187â190. doi:10.1287/mnsc.6.2.187.
Derniame, Jean Claude; Pair, Claude (1971), ProblÃ¨mes de cheminement dans les
graphes (Path Problems in Graphs), Dunod (Paris)
Dijkstra,_E._W. (1959). "A note on two problems in connexion with graphs".
Numerische Mathematik. 1: 269â271. doi:10.1007/BF01386390.
Ford, L. R. (1956). "Network_Flow_Theory". Rand Corporation. P-923.
Fredman,_Michael_Lawrence; Tarjan,_Robert_E. (1984). Fibonacci heaps and their
uses in improved network optimization algorithms. 25th Annual Symposium on
Foundations of Computer Science. IEEE. pp. 338â346. doi:10.1109/
SFCS.1984.715934. ISBN 0-8186-0591-X.
Fredman,_Michael_Lawrence; Tarjan,_Robert_E. (1987). "Fibonacci heaps and their
uses in improved network optimization algorithms". Journal of the Association
for Computing Machinery. 34 (3): 596â615. doi:10.1145/28869.28874.
Gabow, H. N. (1983). "Scaling algorithms for network problems". Proceedings_of
the_24th_Annual_Symposium_on_Foundations_of_Computer_Science_(FOCS_1983) (PDF).
pp. 248â258. doi:10.1109/SFCS.1983.68.
Gabow, Harold N. (1985). "Scaling algorithms for network problems". Journal_of
Computer_and_System_Sciences. 31 (2): 148â168. doi:10.1016/0022-0000
(85)90039-X. MR 0828519.
Hagerup, Torben (2000). Montanari, Ugo; Rolim, JosÃ© D. P.; Welzl, Emo (eds.).
Improved_Shortest_Paths_on_the_Word_RAM. Proceedings of the 27th International
Colloquium on Automata, Languages and Programming. pp. 61â72. ISBN 978-3-540-
67715-4.
Johnson,_Donald_B. (1977). "Efficient algorithms for shortest paths in sparse
networks". Journal_of_the_ACM. 24 (1): 1â13. doi:10.1145/321992.321993.
Johnson,_Donald_B. (December 1981). "A priority queue in which initialization
and queue operations take O(log log D) time". Mathematical Systems Theory. 15
(1): 295â309. doi:10.1007/BF01786986. MR 0683047.
Karlsson, Rolf G.; Poblete, Patricio V. (1983). "An O(m log log D) algorithm
for shortest paths". Discrete_Applied_Mathematics. 6 (1): 91â93. doi:10.1016/
0166-218X(83)90104-X. MR 0700028.
Leyzorek, M.; Gray, R. S.; Johnson, A. A.; Ladew, W. C.; Meaker, S. R., Jr.;
Petry, R. M.; Seitz, R. N. (1957). Investigation of Model Techniques â First
Annual Report â 6 June 1956 â 1 July 1957 â A Study of Model Techniques
for Communication Systems. Cleveland, Ohio: Case Institute of Technology.
Moore,_E._F. (1959). "The shortest path through a maze". Proceedings of an
International Symposium on the Theory of Switching (Cambridge, Massachusetts,
2â5 April 1957). Cambridge: Harvard University Press. pp. 285â292.
Pettie, Seth; Ramachandran, Vijaya (2002). Computing_shortest_paths_with
comparisons_and_additions. Proceedings of the Thirteenth Annual ACM-SIAM
Symposium on Discrete Algorithms. pp. 267â276. ISBN 978-0-89871-513-2.
Pettie, Seth (26 January 2004). "A new approach to all-pairs shortest paths on
real-weighted graphs". Theoretical Computer Science. 312 (1): 47â74. doi:
10.1016/s0304-3975(03)00402-x.
Pollack, Maurice; Wiebenson, Walter (MarchâApril 1960). "Solution of the
Shortest-Route ProblemâA Review". Oper. Res. 8 (2): 224â230. doi:10.1287/
opre.8.2.224.
 Attributes Dijkstra's algorithm to Minty ("private communication") on p.225.
Schrijver, Alexander (2004). Combinatorial Optimization â Polyhedra and
Efficiency. Algorithms and Combinatorics. 24. Springer. ISBN 978-3-540-20456-5.
 Here: vol.A, sect.7.5b, p. 103
Shimbel, Alfonso (1953). "Structural parameters of communication networks".
Bulletin of Mathematical Biophysics. 15 (4): 501â507. doi:10.1007/BF02476438.
Shimbel, A. (1955). Structure in communication nets. Proceedings of the
Symposium on Information Networks. New York, NY: Polytechnic Press of the
Polytechnic Institute of Brooklyn. pp. 199â203.
Thorup, Mikkel (1999). "Undirected single-source shortest paths with positive
integer weights in linear time". Journal of the ACM. 46 (3): 362â394. doi:
10.1145/316542.316548.
Thorup, Mikkel (2004). "Integer_priority_queues_with_decrease_key_in_constant
time_and_the_single_source_shortest_paths_problem". Journal of Computer and
System Sciences. 69 (3): 330â353. doi:10.1016/j.jcss.2004.04.003.
Whiting, P. D.; Hillier, J. A. (MarchâJune 1960). "A Method for Finding the
Shortest Route through a Road Network". Operational Research Quarterly. 11 (1/
2): 37â40. doi:10.1057/jors.1960.32.
Williams,_Ryan (2014). "Faster all-pairs shortest paths via circuit
complexity". Proceedings_of_the_46th_Annual_ACM_Symposium_on_Theory_of
Computing_(STOC_'14). New York: ACM. pp. 664â673. arXiv:1312.6680. doi:
10.1145/2591796.2591811. MR 3238994.
***** Further reading[edit] *****
    * Frigioni, D.; Marchetti-Spaccamela, A.; Nanni, U. (1998). "Fully dynamic
      output bounded single source shortest path problem". Proc. 7th Annu. ACM-
      SIAM Symp. Discrete Algorithms. Atlanta, GA. pp. 212â221.
      CiteSeerX 10.1.1.32.9856.
Dreyfus, S. E. (October 1967). An_Appraisal_of_Some_Shortest_Path_Algorithms
(PDF) (Report). Project Rand. United States Air Force. RM-5433-PR.
 DTIC AD-661265.
Authority_control [Edit_this_at_Wikidata]     * GND: 4138403-9

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Shortest_path_problem&oldid=906147832"
Categories:
    * Network_theory
    * Polynomial-time_problems
    * Computational_problems_in_graph_theory
    * Edsger_W._Dijkstra
Hidden categories:
    * Articles_lacking_in-text_citations_from_June_2009
    * All_articles_lacking_in-text_citations
    * Incomplete_lists_from_February_2011
    * Incomplete_lists_from_December_2012
    * Articles_needing_additional_references_from_December_2015
    * All_articles_needing_additional_references
    * Articles_to_be_expanded_from_August_2014
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
    * Wikipedia_articles_with_GND_identifiers
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
    * Italiano
    * LietuviÅ³
    * Bahasa_Melayu
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 13 July 2019, at 23:39 (UTC).
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
