The following text has been accessed from https://en.wikipedia.org/wiki/Spectral_density#Power_spectral_density at Thu Aug 8 23:28:14 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Spectral density ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Relative importance of certain frequencies in a composite signal
This article is about signal processing and relation of spectra to time-series.
For further applications in the physical sciences, see Spectrum_Â§ Physical
science.
"Spectral power density" redirects here. It is not to be confused with Spectral
power.
The spectral density of a fluorescent_light as a function of optical wavelength
shows peaks at atomic transitions, indicated by the numbered arrows.
The voice waveform over time (left) has a broad audio power spectrum (right).
The power spectrum      S  x x   ( f )   {\displaystyle S_{xx}(f)}  [S_{{xx}}
(f)] of a time_series     x ( t )   {\displaystyle x(t)}  [x(t)] describes the
distribution of power into frequency components composing that signal.[1]
According to Fourier_analysis, any physical signal can be decomposed into a
number of discrete frequencies, or a spectrum of frequencies over a continuous
range. The statistical average of a certain signal or sort of signal (including
noise) as analyzed in terms of its frequency content, is called its spectrum.
When the energy of the signal is concentrated around a finite time interval,
especially if its total energy is finite, one may compute the energy spectral
density. More commonly used is the power spectral density (or simply power
spectrum), which applies to signals existing over all time, or over a time
period large enough (especially in relation to the duration of a measurement)
that it could as well have been over an infinite time interval. The power
spectral density (PSD) then refers to the spectral energy distribution that
would be found per unit time, since the total energy of such a signal over all
time would generally be infinite. Summation or integration of the spectral
components yields the total power (for a physical process) or variance (in a
statistical process), identical to what would be obtained by integrating      x
2   ( t )   {\displaystyle x^{2}(t)}  [{\displaystyle x^{2}(t)}] over the time
domain, as dictated by Parseval's_theorem.[2]
The spectrum of a physical process     x ( t )   {\displaystyle x(t)}  [x(t)]
often contains essential information about the nature of     x   {\displaystyle
x}  [x]. For instance, the pitch and timbre of a musical instrument are
immediately determined from a spectral analysis. The color of a light source is
determined by the spectrum of the electromagnetic wave's electric field     E
( t )   {\displaystyle E(t)}  [E(t)] as it fluctuates at an extremely high
frequency. Obtaining a spectrum from time series such as these involves the
Fourier_transform, and generalizations based on Fourier analysis. In many cases
the time domain is not specifically employed in practice, such as when a
dispersive prism is used to obtain a spectrum of light in a spectrograph, or
when a sound is perceived through its effect on the auditory receptors of the
inner ear, each of which is sensitive to a particular frequency.
However this article concentrates on situations in which the time series is
known (at least in a statistical sense) or directly measured (such as by a
microphone sampled by a computer). The power spectrum is important in
statistical_signal_processing and in the statistical study of stochastic
processes, as well as in many other branches of physics and engineering.
Typically the process is a function of time, but one can similarly discuss data
in the spatial domain being decomposed in terms of spatial_frequency.[3]
⁰
***** Contents *****
    * 1_Explanation
    * 2_Definition
          o 2.1_Energy_spectral_density
          o 2.2_Power_spectral_density
                # 2.2.1_Properties_of_the_power_spectral_density
          o 2.3_Cross_power_spectral_density
    * 3_Estimation
    * 4_Properties
    * 5_Related_concepts
    * 6_Applications
          o 6.1_Electrical_engineering
          o 6.2_Cosmology
    * 7_See_also
    * 8_Notes
    * 9_References
    * 10_External_links
***** Explanation[edit] *****
Further information: Spectrum
Any signal that can be represented as a variable that varies in time has a
corresponding frequency spectrum. This includes familiar entities such as
visible_light (perceived as color), musical notes (perceived as pitch), radio/
TV (specified by their frequency, or sometimes wavelength) and even the regular
rotation of the earth. When these signals are viewed in the form of a frequency
spectrum, certain aspects of the received signals or the underlying processes
producing them are revealed. In some cases the frequency spectrum may include a
distinct peak corresponding to a sine_wave component. And additionally there
may be peaks corresponding to harmonics of a fundamental peak, indicating a
periodic signal which is not simply sinusoidal. Or a continuous spectrum may
show narrow frequency intervals which are strongly enhanced corresponding to
resonances, or frequency intervals containing almost zero power as would be
produced by a notch_filter.
In physics, the signal might be a wave, such as an electromagnetic_wave, an
acoustic_wave, or the vibration of a mechanism. The power spectral density
(PSD) of the signal describes the power present in the signal as a function of
frequency, per unit frequency. Power spectral density is commonly expressed in
watts per hertz (W/Hz).[4]
When a signal is defined in terms only of a voltage, for instance, there is no
unique power associated with the stated amplitude. In this case "power" is
simply reckoned in terms of the square of the signal, as this would always be
proportional to the actual power delivered by that signal into a given
impedance. So one might use units of V2 Hzâ1 for the PSD and V2 s Hzâ1 for
the ESD (energy spectral density)[5] even though no actual "power" or "energy"
is specified.
Sometimes one encounters an amplitude spectral density (ASD), which is the
square root of the PSD; the ASD of a voltage signal has units of V Hzâ1/2.[6]
This is useful when the shape of the spectrum is rather constant, since
variations in the ASD will then be proportional to variations in the signal's
voltage level itself. But it is mathematically preferred to use the PSD, since
only in that case is the area under the curve meaningful in terms of actual
power over all frequency or over a specified bandwidth.
In the general case, the units of PSD will be the ratio of units of variance
per unit of frequency; so, for example, a series of displacement values (in
meters) over time (in seconds) will have PSD in units of m2/Hz. For random
vibration analysis, units of g2 Hzâ1 are frequently used for the PSD of
acceleration. Here g denotes the g-force.[7]
Mathematically, it is not necessary to assign physical dimensions to the signal
or to the independent variable. In the following discussion the meaning of x(t)
will remain unspecified, but the independent variable will be assumed to be
that of time.
***** Definition[edit] *****
**** Energy spectral density[edit] ****
"Energy spectral density" redirects here. It is not to be confused with Energy
spectrum.
Energy spectral density describes how the energy of a signal or a time_series
is distributed with frequency. Here, the term energy is used in the generalized
sense of signal processing;[8] that is, the energy     E   {\displaystyle E}
[E] of a signal     x ( t )   {\displaystyle x(t)}  [x(t)] is
         E =  &#x222B;  &#x2212; &#x221E;   &#x221E;    |  x ( t )   |   2    d
      t .   {\displaystyle E=\int _{-\infty }^{\infty }|x(t)|^{2}\,dt.}  [
      {\displaystyle E=\int _{-\infty }^{\infty }|x(t)|^{2}\,dt.}]
