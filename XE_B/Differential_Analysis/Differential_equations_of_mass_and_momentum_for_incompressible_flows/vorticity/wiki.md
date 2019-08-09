The following text has been accessed from https://en.wikipedia.org/wiki/Vorticity at Fri Aug 9 01:21:16 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Vorticity ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (May 2009)(Learn_how_and_when
 to_remove_this_template_message)
Continuum_mechanics
Laws
Conservations
    * Mass
    * Momentum
    * Energy
Inequalities
    * ClausiusâDuhem_(entropy)
Solid_mechanics
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
In continuum_mechanics, the vorticity is a pseudovector field that describes
the local spinning motion of a continuum near some point (the tendency of
something to rotate[1]), as would be seen by an observer located at that point
and traveling along with the flow.
Conceptually, vorticity could be determined by marking parts of a continuum in
a small neighborhood of the point in question, and watching their relative
displacements as they move along the flow. The vorticity vector would be twice
the mean angular_velocity vector of those particles relative to their center_of
mass, oriented according to the right-hand_rule. This quantity must not be
confused with the angular velocity of the particles relative to some other
point.
More precisely, the vorticity is a pseudovector field Ïâ, defined as the
curl (rotational) of the flow_velocity uâ vector. The definition can be
expressed by the vector_analysis formula:
            &#x03C9; &#x2192;    &#x2261; &#x2207; &#x00D7;    u &#x2192;     ,
      {\displaystyle {\vec {\omega }}\equiv \nabla \times {\vec {u}}\,,}  [
      {\displaystyle {\vec {\omega }}\equiv \nabla \times {\vec {u}}\,,}]
where â is the del_operator. The vorticity of a two-dimensional_flow is
always perpendicular to the plane of the flow, and therefore can be considered
a scalar_field.
The vorticity is related to the flow's circulation (line integral of the
velocity) along a closed path by the (classical) Stokes'_theorem.[2] Namely,
for any infinitesimal surface_element C with normal_direction nâ and area dA,
the circulation dÎ along the perimeter of C is the dot_product Ïâ â (dA
nâ) where Ïâ is the vorticity at the center of C.[2]
Many phenomena, such as the blowing out of a candle by a puff of air, are more
readily explained in terms of vorticity, rather than the basic concepts of
pressure and velocity. This applies, in particular, to the formation and motion
of vortex_rings.
The name vorticity was created by Horace_Lamb in 1916[3].
⁰
***** Contents *****
    * 1_Examples
    * 2_Mathematical_definition
    * 3_Vorticity_to_Velocity
    * 4_Evolution
    * 5_Vortex_lines_and_vortex_tubes
    * 6_Vorticity_meters
          o 6.1_Rotating-vane_vorticity_meter
          o 6.2_Non-rotating_vorticity_meters
    * 7_Specific_sciences
          o 7.1_Aeronautics
          o 7.2_Atmospheric_sciences
    * 8_See_also
          o 8.1_Fluid_dynamics
          o 8.2_Atmospheric_sciences
    * 9_References
    * 10_Bibliography
    * 11_Further_reading
    * 12_External_links
***** Examples[edit] *****
In a mass of continuum that is rotating like a rigid body, the vorticity is
twice the angular_velocity vector of that rotation. This is the case, for
example, in the central core of a Rankine_vortex.
The vorticity may be nonzero even when all particles are flowing along straight
and parallel pathlines, if there is shear (that is, if the flow speed varies
across streamlines). For example, in the laminar_flow within a pipe with
constant cross_section, all particles travel parallel to the axis of the pipe;
but faster near that axis, and practically stationary next to the walls. The
vorticity will be zero on the axis, and maximum near the walls, where the shear
is largest.
Conversely, a flow may have zero vorticity even though its particles travel
along curved trajectories. An example is the ideal irrotational_vortex, where
most particles rotate about some straight axis, with speed inversely
proportional to their distances to that axis. A small parcel of continuum that
does not straddle the axis will be rotated in one sense but sheared in the
opposite sense, in such a way that their mean angular velocity about their
center of mass is zero.
      Example flows:
      [Vorticity_Figure_01_a- [Vorticity_Figure_03_a-  [Vorticity_Figure_02_a-
      m.gif]                  m.gif]                   m.gif]
      Rigid-body-like vortex  Parallel flow with shear Irrotational vortex
      v â r                                       v â 1/r
      where v is the velocity of the flow, r is the distance to the center of
      the vortex and â indicates proportionality.
      Absolute velocities around the highlighted point:
      [Vorticity_Figure_01    [Vorticity_Figure_03     [Vorticity_Figure_02
      b.png]                  b.png]                   b.png]
      Relative velocities (magnified) around the highlighted point
      [Vorticity_Figure_01    [Vorticity_Figure_03     [Vorticity_Figure_02
      c.png]                  c.png]                   c.png]
      Vorticity â  0      Vorticity â  0       Vorticity = 0
