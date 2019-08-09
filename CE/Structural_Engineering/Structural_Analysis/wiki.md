The following text has been accessed from https://en.wikipedia.org/wiki/Structural_analysis at Thu Aug 8 23:49:27 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Structural analysis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about structural studies in engineering. For social-science
usage, see Structuralism. For other uses, see Structure_(disambiguation).
    * v
    * t
    * e
Mechanical failure modes
    * Buckling
    * Corrosion
    * Corrosion_fatigue
    * Creep
    * Fatigue
    * Fouling
    * Fracture
    * Hydrogen_embrittlement
    * Impact
    * Mechanical_overload
    * Stress_corrosion_cracking
    * Thermal_shock
    * Wear
    * Yielding
 This article needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be challenged
 and removed.
 Find sources: "Structural_analysis" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (December 2018)(Learn_how_and_when_to_remove_this_template_message)

Structural analysis is the determination of the effects of loads on physical
structures and their components. Structures subject to this type of analysis
include all that must withstand loads, such as buildings, bridges, vehicles,
furniture, attire, soil strata, prostheses and biological tissue. Structural
analysis employs the fields of applied_mechanics, materials_science and applied
mathematics to compute a structure's deformations, internal forces, stresses,
support reactions, accelerations, and stability. The results of the analysis
are used to verify a structure's fitness for use, often precluding physical
tests. Structural analysis is thus a key part of the engineering_design_of
structures.
⁰
***** Contents *****
    * 1_Structures_and_Loads
          o 1.1_Classification_of_structures
          o 1.2_Loads
    * 2_Analytical_methods
          o 2.1_Limitations
    * 3_Strength_of_materials_methods_(classical_methods)
          o 3.1_Example
                # 3.1.1_Method_of_Joints
                # 3.1.2_Method_of_Sections
                      # 3.1.2.1_Method_1:_Ignore_the_right_side
                      # 3.1.2.2_Method_2:_Ignore_the_left_side
    * 4_Elasticity_methods
    * 5_Methods_using_numerical_approximation
    * 6_Timeline
    * 7_See_also
    * 8_References
