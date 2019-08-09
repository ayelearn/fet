The following text has been accessed from https://en.wikipedia.org/wiki/Solid_mechanics at Thu Aug 8 23:49:47 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Solid mechanics ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article has multiple issues. Please help improve_it or discuss these
 issues on the talk_page. (Learn_how_and_when_to_remove_these_template
 messages)
  This article includes a list_of_references, but its sources remain unclear
  because it has insufficient inline_citations. Please help to improve this
  article by introducing more precise citations. (December 2014)(Learn_how_and
  when_to_remove_this_template_message)
  This article has an unclear citation style. The references used may be made
  clearer with a different or consistent style of citation and footnoting.
  (June 2014)(Learn_how_and_when_to_remove_this_template_message)
 (Learn_how_and_when_to_remove_this_template_message)
Continuum_mechanics
Laws
Conservations
    * Mass
    * Momentum
    * Energy
Inequalities
    * ClausiusâDuhem_(entropy)
Solid mechanics
    * Deformation
    * Elasticity
          o linear
    * Plasticity
    * Hooke's_law
    * Stress
    * Finite_strain
    * Infinitesimal_strain
    * Compatibility
    * Bending
    * Contact_mechanics
          o frictional
    * Material_failure_theory
    * Fracture_mechanics
Fluid_mechanics
Fluids
    * Statics Â· Dynamics
    * Archimedes'_principle Â· Bernoulli's_principle
    * NavierâStokes_equations
    * Poiseuille_equation Â· Pascal's_law
    * Viscosity
          o (Newtonian Â· non-Newtonian)
    * Buoyancy Â· Mixing Â· Pressure
Liquids
    * Surface_tension
    * Capillary_action
Gases
    * Atmosphere
    * Boyle's_law
    * Charles's_law
    * Gay-Lussac's_law
    * Combined_gas_law
Plasma
Rheology
    * Viscoelasticity
    * Rheometry
    * Rheometer
Smart_fluids
    * Electrorheological
    * Magnetorheological
    * Ferrofluids
Scientists
    * Bernoulli
    * Boyle
    * Cauchy
    * Charles
    * Euler
    * Gay-Lussac
    * Hooke
    * Pascal
    * Newton
    * Navier
    * Stokes
    * v
    * t
    * e
Solid mechanics, also known as mechanics of solids, is the branch of continuum
mechanics that studies the behavior of solid materials, especially their motion
and deformation under the action of forces, temperature changes, phase changes,
and other external or internal agents.
Solid mechanics is fundamental for civil, aerospace, nuclear, biomedical and
mechanical_engineering, for geology, and for many branches of physics such as
materials_science.[1] It has specific applications in many other areas, such as
understanding the anatomy of living beings, and the design of dental_prostheses
and surgical_implants. One of the most common practical applications of solid
mechanics is the Euler-Bernoulli_beam_equation. Solid mechanics extensively
uses tensors to describe stresses, strains, and the relationship between them.
Solid mechanics is a vast subject because of the wide range of solid materials
available, such as steel, wood, concrete, biological materials, textiles,
geological materials, and plastics.
⁰
***** Contents *****
    * 1_Fundamental_aspects
    * 2_Relationship_to_continuum_mechanics
    * 3_Response_models
    * 4_Timeline
    * 5_See_also
    * 6_References
          o 6.1_Notes
          o 6.2_Bibliography
***** Fundamental aspects[edit] *****
A solid is a material that can support a substantial amount of shearing_force
over a given time scale during a natural or industrial process or action. This
is what distinctly distinguishes solids from fluids, because fluids also
support normal forces which are those forces that are directed perpendicular to
the material plane across from which they act and normal stress is the normal
force per unit area of that material plane. Shearing forces in contrast with
normal forces, act parallel rather than perpendicular to the material plane and
the shearing force per unit area is called shear stress.
Therefore, solid mechanics examines the shear stress, deformation and the
failure of solid materials and structures.
The most common topics covered in solid mechanics include:
   1. stability of structures - examining whether structures can return to a
      given equilibrium after disturbance or partial/complete failure
   2. dynamical systems and chaos - dealing with mechanical systems highly
      sensitive to their given initial position
   3. thermomechanics - analyzing materials with models derived from principles
      of thermodynamics
   4. biomechanics - solid mechanics applied to biological materials e.g.
      bones, heart tissue
   5. geomechanics - solid mechanics applied to geological materials e.g. ice,
      soil, rock
   6. vibrations of solids and structures - examining vibration and wave
      propagation from vibrating particles and structures i.e. vital in
      mechanical, civil, mining, aeronautical, maritime/marine, aerospace
      engineering
   7. fracture and damage mechanics - dealing with crack-growth mechanics in
      solid materials
   8. composite materials - solid mechanics applied to materials made up of
      more than one compound e.g. reinforced_plastics, reinforced_concrete,
      fiber_glass
   9. variational formulations and computational mechanics - numerical
      solutions to mathematical equations arising from various branches of
      solid mechanics e.g. finite_element_method_(FEM)
  10. experimental mechanics - design and analysis of experimental methods to
      examine the behavior of solid materials and structures
