The following text has been accessed from https://en.wikipedia.org/wiki/Fanno_flow at Thu Aug 8 23:15:56 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Fanno flow ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Fanno flow is the adiabatic flow through a constant area duct where the effect
of friction is considered.[1] Compressibility effects often come into
consideration, although the Fanno flow model certainly also applies to
incompressible_flow. For this model, the duct area remains constant, the flow
is assumed to be steady and one-dimensional, and no mass is added within the
duct. The Fanno flow model is considered an irreversible process due to viscous
effects. The viscous friction causes the flow properties to change along the
duct. The frictional effect is modeled as a shear stress at the wall acting on
the fluid with uniform properties over any cross section of the duct.
For a flow with an upstream Mach_number greater than 1.0 in a sufficiently long
enough duct, deceleration occurs and the flow can become choked. On the other
hand, for a flow with an upstream Mach number less than 1.0, acceleration
occurs and the flow can become choked in a sufficiently long duct. It can be
shown that for flow of calorically perfect gas the maximum entropy occurs at
M = 1.0. Fanno flow is named after Gino_Girolamo_Fanno.
⁰
***** Contents *****
    * 1_Theory
    * 2_Additional_Fanno_flow_relations
    * 3_Applications
    * 4_See_also
    * 5_References
    * 6_External_links
***** Theory[edit] *****
Figure 1 A Fanno Line is plotted on the dimensionless H-ÎS axis.
The Fanno flow model begins with a differential_equation that relates the
change in Mach number with respect to the length of the duct, dM/dx. Other
terms in the differential equation are the heat_capacity_ratio, Î³, the Fanning
friction_factor, f, and the hydraulic_diameter, Dh:
         &#xA0;    d  M  2     M  2     =    &#x03B3;  M  2     1 &#x2212;  M
      2       (  1 +    &#x03B3; &#x2212; 1  2    M  2    )     4 f   D  h
      d x   {\displaystyle \ {\frac {dM^{2}}{M^{2}}}={\frac {\gamma M^{2}}{1-M^
      {2}}}\left(1+{\frac {\gamma -1}{2}}M^{2}\right){\frac {4f}{D_{h}}}dx}  [\
      \frac{dM^2}{M^2} = \frac{\gamma M^2}{1 - M^2}\left(1 + \frac{\gamma - 1}
      {2}M^2\right)\frac{4f}{D_h}dx ]
Assuming the Fanning friction factor is a constant along the duct wall, the
differential equation can be solved easily.[2][3] One must keep in mind,
however, that the value of the Fanning friction factor can be difficult to
determine for supersonic and especially hypersonic flow velocities. The
resulting relation is shown below where L* is the required duct length to choke
the flow assuming the upstream Mach number is supersonic. The left-hand side is
often called the Fanno parameter.
         &#xA0;    4 f  L  &#x2217;     D  h     =  (    1 &#x2212;  M  2
      &#x03B3;  M  2      )  +  (    &#x03B3; + 1   2 &#x03B3;    )  ln
      &#x2061;  [    M  2     (   2  &#x03B3; + 1    )   (  1 +    &#x03B3;
      &#x2212; 1  2    M  2    )     ]    {\displaystyle \ {\frac {4fL^{*}}{D_
      {h}}}=\left({\frac {1-M^{2}}{\gamma M^{2}}}\right)+\left({\frac {\gamma
      +1}{2\gamma }}\right)\ln \left[{\frac {M^{2}}{\left({\frac {2}{\gamma
      +1}}\right)\left(1+{\frac {\gamma -1}{2}}M^{2}\right)}}\right]}  [\ \frac
      {4fL^*}{D_h} = \left(\frac{1 - M^2}{\gamma M^2}\right) + \left(\frac
      {\gamma + 1}{2\gamma}\right)\ln\left[\frac{M^2}{\left(\frac{2}{\gamma +
      1}\right)\left(1 + \frac{\gamma - 1}{2}M^2\right)}\right]]