***** Structures and Loads[edit] *****
A structure refers to a body or system of connected parts used to support a
load. Important examples related to Civil_Engineering include buildings,
bridges, and towers; and in other branches of engineering, ship and aircraft
frames, tanks, pressure vessels, mechanical systems, and electrical supporting
structures are important. To design a structure, an engineer must account for
its safety, aesthetics, and serviceability, while considering economic and
environmental constraints. Other branches of engineering work on a wide variety
of non-building_structures.
**** Classification of structures[edit] ****
A structural system is the combination of structural elements and their
materials. It is important for a structural engineer to be able to classify a
structure by either its form or its function, by recognizing the various
elements composing that structure. The structural elements guiding the systemic
forces through the materials are not only such as a connecting rod, a truss, a
beam, or a column, but also a cable, an arch, a cavity or channel, and even an
angle, a surface structure, or a frame.
**** Loads[edit] ****
Main article: Structural_load
Once the dimensional requirement for a structure have been defined, it becomes
necessary to determine the loads the structure must support. Structural design,
therefore begins with specifying loads that act on the structure. The design
loading for a structure is often specified in building_codes. There are two
types of codes: general building codes and design codes, engineers must satisfy
all of the code's requirements in order for the structure to remain reliable.
There are two types of loads that structure engineering must encounter in the
design. The first type of loads are dead loads that consist of the weights of
the various structural members and the weights of any objects that are
permanently attached to the structure. For example, columns, beams, girders,
the floor slab, roofing, walls, windows, plumbing, electrical fixtures, and
other miscellaneous attachments. The second type of loads are live loads which
vary in their magnitude and location. There are many different types of live
loads like building loads, highway bridge loads, railroad bridge loads, impact
loads, wind loads, snow loads, earthquake loads, and other natural loads.
***** Analytical methods[edit] *****
To perform an accurate analysis a structural engineer must determine
information such as structural_loads, geometry, support conditions, and
material properties. The results of such an analysis typically include support
reactions, stresses and displacements. This information is then compared to
criteria that indicate the conditions of failure. Advanced structural analysis
may examine dynamic_response, stability and non-linear behavior. There are
three approaches to the analysis: the mechanics_of_materials approach (also
known as strength of materials), the elasticity_theory approach (which is
actually a special case of the more general field of continuum_mechanics), and
the finite_element approach. The first two make use of analytical formulations
which apply mostly simple linear elastic models, leading to closed-form
solutions, and can often be solved by hand. The finite element approach is
actually a numerical method for solving differential equations generated by
theories of mechanics such as elasticity theory and strength of materials.
However, the finite-element method depends heavily on the processing power of
computers and is more applicable to structures of arbitrary size and
complexity.
Regardless of approach, the formulation is based on the same three fundamental
relations: equilibrium, constitutive, and compatibility. The solutions are
approximate when any of these relations are only approximately satisfied, or
only an approximation of reality.
**** Limitations[edit] ****
Each method has noteworthy limitations. The method of mechanics of materials is
limited to very simple structural elements under relatively simple loading
conditions. The structural elements and loading conditions allowed, however,
are sufficient to solve many useful engineering problems. The theory of
elasticity allows the solution of structural elements of general geometry under
general loading conditions, in principle. Analytical solution, however, is
limited to relatively simple cases. The solution of elasticity problems also
requires the solution of a system of partial differential equations, which is
considerably more mathematically demanding than the solution of mechanics of
materials problems, which require at most the solution of an ordinary
differential equation. The finite element method is perhaps the most
restrictive and most useful at the same time. This method itself relies upon
other structural theories (such as the other two discussed here) for equations
to solve. It does, however, make it generally possible to solve these
equations, even with highly complex geometry and loading conditions, with the
restriction that there is always some numerical error. Effective and reliable
use of this method requires a solid understanding of its limitations.
***** Strength of materials methods (classical methods)[edit] *****
The simplest of the three methods here discussed, the mechanics of materials
method is available for simple structural members subject to specific loadings
such as axially loaded bars, prismatic beams in a state of pure_bending, and
circular shafts subject to torsion. The solutions can under certain conditions
be superimposed using the superposition_principle to analyze a member
undergoing combined loading. Solutions for special cases exist for common
structures such as thin-walled pressure vessels.
For the analysis of entire systems, this approach can be used in conjunction
with statics, giving rise to the method of sections and method of joints for
truss analysis, moment_distribution_method for small rigid frames, and portal
frame and cantilever method for large rigid frames. Except for moment
distribution, which came into use in the 1930s, these methods were developed in
their current forms in the second half of the nineteenth century. They are
still used for small structures and for preliminary design of large structures.
The solutions are based on linear isotropic infinitesimal elasticity and
EulerâBernoulli beam theory. In other words, they contain the assumptions
(among others) that the materials in question are elastic, that stress is
related linearly to strain, that the material (but not the structure) behaves
identically regardless of direction of the applied load, that all deformations
are small, and that beams are long relative to their depth. As with any
simplifying assumption in engineering, the more the model strays from reality,
the less useful (and more dangerous) the result.
**** Example[edit] ****
There are 2 commonly used methods to find the truss element forces, namely the
Method of Joints and the Method of Sections. Below is an example that is solved
using both of these methods. The first diagram below is the presented problem
for which we need to find the truss element forces. The second diagram is the
loading diagram and contains the reaction forces from the joints.
      [Truss_Structure_Analysis,_Full_Figure2.jpg]
Since there is a pin joint at A, it will have 2 reaction forces. One in the x
direction and the other in the y direction. At point B, we have a roller joint
and hence we only have 1 reaction force in the y direction. Let us assume these
forces to be in their respective positive directions (if they are not in the
positive directions like we have assumed, then we will get a negative value for
them).
      [Truss_Structure_Analysis,_FBD2.jpg]
