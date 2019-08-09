The following text has been accessed from https://en.wikipedia.org/wiki/Maximum_power_transfer_theorem at Thu Aug 8 22:53:43 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Maximum power transfer theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In electrical_engineering, the maximum power transfer theorem states that, to
obtain maximum external power from a source with a finite internal_resistance,
the resistance of the load must equal the resistance of the source as viewed
from its output terminals. Moritz_von_Jacobi published the maximum power
(transfer) theorem around 1840; it is also referred to as "Jacobi's law".[1]
The theorem results in maximum power transfer across the circuit, and not
maximum efficiency. If the resistance of the load is made larger than the
resistance of the source, then efficiency is higher, since a higher percentage
of the source power is transferred to the load, but the magnitude of the load
power is lower since the total circuit resistance goes up.
If the load resistance is smaller than the source resistance, then most of the
power ends up being dissipated in the source, and although the total power
dissipated is higher, due to a lower total resistance, it turns out that the
amount dissipated in the load is reduced.
The theorem states how to choose (so as to maximize power transfer) the load
resistance, once the source resistance is given. It is a common misconception
to apply the theorem in the opposite scenario. It does not say how to choose
the source resistance for a given load resistance. In fact, the source
resistance that maximizes power transfer is always zero, regardless of the
value of the load resistance.
The theorem can be extended to alternating_current circuits that include
reactance, and states that maximum power transfer occurs when the load
impedance is equal to the complex_conjugate of the source impedance.
⁰
***** Contents *****
    * 1_Maximizing_power_transfer_versus_power_efficiency
    * 2_Impedance_matching
    * 3_Calculus-based_proof_for_purely_resistive_circuits
    * 4_In_reactive_circuits
          o 4.1_Proof
    * 5_Notes
    * 6_References
    * 7_External_links
***** Maximizing power transfer versus power efficiency[edit] *****
The theorem was originally misunderstood (notably by Joule) to imply that a
system consisting of an electric motor driven by a battery could not be more
than 50% efficient since, when the impedances were matched, the power lost as
heat in the battery would always be equal to the power delivered to the motor.
In 1880 this assumption was shown to be false by either Edison or his colleague
Francis_Robbins_Upton, who realized that maximum efficiency was not the same as
maximum power transfer.
To achieve maximum efficiency, the resistance of the source (whether a battery
or a dynamo) could be (or should be) made as close to zero as possible. Using
this new understanding, they obtained an efficiency of about 90%, and proved
that the electric_motor was a practical alternative to the heat_engine.
[Source_and_load_circuit.svg] [Maximum_Power_Transfer_Graph.svg]
The condition of maximum power transfer does not result in maximum efficiency.
If we define the efficiency Î· as the ratio of power dissipated by the load,
RL, to power developed by the source, VS, then it is straightforward to
calculate from the above circuit diagram that
         &#x03B7; =    R   L      R   L    +  R   S       =   1  1 +  R   S
      /   R   L       .   {\displaystyle \eta ={\frac {R_{\mathrm {L} }}{R_
      {\mathrm {L} }+R_{\mathrm {S} }}}={\frac {1}{1+R_{\mathrm {S} }/R_
      {\mathrm {L} }}}.}  [{\displaystyle \eta ={\frac {R_{\mathrm {L} }}{R_
      {\mathrm {L} }+R_{\mathrm {S} }}}={\frac {1}{1+R_{\mathrm {S} }/R_
      {\mathrm {L} }}}.}]
Consider three particular cases:
    * If      R   L    =  R   S      {\displaystyle R_{\mathrm {L} }=R_{\mathrm
      {S} }}  [R_{{\mathrm  {L}}}=R_{{\mathrm  {S}}}], then     &#x03B7; = 0.5
      ,   {\displaystyle \eta =0.5,}  [\eta =0.5,]
    * If      R   L    &#x2192; &#x221E;   {\displaystyle R_{\mathrm {L} }\to
      \infty }  [{\displaystyle R_{\mathrm {L} }\to \infty }] or      R   S
      = 0 ,   {\displaystyle R_{\mathrm {S} }=0,}  [{\displaystyle R_{\mathrm
      {S} }=0,}] then     &#x03B7; = 1 ,   {\displaystyle \eta =1,}  [\eta =1,]
    * If      R   L    = 0   {\displaystyle R_{\mathrm {L} }=0}  [
      {\displaystyle R_{\mathrm {L} }=0}], then     &#x03B7; = 0.
      {\displaystyle \eta =0.}  [\eta =0.]