The energy spectral density is most suitable for transientsâthat is, pulse-
like signalsâhaving a finite total energy. In this case, Parseval's_theorem
[9] gives us an alternate expression for the energy of the signal:
          &#x222B;  &#x2212; &#x221E;   &#x221E;    |  x ( t )   |   2    d t =
      &#x222B;  &#x2212; &#x221E;   &#x221E;    |     x &#x005E;    ( f )   |
      2    d f ,   {\displaystyle \int _{-\infty }^{\infty }|x(t)|^{2}\,dt=\int
      _{-\infty }^{\infty }|{\hat {x}}(f)|^{2}\,df,}  [{\displaystyle \int _{-
      \infty }^{\infty }|x(t)|^{2}\,dt=\int _{-\infty }^{\infty }|{\hat {x}}
      (f)|^{2}\,df,}]
where
            x &#x005E;    ( f ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;    e
      &#x2212; 2 &#x03C0; i f t   x ( t )  d t ,   {\displaystyle {\hat {x}}
      (f)=\int _{-\infty }^{\infty }e^{-2\pi ift}x(t)\,dt,}  [{\displaystyle
      {\hat {x}}(f)=\int _{-\infty }^{\infty }e^{-2\pi ift}x(t)\,dt,}]
is the Fourier_transform of the signal and     f   {\displaystyle f}  [f] is
the frequency in Hz, i.e., cycles per second. Often used is the angular
frequency     &#x03C9; = 2 &#x03C0; f   {\displaystyle \omega =2\pi f}  [\omega
=2\pi f]. Since the integral on the right-hand side is the energy of the
signal, the integrand       |     x &#x005E;    ( f )  |   2     {\displaystyle
\left|{\hat {x}}(f)\right|^{2}}  [{\displaystyle \left|{\hat {x}}(f)\right|^
{2}}] can be interpreted as a density_function describing the energy per unit
frequency contained in the signal at the frequency     f   {\displaystyle f}
[f]. In light of this, the energy spectral density of a signal     x ( t )
{\displaystyle x(t)}  [x(t)] is defined as[9]
    S  x x   ( f ) =   |     x &#x005E;    ( f )  |   2         
{\displaystyle S_{xx}(f)=\left|{\hat {x}}(f)\right|^{2}}  [       (Eq.1)
{\displaystyle S_{xx}(f)=\left|{\hat {x}}(f)\right|^{2}}]
As a physical example of how one might measure the energy spectral density of a
signal, suppose     V ( t )   {\displaystyle V(t)}  [V(t)] represents the
potential (in volts) of an electrical pulse propagating along a transmission
line of impedance     Z   {\displaystyle Z}  [Z], and suppose the line is
terminated with a matched resistor (so that all of the pulse energy is
delivered to the resistor and none is reflected back). By Ohm's_law, the power
delivered to the resistor at time     t   {\displaystyle t}  [t] is equal to
V ( t  )  2    /  Z   {\displaystyle V(t)^{2}/Z}  [V(t)^{2}/Z], so the total
energy is found by integrating     V ( t  )  2    /  Z   {\displaystyle V(t)^
{2}/Z}  [V(t)^{2}/Z] with respect to time over the duration of the pulse. To
find the value of the energy spectral density      S  x x   ( f )
{\displaystyle S_{xx}(f)}  [S_{{xx}}(f)] at frequency     f   {\displaystyle f}
[f], one could insert between the transmission line and the resistor a bandpass
filter which passes only a narrow range of frequencies (    &#x0394; f
{\displaystyle \Delta f}  [\Delta f], say) near the frequency of interest and
then measure the total energy     E ( f )   {\displaystyle E(f)}  [E(f)]
dissipated across the resistor. The value of the energy spectral density at
f   {\displaystyle f}  [f] is then estimated to be     E ( f )  /  &#x0394; f
{\displaystyle E(f)/\Delta f}  [E(f)/\Delta f]. In this example, since the
power     V ( t  )  2    /  Z   {\displaystyle V(t)^{2}/Z}  [V(t)^{2}/Z] has
units of V2 Î©â1, the energy     E ( f )   {\displaystyle E(f)}  [E(f)] has
units of V2 s Î©â1 = J, and hence the estimate     E ( f )  /  &#x0394; f
{\displaystyle E(f)/\Delta f}  [E(f)/\Delta f] of the energy spectral density
has units of J Hzâ1, as required. In many situations, it is common to forgo
the step of dividing by     Z   {\displaystyle Z}  [Z] so that the energy
spectral density instead has units of V2 s Hzâ1.
This definition generalizes in a straightforward manner to a discrete signal
with an infinite number of values      x  n     {\displaystyle x_{n}}  [x_{n}]
such as a signal sampled at discrete times      x  n   = x ( n &#x0394; t )
{\displaystyle x_{n}=x(n\Delta t)}  [x_{n}=x(n\Delta t)]:
          S  x x   ( f ) = ( &#x0394; t  )  2     |   &#x2211;  n = &#x2212;
      &#x221E;   &#x221E;    x  n    e  &#x2212; 2 &#x03C0; i f n &#x0394; t
      |   2   =     x &#x005E;     d   ( f )     x &#x005E;     d   &#x2217;
      ( f ) ,   {\displaystyle S_{xx}(f)=(\Delta t)^{2}\left|\sum _{n=-\infty
      }^{\infty }x_{n}e^{-2\pi ifn\Delta t}\right|^{2}={\hat {x}}_{d}(f){\hat
      {x}}_{d}^{*}(f),}  [{\displaystyle S_{xx}(f)=(\Delta t)^{2}\left|\sum _
      {n=-\infty }^{\infty }x_{n}e^{-2\pi ifn\Delta t}\right|^{2}={\hat {x}}_
      {d}(f){\hat {x}}_{d}^{*}(f),}]
where         x &#x005E;     d   ( f )   {\displaystyle {\hat {x}}_{d}(f)}  [
{\hat {x}}_{d}(f)] is the discrete_Fourier_transform of      x  n
{\displaystyle x_{n}}  [x_{n}] and         x &#x005E;     d   &#x2217;   ( f )
{\displaystyle {\hat {x}}_{d}^{*}(f)}  [{\hat {x}}_{d}^{*}(f)] is the complex
conjugate of         x &#x005E;     d   ( f ) .   {\displaystyle {\hat {x}}_{d}
(f).}  [{\displaystyle {\hat {x}}_{d}(f).}] The sampling interval     &#x0394;
t   {\displaystyle \Delta t}  [\Delta t] is needed to keep the correct physical
units and to ensure that we recover the continuous case in the limit
&#x0394; t &#x2192; 0   {\displaystyle \Delta t\to 0}  [{\displaystyle \Delta
t\to 0}]; however, in the mathematical sciences, the interval is often set to
1.
**** Power spectral density[edit] ****
Not to be confused with Spectral_power_distribution.
The above definition of energy spectral density is suitable for transients
(pulse-like signals) whose energy is concentrated around one time window; then
the Fourier transforms of the signals generally exist. For continuous signals
over all time, such as stationary_processes, one must rather define the power
spectral density (PSD); this describes how power of a signal or time series is
distributed over frequency, as in the simple example given previously. Here,
power can be the actual physical power, or more often, for convenience with
abstract signals, is simply identified with the squared value of the signal.
For example, statisticians study the variance of a function over time     x ( t
)   {\displaystyle x(t)}  [x(t)] (or over another independent variable), and
using an analogy with electrical signals (among other physical processes), it
is customary to refer to it as the power spectrum even when there is no
physical power involved. If one were to create a physical voltage source which
followed     x ( t )   {\displaystyle x(t)}  [x(t)] and applied it to the
terminals of a 1 ohm resistor, then indeed the instantaneous power dissipated
in that resistor would be given by     x ( t  )  2     {\displaystyle x(t)^{2}}
[{\displaystyle x(t)^{2}}] watts.
The average power     P   {\displaystyle P}  [P] of a signal     x ( t )
{\displaystyle x(t)}  [x(t)] over all time is therefore given by the following
time average:
         P =  lim  T &#x2192; &#x221E;     1 T    &#x222B;  0   T    |  x ( t )
      |   2    d t   {\displaystyle P=\lim _{T\to \infty }{\frac {1}{T}}\int _
      {0}^{T}|x(t)|^{2}\,dt}  [{\displaystyle P=\lim _{T\to \infty }{\frac {1}
      {T}}\int _{0}^{T}|x(t)|^{2}\,dt}].
