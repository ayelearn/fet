The following text has been accessed from https://en.wikipedia.org/wiki/Yield_(engineering) at Thu Aug 8 22:56:48 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Yield (engineering) ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
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
The yield point is the point on a stressâstrain curve that indicates the
limit of elastic behavior and the beginning plastic behavior. Yield strength or
yield stress is the material_property defined as the stress at which a material
begins to deform_plastically whereas yield point is the point where nonlinear
(elastic + plastic) deformation begins. Prior to the yield point the material
will deform elastically and will return to its original shape when the applied
stress is removed. Once the yield point is passed, some fraction of the
deformation will be permanent and non-reversible.
The yield point determines the limits of performance for mechanical components,
since it represents the upper limit to forces that can be applied without
permanent deformation. In structural_engineering, this is a soft failure mode
which does not normally cause catastrophic_failure or ultimate_failure unless
it accelerates buckling.
Advances in measurement techniques allow higher precision mapping of the yield
point which, as Marcus Reiner stated, showed "there was no yield point"[1]
Yield strength is the critical material property exploited by many fundamental
techniques of material-working: to reshape material with pressure (such as
forging, rolling, pressing, bending, extruding, or hydroforming), to separate
material by cutting (such as machining) or shearing, and to join components
rigidly with fasteners. Yield load can be taken as the load applied to the
centre of a carriage spring to straighten its leaves.
The offset yield point (or proof stress) is the stress at which 0.2% plastic
deformation occurs.
In the three-dimensional principal stresses (     &#x03C3;  1   ,  &#x03C3;  2
,  &#x03C3;  3     {\displaystyle \sigma _{1},\sigma _{2},\sigma _{3}}  [
{\displaystyle \sigma _{1},\sigma _{2},\sigma _{3}}]), an infinite number of
yield points form together a yield_surface.
⁰
***** Contents *****
    * 1_Definition
    * 2_Theoretical_yield_strength
          o 2.1_Derivation
          o 2.2_Typical_values_of_theoretical_and_experimental_yield_stress
    * 3_Yield_criterion
          o 3.1_Isotropic_yield_criteria
          o 3.2_Anisotropic_yield_criteria
    * 4_Factors_influencing_yield_strength
          o 4.1_Strengthening_mechanisms
                # 4.1.1_Work_hardening
                # 4.1.2_Solid_solution_strengthening
                # 4.1.3_Particle/precipitate_strengthening
                # 4.1.4_Grain_boundary_strengthening
    * 5_Testing
    * 6_Implications_for_structural_engineering
    * 7_Typical_yield_and_ultimate_strengths
    * 8_See_also
    * 9_References
          o 9.1_Notes
          o 9.2_Bibliography
