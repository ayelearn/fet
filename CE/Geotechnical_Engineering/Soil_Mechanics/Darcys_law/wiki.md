The following text has been accessed from https://en.wikipedia.org/wiki/Darcy%27s_law at Thu Aug 8 23:43:58 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Darcy's law ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Darcy's law is an equation that describes the flow of a fluid through a porous
medium. The law was formulated by Henry_Darcy based on results of experiments
[1] on the flow of water through beds of sand, forming the basis of
hydrogeology, a branch of earth_sciences.
⁰
***** Contents *****
    * 1_Background
    * 2_Description
    * 3_Derivation
    * 4_Additional_forms_of_Darcy's_law
          o 4.1_Darcy's_law_in_petroleum_engineering
          o 4.2_DarcyâForchheimer_law
          o 4.3_Darcy's_law_for_gases_in_fine_media_(Knudsen_diffusion_or
            Klinkenberg_effect)
          o 4.4_Darcy's_law_for_short_time_scales
          o 4.5_Brinkman_form_of_Darcy's_law
    * 5_Validity_of_Darcy's_law
    * 6_See_also
    * 7_References
***** Background[edit] *****
Darcy's law was determined experimentally by Darcy. It has since been derived
from the NavierâStokes_equations via homogenization.[2] It is analogous to
Fourier's_law in the field of heat_conduction, Ohm's_law in the field of
electrical_networks, or Fick's_law in diffusion theory.
One application of Darcy's law is to analyze water flow through an aquifer;
Darcy's law along with the equation of conservation_of_mass are equivalent to
the groundwater_flow_equation, one of the basic relationships of hydrogeology.
Morris_Muskat first[citation_needed] refined Darcy's equation for single phase
flow by including viscosity in the single (fluid) phase equation of Darcy, and
this change made it suitable for the petroleum industry. Based on experimental
results worked out by his colleagues Wyckoff and Botset, Muskat and Meres also
generalized Darcy's law to cover multiphase flow of water, oil and gas in the
porous medium of a petroleum reservoir. The generalized multiphase flow
equations by Muskat and others provide the analytical foundation for reservoir
engineering that exists to this day.
***** Description[edit] *****
Diagram showing definitions and directions for Darcy's law.
Darcy's law, as refined by Morris_Muskat, in the absence of gravitational
forces, is a simple proportional relationship between the instantaneous flow
rate through a porous medium of permeability     k   {\displaystyle k}  [k],
the dynamic viscosity of the fluid and the pressure drop over a given distance
in a homogeneously permeable medium.[3]
         Q = &#x2212;    k A  (   p   b    &#x2212;  p   a     )    &#x03BC; L
      .   {\displaystyle Q=-{\frac {kA\left(p_{\mathrm {b} }-p_{\mathrm {a}
      }\right)}{\mu L}}\,.}  [{\displaystyle Q=-{\frac {kA\left(p_{\mathrm {b}
      }-p_{\mathrm {a} }\right)}{\mu L}}\,.}]
This equation, for single phase (fluid) flow, is the defining_equation [4] for
absolute permeability (single phase permeability). The total discharge, Q
(units of volume per time, e.g., m3/s) is equal to the product of the intrinsic
permeability of the medium, k (m2), the cross-sectional area to flow, A (units
of area, e.g., m2), and the total pressure drop pb â pa (pascals), all
divided by the dynamic viscosity, Î¼ (PaÂ·s) and the length over which the
pressure drop is taking place L (m).
The negative sign is needed because fluid flows from high pressure to low
pressure. Note that the elevation_head must be taken into account if the inlet
and outlet are at different elevations. If the change in pressure is negative
(where pa > pb), then the flow will be in the positive x direction. There have
been several proposals for a constitutive_equation for absolute permeability,
and the most famous one is probably the Kozeny_equation (also called
KozenyâCarman_equation).
Dividing both sides of the equation by the area and using more general notation
leads to
         q = &#x2212;   k &#x03BC;   &#x2207; p  ,   {\displaystyle q=-{\frac
      {k}{\mu }}\nabla p\,,}  [{\displaystyle q=-{\frac {k}{\mu }}\nabla p\,,}]
