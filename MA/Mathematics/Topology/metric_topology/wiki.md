The following text has been accessed from https://en.wikipedia.org/wiki/Metric_space at Fri Aug 9 02:34:22 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Metric space ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, a metric space is a set together with a metric_on_the_set. The
metric is a function that defines a concept of distance between any two members
of the set, which are usually called points. The metric satisfies a few simple
properties. Informally:
    * the distance from a point to itself is zero,
    * the distance between two distinct points is positive,
    * the distance from A to B is the same as the distance from B to A, and
    * the distance from A to B (directly) is less than or equal to the distance
      from A to B via any third point C.
A metric on a space induces topological_properties like open and closed_sets,
which lead to the study of more abstract topological_spaces.
The most familiar metric space is 3-dimensional_Euclidean_space. In fact, a
"metric" is the generalization of the Euclidean_metric arising from the four
long-known properties of the Euclidean distance. The Euclidean metric defines
the distance between two points as the length of the straight line_segment
connecting them. Other metric spaces occur for example in elliptic_geometry and
hyperbolic_geometry, where distance on a sphere measured by angle is a metric,
and the hyperboloid_model of hyperbolic geometry is used by special_relativity
as a metric space of velocities.
⁰
***** Contents *****
    * 1_History
    * 2_Definition
    * 3_Examples_of_metric_spaces
    * 4_Open_and_closed_sets,_topology_and_convergence
    * 5_Types_of_metric_spaces
          o 5.1_Complete_spaces
          o 5.2_Bounded_and_totally_bounded_spaces
          o 5.3_Compact_spaces
          o 5.4_Locally_compact_and_proper_spaces
          o 5.5_Connectedness
          o 5.6_Separable_spaces
          o 5.7_Pointed_metric_spaces
    * 6_Types_of_maps_between_metric_spaces
          o 6.1_Continuous_maps
          o 6.2_Uniformly_continuous_maps
          o 6.3_Lipschitz-continuous_maps_and_contractions
          o 6.4_Isometries
          o 6.5_Quasi-isometries
    * 7_Notions_of_metric_space_equivalence
    * 8_Topological_properties
    * 9_Distance_between_points_and_sets;_Hausdorff_distance_and_Gromov_metric
    * 10_Product_metric_spaces
          o 10.1_Continuity_of_distance
    * 11_Quotient_metric_spaces
    * 12_Generalizations_of_metric_spaces
          o 12.1_Metric_spaces_as_enriched_categories
    * 13_See_also
    * 14_Notes
    * 15_References
    * 16_External_links
***** History[edit] *****
         This section needs expansion with: Reasons for generalizing the
[[icon]] Euclidean metric, first non-Euclidean metrics studied, consequences
         for mathematics. You can help by adding_to_it. (August 2011)
In 1906 Maurice_FrÃ©chet introduced metric spaces in his work Sur quelques
points du calcul fonctionnel.[1] However the name is due to Felix_Hausdorff.
***** Definition[edit] *****
A metric space is an ordered_pair     ( M , d )   {\displaystyle (M,d)}  [
(M,d)] where     M   {\displaystyle M}  [M] is a set and     d   {\displaystyle
d}  [d] is a metric on     M   {\displaystyle M}  [M], i.e., a function
         d &#x003A; M &#x00D7; M &#x2192;  R    {\displaystyle d\colon M\times
      M\to \mathbb {R} }  [d \colon M \times M \to \mathbb{R}]
such that for any     x , y , z &#x2208; M   {\displaystyle x,y,z\in M}
[x,y,z\in M], the following holds:[2]
            d ( x , y ) = 0 &#x21D4; x = y
         {\displaystyle d
      1. (x,y)=0\Leftrightarrow x=y}  [      identity_of_indiscernibles
         {\displaystyle d
         (x,y)=0\Leftrightarrow x=y}]
            d ( x , y ) = d ( y , x )
      2. {\displaystyle d(x,y)=d(y,x)}  [    symmetry
         {\displaystyle d(x,y)=d(y,x)}]
            d ( x , z ) &#x2264; d ( x , y )
         + d ( y , z )   {\displaystyle d    subadditivity or triangle
      3. (x,z)\leq d(x,y)+d(y,z)}  [         inequality
         {\displaystyle d(x,z)\leq d(x,y)+d
         (y,z)}]
Given the above three axioms, we also have that     d ( x , y ) &#x2265; 0
{\displaystyle d(x,y)\geq 0}  [{\displaystyle d(x,y)\geq 0}] for any     x , y
&#x2208; M   {\displaystyle x,y\in M}  [x, y \in M]. This is deduced as
follows:
         d ( x , y ) + d ( y , x ) &#x2265; d ( x
      , x )   {\displaystyle d(x,y)+d(y,x)\geq d  by triangle inequality
      (x,x)}  [d(x,y) + d(y,x) \ge d(x,x)]
         d ( x , y ) + d ( x , y ) &#x2265; d ( x
      , x )   {\displaystyle d(x,y)+d(x,y)\geq d  by symmetry
      (x,x)}  [d(x,y) + d(x,y) \ge d(x,x)]
         2 d ( x , y ) &#x2265; 0
      {\displaystyle 2d(x,y)\geq 0}  [2d(x,y) \ge by identity of indiscernibles
      0]
         d ( x , y ) &#x2265; 0   {\displaystyle  we have non-negativity
      d(x,y)\geq 0}  [d(x,y)\geq 0]
