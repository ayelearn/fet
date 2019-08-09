The following text has been accessed from https://en.wikipedia.org/wiki/Bode_plot at Thu Aug 8 22:54:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Bode plot ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article needs additional citations for verification. Please help improve_this_article by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and removed.
 Find sources: "Bode_plot" â news Â· newspapers Â· books Â· scholar Â· JSTOR (December 2011)
 (Learn_how_and_when_to_remove_this_template_message)
Figure 1(a): The Bode plot for a first-order (one-pole) highpass_filter; the
straight-line approximations are labeled "Bode pole"; phase varies from 90Â° at
low frequencies (due to the contribution of the numerator, which is 90Â° at all
frequencies) to 0Â° at high frequencies (where the phase contribution of the
denominator is −90Â° and cancels the contribution of the numerator).
Figure 1(b): The Bode plot for a first-order (one-pole) lowpass_filter; the
straight-line approximations are labeled "Bode pole"; phase is 90Â° lower than
for Figure 1(a) because the phase contribution of the numerator is 0Â° at all
frequencies.
In electrical_engineering and control_theory, a Bode plot /ËboÊdi/ is a graph
of the frequency_response of a system. It is usually a combination of a Bode
magnitude plot, expressing the magnitude (usually in decibels) of the frequency
response, and a Bode phase plot, expressing the phase_shift.
As originally conceived by Hendrik_Wade_Bode in the 1930s, the plot is an
asymptotic approximation of the frequency response, using_straight_line
segments.[1]
⁰
***** Contents *****
    * 1_Overview
    * 2_Definition
    * 3_Frequency_response
    * 4_Rules_for_handmade_Bode_plot
          o 4.1_Straight-line_amplitude_plot
          o 4.2_Corrected_amplitude_plot
          o 4.3_Straight-line_phase_plot
    * 5_Example
          o 5.1_Magnitude_plot
          o 5.2_Phase_plot
          o 5.3_Normalized_plot
    * 6_An_example_with_zero_and_pole
    * 7_Gain_margin_and_phase_margin
          o 7.1_Examples_using_Bode_plots
    * 8_Bode_plotter
    * 9_Related_plots
    * 10_Appendix
          o 10.1_Proof_for_the_relation_to_frequency_response
    * 11_See_also
    * 12_Notes
    * 13_References
    * 14_External_links
***** Overview[edit] *****
Among his several important contributions to circuit theory and control theory,
engineer Hendrik_Wade_Bode, while working at Bell Labs in the United States in
the 1930s, devised a simple but accurate method for graphing gain and phase-
shift plots. These bear his name, Bode gain plot and Bode phase plot. "Bode" is
often pronounced /ËboÊdi/ BOH-dee although the Dutch pronunciation is Bo-duh.
(Dutch: [ËboËdÉ]).[2][3]
Bode was faced with the problem of designing stable amplifiers with feedback
for use in telephone networks. He developed the graphical design technique of
the Bode plots to show the gain_margin and phase_margin required to maintain
stability under variations in circuit characteristics caused during manufacture
or during operation.[4] The principles developed were applied to design
problems of servomechanisms and other feedback control systems. The Bode plot
is an example of analysis in the frequency_domain.
***** Definition[edit] *****
The Bode plot for a linear,_time-invariant system with transfer_function     H
( s )   {\displaystyle H(s)}  [H(s)] (    s   {\displaystyle s}  [s] being the
complex frequency in the Laplace_domain) consists of a magnitude plot and a
phase plot.
The Bode magnitude plot is the graph of the function      |  H ( s = j &#x03C9;
)  |    {\displaystyle |H(s=j\omega )|}  [|H(s=j\omega )|] of frequency
&#x03C9;   {\displaystyle \omega }  [\omega ] (with     j   {\displaystyle j}
[j] being the imaginary_unit). The     &#x03C9;   {\displaystyle \omega }
[\omega ]-axis of the magnitude plot is logarithmic and the magnitude is given
in decibels, i.e., a value for the magnitude      |  H  |    {\displaystyle
|H|}  [|H|] is plotted on the axis at     20  log  10   &#x2061;  |  H  |
{\displaystyle 20\log _{10}|H|}  [20\log _{10}|H|].
The Bode phase plot is the graph of the phase, commonly expressed in degrees,
of the transfer function     arg &#x2061;  (  H ( s = j &#x03C9; )  )
{\displaystyle \arg \left(H(s=j\omega )\right)}  [\arg \left(H(s=j\omega
)\right)] as a function of     &#x03C9;   {\displaystyle \omega }  [\omega ].
The phase is plotted on the same logarithmic     &#x03C9;   {\displaystyle
\omega }  [\omega ]-axis as the magnitude plot, but the value for the phase is
plotted on a linear vertical axis.
***** Frequency response[edit] *****
This section illustrates that a Bode Plot is a visualization of the frequency
response of a system.
Consider a linear,_time-invariant system with transfer function     H ( s )
{\displaystyle H(s)}  [H(s)]. Assume that the system is subject to a sinusoidal
input with frequency     &#x03C9;   {\displaystyle \omega }  [\omega ],
               u ( t ) = sin &#x2061; ( &#x03C9; t )  ,   {\displaystyle u
            (t)=\sin(\omega t)\;,}  [u(t) = \sin (\omega t) \; ,]
that is applied persistently, i.e. from a time     &#x2212; &#x221E;
{\displaystyle -\infty }  [-\infty ] to a time     t   {\displaystyle t}  [t].
The response will be of the form
               y ( t ) =  y  0   sin &#x2061; ( &#x03C9; t + &#x03C6; )  ,
            {\displaystyle y(t)=y_{0}\sin(\omega t+\varphi )\;,}  [y(t) = y_0
            \sin (\omega t + \varphi) \;, ]
i.e., also a sinusoidal signal with amplitude      y  0     {\displaystyle y_
{0}}  [y_{0}] shifted in phase with respect to the input by a phase
&#x03C6;   {\displaystyle \varphi }  [\varphi ].
It can be shown[5] that the magnitude of the response is
                y  0   =  |  H (  j  &#x03C9; )  |     {\displaystyle    
            y_{0}=|H(\mathrm {j} \omega )|\;}  [y_0 = |H(\mathrm{j}        (1)
            \omega)| \; ]
