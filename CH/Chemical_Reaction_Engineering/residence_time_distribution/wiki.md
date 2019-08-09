The following text has been accessed from https://en.wikipedia.org/wiki/Residence_time at Fri Aug 9 01:20:12 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Residence time ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other uses, see Residence_time_(disambiguation).
 It has been suggested that Space_time_(chemical_engineering) be merged into
 this article. (Discuss)Proposed since May 2018.
For material flowing through a volume, the residence time is a measure of how
much time the matter spends in it. Examples include fluids in a chemical
reactor, specific elements in a geochemical reservoir, water in a catchment,
bacteria in a culture vessel and drugs in human body. A molecule or small
parcel of fluid has a single residence time, but more complex systems have a
residence time distribution (RTD).
There are at least three time constants that are used to represent a residence
time distribution. The turn-over time or flushing time is the ratio of the
material in the volume to the rate at which it passes through; the mean age is
the mean length of time the material in the reservoir has spent there; and the
mean transit time is the mean length of time the material spends in the
reservoir.
Applications of residence times or residence time distributions can be found in
a wide variety of disciplines including environmental_science, engineering,
chemistry, and hydrology.
⁰
***** Contents *****
    * 1_History
    * 2_Distributions
    * 3_Time_constants
          o 3.1_Mean_residence_time
          o 3.2_Mean_transit_time
          o 3.3_Flushing_time
          o 3.4_Relationship_between_times
    * 4_Simple_flow_models
          o 4.1_Plug_flow_reactor
          o 4.2_Continuous_stirred-tank_reactor
          o 4.3_Laminar_flow_reactor
    * 5_Determining_the_RTD_experimentally
          o 5.1_Pulse_experiments
          o 5.2_Step_experiments
    * 6_Applications
          o 6.1_Chemical_reactors
          o 6.2_Groundwater_flow
          o 6.3_Water_treatment
          o 6.4_Surface_science
          o 6.5_Environmental
          o 6.6_Pharmacology
          o 6.7_Queuing_theory
          o 6.8_Biochemical
    * 7_See_also
    * 8_References
    * 9_Further_reading
    * 10_External_links
***** History[edit] *****
The concept of residence time originated in models of chemical reactors. The
first such model was an axial dispersion model by Irving_Langmuir in 1908. This
received little attention for 45 years; other models were developed such as the
plug_flow_reactor_model and the continuous_stirred-tank_reactor, and the
concept of a washout function (representing the response to a sudden change in
the input) was introduced. Then, in 1953, Peter_Danckwerts resurrected the
axial dispersion model and formulated the modern concept of residence time.[1]
***** Distributions[edit] *****
Basic residence time theory treats a system with an input and an output, both
of which have flow only in one direction. The system is homogeneous and the
substance that is flowing through is conserved (neither created nor destroyed).
A small particle entering the system will eventually leave, and the time spent
there is its residence time. In a particularly simple model of flow, plug_flow,
particles that enter at the same time continue to move at the same rate and
leave together. In this case, there is only one residence time. Generally,
though, their rates vary and there is a distribution of exit times. One measure
of this is the washout function     W ( t )   {\displaystyle W(t)}  [W(t)], the
fraction of particles leaving the system after having been there for a time
t   {\displaystyle t}  [t] or greater. Its complement,     F ( t ) = 1 &#x2212;
W ( t )   {\displaystyle F(t)=1-W(t)}  [{\displaystyle F(t)=1-W(t)}], is the
cumulative distribution function. The differential distribution, also known as
the residence time distribution or exit age distribution,[2]:260â261 is given
by
         E ( t ) = d F ( t )  /  d t .   {\displaystyle E(t)=dF(t)/dt.}  [
      {\displaystyle E(t)=dF(t)/dt.}]
This has the properties of a probability_distribution: it is always nonnegative
and
          &#x222B;  0   &#x221E;   E ( t ) d t = 1.   {\displaystyle \int _{0}^
      {\infty }E(t)dt=1.}  [{\displaystyle \int _{0}^{\infty }E(t)dt=1.}][1]
      [2]:260â261
One can also define a density function based on the flux (mass per unit time)
out of the system. The transit time function is the fraction of particles
leaving the system that have been in it for up to a given time. It is the
integral of a distribution     I ( t )   {\displaystyle I(t)}  [I(t)]. If, in a
steady state, the mass in the system is      M  0     {\displaystyle M_{0}}
[M_{0}] and the outgoing flux is      F  0     {\displaystyle F_{0}}  [F_{0}],
the distributions are related by
          F  0   I ( t ) = &#x2212;  M  0      d E ( t )   d t    .
      {\displaystyle F_{0}I(t)=-M_{0}{\frac {dE(t)}{dt}}.}  [{\displaystyle F_
      {0}I(t)=-M_{0}{\frac {dE(t)}{dt}}.}]
