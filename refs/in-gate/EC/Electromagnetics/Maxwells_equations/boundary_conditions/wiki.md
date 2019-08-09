The following text has been accessed from https://en.wikipedia.org/wiki/Boundary_value_problem at Fri Aug 9 03:43:23 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Boundary value problem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Shows a region where a differential_equation is valid and the associated
boundary values
In mathematics, in the field of differential_equations, a boundary value
problem is a differential equation together with a set of additional
constraints, called the boundary conditions.[1] A solution to a boundary value
problem is a solution to the differential equation which also satisfies the
boundary conditions.
Boundary value problems arise in several branches of physics as any physical
differential equation will have them. Problems involving the wave_equation,
such as the determination of normal_modes, are often stated as boundary value
problems. A large class of important boundary value problems are the
SturmâLiouville_problems. The analysis of these problems involves the
eigenfunctions of a differential_operator.
To be useful in applications, a boundary value problem should be well_posed.
This means that given the input to the problem there exists a unique solution,
which depends continuously on the input. Much theoretical work in the field of
partial_differential_equations is devoted to proving that boundary value
problems arising from scientific and engineering applications are in fact well-
posed.
Among the earliest boundary value problems to be studied is the Dirichlet
problem, of finding the harmonic_functions (solutions to Laplace's_equation);
the solution was given by the Dirichlet's_principle.
⁰
***** Contents *****
    * 1_Explanation
    * 2_Types_of_boundary_value_problems
          o 2.1_Boundary_value_conditions
                # 2.1.1_Examples
          o 2.2_Differential_operators
    * 3_Applications
          o 3.1_Electromagnetic_potential
    * 4_See_also
    * 5_Notes
    * 6_References
    * 7_External_links
***** Explanation[edit] *****
Boundary value problems are similar to initial_value_problems. A boundary value
problem has conditions specified at the extremes ("boundaries") of the
independent variable in the equation whereas an initial value problem has all
of the conditions specified at the same value of the independent variable (and
that value is at the lower boundary of the domain, thus the term "initial"
value). A boundary value is a data value that corresponds to a minimum or
maximum input, internal, or output value specified for a system or component.
[2]
For example, if the independent variable is time over the domain [0,1], a
boundary value problem would specify values for     y ( t )   {\displaystyle y
(t)}  [y(t)] at both     t = 0   {\displaystyle t=0}  [t=0] and     t = 1
{\displaystyle t=1}  [t=1], whereas an initial value problem would specify a
value of     y ( t )   {\displaystyle y(t)}  [y(t)] and      y &#x2032;  ( t )
{\displaystyle y'(t)}  [y'(t)] at time     t = 0   {\displaystyle t=0}  [t=0].
Finding the temperature at all points of an iron bar with one end kept at
absolute_zero and the other end at the freezing point of water would be a
boundary value problem.
If the problem is dependent on both space and time, one could specify the value
of the problem at a given point for all time or at a given time for all space.
Concretely, an example of a boundary value (in one spatial dimension) is the
problem
          y &#x2033;  ( x ) + y ( x ) = 0   {\displaystyle y''(x)+y(x)=0}  [
      {\displaystyle y''(x)+y(x)=0}]
to be solved for the unknown function     y ( x )   {\displaystyle y(x)}  [y
(x)] with the boundary conditions
         y ( 0 ) = 0 , &#xA0; y ( &#x03C0;  /  2 ) = 2.   {\displaystyle y
      (0)=0,\ y(\pi /2)=2.}  [y(0)=0,\ y(\pi /2)=2.]
Without the boundary conditions, the general solution to this equation is
         y ( x ) = A sin &#x2061; ( x ) + B cos &#x2061; ( x ) .
      {\displaystyle y(x)=A\sin(x)+B\cos(x).}  [{\displaystyle y(x)=A\sin
      (x)+B\cos(x).}]
From the boundary condition     y ( 0 ) = 0   {\displaystyle y(0)=0}  [y(0)=0]
one obtains
         0 = A &#x22C5; 0 + B &#x22C5; 1   {\displaystyle 0=A\cdot 0+B\cdot 1}
      [0=A\cdot 0+B\cdot 1]
which implies that     B = 0.   {\displaystyle B=0.}  [B=0.] From the boundary
condition     y ( &#x03C0;  /  2 ) = 2   {\displaystyle y(\pi /2)=2}  [y(\pi /
2)=2] one finds
         2 = A &#x22C5; 1   {\displaystyle 2=A\cdot 1}  [2=A\cdot 1]
and so     A = 2.   {\displaystyle A=2.}  [A=2.] One sees that imposing
boundary conditions allowed one to determine a unique solution, which in this
case is
         y ( x ) = 2 sin &#x2061; ( x ) .   {\displaystyle y(x)=2\sin(x).}  [
      {\displaystyle y(x)=2\sin(x).}]
