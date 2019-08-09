The following text has been accessed from https://en.wikipedia.org/wiki/Fourier_analysis at Fri Aug 9 03:11:16 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Fourier analysis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Fourier_transforms
Continuous_Fourier_transform
Fourier_series
Discrete-time_Fourier_transform
Discrete_Fourier_transform
Discrete_Fourier_transform_over_a_ring
Fourier analysis
Related_transforms
Branch of mathematics regarding periodic and continuous signals
Bass guitar time signal of open string A note (55 Hz).
Fourier transform of bass guitar time signal of open string A note (55 Hz).
Fourier analysis reveals the oscillatory components of signals and functions.
In mathematics, Fourier analysis (/ËfÊrieÉª,_-iÉr/)[1] is the study of the
way general functions may be represented or approximated by sums of simpler
trigonometric_functions. Fourier analysis grew from the study of Fourier
series, and is named after Joseph_Fourier, who showed that representing a
function as a sum of trigonometric functions greatly simplifies the study of
heat_transfer.
Today, the subject of Fourier analysis encompasses a vast spectrum of
mathematics. In the sciences and engineering, the process of decomposing a
function into oscillatory components is often called Fourier analysis, while
the operation of rebuilding the function from these pieces is known as Fourier
synthesis. For example, determining what component frequencies are present in a
musical note would involve computing the Fourier transform of a sampled musical
note. One could then re-synthesize the same sound by including the frequency
components as revealed in the Fourier analysis. In mathematics, the term
Fourier analysis often refers to the study of both operations.
The decomposition process itself is called a Fourier_transformation. Its
output, the Fourier transform, is often given a more specific name, which
depends on the domain and other properties of the function being transformed.
Moreover, the original concept of Fourier analysis has been extended over time
to apply to more and more abstract and general situations, and the general
field is often known as harmonic_analysis. Each transform used for analysis
(see list_of_Fourier-related_transforms) has a corresponding inverse transform
that can be used for synthesis.
⁰
***** Contents *****
    * 1_Applications
          o 1.1_Applications_in_signal_processing
    * 2_Variants_of_Fourier_analysis
          o 2.1_(Continuous)_Fourier_transform
          o 2.2_Fourier_series
          o 2.3_Discrete-time_Fourier_transform_(DTFT)
          o 2.4_Discrete_Fourier_transform_(DFT)
          o 2.5_Summary
          o 2.6_Symmetry_properties
          o 2.7_Fourier_transforms_on_arbitrary_locally_compact_abelian
            topological_groups
          o 2.8_Timeâfrequency_transforms
    * 3_History
    * 4_Interpretation_in_terms_of_time_and_frequency
    * 5_See_also
    * 6_Notes
    * 7_References
    * 8_Further_reading
    * 9_External_links
***** Applications[edit] *****
Fourier analysis has many scientific applications â in physics, partial
differential_equations, number_theory, combinatorics, signal_processing,
digital_image_processing, probability_theory, statistics, forensics, option
pricing, cryptography, numerical_analysis, acoustics, oceanography, sonar,
optics, diffraction, geometry, protein structure analysis, and other areas.
This wide applicability stems from many useful properties of the transforms:
    * The transforms are linear_operators and, with proper normalization, are
      unitary as well (a property known as Parseval's_theorem or, more
      generally, as the Plancherel_theorem, and most generally via Pontryagin
      duality) (Rudin_1990).
    * The transforms are usually invertible.
    * The exponential_functions are eigenfunctions of differentiation, which
      means that this representation transforms linear differential_equations
      with constant_coefficients into ordinary algebraic ones (Evans_1998).
      Therefore, the behavior of a linear_time-invariant_system can be analyzed
      at each frequency independently.
    * By the convolution_theorem, Fourier transforms turn the complicated
      convolution operation into simple multiplication, which means that they
      provide an efficient way to compute convolution-based operations such as
      polynomial multiplication and multiplying_large_numbers (Knuth_1997).
    * The discrete version of the Fourier transform (see below) can be
      evaluated quickly on computers using Fast_Fourier_Transform (FFT)
      algorithms. (Conte_&_de_Boor_1980)
In forensics, laboratory infrared spectrophotometers use Fourier transform
analysis for measuring the wavelengths of light at which a material will absorb
in the infrared spectrum. The FT method is used to decode the measured signals
and record the wavelength data. And by using a computer, these Fourier
calculations are rapidly carried out, so that in a matter of seconds, a
computer-operated FT-IR instrument can produce an infrared absorption pattern
comparable to that of a prism instrument.[2]
Fourier transformation is also useful as a compact representation of a signal.
For example, JPEG compression uses a variant of the Fourier transformation
(discrete_cosine_transform) of small square pieces of a digital image. The
Fourier components of each square are rounded to lower arithmetic_precision,
and weak components are eliminated entirely, so that the remaining components
can be stored very compactly. In image reconstruction, each image square is
reassembled from the preserved approximate Fourier-transformed components,
which are then inverse-transformed to produce an approximation of the original
image.
**** Applications in signal processing[edit] ****
When processing signals, such as audio, radio_waves, light waves, seismic
waves, and even images, Fourier analysis can isolate narrowband components of a
compound waveform, concentrating them for easier detection or removal. A large
family of signal processing techniques consist of Fourier-transforming a
signal, manipulating the Fourier-transformed data in a simple way, and
reversing the transformation.[3]
Some examples include:
    * Equalization of audio recordings with a series of bandpass_filters;
    * Digital radio reception without a superheterodyne circuit, as in a modern
      cell phone or radio_scanner;
    * Image_processing to remove periodic or anisotropic artifacts such as
      jaggies from interlaced video, strip artifacts from strip_aerial
      photography, or wave patterns from radio_frequency_interference in a
      digital camera;
    * Cross_correlation of similar images for co-alignment;
    * X-ray_crystallography to reconstruct a crystal structure from its
      diffraction pattern;
    * Fourier_transform_ion_cyclotron_resonance mass spectrometry to determine
      the mass of ions from the frequency of cyclotron motion in a magnetic
      field;
    * Many other forms of spectroscopy, including infrared and nuclear_magnetic
      resonance spectroscopies;
    * Generation of sound spectrograms used to analyze sounds;
    * Passive sonar used to classify targets based on machinery noise.
