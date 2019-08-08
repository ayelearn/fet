The following text has been accessed from https://en.wikipedia.org/wiki/Conservation_law at Thu Aug 8 23:16:26 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Conservation law ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about conservation in physics. For the legal aspects of
environmental conservation, see Environmental_law and Conservation_movement.
For other uses, see Conservation_(disambiguation).
In physics, a conservation law states that a particular measurable property of
an isolated physical_system does not change as the system evolves over time.
Exact conservation laws include conservation_of_energy, conservation_of_linear
momentum, conservation_of_angular_momentum, and conservation_of_electric
charge. There are also many approximate conservation laws, which apply to such
quantities as mass, parity, lepton_number, baryon_number, strangeness,
hypercharge, etc. These quantities are conserved in certain classes of physics
processes, but not in all.
A local conservation law is usually expressed mathematically as a continuity
equation, a partial_differential_equation which gives a relation between the
amount of the quantity and the "transport" of that quantity. It states that the
amount of the conserved quantity at a point or within a volume can only change
by the amount of the quantity which flows in or out of the volume.
From Noether's_theorem, each conservation law is associated with a symmetry in
the underlying physics.
⁰
***** Contents *****
    * 1_Conservation_laws_as_fundamental_laws_of_nature
    * 2_Exact_laws
    * 3_Approximate_laws
    * 4_Global_and_local_conservation_laws
    * 5_Differential_forms
    * 6_Integral_and_weak_forms
    * 7_See_also
          o 7.1_Examples_and_applications
    * 8_Notes
    * 9_References
    * 10_External_links
***** Conservation laws as fundamental laws of nature[edit] *****
Conservation laws are fundamental to our understanding of the physical world,
in that they describe which processes can or cannot occur in nature. For
example, the conservation law of energy states that the total quantity of
energy in an isolated system does not change, though it may change form. In
general, the total quantity of the property governed by that law remains
unchanged during physical processes. With respect to classical physics,
conservation laws include conservation of energy, mass (or matter), linear
momentum, angular momentum, and electric charge. With respect to particle
physics, particles cannot be created or destroyed except in pairs, where one is
ordinary and the other is an antiparticle. With respect to symmetries and
invariance principles, three special conservation laws have been described,
associated with inversion or reversal of space, time, and charge.
Conservation laws are considered to be fundamental laws of nature, with broad
application in physics, as well as in other fields such as chemistry, biology,
geology, and engineering.
Most conservation laws are exact, or absolute, in the sense that they apply to
all possible processes. Some conservation laws are partial, in that they hold
for some processes but not for others.
One particularly important result concerning conservation laws is Noether's
theorem, which states that there is a one-to-one correspondence between each
one of them and a differentiable symmetry of nature. For example, the
conservation of energy follows from the time-invariance of physical systems,
and the conservation of angular momentum arises from the fact that physical
systems behave the same regardless of how they are oriented in space.
***** Exact laws[edit] *****
A partial listing of physical conservation equations due_to_symmetry that are
said to be exact laws, or more precisely have never been proven to be violated:
Conservation Respective Noether     Number of dimensions
Law          symmetry invariance
Conservation Time
of_mass-     invariance             1         translation about time axis
energy
Conservation Translation
of_linear    symmetry               3         translation about x,y,z position
momentum
Conservation Rotation    Lorentz
of_angular   invariance  invariance 3         rotation about x,y,z axes
momentum                 symmetry
CPT_symmetry
(combining
charge       Lorentz                          (charge inversion q â âq) + (position inversion r â âr) + 
conjugation, invariance             1 + 1 +(time inversion t â ât)
parity and
time
reversal)
Conservation
of_electric  Gauge_invariance       1â4  scalar field (1D) in 4D spacetime (x,y,z + time evolution)
charge
Conservation
of color     SU(3) Gauge_invariance 3         r,g,b
charge
Conservation SU(2)L Gauge
of weak      invariance             1         weak charge
isospin
Conservation Probability invariance
of           [1]                    1 â�total probability always = 1 in whole x,y,z space, during time evolution
probability
***** Approximate laws[edit] *****
There are also approximate conservation laws. These are approximately true in
particular situations, such as low speeds, short time scales, or certain
interactions.
    * Conservation_of_rest_mass
    * Conservation of baryon_number (See chiral_anomaly and sphaleron)
    * Conservation of lepton_number (In the Standard_Model)
    * Conservation of flavor (violated by the weak_interaction)
    * Conservation of parity
    * Invariance under charge_conjugation
    * Invariance under time_reversal
    * CP_symmetry, the combination of charge conjugation and parity (equivalent
      to time reversal if CPT holds)