***** Types of boundary value problems[edit] *****
**** Boundary value conditions[edit] ****
Finding a function to describe the temperature of this idealised 2D rod is a
boundary value problem with Dirichlet_boundary_conditions. Any solution
function will both solve the heat_equation, and fulfill the boundary conditions
of a temperature of 0 K on the left boundary and a temperature of 273.15 K on
the right boundary.
A boundary condition which specifies the value of the function itself is a
Dirichlet_boundary_condition, or first-type boundary condition. For example, if
one end of an iron rod is held at absolute zero, then the value of the problem
would be known at that point in space.
A boundary condition which specifies the value of the normal_derivative of the
function is a Neumann_boundary_condition, or second-type boundary condition.
For example, if there is a heater at one end of an iron rod, then energy would
be added at a constant rate but the actual temperature would not be known.
If the boundary has the form of a curve or surface that gives a value to the
normal derivative and the variable itself then it is a Cauchy_boundary
condition.
*** Examples[edit] ***
Summary of boundary conditions for the unknown function,     y   {\displaystyle
y}  [y], constants      c  0     {\displaystyle c_{0}}  [c_{0}] and      c  1
{\displaystyle c_{1}}  [c_{1}] specified by the boundary conditions, and known
scalar functions     f   {\displaystyle f}  [f] and     g   {\displaystyle g}
[g] specified by the boundary conditions.
Name      Form on 1st part of boundary     Form on 2nd part of boundary
Dirichlet    y = f   {\displaystyle y=f}  [y=f]
Neumann         &#x2202; y   &#x2202; n    = f   {\displaystyle {\partial y
          \over \partial n}=f}  [{\partial y \over \partial n}=f]
              c  0   y +  c  1      &#x2202; y   &#x2202; n    = f
Robin     {\displaystyle c_{0}y+c_{1}{\partial y \over \partial n}=f}  [c_
          {0}y+c_{1}{\partial y \over \partial n}=f]
                                               c  0   y +  c  1      &#x2202; y
             y = f   {\displaystyle y=f}   &#x2202; n    = f   {\displaystyle
Mixed     [y=f]                            c_{0}y+c_{1}{\partial y \over
                                           \partial n}=f}  [c_{0}y+c_{1}
                                           {\partial y \over \partial n}=f]
          both     y = f   {\displaystyle y=f}  [y=f], and      c  0
Cauchy    &#x2202; y   &#x2202; n    = g   {\displaystyle c_{0}{\partial y
          \over \partial n}=g}  [{\displaystyle c_{0}{\partial y \over \partial
          n}=g}]
**** Differential operators[edit] ****
Aside from the boundary condition, boundary value problems are also classified
according to the type of differential operator involved. For an elliptic
operator, one discusses elliptic_boundary_value_problems. For a hyperbolic
operator, one discusses hyperbolic_boundary_value_problems. These categories
are further subdivided into linear and various nonlinear types.
***** Applications[edit] *****
**** Electromagnetic potential[edit] ****
See also: Laplace's_equation_Â§ Boundary_conditions
In electrostatics, a common problem is to find a function which describes the
electric_potential of a given region. If the region does not contain charge,
the potential must be a solution to Laplace's_equation (a so-called harmonic
function). The boundary conditions in this case are the Interface_conditions
for_electromagnetic_fields. If there is no current_density in the region, it is
also possible to define a magnetic_scalar_potential using a similar procedure.
***** See also[edit] *****
Related mathematics:           Physical applications:
    * Initial_value_problem        * Waves              Numerical algorithms:
    * Green's_function             * Normal_mode            * Shooting_method
    * Stochastic_processes_and     * Electrostatics         * Direct_multiple
      boundary_value_problems      * Potential_theory         shooting_method
    * Sturm–Liouville_theory     * Computation_of         * Walk-on-spheres
    * Sommerfeld_radiation           radiowave                method
      condition                      attenuation_in_the     * Finite_Difference
    * Perfect_thermal_contact        atmosphere               Method
      condition                    * Black_hole
***** Notes[edit] *****
   1. ^Daniel Zwillinger (12 May 2014). Handbook_of_Differential_Equations.
      Elsevier Science. pp. 536â. ISBN 978-1-4832-2096-3.
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
   3. ^ISO/IEC/IEEE International Standard - Systems and software engineering.
      ISO/IEC/IEEE 24765:2010(E). pp. vol., no., pp.1â418.
***** References[edit] *****
    * A. D. Polyanin and V. F. Zaitsev, Handbook of Exact Solutions for
      Ordinary Differential Equations (2nd edition), Chapman & Hall/CRC Press,
      Boca Raton, 2003.
ISBN 1-58488-297-2.
A. D. Polyanin, Handbook of Linear Partial Differential Equations for Engineers
and Scientists, Chapman & Hall/CRC Press, Boca Raton, 2002.
ISBN 1-58488-299-9.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Boundary_value_problems_in
      potential_theory", Encyclopedia_of_Mathematics, Springer Science+Business
      Media B.V. / Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Hazewinkel,_Michiel, ed. (2001) [1994], "Boundary_value_problem,_complex-
variable_methods", Encyclopedia_of_Mathematics, Springer Science+Business Media
B.V. / Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Linear_Partial_Differential_Equations:_Exact_Solutions_and_Boundary_Value
Problems at EqWorld: The World of Mathematical Equations.
"Boundary_value_problem". Scholarpedia.
                                              * BNF: cb11942188p (data)
                                              * GND: 4048395-2
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85016102
                                              * NDL: 00567211
                                              * SUDOC: 027364100

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Boundary_value_problem&oldid=906978959"
Categories:
    * Ordinary_differential_equations
    * Partial_differential_equations
    * Boundary_conditions
    * Mathematical_problems
Hidden categories:
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
    * Wikipedia_articles_with_SUDOC_identifiers
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ×¢××¨××ª
    * Magyar
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 19 July 2019, at 16:23 (UTC).
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