***** Variants of Fourier analysis[edit] *****
A Fourier transform and 3 variations caused by periodic sampling (at interval
T) and/or periodic summation (at interval P) of the underlying time-domain
function. The relative computational ease of the DFT sequence and the insight
it gives into S( f ) make it a popular analysis tool.
**** (Continuous) Fourier transform[edit] ****
Main article: Fourier_transform
Most often, the unqualified term Fourier transform refers to the transform of
functions of a continuous real argument, and it produces a continuous function
of frequency, known as a frequency distribution. One function is transformed
into another, and the operation is reversible. When the domain of the input
(initial) function is time (t), and the domain of the output (final) function
is ordinary_frequency, the transform of function s(t) at frequency f is given
by the complex number:
         S ( f ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;   s ( t ) &#x22C5;
      e  &#x2212; i 2 &#x03C0; f t    d t .   {\displaystyle S(f)=\int _{-
      \infty }^{\infty }s(t)\cdot e^{-i2\pi ft}\,dt.}  [{\displaystyle S
      (f)=\int _{-\infty }^{\infty }s(t)\cdot e^{-i2\pi ft}\,dt.}]
Evaluating this quantity for all values of f produces the frequency-domain
function. Then s(t) can be represented as a recombination of complex
exponentials of all possible frequencies:
         s ( t ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;   S ( f ) &#x22C5;
      e  i 2 &#x03C0; f t    d f ,   {\displaystyle s(t)=\int _{-\infty }^
      {\infty }S(f)\cdot e^{i2\pi ft}\,df,}  [{\displaystyle s(t)=\int _{-
      \infty }^{\infty }S(f)\cdot e^{i2\pi ft}\,df,}]
which is the inverse transform formula. The complex number, S( f ), conveys
both amplitude and phase of frequency f.
See Fourier_transform for much more information, including:
    * conventions for amplitude normalization and frequency scaling/units
    * transform properties
    * tabulated transforms of specific functions
    * an extension/generalization for functions of multiple dimensions, such as
      images.
**** Fourier series[edit] ****
Main article: Fourier_series
The Fourier transform of a periodic function, sP(t), with period P, becomes a
Dirac_comb function, modulated by a sequence of complex coefficients:
         S [ k ] =   1 P    &#x222B;  P    s  P   ( t ) &#x22C5;  e  &#x2212; i
      2 &#x03C0;   k P   t    d t   {\displaystyle S[k]={\frac {1}{P}}\int _
      {P}s_{P}(t)\cdot e^{-i2\pi {\frac {k}{P}}t}\,dt}  [{\displaystyle S[k]=
      {\frac {1}{P}}\int _{P}s_{P}(t)\cdot e^{-i2\pi {\frac {k}{P}}t}\,dt}]
for all integer values of k, and where â«P is the integral over any interval
of length P.
The inverse transform, known as Fourier series, is a representation of sP(t) in
terms of a summation of a potentially infinite number of harmonically related
sinusoids or complex_exponential functions, each with an amplitude and phase
specified by one of the coefficients:
          s  P   ( t ) =  &#x2211;  k = &#x2212; &#x221E;   &#x221E;   S [ k ]
      &#x22C5;  e  i 2 &#x03C0;   k P   t        &#x27FA;      F
      &#x2211;  k = &#x2212; &#x221E;   + &#x221E;   S [ k ]  &#x03B4;  (  f
      &#x2212;   k P    )  .   {\displaystyle s_{P}(t)=\sum _{k=-\infty }^
      {\infty }S[k]\cdot e^{i2\pi {\frac {k}{P}}t}\quad {\stackrel
      {\displaystyle {\mathcal {F}}}{\Longleftrightarrow }}\quad \sum _{k=-
      \infty }^{+\infty }S[k]\,\delta \left(f-{\frac {k}{P}}\right).}  [
      {\displaystyle s_{P}(t)=\sum _{k=-\infty }^{\infty }S[k]\cdot e^{i2\pi
      {\frac {k}{P}}t}\quad {\stackrel {\displaystyle {\mathcal {F}}}
      {\Longleftrightarrow }}\quad \sum _{k=-\infty }^{+\infty }S[k]\,\delta
      \left(f-{\frac {k}{P}}\right).}]
When sP(t), is expressed as a periodic_summation of another function, s(t):
          s  P   ( t )  &#x225C;   &#x2211;  m = &#x2212; &#x221E;   &#x221E;
      s ( t &#x2212; m P ) ,   {\displaystyle s_{P}(t)\,\triangleq \,\sum _{m=-
      \infty }^{\infty }s(t-mP),}  [{\displaystyle s_{P}(t)\,\triangleq \,\sum
      _{m=-\infty }^{\infty }s(t-mP),}]
the coefficients are proportional to samples of S( f ) at discrete intervals of
1/P:
         S [ k ] =   1 P   &#x22C5; S  (   k P   )  .   {\displaystyle S[k]=
      {\frac {1}{P}}\cdot S\left({\frac {k}{P}}\right).}  [{\displaystyle S[k]=
      {\frac {1}{P}}\cdot S\left({\frac {k}{P}}\right).}][note_1]