***** Relationship to continuum mechanics[edit] *****
As shown in the following table, solid mechanics inhabits a central place
within continuum mechanics. The field of rheology presents an overlap between
solid and fluid mechanics.
 ____________________________________________________________________________
|                |                   |Elasticity                             |
|                |                   |Describes materials that return to     |
|                |Solid mechanics    |their rest shape after applied stresses|
|                |The study of the   |are_removed.___________________________|
|                |physics of         |Plasticity         |                   |
|                |continuous         |Describes materials|                   |
|Continuum       |materials with a   |that permanently   |                   |
|mechanics       |defined rest shape.|deform after a     |Rheology           |
|The study of the|                   |sufficient applied |The study of       |
|physics of      |___________________|stress.____________|materials with both|
|continuous      |Fluid_mechanics    |Non-Newtonian      |solid and fluid    |
|materials       |The study of the   |fluids do not      |characteristics.   |
|                |physics of         |undergo strain     |                   |
|                |continuous         |rates proportional |                   |
|                |materials which    |to the applied     |                   |
|                |deform when        |shear_stress.______|___________________|
|                |subjected to a     |Newtonian_fluids undergo strain rates  |
|                |force.             |proportional to the applied shear      |
|________________|___________________|stress.________________________________|
***** Response models[edit] *****
A material has a rest shape and its shape departs away from the rest shape due
to stress. The amount of departure from rest shape is called deformation, the
proportion of deformation to original size is called strain. If the applied
stress is sufficiently low (or the imposed strain is small enough), almost all
solid materials behave in such a way that the strain is directly proportional
to the stress; the coefficient of the proportion is called the modulus_of
elasticity. This region of deformation is known as the linearly elastic region.
It is most common for analysts in solid mechanics to use linear material
models, due to ease of computation. However, real materials often exhibit non-
linear behavior. As new materials are used and old ones are pushed to their
limits, non-linear material models are becoming more common.
These are basic models that describe how a solid responds to an applied stress:
   1. Elasticity â When an applied stress is removed, the material returns to
      its undeformed state. Linearly elastic materials, those that deform
      proportionally to the applied load, can be described by the linear
      elasticity equations such as Hooke's_law.
   2. Viscoelasticity â These are materials that behave elastically, but also
      have damping: when the stress is applied and removed, work has to be done
      against the damping effects and is converted in heat within the material
      resulting in a hysteresis_loop in the stressâstrain curve. This implies
      that the material response has time-dependence.
   3. Plasticity â Materials that behave elastically generally do so when the
      applied stress is less than a yield value. When the stress is greater
      than the yield stress, the material behaves plastically and does not
      return to its previous state. That is, deformation that occurs after
      yield is permanent.
   4. Viscoplasticity - Combines theories of viscoelasticity and plasticity and
      applies to materials like gels and mud.
   5. Thermoelasticity - There is coupling of mechanical with thermal
      responses. In general, thermoelasticity is concerned with elastic solids
      under conditions that are neither isothermal nor adiabatic. The simplest
      theory involves the Fourier's_law of heat conduction, as opposed to
      advanced theories with physically more realistic models.
***** Timeline[edit] *****
    * 1452â1519 Leonardo_da_Vinci made many contributions
    * 1638: Galileo_Galilei published the book "Two_New_Sciences" in which he
      examined the failure of simple structures
Galileo_Galilei published the book "Two_New_Sciences" in which he examined the
failure of simple structures
    * 1660: Hooke's_law by Robert_Hooke
    * 1687: Isaac_Newton published "Philosophiae_Naturalis_Principia
      Mathematica" which contains Newton's_laws_of_motion
Isaac_Newton published "Philosophiae_Naturalis_Principia_Mathematica" which
contains the Newton's_laws_of_motion
    * 1750: EulerâBernoulli_beam_equation
    * 1700â1782: Daniel_Bernoulli introduced the principle of virtual_work
    * 1707â1783: Leonhard_Euler developed the theory of buckling of columns
Leonhard_Euler developed the theory of buckling of columns
    * 1826: Claude-Louis_Navier published a treatise on the elastic behaviors
      of structures
    * 1873: Carlo_Alberto_Castigliano presented his dissertation "Intorno ai
      sistemi elastici", which contains his_theorem for computing displacement
      as partial derivative of the strain energy. This theorem includes the
      method of least work as a special case
    * 1874: Otto_Mohr formalized the idea of a statically indeterminate
      structure.
    * 1922: Timoshenko corrects the Euler-Bernoulli_beam_equation
    * 1936: Hardy_Cross' publication of the moment distribution method, an
      important innovation in the design of continuous frames.
    * 1941: Alexander_Hrennikoff solved the discretization of plane elasticity
      problems using a lattice framework
    * 1942: R._Courant divided a domain into finite subregions
    * 1956: J. Turner, R. W. Clough, H. C. Martin, and L. J. Topp's paper on
      the "Stiffness and Deflection of Complex Structures" introduces the name
      "finite-element method" and is widely recognized as the first
      comprehensive treatment of the method as it is known today