***** Definition[edit] *****
Stressâstrain_curve showing typical yield behavior for nonferrous_alloys.
(Stress,     &#x03C3;   {\displaystyle \sigma }  [\sigma ], shown as a function
of strain,     &#x03F5;   {\displaystyle \epsilon }  [\epsilon ].)
   1. True_elastic_limit
   2. Proportionality_limit
   3. Elastic_limit
   4. Offset yield_strength
It is often difficult to precisely define yielding due to the wide variety of
stressâstrain_curves exhibited by real materials. In addition, there are
several possible ways to define yielding:[2]
  True elastic limit
      The lowest stress at which dislocations move. This definition is rarely
      used, since dislocations move at very low stresses, and detecting such
      movement is very difficult.
  Proportionality limit
      Up to this amount of stress, stress is proportional to strain (Hooke's
      law), so the stressâstrain graph is a straight line, and the gradient
      will be equal to the elastic_modulus of the material.
  Elastic limit (yield strength)
      Beyond the elastic limit, permanent deformation will occur. The elastic
      limit is therefore the lowest stress point at which permanent deformation
      can be measured. This requires a manual load-unload procedure, and the
      accuracy is critically dependent on the equipment used and operator
      skill. For elastomers, such as rubber, the elastic limit is much larger
      than the proportionality limit. Also, precise strain measurements have
      shown that plastic strain begins at low stresses.[3][4]
  Yield point
      The point in the stressâstrain curve at which the curve levels off and
      plastic deformation begins to occur.[5]
  Offset yield point (proof stress)
      When a yield point is not easily defined based on the shape of the
      stressâstrain curve an offset yield point is arbitrarily defined. The
      value for this is commonly set at 0.1% or 0.2% plastic strain.[6] The
      offset value is given as a subscript, e.g., Rp0.2 = 310 MPa or Rp1.0= 350
      N/mmÂ².[7] For most practical engineering uses, this Rp0.2 is multiplied
      by a factor of safety to obtain a lower value of the offset yield point
      (Rv0.2).[8] High strength steel and aluminum alloys do not exhibit a
      yield point, so this offset yield point is used on these materials.[6]
  Upper and lower yield points
      Some metals, such as mild_steel, reach an upper yield point before
      dropping rapidly to a lower yield point. The material response is linear
      up until the upper yield point, but the lower yield point is used in
      structural engineering as a conservative value. If a metal is only
      stressed to the upper yield point, and beyond, LÃ¼ders_bands can develop.
      [9]
***** Theoretical yield strength[edit] *****
The theoretical yield strength can be estimated by considering the process of
yield at the atomic level. In a perfect crystal, shearing results in the
displacement of an entire plane of atoms by one interatomic separation
distance, b, relative to the plane below. In order for the atoms to move,
considerable force must be applied to overcome the lattice energy and move the
atoms in the top plane over the lower atoms and into a new lattice site. The
applied stress to overcome the resistance of a perfect lattice to shear is the
theoretical yield strength, τmax.
**** Derivation[edit] ****
The stress displacement curve of a plane of atoms varies sinusoidally as stress
peaks when an atom is forced over the atom below and then falls as the atom
slides into the next lattice point.[10]
         &#x03C4; =  &#x03C4;  max   sin &#x2061;  (    2 &#x03C0; x  b   )
      {\displaystyle \tau =\tau _{\max }\sin \left({\frac {2\pi x}{b}}\right)}
      [{\displaystyle \tau =\tau _{\max }\sin \left({\frac {2\pi x}
      {b}}\right)}]
where     b   {\displaystyle b}  [b] is the interatomic separation distance.
Since τ = G γ and dτ/dγ = G at small strains (ie. Single atomic distance
displacements), this equation becomes:
         G =    d &#x03C4;   d x    =    2 &#x03C0;  b    &#x03C4;  max   cos
      &#x2061;  (    2 &#x03C0; x  b   )  =    2 &#x03C0;  b    &#x03C4;  max
      {\displaystyle G={\frac {d\tau }{dx}}={\frac {2\pi }{b}}\tau _{\max }\cos
      \left({\frac {2\pi x}{b}}\right)={\frac {2\pi }{b}}\tau _{\max }}  [
      {\displaystyle G={\frac {d\tau }{dx}}={\frac {2\pi }{b}}\tau _{\max }\cos
      \left({\frac {2\pi x}{b}}\right)={\frac {2\pi }{b}}\tau _{\max }}]
For small displacement of γ=x/a, where a is the spacing of atoms on the slip
plane, this can be rewritten as:
         G =    d &#x03C4;   d &#x03B3;    =    2 &#x03C0;  b    &#x03C4;  max
      {\displaystyle G={\frac {d\tau }{d\gamma }}={\frac {2\pi }{b}}\tau _{\max
      }}  [{\displaystyle G={\frac {d\tau }{d\gamma }}={\frac {2\pi }{b}}\tau _
      {\max }}]
Giving a value of τmax equal to:
          &#x03C4;  max   =    G b   2 &#x03C0; a      {\displaystyle \tau _
      {\max }={\frac {Gb}{2\pi a}}}  [{\displaystyle \tau _{\max }={\frac {Gb}
      {2\pi a}}}]
