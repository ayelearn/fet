The following text has been accessed from https://en.wikipedia.org/wiki/Heat_transfer_through_fins at Fri Aug 9 03:20:59 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Heat transfer through fins ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Fins are extensions on exterior surfaces of objects that increase the rate of
heat_transfer to or from the object by increasing convection. This is achieved
by increasing the surface_area of the body, which in turn increases the heat
transfer rate by a sufficient degree. This is an efficient way of increasing
the rate, since the alternative way of doing so is by increasing either the
heat_transfer_coefficient (which depends on the nature of materials being used
and the conditions of use) or the temperature_gradient (which depends on the
conditions of use). Clearly, changing the shape of the bodies is more
convenient. Fins are therefore a very popular solution to increase the heat
transfer from surfaces and are widely used in a number of objects. The fin
material should preferably have high thermal_conductivity. In most applications
the fin is surrounded by a fluid in motion,[1] which heats or cools it quickly
due to the large surface area, and subsequently the heat gets transferred to or
from the body quickly due to the high thermal conductivity of the fin. For
optimal Heat transfer performance with minimal cost, the dimensions and shape
of the fin have to be calculated for specific applications, and this is called
design of a fin. A common way of doing so is by creating a model of the fin and
then simulating it under required service conditions.
***** Modeling[edit] *****
Consider a body with fins on its outer surface, with air flowing around it.
The heat transfer rate depends on
    * Shape and geometry of the external surface
    * Surface area of the body
    * Velocity of the wind (or any fluid in other cases)
    * Temperature of surroundings
Modelling of the fins in this case involves, experimenting on this physical
model and optimizing the number of fins and fin pitch for maximum performance.
[2]
One of the experimentally obtained equations for heat transfer coefficient for
the fin surface for low wind velocities is:
   k = 2.11  v  0.71    &#x03B8;  0.44    a  &#x2212; 0.14     {\displaystyle
k=2.11v^{0.71}\theta ^{0.44}a^{-0.14}}
[{\displaystyle k=2.11v^{0.71}\theta ^{0.44}a^{-0.14}}]
where
k= Fin surface heat transfer coefficient [W/m2K ]
a=fin length [mm]
v=wind velocity [km/hr]
Î¸=fin pitch [mm]
Another equation for high fluid velocities, obtained from experiments conducted
by Gibson, is
   k = 241.7 [ 0.0247 &#x2212; 0.00148 (  a  0.8    /   &#x03B8;  0.4   ) ]  v
0.73     {\displaystyle k=241.7[0.0247-0.00148(a^{0.8}/\theta ^{0.4})]v^{0.73}}
[{\displaystyle k=241.7[0.0247-0.00148(a^{0.8}/\theta ^{0.4})]v^{0.73}}]
where
k=Fin surface heat transfer coefficient[W/m2K ]
a=Fin length[mm]
Î¸=Fin pitch[mm]
v=Wind velocity[km/hr]
A more accurate equation for fin surface heat transfer coefficient is:
    k  a v g   = ( 2.47 &#x2212; 2.55  /   &#x03B8;  0.4   )  v  0.9   0.0872
&#x03B8; + 4.31   {\displaystyle k_{avg}=(2.47-2.55/\theta ^{0.4})v^
{0.9}0.0872\theta +4.31}
[{\displaystyle k_{avg}=(2.47-2.55/\theta ^{0.4})v^{0.9}0.0872\theta +4.31}]
where
k (avg)= Fin surface heat transfer coefficient[W/m2K ]
Î¸=Fin pitch[mm]
v=Wind velocity[km/hr]
All these equations can be used to evaluate average heat transfer coefficient
for various fin designs.
***** Design[edit] *****
The momentum conservation equation for this case is given as follows:
      &#x2202; ( &#x03C1; v )   &#x2202; t    + v &#x2207; . ( &#x03C1; v ) =
&#x2212; &#x2207; P + &#x2207; . &#x03C4; + F + &#x03C1; g   {\displaystyle
{\partial (\rho v) \over \partial t}+v\nabla .(\rho v)=-\nabla P+\nabla .\tau
+F+\rho g}
[{\displaystyle {\partial (\rho v) \over \partial t}+v\nabla .(\rho v)=-\nabla
P+\nabla .\tau +F+\rho g}]
This is used in combination with the continuity equation.
The energy equation is also needed, which is:
      &#x2202; ( &#x03C1; E )   &#x2202; t    + &#x2207; . [ v ( &#x03C1; E + p
) ] = &#x2207; . [  k  e f f   &#x2207; T &#x2212;  &#x03A3;  j    h  j    J  j
+ ( &#x03C4; . v ) ]   {\displaystyle {\partial (\rho E) \over \partial
t}+\nabla .[v(\rho E+p)]=\nabla .[k_{eff}\nabla T-\Sigma _{j}h_{j}J_{j}+(\tau
.v)]}
[{\displaystyle {\partial (\rho E) \over \partial t}+\nabla .[v(\rho
E+p)]=\nabla .[k_{eff}\nabla T-\Sigma _{j}h_{j}J_{j}+(\tau .v)]}]
.
The above equation, on solving, gives the temperature profile for the fluid
region.
When solved as a scalar equation, it can be used to calculate the temperatures
at the fin and cylinder surfaces, by reducing to:
    &#x2207;  2   T +     q .   k   =   1 &#x03B1;      &#x2202; T   &#x2202; t
{\displaystyle \nabla ^{2}T+{{\overset {.}{q}} \over k}={1 \over \alpha }
{\partial T \over \partial t}}
[{\displaystyle \nabla ^{2}T+{{\overset {.}{q}} \over k}={1 \over \alpha }
{\partial T \over \partial t}}]
Where:
q = internal heat generation = 0 (in this case).
Also dT/dt = 0 due to steady state assumption.
These flow and energy equations can be set up and solved in any simulation
software, e.g. Fluent. In order to do so, all parameters of flow and thermal
conditions like fluid velocity and temperature of body have to be specified
according to the requirement. Also, the boundary_conditions and assumptions if
any must be specified.
This results in velocity profiles and temperature profiles for various surfaces
and this knowledge can be used to design the fin.
***** References[edit] *****
   1. ^ "MIT_Thermodynamics"
   2. ^ Agarwal, Shrikhande, and Srinivasan "Heat_Transfer_Simulation_by_CFD
      from_Fins_of_an_Air_Cooled_Motorcycle_Engine_under_Varying_Climatic
      Conditions" WCE 2011, July 6â8, 2011, London, U.K.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Heat_transfer_through_fins&oldid=816794890"
Categories:
    * Unit_operations
    * Transport_phenomena
    * Heat_transfer
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
Add_links
    * This page was last edited on 23 December 2017, at 19:12 (UTC).
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
