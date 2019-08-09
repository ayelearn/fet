The following text has been accessed from https://en.wikipedia.org/wiki/Rayleigh_flow at Thu Aug 8 23:15:51 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Rayleigh flow ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Rayleigh flow refers to frictionless, non-Adiabatic flow through a constant
area duct where the effect of heat addition or rejection is considered.
Compressibility effects often come into consideration, although the Rayleigh
flow model certainly also applies to incompressible_flow. For this model, the
duct area remains constant and no mass is added within the duct. Therefore,
unlike Fanno_flow, the stagnation_temperature is a variable. The heat addition
causes a decrease in stagnation_pressure, which is known as the Rayleigh effect
and is critical in the design of combustion systems. Heat addition will cause
both supersonic and subsonic Mach_numbers to approach Mach 1, resulting in
choked_flow. Conversely, heat rejection decreases a subsonic Mach number and
increases a supersonic Mach number along the duct. It can be shown that for
calorically perfect flows the maximum entropy occurs at M = 1. Rayleigh flow is
named after John_Strutt,_3rd_Baron_Rayleigh.
⁰
***** Contents *****
    * 1_Theory
    * 2_Additional_Rayleigh_Flow_Relations
    * 3_Applications
    * 4_See_also
    * 5_References
    * 6_External_links
***** Theory[edit] *****
Figure 1 A Rayleigh Line is plotted on the dimensionless H-ÎS axis.
The Rayleigh flow model begins with a differential_equation that relates the
change in Mach number with the change in stagnation_temperature, T0. The
differential equation is shown below.
         &#xA0;    d  M  2     M  2     =    1 + &#x03B3;  M  2     1 &#x2212;
      M  2       (  1 +    &#x03B3; &#x2212; 1  2    M  2    )     d  T  0
      T  0       {\displaystyle \ {\frac {dM^{2}}{M^{2}}}={\frac {1+\gamma M^
      {2}}{1-M^{2}}}\left(1+{\frac {\gamma -1}{2}}M^{2}\right){\frac {dT_{0}}
      {T_{0}}}}  [{\displaystyle \ {\frac {dM^{2}}{M^{2}}}={\frac {1+\gamma M^
      {2}}{1-M^{2}}}\left(1+{\frac {\gamma -1}{2}}M^{2}\right){\frac {dT_{0}}
      {T_{0}}}}]
Solving the differential equation leads to the relation shown below, where T0*
is the stagnation temperature at the throat location of the duct which is
required for thermally choking the flow.
         &#xA0;    T  0    T  0   &#x2217;     =    2  (  &#x03B3; + 1  )   M
      2      (  1 + &#x03B3;  M  2    )   2      (  1 +    &#x03B3; &#x2212; 1
      2    M  2    )    {\displaystyle \ {\frac {T_{0}}{T_{0}^{*}}}={\frac
      {2\left(\gamma +1\right)M^{2}}{\left(1+\gamma M^{2}\right)^{2}}}\left(1+
      {\frac {\gamma -1}{2}}M^{2}\right)}  [{\displaystyle \ {\frac {T_{0}}{T_
      {0}^{*}}}={\frac {2\left(\gamma +1\right)M^{2}}{\left(1+\gamma M^
      {2}\right)^{2}}}\left(1+{\frac {\gamma -1}{2}}M^{2}\right)}]
These values are significant in the design of combustion systems. For example,
if a turbojet combustion chamber has a maximum temperature of T0* = 2000 K, T0
and M at the entrance to the combustion chamber must be selected so thermal
choking does not occur, which will limit the mass flow rate of air into the
engine and decrease thrust.
For the Rayleigh flow model, the dimensionless change in entropy relation is
shown below.
         &#xA0; &#x0394; S =    &#x0394; s   c  p     = l n  [   M  2
      (    &#x03B3; + 1   1 + &#x03B3;  M  2      )     &#x03B3; + 1  &#x03B3;
      ]    {\displaystyle \ \Delta S={\frac {\Delta s}{c_{p}}}=ln\left[M^
      {2}\left({\frac {\gamma +1}{1+\gamma M^{2}}}\right)^{\frac {\gamma +1}
      {\gamma }}\right]}  [{\displaystyle \ \Delta S={\frac {\Delta s}{c_
      {p}}}=ln\left[M^{2}\left({\frac {\gamma +1}{1+\gamma M^{2}}}\right)^
      {\frac {\gamma +1}{\gamma }}\right]}]
The above equation can be used to plot the Rayleigh line on a Mach number
versus ÎS graph, but the dimensionless enthalpy, H, versus ÎS diagram is more
often used. The dimensionless enthalpy equation is shown below with an equation
relating the static_temperature with its value at the choke location for a
calorically perfect gas where the heat_capacity at constant pressure, cp,
remains constant.
             H    =   h  h  &#x2217;     =     c  p   T    c  p    T  &#x2217;
      =   T  T  &#x2217;           T  T  &#x2217;        =   [     (  &#x03B3;
      + 1  )  M   1 + &#x03B3;  M  2      ]   2         {\displaystyle {\begin
      {aligned}H&={\frac {h}{h^{*}}}={\frac {c_{p}T}{c_{p}T^{*}}}={\frac {T}{T^
      {*}}}\\{\frac {T}{T^{*}}}&=\left[{\frac {\left(\gamma +1\right)M}
      {1+\gamma M^{2}}}\right]^{2}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}H&={\frac {h}{h^{*}}}={\frac {c_{p}T}{c_{p}T^{*}}}={\frac {T}{T^
      {*}}}\\{\frac {T}{T^{*}}}&=\left[{\frac {\left(\gamma +1\right)M}
      {1+\gamma M^{2}}}\right]^{2}\end{aligned}}}]
