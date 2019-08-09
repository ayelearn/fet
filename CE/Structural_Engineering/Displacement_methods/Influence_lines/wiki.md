The following text has been accessed from https://en.wikipedia.org/wiki/Influence_line at Thu Aug 8 23:48:51 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Influence line ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
[A_simply_supported_beam_and_four_different_influence_lines.]
Figure 1: (a) This simple supported beam is shown with a unit load placed a
distance x from the left end. Its influence lines for four different functions:
(b) the reaction at the left support (denoted A), (c) the reaction at the right
support (denoted C), (d) one for shear at a point B along the beam, and (e) one
for moment also at point B.
In engineering, an influence line graphs the variation of a function (such as
the shear felt in a structure member) at a specific point on a beam or truss
caused by a unit load placed at any point along the structure.[1][2][3][4][5]
Some of the common functions studied with influence lines include reactions
(the forces that the structureâs supports must apply in order for the
structure to remain static), shear, moment, and deflection (Deformation) [6].
Influence lines are important in designing beams and trusses used in bridges,
crane rails, conveyor_belts, floor girders, and other structures where loads
will move along their span.[5] The influence lines show where a load will
create the maximum effect for any of the functions studied.
Influence lines are both scalar and additive.[5] This means that they can be
used even when the load that will be applied is not a unit load or if there are
multiple loads applied. To find the effect of any non-unit load on a structure,
the ordinate results obtained by the influence line are multiplied by the
magnitude of the actual load to be applied. The entire influence line can be
scaled, or just the maximum and minimum effects experienced along the line. The
scaled maximum and minimum are the critical magnitudes that must be designed
for in the beam or truss.
In cases where multiple loads may be in effect, the influence lines for the
individual loads may be added together in order to obtain the total effect felt
by the structure at a given point. When adding the influence lines together, it
is necessary to include the appropriate offsets due to the spacing of loads
across the structure. For example, a truck load is applied to the structure.
Rear axle, B, is three feet behind front axle, A, then the effect of A at x
feet along the structure must be added to the effect of B at (x â 3) feet
along the structureânot the effect of B at x feet along the structure.
Many loads are distributed rather than concentrated. Influence lines can be
used with either concentrated or distributed loadings. For a concentrated (or
point) load, a unit point load is moved along the structure. For a distributed
load of a given width, a unit-distributed load of the same width is moved along
the structure, noting that as the load nears the ends and moves off the
structure only part of the total load is carried by the structure. The effect
of the distributed unit load can also be obtained by integrating the point
loadâs influence line over the corresponding length of the structures.
⁰
***** Contents *****
    * 1_Demonstration_from_Betti's_theorem
    * 2_Concept
    * 3_Methods_for_constructing_influence_lines
          o 3.1_Tabulate_values
          o 3.2_Influence-line_equations
          o 3.3_MÃ¼ller-Breslau's_Principle
    * 4_Alternate_loading_cases
          o 4.1_Multiple_loads
          o 4.2_Distributed_loads
    * 5_Indeterminate_structures
    * 6_See_also
    * 7_References
***** Demonstration from Betti's theorem[edit] *****
Influence lines are based on Betti's_theorem. From there, consider two external
force systems,      F  i   P     {\displaystyle F_{i}^{P}}  [F_{i}^{P}] and
F  i   Q     {\displaystyle F_{i}^{Q}}  [F_{i}^{Q}], each one associated with a
displacement field whose displacements measured in the force's point of
application are represented by      d  i   P     {\displaystyle d_{i}^{P}}  [d_
{i}^{P}] and      d  i   Q     {\displaystyle d_{i}^{Q}}  [d_{i}^{Q}].
Consider that the      F  i   P     {\displaystyle F_{i}^{P}}  [F_{i}^{P}]
system represents actual forces applied to the structure, which are in
equilibrium. Consider that the      F  i   Q     {\displaystyle F_{i}^{Q}}  [F_
{i}^{Q}] system is formed by a single force,      F  Q     {\displaystyle F^
{Q}}  [F^{Q}]. The displacement field      d  i   Q     {\displaystyle d_{i}^
{Q}}  [d_{i}^{Q}] associated with this forced is defined by releasing the
structural restraints acting on the point where      F  Q     {\displaystyle F^
{Q}}  [F^{Q}] is applied and imposing a relative unit displacement which is
kinematically admissible in the negative direction, represented as      d  1
Q   = &#x2212; 1   {\displaystyle d_{1}^{Q}=-1}  [d_{1}^{Q}=-1]. From Betti's
theorem, we obtain the following result:
   &#x2212;  F  1   P   +  &#x2211;  i = 2   n    F  i   P    d  i   Q   =  F
