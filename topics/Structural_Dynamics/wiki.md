The following text has been accessed from https://en.wikipedia.org/wiki/Structural_dynamics at Thu Aug 8 23:12:04 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Structural dynamics ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Structural dynamics, is a type of structural_analysis which covers the behavior
of a structure subjected to dynamic (actions having high acceleration) loading.
Dynamic loads include people, wind, waves, traffic, earthquakes, and blasts.
Any structure can be subjected to dynamic loading. Dynamic analysis can be used
to find dynamic displacements, time history, and modal_analysis.
Structural analysis is mainly concerned with finding out the behavior of a
physical structure when subjected to force. This action can be in the form of
load due to the weight of things such as people, furniture, wind, snow, etc. or
some other kind of excitation such as an earthquake, shaking of the ground due
to a blast nearby, etc. In essence all these loads are dynamic, including the
self-weight of the structure because at some point in time these loads were not
there. The distinction is made between the dynamic and the static analysis on
the basis of whether the applied action has enough acceleration in comparison
to the structure's natural frequency. If a load is applied sufficiently slowly,
the inertia forces (Newton's_first_law_of_motion) can be ignored and the
analysis can be simplified as static analysis.
A static load is one which varies very slowly. A dynamic load is one which
changes with time fairly quickly in comparison to the structure's natural
frequency. If it changes slowly, the structure's response may be determined
with static analysis, but if it varies quickly (relative to the structure's
ability to respond), the response must be determined with a dynamic analysis.
Dynamic analysis for simple structures can be carried out manually, but for
complex structures finite_element_analysis can be used to calculate the mode
shapes and frequencies.
⁰
***** Contents *****
    * 1_Displacements
    * 2_Time_history_analysis
          o 2.1_Example
    * 3_Damping
    * 4_Modal_analysis
          o 4.1_Energy_method
          o 4.2_Modal_response
    * 5_Modal_participation_factor
    * 6_External_links
***** Displacements[edit] *****
A dynamic load can have a significantly larger effect than a static load of the
same magnitude due to the structure's inability to respond quickly to the
loading (by deflecting). The increase in the effect of a dynamic load is given
by the dynamic_amplification_factor (DAF) or dynamic load factor(DLF):
         D A F = D L F =    u  m a x    u  s t a t i c       {\displaystyle
      DAF=DLF={\frac {u_{max}}{u_{static}}}}  [{\displaystyle DAF=DLF={\frac
      {u_{max}}{u_{static}}}}]
where u is the deflection of the structure due to the applied load.
Graphs of dynamic amplification factors vs non-dimensional rise_time (tr/T)
exist for standard loading functions (for an explanation of rise time, see time
history analysis below). Hence the DAF for a given loading can be read from the
graph, the static deflection can be easily calculated for simple structures and
the dynamic deflection found.
***** Time history analysis[edit] *****
A full time history will give the response of a structure over time during and
after the application of a load. To find the full time history of a structure's
response, you must solve the structure's equation_of_motion.
**** Example[edit] ****
[Single_degree_of_freedom_system:_simple_mass_spring_model]
A simple single degree_of_freedom system (a mass, M, on a spring of stiffness
k, for example) has the following equation of motion:
         M    x &#x00A8;    + k x = F ( t )   {\displaystyle M{\ddot {x}}+kx=F
      (t)}  [M{{\ddot  {x}}}+kx=F(t)]
where        x &#x00A8;      {\displaystyle {\ddot {x}}}  [{\ddot {x}}] is the
acceleration (the double derivative of the displacement) and x is the
displacement.
If the loading F(t) is a Heaviside_step_function (the sudden application of a
constant load), the solution to the equation of motion is:
         x =    F  0   k   [ 1 &#x2212; c o s  ( &#x03C9; t )  ]
      {\displaystyle x={\frac {F_{0}}{k}}[1-cos{(\omega t)}]}  [x={\frac  {{F_
      {0}}}{{k}}}[1-cos{(\omega t)}]]
where     &#x03C9; =    k M      {\displaystyle \omega ={\sqrt {\frac {k}{M}}}}
[\omega ={\sqrt  {{\frac  {{k}}{{M}}}}}] and the fundamental natural frequency,
f =   &#x03C9;  2 &#x03C0;      {\displaystyle f={\frac {\omega }{2\pi }}}  [f=
{\frac  {\omega }{2\pi }}].
The static deflection of a single degree of freedom system is:
          x  s t a t i c   =    F  0   k     {\displaystyle x_{static}={\frac
      {F_{0}}{k}}}  [x_{{static}}={\frac  {{F_{0}}}{{k}}}]