The function     d   {\displaystyle d}  [d] is also called distance function or
simply distance. Often,     d   {\displaystyle d}  [d] is omitted and one just
writes     M   {\displaystyle M}  [M] for a metric space if it is clear from
the context what metric is used.
Ignoring mathematical details, for any system of roads and terrains the
distance between two locations can be defined as the length of the shortest
route connecting those locations. To be a metric there shouldn't be any one-way
roads. The triangle inequality expresses the fact that detours aren't
shortcuts. If the distance between two points is zero, the two points are
indistinguishable from one-another. Many of the examples below can be seen as
concrete versions of this general idea.
***** Examples of metric spaces[edit] *****
    * The real_numbers with the distance function     d ( x , y ) = | y
      &#x2212; x |   {\displaystyle d(x,y)=\vert y-x\vert }  [d(x,y) = \vert y
      - x \vert] given by the absolute_difference, and, more generally,
      Euclidean_n-space with the Euclidean_distance, are complete metric
      spaces. The rational_numbers with the same distance function also form a
      metric space, but not a complete one.
    * The positive_real_numbers with distance function     d ( x , y ) = | log
      &#x2061; ( y  /  x ) |   {\displaystyle d(x,y)=\vert \log(y/x)\vert }  [d
      (x,y) =\vert \log(y/x) \vert] is a complete metric space.
    * Any normed_vector_space is a metric space by defining     d ( x , y ) =
      &#x2016; y &#x2212; x &#x2016;   {\displaystyle d(x,y)=\lVert y-x\rVert }
      [d(x,y) = \lVert y - x \rVert], see also metrics_on_vector_spaces. (If
      such a space is complete, we call it a Banach_space.) Examples:
          o The Manhattan_norm gives rise to the Manhattan_distance, where the
            distance between any two points, or vectors, is the sum of the
            differences between corresponding coordinates.
          o The maximum_norm gives rise to the Chebyshev_distance or chessboard
            distance, the minimal number of moves a chess_king would take to
            travel from     x   {\displaystyle x}  [x] to     y
            {\displaystyle y}  [y].
    * The British_Rail metric (also called the âpost office metricâ or the
      âSNCF metricâ) on a normed_vector_space is given by     d ( x , y ) =
      &#x2016; x &#x2016; + &#x2016; y &#x2016;   {\displaystyle d(x,y)=\lVert
      x\rVert +\lVert y\rVert }  [d(x,y) = \lVert x \rVert + \lVert y \rVert]
      for distinct points     x   {\displaystyle x}  [x] and     y
      {\displaystyle y}  [y], and     d ( x , x ) = 0   {\displaystyle d
      (x,x)=0}  [d(x,x) = 0]. More generally     &#x2016; . &#x2016;
      {\displaystyle \lVert .\rVert }  [\lVert . \rVert] can be replaced with a
      function     f   {\displaystyle f}  [f] taking an arbitrary set     S
      {\displaystyle S}  [S] to non-negative reals and taking the value     0
      {\displaystyle 0}  [{\displaystyle 0}] at most once: then the metric is
      defined on     S   {\displaystyle S}  [S] by     d ( x , y ) = f ( x ) +
      f ( y )   {\displaystyle d(x,y)=f(x)+f(y)}  [d(x,y) = f(x) + f(y)] for
      distinct points     x   {\displaystyle x}  [x] and     y   {\displaystyle
      y}  [y], and     d ( x , x ) = 0   {\displaystyle d(x,x)=0}  [d(x,x) =
      0]. The name alludes to the tendency of railway journeys to proceed via
      London (or Paris) irrespective of their final destination.
    * If     ( M , d )   {\displaystyle (M,d)}  [(M,d)] is a metric space and
      X   {\displaystyle X}  [X] is a subset of     M   {\displaystyle M}  [M],
      then     ( X , d )   {\displaystyle (X,d)}  [(X,d)] becomes a metric
      space by restricting the domain of     d   {\displaystyle d}  [d] to
      X &#x00D7; X   {\displaystyle X\times X}  [X\times X].
    * The discrete_metric, where     d ( x , y ) = 0   {\displaystyle d(x,y)=0}
      [d(x,y) = 0] if     x = y   {\displaystyle x=y}  [x=y] and     d ( x , y
      ) = 1   {\displaystyle d(x,y)=1}  [d(x,y) = 1] otherwise, is a simple but
      important example, and can be applied to all sets. This, in particular,
      shows that for any set, there is always a metric space associated to it.
      Using this metric, any point is an open_ball, and therefore every subset
      is open and the space has the discrete_topology.
    * A finite metric space is a metric space having a finite number of points.
      Not every finite metric space can be isometrically embedded in a
      Euclidean_space.[3][4]
    * The hyperbolic_plane is a metric space. More generally:
          o If     M   {\displaystyle M}  [M] is any connected Riemannian
            manifold, then we can turn     M   {\displaystyle M}  [M] into a
            metric space by defining the distance of two points as the infimum
            of the lengths of the paths (continuously differentiable curves)
            connecting them.
          o If     X   {\displaystyle X}  [X] is some set and     M
            {\displaystyle M}  [M] is a metric space, then, the set of all
            bounded_functions     f &#x003A; X &#x2192; M   {\displaystyle
            f\colon X\rightarrow M}  [f \colon X \rightarrow M] (i.e. those
            functions whose image is a bounded_subset of     M   {\displaystyle
            M}  [M]) can be turned into a metric space by defining     d ( f ,
            g ) =  sup  x &#x2208; X   d ( f ( x ) , g ( x ) )   {\displaystyle
            d(f,g)=\sup _{x\in X}d(f(x),g(x))}  [d(f,g) = \sup_{x \in X} d(f
            (x),g(x))] for any two bounded functions     f   {\displaystyle f}
            [f] and     g   {\displaystyle g}  [g] (where     sup
            {\displaystyle \sup }  [\sup ] is supremum).[5] This metric is
            called the uniform_metric or supremum metric, and If     M
            {\displaystyle M}  [M] is complete, then this function_space is
            complete as well. If X is also a topological space, then the set of
            all bounded continuous functions from     X   {\displaystyle X}
            [X] to     M   {\displaystyle M}  [M] (endowed with the uniform
            metric), will also be a complete metric if M is.
          o If     G   {\displaystyle G}  [G] is an undirected_connected_graph,
            then the set     V   {\displaystyle V}  [V] of vertices of     G
            {\displaystyle G}  [G] can be turned into a metric space by
            defining     d ( x , y )   {\displaystyle d(x,y)}  [d(x,y)] to be
            the length of the shortest path connecting the vertices     x
            {\displaystyle x}  [x] and     y   {\displaystyle y}  [y]. In
            geometric_group_theory this is applied to the Cayley_graph of a
            group, yielding the word_metric.
    * Graph_edit_distance is a measure of dissimilarity between two graphs,
      defined as the minimal number of graph_edit_operations required to
      transform one graph into another.
    * The Levenshtein_distance is a measure of the dissimilarity between two
      strings     u   {\displaystyle u}  [u] and     v   {\displaystyle v}
      [v], defined as the minimal number of character deletions, insertions, or
      substitutions required to transform     u   {\displaystyle u}  [u] into
      v   {\displaystyle v}  [v]. This can be thought of as a special case of
      the shortest path metric in a graph and is one example of an edit
      distance.
    * Given a metric space     ( X , d )   {\displaystyle (X,d)}  [(X,d)] and
      an increasing concave_function     f &#x003A; [ 0 , &#x221E; ) &#x2192;
      [ 0 , &#x221E; )   {\displaystyle f\colon [0,\infty )\rightarrow
      [0,\infty )}  [f \colon [0,\infty) \rightarrow [0,\infty)] such that
      f ( x ) = 0   {\displaystyle f(x)=0}  [f(x) = 0] if and only if     x = 0
      {\displaystyle x=0}  [x=0], then     f &#x2218; d   {\displaystyle f\circ
      d}  [f \circ d] is also a metric on     X   {\displaystyle X}  [X].
    * Given an injective_function     f   {\displaystyle f}  [f] from any set
      A   {\displaystyle A}  [A] to a metric space     ( X , d )
      {\displaystyle (X,d)}  [(X,d)],     d ( f ( x ) , f ( y ) )
      {\displaystyle d(f(x),f(y))}  [d(f(x), f(y))] defines a metric on     A
      {\displaystyle A}  [A].
    * Using T-theory, the tight_span of a metric space is also a metric space.
      The tight span is useful in several types of analysis.
    * The set of all     m   {\displaystyle m}  [m] by     n   {\displaystyle
      n}  [n] matrices over some field is a metric space with respect to the
      rank distance     d ( X , Y ) =  r a n k  ( Y &#x2212; X )
      {\displaystyle d(X,Y)=\mathrm {rank} (Y-X)}  [d(X,Y) = \mathrm{rank}(Y -
      X)].
    * The Helly_metric is used in game_theory.
***** Open and closed sets, topology and convergence[edit] *****
Every metric space is a topological_space in a natural manner, and therefore
all definitions and theorems about general topological spaces also apply to all
metric spaces.
About any point     x   {\displaystyle x}  [x] in a metric space     M
{\displaystyle M}  [M] we define the open_ball of radius     r > 0
{\displaystyle r>0}  [r > 0] (where     r   {\displaystyle r}  [r] is a real
number) about     x   {\displaystyle x}  [x] as the set
         B ( x ; r ) = { y &#x2208; M : d ( x , y ) < r } .   {\displaystyle B
      (x;r)=\{y\in M:d(x,y)<r\}.}  [B(x;r) = \{y \in M : d(x,y) < r\}.]
These open balls form the base for a topology on M, making it a topological
space.
Explicitly, a subset     U   {\displaystyle U}  [U] of     M   {\displaystyle
M}  [M] is called open if for every     x   {\displaystyle x}  [x] in     U
{\displaystyle U}  [U] there exists an     r > 0   {\displaystyle r>0}  [r > 0]
such that     B ( x ; r )   {\displaystyle B(x;r)}  [B(x;r)] is contained in
U   {\displaystyle U}  [U]. The complement of an open set is called closed. A
neighborhood of the point     x   {\displaystyle x}  [x] is any subset of     M
{\displaystyle M}  [M] that contains an open ball about     x   {\displaystyle
x}  [x] as a subset.
A topological space which can arise in this way from a metric space is called a
metrizable space; see the article on metrization_theorems for further details.
A sequence (     x  n     {\displaystyle x_{n}}  [x_{n}]) in a metric space
M   {\displaystyle M}  [M] is said to converge to the limit     x &#x2208; M
{\displaystyle x\in M}  [x\in M] iff for every     &#x03F5; > 0
{\displaystyle \epsilon >0}  [\epsilon >0], there exists a natural number N
such that     d (  x  n   , x ) < &#x03F5;   {\displaystyle d(x_{n},x)<\epsilon
}  [d(x_n,x) < \epsilon ] for all     n > N   {\displaystyle n>N}  [n>N].
Equivalently, one can use the general definition of convergence available in
all topological spaces.
A subset     A   {\displaystyle A}  [A] of the metric space     M
{\displaystyle M}  [M] is closed iff every sequence in     A   {\displaystyle
A}  [A] that converges to a limit in     M   {\displaystyle M}  [M] has its
limit in     A   {\displaystyle A}  [A].
***** Types of metric spaces[edit] *****
**** Complete spaces[edit] ****
Main article: Complete_metric_space
A metric space     M   {\displaystyle M}  [M] is said to be complete if every
Cauchy_sequence converges in     M   {\displaystyle M}  [M]. That is to say: if
d (  x  n   ,  x  m   ) &#x2192; 0   {\displaystyle d(x_{n},x_{m})\to 0}  [d
(x_n, x_m) \to 0] as both     n   {\displaystyle n}  [n] and     m
{\displaystyle m}  [m] independently go to infinity, then there is some     y
&#x2208; M   {\displaystyle y\in M}  [y\in M] with     d (  x  n   , y )
&#x2192; 0   {\displaystyle d(x_{n},y)\to 0}  [d(x_n, y) \to 0].
Every Euclidean_space is complete, as is every closed subset of a complete
space. The rational numbers, using the absolute value metric     d ( x , y ) =
| x &#x2212; y |   {\displaystyle d(x,y)=\vert x-y\vert }  [d(x,y) = \vert x -
y \vert], are not complete.
Every metric space has a unique (up to isometry) completion, which is a
complete space that contains the given space as a dense subset. For example,
the real numbers are the completion of the rationals.
If     X   {\displaystyle X}  [X] is a complete subset of the metric space
M   {\displaystyle M}  [M], then     X   {\displaystyle X}  [X] is closed in
M   {\displaystyle M}  [M]. Indeed, a space is complete iff it is closed in any
containing metric space.
Every complete metric space is a Baire_space.
**** Bounded and totally bounded spaces[edit] ****
Diameter of a set.
See also: bounded_set
A metric space M is called bounded if there exists some number r, such that d
(x,y) â¤ r for all x and y in M. The smallest possible such r is called the
diameter of M. The space M is called precompact or totally_bounded if for every
r > 0 there exist finitely many open balls of radius r whose union covers M.
Since the set of the centres of these balls is finite, it has finite diameter,
from which it follows (using the triangle inequality) that every totally
bounded space is bounded. The converse does not hold, since any infinite set
can be given the discrete metric (one of the examples above) under which it is
bounded and yet not totally bounded.
Note that in the context of intervals in the space of real_numbers and
occasionally regions in a Euclidean space       R   n     {\displaystyle
\mathbb {R} ^{n}}  [{\displaystyle \mathbb {R} ^{n}}] a bounded set is referred
to as "a finite interval" or "finite region". However boundedness should not in
general be confused with "finite", which refers to the number of elements, not
to how far the set extends; finiteness implies boundedness, but not conversely.
Also note that an unbounded subset of       R   n     {\displaystyle \mathbb
{R} ^{n}}  [{\displaystyle \mathbb {R} ^{n}}] may have a finite volume.
**** Compact spaces[edit] ****
A metric space M is compact if every sequence in M has a subsequence that
converges to a point in M. This is known as sequential_compactness and, in
metric spaces (but not in general topological spaces), is equivalent to the
topological notions of countable_compactness and compactness defined via open
covers.
Examples of compact metric spaces include the closed interval [0,1] with the
absolute value metric, all metric spaces with finitely many points, and the
Cantor_set. Every closed subset of a compact space is itself compact.
A metric space is compact iff it is complete and totally bounded. This is known
as the HeineâBorel_theorem. Note that compactness depends only on the
topology, while boundedness depends on the metric.
Lebesgue's_number_lemma states that for every open cover of a compact metric
space M, there exists a "Lebesgue number" Î´ such that every subset of M of
diameter < Î´ is contained in some member of the cover.
Every compact metric space is second_countable,[6] and is a continuous image of
the Cantor_set. (The latter result is due to Pavel_Alexandrov and Urysohn.)
**** Locally compact and proper spaces[edit] ****
A metric space is said to be locally_compact if every point has a compact
neighborhood. Euclidean spaces are locally compact, but infinite-dimensional
Banach spaces are not.
A space is proper if every closed ball {y : d(x,y) â¤ r} is compact. Proper
spaces are locally compact, but the converse is not true in general.
**** Connectedness[edit] ****
A metric space     M   {\displaystyle M}  [M] is connected if the only subsets
that are both open and closed are the empty set and     M   {\displaystyle M}
[M] itself.
A metric space     M   {\displaystyle M}  [M] is path_connected if for any two
points     x , y &#x2208; M   {\displaystyle x,y\in M}  [x, y \in M] there
exists a continuous map     f &#x003A; [ 0 , 1 ] &#x2192; M   {\displaystyle
f\colon [0,1]\to M}  [f\colon [0,1] \to M] with     f ( 0 ) = x
{\displaystyle f(0)=x}  [f(0)=x] and     f ( 1 ) = y   {\displaystyle f(1)=y}
[f(1)=y]. Every path connected space is connected, but the converse is not true
in general.
There are also local versions of these definitions: locally_connected_spaces
and locally_path_connected_spaces.
Simply_connected_spaces are those that, in a certain sense, do not have
"holes".
**** Separable spaces[edit] ****
A metric space is separable_space if it has a countable dense subset. Typical
examples are the real numbers or any Euclidean space. For metric spaces (but
not for general topological spaces) separability is equivalent to second-
countability and also to the LindelÃ¶f property.
**** Pointed metric spaces[edit] ****
If     X   {\displaystyle X}  [X] is a nonempty metric space and      x  0
&#x2208; X   {\displaystyle x_{0}\in X}  [x_{0}\in X] then     ( X ,  x  0   )
{\displaystyle (X,x_{0})}  [(X,x_{0})] is called a pointed metric space, and
x  0     {\displaystyle x_{0}}  [x_{0}] is called a distinguished point. Note
that a pointed metric space is just a nonempty metric space with attention
drawn to its distinguished point, and that any nonempty metric space can be
viewed as a pointed metric space. The distinguished point is sometimes denoted
0   {\displaystyle 0}  [{\displaystyle 0}] due to its similar behavior to zero
in certain contexts.
***** Types of maps between metric spaces[edit] *****
Suppose (M1,d1) and (M2,d2) are two metric spaces.
**** Continuous maps[edit] ****
Main article: Continuous_function_(topology)
The map f:M1âM2 is continuous if it has one (and therefore all) of the
following equivalent properties:
  General topological continuity
      for every open set U in M2, the preimage f -1(U) is open in M1
      This is the general definition of continuity_in_topology.
  Sequential continuity
      if (xn) is a sequence in M1 that converges to x in M1, then the sequence
      (f(xn)) converges to f(x) in M2.
      This is sequential_continuity, due to Eduard_Heine.
  Îµ-Î´ definition
      for every x in M1 and every Îµ>0 there exists Î´>0 such that for all y in
      M1 we have
                d  1   ( x , y ) < &#x03B4; &#x21D2;  d  2   ( f ( x ) , f ( y
            ) ) < &#x03B5; .   {\displaystyle d_{1}(x,y)<\delta \Rightarrow d_
            {2}(f(x),f(y))<\varepsilon .}  [d_1(x,y)<\delta \Rightarrow d_2(f
            (x),f(y))< \varepsilon.]
      This uses the (Îµ,_Î´)-definition_of_limit, and is due to Augustin_Louis
      Cauchy.
