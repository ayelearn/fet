The following text has been accessed from https://en.wikipedia.org/wiki/Shell_balance at Fri Aug 9 03:25:52 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Shell balance ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In fluid_mechanics, it may be necessary to determine how a fluid velocity
changes across the flow. This can be done with a shell balance.
A shell is a differential_element of the flow. By looking at the momentum and
forces on one small portion, it is possible to integrate over the flow to see
the larger picture of the flow as a whole. The balance is determining what goes
into and out of the shell. Momentum enters and leaves the shell through fluid
entering and leaving the shell and through shear_stress. In addition, there are
pressure and gravity forces on the shell. The goal of a shell balance is to
determine the velocity profile of the flow. The velocity profile is an equation
to calculate the velocity based on a specific location in the flow. From this,
it is possible to find a velocity for any point across the flow.
⁰
***** Contents *****
    * 1_Applications
    * 2_Requirements
    * 3_Performing_shell_balances
    * 4_Resources
***** Applications[edit] *****
Shell Balances can be used for many situations. For example, flow in a pipe,
flow of multiple fluids around each other, or flow due to pressure difference.
Although terms in the shell balance and boundary conditions will change, the
basic set up and process is the same. This system is useful to analyze any
fluid flow that holds true for the requirements listed below.
***** Requirements[edit] *****
In order for a shell balance to work, the flow must:
   1. Be laminar_flow
   2. Be without bends or curves in the flow
   3. Steady_State
   4. Have two boundary conditions
Boundary Conditions are used to find constants of integration.
   1. Fluid - Solid Boundary: No-slip_condition, the velocity of a liquid at a
      solid is equal to the velocity of the solid
   2. Liquid - Gas Boundary: Shear_Stress = 0
   3. Liquid - Liquid Boundary: Equal velocity and shear_stress on both liquids
***** Performing shell balances[edit] *****
The following is an outline of how to perform a basic shell balance.
If fluid is flowing between two horizontal surfaces, each with area A touching
the fluid, a differential shell of height Îy can be drawn between them as
shown in the diagram below.
[Diagram_of_the_shell_balance_process_in_fluid_mechanics]
In this example, the top surface is moving at velocity U and the bottom surface
is stationary
density of fluid = Ï
viscosity of fluid = Î¼
velocity in x direction =      V  x     {\displaystyle V_{x}}  [V_x], shown by
the diagonal line above. This is what a shell balance is solving for.
Conservation_of_Momentum is the Key of a Shell Balance
rate of momentum in - rate of momentum out + sum of all forces = 0
To perform a shell balance, follow the following basic steps:
1. Find momentum from shear stress
(Momentum from Shear Stress Into System) - (Momentum from Shear Stress Out of
System)
Momentum from Shear Stress goes into the shell at y and leaves the system at
y + Îy.
Shear stress = Ïyx, area = A, momentum = ÏyxA
2. Find momentum from flow
Momentum flows into the system at x = 0 and out at x = L
The flow is steady state. Therefore, the momentum flow at x = 0 is equal to the
moment of flow at x = L. Therefore, these cancel out.
3. Find gravity force on the shell
4. Find pressure forces
5. Plug into conservation of momentum and solve for Ïyx
6. Apply Newton's law of viscosity for a Newtonian_fluid
Ïyx = -Î¼(dVx/dy)
7. Integrate to find equation for velocity and use Boundary Conditions to find
constants of integration
Boundary 1: Top Surface: y = 0 and Vx = U
Boundary 2: Bottom Surface: y = D and Vx = 0
For examples of performing shell balances, visit the resources listed below.
***** Resources[edit] *****
    * "Problem_Solutions_in_Transport_Phenomena :_Fluid_Mechanics_Problems".
      Retrieved 2007-10-06.
    * Harriott, Peter; W. McCabe; J. Smith (2004). Unit_Operations_of_Chemical
      Engineering:_Seventh_Edition. McGraw-Hill Professional. pp. 68â132.
      ISBN 9780072848236.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Shell_balance&oldid=804048984"
Categories:
    * Fluid_mechanics
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
    * This page was last edited on 6 October 2017, at 11:30 (UTC).
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