Equally important to the Fanno flow model is the dimensionless ratio of the
change in entropy over the heat_capacity at constant pressure, cp.
         &#xA0; &#x0394; S =    &#x0394; s   c  p     = ln &#x2061;  [   M
      &#x03B3; &#x2212; 1  &#x03B3;      (   [   2  &#x03B3; + 1    ]   [  1 +
      &#x03B3; &#x2212; 1  2    M  2    ]   )     &#x2212; ( &#x03B3; + 1 )   2
      &#x03B3;      ]    {\displaystyle \ \Delta S={\frac {\Delta s}{c_
      {p}}}=\ln \left[M^{\frac {\gamma -1}{\gamma }}\left(\left[{\frac {2}
      {\gamma +1}}\right]\left[1+{\frac {\gamma -1}{2}}M^{2}\right]\right)^
      {\frac {-(\gamma +1)}{2\gamma }}\right]}  [\ \Delta S = \frac{\Delta s}
      {c_p} = \ln\left[M^\frac{\gamma - 1}{\gamma}\left(\left[\frac{2}{\gamma +
      1}\right]\left[1 + \frac{\gamma - 1}{2}M^2\right]\right)^\frac{-(\gamma +
      1)}{2\gamma}\right] ]
The above equation can be rewritten in terms of a static to stagnation
temperature ratio, which, for a calorically perfect gas, is equal to the
dimensionless enthalpy ratio, H:
         &#xA0; H =   h  h  0     =     c  p   T    c  p    T  0      =   T  T
      0       {\displaystyle \ H={\frac {h}{h_{0}}}={\frac {c_{p}T}{c_{p}T_
      {0}}}={\frac {T}{T_{0}}}}  [\ H = \frac{h}{h_0} = \frac{c_pT}{c_pT_0} =
      \frac{T}{T_0} ]
         &#xA0; &#x0394; S =    &#x0394; s   c  p     = ln &#x2061;  [
      (    1 H   &#x2212; 1  )     &#x03B3; &#x2212; 1   2 &#x03B3;       (   2
      &#x03B3; &#x2212; 1    )     &#x03B3; &#x2212; 1   2 &#x03B3;
      (    &#x03B3; + 1  2   )     &#x03B3; + 1   2 &#x03B3;       ( H )
      &#x03B3; + 1   2 &#x03B3;      ]    {\displaystyle \ \Delta S={\frac
      {\Delta s}{c_{p}}}=\ln \left[\left({\frac {1}{H}}-1\right)^{\frac {\gamma
      -1}{2\gamma }}\left({\frac {2}{\gamma -1}}\right)^{\frac {\gamma -1}
      {2\gamma }}\left({\frac {\gamma +1}{2}}\right)^{\frac {\gamma +1}{2\gamma
      }}\left(H\right)^{\frac {\gamma +1}{2\gamma }}\right]}  [\ \Delta S =
      \frac{\Delta s}{c_p} = \ln\left[\left(\frac{1}{H} - 1\right)^\frac{\gamma
      - 1}{2\gamma}\left(\frac{2}{\gamma - 1}\right)^\frac{\gamma - 1}
      {2\gamma}\left(\frac{\gamma + 1}{2}\right)^\frac{\gamma + 1}
      {2\gamma}\left(H\right)^\frac{\gamma + 1}{2\gamma}\right] ]