A sufficient condition for recovering s(t) (and therefore S( f )) from just
these samples (i.e. from the Fourier series) is that the non-zero portion of s
(t) be confined to a known interval of duration P, which is the frequency
domain dual of the NyquistâShannon_sampling_theorem.
See Fourier_series for more information, including the historical development.
**** Discrete-time Fourier transform (DTFT)[edit] ****
Main article: Discrete-time_Fourier_transform
The DTFT is the mathematical dual of the time-domain Fourier series. Thus, a
convergent periodic_summation in the frequency domain can be represented by a
Fourier series, whose coefficients are samples of a related continuous time
function:
          S   1 T    ( f ) &#xA0; &#x225C; &#xA0;      &#x2211;  k = &#x2212;
      &#x221E;   &#x221E;   S  (  f &#x2212;   k T    )  &#x2261;      &#x2211;
      n = &#x2212; &#x221E;   &#x221E;   s [ n ] &#x22C5;  e  &#x2212; i 2
      &#x03C0; f n T    &#x23DE;    Fourier series (DTFT)    &#x23DF;
      Poisson summation formula   =   F    {   &#x2211;  n = &#x2212; &#x221E;
      &#x221E;   s [ n ] &#xA0; &#x03B4; ( t &#x2212; n T )  }  ,
      {\displaystyle S_{\frac {1}{T}}(f)\ \triangleq \ \underbrace {\sum _{k=-
      \infty }^{\infty }S\left(f-{\frac {k}{T}}\right)\equiv \overbrace {\sum _
      {n=-\infty }^{\infty }s[n]\cdot e^{-i2\pi fnT}} ^{\text{Fourier series
      (DTFT)}}} _{\text{Poisson summation formula}}={\mathcal {F}}\left\{\sum _
      {n=-\infty }^{\infty }s[n]\ \delta (t-nT)\right\},\,}  [{\displaystyle S_
      {\frac {1}{T}}(f)\ \triangleq \ \underbrace {\sum _{k=-\infty }^{\infty
      }S\left(f-{\frac {k}{T}}\right)\equiv \overbrace {\sum _{n=-\infty }^
      {\infty }s[n]\cdot e^{-i2\pi fnT}} ^{\text{Fourier series (DTFT)}}} _
      {\text{Poisson summation formula}}={\mathcal {F}}\left\{\sum _{n=-\infty
      }^{\infty }s[n]\ \delta (t-nT)\right\},\,}]
which is known as the DTFT. Thus the DTFT of the s[n] sequence is also the
Fourier transform of the modulated Dirac_comb function.[note_2]
The Fourier series coefficients (and inverse transform), are defined by:
         s [ n ] &#xA0; &#x225C; &#xA0; T  &#x222B;   1 T     S   1 T    ( f )
      &#x22C5;  e  i 2 &#x03C0; f n T    d f = T      &#x222B;  &#x2212;
      &#x221E;   &#x221E;   S ( f ) &#x22C5;  e  i 2 &#x03C0; f n T    d f
      &#x23DF;    &#x225C;  s ( n T )   .   {\displaystyle s[n]\ \triangleq \
      T\int _{\frac {1}{T}}S_{\frac {1}{T}}(f)\cdot e^{i2\pi
      fnT}\,df=T\underbrace {\int _{-\infty }^{\infty }S(f)\cdot e^{i2\pi
      fnT}\,df} _{\triangleq \,s(nT)}.}  [{\displaystyle s[n]\ \triangleq \
      T\int _{\frac {1}{T}}S_{\frac {1}{T}}(f)\cdot e^{i2\pi
      fnT}\,df=T\underbrace {\int _{-\infty }^{\infty }S(f)\cdot e^{i2\pi
      fnT}\,df} _{\triangleq \,s(nT)}.}]
Parameter T corresponds to the sampling interval, and this Fourier series can
now be recognized as a form of the Poisson_summation_formula. Thus we have the
important result that when a discrete data sequence, s[n], is proportional to
samples of an underlying continuous function, s(t), one can observe a periodic
summation of the continuous Fourier transform, S( f ). That is a cornerstone in
the foundation of digital_signal_processing. Furthermore, under certain
idealized conditions one can theoretically recover S( f ) and s(t) exactly. A
sufficient condition for perfect recovery is that the non-zero portion of S
( f ) be confined to a known frequency interval of width 1/T. When that
interval is [â1/2T, 1/2T], the applicable reconstruction formula is the
WhittakerâShannon_interpolation_formula.
Another reason to be interested in S1/T( f ) is that it often provides insight
into the amount of aliasing caused by the sampling process.
Applications of the DTFT are not limited to sampled functions. See Discrete-
time_Fourier_transform for more information on this and other topics,
including:
    * normalized frequency units
    * windowing (finite-length sequences)
    * transform properties
    * tabulated transforms of specific functions
**** Discrete Fourier transform (DFT)[edit] ****
Main article: Discrete_Fourier_transform
Similar to a Fourier series, the DTFT of a periodic sequence, sN[n], with
period N, becomes a Dirac comb function, modulated by a sequence of complex
coefficients (see DTFT/Periodic_data):
         S [ k ] =  &#x2211;  n    s  N   [ n ] &#x22C5;  e  &#x2212; i 2
      &#x03C0;   k N   n   ,   {\displaystyle S[k]=\sum _{n}s_{N}[n]\cdot e^{-
      i2\pi {\frac {k}{N}}n},}  [{\displaystyle S[k]=\sum _{n}s_{N}[n]\cdot e^
      {-i2\pi {\frac {k}{N}}n},}]   where ân is the sum over any sequence of
      length N.
The S[k] sequence is what is customarily known as the DFT of {{math|sN.  It is
also N-periodic, so it is never necessary to compute more than N coefficients.
The inverse transform is given by:
          s  N   [ n ] =   1 N    &#x2211;  k   S [ k ] &#x22C5;  e  i 2
      &#x03C0;   n N   k   ,   {\displaystyle s_{N}[n]={\frac {1}{N}}\sum _{k}S
      [k]\cdot e^{i2\pi {\frac {n}{N}}k},}  [{\displaystyle s_{N}[n]={\frac {1}
      {N}}\sum _{k}S[k]\cdot e^{i2\pi {\frac {n}{N}}k},}]   where âk is the
      sum over any sequence of length N.
When sN[n] is expressed as a periodic_summation of another function:
          s  N   [ n ]  &#x225C;   &#x2211;  m = &#x2212; &#x221E;   &#x221E;
      s [ n &#x2212; m N ] ,   {\displaystyle s_{N}[n]\,\triangleq \,\sum _{m=-
      \infty }^{\infty }s[n-mN],}  [{\displaystyle s_{N}[n]\,\triangleq \,\sum
      _{m=-\infty }^{\infty }s[n-mN],}]   and       s [ n ]  &#x225C;  s ( n T
      ) ,   {\displaystyle s[n]\,\triangleq \,s(nT),}  [{\displaystyle s
      [n]\,\triangleq \,s(nT),}][note_3]
the coefficients are proportional to samples of S1/T( f ) at discrete intervals
of 1/P = 1/NT:
         S [ k ] =   1 T   &#x22C5;  S   1 T     (   k P   )  .
      {\displaystyle S[k]={\frac {1}{T}}\cdot S_{\frac {1}{T}}\left({\frac {k}
      {P}}\right).}  [{\displaystyle S[k]={\frac {1}{T}}\cdot S_{\frac {1}
      {T}}\left({\frac {k}{P}}\right).}][note_4]
