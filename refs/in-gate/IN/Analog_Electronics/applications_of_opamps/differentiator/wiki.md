The following text has been accessed from https://en.wikipedia.org/wiki/Differentiator at Fri Aug 9 01:27:16 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Differentiator ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article needs additional citations for verification. Please help improve_this_article by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and removed.
 Find sources: "Differentiator" â news Â· newspapers Â· books Â· scholar Â· JSTOR (December
 2009)(Learn_how_and_when_to_remove_this_template_message)
In electronics, a differentiator is a circuit that is designed such that the
output of the circuit is approximately directly proportional to the rate of
change (the time derivative) of the input. An active differentiator includes
some form of amplifier. A passive differentiator circuit is made of only
resistors and capacitors.
⁰
***** Contents *****
    * 1_Passive_differentiator
          o 1.1_Transfer_function
          o 1.2_Impulse_response
    * 2_Active_differentiator
          o 2.1_Ideal_differentiator
                # 2.1.1_Operation
                # 2.1.2_Frequency_response
                # 2.1.3_Advantages
                # 2.1.4_Limitations
          o 2.2_Practical_differentiator
                # 2.2.1_Frequency_response
          o 2.3_Applications
    * 3_See_also
    * 4_References
***** Passive differentiator[edit] *****
Figure 1: Capacitive Differentiator
Figure 2: Inductive Differentiator
A true differentiator cannot be physically realized, because it has infinite
gain at infinite frequency. A similar effect can be achieved, however, by
limiting the gain above some frequency. Therefore, a passive differentiator
circuit can be made using a simple first-order high-pass_filter, with the cut-
off frequency set to be far above the highest frequency in the signal. This is
a four-terminal network consisting of two passive elements as shown in
figures 1 and 2.
**** Transfer function[edit] ****
The analysis here is for the capacitive circuit in figure 1. The inductive case
in figure 2 can be handled in a similar way.
The transfer_function shows the dependence of the network gain on the signal
frequency for sinusoidal signals.
According to Ohm's_law,
         Y = X    Z  R     Z  R   +  Z  C      = X   R  R +   1  j &#x03C9; C
      = X   1  1 +   1  j &#x03C9; R C       ,   {\displaystyle Y=X{\frac {Z_
      {R}}{Z_{R}+Z_{C}}}=X{\frac {R}{R+{\frac {1}{j\omega C}}}}=X{\frac {1}{1+
      {\frac {1}{j\omega RC}}}},}  [Y=X{\frac  {Z_{R}}{Z_{R}+Z_{C}}}=X{\frac
      {R}{R+{\frac  {1}{j\omega C}}}}=X{\frac  {1}{1+{\frac  {1}{j\omega
      RC}}}},]
where     X   {\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y] are
input and output signals' amplitudes respectively, and      Z  R
{\displaystyle Z_{R}}  [Z_{R}] and      Z  C     {\displaystyle Z_{C}}  [Z_{C}]
are the resistor's and capacitor's impedances. Therefore, the complex transfer
function is
         K ( j &#x03C9; ) =   1  1 +   1  j &#x03C9; R C       =   1  1 +
      &#x03C9;  0    j &#x03C9;       ,   {\displaystyle K(j\omega )={\frac {1}
      {1+{\frac {1}{j\omega RC}}}}={\frac {1}{1+{\frac {\omega _{0}}{j\omega
      }}}},}  [K(j\omega )={\frac  {1}{1+{\frac  {1}{j\omega RC}}}}={\frac  {1}
      {1+{\frac  {\omega _{0}}{j\omega }}}},]
where
          &#x03C9;  0   =   1  R C    .   {\displaystyle \omega _{0}={\frac {1}
      {RC}}.}  [\omega _{0}={\frac  {1}{RC}}.]
