The following text has been accessed from https://en.wikipedia.org/wiki/Photogrammetry at Fri Aug 9 02:27:45 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Photogrammetry ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article has an unclear citation style. The references used may be made
 clearer with a different or consistent style of citation and footnoting. (June
 2019)(Learn_how_and_when_to_remove_this_template_message)
The science of making measurements using photography
Low altitude aerial photograph for use in photogrammetry. Location: Three Arch
Bay, Laguna Beach, CA.
Photogrammetry falls under the broader category of Geomatics, and, according to
the American Society for Photogrammetry and Remote Sensing, is defined as, "the
art, science and technology of obtaining reliable information about physical
objects and the environment through the process of recording, measuring and
interpreting photographic images and patterns of electromagnetic radiant
imagery and other phenomena".[1] A simplified definition could be the
extraction of three-dimensional measurements from two-dimensional data (i.e.
images). Close-range photogrammetry refers to the collection of photography
from a lesser distance than traditional aerial (or orbital) photogrammetry.
'Digital' is also an important piece of the name, as this implies the modern
digital techniques discussed in this guide. Photogrammetry is as old as modern
photography, dating to the mid-19th century and in the simplest example, the
distance between two points that lie on a plane parallel to the photographic
image_plane,it can be determined by measuring their distance on the image, if
the scale (s) of the image is known.
Photogrammetric analysis may be applied to one photograph, or may use high-
speed_photography and remote_sensing to detect, measure and record complex 2D
and 3D motion_fields by feeding measurements and imagery_analysis into
computational_models in an attempt to successively estimate, with increasing
accuracy, the actual, 3D relative motions.
From its beginning with the stereoplotters used to plot contour_lines on
topographic_maps, it now has a very wide range of uses such as sonar, radar,
and lidar.
⁰
***** Contents *****
    * 1_Methods
          o 1.1_Stereophotogrammetry
    * 2_Integration
    * 3_Applications
          o 3.1_Mapping
          o 3.2_Archaeology
          o 3.3_3D_modeling
    * 4_Software
    * 5_See_also
    * 6_References
    * 7_External_links
