The following text has been accessed from https://en.wikipedia.org/wiki/Steady_state_(chemistry) at Fri Aug 9 02:05:00 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Steady state (chemistry) ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other uses, see Steady_state_(disambiguation).
In chemistry, a steady state is a situation in which all state_variables are
constant in spite of ongoing processes that strive to change them. For an
entire system to be at steady state, i.e. for all state variables of a system
to be constant, there must be a flow through the system (compare mass_balance).
A simple example of such a system is the case of a bathtub with the tap running
but with the drain unplugged: after a certain time, the water flows in and out
at the same rate, so the water level (the state variable Volume) stabilizes and
the system is in a steady state.
The steady state concept is different from chemical_equilibrium. Although both
may create a situation where a concentration does not change, in a system at
chemical equilibrium, the net reaction rate is zero (products transform into
reactants at the same rate as reactants transform into products), while no such
limitation exists in the steady state concept. Indeed, there does not have to
be a reaction at all for a steady state to develop.
The term steady state is also used to describe a situation where some, but not
all, of the state variables of a system are constant. For such a steady state
to develop, the system does not have to be a flow system. Therefore, such a
steady state can develop in a closed system where a series of chemical
reactions take place. Literature in chemical_kinetics usually refers to this
case, calling it steady state approximation.
In simple systems the steady state is approached by state variables gradually
decreasing or increasing until they reach their steady state value. In more
complex systems state variable might fluctuate around the theoretical steady
state either forever (a limit_cycle) or gradually coming closer and closer. It
theoretically takes an infinite time to reach steady state, just as it takes an
infinite time to reach chemical equilibrium.
Both concepts are, however, frequently used approximations because of the
substantial mathematical simplifications these concepts offer. Whether or not
these concepts can be used depends on the error the underlying assumptions
introduce. So, even though a steady state, from a theoretical point of view,
requires constant drivers (e.g. constant inflow rate and constant
concentrations in the inflow), the error introduced by assuming steady state
for a system with non-constant drivers may be negligible if the steady state is
approached fast enough (relatively speaking).
⁰
***** Contents *****
    * 1_Steady_state_approximation_in_chemical_kinetics
          o 1.1_Reaction_rates
          o 1.2_Analytical_solutions
          o 1.3_Steady_state
          o 1.4_Validity
    * 2_See_also
    * 3_Notes_and_references
    * 4_External_links