The amplitude transfer function
         H ( &#x03C9; ) &#x225C;  |  K ( j &#x03C9; )  |  =   1  1 +
      (    &#x03C9;  0   &#x03C9;   )   2      ,   {\displaystyle H(\omega
      )\triangleq |K(j\omega )|={\frac {1}{\sqrt {1+\left({\frac {\omega _{0}}
      {\omega }}\right)^{2}}}},}  [{\displaystyle H(\omega )\triangleq |K
      (j\omega )|={\frac {1}{\sqrt {1+\left({\frac {\omega _{0}}{\omega
      }}\right)^{2}}}},}]
and the phase transfer function
         &#x03D5; ( &#x03C9; ) &#x225C; arg &#x2061; K ( j &#x03C9; ) = arctan
      &#x2061;    &#x03C9;  0   &#x03C9;   ,   {\displaystyle \phi (\omega
      )\triangleq \arg K(j\omega )=\arctan {\frac {\omega _{0}}{\omega }},}
      [\phi (\omega )\triangleq \arg K(j\omega )=\arctan {\frac  {\omega _{0}}
      {\omega }},]
which are both shown in Figure 3.
Figure 3: Amplitude and phase transfer functions for a passive differentiator
circuit
Transfer functions for the second circuit are the same (with      &#x03C9;  0
=   R L     {\displaystyle \omega _{0}={\frac {R}{L}}}  [\omega _{0}={\frac
{R}{L}}]).
**** Impulse response[edit] ****
The circuit's impulse_response, which is shown in figure 4, can be derived as
an inverse Laplace_transform of the complex transfer function:
         h ( t ) =    L    &#x2212; 1    {  K ( p )  }  = &#x03B4; ( t )
      &#x2212;  &#x03C9;  0    e  &#x2212;  &#x03C9;  0   t   = &#x03B4; ( t )
      &#x2212;   1 &#x03C4;    e  &#x2212;   t &#x03C4;       {\displaystyle h
      (t)={\mathcal {L}}^{-1}\left\{K(p)\right\}=\delta (t)-\omega _{0}e^{-
      \omega _{0}t}=\delta (t)-{\frac {1}{\tau }}e^{-{\frac {t}{\tau }}}}  [h
      (t)={\mathcal  {L}}^{{-1}}\left\{K(p)\right\}=\delta (t)-\omega _{0}e^{{-
      \omega _{0}t}}=\delta (t)-{\frac  {1}{\tau }}e^{{-{\frac  {t}{\tau }}}}]
where     &#x03C4; =   1  &#x03C9;  0       {\displaystyle \tau ={\frac {1}
{\omega _{0}}}}  [\tau ={\frac  {1}{\omega _{0}}}] is a time constant, and
&#x03B4; ( t )   {\displaystyle \delta (t)}  [\delta (t)] is a delta_function.
Figure 4: An impulse response of a passive differentiator circuit
***** Active differentiator[edit] *****
**** Ideal differentiator[edit] ****
[Opampdifferentiating.svg]
A differentiator circuit (also known as a differentiating amplifier) consists
of an operational_amplifier in which a resistor R provides negative_feedback
and a capacitor is used at the input side. The circuit is based on the
capacitor's current to voltage relationship
         V = V ( &#x221E; ) + [ ( V ( 0 + ) &#x2212; V ( &#x221E; ) ]  e
      &#x2212;   t &#x03C4;     ,   {\displaystyle V=V(\infty )+[(V(0+)-V
      (\infty )]e^{-{\frac {t}{\tau }}},}  [{\displaystyle V=V(\infty )+[(V
      (0+)-V(\infty )]e^{-{\frac {t}{\tau }}},}]
         I = C    d V   d t    ,   {\displaystyle I=C{\frac {dV}{dt}},}  [
      {\displaystyle I=C{\frac {dV}{dt}},}]
where I is the current through the capacitor, C is the capacitance of the
capacitor, and V is the voltage across the capacitor. The current flowing
through the capacitor is then proportional to the derivative of the voltage
across the capacitor. This current can then be connected to a resistor, which
has the current to voltage relationship
         I =   V R   ,   {\displaystyle I={\frac {V}{R}},}  [I={\frac {V}{R}},]
where R is the resistance of the resistor.
Note that the op amp input has a very high input impedance (it also forms a
virtual_ground due to the presence of negative feedback), so the entire input
current has to flow through R.
If Vout is the voltage across the resistor and Vin is the voltage across the
capacitor, we can rearrange these two equations to obtain the following
equation:
          V  out   = &#x2212; R C    d  V  in     d t    .   {\displaystyle V_
      {\text{out}}=-RC{\frac {dV_{\text{in}}}{dt}}.}  [{\displaystyle V_{\text
      {out}}=-RC{\frac {dV_{\text{in}}}{dt}}.}]