where q is the flux (discharge per unit area, with units of length per time, m/
s) and âp is the pressure_gradient vector (Pa/m). This value of flux, often
referred to as the Darcy flux or Darcy velocity, is not the velocity which the
fluid traveling through the pores is experiencing. The fluid velocity (v) is
related to the Darcy flux (q) by the porosity (Ï). The flux is divided by
porosity to account for the fact that only a fraction of the total formation
volume is available for flow. The fluid velocity would be the velocity a
conservative tracer would experience if carried by the fluid through the
formation.
         v =   q &#x03C6;    .   {\displaystyle v={\frac {q}{\varphi }}\,.}  [
      {\displaystyle v={\frac {q}{\varphi }}\,.}]
Darcy's law is a simple mathematical statement which neatly summarizes several
familiar properties that groundwater flowing in aquifers exhibits, including:
    * if there is no pressure gradient over a distance, no flow occurs (these
      are hydrostatic conditions),
    * if there is a pressure gradient, flow will occur from high pressure
      towards low pressure (opposite the direction of increasing gradient â
      hence the negative sign in Darcy's law),
    * the greater the pressure gradient (through the same formation material),
      the greater the discharge rate, and
    * the discharge rate of fluid will often be different â through different
      formation materials (or even through the same material, in a different
      direction) â even if the same pressure gradient exists in both cases.
A graphical illustration of the use of the steady-state groundwater_flow
equation (based on Darcy's law and the conservation of mass) is in the
construction of flownets, to quantify the amount of groundwater flowing under a
dam.
Darcy's law is only valid for slow, viscous flow; however, most groundwater
flow cases fall in this category. Typically any flow with a Reynolds_number
less than one is clearly laminar, and it would be valid to apply Darcy's law.
Experimental tests have shown that flow regimes with Reynolds numbers up to 10
may still be Darcian, as in the case of groundwater flow. The Reynolds number
(a dimensionless parameter) for porous media flow is typically expressed as
          R e  =    &#x03C1; v  d  30    &#x03BC;    ,   {\displaystyle \mathrm
      {Re} ={\frac {\rho vd_{30}}{\mu }}\,,}  [{\displaystyle \mathrm {Re} =
      {\frac {\rho vd_{30}}{\mu }}\,,}]
where Ï is the density of water (units of mass per volume), v is the specific
discharge (not the pore velocity â with units of length per time), d30 is a
representative grain diameter for the porous media (often taken as the 30%
passing size from a grain_size analysis using sieves â with units of length),
and Î¼ is the dynamic viscosity of the fluid.
***** Derivation[edit] *****
For stationary, creeping, incompressible flow, i.e. D(Ïui)/Dt â 0, the
NavierâStokes equation simplifies to the Stokes_equation:
         &#x03BC;  &#x2207;  2    u  i   + &#x03C1;  g  i   &#x2212;  &#x2202;
      i   p = 0  ,   {\displaystyle \mu \nabla ^{2}u_{i}+\rho g_{i}-\partial _
      {i}p=0\,,}  [{\displaystyle \mu \nabla ^{2}u_{i}+\rho g_{i}-\partial _
      {i}p=0\,,}]
where Î¼ is the viscosity, ui is the velocity in the i direction, gi is the
gravity component in the i direction and p is the pressure. Assuming the
viscous resisting force is linear with the velocity we may write:
         &#x2212;   (  k  i j   )   &#x2212; 1   &#x03BC; &#x03C6;  u  j   +
      &#x03C1;  g  i   &#x2212;  &#x2202;  i   p = 0  ,   {\displaystyle -\left
      (k_{ij}\right)^{-1}\mu \varphi u_{j}+\rho g_{i}-\partial _{i}p=0\,,}  [
      {\displaystyle -\left(k_{ij}\right)^{-1}\mu \varphi u_{j}+\rho g_{i}-
      \partial _{i}p=0\,,}]
where Ï is the porosity, and kij is the second order permeability tensor. This
gives the velocity in the n direction,
          k  n i     (  k  i j   )   &#x2212; 1    u  j   =  &#x03B4;  n j    u
      j   =  u  n   = &#x2212;    k  n i    &#x03C6; &#x03BC;     (   &#x2202;
      i   p &#x2212; &#x03C1;  g  i    )   ,   {\displaystyle k_{ni}\left(k_
      {ij}\right)^{-1}u_{j}=\delta _{nj}u_{j}=u_{n}=-{\frac {k_{ni}}{\varphi
      \mu }}\left(\partial _{i}p-\rho g_{i}\right)\,,}  [{\displaystyle k_
      {ni}\left(k_{ij}\right)^{-1}u_{j}=\delta _{nj}u_{j}=u_{n}=-{\frac {k_
      {ni}}{\varphi \mu }}\left(\partial _{i}p-\rho g_{i}\right)\,,}]