***** See also[edit] *****
 Wikiversity has learning resources about Solid_mechanics
 Wikibooks has a book on the topic of: Solid_mechanics
    * Strength_of_materials - Specific definitions and the relationships
      between stress and strain.
    * Applied_mechanics
    * Materials_science
    * Continuum_mechanics
    * Fracture_mechanics
    * Impact_(mechanics)
***** References[edit] *****
**** Notes[edit] ****
   1. ^Allan Bower (2009). Applied_mechanics_of_solids. CRC press. Retrieved
      March 5, 2017.
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
**** Bibliography[edit] ****
    * L.D._Landau, E.M._Lifshitz, Course_of_Theoretical_Physics: Theory of
      Elasticity Butterworth-Heinemann,
ISBN 0-7506-2633-X
J.E. Marsden, T.J. Hughes, Mathematical Foundations of Elasticity, Dover,
ISBN 0-486-67865-2
P.C. Chou, N. J. Pagano, Elasticity: Tensor, Dyadic, and Engineering
Approaches, Dover,
ISBN 0-486-66958-0
R.W. Ogden, "Non-linear Elastic Deformation", Dover,
ISBN 0-486-69648-0
S._Timoshenko and J.N. Goodier," Theory of elasticity", 3d ed., New York,
McGraw-Hill, 1970.
A.I. Lurie, "Theory of Elasticity", Springer, 1999.
L.B. Freund, "Dynamic Fracture Mechanics", Cambridge University Press, 1990.
R. Hill, "The Mathematical Theory of Plasticity", Oxford University, 1950.
J. Lubliner, "Plasticity Theory", Macmillan Publishing Company, 1990.
J. Ignaczak, M. Ostoja-Starzewski, "Thermoelasticity with Finite Wave Speeds,"
Oxford University Press, 2010.
D. Bigoni, "Nonlinear Solid Mechanics: Bifurcation Theory and Material
Instability," Cambridge University Press, 2012.
Y. C. Fung, Pin Tong and Xiaohong Chen, "Classical and Computational Solid
Mechanics", 2nd Edition, World Scientific Publishing, 2017,
ISBN 978-981-4713-64-1.
    * v
    * t
    * e
Branches_of_physics
                      * Theoretical
                            o Phenomenology
Divisions             * Computational
                      * Experimental
                      * Applied
                                            * Continuum
                  Classical_mechanics             o Solid
                                                  o Fluid
                                            * Acoustics
                                            * Electrostatics
                  Electrodynamics           * Magnetostatics
                                            * Plasma_physics
Classical                                   * Accelerator_physics
                                            * Thermodynamics
                                            * Condensed_matter
                                                  o Materials
                  Statistical_mechanics           o Mesoscopic
                                                  o Polymers
                                                  o Soft
                                                  o Solid-state
                                          * Quantum_electrodynamics
                  Quantum_mechanics       * Quantum_field_theory
                                          * Quantum_gravity
                                          * Quantum_information
                  Relativity              * General
                                          * Special
                                          * Astroparticle
                  Particle_physics        * Nuclear
                                          * Quantum_chromodynamics
Modern                                    * Atomic_physics
                  Atomic,_molecular       * Molecular_physics
                  and_optical_physics     * Optics
                                          * Photonics
                                          * Quantum_optics
                                          * Astrophysics
                                                o Nuclear
                  Cosmology               * Celestial_mechanics
                                          * Solar
                                                o Heliophysics
                                          * Space_physics
                      * Agrophysics
                      * Biophysics
                            o Medical
                            o Neurophysics
                      * Engineering
                      * Geophysics
Interdisciplinary           o Atmospheric
                            o Cloud
                      * Mathematical
                      * Physical_chemistry
                            o Chemical_physics
                      * Quantum_computing
                      * Social_physics
                            o Econophysics
                      * History_of_physics
See also              * Nobel_Prize_in_Physics
                      * Timeline_of_physics_discoveries
                      * Theory_of_everything

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Solid_mechanics&oldid=908154395"
Categories:
    * Solid_mechanics
    * Mechanics
    * Continuum_mechanics
    * Rigid_bodies_mechanics
Hidden categories:
    * Articles_lacking_in-text_citations_from_December_2014
    * All_articles_lacking_in-text_citations
    * Wikipedia_references_cleanup_from_June_2014
    * All_articles_needing_references_cleanup
    * Articles_covered_by_WikiProject_Wikify_from_June_2014
    * All_articles_covered_by_WikiProject_Wikify
    * Articles_with_multiple_maintenance_issues
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Ido
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à¤®à¤°à¤¾à¤ à¥
    * Bahasa_Melayu
    * áá¶áá¶ááááá
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à·à·à¶à·à¶½
    * Simple_English
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 27 July 2019, at 20:40 (UTC).
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