***** Methods[edit] *****
A data model of photogrammetry[2]
Photogrammetry has been defined by the American_Society_for_Photogrammetry_and
Remote_Sensing (ASPRS) as the art, science, and technology of obtaining
reliable information about physical objects and the environment through
processes of recording, measuring and interpreting photographic images and
patterns of recorded radiant electromagnetic energy and other phenomena.[3]
Photogrammetry uses methods from many disciplines, including optics and
projective_geometry. Digital image capturing and photogrammetric processing
includes several well defined stages, which allow the generation of 2D or 3D
digital models of the object as an end product.[4] The data model on the right
shows what type of information can go into and come out of photogrammetric
methods.
The 3D co-ordinates define the locations of object points in the 3D_space. The
image co-ordinates define the locations of the object points' images on the
film or an electronic imaging device. The exterior_orientation[5] of a camera
defines its location in space and its view direction. The inner_orientation
defines the geometric parameters of the imaging process. This is primarily the
focal length of the lens, but can also include the description of lens
distortions. Further additional observations play an important role: With scale
bars, basically a known distance of two points in space, or known fix points,
the connection to the basic measuring units is created.
Each of the four main variables can be an input or an output of a
photogrammetric method.
Algorithms for photogrammetry typically attempt to minimize the sum of the
squares_of_errors over the coordinates and relative displacements of the
reference points. This minimization is known as bundle_adjustment and is often
performed using the LevenbergâMarquardt_algorithm.
**** Stereophotogrammetry[edit] ****
"Stereophotogrammetry" redirects here. It is not to be confused with Roentgen
stereophotogrammetry.
Main article: 3D_reconstruction_from_multiple_images
Main category: Stereophotogrammetry
See also: Computer_stereo_vision
A special case, called stereophotogrammetry, involves estimating the three-
dimensional coordinates of points on an object employing measurements made in
two or more photographic images taken from different positions (see
stereoscopy). Common points are identified on each image. A line of sight (or
ray) can be constructed from the camera location to the point on the object. It
is the intersection of these rays (triangulation) that determines the three-
dimensional location of the point. More sophisticated algorithms can exploit
other information about the scene that is known a_priori, for example
symmetries, in some cases allowing reconstructions of 3D coordinates from only
one camera position. Stereophotogrammetry is emerging as a robust non-
contacting measurement technique to determine dynamic characteristics and mode
shapes of non-rotating[6][7] and rotating structures.[8][9]
***** Integration[edit] *****
Photogrammetric data with a dense range data in which scanners complement each
other. Photogrammetry is more accurate in the x and y direction while range
data are generally more accurate in the z direction[citation_needed]. This
range data can be supplied by techniques like LiDAR, laser scanners (using time
of flight, triangulation or interferometry), white-light digitizers and any
other technique that scans an area and returns x, y, z coordinates for multiple
discrete points (commonly called "point_clouds"). Photos can clearly define the
edges of buildings when the point cloud footprint can not. It is beneficial to
incorporate the advantages of both systems and integrate them to create a
better product.
A 3D visualization can be created by georeferencing the aerial photos[10][11]
and LiDAR data in the same reference frame, orthorectifying the aerial photos,
and then draping the orthorectified images on top of the LiDAR grid. It is also
possible to create digital terrain models and thus 3D visualisations using
pairs (or multiples) of aerial photographs or satellite (e.g. SPOT_satellite
imagery). Techniques such as adaptive least squares stereo matching are then
used to produce a dense array of correspondences which are transformed through
a camera model to produce a dense array of x, y, z data which can be used to
produce digital_terrain_model and orthoimage products. Systems which use these
techniques, e.g. the ITG system, were developed in the 1980s and 1990s but have
since been supplanted by LiDAR and radar-based approaches, although these
techniques may still be useful in deriving elevation models from old aerial
photographs or satellite images.
***** Applications[edit] *****
[File:Video of a 3d model of Horatio Nelson bust in Monmouth Museum, Wales,
produced using photogrammetry.ogv]Play_media
Video of a 3D model of Horatio_Nelson bust in Monmouth_Museum, produced using
photogrammetry
[File:Gibraltar 1 3d model, created using photogrammetry.ogv]Play_media
Gibraltar_1 Neanderthal skull 3D wireframe model, created with 123d Catch
Photogrammetry is used in fields such as topographic_mapping, architecture,
engineering, manufacturing, quality_control, police investigation, cultural
heritage, and geology. Archaeologists use it to quickly produce plans of large
or complex sites, and meteorologists use it to determine the wind speed of
tornados when objective weather data cannot be obtained.
Photograph of person using controller to explore a 3D Photogrammetry
experience, Future Cities by DERIVE, recreating Tokyo.
It is also used to combine live_action with computer-generated_imagery in
movies post-production; The_Matrix is a good example of the use of
photogrammetry in film (details are given in the DVD extras). Photogrammetry
was used extensively to create photorealistic environmental assets for video
games including The_Vanishing_of_Ethan_Carter as well as EA_DICE's Star_Wars
Battlefront.[12] The main character of the game Hellblade:_Senua's_Sacrifice
was derived from photogrammetric motion-capture models taken of actress Melina
Juergens.[13]
Photogrammetry is also commonly employed in collision engineering, especially
with automobiles. When litigation for accidents occurs and engineers need to
determine the exact deformation present in the vehicle, it is common for
several years to have passed and the only evidence that remains is accident
scene photographs taken by the police. Photogrammetry is used to determine how
much the car in question was deformed, which relates to the amount of energy
required to produce that deformation. The energy can then be used to determine
important information about the crash (such as the velocity at time of impact).
**** Mapping[edit] ****
 This section contains too_many_quotations for an encyclopedic entry. Please
 help_improve_the_article by presenting facts as a neutrally-worded summary
 with appropriate_citations. Consider transferring direct quotations to
 Wikiquote. (June 2019)