which gives Darcy's law for the volumetric flux density in the n direction,
          q  n   = &#x2212;    k  n i   &#x03BC;    (   &#x2202;  i   p
      &#x2212; &#x03C1;  g  i    )   .   {\displaystyle q_{n}=-{\frac {k_{ni}}
      {\mu }}\left(\partial _{i}p-\rho g_{i}\right)\,.}  [{\displaystyle q_
      {n}=-{\frac {k_{ni}}{\mu }}\left(\partial _{i}p-\rho g_{i}\right)\,.}]
In isotropic porous_media the off-diagonal elements in the permeability tensor
are zero, kij = 0 for i â  j and the diagonal elements are identical, kii = k,
and the common form is obtained
          q  = &#x2212;   k &#x03BC;    (   &#x2207;  p &#x2212; &#x03C1;  g
      )   .   {\displaystyle {\boldsymbol {q}}=-{\frac {k}{\mu }}\left(
      {\boldsymbol {\nabla }}p-\rho {\boldsymbol {g}}\right)\,.}  [
      {\displaystyle {\boldsymbol {q}}=-{\frac {k}{\mu }}\left({\boldsymbol
      {\nabla }}p-\rho {\boldsymbol {g}}\right)\,.}]
The above equation is a governing_equation for single phase fluid flow in a
porous medium.
***** Additional forms of Darcy's law[edit] *****
**** Darcy's law in petroleum engineering[edit] ****
Another derivation of Darcy's law is used extensively in petroleum_engineering
to determine the flow through permeable media â the most simple of which is
for a one-dimensional, homogeneous rock formation with a single fluid phase and
constant fluid viscosity.
         Q =    k A  &#x03BC;    (    &#x2202; p   &#x2202; x    )   ,
      {\displaystyle Q={\frac {kA}{\mu }}\left({\frac {\partial p}{\partial
      x}}\right)\,,}  [{\displaystyle Q={\frac {kA}{\mu }}\left({\frac
      {\partial p}{\partial x}}\right)\,,}]
where Q is the flowrate of the formation (in units of volume per unit time), k
is the permeability of the formation (typically in millidarcys), A is the
cross-sectional area of the formation, Î¼ is the viscosity of the fluid
(typically in units of centipoise). âp/âx represents the pressure change
per unit length of the formation. This equation can also be solved for
permeability and is used to measure it, forcing a fluid of known viscosity
through a core of a known length and area, and measuring the pressure drop
across the length of the core.
Almost all oil reservoirs have a water zone below the oil leg, and some have
also a gas cap above the oil leg. When the reservoir pressure drops due to oil
production, water flows into the oil zone from below, and gas flows into the
oil zone from above (if the gas cap exists), and we get a simultaneous flow and
immiscible mixing of all fluid phases in the oil zone. The operator of the oil
field may also inject water (and/or gas) in order to improve oil production.
The petroleum industry is therefore using a generalized Darcy equation for
multiphase flow that was developed by Muskat et alios. Because Darcy's name is
so widespread and strongly associated with flow in porous media, the multiphase
equation is denoted Darcy's_law_for_multiphase_flow or generalized Darcy
equation (or law) or simply Darcy's equation (or law) or simply flow equation
if the context says that the text is discussing the multiphase equation of
Muskat et alios. Multiphase flow in oil and gas reservoirs is a comprehensive
topic, and one of many articles about this topic is Darcy's_law_for_multiphase
flow.
**** DarcyâForchheimer law[edit] ****
For flows in porous media with Reynolds_numbers greater than about 1 to 10,
inertial effects can also become significant. Sometimes an inertial term is
added to the Darcy's equation, known as Forchheimer term. This term is able to
account for the non-linear behavior of the pressure difference vs flow data.[5]
            &#x2202; p   &#x2202; x    = &#x2212;   &#x03BC; k   q &#x2212;
      &#x03C1;  k  1      q  2    ,   {\displaystyle {\frac {\partial p}
      {\partial x}}=-{\frac {\mu }{k}}q-{\frac {\rho }{k_{1}}}q^{2}\,,}  [
      {\displaystyle {\frac {\partial p}{\partial x}}=-{\frac {\mu }{k}}q-
      {\frac {\rho }{k_{1}}}q^{2}\,,}]