Conversely, when one wants to compute an arbitrary number (N) of discrete
samples of one cycle of a continuous DTFT, S1/T( f ), it can be done by
computing the relatively simple DFT of sN[n], as defined above. In most cases,
N is chosen equal to the length of non-zero portion of s[n]. Increasing N,
known as zero-padding or interpolation, results in more closely spaced samples
of one cycle of S1/T( f ). Decreasing N, causes overlap (adding) in the time-
domain (analogous to aliasing), which corresponds to decimation in the
frequency domain. (see Sampling_the_DTFT) In most cases of practical interest,
the s[n] sequence represents a longer sequence that was truncated by the
application of a finite-length window_function or FIR_filter array.
The DFT can be computed using a fast_Fourier_transform (FFT) algorithm, which
makes it a practical and important transformation on computers.
See Discrete_Fourier_transform for much more information, including:
    * transform properties
    * applications
    * tabulated transforms of specific functions
**** Summary[edit] ****
For periodic functions, both the Fourier transform and the DTFT comprise only a
discrete set of frequency components (Fourier series), and the transforms
diverge at those frequencies. One common practice (not discussed above) is to
handle that divergence via Dirac_delta and Dirac_comb functions. But the same
spectral information can be discerned from just one cycle of the periodic
function, since all the other cycles are identical. Similarly, finite-duration
functions can be represented as a Fourier series, with no actual loss of
information except that the periodicity of the inverse transform is a mere
artifact.
We also note that it is common in practice for the duration of s(â¢) to be
limited to the period, P or N.  But these formulas do not require that
condition.
                       s(t) transforms (continuous-time)
          Continuous frequency               Discrete frequencies
                                                      1 P   &#x22C5; S  (   k P
                                             )   &#x23DE;    S [ k ]
                                             &#x225C;    1 P    &#x222B;
                                             &#x2212; &#x221E;   &#x221E;   s
                                             ( t ) &#x22C5;  e  &#x2212; i 2
                                             &#x03C0;   k P   t    d t &#x2261;
                                             1 P    &#x222B;  P    s  P   ( t )
             S ( f )  &#x225C;   &#x222B;    &#x22C5;  e  &#x2212; i 2 &#x03C0;
          &#x2212; &#x221E;   &#x221E;   s   k P   t    d t   {\displaystyle
          ( t ) &#x22C5;  e  &#x2212; i 2    \overbrace {{\frac {1}{P}}\cdot
          &#x03C0; f t    d t                S\left({\frac {k}{P}}\right)} ^{S
          {\displaystyle S(f)\,\triangleq    [k]}\,\triangleq \,{\frac {1}
Transform \,\int _{-\infty }^{\infty }s      {P}}\int _{-\infty }^{\infty }s
          (t)\cdot e^{-i2\pi ft}\,dt}  [     (t)\cdot e^{-i2\pi {\frac {k}
          {\displaystyle S(f)\,\triangleq    {P}}t}\,dt\equiv {\frac {1}
          \,\int _{-\infty }^{\infty }s      {P}}\int _{P}s_{P}(t)\cdot e^{-
          (t)\cdot e^{-i2\pi ft}\,dt}]       i2\pi {\frac {k}{P}}t}\,dt}  [
                                             {\displaystyle \overbrace {{\frac
                                             {1}{P}}\cdot S\left({\frac {k}
                                             {P}}\right)} ^{S[k]}\,\triangleq
                                             \,{\frac {1}{P}}\int _{-\infty }^
                                             {\infty }s(t)\cdot e^{-i2\pi
                                             {\frac {k}{P}}t}\,dt\equiv {\frac
                                             {1}{P}}\int _{P}s_{P}(t)\cdot e^{-
                                             i2\pi {\frac {k}{P}}t}\,dt}]
                                                     s  P   ( t ) =  &#x2211;
                                             k = &#x2212; &#x221E;   &#x221E;
                                             S [ k ] &#x22C5;  e  i 2 &#x03C0;
             s ( t ) =  &#x222B;  &#x2212;   k P   t    &#x23DF;    Poisson
          &#x221E;   &#x221E;   S ( f )      summation formula (Fourier series)
          &#x22C5;  e  i 2 &#x03C0; f t    d {\displaystyle \underbrace {s_{P}
          f   {\displaystyle s(t)=\int _{-   (t)=\sum _{k=-\infty }^{\infty }S
Inverse   \infty }^{\infty }S(f)\cdot e^     [k]\cdot e^{i2\pi {\frac {k}
          {i2\pi ft}\,df}  [{\displaystyle s {P}}t}} _{\text{Poisson summation
          (t)=\int _{-\infty }^{\infty }S    formula (Fourier series)}}\,}  [
          (f)\cdot e^{i2\pi ft}\,df}]        {\displaystyle \underbrace {s_{P}
                                             (t)=\sum _{k=-\infty }^{\infty }S
                                             [k]\cdot e^{i2\pi {\frac {k}
                                             {P}}t}} _{\text{Poisson summation
                                             formula (Fourier series)}}\,}]
                       s(nT) transforms (discrete-time)
          Continuous frequency               Discrete frequencies
                                                          1 T    S   1 T
                                             (   k  N T    )   &#x23DE;    S
                                             [ k ]       &#x225C;   &#x2211;  n
                                             = &#x2212; &#x221E;   &#x221E;   s
                                             ( n T ) &#x22C5;  e  &#x2212; i 2
                                             &#x03C0;    k n  N
                   1 T    S   1 T    ( f )   &#x2261;      &#x2211;  n    s  P
          &#x225C;   &#x2211;  n = &#x2212;  ( n T ) &#x22C5;  e  &#x2212; i 2
          &#x221E;   &#x221E;   s ( n T )    &#x03C0;    k n  N      &#x23DF;
          &#x22C5;  e  &#x2212; i 2 &#x03C0; DFT          {\displaystyle
          f n T    &#x23DF;    Poisson       {\begin{aligned}\overbrace {{\frac
          summation formula (DTFT)           {1}{T}}S_{\frac {1}{T}}\left(
          {\displaystyle \underbrace {{\frac {\frac {k}{NT}}\right)} ^{S
          {1}{T}}S_{\frac {1}{T}}            [k]}\,&\triangleq \,\sum _{n=-
Transform (f)\,\triangleq \,\sum _{n=-\infty \infty }^{\infty }s(nT)\cdot e^{-
          }^{\infty }s(nT)\cdot e^{-i2\pi    i2\pi {\frac {kn}{N}}}\\&\equiv
          fnT}} _{\text{Poisson summation    \underbrace {\sum _{n}s_{P}
          formula (DTFT)}}}  [{\displaystyle (nT)\cdot e^{-i2\pi {\frac {kn}
          \underbrace {{\frac {1}{T}}S_      {N}}}} _{\text{DFT}}\,\end
          {\frac {1}{T}}(f)\,\triangleq      {aligned}}}  [{\displaystyle
          \,\sum _{n=-\infty }^{\infty }s    {\begin{aligned}\overbrace {{\frac
          (nT)\cdot e^{-i2\pi fnT}} _{\text  {1}{T}}S_{\frac {1}{T}}\left(
          {Poisson summation formula         {\frac {k}{NT}}\right)} ^{S
          (DTFT)}}}]                         [k]}\,&\triangleq \,\sum _{n=-
                                             \infty }^{\infty }s(nT)\cdot e^{-
                                             i2\pi {\frac {kn}{N}}}\\&\equiv
                                             \underbrace {\sum _{n}s_{P}
                                             (nT)\cdot e^{-i2\pi {\frac {kn}
                                             {N}}}} _{\text{DFT}}\,\end
                                             {aligned}}}]
             s ( n T ) = T  &#x222B;   1 T
          1 T    S   1 T    ( f ) &#x22C5;
          e  i 2 &#x03C0; f n T    d f
          {\displaystyle s(nT)=T\int _{\frac
          {1}{T}}{\frac {1}{T}}S_{\frac {1}          s  P   ( n T )    =
          {T}}(f)\cdot e^{i2\pi fnT}\,df}  [ 1 N    &#x2211;  k   S [ k ]
          {\displaystyle s(nT)=T\int _{\frac &#x22C5;  e  i 2 &#x03C0;    k n
          {1}{T}}{\frac {1}{T}}S_{\frac {1}  N      &#x23DE;    inverse DFT
          {T}}(f)\cdot e^{i2\pi fnT}\,df}]   =    1 P     &#x2211;  k    S   1
              &#x2211;  n = &#x2212;         T     (   k P   )  &#x22C5;  e  i
          &#x221E;   &#x221E;   s ( n T )    2 &#x03C0;    k n  N
          &#x22C5; &#x03B4; ( t &#x2212; n T {\displaystyle {\begin{aligned}s_
          ) =      &#x222B;  &#x2212;        {P}(nT)&=\overbrace {{\frac {1}
          &#x221E;   &#x221E;     1 T        {N}}\sum _{k}S[k]\cdot e^{i2\pi
          &#xA0;  S   1 T    ( f ) &#x22C5;  {\frac {kn}{N}}}} ^{\text{inverse
