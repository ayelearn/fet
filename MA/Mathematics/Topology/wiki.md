The following text has been accessed from https://en.wikipedia.org/wiki/Topology at Fri Aug 9 02:34:13 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Topology ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Branch of mathematics
This article is about the branch of mathematics. For the mathematical
structure, see Topological_space. For other uses, see Topology_
(disambiguation).
Not to be confused with topography.
MÃ¶bius_strips, which have only one surface and one edge, are a kind of object
studied in topology.
In mathematics, topology (from the Greek ÏÏÏÎ¿Ï, place, and Î»ÏÎ³Î¿Ï,
study) is concerned with the properties of a geometric_object that are
preserved under continuous deformations, such as stretching, twisting,
crumpling and bending, but not tearing or gluing.
A topological_space is a set endowed with a structure, called a topology, which
allows defining continuous deformation of subspaces, and, more generally, all
kinds of continuity. Euclidean_spaces, and, more generally, metric_spaces are
examples of topological spaces, as any distance or metric defines a topology.
The deformations that are considered in topology are homeomorphisms and
homotopies. A property that is invariant under such deformations is a
topological_property. Basic examples of topological properties are: the
dimension, which allows distinguishing between a line and a surface;
compactness, which allows distinguishing between a line and a circle;
connectedness, which allows distinguishing a circle from two non-intersecting
circles.
The ideas underlying topology go back to Gottfried_Leibniz, who in the 17th
century envisioned the geometria situs and analysis situs. Leonhard_Euler's
Seven_Bridges_of_KÃ¶nigsberg problem and polyhedron_formula are arguably the
field's first theorems. The term topology was introduced by Johann_Benedict
Listing in the 19th century, although it was not until the first decades of the
20th century that the idea of a topological space was developed.
A three-dimensional depiction of a thickened trefoil_knot, the simplest non-
trivial_knot
⁰
***** Contents *****
    * 1_Motivation
    * 2_History
    * 3_Concepts
          o 3.1_Topologies_on_sets
          o 3.2_Continuous_functions_and_homeomorphisms
          o 3.3_Manifolds
    * 4_Topics
          o 4.1_General_topology
          o 4.2_Algebraic_topology
          o 4.3_Differential_topology
          o 4.4_Geometric_topology
          o 4.5_Generalizations
    * 5_Applications
          o 5.1_Biology
          o 5.2_Computer_science
          o 5.3_Physics
          o 5.4_Robotics
          o 5.5_Games_and_puzzles
          o 5.6_Fiber_art
    * 6_See_also
    * 7_References
          o 7.1_Citations
          o 7.2_Bibliography
    * 8_Further_reading
    * 9_External_links
***** Motivation[edit] *****
The motivating insight behind topology is that some geometric problems depend
not on the exact shape of the objects involved, but rather on the way they are
put together. For example, the square and the circle have many properties in
common: they are both one dimensional objects (from a topological point of
view) and both separate the plane into two parts, the part inside and the part
outside.
In one of the first papers in topology, Leonhard Euler demonstrated that it was
impossible to find a route through the town of KÃ¶nigsberg (now Kaliningrad)
that would cross each of its seven bridges exactly once. This result did not
depend on the lengths of the bridges or on their distance from one another, but
only on connectivity properties: which bridges connect to which islands or
riverbanks. This Seven Bridges of KÃ¶nigsberg problem led to the branch of
mathematics known as graph_theory.
A continuous deformation (a type of homeomorphism) of a mug into a doughnut
(torus) and a cow into a sphere
Similarly, the hairy_ball_theorem of algebraic topology says that "one cannot
comb the hair flat on a hairy ball without creating a cowlick." This fact is
immediately convincing to most people, even though they might not recognize the
more formal statement of the theorem, that there is no nonvanishing continuous
tangent_vector_field on the sphere. As with the Bridges of KÃ¶nigsberg, the
result does not depend on the shape of the sphere; it applies to any kind of
smooth blob, as long as it has no holes.
To deal with these problems that do not rely on the exact shape of the objects,
one must be clear about just what properties these problems do rely on. From
this need arises the notion of homeomorphism. The impossibility of crossing
each bridge just once applies to any arrangement of bridges homeomorphic to
those in KÃ¶nigsberg, and the hairy ball theorem applies to any space
homeomorphic to a sphere.
Intuitively, two spaces are homeomorphic if one can be deformed into the other
without cutting or gluing. A traditional joke is that a topologist cannot
distinguish a coffee mug from a doughnut, since a sufficiently pliable doughnut
could be reshaped to a coffee cup by creating a dimple and progressively
enlarging it, while shrinking the hole into a handle.[1]
Homeomorphism can be considered the most basic topological_equivalence. Another
is homotopy_equivalence. This is harder to describe without getting technical,
but the essential notion is that two objects are homotopy equivalent if they
both result from "squishing" some larger object.
 __Equivalence_classes_of_the_English_(i.e.,_Latin)_alphabet_(sans-serif)__