***** Steady state approximation in chemical kinetics[edit] *****
The steady state approximation,[1] occasionally called the stationary-state
approximation, involves setting the rate of change of a reaction_intermediate
in a reaction_mechanism equal to zero so that the kinetic equations can be
simplified by setting the rate of formation of the intermediate equal to the
rate of its destruction.
In practice it is sufficient that the rates of formation and destruction are
approximately equal, which means that the net rate of variation of the
concentration of the intermediate is small compared to the formation and
destruction, and the concentration of the intermediate varies only slowly.
[citation_needed]
Its use facilitates the resolution of the differential_equations that arise
from rate_equations, which lack an analytical_solution for most mechanisms
beyond the most simple ones. The steady state approximation is applied, for
example in Michaelis-Menten_kinetics.
As an example, the steady state approximation will be applied to two
consecutive, irreversible, homogeneous first order reactions in a closed
system. (For heterogeneous reactions, see reactions_on_surfaces.) This model
corresponds, for example, to a series of nuclear_decompositions like       U
239  &#x27F6;  Np     239  &#x27F6;  Pu     239      {\displaystyle {\ce {^
{239}U -> ^{239}Np -> ^{239}Pu\!}}}  [{\displaystyle {\ce {^{239}U -> ^{239}Np
-> ^{239}Pu\!}}}].
If the rate constants for the following reaction are      k  1
{\displaystyle k_{1}}  [k_{1}] and      k  2     {\displaystyle k_{2}}  [k_
{2}];      A &#x27F6; B &#x27F6; C    {\displaystyle {\ce {A -> B -> C}}}  [
{\displaystyle {\ce {A -> B -> C}}}], combining the rate_equations with a mass
balance for the system yields three coupled differential equations:
**** Reaction rates[edit] ****
For species A:        d [  A  ]   d t    = &#x2212;  k  1   [  A  ]
{\displaystyle {\frac {d[{\ce {A}}]}{dt}}=-k_{1}[{\ce {A}}]}  [{\displaystyle
{\frac {d[{\ce {A}}]}{dt}}=-k_{1}[{\ce {A}}]}]
For species B:        d [  B  ]   d t    =  k  1   [  A  ] &#x2212;  k  2
[  B  ]   {\displaystyle {\frac {d[{\ce {B}}]}{dt}}=k_{1}[{\ce {A}}]-k_{2}[{\ce
{B}}]}  [{\displaystyle {\frac {d[{\ce {B}}]}{dt}}=k_{1}[{\ce {A}}]-k_{2}[{\ce
{B}}]}], Here the first (positive) term represents the formation of B by the
first step      A &#x27F6; B    {\displaystyle {\ce {A -> B}}}  [{\displaystyle
{\ce {A -> B}}}], whose rate depends on the initial reactant A. The second
(negative) term represents the consumption of B by the second step      B
&#x27F6; C    {\displaystyle {\ce {B -> C}}}  [{\displaystyle {\ce {B -> C}}}],
whose rate depends on B as the reactant in that step.
For species C:        d [  C  ]   d t    =  k  2   [  B  ]   {\displaystyle
{\frac {d[{\ce {C}}]}{dt}}=k_{2}[{\ce {B}}]}  [{\displaystyle {\frac {d[{\ce
{C}}]}{dt}}=k_{2}[{\ce {B}}]}], the rate of formation of C by the second step.
**** Analytical solutions[edit] ****
The analytical solutions for these equations (supposing that initial
concentrations of every substance except for A are zero) are:[2]
         [   A   ] = [   A    ]  0    e  &#x2212;  k  1   t     {\displaystyle
      [{{\ce {A}}}]=[{{\ce {A}}}]_{0}e^{-k_{1}t}}  [{\displaystyle [{\ce {A}}]=
      [{\ce {A}}]_{0}e^{-k_{1}t}}]
          [   B   ]  =   {      [   A   ]   0      k  1     k  2   &#x2212;  k
      1       (   e  &#x2212;  k  1   t   &#x2212;  e  &#x2212;  k  2   t    )
      ;    k  1   &#x2260;  k  2            [   A   ]   0    k  1   t  e
      &#x2212;  k  1   t   ;    otherwise          {\displaystyle \left[{{\ce
      {B}}}\right]={\begin{cases}\left[{{\ce {A}}}\right]_{0}{\frac {k_{1}}{k_
      {2}-k_{1}}}\left(e^{-k_{1}t}-e^{-k_{2}t}\right);&k_{1}\neq k_{2}\\\\\left
      [{{\ce {A}}}\right]_{0}k_{1}te^{-k_{1}t};&{\text{otherwise}}\\\end
      {cases}}}  [{\displaystyle \left[{\ce {B}}\right]={\begin{cases}\left[
      {\ce {A}}\right]_{0}{\frac {k_{1}}{k_{2}-k_{1}}}\left(e^{-k_{1}t}-e^{-k_
      {2}t}\right);&k_{1}\neq k_{2}\\\\\left[{\ce {A}}\right]_{0}k_{1}te^{-k_
      {1}t};&{\text{otherwise}}\\\end{cases}}}]
          [   C   ]  =   {      [   A   ]   0    (  1 +     k  1    e  &#x2212;
      k  2   t   &#x2212;  k  2    e  &#x2212;  k  1   t      k  2   &#x2212;
      k  1       )  ;    k  1   &#x2260;  k  2            [   A   ]   0    (  1
      &#x2212;  e  &#x2212;  k  1   t   &#x2212;  k  1   t  e  &#x2212;  k  1
      t    )  ;    otherwise          {\displaystyle \left[{{\ce {C}}}\right]=
      {\begin{cases}\left[{{\ce {A}}}\right]_{0}\left(1+{\frac {k_{1}e^{-k_
      {2}t}-k_{2}e^{-k_{1}t}}{k_{2}-k_{1}}}\right);&k_{1}\neq k_{2}\\\\\left[{
      {\ce {A}}}\right]_{0}\left(1-e^{-k_{1}t}-k_{1}te^{-k_{1}t}\right);&{\text
      {otherwise}}\\\end{cases}}}  [{\displaystyle \left[{\ce {C}}\right]=
      {\begin{cases}\left[{\ce {A}}\right]_{0}\left(1+{\frac {k_{1}e^{-k_{2}t}-
      k_{2}e^{-k_{1}t}}{k_{2}-k_{1}}}\right);&k_{1}\neq k_{2}\\\\\left[{\ce
      {A}}\right]_{0}\left(1-e^{-k_{1}t}-k_{1}te^{-k_{1}t}\right);&{\text
      {otherwise}}\\\end{cases}}}]
**** Steady state[edit] ****
If the steady state approximation is applied, then the derivative of the
concentration of the intermediate is set to zero. This reduces the second
differential equation to an algebraic equation which is much easier to solve.
            d [   B   ]   d t    = 0 =  k  1   [   A   ] &#x2212;  k  2   [   B
      ] &#x21D2;  [   B   ] =    k  1    k  2     [   A   ]   {\displaystyle
      {\frac {d[{{\ce {B}}}]}{dt}}=0=k_{1}[{{\ce {A}}}]-k_{2}[{{\ce
      {B}}}]\Rightarrow \;[{{\ce {B}}}]={\frac {k_{1}}{k_{2}}}[{{\ce {A}}}]}  [
      {\displaystyle {\frac {d[{\ce {B}}]}{dt}}=0=k_{1}[{\ce {A}}]-k_{2}[{\ce
      {B}}]\Rightarrow \;[{\ce {B}}]={\frac {k_{1}}{k_{2}}}[{\ce {A}}]}].