***** Global and local conservation laws[edit] *****
The total amount of some conserved quantity in the universe could remain
unchanged if an equal amount were to appear at one point A and simultaneously
disappear from another separate point B. For example, an amount of energy could
appear on Earth without changing the total amount in the Universe if the same
amount of energy were to disappear from a remote region of the Universe. This
weak form of "global" conservation is really not a conservation law because it
is not Lorentz_invariant, so phenomena like the above do not occur in nature.
[2][3] Due to special_relativity, if the appearance of the energy at A and
disappearance of the energy at B are simultaneous in one inertial_reference
frame, they will not be simultaneous in other inertial reference frames moving
with respect to the first. In a moving frame one will occur before the other;
either the energy at A will appear before or after the energy at B disappears.
In both cases, during the interval energy will not be conserved.
A stronger form of conservation law requires that, for the amount of a
conserved quantity at a point to change, there must be a flow, or flux of the
quantity into or out of the point. For example, the amount of electric_charge
in a volume is never found to change without an electric_current into or out of
the volume that carries the difference in charge. Since it only involves
continuous local changes, this stronger type of conservation law is Lorentz
invariant; a quantity conserved in one reference frame is conserved in all
moving reference frames.[2][3] This is called a local conservation law.[2][3]
Local conservation also implies global conservation; that the total amount of
the conserved quantity in the Universe remains constant. All of the
conservation laws listed above are local conservation laws. A local
conservation law is expressed mathematically by a continuity_equation, which
states that the change in the quantity in a volume is equal to the total net
"flux" of the quantity through the surface of the volume. The following
sections discuss continuity equations in general.
***** Differential forms[edit] *****
See also: conservation_form and continuity_equation
In continuum mechanics, the most general form of an exact conservation law is
given by a continuity_equation. For example, conservation of electric charge q
is
            &#x2202; &#x03C1;   &#x2202; t    = &#x2212; &#x2207; &#x22C5;  j
      {\displaystyle {\frac {\partial \rho }{\partial t}}=-\nabla \cdot \mathbf
      {j} \,}  [{\frac  {\partial \rho }{\partial t}}=-\nabla \cdot {\mathbf
      {j}}\,]
where ââ is the divergence operator, Ï is the density of q (amount per
unit volume), j is the flux of q (amount crossing a unit area in unit time),
and t is time.
If we assume that the motion u of the charge is a continuous function of
position and time, then
          j  = &#x03C1;  u    {\displaystyle \mathbf {j} =\rho \mathbf {u} }  [
      {\mathbf  {j}}=\rho {\mathbf  {u}}]
            &#x2202; &#x03C1;   &#x2202; t    = &#x2212; &#x2207; &#x22C5;
      ( &#x03C1;  u  )  .   {\displaystyle {\frac {\partial \rho }{\partial
      t}}=-\nabla \cdot (\rho \mathbf {u} )\,.}  [{\frac  {\partial \rho }
      {\partial t}}=-\nabla \cdot (\rho {\mathbf  {u}})\,.]
In one space dimension this can be put into the form of a homogeneous first-
order quasilinear hyperbolic_equation:[4]
          y  t   + A ( y )  y  x   = 0   {\displaystyle y_{t}+A(y)y_{x}=0}  [y_
      {t}+A(y)y_{x}=0]
where the dependent variable y is called the density of a conserved quantity,
and A(y) is called the current_jacobian, and the subscript_notation_for_partial
derivatives has been employed. The more general inhomogeneous case:
          y  t   + A ( y )  y  x   = s   {\displaystyle y_{t}+A(y)y_{x}=s}  [y_
      {t}+A(y)y_{x}=s]