As an illustration, for a human population to be in a steady state, the deaths
per year of people older than     t   {\displaystyle t}  [t] years (the left
hand side of the equation) must be balanced by the number of people per year
reaching age     t   {\displaystyle t}  [t] (the right hand side).[3]
***** Time constants[edit] *****
"Residence time" can be a synonym for more than one constant used to represent
the distribution.[4]
**** Mean residence time[edit] ****
Some statistical properties of the residence time distribution are frequently
used. The mean residence time, or mean age, is given by the first moment of the
residence time distribution:
         &#x03C4; =  &#x222B;  0   &#x221E;   t E ( t ) d t   {\displaystyle
      \tau =\int _{0}^{\infty }tE(t)dt}  [{\displaystyle \tau =\int _{0}^
      {\infty }tE(t)dt}],
and the variance is given by
          &#x03C3;  t   2   =  &#x222B;  0   &#x221E;     (  t &#x2212;
      &#x03C4;  )   2   E ( t ) d t   {\displaystyle \sigma _{t}^{2}=\int _{0}^
      {\infty }\left(t-\tau \right)^{2}E(t)dt}  [{\displaystyle \sigma _{t}^
      {2}=\int _{0}^{\infty }\left(t-\tau \right)^{2}E(t)dt}]
or by the dimensionless form      &#x03C3;  2   =  &#x03C3;  t   2    /
&#x03C4;  2     {\displaystyle \sigma ^{2}=\sigma _{t}^{2}/\tau ^{2}}  [
{\displaystyle \sigma ^{2}=\sigma _{t}^{2}/\tau ^{2}}].[1]
**** Mean transit time[edit] ****
The mean transit time is the first moment of the transit time distribution:
          t   t    =  &#x222B;  0   &#x221E;   t I ( t ) d t .   {\displaystyle
      t_{\mathrm {t} }=\int _{0}^{\infty }tI(t)dt.}  [{\displaystyle t_{\mathrm
      {t} }=\int _{0}^{\infty }tI(t)dt.}]
**** Flushing time[edit] ****
The turnover time, also known as the flushing time,[5] is simply the ratio of
mass to flux:
          t  0   =  M  0    /   F  0   .   {\displaystyle t_{0}=M_{0}/F_{0}.}
      [{\displaystyle t_{0}=M_{0}/F_{0}.}]
When applied to liquids, it is also known as the hydraulic retention time
(HRT), hydraulic residence time or hydraulic detention time.[6]
**** Relationship between times[edit] ****
It can be shown that, in a steady state, the mean transit time and flushing
time are equal (     t  t   =  t  0     {\displaystyle t_{t}=t_{0}}  [
{\displaystyle t_{t}=t_{0}}]).[3]
The relationship between      t  0     {\displaystyle t_{0}}  [t_{0}] or      t
t      {\displaystyle t_{\mathrm {t} }}  [{\displaystyle t_{\mathrm {t} }}] and
&#x03C4;   {\displaystyle \tau }  [\tau ] is determined by the type of
distribution:[3]
    *    &#x03C4; <  t  0     {\displaystyle \tau <t_{0}}  [{\displaystyle \tau
      <t_{0}}]: it takes some time for particles to begin leaving the system.
      Examples include water in a lake with inlet and outlet on opposite sides;
      and a nuclear_bomb_test where radioactive_material is introduced high in
      the stratosphere and filters down to the troposphere.
    *    &#x03C4; =  t  0     {\displaystyle \tau =t_{0}}  [{\displaystyle \tau
      =t_{0}}]: the frequency functions     E ( t )   {\displaystyle E(t)}  [E
      (t)] and     I ( t )   {\displaystyle I(t)}  [I(t)] are exponential, as
      in the CSTR model above. Such a distribution occurs whenever all
      particles have a fixed probability per unit time of leaving the system.
      Examples include radioactive_decay and first_order_chemical_reactions
      (where the reaction rate is proportional to the amount of reactant).
    *    &#x03C4; >  t  0     {\displaystyle \tau >t_{0}}  [{\displaystyle \tau
      >t_{0}}]: most of the particles pass through quickly, but some are held
      up. This can happen when the main source and sink are very close together
      or the same. For example, most water_vapor rising from the ocean surface
      soon returns to the ocean, but water vapor that gets sufficiently far
      away will probably return much later in the form of rain.[3]