Photomapping is the process of making a map with "cartographic enhancements"
[14] that have been drawn from a photomosaic[15] that is "a composite
photographic image of the ground" or more precisely as a controlled photomosaic
where "individual photographs are rectified for tilt and brought to a common
scale (at least at certain control points)."
Rectification of imagery is generally achieved by "fitting the projected images
of each photograph to a set of four control points whose positions have been
derived from an existing map or from ground measurements. When these rectified,
scaled photographs are positioned on a grid of control points, a good
correspondence can be achieved between them through skillful trimming and
fitting and the use of the areas around the principal point where the relief
displacements (which cannot be removed) are at a minimum."[14]
"It is quite reasonable to conclude that some form of photomap will become the
standard general map of the future."[16] go on to suggest[who?] that,
"photomapping would appear to be the only way to take reasonable advantage" of
future data sources like high altitude aircraft and satellite imagery. The
highest resolution aerial photomaps on GoogleEarth are approximately 2.5 cm
(0.98 in) spatial resolution images. The highest resolution photomap of ortho
images was made in Hungary in 2012 with a 0.5 cm (0.20 in) spatial resolution.
**** Archaeology[edit] ****
Using a pentop computer to photomap an archaeological excavation in the field
Demonstrating the link between orthophotomapping and archaeology,[17] historic
airphotos photos were used to aid in developing a reconstruction of the Ventura
mission that guided excavations of the structure's walls.
Pteryx_UAV, a civilian UAV for aerial photography and photomapping with roll-
stabilised camera head
Overhead photography has been widely applied for mapping surface remains and
excavation exposures at archaeological sites. Suggested platforms for capturing
these photographs has included: War Balloons from World War I;[18] rubber
meteorological balloons;[19] kites;[19][20] wooden platforms, metal frameworks,
constructed over an excavation exposure;[19] ladders both alone and held
together with poles or planks; three legged ladders; single and multi-section
poles;[21][22] bipods;[23][24][25][26] tripods;[27] tetrapods[28][29] aerial
bucket trucks ("cherry pickers"),[30] and light weight individuals dangling
from the limb of a nearby tree.
Hand held near nadir over head digital photographs have been used with
geographic information systems (GIS) to record excavation exposures.[31][32]
[33][34][35]
Photogrammetry is increasingly being used in maritime_archaeology because of
the relative ease of mapping sites compared to traditional methods, allowing
the creation of 3D maps which can be rendered in virtual reality.[36]
**** 3D modeling[edit] ****
A somewhat similar application is the scanning of objects to automatically make
3D models of them. The produced model often still contains gaps, so additional
cleanup with software like MeshLab, netfabb or MeshMixer is often still
necessary.[37]
***** Software[edit] *****
There exist many software_packages for photogrammetry; see comparison_of
photogrammetry_software.
***** See also[edit] *****
Main category: Photogrammetry
    * 3D_data_acquisition_and_object_reconstruction
    * 3D_reconstruction_from_multiple_images
    * Aerial_survey
    * Computer_vision
    * Digital_image_correlation_and_tracking
    * Edouard_Deville
    * Epipolar_geometry
    * Geoinformatics
    * Geomatics_engineering
    * Geographic_information_system
    * International_Society_for_Photogrammetry_and_Remote_Sensing
    * Mobile_Mapping
    * Periscope
    * Photomapping
    * Rangefinder
    * Solid_image
    * Stereoplotter
    * Simultaneous_localization_and_mapping
    * Structure_from_motion
    * Surveying
    * Videogrammetry