so you can write, by combining the above formulae:
         x =  x  s t a t i c   [ 1 &#x2212; c o s ( &#x03C9; t ) ]
      {\displaystyle x=x_{static}[1-cos(\omega t)]}  [x=x_{{static}}[1-cos
      (\omega t)]]
This gives the (theoretical) time history of the structure due to a load F(t),
where the false assumption is made that there is no damping.
Although this is too simplistic to apply to a real structure, the Heaviside
Step Function is a reasonable model for the application of many real loads,
such as the sudden addition of a piece of furniture, or the removal of a prop
to a newly cast concrete floor. However, in reality loads are never applied
instantaneously - they build up over a period of time (this may be very short
indeed). This time is called the rise_time.
As the number of degrees of freedom of a structure increases it very quickly
becomes too difficult to calculate the time history manually - real structures
are analysed using non-linear finite_element_analysis software.
***** Damping[edit] *****
Any real structure will dissipate energy (mainly through friction). This can be
modelled by modifying the DAF
         D A F = 1 +  e  &#x2212; c &#x03C0;     {\displaystyle DAF=1+e^{-c\pi
      }}  [DAF=1+e^{{-c\pi }}]
where     c =   Damping Coefficient Critical Damping Coefficient
{\displaystyle c={\frac {\text{Damping Coefficient}}{\text{Critical Damping
Coefficient}}}}  [c={\frac  {{{\text{Damping Coefficient}}}}{{{\text{Critical
Damping Coefficient}}}}}] and is typically 2%-10% depending on the type of
construction:
    * Bolted steel ~6%
    * Reinforced concrete ~ 5%
    * Welded steel ~ 2%
    * Brick masonry ~ 10%
Methods to increase damping
One of the widely used methods to increase damping is to attach a layer of
material with a high Damping Coefficient, for example rubber, to a vibrating
structure.
***** Modal analysis[edit] *****
A modal_analysis calculates the frequency modes or natural frequencies of a
given system, but not necessarily its full-time history response to a given
input. The natural frequency of a system is dependent only on the stiffness of
the structure and the mass which participates with the structure (including
self-weight). It is not dependent on the load function.
It is useful to know the modal frequencies of a structure as it allows you to
ensure that the frequency of any applied periodic loading will not coincide
with a modal frequency and hence cause resonance, which leads to large
oscillations.
The method is:
   1. Find the natural modes (the shape adopted by a structure) and natural
      frequencies
   2. Calculate the response of each mode
   3. Optionally superpose the response of each mode to find the full modal
      response to a given loading
**** Energy method[edit] ****
It is possible to calculate the frequency of different mode shape of system
manually by the energy_method. For a given mode shape of a multiple degree of
freedom system you can find an "equivalent" mass, stiffness and applied force
for a single degree of freedom system. For simple structures the basic mode
shapes can be found by inspection, but it is not a conservative method.
Rayleigh's principle states:
"The frequency Ï of an arbitrary mode of vibration, calculated by the energy
method, is always greater than - or equal to - the fundamental frequency Ïn."
For an assumed mode shape        u &#x00AF;    ( x )   {\displaystyle {\bar
{u}}(x)}  [{\bar  {u}}(x)], of a structural system with mass M; bending
stiffness, EI (Young's_modulus, E, multiplied by the second_moment_of_area, I);
and applied force, F(x):
          Equivalent mass,&#xA0;   M  e q   = &#x222B;  M     u &#x00AF;     2
      d u   {\displaystyle {\text{Equivalent mass, }}M_{eq}=\int {M{\bar {u}}^
      {2}}du}  [{\text{Equivalent mass, }}M_{{eq}}=\int {M{\bar  {u}}^{2}}du]
          Equivalent stiffness,&#xA0;   k  e q   = &#x222B;  E I   (       d  2
      u &#x00AF;      d  x  2         )    2    d x   {\displaystyle {\text
      {Equivalent stiffness, }}k_{eq}=\int {EI{\bigg (}{\frac {d^{2}{\bar {u}}}
      {dx^{2}}}{\bigg )}^{2}}dx}  [{\text{Equivalent stiffness, }}k_{{eq}}=\int
      {EI{\bigg (}{\frac  {{d^{2}{\bar  {u}}}}{{dx^{2}}}}{\bigg )}^{2}}dx]
          Equivalent force,&#xA0;   F  e q   = &#x222B;  F    u &#x00AF;     d
      x   {\displaystyle {\text{Equivalent force, }}F_{eq}=\int {F{\bar
      {u}}}dx}  [{\text{Equivalent force, }}F_{{eq}}=\int {F{\bar  {u}}}dx]