***** Simple flow models[edit] *****
**** Plug flow reactor[edit] ****
In an ideal plug_flow_reactor the fluid elements leave in the same order they
arrived, not mixing with those in front and behind. Therefore, fluid entering
at time     t   {\displaystyle t}  [t] will exit at time     t + &#x03C4;
{\displaystyle t+\tau }  [t+\tau ], where     &#x03C4;   {\displaystyle \tau }
[\tau ] is the residence time. The fraction leaving is a step function, going
from 0 to 1 at time     &#x03C4;   {\displaystyle \tau }  [\tau ]. The
distribution function is therefore a Dirac_delta_function at     &#x03C4;
{\displaystyle \tau }  [\tau ].
         E ( t ) = &#x03B4; ( t &#x2212; &#x03C4; )    {\displaystyle E
      (t)=\delta (t-\tau )\,}  [{\displaystyle E(t)=\delta (t-\tau )\,}]
The mean is     &#x03C4;   {\displaystyle \tau }  [\tau ] and the variance is
zero.[1]
The RTD of a real reactor deviates from that of an ideal reactor, depending on
the hydrodynamics within the vessel. A non-zero variance indicates that there
is some dispersion along the path of the fluid, which may be attributed to
turbulence, a non-uniform velocity profile, or diffusion. If the mean of the
E ( t )   {\displaystyle E(t)}  [E(t)] curve arrives earlier than the expected
time     &#x03C4;   {\displaystyle \tau }  [\tau ] it indicates that there is
stagnant_fluid within the vessel. If the RTD curve shows more than one main
peak it may indicate channeling, parallel paths to the exit, or strong internal
circulation.
**** Continuous stirred-tank reactor[edit] ****
In an ideal continuous_stirred-tank_reactor (CSTR), the flow at the inlet is
completely and instantly mixed into the bulk of the reactor. The reactor and
the outlet fluid have identical, homogeneous compositions at all times. The
residence time distribution is exponential:
         E ( t ) =   1 &#x03C4;   exp &#x2061;  (    &#x2212; t  &#x03C4;   )
      .   {\displaystyle E(t)={\frac {1}{\tau }}\exp \left({\frac {-t}{\tau
      }}\right).}  [{\displaystyle E(t)={\frac {1}{\tau }}\exp \left({\frac {-
      t}{\tau }}\right).}]
The mean is     &#x03C4;   {\displaystyle \tau }  [\tau ] and the variance is
1.[1] A notable difference from the plug flow reactor is that material
introduced into the system will never completely leave it.[5]
In reality, it is impossible to obtain such rapid mixing, especially on
industrial scales where reactor vessels may range between 1 and thousands of
cubic meters, and hence the RTD of a real reactor will deviate from the ideal
exponential decay. For example, there will be some finite delay before     E
( t )   {\displaystyle E(t)}  [E(t)] reaches its maximum value and the length
of the delay will reflect the rate of mass transfer within the reactor. Just as
was noted for a plug-flow reactor, an early mean will indicate some stagnant
fluid within the vessel, while the presence of multiple peaks could indicate
channeling, parallel paths to the exit, or strong internal circulation. Short-
circuiting fluid within the reactor would appear in an RTD curve as a small
pulse of concentrated tracer that reaches the outlet shortly after injection.
**** Laminar flow reactor[edit] ****
In a laminar_flow_reactor, the fluid flows through a long tube or parallel
plate reactor and the flow is in layers parallel to the walls of the tube. The
velocity of the flow is a parabolic function of radius. In the absence of
molecular_diffusion, the RTD is[7]
         E ( t ) = 0 ,  t <= &#x03C4;  /  2   {\displaystyle E(t)=0,\quad
      t<=\tau /2}  [{\displaystyle E(t)=0,\quad t<=\tau /2}]
and
         E ( t ) =    &#x03C4;  2    2  t  3       t > &#x03C4;  /  2.
      {\displaystyle E(t)={\frac {\tau ^{2}}{2t^{3}}}\quad t>\tau /2.}  [
      {\displaystyle E(t)={\frac {\tau ^{2}}{2t^{3}}}\quad t>\tau /2.}]
