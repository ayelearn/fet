The following text has been accessed from https://en.wikipedia.org/wiki/London_equations at Fri Aug 9 03:09:32 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** London equations ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
As a material drops below its superconducting critical temperature, magnetic
fields within the material are expelled via the Meissner_effect. The London
equations give a quantitative explanation of this effect.
Part of a series of articles about
Electromagnetism
[Solenoid]
    * Electricity
    * Magnetism
Electrostatics
    * Conductor
    * Coulomb's_law
    * Electric_charge
    * Electric_dipole_moment
    * Electric_field
    * Electric_flux / potential_energy
    * Electrostatic_discharge
    * Gauss's_law
    * Induction
    * Insulator
    * Polarization_density
    * Static_electricity
    * Triboelectricity
Magnetostatics
    * AmpÃ¨re's_law
    * BiotâSavart_law
    * Gauss's_law_for_magnetism
    * Magnetic_field
    * Magnetic_flux
    * Magnetic_dipole_moment
    * Magnetization
    * Magnetomotive_force
Electrodynamics
    * Lorentz_force_law
    * Electromagnetic_induction
    * Faraday's_law
    * Lenz's_law
    * Displacement_current
    * Magnetic_potential
    * Maxwell's_equations
    * Electromagnetic_field
    * Electromagnetic_pulse
    * Electromagnetic_radiation
    * Maxwell_tensor
    * Poynting_vector
    * LiÃ©nardâWiechert_potential
    * Jefimenko's_equations
    * Eddy_current
    * London equations
    * Mathematical_descriptions_of_the_electromagnetic_field
Electrical_network
    * Alternating_current
    * Capacitance
    * Direct_current
    * Electric_current
    * Electric_potential
    * Electromotive_force
    * Impedance
    * Inductance
    * Ohm's_law
    * Parallel_circuit
    * Resistance
    * Resonant_cavities
    * Series_circuit
    * Voltage
    * Waveguides
Covariant_formulation
    * Electromagnetic_tensor
      (stressâenergy_tensor)
    * Four-current
    * Electromagnetic_four-potential
Scientists
    * AmpÃ¨re
    * Biot
    * Coulomb
    * Faraday
    * Gauss
    * Heaviside
    * Henry
    * Hertz
    * Lenz
    * Lorentz
    * Maxwell
    * Ãrsted
    * Savart
    * Tesla
    * Volta
    * Weber
    * v
    * t
    * e
The London equations, developed by brothers Fritz and Heinz_London in 1935,[1]
relate current to electromagnetic_fields in and around a superconductor.
Arguably the simplest meaningful description of superconducting phenomena, they
form the genesis of almost any modern introductory text on the subject.[2][3]
[4] A major triumph of the equations is their ability to explain the Meissner
effect,[5] wherein a material exponentially expels all internal magnetic fields
as it crosses the superconducting threshold.
⁰
***** Contents *****
    * 1_Formulations
    * 2_London_penetration_depth
    * 3_Rationale_for_the_London_equations
          o 3.1_Original_arguments
          o 3.2_Canonical_momentum_arguments
    * 4_References
***** Formulations[edit] *****
There are two London equations when expressed in terms of measurable fields:
            &#x2202;   j   s     &#x2202; t    =     n  s    e  2    m    E  ,
      &#x2207;  &#x00D7;   j   s   = &#x2212;     n  s    e  2    m    B  .
      {\displaystyle {\frac {\partial \mathbf {j} _{s}}{\partial t}}={\frac {n_
      {s}e^{2}}{m}}\mathbf {E} ,\qquad \mathbf {\nabla } \times \mathbf {j} _
      {s}=-{\frac {n_{s}e^{2}}{m}}\mathbf {B} .}  [{\displaystyle {\frac
      {\partial \mathbf {j} _{s}}{\partial t}}={\frac {n_{s}e^{2}}{m}}\mathbf
      {E} ,\qquad \mathbf {\nabla } \times \mathbf {j} _{s}=-{\frac {n_{s}e^
      {2}}{m}}\mathbf {B} .}]
Here        j    s     {\displaystyle {\mathbf {j} }_{s}}  [{{\mathbf  {j}}}_
{s}] is the superconducting current_density, E and B are respectively the
electric and magnetic fields within the superconductor,     e    {\displaystyle
e\,}  [e\,] is the charge of an electron & proton,     m    {\displaystyle m\,}
[m\,] is electron mass, and      n  s      {\displaystyle n_{s}\,}  [n_s\,] is
a phenomenological constant loosely associated with a number density of
superconducting carriers.[6] Throughout this article SI_units are employed.
On the other hand, if one is willing to abstract away slightly, both the
expressions above can more neatly be written in terms of a single "London
Equation"[6][7] in terms of the vector_potential A:
           j   s   = &#x2212;     n  s    e  2    m    A  .   {\displaystyle
      \mathbf {j} _{s}=-{\frac {n_{s}e^{2}}{m}}\mathbf {A} .}  [{\displaystyle
      \mathbf {j} _{s}=-{\frac {n_{s}e^{2}}{m}}\mathbf {A} .}]
