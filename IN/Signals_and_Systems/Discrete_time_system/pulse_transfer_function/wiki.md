The following text has been accessed from https://en.wikipedia.org/wiki/Transfer_function at Fri Aug 9 01:31:41 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Transfer function ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article may contain too much repetition or redundant language. Please
 help improve_it by merging similar text or removing repeated statements.
 (December 2014)(Learn_how_and_when_to_remove_this_template_message)
In engineering, a transfer function (also known as system function[1] or
network function) of an electronic or control_system component is a
mathematical_function which theoretically_models the device's output for each
possible input.[2][3][4] In its simplest form, this function is a two-
dimensional graph of an independent scalar input versus the dependent scalar
output, called a transfer curve or characteristic curve. Transfer functions for
components are used to design and analyze systems assembled from components,
particularly using the block_diagram technique, in electronics and control
theory.
The dimensions and units of the transfer function model the output response of
the device for a range of possible inputs. For example, the transfer function
of a two-port electronic circuit like an amplifier might be a two-dimensional
graph of the scalar voltage at the output as a function of the scalar voltage
applied to the input; the transfer function of an electromechanical actuator
might be the mechanical displacement of the movable arm as a function of
electrical current applied to the device; the transfer function of a
photodetector might be the output voltage as a function of the luminous
intensity of incident light of a given wavelength.
The term "transfer function" is also used in the frequency_domain analysis of
systems using transform methods such as the Laplace_transform; here it means
the amplitude of the output as a function of the frequency of the input signal.
For example, the transfer function of an electronic_filter is the voltage
amplitude at the output as a function of the frequency of a constant amplitude
sine_wave applied to the input. For optical imaging devices, the optical
transfer_function is the Fourier_transform of the point_spread_function (hence
a function of spatial_frequency).
⁰
***** Contents *****
    * 1_Linear_time-invariant_systems
          o 1.1_Direct_derivation_from_differential_equations
          o 1.2_Gain,_transient_behavior_and_stability
    * 2_Signal_processing
          o 2.1_Common_transfer_function_families
    * 3_Control_engineering
    * 4_Optics
    * 5_Non-linear_systems
    * 6_See_also
    * 7_References
    * 8_External_links
***** Linear time-invariant systems[edit] *****
Transfer functions are commonly used in the analysis of systems such as single-
input_single-output filters in the fields of signal_processing, communication
theory, and control_theory. The term is often used exclusively to refer to
linear_time-invariant (LTI) systems. Most real systems have non-linear input/
output characteristics, but many systems, when operated within nominal
parameters (not "over-driven") have behavior close enough to linear that LTI
system_theory is an acceptable representation of the input/output behavior.
The descriptions below are given in terms of a complex variable,     s =
&#x03C3; + j &#x22C5; &#x03C9;   {\displaystyle s=\sigma +j\cdot \omega }  [s =
\sigma + j \cdot \omega], which bears a brief explanation. In many
applications, it is sufficient to define     &#x03C3; = 0   {\displaystyle
\sigma =0}  [\sigma =0] (thus     s = j &#x22C5; &#x03C9;   {\displaystyle
s=j\cdot \omega }  [s = j \cdot \omega]), which reduces the Laplace_transforms
with complex arguments to Fourier_transforms with real argument Ï. The
applications where this is common are ones where there is interest only in the
steady-state response of an LTI system, not the fleeting turn-on and turn-off
behaviors or stability issues. That is usually the case for signal_processing
and communication_theory.
Thus, for continuous-time input signal     x ( t )   {\displaystyle x(t)}  [x
(t)] and output     y ( t )   {\displaystyle y(t)}  [y(t)], the transfer
function     H ( s )   {\displaystyle H(s)}  [H(s)] is the linear mapping of
the Laplace transform of the input,     X ( s ) =   L    {  x ( t )  }
{\displaystyle X(s)={\mathcal {L}}\left\{x(t)\right\}}  [X(s) = \mathcal
{L}\left\{x(t)\right\}], to the Laplace transform of the output     Y ( s ) =
L    {  y ( t )  }    {\displaystyle Y(s)={\mathcal {L}}\left\{y(t)\right\}}
[Y(s) = \mathcal{L}\left\{y(t)\right\}]:
         Y ( s ) = H ( s )  X ( s )   {\displaystyle Y(s)=H(s)\;X(s)}  [ Y(s) =
      H(s)\;X(s) ]
