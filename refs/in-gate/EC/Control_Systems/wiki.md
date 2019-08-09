The following text has been accessed from https://en.wikipedia.org/wiki/Control_system at Fri Aug 9 03:43:51 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Control system ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other uses, see Control_system_(disambiguation).
The centrifugal_governor is an early proportional_control mechanism.
A control system manages, commands, directs, or regulates the behavior of other
devices or systems using control_loops. It can range from a single home heating
controller using a thermostat controlling a domestic boiler to large Industrial
control_systems which are used for controlling processes or machines.
For continuously modulated control, a feedback_controller is used to
automatically control a process or operation. The control system compares the
value or status of the process_variable (PV) being controlled with the desired
value or setpoint (SP), and applies the difference as a control signal to bring
the process variable output of the plant to the same value as the setpoint.
For sequential and combinational_logic, software_logic, such as in a
programmable_logic_controller, is used.
⁰
***** Contents *****
    * 1_Open-loop_and_closed-loop_control
    * 2_Feedback_control_systems
    * 3_Logic_control
    * 4_Onâoff_control
    * 5_Linear_control
          o 5.1_Proportional_control
                # 5.1.1_Furnace_example
                      # 5.1.1.1_Underdamped
                      # 5.1.1.2_Overdamped
          o 5.2_PID_control
                # 5.2.1_Derivative_action
                # 5.2.2_Integral_action
                # 5.2.3_Ramp_up %_per_minute
          o 5.3_Other_techniques
    * 6_Fuzzy_logic
    * 7_Physical_implementation
    * 8_See_also
    * 9_References
    * 10_External_links