The last equation suffers from only the disadvantage that it is not gauge
invariant, but is true only in the Coulomb_gauge, where the divergence of A is
zero.[8] This equation holds for magnetic fields that vary slowly in space.[4]
***** London penetration depth[edit] *****
If the second of London's equations is manipulated by applying Ampere's_law,[9]
         &#x2207; &#x00D7;  B  =  &#x03BC;  0    j    {\displaystyle \nabla
      \times \mathbf {B} =\mu _{0}\mathbf {j} }  [{\displaystyle \nabla \times
      \mathbf {B} =\mu _{0}\mathbf {j} }],
then the result is the differential equation
          &#x2207;  2    B  =   1  &#x03BB;  2      B  ,  &#x03BB; &#x2261;
      m   &#x03BC;  0    n  s    e  2       .   {\displaystyle \nabla ^
      {2}\mathbf {B} ={\frac {1}{\lambda ^{2}}}\mathbf {B} ,\qquad \lambda
      \equiv {\sqrt {\frac {m}{\mu _{0}n_{s}e^{2}}}}.}  [{\displaystyle \nabla
      ^{2}\mathbf {B} ={\frac {1}{\lambda ^{2}}}\mathbf {B} ,\qquad \lambda
      \equiv {\sqrt {\frac {m}{\mu _{0}n_{s}e^{2}}}}.}]
Thus, the London equations imply a characteristic length scale,     &#x03BB;
{\displaystyle \lambda }  [\lambda ], over which external magnetic fields are
exponentially suppressed. This value is the London_penetration_depth.
For an example, consider a superconductor within free space where the magnetic
field outside the superconductor is a constant value pointed parallel to the
superconducting boundary plane in the z direction. If x leads perpendicular to
the boundary then the solution inside the superconductor may be shown to be
          B  z   ( x ) =  B  0    e  &#x2212; x  /  &#x03BB;   .
      {\displaystyle B_{z}(x)=B_{0}e^{-x/\lambda }.\,}  [B_{z}(x)=B_{0}e^{{-x/
      \lambda }}.\,]
From here the physical meaning of the London penetration depth can perhaps most
easily be discerned.
***** Rationale for the London equations[edit] *****
**** Original arguments[edit] ****
While it is important to note that the above equations cannot be formally
derived,[10] the Londons did follow a certain intuitive logic in the
formulation of their theory. Substances across a stunningly wide range of
composition behave roughly according to Ohm's law, which states that current is
proportional to electric field. However, such a linear relationship is
impossible in a superconductor for, almost by definition, the electrons in a
superconductor flow with no resistance whatsoever. To this end, the London
brothers imagined electrons as if they were free electrons under the influence
of a uniform external electric field. According to the Lorentz_force_law
          F  = e  E  + e  v  &#x00D7;  B    {\displaystyle \mathbf {F}
      =e\mathbf {E} +e\mathbf {v} \times \mathbf {B} }  [{\displaystyle \mathbf
      {F} =e\mathbf {E} +e\mathbf {v} \times \mathbf {B} }]
these electrons should encounter a uniform force, and thus they should in fact
accelerate uniformly. This is precisely what the first London equation states.
To obtain the second equation, take the curl of the first London equation and
apply Faraday's_law,
         &#x2207; &#x00D7;  E  = &#x2212;    &#x2202;  B    &#x2202; t
      {\displaystyle \nabla \times \mathbf {E} =-{\frac {\partial \mathbf {B} }
      {\partial t}}}  [\nabla \times \mathbf {E} =-{\frac {\partial \mathbf {B}
      }{\partial t}}],
to obtain
           &#x2202;  &#x2202; t     (  &#x2207; &#x00D7;   j   s   +     n  s
      e  2    m    B   )  = 0.   {\displaystyle {\frac {\partial }{\partial
      t}}\left(\nabla \times \mathbf {j} _{s}+{\frac {n_{s}e^{2}}{m}}\mathbf
      {B} \right)=0.}  [{\displaystyle {\frac {\partial }{\partial t}}\left
      (\nabla \times \mathbf {j} _{s}+{\frac {n_{s}e^{2}}{m}}\mathbf {B}
      \right)=0.}]