then, as above:
         &#x03C9; =     k  e q    M  e q        {\displaystyle \omega ={\sqrt
      {\frac {k_{eq}}{M_{eq}}}}}  [\omega ={\sqrt  {{\frac  {{k_{{eq}}}}{{M_{
      {eq}}}}}}}]
**** Modal response[edit] ****
The complete modal response to a given load F(x,t) is     v ( x , t ) =
&#x2211;   u  n   ( x , t )    {\displaystyle v(x,t)=\sum {u_{n}(x,t)}}  [v
(x,t)=\sum {u_{n}(x,t)}]. The summation can be carried out by one of three
common methods:
    * Superpose complete time histories of each mode (time consuming, but
      exact)
    * Superpose the maximum amplitudes of each mode (quick but conservative)
    * Superpose the square root of the sum of squares (good estimate for well-
      separated frequencies, but unsafe for closely spaced frequencies)
To superpose the individual modal responses manually, having calculated them by
the energy method:
Assuming that the rise time tr is known (T = 2Ï/Ï), it is possible to read
the DAF from a standard graph. The static displacement can be calculated with
u  s t a t i c   =    F  1 , e q    k  1 , e q       {\displaystyle u_{static}=
{\frac {F_{1,eq}}{k_{1,eq}}}}  [u_{{static}}={\frac  {F_{{1,eq}}}{k_{
{1,eq}}}}]. The dynamic displacement for the chosen mode and applied force can
then be found from:
          u  m a x   =  u  s t a t i c   D A F   {\displaystyle u_{max}=u_
      {static}DAF}  [u_{{max}}=u_{{static}}DAF]
***** Modal participation factor[edit] *****
For real systems there is often mass participating in the forcing_function
(such as the mass of ground in an earthquake) and mass participating in inertia
effects (the mass of the structure itself, Meq). The modal_participation_factor
Î is a comparison of these two masses. For a single degree of freedom system
Î = 1.
      Î     =    &#x2211;   M  n       u &#x00AF;     n      &#x2211;   M  n
      u &#x00AF;     n   2         {\displaystyle ={\frac {\sum {M_{n}{\bar
      {u}}_{n}}}{\sum {M_{n}{\bar {u}}_{n}^{2}}}}}  [={\frac  {\sum {M_{n}{\bar
      {u}}_{n}}}{\sum {M_{n}{\bar  {u}}_{n}^{2}}}}]
***** External links[edit] *****
    * DYSSOLVE:_Dynamic_System_Solver - An encrypted-source, lightweight, free-
      of-charge software that can be used to solve basic structural dynamics
      problems.
    * Structural_Dynamics_and_Vibration_Laboratory_of_McGill_University
    * Frame3DD_open_source_3D_structural_dynamics_analysis_program
    * Frequency_response_function_from_modal_parameters
    * Structural_Dynamics_Tutorials_&_Matlab_scripts
    * AIAA_Exploring_Structural_Dynamics (http://
      www.exploringstructuraldynamics.org/ ) - Structural Dynamics in Aerospace
      Engineering: Interactive Demos, Videos & Interviews with Practicing
      Engineers

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Structural_dynamics&oldid=904433326"
Categories:
    * Structural_analysis
    * Dynamics_(mechanics)
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
    * Deutsch
    * ÙØ§Ø±Ø³Û
    * Italiano
    * PortuguÃªs
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 2 July 2019, at 04:06 (UTC).
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