or
         H ( s ) =    Y ( s )   X ( s )    =      L    {  y ( t )  }      L
      {  x ( t )  }       {\displaystyle H(s)={\frac {Y(s)}{X(s)}}={\frac {
      {\mathcal {L}}\left\{y(t)\right\}}{{\mathcal {L}}\left\{x(t)\right\}}}}
      [ H(s) = \frac{Y(s)}{X(s)} = \frac{ \mathcal{L}\left\{y(t)\right\} }
      { \mathcal{L}\left\{x(t)\right\} } ].
In discrete-time systems, the relation between an input signal     x ( t )
{\displaystyle x(t)}  [x(t)] and output     y ( t )   {\displaystyle y(t)}  [y
(t)] is dealt with using the z-transform, and then the transfer function is
similarly written as     H ( z ) =    Y ( z )   X ( z )      {\displaystyle H
(z)={\frac {Y(z)}{X(z)}}}  [H(z) = \frac{Y(z)}{X(z)}] and this is often
referred to as the pulse-transfer function.[citation_needed]
**** Direct derivation from differential equations[edit] ****
Consider a linear_differential_equation with constant coefficients
         L [ u ] =     d  n   u   d  t  n      +  a  1       d  n &#x2212; 1
      u   d  t  n &#x2212; 1      + &#x22EF; +  a  n &#x2212; 1      d u   d t
      +  a  n   u = r ( t )   {\displaystyle L[u]={\frac {d^{n}u}{dt^{n}}}+a_
      {1}{\frac {d^{n-1}u}{dt^{n-1}}}+\dotsb +a_{n-1}{\frac {du}{dt}}+a_{n}u=r
      (t)}  [ L[u] = \frac{d^nu}{dt^n} + a_1\frac{d^{n-1}u}{dt^{n-1}} + \dotsb
      + a_{n-1}\frac{du}{dt} + a_nu = r(t) ]
where u and r are suitably smooth functions of t, and L is the operator defined
on the relevant function space, that transforms u into r. That kind of equation
can be used to constrain the output function u in terms of the forcing function
r. The transfer function can be used to define an operator     F [ r ] = u
{\displaystyle F[r]=u}  [F[r] = u ] that serves as a right inverse of L,
meaning that     L [ F [ r ] ] = r   {\displaystyle L[F[r]]=r}  [L[F[r]] = r].
Solutions of the homogeneous, constant-coefficient_differential_equation     L
[ u ] = 0   {\displaystyle L[u]=0}  [L[u] = 0] can be found by trying     u =
e  &#x03BB; t     {\displaystyle u=e^{\lambda t}}  [u = e^{\lambda t}]. That
substitution yields the characteristic_polynomial
          p  L   ( &#x03BB; ) =  &#x03BB;  n   +  a  1    &#x03BB;  n &#x2212;
      1   + &#x22EF; +  a  n &#x2212; 1   &#x03BB; +  a  n      {\displaystyle
      p_{L}(\lambda )=\lambda ^{n}+a_{1}\lambda ^{n-1}+\dotsb +a_{n-1}\lambda
      +a_{n}\,}  [ p_L(\lambda) = \lambda^n + a_1\lambda^{n-1} + \dotsb + a_{n-
      1}\lambda + a_n\,]