The theoretical yield strength can be approximated as τmax = G/30.
**** Typical values of theoretical and experimental yield stress[edit] ****
The theoretical yield strength of a perfect crystal is much higher than the
observed stress at initiation of plastic flow. Theoretical and experimental
yield stresses of common materials are shown in the table below.[11]
Material Theoretical Shear Strength (GPa) Experimental Shear Strength (MPa)
Ag       1.0                              0.37
Al       0.9                              0.78
Cu       1.4                              0.49
Ni       2.6                              3.2
α-Fe    2.6                              27.5
That experimentally measured yield strength is significantly lower than the
expected theoretical value can be explained by the presence of dislocations and
defects in the materials. Indeed, whiskers with perfect single crystal
structure and defect free surfaces have been shown to demonstrate yield stress
approaching the theoretical value. For example, nanowhiskers of copper were
shown to undergo brittle fracture at 1 GPa,[12] a value much higher than the
strength of bulk copper and approaching the theoretical value.
***** Yield criterion[edit] *****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (June 2013)(Learn_how_and_when_to_remove_this_template_message)
A yield criterion, often expressed as yield surface, or yield locus, is a
hypothesis concerning the limit of elasticity under any combination of
stresses. There are two interpretations of yield criterion: one is purely
mathematical in taking a statistical approach while other models attempt to
provide a justification based on established physical principles. Since stress
and strain are tensor qualities they can be described on the basis of three
principal directions, in the case of stress these are denoted by      &#x03C3;
1       {\displaystyle \sigma _{1}\,\!}  [{\displaystyle \sigma _{1}\,\!}],
&#x03C3;  2       {\displaystyle \sigma _{2}\,\!}  [{\displaystyle \sigma _
{2}\,\!}], and      &#x03C3;  3       {\displaystyle \sigma _{3}\,\!}  [
{\displaystyle \sigma _{3}\,\!}].
The following represent the most common yield criterion as applied to an
isotropic material (uniform properties in all directions). Other equations have
been proposed or are used in specialist situations.
**** Isotropic yield criteria[edit] ****
Maximum Principal Stress Theory â by W.J.M Rankine(1850). Yield occurs when
the largest principal stress exceeds the uniaxial tensile yield strength.
Although this criterion allows for a quick and easy comparison with
experimental data it is rarely suitable for design purposes. This theory gives
good predictions for brittle materials.
          &#x03C3;  1   &#x2264;  &#x03C3;  y       {\displaystyle \sigma _
      {1}\leq \sigma _{y}\,\!}  [{\displaystyle \sigma _{1}\leq \sigma _
      {y}\,\!}]
Maximum Principal Strain Theory â by St.Venant. Yield occurs when the maximum
principal strain reaches the strain corresponding to the yield point during a
simple tensile test. In terms of the principal stresses this is determined by
the equation:
          &#x03C3;  1   &#x2212; &#x03BD;  (   &#x03C3;  2   +  &#x03C3;  3
      )  &#x2264;  &#x03C3;  y   .     {\displaystyle \sigma _{1}-\nu \left
      (\sigma _{2}+\sigma _{3}\right)\leq \sigma _{y}.\,\!}  [{\displaystyle
      \sigma _{1}-\nu \left(\sigma _{2}+\sigma _{3}\right)\leq \sigma _
      {y}.\,\!}]
Maximum Shear Stress Theory â Also known as the Tresca_yield_criterion, after
the French scientist Henri_Tresca. This assumes that yield occurs when the
shear stress     &#x03C4;    {\displaystyle \tau \!}  [\tau \!] exceeds the
shear yield strength      &#x03C4;  y      {\displaystyle \tau _{y}\!}  [\tau _
{y}\!]:
         &#x03C4; =     &#x03C3;  1   &#x2212;  &#x03C3;  3    2   &#x2264;
      &#x03C4;  y   .     {\displaystyle \tau ={\frac {\sigma _{1}-\sigma _{3}}
      {2}}\leq \tau _{y}.\,\!}  [{\displaystyle \tau ={\frac {\sigma _{1}-
      \sigma _{3}}{2}}\leq \tau _{y}.\,\!}]
Total Strain Energy Theory â This theory assumes that the stored energy
associated with elastic deformation at the point of yield is independent of the
specific stress tensor. Thus yield occurs when the strain energy per unit
volume is greater than the strain energy at the elastic limit in simple
tension. For a 3-dimensional stress state this is given by:
          &#x03C3;  1   2   +  &#x03C3;  2   2   +  &#x03C3;  3   2   &#x2212;
      2 &#x03BD;  (   &#x03C3;  1    &#x03C3;  2   +  &#x03C3;  2    &#x03C3;
      3   +  &#x03C3;  1    &#x03C3;  3    )  &#x2264;  &#x03C3;  y   2   .
      {\displaystyle \sigma _{1}^{2}+\sigma _{2}^{2}+\sigma _{3}^{2}-2\nu \left
      (\sigma _{1}\sigma _{2}+\sigma _{2}\sigma _{3}+\sigma _{1}\sigma _
      {3}\right)\leq \sigma _{y}^{2}.\,\!}  [{\displaystyle \sigma _{1}^
      {2}+\sigma _{2}^{2}+\sigma _{3}^{2}-2\nu \left(\sigma _{1}\sigma _
      {2}+\sigma _{2}\sigma _{3}+\sigma _{1}\sigma _{3}\right)\leq \sigma _{y}^
      {2}.\,\!}]