and that the phase shift is
               &#x03C6; = arg &#x2061; H (  j  &#x03C9; )  .             
            {\displaystyle \varphi =\arg H(\mathrm {j} \omega )\;.}        (2)
            [\varphi = \arg H(\mathrm{j} \omega) \;. ]
A sketch for the proof of these equations is given in the appendix.
In summary, subjected to an input with frequency     &#x03C9;   {\displaystyle
\omega }  [\omega ] the system responds at the same frequency with an output
that is amplified by a factor      |  H (  j  &#x03C9; )  |    {\displaystyle
|H(\mathrm {j} \omega )|}  [|H(\mathrm{j} \omega)|] and phase-shifted by
arg &#x2061; ( H (  j  &#x03C9; ) )   {\displaystyle \arg(H(\mathrm {j} \omega
))}  [\arg( H(\mathrm{j} \omega) )]. These quantities, thus, characterize the
frequency response and are shown in the Bode plot.
***** Rules for handmade Bode plot[edit] *****
For many practical problems, the detailed Bode plots can be approximated with
straight-line segments that are asymptotes of the precise response. The effect
of each of the terms of a multiple element transfer_function can be
approximated by a set of straight lines on a Bode plot. This allows a graphical
solution of the overall frequency response function. Before widespread
availability of digital computers, graphical methods were extensively used to
reduce the need for tedious calculation; a graphical solution could be used to
identify feasible ranges of parameters for a new design.
The premise of a Bode plot is that one can consider the log of a function in
the form:
         f ( x ) = A &#x220F; ( x &#x2212;  c  n    )   a  n
      {\displaystyle f(x)=A\prod (x-c_{n})^{a_{n}}}  [f(x)=A\prod (x-c_{n})^{
      {a_{n}}}]
as a sum of the logs of its zeros_and_poles:
         log &#x2061; ( f ( x ) ) = log &#x2061; ( A ) + &#x2211;  a  n   log
      &#x2061; ( x &#x2212;  c  n   )  .   {\displaystyle \log(f(x))=\log
      (A)+\sum a_{n}\log(x-c_{n})\;.}  [\log(f(x))=\log(A)+\sum a_{n}\log(x-c_
      {n})\;.]
This idea is used explicitly in the method for drawing phase diagrams. The
method for drawing amplitude plots implicitly uses this idea, but since the log
of the amplitude of each pole or zero always starts at zero and only has one
asymptote change (the straight lines), the method can be simplified.
**** Straight-line amplitude plot[edit] ****
Amplitude decibels is usually done using      d B  = 20  log  10   &#x2061; ( X
)   {\displaystyle \mathbf {dB} =20\log _{10}(X)}  [{\mathbf  {dB}}=20\log _{
{10}}(X)] to define decibels. Given a transfer function in the form
         H ( s ) = A &#x220F;    ( s &#x2212;  x  n    )   a  n       ( s
      &#x2212;  y  n    )   b  n          {\displaystyle H(s)=A\prod {\frac {
      (s-x_{n})^{a_{n}}}{(s-y_{n})^{b_{n}}}}}  [H(s)=A\prod {\frac  {(s-x_{n})^
      {{a_{n}}}}{(s-y_{n})^{{b_{n}}}}}]
where      x  n     {\displaystyle x_{n}}  [x_{n}] and      y  n
{\displaystyle y_{n}}  [y_{n}] are constants,     s =  j  &#x03C9;
{\displaystyle s=\mathrm {j} \omega }  [s={\mathrm  {j}}\omega ],      a  n   ,
b  n   > 0   {\displaystyle a_{n},b_{n}>0}  [a_n, b_n > 0], and     H
{\displaystyle H}  [H] is the transfer function:
    * at every value of s where     &#x03C9; =  x  n     {\displaystyle \omega
      =x_{n}}  [\omega = x_n] (a zero), increase the slope of the line by
      20 &#x22C5;  a  n     d B    {\displaystyle 20\cdot a_{n}\,\mathrm {dB} }
      [20\cdot a_{n}\,{\mathrm  {dB}}] per decade.
    * at every value of s where     &#x03C9; =  y  n     {\displaystyle \omega
      =y_{n}}  [\omega = y_n] (a pole), decrease the slope of the line by
      20 &#x22C5;  b  n     d B    {\displaystyle 20\cdot b_{n}\,\mathrm {dB} }
      [20\cdot b_{n}\,{\mathrm  {dB}}] per decade.
    * The initial value of the graph depends on the boundaries. The initial
      point is found by putting the initial angular frequency     &#x03C9;
      {\displaystyle \omega }  [\omega ] into the function and finding      |
      H (  j  &#x03C9; )  |    {\displaystyle |H(\mathrm {j} \omega )|}  [|H(
      {\mathrm  {j}}\omega )|].
    * The initial slope of the function at the initial value depends on the
      number and order of zeros and poles that are at values below the initial
      value, and is found using the first two rules.
