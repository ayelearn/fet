The following text has been accessed from https://en.wikipedia.org/wiki/Minimum_spanning_tree at Fri Aug 9 01:09:45 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Minimum spanning tree ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
data structure, subgraph of a weighted graph
A planar_graph and its minimum spanning tree. Each edge is labeled with its
weight, which here is roughly proportional to its length.
A minimum spanning tree (MST) or minimum weight spanning tree is a subset of
the edges of a connected, edge-weighted undirected graph that connects all the
vertices together, without any cycles and with the minimum possible total edge
weight. That is, it is a spanning_tree whose sum of edge weights is as small as
possible. More generally, any edge-weighted undirected graph (not necessarily
connected) has a minimum spanning forest, which is a union of the minimum
spanning trees for its connected_components.
There are quite a few use cases for minimum spanning trees. One example would
be a telecommunications company trying to lay cable in a new neighborhood. If
it is constrained to bury the cable only along certain paths (e.g. roads), then
there would be a graph containing the points (e.g. houses) connected by those
paths. Some of the paths might be more expensive, because they are longer, or
require the cable to be buried deeper; these paths would be represented by
edges with larger weights. Currency is an acceptable unit for edge weight –
there is no requirement for edge lengths to obey normal rules of geometry such
as the triangle_inequality. A spanning tree for that graph would be a subset of
those paths that has no cycles but still connects every house; there might be
several spanning trees possible. A minimum spanning tree would be one with the
lowest total cost, representing the least expensive path for laying the cable.
⁰
***** Contents *****
    * 1_Properties
          o 1.1_Possible_multiplicity
          o 1.2_Uniqueness
          o 1.3_Minimum-cost_subgraph
          o 1.4_Cycle_property
          o 1.5_Cut_property
          o 1.6_Minimum-cost_edge
          o 1.7_Contraction
    * 2_Algorithms
          o 2.1_Classic_algorithms
          o 2.2_Faster_algorithms
          o 2.3_Linear-time_algorithms_in_special_cases
                # 2.3.1_Dense_graphs
                # 2.3.2_Integer_weights
          o 2.4_Decision_trees
          o 2.5_Optimal_algorithm
          o 2.6_Parallel_and_distributed_algorithms
    * 3_MST_on_complete_graphs
    * 4_Applications
    * 5_Related_problems
    * 6_References
    * 7_Further_reading
    * 8_External_links
***** Properties[edit] *****
**** Possible multiplicity[edit] ****
If there are n vertices in the graph, then each spanning tree has n − 1 edges.
This figure shows there may be more than one minimum spanning tree in a graph.
In the figure, the two trees below the graph are two possibilities of minimum
spanning tree of the given graph.
There may be several minimum spanning trees of the same weight; in particular,
if all the edge weights of a given graph are the same, then every spanning tree
of that graph is minimum.
**** Uniqueness[edit] ****
If each edge has a distinct weight then there will be only one, unique minimum
spanning tree. This is true in many realistic situations, such as the
telecommunications company example above, where it's unlikely any two paths
have exactly the same cost. This generalizes to spanning forests as well.
Proof:
   1. Assume_the_contrary, that there are two different MSTs A and B.
   2. Since A and B differ despite containing the same nodes, there is at least
      one edge that belongs to one but not the other. Among such edges, let e1
      be the one with least weight; this choice is unique because the edge
      weights are all distinct. Without loss of generality, assume e1 is in A.
   3. As B is an MST, {e1}     &#x222A;   {\displaystyle \cup }  [\cup ] B must
      contain a cycle C with e1.
   4. As a tree, A contains no cycles, therefore C must have an edge e2 that is
      not in A.
   5. Since e1 was chosen as the unique lowest-weight edge among those
      belonging to exactly one of A and B, the weight of e2 must be greater
      than the weight of e1.
   6. As e1 and e2 are part of the cycle C, replacing e2 with e1 in B therefore
      yields a spanning tree with a smaller weight.
   7. This contradicts the assumption that B is a MST.