Maximum Distortion Energy Theory (von_Mises_yield_criterion) â This theory
proposes that the total strain energy can be separated into two components: the
volumetric (hydrostatic) strain energy and the shape (distortion or shear)
strain energy. It is proposed that yield occurs when the distortion component
exceeds that at the yield point for a simple tensile test. This theory is also
known as the von_Mises_yield_criterion.
Based on a different theoretical underpinning this expression is also referred
to as octahedral shear stress theory.[citation_needed]
Other commonly used isotropic yield criteria are the
    * von_Mises_yield_criterion
    * Mohr-Coulomb_yield_criterion
    * Drucker-Prager_yield_criterion
    * Bresler-Pister_yield_criterion
    * Willam-Warnke_yield_criterion
The yield_surfaces corresponding to these criteria have a range of forms.
However, most isotropic yield criteria correspond to convex yield surfaces.
**** Anisotropic yield criteria[edit] ****
When a metal is subjected to large plastic deformations the grain sizes and
orientations change in the direction of deformation. As a result, the plastic
yield behavior of the material shows directional dependency. Under such
circumstances, the isotropic yield criteria such as the von Mises yield
criterion are unable to predict the yield behavior accurately. Several
anisotropic yield criteria have been developed to deal with such situations.
Some of the more popular anisotropic yield criteria are:
    * Hill's_quadratic_yield_criterion
    * Generalized_Hill_yield_criterion
    * Hosford_yield_criterion
***** Factors influencing yield strength[edit] *****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (June 2013)(Learn_how_and_when_to_remove_this_template_message)
The stress at which yield occurs is dependent on both the rate of deformation
(strain rate) and, more significantly, the temperature at which the deformation
occurs. In general, the yield strength increases with strain rate and decreases
with temperature. When the latter is not the case, the material is said to
exhibit yield_strength_anomaly, which is typical for superalloys and leads to
their use in applications requiring high strength at high temperatures.
Early work by Alder and Philips[13] found that the relationship between yield
strength and strain rate (at constant temperature) was best described by a
power law relationship of the form
          &#x03C3;  y   = C   (    &#x03F5; &#x02D9;    )   m
      {\displaystyle \sigma _{y}=C\left({\dot {\epsilon }}\right)^{m}\,\!}  [
      {\displaystyle \sigma _{y}=C\left({\dot {\epsilon }}\right)^{m}\,\!}]
where C is a constant and m is the strain rate sensitivity. The latter
generally increases with temperature, and materials where m reaches a value
greater than ~0.5 tend to exhibit super_plastic_behavior. m can be found from a
log-log plot of yield strength at a fixed plastic strain versus the strain
rate.[14]
         m =    &#x2202; ln &#x2061; &#x03C3; ( &#x03F5; )   &#x2202; ln
      &#x2061; (    &#x03F5; &#x02D9;    )      {\displaystyle m={\frac
      {\partial \ln \sigma (\epsilon )}{\partial \ln({\dot {\epsilon }})}}}  [
      {\displaystyle m={\frac {\partial \ln \sigma (\epsilon )}{\partial \ln(
      {\dot {\epsilon }})}}}]
Later, more complex equations were proposed that simultaneously dealt with both
temperature and strain rate:
          &#x03C3;  y   =   1 &#x03B1;    sinh  &#x2212; 1   &#x2061;   [   Z A
      ]    1 n        {\displaystyle \sigma _{y}={\frac {1}{\alpha }}\sinh ^{-
      1}\left[{\frac {Z}{A}}\right]^{\frac {1}{n}}\,\!}  [{\displaystyle \sigma
      _{y}={\frac {1}{\alpha }}\sinh ^{-1}\left[{\frac {Z}{A}}\right]^{\frac
      {1}{n}}\,\!}]
where Î± and A are constants and Z is the temperature-compensated strain-rate
â often described by the Zener-Hollomon_parameter:
         Z =  (    &#x03F5; &#x02D9;    )  exp &#x2061;  (    Q  H W    R T
      )      {\displaystyle Z=\left({\dot {\epsilon }}\right)\exp \left({\frac
      {Q_{HW}}{RT}}\right)\,\!}  [{\displaystyle Z=\left({\dot {\epsilon
      }}\right)\exp \left({\frac {Q_{HW}}{RT}}\right)\,\!}]