Therefore,        d [   C   ]   d t    =  k  1   [   A   ]   {\displaystyle
{\frac {d[{{\ce {C}}}]}{dt}}=k_{1}[{{\ce {A}}}]}  [{\displaystyle {\frac {d[
{\ce {C}}]}{dt}}=k_{1}[{\ce {A}}]}], so that     [   C   ] = [   A    ]  0
(  1 &#x2212;  e  &#x2212;  k  1   t    )    {\displaystyle [{{\ce {C}}}]=[{
{\ce {A}}}]_{0}\left(1-e^{-k_{1}t}\right)}  [{\displaystyle [{\ce {C}}]=[{\ce
{A}}]_{0}\left(1-e^{-k_{1}t}\right)}].
**** Validity[edit] ****
Concentration vs. time. Concentration of intermediate in green, product in blue
and substrate in red
(     k  2    /   k  1   = 0.5   {\displaystyle k_{2}/k_{1}=0.5}  [k_{2}/k_
{1}=0.5])
Concentration vs. time. Concentration of intermediate in green, product in blue
and substrate in red
(     k  2    /   k  1   = 10   {\displaystyle k_{2}/k_{1}=10}  [k_{2}/k_
{1}=10])
The analytical and approximated solutions should now be compared in order to
decide when it is valid to use the steady state approximation. The analytical
solution transforms into the approximate one when      k  2   &#x226B;  k  1
{\displaystyle k_{2}\gg k_{1}}  [k_{2}\gg k_{1}], because then      e  &#x2212;
k  2   t   &#x226A;  e  &#x2212;  k  1   t     {\displaystyle e^{-k_{2}t}\ll e^
{-k_{1}t}}  [e^{{-k_{2}t}}\ll e^{{-k_{1}t}}] and      k  2   &#x2212;  k  1
&#x2248;   k  2     {\displaystyle k_{2}-k_{1}\approx \;k_{2}}  [k_{2}-k_
{1}\approx \;k_{2}]. Therefore, it is valid to apply the steady state
approximation only if the second reaction is much faster than the first one
(k2/k1 > 10 is a common criterion), because that means that the intermediate
forms slowly and reacts readily so its concentration stays low.
The graphs show concentrations of A (red), B (green) and C (blue) in two cases,
calculated from the analytical solution.
When the first reaction is faster it is not valid to assume that the variation
of [B] is very small, because [B] is neither low or close to constant: first A
transforms into B rapidly and B accumulates because it disappears slowly. As
the concentration of A decreases its rate of transformation decreases, at the
same time the rate of reaction of B into C increases as more B is formed, so a
maximum is reached when     t =   {       ln &#x2061;  (    k  1    k  2     )
k  1   &#x2212;  k  2          k  1   &#x2260;  k  2            1  k  1
otherwise          {\displaystyle t={\begin{cases}{\frac {\ln \left({\frac {k_
{1}}{k_{2}}}\right)}{k_{1}-k_{2}}}&\,k_{1}\neq k_{2}\\\\{\frac {1}{k_{1}}}&\,
{\text{otherwise}}\\\end{cases}}}  [{\displaystyle t={\begin{cases}{\frac {\ln
\left({\frac {k_{1}}{k_{2}}}\right)}{k_{1}-k_{2}}}&\,k_{1}\neq k_{2}\\\\{\frac
{1}{k_{1}}}&\,{\text{otherwise}}\\\end{cases}}}].
From then on the concentration of B decreases.
When the second reaction is faster, after a short induction_period,
concentration of B remains low (and more or less constant) because its rate of
formation and disappearance are almost equal and the steady state approximation
can be used.
The equilibrium approximation can be used sometimes in chemical kinetics to
yield similar results to the steady state approximation. It consists in
assuming that the intermediate arrives rapidly at chemical equilibrium with the
reactants. For example, Michaelis-Menten_kinetics can be derived assuming
equilibrium instead of steady state. Normally the requirements for applying the
steady state approximation are laxer: the concentration of the intermediate is
only needed to be low and more or less constant (as seen, this has to do only
with the rates at which it appears and disappears) but it is not needed to be
at equilibrium.
***** See also[edit] *****
    * Lindemann_mechanism
    * Reaction_progress_kinetic_analysis
***** Notes and references[edit] *****
   1. ^ IUPAC_Gold_Book_definition_of_steady_state
   2. ^ P. W. Atkins and J. de Paula, Physical Chemistry (8th edition,
      W.H.Freeman 2006), p.811
   3. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   4. ISBN 0-7167-8759-8
***** External links[edit] *****
    * https://chem.libretexts.org/Core/Physical_and_Theoretical_Chemistry/
      Kinetics/Reaction_Mechanisms/Steady-State_Approximation

Retrieved from "https://en.wikipedia.org/w/index.php?title=Steady_state_
(chemistry)&oldid=879261737"
Categories:
    * Chemical_kinetics
    * Physical_chemistry
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2016
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
    * Eesti
    * FranÃ§ais
    * Italiano
    * Norsk
    * Polski
    * PortuguÃªs
    * SlovenÄina
    * Suomi
Edit_links
    * This page was last edited on 20 January 2019, at 02:49 (UTC).
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