Since the system is in static equilibrium, the sum of forces in any direction
is zero and the sum of moments about any point is zero. Therefore, the
magnitude and direction of the reaction forces can be calculated.
         &#x2211;  M  A   = 0 = &#x2212; 10 &#x2217; 1 + 2 &#x2217;  R  B
      &#x21D2;  R  B   = 5   {\displaystyle \sum M_{A}=0=-10*1+2*R_
      {B}\Rightarrow R_{B}=5}  [\sum M_{A}=0=-10*1+2*R_{B}\Rightarrow R_{B}=5]
         &#x2211;  F  y   = 0 =  R  A y   +  R  B   &#x2212; 10 &#x21D2;  R  A
      y   = 5   {\displaystyle \sum F_{y}=0=R_{Ay}+R_{B}-10\Rightarrow R_
      {Ay}=5}  [\sum F_{y}=0=R_{{Ay}}+R_{B}-10\Rightarrow R_{{Ay}}=5]
         &#x2211;  F  x   = 0 =  R  A x     {\displaystyle \sum F_{x}=0=R_{Ax}}
      [\sum F_{x}=0=R_{{Ax}}]
*** Method of Joints[edit] ***
This type of method uses the force balance in the x and y directions at each of
the joints in the truss structure.
      [Truss_Structure_Analysis,_Method_of_Joints2.png]
At A,
         &#x2211;  F  y   = 0 =  R  A y   +  F  A D   sin &#x2061; ( 60 ) = 5 +
      F  A D      3  2   &#x21D2;  F  A D   = &#x2212;   10  3
      {\displaystyle \sum F_{y}=0=R_{Ay}+F_{AD}\sin(60)=5+F_{AD}{\frac {\sqrt
      {3}}{2}}\Rightarrow F_{AD}=-{\frac {10}{\sqrt {3}}}}  [\sum F_{y}=0=R_{
      {Ay}}+F_{{AD}}\sin(60)=5+F_{{AD}}{\frac  {{\sqrt  {3}}}{2}}\Rightarrow F_
      {{AD}}=-{\frac  {10}{{\sqrt  {3}}}}]
         &#x2211;  F  x   = 0 =  R  A x   +  F  A D   cos &#x2061; ( 60 ) +  F
      A B   = 0 &#x2212;   10  3      1 2   +  F  A B   &#x21D2;  F  A B   =
      5  3      {\displaystyle \sum F_{x}=0=R_{Ax}+F_{AD}\cos(60)+F_{AB}=0-
      {\frac {10}{\sqrt {3}}}{\frac {1}{2}}+F_{AB}\Rightarrow F_{AB}={\frac {5}
      {\sqrt {3}}}}  [\sum F_{x}=0=R_{{Ax}}+F_{{AD}}\cos(60)+F_{{AB}}=0-{\frac
      {10}{{\sqrt  {3}}}}{\frac  {1}{2}}+F_{{AB}}\Rightarrow F_{{AB}}={\frac
      {5}{{\sqrt  {3}}}}]
At D,
         &#x2211;  F  y   = 0 = &#x2212; 10 &#x2212;  F  A D   sin &#x2061;
      ( 60 ) &#x2212;  F  B D   sin &#x2061; ( 60 ) = &#x2212; 10 &#x2212;
      (  &#x2212;   10  3     )     3  2   &#x2212;  F  B D      3  2
      &#x21D2;  F  B D   = &#x2212;   10  3      {\displaystyle \sum F_{y}=0=-
      10-F_{AD}\sin(60)-F_{BD}\sin(60)=-10-\left(-{\frac {10}{\sqrt
      {3}}}\right){\frac {\sqrt {3}}{2}}-F_{BD}{\frac {\sqrt {3}}
      {2}}\Rightarrow F_{BD}=-{\frac {10}{\sqrt {3}}}}  [\sum F_{y}=0=-10-F_{
      {AD}}\sin(60)-F_{{BD}}\sin(60)=-10-\left(-{\frac  {10}{{\sqrt
      {3}}}}\right){\frac  {{\sqrt  {3}}}{2}}-F_{{BD}}{\frac  {{\sqrt  {3}}}
      {2}}\Rightarrow F_{{BD}}=-{\frac  {10}{{\sqrt  {3}}}}]
         &#x2211;  F  x   = 0 = &#x2212;  F  A D   cos &#x2061; ( 60 ) +  F  B
      D   cos &#x2061; ( 60 ) +  F  C D   = &#x2212;   10  3      1 2   +   10
      3      1 2   +  F  C D   &#x21D2;  F  C D   = 0   {\displaystyle \sum F_
      {x}=0=-F_{AD}\cos(60)+F_{BD}\cos(60)+F_{CD}=-{\frac {10}{\sqrt {3}}}
      {\frac {1}{2}}+{\frac {10}{\sqrt {3}}}{\frac {1}{2}}+F_{CD}\Rightarrow F_
      {CD}=0}  [\sum F_{x}=0=-F_{{AD}}\cos(60)+F_{{BD}}\cos(60)+F_{{CD}}=-
      {\frac  {10}{{\sqrt  {3}}}}{\frac  {1}{2}}+{\frac  {10}{{\sqrt  {3}}}}
      {\frac  {1}{2}}+F_{{CD}}\Rightarrow F_{{CD}}=0]