The variance is infinite. In a real system, diffusion will eventually mix the
layers so that the tail of the RTD becomes exponential and the variance finite;
but laminar flow reactors can have variance greater than 1, the maximum for
CTSD reactors.[1]
***** Determining the RTD experimentally[edit] *****
Residence time distributions are measured by introducing a non-reactive tracer
into the system at the inlet. Its input concentration is changed according to a
known function and the output concentration measured. The tracer should not
modify the physical characteristics of the fluid (equal density, equal
viscosity) or the hydrodynamic conditions and it should be easily detectable.
[8] In general, the change in tracer concentration will either be a pulse or a
step. Other functions are possible, but they require more calculations to
deconvolute the RTD curve.
**** Pulse experiments[edit] ****
This method required the introduction of a very small volume of concentrated
tracer at the inlet of the reactor, such that it approaches the Dirac_delta
function.[9][7] Although an infinitely short injection cannot be produced, it
can be made much smaller than the mean residence time of the vessel. If a mass
of tracer,     M   {\displaystyle M}  [M], is introduced into a vessel of
volume     V   {\displaystyle V}  [V] and an expected residence time of
&#x03C4;   {\displaystyle \tau }  [\tau ], the resulting curve of     C ( t )
{\displaystyle C(t)}  [C(t)] can be transformed into a dimensionless residence
time distribution curve by the following relation:
         E ( t ) =    C ( t )    &#x222B;  0   &#x221E;   C ( t ) &#xA0; d t
      {\displaystyle E(t)={\frac {C(t)}{\int _{0}^{\infty }C(t)\ dt}}}  [
      {\displaystyle E(t)={\frac {C(t)}{\int _{0}^{\infty }C(t)\ dt}}}]
**** Step experiments[edit] ****
The concentration of tracer in a step experiment at the reactor inlet changes
abruptly from 0 to      C  0     {\displaystyle C_{0}}  [C_{0}]. The
concentration of tracer at the outlet is measured and normalized to the
concentration      C  0     {\displaystyle C_{0}}  [C_{0}] to obtain the non-
dimensional curve     F ( t )   {\displaystyle F(t)}  [F(t)] which goes from 0
to 1:
         F ( t ) =    C ( t )   C  0       {\displaystyle F(t)={\frac {C(t)}{C_
      {0}}}}  [{\displaystyle F(t)={\frac {C(t)}{C_{0}}}}].