The equation above can be used to plot the Fanno line, which represents a locus
of states for given Fanno flow conditions on an H-ÎS diagram. In the diagram,
the Fanno line reaches maximum entropy at H = 0.833 and the flow is choked.
According to the Second_law_of_thermodynamics, entropy must always increase for
Fanno flow. This means that a subsonic flow entering a duct with friction will
have an increase in its Mach number until the flow is choked. Conversely, the
Mach number of a supersonic flow will decrease until the flow is choked. Each
point on the Fanno line corresponds with a different Mach number, and the
movement to choked flow is shown in the diagram.
The Fanno line defines the possible states for a gas when the mass flow rate
and total enthalpy are held constant, but the momentum varies. Each point on
the Fanno line will have a different momentum value, and the change in momentum
is attributable to the effects of friction.[4]
***** Additional Fanno flow relations[edit] *****
Figure 2 Common thermodynamic property ratios plotted as a function of Mach
number using the Fanno flow model.
As was stated earlier, the area and mass flow rate in the duct are held
constant for Fanno flow. Additionally, the stagnation_temperature remains
constant. These relations are shown below with the * symbol representing the
throat location where choking can occur. A stagnation property contains a 0
subscript.
             A    =  A  &#x2217;   =   constant        T  0      =  T  0
      &#x2217;   =   constant          m &#x02D9;       =     m &#x02D9;
      &#x2217;   =   constant         {\displaystyle {\begin{aligned}A&=A^{*}=
      {\mbox{constant}}\\T_{0}&=T_{0}^{*}={\mbox{constant}}\\{\dot {m}}&={\dot
      {m}}^{*}={\mbox{constant}}\end{aligned}}}  [\begin{align}
      A &= A^* = \mbox{constant} \\
      T_0 &= T_0^* = \mbox{constant} \\
      \dot{m} &= \dot{m}^* = \mbox{constant}
      \end{align} ]