At C,
         &#x2211;  F  y   = 0 = &#x2212;  F  B C   &#x21D2;  F  B C   = 0
      {\displaystyle \sum F_{y}=0=-F_{BC}\Rightarrow F_{BC}=0}  [\sum F_{y}=0=-
      F_{{BC}}\Rightarrow F_{{BC}}=0]
Although we have found the forces in each of the truss elements, it is a good
practice to verify the results by completing the remaining force balances.
         &#x2211;  F  x   = &#x2212;  F  C D   = &#x2212; 0 = 0 &#x21D2; v e r
      i f i e d   {\displaystyle \sum F_{x}=-F_{CD}=-0=0\Rightarrow verified}
      [\sum F_{x}=-F_{{CD}}=-0=0\Rightarrow verified]
At B,
         &#x2211;  F  y   =  R  B   +  F  B D   sin &#x2061; ( 60 ) +  F  B C
      = 5 +  (  &#x2212;   10  3     )     3  2   + 0 = 0 &#x21D2; v e r i f i
      e d   {\displaystyle \sum F_{y}=R_{B}+F_{BD}\sin(60)+F_{BC}=5+\left(-
      {\frac {10}{\sqrt {3}}}\right){\frac {\sqrt {3}}{2}}+0=0\Rightarrow
      verified}  [\sum F_{y}=R_{B}+F_{{BD}}\sin(60)+F_{{BC}}=5+\left(-{\frac
      {10}{{\sqrt  {3}}}}\right){\frac  {{\sqrt  {3}}}{2}}+0=0\Rightarrow
      verified]
         &#x2211;  F  x   = &#x2212;  F  A B   &#x2212;  F  B D   cos &#x2061;
      ( 60 ) =   5  3    &#x2212;   10  3      1 2   = 0 &#x21D2; v e r i f i e
      d   {\displaystyle \sum F_{x}=-F_{AB}-F_{BD}\cos(60)={\frac {5}{\sqrt
      {3}}}-{\frac {10}{\sqrt {3}}}{\frac {1}{2}}=0\Rightarrow verified}  [\sum
      F_{x}=-F_{{AB}}-F_{{BD}}\cos(60)={\frac  {5}{{\sqrt  {3}}}}-{\frac  {10}{
      {\sqrt  {3}}}}{\frac  {1}{2}}=0\Rightarrow verified]
*** Method of Sections[edit] ***
** Method 1: Ignore the right side[edit] **
      [Truss_Structure_Analysis,_Method_of_Sections_Left2.jpg]
         &#x2211;  M  D   = 0 = &#x2212; 5 &#x2217; 1 +   3   &#x2217;  F  A B
      &#x21D2;  F  A B   =   5  3      {\displaystyle \sum M_{D}=0=-5*1+{\sqrt
      {3}}*F_{AB}\Rightarrow F_{AB}={\frac {5}{\sqrt {3}}}}  [\sum M_{D}=0=-
      5*1+{\sqrt  {3}}*F_{{AB}}\Rightarrow F_{{AB}}={\frac  {5}{{\sqrt  {3}}}}]
         &#x2211;  F  y   = 0 =  R  A y   &#x2212;  F  B D   sin &#x2061; ( 60
      ) &#x2212; 10 = 5 &#x2212;  F  B D      3  2   &#x2212; 10 &#x21D2;  F  B
      D   = &#x2212;   10  3      {\displaystyle \sum F_{y}=0=R_{Ay}-F_{BD}\sin
      (60)-10=5-F_{BD}{\frac {\sqrt {3}}{2}}-10\Rightarrow F_{BD}=-{\frac {10}
      {\sqrt {3}}}}  [\sum F_{y}=0=R_{{Ay}}-F_{{BD}}\sin(60)-10=5-F_{{BD}}
      {\frac  {{\sqrt  {3}}}{2}}-10\Rightarrow F_{{BD}}=-{\frac  {10}{{\sqrt
      {3}}}}]
         &#x2211;  F  x   = 0 =  F  A B   +  F  B D   cos &#x2061; ( 60 ) +  F
      C D   =   5  3    &#x2212;   10  3      1 2   +  F  C D   &#x21D2;  F  C
      D   = 0   {\displaystyle \sum F_{x}=0=F_{AB}+F_{BD}\cos(60)+F_{CD}={\frac
      {5}{\sqrt {3}}}-{\frac {10}{\sqrt {3}}}{\frac {1}{2}}+F_{CD}\Rightarrow
      F_{CD}=0}  [\sum F_{x}=0=F_{{AB}}+F_{{BD}}\cos(60)+F_{{CD}}={\frac  {5}{
      {\sqrt  {3}}}}-{\frac  {10}{{\sqrt  {3}}}}{\frac  {1}{2}}+F_{
      {CD}}\Rightarrow F_{{CD}}=0]