Moreover, f is continuous if and only if it is continuous on every compact
subset of M1.
The image of every compact set under a continuous function is compact, and the
image of every connected set under a continuous function is connected.
**** Uniformly continuous maps[edit] ****
The map Æ : M1 â M2 is uniformly_continuous if for every Îµ > 0 there exists
Î´ > 0 such that
          d  1   ( x , y ) < &#x03B4; &#x21D2;  d  2   ( f ( x ) , f ( y ) ) <
      &#x03B5;    for all    x , y &#x2208;  M  1   .   {\displaystyle d_{1}
      (x,y)<\delta \Rightarrow d_{2}(f(x),f(y))<\varepsilon \quad {\mbox{for
      all}}\quad x,y\in M_{1}.}  [d_1(x,y)<\delta \Rightarrow d_2(f(x),f(y))<
      \varepsilon \quad\mbox{for all}\quad x,y\in M_1.]
Every uniformly continuous map Æ : M1 â M2 is continuous. The converse is
true if M1 is compact (HeineâCantor_theorem).
Uniformly continuous maps turn Cauchy sequences in M1 into Cauchy sequences in
M2. For continuous maps this is generally wrong; for example, a continuous map
from the open interval (0,1) onto the real line turns some Cauchy sequences
into unbounded sequences.
**** Lipschitz-continuous maps and contractions[edit] ****
Main article: Lipschitz_continuity
Given a real number K > 0, the map Æ : M1 â M2 is K-Lipschitz_continuous if
          d  2   ( f ( x ) , f ( y ) ) &#x2264; K  d  1   ( x , y )    for all
      x , y &#x2208;  M  1   .   {\displaystyle d_{2}(f(x),f(y))\leq Kd_{1}
      (x,y)\quad {\mbox{for all}}\quad x,y\in M_{1}.}  [d_2(f(x),f(y))\leq K
      d_1(x,y)\quad\mbox{for all}\quad x,y\in M_1.]