The inhomogeneous case can be easily solved if the input function r is also of
the form     r ( t ) =  e  s t     {\displaystyle r(t)=e^{st}}  [r(t) = e^{s
t}]. In that case, by substituting     u = H ( s )  e  s t     {\displaystyle
u=H(s)e^{st}}  [u = H(s)e^{s t}] one finds that     L [ H ( s )  e  s t   ] =
e  s t     {\displaystyle L[H(s)e^{st}]=e^{st}}  [L[H(s) e^{s t}] = e^{s t}] if
we define
         H ( s ) =   1   p  L   ( s )      wherever&#xA0;    p  L   ( s )
      &#x2260; 0.   {\displaystyle H(s)={\frac {1}{p_{L}(s)}}\qquad {\text
      {wherever }}\quad p_{L}(s)\neq 0.}  [{\displaystyle H(s)={\frac {1}{p_{L}
      (s)}}\qquad {\text{wherever }}\quad p_{L}(s)\neq 0.}]
Taking that as the definition of the transfer function requires careful
disambiguation[clarification_needed] between complex vs. real values, which is
traditionally influenced[clarification_needed] by the interpretation of abs(H
(s)) as the gain and -atan(H(s)) as the phase_lag. Other definitions of the
transfer function are used: for example     1  /   p  L   ( i k ) .
{\displaystyle 1/p_{L}(ik).}  [1/p_L(ik) .][5]
**** Gain, transient behavior and stability[edit] ****
A general sinusoidal input to a system of frequency      &#x03C9;  0    /  ( 2
&#x03C0; )   {\displaystyle \omega _{0}/(2\pi )}  [{\displaystyle \omega _{0}/
(2\pi )}] may be written     exp &#x2061; ( j  &#x03C9;  0   t )
{\displaystyle \exp(j\omega _{0}t)}  [{\displaystyle \exp(j\omega _{0}t)}]. The
response of a system to a sinusoidal input beginning at time     t = 0
{\displaystyle t=0}  [t=0] will consist of the sum of the steady-state response
and a transient response. The steady-state response is the output of the system
in the limit of infinite time, and the transient response is the difference
between the response and the steady state response (It corresponds to the
homogeneous solution of the above differential equation.) The transfer function
for an LTI system may be written as the product:
         H ( s ) =  &#x220F;  i = 1   N     1  s &#x2212;  s   P  i
      {\displaystyle H(s)=\prod _{i=1}^{N}{\frac {1}{s-s_{P_{i}}}}}  [
      {\displaystyle H(s)=\prod _{i=1}^{N}{\frac {1}{s-s_{P_{i}}}}}]
where sPi are the N roots of the characteristic polynomial and will therefore
be the poles of the transfer function. Consider the case of a transfer function
with a single pole     H ( s ) =   1  s &#x2212;  s  P        {\displaystyle H
(s)={\frac {1}{s-s_{P}}}}  [{\displaystyle H(s)={\frac {1}{s-s_{P}}}}] where
s  P   =  &#x03C3;  P   + j  &#x03C9;  P     {\displaystyle s_{P}=\sigma _
{P}+j\omega _{P}}  [{\displaystyle s_{P}=\sigma _{P}+j\omega _{P}}]. The
Laplace transform of a general sinusoid of unit amplitude will be       1  s
&#x2212; j  &#x03C9;  i        {\displaystyle {\frac {1}{s-j\omega _{i}}}}  [
{\displaystyle {\frac {1}{s-j\omega _{i}}}}]. The Laplace transform of the
output will be        H ( s )   ( s &#x2212; j  &#x03C9;  0   )
{\displaystyle {\frac {H(s)}{(s-j\omega _{0})}}}  [{\displaystyle {\frac {H(s)}
{(s-j\omega _{0})}}}] and the temporal output will be the inverse Laplace
transform of that function:
         g ( t ) =     e  j   &#x03C9;  0    t   &#x2212;  e  (  &#x03C3;  P
      + j   &#x03C9;  P   ) t     &#x2212;  &#x03C3;  P   + j (  &#x03C9;  0
      &#x2212;  &#x03C9;  P   )      {\displaystyle g(t)={\frac {e^{j\,\omega _
      {0}\,t}-e^{(\sigma _{P}+j\,\omega _{P})t}}{-\sigma _{P}+j(\omega _{0}-
      \omega _{P})}}}  [{\displaystyle g(t)={\frac {e^{j\,\omega _{0}\,t}-e^{
      (\sigma _{P}+j\,\omega _{P})t}}{-\sigma _{P}+j(\omega _{0}-\omega _
      {P})}}}]