To handle irreducible 2nd order polynomials,     a  x  2   + b x + c
{\displaystyle ax^{2}+bx+c}  [ax^{2}+bx+c] can, in many cases, be approximated
as     (   a   x +   c    )  2     {\displaystyle ({\sqrt {a}}x+{\sqrt {c}})^
{2}}  [ (\sqrt{a}x + \sqrt{c})^2 ].
Note that zeros and poles happen when     &#x03C9;   {\displaystyle \omega }
[\omega ] is equal to a certain      x  n     {\displaystyle x_{n}}  [x_{n}] or
y  n     {\displaystyle y_{n}}  [y_{n}]. This is because the function in
question is the magnitude of     H (  j  &#x03C9; )   {\displaystyle H(\mathrm
{j} \omega )}  [H({\mathrm  {j}}\omega )], and since it is a complex function,
|  H (  j  &#x03C9; )  |  =   H &#x22C5;  H  &#x2217;       {\displaystyle |H
(\mathrm {j} \omega )|={\sqrt {H\cdot H^{*}}}}  [|H({\mathrm  {j}}\omega )|=
{\sqrt  {H\cdot H^{*}}}]. Thus at any place where there is a zero or pole
involving the term     ( s +  x  n   )   {\displaystyle (s+x_{n})}  [(s+x_
{n})], the magnitude of that term is       (  x  n   +  j  &#x03C9; ) &#x22C5;
(  x  n   &#x2212;  j  &#x03C9; )   =    x  n   2   +  &#x03C9;  2
{\displaystyle {\sqrt {(x_{n}+\mathrm {j} \omega )\cdot (x_{n}-\mathrm {j}
\omega )}}={\sqrt {x_{n}^{2}+\omega ^{2}}}}  [{\sqrt  {(x_{n}+{\mathrm
{j}}\omega )\cdot (x_{n}-{\mathrm  {j}}\omega )}}={\sqrt  {x_{n}^{2}+\omega ^
{2}}}].
**** Corrected amplitude plot[edit] ****
To correct a straight-line amplitude plot:
    * at every zero, put a point     3 &#x22C5;  a  n   &#xA0;  d B
      {\displaystyle 3\cdot a_{n}\ \mathrm {dB} }  [3 \cdot a_n\ \mathrm{dB}]
      above the line,
    * at every pole, put a point     3 &#x22C5;  b  n   &#xA0;  d B
      {\displaystyle 3\cdot b_{n}\ \mathrm {dB} }  [3 \cdot b_n\ \mathrm{dB}]
      below the line,
    * draw a smooth curve through those points using the straight lines as
      asymptotes (lines which the curve approaches).
Note that this correction method does not incorporate how to handle complex
values of      x  n     {\displaystyle x_{n}}  [x_{n}] or      y  n
{\displaystyle y_{n}}  [y_{n}]. In the case of an irreducible polynomial, the
best way to correct the plot is to actually calculate the magnitude of the
transfer function at the pole or zero corresponding to the irreducible
polynomial, and put that dot over or under the line at that pole or zero.
**** Straight-line phase plot[edit] ****
Given a transfer function in the same form as above:
         H ( s ) = A &#x220F;    ( s &#x2212;  x  n    )   a  n       ( s
      &#x2212;  y  n    )   b  n          {\displaystyle H(s)=A\prod {\frac {
      (s-x_{n})^{a_{n}}}{(s-y_{n})^{b_{n}}}}}  [H(s)=A\prod {\frac  {(s-x_{n})^
      {{a_{n}}}}{(s-y_{n})^{{b_{n}}}}}]
the idea is to draw separate plots for each pole and zero, then add them up.
The actual phase curve is given by     &#x2212; arctan &#x2061;  (      I m
[ H ( s ) ]    R e  [ H ( s ) ]     )    {\displaystyle -\arctan \left({\tfrac
{\mathrm {Im} [H(s)]}{\mathrm {Re} [H(s)]}}\right)}  [-\arctan \left({\tfrac  {
{\mathrm  {Im}}[H(s)]}{{\mathrm  {Re}}[H(s)]}}\right)].
To draw the phase plot, for each pole and zero:
    * if     A   {\displaystyle A}  [A] is positive, start line (with zero
      slope) at     0 deg   {\displaystyle 0\deg }  [0\deg ]
    * if     A   {\displaystyle A}  [A] is negative, start line (with zero
      slope) at     &#x2212; 180 deg   {\displaystyle -180\deg }  [
      {\displaystyle -180\deg }]
    * if the sum of the number of unstable zeros and poles is odd, add 180
      degrees to that basis
    * at every     &#x03C9; =  |   x  n    |    {\displaystyle \omega =|x_{n}|}
      [ \omega = |x_n| ] (for stable zeros â     Re &#x2061; ( z ) < 0
      {\displaystyle \operatorname {Re} (z)<0}  [\operatorname {Re}(z)<0]),
      increase the slope by     45 &#x22C5;  a  n     {\displaystyle 45\cdot a_
      {n}}  [45 \cdot a_n] degrees per decade, beginning one decade before
      &#x03C9; =  |   x  n    |    {\displaystyle \omega =|x_{n}|}  [ \omega =
      |x_n| ] (E.g.:         |   x  n    |   10     {\displaystyle {\frac {|x_
      {n}|}{10}}}  [ \frac{|x_n|}{10} ])
    * at every     &#x03C9; =  |   y  n    |    {\displaystyle \omega =|y_{n}|}
      [ \omega = |y_n| ] (for stable poles â     Re &#x2061; ( p ) < 0
      {\displaystyle \operatorname {Re} (p)<0}  [\operatorname {Re}(p)<0]),
      decrease the slope by     45 &#x22C5;  b  n     {\displaystyle 45\cdot b_
      {n}}  [45 \cdot b_n] degrees per decade, beginning one decade before
      &#x03C9; =  |   y  n    |    {\displaystyle \omega =|y_{n}|}  [ \omega =
      |y_n| ] (E.g.:         |   y  n    |   10     {\displaystyle {\frac {|y_
      {n}|}{10}}}  [ \frac{|y_n|}{10} ])
    * "unstable" (right half plane) poles and zeros (    Re &#x2061; ( s ) > 0
      {\displaystyle \operatorname {Re} (s)>0}  [\operatorname {Re}(s)>0]) have
      opposite behavior
    * flatten the slope again when the phase has changed by     90 &#x22C5;  a
      n     {\displaystyle 90\cdot a_{n}}  [90 \cdot a_n] degrees (for a zero)
      or     90 &#x22C5;  b  n     {\displaystyle 90\cdot b_{n}}  [90 \cdot
      b_n] degrees (for a pole),
    * After plotting one line for each pole or zero, add the lines together to
      obtain the final phase plot; that is, the final phase plot is the
      superposition of each earlier phase plot.