From the above equation following conclusions can be made:
    * Output is proportional to the time derivative of the input. Hence, the op
      amp acts as a differentiator.
    * Above equation is true for any frequency signal.
    * The negative sign indicates that there is 180Â° phase shift in the output
      with respect to the input,
Thus, it can be shown that in an ideal situation the voltage across the
resistor will be proportional to the derivative of the voltage across the
capacitor with a gain of RC.
*** Operation[edit] ***
Input signals are applied to the capacitor C. Capacitive reactance is the
important factor in the analysis of the operation of a differentiator.
Capacitive reactance is Xc = 1/2ÏfC. Capacitive reactance is inversely
proportional to the rate of change of input voltage applied to the capacitor.
At low frequency, the reactance of a capacitor is high, and at high frequency
reactance is low. Therefore, at low frequencies and for slow changes in input
voltage, the gain, Rf/Xc, is low, while at higher frequencies and for fast
changes the gain is high, producing larger output voltages.
If a constant DC voltage is applied as input, then the output voltage is zero.
If the input voltage changes from zero to negative, the output voltage is
positive. If the applied input voltage changes from zero to positive, the
output voltage is negative. If a square-wave input is applied to a
differentiator, then a spike waveform is obtained at the output.
The active differentiator isolates the load of the succeeding stages, so it has
the same response independent of the load.
*** Frequency response[edit] ***
[Bode_Plot_(Frequency_Response)_of_an_Ideal_Differentiator.png]
*** Advantages[edit] ***
A small time constant is sufficient to cause differentiation of the input
signal
*** Limitations[edit] ***
At high frequencies:
    * this simple differentiator circuit becomes unstable and starts to
      oscillate;
    * the circuit becomes sensitive to noise, that is, when amplified, noise
      dominates the input/message signal.
**** Practical differentiator[edit] ****
[Practical_Differentiator_Circuit_Diagram.png]
In order to overcome the limitations of the ideal differentiator, an additional
small-value capacitor C1 is connected across the feedback resistor R, which
avoids the differentiator circuit to run into oscillations (that is, become
unstable), and a resistor R1 is connected in series with the capacitor C, which
limits the increase in gain to a ratio of R/R1.
Since negative feedback is present through the resistor R, we can apply the
virtual_ground concept, that is, the voltage at the inverting terminal =
voltage at the non-inverting terminal = 0.
Applying nodal analysis, we get
            0 &#x2212; V 0  R   +    0 &#x2212; V 0   1  s C 1     +    0
      &#x2212; V i   R 1 +   1  s C       = 0 ,   {\displaystyle {\frac {0-V0}
      {R}}+{\frac {0-V0}{\frac {1}{sC1}}}+{\frac {0-Vi}{R1+{\frac {1}
      {sC}}}}=0,}  [{\displaystyle {\frac {0-V0}{R}}+{\frac {0-V0}{\frac {1}
      {sC1}}}+{\frac {0-Vi}{R1+{\frac {1}{sC}}}}=0,}]
         &#x2212; V 0  (    1 R   + s C 1  )  =    V i   R 1 +   1  s C       .
      {\displaystyle -V0\left({\frac {1}{R}}+sC1\right)={\frac {Vi}{R1+{\frac
      {1}{sC}}}}.}  [{\displaystyle -V0\left({\frac {1}{R}}+sC1\right)={\frac
      {Vi}{R1+{\frac {1}{sC}}}}.}]