where QHW is the activation energy for hot deformation and T is the absolute
temperature.
**** Strengthening mechanisms[edit] ****
There are several ways in which crystalline and amorphous materials can be
engineered to increase their yield strength. By altering dislocation density,
impurity levels, grain size (in crystalline materials), the yield strength of
the material can be fine tuned. This occurs typically by introducing defects
such as impurities dislocations in the material. To move this defect
(plastically deforming or yielding the material), a larger stress must be
applied. This thus causes a higher yield stress in the material. While many
material properties depend only on the composition of the bulk material, yield
strength is extremely sensitive to the materials processing as well.
These mechanisms for crystalline materials include
    * Work_hardening
    * Solid_solution_strengthening
    * Precipitation_strengthening
    * Grain_boundary_strengthening
*** Work hardening[edit] ***
Where deforming the material will introduce dislocations, which increases their
density in the material. This increases the yield strength of the material,
since now more stress must be applied to move these dislocations through a
crystal lattice. Dislocations can also interact with each other, becoming
entangled.
The governing formula for this mechanism is:
         &#x0394;  &#x03C3;  y   = G b   &#x03C1;     {\displaystyle \Delta
      \sigma _{y}=Gb{\sqrt {\rho }}}  [{\displaystyle \Delta \sigma _{y}=Gb
      {\sqrt {\rho }}}]
where      &#x03C3;  y     {\displaystyle \sigma _{y}}  [\sigma_y] is the yield
stress, G is the shear elastic modulus, b is the magnitude of the Burgers
vector, and     &#x03C1;   {\displaystyle \rho }  [\rho ] is the dislocation
density.
*** Solid solution strengthening[edit] ***
By alloying the material, impurity atoms in low concentrations will occupy a
lattice position directly below a dislocation, such as directly below an extra
half plane defect. This relieves a tensile strain directly below the
dislocation by filling that empty lattice space with the impurity atom.
The relationship of this mechanism goes as:
         &#x0394; &#x03C4; = G b    C  s      &#x03F5;   3 2
      {\displaystyle \Delta \tau =Gb{\sqrt {C_{s}}}\epsilon ^{\frac {3}{2}}}  [
      {\displaystyle \Delta \tau =Gb{\sqrt {C_{s}}}\epsilon ^{\frac {3}{2}}}]
where     &#x03C4;   {\displaystyle \tau }  [\tau ] is the shear_stress,
related to the yield stress,     G   {\displaystyle G}  [G] and     b
{\displaystyle b}  [b] are the same as in the above example,      C  s
{\displaystyle C_{s}}  [C_{s}] is the concentration of solute and     &#x03F5;
{\displaystyle \epsilon }  [\epsilon ] is the strain induced in the lattice due
to adding the impurity.
*** Particle/precipitate strengthening[edit] ***
Where the presence of a secondary phase will increase yield strength by
blocking the motion of dislocations within the crystal. A line defect that,
while moving through the matrix, will be forced against a small particle or
precipitate of the material. Dislocations can move through this particle either
by shearing the particle, or by a process known as bowing or ringing, in which
a new ring of dislocations is created around the particle.
The shearing formula goes as:
         &#x0394; &#x03C4; =    r  particle    l  interparticle      &#x03B3;
      particle-matrix     {\displaystyle \Delta \tau ={\frac {r_{\text
      {particle}}}{l_{\text{interparticle}}}}\gamma _{\text{particle-matrix}}}
      [{\displaystyle \Delta \tau ={\frac {r_{\text{particle}}}{l_{\text
      {interparticle}}}}\gamma _{\text{particle-matrix}}}]
and the bowing/ringing formula:
         &#x0394; &#x03C4; =    G b    l  interparticle   &#x2212; 2  r
      particle        {\displaystyle \Delta \tau ={\frac {Gb}{l_{\text
      {interparticle}}-2r_{\text{particle}}}}}  [{\displaystyle \Delta \tau =
      {\frac {Gb}{l_{\text{interparticle}}-2r_{\text{particle}}}}}]