Note that a stationary_process, for instance, may have a finite power but an
infinite energy. After all, energy is the integral of power, and the stationary
signal continues over an infinite time. That is the reason that we cannot use
the energy spectral density as defined above in such cases.
In analyzing the frequency content of the signal     x ( t )   {\displaystyle x
(t)}  [x(t)], one might like to compute the ordinary Fourier transform        x
&#x005E;    ( &#x03C9; )   {\displaystyle {\hat {x}}(\omega )}  [{\hat {x}}
(\omega )]; however, for many signals of interest the Fourier transform does
not formally exist.[N_1] Because of this complication one can as well work with
a truncated Fourier transform where the signal is integrated only over a finite
interval     [ 0 , T ]   {\displaystyle [0,T]}  [[0,T]]:
            x &#x005E;    ( &#x03C9; ) =   1  T     &#x222B;  0   T   x ( t )
      e  &#x2212; i &#x03C9; t    d t   {\displaystyle {\hat {x}}(\omega )=
      {\frac {1}{\sqrt {T}}}\int _{0}^{T}x(t)e^{-i\omega t}\,dt}  [
      {\displaystyle {\hat {x}}(\omega )={\frac {1}{\sqrt {T}}}\int _{0}^{T}x
      (t)e^{-i\omega t}\,dt}].
