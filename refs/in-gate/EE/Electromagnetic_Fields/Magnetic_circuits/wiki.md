The following text has been accessed from https://en.wikipedia.org/wiki/Magnetic_circuit at Thu Aug 8 22:55:51 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Magnetic circuit ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Part of a series on
Magnetic circuits
Conventional magnetic circuits
    * Magnetomotive_force       F     {\displaystyle {\mathcal {F}}}  [
      {\mathcal {F}}]
    * Magnetic_flux     &#x03A6;   {\displaystyle \Phi }  [\Phi ]
    * Magnetic_reluctance       R     {\displaystyle {\mathcal {R}}}  [\mathcal
      R]
Phasor magnetic circuits
    * Complex_reluctance      Z  &#x03BC;     {\displaystyle Z_{\mu }}  [Z_\mu
      ]
Related concepts
    * Magnetic_permeability     &#x03BC;   {\displaystyle \mu }  [\mu ]
Gyrator-capacitor_model variables
    * Magnetic_impedance      z   M      {\displaystyle z_{\mathrm {M} }}
      [z_\mathrm{M}]
    * Effective_resistance      r   M      {\displaystyle r_{\mathrm {M} }}
      [r_\mathrm{M}]
    * Magnetic_inductivity      L   M      {\displaystyle L_{\mathrm {M} }}
      [L_\mathrm{M}]
    * Magnetic_capacitivity      C   M      {\displaystyle C_{\mathrm {M} }}
      [C_\mathrm{M}]
[Stylised_atom_with_three_Bohr_model_orbits_and_stylised_nucleus.svg] Physics
portal
    * v
    * t
    * e
A magnetic circuit is made up of one or more closed loop paths containing a
magnetic_flux. The flux is usually generated by permanent_magnets or
electromagnets and confined to the path by magnetic_cores consisting of
ferromagnetic_materials like iron, although there may be air gaps or other
materials in the path. Magnetic circuits are employed to efficiently channel
magnetic_fields in many devices such as electric_motors, generators,
transformers, relays, lifting electromagnets, SQUIDs, galvanometers, and
magnetic recording_heads.
The concept of a "magnetic circuit" exploits a one-to-one correspondence
between the equations of the magnetic field in an unsaturated ferromagnetic
material to that of an electrical_circuit. Using this concept the magnetic
fields of complex devices such as transformers can be quickly solved using the
methods and techniques developed for electrical circuits.
Some examples of magnetic circuits are:
    * horseshoe magnet with iron keeper (low-reluctance circuit)
    * horseshoe magnet with no keeper (high-reluctance circuit)
    * electric_motor (variable-reluctance circuit)
    * some types of pickup_cartridge (variable-reluctance circuits)
⁰
***** Contents *****
    * 1_Magnetomotive_force_(MMF)
    * 2_Magnetic_flux
    * 3_Ohm's_law_for_magnetic_circuits
    * 4_Reluctance
    * 5_Microscopic_origins_of_reluctance
    * 6_Summary_of_analogy_between_magnetic_circuits_and_electrical_circuits
    * 7_Limitations_of_the_analogy
    * 8_Circuit_laws
    * 9_Applications
    * 10_See_also
    * 11_References
    * 12_External_links
***** Magnetomotive force (MMF)[edit] *****
Main article: magnetomotive_force
Similar to the way that electromotive force (EMF) drives a current of
electrical charge in electrical circuits, magnetomotive_force (MMF) 'drives'
magnetic flux through magnetic circuits. The term 'magnetomotive force',
though, is a misnomer since it is not a force nor is anything moving. It is
perhaps better to call it simply MMF. In analogy to the definition of EMF, the
magnetomotive force        F      {\displaystyle \scriptstyle {\mathcal {F}}}
[\scriptstyle {\mathcal {F}}] around a closed loop is defined as:
           F   =    &#x222E;      &#x2061;  H  &#x22C5; d &#x2061;  l
      {\displaystyle {\mathcal {F}}=\oint \mathbf {H} \cdot \operatorname {d}
      \mathbf {l} }  [{\mathcal  {F}}=\oint {\mathbf  {H}}\cdot \operatorname
      {d}{\mathbf  {l}}]