The efficiency is only 50% when maximum power transfer is achieved, but
approaches 100% as the load resistance approaches infinity, though the total
power level tends towards zero.
Efficiency also approaches 100% if the source resistance approaches zero, and
0% if the load resistance approaches zero. In the latter case, all the power is
consumed inside the source (unless the source also has no resistance), so the
power dissipated in a short_circuit is zero.
***** Impedance matching[edit] *****
Main article: impedance_matching
A related concept is reflectionless impedance_matching.
In radio frequency transmission_lines, and other electronics, there is often a
requirement to match the source_impedance (at the transmitter) to the load
impedance (such as an antenna) to avoid reflections in the transmission_line
that could overload or damage the transmitter.
***** Calculus-based proof for purely resistive circuits[edit] *****
(See Cartwright[2] for a non-calculus-based proof)
[Circuit_diagram]
In the diagram opposite, power is being transferred from the source, with
voltage V and fixed source_resistance RS, to a load with resistance RL,
resulting in a current I. By Ohm's_law, I is simply the source voltage divided
by the total circuit resistance:
         I =   V   R   S    +  R   L       .   {\displaystyle I={\frac {V}{R_
      {\mathrm {S} }+R_{\mathrm {L} }}}.}  [I={\frac  {V}{R_{{\mathrm  {S}}}+R_
      {{\mathrm  {L}}}}}.]
The power PL dissipated in the load is the square of the current multiplied by
the resistance:
          P   L    =  I  2    R   L    =   (   V   R   S    +  R   L       )
      2    R   L    =    V  2     R   S    2    /   R   L    + 2  R   S    +  R
      L       .   {\displaystyle P_{\mathrm {L} }=I^{2}R_{\mathrm {L} }=\left(
      {\frac {V}{R_{\mathrm {S} }+R_{\mathrm {L} }}}\right)^{2}R_{\mathrm {L}
      }={\frac {V^{2}}{R_{\mathrm {S} }^{2}/R_{\mathrm {L} }+2R_{\mathrm {S}
      }+R_{\mathrm {L} }}}.}  [P_{{\mathrm  {L}}}=I^{2}R_{{\mathrm  {L}}}=\left
      ({\frac  {V}{R_{{\mathrm  {S}}}+R_{{\mathrm  {L}}}}}\right)^{2}R_{
      {\mathrm  {L}}}={\frac  {V^{2}}{R_{{\mathrm  {S}}}^{2}/R_{{\mathrm
      {L}}}+2R_{{\mathrm  {S}}}+R_{{\mathrm  {L}}}}}.]
The value of RL for which this expression is a maximum could be calculated by
differentiating it, but it is easier to calculate the value of RL for which the
denominator
          R   S    2    /   R   L    + 2  R   S    +  R   L      {\displaystyle
      R_{\mathrm {S} }^{2}/R_{\mathrm {L} }+2R_{\mathrm {S} }+R_{\mathrm {L} }}
      [R_{{\mathrm  {S}}}^{2}/R_{{\mathrm  {L}}}+2R_{{\mathrm  {S}}}+R_{
      {\mathrm  {L}}}]
is a minimum. The result will be the same in either case. Differentiating the
denominator with respect to RL:
           d  d  R   L        (   R   S    2    /   R   L    + 2  R   S    +  R
      L     )  = &#x2212;  R   S    2    /   R   L    2   + 1.   {\displaystyle
      {\frac {d}{dR_{\mathrm {L} }}}\left(R_{\mathrm {S} }^{2}/R_{\mathrm {L}
      }+2R_{\mathrm {S} }+R_{\mathrm {L} }\right)=-R_{\mathrm {S} }^{2}/R_
      {\mathrm {L} }^{2}+1.}  [{\frac  {d}{dR_{{\mathrm  {L}}}}}\left(R_{
      {\mathrm  {S}}}^{2}/R_{{\mathrm  {L}}}+2R_{{\mathrm  {S}}}+R_{{\mathrm
      {L}}}\right)=-R_{{\mathrm  {S}}}^{2}/R_{{\mathrm  {L}}}^{2}+1.]
For a maximum or minimum, the first derivative is zero, so
          R   S    2    /   R   L    2   = 1   {\displaystyle R_{\mathrm {S} }^
      {2}/R_{\mathrm {L} }^{2}=1}  [R_{{\mathrm  {S}}}^{2}/R_{{\mathrm  {L}}}^
      {2}=1]
