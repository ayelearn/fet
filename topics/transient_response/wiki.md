The following text has been accessed from https://en.wikipedia.org/wiki/Transient_response at Fri Aug 9 01:30:34 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Transient response ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
the response of a system to a change from an equilibrium state
Damped_oscillation is a typical transient response, where the output value
oscillates until finally reaching a steady-state value (The underdamped
response case).
In electrical_engineering and mechanical_engineering, a transient response is
the response of a system to a change from an equilibrium or a steady_state. The
transient response is not necessarily tied to abrupt events but to any event
that affects the equilibrium of the system. The impulse_response and step
response are transient responses to a specific input (an impulse and a step,
respectively).
⁰
***** Contents *****
    * 1_Damping
    * 2_Properties
    * 3_See_also
    * 4_References
***** Damping[edit] *****
The response can be classified as one of three types of damping that describes
the output in relation to the steady-state_response.
  Underdamped
      An underdamped response is one that oscillates within a decaying
      envelope. The more underdamped the system, the more oscillations and
      longer it takes to reach steady-state. Here damping_ratio is always less
      than one.
  Critically damped
      A critically_damped response is that response which reaches the steady-
      state value the fastest without being underdamped. It is related to
      critical_points in the sense that it straddles the boundary of
      underdamped and overdamped responses. Here, damping ratio is always equal
      to one. There should be no oscillation about the steady state value in
      the ideal case.
  Overdamped
      An overdamped response is the response that does not oscillate about the
      steady-state value but takes longer to reach steady-state than the
      critically damped case. Here damping ratio is greater than one.
***** Properties[edit] *****
Typical second order transient system properties
Transient response can be quantified with the following properties.
  Rise time
      Rise_time refers to the time required for a signal to change from a
      specified low value to a specified high value. Typically, these values
      are 10% and 90% of the step height.
  Overshoot
      Overshoot is when a signal or function exceeds its target. It is often
      associated with ringing.
  Settling time
      Settling_time is the time elapsed from the application of an ideal
      instantaneous step input to the time at which the output has entered and
      remained within a specified error_band[1], the time after which equality
      is satisfied:
Illustration for the concept of "settling time"[1]
          |  h ( t ) &#x2212;  h  s t    |  &#x2A7D; &#x03F5;   {\displaystyle
      |h(t)-h_{st}|\leqslant \epsilon }  [{\displaystyle |h(t)-h_{st}|\leqslant
      \epsilon }]
      where      h  s t     {\displaystyle h_{st}}  [{\displaystyle h_{st}}] is
      the steady-state value, and     &#x03F5;   {\displaystyle \epsilon }
      [\epsilon ] is an advance predetermined positive number.
      For linear continuous dynamical systems, it is the usual to consider its
      transient response caused by the unit_step_perturbation; but in this case
      the steady-state value is reached in an infinitely long time. If,
      however, the accuracy of reaching the steady-state value is limited to a
      small value     &#x03F5;   {\displaystyle \epsilon }  [\epsilon ]
      specified error band, then the duration of the transient response     t
      {\displaystyle t}  [t] is a finite quantity.
  Delay-time
      The delay time is the time required for the response to reach half the
      final value the very first time.[2]
  Peak time
      The peak time is the time required for the response to reach the first
      peak of the overshoot.[2]
  Steady-state error
      2003's Instrument Engineers' Handbook defines the steady-state error of a
      system as "the difference between the desired final output and the actual
      one" when the system reaches a steady_state, when its behavior may be
      expected to continue if the system is undisturbed.[3]
***** See also[edit] *****
    * Attractor
    * Carrying_capacity
    * Control_theory
    * Dynamical_system
    * Ecological_footprint
    * Economic_growth
    * Engine_test_stand
    * Equilibrium_point
    * List_of_types_of_equilibrium
    * Evolutionary_economics
    * Growth_curve
    * Herman_Daly
    * Homeostasis
    * Limit_cycle
    * Limits_to_Growth
    * Population_dynamics
    * Race_condition
    * Simulation
    * State_function
    * Steady_state
    * Steady_state_economy
    * Steady_State_theory
    * Systems_theory
    * Thermodynamic_equilibrium
    * Transient_state
***** References[edit] *****
   1. ^ a bGlushkov, V. M. Encyclopedia of Cybernetics (in Russian) (1 ed.).
      Kiev: USE. p. 624.
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
   3. ^ a bOgata, Katsuhiko. Modern Control Engineering (4 ed.). Prentice-Hall.
      p. 230. ISBN 0-13-043245-8.
   4. ^LiptÃ¡k, BÃ©la G. (2003). Instrument Engineers' Handbook: Process
      control and optimization (4th ed.). CRC Press. p. 108. ISBN 0-8493-1081-
      4.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Transient_response&oldid=909497626"
Categories:
    * Engineering_concepts
    * Control_theory
Hidden categories:
    * CS1_Russian-language_sources_(ru)
    * Articles_with_short_description
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
    * Eesti
    * ÙØ§Ø±Ø³Û
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * æ¥æ¬èª
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 5 August 2019, at 20:22 (UTC).
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