is not a conservation equation but the general kind of balance_equation
describing a dissipative_system. The dependent variable y is called a
nonconserved quantity, and the inhomogeneous term s(y,x,t) is the-source, or
dissipation. For example, balance equations of this kind are the momentum and
energy Navier-Stokes_equations, or the entropy_balance for a general isolated
system.
In the one-dimensional space a conservation equation is a first-order
quasilinear hyperbolic_equation that can be put into the advection form:
          y  t   + a ( y )  y  x   = 0   {\displaystyle y_{t}+a(y)y_{x}=0}  [y_
      {t}+a(y)y_{x}=0]
where the dependent variable y(x,t) is called the density of the conserved
(scalar) quantity (c.q.(d.) = conserved quantity (density)), and a(y) is called
the current coefficient, usually corresponding to the partial_derivative in the
conserved quantity of a current_density (c.d.) of the conserved quantity j(y):
[4]
         a ( y ) =  j  y   ( y )   {\displaystyle a(y)=j_{y}(y)}  [a(y)=j_{y}
      (y)]
In this case since the chain_rule applies:
          j  x   =  j  y   ( y )  y  x   = a ( y )  y  x     {\displaystyle j_
      {x}=j_{y}(y)y_{x}=a(y)y_{x}}  [j_{x}=j_{y}(y)y_{x}=a(y)y_{x}]
the conservation equation can be put into the current density form:
          y  t   +  j  x   ( y ) = 0   {\displaystyle y_{t}+j_{x}(y)=0}  [y_
      {t}+j_{x}(y)=0]
In a space with more than one dimension the former definition can be extended
to an equation that can be put into the form:
          y  t   +  a  ( y ) &#x22C5; &#x2207; y = 0   {\displaystyle y_
      {t}+\mathbf {a} (y)\cdot \nabla y=0}  [y_{t}+{\mathbf  a}(y)\cdot \nabla
      y=0]
where the conserved quantity is y(r,t),    &#x22C5;   {\displaystyle \cdot }
[\cdot ] denotes the scalar_product, ∇ is the nabla operator, here indicating a
gradient, and a(y) is a vector of current coefficients, analogously
corresponding to the divergence of a vector c.d. associated to the c.q. j(y):
          y  t   + &#x2207; &#x22C5;  j  ( y ) = 0   {\displaystyle y_
      {t}+\nabla \cdot \mathbf {j} (y)=0}  [y_{t}+\nabla \cdot {\mathbf  j}
      (y)=0]
This is the case for the continuity_equation:
          &#x03C1;  t   + &#x2207; &#x22C5; ( &#x03C1;  u  ) = 0
      {\displaystyle \rho _{t}+\nabla \cdot (\rho \mathbf {u} )=0}  [\rho _
      {t}+\nabla \cdot (\rho {\mathbf  u})=0]
Here the conserved quantity is the mass, with density ρ(r,t) and current
density ρu, identical to the momentum_density, while u(r,t) is the flow
velocity.
In the general case a conservation equation can be also a system of this kind
of equations (a vector_equation) in the form:[4]
           y   t   +  A  (  y  ) &#x22C5; &#x2207;  y  =  0    {\displaystyle
      \mathbf {y} _{t}+\mathbf {A} (\mathbf {y} )\cdot \nabla \mathbf {y}
      =\mathbf {0} }  [{\mathbf  y}_{t}+{\mathbf  A}({\mathbf  y})\cdot \nabla
      {\mathbf  y}={\mathbf  0}]
where y is called the conserved (vector) quantity, ∇ y is its gradient, 0 is
the zero_vector, and A(y) is called the Jacobian of the current density. In
fact as in the former scalar case, also in the vector case A(y) usually
corresponding to the Jacobian of a current_density_matrix J(y):
          A  (  y  ) =   J    y    (  y  )   {\displaystyle \mathbf {A}
      (\mathbf {y} )=\mathbf {J} _{\mathbf {y} }(\mathbf {y} )}  [{\mathbf  A}(
      {\mathbf  y})={\mathbf  J}_{{{\mathbf  y}}}({\mathbf  y})]