Every Lipschitz-continuous map is uniformly continuous, but the converse is not
true in general.
If K < 1, then Æ is called a contraction. Suppose M2 = M1 and M1 is complete.
If Æ is a contraction, then Æ admits a unique fixed point (Banach_fixed_point
theorem). If M1 is compact, the condition can be weakened a bit: Æ admits a
unique fixed point if
         d ( f ( x ) , f ( y ) ) < d ( x , y )    for all    x &#x2260; y
      &#x2208;  M  1     {\displaystyle d(f(x),f(y))<d(x,y)\quad {\mbox{for
      all}}\quad x\neq y\in M_{1}}  [ d(f(x), f(y)) < d(x, y) \quad \mbox{for
      all} \quad x \ne y \in M_1].
**** Isometries[edit] ****
The map f:M1âM2 is an isometry if
          d  2   ( f ( x ) , f ( y ) ) =  d  1   ( x , y )    for all    x , y
      &#x2208;  M  1     {\displaystyle d_{2}(f(x),f(y))=d_{1}(x,y)\quad {\mbox
      {for all}}\quad x,y\in M_{1}}  [d_2(f(x),f(y))=d_1(x,y)\quad\mbox{for
      all}\quad x,y\in M_1]
Isometries are always injective; the image of a compact or complete set under
an isometry is compact or complete, respectively. However, if the isometry is
not surjective, then the image of a closed (or open) set need not be closed (or
open).
**** Quasi-isometries[edit] ****
The map f : M1 â M2 is a quasi-isometry if there exist constants A â¥ 1 and
B â¥ 0 such that
           1 A    d  2   ( f ( x ) , f ( y ) ) &#x2212; B &#x2264;  d  1   ( x
      , y ) &#x2264; A  d  2   ( f ( x ) , f ( y ) ) + B  &#xA0;for all&#xA0;
      x , y &#x2208;  M  1     {\displaystyle {\frac {1}{A}}d_{2}(f(x),f(y))-
      B\leq d_{1}(x,y)\leq Ad_{2}(f(x),f(y))+B{\text{ for all }}x,y\in M_{1}}
      [\frac{1}{A} d_2(f(x),f(y))-B\leq d_1(x,y)\leq A d_2(f(x),f(y))+B \text
      { for all } x,y\in M_1]