Inverse   e  i 2 &#x03C0; f t    d f         DFT}}\\&={\tfrac {1}{P}}\sum _
          &#x23DF;    inverse Fourier        {k}S_{\frac {1}{T}}\left({\frac
          transform      {\displaystyle \sum {k}{P}}\right)\cdot e^{i2\pi
          _{n=-\infty }^{\infty }s(nT)\cdot  {\frac {kn}{N}}}\end{aligned}}}  [
          \delta (t-nT)=\underbrace {\int _  {\displaystyle {\begin{aligned}s_
          {-\infty }^{\infty }{\frac {1}     {P}(nT)&=\overbrace {{\frac {1}
          {T}}\ S_{\frac {1}{T}}(f)\cdot e^  {N}}\sum _{k}S[k]\cdot e^{i2\pi
          {i2\pi ft}\,df} _{\text{inverse    {\frac {kn}{N}}}} ^{\text{inverse
          Fourier transform}}\,}  [          DFT}}\\&={\tfrac {1}{P}}\sum _
          {\displaystyle \sum _{n=-\infty }^ {k}S_{\frac {1}{T}}\left({\frac
          {\infty }s(nT)\cdot \delta (t-     {k}{P}}\right)\cdot e^{i2\pi
          nT)=\underbrace {\int _{-\infty }^ {\frac {kn}{N}}}\end{aligned}}}]
          {\infty }{\frac {1}{T}}\ S_{\frac
          {1}{T}}(f)\cdot e^{i2\pi ft}\,df}
          _{\text{inverse Fourier
          transform}}\,}]
**** Symmetry properties[edit] ****
When the real and imaginary parts of a complex function are decomposed into
their even_and_odd_parts, there are four components, denoted below by the
subscripts RE, RO, IE, and IO. And there is a one-to-one mapping between the
four components of a complex time function and the four components of its
complex frequency transform:[4]
              Time domain    s   =    s     RE       +    s     RO       +   i
      s     IE       +      i &#xA0;  s     IO      &#x23DF;          &#x21D5;
      F        &#x21D5;     F      &#xA0; &#xA0;   &#x21D5;     F      &#xA0;
      &#xA0;   &#x21D5;     F      &#xA0; &#xA0;   &#x21D5;     F
      Frequency domain    S   =    S  RE     +       i &#xA0;  S  IO
      &#x23DE;     +   i  S  IE     +    S  RO         {\displaystyle {\begin
      {array}{rccccccccc}{\text{Time domain}}&s&=&s_{_{\text{RE}}}&+&s_{_{\text
      {RO}}}&+&is_{_{\text{IE}}}&+&\underbrace {i\ s_{_{\text{IO}}}} \\&{\Bigg
      \Updownarrow }{\mathcal {F}}&&{\Bigg \Updownarrow }{\mathcal {F}}&&\ \
      {\Bigg \Updownarrow }{\mathcal {F}}&&\ \ {\Bigg \Updownarrow }{\mathcal
      {F}}&&\ \ {\Bigg \Updownarrow }{\mathcal {F}}\\{\text{Frequency
      domain}}&S&=&S_{\text{RE}}&+&\overbrace {\,i\ S_{\text{IO}}\,} &+&iS_
      {\text{IE}}&+&S_{\text{RO}}\end{array}}}  [{\displaystyle {\begin{array}
      {rccccccccc}{\text{Time domain}}&s&=&s_{_{\text{RE}}}&+&s_{_{\text
      {RO}}}&+&is_{_{\text{IE}}}&+&\underbrace {i\ s_{_{\text{IO}}}} \\&{\Bigg
      \Updownarrow }{\mathcal {F}}&&{\Bigg \Updownarrow }{\mathcal {F}}&&\ \
      {\Bigg \Updownarrow }{\mathcal {F}}&&\ \ {\Bigg \Updownarrow }{\mathcal
      {F}}&&\ \ {\Bigg \Updownarrow }{\mathcal {F}}\\{\text{Frequency
      domain}}&S&=&S_{\text{RE}}&+&\overbrace {\,i\ S_{\text{IO}}\,} &+&iS_
      {\text{IE}}&+&S_{\text{RO}}\end{array}}}]