More generally, if the edge weights are not all distinct then only the (multi-
)set of weights in minimum spanning trees is certain to be unique; it is the
same for all minimum spanning trees.[1]
**** Minimum-cost subgraph[edit] ****
If the weights are positive, then a minimum spanning tree is in fact a minimum-
cost subgraph connecting all vertices, since subgraphs containing cycles
necessarily have more total weight.
**** Cycle property[edit] ****
For any cycle C in the graph, if the weight of an edge e of C is larger than
the individual weights of all other edges of C, then this edge cannot belong to
an MST.
Proof: Assume_the_contrary, i.e. that e belongs to an MST T1. Then deleting e
will break T1 into two subtrees with the two ends of e in different subtrees.
The remainder of C reconnects the subtrees, hence there is an edge f of C with
ends in different subtrees, i.e., it reconnects the subtrees into a tree T2
with weight less than that of T1, because the weight of f is less than the
weight of e.
**** Cut property[edit] ****
This figure shows the cut property of MSTs. T is the only MST of the given
graph. If S = {A,B,D,E}, thus V-S = {C,F}, then there are 3 possibilities of
the edge across the cut(S,V-S), they are edges BC, EC, EF of the original
graph. Then, e is one of the minimum-weight-edge for the cut, therefore S âª
{e} is part of the MST T.
For any cutCof the graph, if the weight of an edgeein the cut-set ofCis
strictly smaller than the weights of all other edges of the cut-set ofC, then
this edge belongs to all MSTs of the graph.
Proof: Assume that there is an MST T that does not contain e. Adding e to T
will produce a cycle, that crosses the cut once at e and crosses back at
another edge e'. Deleting e' we get a spanning tree Tâ{e'}âª{e} of strictly
smaller weight than T. This contradicts the assumption that T was a MST.
By a similar argument, if more than one edge is of minimum weight across a cut,
then each such edge is contained in some minimum spanning tree.
**** Minimum-cost edge[edit] ****
If the minimum cost edgeeof a graph is unique, then this edge is included in
any MST.
Proof: if e was not included in the MST, removing any of the (larger cost)
edges in the cycle formed after adding e to the MST, would yield a spanning
tree of smaller weight.
**** Contraction[edit] ****
If T is a tree of MST edges, then we cancontractT into a single vertex while
maintaining the invariant that the MST of the contracted graph plus T gives the
MST for the graph before contraction.[2]
***** Algorithms[edit] *****
In all of the algorithms below, m is the number of edges in the graph and n is
the number of vertices.
**** Classic algorithms[edit] ****
The first algorithm for finding a minimum spanning tree was developed by Czech
scientist Otakar_BorÅ¯vka in 1926 (see BorÅ¯vka's_algorithm). Its purpose was
an efficient electrical coverage of Moravia. The algorithm proceeds in a
sequence of stages. In each stage, called Boruvka step, it identifies a forest
F consisting of the minimum-weight edge incident to each vertex in the graph G,
then forms the graph      G  1   = G &#x2216; F   {\displaystyle G_
{1}=G\setminus F}  [{\displaystyle G_{1}=G\setminus F}] as the input to the
next step. Here     G &#x2216; F   {\displaystyle G\setminus F}  [
{\displaystyle G\setminus F}] denotes the graph derived from G by contracting
edges in F (by the Cut_property, these edges belong to the MST). Each Boruvka
step takes linear time. Since the number of vertices is reduced by at least
half in each step, Boruvka's algorithm takes O(m log n) time.[2]
A second algorithm is Prim's_algorithm, which was invented by VojtÄch_JarnÃ­k
in 1930 and rediscovered by Prim in 1957 and Dijkstra in 1959. Basically, it
grows the MST (T) one edge at a time. Initially, T contains an arbitrary
vertex. In each step, T is augmented with a least-weight edge (x,y) such that x
is in T and y is not yet in T. By the Cut_property, all edges added to T are in
the MST. Its run-time is either O(m log n) or O(m + n log n), depending on the
data-structures used.
A third algorithm commonly in use is Kruskal's_algorithm, which also takes O(m
log n) time.
A fourth algorithm, not as commonly used, is the reverse-delete_algorithm,
which is the reverse of Kruskal's algorithm. Its runtime is O(m log n (log log
n)3).
All these four are greedy_algorithms. Since they run in polynomial time, the
problem of finding such trees is in FP, and related decision_problems such as
determining whether a particular edge is in the MST or determining if the
minimum total weight exceeds a certain value are in P.
**** Faster algorithms[edit] ****
Several researchers have tried to find more computationally-efficient
algorithms.
In a comparison model, in which the only allowed operations on edge weights are
pairwise comparisons, Karger,_Klein_&_Tarjan_(1995) found a linear_time
randomized_algorithm based on a combination of BorÅ¯vka's algorithm and the
reverse-delete algorithm.[3][4]
The fastest non-randomized comparison-based algorithm with known complexity, by
Bernard_Chazelle, is based on the soft_heap, an approximate priority queue.[5]
[6] Its running time is O(m Î±(m,n)), where Î± is the classical functional
inverse_of_the_Ackermann_function. The function Î± grows extremely slowly, so
that for all practical purposes it may be considered a constant no greater than
4; thus Chazelle's algorithm takes very close to linear time.
**** Linear-time algorithms in special cases[edit] ****
*** Dense graphs[edit] ***
If the graph is dense (i.e. m/n â¥ log log log n), then a deterministic
algorithm by Fredman and Tarjan finds the MST in time O(m).[7] The algorithm
executes a number of phases. Each phase executes Prim's_algorithm many times,
each for a limited number of steps. The run-time of each phase is O(m+n). If
the number of vertices before a phase is      n &#x2032;    {\displaystyle n'}
[n'], the number of vertices remaining after a phase is at most      n &#x2032;
/   2  m  /   n &#x2032;      {\displaystyle n'/2^{m/n'}}  [n'/2^{m/n'}].
Hence, at most      log  &#x2217;   &#x2061;  n    {\displaystyle \log ^{*}{n}}
[{\displaystyle \log ^{*}{n}}] phases are needed, which gives a linear run-time
for dense graphs.[2]
There are other algorithms that work in linear time on dense graphs.[5][8]
*** Integer weights[edit] ***
If the edge weights are integers represented in binary, then deterministic
algorithms are known that solve the problem in O(m + n) integer operations.[9]
Whether the problem can be solved deterministically for a general graph in
linear time by a comparison-based algorithm remains an open question.
**** Decision trees[edit] ****
Given graph G where the nodes and edges are fixed but the weights are unknown,
it is possible to construct a binary decision_tree (DT) for calculating the MST
for any permutation of weights. Each internal node of the DT contains a
comparison between two edges, e.g. "Is the weight of the edge between x and y
larger than the weight of the edge between w and z?". The two children of the
node correspond to the two possible answers "yes" or "no". In each leaf of the
DT, there is a list of edges from G that correspond to an MST. The runtime
complexity of a DT is the largest number of queries required to find the MST,
which is just the depth of the DT. A DT for a graph G is called optimal if it
has the smallest depth of all correct DTs for G.
For every integer r, it is possible to find optimal decision trees for all
graphs on r vertices by brute-force_search. This search proceeds in two steps.
A. Generating all potential DTs
    * There are      2    (   r 2   )       {\displaystyle 2^{r \choose 2}}
      [2^{{r \choose 2}}] different graphs on r vertices.
    * For each graph, an MST can always be found using r(r-1) comparisons, e.g.
      by Prim's_algorithm.
    * Hence, the depth of an optimal DT is less than      r  2
      {\displaystyle r^{2}}  [r^{2}].
    * Hence, the number of internal nodes in an optimal DT is less than      2
      r  2       {\displaystyle 2^{r^{2}}}  [2^{r^{2}}].
    * Every internal node compares two edges. The number of edges is at most
      r  2     {\displaystyle r^{2}}  [r^{2}] so the different number of
      comparisons is at most      r  4     {\displaystyle r^{4}}  [r^{4}].
    * Hence, the number of potential DTs is less than:       (  r  4   )   (  2
      r  2     )   =  r   2  (  r  2   + 2 )       {\displaystyle {(r^{4})}^{
      (2^{r^{2}})}=r^{2^{(r^{2}+2)}}}  [{(r^{4})}^{(2^{r^{2}})}=r^{2^{(r^
      {2}+2)}}].
B. Identifying the correct DTs To check if a DT is correct, it should be
checked on all possible permutations of the edge weights.
    * The number of such permutations is at most     (  r  2   ) !
      {\displaystyle (r^{2})!}  [(r^{2})!].
    * For each permutation, solve the MST problem on the given graph using any
      existing algorithm, and compare the result to the answer given by the DT.
    * The running time of any MST algorithm is at most     (  r  2   )
      {\displaystyle (r^{2})}  [(r^{2})], so the total time required to check
      all permutations is at most     (  r  2   + 1 ) !   {\displaystyle (r^
      {2}+1)!}  [(r^{2}+1)!].
Hence, the total time required for finding an optimal DT for all graphs with r
vertices is:      2    (   r 2   )     &#x22C5;  r   2  (  r  2   + 2 )
&#x22C5; (  r  2   + 1 ) !   {\displaystyle 2^{r \choose 2}\cdot r^{2^{(r^
{2}+2)}}\cdot (r^{2}+1)!}  [2^{r \choose 2}\cdot r^{2^{(r^{2}+2)}}\cdot (r^
{2}+1)!], which is less than:      2   2   r  2   + o ( r )
{\displaystyle 2^{2^{r^{2}+o(r)}}}  [2^{2^{r^{2}+o(r)}}].[2]
See also: Decision_tree_model
**** Optimal algorithm[edit] ****
Seth Pettie and Vijaya Ramachandran have found a provably optimal deterministic
comparison-based minimum spanning tree algorithm.[2] The following is a
simplified description of the algorithm.
   1. Let     r = log &#x2061; log &#x2061; log &#x2061; n   {\displaystyle
      r=\log \log \log n}  [r=\log \log \log n], where n is the number of
      vertices. Find all optimal decision trees on r vertices. This can be done
      in time O(n) (see Decision_trees above).
   2. Partition the graph to components with at most r vertices in each
      component. This partition can be done in time O(m).
   3. Use the optimal decision trees to find an MST for each component.
   4. Contract each connected component spanned by the MSTs to a single vertex.
   5. It is possible to prove that the resulting graph has at most n/
      r vertices. Hence, the graph is dense and we can use any algorithm which
      works on Dense_graphs in time O(m).