and a constant C â¥ 0 such that every point in M2 has a distance at most C
from some point in the image f(M1).
Note that a quasi-isometry is not required to be continuous. Quasi-isometries
compare the "large-scale structure" of metric spaces; they find use in
geometric_group_theory in relation to the word_metric.
***** Notions of metric space equivalence[edit] *****
Given two metric spaces (M1, d1) and (M2, d2):
    * They are called homeomorphic (topologically isomorphic) if there exists a
      homeomorphism between them (i.e., a bijection continuous in both
      directions).
    * They are called uniformic (uniformly isomorphic) if there exists a
      uniform_isomorphism between them (i.e., a bijection uniformly continuous
      in both directions).
    * They are called isometric if there exists a bijective isometry between
      them. In this case, the two metric spaces are essentially identical.
    * They are called quasi-isometric if there exists a quasi-isometry between
      them.
***** Topological properties[edit] *****
Metric spaces are paracompact[7] Hausdorff_spaces[8] and hence normal (indeed
they are perfectly normal). An important consequence is that every metric space
admits partitions_of_unity and that every continuous real-valued function
defined on a closed subset of a metric space can be extended to a continuous
map on the whole space (Tietze_extension_theorem). It is also true that every
real-valued Lipschitz-continuous map defined on a subset of a metric space can
be extended to a Lipschitz-continuous map on the whole space.
Metric spaces are first_countable since one can use balls with rational radius
as a neighborhood base.
The metric topology on a metric space M is the coarsest topology on M relative
to which the metric d is a continuous map from the product of M with itself to
the non-negative real numbers.
***** Distance between points and sets; Hausdorff distance and Gromov metric
[edit] *****
A simple way to construct a function separating a point from a closed set (as
required for a completely_regular space) is to consider the distance_between
the_point_and_the_set. If (M,d) is a metric space, S is a subset of M and x is
a point of M, we define the distance from x to S as
         d ( x , S ) = inf { d ( x , s ) : s &#x2208; S }   {\displaystyle d
      (x,S)=\inf\{d(x,s):s\in S\}}  [d(x,S) = \inf\{d(x,s) : s \in S \} ] where
      inf   {\displaystyle \inf }  [\inf] represents the infimum.
Then d(x, S) = 0 if and only if x belongs to the closure of S. Furthermore, we
have the following generalization of the triangle inequality:
         d ( x , S ) &#x2264; d ( x , y ) + d ( y , S ) ,   {\displaystyle d
      (x,S)\leq d(x,y)+d(y,S),}  [d(x,S) \leq d(x,y) + d(y,S),]