where the additional term k1 is known as inertial permeability.
The flow in the middle of a sandstone reservoir is so slow that Forchheimer's
equation is usually not needed, but the gas flow into a gas production well may
be high enough to justify use of Forchheimer's equation. In this case the
inflow performance calculations for the well, not the grid cell of the 3D
model, is based on the Forchheimer equation. The effect of this is that an
additional rate-dependent skin appears in the inflow performance formula.
Some carbonate reservoirs have lots of fractures, and Darcy's equation for
multiphase flow is generalized in order to govern both flow in fractures and
flow in the matrix (i.e. the traditional porous rock). The irregular surface of
the fracture walls and high flow rate in the fractures, may justify use of
Forchheimer's equation.
**** Darcy's law for gases in fine media (Knudsen diffusion or Klinkenberg
effect)[edit] ****
For gas flow in small characteristic dimensions (e.g., very fine sand,
nanoporous structures etc.), the particle-wall interactions become more
frequent, giving rise to additional wall friction (Knudsen friction). For a
flow in this region, where both viscous and Knudsen friction are present, a new
formulation needs to be used. Knudsen presented a semi-empirical model for flow
in transition regime based on his experiments on small capillaries.[6][7] For a
porous medium, the Knudsen equation can be given as [7]
         N = &#x2212;  (    k &#x03BC;       p  a   +  p  b    2   +  D   K
      e f f     )    1   R   g    T        p   b    &#x2212;  p   a     L    ,
      {\displaystyle N=-\left({\frac {k}{\mu }}{\frac {p_{a}+p_{b}}{2}}+D_
      {\mathrm {K} }^{\mathrm {eff} }\right){\frac {1}{R_{\mathrm {g} }T}}
      {\frac {p_{\mathrm {b} }-p_{\mathrm {a} }}{L}}\,,}  [{\displaystyle N=-
      \left({\frac {k}{\mu }}{\frac {p_{a}+p_{b}}{2}}+D_{\mathrm {K} }^{\mathrm
      {eff} }\right){\frac {1}{R_{\mathrm {g} }T}}{\frac {p_{\mathrm {b} }-p_
      {\mathrm {a} }}{L}}\,,}]
where N is the molar flux, Rg is the gas constant, T is the temperature, Deff
K is the effective Knudsen diffusivity of the porous media. The model can also
be derived from the first-principle-based binary friction model (BFM).[8][9]
The differential equation of transition flow in porous media based on BFM is
given as[8]
            &#x2202; p   &#x2202; x    = &#x2212;  R   g    T   (     k p
      &#x03BC;   +  D   K     )   &#x2212; 1   N  .   {\displaystyle {\frac
      {\partial p}{\partial x}}=-R_{\mathrm {g} }T\left({\frac {kp}{\mu }}+D_
      {\mathrm {K} }\right)^{-1}N\,.}  [{\displaystyle {\frac {\partial p}
      {\partial x}}=-R_{\mathrm {g} }T\left({\frac {kp}{\mu }}+D_{\mathrm {K}
      }\right)^{-1}N\,.}]
This equation is valid for capillaries as well as porous media. The terminology
of the Knudsen effect and Knudsen diffusivity is more common in mechanical and
chemical_engineering. In geological and petrochemical engineering, this effect
is known as the Klinkenberg_effect. Using the definition of molar flux, the
above equation can be rewritten as
            &#x2202; p   &#x2202; x    = &#x2212;  R   g    T   (     k p
      &#x03BC;   +  D   K     )   &#x2212; 1      p   R   g    T     q  .
      {\displaystyle {\frac {\partial p}{\partial x}}=-R_{\mathrm {g} }T\left(
      {\frac {kp}{\mu }}+D_{\mathrm {K} }\right)^{-1}{\dfrac {p}{R_{\mathrm {g}
      }T}}q\,.}  [{\displaystyle {\frac {\partial p}{\partial x}}=-R_{\mathrm
      {g} }T\left({\frac {kp}{\mu }}+D_{\mathrm {K} }\right)^{-1}{\dfrac {p}{R_
      {\mathrm {g} }T}}q\,.}]