In these formulas,      r  particle      {\displaystyle r_{\text{particle}}\,}
[{\displaystyle r_{\text{particle}}\,}] is the particle radius,      &#x03B3;
particle-matrix      {\displaystyle \gamma _{\text{particle-matrix}}\,}  [
{\displaystyle \gamma _{\text{particle-matrix}}\,}] is the surface tension
between the matrix and the particle,      l  interparticle      {\displaystyle
l_{\text{interparticle}}\,}  [{\displaystyle l_{\text{interparticle}}\,}] is
the distance between the particles.
*** Grain boundary strengthening[edit] ***
Where a buildup of dislocations at a grain boundary causes a repulsive force
between dislocations. As grain size decreases, the surface area to volume ratio
of the grain increases, allowing more buildup of dislocations at the grain
edge. Since it requires a lot of energy to move dislocations to another grain,
these dislocations build up along the boundary, and increase the yield stress
of the material. Also known as Hall-Petch strengthening, this type of
strengthening is governed by the formula:
          &#x03C3;  y   =  &#x03C3;  0   + k  d  &#x2212;   1 2
      {\displaystyle \sigma _{y}=\sigma _{0}+kd^{-{\frac {1}{2}}}\,}  [
      {\displaystyle \sigma _{y}=\sigma _{0}+kd^{-{\frac {1}{2}}}\,}]
where
          &#x03C3;  0     {\displaystyle \sigma _{0}}  [\sigma _{0}] is the
      stress required to move dislocations,
      k is a material constant, and
      d is the grain size.
***** Testing[edit] *****
Yield strength testing involves taking a small sample with a fixed cross-
section area, and then pulling it with a controlled, gradually increasing force
until the sample changes shape or breaks. This is called a Tensile_Test.
Longitudinal and/or transverse strain is recorded using mechanical or optical
extensometers.
Yield behaviour can also be simulated using virtual tests (on computer models
of materials), particularly where macroscopic yield is governed by the
microstructural architecture of the material being studied.[15]
Indentation_hardness correlates roughly linearly with tensile strength for most
steels, but measurements on one material cannot be used as a scale to measure
strengths on another.[16] Hardness testing can therefore be an economical
substitute for tensile testing, as well as providing local variations in yield
strength due to, e.g., welding or forming operations. However, for critical
situations tension testing is done to eliminate ambiguity.
***** Implications for structural engineering[edit] *****
Yielded structures have a lower stiffness, leading to increased deflections and
decreased buckling strength. The structure will be permanently deformed when
the load is removed, and may have residual stresses. Engineering metals display
strain hardening, which implies that the yield stress is increased after
unloading from a yield state. Highly optimized structures, such as airplane
beams and components, rely on yielding as a fail-safe failure mode. No safety
factor is therefore needed when comparing limit loads (the highest loads
expected during normal operation) to yield criteria.[citation_needed]
***** Typical yield and ultimate strengths[edit] *****
Note: many of the values depend on manufacturing process and purity/
composition.
 _____________________________________________________________________________
|                                     |Yield    |Ultimate |          |Free    |
|Material                             |strength |strength |Density   |breaking|
|                                     |(MPa)    |(MPa)    |(g/cmÂ³)|length  |
|_____________________________________|_________|_________|__________|(km)____|
|ASTM_A36_steel_______________________|250______|400______|7.87______|3.2_____|
|Steel,_API_5L_X65[17]________________|448______|531______|7.85______|5.8_____|
|Steel,_high_strength_alloy_ASTM_A514_|690______|760______|7.85______|9.0_____|
|Steel,_prestressing_strands__________|1650_____|1860_____|7.85______|21.6____|
|Piano_wire                           |        |1740-3300|7.8       |28.7    |
|_____________________________________|_________|[18]_____|__________|________|
|Carbon_fiber_(CF,_CFK)_______________|_________|5650[19]_|1.75______|329_____|
|High-density_polyethylene_(HDPE)_____|26â3|37_______|0.95______|2.8_____|
|Polypropylene________________________|12â4|19.7â�|0.91______|1.3_____|
|Stainless_steel AISI 302 â cold-|520      |860      |         |        |
|rolled_______________________________|_________|_________|__________|________|
|Cast_iron_4.5%_C,_ASTM_A-48[20]______|[a]______|172______|7.20______|2.4_____|
|Titanium_alloy_(6%_Al,_4%_V)_________|830______|900______|4.51______|18.8____|
|Aluminium_alloy_2014-T6______________|400______|455______|2.7_______|15.1____|
|Copper_99.9%_Cu______________________|70_______|220______|8.92______|0.8_____|
|Cupronickel 10% Ni, 1.6% Fe, 1% Mn,  |130      |350      |8.94      |1.4     |
|balance_Cu___________________________|_________|_________|__________|________|
|Brass                                |Approx.  |550      |8.5       |3.8     |
|_____________________________________|200+_____|_________|__________|________|
|Spider_silk__________________________|1150_(??)|1400_____|1.31______|109_____|
|Silkworm_silk________________________|500______| _______| ________|25______|
|Aramid_(Kevlar_or_Twaron)____________|3620_____|3757_____|1.44______|256.3___|
|UHMWPE[22][23]_______________________|20_______|35[24]___|0.97______|2.1_____|
|Bone_(limb)__________________________|104â|130______| ________|3_______|
|Nylon,_type_6/6______________________|45_______|75_______| ________|2_______|
   1. ^ Grey cast iron does not have a well defined yield strength because the
      stressâstrain relationship is atypical. The yield strength can vary
      from 65 to 80% of the tensile strength.[21]
 ___________________Elements_in_the_annealed_state[25]____________________