which in particular shows that the map     x &#x21A6; d ( x , S )
{\displaystyle x\mapsto d(x,S)}  [x\mapsto d(x,S)] is continuous.
Given two subsets S and T of M, we define their Hausdorff_distance to be
          d  H   ( S , T ) = max { sup { d ( s , T ) : s &#x2208; S } , sup { d
      ( t , S ) : t &#x2208; T } }   {\displaystyle d_{H}(S,T)=\max\{\sup\{d
      (s,T):s\in S\},\sup\{d(t,S):t\in T\}\}}  [d_H(S,T) = \max \{ \sup\{d(s,T)
      : s \in S \} , \sup\{ d(t,S) : t \in T \} \} ] where     sup
      {\displaystyle \sup }  [\sup ] represents the supremum.
In general, the Hausdorff distance dH(S,T) can be infinite. Two sets are close
to each other in the Hausdorff distance if every element of either set is close
to some element of the other set.
The Hausdorff distance dH turns the set K(M) of all non-empty compact subsets
of M into a metric space. One can show that K(M) is complete if M is complete.
(A different notion of convergence of compact subsets is given by the
Kuratowski_convergence.)
One can then define the GromovâHausdorff_distance between any two metric
spaces by considering the minimal Hausdorff distance of isometrically embedded
versions of the two spaces. Using this distance, the class of all (isometry
classes of) compact metric spaces becomes a metric space in its own right.
***** Product metric spaces[edit] *****
If     (  M  1   ,  d  1   ) , &#x2026; , (  M  n   ,  d  n   )
{\displaystyle (M_{1},d_{1}),\ldots ,(M_{n},d_{n})}  [(M_1,d_1),\ldots,
(M_n,d_n)] are metric spaces, and N is the Euclidean_norm on Rn, then
(    M  1   &#x00D7; &#x2026; &#x00D7;  M  n   , N (  d  1   , &#x2026; ,  d  n
)   )     {\displaystyle {\Big (}M_{1}\times \ldots \times M_{n},N(d_{1},\ldots
,d_{n}){\Big )}}  [\Big(M_1\times \ldots \times M_n, N(d_1,\ldots,d_n)\Big)] is
a metric space, where the product_metric is defined by
         N (  d  1   , . . . ,  d  n   )   (   (  x  1   , &#x2026; ,  x  n   )
      , (  y  1   , &#x2026; ,  y  n   )   )   = N   (    d  1   (  x  1   ,  y
      1   ) , &#x2026; ,  d  n   (  x  n   ,  y  n   )   )   ,   {\displaystyle
      N(d_{1},...,d_{n}){\Big (}(x_{1},\ldots ,x_{n}),(y_{1},\ldots ,y_{n})
      {\Big )}=N{\Big (}d_{1}(x_{1},y_{1}),\ldots ,d_{n}(x_{n},y_{n}){\Big )},}
      [N(d_1,...,d_n)\Big((x_1,\ldots,x_n),(y_1,\ldots,y_n)\Big) = N\Big(d_1
      (x_1,y_1),\ldots,d_n(x_n,y_n)\Big),]
and the induced topology agrees with the product_topology. By the equivalence
of norms in finite dimensions, an equivalent metric is obtained if N is the
taxicab_norm, a p-norm, the max_norm, or any other norm which is non-decreasing
as the coordinates of a positive n-tuple increase (yielding the triangle
inequality).
Similarly, a countable product of metric spaces can be obtained using the
following metric
         d ( x , y ) =  &#x2211;  i = 1   &#x221E;     1  2  i         d  i
      (  x  i   ,  y  i   )   1 +  d  i   (  x  i   ,  y  i   )    .
      {\displaystyle d(x,y)=\sum _{i=1}^{\infty }{\frac {1}{2^{i}}}{\frac {d_
      {i}(x_{i},y_{i})}{1+d_{i}(x_{i},y_{i})}}.}  [d(x,y)=\sum_{i=1}^\infty
      \frac1{2^i}\frac{d_i(x_i,y_i)}{1+d_i(x_i,y_i)}.]
An uncountable product of metric spaces need not be metrizable. For example,
R    R      {\displaystyle \mathbf {R} ^{\mathbf {R} }}  [\mathbf{R}^\mathbf
{R}] is not first-countable and thus isn't metrizable.
**** Continuity of distance[edit] ****
In the case of a single space     ( M , d )   {\displaystyle (M,d)}  [(M,d)],
the distance map     d &#x003A; M &#x00D7; M &#x2192;  R  +     {\displaystyle
d\colon M\times M\rightarrow R^{+}}  [d\colon M\times M \rightarrow R^+] (from
the definition) is uniformly continuous with respect to any of the above
product metrics     N ( d , d )   {\displaystyle N(d,d)}  [N(d,d)], and in
particular is continuous with respect to the product topology of     M &#x00D7;
M   {\displaystyle M\times M}  [M\times M].
***** Quotient metric spaces[edit] *****
If M is a metric space with metric d, and ~ is an equivalence_relation on M,
then we can endow the quotient set M/~ with the following (pseudo)metric. Given
two equivalence classes [x] and [y], we define
          d &#x2032;  ( [ x ] , [ y ] ) = inf { d (  p  1   ,  q  1   ) + d
      (  p  2   ,  q  2   ) + &#x22EF; + d (  p  n   ,  q  n   ) }
      {\displaystyle d'([x],[y])=\inf\{d(p_{1},q_{1})+d(p_{2},q_{2})+\dotsb +d
      (p_{n},q_{n})\}}  [d'([x],[y]) = \inf\{d(p_1,q_1)+d(p_2,q_2)+\dotsb+d(p_
      {n},q_{n})\}]