Q   &#x00D7; 0  &#x27FA;   F  1   P   =  &#x2211;  i = 2   n    F  i   P    d
i   Q     {\displaystyle -F_{1}^{P}+\sum _{i=2}^{n}F_{i}^{P}d_{i}^{Q}=F^
{Q}\times 0\iff F_{1}^{P}=\sum _{i=2}^{n}F_{i}^{P}d_{i}^{Q}}  [-F_{1}^{P}+\sum
_{{i=2}}^{n}F_{i}^{P}d_{i}^{Q}=F^{Q}\times 0\iff F_{1}^{P}=\sum _{{i=2}}^{n}F_
{i}^{P}d_{i}^{Q}]
***** Concept[edit] *****
When designing a beam or truss, it is necessary to design for the scenarios
causing the maximum expected reactions, shears, and moments within the
structure members in order to ensure that no member will fail during the life
of the structure. When dealing with dead_loads (loads that never move, such as
the weight of the structure itself), this is relatively easy because the loads
are easy to predict and plan for. For live_loads (any load that will be moved
during the life of the structure, such as furniture and people), it becomes
much harder to predict where the loads will be or how concentrated or
distributed they will be throughout the life of the structure.
Influence lines graph the response of a beam or truss as a unit load travels
across it. The influence line allows the designers to discover quickly where to
place a live load in order to calculate the maximum resulting response for each
of the following functions: reaction, shear, or moment. The designer can then
scale the influence line by the greatest expected load to calculate the maximum
response of each function for which the beam or truss must be designed.
Influence lines can also be used to find the responses of other functions (such
as deflection or axial force) to the applied unit load, but these uses of
influence lines are less common.
***** Methods for constructing influence lines[edit] *****
There are three methods used for constructing the influence line. The first is
to tabulate the influence values for multiple points along the structure, then
use those points to create the influence line.[5] The second is to determine
the influence-line equations that apply to the structure, thereby solving for
all points along the influence line in terms of x, where x is the number of
feet from the start of the structure to the point where the unit load is
applied.[1][2][3][4][5] The third method is called the MÃ¼ller-Breslau's
principle. It creates a qualitative influence line.[1][2][5] This influence
line will still provide the designer with an accurate idea of where the unit
load will produce the largest response of a function at the point being
studied, but it cannot be used directly to calculate what the magnitude that
response will be, whereas the influence lines produced by the first two methods
can.
**** Tabulate values[edit] ****
In order to tabulate the influence values with respect to some point A on the
structure, a unit load must be placed at various points along the structure.
Statics is used to calculate what the value of the function (reaction, shear,
or moment) is at point A. Typically an upwards reaction is seen as positive.
Shear and moments are given positive or negative values according to the same
conventions used for shear_and_moment_diagrams.
R. C. Hibbeler states, in his book Structural Analysis, âAll statically
determinate beams will have influence lines that consist of straight line
segments.â[5] Therefore, it is possible to minimize the number of
computations by recognizing the points that will cause a change in the slope of
the influence line and only calculating the values at those points. The slope
of the inflection line can change at supports, mid-spans, and joints.
An influence line for a given function, such as a reaction, axial force, shear
force, or bending moment, is a graph that shows the variation of that function
at any given point on a structure due to the application of a unit load at any
point on the structure.
An influence line for a function differs from a shear, axial, or bending moment
diagram. Influence lines can be generated by independently applying a unit load
at several points on a structure and determining the value of the function due
to this load, i.e. shear, axial, and moment at the desired location. The
calculated values for each function are then plotted where the load was applied
and then connected together to generate the influence line for the function.
Once the influence values have been tabulated, the influence line for the
function at point A can be drawn in terms of x. First, the tabulated values
must be located. For the sections in between the tabulated points,
interpolation is required. Therefore, straight lines may be drawn to connect
the points. Once this is done, the influence line is complete.
**** Influence-line equations[edit] ****
It is possible to create equations defining the influence line across the
entire span of a structure. This is done by solving for the reaction, shear, or
moment at the point A caused by a unit load placed at x feet along the
structure instead of a specific distance. This method is similar to the
tabulated values method, but rather than obtaining a numeric solution, the
outcome is an equation in terms of x.[5]
It is important to understanding where the slope of the influence line changes
for this method because the influence-line equation will change for each linear
section of the influence line. Therefore, the complete equation will be a
piecewise_linear_function which has a separate influence-line equation for each
linear section of the influence line.[5]
**** MÃ¼ller-Breslau's Principle[edit] ****
According to www.public.iastate.edu, âThe_MÃ¼ller-Breslau_Principle can be
utilized to draw qualitative influence lines, which are directly proportional
to the actual influence line.â[2] Instead of moving a unit load along a beam,
the MÃ¼ller-Breslau Principle finds the deflected shape of the beam caused by
first releasing the beam at the point being studied, and then applying the
function (reaction, shear, or moment) being studied to that point. The
principle states that the influence line of a function will have a scaled shape
that is the same as the deflected shape of the beam when the beam is acted upon
by the function.
In order to understand how the beam will deflect under the function, it is
necessary to remove the beamâs capacity to resist the function. Below are
explanations of how to find the influence lines of a simply supported, rigid
beam (such as the one displayed in Figure 1).
          * When determining the reaction caused at a support, the support is
            replaced with a roller, which cannot resist a vertical reaction.[2]
            [5] Then an upward (positive) reaction is applied to the point
            where the support was. Since the support has been removed, the beam
            will rotate upwards, and since the beam is rigid, it will create a
            triangle with the point at the second support. If the beam extends
            beyond the second support as a cantilever, a similar triangle will
            be formed below the cantilevers position. This means that the
            reactionâs influence line will be a straight, sloping line with a
            value of zero at the location of the second support.
          * When determining the shear caused at some point B along the beam,
            the beam must be cut and a roller-guide (which is able to resist
            moments but not shear) must be inserted at point B.[2][5] Then, by
            applying a positive shear to that point, it can be seen that the
            left side will rotate down, but the right side will rotate up. This
            creates a discontinuous influence line which reaches zero at the
            supports and whose slope is equal on either side of the
            discontinuity. If point B is at a support, then the deflection
            between point B and any other supports will still create a
            triangle, but if the beam is cantilevered, then the entire
            cantilevered side will move up or down creating a rectangle.
          * When determining the moment caused by at some point B along the
            beam, a hinge will be placed at point B, releasing it to moments
            but resisting shear.[2][5] Then when a positive moment is placed at
            point B, both sides of the beam will rotate up. This will create a
            continuous influence line, but the slopes will be equal and
            opposite on either side of the hinge at point B. Since the beam is
            simply supported, its end supports (pins) cannot resist moment;
            therefore, it can be observed that the supports will never
            experience moments in a static situation regardless of where the
            load is placed.