The above equation can be manipulated to solve for M as a function of H.
However, due to the form of the T/T* equation, a complicated multi-root
relation is formed for M = M(T/T*). Instead, M can be chosen as an independent
variable where ÎS and H can be matched up in a chart as shown in Figure 1.
Figure 1 shows that heating will increase an upstream, subsonic Mach number
until M = 1.0 and the flow chokes. Conversely, adding heat to a duct with an
upstream, supersonic Mach number will cause the Mach number to decrease until
the flow chokes. Cooling produces the opposite result for each of those two
cases. The Rayleigh flow model reaches maximum entropy at M = 1.0 For subsonic
flow, the maximum value of H occurs at M = 0.845. This indicates that cooling,
instead of heating, causes the Mach number to move from 0.845 to 1.0 This is
not necessarily correct as the stagnation temperature always increases to move
the flow from a subsonic Mach number to M = 1, but from M = 0.845 to M = 1.0
the flow accelerates faster than heat is added to it. Therefore, this is a
situation where heat is added but T/T* decreases in that region.
***** Additional Rayleigh Flow Relations[edit] *****
The area and mass flow rate are held constant for Rayleigh flow. Unlike Fanno
flow, the Fanning_friction_factor, f, remains constant. These relations are
shown below with the * symbol representing the throat location where choking
can occur.
             A    =  A  &#x2217;   =   constant          m &#x02D9;       =
      m &#x02D9;     &#x2217;   =   constant         {\displaystyle {\begin
      {aligned}A&=A^{*}={\mbox{constant}}\\{\dot {m}}&={\dot {m}}^{*}={\mbox
      {constant}}\\\end{aligned}}}  [{\displaystyle {\begin{aligned}A&=A^{*}=
      {\mbox{constant}}\\{\dot {m}}&={\dot {m}}^{*}={\mbox{constant}}\\\end
      {aligned}}}]