where the infimum is taken over all finite sequences     (  p  1   ,  p  2   ,
&#x2026; ,  p  n   )   {\displaystyle (p_{1},p_{2},\dots ,p_{n})}  [(p_1, p_2,
\dots, p_n)] and     (  q  1   ,  q  2   , &#x2026; ,  q  n   )
{\displaystyle (q_{1},q_{2},\dots ,q_{n})}  [(q_1, q_2, \dots, q_n)] with
[  p  1   ] = [ x ]   {\displaystyle [p_{1}]=[x]}  [[p_1]=[x]],     [  q  n   ]
= [ y ]   {\displaystyle [q_{n}]=[y]}  [[q_n]=[y]],     [  q  i   ] = [  p  i +
1   ] , i = 1 , 2 , &#x2026; , n &#x2212; 1   {\displaystyle [q_{i}]=[p_
{i+1}],i=1,2,\dots ,n-1}  [[q_i]=[p_{i+1}], i=1,2,\dots, n-1]. In general this
will only define a pseudometric, i.e.      d &#x2032;  ( [ x ] , [ y ] ) = 0
{\displaystyle d'([x],[y])=0}  [d'([x],[y])=0] does not necessarily imply that
[ x ] = [ y ]   {\displaystyle [x]=[y]}  [[x]=[y]]. However, for nice
equivalence relations (e.g., those given by gluing together polyhedra along
faces), it is a metric.
The quotient metric d is characterized by the following universal_property. If
f : ( M , d ) &#x27F6; ( X , &#x03B4; )   {\displaystyle f:(M,d)\longrightarrow
(X,\delta )}  [f:(M,d)\longrightarrow(X,\delta)] is a metric_map between metric
spaces (that is,     &#x03B4; ( f ( x ) , f ( y ) ) &#x2264; d ( x , y )
{\displaystyle \delta (f(x),f(y))\leq d(x,y)}  [\delta(f(x),f(y))\le d(x,y)]
for all x, y) satisfying f(x)=f(y) whenever     x &#x223C; y ,   {\displaystyle
x\sim y,}  [x\sim y,] then the induced function       f &#x00AF;   &#x003A; M
/  &#x223C;&#x27F6; X   {\displaystyle {\overline {f}}\colon M/\sim
\longrightarrow X}  [\overline{f}\colon M/\sim\longrightarrow X], given by
f &#x00AF;   ( [ x ] ) = f ( x )   {\displaystyle {\overline {f}}([x])=f(x)}
[\overline{f}([x])=f(x)], is a metric map       f &#x00AF;   &#x003A; ( M  /
&#x223C; ,  d &#x2032;  ) &#x27F6; ( X , &#x03B4; ) .   {\displaystyle
{\overline {f}}\colon (M/\sim ,d')\longrightarrow (X,\delta ).}  [\overline
{f}\colon (M/\sim,d')\longrightarrow (X,\delta).]
A topological space is sequential if and only if it is a quotient of a metric
space.[9]
***** Generalizations of metric spaces[edit] *****
    * Every metric space is a uniform_space in a natural manner, and every
      uniform space is naturally a topological_space. Uniform and topological
      spaces can therefore be regarded as generalizations of metric spaces.
    * If we consider the first definition of a metric space given_above and
      relax the second requirement, we arrive at the concepts of a pseudometric
      space or a dislocated metric space.[10] If we remove the third or fourth,
      we arrive at a quasimetric_space, or a semimetric_space.
    * If the distance function takes values in the extended_real_number_line
      Râª{+â}, but otherwise satisfies all four conditions, then it is
      called an extended metric and the corresponding space is called an
      &#x221E;   {\displaystyle \infty }  [\infty ]-metric space. If the
      distance function takes values in some (suitable) ordered set (and the
      triangle inequality is adjusted accordingly), then we arrive at the
      notion of generalized ultrametric.[10]
    * Approach_spaces are a generalization of metric spaces, based on point-to-
      set distances, instead of point-to-point distances.
    * A continuity_space is a generalization of metric spaces and posets, that
      can be used to unify the notions of metric spaces and domains.
    * A partial metric space is intended to be the least generalisation of the
      notion of a metric space, such that the distance of each point from
      itself is no longer necessarily zero.[11]
**** Metric spaces as enriched categories[edit] ****
The ordered set     (  R  , &#x2265; )   {\displaystyle (\mathbb {R} ,\geq )}
[(\mathbb {R} ,\geq )] can be seen as a category by requesting exactly one
morphism     a &#x2192; b   {\displaystyle a\to b}  [a\to b] if     a &#x2265;
b   {\displaystyle a\geq b}  [a\geq b] and none otherwise. By using     +
{\displaystyle +}  [+] as the tensor_product and     0   {\displaystyle 0}  [
{\displaystyle 0}] as the identity, it becomes a monoidal_category      R
&#x2217;     {\displaystyle R^{*}}  [R^{*}]. Every metric space     ( M , d )
{\displaystyle (M,d)}  [(M,d)] can now be viewed as a category      M  &#x2217;
{\displaystyle M^{*}}  [M^*] enriched over      R  &#x2217;     {\displaystyle
R^{*}}  [R^{*}]:
    * Set     Ob &#x2061; (  M  &#x2217;   ) := M   {\displaystyle
      \operatorname {Ob} (M^{*}):=M}  [\operatorname {Ob}(M^{*}):=M]
    * For each     X , Y &#x2208; M   {\displaystyle X,Y\in M}  [X,Y\in M] set
      Hom &#x2061; ( X , Y ) := d ( X , Y ) &#x2208; Ob &#x2061; (  R  &#x2217;
      )   {\displaystyle \operatorname {Hom} (X,Y):=d(X,Y)\in \operatorname
      {Ob} (R^{*})}  [\operatorname{Hom}(X,Y):=d(X,Y)\in \operatorname{Ob}
      (R^*)]
    * The composition morphism     Hom &#x2061; ( Y , Z ) &#x2297; Hom &#x2061;
      ( X , Y ) &#x2192; Hom &#x2061; ( X , Z )   {\displaystyle \operatorname
      {Hom} (Y,Z)\otimes \operatorname {Hom} (X,Y)\to \operatorname {Hom}
      (X,Z)}  [\operatorname{Hom}(Y,Z)\otimes \operatorname{Hom}(X,Y)\to
      \operatorname{Hom}(X,Z)] will be the unique morphism in      R  &#x2217;
      {\displaystyle R^{*}}  [R^{*}] given from the triangle inequality     d
      ( y , z ) + d ( x , y ) &#x2265; d ( x , z )   {\displaystyle d(y,z)+d
      (x,y)\geq d(x,z)}  [d(y,z)+d(x,y)\geq d(x,z)]
    * The identity morphism     0 &#x2192; Hom &#x2061; ( X , X )
      {\displaystyle 0\to \operatorname {Hom} (X,X)}  [0\to \operatorname{Hom}
      (X,X)] will be the unique morphism given from the fact that     0
      &#x2265; d ( X , X )   {\displaystyle 0\geq d(X,X)}  [0\geq d(X,X)].
    * Since      R  &#x2217;     {\displaystyle R^{*}}  [R^{*}] is a poset, all
      diagrams that are required for an enriched category commute
      automatically.