The MÃ¼ller-Breslau Principle can only produce qualitative influence lines.[2]
[5] This means that engineers can use it to determine where to place a load to
incur the maximum of a function, but the magnitude of that maximum cannot be
calculated from the influence line. Instead, the engineer must use statics to
solve for the functions value in that loading case.
***** Alternate loading cases[edit] *****
**** Multiple loads[edit] ****
The simplest loading case is a single point load, but influence lines can also
be used to determine responses due to multiple loads and distributed loads.
Sometimes it is known that multiple loads will occur at some fixed distance
apart. For example, on a bridge the wheels of cars or trucks create point loads
that act at relatively standard distances.
In order to calculate the response of a function to all of these point loads
using an influence line, the results found with the influence line can be
scaled for each load, and then the scaled magnitudes can be summed to find the
total response that the structure must withstand.[5] The point loads can have
different magnitudes themselves, but even if they apply the same force to the
structure, it will be necessary to scale them separately because they act at
different distances along the structure. For example, if a car's wheels are 10
feet apart, then when the first set is 13 feet onto the bridge, the second set
will be only 3 feet onto the bridge. If the first set of wheels is 7 feet onto
the bridge, the second set has not yet reached the bridge, and therefore only
the first set is placing a load on the bridge.
Also, if, between two loads, one of the loads is heavier, the loads must be
examined in both loading orders (the larger load on the right and the larger
load on the left) to ensure that the maximum load is found. If there are three
or more loads, then the number of cases to be examined will increase.
**** Distributed loads[edit] ****
Many loads do not act as point loads, but instead act over an extended length
or area as distributed loads. For example, a tractor with continuous_tracks
will apply a load distributed over the length of each track.
In order to find the effect of a distributed load, the designer can integrate
an influence line, found using a point load, over the affected distance of the
structure.[5] For example, if a three-foot-long track acts between 5 feet and 8
feet along a beam, the influence line of that beam must be integrated between 5
and 8 feet. The integration of the influence line gives the effect that would
be felt if the distributed load had a unit magnitude. Therefore, after
integrating, the designer must still scale the results to get the actual effect
of the distributed load.
***** Indeterminate structures[edit] *****
While the influence lines of statically determinate structures (as mentioned
above) are made up of straight line segments, the same is not true for
indeterminate structures. Indeterminate structures are not considered rigid;
therefore, the influence lines drawn for them will not be straight lines but
rather curves. The methods above can still be used to determine the influence
lines for the structure, but the work becomes much more complex as the
properties of the beam itself must be taken into consideration.
***** See also[edit] *****
    * Beam
    * Shear_and_Moment_Diagram
    * Dead_and_Live_Loads
    * MÃ¼ller-Breslau's_principle