or
          R   L    = &#x00B1;  R   S    .   {\displaystyle R_{\mathrm {L} }=\pm
      R_{\mathrm {S} }.}  [R_{{\mathrm  {L}}}=\pm R_{{\mathrm  {S}}}.]
In practical resistive circuits, RS and RL are both positive, so the positive
sign in the above is the correct solution.
To find out whether this solution is a minimum or a maximum, the denominator
expression is differentiated again:
             d  2     d  R   L    2       (   R   S    2    /   R   L    + 2  R
      S    +  R   L     )  =  2  R   S    2     /    R   L    3    .
      {\displaystyle {{d^{2}} \over {dR_{\mathrm {L} }^{2}}}\left({R_{\mathrm
      {S} }^{2}/R_{\mathrm {L} }+2R_{\mathrm {S} }+R_{\mathrm {L} }}\right)=
      {2R_{\mathrm {S} }^{2}}/{R_{\mathrm {L} }^{3}}.\,\!}  [{{d^{2}} \over
      {dR_{{\mathrm  {L}}}^{2}}}\left({R_{{\mathrm  {S}}}^{2}/R_{{\mathrm
      {L}}}+2R_{{\mathrm  {S}}}+R_{{\mathrm  {L}}}}\right)={2R_{{\mathrm
      {S}}}^{2}}/{R_{{\mathrm  {L}}}^{3}}.\,\!]
This is always positive for positive values of      R   S        {\displaystyle
R_{\mathrm {S} }\,\!}  [R_{{\mathrm  {S}}}\,\!] and      R   L
{\displaystyle R_{\mathrm {L} }\,\!}  [R_{{\mathrm  {L}}}\,\!], showing that
the denominator is a minimum, and the power is therefore a maximum, when
          R   S    =  R   L    .     {\displaystyle R_{\mathrm {S} }=R_{\mathrm
      {L} }.\,\!}  [R_{{\mathrm  {S}}}=R_{{\mathrm  {L}}}.\,\!]
The above proof assumes fixed source resistance      R   S
{\displaystyle R_{\mathrm {S} }\,\!}  [R_{{\mathrm  {S}}}\,\!]. When the source
resistance can be varied, power transferred to the load can be increased by
reducing      R   S        {\displaystyle R_{\textrm {S}}\,\!}  [{\displaystyle
R_{\textrm {S}}\,\!}]. For example, a 100 Volt source with an      R   S
{\displaystyle R_{\textrm {S}}\,\!}  [{\displaystyle R_{\textrm {S}}\,\!}] of
10 &#xA0; &#x03A9;   {\displaystyle 10~\Omega }  [{\displaystyle 10~\Omega }]
will deliver 250 watts of power to a     10 &#xA0; &#x03A9;   {\displaystyle
10~\Omega }  [{\displaystyle 10~\Omega }] load; reducing      R   S
{\displaystyle R_{\textrm {S}}\,\!}  [{\displaystyle R_{\textrm {S}}\,\!}] to
0 &#xA0; &#x03A9;   {\displaystyle 0~\Omega }  [{\displaystyle 0~\Omega }]
increases the power delivered to 1000 watts.
Note that this shows that maximum power transfer can also be interpreted as the
load voltage being equal to one-half of the Thevenin voltage equivalent of the
source.[3]
***** In reactive circuits[edit] *****
The power transfer theorem also applies when the source and/or load are not
purely resistive.
A refinement of the maximum power theorem says that any reactive components of
source and load should be of equal magnitude but opposite sign. (See below for
a derivation.)
    * This means that the source and load impedances should be complex
      conjugates of each other.
    * In the case of purely resistive circuits, the two concepts are identical.