This equation can be rearranged into the following equation
         q = &#x2212;   k &#x03BC;    (  1 +     D   K    &#x03BC;  k     1 p
      )     &#x2202; p   &#x2202; x     .   {\displaystyle q=-{\frac {k}{\mu
      }}\left(1+{\frac {D_{\mathrm {K} }\mu }{k}}{\frac {1}{p}}\right){\frac
      {\partial p}{\partial x}}\,.}  [{\displaystyle q=-{\frac {k}{\mu }}\left
      (1+{\frac {D_{\mathrm {K} }\mu }{k}}{\frac {1}{p}}\right){\frac {\partial
      p}{\partial x}}\,.}]
Comparing this equation with conventional Darcy's law, a new formulation can be
given as
         q = &#x2212;    k   e f f    &#x03BC;      &#x2202; p   &#x2202; x
      ,   {\displaystyle q=-{\frac {k^{\mathrm {eff} }}{\mu }}{\frac {\partial
      p}{\partial x}}\,,}  [{\displaystyle q=-{\frac {k^{\mathrm {eff} }}{\mu
      }}{\frac {\partial p}{\partial x}}\,,}]
where
          k   e f f    = k  (  1 +     D   K    &#x03BC;  k     1 p    )   .
      {\displaystyle k^{\mathrm {eff} }=k\left(1+{\frac {D_{\mathrm {K} }\mu }
      {k}}{\frac {1}{p}}\right)\,.}  [{\displaystyle k^{\mathrm {eff} }=k\left
      (1+{\frac {D_{\mathrm {K} }\mu }{k}}{\frac {1}{p}}\right)\,.}]
This is equivalent to the effective permeability formulation proposed by
Klinkenberg:[10]
          k   e f f    = k  (  1 +   b p    )   .   {\displaystyle k^{\mathrm
      {eff} }=k\left(1+{\frac {b}{p}}\right)\,.}  [{\displaystyle k^{\mathrm
      {eff} }=k\left(1+{\frac {b}{p}}\right)\,.}]
where b is known as the Klinkenberg parameter, which depends on the gas and the
porous medium structure. This is quite evident if we compare the above
formulations. The Klinkenberg parameter b is dependent on permeability, Knudsen
diffusivity and viscosity (i.e., both gas and porous medium properties).
**** Darcy's law for short time scales[edit] ****
For very short time scales, a time derivative of flux may be added to Darcy's
law, which results in valid solutions at very small times (in heat transfer,
this is called the modified form of Fourier's_law),
         &#x03C4;    &#x2202; q   &#x2202; t    + q = &#x2212; k &#x2207; h  ,
      {\displaystyle \tau {\frac {\partial q}{\partial t}}+q=-k\nabla h\,,}  [
      {\displaystyle \tau {\frac {\partial q}{\partial t}}+q=-k\nabla h\,,}]
where Ï is a very small time constant which causes this equation to reduce to
the normal form of Darcy's law at "normal" times (> nanoseconds). The main
reason for doing this is that the regular groundwater_flow_equation (diffusion
equation) leads to singularities at constant head boundaries at very small
times. This form is more mathematically rigorous, but leads to a hyperbolic
groundwater flow equation, which is more difficult to solve and is only useful
at very small times, typically out of the realm of practical use.
**** Brinkman form of Darcy's law[edit] ****
Another extension to the traditional form of Darcy's law is the Brinkman term,
which is used to account for transitional flow between boundaries (introduced
by Brinkman in 1949[11]),
         &#x2212; &#x03B2;  &#x2207;  2   q + q = &#x2212;   k &#x03BC;
      &#x2207; p  ,   {\displaystyle -\beta \nabla ^{2}q+q=-{\frac {k}{\mu
      }}\nabla p\,,}  [{\displaystyle -\beta \nabla ^{2}q+q=-{\frac {k}{\mu
      }}\nabla p\,,}]
where Î² is an effective viscosity term. This correction term accounts for flow
through medium where the grains of the media are porous themselves, but is
difficult to use, and is typically neglected. For example, if a porous
extracellular_matrix degrades to form large pores throughout the matrix, the
viscous term applies in the large pores, while Darcy's law applies in the
remaining intact region. This scenario was considered in a theoretical and
modelling study.[12] In the proposed model, the Brinkman equation is connected
to a set of reaction-diffusion-convection_equations.
***** Validity of Darcy's law[edit] *****
Darcy's law is valid for laminar_flow through sediments. In fine-grained
sediments, the dimensions of interstices are small and thus flow is laminar.
Coarse-grained sediments also behave similarly but in very coarse-grained
sediments the flow may be turbulent.[13] Hence Darcy's law is not always valid
in such sediments. For flow through commercial circular pipes, the flow is
laminar when Reynolds number is less than 2000 and turbulent when it is more
than 4000, but in some sediments it has been found that flow is laminar when
the value of Reynolds number is less than 1.[14]
***** See also[edit] *****
    * The darcy, a unit of fluid permeability
    * Hydrogeology
    * Groundwater_flow_equation
    * Mathematical_model
