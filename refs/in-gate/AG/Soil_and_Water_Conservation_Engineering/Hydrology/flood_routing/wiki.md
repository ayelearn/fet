The following text has been accessed from https://en.wikipedia.org/wiki/Routing_(hydrology) at Fri Aug 9 00:52:14 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Routing (hydrology) ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Flood routing" redirects here. For the PCB routing algorithm, see Flood
router.
In hydrology, routing is a technique used to predict the changes in shape of a
hydrograph as water moves through a river_channel or a reservoir. In flood
forecasting, hydrologists may want to know how a short burst of intense rain in
an area upstream of a city will change as it reaches the city. Routing can be
used to determine whether the pulse of rain reaches the city as a deluge or a
trickle.
Routing also can be used to predict the hydrograph shape (and thus lowland
flooding potential) subsequent to multiple rainfall events in different sub-
catchments of the watershed. Timing and duration of the rainfall events, as
well as factors such as antecedent moisture conditions, overall watershed
shape, along with subcatchment-area shapes, land slopes (topography/
physiography), geology/hydrogeology (i.e. forests and aquifers can serve as
giant sponges that absorb rainfall and slowly release it over subsequent weeks
and months), and stream-reach lengths all play a role here. The result can be
an additive effect (i.e. a large flood if each subcatchment's respective
hydrograph peak arrives at the watershed mouth at the same point in time,
thereby effectively causing a "stacking" of the hydrograph peaks), or a more
distributed-in-time effect (i.e. a lengthy but relatively modest flood,
effectively attenuated in time, as the individual subcatchment peaks arrive at
the mouth of the main watershed channel in orderly succession).[1] [2] [3]
Other uses of routing include reservoir and channel design, floodplain studies
and watershed simulations.[4]
If the water flow at a particular point, A, in a stream is measured over time
with a flow gauge, this information can be used to create a hydrograph. A short
period of intense rain, normally called a flood_event, can cause a bulge in the
graph, as the increased water travels down the river, reaches the flow gauge at
A, and passes along it. If another flow gauge at B, downstream of A is set up,
one would expect the graph's bulge (or floodwave) to have the same shape.
However, the shape of the river and flow resistance within a river (from the
river_bed, for example) can affect the shape of the floodwave. Oftentimes, the
floodwave will be attenuated (have a reduced peak flow).
Routing techniques can be broadly classified as hydraulic (or distributed)
routing, hydrologic (or lumped) routing or semi-distributed routing. In
general, based on the available field data and goals of the project, one of
routing procedures is selected.
⁰
***** Contents *****
    * 1_Hydraulic_(or_distributed)_routing
    * 2_Hydrologic_(or_lumped)_routing
    * 3_Semi-distributed_routing
    * 4_Flood_routing
    * 5_Runoff_Routing
    * 6_See_also
    * 7_References
***** Hydraulic (or distributed) routing[edit] *****
Hydraulic routing is based on the solution of partial_differential_equations of
unsteady open-channel_flow. The equations used are the Saint-Venant_equations
or the associated dynamic wave equations.[5][6]
The hydraulic models (e.g. dynamic and diffusion wave models) require the
gathering of a lot of data related to river geometry and morphology and consume
a lot of computer resources in order to solve the equations numerically.[7][8]
[9]
***** Hydrologic (or lumped) routing[edit] *****
Hydrologic routing uses the continuity equation for hydrology. In its simplest
form, inflow to the river reach is equal to the outflow of the river reach plus
the change of storage:
         I = O +    &#x0394; S   &#x0394; t      {\displaystyle I=O+{\frac
      {\Delta S}{\Delta t}}}  [{\displaystyle I=O+{\frac {\Delta S}{\Delta
      t}}}], where
    * I is average inflow to the reach during     &#x0394; t   {\displaystyle
      \Delta t}  [\Delta t]
    * O is average outflow from the reach during     &#x0394; t
      {\displaystyle \Delta t}  [\Delta t]; and
    * S is the water currently in the reach (known as storage)
The hydrologic models (e.g. linear and nonlinear Muskingum models) need to
estimate hydrologic parameters using recorded data in both upstream and
downstream sections of rivers and/or by applying robust optimization techniques
to solve the one-dimensional conservation of mass and storage-continuity
equation.[10]
***** Semi-distributed routing[edit] *****
Semi-distributed models such as MuskingumâCunge family procedures are also
available. Simple physical concepts and common river characteristics such as
channel geometry, reach length, roughness coefficient, and slope are used to
estimate the model parameters without complex and expensive numerical
solutions.[11][12][13]
***** Flood routing[edit] *****
Flood routing is a procedure to determine the time and magnitude of flow (i.e.,
the flow hydrograph) at a point on a watercourse from known or assumed
hydrographs at one or more points upstream. The procedure is specifically known
as Flood routing, if the flow is a flood.[14][15] In order to determine the
change in shape of a hydrograph of a flood as it travels through a natural
river or artificial channel, different flood simulation techniques can be used.
Traditionally, the hydraulic (e.g. dynamic and diffusion wave models) and
hydrologic (e.g. linear and nonlinear Muskingum models) routing procedures that
are well known as distributed and lumped ways to hydraulic and hydrologic
practitioners, respectively, can be utilized. The hydrologic models need to
estimate hydrologic parameters using recorded data in both upstream and
downstream sections of rivers and/or by applying robust optimization techniques
to solve the one-dimensional conservation of mass and storage-continuity
equation.[16] On the other hand, hydraulic models require the gathering of a
lot of data related to river geometry and morphology and consume a lot of
computer resources in order to solve the equations numerically.[17][18][19]
However, semi-distributed models such as MuskingumâCunge family procedures
are also available. Simple physical concepts and common river characteristic
consisting of channel geometry, reach length, roughness coefficient, and slope
are used to estimate the model parameters without complex and expensive
numerical solutions.[20][21][22] In general, based on the available field data
and goals of a project, one of these approaches is utilized for the simulation
of flooding in rivers and channels.
***** Runoff Routing[edit] *****
Runoff routing is a procedure to calculate a surface runoff hydrograph from
rainfall. Losses are removed from rainfall to determine the rainfall excess
which is then converted to a hydrograph and routed through conceptual storages
that represent the storage discharge behaviour of overland and channel flow.
[23] [24]
***** See also[edit] *****
    * Hydrograph
    * One-dimensional_Saint-Venant_equations