|Homeomorphism____________________|Homotopy_equivalence____________________|
|[{A,R}_{B}_                      |[{A,R,D,O,P,Q}_{B},_                    |
|{C,G,I,J,L,M,N,S,U,V,W,Z},_{D,O}_|{C,E,F,G,H,I,J,K,L,M,N,S,T,U,V,W,X,Y,Z}]|
|{E,F,T,Y}_{H,K},_{P,Q}_{X}]______|________________________________________|
An introductory exercise is to classify the uppercase letters of the English
alphabet according to homeomorphism and homotopy equivalence. The result
depends on the font used, and on whether the strokes making up the letters have
some thickness or are ideal curves with no thickness. The figures here use the
sans-serif Myriad font and are assumed to consist of ideal curves without
thickness. Homotopy equivalence is a coarser relationship than homeomorphism; a
homotopy equivalence class can contain several homeomorphism classes. The
simple case of homotopy equivalence described above can be used here to show
two letters are homotopy equivalent. For example, O fits inside P and the tail
of the P can be squished to the "hole" part.
Homeomorphism classes are:
    * no holes corresponding with C, G, I, J, L, M, N, S, U, V, W, and Z;
    * no holes and three tails corresponding with E, F, T, and Y;
    * no holes and four tails corresponding with X;
    * one hole and no tail corresponding with D and O;
    * one hole and one tail corresponding with P and Q;
    * one hole and two tails corresponding with A and R;
    * two holes and no tail corresponding with B; and
    * a bar with four tails corresponding with H and K; the "bar" on the K is
      almost too short to see.
Homotopy classes are larger, because the tails can be squished down to a point.
They are:
    * one hole,
    * two holes, and
    * no holes.
To classify the letters correctly, we must show that two letters in the same
class are equivalent and two letters in different classes are not equivalent.
In the case of homeomorphism, this can be done by selecting points and showing
their removal disconnects the letters differently. For example, X and Y are not
homeomorphic because removing the center point of the X leaves four pieces;
whatever point in Y corresponds to this point, its removal can leave at most
three pieces. The case of homotopy equivalence is harder and requires a more
elaborate argument showing an algebraic invariant, such as the fundamental
group, is different on the supposedly differing classes.
Letter topology has practical relevance in stencil typography. For instance,
Braggadocio font stencils are made of one connected piece of material.
***** History[edit] *****
The Seven_Bridges_of_KÃ¶nigsberg was a problem solved by Euler.
Topology, as a well-defined mathematical discipline, originates in the early
part of the twentieth century, but some isolated results can be traced back
several centuries.[2] Among these are certain questions in geometry
investigated by Leonhard_Euler. His 1736 paper on the Seven_Bridges_of
KÃ¶nigsberg is regarded as one of the first practical applications of topology.
[2] On 14 November 1750, Euler wrote to a friend that he had realised the
importance of the edges of a polyhedron. This led to his polyhedron_formula, V
â E + F = 2 (where V, E, and F respectively indicate the number of vertices,
edges, and faces of the polyhedron). Some authorities regard this analysis as
the first theorem, signalling the birth of topology.[3][4]
Further contributions were made by Augustin-Louis_Cauchy, Ludwig_SchlÃ¤fli,
Johann_Benedict_Listing, Bernhard_Riemann and Enrico_Betti.[5] Listing
introduced the term "Topologie" in Vorstudien zur Topologie, written in his
native German, in 1847, having used the word for ten years in correspondence
before its first appearance in print.[6] The English form "topology" was used
in 1883 in Listing's obituary in the journal Nature to distinguish "qualitative
geometry from the ordinary geometry in which quantitative relations chiefly are
treated".[7] The term "topologist" in the sense of a specialist in topology was
used in 1905 in the magazine Spectator.[citation_needed]
Their work was corrected, consolidated and greatly extended by Henri_PoincarÃ©.
In 1895, he published his ground-breaking paper on Analysis_Situs, which
introduced the concepts now known as homotopy and homology, which are now
considered part of algebraic_topology.[5]
             Topological characteristics of closed 2-manifolds[5]
                                             Betti_numbers        Torsion