The step- and pulse-responses of a reactor are related by the following:
         F ( t ) =  &#x222B;  0   t   E (  t &#x2032;  )  d  t &#x2032;   E ( t
      ) =    d F ( t )   d t      {\displaystyle F(t)=\int _{0}^{t}E
      (t')\,dt'\qquad E(t)={\frac {dF(t)}{dt}}}  [{\displaystyle F(t)=\int _
      {0}^{t}E(t')\,dt'\qquad E(t)={\frac {dF(t)}{dt}}}]
A step experiment is often easier to perform than a pulse experiment, but it
tends to smooth over some of the details that a pulse response could show. It
is easy to numerically integrate an experimental pulse response to obtain a
very high-quality estimate of the step response, but the reverse is not the
case because any noise in the concentration measurement will be amplified by
numeric differentiation.
***** Applications[edit] *****
**** Chemical reactors[edit] ****
In chemical_reactors, the goal is to make components react with a high yield.
In a homogeneous, first-order_reaction, the probability that an atom or
molecule will react depends only on its residence time:
          P   R    = exp &#x2061;  (  &#x2212; k t  )    {\displaystyle P_
      {\mathrm {R} }=\exp \left(-kt\right)}  [{\displaystyle P_{\mathrm {R}
      }=\exp \left(-kt\right)}]
for a rate_constant     k   {\displaystyle k}  [k]. Given a RTD, the average
probability is equal to the ratio of the concentration     a   {\displaystyle
a}  [a] of the component before and after:[1]
            P   R    &#x00AF;   =  a   o u t     /   a   i n    =  &#x222B;  0
      &#x221E;   exp &#x2061;  (  &#x2212; k t  )  E ( t ) d t .
      {\displaystyle {\overline {P_{\mathrm {R} }}}=a_{\mathrm {out} }/a_
      {\mathrm {in} }=\int _{0}^{\infty }\exp \left(-kt\right)E(t)dt.}  [
      {\displaystyle {\overline {P_{\mathrm {R} }}}=a_{\mathrm {out} }/a_
      {\mathrm {in} }=\int _{0}^{\infty }\exp \left(-kt\right)E(t)dt.}]
If the reaction is more complicated, then the output is not uniquely determined
by the RTD. It also depends on the degree of micromixing, the mixing between
molecules that entered at different times. If there is no mixing, the system is
said to be completely segregated, and the output can be given in the form
          a   o u t    =  &#x222B;  0   &#x221E;    a   b a t c h    ( t ) E
      ( t ) d t .   {\displaystyle a_{\mathrm {out} }=\int _{0}^{\infty }a_
      {\mathrm {batch} }(t)E(t)dt.}  [{\displaystyle a_{\mathrm {out} }=\int _
      {0}^{\infty }a_{\mathrm {batch} }(t)E(t)dt.}]
For given RTD, there is an upper limit on the amount of mixing that can occur,
called the maximum mixedness, and this determines the achievable yield. A
continuous stirred-tank reactor can be anywhere in the spectrum between
completely segregated and perfect_mixing.[1]
**** Groundwater flow[edit] ****
Hydraulic residence time (HRT) is an important factor in the transport of
environmental toxins or other chemicals through groundwater. The amount of time
that a pollutant spends traveling through a delineated subsurface space is
related to the saturation and the hydraulic_conductivity of the soil or rock.
[10] Porosity is another significant contributing factor to the mobility of
water through the ground (e.g. toward the water_table). The intersection
between pore density and size determines the degree or magnitude of the flow
rate through the media. This idea can be illustrated by a comparison of the
ways water moves through clay versus gravel. The retention time through a
specified vertical distance in clay will be longer than through the same
distance in gravel, even though they are both characterized as high porosity
materials. This is because the pore sizes are much larger in gravel media than
in clay, and so there is less hydrostatic_tension working against the
subsurface pressure_gradient and gravity.
Groundwater flow is important parameter for consideration in the design of
waste rock basins for mining operations. Waste rock is heterogeneous material
with particles varying from boulders to clay-sized particles, and it contains
sulfidic_pollutants which must be controlled such that they do not compromise
the quality of the water table and also so the runoff does not create
environmental problems in the surrounding areas.[10] Aquitards are clay zones
that can have such a degree of impermeability that they partially or completely
retard water flow.[6][11] These clay lenses can slow or stop seepage into the
water table, although if an aquitard is fractured and contaminated then it can
become a long-term source of groundwater contamination due to its low
permeability and high HRT.[11]
**** Water treatment[edit] ****
See also: Activated_sludge and Waste_stabilization_pond
Primary_treatment for wastewater or drinking water includes settling in a
sedimentation chamber to remove as much of the solid matter as possible before
applying additional treatments.[6] The amount removed is controlled by the
hydraulic residence time (HRT).[6] When water flows through a volume at a
slower rate, less energy is available to keep solid particles entrained in the
stream and there is more time for them to settle to the bottom. Typical HRTs
for sedimentation basins are around two hours,[6] although some groups
recommend longer times to remove micropollutants such as pharmaceuticals and
hormones.[12]
Disinfection is the last step in the tertiary_treatment of wastewater or
drinking water. The types of pathogens that occur in untreated water include
those that are easily killed like bacteria and viruses, and those that are more
robust such as protozoa and cysts.[6] The disinfection chamber must have a long
enough HRT to kill or deactivate all of them.
**** Surface science[edit] ****
See also: Surface_science
Atoms and molecules of gas or liquid can be trapped on a solid surface in a
process called adsorption. This is an exothermic_process involving a release of
heat, and heating the surface increases the probability that an atom will
escape within a given time. At a given temperature     T   {\displaystyle T}
[T], the residence time of an adsorbed atom is given by
         &#x03C4; =  &#x03C4;  0   exp &#x2061;  (    E   a     R T    )  ,
      {\displaystyle \tau =\tau _{0}\exp \left({\frac {E_{\mathrm {a} }}
      {RT}}\right),}  [{\displaystyle \tau =\tau _{0}\exp \left({\frac {E_
      {\mathrm {a} }}{RT}}\right),}]
where     R   {\displaystyle R}  [R] is the gas_constant,      E   a
{\displaystyle E_{\mathrm {a} }}  [{\displaystyle E_{\mathrm {a} }}] is an
activation_energy, and      &#x03C4;  0     {\displaystyle \tau _{0}}  [\tau _
{0}] is a prefactor that is correlated with the vibration times of the surface
atoms (generally of the order of      10  &#x2212; 12     {\displaystyle 10^{-
12}}  [10^{-12}] seconds).[13]:27[14]:196
In vacuum_technology, the residence time of gases on the surfaces of a vacuum
chamber can determine the pressure due to outgassing. If the chamber can be
heated, the above equation shows that the gases can be "baked out"; but if not,
then surfaces with a low residence time are needed to achieve ultra-high
vacuums.[14]:195
**** Environmental[edit] ****
In environmental terms, the residence time definition is adapted to fit with
ground water, the atmosphere, glaciers, lakes, streams, and oceans. More
specifically it is the time during which water remains within an aquifer, lake,
river, or other water body before continuing around the hydrological_cycle. The
time involved may vary from days for shallow gravel aquifers to millions of
years for deep aquifers with very low values for hydraulic_conductivity.
Residence times of water in rivers are a few days, while in large lakes
residence time ranges up to several decades. Residence times of continental ice
sheets is hundreds of thousands of years, of small glaciers a few decades.
Ground water residence time applications are useful for determining the amount
of time it will take for a pollutant to reach and contaminate a ground water
drinking water source and at what concentration it will arrive. This can also
work to the opposite effect to determine how long until a ground water source
becomes uncontaminated via inflow, outflow, and volume. The residence time of
lakes and streams is important as well to determine the concentration of
pollutants in a lake and how this may affect the local population and marine
life.
Hydrology, the study of water, discusses the water budget in terms of residence
time. The amount of time that water spends in each different stage of life
(glacier, atmosphere, ocean, lake, stream, river), is used to show the relation
of all of the water on the earth and how it relates in its different forms.
**** Pharmacology[edit] ****
A large class of drugs are enzyme_inhibitors that bind to enzymes in the body
and inhibit their activity. In this case it is the drug-target residence time
(the length of time the drug stays bound to the target) that is of interest.
Drugs with long residence times are desirable because they remain effective for
longer and therefore can be used in lower doses.[15]:88 This residence time is
determined by the kinetics of the interaction and is proportional to the half
life of the chemical_dissociation.[16] One way to measure the residence time is
in a preincubation-dilution experiment where a target enzyme is incubated with
the inhibitor, allowed to approach equilibrium, then rapidly diluted. The
amount of product is measured and compared to a control in which no inhibitor
is added.[15]:87â88
Residence time can also refer to the amount of time that a drug spends in the
part of the body where it needs to be absorbed. The longer the residence time,
the more of it can be absorbed. If the drug is delivered in an oral form and
destined for the upper_intestines, it usually moves with food and its residence
time is roughly that of the food. This generally allows 3 to 8 hours for
absorption.[17]:196 If the drug is delivered through a mucous_membrane in the
mouth, the residence time is short because saliva washes it away. Strategies to
increase this residence time include bioadhesive polymers, gums, lozenges and
dry powders.[17]:274
**** Queuing theory[edit] ****
Beyond fluid dynamics and chemistry, the definition(s) of residence time can be
applied to any flow_network, where the flows of generic "resources" is modeled
(e.g.: people, cars, money, products). Most notably, the over-mentioned
definition of residence time is extended to stationary random processes by
averaging on time (fluid_limit), obtaining the so-called Little's_Law, which is
a prominent relation in queueing_theory and supply_chain_management. In the
context of queueing theory, the residence time is addressed as waiting time,
while in the context of supply chain management it is most often addressed as
lead_time.
**** Biochemical[edit] ****
In size-exclusion_chromatography, the residence time of a molecule is related
to its volume, which is roughly proportional to its molecular weight. Residence
times also affect the performance of continuous_fermentors.[1]
Biofuel_cells utilize the metabolic processes of anodophiles (electronegative
bacteria) to convert chemical energy from organic matter into electricity.[18]
[19][20] A biofuel cell mechanism consists of an anode and a cathode that are
separated by an internal proton_exchange_membrane (PEM) and connected in an
external circuit with an external load. Anodophiles grow on the anode and
consume biodegradable organic molecules to produce electrons, protons, and
carbon_dioxide gas, and as the electrons travel though the circuit they feed
the external load.[19][20] The HRT for this application is the rate at which
the feed molecules are passed through the anodic chamber.[20] This can be
quantified by dividing the volume of the anodic chamber by the rate at which
the feed solution is passed into the chamber.[19] The hydraulic residence time
(HRT) affects the substrate loading rate of the microorganisms that the
anodophiles consume, which affects the electrical output.[20][21] Longer HRTs
reduce substrate loading in the anodic chamber which can lead to reduced
anodophile population and performance when there is a deficiency of nutrients.
[20] Shorter HRTs support the development of non-exoelectrogenous bacteria
which can reduce the Coulombic_efficiency electrochemical performance of the
fuel cell if the anodophiles must compete for resources or if they do not have
ample time to effectively degrade nutrients.[20]
***** See also[edit] *****
    * Anaerobic_digestion#Residence_time
    * Baseflow_residence_time
    * Estuarine_water_circulation#Residence_time
    * Lake_retention_time
    * Micromixing
    * RTD_studies_of_plug_flow_reactor
    * Space_time_(chemical_engineering)
    * Water_cycle#Residence_times