The second term in the numerator is the transient response, and in the limit of
infinite time it will diverge to infinity if σP is positive. In order for a
system to be stable, its transfer function must have no poles whose real parts
are positive. If the transfer function is strictly stable, the real parts of
all poles will be negative, and the transient behavior will tend to zero in the
limit of infinite time. The steady-state output will be:
         g ( &#x221E; ) =    e  j   &#x03C9;  0    t    &#x2212;  &#x03C3;  P
      + j (  &#x03C9;  0   &#x2212;  &#x03C9;  P   )      {\displaystyle g
      (\infty )={\frac {e^{j\,\omega _{0}\,t}}{-\sigma _{P}+j(\omega _{0}-
      \omega _{P})}}}  [{\displaystyle g(\infty )={\frac {e^{j\,\omega _
      {0}\,t}}{-\sigma _{P}+j(\omega _{0}-\omega _{P})}}}]
The frequency_response (or "gain") G of the system is defined as the absolute
value of the ratio of the output amplitude to the steady-state input amplitude:
         G (  &#x03C9;  i   ) =  |   1  &#x2212;  &#x03C3;  P   + j (  &#x03C9;
      0   &#x2212;  &#x03C9;  P   )    |  =   1   &#x03C3;  P   2   +
      (  &#x03C9;  P   &#x2212;  &#x03C9;  0    )  2        {\displaystyle G
      (\omega _{i})=\left|{\frac {1}{-\sigma _{P}+j(\omega _{0}-\omega _
      {P})}}\right|={\frac {1}{\sqrt {\sigma _{P}^{2}+(\omega _{P}-\omega _
      {0})^{2}}}}}  [{\displaystyle G(\omega _{i})=\left|{\frac {1}{-\sigma _
      {P}+j(\omega _{0}-\omega _{P})}}\right|={\frac {1}{\sqrt {\sigma _{P}^
      {2}+(\omega _{P}-\omega _{0})^{2}}}}}]
which is just the absolute value of the transfer function     H ( s )
{\displaystyle H(s)}  [H(s)] evaluated at     j  &#x03C9;  i     {\displaystyle
j\omega _{i}}  [{\displaystyle j\omega _{i}}]. This result can be shown to be
valid for any number of transfer function poles.
***** Signal processing[edit] *****
Let     x ( t ) &#xA0;   {\displaystyle x(t)\ }  [ x(t) \ ] be the input to a
general linear_time-invariant_system, and     y ( t ) &#xA0;   {\displaystyle y
(t)\ }  [ y(t) \ ] be the output, and the bilateral_Laplace_transform of     x
( t ) &#xA0;   {\displaystyle x(t)\ }  [ x(t) \ ] and     y ( t ) &#xA0;
{\displaystyle y(t)\ }  [ y(t) \ ] be
             X ( s )    =   L    {  x ( t )  }  &#xA0;     =    d e f
      &#xA0;  &#x222B;  &#x2212; &#x221E;   &#x221E;   x ( t )  e  &#x2212; s t
      d t ,     Y ( s )    =   L    {  y ( t )  }  &#xA0;     =    d e f
      &#xA0;  &#x222B;  &#x2212; &#x221E;   &#x221E;   y ( t )  e  &#x2212; s t
      d t .       {\displaystyle {\begin{aligned}X(s)&={\mathcal {L}}\left\{x
      (t)\right\}\ {\stackrel {\mathrm {def} }{=}}\ \int _{-\infty }^{\infty }x
      (t)e^{-st}\,dt,\\Y(s)&={\mathcal {L}}\left\{y(t)\right\}\ {\stackrel
      {\mathrm {def} }{=}}\ \int _{-\infty }^{\infty }y(t)e^{-st}\,dt.\end
      {aligned}}}  [{\begin{aligned}X(s)&={\mathcal  {L}}\left\{x(t)\right\}\
      {\stackrel  {{\mathrm  {def}}}{=}}\ \int _{{-\infty }}^{{\infty }}x(t)e^{
      {-st}}\,dt,\\Y(s)&={\mathcal  {L}}\left\{y(t)\right\}\ {\stackrel  {
      {\mathrm  {def}}}{=}}\ \int _{{-\infty }}^{{\infty }}y(t)e^{{-
      st}}\,dt.\end{aligned}}]