Physically realizable sources and loads are not usually purely resistive,
having some inductive or capacitive components, and so practical applications
of this theorem, under the name of complex conjugate impedance matching, do, in
fact, exist.
If the source is totally inductive (capacitive), then a totally capacitive
(inductive) load, in the absence of resistive losses, would receive 100% of the
energy from the source but send it back after a quarter cycle.
The resultant circuit is nothing other than a resonant LC_circuit in which the
energy continues to oscillate to and from. This oscillation is called reactive
power.
Power_factor_correction (where an inductive reactance is used to "balance out"
a capacitive one), is essentially the same idea as complex conjugate impedance
matching although it is done for entirely different reasons.
For a fixed reactive source, the maximum power theorem maximizes the real power
(P) delivered to the load by complex conjugate matching the load to the source.
For a fixed reactive load, power factor correction minimizes the apparent_power
(S) (and unnecessary current) conducted by the transmission lines, while
maintaining the same amount of real power transfer.
This is done by adding a reactance to the load to balance out the load's own
reactance, changing the reactive load impedance into a resistive load
impedance.
**** Proof[edit] ****
[source_and_load_impedance_diagram]
In this diagram, AC_power is being transferred from the source, with phasor
magnitude of voltage      |   V  S    |    {\displaystyle |V_{\text{S}}|}  [
{\displaystyle |V_{\text{S}}|}] (positive peak voltage) and fixed source
impedance      Z  S     {\displaystyle Z_{\text{S}}}  [{\displaystyle Z_{\text
{S}}}] (S for source), to a load with impedance      Z  L     {\displaystyle Z_
{\text{L}}}  [{\displaystyle Z_{\text{L}}}] (L for load), resulting in a
(positive) magnitude      |  I  |    {\displaystyle |I|}  [|I|] of the current
phasor     I   {\displaystyle I}  [I]. This magnitude      |  I  |
{\displaystyle |I|}  [|I|] results from dividing the magnitude of the source
voltage by the magnitude of the total circuit impedance:
          |  I  |  =     |   V  S    |     |   Z  S   +  Z  L    |     .
      {\displaystyle |I|={|V_{\text{S}}| \over |Z_{\text{S}}+Z_{\text{L}}|}.}
      [{\displaystyle |I|={|V_{\text{S}}| \over |Z_{\text{S}}+Z_{\text{L}}|}.}]
The average power      P  L     {\displaystyle P_{\text{L}}}  [{\displaystyle
P_{\text{L}}}] dissipated in the load is the square of the current multiplied
by the resistive portion (the real part)      R  L     {\displaystyle R_{\text
{L}}}  [{\displaystyle R_{\text{L}}}] of the load impedance      Z  L
{\displaystyle Z_{\text{L}}}  [{\displaystyle Z_{\text{L}}}]:
              P  L      =  I  rms   2    R  L   =   1 2    |  I   |   2    R  L
      =   1 2     (     |   V  S    |     |   Z  S   +  Z  L    |     )   2
      R  L   =   1 2       |   V  S     |   2    R  L     (  R  S   +  R  L
      )  2   + (  X  S   +  X  L    )  2      ,       {\displaystyle {\begin
      {aligned}P_{\text{L}}&=I_{\text{rms}}^{2}R_{\text{L}}={1 \over 2}|I|^
      {2}R_{\text{L}}\\&={1 \over 2}\left({|V_{\text{S}}| \over |Z_{\text
      {S}}+Z_{\text{L}}|}\right)^{2}R_{\text{L}}={1 \over 2}{|V_{\text{S}}|^
      {2}R_{\text{L}} \over (R_{\text{S}}+R_{\text{L}})^{2}+(X_{\text{S}}+X_
      {\text{L}})^{2}},\end{aligned}}}  [{\displaystyle {\begin{aligned}P_
      {\text{L}}&=I_{\text{rms}}^{2}R_{\text{L}}={1 \over 2}|I|^{2}R_{\text
      {L}}\\&={1 \over 2}\left({|V_{\text{S}}| \over |Z_{\text{S}}+Z_{\text
      {L}}|}\right)^{2}R_{\text{L}}={1 \over 2}{|V_{\text{S}}|^{2}R_{\text{L}}
      \over (R_{\text{S}}+R_{\text{L}})^{2}+(X_{\text{S}}+X_{\text{L}})^
      {2}},\end{aligned}}}]