Another way to visualize vorticity is to imagine that, instantaneously, a tiny
part of the continuum becomes solid and the rest of the flow disappears. If
that tiny new solid particle is rotating, rather than just moving with the
flow, then there is vorticity in the flow. In the figure below, the left
subfigure demonstrates no vorticity, and the right subfigure demonstrates
existence of vorticity.
      [Illustration_of_vorticity.svg]
***** Mathematical definition[edit] *****
Mathematically, the vorticity of a three-dimensional flow is a pseudovector
field, usually denoted by Ïâ, defined as the curl or rotational of the
velocity field vâ describing the continuum motion. In Cartesian_coordinates:
                &#x03C9; &#x2192;    = &#x2207; &#x00D7;    v &#x2192;       =
      (      &#x2202;  &#x2202; x        &#x2202;  &#x2202; y        &#x2202;
      &#x2202; z       )   &#x00D7;   (     v  x      v  y      v  z      )
      =   (       &#x2202;  v  z     &#x2202; y    &#x2212;    &#x2202;  v  y
      &#x2202; z         &#x2202;  v  x     &#x2202; z    &#x2212;    &#x2202;
      v  z     &#x2202; x         &#x2202;  v  y     &#x2202; x    &#x2212;
      &#x2202;  v  x     &#x2202; y       )    .       {\displaystyle {\begin
      {aligned}{\vec {\omega }}=\nabla \times {\vec {v}}&={\begin{pmatrix}
      {\frac {\partial }{\partial x}}&{\frac {\partial }{\partial y}}&{\frac
      {\partial }{\partial z}}\end{pmatrix}}\times {\begin{pmatrix}v_{x}&v_
      {y}&v_{z}\end{pmatrix}}\\[6px]&={\begin{pmatrix}{\frac {\partial v_{z}}
      {\partial y}}-{\frac {\partial v_{y}}{\partial z}}&{\frac {\partial v_
      {x}}{\partial z}}-{\frac {\partial v_{z}}{\partial x}}&{\frac {\partial
      v_{y}}{\partial x}}-{\frac {\partial v_{x}}{\partial y}}\end
      {pmatrix}}\,.\end{aligned}}}  [{\displaystyle {\begin{aligned}{\vec
      {\omega }}=\nabla \times {\vec {v}}&={\begin{pmatrix}{\frac {\partial }
      {\partial x}}&{\frac {\partial }{\partial y}}&{\frac {\partial }{\partial
      z}}\end{pmatrix}}\times {\begin{pmatrix}v_{x}&v_{y}&v_{z}\end{pmatrix}}\\
      [6px]&={\begin{pmatrix}{\frac {\partial v_{z}}{\partial y}}-{\frac
      {\partial v_{y}}{\partial z}}&{\frac {\partial v_{x}}{\partial z}}-{\frac
      {\partial v_{z}}{\partial x}}&{\frac {\partial v_{y}}{\partial x}}-{\frac
      {\partial v_{x}}{\partial y}}\end{pmatrix}}\,.\end{aligned}}}]