From this, various relationships are apparent, for example:
    * The transform of a real-valued function (sRE+ sRO) is the even_symmetric
      function SRE+ i SIO. Conversely, an even-symmetric transform implies a
      real-valued time-domain.
    * The transform of an imaginary-valued function (i sIE+ i sIO) is the odd
      symmetric function SRO+ i SIE, and the converse is true.
    * The transform of an even-symmetric function (sRE+ i sIO) is the real-
      valued function SRE+ SRO, and the converse is true.
    * The transform of an odd-symmetric function (sRO+ i sIE) is the imaginary-
      valued function i SIE+ i SIO, and the converse is true.
**** Fourier transforms on arbitrary locally compact abelian topological groups
[edit] ****
The Fourier variants can also be generalized to Fourier transforms on arbitrary
locally_compact Abelian topological_groups, which are studied in harmonic
analysis; there, the Fourier transform takes functions on a group to functions
on the dual group. This treatment also allows a general formulation of the
convolution_theorem, which relates Fourier transforms and convolutions. See
also the Pontryagin_duality for the generalized underpinnings of the Fourier
transform.
More specific, Fourier analysis can be done on cosets,[5] even discrete cosets.
**** Timeâfrequency transforms[edit] ****
Further information: Timeâfrequency_analysis
In signal_processing terms, a function (of time) is a representation of a
signal with perfect time resolution, but no frequency information, while the
Fourier transform has perfect frequency resolution, but no time information.
As alternatives to the Fourier transform, in timeâfrequency_analysis, one
uses timeâfrequency transforms to represent signals in a form that has some
time information and some frequency information â by the uncertainty
principle, there is a trade-off between these. These can be generalizations of
the Fourier transform, such as the short-time_Fourier_transform, the Gabor
transform or fractional_Fourier_transform (FRFT), or can use different
functions to represent signals, as in wavelet_transforms and chirplet
transforms, with the wavelet analog of the (continuous) Fourier transform being
the continuous_wavelet_transform.
***** History[edit] *****
See also: Fourier_series_Â§ Historical_development
A primitive form of harmonic series dates back to ancient Babylonian
mathematics, where they were used to compute ephemerides (tables of
astronomical positions).[6][7][8][9]
The classical Greek concepts of deferent_and_epicycle in the Ptolemaic_system
of astronomy were related to Fourier series (see Deferent_and_epicycle:
Mathematical_formalism).
In modern times, variants of the discrete Fourier transform were used by Alexis
Clairaut in 1754 to compute an orbit,[10] which has been described as the first
formula for the DFT,[11] and in 1759 by Joseph_Louis_Lagrange, in computing the
coefficients of a trigonometric series for a vibrating string.[12] Technically,
Clairaut's work was a cosine-only series (a form of discrete_cosine_transform),
while Lagrange's work was a sine-only series (a form of discrete_sine
transform); a true cosine+sine DFT was used by Gauss in 1805 for trigonometric
interpolation of asteroid orbits.[13] Euler and Lagrange both discretized the
vibrating string problem, using what would today be called samples.[12]
An early modern development toward Fourier analysis was the 1770 paper
RÃ©flexions_sur_la_rÃ©solution_algÃ©brique_des_Ã©quations by Lagrange, which in
the method of Lagrange_resolvents used a complex Fourier decomposition to study
the solution of a cubic:[14] Lagrange transformed the roots x1, x2, x3 into the
resolvents:
              r  1      =  x  1   +  x  2   +  x  3        r  2      =  x  1
      + &#x03B6;  x  2   +  &#x03B6;  2    x  3        r  3      =  x  1   +
      &#x03B6;  2    x  2   + &#x03B6;  x  3         {\displaystyle {\begin
      {aligned}r_{1}&=x_{1}+x_{2}+x_{3}\\r_{2}&=x_{1}+\zeta x_{2}+\zeta ^{2}x_
      {3}\\r_{3}&=x_{1}+\zeta ^{2}x_{2}+\zeta x_{3}\end{aligned}}}  [{\begin
      {aligned}r_{1}&=x_{1}+x_{2}+x_{3}\\r_{2}&=x_{1}+\zeta x_{2}+\zeta ^{2}x_
      {3}\\r_{3}&=x_{1}+\zeta ^{2}x_{2}+\zeta x_{3}\end{aligned}}]
where Î¶ is a cubic root_of_unity, which is the DFT of order 3.
A number of authors, notably Jean_le_Rond_d'Alembert, and Carl_Friedrich_Gauss
used trigonometric_series to study the heat_equation,[15] but the breakthrough
development was the 1807 paper MÃ©moire_sur_la_propagation_de_la_chaleur_dans
les_corps_solides by Joseph_Fourier, whose crucial insight was to model all
functions by trigonometric series, introducing the Fourier series.
Historians are divided as to how much to credit Lagrange and others for the
development of Fourier theory: Daniel_Bernoulli and Leonhard_Euler had
introduced trigonometric representations of functions,[11] and Lagrange had
given the Fourier series solution to the wave equation,[11] so Fourier's
contribution was mainly the bold claim that an arbitrary function could be
represented by a Fourier series.[11]
The subsequent development of the field is known as harmonic_analysis, and is
also an early instance of representation_theory.
The first fast Fourier transform (FFT) algorithm for the DFT was discovered
around 1805 by Carl_Friedrich_Gauss when interpolating measurements of the
orbit of the asteroids Juno and Pallas, although that particular FFT algorithm
is more often attributed to its modern rediscoverers Cooley_and_Tukey.[13][16]
***** Interpretation in terms of time and frequency[edit] *****
In signal_processing, the Fourier transform often takes a time_series or a
function of continuous_time, and maps it into a frequency_spectrum. That is, it
takes a function from the time domain into the frequency domain; it is a
decomposition of a function into sinusoids of different frequencies; in the
case of a Fourier_series or discrete_Fourier_transform, the sinusoids are
harmonics of the fundamental frequency of the function being analyzed.
When the function f is a function of time and represents a physical signal, the
transform has a standard interpretation as the frequency spectrum of the
signal. The magnitude of the resulting complex-valued function F at frequency
Ï represents the amplitude of a frequency component whose initial_phase is
given by the phase of F.
Fourier transforms are not limited to functions of time, and temporal
frequencies. They can equally be applied to analyze spatial frequencies, and
indeed for nearly any function domain. This justifies their use in such diverse
branches as image_processing, heat_conduction, and automatic_control.
***** See also[edit] *****
    * Generalized_Fourier_series
    * FourierâBessel_series
    * Fourier-related_transforms
    * Laplace_transform (LT)
    * Two-sided_Laplace_transform
    * Mellin_transform
    * Non-uniform_discrete_Fourier_transform (NDFT)
    * Quantum_Fourier_transform (QFT)
    * Number-theoretic_transform
    * Least-squares_spectral_analysis
    * Basis_vectors
    * Bispectrum
    * Characteristic_function_(probability_theory)
    * Orthogonal_functions
    * Schwartz_space
    * Spectral_density
    * Spectral_density_estimation
    * Spectral_music
    * Wavelet