Then the output is related to the input by the transfer function     H ( s )
{\displaystyle H(s)}  [H(s)] as
         Y ( s ) = H ( s ) X ( s )    {\displaystyle Y(s)=H(s)X(s)\,}  [ Y(s) =
      H(s) X(s)  \, ]
and the transfer function itself is therefore
         H ( s ) =    Y ( s )   X ( s )    .   {\displaystyle H(s)={\frac {Y
      (s)}{X(s)}}.}  [H(s)={\frac  {Y(s)}{X(s)}}.]
In particular, if a complex harmonic signal with a sinusoidal component with
amplitude      |  X  |  &#xA0;   {\displaystyle |X|\ }  [|X| \ ], angular
frequency     &#x03C9; &#xA0;   {\displaystyle \omega \ }  [\omega \ ] and
phase     arg &#x2061; ( X ) &#xA0;   {\displaystyle \arg(X)\ }  [\arg(X) \ ],
where arg is the argument
         x ( t ) = X  e  j &#x03C9; t   =  |  X  |   e  j ( &#x03C9; t + arg
      &#x2061; ( X ) )     {\displaystyle x(t)=Xe^{j\omega t}=|X|e^{j(\omega
      t+\arg(X))}}  [ x(t) = Xe^{j\omega t} = |X|e^{j(\omega t + \arg(X))} ]
      where     X =  |  X  |   e  j arg &#x2061; ( X )     {\displaystyle
      X=|X|e^{j\arg(X)}}  [ X = |X|e^{j\arg(X)}  ]
is input to a linear time-invariant system, then the corresponding component in
the output is:
             y ( t )    = Y  e  j &#x03C9; t   =  |  Y  |   e  j ( &#x03C9; t +
      arg &#x2061; ( Y ) )   ,     Y    =  |  Y  |   e  j arg &#x2061; ( Y )
      .       {\displaystyle {\begin{aligned}y(t)&=Ye^{j\omega t}=|Y|e^{j
      (\omega t+\arg(Y))},\\Y&=|Y|e^{j\arg(Y)}.\end{aligned}}}  [{\begin
      {aligned}y(t)&=Ye^{{j\omega t}}=|Y|e^{{j(\omega t+\arg(Y))}},\\Y&=|Y|e^{
      {j\arg(Y)}}.\end{aligned}}]
Note that, in a linear time-invariant system, the input frequency     &#x03C9;
&#xA0;   {\displaystyle \omega \ }  [\omega \ ] has not changed, only the
amplitude and the phase angle of the sinusoid has been changed by the system.
The frequency_response     H ( j &#x03C9; ) &#xA0;   {\displaystyle H(j\omega
)\ }  [ H(j \omega) \ ] describes this change for every frequency     &#x03C9;
&#xA0;   {\displaystyle \omega \ }  [\omega \ ] in terms of gain:
         G ( &#x03C9; ) =     |  Y  |     |  X  |     =  |  H ( j &#x03C9; )  |
      &#xA0;   {\displaystyle G(\omega )={\frac {|Y|}{|X|}}=|H(j\omega )|\ }
      [G(\omega) = \frac{|Y|}{|X|} = |H(j \omega)| \ ]
and phase shift:
         &#x03D5; ( &#x03C9; ) = arg &#x2061; ( Y ) &#x2212; arg &#x2061; ( X )
      = arg &#x2061; ( H ( j &#x03C9; ) ) .   {\displaystyle \phi (\omega
      )=\arg(Y)-\arg(X)=\arg(H(j\omega )).}  [\phi (\omega )=\arg(Y)-\arg
      (X)=\arg(H(j\omega )).]