***** Example[edit] *****
To create a straight-line plot for a first-order (one-pole) lowpass filter, one
considers the transfer function in terms of the angular frequency:
          H   l p    (  j  &#x03C9; ) =   1  1 +  j    &#x03C9;   &#x03C9;   c
      .   {\displaystyle H_{\mathrm {lp} }(\mathrm {j} \omega )={1 \over
      1+\mathrm {j} {\omega \over {\omega _{\mathrm {c} }}}}\;.}  [H_{\mathrm
      {lp}}(\mathrm{j} \omega)  = {1 \over 1 + \mathrm{j}{\omega \over {
      {\omega_\mathrm{c}}}}} \; .]
The above equation is the normalized form of the transfer function. The Bode
plot is shown in Figure 1(b) above, and construction of the straight-line
approximation is discussed next.
**** Magnitude plot[edit] ****
The magnitude (in decibels) of the transfer function above, (normalized and
converted to angular frequency form), given by the decibel gain expression
A   v d B      {\displaystyle A_{\mathrm {vdB} }}  [A_\mathrm{vdB}]:
              A   v d B       = 20 &#x22C5; log &#x2061;  |   H   l p    (  j
      &#x03C9; )  |        = 20 &#x22C5; log &#x2061;   1  |  1 +  j
      &#x03C9;  &#x03C9;   c       |          = &#x2212; 20 &#x22C5; log
      &#x2061;  |  1 +  j    &#x03C9;  &#x03C9;   c       |        = &#x2212;
      10 &#x22C5; log &#x2061;  (  1 +    &#x03C9;  2    &#x03C9;   c    2
      )        {\displaystyle {\begin{aligned}A_{\mathrm {vdB} }&=20\cdot \log
      |H_{\mathrm {lp} }(\mathrm {j} \omega )|\\&=20\cdot \log {\frac {1}
      {\left|1+\mathrm {j} {\frac {\omega }{\omega _{\mathrm {c}
      }}}\right|}}\\&=-20\cdot \log \left|1+\mathrm {j} {\frac {\omega }{\omega
      _{\mathrm {c} }}}\right|\\&=-10\cdot \log \left(1+{\frac {\omega ^{2}}
      {\omega _{\mathrm {c} }^{2}}}\right)\end{aligned}}}  [\begin{align}
      A_\mathrm{vdB} &= 20 \cdot \log|H_{\mathrm{lp}}(\mathrm{j}\omega)| \\
          &= 20 \cdot \log \frac{1}{\left| 1 + \mathrm{j} \frac{\omega}
      {\omega_\mathrm{c}} \right|} \\
          &= -20 \cdot \log \left| 1 + \mathrm{j} \frac{\omega}{\omega_\mathrm
      {c}} \right| \\
          &= -10 \cdot \log \left( 1 + \frac{\omega^2}{\omega_\mathrm{c}^2}
      \right)
      \end{align}]
then plotted versus input frequency     &#x03C9;   {\displaystyle \omega }
[\omega ] on a logarithmic scale, can be approximated by two lines and it forms
the asymptotic (approximate) magnitude Bode plot of the transfer function:
    * for angular frequencies below      &#x03C9;   c      {\displaystyle
      \omega _{\mathrm {c} }}  [\omega_\mathrm{c}] it is a horizontal line at
      0 dB since at low frequencies the       &#x03C9;   &#x03C9;   c
      {\displaystyle {\omega \over {\omega _{\mathrm {c} }}}}  [{\omega \over
      {\omega_\mathrm{c}}}] term is small and can be neglected, making the
      decibel gain equation above equal to zero,
    * for angular frequencies above      &#x03C9;   c      {\displaystyle
      \omega _{\mathrm {c} }}  [\omega_\mathrm{c}] it is a line with a slope of
      â20 dB per decade since at high frequencies the       &#x03C9;
      &#x03C9;   c         {\displaystyle {\omega \over {\omega _{\mathrm {c}
      }}}}  [{\omega \over {\omega_\mathrm{c}}}] term dominates and the decibel
      gain expression above simplifies to     &#x2212; 20 log &#x2061;
      &#x03C9;   &#x03C9;   c         {\displaystyle -20\log {\omega \over
      {\omega _{\mathrm {c} }}}}  [-20 \log {\omega \over {\omega_\mathrm{c}}}]
      which is a straight line with a slope of     &#x2212; 20   d B
      {\displaystyle -20\,\mathrm {dB} }  [-20\,{\mathrm  {dB}}] per decade.
These two lines meet at the corner_frequency. From the plot, it can be seen
that for frequencies well below the corner frequency, the circuit has an
attenuation of 0 dB, corresponding to a unity pass band gain, i.e. the
amplitude of the filter output equals the amplitude of the input. Frequencies
above the corner frequency are attenuated â the higher the frequency, the
higher the attenuation.
**** Phase plot[edit] ****
The phase Bode plot is obtained by plotting the phase angle of the transfer
function given by
         arg &#x2061;  H   l p    (  j  &#x03C9; ) = &#x2212;  tan  &#x2212; 1
      &#x2061;   &#x03C9;   &#x03C9;   c         {\displaystyle \arg H_{\mathrm
      {lp} }(\mathrm {j} \omega )=-\tan ^{-1}{\omega \over {\omega _{\mathrm
      {c} }}}}  [\arg H_{\mathrm{lp}}(\mathrm{j} \omega) = -\tan^{-1}{\omega
      \over {\omega_\mathrm{c}}}]