Manifold       Euler_num      Orientability                       coefficient
                                             b0 b1             b2 (1-dim)

Sphere         2              Orientable     1  0              1  none
Torus          0              Orientable     1  2              1  none
2-holed torus  â2        Orientable     1  4              1  none
g-holed torus  2 â 2g    Orientable     1  2g             1  none
(genus g)
Projective     1              Non-orientable 1  0              0  2
plane
Klein_bottle   0              Non-orientable 1  1              0  2
Sphere with c
cross-caps (c  2 â c     Non-orientable 1  c â 1     0  2
> 0)
2-Manifold
with g holes   2 â (2g + Non-orientable 1  (2g + c) â01 2
and c cross-
caps (c > 0)
Unifying the work on function spaces of Georg_Cantor, Vito_Volterra, Cesare
ArzelÃ , Jacques_Hadamard, Giulio_Ascoli and others, Maurice_FrÃ©chet
introduced the metric_space in 1906.[8] A metric space is now considered a
special case of a general topological space, with any given topological space
potentially giving rise to many distinct metric spaces. In 1914, Felix
Hausdorff coined the term "topological space" and gave the definition for what
is now called a Hausdorff_space.[9] Currently, a topological space is a slight
generalization of Hausdorff spaces, given in 1922 by Kazimierz_Kuratowski.[10]
Modern topology depends strongly on the ideas of set theory, developed by Georg
Cantor in the later part of the 19th century. In addition to establishing the
basic ideas of set theory, Cantor considered point sets in Euclidean_space as
part of his study of Fourier_series. For further developments, see point-set
topology and algebraic topology.
***** Concepts[edit] *****
**** Topologies on sets[edit] ****
Main article: Topological_space
The term topology also refers to a specific mathematical idea central to the
area of mathematics called topology. Informally, a topology tells how elements
of a set relate spatially to each other. The same set can have different
topologies. For instance, the real_line, the complex_plane, and the Cantor_set
can be thought of as the same set with different topologies.
Formally, let X be a set and let Ï be a family of subsets of X. Then Ï is
called a topology on X if:
   1. Both the empty set and X are elements of Ï.
   2. Any union of elements of Ï is an element of Ï.
   3. Any intersection of finitely many elements of Ï is an element of Ï.
If Ï is a topology on X, then the pair (X, Ï) is called a topological space.
The notation XÏ may be used to denote a set X endowed with the particular
topology Ï.
The members of Ï are called open sets in X. A subset of X is said to be closed
if its complement is in Ï (i.e., its complement is open). A subset of X may be
open, closed, both (a clopen_set), or neither. The empty set and X itself are
always both closed and open. An open subset of X which contains a point x is
called a neighborhood of x.
**** Continuous functions and homeomorphisms[edit] ****
Main articles: Continuous_function and homeomorphism
A function or map from one topological space to another is called continuous if
the inverse image of any open set is open. If the function maps the real
numbers to the real numbers (both spaces with the standard topology), then this
definition of continuous is equivalent to the definition of continuous in
calculus. If a continuous function is one-to-one and onto, and if the inverse
of the function is also continuous, then the function is called a homeomorphism
and the domain of the function is said to be homeomorphic to the range. Another
way of saying this is that the function has a natural extension to the
topology. If two spaces are homeomorphic, they have identical topological
properties, and are considered topologically the same. The cube and the sphere
are homeomorphic, as are the coffee cup and the doughnut. But the circle is not
homeomorphic to the doughnut.
**** Manifolds[edit] ****
Main article: Manifold
While topological spaces can be extremely varied and exotic, many areas of
topology focus on the more familiar class of spaces known as manifolds. A
manifold is a topological space that resembles Euclidean space near each point.
More precisely, each point of an n-dimensional manifold has a neighborhood that
is homeomorphic to the Euclidean space of dimension n. Lines and circles, but
not figure_eights, are one-dimensional manifolds. Two-dimensional manifolds are
also called surfaces, although not all surfaces are manifolds. Examples include
the plane, the sphere, and the torus, which can all be realized without self-
intersection in three dimensions, and the Klein bottle and real_projective
plane, which cannot (that is, all their realizations are surfaces that are not
manifolds).
***** Topics[edit] *****
**** General topology[edit] ****
Main article: General_topology
General topology is the branch of topology dealing with the basic set-theoretic
definitions and constructions used in topology.[11][12] It is the foundation of
most other branches of topology, including differential topology, geometric
topology, and algebraic topology. Another name for general topology is point-
set topology.
The basic object of study is topological_spaces, which are sets equipped with a
topology, that is, a family of subsets, called open sets, which is closed under
finite intersections and (finite or infinite) unions. The fundamental concepts
of topology, such as continuity, compactness, and connectedness, can be defined
in terms of open sets. Intuitively, continuous functions take nearby points to
nearby points. Compact sets are those that can be covered by finitely many sets
of arbitrarily small size. Connected sets are sets that cannot be divided into
two pieces that are far apart. The words nearby, arbitrarily small, and far
apart can all be made precise by using open sets. Several topologies can be
defined on a given space. Changing a topology consists of changing the
collection of open sets, and this changes which functions are continuous, and
which subsets are compact or connected.
Metric_spaces are an important class of topological spaces where distances
between any two points are defined by a function called a metric. In a metric
space, an open set is a union of open disks, where an open disk of radius r
centered at x is the set of the points whose distance to x is less than d. Many
common spaces are topological space whose topology can be defined by a metric.
This is the case of the real_line, the complex_plane, real and complex vector
spaces and Euclidean_spaces. Having a metric simplifies many proofs.
**** Algebraic topology[edit] ****
Main article: Algebraic_topology
Algebraic topology is a branch of mathematics that uses tools from algebra to
study topological spaces.[13] The basic goal is to find algebraic invariants
that classify topological spaces up_to homeomorphism, though usually most
classify up to homotopy equivalence.
The most important of these invariants are homotopy_groups, homology, and
cohomology.
Although algebraic topology primarily uses algebra to study topological
problems, using topology to solve algebraic problems is sometimes also
possible. Algebraic topology, for example, allows for a convenient proof that
any subgroup of a free_group is again a free group.
**** Differential topology[edit] ****
Main article: Differential_topology
Differential topology is the field dealing with differentiable_functions on
differentiable_manifolds.[14] It is closely related to differential_geometry
and together they make up the geometric theory of differentiable manifolds.
More specifically, differential topology considers the properties and
structures that require only a smooth_structure on a manifold to be defined.
Smooth manifolds are 'softer' than manifolds with extra geometric structures,
which can act as obstructions to certain types of equivalences and deformations
that exist in differential topology. For instance, volume and Riemannian
curvature are invariants that can distinguish different geometric structures on
the same smooth manifoldâthat is, one can smoothly "flatten out" certain
manifolds, but it might require distorting the space and affecting the
curvature or volume.
**** Geometric topology[edit] ****
Main article: Geometric_topology
Geometric topology is a branch of topology that primarily focuses on low-
dimensional manifolds (i.e. spaces of dimensions 2, 3, and 4) and their
interaction with geometry, but it also includes some higher-dimensional
topology.[15][16] Some examples of topics in geometric topology are
orientability, handle_decompositions, local_flatness, crumpling and the planar
and higher-dimensional SchÃ¶nflies_theorem.
In high-dimensional topology, characteristic_classes are a basic invariant, and
surgery_theory is a key theory.
Low-dimensional topology is strongly geometric, as reflected in the
uniformization_theorem in 2 dimensions â every surface admits a constant
curvature metric; geometrically, it has one of 3 possible geometries: positive
curvature/spherical, zero curvature/flat, and negative curvature/hyperbolic â
and the geometrization_conjecture (now theorem) in 3 dimensions â every 3-
manifold can be cut into pieces, each of which has one of eight possible
geometries.
2-dimensional topology can be studied as complex_geometry in one variable
(Riemann surfaces are complex curves) â by the uniformization theorem every
conformal_class of metrics is equivalent to a unique complex one, and 4-
dimensional topology can be studied from the point of view of complex geometry
in two variables (complex surfaces), though not every 4-manifold admits a
complex structure.
**** Generalizations[edit] ****
Occasionally, one needs to use the tools of topology but a "set of points" is
not available. In pointless_topology one considers instead the lattice of open
sets as the basic notion of the theory,[17] while Grothendieck_topologies are
structures defined on arbitrary categories that allow the definition of sheaves
on those categories, and with that the definition of general cohomology
theories.[18]
***** Applications[edit] *****
**** Biology[edit] ****
Knot_theory, a branch of topology, is used in biology to study the effects of
certain enzymes on DNA. These enzymes cut, twist, and reconnect the DNA,
causing knotting with observable effects such as slower electrophoresis.[19]
Topology is also used in evolutionary_biology to represent the relationship
between phenotype and genotype.[20] Phenotypic forms that appear quite
different can be separated by only a few mutations depending on how genetic
changes map to phenotypic changes during development. In neuroscience,
topological quantities like the Euler characteristic and Betti number have been
used to measure the complexity of patterns of activity in neural networks.
**** Computer science[edit] ****
Topological_data_analysis uses techniques from algebraic topology to determine
the large scale structure of a set (for instance, determining if a cloud of
points is spherical or toroidal). The main method used by topological data
analysis is:
   1. Replace a set of data points with a family of simplicial_complexes,
      indexed by a proximity parameter.
   2. Analyse these topological complexes via algebraic topology â
      specifically, via the theory of persistent_homology.[21]
   3. Encode the persistent homology of a data set in the form of a
      parameterized version of a Betti_number, which is called a barcode.[21]
**** Physics[edit] ****
Topology is relevant to physics in areas such as condensed_matter_physics,[22]
quantum_field_theory and physical_cosmology.
The topological dependence of mechanical properties in solids is of interest in
disciplines of mechanical_engineering and materials_science. Electrical and
mechanical properties depend on the arrangement and network structures of
molecules and elementary units in materials.[23] The compressive_strength of
crumpled topologies is studied in attempts to understand the high strength to
weight of such structures that are mostly empty space.[24] Topology is of
further significance in Contact_mechanics where the dependence of stiffness and
friction on the dimensionality of surface structures is the subject of interest
with applications in multi-body physics.
A topological_quantum_field_theory (or topological field theory or TQFT) is a
quantum field theory that computes topological_invariants.
Although TQFTs were invented by physicists, they are also of mathematical
interest, being related to, among other things, knot_theory, the theory of
four-manifolds in algebraic topology, and to the theory of moduli_spaces in
algebraic geometry. Donaldson, Jones, Witten, and Kontsevich have all won
Fields_Medals for work related to topological field theory.
The topological classification of Calabi-Yau_manifolds has important
implications in string_theory, as different manifolds can sustain different
kinds of strings.[25]
In cosmology, topology can be used to describe the overall shape of the
universe.[26] This area of research is commonly known as spacetime_topology.
**** Robotics[edit] ****
The possible positions of a robot can be described by a manifold called
configuration_space.[27] In the area of motion_planning, one finds paths
between two points in configuration space. These paths represent a motion of
the robot's joints and other parts into the desired pose.[28]
**** Games and puzzles[edit] ****
Tanglement_puzzles are based on topological aspects of the puzzle's shapes and
components.[29][30][31][32]
**** Fiber art[edit] ****
In order to create a continuous join of pieces in a modular construction, it is
necessary to create an unbroken path in an order which surrounds each piece and
traverses each edge only once. This process is an application of the Eulerian
path.[33]
***** See also[edit] *****
    * [icon]Topology_portal
    * [icon]Mathematics_portal
    * Equivariant_topology
    * List_of_algebraic_topology_topics
    * List_of_examples_in_general_topology
    * List_of_general_topology_topics
    * List_of_geometric_topology_topics
    * List_of_topology_topics
    * Publications_in_topology
    * Topoisomer
    * Topology_glossary
    * Topological_geometry
    * Topological_order
***** References[edit] *****
**** Citations[edit] ****
   1. ^Hubbard, John H.; West, Beverly H. (1995). Differential_Equations:_A
      Dynamical_Systems_Approach._Part_II:_Higher-Dimensional_Systems. Texts in
      Applied Mathematics. 18. Springer. p. 204. ISBN 978-0-387-94377-0.
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
   3. ^ a b Croom_1989, p. 7
   4. ^ Richeson_2008, p. 63
   5. ^ Aleksandrov_1969, p. 204
   6. ^ a b c Richeson (2008)
   7. ^ Listing, Johann Benedict, "Vorstudien zur Topologie", Vandenhoeck und
      Ruprecht, GÃ¶ttingen, p. 67, 1848
   8. ^ Tait, Peter Guthrie, "Johann Benedict Listing (obituary)", Nature 27, 1
      February 1883, pp. 316â317
   9. ^FrÃ©chet, Maurice (1906). Sur quelques points du calcul fonctionnel. PhD
      dissertation. OCLC 8897542.
  10. ^ Hausdorff, Felix, "GrundzÃ¼ge der Mengenlehre", Leipzig: Veit. In
      (Hausdorff Werke, II (2002), 91â576)
  11. ^ Croom_1989, p. 129
  12. ^ Munkres, James R. Topology. Vol. 2. Upper Saddle River: Prentice Hall,
      2000.
  13. ^ Adams, Colin Conrad, and Robert David Franzosa. Introduction to
      topology: pure and applied. Pearson Prentice Hall, 2008.
  14. ^ Allen Hatcher, Algebraic_topology. (2002) Cambridge University Press,
      xii+544 pp. 
  15. ISBN 0-521-79160-X, 0-521-79540-0.
  16. ^Lee, John M. (2006). Introduction to Smooth Manifolds. Springer-Verlag.
      ISBN 978-0-387-95448-6.
  17. ^Budney, Ryan (2011). "What_is_geometric_topology?". mathoverflow.net.
      Retrieved 29 December 2013.
  18. ^ R.B. Sher and R.J. Daverman (2002), Handbook of Geometric Topology,
      North-Holland.
  19. ISBN 0-444-82432-4
  20. ^Johnstone,_Peter_T. (1983). "The_point_of_pointless_topology". Bulletin
      of the American Mathematical Society. 8 (1): 41â53. doi:10.1090/s0273-
      0979-1983-15080-2.
  21. ^Artin,_Michael (1962). Grothendieck topologies. Cambridge, MA: Harvard
      University, Dept. of Mathematics. Zbl 0208.48701.
  22. ^Adams,_Colin (2004). The Knot Book: An Elementary Introduction to the
      Mathematical Theory of Knots. American Mathematical Society. ISBN 978-0-
      8218-3678-1
  23. ^Stadler, BÃ¤rbel M.R.; Stadler, Peter F.; Wagner, GÃ¼nter P.; Fontana,
      Walter (2001). "The Topology of the Possible: Formal Spaces Underlying
      Patterns of Evolutionary Change". Journal of Theoretical Biology. 213
      (2): 241â274. CiteSeerX 10.1.1.63.7808. doi:10.1006/jtbi.2001.2423.
      PMID 11894994.
  24. ^ a bGunnar Carlsson (April 2009). "Topology_and_data" (PDF). Bulletin
      (New Series) of the American Mathematical Society. 46 (2): 255â308.
      doi:10.1090/S0273-0979-09-01249-X.
  25. ^"The_Nobel_Prize_in_Physics_2016". Nobel Foundation. 4 October 2016.
      Retrieved 12 October 2016.
  26. ^Stephenson, C.; et., al. (2017). "Topological_properties_of_a_self-
      assembled_electrical_network_via_ab_initio_calculation". Sci. Rep. 7:
      41621. Bibcode:2017NatSR...741621S. doi:10.1038/srep41621. PMC 5290745.
      PMID 28155863.
  27. ^Cambou, Anne Dominique; Narayanan, Menon (2011). "Three-dimensional
      structure_of_a_sheet_crumpled_into_a_ball". Proceedings of the National
      Academy of Sciences. 108 (36): 14741â14745. arXiv:1203.5826. Bibcode:
      2011PNAS..10814741C. doi:10.1073/pnas.1019192108. PMC 3169141.
      PMID 21873249.
  28. ^ Yau, S. & Nadis, S.; The Shape of Inner Space, Basic Books, 2010.
  29. ^ The Shape of Space: How to Visualize Surfaces and Three-dimensional
      Manifolds 2nd ed (Marcel Dekker, 1985,
  30. ISBN 0-8247-7437-X)
  31. ^ John J. Craig, Introduction to Robotics: Mechanics and Control, 3rd Ed.
      Prentice-Hall, 2004
  32. ^ Michael Farber, Invitation to Topological Robotics, European
      Mathematical Society, 2008
  33. ^ https://math.stackexchange.com How to reason about disentanglement
      puzzles.
  34. ^Horak, Mathew (2006). "Disentangling Topological Puzzles by Using Knot
      Theory". Mathematics Magazine. 79 (5): 368â375. doi:10.2307/27642974.
      JSTOR 27642974.
  35. .
  36. ^ http://sma.epfl.ch/Notes.pdf A Topological Puzzle, Inta Bertuccioni,
      December 2003.
  37. ^ https://www.futilitycloset.com/the-figure-8-puzzle The Figure Eight
      Puzzle, Science and Math, June 2012.
  38. ^ Eckman, Edie: Connect the shapes crochet motifs: creative techniques
      for joining motifs of all shapes. Â©2012 Storey Publishing
**** Bibliography[edit] ****
    * Aleksandrov, P.S. (1969) [1956], "Chapter XVIII Topology", in
      Aleksandrov, A.D.; Kolmogorov, A.N.; Lavrent'ev, M.A. (eds.), Mathematics
      / Its Content, Methods and Meaning (2nd ed.), The M.I.T. Press
Croom, Fred H. (1989), Principles of Topology, Saunders College Publishing,
ISBN 978-0-03-029804-2
Richeson, D. (2008), Euler's Gem: The Polyhedron Formula and the Birth of
Topology, Princeton University Press
***** Further reading[edit] *****
    * Ryszard_Engelking, General Topology, Heldermann Verlag, Sigma Series in
      Pure Mathematics, December 1989,
ISBN 3-88538-006-4.
Bourbaki; Elements of Mathematics: General Topology, AddisonâWesley (1966).
Breitenberger, E. (2006). "Johann Benedict Listing". In James, I.M. (ed.).
History of Topology. North Holland. ISBN 978-0-444-82375-5.
Kelley,_John_L. (1975). General Topology. Springer-Verlag. ISBN 978-0-387-
90125-1.
Brown,_Ronald (2006). Topology_and_Groupoids. Booksurge. ISBN 978-1-4196-2722-
4.
 (Provides a well motivated, geometric account of general topology, and shows
the use of groupoids in discussing van_Kampen's_theorem, covering_spaces, and
orbit_spaces.)
WacÅaw_SierpiÅski, General Topology, Dover Publications, 2000,
ISBN 0-486-41148-6
Pickover,_Clifford_A. (2006). The MÃ¶bius Strip: Dr. August MÃ¶bius's Marvelous
Band in Mathematics, Games, Literature, Art, Technology, and Cosmology.
Thunder's Mouth Press. ISBN 978-1-56025-826-1.
 (Provides a popular introduction to topology and geometry)
Gemignani, Michael C. (1990) [1967], Elementary Topology (2nd ed.), Dover
Publications Inc., ISBN 978-0-486-66522-1
***** External links[edit] *****
 Wikimedia Commons has media related to Topology.
 Wikiquote has quotations related to: Topology
 Wikibooks has more on the topic of: Topology
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Topology,_general", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Elementary_Topology:_A_First_Course Viro, Ivanov, Netsvetaev, Kharlamov.
Topology at Curlie
The_Topological_Zoo at The_Geometry_Center.
Topology_Atlas
Topology_Course_Lecture_Notes Aisling McCluskey and Brian McMaster, Topology
Atlas.
Topology_Glossary
Moscow_1935:_Topology_moving_towards_America, a historical essay by Hassler
Whitney.
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
    * v
    * t
    * e
Areas_of_mathematics
                  * Category_theory
                  * Information_theory
Foundations       * Mathematical_logic
                  * Philosophy_of_mathematics
                  * Set_theory
                  * Abstract
Algebra           * Elementary
                  * Linear
                  * Multilinear
                  * Calculus
                  * Real_analysis
Analysis          * Complex_analysis
                  * Differential_equations
                  * Functional_analysis
                  * Combinatorics
Discrete          * Graph_theory
                  * Order_theory
                  * Game_theory
                  * Algebraic
                  * Analytic
Geometry          * Differential
                  * Discrete
                  * Euclidean
                  * Finite
                  * Arithmetic
Number_theory     * Algebraic_number_theory
                  * Analytic_number_theory
                  * Diophantine_geometry
                  * Algebraic
Topology          * Differential
                  * Geometric
                  * Control_theory
                  * Mathematical_economics
                  * Mathematical_finance
Applied           * Mathematical_physics
                  * Mathematical_statistics
                  * Probability
                  * Statistics
                  * Computer_science
                  * Theory_of_computation
Computational     * Numerical_analysis
                  * Optimization
                  * Computer_algebra
                  * History_of_mathematics
Others            * Recreational_mathematics
                  * Mathematics_and_art
                  * Mathematics_education
    * [Category] Category
    * [Portal] Portal
    * [Commons page]Commons
    * [WikiProject]WikiProject
Authority_control [Edit_this_at_Wikidata]     * GND: 4060425-1
                                              * NDL: 00573284

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Topology&oldid=903581937"
Categories:
    * Topology
    * Mathematical_structures
Hidden categories:
    * Articles_with_inconsistent_citation_formats
    * Articles_with_short_description
    * Use_dmy_dates_from_July_2012
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_July_2009
    * Articles_with_Curlie_links
    * Wikipedia_articles_with_GND_identifiers
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
    * Wikibooks
    * Wikiquote
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AragonÃ©s
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * à½à½¼à½à¼à½¡à½²à½
    * Bosanski
    * CatalÃ 
    * Ð§ÓÐ²Ð°ÑÐ»Ð°
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
    * Furlan
    * Gaeilge
    * Galego
    * è´èª
    * Ð¥Ð°Ð»ÑÐ¼Ð³
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Ido
    * Bahasa_Indonesia
    * Interlingua
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Kiswahili
    * Latina
    * LatvieÅ¡u
    * ÐÐµÐ·Ð³Ð¸
    * LietuviÅ³
    * Lingua_Franca_Nova
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * áá¼ááºáá¬áá¬áá¬
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Novial
    * Occitan
    * ÐÐ»ÑÐº_Ð¼Ð°ÑÐ¸Ð¹
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Ù¾ÙØ¬Ø§Ø¨Û
    * Patois
    * áá¶áá¶ááááá
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * Qaraqalpaqsha
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Sicilianu
    * à·à·à¶à·à¶½
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * TÃ¼rkmenÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * æè¨
    * Winaray
    * ××Ö´×××©
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 26 June 2019, at 14:58 (UTC).
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