The phase_delay (i.e., the frequency-dependent amount of delay introduced to
the sinusoid by the transfer function) is:
          &#x03C4;  &#x03D5;   ( &#x03C9; ) = &#x2212;    &#x03D5; ( &#x03C9; )
      &#x03C9;   .   {\displaystyle \tau _{\phi }(\omega )=-{\frac {\phi
      (\omega )}{\omega }}.}  [\tau _{{\phi }}(\omega )=-{\frac  {\phi (\omega
      )}{\omega }}.]
The group_delay (i.e., the frequency-dependent amount of delay introduced to
the envelope of the sinusoid by the transfer function) is found by computing
the derivative of the phase shift with respect to angular frequency
&#x03C9; &#xA0;   {\displaystyle \omega \ }  [\omega \ ],
          &#x03C4;  g   ( &#x03C9; ) = &#x2212;    d &#x03D5; ( &#x03C9; )   d
      &#x03C9;    .   {\displaystyle \tau _{g}(\omega )=-{\frac {d\phi (\omega
      )}{d\omega }}.}  [\tau _{{g}}(\omega )=-{\frac  {d\phi (\omega )}{d\omega
      }}.]
The transfer function can also be shown using the Fourier_transform which is
only a special case of the bilateral_Laplace_transform for the case where     s
= j &#x03C9;   {\displaystyle s=j\omega }  [ s = j \omega ].
**** Common transfer function families[edit] ****
While any LTI system can be described by some transfer function or another,
there are certain "families" of special transfer functions that are commonly
used.
Some common transfer function families and their particular characteristics
are:
    * Butterworth_filter – maximally flat in passband and stopband for the
      given order
    * Chebyshev_filter_(Type_I) – maximally flat in stopband, sharper cutoff
      than a Butterworth filter of the same order
    * Chebyshev_filter_(Type_II) – maximally flat in passband, sharper cutoff
      than a Butterworth filter of the same order
    * Bessel_filter – best pulse response for a given order because it has no
      group delay ripple
    * Elliptic_filter – sharpest cutoff (narrowest transition between pass band
      and stop band) for the given order
    * Optimum_"L"_filter
    * Gaussian_filter – minimum group delay; gives no overshoot to a step
      function
    * Hourglass_filter
    * Raised-cosine_filter
***** Control engineering[edit] *****
In control_engineering and control_theory the transfer function is derived
using the Laplace_transform.
The transfer function was the primary tool used in classical control
engineering. However, it has proven to be unwieldy for the analysis of
multiple-input_multiple-output_(MIMO) systems, and has been largely supplanted
by state_space representations for such systems.[citation_needed] In spite of
this, a transfer_matrix can always be obtained for any linear system, in order
to analyze its dynamics and other properties: each element of a transfer matrix
is a transfer function relating a particular input variable to an output
variable.
A useful representation bridging state_space and transfer function methods was
proposed by Howard_H._Rosenbrock and is referred to as Rosenbrock_system
matrix.
***** Optics[edit] *****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (December 2014)(Learn_how_and_when_to_remove_this_template_message)
In optics, modulation_transfer_function indicates the capability of optical
contrast transmission.
For example, when observing a series of black-white-light fringes drawn with a
specific spatial frequency, the image quality may decay. White fringes fade
while black ones turn brighter.
The modulation transfer function in a specific spatial frequency is defined by
          M T F  ( f ) =    M (  i m a g e  )   M (  s o u r c e  )    ,
      {\displaystyle \mathrm {MTF} (f)={\frac {M(\mathrm {image} )}{M(\mathrm
      {source} )}},}  [{\displaystyle \mathrm {MTF} (f)={\frac {M(\mathrm
      {image} )}{M(\mathrm {source} )}},}]