This is the amplitude spectral density. Then the power spectral density can be
defined as[11][12]
    S  x x   ( &#x03C9; ) =  lim  T &#x2192; &#x221E;    E   [   |
x &#x005E;    ( &#x03C9; )  |   2   ]    {\displaystyle S_{xx}
(\omega )=\lim _{T\to \infty }\mathbf {E} \left[\left|{\hat {x}}      (Eq.2)
(\omega )\right|^{2}\right]}  [{\displaystyle S_{xx}(\omega )=\lim    
_{T\to \infty }\mathbf {E} \left[\left|{\hat {x}}(\omega )\right|^
{2}\right]}]
Here      E    {\textstyle \mathbf {E} }  [{\textstyle \mathbf {E} }] denotes
the expected_value; explicitly, we have[12]
          E   [   |     x &#x005E;    ( &#x03C9; )  |   2   ]  =  E   [    1 T
      &#x222B;  0   T    x  &#x2217;   ( t )  e  i &#x03C9; t    d t  &#x222B;
      0   T   x (  t &#x2032;  )  e  &#x2212; i &#x03C9;  t &#x2032;     d  t
      &#x2032;   ]  =   1 T    &#x222B;  0   T    &#x222B;  0   T    E   [   x
      &#x2217;   ( t ) x (  t &#x2032;  )  ]   e  i &#x03C9; ( t &#x2212;  t
      &#x2032;  )    d t  d  t &#x2032;  .   {\displaystyle \mathbf {E} \left
      [\left|{\hat {x}}(\omega )\right|^{2}\right]=\mathbf {E} \left[{\frac {1}
      {T}}\int _{0}^{T}x^{*}(t)e^{i\omega t}\,dt\int _{0}^{T}x(t')e^{-i\omega
      t'}\,dt'\right]={\frac {1}{T}}\int _{0}^{T}\int _{0}^{T}\mathbf {E} \left
      [x^{*}(t)x(t')\right]e^{i\omega (t-t')}\,dt\,dt'.}  [{\displaystyle
      \mathbf {E} \left[\left|{\hat {x}}(\omega )\right|^{2}\right]=\mathbf {E}
      \left[{\frac {1}{T}}\int _{0}^{T}x^{*}(t)e^{i\omega t}\,dt\int _{0}^{T}x
      (t')e^{-i\omega t'}\,dt'\right]={\frac {1}{T}}\int _{0}^{T}\int _{0}^
      {T}\mathbf {E} \left[x^{*}(t)x(t')\right]e^{i\omega (t-t')}\,dt\,dt'.}]
In the latter form (for a stationary_random_process), one can make the change
of variables     &#x0394; t = t &#x2212;  t &#x2032;    {\displaystyle \Delta
t=t-t'}  [\Delta t=t-t'] and with the limits of integration (rather than
[ 0 , T ]   {\displaystyle [0,T]}  [[0,T]]) approaching infinity, the resulting
power spectral density      S  x x   ( &#x03C9; )   {\displaystyle S_{xx}
(\omega )}  [S_{xx}(\omega )] and the autocorrelation_function of this signal
are seen to be Fourier transform pairs (WienerâKhinchin_theorem). The
autocorrelation function is a statistic defined as
          R  x x   ( &#x03C4; ) = &#x27E8; X ( t ) X ( t + &#x03C4; ) &#x27E9;
      =  E  [ X ( t ) X ( t + &#x03C4; ) ]   {\displaystyle R_{xx}(\tau
      )=\langle X(t)X(t+\tau )\rangle =\mathbf {E} [X(t)X(t+\tau )]}  [
      {\displaystyle R_{xx}(\tau )=\langle X(t)X(t+\tau )\rangle =\mathbf {E}
      [X(t)X(t+\tau )]}]
or more generally as
          R  x x   ( &#x03C4; ) = &#x27E8; X ( t ) X ( t &#x2212; &#x03C4;  )
      &#x2217;   &#x27E9; = &#x27E8; X ( t  )  &#x2217;   X ( t + &#x03C4; )
      &#x27E9;   {\displaystyle R_{xx}(\tau )=\langle X(t)X(t-\tau )^{*}\rangle
      =\langle X(t)^{*}X(t+\tau )\rangle }  [{\displaystyle R_{xx}(\tau
      )=\langle X(t)X(t-\tau )^{*}\rangle =\langle X(t)^{*}X(t+\tau )\rangle }]
in the case that     X ( t )   {\displaystyle X(t)}  [X(t)] is complex-valued.
Provided that      R  x x   ( &#x03C4; )   {\displaystyle R_{xx}(\tau )}  [
{\displaystyle R_{xx}(\tau )}] is absolutely integrable (which is not always
true)[13],
    S  x x   ( &#x03C9; ) =  &#x222B;  &#x2212; &#x221E;
&#x221E;    R  x x   ( &#x03C4; )  e  &#x2212; i &#x03C9; &#x03C4;
d &#x03C4; =     R &#x005E;     x x   ( &#x03C9; )                    
{\displaystyle S_{xx}(\omega )=\int _{-\infty }^{\infty }R_{xx}         (Eq.3)
(\tau )e^{-i\omega \tau }\,d\tau ={\hat {R}}_{xx}(\omega )}  [
{\displaystyle S_{xx}(\omega )=\int _{-\infty }^{\infty }R_{xx}
(\tau )e^{-i\omega \tau }\,d\tau ={\hat {R}}_{xx}(\omega )}]
Many authors use this equality to actually define the power spectral density.
[14]
The power of the signal in a given frequency band     [  f  1   ,  f  2   ]
{\displaystyle [f_{1},f_{2}]}  [[f_{1},f_{2}]] (or     [  &#x03C9;  1   ,
&#x03C9;  2   ]   {\displaystyle [\omega _{1},\omega _{2}]}  [[\omega _
{1},\omega _{2}]]) can be calculated by integrating over frequency. Since
S  x x   ( &#x2212; &#x03C9; ) =  S  x x   ( &#x03C9; )   {\displaystyle S_{xx}
(-\omega )=S_{xx}(\omega )}  [S_{xx}(-\omega )=S_{xx}(\omega )], an equal
amount of power can be attributed to positive and negative frequencies, which
accounts for the factor of 2 in the following form (such trivial factors
dependent on conventions used):
          P   b a n d l i m i t e d    = 2  &#x222B;   f  1      f  2      S  x
      x   ( 2 &#x03C0;  f )  d f =   1 &#x03C0;    &#x222B;   &#x03C9;  1
      &#x03C9;  2      S  x x   ( &#x03C9; ) d &#x03C9;   {\displaystyle P_
      {\mathsf {bandlimited}}=2\int _{f_{1}}^{f_{2}}S_{xx}(2\pi \!f)\,df={\frac
      {1}{\pi }}\int _{\omega _{1}}^{\omega _{2}}S_{xx}(\omega )d\omega }  [
      {\displaystyle P_{\mathsf {bandlimited}}=2\int _{f_{1}}^{f_{2}}S_{xx}
      (2\pi \!f)\,df={\frac {1}{\pi }}\int _{\omega _{1}}^{\omega _{2}}S_{xx}
      (\omega )d\omega }]
More generally, similar techniques may be used to estimate a time-varying
spectral density. In this case the truncated Fourier transform defined above
over the finite time interval     ( 0 , T )   {\displaystyle (0,T)}  [
{\displaystyle (0,T)}] is not evaluated in the limit of     T   {\displaystyle
T}  [T] approaching infinity. This results in decreased spectral coverage and
resolution since frequencies of less than     1  /  T   {\displaystyle 1/T}
[1/T] are not sampled, and results at frequencies which are not an integer
multiple of     1  /  T   {\displaystyle 1/T}  [1/T] are not independent. Just
using a single such time series, the estimated power spectrum will be very
"noisy"; however this can be alleviated if it is possible to evaluate the
expected value (in the above equation) using a large (or infinite) number of
short-term spectra corresponding to statistical_ensembles of realizations of
x ( t )   {\displaystyle x(t)}  [x(t)] evaluated over the specified time
window.
This definition of the power spectral density can be generalized to discrete
time variables      x  n     {\displaystyle x_{n}}  [x_{n}]. As above we can
consider a finite window of     1 &#x2264; n &#x2264; N   {\displaystyle 1\leq
n\leq N}  [1\leq n\leq N] with the signal sampled at discrete times      x  n
= x ( n &#x0394; t )   {\displaystyle x_{n}=x(n\Delta t)}  [x_{n}=x(n\Delta t)]
for a total measurement period     T = N &#x0394; t   {\displaystyle T=N\Delta
t}  [T=N\Delta t]. Then a single estimate of the PSD can be obtained through
summation rather than integration:
             S &#x007E;     x x   ( &#x03C9; ) =    ( &#x0394; t  )  2    T
      |   &#x2211;  n = 1   N    x  n    e  &#x2212; i &#x03C9; n &#x0394; t
      |   2     {\displaystyle {\tilde {S}}_{xx}(\omega )={\frac {(\Delta t)^
      {2}}{T}}\left|\sum _{n=1}^{N}x_{n}e^{-i\omega n\Delta t}\right|^{2}}  [
      {\displaystyle {\tilde {S}}_{xx}(\omega )={\frac {(\Delta t)^{2}}
      {T}}\left|\sum _{n=1}^{N}x_{n}e^{-i\omega n\Delta t}\right|^{2}}].
As before, the actual PSD is achieved when     N   {\displaystyle N}  [N] (and
thus     T   {\displaystyle T}  [T]) approach infinity and the expected value
is formally applied. In a real-world application, one would typically average
this single-measurement PSD over many trials to obtain a more accurate estimate
of the theoretical PSD of the physical process underlying the individual
measurements. This computed PSD is sometimes called a periodogram. This
periodogram converges to the true PSD as the number of estimates as well as the
averaging time interval     T   {\displaystyle T}  [T] approach infinity (Brown
& Hwang[15]).
If two signals both possess power spectral densities, then the #Cross-spectral
density can similarly be calculated; as the PSD is related to the
autocorrelation, so is the cross-spectral density related to the cross-
correlation.
*** Properties of the power spectral density[edit] ***
Some properties of the PSD include:[16]
    * The spectrum of a real valued process (or even a complex process using
      the above definition) is real and an even_function of frequency:      S
      x x   ( &#x2212; &#x03C9; ) =  S  x x   ( &#x03C9; )   {\displaystyle S_
      {xx}(-\omega )=S_{xx}(\omega )}  [S_{xx}(-\omega )=S_{xx}(\omega )].
    * If the process is continuous and purely indeterministic[clarification
      needed], the autocovariance function can be reconstructed by using the
      Inverse_Fourier_transform
    * The PSD can be used to compute the variance (net power) of a process by
      integrating over frequency:
                Var  (  X  n   ) =   1 &#x03C0;    &#x222B;  0   &#x221E;     S
            x x   ( &#x03C9; )  d &#x03C9; .   {\displaystyle {\text{Var}}(X_
            {n})={\frac {1}{\pi }}\int _{0}^{\infty }\!S_{xx}(\omega )\,d\omega
            .}  [{\displaystyle {\text{Var}}(X_{n})={\frac {1}{\pi }}\int _{0}^
            {\infty }\!S_{xx}(\omega )\,d\omega .}]
    * Being based on the Fourier transform, the PSD is a linear function of the
      autocovariance function in the sense that if      R  x x
      {\displaystyle R_{xx}}  [R_{{xx}}] is decomposed into two functions
                R  x x   ( &#x03C4; ) =  &#x03B1;  1    R  x x , 1   ( &#x03C4;
            ) +  &#x03B1;  2    R  x x , 2   ( &#x03C4; )   {\displaystyle R_
            {xx}(\tau )=\alpha _{1}R_{xx,1}(\tau )+\alpha _{2}R_{xx,2}(\tau )}
            [{\displaystyle R_{xx}(\tau )=\alpha _{1}R_{xx,1}(\tau )+\alpha _
            {2}R_{xx,2}(\tau )}] ,
      then
                S  x x   ( &#x03C9; ) =  &#x03B1;  1    S  x x , 1   ( &#x03C9;
            ) +  &#x03B1;  2    S  x x , 2   ( &#x03C9; ) .   {\displaystyle S_
            {xx}(\omega )=\alpha _{1}S_{xx,1}(\omega )+\alpha _{2}S_{xx,2}
            (\omega ).}  [{\displaystyle S_{xx}(\omega )=\alpha _{1}S_{xx,1}
            (\omega )+\alpha _{2}S_{xx,2}(\omega ).}]