The MMF represents the potential that a hypothetical magnetic_charge would gain
by completing the loop. The magnetic flux that is driven is not a current of
magnetic charge; it merely has the same relationship to MMF that electric
current has to EMF. (See microscopic origins of reluctance below for a further
description.)
The unit of magnetomotive force is the ampere-turn (At), represented by a
steady, direct electric_current of one ampere flowing in a single-turn loop of
electrically conducting material in a vacuum. The gilbert (Gb), established by
the IEC in 1930,[1] is the CGS unit of magnetomotive force and is a slightly
smaller unit than the ampere-turn. The unit is named after William_Gilbert
(1544â1603) English physician and natural philosopher.
             1   Gb     =   10  4 &#x03C0;      At        &#x2248; 0.795775
      At        {\displaystyle {\begin{aligned}1\;{\text{Gb}}&={\frac {10}{4\pi
      }}\;{\text{At}}\\&\approx 0.795775\;{\text{At}}\end{aligned}}}  [{\begin
      {aligned}1\;{\text{Gb}}&={\frac  {10}{4\pi }}\;{\text{At}}\\&\approx
      0.795775\;{\text{At}}\end{aligned}}][2]
The magnetomotive force can often be quickly calculated using AmpÃ¨re's_law.
For example, the magnetomotive force       F     {\displaystyle {\mathcal {F}}}
[{\mathcal {F}}] of long coil is:
           F   = N I   {\displaystyle {\mathcal {F}}=NI}  [{\mathcal  {F}}=NI]
where N is the number of turns and I is the current in the coil. In practice
this equation is used for the MMF of real inductors with N being the winding
number of the inducting coil.
***** Magnetic flux[edit] *****
Main article: Magnetic_flux
An applied MMF 'drives' magnetic_flux through the magnetic components of the
system. The magnetic flux through a magnetic component is proportional to the
number of magnetic_field_lines that pass through the cross sectional area of
that component. This is the net number, i.e. the number passing through in one
direction, minus the number passing through in the other direction. The
direction of the magnetic field vector B is by definition from the south to the
north pole of a magnet inside the magnet; outside the field lines go from north
to south.
The flux through an element of area perpendicular to the direction of magnetic
field is given by the product of the magnetic_field and the area element. More
generally, magnetic flux Î¦ is defined by a scalar_product of the magnetic
field and the area element vector. Quantitatively, the magnetic flux through a
surface S is defined as the integral of the magnetic field over the area of the
surface
          &#x03A6;  m   = &#x222B;      &#x222B;  S    B  &#x22C5; d &#x2061;
      S    {\displaystyle \Phi _{m}=\int \!\!\!\!\int _{S}\mathbf {B} \cdot
      \operatorname {d} \mathbf {S} }  [\Phi _{m}=\int \!\!\!\!\int _{S}
      {\mathbf  {B}}\cdot \operatorname {d}{\mathbf  S}]
For a magnetic component the area S used to calculate the magnetic flux Î¦ is
usually chosen to be the cross-sectional area of the component.
The SI unit of magnetic flux is the weber (in derived units: volt-seconds), and
the unit of magnetic field is the weber per square meter, or tesla.
***** Ohm's law for magnetic circuits[edit] *****
In electronic_circuits, Ohm's_law is an empirical relation between the EMF
E      {\displaystyle \scriptstyle {\mathcal {E}}}  [\scriptstyle {\mathcal
{E}}] applied across an element and the current I it generates through that
element. It is written as:
           E   = I R   {\displaystyle {\mathcal {E}}=IR}  [{\mathcal  {E}}=IR]
where R is the electrical_resistance of that material. There is a counterpart
to Ohm's_law used in magnetic circuits. This law is often called Hopkinson's
law, after John_Hopkinson, but was actually formulated earlier by Henry
Augustus_Rowland in 1873.[3] It states that[4][5]
           F   = &#x03A6;   R     {\displaystyle {\mathcal {F}}=\Phi {\mathcal
      {R}}}  [{\displaystyle {\mathcal {F}}=\Phi {\mathcal {R}}}]