***** Notes[edit] *****
   1. ^
                &#x222B;  P    (   &#x2211;  m = &#x2212; &#x221E;   &#x221E;
            s ( t &#x2212; m P )  )  &#x22C5;  e  &#x2212; i 2 &#x03C0;   k P
            t    d t =      &#x222B;  &#x2212; &#x221E;   &#x221E;   s ( t )
            &#x22C5;  e  &#x2212; i 2 &#x03C0;   k P   t    d t  &#x23DF;
            &#x225C;  S  (   k P   )      {\displaystyle \int _{P}\left(\sum _
            {m=-\infty }^{\infty }s(t-mP)\right)\cdot e^{-i2\pi {\frac {k}
            {P}}t}\,dt=\underbrace {\int _{-\infty }^{\infty }s(t)\cdot e^{-
            i2\pi {\frac {k}{P}}t}\,dt} _{\triangleq \,S\left({\frac {k}
            {P}}\right)}}  [{\displaystyle \int _{P}\left(\sum _{m=-\infty }^
            {\infty }s(t-mP)\right)\cdot e^{-i2\pi {\frac {k}
            {P}}t}\,dt=\underbrace {\int _{-\infty }^{\infty }s(t)\cdot e^{-
            i2\pi {\frac {k}{P}}t}\,dt} _{\triangleq \,S\left({\frac {k}
            {P}}\right)}}]
   2. ^ We may also note that:
                    &#x2211;  n = &#x2212; &#x221E;   + &#x221E;   T &#x22C5; s
            ( n T ) &#x03B4; ( t &#x2212; n T )    =  &#x2211;  n = &#x2212;
            &#x221E;   + &#x221E;   T &#x22C5; s ( t ) &#x03B4; ( t &#x2212; n
            T )       = s ( t ) &#x22C5; T  &#x2211;  n = &#x2212; &#x221E;   +
            &#x221E;   &#x03B4; ( t &#x2212; n T ) .       {\displaystyle
            {\begin{aligned}\sum _{n=-\infty }^{+\infty }T\cdot s(nT)\delta (t-
            nT)&=\sum _{n=-\infty }^{+\infty }T\cdot s(t)\delta (t-nT)\\&=s
            (t)\cdot T\sum _{n=-\infty }^{+\infty }\delta (t-nT).\end
            {aligned}}}  [{\displaystyle {\begin{aligned}\sum _{n=-\infty }^
            {+\infty }T\cdot s(nT)\delta (t-nT)&=\sum _{n=-\infty }^{+\infty
            }T\cdot s(t)\delta (t-nT)\\&=s(t)\cdot T\sum _{n=-\infty }^{+\infty
            }\delta (t-nT).\end{aligned}}}]
      Consequently, a common practice is to model "sampling" as a
      multiplication by the Dirac_comb function, which of course is only
      "possible" in a purely mathematical sense.
   3. ^ Note that this definition differs from the DTFT section by a factor of
      T.
   4. ^
                &#x2211;  n = 0   N &#x2212; 1    (   &#x2211;  m = &#x2212;
            &#x221E;   &#x221E;   s ( [ n &#x2212; m N ] T )  )  &#x22C5;  e
            &#x2212; i 2 &#x03C0;   k N   n   =      &#x2211;  n = &#x2212;
            &#x221E;   &#x221E;   s ( n T ) &#x22C5;  e  &#x2212; i 2 &#x03C0;
            k N   n    &#x23DF;    &#x225C;    1 T    S   1 T     (   k  N T
            )      {\displaystyle \sum _{n=0}^{N-1}\left(\sum _{m=-\infty }^
            {\infty }s([n-mN]T)\right)\cdot e^{-i2\pi {\frac {k}
            {N}}n}=\underbrace {\sum _{n=-\infty }^{\infty }s(nT)\cdot e^{-
            i2\pi {\frac {k}{N}}n}} _{\triangleq \,{\frac {1}{T}}S_{\frac {1}
            {T}}\left({\frac {k}{NT}}\right)}}  [{\displaystyle \sum _{n=0}^{N-
            1}\left(\sum _{m=-\infty }^{\infty }s([n-mN]T)\right)\cdot e^{-
            i2\pi {\frac {k}{N}}n}=\underbrace {\sum _{n=-\infty }^{\infty }s
            (nT)\cdot e^{-i2\pi {\frac {k}{N}}n}} _{\triangleq \,{\frac {1}
            {T}}S_{\frac {1}{T}}\left({\frac {k}{NT}}\right)}}]