** Method 2: Ignore the left side[edit] **
      [Truss_Structure_Analysis,_Method_of_Sections_Right2.jpg]
         &#x2211;  M  B   = 0 =   3   &#x2217;  F  C D   &#x21D2;  F  C D   = 0
      {\displaystyle \sum M_{B}=0={\sqrt {3}}*F_{CD}\Rightarrow F_{CD}=0}
      [\sum M_{B}=0={\sqrt  {3}}*F_{{CD}}\Rightarrow F_{{CD}}=0]
         &#x2211;  F  y   = 0 =  F  B D   sin &#x2061; ( 60 ) +  R  B   =  F  B
      D      3  2   + 5 &#x21D2;  F  B D   = &#x2212;   10  3
      {\displaystyle \sum F_{y}=0=F_{BD}\sin(60)+R_{B}=F_{BD}{\frac {\sqrt {3}}
      {2}}+5\Rightarrow F_{BD}=-{\frac {10}{\sqrt {3}}}}  [\sum F_{y}=0=F_{
      {BD}}\sin(60)+R_{B}=F_{{BD}}{\frac  {{\sqrt  {3}}}{2}}+5\Rightarrow F_{
      {BD}}=-{\frac  {10}{{\sqrt  {3}}}}]
         &#x2211;  F  x   = 0 = &#x2212;  F  A B   &#x2212;  F  B D   cos
      &#x2061; ( 60 ) &#x2212;  F  C D   = &#x2212;  F  A B   &#x2212;
      (  &#x2212;   10  3     )    1 2   &#x2212; 0 &#x21D2;  F  A B   =   5  3
      {\displaystyle \sum F_{x}=0=-F_{AB}-F_{BD}\cos(60)-F_{CD}=-F_{AB}-\left(-
      {\frac {10}{\sqrt {3}}}\right){\frac {1}{2}}-0\Rightarrow F_{AB}={\frac
      {5}{\sqrt {3}}}}  [\sum F_{x}=0=-F_{{AB}}-F_{{BD}}\cos(60)-F_{{CD}}=-F_{
      {AB}}-\left(-{\frac  {10}{{\sqrt  {3}}}}\right){\frac  {1}{2}}-
      0\Rightarrow F_{{AB}}={\frac  {5}{{\sqrt  {3}}}}]
The truss elements forces in the remaining members can be found by using the
above method with a section passing through the remaining members.
***** Elasticity methods[edit] *****
Elasticity methods are available generally for an elastic solid of any shape.
Individual members such as beams, columns, shafts, plates and shells may be
modeled. The solutions are derived from the equations of linear_elasticity. The
equations of elasticity are a system of 15 partial differential equations. Due
to the nature of the mathematics involved, analytical solutions may only be
produced for relatively simple geometries. For complex geometries, a numerical
solution method such as the finite element method is necessary.
***** Methods using numerical approximation[edit] *****
It is common practice to use approximate solutions of differential equations as
the basis for structural analysis. This is usually done using numerical
approximation techniques. The most commonly used numerical approximation in
structural analysis is the Finite_Element_Method.
The finite element method approximates a structure as an assembly of elements
or components with various forms of connection between them and each element of
which has an associated stiffness. Thus, a continuous system such as a plate or
shell is modeled as a discrete system with a finite number of elements
interconnected at finite number of nodes and the overall stiffness is the
result of the addition of the stiffness of the various elements. The behaviour
of individual elements is characterized by the element's stiffness (or
flexibility) relation. The assemblage of the various stiffness's into a master
stiffness matrix that represents the entire structure leads to the system's
stiffness or flexibility relation. To establish the stiffness (or flexibility)
of a particular element, we can use the mechanics of materials approach for
simple one-dimensional bar elements, and the elasticity approach for more
complex two- and three-dimensional elements. The analytical and computational
development are best effected throughout by means of matrix_algebra, solving
partial_differential_equations.
Early applications of matrix methods were applied to articulated frameworks
with truss, beam and column elements; later and more advanced matrix methods,
referred to as "finite_element_analysis", model an entire structure with one-,
two-, and three-dimensional elements and can be used for articulated systems
together with continuous systems such as a pressure_vessel, plates, shells, and
three-dimensional solids. Commercial computer software for structural analysis
typically uses matrix finite-element analysis, which can be further classified
into two main approaches: the displacement or stiffness_method and the force or
flexibility_method. The stiffness method is the most popular by far thanks to
its ease of implementation as well as of formulation for advanced applications.
The finite-element technology is now sophisticated enough to handle just about
any system as long as sufficient computing power is available. Its
applicability includes, but is not limited to, linear and non-linear analysis,
solid and fluid interactions, materials that are isotropic, orthotropic, or
anisotropic, and external effects that are static, dynamic, and environmental
factors. This, however, does not imply that the computed solution will
automatically be reliable because much depends on the model and the reliability
of the data input.
***** Timeline[edit] *****
    * 1452â1519 Leonardo_da_Vinci made many contributions
    * 1638: Galileo_Galilei published the book "Two_New_Sciences" in which he
      examined the failure of simple structures
    * 1660: Hooke's_law by Robert_Hooke
    * 1687: Isaac_Newton published "Philosophiae_Naturalis_Principia
      Mathematica" which contains the Newton's_laws_of_motion
    * 1750: EulerâBernoulli_beam_equation
    * 1700â1782: Daniel_Bernoulli introduced the principle of virtual_work
    * 1707â1783: Leonhard_Euler developed the theory of buckling of columns
    * 1826: Claude-Louis_Navier published a treatise on the elastic behaviors
      of structures
    * 1873: Carlo_Alberto_Castigliano presented his dissertation "Intorno ai
      sistemi elastici", which contains his_theorem for computing displacement
      as partial derivative of the strain energy. This theorem includes the
      method of 'least work' as a special case
    * 1936: Hardy_Cross' publication of the moment distribution method which
      was later recognized as a form of the relaxation method applicable to the
      problem of flow in pipe-network
    * 1941: Alexander_Hrennikoff submitted his D.Sc thesis in MIT on the
      discretization of plane elasticity problems using a lattice framework
    * 1942: R._Courant divided a domain into finite subregions
    * 1956: J. Turner, R._W._Clough, H. C. Martin, and L. J. Topp's paper on
      the "Stiffness and Deflection of Complex Structures" introduces the name
      "finite-element method" and is widely recognized as the first
      comprehensive treatment of the method as it is known today
***** See also[edit] *****
    * Limit_state_design
    * Structural_engineering_theory
    * Structural_integrity_and_failure
    * Stressâstrain_analysis
    * Probabilistic_Assessment_of_Structures
***** References[edit] *****
 Wikibooks has more on the topic of: Structural_analysis
 Wikiversity has learning resources about Structural_analysis

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Structural_analysis&oldid=885089959"
Categories:
    * Structural_analysis
Hidden categories:
    * Articles_needing_additional_references_from_December_2018
    * All_articles_needing_additional_references
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
    * Alemannisch
    * á áá­á
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * à´®à´²à´¯à´¾à´³à´
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 25 February 2019, at 22:11 (UTC).
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