The integrated spectrum or power spectral distribution     F ( &#x03C9; )
{\displaystyle F(\omega )}  [F(\omega )] is defined as[dubious  – discuss][17]
         F ( &#x03C9; ) =  &#x222B;  &#x2212; &#x221E;   &#x03C9;    S  x x
      (  &#x03C9; &#x2032;  )  d  &#x03C9; &#x2032;  .   {\displaystyle F
      (\omega )=\int _{-\infty }^{\omega }S_{xx}(\omega ')\,d\omega '.}  [F
      (\omega )=\int _{-\infty }^{\omega }S_{xx}(\omega ')\,d\omega '.]
**** Cross power spectral density [edit] ****
See also: Coherence_(signal_processing)
Given two signals     x ( t )   {\displaystyle x(t)}  [x(t)] and     y ( t )
{\displaystyle y(t)}  [y(t)], each of which possess power spectral densities
S  x x   ( &#x03C9; )   {\displaystyle S_{xx}(\omega )}  [S_{xx}(\omega )] and
S  y y   ( &#x03C9; )   {\displaystyle S_{yy}(\omega )}  [S_{yy}(\omega )], it
is possible to define a cross power spectral density (CPSD) or cross spectral
density (CSD) given by
          S  x y   ( &#x03C9; ) =  lim  T &#x2192; &#x221E;    E   [    (   F
      x   T   ( &#x03C9; )  )   &#x2217;    F  y   T   ( &#x03C9; )  ]  .
      {\displaystyle S_{xy}(\omega )=\lim _{T\to \infty }\mathbf {E} \left
      [\left(F_{x}^{T}(\omega )\right)^{*}F_{y}^{T}(\omega )\right].}  [
      {\displaystyle S_{xy}(\omega )=\lim _{T\to \infty }\mathbf {E} \left
      [\left(F_{x}^{T}(\omega )\right)^{*}F_{y}^{T}(\omega )\right].}]
The cross-spectral density (or 'cross power spectrum') is thus the Fourier
transform of the cross-correlation function.
          S  x y   ( &#x03C9; ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;    R
      x y   ( t )  e  &#x2212; j &#x03C9; t   d t =  &#x222B;  &#x2212;
      &#x221E;   &#x221E;    [   &#x222B;  &#x2212; &#x221E;   &#x221E;   x
      ( &#x03C4; ) &#x22C5; y ( &#x03C4; + t ) d &#x03C4;  ]   e  &#x2212; j
      &#x03C9; t   d t ,   {\displaystyle S_{xy}(\omega )=\int _{-\infty }^
      {\infty }R_{xy}(t)e^{-j\omega t}dt=\int _{-\infty }^{\infty }\left[\int _
      {-\infty }^{\infty }x(\tau )\cdot y(\tau +t)d\tau \right]e^{-j\omega
      t}dt,}  [{\displaystyle S_{xy}(\omega )=\int _{-\infty }^{\infty }R_{xy}
      (t)e^{-j\omega t}dt=\int _{-\infty }^{\infty }\left[\int _{-\infty }^
      {\infty }x(\tau )\cdot y(\tau +t)d\tau \right]e^{-j\omega t}dt,}]
where      R  x y   ( t )   {\displaystyle R_{xy}(t)}  [R_{{xy}}(t)] is the
cross-correlation of     x ( t )   {\displaystyle x(t)}  [x(t)] and     y ( t )
{\displaystyle y(t)}  [y(t)].
By an extension of the WienerâKhinchin theorem, the Fourier transform of the
cross-spectral density      S  x y   ( &#x03C9; )   {\displaystyle S_{xy}
(\omega )}  [S_{xy}(\omega )] is the cross-covariance function.[18] In light of
this, the PSD is seen to be a special case of the CSD for     x ( t ) = y ( t )
{\displaystyle x(t)=y(t)}  [x(t)=y(t)].
For discrete signals xn and yn, the relationship between the cross-spectral
density and the cross-covariance is
          S  x y   ( &#x03C9; ) =   1  2 &#x03C0;     &#x2211;  n = &#x2212;
      &#x221E;   &#x221E;    R  x y   ( n )  e  &#x2212; j &#x03C9; n
      {\displaystyle S_{xy}(\omega )={\frac {1}{2\pi }}\sum _{n=-\infty }^
      {\infty }R_{xy}(n)e^{-j\omega n}}  [{\displaystyle S_{xy}(\omega )={\frac
      {1}{2\pi }}\sum _{n=-\infty }^{\infty }R_{xy}(n)e^{-j\omega n}}]
***** Estimation[edit] *****
Main article: Spectral_density_estimation
The goal of spectral density estimation is to estimate the spectral density of
a random_signal from a sequence of time samples. Depending on what is known
about the signal, estimation techniques can involve parametric or non-
parametric approaches, and may be based on time-domain or frequency-domain
analysis. For example, a common parametric technique involves fitting the
observations to an autoregressive_model. A common non-parametric technique is
the periodogram.
The spectral density is usually estimated using Fourier_transform methods (such
as the Welch_method), but other techniques such as the maximum_entropy method
can also be used.
***** Properties[edit] *****
    * The spectral density of     f ( t )   {\displaystyle f(t)}  [f(t)] and
      the autocorrelation of     f ( t )   {\displaystyle f(t)}  [f(t)] form a
      Fourier transform pair (for PSD versus ESD, different definitions of
      autocorrelation function are used). This result is known as
      WienerâKhinchin_theorem.
    * One of the results of Fourier analysis is Parseval's_theorem which states
      that the area under the energy spectral density curve is equal to the
      area under the square of the magnitude of the signal, the total energy:
                &#x222B;  &#x2212; &#x221E;   &#x221E;     |  f ( t )  |   2
            d t =  &#x222B;  &#x2212; &#x221E;   &#x221E;   E S D ( &#x03C9; )
            d &#x03C9; .   {\displaystyle \int _{-\infty }^{\infty }\left|f
            (t)\right|^{2}\,dt=\int _{-\infty }^{\infty }ESD(\omega )\,d\omega
            .}  [\int _{-\infty }^{\infty }\left|f(t)\right|^{2}\,dt=\int _{-
            \infty }^{\infty }ESD(\omega )\,d\omega .]
      The above theorem holds true in the discrete cases as well. A similar
      result holds for power: the area under the power spectral density curve
      is equal to the total signal power, which is     R ( 0 )   {\displaystyle
      R(0)}  [R(0)], the autocorrelation function at zero lag. This is also (up
      to a constant which depends on the normalization factors chosen in the
      definitions employed) the variance of the data comprising the signal.
***** Related concepts[edit] *****
Not to be confused with Spectral_density_(physical_science).
    * The spectral_centroid of a signal is the midpoint of its spectral density
      function, i.e. the frequency that divides the distribution into two equal
      parts.
    * The spectral_edge_frequency of a signal is an extension of the previous
      concept to any proportion instead of two equal parts.
    * The spectral density is a function of frequency, not a function of time.
      However, the spectral density of small windows of a longer signal may be
      calculated, and plotted versus time associated with the window. Such a
      graph is called a spectrogram. This is the basis of a number of spectral
      analysis techniques such as the short-time_Fourier_transform and
      wavelets.
    * A "spectrum" generally means the power spectral density, as discussed
      above, which depicts the distribution of signal content over frequency.
      This is not to be confused with the frequency_response of a transfer
      function which also includes a phase (or equivalently, a real and
      imaginary part as a function of frequency). For transfer functions,
      (e.g., Bode_plot, chirp) the complete frequency response may be graphed
      in two parts, amplitude versus frequency and phase versus frequency (or
      less commonly, as real and imaginary parts of the transfer function). The
      impulse_response (in the time domain)     h ( t )   {\displaystyle h(t)}
      [h(t)], cannot generally be uniquely recovered from the amplitude
      spectral density part alone without the phase function. Although these
      are also Fourier transform pairs, there is no symmetry (as there is for
      the autocorrelation) forcing the Fourier transform to be real-valued. See
      spectral_phase and phase_noise.
***** Applications[edit] *****
**** Electrical engineering[edit] ****
Spectrogram of an FM_radio signal with frequency on the horizontal axis and
time increasing upwards on the vertical axis.
The concept and use of the power spectrum of a signal is fundamental in
electrical_engineering, especially in electronic_communication_systems,
including radio_communications, radars, and related systems, plus passive
remote_sensing technology. Electronic instruments called spectrum_analyzers are
used to observe and measure the power spectra of signals.
The spectrum analyzer measures the magnitude of the short-time_Fourier
transform (STFT) of an input signal. If the signal being analyzed can be
considered a stationary process, the STFT is a good smoothed estimate of its
power spectral density.
**** Cosmology[edit] ****
Primordial_fluctuations, density variations in the early universe, are
quantified by a power spectrum which gives the power of the variations as a
function of spatial scale.
***** See also[edit] *****
    * Noise_spectral_density
    * Spectral_density_estimation
    * Spectral_efficiency
    * Spectral_power_distribution
    * Brightness_temperature
    * Colors_of_noise
    * Spectral_leakage
    * Window_function
    * Bispectrum
    * Whittle_likelihood
***** Notes[edit] *****
   1. ^ Some authors (e.g. Risken[10]) still use the non-normalized Fourier
      transform in a formal way to formulate a definition of the power spectral
      density
               &#x27E8;    x &#x005E;    ( &#x03C9; )     x &#x005E;
            &#x2217;   (  &#x03C9; &#x2032;  ) &#x27E9; = 2 &#x03C0; f
            ( &#x03C9; ) &#x03B4; ( &#x03C9; &#x2212;  &#x03C9; &#x2032;  )
            {\displaystyle \langle {\hat {x}}(\omega ){\hat {x}}^{\ast }(\omega
            ')\rangle =2\pi f(\omega )\delta (\omega -\omega ')}  [
            {\displaystyle \langle {\hat {x}}(\omega ){\hat {x}}^{\ast }(\omega
            ')\rangle =2\pi f(\omega )\delta (\omega -\omega ')}],
      where     &#x03B4; ( &#x03C9; &#x2212;  &#x03C9; &#x2032;  )
      {\displaystyle \delta (\omega -\omega ')}  [\delta (\omega -\omega ')] is
      the Dirac_delta_function. Such formal statements may sometimes be useful
      to guide the intuition, but should always be used with utmost care.
***** References[edit] *****
   1. ^P_Stoica & R Moses (2005). "Spectral_Analysis_of_Signals" (PDF).
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
   3. ^P_Stoica & R Moses (2005). "Spectral_Analysis_of_Signals" (PDF).
   4. ^P_Stoica & R Moses (2005). "Spectral_Analysis_of_Signals" (PDF).
   5. ^GÃ©rard Maral (2003). VSAT_Networks. John Wiley and Sons. ISBN 978-0-
      470-86684-9.
   6. ^Michael Peter Norton & Denis G. Karczub (2003). Fundamentals_of_Noise
      and_Vibration_Analysis_for_Engineers. Cambridge_University_Press.
      ISBN 978-0-521-49913-2.
   7. ^Michael Cerna & Audrey F. Harvey (2000). "The_Fundamentals_of_FFT-Based
      Signal_Analysis_and_Measurement" (PDF).
   8. ^Alessandro Birolini (2007). Reliability_Engineering. Springer. p. 83.
      ISBN 978-3-540-49388-4.
   9. ^Oppenheim; Verghese. Signals, Systems, and Inference. pp. 32â4.
  10. ^ a bStein, Jonathan Y. (2000). Digital Signal Processing: A Computer
      Science Perspective. Wiley. p. 115.
  11. ^Hannes Risken (1996). The_FokkerâPlanck_Equation:_Methods_of_Solution
      and_Applications (2nd ed.). Springer. p. 30. ISBN 9783540615309.
  12. ^Fred Rieke; William Bialek & David Warland (1999). Spikes: Exploring the
      Neural Code (Computational Neuroscience). MIT_Press. ISBN 978-0262681087.
  13. ^ a bScott Millers & Donald Childers (2012). Probability and random
      processes. Academic_Press. pp. 370â5.
  14. ^ The WienerâKhinchin_theorem makes sense of this formula for any wide-
      sense_stationary_process under weaker hypotheses:      R  x x
      {\displaystyle R_{xx}}  [{\displaystyle R_{xx}}] does not need to be
      absolutely integrable, it only needs to exist. But the integral can no
      longer be interpreted as usual. The formula also makes sense if
      interpreted as involving distributions (in the sense of Laurent_Schwartz,
      not in the sense of a statistical Cumulative_distribution_function)
      instead of functions. If      R  x x     {\displaystyle R_{xx}}  [
      {\displaystyle R_{xx}}] is continuous, Bochner's_theorem can be used to
      prove that its Fourier transform exists as a positive measure, whose
      distribution function is F (but not necessarily as a function and not
      necessarily possessing a probability density).
  15. ^Dennis Ward Ricker (2003). Echo_Signal_Processing. Springer. ISBN 978-1-
      4020-7395-3.
  16. ^Robert Grover Brown & Patrick Y.C. Hwang (1997). Introduction to Random
      Signals and Applied Kalman Filtering. John_Wiley_&_Sons. ISBN 978-0-471-
      12839-7.
  17. ^Storch, H. Von; F. W Zwiers (2001). Statistical analysis in climate
      research. Cambridge University Press. ISBN 978-0-521-01230-0.
  18. ^ An Introduction to the Theory of Random Signals and Noise, Wilbur B.
      Davenport and Willian L. Root, IEEE Press, New York, 1987,
  19. ISBN 0-87942-235-1
  20. ^William D Penny (2009). "Signal_Processing_Course,_chapter_7".
***** External links[edit] *****
    * Power_Spectral_Density_Matlab_scripts
    * v
    * t
    * e
Decibel suffixes (dB)
    * dBm (or dBmW)
    * dBW
    * dBV
    * dBm/Hz
          o PSD
    * dBA
    * dBZ (radar)
    * dBsm
    * dBc
    * dBi
    * dBFS
    * dBrn
    * dB-Hz
  See also
      logarithmic_unit
      link_budget
      signal_noise
      telecommunication

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Spectral_density&oldid=902093426"
Categories:
    * Frequency-domain_analysis
    * Signal_processing
    * Waves
    * Spectroscopy
    * Scattering
    * Fourier_analysis
    * Radio_spectrum
Hidden categories:
    * Use_American_English_from_March_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * Wikipedia_articles_needing_clarification_from_December_2015
    * All_accuracy_disputes
    * Articles_with_disputed_statements_from_December_2015
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
    * Boarisch
    * CatalÃ 
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 16 June 2019, at 14:18 (UTC).
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