versus     &#x03C9;   {\displaystyle \omega }  [\omega ], where     &#x03C9;
{\displaystyle \omega }  [\omega ] and      &#x03C9;   c      {\displaystyle
\omega _{\mathrm {c} }}  [\omega_\mathrm{c}] are the input and cutoff angular
frequencies respectively. For input frequencies much lower than corner, the
ratio       &#x03C9;   &#x03C9;   c         {\displaystyle {\omega \over
{\omega _{\mathrm {c} }}}}  [ {\omega \over {\omega_\mathrm{c}}}] is small and
therefore the phase angle is close to zero. As the ratio increases the absolute
value of the phase increases and becomes â45 degrees when     &#x03C9; =
&#x03C9;   c      {\displaystyle \omega =\omega _{\mathrm {c} }}  [\omega
=\omega_\mathrm{c}]. As the ratio increases for input frequencies much greater
than the corner frequency, the phase angle asymptotically approaches −90
degrees. The frequency scale for the phase plot is logarithmic.
**** Normalized plot[edit] ****
The horizontal frequency axis, in both the magnitude and phase plots, can be
replaced by the normalized (nondimensional) frequency ratio       &#x03C9;
&#x03C9;   c         {\displaystyle {\omega \over {\omega _{\mathrm {c} }}}}  [
{\omega \over {\omega_\mathrm{c}}}]. In such a case the plot is said to be
normalized and units of the frequencies are no longer used since all input
frequencies are now expressed as multiples of the cutoff frequency
&#x03C9;   c      {\displaystyle \omega _{\mathrm {c} }}  [\omega_\mathrm{c}].
***** An example with zero and pole[edit] *****
Figures 2-5 further illustrate construction of Bode plots. This example with
both a pole and a zero shows how to use superposition. To begin, the components
are presented separately.
Figure 2 shows the Bode magnitude plot for a zero and a low-pass pole, and
compares the two with the Bode straight line plots. The straight-line plots are
horizontal up to the pole (zero) location and then drop (rise) at 20 dB/decade.
The second Figure 3 does the same for the phase. The phase plots are horizontal
up to a frequency factor of ten below the pole (zero) location and then drop
(rise) at 45Â°/decade until the frequency is ten times higher than the pole
(zero) location. The plots then are again horizontal at higher frequencies at a
final, total phase change of 90Â°.
Figure 4 and Figure 5 show how superposition (simple addition) of a pole and
zero plot is done. The Bode straight line plots again are compared with the
exact plots. The zero has been moved to higher frequency than the pole to make
a more interesting example. Notice in Figure 4 that the 20 dB/decade drop of
the pole is arrested by the 20 dB/decade rise of the zero resulting in a
horizontal magnitude plot for frequencies above the zero location. Notice in
Figure 5 in the phase plot that the straight-line approximation is pretty
approximate in the region where both pole and zero affect the phase. Notice
also in Figure 5 that the range of frequencies where the phase changes in the
straight line plot is limited to frequencies a factor of ten above and below
the pole (zero) location. Where the phase of the pole and the zero both are
present, the straight-line phase plot is horizontal because the 45Â°/decade
drop of the pole is arrested by the overlapping 45Â°/decade rise of the zero in
the limited range of frequencies where both are active contributors to the
phase.
    * Example with pole and zero
    * Figure 2: Bode magnitude plot for zero and low-pass pole; curves labeled
      "Bode" are the straight-line Bode plots
    * Figure 3: Bode phase plot for zero and low-pass pole; curves labeled
      "Bode" are the straight-line Bode plots
    * Figure 4: Bode magnitude plot for pole-zero combination; the location of
      the zero is ten times higher than in Figures 2 and 3; curves labeled
      "Bode" are the straight-line Bode plots
    * Figure 5: Bode phase plot for pole-zero combination; the location of the
      zero is ten times higher than in Figures 2 and 3; curves labeled "Bode"
      are the straight-line Bode plots
***** Gain margin and phase margin[edit] *****
See also: Phase_margin
Bode plots are used to assess the stability of negative_feedback_amplifiers by
finding the gain and phase_margins of an amplifier. The notion of gain and
phase margin is based upon the gain expression for a negative feedback
amplifier given by
                A   F B    =    A   O L     1 + &#x03B2;  A   O L        ,
            {\displaystyle A_{\mathrm {FB} }={\frac {A_{\mathrm {OL} }}{1+\beta
            A_{\mathrm {OL} }}}\;,}  [A_{{\mathrm  {FB}}}={\frac  {A_{{\mathrm
            {OL}}}}{1+\beta A_{{\mathrm  {OL}}}}}\;,]
where AFB is the gain of the amplifier with feedback (the closed-loop gain), Î²
is the feedback factor and AOL is the gain without feedback (the open-loop
gain). The gain AOL is a complex function of frequency, with both magnitude and
phase.[note_1] Examination of this relation shows the possibility of infinite
gain (interpreted as instability) if the product Î²AOL = −1. (That is, the
magnitude of Î²AOL is unity and its phase is −180Â°, the so-called Barkhausen
stability_criterion). Bode plots are used to determine just how close an
amplifier comes to satisfying this condition.
Key to this determination are two frequencies. The first, labeled here as f180,
is the frequency where the open-loop gain flips sign. The second, labeled here
f0 dB, is the frequency where the magnitude of the product | Î² AOL | = 1 (in
dB, magnitude 1 is 0 dB). That is, frequency f180 is determined by the
condition:
         &#x03B2;  A   O L     (  f  180   )  = &#x2212;  |  &#x03B2;  A   O L
      (  f  180   )   |  = &#x2212;  |  &#x03B2;  A   O L      |   180    ,
      {\displaystyle \beta A_{\mathrm {OL} }\left(f_{180}\right)=-|\beta A_
      {\mathrm {OL} }\left(f_{180}\right)|=-|\beta A_{\mathrm {OL} }|_{180}\;,}
      [\beta A_{{\mathrm  {OL}}}\left(f_{{180}}\right)=-|\beta A_{{\mathrm
      {OL}}}\left(f_{{180}}\right)|=-|\beta A_{{\mathrm  {OL}}}|_{{180}}\;,]
where vertical bars denote the magnitude of a complex number (for example,
|  a +  j  b  |  =   [   a  2   +  b  2    ]    1 2      {\displaystyle
|a+\mathrm {j} b|=\left[a^{2}+b^{2}\right]^{\frac {1}{2}}}  [|a+{\mathrm
{j}}b|=\left[a^{2}+b^{2}\right]^{{{\frac  12}}}]), and frequency f0 dB is
determined by the condition:
          |  &#x03B2;  A   O L     (  f   0 d B    )   |  = 1  .
      {\displaystyle |\beta A_{\mathrm {OL} }\left(f_{\mathrm {0dB}
      }\right)|=1\;.}  [|\beta A_{{\mathrm  {OL}}}\left(f_{{\mathrm
      {0dB}}}\right)|=1\;.]