***** References[edit] *****
   1. ^ a b c d e f g h iNauman, E. Bruce (May 2008). "Residence Time Theory".
      Industrial & Engineering Chemistry Research. 47 (10): 3752â3766. doi:
      10.1021/ie071635a.
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
   3. ^ a bLevenspiel, Octave (1999). Chemical reaction engineering (3rd ed.).
      New York: Wiley. ISBN 978-1-60119-921-8.
   4. ^ a b c dBolin, Bert; Rodhe, Henning (February 1973). "A note on the
      concepts of age distribution and transit time in natural reservoirs".
      Tellus. 25 (1): 58â62. doi:10.1111/j.2153-3490.1973.tb01594.x.
   5. ^Schwartz, Stephen E. (1979). "Residence times in reservoirs under non-
      steady-state conditions: application to atmospheric SO2 and aerosol
      sulfate". Tellus. 31 (6): 530â547. doi:10.1111/j.2153-
      3490.1979.tb00935.x.
   6. ^ a bMonsen, Nancy E.; Cloern, James E.; Lucas, Lisa V.; Monismith,
      Stephen G. (September 2002). "A comment on the use of flushing time,
      residence time, and age as transport time scales". Limnology and
      Oceanography. 47 (5): 1545â1553. doi:10.4319/lo.2002.47.5.1545.
   7. ^ a b c d e fDavis, Mackenzie L.; Masten, Susan J. (2004). Principles of
      environmental engineering and science. Boston, Mass.: McGraw-Hill Higher
      Education. pp. 150, 267, 480, 500. ISBN 9780072921861.
   8. ^ a bColli, A. N.; Bisang, J. M. (September 2015). "Study of the
      influence of boundary conditions, non ideal stimulus and dynamics of
      sensors on the evaluation of residence time distributions".
      Electrochimica Acta. 176: 463â471. doi:10.1016/j.electacta.2015.07.019.
   9. ^Fogler, H. Scott (2006). Elements of chemical reaction engineering (4th
      ed.). Upper Saddle River, NJ: Prentice Hall. ISBN 978-0130473943.
  10. ^Colli, A. N.; Bisang, J. M. (August 2011). "Evaluation of the
      hydrodynamic behaviour of turbulence promoters in parallel plate
      electrochemical reactors by means of the dispersion model".
      Electrochimica Acta. 56 (21): 7312â7318. doi:10.1016/
      j.electacta.2011.06.047.
  11. ^ a bNoel, M. (1999). "Some_physical_properties_of_water_transport_in
      waste_material" (PDF). Mine, Water & Environment. 1999 IMWA Congress.
  12. ^ a bFaybishenko, Boris; Witherspoon, Paul A.; Gale, John (2005).
      Dynamics of fluids and transport in fractured rock. Washington: American
      Geophysical Union. pp. 165â167. ISBN 9780875904276.
  13. ^Ejhed, H.; FÃ¥ng, J.; Hansen, K.; Graae, L.; Rahmberg, M.; MagnÃ©r, J.;
      Dorgeloh, E.; Plaza, G. (March 2018). "The effect of hydraulic retention
      time in onsite wastewater treatment and removal of pharmaceuticals,
      hormones and phenolic utility substances". Science of the Total
      Environment. 618: 250â261. doi:10.1016/j.scitotenv.2017.11.011.
  14. ^Somorjai, Gabor A.; Li, Yimin (2010). Introduction to surface chemistry
      and catalysis (2nd ed.). Hoboken, N.J.: Wiley. ISBN 9780470508237.
  15. ^ a bHucknall, D.J.; Morris, A. (2003). Vacuum technology calculations in
      chemistry. Cambridge: RSC. ISBN 9781847552273.
  16. ^ a bLi, Jie Jack; Corey, E. J., eds. (2013). Drug discovery practices,
      processes, and perspectives. Hoboken, N.J.: John Wiley & Sons.
      ISBN 9781118354469.
  17. ^KeserÃ¼, GyÃ¶rgy; Swinney, David C.; Mannhold, Raimund; Kubinyi, Hugo;
      Folkers, Gerd (eds.). Thermodynamics and Kinetics of Drug Binding.
      ISBN 9783527335824.
  18. ^ a bMitra, Ashim K.; Kwatra, Deep; Vadlapudi, Aswani Dutt, eds. (2014).
      Drug Delivery. Jones & Bartlett Publishers. ISBN 9781449674267.
  19. ^Cheng, Ka Yu; Ho, Goen; Cord-Ruwisch, Ralf (January 2010). "Anodophilic
      Biofilm Catalyzes Cathodic Oxygen Reduction". Environmental Science &
      Technology. 44 (1): 518â525. doi:10.1021/es9023833.
  20. ^ a b cChouler, Jon; Di Lorenzo, Mirella (16 July 2015). "Water Quality
      Monitoring in Developing Countries; Can Microbial Fuel Cells be the
      Answer?". Biosensors. 5 (3): 450â470. doi:10.3390/bios5030450.
  21. ^ a b c d e fSantos, JoÃ£o B. Costa; de Barros, Vanine V. Silva; Linares,
      JosÃ© J. (30 November 2016). "The Hydraulic Retention Time as a Key
      Parameter for the Performance of a Cyclically Fed Glycerol-Based
      Microbial Fuel Cell from Biodiesel". Journal of the Electrochemical
      Society. 164 (3): H3001âH3006. doi:10.1149/2.0011703jes.
  22. ^Robertson, D.M (2016). "Water_Quality_and_the_Effects_of_Changes_in
      Phosphorus_Loading,_Red_Cedar_Lakes,_Barron_and_Washburn_Counties,
      Wisconsin". United States Geological Survey.