Differential equations can also be developed and solved to describe Fanno flow
property ratios with respect to the values at the choking location. The ratios
for the pressure, density, temperature, velocity and stagnation pressure are
shown below, respectively. They are represented graphically along with the
Fanno parameter.
               p  p  &#x2217;        =   1 M     1   (   2  &#x03B3; + 1    )
      (  1 +    &#x03B3; &#x2212; 1  2    M  2    )           &#x03C1;
      &#x03C1;  &#x2217;        =   1 M      (   2  &#x03B3; + 1    )   (  1 +
      &#x03B3; &#x2212; 1  2    M  2    )          T  T  &#x2217;        =   1
      (   2  &#x03B3; + 1    )   (  1 +    &#x03B3; &#x2212; 1  2    M  2    )
      V  V  &#x2217;        = M   1   (   2  &#x03B3; + 1    )   (  1 +
      &#x03B3; &#x2212; 1  2    M  2    )            p  0    p  0   &#x2217;
      =   1 M     [   (   2  &#x03B3; + 1    )   (  1 +    &#x03B3; &#x2212; 1
      2    M  2    )   ]     &#x03B3; + 1   2  (  &#x03B3; &#x2212; 1  )
      {\displaystyle {\begin{aligned}{\frac {p}{p^{*}}}&={\frac {1}{M}}{\frac
      {1}{\sqrt {\left({\frac {2}{\gamma +1}}\right)\left(1+{\frac {\gamma -1}
      {2}}M^{2}\right)}}}\\{\frac {\rho }{\rho ^{*}}}&={\frac {1}{M}}{\sqrt
      {\left({\frac {2}{\gamma +1}}\right)\left(1+{\frac {\gamma -1}{2}}M^
      {2}\right)}}\\{\frac {T}{T^{*}}}&={\frac {1}{\left({\frac {2}{\gamma
      +1}}\right)\left(1+{\frac {\gamma -1}{2}}M^{2}\right)}}\\{\frac {V}{V^
      {*}}}&=M{\frac {1}{\sqrt {\left({\frac {2}{\gamma +1}}\right)\left(1+
      {\frac {\gamma -1}{2}}M^{2}\right)}}}\\{\frac {p_{0}}{p_{0}^{*}}}&={\frac
      {1}{M}}\left[\left({\frac {2}{\gamma +1}}\right)\left(1+{\frac {\gamma -
      1}{2}}M^{2}\right)\right]^{\frac {\gamma +1}{2\left(\gamma -
      1\right)}}\end{aligned}}}  [\begin{align}
      \frac{p}{p^*} &= \frac{1}{M}\frac{1}{\sqrt{\left(\frac{2}{\gamma +
      1}\right)\left(1 + \frac{\gamma - 1}{2}M^2\right)}} \\
      \frac{\rho}{\rho^*} &= \frac{1}{M}\sqrt{\left(\frac{2}{\gamma +
      1}\right)\left(1 + \frac{\gamma - 1}{2}M^2\right)} \\
      \frac{T}{T^*} &= \frac{1}{\left(\frac{2}{\gamma + 1}\right)\left(1 +
      \frac{\gamma - 1}{2}M^2\right)} \\
      \frac{V}{V^*} &= M\frac{1}{\sqrt{\left(\frac{2}{\gamma + 1}\right)\left(1
      + \frac{\gamma - 1}{2}M^2\right)}} \\
      \frac{p_0}{p_0^*} &= \frac{1}{M}\left[\left(\frac{2}{\gamma +
      1}\right)\left(1 + \frac{\gamma - 1}{2}M^2\right)\right]^\frac{\gamma +
      1}{2\left(\gamma - 1\right)}
      \end{align} ]
***** Applications[edit] *****
Figure 3 A supersonic nozzle leading into a constant area duct is depicted. The
initial conditions exist at point 1. Point 2 exists at the nozzle throat, where
M = 1. Point 3 labels the transition from isentropic to Fanno flow. Points 4
and 5 give the pre- and post-shock wave conditions, and point E is the exit
from the duct.
Figure 4 The H-S diagram is depicted for the conditions of Figure 3. Entropy is
constant for isentropic flow, so the conditions at point 1 move down vertically
to point 3. Next, the flow follows the Fanno line until a shock changes the
flow from supersonic to subsonic. The flow then follows the Fanno line again,
almost reaching a choked condition before exiting the duct.
Figure 5 Fanno and Rayleigh Line Intersection Chart.
The Fanno flow model is often used in the design and analysis of nozzles. In a
nozzle, the converging or diverging area is modeled with isentropic flow, while
the constant area section afterwards is modeled with Fanno flow. For given
upstream conditions at point 1 as shown in Figures 3 and 4, calculations can be
made to determine the nozzle exit Mach number and the location of a normal
shock in the constant area duct. Point 2 labels the nozzle throat, where M = 1
if the flow is choked. Point 3 labels the end of the nozzle where the flow
transitions from isentropic to Fanno. With a high enough initial pressure,
supersonic flow can be maintained through the constant area duct, similar to
the desired performance of a blowdown-type supersonic_wind_tunnel. However,
these figures show the shock wave before it has moved entirely through the
duct. If a shock wave is present, the flow transitions from the supersonic
portion of the Fanno line to the subsonic portion before continuing towards M =
1. The movement in Figure 4 is always from the left to the right in order to
satisfy the second law of thermodynamics.
The Fanno flow model is also used extensively with the Rayleigh_flow model.
These two models intersect at points on the enthalpy-entropy and Mach number-
entropy diagrams, which is meaningful for many applications. However, the
entropy values for each model are not equal at the sonic state. The change in
entropy is 0 at M = 1 for each model, but the previous statement means the
change in entropy from the same arbitrary point to the sonic point is different
for the Fanno and Rayleigh flow models. If initial values of si and Mi are
defined, a new equation for dimensionless entropy versus Mach number can be
defined for each model. These equations are shown below for Fanno and Rayleigh
flow, respectively.
             &#x0394;  S  F      =    s &#x2212;  s  i     c  p     = ln
      &#x2061;  [    (   M  M  i     )     &#x03B3; &#x2212; 1  &#x03B3;
      (    1 +    &#x03B3; &#x2212; 1  2    M  i   2     1 +    &#x03B3;
      &#x2212; 1  2    M  2      )     &#x03B3; + 1   2 &#x03B3;      ]
      &#x0394;  S  R      =    s &#x2212;  s  i     c  p     = ln &#x2061;
      [    (   M  M  i     )   2     (    1 + &#x03B3;  M  i   2     1 +
      &#x03B3;  M  2      )     &#x03B3; + 1  &#x03B3;     ]
      {\displaystyle {\begin{aligned}\Delta S_{F}&={\frac {s-s_{i}}{c_{p}}}=\ln
      \left[\left({\frac {M}{M_{i}}}\right)^{\frac {\gamma -1}{\gamma }}\left(
      {\frac {1+{\frac {\gamma -1}{2}}M_{i}^{2}}{1+{\frac {\gamma -1}{2}}M^
      {2}}}\right)^{\frac {\gamma +1}{2\gamma }}\right]\\\Delta S_{R}&={\frac
      {s-s_{i}}{c_{p}}}=\ln \left[\left({\frac {M}{M_{i}}}\right)^{2}\left(
      {\frac {1+\gamma M_{i}^{2}}{1+\gamma M^{2}}}\right)^{\frac {\gamma +1}
      {\gamma }}\right]\end{aligned}}}  [\begin{align}
      \Delta S_F &= \frac{s - s_i}{c_p} = \ln\left[\left(\frac{M}
      {M_i}\right)^\frac{\gamma - 1}{\gamma}\left(\frac{1 + \frac{\gamma - 1}
      {2}M_i^2}{1 + \frac{\gamma - 1}{2}M^2}\right)^\frac{\gamma + 1}
      {2\gamma}\right] \\
      \Delta S_R &= \frac{s - s_i}{c_p} = \ln\left[\left(\frac{M}
      {M_i}\right)^2\left(\frac{1 + \gamma M_i^2}{1 + \gamma M^2}\right)^\frac
      {\gamma + 1}{\gamma}\right]
      \end{align} ]
Figure 5 shows the Fanno and Rayleigh lines intersecting with each other for
initial conditions of si = 0 and Mi = 3. The intersection points are calculated
by equating the new dimensionless entropy equations with each other, resulting
in the relation below.
         &#xA0;  (  1 +    &#x03B3; &#x2212; 1  2    M  i   2    )   [    M  i
      2     (  1 + &#x03B3;  M  i   2    )   2     ]  =  (  1 +    &#x03B3;
      &#x2212; 1  2    M  2    )   [    M  2     (  1 + &#x03B3;  M  2    )   2
      ]    {\displaystyle \ \left(1+{\frac {\gamma -1}{2}}M_{i}^{2}\right)\left
      [{\frac {M_{i}^{2}}{\left(1+\gamma M_{i}^{2}\right)^{2}}}\right]=\left(1+
      {\frac {\gamma -1}{2}}M^{2}\right)\left[{\frac {M^{2}}{\left(1+\gamma M^
      {2}\right)^{2}}}\right]}  [\ \left(1 + \frac{\gamma - 1}
      {2}M_i^2\right)\left[\frac{M_i^2}{\left(1 + \gamma M_i^2\right)^2}\right]
      = \left(1 + \frac{\gamma - 1}{2}M^2\right)\left[\frac{M^2}{\left(1 +
      \gamma M^2\right)^2}\right] ]
The intersection points occur at the given initial Mach number and its post-
normal_shock value. For Figure 5, these values are M = 3 and 0.4752, which can
be found the normal shock tables listed in most compressible flow textbooks. A
given flow with a constant duct area can switch between the Fanno and Rayleigh
models at these points.
***** See also[edit] *****
    * Rayleigh_flow
    * Isentropic_process
    * Isothermal_flow
    * Gas_dynamics
    * Compressible_flow
    * Choked_flow
    * Enthalpy
    * Entropy
    * Isentropic_nozzle_flow
***** References[edit] *****
   1. ^ Shapiro, A.H., The Dynamics and Thermodynamics of Compressible Fluid
      Flow, Volume 1, Ronald Press, 1953.
   2. ^ Zucker, R.D., Biblarz, O., Fundamentals of Gas Dynamics, John Wiley &
      Sons, 2002.
   3. ^ Hodge, B.K., and Koenig, K., Compressible Fluid Dynamics with Personal
      Computer Applications, Prentice Hall, 1995.
   4. ^ The Phenomena of Fluid Motions, R. S. Brodkey, p187, R. S. Brodkey
      (pub), 1995
***** External links[edit] *****
    * Purdue_University_Adiabatic_and_Isothermal_Fanno_flow_calculators
    * University_of_Kentucky_Fanno_flow_Webcalculator
    * Maurice_W._Downey,_Gino_Fanno

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Fanno_flow&oldid=853297262"
Categories:
    * Flow_regimes
    * Aerodynamics
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
    * EspaÃ±ol
    * Italiano
    * ×¢××¨××ª
Edit_links
    * This page was last edited on 3 August 2018, at 19:12 (UTC).
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