***** Open-loop and closed-loop control[edit] *****
There are two common classes of control action: open loop and closed loop. In
an open-loop control system, the control action from the controller is
independent of the process variable. An example of this is a central heating
boiler controlled only by a timer. The control action is the switching on or
off of the boiler. The process variable is the building temperature.This
controller operates the heating system for a constant time regardless of the
temperature of the building.
In a closed-loop control system, the control action from the controller is
dependent on the desired and actual process variable. In the case of the boiler
analogy, this would utilise a thermostat to monitor the building temperature,
and feed back a signal to ensure the controller output maintains the building
temperature close to that set on the thermostat. A closed loop controller has a
feedback loop which ensures the controller exerts a control action to control a
process variable at the same value as the setpoint. For this reason, closed-
loop controllers are also called feedback controllers.[1]
***** Feedback control systems[edit] *****
Example of a single industrial control loop; showing continuously modulated
control of process flow.
A basic feedback loop
In the case of linear feedback systems, a control_loop including sensors,
control algorithms, and actuators is arranged in an attempt to regulate a
variable at a setpoint (SP). An everyday example is the cruise_control on a
road vehicle; where external influences such as gradients would cause speed
changes, and the driver has the ability to alter the desired set speed. The PID
algorithm in the controller restores the actual speed to the desired speed in
the optimum way, with minimal delay or overshoot, by controlling the power
output of the vehicle's engine.
Control systems that include some sensing of the results they are trying to
achieve are making use of feedback and can adapt to varying circumstances to
some extent. Open-loop_control_systems do not make use of feedback, and run
only in pre-arranged ways.
***** Logic control[edit] *****
Logic control systems for industrial and commercial machinery were historically
implemented by interconnected electrical relays and cam_timers using ladder
logic. Today, most such systems are constructed with microcontrollers or more
specialized programmable_logic_controllers (PLCs). The notation of ladder logic
is still in use as a programming method for PLCs.[2]
Logic controllers may respond to switches and sensors, and can cause the
machinery to start and stop various operations through the use of actuators.
Logic controllers are used to sequence mechanical operations in many
applications. Examples include elevators, washing machines and other systems
with interrelated operations. An automatic sequential control system may
trigger a series of mechanical actuators in the correct sequence to perform a
task. For example, various electric and pneumatic transducers may fold and glue
a cardboard box, fill it with product and then seal it in an automatic
packaging machine.
PLC software can be written in many different ways â ladder diagrams, SFC
(sequential_function_charts) or statement_lists.[3]
***** Onâoff control[edit] *****
Main article: Bangâbang_control
Onâoff control uses a feedback controller that switches abruptly between two
states. A simple bi-metallic domestic thermostat can be described as an on-off
controller. When the temperature in the room (PV) goes below the user setting
(SP), the heater is switched on. Another example is a pressure switch on an air
compressor. When the pressure (PV) drops below the setpoint (SP) the compressor
is powered. Refrigerators and vacuum pumps contain similar mechanisms. Simple
onâoff control systems like these can be cheap and effective.
***** Linear control[edit] *****
Linear control systems use negative_feedback to produce a control signal to
maintain the controlled PV at the desired SP. There are several types of linear
control systems with different capabilities.
**** Proportional control[edit] ****
Main article: Proportional_control
Step responses for a second order system defined by the transfer_function     H
( s ) =    &#x03C9;  n   2     s  2   + 2 &#x03B6;  &#x03C9;  n   s +  &#x03C9;
n   2        {\displaystyle H(s)={\frac {\omega _{n}^{2}}{s^{2}+2\zeta \omega _
{n}s+\omega _{n}^{2}}}}  [{\displaystyle H(s)={\frac {\omega _{n}^{2}}{s^
{2}+2\zeta \omega _{n}s+\omega _{n}^{2}}}}], where     &#x03B6;
{\displaystyle \zeta }  [\zeta ] is the damping ratio and      &#x03C9;  n
{\displaystyle \omega _{n}}  [\omega _{n}] is the undamped natural frequency.
Proportional control is a type of linear feedback control system in which a
correction is applied to the controlled variable which is proportional to the
difference between the desired value (SP) and the measured value (PV). Two
classic mechanical examples are the toilet bowl float_proportioning_valve and
the fly-ball_governor.
The proportional control system is more complex than an onâoff control
system, but simpler than a proportional-integral-derivative (PID) control
system used, for instance, in an automobile cruise_control. Onâoff control
will work for systems that do not require high accuracy or responsiveness, but
is not effective for rapid and timely corrections and responses. Proportional
control overcomes this by modulating the manipulated variable (MV), such as a
control_valve, at a gain level which avoids instability, but applies correction
as fast as practicable by applying the optimum quantity of proportional
correction.
A drawback of proportional control is that it cannot eliminate the residual
SPâPV error, as it requires an error to generate a proportional output. A PI
controller can be used to overcome this. The PI controller uses a proportional
term (P) to remove the gross error, and an integral term (I) to eliminate the
residual offset error by integrating the error over time.
In some systems there are practical limits to the range of the MV. For example,
a heater has a limit to how much heat it can produce and a valve can open only
so far. Adjustments to the gain simultaneously alter the range of error values
over which the MV is between these limits. The width of this range, in units of
the error variable and therefore of the PV, is called the proportional band
(PB).
*** Furnace example[edit] ***
When controlling the temperature of an industrial_furnace, it is usually better
to control the opening of the fuel valve in proportion to the current needs of
the furnace. This helps avoid thermal shocks and applies heat more effectively.
At low gains, only a small corrective action is applied when errors are
detected. The system may be safe and stable, but may be sluggish in response to
changing conditions. Errors will remain uncorrected for relatively long periods
of time and the system is overdamped. If the proportional gain is increased,
such systems become more responsive and errors are dealt with more quickly.
There is an optimal value for the gain setting when the overall system is said
to be critically_damped. Increases in loop gain beyond this point lead to
oscillations in the PV and such a system is underdamped.
** Underdamped[edit] **
In the furnace example, suppose the temperature is increasing towards a
setpoint. Once the setpoint is reached, stored heat within the heater sub-
system and in the walls of the furnace will keep the measured temperature
rising beyond what is required. After rising above the setpoint, the
temperature falls back and eventually heat is applied again. Now the heater and
the furnace walls cool and the temperature falls too low before its fall is
arrested and the cycle repeats.
The temperature oscillations that an underdamped furnace control system
produces are unacceptable for many reasons, including the waste of fuel and
time (each oscillation cycle may take many minutes), as well as the likelihood
of seriously overheating both the furnace and its contents.
** Overdamped[edit] **
Suppose that the gain of the control system is reduced drastically and it is
restarted. As the temperature approaches, say 30Â° below SP (A 60Â°
proportional band (PB) this time), the heat input begins to be reduced, the
rate of heating of the furnace has time to slow and, as the heat is still
further reduced, it eventually is brought up to setpoint, just as 50% power
input is reached and the furnace is operating as required. There was some
wasted time while the furnace crept to its final temperature using only 52%
then 51% of available power, but at least no harm was done. By carefully
increasing the gain (i.e. reducing the width of the PB) this overdamped and
sluggish behavior can be improved until the system is critically damped for
this SP temperature. Doing this is known as 'tuning' the control system. A
well-tuned proportional furnace temperature control system will usually be more
effective than on-off control, but will still respond more slowly than the
furnace could under skillful manual control.
**** PID control[edit] ****
A block_diagram of a PID controller
Effects of varying PID parameters (Kp,Ki,Kd) on the step response of a system.
Main article: PID_controller
Apart from sluggish performance to avoid oscillations, another problem with
proportional-only control is that power application is always in direct
proportion to the error. In the example above we assumed that the set
temperature could be maintained with 50% power. What happens if the furnace is
required in a different application where a higher set temperature will require
80% power to maintain it? If the gain was finally set to a 50Â° PB, then 80%
power will not be applied unless the furnace is 15Â° below setpoint, so for
this other application the operators will have to remember always to set the
setpoint temperature 15Â° higher than actually needed. This 15Â° figure is not
completely constant either: it will depend on the surrounding ambient
temperature, as well as other factors that affect heat loss from or absorption
within the furnace.
To resolve these two problems, many feedback control schemes include
mathematical extensions to improve performance. The most common extensions lead
to proportional-integral-derivative control, or PID_control.
*** Derivative action[edit] ***
The derivative part is concerned with the rate-of-change of the error with
time: If the measured variable approaches the setpoint rapidly, then the
actuator is backed off early to allow it to coast to the required level;
conversely if the measured value begins to move rapidly away from the setpoint,
extra effort is appliedâin proportion to that rapidityâto try to maintain
it.
Derivative action makes a control system behave much more intelligently. On
control systems like the tuning of the temperature of a furnace, or perhaps the
motion-control of a heavy item like a gun or camera on a moving vehicle, the
derivative action of a well-tuned PID controller can allow it to reach and
maintain a setpoint better than most skilled human operators could.
If derivative action is over-applied, it can lead to oscillations too. An
example would be a PV that increased rapidly towards SP, then halted early and
seemed to "shy away" from the setpoint before rising towards it again.
*** Integral action[edit] ***
Change of response of second order system to a step input for varying Ki
values.
The integral term magnifies the effect of long-term steady-state errors,
applying ever-increasing effort until they reduce to zero. In the example of
the furnace above working at various temperatures, if the heat being applied
does not bring the furnace up to setpoint, for whatever reason, integral action
increasingly moves the proportional band relative to the setpoint until the PV
error is reduced to zero and the setpoint is achieved.
*** Ramp up % per minute[edit] ***
Some controllers include the option to limit the "ramp up % per minute". This
option can be very helpful in stabilizing small boilers (3 MBTUH), especially
during the summer, during light loads. A utility boiler "unit may be required
to change load at a rate of as much as 5% per minute (IEA Coal Online - 2,
2007)".[4]
**** Other techniques[edit] ****
It is possible to filter the PV or error signal. Doing so can reduce the
response of the system to undesirable frequencies, to help reduce instability
or oscillations. Some feedback systems will oscillate at just one frequency. By
filtering out that frequency, more "stiff" feedback can be applied, making the
system more responsive without shaking itself apart.
Feedback systems can be combined. In cascade_control, one control loop applies
control algorithms to a measured variable against a setpoint, but then provides
a varying setpoint to another control loop rather than affecting process
variables directly. If a system has several different measured variables to be
controlled, separate control systems will be present for each of them.
Control_engineering in many applications produces control systems that are more
complex than PID control. Examples of such fields include fly-by-wire aircraft
control systems, chemical plants, and oil refineries. Model_predictive_control
systems are designed using specialized computer-aided-design software and
empirical mathematical models of the system to be controlled.
Hybrid systems of PID and logic control are widely used. The output from a
linear controller may be interlocked by logic for instance.
***** Fuzzy logic[edit] *****
Main article: Fuzzy_logic
Fuzzy_logic is an attempt to apply the easy design of logic controllers to the
control of complex continuously varying systems. Basically, a measurement in a
fuzzy logic system can be partly true, that is if yes is 1 and no is 0, a fuzzy
measurement can be between 0 and 1.
The rules of the system are written in natural language and translated into
fuzzy logic. For example, the design for a furnace would start with: "If the
temperature is too high, reduce the fuel to the furnace. If the temperature is
too low, increase the fuel to the furnace."
Measurements from the real world (such as the temperature of a furnace) are
converted to values between 0 and 1 by seeing where they fall on a triangle.
Usually, the tip of the triangle is the maximum possible value which translates
to 1.
Fuzzy logic, then, modifies Boolean_logic to be arithmetical. Usually the "not"
operation is "output = 1 - input," the "and" operation is "output = input.1
multiplied by input.2," and "or" is "output = 1 - ((1 - input.1) multiplied by
(1 - input.2))". This reduces to Boolean_arithmetic if values are restricted to
0 and 1, instead of allowed to range in the unit_interval [0,1].
The last step is to "defuzzify" an output. Basically, the fuzzy calculations
make a value between zero and one. That number is used to select a value on a
line whose slope and height converts the fuzzy value to a real-world output
number. The number then controls real machinery.
If the triangles are defined correctly and rules are right the result can be a
good control system.
When a robust fuzzy design is reduced into a single, quick calculation, it
begins to resemble a conventional feedback loop solution and it might appear
that the fuzzy design was unnecessary. However, the fuzzy logic paradigm may
provide scalability for large control systems where conventional methods become
unwieldy or costly to derive.
Fuzzy_electronics is an electronic technology that uses fuzzy logic instead of
the two-value logic more commonly used in digital_electronics.
***** Physical implementation[edit] *****
A DCS control room where plant information and controls are displayed on
computer graphics screens. The operators are seated as they can view and
control any part of the process from their screens, whilst retaining a plant
overview.
A control panel of a hydraulic heat press machine with dedicated software for
that function
The range of implementation is from compact_controllers often with dedicated
software for a particular machine or device, to distributed_control_systems for
industrial process control.
Logic systems and feedback controllers are usually implemented with
programmable_logic_controllers.
***** See also[edit] *****
    * Behavior_trees_(artificial_intelligence,_robotics_and_control)
    * Building_automation
    * Coefficient_diagram_method
    * Control_engineering
    * Control_theory
    * Cybernetics
    * Distributed_control_system
    * Droop_speed_control
    * Education_and_training_of_electrical_and_electronics_engineers
    * EPICS
    * Good_regulator
    * Hierarchical_control_system
    * HVAC_control_system
    * Industrial_control_systems
    * Motion_control
    * Networked_control_system
    * Numerical_control
    * Perceptual_control_theory
    * PID_controller
    * Process_control
    * Process_optimization
    * Programmable_logic_controller
    * Sampled_data_systems
    * SCADA
    * VisSim