|Element  |Young's modulus|Proof or yield stress|Ultimate tensile Strength|
|_________|(GPa)__________|(MPa)________________|(MPa)____________________|
|Aluminium|70_____________|15â20___________|40â50_______________|
|Copper___|130____________|33___________________|210______________________|
|Iron_____|211____________|80â100__________|350______________________|
|Nickel___|170____________|14â35___________|140â195_____________|
|Silicon__|107____________|5000â9000_______| _______________________|
|Tantalum_|186____________|180__________________|200______________________|
|Tin______|47_____________|9â14____________|15â200______________|
|Titanium_|120____________|100â225_________|240â370_____________|
|Tungsten_|411____________|550__________________|550â620_____________|
***** See also[edit] *****
    * Elastic_modulus
    * Linear_elasticity
    * Piola-Kirchhoff_stress_tensor
    * Specified_Minimum_Yield_Strength
    * Strain_tensor
    * Stress_concentration
    * Tensile_strength
    * Virial_stress
    * Yield_curve_(physics)
    * Yield_surface
***** References[edit] *****
**** Notes[edit] ****
   1. ^Reiner, Markus (1943), Ten Lectures on Theoretical Rheology, Jerusalem:
      Rubin Mass, p. 137
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
   3. ^ G. Dieter, Mechanical Metallurgy, McGraw-Hill, 1986
   4. ^Flinn, Richard A.; Trojan, Paul K. (1975). Engineering Materials and
      their Applications. Boston: Houghton Mifflin Company. p. 61. ISBN 978-0-
      395-18916-0.
   5. ^Kumagai, Naoichi; Sasajima, Sadao; Ito, Hidebumi (15 February 1978).
      "å²©ç³ã®é·å¹´ã¯ãªã¼ãå®é¨ :
      å·¨å¤§è©¦çç´20å¹´éã»å°è©¦çç´3å¹´éã®çµæ" [Long-term Creep
      of Rocks: Results with Large Specimens Obtained in about 20 Years and
      Those with Small Specimens in about 3 Years]. Journal of the Society of
      Materials Science (Japan) (in Japanese). 27 (293): 157â161. Retrieved
      16 June 2008.
   6. ^ Ross_1999, p. 56.
   7. ^ a b Ross_1999, p. 59.
   8. ^ ISO 6892-1:2009
   9. ^"Factor_of_safety", Wikipedia, 16 January 2019, retrieved 22 January
      2019
  10. ^ Degarmo, p. 377.
  11. ^H., Courtney, Thomas (2005). Mechanical behavior of materials. Waveland
      Press. ISBN 978-1577664253. OCLC 894800884.
  12. ^H., Courtney, Thomas (2005). Mechanical behavior of materials. Waveland
      Press. ISBN 978-1577664253. OCLC 894800884.
  13. ^Richter, Gunther (2009). "Ultrahigh Strength Single Crystalline
      Nanowhiskers Grown by Physical Vapor Deposition". Nano Letters. 9 (8):
      3048â3052. CiteSeerX 10.1.1.702.1801. doi:10.1021/nl9015107.
      PMID 19637912.
  14. ^Alder, J.F.; Phillips, V.A. (1954). "The effect of strain rate and
      temperature on the resistance of aluminium, copper, and steel to
      compression". J Inst Met. 83: 80â86.
  15. ^ Dynamic_Behavior_of_a_Rare-Earth-Containing_Mg_Alloy,_WE43B-T5,_Plate
      with_Comparison_to_Conventional_Alloy,_AM30-F_,_Sean_Agnew,_Wilburn
      Whittington,_Andrew_Oppedal,_Haitham_El_Kadiri,_Matthew_Shaeffer,_K._T.
      Ramesh,_Jishnu_Bhattacharyya,_Rick_Delorme,_Bruce_Davis_,_Volume_66,
      Issue_2_/_February,_2014
  16. ^Levrero, F.; Margetts, L.; et al. (2016). "Evaluating_the_macroscopic
      yield_behaviour_of_trabecular_bone_using_a_nonlinear_homogenisation
      approach". Journal of the Mechanical Behavior of Biomedical Materials.
      61: 384â396. doi:10.1016/j.jmbbm.2016.04.008. PMID 27108348.
  17. ^ Correlation_of_Yield_Strength_and_Tensile_Strength_with_Hardness_for
      Steels_,_E.J._Pavlina_and_C.J._Van_Tyne,_Journal_of_Materials_Engineering
      and_Performance,_Volume_17,_Number_6_/_December,_2008
  18. ^ ussteel.com
  19. ^ ASTM A228-A228M-14
  20. ^ complore.com
  21. ^ Beer,_Johnston_&_Dewolf_2001, p. 746.
  22. ^ Avallone_et_al._2006, p. 6â35.
  23. ^ Technical_Product_Data_Sheets_UHMWPE
  24. ^ unitex-deutschland.eu
  25. ^ matweb.com
  26. ^ A.M. Howatson, P.G. Lund and J.D. Todd, "Engineering Tables and Data",
      p. 41.