***** References[edit] *****
   1. ^"Fourier". Dictionary.com Unabridged. Random_House.
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
   3. ^Saferstein, Richard (2013). Criminalistics: An Introduction to Forensic
      Science.
   4. ^Rabiner, Lawrence R.; Gold, Bernard (1975). Theory and Application of
      Digital Signal Processing. Englewood Cliffs, NJ.
   5. ^Proakis, John G.; Manolakis, Dimitri G. (1996), Digital Signal
      Processing: Principles, Algorithms and Applications (3 ed.), New Jersey:
      Prentice-Hall International, p. 291, ISBN 9780133942897, sAcfAQAAIAAJ
   6. ^ Forrest, Brian. (1998). Fourier Analysis on Coset Spaces. Rocky
      Mountain Journal of Mathematics. 28. 10.1216/rmjm/1181071828.
   7. ^Prestini, Elena (2004). The_Evolution_of_Applied_Harmonic_Analysis:
      Models_of_the_Real_World. BirkhÃ¤user. p. 62. ISBN 978-0-8176-4125-2.
   8. ^Rota,_Gian-Carlo; Palombi, Fabrizio (1997). Indiscrete_Thoughts.
      BirkhÃ¤user. p. 11. ISBN 978-0-8176-3866-5.
   9. ^Neugebauer,_Otto (1969) [1957]. The_Exact_Sciences_in_Antiquity (2nd
      ed.). Dover_Publications. ISBN 978-0-486-22332-2.
  10. ^Brack-Bernsen,_Lis; Brack, Matthias (2004). "Analyzing shell structure
      from Babylonian and modern times". International Journal of Modern
      Physics E. 13 (1): 247. arXiv:physics/0310126. Bibcode:
      2004IJMPE..13..247B. doi:10.1142/S0218301304002028.
  11. ^Terras,_Audrey (1999). Fourier_Analysis_on_Finite_Groups_and
      Applications. Cambridge_University_Press. p. 30. ISBN 978-0-521-45718-7.
  12. ^ a b c dBriggs, William L.; Henson, Van Emden (1995). The_DFT:_An
      Owner's_Manual_for_the_Discrete_Fourier_Transform. SIAM. p. 4. ISBN 978-
      0-89871-342-8.
  13. ^ a bBriggs, William L.; Henson, Van Emden (1995). The_DFT:_An_Owner's
      Manual_for_the_Discrete_Fourier_Transform. SIAM. p. 2. ISBN 978-0-89871-
      342-8.
  14. ^ a bHeideman, M. T.; Johnson, D. H.; Burrus, C. S. (1984). "Gauss and
      the history of the fast Fourier transform". IEEE ASSP Magazine. 1 (4):
      14â21. doi:10.1109/MASSP.1984.1162257.
  15. ^ Knapp, Anthony W. (2006). Basic_Algebra. Springer. p. 501. ISBN 978-0-
      8176-3248-9.
  16. ^Narasimhan, T. N. (February 1999). "Fourier's heat conduction equation:
      History, influence, and connections". Reviews of Geophysics. 37 (1):
      151â172. Bibcode:1999RvGeo..37..151N. CiteSeerX 10.1.1.455.4798. doi:
      10.1029/1998RG900006. ISSN 1944-9208. OCLC 5156426043.
  17. ^Terras,_Audrey (1999). Fourier_Analysis_on_Finite_Groups_and
      Applications. Cambridge University Press. p. 31. ISBN 978-0-521-45718-7.
***** Further reading[edit] *****
    * Conte, S. D.; de Boor, Carl (1980). Elementary Numerical Analysis (Third
      ed.). New York: McGraw Hill, Inc. ISBN 978-0-07-066228-5.
Evans, L. (1998). Partial Differential Equations. American Mathematical
Society. ISBN 978-3-540-76124-2.
Howell, Kenneth B. (2001). Principles of Fourier Analysis. CRC Press. ISBN 978-
0-8493-8275-8.
Kamen, E. W.; Heck, B. S. (2 March 2000). Fundamentals of Signals and Systems
Using the Web and Matlab (2 ed.). Prentiss-Hall. ISBN 978-0-13-017293-8.
Knuth, Donald E. (1997). The_Art_of_Computer_Programming_Volume_2:
Seminumerical_Algorithms (3rd ed.). Addison-Wesley Professional. Section
4.3.3.C: Discrete Fourier transforms, pg.305. ISBN 978-0-201-89684-8.
MÃ¼ller, Meinard (2015). The_Fourier_Transform_in_a_Nutshell (PDF). Springer.
In Fundamentals_of_Music_Processing, Section 2.1, p. 40â56. doi:10.1007/978-
3-319-21945-5. ISBN 978-3-319-21944-8.
Polyanin, A. D.; Manzhirov, A. V. (1998). Handbook of Integral Equations. Boca
Raton: CRC Press. ISBN 978-0-8493-2876-3.
Rudin, Walter (1990). Fourier Analysis on Groups. Wiley-Interscience. ISBN 978-
0-471-52364-2.
Smith, Steven W. (1999). The_Scientist_and_Engineer's_Guide_to_Digital_Signal
Processing (Second ed.). San Diego: California Technical Publishing. ISBN 978-
0-9660176-3-2.
Stein, E. M.; Weiss, G. (1971). Introduction to Fourier Analysis on Euclidean
Spaces. Princeton University Press. ISBN 978-0-691-08078-9.
***** External links[edit] *****
    * Tables_of_Integral_Transforms at EqWorld: The World of Mathematical
      Equations.
    * An_Intuitive_Explanation_of_Fourier_Theory by Steven Lehar.
    * Lectures_on_Image_Processing:_A_collection_of_18_lectures_in_pdf_format
      from_Vanderbilt_University._Lecture_6_is_on_the_1-_and_2-D_Fourier
      Transform._Lectures_7â15_make_use_of_it., by Alan Peters
    * Moriarty, Philip; Bowley, Roger (2009). "â_Summation_(and_Fourier
      Analysis)". Sixty Symbols. Brady_Haran for the University_of_Nottingham.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Fourier_analysis&oldid=905954314"
Categories:
    * Fourier_analysis
    * Integral_transforms
    * Digital_signal_processing
    * Mathematical_physics
    * Mathematics_of_computing
    * Time_series
    * Joseph_Fourier
Hidden categories:
    * Use_dmy_dates_from_April_2012
    * Use_American_English_from_March_2019
    * All_Wikipedia_articles_written_in_American_English
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
**** In other projects ****
    * Wikimedia_Commons
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * à¦¬à¦¾à¦à¦²à¦¾
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * Galego
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * LietuviÅ³
    * Magyar
    * Bahasa_Melayu
    * Nederlands
    * Norsk
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 12 July 2019, at 16:04 (UTC).
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