The runtime of all steps in the algorithm is O(m), except for the step of using
the decision trees. We don't know the runtime of this step, but we know that it
is optimal - no algorithm can do better than the optimal decision tree.
Thus, this algorithm has the peculiar property that it is provably optimal
although its runtime complexity is unknown.
**** Parallel and distributed algorithms[edit] ****
Research has also considered parallel_algorithms for the minimum spanning tree
problem. With a linear number of processors it is possible to solve the problem
in     O ( log &#x2061; n )   {\displaystyle O(\log n)}  [O(\log n)] time.[10]
[11] Bader_&_Cong_(2006) demonstrate an algorithm that can compute MSTs 5 times
faster on 8 processors than an optimized sequential algorithm.[12]
Other specialized algorithms have been designed for computing minimum spanning
trees of a graph so large that most of it must be stored on disk at all times.
These external storage algorithms, for example as described in "Engineering an
External Memory Minimum Spanning Tree Algorithm" by Roman, Dementiev et al.,
[13] can operate, by authors' claims, as little as 2 to 5 times slower than a
traditional in-memory algorithm. They rely on efficient external_storage
sorting_algorithms and on graph_contraction techniques for reducing the graph's
size efficiently.
The problem can also be approached in a distributed_manner. If each node is
considered a computer and no node knows anything except its own connected
links, one can still calculate the distributed_minimum_spanning_tree.
***** MST on complete graphs[edit] *****
Alan_M._Frieze showed that given a complete_graph on n vertices, with edge
weights that are independent identically distributed random variables with
distribution function     F   {\displaystyle F}  [F] satisfying      F &#x2032;
( 0 ) > 0   {\displaystyle F'(0)>0}  [F'(0)>0], then as n approaches +â the
expected weight of the MST approaches     &#x03B6; ( 3 )  /   F &#x2032;  ( 0 )
{\displaystyle \zeta (3)/F'(0)}  [\zeta (3)/F'(0)], where     &#x03B6;
{\displaystyle \zeta }  [\zeta ] is the Riemann_zeta_function. Frieze and
Steele also proved convergence in probability. Svante_Janson proved a central
limit_theorem for weight of the MST.
For uniform random weights in     [ 0 , 1 ]   {\displaystyle [0,1]}  [[0,1]],
the exact expected size of the minimum spanning tree has been computed for
small complete graphs.[14]
Vertices Expected size               Approximate expected size
2        1 / 2                       0.5
3        3 / 4                       0.75
4        31 / 35                     0.8857143
5        893 / 924                   0.9664502
6        278 / 273                   1.0183151
7        30739 / 29172               1.053716
8        199462271 / 184848378       1.0790588
9        126510063932 / 115228853025 1.0979027
***** Applications[edit] *****
Minimum spanning trees have direct applications in the design of networks,
including computer_networks, telecommunications_networks, transportation
networks, water_supply_networks, and electrical_grids (which they were first
invented for, as mentioned above).[15] They are invoked as subroutines in
algorithms for other problems, including the Christofides_algorithm for
approximating the traveling_salesman_problem,[16] approximating the multi-
terminal minimum cut problem (which is equivalent in the single-terminal case
to the maximum_flow_problem),[17] and approximating the minimum-cost weighted
perfect matching.[18]
Other practical applications based on minimal spanning trees include:
    * Taxonomy.[19]
    * Cluster_analysis: clustering points in the plane,[20] single-linkage
      clustering (a method of hierarchical_clustering),[21] graph-theoretic
      clustering,[22] and clustering gene_expression data.[23]
    * Constructing trees for broadcasting in computer networks.[24]
    * Image_registration[25] and segmentation[26] – see minimum_spanning_tree-
      based_segmentation.
    * Curvilinear feature_extraction in computer_vision.[27]
    * Handwriting_recognition of mathematical expressions.[28]
    * Circuit_design: implementing efficient multiple constant multiplications,
      as used in finite_impulse_response filters.[29]
    * Regionalisation of socio-geographic areas, the grouping of areas into
      homogeneous, contiguous regions.[30]
    * Comparing ecotoxicology data.[31]
    * Topological observability in power systems.[32]
    * Measuring homogeneity of two-dimensional materials.[33]
    * Minimax process_control.[34]
    * Minimum spanning trees can also be used to describe financial markets.
      [35][36] A correlation matrix can be created by calculating a coefficient
      of correlation between any two stocks. This matrix can be represented
      topologically as a complex network and a minimum spanning tree can be
      constructed to visualize relationships.
***** Related problems[edit] *****
The problem of finding the Steiner_tree of a subset of the vertices, that is,
minimum tree that spans the given subset, is known to be NP-Complete.[37]
A related problem is the k-minimum_spanning_tree (k-MST), which is the tree
that spans some subset of k vertices in the graph with minimum weight.
A set of k-smallest spanning trees is a subset of k spanning trees (out of all
possible spanning trees) such that no spanning tree outside the subset has
smaller weight.[38][39][40] (Note that this problem is unrelated to the k-
minimum spanning tree.)
The Euclidean_minimum_spanning_tree is a spanning tree of a graph with edge
weights corresponding to the Euclidean distance between vertices which are
points in the plane (or space).
The rectilinear_minimum_spanning_tree is a spanning tree of a graph with edge
weights corresponding to the rectilinear_distance between vertices which are
points in the plane (or space).
In the distributed_model, where each node is considered a computer and no node
knows anything except its own connected links, one can consider distributed
minimum_spanning_tree. The mathematical definition of the problem is the same
but there are different approaches for a solution.
The capacitated_minimum_spanning_tree is a tree that has a marked node (origin,
or root) and each of the subtrees attached to the node contains no more than a
c nodes. c is called a tree capacity. Solving CMST optimally is NP-hard,[41]
but good heuristics such as Esau-Williams and Sharma produce solutions close to
optimal in polynomial time.
The degree_constrained_minimum_spanning_tree is a minimum spanning tree in
which each vertex is connected to no more than d other vertices, for some given
number d. The case d = 2 is a special case of the traveling_salesman_problem,
so the degree constrained minimum spanning tree is NP-hard in general.
For directed_graphs, the minimum spanning tree problem is called the
Arborescence problem and can be solved in quadratic time using the ChuâLiu/
Edmonds_algorithm.
A maximum spanning tree is a spanning tree with weight greater than or equal to
the weight of every other spanning tree. Such a tree can be found with
algorithms such as Prim's or Kruskal's after multiplying the edge weights by -
1 and solving the MST problem on the new graph. A path in the maximum spanning
tree is the widest_path in the graph between its two endpoints: among all
possible paths, it maximizes the weight of the minimum-weight edge.[42] Maximum
spanning trees find applications in parsing algorithms for natural_languages
[43] and in training algorithms for conditional_random_fields.
The dynamic MST problem concerns the update of a previously computed MST after
an edge weight change in the original graph or the insertion/deletion of a
vertex.[44][45][46]
The minimum labeling spanning tree problem is to find a spanning tree with
least types of labels if each edge in a graph is associated with a label from a
finite label set instead of a weight.[47]
A bottleneck edge is the highest weighted edge in a spanning tree. A spanning
tree is a minimum_bottleneck_spanning_tree (or MBST) if the graph does not
contain a spanning tree with a smaller bottleneck edge weight. A MST is
necessarily a MBST (provable by the cut_property), but a MBST is not
necessarily a MST.[48][49]
***** References[edit] *****
   1. ^"Do_the_minimum_spanning_trees_of_a_weighted_graph_have_the_same_number
      of_edges_with_a_given_weight?". cs.stackexchange.com. Retrieved 4 April
      2018.
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
   3. ^ a b c d ePettie, Seth; Ramachandran, Vijaya (2002), "An optimal minimum
      spanning tree algorithm", Journal_of_the_Association_for_Computing
      Machinery, 49 (1): 16â34, doi:10.1145/505241.505243, MR 2148431
   4. .
   5. ^Karger,_David_R.; Klein, Philip N.; Tarjan,_Robert_E. (1995), "A
      randomized linear-time algorithm to find minimum spanning trees", Journal
      of_the_Association_for_Computing_Machinery, 42 (2): 321â328, doi:
      10.1145/201019.201022, MR 1409738
   6. ^Pettie, Seth; Ramachandran, Vijaya (2002), "Minimizing randomness in
      minimum spanning tree, parallel connectivity, and set maxima algorithms",
      Proc._13th_ACM-SIAM_Symposium_on_Discrete_Algorithms_(SODA_'02), San
      Francisco, California, pp. 713â722
   7. .
   8. ^ a bChazelle,_Bernard (2000), "A minimum spanning tree algorithm with
      inverse-Ackermann type complexity", Journal_of_the_Association_for
      Computing_Machinery, 47 (6): 1028â1047, doi:10.1145/355541.355562,
      MR 1866456
   9. .
  10. ^Chazelle,_Bernard (2000), "The_soft_heap:_an_approximate_priority_queue
      with_optimal_error_rate" (PDF), Journal_of_the_Association_for_Computing
      Machinery, 47 (6): 1012â1027, doi:10.1145/355541.355554, MR 1866455
  11. .
  12. ^Fredman, M. L.; Tarjan, R. E. (1987). "Fibonacci heaps and their uses in
      improved network optimization algorithms". Journal of the ACM. 34 (3):
      596. doi:10.1145/28869.28874.
  13. ^Gabow, H. N.; Galil, Z.; Spencer, T.; Tarjan, R. E. (1986). "Efficient
      algorithms for finding minimum spanning trees in undirected and directed
      graphs". Combinatorica. 6 (2): 109. doi:10.1007/bf02579168.
  14. ^Fredman,_M._L.; Willard,_D._E. (1994), "Trans-dichotomous algorithms for
      minimum spanning trees and shortest paths", Journal_of_Computer_and
      System_Sciences, 48 (3): 533â551, doi:10.1016/S0022-0000(05)80064-9,
      MR 1279413
  15. .
  16. ^Chong, Ka Wong; Han, Yijie; Lam, Tak Wah (2001), "Concurrent threads and
      optimal parallel minimum spanning trees algorithm", Journal_of_the
      Association_for_Computing_Machinery, 48 (2): 297â323, doi:10.1145/
      375827.375847, MR 1868718
  17. .
  18. ^Pettie, Seth; Ramachandran, Vijaya (2002), "A_randomized_time-work
      optimal_parallel_algorithm_for_finding_a_minimum_spanning_forest" (PDF),
      SIAM_Journal_on_Computing, 31 (6): 1879â1895, doi:10.1137/
      S0097539700371065, MR 1954882
  19. .
  20. ^Bader,_David_A.; Cong, Guojing (2006), "Fast shared-memory algorithms
      for computing the minimum spanning forest of sparse graphs", Journal of
      Parallel and Distributed Computing, 66 (11): 1366â1378, doi:10.1016/
      j.jpdc.2006.06.001
  21. .
  22. ^Dementiev, Roman; Sanders, Peter; Schultes, Dominik; Sibeyn, Jop F.
      (2004), "Engineering an external memory minimum spanning tree algorithm",
      Proc._IFIP_18th_World_Computer_Congress,_TC1_3rd_International_Conference
      on_Theoretical_Computer_Science_(TCS2004) (PDF), pp. 195â208
  23. .
  24. ^Steele,_J._Michael (2002), "Minimal spanning trees for graphs with
      random edge lengths", Mathematics and computer science, II (Versailles,
      2002), Trends Math., Basel: BirkhÃ¤user, pp. 223â245, MR 1940139
  25. ^Graham,_R._L.; Hell,_Pavol (1985), "On the history of the minimum
      spanning tree problem", Annals of the History of Computing, 7 (1):
      43â57, doi:10.1109/MAHC.1985.10011, MR 0783327
  26. ^ Nicos Christofides, Worst-case_analysis_of_a_new_heuristic_for_the
      travelling_salesman_problem, Report 388, Graduate School of Industrial
      Administration, CMU, 1976.
  27. ^Dahlhaus, E.; Johnson,_D._S.; Papadimitriou,_C._H.; Seymour,_P._D.;
      Yannakakis,_M. (August 1994). "The_complexity_of_multiterminal_cuts"
      (PDF). SIAM_Journal_on_Computing. 23 (4): 864â894. doi:10.1137/
      S0097539792225297. Archived from the_original (PDF) on 24 August 2004.
      Retrieved 17 December 2012.
  28. ^Supowit, Kenneth J.; Plaisted, David A.; Reingold, Edward M. (1980).
      Heuristics_for_weighted_perfect_matching. 12th Annual ACM Symposium on
      Theory of Computing (STOC '80). New York, NY, USA: ACM. pp. 398â419.
      doi:10.1145/800141.804689.
  29. ^Sneath, P. H. A. (1 August 1957). "The Application of Computers to
      Taxonomy". Journal of General Microbiology. 17 (1): 201â226. doi:
      10.1099/00221287-17-1-201. PMID 13475686.
  30. ^Asano,_T.; Bhattacharya, B.; Keil, M.; Yao,_F. (1988). Clustering
      algorithms based on minimum and maximum spanning trees. Fourth Annual
      Symposium on Computational Geometry (SCG '88). 1. pp. 252â257. doi:
      10.1145/73393.73419.
  31. ^Gower, J. C.; Ross, G. J. S. (1969). "Minimum Spanning Trees and Single
      Linkage Cluster Analysis". Journal of the Royal Statistical Society. C
      (Applied Statistics). 18 (1): 54â64. doi:10.2307/2346439.
      JSTOR 2346439.
  32. ^PÃ¤ivinen, Niina (1 May 2005). "Clustering with a minimum spanning tree
      of scale-free-like structure". Pattern Recognition Letters. 26 (7):
      921â930. doi:10.1016/j.patrec.2004.09.039.
  33. ^Xu, Y.; Olman, V.; Xu, D. (1 April 2002). "Clustering gene expression
      data using a graph-theoretic approach: an application of minimum spanning
      trees". Bioinformatics. 18 (4): 536â545. doi:10.1093/bioinformatics/
      18.4.536. PMID 12016051.
  34. ^Dalal, Yogen K.; Metcalfe, Robert M. (1 December 1978). "Reverse path
      forwarding of broadcast packets". Communications of the ACM. 21 (12):
      1040â1048. doi:10.1145/359657.359665.
  35. ^Ma, B.; Hero, A.; Gorman, J.; Michel, O. (2000). Image_registration_with
      minimum_spanning_tree_algorithm (PDF). International Conference on Image
      Processing. 1. pp. 481â484. doi:10.1109/ICIP.2000.901000.
  36. ^ P. Felzenszwalb, D. Huttenlocher: Efficient Graph-Based Image
      Segmentation. IJCV 59(2) (September 2004)
  37. ^Suk, Minsoo; Song, Ohyoung (1 June 1984). "Curvilinear feature
      extraction using minimum spanning trees". Computer Vision, Graphics, and
      Image Processing. 26 (3): 400â411. doi:10.1016/0734-189X(84)90221-4.
  38. ^Tapia, Ernesto; Rojas, RaÃºl (2004). "Recognition_of_On-line_Handwritten
      Mathematical_Expressions_Using_a_Minimum_Spanning_Tree_Construction_and
      Symbol_Dominance" (PDF). Graphics Recognition. Recent Advances and
      Perspectives. Lecture Notes in Computer Science. 3088. Berlin Heidelberg:
      Springer-Verlag. pp. 329â340. ISBN 978-3540224785.
  39. ^Ohlsson, H. (2004). Implementation of low complexity FIR filters using a
      minimum spanning tree. 12th IEEE Mediterranean Electrotechnical
      Conference (MELECON 2004). 1. pp. 261â264. doi:10.1109/
      MELCON.2004.1346826.
  40. ^AssunÃÃ£o, R. M.; M. C. Neves; G. CÃ¢mara; C. Da Costa Freitas (2006).
      "Efficient regionalization techniques for socioâeconomic geographical
      units using minimum spanning trees". International Journal of
      Geographical Information Science. 20 (7): 797â811. doi:10.1080/
      13658810600665111.
  41. ^Devillers, J.; Dore, J.C. (1 April 1989). "Heuristic potency of the
      minimum spanning tree (MST) method in toxicology". Ecotoxicology and
      Environmental Safety. 17 (2): 227â235. doi:10.1016/0147-6513(89)90042-
      0. PMID 2737116.
  42. ^Mori, H.; Tsuzuki, S. (1 May 1991). "A fast method for topological
      observability analysis using a minimum spanning tree technique". IEEE
      Transactions on Power Systems. 6 (2): 491â500. doi:10.1109/59.76691.
  43. ^Filliben, James J.; Kafadar,_Karen; Shier, Douglas R. (1 January 1983).
      "Testing for homogeneity of two-dimensional surfaces". Mathematical
      Modelling. 4 (2): 167â189. doi:10.1016/0270-0255(83)90026-X.
  44. ^Kalaba, Robert E. (1963), Graph_Theory_and_Automatic_Control (PDF)
  45. ^ Mantegna, R. N. (1999). Hierarchical_structure_in_financial_markets.
      The European Physical Journal B-Condensed Matter and Complex Systems, 11
      (1), 193-197.
  46. ^ Djauhari, M., & Gan, S. (2015). Optimality_problem_of_network_topology
      in_stocks_market_analysis. Physica A: Statistical Mechanics and Its
      Applications, 419, 108-114.
  47. ^Garey,_Michael_R.; Johnson,_David_S. (1979), Computers_and
      Intractability:_A_Guide_to_the_Theory_of_NP-Completeness, W. H. Freeman,
      ISBN 0-7167-1045-5
  48. . ND12
  49. ^Gabow, Harold N. (1977), "Two algorithms for generating weighted
      spanning trees in order", SIAM_Journal_on_Computing, 6 (1): 139â150,
      doi:10.1137/0206011, MR 0441784
  50. .
  51. ^Eppstein,_David (1992), "Finding the k smallest spanning trees", BIT, 32
      (2): 237â248, doi:10.1007/BF01994879, MR 1172188
  52. .
  53. ^Frederickson, Greg N. (1997), "Ambivalent_data_structures_for_dynamic_2-
      edge-connectivity_and_k_smallest_spanning_trees", SIAM_Journal_on
      Computing, 26 (2): 484â538, doi:10.1137/S0097539792226825, MR 1438526
  54. .
  55. ^Jothi, Raja; Raghavachari, Balaji (2005), "Approximation Algorithms for
      the Capacitated Minimum Spanning Tree Problem and Its Variants in Network
      Design", ACM Trans. Algorithms, 1 (2): 265â282, doi:10.1145/
      1103963.1103967
  56. ^Hu, T. C. (1961), "The maximum capacity route problem", Operations
      Research, 9 (6): 898â900, doi:10.1287/opre.9.6.898, JSTOR 167055
  57. .
  58. ^McDonald, Ryan; Pereira, Fernando; Ribarov, Kiril; HajiÄ, Jan (2005).
      "Non-projective_dependency_parsing_using_spanning_tree_algorithms" (PDF).
      Proc. HLT/EMNLP.
  59. ^Spira, P. M.; Pan, A. (1975), "On_finding_and_updating_spanning_trees
      and_shortest_paths" (PDF), SIAM Journal on Computing, 4 (3): 375â380,
      doi:10.1137/0204032, MR 0378466
  60. .
  61. ^Holm, Jacob; de Lichtenberg, Kristian; Thorup,_Mikkel (2001), "Poly-
      logarithmic deterministic fully dynamic algorithms for connectivity,
      minimum spanning tree, 2-edge, and biconnectivity", Journal_of_the
      Association_for_Computing_Machinery, 48 (4): 723â760, doi:10.1145/
      502090.502095, MR 2144928
  62. .
  63. ^Chin, F.; Houck, D. (1978), "Algorithms for updating minimal spanning
      trees", Journal_of_Computer_and_System_Sciences, 16 (3): 333â344, doi:
      10.1016/0022-0000(78)90022-3
  64. .
  65. ^Chang, R.S.; Leu, S.J. (1997), "The minimum labeling spanning trees",
      Information_Processing_Letters, 63 (5): 277â282, doi:10.1016/s0020-0190
      (97)00127-0
  66. .
  67. ^"Everything_about_Bottleneck_Spanning_Tree". flashing-
      thoughts.blogspot.ru. Retrieved 4 April 2018.
  68. ^ http://pages.cpsc.ucalgary.ca/~dcatalin/413/t4.pdf
***** Further reading[edit] *****
    * Otakar_Boruvka_on_Minimum_Spanning_Tree_Problem_(translation_of_the_both
      1926_papers,_comments,_history)_(2000) Jaroslav_NeÅ¡etÅil, Eva MilkovÃ¡,
      Helena NesetrilovÃ¡. (Section 7 gives his algorithm, which looks like a
      cross between Prim's and Kruskal's.)
    * Thomas_H._Cormen, Charles_E._Leiserson, Ronald_L._Rivest, and Clifford
      Stein. Introduction_to_Algorithms, Second Edition. MIT Press and McGraw-
      Hill, 2001.
ISBN 0-262-03293-7. Chapter 23: Minimum Spanning Trees, pp. 561–579.
Eisner, Jason (1997). State-of-the-art_algorithms_for_minimum_spanning_trees:_A
tutorial_discussion. Manuscript, University of Pennsylvania, April. 78 pp.
Kromkowski, John David. "Still Unmelted after All These Years", in Annual
Editions, Race and Ethnic Relations, 17/e (2009 McGraw Hill) (Using minimum
spanning tree as method of demographic analysis of ethnic diversity across the
United States).
***** External links[edit] *****
 Wikimedia Commons has media related to Minimum_spanning_trees.
    * Implemented_in_BGL,_the_Boost_Graph_Library
    * The_Stony_Brook_Algorithm_Repository_-_Minimum_Spanning_Tree_codes
    * Implemented_in_QuickGraph_for_.Net

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Minimum_spanning_tree&oldid=907259173"
Categories:
    * Spanning_tree
    * Polynomial-time_problems
Hidden categories:
    * Use_American_English_from_April_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * Commons_category_link_is_on_Wikidata
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
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Svenska
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 21 July 2019, at 17:21 (UTC).
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