Differential equations can also be developed and solved to describe Rayleigh
flow property ratios with respect to the values at the choking location. The
ratios for the pressure, density, static temperature, velocity and stagnation
pressure are shown below, respectively. They are represented graphically along
with the stagnation temperature ratio equation from the previous section. A
stagnation property contains a '0' subscript.
               p  p  &#x2217;        =    &#x03B3; + 1   1 + &#x03B3;  M  2
      &#x03C1;  &#x03C1;  &#x2217;        =    1 + &#x03B3;  M  2
      (  &#x03B3; + 1  )   M  2            T  T  &#x2217;        =
      (  &#x03B3; + 1  )   2    M  2      (  1 + &#x03B3;  M  2    )   2
      v  v  &#x2217;        =     (  &#x03B3; + 1  )   M  2     1 + &#x03B3;  M
      2             p  0    p  0   &#x2217;        =    &#x03B3; + 1   1 +
      &#x03B3;  M  2        [   (   2  &#x03B3; + 1    )   (  1 +    &#x03B3;
      &#x2212; 1  2    M  2    )   ]    &#x03B3;  &#x03B3; &#x2212; 1
      {\displaystyle {\begin{aligned}{\frac {p}{p^{*}}}&={\frac {\gamma +1}
      {1+\gamma M^{2}}}\\{\frac {\rho }{\rho ^{*}}}&={\frac {1+\gamma M^{2}}
      {\left(\gamma +1\right)M^{2}}}\\{\frac {T}{T^{*}}}&={\frac {\left(\gamma
      +1\right)^{2}M^{2}}{\left(1+\gamma M^{2}\right)^{2}}}\\{\frac {v}{v^
      {*}}}&={\frac {\left(\gamma +1\right)M^{2}}{1+\gamma M^{2}}}\\{\frac {p_
      {0}}{p_{0}^{*}}}&={\frac {\gamma +1}{1+\gamma M^{2}}}\left[\left({\frac
      {2}{\gamma +1}}\right)\left(1+{\frac {\gamma -1}{2}}M^{2}\right)\right]^
      {\frac {\gamma }{\gamma -1}}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}{\frac {p}{p^{*}}}&={\frac {\gamma +1}{1+\gamma M^{2}}}\\{\frac
      {\rho }{\rho ^{*}}}&={\frac {1+\gamma M^{2}}{\left(\gamma +1\right)M^
      {2}}}\\{\frac {T}{T^{*}}}&={\frac {\left(\gamma +1\right)^{2}M^{2}}{\left
      (1+\gamma M^{2}\right)^{2}}}\\{\frac {v}{v^{*}}}&={\frac {\left(\gamma
      +1\right)M^{2}}{1+\gamma M^{2}}}\\{\frac {p_{0}}{p_{0}^{*}}}&={\frac
      {\gamma +1}{1+\gamma M^{2}}}\left[\left({\frac {2}{\gamma
      +1}}\right)\left(1+{\frac {\gamma -1}{2}}M^{2}\right)\right]^{\frac
      {\gamma }{\gamma -1}}\end{aligned}}}]
***** Applications[edit] *****
Figure 3 Fanno and Rayleigh Line Intersection Chart.
The Rayleigh flow model has many analytical uses, most notably involving
aircraft engines. For instance, the combustion chambers inside turbojet engines
usually have a constant area and the fuel mass addition is negligible. These
properties make the Rayleigh flow model applicable for heat addition to the
flow through combustion, assuming the heat addition does not result in
dissociation of the air-fuel mixture. Producing a shock wave inside the
combustion chamber of an engine due to thermal choking is very undesirable due
to the decrease in mass flow rate and thrust. Therefore, the Rayleigh flow
model is critical for an initial design of the duct geometry and combustion
temperature for an engine.
The Rayleigh flow model is also used extensively with the Fanno_flow model.
These two models intersect at points on the enthalpy-entropy and Mach number-
entropy diagrams, which is meaningful for many applications. However, the
entropy values for each model are not equal at the sonic state. The change in
entropy is 0 at M = 1 for each model, but the previous statement means the
change in entropy from the same arbitrary point to the sonic point is different
for the Fanno and Rayleigh flow models. If initial values of si and Mi are
defined, a new equation for dimensionless entropy versus Mach number can be
defined for each model. These equations are shown below for Fanno and Rayleigh
flow, respectively.
             &#x0394;  S  F      =    s &#x2212;  s  i     c  p     = l n
      [    (   M  M  i     )     &#x03B3; &#x2212; 1  &#x03B3;      (    1 +
      &#x03B3; &#x2212; 1  2    M  i   2     1 +    &#x03B3; &#x2212; 1  2    M
      2      )     &#x03B3; + 1   2 &#x03B3;      ]      &#x0394;  S  R      =
      s &#x2212;  s  i     c  p     = l n  [    (   M  M  i     )   2
      (    1 + &#x03B3;  M  i   2     1 + &#x03B3;  M  2      )     &#x03B3; +
      1  &#x03B3;     ]        {\displaystyle {\begin{aligned}\Delta S_{F}&=
      {\frac {s-s_{i}}{c_{p}}}=ln\left[\left({\frac {M}{M_{i}}}\right)^{\frac
      {\gamma -1}{\gamma }}\left({\frac {1+{\frac {\gamma -1}{2}}M_{i}^{2}}{1+
      {\frac {\gamma -1}{2}}M^{2}}}\right)^{\frac {\gamma +1}{2\gamma
      }}\right]\\\Delta S_{R}&={\frac {s-s_{i}}{c_{p}}}=ln\left[\left({\frac
      {M}{M_{i}}}\right)^{2}\left({\frac {1+\gamma M_{i}^{2}}{1+\gamma M^
      {2}}}\right)^{\frac {\gamma +1}{\gamma }}\right]\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\Delta S_{F}&={\frac {s-s_{i}}{c_
      {p}}}=ln\left[\left({\frac {M}{M_{i}}}\right)^{\frac {\gamma -1}{\gamma
      }}\left({\frac {1+{\frac {\gamma -1}{2}}M_{i}^{2}}{1+{\frac {\gamma -1}
      {2}}M^{2}}}\right)^{\frac {\gamma +1}{2\gamma }}\right]\\\Delta S_{R}&=
      {\frac {s-s_{i}}{c_{p}}}=ln\left[\left({\frac {M}{M_{i}}}\right)^{2}\left
      ({\frac {1+\gamma M_{i}^{2}}{1+\gamma M^{2}}}\right)^{\frac {\gamma +1}
      {\gamma }}\right]\end{aligned}}}]