where modulation (M) is computed from the following image or light brightness:
         M =     L  max   &#x2212;  L  min      L  max   +  L  min      .
      {\displaystyle M={\frac {L_{\max }-L_{\min }}{L_{\max }+L_{\min }}}.}
      [M={\frac  {L_{{\max }}-L_{{\min }}}{L_{{\max }}+L_{{\min }}}}.]
***** Non-linear systems[edit] *****
Transfer functions do not properly exist for many non-linear_systems. For
example, they do not exist for relaxation_oscillators;[6] however, describing
functions can sometimes be used to approximate such nonlinear time-invariant
systems.
***** See also[edit] *****
    * Analog_computer
    * Black_box
    * Bode_plot
    * Convolution
    * Duhamel's_principle
    * Frequency_response
    * Impulse_response
    * Laplace_transform
    * LTI_system_theory
    * Nyquist_plot
    * Operational_amplifier
    * Optical_transfer_function
    * Proper_transfer_function
    * Rosenbrock_system_matrix
    * Semilog_graph
    * Signal-flow_graph
    * Signal_transfer_function
***** References[edit] *****
   1. ^ Bernd_Girod, Rudolf Rabenstein, Alexander Stenger, Signals and systems,
      2nd ed., Wiley, 2001,
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
   3. ISBN 0-471-98800-6 p. 50
   4. ^M. A. Laughton; D.F. Warne. Electrical Engineer's Reference Book (16
      ed.). Newnes. pp. 14/9â14/10. ISBN 978-0-08-052354-5.
   5. ^E. A. Parr (1993). Logic Designer's Handbook: Circuits and Systems (2nd
      ed.). Newness. pp. 65â66. ISBN 978-1-4832-9280-9.
   6. ^Ian Sinclair; John Dunton (2007). Electronic and Electrical Servicing:
      Consumer and Commercial Electronics. Routledge. p. 172. ISBN 978-0-7506-
      6988-7.
   7. ^Birkhoff, Garrett; Rota, Gian-Carlo (1978). Ordinary differential
      equations. New York: John Wiley & Sons. ISBN 978-0-471-05224-1.
   8. [page needed]
   9. ^Valentijn De Smedt, Georges Gielen and Wim Dehaene (2015). Temperature-
      and Supply Voltage-Independent Time References for Wireless Sensor
      Networks. Springer. p. 47. ISBN 978-3-319-09003-0.
***** External links[edit] *****
    * "Transfer_function". PlanetMath.
ECE_209:_Review_of_Circuits_as_LTI_Systems — Short primer on the mathematical
analysis of (electrical) LTI systems.
ECE_209:_Sources_of_Phase_Shift — Gives an intuitive explanation of the source
of phase shift in two simple LTI systems. Also verifies simple transfer
functions by using trigonometric identities.
Transfer_function_model_in_Mathematica
[1] for resonant frequency
[2] frequency scaling op amp

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Transfer_function&oldid=908246480"
Categories:
    * Electrical_circuits
    * Transfer_functions
    * Frequency-domain_analysis
    * Types_of_functions
Hidden categories:
    * Wikipedia_articles_needing_page_number_citations_from_April_2013
    * Wikipedia_articles_with_style_issues_from_December_2014
    * All_articles_with_style_issues
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_April_2013
    * Wikipedia_articles_needing_clarification_from_January_2017
    * Articles_with_unsourced_statements_from_December_2014
    * Articles_needing_additional_references_from_December_2014
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * CatalÃ 
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
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