***** Further reading[edit] *****
    * Davis, M; Masten, Susan (2013). Principles of environmental engineering
      and science. New York: McGraw Hill. ISBN 9780077492199.
Leckner, Bo; Ghirelli, Frederico (2004). "Transport equation for local
residence time of a fluid". Chemical Engineering Science. 59 (3): 513â523.
doi:10.1016/j.ces.2003.10.013.
Lee, Peter I.D.; Amidon, Gordon L. (1996). "2. Time constant approach".
Pharmacokinetic analysis : a practical approach. Lancaster, Penn.: Technomic
Pub. pp. 15â60. ISBN 9781566764254.
</ref>
MacMullin, R.B.; Weber, M. (1935). "The theory of short-circuiting in
continuous-flow mixing vessels in series and kinetics of chemical reactions in
such systems". Transactions of American Institute of Chemical Engineers. 31
(2): 409â458.
Montgomery, Carla W. (2013). Environmental Geology (10th ed.). McGraw-Hill
Education. ISBN 9781259254598.
Nauman, E. Bruce (2004). "Residence Time Distributions". Handbook of Industrial
Mixing: Science and Practice. Wiley Interscience. pp. 1â17. ISBN 0-471-26919-
0.
Rowland, Malcolm; Tozer, Thomas N. (2011). Clinical Pharmacokinetics and
Pharmacodynamics: Concepts and Applications (4th ed.). New York, NY: Lippincott
Williams and Wilkins. ISBN 9780781750097.
Wolf, David; Resnick, William (November 1963). "Residence Time Distribution in
Real Systems". Industrial & Engineering Chemistry Fundamentals. 2 (4):
287â293. doi:10.1021/i160008a008.
***** External links[edit] *****
    * Mean_residence_time_(MRT):_Understanding_how_long_drug_molecules_stay_in
      the_body
    * Calculate_the_Hydraulic_Retention_Time (Lenntech)

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Residence_time&oldid=881495909"
Categories:
    * Aerospace_engineering
    * Biogeochemical_cycle
    * Chemical_reaction_engineering
    * Ecology
    * Environmental_engineering
    * Geochemistry
    * Hydraulic_engineering
    * Pharmacokinetics
    * Queueing_theory
    * Waste_treatment_technology
Hidden categories:
    * CS1:_long_volume_value
    * Articles_to_be_merged_from_May_2018
    * All_articles_to_be_merged
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
    * EspaÃ±ol
    * FranÃ§ais
Edit_links
    * This page was last edited on 2 February 2019, at 23:34 (UTC).
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