***** References[edit] *****
   1. ^ Tague, CL and LE Band. Evaluating explicit and implicit routing for
      watershed hydro-ecological models of forest hydrology at the small
      catchment scale. Hydrological Processes 15, pages 1415â1439 (2001).
      Available online at http://andrewsforest.oregonstate.edu/pubs/pdf/
      pub3128.pdf
   2. ^ Example Watershed Configurations. Texas A&M University. Available
      online at http://swat.tamu.edu/media/69422/Appendix-B.pdf
   3. ^ Watershed Delineation, Lecture 3. Utah State University, United States
      Environmental Protection Agency, and AquaTerra Consultants. Available
      online at https://www.epa.gov/sites/production/files/2015-07/documents/
      lecture-3-watershed-delineation.pdf
   4. ^EM 1110-2-1417 (1994). "Chapter_9_-_Streamflow_and_Reservoir_Routing"
      (PDF). Flood Run-off Analysis. U.S. Army Corps of Engineers. p. 9-1.
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
   6. [permanent_dead_link]
   7. ^ Chow V. T, Maidment D. R, Mays L.W (1988). Applied Hydrology.
      McGraw1Hill International Editions: Singapore.
   8. ^ Akan A. O (2006). Open Channel Hydraulics. Elsevier, New York, NY, USA.
   9. ^ Chaudhry MH (1993) Open-Channel Flow. Prentice Hall, Englewood Cliffs,
      NJ, USA.
  10. ^ Samani H. M. V, Shamsipour G. A (2004). Hydrologic flood routing in
      branched river systems via nonlinear optimization. Journal of Hydraulic
      Research, 42(1): 55-59.
  11. ^ Akbari G. H, Barati R (2012). Comprehensive analysis of flooding in
      unmanaged catchments. Proceedings of the Institution of Civil Engineers-
      Water Management, 165(4): 229-238.
  12. ^ Barati R (2011). Parameter estimation of nonlinear Muskingum models
      using Nelder-Mead Simplex algorithm. Journal of Hydrologic Engineering,
      16(11): 946-954.
  13. ^ Cunge J. A (1969). On the subject of a flood propagation computational
      method (Muskingum method). Journal of Hydraulic Research, 7(2): 2051230.
  14. ^ Perumal M (1994). Hydrodynamic derivation of a variable parameter
      Muskingum method: 1. Theory and solution procedure. Hydrological sciences
      journal, 39(5): 431â442.
  15. ^ Barati R, Akbari GH and Rahimi S (2013) Flood routing of an unmanaged
      river basin using MuskingumâCunge model; field application and
      numerical experiments. Caspian Journal of Applied Sciences Research, 2
      (6):08-20.
  16. ^ Chow V. T, Maidment D. R, Mays L.W (1988). Applied Hydrology.
      McGraw1Hill International Editions: Singapore.
  17. ^ Akan A. O (2006). Open Channel Hydraulics. Elsevier, New York, NY, USA.
  18. ^ Barati R (2011). Parameter estimation of nonlinear Muskingum models
      using Nelder-Mead Simplex algorithm. Journal of Hydrologic Engineering,
      16(11): 946-954.
  19. ^ Chaudhry MH (1993) Open-Channel Flow. Prentice Hall, Englewood Cliffs,
      NJ, USA.
  20. ^ Samani H. M. V, Shamsipour G. A (2004). Hydrologic flood routing in
      branched river systems via nonlinear optimization. Journal of Hydraulic
      Research, 42(1): 55-59.
  21. ^ Akbari G. H, Barati R (2012). Comprehensive analysis of flooding in
      unmanaged catchments. Proceedings of the Institution of Civil Engineers-
      Water Management, 165(4): 229-238.
  22. ^ Cunge J. A (1969). On the subject of a flood propagation computational
      method (Muskingum method). Journal of Hydraulic Research, 7(2): 2051230.
  23. ^ Perumal M (1994). Hydrodynamic derivation of a variable parameter
      Muskingum method: 1. Theory and solution procedure. Hydrological sciences
      journal, 39(5): 431â442.
  24. ^ Barati R, Akbari GH and Rahimi S (2013) Flood routing of an unmanaged
      river basin using MuskingumâCunge model; field application and
      numerical experiments. Caspian Journal of Applied Sciences Research.
  25. ^ Laurenson, E. M. (1964). A catchment storage model for runoff routing.
      Journal of Hydrology, 2(2): 141-163.
  26. ^  Mein, R. G., E. M. Laurenson and T. A. McMahon (1974). Simple
      nonlinear model for flood estimation. Journal of the Hydraulics Division,
      American Society of Civil Engineers 100(HY11): 1507-1518.

Retrieved from "https://en.wikipedia.org/w/index.php?title=Routing_
(hydrology)&oldid=865196085"
Categories:
    * Hydrology
    * Soil_mechanics
    * Soil_physics
    * Water
Hidden categories:
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_April_2018
    * Articles_with_permanently_dead_external_links
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
Edit_links
    * This page was last edited on 22 October 2018, at 11:35 (UTC).
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