where        F      {\displaystyle \scriptstyle {\mathcal {F}}}  [\scriptstyle
{\mathcal {F}}] is the magnetomotive force (MMF) across a magnetic element,
&#x03A6;    {\displaystyle \scriptstyle \Phi }  [\scriptstyle \Phi ] is the
magnetic_flux through the magnetic element, and        R      {\displaystyle
\scriptstyle {\mathcal {R}}}  [\scriptstyle {\mathcal  {R}}] is the magnetic
reluctance of that element. (It will be shown later that this relationship is
due to the empirical relationship between the H-field and the magnetic field B,
B=Î¼H, where Î¼ is the permeability of the material). Like Ohm's law,
Hopkinson's law can be interpreted either as an empirical equation that works
for some materials, or it may serve as a definition of reluctance.
Hopkinson's law is not a correct analogy with Ohm's law in terms of modelling
power and energy flow. In particular, there is no power dissipation associated
with a magnetic reluctance in the same way as there is a dissipation in an
electrical resistance. The magnetic resistance that is a true analogy of
electrical resistance in this respect is defined as the ratio of magnetomotive
force and the rate of change of magnetic flux. Here rate of change of magnetic
flux is standing in for electrical current and the Ohm's law analogy becomes,
           F   =    d &#x03A6;   d t     R   m      {\displaystyle {\mathcal
      {F}}={\frac {d\Phi }{dt}}R_{\mathrm {m} }}  [{\displaystyle {\mathcal
      {F}}={\frac {d\Phi }{dt}}R_{\mathrm {m} }}]
where       R   m       {\displaystyle \scriptstyle R_{\mathrm {m} }}  [
{\displaystyle \scriptstyle R_{\mathrm {m} }}] is the magnetic resistance. This
relationship is part of an electrical-magnetic analogy called the gyrator-
capacitor_model and is intended to overcome the drawbacks of the reluctance
model. The gyrator-capacitor model is, in turn, part of a wider_group_of
compatible_analogies used to model systems across multiple energy domains.
***** Reluctance[edit] *****
Main article: Reluctance
Magnetic reluctance, or magnetic resistance, is analogous to resistance in an
electrical circuit (although it does not dissipate magnetic energy). In
likeness to the way an electric_field causes an electric_current to follow the
path_of_least_resistance, a magnetic_field causes magnetic_flux to follow the
path of least magnetic reluctance. It is a scalar, extensive_quantity, akin to
electrical resistance.
The total reluctance is equal to the ratio of the MMF in a passive magnetic
circuit and the magnetic_flux in this circuit. In an AC field, the reluctance
is the ratio of the amplitude values for a sinusoidal MMF and magnetic flux.
(see phasors)
The definition can be expressed as:
           R   =    F  &#x03A6;     {\displaystyle {\mathcal {R}}={\frac
      {\mathcal {F}}{\Phi }}}  [{\mathcal  {R}}={\frac  {{\mathcal  {F}}}{\Phi
      }}]
where        R      {\displaystyle \scriptstyle {\mathcal {R}}}  [\scriptstyle
{\mathcal  {R}}] is the reluctance in ampere-turns per weber (a unit that is
equivalent to turns per henry).
Magnetic flux always forms a closed loop, as described by Maxwell's_equations,
but the path of the loop depends on the reluctance of the surrounding
materials. It is concentrated around the path of least reluctance. Air and
vacuum have high reluctance, while easily magnetized materials such as soft
iron have low reluctance. The concentration of flux in low-reluctance materials
forms strong temporary poles and causes mechanical forces that tend to move the
materials towards regions of higher flux so it is always an attractive force
(pull).
The inverse of reluctance is called permeance.
           P   =   1  R      {\displaystyle {\mathcal {P}}={\frac {1}{\mathcal
      {R}}}}  [{\mathcal  {P}}={\frac  {1}{{\mathcal  {R}}}}]
Its SI derived unit is the henry (the same as the unit of inductance, although
the two concepts are distinct).
***** Microscopic origins of reluctance[edit] *****
The reluctance of a magnetically uniform magnetic circuit element can be
calculated as:
           R   =   l  &#x03BC; A      {\displaystyle {\mathcal {R}}={\frac {l}
      {\mu A}}}  [{\mathcal  {R}}={\frac  {l}{\mu A}}]