In words, the vorticity tells how the velocity vector changes when one moves by
an infinitesimal distance in a direction perpendicular to it.
In a two-dimensional flow where the velocity is independent of the z coordinate
and has no z component, the vorticity vector is always parallel to the z axis,
and therefore can be expressed as a scalar field multiplied by a constant unit
vector zâ:
                &#x03C9; &#x2192;    = &#x2207; &#x00D7;    v &#x2192;       =
      (      &#x2202;  &#x2202; x        &#x2202;  &#x2202; y        &#x2202;
      &#x2202; z       )   &#x00D7;  (   v  x   ,  v  y   , 0  )        =
      (     &#x2202;  v  y     &#x2202; x    &#x2212;    &#x2202;  v  x
      &#x2202; y     )     z &#x2192;     .       {\displaystyle {\begin
      {aligned}{\vec {\omega }}=\nabla \times {\vec {v}}&={\begin{pmatrix}
      {\frac {\partial }{\partial x}}&{\frac {\partial }{\partial y}}&{\frac
      {\partial }{\partial z}}\end{pmatrix}}\times \left(v_{x},v_{y},0\right)\\
      [6px]&=\left({\frac {\partial v_{y}}{\partial x}}-{\frac {\partial v_{x}}
      {\partial y}}\right){\vec {z}}\,.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}{\vec {\omega }}=\nabla \times {\vec {v}}&={\begin{pmatrix}
      {\frac {\partial }{\partial x}}&{\frac {\partial }{\partial y}}&{\frac
      {\partial }{\partial z}}\end{pmatrix}}\times \left(v_{x},v_{y},0\right)\\
      [6px]&=\left({\frac {\partial v_{y}}{\partial x}}-{\frac {\partial v_{x}}
      {\partial y}}\right){\vec {z}}\,.\end{aligned}}}]
***** Vorticity to Velocity[edit] *****
The inverse curl of a three-dimensional vector field can be obtained with the
Biot-Savart_law up to an integration_constant, hâ:
            v &#x2192;    ( p ) =   1  4 &#x03C0;    &#x222D;       &#x03C9;
      &#x2192;    ( x ) &#x00D7; ( p &#x2212; x )   &#x2016; p &#x2212; x
      &#x2016;  3      d x +    h &#x2192;      {\displaystyle {\vec {v}}(p)=
      {\frac {1}{4\pi }}\iiint {\frac {{\vec {\omega }}(x)\times (p-x)}{\|p-
      x\|^{3}}}dx+{\vec {h}}}  [{\displaystyle {\vec {v}}(p)={\frac {1}{4\pi
      }}\iiint {\frac {{\vec {\omega }}(x)\times (p-x)}{\|p-x\|^{3}}}dx+{\vec
      {h}}}]
The vector field in the integrand has the shape of a rotation of center x, axis
Ïâ and falloff 1/||p-x||^3. Thus the resulting velocity can be understood as
the field induced at p by a continuum of paddle wheels defined by vorticity.
Because the integrand has a zero divergence, the Biot-Savart integral produces
an incompressible_vector_field. The integration_constant, hâ, is an
irrotational_field defined by the boundary_conditions and the differential
properties of vâ. If vâ is known to be incompressible, then hâ must be
the gradient of a harmonic_field and is a solution to Laplaceâs_equation.
Because of the singularity of the integrand when p=x, this integral usually
cannot be computed with a Riemann_sum and requires finding a set of simple
shapes on which it has a closed_form. One application for this formula is to
recover the velocity field of a vorticity field that has evolved in time.
***** Evolution[edit] *****
The evolution of the vorticity field in time is described by the vorticity
equation, which can be derived from the NavierâStokes_equations.
In many real flows where the viscosity can be neglected (more precisely, in
flows with high Reynolds_number), the vorticity field can be modeled well by a
collection of discrete vortices, the vorticity being negligible everywhere
except in small regions of space surrounding the axes of the vortices. This is
clearly true in the case of two-dimensional potential_flow (i.e. two-
dimensional zero viscosity flow), in which case the flowfield can be modeled as
a complex-valued field on the complex_plane.
Vorticity is a useful tool to understand how the ideal potential flow solutions
can be perturbed to model real flows. In general, the presence of viscosity
causes a diffusion of vorticity away from the vortex cores into the general
flow field. This flow is accounted for by the diffusion term in the vorticity
transport equation. Thus, in cases of very viscous flows (e.g. Couette_Flow),
the vorticity will be diffused throughout the flow field and it is probably
simpler to look at the velocity field than at the vorticity.
***** Vortex lines and vortex tubes[edit] *****
A vortex line or vorticity line is a line which is everywhere tangent to the
local vorticity vector. Vortex lines are defined by the relation[4]
            d x   &#x03C9;  x     =    d y   &#x03C9;  y     =    d z
      &#x03C9;  z      ,   {\displaystyle {\frac {dx}{\omega _{x}}}={\frac {dy}
      {\omega _{y}}}={\frac {dz}{\omega _{z}}}\,,}  [{\displaystyle {\frac {dx}
      {\omega _{x}}}={\frac {dy}{\omega _{y}}}={\frac {dz}{\omega _{z}}}\,,}]