One measure of proximity to instability is the gain margin. The Bode phase plot
locates the frequency where the phase of Î²AOL reaches −180Â°, denoted here as
frequency f180. Using this frequency, the Bode magnitude plot finds the
magnitude of Î²AOL. If |Î²AOL|180 = 1, the amplifier is unstable, as mentioned.
If AOL|180 < 1, instability does not occur, and the separation in dB of the
magnitude of |Î²AOL|180 from |Î²AOL| = 1 is called the gain margin. Because a
magnitude of one is 0 dB, the gain margin is simply one of the equivalent
forms:     20  log  10   &#x2061; (  |  &#x03B2;  A   O L      |   180   ) = 20
log  10   &#x2061; (  |   A   O L     |  ) &#x2212; 20  log  10   &#x2061;
(  &#x03B2;  &#x2212; 1   )   {\displaystyle 20\log _{10}(|\beta A_{\mathrm
{OL} }|_{180})=20\log _{10}(|A_{\mathrm {OL} }|)-20\log _{10}(\beta ^{-1})}  [
{\displaystyle 20\log _{10}(|\beta A_{\mathrm {OL} }|_{180})=20\log _{10}(|A_
{\mathrm {OL} }|)-20\log _{10}(\beta ^{-1})}].
Another equivalent measure of proximity to instability is the phase_margin. The
Bode magnitude plot locates the frequency where the magnitude of |Î²AOL|
reaches unity, denoted here as frequency f0 dB. Using this frequency, the Bode
phase plot finds the phase of Î²AOL. If the phase of Î²AOL( f0 dB) > −180Â°,
the instability condition cannot be met at any frequency (because its magnitude
is going to be < 1 when f = f180), and the distance of the phase at f0 dB in
degrees above −180Â° is called the phase margin.
If a simple yes or no on the stability issue is all that is needed, the
amplifier is stable if f0 dB < f180. This criterion is sufficient to predict
stability only for amplifiers satisfying some restrictions on their pole and
zero positions (minimum_phase systems). Although these restrictions usually are
met, if they are not another method must be used, such as the Nyquist_plot.[6]
[7] Optimal gain and phase margins may be computed using NevanlinnaâPick
interpolation theory.[8]
**** Examples using Bode plots[edit] ****
Figures 6 and 7 illustrate the gain behavior and terminology. For a three-pole
amplifier, Figure 6 compares the Bode plot for the gain without feedback (the
open-loop gain) AOL with the gain with feedback AFB (the closed-loop gain). See
negative_feedback_amplifier for more detail.
In this example, AOL = 100 dB at low frequencies, and 1 / Î² = 58 dB. At low
frequencies, AFB â 58 dB as well.
Because the open-loop gain AOL is plotted and not the product Î² AOL, the
condition AOL = 1 / Î² decides f0 dB. The feedback gain at low frequencies and
for large AOL is AFB â 1 / Î² (look at the formula for the feedback gain at
the beginning of this section for the case of large gain AOL), so an equivalent
way to find f0 dB is to look where the feedback gain intersects the open-loop
gain. (Frequency f0 dB is needed later to find the phase margin.)
Near this crossover of the two gains at f0 dB, the Barkhausen criteria are
almost satisfied in this example, and the feedback amplifier exhibits a massive
peak in gain (it would be infinity if Î² AOL = â1). Beyond the unity gain
frequency f0 dB, the open-loop gain is sufficiently small that AFB â AOL
(examine the formula at the beginning of this section for the case of small
AOL).
Figure 7 shows the corresponding phase comparison: the phase of the feedback
amplifier is nearly zero out to the frequency f180 where the open-loop gain has
a phase of â180Â°. In this vicinity, the phase of the feedback amplifier
plunges abruptly downward to become almost the same as the phase of the open-
loop amplifier. (Recall, AFB â AOL for small AOL.)
Comparing the labeled points in Figure 6 and Figure 7, it is seen that the
unity gain frequency f0 dB and the phase-flip frequency f180 are very nearly
equal in this amplifier, f180 â f0 dB â 3.332 kHz, which means the gain
margin and phase margin are nearly zero. The amplifier is borderline stable.
Figures 8 and 9 illustrate the gain margin and phase margin for a different
amount of feedback Î². The feedback factor is chosen smaller than in Figure 6
or 7, moving the condition | Î² AOL | = 1 to lower frequency. In this example,
1 / Î² = 77 dB, and at low frequencies AFB â 77 dB as well.
Figure 8 shows the gain plot. From Figure 8, the intersection of 1 / Î² and AOL
occurs at f0 dB = 1 kHz. Notice that the peak in the gain AFB near f0 dB is
almost gone.[note_2][9]
Figure 9 is the phase plot. Using the value of f0 dB = 1 kHz found above from
the magnitude plot of Figure 8, the open-loop phase at f0 dB is â135Â°, which
is a phase margin of 45Â° above â180Â°.
Using Figure 9, for a phase of â180Â° the value of f180 = 3.332 kHz (the same
result as found earlier, of course[note_3]). The open-loop gain from Figure 8
at f180 is 58 dB, and 1 / Î² = 77 dB, so the gain margin is 19 dB.
Stability is not the sole criterion for amplifier response, and in many
applications a more stringent demand than stability is good step_response. As a
rule_of_thumb, good step response requires a phase margin of at least 45Â°, and
often a margin of over 70Â° is advocated, particularly where component
variation due to manufacturing tolerances is an issue.[9] See also the
discussion of phase margin in the step_response article.
    * Examples
    * Figure 6: Gain of feedback amplifier AFB in dB and corresponding open-
      loop amplifier AOL. Parameter 1/Î² = 58 dB, and at low frequencies AFB
      â 58 dB as well. The gain margin in this amplifier is nearly zero
      because | Î²AOL| = 1 occurs at almost f = f180Â°.
    * Figure 7: Phase of feedback amplifier Â°AFB in degrees and corresponding
      open-loop amplifier Â°AOL. The phase margin in this amplifier is nearly
      zero because the phase-flip occurs at almost the unity gain frequency f =
      f0 dB where | Î²AOL| = 1.
    * Figure 8: Gain of feedback amplifier AFB in dB and corresponding open-
      loop amplifier AOL. In this example, 1 / Î² = 77 dB. The gain margin in
      this amplifier is 19 dB.
    * Figure 9: Phase of feedback amplifier AFB in degrees and corresponding
      open-loop amplifier AOL. The phase margin in this amplifier is 45Â°.