***** References[edit] *****
   1. ^Darcy, H. (1856). Les fontaines publiques de la ville de Dijon. Paris:
      Dalmont.
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
   3. ^Whitaker, S. (1986). "Flow in porous media I: A theoretical derivation
      of Darcy's law". Transport in Porous Media. 1: 3â25. doi:10.1007/
      BF01036523.
   4. ^Liu, Mingchao; Wu, Jian; Gan, Yixiang; Hanaor, Dorian A. H; Chen, C. Q
      (2016). "Evaporation_limited_radial_capillary_penetration_in_porous
      media" (PDF). Langmuir. 32 (38): 9899â9904. doi:10.1021/
      acs.langmuir.6b02404. PMID 27583455.
   5. ^Zarandi, M. Amin F.; Pillai, Krishna M.; Kimmel, Adam S. (2018).
      "Spontaneous imbibition of liquids in glass-fiber wicks. Part I:
      Usefulness of a sharp-front approach". AIChE Journal. 64: 294â305. doi:
      10.1002/aic.15965.
   6. ^Bejan, A. (1984). Convection Heat Transfer. John Wiley & Sons.
   7. ^Cunningham, R. E.; Williams, R. J. J. (1980). Diffusion in Gases and
      Porous Media. New York: Plenum Press.
   8. ^ a bCarrigy, N.; Pant, L. M.; Mitra, S. K.; Secanell, M. (2013).
      "Knudsen_diffusivity_and_permeability_of_pemfc_microporous_coated_gas
      diffusion_layers_for_different_polytetrafluoroethylene_loadings". Journal
      of the Electrochemical Society. 160 (2): F81â89. doi:10.1149/
      2.036302jes.
   9. ^ a bPant, L. M.; Mitra, S. K.; Secanell, M. (2012). "Absolute
      permeability and Knudsen diffusivity measurements in PEMFC gas diffusion
      layers and micro porous layers". Journal of Power Sources. 206:
      153â160. doi:10.1016/j.jpowsour.2012.01.099.
  10. ^Kerkhof, P. (1996). "A_modified_MaxwellâStefan_model_for_transport
      through_inert_membranes:_The_binary_friction_model". Chemical Engineering
      Journal and the Biochemical Engineering Journal. 64 (3): 319â343. doi:
      10.1016/S0923-0467(96)03134-X.
  11. ^Klinkenberg, L. J. (1941). "The permeability of porous media to liquids
      and gases". Drilling and Production Practice. American Petroleum
      Institute. pp. 200â213.
  12. ^Brinkman, H. C. (1949). "A calculation of the viscous force exerted by a
      flowing fluid on a dense swarm of particles". Applied Scientific
      Research. 1: 27â34. CiteSeerX 10.1.1.454.3769. doi:10.1007/BF02120313.
  13. ^Wertheim, Kenneth Y.; Roose, Tiina (April 2017). "A_Mathematical_Model
      of_Lymphangiogenesis_in_a_Zebrafish_Embryo". Bulletin of Mathematical
      Biology. 79 (4): 693â737. doi:10.1007/s11538-017-0248-7. ISSN 1522-
      9602. PMC 5501200. PMID 28233173.
  14. ^Jin, Y.; Uth, M.-F.; Kuznetsov, A. V.; Herwig, H. (2 February 2015).
      "Numerical investigation of the possibility of macroscopic turbulence in
      porous media: a direct numerical simulation study". Journal of Fluid
      Mechanics. 766: 76â103. Bibcode:2015JFM...766...76J. doi:10.1017/
      jfm.2015.9.
  15. ^Arora, K. R. (1989). Soil Mechanics and Foundation Engineering. Standard
      Publishers.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Darcy%27s_law&oldid=901226274"
Categories:
    * Water
    * Civil_engineering
    * Soil_mechanics
    * Soil_physics
    * Hydrology
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_October_2018
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LietuviÅ³
    * Magyar
    * Bahasa_Melayu
    * Nederlands
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Svenska
    * à°¤à±à°²à±à°à±
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 10 June 2019, at 13:47 (UTC).
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