where
      l is the length of the element in metres
          &#x03BC;  =   &#x03BC;  r    &#x03BC;  0      {\displaystyle
      \scriptstyle \mu \;=\;\mu _{r}\mu _{0}}  [\scriptstyle \mu \;=\;\mu _
      {r}\mu _{0}] is the permeability of the material (     &#x03BC;  r
      {\displaystyle \scriptstyle \mu _{r}}  [\scriptstyle \mu _{r}] is the
      relative permeability of the material (dimensionless), and      &#x03BC;
      0      {\displaystyle \scriptstyle \mu _{0}}  [\scriptstyle \mu _{0}] is
      the permeability of free space)
      A is the cross-sectional area of the circuit in square_metres
This is similar to the equation for electrical resistance in materials, with
permeability being analogous to conductivity; the reciprocal of the
permeability is known as magnetic reluctivity and is analogous to resistivity.
Longer, thinner geometries with low permeabilities lead to higher reluctance.
Low reluctance, like low resistance in electric circuits, is generally
preferred.[citation_needed]
***** Summary of analogy between magnetic circuits and electrical circuits
[edit] *****
The following table summarizes the mathematical analogy between electrical
circuit theory and magnetic circuit theory. This is mathematical analogy and
not a physical one. Objects in the same row have the same mathematical role;
the physics of the two theories are very different. For example, current is the
flow of electrical charge, while magnetic flux is not the flow of any quantity.
         Analogy between 'magnetic circuits' and electrical circuits
Magnetic                              Electric
Name          Symbol         Units    Name          Symbol         Units
                   F   =                                 E   =
              &#x222B;  H                           &#x222B;  E
              &#x22C5; d                            &#x22C5; d
              &#x2061;  l                           &#x2061;  l
              {\displaystyle                        {\displaystyle
              {\mathcal                             {\mathcal
              {F}}=\int                             {E}}=\int
              \mathbf {H}                           \mathbf {E}
Magnetomotive \cdot          ampere-  Electromotive \cdot
force (MMF)   \operatorname  turn     force (EMF)   \operatorname  volt
              {d} \mathbf                           {d} \mathbf
              {l} }  [                              {l} }  [
              {\mathcal                             {\mathcal
              {F}}=\int                             {E}}=\int
              {\mathbf                              {\mathbf
              {H}}\cdot                             {E}}\cdot
              \operatorname                         \operatorname
              {d}{\mathbf                           {d}{\mathbf
              {l}}]                                 {l}}]
Magnetic                     ampere/  Electric                     volt/meter
field         H              meter    field         E              = newton/
                                                                   coulomb
                 &#x03A6;