where Ïâ = (Ïx, Ïy, Ïz) is the vorticity vector in Cartesian_coordinates.
A vortex tube is the surface in the continuum formed by all vortex lines
passing through a given (reducible) closed curve in the continuum. The
'strength' of a vortex tube (also called vortex flux)[5] is the integral of the
vorticity across a cross-section of the tube, and is the same everywhere along
the tube (because vorticity has zero divergence). It is a consequence of
Helmholtz's_theorems (or equivalently, of Kelvin's_circulation_theorem) that in
an inviscid fluid the 'strength' of the vortex tube is also constant with time.
Viscous effects introduce frictional losses and time dependence.
In a three-dimensional flow, vorticity (as measured by the volume_integral of
the square of its magnitude) can be intensified when a vortex line is extended
â a phenomenon known as vortex_stretching.[6] This phenomenon occurs in the
formation of a bathtub vortex in outflowing water, and the build-up of a
tornado by rising air currents.
Helicity is vorticity in motion along a third axis in a corkscrew fashion.
***** Vorticity meters[edit] *****
**** Rotating-vane vorticity meter[edit] ****
A rotating-vane vorticity meter was invented by Russian hydraulic engineer A.
Ya. Milovich (1874â1958). In 1913 he proposed a cork with four blades
attached as a device qualitatively showing the magnitude of the vertical
projection of the vorticity and demonstrated a motion-picture photography of
float's motion on the water surface in a model of river bend.[7]
Rotating-vane vorticity meters are commonly shown in educational films on
continuum mechanics (famous examples include the NCFMF's "Vorticity"[8] and
"Fundamental Principles of Flow" by Iowa Institute of Hydraulic Research[9]).
**** Non-rotating vorticity meters[edit] ****
[[icon]] This section is empty. You can help by adding_to_it. (July 2014)
***** Specific sciences[edit] *****
**** Aeronautics[edit] ****
In aerodynamics, the lift distribution over a finite wing may be approximated
by assuming that each segment of the wing has a semi-infinite trailing vortex
behind it. It is then possible to solve for the strength of the vortices using
the criterion that there be no flow induced through the surface of the wing.
This procedure is called the vortex panel method of computational_fluid
dynamics. The strengths of the vortices are then summed to find the total
approximate circulation about the wing. According to the KuttaâJoukowski
theorem, lift is the product of circulation, airspeed, and air density.
**** Atmospheric sciences[edit] ****
The relative vorticity is the vorticity relative to the Earth induced by the
air velocity field. This air velocity field is often modeled as a two-
dimensional flow parallel to the ground, so that the relative vorticity vector
is generally scalar rotation quantity perpendicular to the ground. Vorticity is
positive when - looking down onto the earth's surface - the wind turns
counterclockwise. In the northern hemisphere, positive vorticity is called
cyclonic_rotation, and negative vorticity is anticyclonic_rotation; the
nomenclature is reversed in the Southern Hemisphere.
The absolute vorticity is computed from the air velocity relative to an
inertial frame, and therefore includes a term due to the Earth's rotation, the
Coriolis_parameter.
The potential_vorticity is absolute vorticity divided by the vertical spacing
between levels of constant (potential)_temperature (or entropy). The absolute
vorticity of an air mass will change if the air mass is stretched (or
compressed) in the vertical direction, but the potential vorticity is conserved
in an adiabatic flow. As adiabatic flow predominates in the atmosphere, the
potential vorticity is useful as an approximate tracer of air masses in the
atmosphere over the timescale of a few days, particularly when viewed on levels
of constant entropy.
The barotropic_vorticity_equation is the simplest way for forecasting the
movement of Rossby_waves (that is, the troughs and ridges of 500 hPa
geopotential_height) over a limited amount of time (a few days). In the 1950s,
the first successful programs for numerical_weather_forecasting utilized that
equation.
In modern numerical weather forecasting models and general_circulation_models
(GCMs), vorticity may be one of the predicted variables, in which case the
corresponding time-dependent equation is a prognostic_equation.
Helicity of the air motion is important in forecasting supercells and the
potential for tornadic activity.
***** See also[edit] *****
    * Barotropic_vorticity_equation
    * D'Alembert's_paradox
    * Enstrophy
    * Velocity_potential
    * Vortex
    * Vortex_tube
    * Vortex_stretching
    * Vortical
    * Horseshoe_vortex
    * Wingtip_vortices
