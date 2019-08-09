The following text has been accessed from https://en.wikipedia.org/wiki/Pipe_network_analysis at Thu Aug 8 23:37:28 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Pipe network analysis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about hydraulic design. For the Australian internet peering and
fibre provider, see PIPE_Networks.
In fluid_dynamics, pipe network analysis is the analysis of the fluid_flow
through a hydraulics network, containing several or many interconnected
branches. The aim is to determine the flow_rates and pressure_drops in the
individual sections of the network. This is a common problem in hydraulic
design.
⁰
***** Contents *****
    * 1_Description
    * 2_Deterministic_network_analysis
    * 3_Probabilistic_network_analysis
    * 4_See_also
    * 5_References
    * 6_Notes
***** Description[edit] *****
To direct water to many users, municipal water supplies often route it through
a water_supply_network. A major part of this network will consist of
interconnected pipes. This network creates a special class of problems in
hydraulic design, with solution methods typically referred to as pipe network
analysis. Water utilities generally make use of specialized software to
automatically solve these problems. However, many such problems can also be
addressed with simpler methods, like a spreadsheet equipped with a solver, or a
modern graphing calculator.
***** Deterministic network analysis[edit] *****
Once the friction factors of the pipes are obtained (or calculated from pipe
friction laws such as the Darcy-Weisbach_equation), we can consider how to
calculate the flow rates and head losses on the network. Generally the head
losses (potential differences) at each node are neglected, and a solution is
sought for the steady-state flows on the network, taking into account the pipe
specifications (lengths and diameters), pipe friction properties and known flow
rates or head losses.
The steady-state flows on the network must satisfy two conditions:
   1. At any junction, the total flow into a junction equals the total flow out
      of that junction (law of conservation of mass, or continuity law, or
      Kirchhoff's_first_law)
   2. Between any two junctions, the head loss is independent of the path taken
      (law of conservation of energy, or Kirchhoff's second law). This is
      equivalent mathematically to the statement that on any closed loop in the
      network, the head loss around the loop must vanish.
[PipeNet.jpg]
If there are sufficient known flow rates, so that the system of equations given
by (1) and (2) above is closed (number of unknowns = number of equations), then
a deterministic solution can be obtained.
The classical approach for solving these networks is to use the Hardy_Cross
method. In this formulation, first you go through and create guess values for
the flows in the network. These initial guesses must satisfy the Kirchhoff laws
(1). That is, if Q7 enters a junction and Q6 and Q4 leave the same junction,
then the initial guess must satisfy Q7 = Q6 + Q4. After the initial guess is
made, then, a loop is considered so that we can evaluate our second condition.
Given a starting node, we work our way around the loop in a clockwise fashion,
as illustrated by Loop 1. We add up the head losses according to the
DarcyâWeisbach equation for each pipe if Q is in the same direction as our
loop like Q1, and subtract the head loss if the flow is in the reverse
direction, like Q4. In other words, we add the head losses around the loop in
the direction of the loop; depending on whether the flow is with or against the
loop, some pipes will have head losses and some will have head gains (negative
losses).
To satisfy the Kirchhoff's second laws (2), we should end up with 0 about each
loop at the steady-state solution. If the actual sum of our head loss is not
equal to 0, then we will adjust all the flows in the loop by an amount given by
the following formula, where a positive adjustment is in the clockwise
direction.
         &#x0394; Q = &#x2212;    &#x2211;     head loss   c     &#x2212;
      &#x2211;     head loss   c c       n &#x22C5; ( &#x2211;     head loss
      c    Q  c     + &#x2211;     head loss   c c    Q  c c     )    ,
      {\displaystyle \Delta Q=-{\frac {\sum {\scriptstyle {\text{head loss}}_
      {c}}-\sum {\scriptstyle {\text{head loss}}_{cc}}}{n\cdot (\sum {\frac {
      {\text{head loss}}_{c}}{Q_{c}}}+\sum {\frac {{\text{head loss}}_{cc}}{Q_
      {cc}}})}},}  [{\displaystyle \Delta Q=-{\frac {\sum {\scriptstyle {\text
      {head loss}}_{c}}-\sum {\scriptstyle {\text{head loss}}_{cc}}}{n\cdot
      (\sum {\frac {{\text{head loss}}_{c}}{Q_{c}}}+\sum {\frac {{\text{head
      loss}}_{cc}}{Q_{cc}}})}},}]
where
    * n is 1.85 for Hazen-Williams and
    * n is 2 for DarcyâWeisbach.
The clockwise specifier (c) means only the flows that are moving clockwise in
our loop, while the counter-clockwise specifier (cc) is only the flows that are
moving counter-clockwise.
This adjustment doesn't solve the problem, since most networks have several
loops. It is okay to use this adjustment, however, because the flow changes
won't alter condition 1, and therefore, the other loops still satisfy condition
1. However, we should use the results from the first loop before we progress to
other loops.
An adaptation of this method is needed to account for water reservoirs attached
to the network, which are joined in pairs by the use of 'pseudo-loops' in the
Hardy Cross scheme. This is discussed further on the Hardy_Cross_method site.
The modern method is simply to create a set of conditions from the above
Kirchhoff laws (junctions and head-loss criteria). Then, use a Root-finding
algorithm to find Q values that satisfy all the equations. The literal friction
loss equations use a term called Q2, but we want to preserve any changes in
direction. Create a separate equation for each loop where the head losses are
added up, but instead of squaring Q, use |Q|Â·Q instead (with |Q| the absolute
value of Q) for the formulation so that any sign changes reflect appropriately
in the resulting head-loss calculation.
***** Probabilistic network analysis[edit] *****
In many situations, especially for real water distribution networks in cities
(which can extend between thousands to millions of nodes), the number of known
variables (flow rates and/or head losses) required to obtain a deterministic
solution will be very large. Many of these variables will not be known, or will
involve considerable uncertainty in their specification. Furthermore, in many
pipe networks, there may be considerable variability in the flows, which can be
described by fluctuations about mean flow rates in each pipe. The above
deterministic methods are unable to account for these uncertainties, whether
due to lack of knowledge or flow variability.
For these reasons, a probabilistic method for pipe network analysis has
recently been developed,[1] based on the maximum_entropy_method of Jaynes.[2]
In this method, a continuous relative entropy function is defined over the
unknown parameters. This entropy is then maximized subject to the constraints
on the system, including Kirchhoff's laws, pipe friction properties and any
specified mean flow rates or head losses, to give a probabilistic statement
(probability_density_function) which describes the system. This can be used to
calculate mean values (expectations) of the flow rates, head losses or any
other variables of interest in the pipe network. This analysis has been
extended using a reduced-parameter entropic formulation, which ensures
consistency of the analysis regardless of the graphical representation of the
network.[3] A comparison of Bayesian and maximum entropy probabilistic
formulations for the analysis of pipe flow networks has also been presented,
showing that under certain assumptions (Gaussian priors), the two approaches
lead to equivalent predictions of mean flow rates.[4]
***** See also[edit] *****
    * Hardy_Cross_method
    * Gas_networks_simulation
***** References[edit] *****
    * N. Hwang, R. Houghtalen, "Fundamentals of Hydraulic Engineering Systems"
      Prentice Hall, Upper Saddle River, NJ. 1996.
    * L.F. Moody, "Friction factors for pipe flow," Trans. ASME, vol. 66, 1944.
    * C. F. Colebrook, "Turbulent flow in pipes, with particular reference to
      the transition region between smooth and rough pipe laws," Jour. Ist.
      Civil Engrs., London (Feb. 1939).
***** Notes[edit] *****
   1. ^ S.H. Waldrip, R.K. Niven, M. Abel, M. Schlegel (2016), Maximum entropy
      analysis of hydraulic pipe flow networks, J. Hydraulic Eng ASCE, 142(9):
      04016028, https://dx.doi.org/10.1061/(ASCE)HY.1943-
      7900.0001126#sthash.5ecR2Gts.dpuf
   2. ^Jaynes, E.T. (2003). Probability Theory: The Logic of Science. Cambridge
      University Press.
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
   4. ^ Waldrip, S.H., Niven, R.K., Abel, M., Schlegel, M. (2017), Reduced-
      parameter method for maximum entropy analysis of hydraulic pipe flow
      networks, J. Hydraulic Eng ASCE, in press
   5. ^ Waldrip, S.H., Niven, R.K. (2017), Comparison between Bayesian and
      maximum entropy analyses of flow networks, Entropy, 19(2): 58, https://
      dx.doi.org/10.3390/e19020058

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Pipe_network_analysis&oldid=841230458"
Categories:
    * Networks
    * Piping
    * Fluid_dynamics
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
    * Deutsch
    * íêµ­ì´
Edit_links
    * This page was last edited on 14 May 2018, at 18:00 (UTC).
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