As it currently stands, this equation permits both constant and exponentially
decaying solutions. The Londons recognized from the Meissner effect that
constant nonzero solutions were nonphysical, and thus postulated that not only
was the time derivative of the above expression equal to zero, but also that
the expression in the parentheses must be identically zero. This results in the
second London equation.
**** Canonical momentum arguments[edit] ****
It is also possible to justify the London equations by other means.[11][12]
Current density is defined according to the equation
           j   s   = &#x2212;  n  s   e  v  .   {\displaystyle \mathbf {j} _
      {s}=-n_{s}e\mathbf {v} .}  [{\displaystyle \mathbf {j} _{s}=-n_
      {s}e\mathbf {v} .}]
Taking this expression from a classical description to a quantum mechanical
one, we must replace values j and v by the expectation values of their
operators. The velocity operator
          v  =   1 m    (   p  + e  A   )    {\displaystyle \mathbf {v} ={\frac
      {1}{m}}\left(\mathbf {p} +e\mathbf {A} \right)}  [{\displaystyle \mathbf
      {v} ={\frac {1}{m}}\left(\mathbf {p} +e\mathbf {A} \right)}]
is defined by dividing the gauge-invariant, kinematic momentum operator by the
particle mass m. [13] Note we are using     &#x2212; e   {\displaystyle -e}  [-
e] as the electron charge. We may then make this replacement in the equation
above. However, an important assumption from the microscopic_theory_of
superconductivity is that the superconducting state of a system is the ground
state, and according to a theorem of Bloch's,[10] in such a state the canonical
momentum p is zero. This leaves
           j   s   = &#x2212;     n  s    e  2    m    A  ,   {\displaystyle
      \mathbf {j} _{s}=-{\frac {n_{s}e^{2}}{m}}\mathbf {A} ,}  [{\displaystyle
      \mathbf {j} _{s}=-{\frac {n_{s}e^{2}}{m}}\mathbf {A} ,}]
which is the London equation according to the second formulation above.
***** References[edit] *****
   1. ^London,_F.; London,_H. (1935). "The Electromagnetic Equations of the
      Supraconductor". Proceedings of the Royal Society A: Mathematical,
      Physical and Engineering Sciences. 149 (866): 71. Bibcode:
      1935RSPSA.149...71L. doi:10.1098/rspa.1935.0048.
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
   3. ^ Michael Tinkham (1996). Introduction to Superconductivity. McGraw-Hill.
      ISBN 0-07-064878-6.
   4. ^Neil_Ashcroft; David_Mermin (1976). Solid State Physics. Saunders
      College. p. 738. ISBN 0-03-083993-9.
   5. ^ a bCharles Kittel (2005). Introduction_to_Solid_State_Physics (8th
      ed.). Wiley. ISBN 0-471-41526-X.
   6. ^Meissner, W.; R. Ochsenfeld (1933). "Ein neuer Effekt bei Eintritt der
      SupraleitfÃ¤higkeit". Naturwissenschaften. 21 (44): 787. Bibcode:
      1933NW.....21..787M. doi:10.1007/BF01504252.
   7. ^ a bJames F. Annett (2004). Superconductivity, Superfluids and
      Condensates. Oxford. p. 58. ISBN 0-19-850756-9.
   8. ^John David Jackson (1999). Classical Electrodynamics. John Wiley & Sons.
      p. 604. ISBN 0-19-850756-9.
   9. ^ Michael Tinkham (1996). Introduction to Superconductivity. McGraw-Hill.
      p. 6. ISBN 0-07-064878-6.
  10. ^ (The displacement is ignored because it is assumed that electric field
      only varies slowly with respect to time, and the term is already
      suppressed by a factor of c.)
  11. ^ a bMichael Tinkham (1996). Introduction to Superconductivity. McGraw-
      Hill. p. 5. ISBN 0-07-064878-6.
  12. ^John David Jackson (1999). Classical Electrodynamics. John Wiley & Sons.
      pp. 603â604. ISBN 0-19-850756-9.
  13. ^Michael Tinkham (1996). Introduction to Superconductivity. McGraw-Hill.
      pp. 5â6. ISBN 0-07-064878-6.
  14. ^L. D. Landau and E. M. Lifshitz (1977). Quantum Mechanics- Non-
      relativistic Theory. Butterworth-Heinemann. pp. 455â458. ISBN 0-7506-
      3539-8.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=London_equations&oldid=865643627"
Categories:
    * Superconductivity
    * Equations
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
    * Deutsch
    * ÙØ§Ø±Ø³Û
    * íêµ­ì´
    * Italiano
    * æ¥æ¬èª
    * Norsk
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 25 October 2018, at 07:16 (UTC).
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