and the conservation equation can be put into the form:
           y   t   + &#x2207; &#x22C5;  J  (  y  ) =  0    {\displaystyle
      \mathbf {y} _{t}+\nabla \cdot \mathbf {J} (\mathbf {y} )=\mathbf {0} }  [
      {\mathbf  y}_{t}+\nabla \cdot {\mathbf  J}({\mathbf  y})={\mathbf  0}]
For example, this the case for Euler equations (fluid dynamics). In the simple
incompressible case they are:
             &#x2207; &#x22C5;  u  = 0        &#x2202;  u    &#x2202; t    +  u
      &#x22C5; &#x2207;  u  + &#x2207; s =  0  ,       {\displaystyle {\begin
      {aligned}\nabla \cdot \mathbf {u} =0\\[1.2ex]{\partial \mathbf {u} \over
      \partial t}+\mathbf {u} \cdot \nabla \mathbf {u} +\nabla s=\mathbf {0}
      ,\end{aligned}}}  [{\displaystyle {\begin{aligned}\nabla \cdot \mathbf
      {u} =0\\[1.2ex]{\partial \mathbf {u}  \over \partial t}+\mathbf {u} \cdot
      \nabla \mathbf {u} +\nabla s=\mathbf {0} ,\end{aligned}}}]
where:
    * u is the flow_velocity vector, with components in a N-dimensional space
      u1, u2 ... uN,
    * s is the specific pressure (pressure per unit density) giving the source
      term,
See also: Euler_equations_(fluid_dynamics)
It can be shown that the conserved (vector) quantity and the c.d. matrix for
these equations are respectively:
           y   =   (    1      u     )   ;    J   =   (     u       u  &#x2297;
      u  + s  I     )   ;    {\displaystyle {\mathbf {y} }={\begin
      {pmatrix}1\\\mathbf {u} \end{pmatrix}};\qquad {\mathbf {J} }={\begin
      {pmatrix}\mathbf {u} \\\mathbf {u} \otimes \mathbf {u} +s\mathbf {I} \end
      {pmatrix}};\qquad }  [{\displaystyle {\mathbf {y} }={\begin
      {pmatrix}1\\\mathbf {u} \end{pmatrix}};\qquad {\mathbf {J} }={\begin
      {pmatrix}\mathbf {u} \\\mathbf {u} \otimes \mathbf {u} +s\mathbf {I} \end
      {pmatrix}};\qquad }]
where    &#x2297;   {\displaystyle \otimes }  [\otimes ] denotes the outer
product.
***** Integral and weak forms[edit] *****
Conservation equations can be also expressed in integral form: the advantage of
the latter is substantially that it requires less smoothness of the solution,
which paves the way to weak_form, extending the class of admissible solutions
to include discontinuous solutions.[5] By integrating in any space-time domain
the current density form in 1-D space:
          y  t   +  j  x   ( y ) = 0   {\displaystyle y_{t}+j_{x}(y)=0}  [y_
      {t}+j_{x}(y)=0]
and by using Green's_theorem, the integral form is:
          &#x222B;  &#x2212; &#x221E;   &#x221E;   y  d x +  &#x222B;  0
      &#x221E;   j ( y )  d t = 0   {\displaystyle \int _{-\infty }^{\infty
      }y\,dx+\int _{0}^{\infty }j(y)\,dt=0}  [{\displaystyle \int _{-\infty }^
      {\infty }y\,dx+\int _{0}^{\infty }j(y)\,dt=0}]
In a similar fashion, for the scalar multidimensional space, the integral form
is:
            &#x222E;      &#x2061; [ y   d  N   r + j ( y )  d t ] = 0
      {\displaystyle \oint [y\,d^{N}r+j(y)\,dt]=0}  [{\displaystyle \oint
      [y\,d^{N}r+j(y)\,dt]=0}]