where      R  S     {\displaystyle R_{\text{S}}}  [{\displaystyle R_{\text
{S}}}] and      R  L     {\displaystyle R_{\text{L}}}  [{\displaystyle R_{\text
{L}}}] denote the resistances, that is the real parts, and      X  S
{\displaystyle X_{\text{S}}}  [{\displaystyle X_{\text{S}}}] and      X  L
{\displaystyle X_{\text{L}}}  [{\displaystyle X_{\text{L}}}] denote the
reactances, that is the imaginary parts, of respectively the source and load
impedances      Z  S     {\displaystyle Z_{\text{S}}}  [{\displaystyle Z_{\text
{S}}}] and      Z  L     {\displaystyle Z_{\text{L}}}  [{\displaystyle Z_{\text
{L}}}].
To determine, for a given source voltage      V  S     {\displaystyle V_{\text
{S}}}  [{\displaystyle V_{\text{S}}}] and impedance      Z  S   ,
{\displaystyle Z_{\text{S}},}  [{\displaystyle Z_{\text{S}},}] the value of the
load impedance      Z  L   ,   {\displaystyle Z_{\text{L}},}  [{\displaystyle
Z_{\text{L}},}] for which this expression for the power yields a maximum, one
first finds, for each fixed positive value of      R  L     {\displaystyle R_
{\text{L}}}  [{\displaystyle R_{\text{L}}}], the value of the reactive term
X  L     {\displaystyle X_{\text{L}}}  [{\displaystyle X_{\text{L}}}] for which
the denominator
         (  R  S   +  R  L    )  2   + (  X  S   +  X  L    )  2
      {\displaystyle (R_{\text{S}}+R_{\text{L}})^{2}+(X_{\text{S}}+X_{\text
      {L}})^{2}\,}  [{\displaystyle (R_{\text{S}}+R_{\text{L}})^{2}+(X_{\text
      {S}}+X_{\text{L}})^{2}\,}]
is a minimum. Since reactances can be negative, this is achieved by adapting
the load reactance to
          X  L   = &#x2212;  X  S   .   {\displaystyle X_{\text{L}}=-X_{\text
      {S}}.}  [{\displaystyle X_{\text{L}}=-X_{\text{S}}.}]
This reduces the above equation to:
          P  L   =   1 2       |   V  S     |   2    R  L     (  R  S   +  R  L
      )  2        {\displaystyle P_{\text{L}}={\frac {1}{2}}{\frac {|V_{\text
      {S}}|^{2}R_{\text{L}}}{(R_{\text{S}}+R_{\text{L}})^{2}}}}  [
      {\displaystyle P_{\text{L}}={\frac {1}{2}}{\frac {|V_{\text{S}}|^{2}R_
      {\text{L}}}{(R_{\text{S}}+R_{\text{L}})^{2}}}}]
and it remains to find the value of      R  L     {\displaystyle R_{\text{L}}}
[{\displaystyle R_{\text{L}}}] which maximizes this expression. This problem
has the same form as in the purely resistive case, and the maximizing condition
therefore is      R  L   =  R  S   .   {\displaystyle R_{\text{L}}=R_{\text
{S}}.}  [{\displaystyle R_{\text{L}}=R_{\text{S}}.}]
The two maximizing conditions
    *     R  L   =  R  S     {\displaystyle R_{\text{L}}=R_{\text{S}}}  [
      {\displaystyle R_{\text{L}}=R_{\text{S}}}]
    *     X  L   = &#x2212;  X  S     {\displaystyle X_{\text{L}}=-X_{\text
      {S}}}  [{\displaystyle X_{\text{L}}=-X_{\text{S}}}]
describe the complex_conjugate of the source impedance, denoted by
&#x2217;   ,   {\displaystyle ^{*},}  [{\displaystyle ^{*},}] and thus can be
concisely combined to:
          Z  L   =  Z  S   &#x2217;   .   {\displaystyle Z_{\text{L}}=Z_{\text
      {S}}^{*}.}  [{\displaystyle Z_{\text{L}}=Z_{\text{S}}^{*}.}]
***** Notes[edit] *****
   1. ^Thompson Phillips (2009-05-30), Dynamo-Electric_Machinery;_A_Manual_for
      Students_of_Electrotechnics, BiblioBazaar, LLC, ISBN 978-1-110-35104-6
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
   3. ^Cartwright, Kenneth V (Spring 2008), "Non-Calculus_Derivation_of_the
      Maximum_Power_Transfer_Theorem" (PDF), Technology Interface, 8 (2): 19
      pages
   4. ^ http://www.electronics-tutorial.net/dccircuits/maximum-power-transfer-
      theorem/index.html
***** References[edit] *****
    * H.W. Jackson (1959) Introduction to Electronic Circuits, Prentice-Hall.
***** External links[edit] *****
    * Conjugate_matching_versus_reflectionless_matching (PDF) taken from
      Electromagnetic_Waves_and_Antennas
    * The_Spark_Transmitter._2._Maximising_Power,_part_1.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Maximum_power_transfer_theorem&oldid=893125255"
Categories:
    * Circuit_theorems
    * Electrical_engineering
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
    * ÙØ§Ø±Ø³Û
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * ä¸­æ
Edit_links
    * This page was last edited on 19 April 2019, at 05:13 (UTC).
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