***** References[edit] *****
   1. ^Jones, Alan D. (1982-09-01). "Manual_of_Photogrammetry,_eds_C.C._Slama,
      C._Theurer_and_S.W._Hendrikson,_American_Society_of_Photogrammetry,_Falls
      Church,_Va.,_1980,_Fourth_Edition,_180_Ã_260mm,_xvi_and_1056_pages_(with
      index),_72_tables,_866_figures._ISBN_0_937294_01_2". Cartography. 12 (4):
      258â258. doi:10.1080/00690805.1982.10438226. ISSN 0069-0805.
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
   3. ^Wiora, Georg (2001). Optische_3D-Messtechnik :_PrÃ¤zise
      Gestaltvermessung_mit_einem_erweiterten_Streifenprojektionsverfahren
      (Doctoral dissertation). (Optical 3D-Metrology : Precise Shape
      Measurement with an extended Fringe Projection Method) (in German).
      Heidelberg: Ruprechts-Karls-UniversitÃ¤t. p. 36. Retrieved 20 October
      2017.
   4. ^ ASPRS_online Archived May 20, 2015, at the Wayback_Machine
   5. ^SuÅ¾iedelytÄ-VisockienÄ J, BagdÅ¾iÅ«naitÄ R, Malys N, Maliene V
      (2015). "Close-range_photogrammetry_enables_documentation_of_environment-
      induced_deformation_of_architectural_heritage". Environmental Engineering
      and Management Journal. 14 (6): 1371â1381.
   6. ^"Ina_Jarve,_Natalja_Liba._The_Effect_of_Various_Principles_of_External
      Orientation_on_the_Overall_Triangulation_Accuracy._TECHNOLOGIJOS_MOKSLAI.
      Estonia._#86,_2010,_pp._59-64" (PDF).
   7. ^SuÅ¾iedelytÄ-VisockienÄ, JÅ«ratÄ (1 March 2013). "Accuracy analysis
      of measuring close-range image points using manual and stereo modes".
      Geodesy and Cartography. 39 (1): 18â22. doi:10.3846/
      20296991.2013.786881.
   8. ^Baqersad, Javad; Carr, Jennifer; et al. (April 26, 2012). Dynamic
      characteristics_of_a_wind_turbine_blade_using_3D_digital_image
      correlation. Proceedings_of_SPIE. 8348.
   9. ^Lundstrom, Troy; Baqersad, Javad; Niezrecki, Christopher; Avitabile,
      Peter (1 January 2012). "Using High-Speed Stereophotogrammetry Techniques
      to Extract Shape Information from Wind Turbine/Rotor Operating Data".
      Topics in Modal Analysis II, Volume 6. Conference Proceedings of the
      Society for Experimental Mechanics Series. Springer, New York, NY.
      pp. 269â275. doi:10.1007/978-1-4614-2419-2_26. ISBN 978-1-4614-2418-5.
  10. ^Lundstrom, Troy; Baqersad, Javad; Niezrecki, Christopher (1 January
      2013). "Using High-Speed Stereophotogrammetry to Collect Operating Data
      on a Robinson R44 Helicopter". Special Topics in Structural Dynamics,
      Volume 6. Conference Proceedings of the Society for Experimental
      Mechanics Series. Springer, New York, NY. pp. 401â410. doi:10.1007/978-
      1-4614-6546-1_44. ISBN 978-1-4614-6545-4.
  11. ^ A._Sechin._Digital_Photogrammetric_Systems:_Trends_and_Developments.
      GeoInformatics._#4,_2014,_pp._32-34.
  12. ^Ahmadi, FF; Ebadi, H (2009). "An_integrated_photogrammetric_and_spatial
      database_management_system_for_producing_fully_structured_data_using
      aerial_and_remote_sensing_images". Sensors (Basel). 9 (4): 2320â33.
      doi:10.3390/s90402320. PMC 3348797. PMID 22574014.
  13. ^"How_we_used_Photogrammetry_to_Capture_Every_Last_Detail_for_Star
      Warsâ¢_Battlefrontâ¢". 19 May 2015.
  14. ^"The_real-time_motion_capture_behind_'Hellblade'". engadget.com.
  15. ^ a b Petrie (1977: 50)
  16. ^ Petrie (1977: 49)
  17. ^ Robinson et al. (1977:10)
  18. ^ Estes et al. (1977)
  19. ^ Capper (1907)
  20. ^ a b c Guy (1932)
  21. ^ Bascom (1941)
  22. ^ Schwartz (1964)
  23. ^ Wiltshire (1967)
  24. ^ Kriegler (1928)
  25. ^ Hampl (1957)
  26. ^ Whittlesey (1966)
  27. ^ Fant and Loy (1972)
  28. ^ Straffin (1971)
  29. ^ Simpson and Cooke (1967)
  30. ^ Hume (1969)
  31. ^ Sterud and Pratt (1975)
  32. ^ Craig (2000)
  33. ^ Craig (2002)
  34. ^ Craig and Aldenderfer (2003)
  35. ^ Craig (2005)
  36. ^ Craig et al. (2006)
  37. ^"Photogrammetry_|_Maritime_Archaeology". web.archive.org. 2019-01-19.
      Retrieved 2019-01-19.
  38. ^ MAKE:3D printing by Anna Kaziunas France
    * "Archaeological Photography", Antiquity, 10, pp. 486â490, 1936