Magnetic_flux {\displaystyle weber    Electric      I              ampere
              \Phi }  [\Phi           current
              ]
                   F   =
              &#x03A6;    R
              m
              {\displaystyle                             E   = I R
              {\mathcal                             {\displaystyle
Hopkinson's   {F}}=\Phi      ampere-                {\mathcal
law or        {\mathcal      turn     Ohm's_law     {E}}=IR}  [
Rowland's law {R}}_{m}}  [                          {\mathcal
              {\displaystyle                        {E}}=IR]
              {\mathcal
              {F}}=\Phi
              {\mathcal
              {R}}_{m}}]
                    R    m
              {\displaystyle
Reluctance    {\mathcal      1/henry  Electrical    R              ohm
              {R}}_{m}}  [            resistance
              {\mathcal
              {R}}_{m}]
                   P   =   1
              R    m
              {\displaystyle
              {\mathcal
              {P}}={\frac             Electric                     1/ohm = mho
Permeance     {1}{{\mathcal  henry    conductance   G = 1/R        = siemens
              {R}}_{m}}}}  [
              {\mathcal
              {P}}={\frac
              {1}{{\mathcal
              {R}}_{m}}}]
                  B  =                                  J  =
              &#x03BC;  H                           &#x03C3;  E
              {\displaystyle                        {\displaystyle
Relation      \mathbf {B}                           \mathbf {J}
between B and =\mu \mathbf            Microscopic   =\sigma
H             {H} }  [                Ohm's law     \mathbf {E} }
              {\mathbf                              [\mathbf {J}
              {B}}=\mu                              =\sigma
              {\mathbf                              \mathbf {E} ]
              {H}}]
Magnetic_flux                         Current                      ampere/
density B     B              tesla    density       J              square
                                                                   meter
Permeability  Î¼           henry/   Electrical    Ï           siemens/
                             meter    conductivity                 meter
***** Limitations of the analogy[edit] *****
When using the analogy between magnetic circuits and electric circuits, the
limitations of this analogy must be kept in mind. Electric and magnetic
circuits are only superficially similar because of the similarity between
Hopkinson's law and Ohm's law. Magnetic circuits have significant differences,
which must be taken into account in their construction:
    * Electric currents represent the flow of particles (electrons) and carry
      power, part or all of which is dissipated as heat in resistances.
      Magnetic fields don't represent a "flow" of anything, and no power is
      dissipated in reluctances.
    * The current in typical electric circuits is confined to the circuit, with
      very little "leakage". In typical magnetic circuits not all of the
      magnetic field is confined to the magnetic circuit because magnetic
      permeability also exists outside materials (see vacuum_permeability).
      Thus, there may be significant "leakage_flux" in the space outside the
      magnetic cores, which must be taken into account but often difficult to
      calculate.
    * Most importantly, magnetic circuits are nonlinear; the reluctance in a
      magnetic circuit is not constant, as resistance is, but varies depending
      on the magnetic field. At high magnetic fluxes the ferromagnetic
      materials used for the cores of magnetic circuits saturate, limiting
      further increase of the magnetic flux through, so above this level the
      reluctance increases rapidly. In addition, ferromagnetic materials suffer
      from hysteresis so the flux in them depends not just on the instantaneous
      MMF but also on the history of MMF. After the source of the magnetic flux
      is turned off, remanent_magnetism is left in ferromagnetic materials,
      creating flux with no MMF.
***** Circuit laws[edit] *****
Magnetic circuit
Magnetic circuits obey other laws that are similar to electrical circuit laws.
For example, the total reluctance         R    T      {\displaystyle
\scriptstyle {\mathcal {R}}_{T}}  [\scriptstyle {\mathcal  {R}}_{T}] of
reluctances         R    1   , &#xA0;    R    2   , &#xA0; &#x2026;
{\displaystyle \scriptstyle {\mathcal {R}}_{1},\ {\mathcal {R}}_{2},\ \dots }
[\scriptstyle {\mathcal  {R}}_{1},\ {\mathcal  {R}}_{2},\ \dots ] in series is:
            R    T   =    R    1   +    R    2   + &#x22EF;   {\displaystyle
      {\mathcal {R}}_{T}={\mathcal {R}}_{1}+{\mathcal {R}}_{2}+\cdots }  [
      {\mathcal  {R}}_{T}={\mathcal  {R}}_{1}+{\mathcal  {R}}_{2}+\cdots ]
This also follows from AmpÃ¨re's_law and is analogous to Kirchhoff's_voltage
law for adding resistances in series. Also, the sum of magnetic fluxes
&#x03A6;  1   , &#xA0;  &#x03A6;  2   , &#xA0; &#x2026;    {\displaystyle
\scriptstyle \Phi _{1},\ \Phi _{2},\ \dots }  [\scriptstyle \Phi _{1},\ \Phi _
{2},\ \dots ] into any node is always zero:
          &#x03A6;  1   +  &#x03A6;  2   + &#x22EF; = 0   {\displaystyle \Phi _
      {1}+\Phi _{2}+\cdots =0}  [\Phi _{1}+\Phi _{2}+\cdots =0]
This follows from Gauss's_law and is analogous to Kirchhoff's_current_law for
analyzing electrical circuits.
Together, the three laws above form a complete system for analysing magnetic
circuits, in a manner similar to electric circuits. Comparing the two types of
circuits shows that:
    * The equivalent to resistance R is the reluctance         R    m
      {\displaystyle \scriptstyle {\mathcal {R}}_{m}}  [\scriptstyle {\mathcal
      {R}}_{m}]
    * The equivalent to current I is the magnetic flux Î¦
    * The equivalent to voltage V is the magnetomotive Force F