where the line integration is performed along the boundary of the domain, in an
anticlock-wise manner.[5]
Moreover, by defining a test_function φ(r,t) continuously differentiable both
in time and space with compact support, the weak_form can be obtained pivoting
on the initial_condition. In 1-D space it is:
          &#x222B;  0   &#x221E;    &#x222B;  &#x2212; &#x221E;   &#x221E;
      &#x03D5;  t   y +  &#x03D5;  x   j ( y )  d x  d t = &#x2212;  &#x222B;
      &#x2212; &#x221E;   &#x221E;   &#x03D5; ( x , 0 ) y ( x , 0 )  d x
      {\displaystyle \int _{0}^{\infty }\int _{-\infty }^{\infty }\phi _
      {t}y+\phi _{x}j(y)\,dx\,dt=-\int _{-\infty }^{\infty }\phi (x,0)y
      (x,0)\,dx}  [{\displaystyle \int _{0}^{\infty }\int _{-\infty }^{\infty
      }\phi _{t}y+\phi _{x}j(y)\,dx\,dt=-\int _{-\infty }^{\infty }\phi (x,0)y
      (x,0)\,dx}]
Note that in the weak form all the partial derivatives of the density and
current density have been passed on to the test function, which with the former
hypothesis is sufficiently smooth to admit these derivatives.[5]
***** See also[edit] *****
    * Invariant_(physics)
    * Conserved_quantity
          o Some kinds of helicity are conserved in dissipationless limit:
            hydrodynamical_helicity, magnetic_helicity, cross-helicity.
    * Conservation_law of the Stressâenergy_tensor
    * Riemann_invariant
    * Philosophy_of_physics
    * Totalitarian_principle
    * Convectionâdiffusion_equation
**** Examples and applications[edit] ****
    * Advection
    * Mass_conservation, or Continuity_equation
    * Charge_conservation
    * Euler_equations_(fluid_dynamics)
    * inviscid Burgers_equation
    * Kinematic_wave
    * Conservation_of_energy
    * Traffic_flow
***** Notes[edit] *****
   1. ^"The_gauge-invariance_of_the_probability_current". Physics Stack
      Exchange. Archived from the original on 18 August 2017. Retrieved 4 May
      2018.
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
   3. ^ a b cAitchison, Ian J. R.; Hey, Anthony J.G. (2012). Gauge_Theories_in
      Particle_Physics:_A_Practical_Introduction:_From_Relativistic_Quantum
      Mechanics_to_QED,_Fourth_Edition,_Vol._1. CRC Press. p. 43. ISBN 978-
      1466512993. Archived from the original on 2018-05-04.
   4. ^ a b cWill, Clifford M. (1993). Theory_and_Experiment_in_Gravitational
      Physics. Cambridge Univ. Press. p. 105. ISBN 978-0521439732. Archived
      from the original on 2017-02-20.
   5. ^ a b c see Toro, p.43
   6. ^ a b c see Toro, p.62-63
***** References[edit] *****
    * Philipson, Schuster, Modeling by Nonlinear Differential Equations:
      Dissipative and Conservative Processes, World Scientific Publishing
      Company 2009.
    * Victor_J._Stenger, 2000. Timeless Reality: Symmetry, Simplicity, and
      Multiple Universes. Buffalo NY: Prometheus Books. Chpt. 12 is a gentle
      introduction to symmetry, invariance, and conservation laws.
    * Toro, E.F. (1999). "Chapter 2. Notions on Hyperbolic PDEs". Riemann
      Solvers and Numerical Methods for Fluid Dynamics. Springer-Verlag.
      ISBN 978-3-540-65966-2.
E. Godlewski and P.A. Raviart, Hyperbolic systems of conservation laws,
Ellipses, 1991.
***** External links[edit] *****
    * Conservation_Laws â Ch. 11-15 in an online textbook

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Conservation_law&oldid=908498692"
Categories:
    * Symmetry
    * Conservation_laws
    * Concepts_in_physics
    * Physical_systems
    * Scientific_laws
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 30 July 2019, at 03:26 (UTC).
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