See the paper by F.W. Lawvere listed below.
***** See also[edit] *****
    * Space_(mathematics)
    * Metric_(mathematics)
    * Metric_signature
    * Metric_tensor
    * Metric_tree
    * Norm_(mathematics)
    * Normed_vector_space
    * Measure_(mathematics)
    * Hilbert_space
    * Hilbert's_fourth_problem
    * Product_metric
    * AleksandrovâRassias_problem
    * Category_of_metric_spaces
    * Classical_Wiener_space
    * Glossary_of_Riemannian_and_metric_geometry
    * Isometry, contraction_mapping and metric_map
    * Lipschitz_continuity
    * Triangle_inequality
    * Ultrametric_space
***** Notes[edit] *****
   1. ^ Rendic. Circ. Mat. Palermo 22 (1906) 1â74
   2. ^B. Choudhary (1992). The_Elements_of_Complex_Analysis. New Age
      International. p. 20. ISBN 978-81-224-0399-2.
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
   4. ^ Nathan_Linial. Finite_Metric_SpacesâCombinatorics,_Geometry_and
      Algorithms,_Proceedings_of_the_ICM,_Beijing_2002,_vol._3,_pp573â586
      Archived 2018-05-02 at the Wayback_Machine
   5. ^ Open_problems_on_embeddings_of_finite_metric_spaces,_edited_by_JirÄ«Ä±
      MatouÅ¡ek,_2007 Archived 2010-12-26 at the Wayback_Machine
   6. ^ SearcÃ³id, p._107.
   7. ^"PlanetMath:_a_compact_metric_space_is_second_countable".
      planetmath.org. Archived from the original on 5 February 2009. Retrieved
      2 May 2018.
   8. ^ Rudin, Mary Ellen. A_new_proof_that_metric_spaces_are_paracompact
      Archived 2016-04-12 at the Wayback_Machine. Proceedings of the American
      Mathematical Society, Vol. 20, No. 2. (Feb., 1969), p. 603.
   9. ^"metric_spaces_are_Hausdorff". PlanetMath.
  10. ^ Goreham, Anthony. Sequential_convergence_in_Topological_Spaces Archived
      2011-06-04 at the Wayback_Machine. Honours' Dissertation, Queen's
      College, Oxford (April, 2001), p. 14
  11. ^ a bPascal Hitzler; Anthony Seda (19 April 2016). Mathematical_Aspects
      of_Logic_Programming_Semantics. CRC Press. ISBN 978-1-4398-2962-2.
  12. ^"Partial_metrics :_welcome". www.dcs.warwick.ac.uk. Archived from the
      original on 27 July 2017. Retrieved 2 May 2018.
***** References[edit] *****
    * Victor Bryant, Metric Spaces: Iteration and Application, Cambridge
      University_Press, 1985,
ISBN 0-521-31897-1.
Dmitri Burago, Yu_D_Burago, Sergei Ivanov, A Course in Metric Geometry,
American Mathematical Society, 2001,
ISBN 0-8218-2129-6.
Athanase Papadopoulos, Metric Spaces, Convexity and Nonpositive Curvature,
European_Mathematical_Society, First edition 2004,
ISBN 978-3-03719-010-4. Second edition 2014,
ISBN 978-3-03719-132-3.
MÃ­cheÃ¡l_Ã_SearcÃ³id, Metric_Spaces, Springer_Undergraduate_Mathematics
Series, 2006,
ISBN 1-84628-369-8.
Lawvere, F. William, "Metric spaces, generalized logic, and closed categories",
[Rend. Sem. Mat. Fis. Milano 43 (1973), 135â166 (1974); (Italian summary)
This is reprinted (with author commentary) at Reprints_in_Theory_and
Applications_of_Categories Also (with an author commentary) in Enriched
categories in the logic of geometry and analysis. Repr. Theory Appl. Categ. No.
1 (2002), 1â37.
    * Weisstein,_Eric_W. "Product_Metric". MathWorld.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Metric_space", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Far_and_near_—_several_examples_of_distance_functions at cut-the-knot.
    * v
    * t
    * e
Topology
                 * General_(point-set)
                 * Algebraic
                 * Combinatorial
                 * Continuum
Fields           * Differential
                 * Geometric
                       o low-dimensional
                 * Homology
                       o cohomology
                 * Set-theoretic
                 * Open_set / Closed_set  [Computer_graphics_rendering_of_a
                 * Continuity              Klein_bottle]
                 * Space
                       o compact
                       o Hausdorff
                       o metric
Key concepts           o uniform
                 * Homotopy
                       o homotopy_group
                       o fundamental_group
                 * Simplicial_complex
                 * CW_complex
                 * Manifold
    * [Category] Category
    * [Portal] Portal
    * [Wikibooks page] Wikibook
    * [Wikiversity page] Wikiversity
    * [List-Class article] Topics
          o general
          o algebraic
          o geometric
    * [List-Class article] Publications
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85084441
                                              * NDL: 00567250

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Metric_space&oldid=908561438"
Categories:
    * Mathematical_analysis
    * Mathematical_structures
    * Metric_geometry
    * Topology
    * Topological_spaces
Hidden categories:
    * Webarchive_template_wayback_links
    * Articles_to_be_expanded_from_August_2011
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * VÃ¨neto
    * Tiáº¿ng_Viá»t
    * æè¨
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 30 July 2019, at 14:15 (UTC).
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