***** Bode plotter[edit] *****
Figure 10: Amplitude diagram of a 10th order Chebyshev_filter plotted using a
Bode Plotter application. The chebyshev transfer function is defined by poles
and zeros which are added by clicking on a graphical complex diagram.
The Bode plotter is an electronic instrument resembling an oscilloscope, which
produces a Bode diagram, or a graph, of a circuit's voltage gain or phase shift
plotted against frequency in a feedback control system or a filter. An example
of this is shown in Figure 10. It is extremely useful for analyzing and testing
filters and the stability of feedback control systems, through the measurement
of corner (cutoff) frequencies and gain and phase margins.
This is identical to the function performed by a vector network_analyzer, but
the network analyzer is typically used at much higher frequencies.
For education/research purposes, plotting Bode diagrams for given transfer
functions facilitates better understanding and getting faster results (see
external links).
***** Related plots[edit] *****
Main articles: Nyquist_plot and Nichols_plot
Two related plots that display the same data in different coordinate_systems
are the Nyquist_plot and the Nichols_plot. These are parametric_plots, with
frequency as the input and magnitude and phase of the frequency response as the
output. The Nyquist plot displays these in polar_coordinates, with magnitude
mapping to radius and phase to argument (angle). The Nichols plot displays
these in rectangular coordinates, on the log_scale.
    * A Nyquist_plot.
    * A Nichols_plot of the same response.
***** Appendix[edit] *****
**** Proof for the relation to frequency response[edit] ****
This section shows that the frequency response is given by the magnitude and
phase of the transfer function in Eqs.(1)-(2).
Slightly changing the requirements for Eqs.(1)-(2) one assumes that the input
has been applied starting at time     t = 0   {\displaystyle t=0}  [t=0] and
one calculates the output in the limit     t &#x2192; &#x221E;   {\displaystyle
t\to \infty }  [t\to \infty ]. In this case, the output is given by the
convolution
               y ( t ) =  &#x222B;  0   t   h ( &#x03C4; ) u ( t &#x2212;
            &#x03C4; ) d &#x03C4;  ,   {\displaystyle y(t)=\int _{0}^{t}h(\tau
            )u(t-\tau )d\tau \;,}  [{\displaystyle y(t)=\int _{0}^{t}h(\tau )u
            (t-\tau )d\tau \;,}]
of the input signal with the inverse Laplace transform of the transfer function
h ( t )   {\displaystyle h(t)}  [h(t)]. Assuming that the signal becomes
periodic with mean 0 and period T after a while, we can add as many periods as
we want to the interval of the integral
                lim  t &#x2192; &#x221E;   y ( t ) =  &#x222B;  0   t   h
            ( &#x03C4; ) u ( t &#x2212; &#x03C4; ) d &#x03C4;  +  &#x222B;  t
            t + T   h ( &#x03C4; ) u ( t &#x2212; &#x03C4; ) d &#x03C4;  + . .
            . =  &#x222B;  0   &#x221E;   h ( &#x03C4; ) u ( t &#x2212;
            &#x03C4; ) d &#x03C4;  .   {\displaystyle \lim _{t\to \infty }y
            (t)=\int _{0}^{t}h(\tau )u(t-\tau )d\tau \;+\int _{t}^{t+T}h(\tau
            )u(t-\tau )d\tau \;+...=\int _{0}^{\infty }h(\tau )u(t-\tau )d\tau
            \;.}  [{\displaystyle \lim _{t\to \infty }y(t)=\int _{0}^{t}h(\tau
            )u(t-\tau )d\tau \;+\int _{t}^{t+T}h(\tau )u(t-\tau )d\tau
            \;+...=\int _{0}^{\infty }h(\tau )u(t-\tau )d\tau \;.}]
Thus, inserting the sinusodial input signal one obtains
                lim  t &#x2192; &#x221E;   y ( t ) =  &#x222B;  0   &#x221E;
            h ( &#x03C4; ) sin &#x2061;  (  &#x03C9; ( t &#x2212; &#x03C4; )  )
            d &#x03C4;  =  &#x222B;  0   &#x221E;   h ( &#x03C4; )  I m   (  e
            j  &#x03C9; ( t &#x2212; &#x03C4; )   )  d &#x03C4;  .
            {\displaystyle \lim _{t\to \infty }y(t)=\int _{0}^{\infty }h(\tau
            )\sin \left(\omega (t-\tau )\right)d\tau \;=\int _{0}^{\infty }h
            (\tau )\mathrm {Im} \left(e^{\mathrm {j} \omega (t-\tau
            )}\right)d\tau \;.}  [{\displaystyle \lim _{t\to \infty }y(t)=\int
            _{0}^{\infty }h(\tau )\sin \left(\omega (t-\tau )\right)d\tau
            \;=\int _{0}^{\infty }h(\tau )\mathrm {Im} \left(e^{\mathrm {j}
            \omega (t-\tau )}\right)d\tau \;.}]
Since     h ( t )   {\displaystyle h(t)}  [h(t)] is a real function this can be
written as
                lim  t &#x2192; &#x221E;   y ( t ) =  I m   {   e   j  &#x03C9;
            t    [   &#x222B;  0   &#x221E;   h ( &#x03C4; )  e  &#x2212;  j
            &#x03C9; &#x03C4;   d &#x03C4; &#xA0;  ]   }   .   {\displaystyle
            \lim _{t\to \infty }y(t)=\mathrm {Im} \left\{e^{\mathrm {j} \omega
            t}\left[\int _{0}^{\infty }h(\tau )e^{-\mathrm {j} \omega \tau
            }d\tau \ \right]\right\}\;.}  [{\displaystyle \lim _{t\to \infty }y
            (t)=\mathrm {Im} \left\{e^{\mathrm {j} \omega t}\left[\int _{0}^
            {\infty }h(\tau )e^{-\mathrm {j} \omega \tau }d\tau \
            \right]\right\}\;.}]
The term in brackets is the definition of the Laplace transform of     h
{\displaystyle h}  [h] at     s =  j  &#x03C9;   {\displaystyle s=\mathrm {j}
\omega }  [s=\mathrm{j} \omega]. Inserting the definition in the form     H
(  j  &#x03C9; ) =  |  H (  j  &#x03C9; )  |  exp &#x2061;  (  arg &#x2061; H
(  j  &#x03C9; )  )    {\displaystyle H(\mathrm {j} \omega )=|H(\mathrm {j}
\omega )|\exp \left(\arg H(\mathrm {j} \omega )\right)}  [H(\mathrm{j} \omega)
= |H(\mathrm{j} \omega )| \exp \left( \arg  H(\mathrm{j} \omega)  \right )] one
obtains the output signal
                lim  t &#x2192; &#x221E;   y ( t ) =  |  H (  j  &#x03C9; )  |
            sin &#x2061;  (  &#x03C9; t + arg &#x2061;  (  H (  j  &#x03C9; )
            )   )     {\displaystyle \lim _{t\to \infty }y(t)=|H(\mathrm {j}
            \omega )|\sin \left(\omega t+\arg \left(H(\mathrm {j} \omega
            )\right)\right)\;}  [\lim_{t \to \infty }y(t) =  |H(\mathrm{j}
            \omega )| \sin \left( \omega t +  \arg\left(H(\mathrm{j} \omega)
            \right)  \right) \; ]