**** Fluid dynamics[edit] ****
    * BiotâSavart_law
    * Circulation
    * Vorticity_equations
    * KuttaâJoukowski_theorem
**** Atmospheric sciences[edit] ****
    * Prognostic_equation
    * Carl-Gustaf_Rossby
    * Hans_Ertel
***** References[edit] *****
   1. ^ Lecture_Notes_from_University_of_Washington Archived October 16, 2015,
      at the Wayback_Machine
   2. ^ a b Clancy, L.J., Aerodynamics, Section 7.11
   3. ^ Truesdell, C. (1954). The kinematics of vorticity (Vol. 954).
      Bloomington: Indiana University Press.
   4. ^Kundu P and Cohen I. Fluid Mechanics.
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
   6. ^ Introduction_to_Astrophysical_Gas_Dynamics Archived June 14, 2011, at
      the Wayback_Machine
   7. ^ Batchelor, section 5.2
   8. ^Joukovsky_N.E. (1914). "On the motion of water at a turn of a river".
      Matematicheskii_Sbornik. 28.
   9. . Reprinted in:Collected_works. 4. Moscow; Leningrad. 1937.
      pp. 193â216, 231â233 (abstract in English).
  10.  "Professor Milovich's float", as Joukovsky refers this vorticity meter
      to, is schematically shown in figure on page 196 of Collected works.
  11. ^ National_Committee_for_Fluid_Mechanics_Films Archived October 21, 2016,
      at the Wayback_Machine
  12. ^ Films_by_Hunter_Rouse_â_IIHR_â_Hydroscience_&_Engineering Archived
      April 21, 2016, at the Wayback_Machine
***** Bibliography[edit] *****
    * Clancy, L.J. (1975), Aerodynamics, Pitman Publishing Limited, London
ISBN 0-273-01120-0
"Weather_Glossary"' The Weather Channel Interactive, Inc.. 2004.
"Vorticity". Integrated Publishing.
***** Further reading[edit] *****
    * Batchelor,_G._K. (2000) [1967], An Introduction to Fluid Dynamics,
      Cambridge University Press, ISBN 0-521-66396-2