Therefore,
            V 0   V i    =    &#x2212; s R C   ( 1 + s R 1 C ) ( 1 + s R C 1 )
      .   {\displaystyle {\frac {V0}{Vi}}={\frac {-sRC}{(1+sR1C)(1+sRC1)}}.}  [
      {\displaystyle {\frac {V0}{Vi}}={\frac {-sRC}{(1+sR1C)(1+sRC1)}}.}]
Hence, there occurs one zero at     s = 0   {\displaystyle s=0}  [s=0] and two
poles at     s = f 1 =    1  2 &#x03C0; R 1 C       {\displaystyle s=f1={\tfrac
{1}{2\pi R1C}}}  [{\displaystyle s=f1={\tfrac {1}{2\pi R1C}}}] and     s = f 2
=    1  2 &#x03C0; R C 1       {\displaystyle s=f2={\tfrac {1}{2\pi RC1}}}  [
{\displaystyle s=f2={\tfrac {1}{2\pi RC1}}}].
*** Frequency response[edit] ***
[Bode_Plot_of_Practical_Differentiator.png]
From the above plot, it can be seen that:
    * when     f < f 1   {\displaystyle f<f1}  [{\displaystyle f<f1}], the
      circuit acts as a differentiator;
    * when     f 1 < f < f 2   {\displaystyle f1<f<f2}  [{\displaystyle
      f1<f<f2}], the circuit acts as a voltage_follower or buffer;
    * when     f > f 2   {\displaystyle f>f2}  [{\displaystyle f>f2}], the
      circuit acts as an integrator.
If     R C 1 = R 1 C = R C   {\displaystyle RC1=R1C=RC}  [{\displaystyle
RC1=R1C=RC}] (say), there occurs one zero at     s = 0   {\displaystyle s=0}
[s=0] and two poles at     s = f a =   1  2 &#x03C0; R C      {\displaystyle
s=fa={\frac {1}{2\pi RC}}}  [{\displaystyle s=fa={\frac {1}{2\pi RC}}}].
For such a differentiator circuit, the frequency response would be
[Bode_Plot_of_Practical_Differentiator_when_RC1=R1C.png]
From the above plot, we observe that:
    * when     f < f a   {\displaystyle f<fa}  [{\displaystyle f<fa}], the
      circuit acts as a differentiator;
    * when     f > f a   {\displaystyle f>fa}  [{\displaystyle f>fa}], the
      circuit acts as an integrator.
**** Applications[edit] ****
The differentiator circuit is essentially a high-pass_filter. It can generate a
square_wave from a triangle_wave input and produce alternating-direction
voltage spikes when a square wave is applied. In ideal cases, a differentiator
reverses the effects of an integrator on a waveform, and conversely. Hence,
they are most commonly used in wave-shaping_circuits to detect high-frequency
components in an input signal. Differentiators are an important part of
electronic analogue_computers and analogue PID_controllers. They are also used
in frequency_modulators as rate-of-change detectors.
A passive differentiator circuit is one of the basic electronic_circuits, being
widely used in circuit analysis based on the equivalent_circuit method.
***** See also[edit] *****
    * Integrator
    * Inverting_differentiator at op amp applications
***** References[edit] *****

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Differentiator&oldid=903530719"
Categories:
    * Analog_circuits
Hidden categories:
    * Articles_needing_additional_references_from_December_2009
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * ÄeÅ¡tina
    * Italiano
    * æ¥æ¬èª
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 26 June 2019, at 06:25 (UTC).
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