Magnetic circuits can be solved for the flux in each branch by application of
the magnetic equivalent of Kirchhoff's_Voltage_Law (KVL) for pure source/
resistance circuits. Specifically, whereas KVL states that the voltage
excitation applied to a loop is equal to the sum of the voltage drops
(resistance times current) around the loop, the magnetic analogue states that
the magnetomotive force (achieved from ampere-turn excitation) is equal to the
sum of MMF drops (product of flux and reluctance) across the rest of the loop.
(If there are multiple loops, the current in each branch can be solved through
a matrix equationâmuch as a matrix solution for mesh circuit branch currents
is obtained in loop analysisâafter which the individual branch currents are
obtained by adding and/or subtracting the constituent loop_currents as
indicated by the adopted sign convention and loop orientations.) Per AmpÃ¨re's
law, the excitation is the product of the current and the number of complete
loops made and is measured in ampere-turns. Stated more generally:
   F = N  I =    &#x222E;      &#x2061;    H &#x2192;    &#x22C5; d &#x2061;
l &#x2192;      {\displaystyle F=N\,I=\oint {\vec {H}}\cdot \operatorname {d}
{\vec {l}}}  [F=N\,I=\oint {\vec  {H}}\cdot \operatorname {d}{\vec  {l}}]
(Note that, per Stokes's theorem, the closed line_integral of HÂ·dl around a
contour is equal to the open surface_integral of curl HÂ·dA across the surface
bounded by the closed contour. Since, from Maxwell's_equations, curl H = J, the
closed line integral of HÂ·dl evaluates to the total current passing through
the surface. This is equal to the excitation, NI, which also measures current
passing through the surface, thereby verifying that the net current flow
through a surface is zero ampere-turns in a closed system that conserves
energy.)
More complex magnetic systems, where the flux is not confined to a simple loop,
must be analysed from first principles by using Maxwell's_equations.
***** Applications[edit] *****
    * Air gaps can be created in the cores of certain transformers to reduce
      the effects of saturation. This increases the reluctance of the magnetic
      circuit, and enables it to store more energy before core saturation. This
      effect is used in the flyback_transformers of cathode-ray tube video
      displays and in some types of switch-mode_power_supply.
    * Variation of reluctance is the principle behind the reluctance_motor (or
      the variable reluctance generator) and the Alexanderson_alternator.
    * Multimedia loudspeakers are typically shielded magnetically, in order to
      reduce magnetic interference caused to televisions and other CRTs. The
      speaker magnet is covered with a material such as soft_iron to minimize
      the stray magnetic field.
Reluctance can also be applied to variable reluctance (magnetic) pickups.
***** See also[edit] *****
    * Magnetic_capacitivity
    * Magnetic_capacitance
    * Magnetic_complex_reluctance
    * Tokamak
***** References[edit] *****
   1. ^ International_Electrotechnical_Commission
   2. ^ Matthew M. Radmanesh, The Gateway to Understanding: Electrons to Waves
      and Beyond, p._539, AuthorHouse, 2005
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
   4. ISBN 1418487406.
   5. ^ Rowland H., Phil. Mag. (4), vol. 46, 1873, p. 140.
   6. ^ Magnetism_(flash)
   7. ^Tesche, Fredrick; Michel Ianoz; TorbjÃ¶rn Karlsson (1997). EMC Analysis
      Methods and Computational Models. Wiley-IEEE. p. 513. ISBN 0-471-15573-X.
***** External links[edit] *****
    * Magnetic-Electric_Analogs by Dennis L. Feucht, Innovatia Laboratories
      (PDF) Archived July 17, 2012, at the Wayback_Machine
    * Interactive_Java_Tutorial_on_Magnetic_Shunts National High Magnetic Field
      Laboratory

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Magnetic_circuit&oldid=870765381"
Categories:
    * Electromagnetism
    * Electric_and_magnetic_fields_in_matter
    * Magnetic_circuits
    * Electrical_analogies
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_August_2009
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * Norsk
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * Ø§Ø±Ø¯Ù
    * ä¸­æ
Edit_links
    * This page was last edited on 26 November 2018, at 21:37 (UTC).
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