Figure 3 shows the Rayleigh and Fanno lines intersecting with each other for
initial conditions of si = 0 and Mi = 3.0 The intersection points are
calculated by equating the new dimensionless entropy equations with each other,
resulting in the relation below.
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
normal_shock value. For Figure 3, these values are M = 3.0 and 0.4752, which
can be found the normal shock tables listed in most compressible flow
textbooks. A given flow with a constant duct area can switch between the
Rayleigh and Fanno models at these points.
***** See also[edit] *****
    * Fanno_flow
    * Isentropic_process
    * Isothermal_flow
    * Gas_dynamics
    * Compressible_flow
    * Choked_flow
    * Enthalpy
    * Entropy
***** References[edit] *****
    * Strutt, John William (Lord Rayleigh) (1910). "Aerial_plane_waves_of
      finite_amplitudes". Proc. R. Soc. Lond. A. 84. pp. 247â284.
, also in:
    * Dover, ed. (1964). Scientific_papers_of_Lord_Rayleigh_(John_William
      Strutt). 5. pp. 573â610.
Zucker, Robert D.; Biblarz O. (2002). "Chapter 10. Rayleigh flow". Fundamentals
of Gas Dynamics. John_Wiley_&_Sons. pp. 277â313. ISBN 0-471-05967-6.
Shapiro, Ascher H. (1953). The Dynamics and Thermodynamics of Compressible
Fluid Flow, Volume 1. Ronald_Press. ISBN 978-0-471-06691-0.
Hodge, B. K.; Koenig K. (1995). Compressible Fluid Dynamics with Personal
Computer Applications. Prentice_Hall. ISBN 0-13-308552-X.
Emanuel, G. (1986). "Chapter 8.2 Rayleigh flow". Gasdynamics: Theory and
Applications. AIAA. pp. 121â133. ISBN 0-930403-12-6.
***** External links[edit] *****
 Wikimedia Commons has media related to Rayleigh_flow.
    * Purdue_University_Rayleigh_flow_calculator
    * University_of_Kentucky_Rayleigh_flow_Webcalculator

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Rayleigh_flow&oldid=851639233"
Categories:
    * Fluid_mechanics
    * Fluid_dynamics
    * Aerodynamics
Hidden categories:
    * Commons_category_link_from_Wikidata
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
    * EspaÃ±ol
    * Italiano
    * ×¢××¨××ª
Edit_links
    * This page was last edited on 23 July 2018, at 16:45 (UTC).
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