Bascom, W. R. (1941), "Possible Applications of Kite Photography to Archaeology
and Ethnology", Illinois State Academy of Science, Transactions, 34,
pp. 62â63
Capper, J. E. (1907), "Photographs of Stonehenge as Seen from a War Balloon",
Archaeologia, 60, pp. 571â572, doi:10.1017/s0261340900005208
Craig, Nathan (2005), The_Formation_of_Early_Settled_Villages_and_the_Emergence
of_Leadership:_A_Test_of_Three_Theoretical_Models_in_the_Rio_Ilave,_Lake
Titicaca_Basin,_Southern_Peru (PDF), Ph.D. Dissertation, University of
California Santa Barbara, archived from the_original (PDF) on 23 July 2011,
retrieved 9 February 2007
Craig, Nathan (2002), "Recording_Large-Scale_Archaeological_Excavations_with
GIS:_Jiskairumoko--Near_Peru's_Lake_Titicaca", ESRI ArcNews, Spring, retrieved
9 February 2007
Craig, Nathan (2000), "Real_Time_GIS_Construction_and_Digital_Data_Recording_of
the_Jiskairumoko,_Excavation_PerÃº", Society for American Archaeology Buletin,
18 (1), archived from the_original on 19 February 2007, retrieved 9 February
2007
Craig, Nathan; Adenderfer, Mark (2003), "Preliminary_Stages_in_the_Development
of_a_Real-Time_Digital_Data_Recording_System_for_Archaeological_Excavation
Using_ArcView_GIS_3.1" (PDF), Journal of GIS in Archaeology, 1, pp. 1â22,
retrieved 9 February 2007
Craig, N., Aldenderfer, M. & Moyes, H. (2006), "Multivariate_Visualization_and
Analysis_of_Photomapped_Artifact_Scatters" (PDF), Journal of Archaeological
Science, 33, pp. 1617â1627, doi:10.1016/j.jas.2006.02.018, archived from the
original (PDF) on 4 October 2007CS1 maint: Multiple names: authors list (link)
Estes, J. E., Jensen, J. R. & Tinney, L. R. (1977), "The Use of Historical
Photography for Mapping Archaeological Sites", Journal of Field Archaeology, 4,
pp. 441â447, doi:10.1179/009346977791490104CS1 maint: Multiple names: authors
list (link)
Fant, J. E. & Loy, W. G. (1972), "Surveying and Mapping", The Minnesota
Messenia Expedition
Guy,_P._L._O. (1932), "Balloon Photography and Archaeological Excavation",
Antiquity, 6, pp. 148â155
Hampl, F. (1957), "ArchÃ¤ologische Feldphotographie", Archaeologia Austriaca,
22, pp. 54â64
Hume, I. N. (1969), Historical Archaeology, New York
Kriegler, K. (1929), "Ãber Photographische Aufnahmen PrÃ¤historischer
GrÃ¤ber", Mittheliungen der Anthropologischen Gesellschaft in Wien, 58,
pp. 113â116
Petrie, G. (1977), "Orthophotomaps", Transactions of the Institute of British
Geographers, 2, pp. 49â70, doi:10.2307/622193
Robinson, A. H., Morrison, J. L. & Meuehrcke, P. C. (1977), "Cartography 1950-
2000", Transactions of the Institute of British Geographers, 2, pp. 3â18,
doi:10.2307/622190CS1 maint: Multiple names: authors list (link)
Schwartz, G. T. (1964), "Stereoscopic Views Taken with an Ordinary Single
Camera--A New Technique for Archaeologists", Archaeometry, pp. 36â42, doi:
10.1111/j.1475-4754.1964.tb00592.x
Simpson, D. D. A. & Booke, F. M. B. (1967), "Photogrammetric Planning at
Grantully Perthshire", Antiquity, 41, pp. 220â221
Straffin, D. (1971), "A Device for Vertical Archaeological Photography", Plains
Anthropologist, 16, pp. 232â234
Wiltshire, J. R. (1967), "A Pole for High Viewpoint Photography", Industrial
Commercial Photography, pp. 53â56
***** External links[edit] *****
 Look up photogrammetry in Wiktionary, the free dictionary.
 Wikimedia Commons has media related to Photogrammetry.
    * RSPSoc_-_Remote_Sensing_and_Photogrammetry_Society_of_UK
    * History_of_Photogrammetry
    * Photogrammetry_overview_on_the_Cultural_Heritage_Imaging_web_site
    * World_Photogrammetry,_the_spanish_website_of_photogrammetry_for_everyone
    * Visual_Revolution_of_the_Vanishing_of_Ethan_Carter
    * Examples_of_photogrammetry
Authority_control [Edit_this_at_Wikidata]     * GND: 4045892-1

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Photogrammetry&oldid=909154541"
Categories:
    * Photogrammetry
Hidden categories:
    * CS1_German-language_sources_(de)
    * Webarchive_template_wayback_links
    * Wikipedia_references_cleanup_from_June_2019
    * All_articles_needing_references_cleanup
    * Articles_covered_by_WikiProject_Wikify_from_June_2019
    * All_articles_covered_by_WikiProject_Wikify
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_January_2019
    * Wikipedia_articles_with_style_issues_from_June_2019
    * All_articles_with_style_issues
    * All_articles_with_specifically_marked_weasel-worded_phrases
    * Articles_with_specifically_marked_weasel-worded_phrases_from_June_2019
    * CS1:_long_volume_value
    * CS1_maint:_Multiple_names:_authors_list
    * Commons_category_link_from_Wikidata
    * Wikipedia_articles_with_GND_identifiers
    * Articles_containing_video_clips
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 3 August 2019, at 13:56 (UTC).
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