***** References[edit] *****
   1. ^ a b c Kharagpur. "Structural_Analysis.pdf,_Version_2_CE_IIT" Archived
      2010-08-19 at the Wayback_Machine. 7 August 2008. Accessed on 26 November
      2010.
   2. ^ a b c d e f g h Dr. Fanous, Fouad. "Introductory_Problems_in_Structural
      Analysis:_Influence_Lines". 20 April 2000. Accessed on 26 November 2010.
   3. ^ a b "Influence_Line_Method_of_Analysis". The Constructor. 10 February
      2010. Accessed on 26 November 2010.
   4. ^ a b "Structural_Analysis:_Influence_Lines". The Foundation Coalition. 2
      December 2010. Accessed on 26 November 2010.
   5. ^ a b c d e f g h i j k l m n o Hibbeler, R.C. (2009). Structural
      Analysis (Seventh Edition). Pearson Prentice Hall, New Jersey.
   6. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   7. ISBN 0-13-602060-7.
   8. ^Zeinali, Yasha (December 2017). "Framework for Flexural Rigidity
      Estimation in Euler-Bernoulli Beams Using Deformation Influence Lines".
      Infrastructures. 2 (4): 23. doi:10.3390/infrastructures2040023.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Influence_line&oldid=908356974"
Categories:
    * Structural_analysis
    * Structural_engineering
Hidden categories:
    * Webarchive_template_wayback_links
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
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * Nederlands
Edit_links
    * This page was last edited on 29 July 2019, at 06:28 (UTC).
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