***** References[edit] *****
 This article needs additional citations for verification. Relevant discussion may be found on
 the talk_page. Please help improve_this_article by adding_citations_to_reliable_sources.
 Unsourced material may be challenged and removed.
 Find sources: "Control_system" â news Â· newspapers Â· books Â· scholar Â· JSTOR (December
 2010)(Learn_how_and_when_to_remove_this_template_message)
   1. ^ "Feedback and control systems" - JJ Di Steffano, AR Stubberud, IJ
      Williams. Schaums outline series, McGraw-Hill 1967
   2. ^Kuphaldt, Tony R. "Chapter_6_LADDER_LOGIC". Lessons In Electric Circuits
      -- Volume IV. Archived from the original on 12 September 2010. Retrieved
      22 September 2010.
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
   4. ^Brady, Ian. "Programmable_logic_controllers_-_benefits_and_applications"
      (PDF). PLCs. Archived (PDF) from the original on 2 February 2014.
      Retrieved 5 December 2011.
   5. ^"Archived_copy" (PDF). Archived (PDF) from the original on 2014-08-05.
      Retrieved 2014-04-07.CS1 maint: Archived copy as title (link)
   6.  ABB: Power Generation Energy Efficient Design of Auxiliary Systems in
      Fossil-Fuel Power Plants, Page 262, Section: Load Following
***** External links[edit] *****
 Wikibooks has a book on the topic of: Control_Systems
    * Semiautonomous_Flight_Direction_-_Reference_unmannedaircraft.org
    * Control_System_Toolbox for design and analysis of control systems.
    * Control_Systems_Manufacturer Design and Manufacture of control systems.
    * Mathematica_functions_for_the_analysis,_design,_and_simulation_of_control
      systems

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Control_system&oldid=909649923"
Categories:
    * Control_theory
    * Control_engineering
    * Systems_engineering
    * Systems_theory
    * Automation
Hidden categories:
    * CS1_maint:_Archived_copy_as_title
    * Articles_needing_additional_references_from_December_2010
    * All_articles_needing_additional_references
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
    * Wikibooks
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * CatalÃ 
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Bahasa_Melayu
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Suomi
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * Zazaki
    * ä¸­æ
Edit_links
    * This page was last edited on 6 August 2019, at 18:48 (UTC).
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