**** Bibliography[edit] ****
    * Avallone, Eugene A. & Baumeister III, Theodore (1996). Mark's Standard
      Handbook for Mechanical Engineers (8th ed.). New York: McGraw-Hill.
      ISBN 978-0-07-004997-0.
Avallone, Eugene A.; Baumeister, Theodore; Sadegh, Ali; Marks, Lionel Simeon
(2006). Mark's_Standard_Handbook_for_Mechanical_Engineers (11th, Illustrated
ed.). McGraw-Hill Professional. ISBN 978-0-07-142867-5.
.
Beer, Ferdinand P.; Johnston, E. Russell; Dewolf, John T. (2001). Mechanics_of
Materials (3rd ed.). McGraw-Hill. ISBN 978-0-07-365935-0.
.
Boresi, A. P., Schmidt, R. J., and Sidebottom, O. M. (1993). Advanced Mechanics
of Materials, 5th edition John Wiley & Sons.
ISBN 0-471-55157-0
Degarmo, E. Paul; Black, J T.; Kohser, Ronald A. (2003). Materials and
Processes in Manufacturing (9th ed.). Wiley. ISBN 978-0-471-65653-1.
.
Oberg, E., Jones, F. D., and Horton, H. L. (1984). Machinery's Handbook, 22nd
edition. Industrial Press.
ISBN 0-8311-1155-0
Ross, C. (1999). Mechanics_of_Solids. City: Albion/Horwood Pub. ISBN 978-1-
898563-67-9.
Shigley, J. E., and Mischke, C. R. (1989). Mechanical Engineering Design, 5th
edition. McGraw Hill.
ISBN 0-07-056899-5
Young, Warren C. & Budynas, Richard G. (2002). Roark's Formulas for Stress and
Strain, 7th edition. New York: McGraw-Hill. ISBN 978-0-07-072542-3.
Engineer's_Handbook

Retrieved from "https://en.wikipedia.org/w/index.php?title=Yield_
(engineering)&oldid=903782616"
Categories:
    * Elasticity_(physics)
    * Mechanics
    * Plasticity_(physics)
    * Solid_mechanics
    * Deformation_(mechanics)
Hidden categories:
    * CS1_Japanese-language_sources_(ja)
    * Articles_needing_additional_references_from_June_2013
    * All_articles_needing_additional_references
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2011
    * Articles_with_unsourced_statements_from_September_2007
    * Use_dmy_dates_from_November_2017
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
    * BÃ¢n-lÃ¢m-gÃº
    * Eesti
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * ×¢××¨××ª
    * æ¥æ¬èª
    * ä¸­æ
Edit_links
    * This page was last edited on 27 June 2019, at 23:13 (UTC).
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