Ohkitani, K., "Elementary Account Of Vorticity And Related Equations".
Cambridge University Press. January 30, 2005.
ISBN 0-521-81984-9
Chorin,_Alexandre_J., "Vorticity and Turbulence". Applied Mathematical
Sciences, Vol 103, Springer-Verlag. March 1, 1994.
ISBN 0-387-94197-5
Majda,_Andrew_J., Andrea L. Bertozzi, "Vorticity and Incompressible Flow".
Cambridge University Press; 2002.
ISBN 0-521-63948-4
Tritton, D. J., "Physical Fluid Dynamics". Van Nostrand Reinhold, New York.
1977.
ISBN 0-19-854493-6
Arfken, G., "Mathematical Methods for Physicists", 3rd ed. Academic Press,
Orlando, Florida. 1985.
ISBN 0-12-059820-5
***** External links[edit] *****
 Wikimedia Commons has media related to Vorticity.
    * Weisstein, Eric W., "Vorticity". Scienceworld.wolfram.com.
    * Doswell III, Charles A., "A_Primer_on_Vorticity_for_Application_in
      Supercells_and_Tornadoes". Cooperative Institute for Mesoscale
      Meteorological Studies, Norman, Oklahoma.
    * Cramer, M. S., "NavierâStokes Equations -- Vorticity_Transport
      Theorems: Introduction". Foundations of Fluid Mechanics.
    * Parker, Douglas, "ENVI 2210 - Atmosphere and Ocean Dynamics, 9:
      Vorticity". School of the Environment, University of Leeds. September
      2001.
    * Graham,_James_R., "Astronomy 202: Astrophysical Gas Dynamics". Astronomy
      Department, UC_Berkeley.
          o "The_vorticity_equation:_incompressible_and_barotropic_fluids".
          o "Interpretation_of_the_vorticity_equation".
          o "Kelvin's_vorticity_theorem_for_incompressible_or_barotropic_flow".
    * "Spherepack_3.1". (includes a collection of FORTRAN vorticity program)
    * "Mesoscale_Compressible_Community_(MC2)[permanent_dead_link] Real-Time
      Model Predictions". (Potential vorticity analysis)
    * v
    * t
    * e
Meteorological data and variables
                 * Adiabatic_processes
                 * Advection
                 * Buoyancy
                 * Lapse_rate
                 * Lightning
General          * Surface_solar_radiation
                 * Surface_weather_analysis
                 * Visibility
                 * Vorticity
                 * Wind
                 * Wind_shear
                 * Cloud
                 * Cloud_condensation_nuclei_(CCN)
                 * Fog
Condensation     * Convective_condensation_level_(CCL)
                 * Lifted_condensation_level_(LCL)
                 * Precipitation
                 * Water_vapor
                 * Convective_available_potential_energy_(CAPE)
                 * Convective_inhibition_(CIN)
                 * Convective_instability
                 * Convective_momentum_transport
                 * Convective_temperature_(Tc)
                 * Equilibrium_level_(EL)
Convection       * Free_convective_layer_(FCL)
                 * Helicity
                 * K_Index
                 * Level_of_free_convection_(LFC)
                 * Lifted_index_(LI)
                 * Maximum_parcel_level_(MPL)
                 * Bulk_Richardson_number_(BRN)
                 * Dew_point_(Td)
                 * Dew_point_depression
                 * Dry-bulb_temperature
                 * Equivalent_temperature_(Te)
                 * Forest_fire_weather_index
                 * Haines_Index
                 * Heat_index
                 * Humidex
                 * Humidity
Temperature      * Relative_humidity_(RH)
                 * Mixing_ratio
                 * Potential_temperature_(Î¸)
                 * Equivalent_potential_temperature_(Î¸e)
                 * Sea_surface_temperature_(SST)
                 * Thermodynamic_temperature
                 * Vapor_pressure
                 * Virtual_temperature
                 * Wet-bulb_temperature
                 * Wet-bulb_potential_temperature
                 * Wind_chill
                 * Atmospheric_pressure
                 * Baroclinity
Pressure         * Barotropicity
                 * Pressure_gradient
                 * Pressure-gradient_force_(PGF)

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Vorticity&oldid=902397435"
Categories:
    * Continuum_mechanics
    * Fluid_dynamics
Hidden categories:
    * Webarchive_template_wayback_links
    * Articles_lacking_in-text_citations_from_May_2009
    * All_articles_lacking_in-text_citations
    * Articles_to_be_expanded_from_July_2014
    * All_articles_to_be_expanded
    * Articles_with_empty_sections_from_July_2014
    * All_articles_with_empty_sections
    * Articles_using_small_message_boxes
    * Commons_category_link_from_Wikidata
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_January_2018
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
**** In other projects ****
    * Wikimedia_Commons
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 18 June 2019, at 14:59 (UTC).
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