stated in Eqs.(1)-(2).
***** See also[edit] *****
    * Analog_signal_processing
    * Phase_margin
    * Bode's_sensitivity_integral
    * Bode's_magnitude_(gain)âphase_relation
    * Electrochemical_impedance_spectroscopy
***** Notes[edit] *****
   1. ^ Ordinarily, as frequency increases the magnitude of the gain drops and
      the phase becomes more negative, although these are only trends and may
      be reversed in particular frequency ranges. Unusual gain behavior can
      render the concepts of gain and phase margin inapplicable. Then other
      methods such as the Nyquist_plot have to be used to assess stability.
   2. ^ The critical amount of feedback where the peak in the gain just
      disappears altogether is the maximally flat or Butterworth design.
   3. ^ The frequency where the open-loop gain flips sign f180 does not change
      with a change in feedback factor; it is a property of the open-loop gain.
      The value of the gain at f180 also does not change with a change in Î².
      Therefore, we could use the previous values from Figures 6 and 7.
      However, for clarity the procedure is described using only Figures 8 and
      9.
***** References[edit] *****
   1. ^R. K. Rao Yarlagadda (2010). Analog and Digital Signals and Systems.
      Springer Science & Business Media. p. 243. ISBN 978-1-4419-0034-0.
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
   3. ^ Van Valkenburg, M. E. University of Illinois at Urbana-Champaign, "In
      memoriam: Hendrik W. Bode (1905-1982)", IEEE Transactions on Automatic
      Control, Vol. AC-29, No 3., March 1984, pp. 193-194. Quote: "Something
      should be said about his name. To his colleagues at Bell Laboratories and
      the generations of engineers that have followed, the pronunciation is
      boh-dee. The Bode family preferred that the original Dutch be used as
      boh-dah."
   4. ^"Vertaling_van_postbode,_NL>EN". mijnwoordenboek.nl. Retrieved 2013-10-
      07.
   5. ^ David A. Mindell Between Human and Machine: Feedback, Control, and
      Computing Before Cybernetics JHU Press, 2004
   6. ISBN 0801880572, pp. 127-131
   7. ^Skogestad, Sigurd; Postlewaite, Ian (2005). Multivariable Feedback
      Control. Chichester, West Sussex, England: John Wiley & Sons, Ltd.
      ISBN 0-470-01167-X.
   8. ^ Thomas H. Lee (2004). The_design_of_CMOS_radio-frequency_integrated
      circuits (Second ed.). Cambridge UK: Cambridge University Press.
      p. Â§14.6 pp. 451â453. ISBN 0-521-83539-9.
   9. ^ William S Levine (1996). The_control_handbook:_the_electrical
      engineering_handbook_series (Second ed.). Boca Raton FL: CRC Press/IEEE
      Press. p. Â§10.1 p. 163. ISBN 0-8493-8570-9.
  10. ^ Allen_Tannenbaum. Invariance and Systems Theory: Algebraic and
      Geometric Aspects. New York, NY: Springer-Verlag. ISBN 9783540105657.
  11. ^ a b Willy M C Sansen (2006). Analog_design_essentials. Dordrecht, The
      Netherlands: Springer. pp. 157â163. ISBN 0-387-25746-2.
***** External links[edit] *****
 Wikimedia Commons has media related to Bode_plots.
    * Explanation_of_Bode_plots_with_movies_and_examples
    * How_to_draw_piecewise_asymptotic_Bode_plots
    * Summarized_drawing_rules (PDF)
    * Bode_plot_applet - Accepts transfer function coefficients as input, and
      calculates magnitude and phase response
    * Circuit_analysis_in_electrochemistry
    * Tim_Green:_Operational_amplifier_stability Includes some Bode plot
      introduction
    * Gnuplot code for generating Bode plot: DIN-A4_printing_template_(pdf)
    * MATLAB_function_for_creating_a_Bode_plot_of_a_system
    * MATLAB_Tech_Talk_videos_explaining_Bode_plots_and_showing_how_to_use_them
      for_control_design
    * Insert_the_poles_and_zeros_and_this_website_will_draw_the_asymptotic_and
      accurate_Bode_plots
    * Mathematica_function_for_creating_the_Bode_plot

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Bode_plot&oldid=908246476"
Categories:
    * Plots_(graphics)
    * Signal_processing
    * Electronic_feedback
    * Electronic_amplifiers
    * Electrical_parameters
    * Classical_control_theory
    * Filter_frequency_response
Hidden categories:
    * Articles_needing_additional_references_from_December_2011
    * All_articles_needing_additional_references
    * Commons_category_link_is_on_Wikidata
    * Commons_category_link_is_on_Wikidata_using_P373
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
    * Wikiversity
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * CatalÃ 
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 28 July 2019, at 13:20 (UTC).
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
