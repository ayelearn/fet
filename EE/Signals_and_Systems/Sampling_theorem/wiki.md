The following text has been accessed from https://en.wikipedia.org/wiki/Nyquist%E2%80%93Shannon_sampling_theorem at Thu Aug 8 22:55:22 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** NyquistâShannon sampling theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Sufficiency theorem for reconstructing signals from samples
Example of magnitude of the Fourier transform of a bandlimited function
In the field of digital_signal_processing, the sampling theorem is a
fundamental bridge between continuous-time_signals and discrete-time_signals.
It establishes a sufficient condition for a sample_rate that permits a discrete
sequence of samples to capture all the information from a continuous-time
signal of finite bandwidth.
Strictly speaking, the theorem only applies to a class of mathematical
functions having a Fourier_transform that is zero outside of a finite region of
frequencies. Intuitively we expect that when one reduces a continuous function
to a discrete sequence and interpolates back to a continuous function, the
fidelity of the result depends on the density (or sample_rate) of the original
samples. The sampling theorem introduces the concept of a sample rate that is
sufficient for perfect fidelity for the class of functions that are bandlimited
to a given bandwidth, such that no actual information is lost in the sampling
process. It expresses the sufficient sample rate in terms of the bandwidth for
the class of functions. The theorem also leads to a formula for perfectly
reconstructing the original continuous-time function from the samples.
Perfect reconstruction may still be possible when the sample-rate criterion is
not satisfied, provided other constraints on the signal are known. (See
Â§ Sampling_of_non-baseband_signals below and compressed_sensing.) In some
cases (when the sample-rate criterion is not satisfied), utilizing additional
constraints allows for approximate reconstructions. The fidelity of these
reconstructions can be verified and quantified utilizing Bochner's_theorem.[1]
The name NyquistâShannon sampling theorem honors Harry_Nyquist and Claude
Shannon. The theorem was also discovered independently by E._T._Whittaker, by
Vladimir_Kotelnikov, and by others. It is thus also known by the names
NyquistâShannonâKotelnikov, WhittakerâShannonâKotelnikov,
WhittakerâNyquistâKotelnikovâShannon, and cardinal theorem of
interpolation.
⁰
***** Contents *****
    * 1_Introduction
    * 2_Aliasing
    * 3_Derivation_as_a_special_case_of_Poisson_summation
    * 4_Shannon's_original_proof
          o 4.1_Notes
    * 5_Application_to_multivariable_signals_and_images
    * 6_Critical_frequency
    * 7_Sampling_of_non-baseband_signals
    * 8_Nonuniform_sampling
    * 9_Sampling_below_the_Nyquist_rate_under_additional_restrictions
    * 10_Historical_background
          o 10.1_Other_discoverers
          o 10.2_Why_Nyquist?
    * 11_See_also
    * 12_Notes
    * 13_References
    * 14_Further_reading
    * 15_External_links
***** Introduction[edit] *****
Sampling is a process of converting a signal (for example, a function of
continuous time and/or space) into a numeric sequence (a function of discrete
time and/or space). Shannon's version of the theorem states:[2]
     If a function     x ( t )   {\displaystyle x(t)}  [x(t)] contains no
     frequencies higher than B hertz, it is completely determined by
     giving its ordinates at a series of points spaced     1  /  ( 2 B )
     {\displaystyle 1/(2B)}  [{\displaystyle 1/(2B)}] seconds apart.
A sufficient sample-rate is therefore anything larger than     2 B
{\displaystyle 2B}  [2B] samples per second. Equivalently, for a given sample
rate      f  s     {\displaystyle f_{s}}  [f_{s}], perfect reconstruction is
guaranteed possible for a bandlimit     B <  f  s    /  2   {\displaystyle B<f_
{s}/2}  [{\displaystyle B<f_{s}/2}].
When the bandlimit is too high (or there is no bandlimit), the reconstruction
exhibits imperfections known as aliasing. Modern statements of the theorem are
sometimes careful to explicitly state that     x ( t )   {\displaystyle x(t)}
[x(t)] must contain no sinusoidal component at exactly frequency B, or that B
must be strictly less than Â½ the sample rate. The threshold     2 B
{\displaystyle 2B}  [2B] is called the Nyquist_rate and is an attribute of the
continuous-time input     x ( t )   {\displaystyle x(t)}  [x(t)] to be sampled.
The sample rate must exceed the Nyquist rate for the samples to suffice to
represent x(t). The threshold fs/2 is called the Nyquist_frequency and is an
attribute of the sampling_equipment. All meaningful frequency components of the
properly sampled x(t) exist below the Nyquist frequency. The condition
described by these inequalities is called the Nyquist criterion, or sometimes
the Raabe condition. The theorem is also applicable to functions of other
domains, such as space, in the case of a digitized image. The only change, in
the case of other domains, is the units of measure applied to t, fs, and B.
The normalized sinc_function: sin(Ïx) / (Ïx) ... showing the central peak at
x = 0, and zero-crossings at the other integer values of x.
The symbol T = 1/fs is customarily used to represent the interval between
samples and is called the sample period or sampling interval. And the samples
of function x(t) are commonly denoted by x[n] = x(nT) (alternatively "xn" in
older signal processing literature), for all integer values of n. A
mathematically ideal way to interpolate the sequence involves the use of sinc
functions. Each sample in the sequence is replaced by a sinc function, centered
on the time axis at the original location of the sample, nT, with the amplitude
of the sinc function scaled to the sample value, x[n]. Subsequently, the sinc
functions are summed into a continuous function. A mathematically equivalent
method is to convolve one sinc function with a series of Dirac_delta pulses,
weighted by the sample values. Neither method is numerically practical.
Instead, some type of approximation of the sinc functions, finite in length, is
used. The imperfections attributable to the approximation are known as
interpolation error.
Practical digital-to-analog_converters produce neither scaled and delayed sinc
functions, nor ideal Dirac_pulses. Instead they produce a piecewise-constant
sequence of scaled and delayed rectangular_pulses (the zero-order_hold),
usually followed by an "anti-aliasing filter" to clean up spurious high-
frequency content.
***** Aliasing[edit] *****
Main article: Aliasing
The samples of two sine waves can be identical when at least one of them is at
a frequency above half the sample rate.
When     x ( t )   {\displaystyle x(t)}  [x(t)] is a function with a Fourier
transform     X ( f )   {\displaystyle X(f)}  [X(f)]:
         X ( f ) &#xA0; &#x225C; &#xA0;  &#x222B;  &#x2212; &#x221E;   &#x221E;
      x ( t ) &#xA0;  e  &#x2212; i 2 &#x03C0; f t   &#xA0;   d   t ,
      {\displaystyle X(f)\ \triangleq \ \int _{-\infty }^{\infty }x(t)\ e^{-
      i2\pi ft}\ {\rm {d}}t,}  [{\displaystyle X(f)\ \triangleq \ \int _{-
      \infty }^{\infty }x(t)\ e^{-i2\pi ft}\ {\rm {d}}t,}]
the Poisson_summation_formula indicates that the samples,     x ( n T )
{\displaystyle x(nT)}  [{\displaystyle x(nT)}], of     x ( t )   {\displaystyle
x(t)}  [x(t)] are sufficient to create a periodic_summation of     X ( f )
{\displaystyle X(f)}  [X(f)]. The result is:
          X  s   ( f ) &#xA0; &#x225C;  &#x2211;  k = &#x2212;
      &#x221E;   &#x221E;   X  (  f &#x2212; k  f  s    )  =
      &#x2211;  n = &#x2212; &#x221E;   &#x221E;   T &#x22C5; x
      ( n T ) &#xA0;  e  &#x2212; i 2 &#x03C0; n T f   ,
      {\displaystyle X_{s}(f)\ \triangleq \sum _{k=-\infty }^       (Eq.1)
      {\infty }X\left(f-kf_{s}\right)=\sum _{n=-\infty }^{\infty    
      }T\cdot x(nT)\ e^{-i2\pi nTf},}  [{\displaystyle X_{s}(f)\
      \triangleq \sum _{k=-\infty }^{\infty }X\left(f-kf_
      {s}\right)=\sum _{n=-\infty }^{\infty }T\cdot x(nT)\ e^{-
      i2\pi nTf},}]
X(f) (top blue) and XA(f) (bottom blue) are continuous Fourier transforms of
two different functions,     x ( t )   {\displaystyle x(t)}  [x(t)] and      x
A   ( t )   {\displaystyle x_{A}(t)}  [{\displaystyle x_{A}(t)}] (not shown).
When the functions are sampled at rate      f  s     {\displaystyle f_{s}}  [f_
{s}], the images (green) are added to the original transforms (blue) when one
examines the discrete-time Fourier transforms (DTFT) of the sequences. In this
hypothetical example, the DTFTs are identical, which means the sampled
sequences are identical, even though the original continuous pre-sampled
functions are not. If these were audio signals,     x ( t )   {\displaystyle x
(t)}  [x(t)] and      x  A   ( t )   {\displaystyle x_{A}(t)}  [{\displaystyle
x_{A}(t)}] might not sound the same. But their samples (taken at rate fs) are
identical and would lead to identical reproduced sounds; thus xA(t) is an alias
of x(t) at this sample rate.
which is a periodic function and its equivalent representation as a Fourier
series, whose coefficients are     T &#x22C5; x ( n T ) .   {\displaystyle
T\cdot x(nT).}  [{\displaystyle T\cdot x(nT).}] This function is also known as
the discrete-time_Fourier_transform (DTFT) of the sample sequence.
As depicted, copies of     X ( f )   {\displaystyle X(f)}  [X(f)] are shifted
by multiples of      f  s     {\displaystyle f_{s}}  [f_{s}] and combined by
addition. For a band-limited function      ( X ( f ) = 0 ,  &#xA0;for all&#xA0;
|  f  |  &#x2265; B )   {\displaystyle (X(f)=0,{\text{ for all }}|f|\geq B)}  [
{\displaystyle (X(f)=0,{\text{ for all }}|f|\geq B)}]  and sufficiently large
f  s   ,   {\displaystyle f_{s},}  [{\displaystyle f_{s},}] it is possible for
the copies to remain distinct from each other. But if the Nyquist criterion is
not satisfied, adjacent copies overlap, and it is not possible in general to
discern an unambiguous     X ( f ) .   {\displaystyle X(f).}  [{\displaystyle X
(f).}] Any frequency component above      f  s    /  2   {\displaystyle f_{s}/
2}  [f_{s}/2] is indistinguishable from a lower-frequency component, called an
alias, associated with one of the copies. In such cases, the customary
interpolation techniques produce the alias, rather than the original component.
When the sample-rate is pre-determined by other considerations (such as an
industry standard),     x ( t )   {\displaystyle x(t)}  [x(t)] is usually
filtered to reduce its high frequencies to acceptable levels before it is
sampled. The type of filter required is a lowpass_filter, and in this
application it is called an anti-aliasing_filter.
Spectrum, Xs(f), of a properly sampled bandlimited signal (blue) and the
adjacent DTFT images (green) that do not overlap. A brick-wall low-pass filter,
H(f), removes the images, leaves the original spectrum, X(f), and recovers the
original signal from its samples.
***** Derivation as a special case of Poisson summation[edit] *****
When there is no overlap of the copies (also known as "images") of     X ( f )
{\displaystyle X(f)}  [X(f)], the     k = 0   {\displaystyle k=0}  [k=0] term
of Eq.1 can be recovered by the product:
         X ( f ) = H ( f ) &#x22C5;  X  s   ( f ) ,   {\displaystyle X(f)=H
      (f)\cdot X_{s}(f),}  [{\displaystyle X(f)=H(f)\cdot X_{s}(f),}]     
      where:
         H ( f ) &#xA0; &#x225C; &#xA0;   {    1    |  f  |  < B     0    |  f
      |  >  f  s   &#x2212; B .         {\displaystyle H(f)\ \triangleq \
      {\begin{cases}1&|f|<B\\0&|f|>f_{s}-B.\end{cases}}}  [{\displaystyle H(f)\
      \triangleq \ {\begin{cases}1&|f|<B\\0&|f|>f_{s}-B.\end{cases}}}]
The sampling theorem is proved since     X ( f )   {\displaystyle X(f)}  [X(f)]
uniquely determines     x ( t ) .   {\displaystyle x(t).}  [{\displaystyle x
(t).}]
All that remains is to derive the formula for reconstruction.     H ( f )
{\displaystyle H(f)}  [H(f)] need not be precisely defined in the region
[ B , &#xA0;  f  s   &#x2212; B ]   {\displaystyle [B,\ f_{s}-B]}  [
{\displaystyle [B,\ f_{s}-B]}] because      X  s   ( f )   {\displaystyle X_{s}
(f)}  [{\displaystyle X_{s}(f)}] is zero in that region. However, the worst
case is when     B =  f  s    /  2 ,   {\displaystyle B=f_{s}/2,}  [
{\displaystyle B=f_{s}/2,}] the Nyquist frequency. A function that is
sufficient for that and all less severe cases is:
         H ( f ) =  r e c t   (   f  f  s     )  =   {    1    |  f  |  <    f
      s   2       0    |  f  |  >    f  s   2   ,         {\displaystyle H
      (f)=\mathrm {rect} \left({\frac {f}{f_{s}}}\right)={\begin{cases}1&|f|<
      {\frac {f_{s}}{2}}\\0&|f|>{\frac {f_{s}}{2}},\end{cases}}}  [H(f)=\mathrm
      {rect} \left({\frac {f}{f_{s}}}\right)={\begin{cases}1&|f|<{\frac {f_{s}}
      {2}}\\0&|f|>{\frac {f_{s}}{2}},\end{cases}}]
where rect(â¢) is the rectangular_function.  Therefore:
         X ( f ) =  r e c t   (   f  f  s     )  &#x22C5;  X  s   ( f )
      {\displaystyle X(f)=\mathrm {rect} \left({\frac {f}{f_{s}}}\right)\cdot
      X_{s}(f)}  [{\displaystyle X(f)=\mathrm {rect} \left({\frac {f}{f_
      {s}}}\right)\cdot X_{s}(f)}]
                     =  r e c t  ( T f ) &#x22C5;  &#x2211;  n = &#x2212;
                  &#x221E;   &#x221E;   T &#x22C5; x ( n T ) &#xA0;  e
                  &#x2212; i 2 &#x03C0; n T f     {\displaystyle =\mathrm
                  {rect} (Tf)\cdot \sum _{n=-\infty }^{\infty }T\cdot x(nT)\ e^
                  {-i2\pi nTf}}  [=\mathrm {rect} (Tf)\cdot \sum _{n=-\infty }^
                  {\infty }T\cdot x(nT)\ e^{-i2\pi nTf}]      (from  Eq.1,
                  above).
                     =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;   x ( n T )
                  &#x22C5;     T &#x22C5;  r e c t  ( T f ) &#x22C5;  e
                  &#x2212; i 2 &#x03C0; n T f    &#x23DF;      F    {   s i n c
                  (    t &#x2212; n T  T   )   }    .   {\displaystyle =\sum _
                  {n=-\infty }^{\infty }x(nT)\cdot \underbrace {T\cdot \mathrm
                  {rect} (Tf)\cdot e^{-i2\pi nTf}} _{{\mathcal {F}}\left\
                  {\mathrm {sinc} \left({\frac {t-nT}{T}}\right)\right\}}.}
                  [=\sum _{n=-\infty }^{\infty }x(nT)\cdot \underbrace {T\cdot
                  \mathrm {rect} (Tf)\cdot e^{-i2\pi nTf}} _{{\mathcal
                  {F}}\left\{\mathrm {sinc} \left({\frac {t-nT}
                  {T}}\right)\right\}}.]     [note_1]
The inverse transform of both sides produces the WhittakerâShannon
interpolation_formula:
         x ( t ) =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;   x ( n T )
      &#x22C5;  s i n c   (    t &#x2212; n T  T   )  ,   {\displaystyle x
      (t)=\sum _{n=-\infty }^{\infty }x(nT)\cdot \mathrm {sinc} \left({\frac
      {t-nT}{T}}\right),}  [x(t)=\sum _{n=-\infty }^{\infty }x(nT)\cdot \mathrm
      {sinc} \left({\frac {t-nT}{T}}\right),]
which shows how the samples,     x ( n T ) ,   {\displaystyle x(nT),}  [
{\displaystyle x(nT),}] can be combined to reconstruct     x ( t ) .
{\displaystyle x(t).}  [{\displaystyle x(t).}]
    * Larger-than-necessary values of fs (smaller values of T), called
      oversampling, have no effect on the outcome of the reconstruction and
      have the benefit of leaving room for a transition band in which H(f) is
      free to take intermediate values. Undersampling, which causes aliasing,
      is not in general a reversible operation.
    * Theoretically, the interpolation formula can be implemented as a low_pass
      filter, whose impulse response is sinc(t/T) and whose input is
      &#x2211;  n = &#x2212; &#x221E;   &#x221E;   x ( n T ) &#x22C5; &#x03B4;
      ( t &#x2212; n T ) ,    {\displaystyle \textstyle \sum _{n=-\infty }^
      {\infty }x(nT)\cdot \delta (t-nT),}  [\textstyle \sum _{n=-\infty }^
      {\infty }x(nT)\cdot \delta (t-nT),] which is a Dirac_comb function
      modulated by the signal samples. Practical digital-to-analog_converters
      (DAC) implement an approximation like the zero-order_hold. In that case,
      oversampling can reduce the approximation error.
***** Shannon's original proof[edit] *****
Poisson shows that the Fourier series in Eq.1 produces the periodic summation
of     X ( f )   {\displaystyle X(f)}  [X(f)], regardless of      f  s
{\displaystyle f_{s}}  [f_{s}] and     B   {\displaystyle B}  [B]. Shannon,
however, only derives the series coefficients for the case      f  s   = 2 B
{\displaystyle f_{s}=2B}  [{\displaystyle f_{s}=2B}]. Virtually quoting
Shannon's original paper:
      Let     X ( &#x03C9; )   {\displaystyle X(\omega )}  [X(\omega )] be the
      spectrum of     x ( t ) .   {\displaystyle x(t).}  [{\displaystyle x
      (t).}]  Then
               x ( t ) =   1  2 &#x03C0;     &#x222B;  &#x2212; &#x221E;
            &#x221E;   X ( &#x03C9; )  e  i &#x03C9; t      d   &#x03C9; =   1
            2 &#x03C0;     &#x222B;  &#x2212; 2 &#x03C0; B   2 &#x03C0; B   X
            ( &#x03C9; )  e  i &#x03C9; t      d   &#x03C9; ,   {\displaystyle
            x(t)={1 \over 2\pi }\int _{-\infty }^{\infty }X(\omega )e^{i\omega
            t}\;{\rm {d}}\omega ={1 \over 2\pi }\int _{-2\pi B}^{2\pi B}X
            (\omega )e^{i\omega t}\;{\rm {d}}\omega ,}  [{\displaystyle x(t)={1
            \over 2\pi }\int _{-\infty }^{\infty }X(\omega )e^{i\omega t}\;{\rm
            {d}}\omega ={1 \over 2\pi }\int _{-2\pi B}^{2\pi B}X(\omega )e^
            {i\omega t}\;{\rm {d}}\omega ,}]
      because     X ( &#x03C9; )   {\displaystyle X(\omega )}  [X(\omega )] is
      assumed to be zero outside the band      |    &#x03C9;  2 &#x03C0;     |
      < B .   {\displaystyle \left|{\tfrac {\omega }{2\pi }}\right|<B.}  [
      {\displaystyle \left|{\tfrac {\omega }{2\pi }}\right|<B.}]  If we let
      t =    n  2 B     ,   {\displaystyle t={\tfrac {n}{2B}},}  [
      {\displaystyle t={\tfrac {n}{2B}},}] where     n   {\displaystyle n}  [n]
      is any positive or negative integer, we obtain:
               x  (    n  2 B     )  =   1  2 &#x03C0;     &#x222B;  &#x2212; 2
            &#x03C0; B   2 &#x03C0; B   X ( &#x03C9; )  e  i &#x03C9;   n  2 B
            d   &#x03C9; .   {\displaystyle x\left({\tfrac {n}{2B}}\right)={1
            \over 2\pi }\int _{-2\pi B}^{2\pi B}X(\omega )e^{i\omega {n \over
            {2B}}}\;{\rm {d}}\omega .}  [x\left({\tfrac {n}{2B}}\right)={1
            \over 2\pi }\int _{-2\pi B}^{2\pi B}X(\omega )e^{i\omega {n \over
            {2B}}}\;{\rm {d}}\omega .]
      On the left are values of     x ( t )   {\displaystyle x(t)}  [x(t)] at
      the sampling points. The integral on the right will be recognized as
      essentially[n_1] the nth coefficient in a Fourier-series expansion of the
      function     X ( &#x03C9; ) ,   {\displaystyle X(\omega ),}  [
      {\displaystyle X(\omega ),}] taking the interval     &#x2212; B
      {\displaystyle -B}  [-B] to     B   {\displaystyle B}  [B] as a
      fundamental period. This means that the values of the samples     x ( n
      /  2 B )   {\displaystyle x(n/2B)}  [{\displaystyle x(n/2B)}] determine
      the Fourier coefficients in the series expansion of     X ( &#x03C9; ) .
      {\displaystyle X(\omega ).}  [{\displaystyle X(\omega ).}]  Thus they
      determine     X ( &#x03C9; ) ,   {\displaystyle X(\omega ),}  [
      {\displaystyle X(\omega ),}] since     X ( &#x03C9; )   {\displaystyle X
      (\omega )}  [X(\omega )] is zero for frequencies greater than B, and for
      lower frequencies     X ( &#x03C9; )   {\displaystyle X(\omega )}  [X
      (\omega )] is determined if its Fourier coefficients are determined. But
      X ( &#x03C9; )   {\displaystyle X(\omega )}  [X(\omega )] determines the
      original function     x ( t )   {\displaystyle x(t)}  [x(t)] completely,
      since a function is determined if its spectrum is known. Therefore the
      original samples determine the function     x ( t )   {\displaystyle x
      (t)}  [x(t)] completely.
Shannon's proof of the theorem is complete at that point, but he goes on to
discuss reconstruction via sinc_functions, what we now call the
WhittakerâShannon_interpolation_formula as discussed above. He does not
derive or prove the properties of the sinc function, but these would have been
[weasel words] familiar to engineers reading his works at the time, since the
Fourier pair relationship between rect (the rectangular function) and sinc was
well known.
      Let      x  n     {\displaystyle x_{n}}  [x_{n}] be the nth sample. Then
      the function     x ( t )   {\displaystyle x(t)}  [x(t)] is represented
      by:
               x ( t ) =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;    x  n
            sin &#x2061; &#x03C0; ( 2 B t &#x2212; n )   &#x03C0; ( 2 B t
            &#x2212; n )    .   {\displaystyle x(t)=\sum _{n=-\infty }^{\infty
            }x_{n}{\sin \pi (2Bt-n) \over \pi (2Bt-n)}.}  [{\displaystyle x
            (t)=\sum _{n=-\infty }^{\infty }x_{n}{\sin \pi (2Bt-n) \over \pi
            (2Bt-n)}.}]
As in the other proof, the existence of the Fourier transform of the original
signal is assumed, so the proof does not say whether the sampling theorem
extends to bandlimited stationary random processes.
**** Notes[edit] ****
   1. ^ The actual coefficient formula contains an additional factor of     1
      /  2 B = T .   {\displaystyle 1/2B=T.}  [{\displaystyle 1/2B=T.}] So
      Shannon's coefficients are     T &#x22C5; x ( n T ) ,   {\displaystyle
      T\cdot x(nT),}  [{\displaystyle T\cdot x(nT),}] which agrees with Eq.1.
***** Application to multivariable signals and images[edit] *****
Main article: Multidimensional_sampling
Subsampled image showing a MoirÃ©_pattern
Properly sampled image
The sampling theorem is usually formulated for functions of a single variable.
Consequently, the theorem is directly applicable to time-dependent signals and
is normally formulated in that context. However, the sampling theorem can be
extended in a straightforward way to functions of arbitrarily many variables.
Grayscale images, for example, are often represented as two-dimensional arrays
(or matrices) of real numbers representing the relative intensities of pixels
(picture elements) located at the intersections of row and column sample
locations. As a result, images require two independent variables, or indices,
to specify each pixel uniquelyâone for the row, and one for the column.
Color images typically consist of a composite of three separate grayscale
images, one to represent each of the three primary colorsâred, green, and
blue, or RGB for short. Other colorspaces using 3-vectors for colors include
HSV, CIELAB, XYZ, etc. Some colorspaces such as cyan, magenta, yellow, and
black (CMYK) may represent color by four dimensions. All of these are treated
as vector-valued_functions over a two-dimensional sampled domain.
Similar to one-dimensional discrete-time signals, images can also suffer from
aliasing if the sampling resolution, or pixel density, is inadequate. For
example, a digital photograph of a striped shirt with high frequencies (in
other words, the distance between the stripes is small), can cause aliasing of
the shirt when it is sampled by the camera's image_sensor. The aliasing appears
as a moirÃ©_pattern. The "solution" to higher sampling in the spatial domain
for this case would be to move closer to the shirt, use a higher resolution
sensor, or to optically blur the image before acquiring it with the sensor.
Another example is shown to the right in the brick patterns. The top image
shows the effects when the sampling theorem's condition is not satisfied. When
software rescales an image (the same process that creates the thumbnail shown
in the lower image) it, in effect, runs the image through a low-pass_filter
first and then downsamples the image to result in a smaller image that does not
exhibit the moirÃ©_pattern. The top image is what happens when the image is
downsampled without low-pass filtering: aliasing results.
The sampling theorem applies to camera systems, where the scene and lens
constitute an analog spatial signal source, and the image sensor is a spatial
sampling device. Each of these components is characterized by a modulation
transfer_function (MTF), representing the precise resolution (spatial
bandwidth) available in that component. Effects of aliasing or blurring can
occur when the lens MTF and sensor MTF are mismatched. When the optical image
which is sampled by the sensor device contains higher spatial frequencies than
the sensor, the under sampling acts as a low-pass filter to reduce or eliminate
aliasing. When the area of the sampling spot (the size of the pixel sensor) is
not large enough to provide sufficient spatial_anti-aliasing, a separate anti-
aliasing filter (optical low-pass filter) may be included in a camera system to
reduce the MTF of the optical image. Instead of requiring an optical filter,
the graphics_processing_unit of smartphone cameras performs digital_signal
processing to remove aliasing with a digital filter. Digital filters also apply
sharpening to amplify the contrast from the lens at high spatial frequencies,
which otherwise falls off rapidly at diffraction limits.
The sampling theorem also applies to post-processing digital images, such as to
up or down sampling. Effects of aliasing, blurring, and sharpening may be
adjusted with digital filtering implemented in software, which necessarily
follows the theoretical principles.
***** Critical frequency[edit] *****
To illustrate the necessity of      f  s   > 2 B   {\displaystyle f_{s}>2B}  [
{\displaystyle f_{s}>2B}], consider the family of sinusoids generated by
different values of     &#x03B8;   {\displaystyle \theta }  [\theta ] in this
formula:
         x ( t ) =    cos &#x2061; ( 2 &#x03C0; B t + &#x03B8; )   cos &#x2061;
      ( &#x03B8; )    &#xA0; = &#xA0; cos &#x2061; ( 2 &#x03C0; B t ) &#x2212;
      sin &#x2061; ( 2 &#x03C0; B t ) tan &#x2061; ( &#x03B8; ) ,  &#x2212;
      &#x03C0;  /  2 < &#x03B8; < &#x03C0;  /  2.   {\displaystyle x(t)={\frac
      {\cos(2\pi Bt+\theta )}{\cos(\theta )}}\ =\ \cos(2\pi Bt)-\sin(2\pi
      Bt)\tan(\theta ),\quad -\pi /2<\theta <\pi /2.}  [x(t)={\frac {\cos(2\pi
      Bt+\theta )}{\cos(\theta )}}\ =\ \cos(2\pi Bt)-\sin(2\pi Bt)\tan(\theta
      ),\quad -\pi /2<\theta <\pi /2.]
A family of sinusoids at the critical frequency, all having the same sample
sequences of alternating +1 and â1. That is, they all are aliases of each
other, even though their frequency is not above half the sample rate.
With      f  s   = 2 B   {\displaystyle f_{s}=2B}  [{\displaystyle f_{s}=2B}]
or equivalently     T = 1  /  2 B   {\displaystyle T=1/2B}  [{\displaystyle
T=1/2B}], the samples are given by:
         x ( n T ) = cos &#x2061; ( &#x03C0; n ) &#x2212;     sin &#x2061;
      ( &#x03C0; n )  &#x23DF;    0   tan &#x2061; ( &#x03B8; ) = ( &#x2212; 1
      )  n     {\displaystyle x(nT)=\cos(\pi n)-\underbrace {\sin(\pi n)} _
      {0}\tan(\theta )=(-1)^{n}}  [x(nT)=\cos(\pi n)-\underbrace {\sin(\pi n)}
      _{0}\tan(\theta )=(-1)^{n}]
regardless of the value of     &#x03B8;   {\displaystyle \theta }  [\theta ].
That sort of ambiguity is the reason for the strict inequality of the sampling
theorem's condition.
***** Sampling of non-baseband signals[edit] *****
As discussed by Shannon:[2]
           A similar result is true if the band does not start at zero
           frequency but at some higher value, and can be proved by a
           linear translation (corresponding physically to single-sideband
           modulation) of the zero-frequency case. In this case the
           elementary pulse is obtained from sin(x)/x by single-side-band
           modulation.
That is, a sufficient no-loss condition for sampling signals that do not have
baseband components exists that involves the width of the non-zero frequency
interval as opposed to its highest frequency component. See Sampling_(signal
processing) for more details and examples.
For example, in order to sample the FM_radio signals in the frequency range of
100â102 MHz, it is not necessary to sample at 204 MHz (twice the upper
frequency), but rather it is sufficient to sample at 4 MHz (twice the width of
the frequency interval).
A bandpass condition is that X(f) = 0, for all nonnegative f outside the open
band of frequencies:
                (    N 2    f   s    ,    N + 1  2    f   s     )  ,
            {\displaystyle \left({\frac {N}{2}}f_{\mathrm {s} },{\frac {N+1}
            {2}}f_{\mathrm {s} }\right),}  [\left({\frac {N}{2}}f_{\mathrm {s}
            },{\frac {N+1}{2}}f_{\mathrm {s} }\right),]
for some nonnegative integer N. This formulation includes the normal baseband
condition as the case N=0.
The corresponding interpolation function is the impulse response of an ideal
brick-wall bandpass_filter (as opposed to the ideal brick-wall lowpass_filter
used above) with cutoffs at the upper and lower edges of the specified band,
which is the difference between a pair of lowpass impulse responses:
               ( N + 1 )  sinc &#x2061;  (    ( N + 1 ) t  T   )  &#x2212; N
            sinc &#x2061;  (    N t  T   )  .   {\displaystyle
            (N+1)\,\operatorname {sinc} \left({\frac {(N+1)t}{T}}\right)-
            N\,\operatorname {sinc} \left({\frac {Nt}{T}}\right).}  [
            (N+1)\,\operatorname {sinc} \left({\frac {(N+1)t}{T}}\right)-
            N\,\operatorname {sinc} \left({\frac {Nt}{T}}\right).]
Other generalizations, for example to signals occupying multiple non-contiguous
bands, are possible as well. Even the most generalized form of the sampling
theorem does not have a provably true converse. That is, one cannot conclude
that information is necessarily lost just because the conditions of the
sampling theorem are not satisfied; from an engineering perspective, however,
it is generally safe to assume that if the sampling theorem is not satisfied
then information will most likely be lost.
***** Nonuniform sampling[edit] *****
The sampling theory of Shannon can be generalized for the case of nonuniform
sampling, that is, samples not taken equally spaced in time. The Shannon
sampling theory for non-uniform sampling states that a band-limited signal can
be perfectly reconstructed from its samples if the average sampling rate
satisfies the Nyquist condition.[3] Therefore, although uniformly spaced
samples may result in easier reconstruction algorithms, it is not a necessary
condition for perfect reconstruction.
The general theory for non-baseband and nonuniform samples was developed in
1967 by Henry_Landau.[4] He proved that the average sampling rate (uniform or
otherwise) must be twice the occupied bandwidth of the signal, assuming it is a
priori known what portion of the spectrum was occupied. In the late 1990s, this
work was partially extended to cover signals of when the amount of occupied
bandwidth was known, but the actual occupied portion of the spectrum was
unknown.[5] In the 2000s, a complete theory was developed (see the section
Sampling_below_the_Nyquist_rate_under_additional_restrictions below) using
compressed_sensing. In particular, the theory, using signal processing
language, is described in this 2009 paper.[6] They show, among other things,
that if the frequency locations are unknown, then it is necessary to sample at
least at twice the Nyquist criteria; in other words, you must pay at least a
factor of 2 for not knowing the location of the spectrum. Note that minimum
sampling requirements do not necessarily guarantee stability.
***** Sampling below the Nyquist rate under additional restrictions[edit] *****
Main article: Undersampling
The NyquistâShannon sampling theorem provides a sufficient_condition for the
sampling and reconstruction of a band-limited signal. When reconstruction is
done via the WhittakerâShannon_interpolation_formula, the Nyquist criterion
is also a necessary condition to avoid aliasing, in the sense that if samples
are taken at a slower rate than twice the band limit, then there are some
signals that will not be correctly reconstructed. However, if further
restrictions are imposed on the signal, then the Nyquist criterion may no
longer be a necessary_condition.
A non-trivial example of exploiting extra assumptions about the signal is given
by the recent field of compressed_sensing, which allows for full reconstruction
with a sub-Nyquist sampling rate. Specifically, this applies to signals that
are sparse (or compressible) in some domain. As an example, compressed sensing
deals with signals that may have a low over-all bandwidth (say, the effective
bandwidth EB), but the frequency locations are unknown, rather than all
together in a single band, so that the passband_technique does not apply. In
other words, the frequency spectrum is sparse. Traditionally, the necessary
sampling rate is thus 2B. Using compressed sensing techniques, the signal could
be perfectly reconstructed if it is sampled at a rate slightly lower than 2EB.
With this approach, reconstruction is no longer given by a formula, but instead
by the solution to a linear_optimization_program.
Another example where sub-Nyquist sampling is optimal arises under the
additional constraint that the samples are quantized in an optimal manner, as
in a combined system of sampling and optimal lossy_compression.[7] This setting
is relevant in cases where the joint effect of sampling and quantization is to
be considered, and can provide a lower bound for the minimal reconstruction
error that can be attained in sampling and quantizing a random_signal. For
stationary Gaussian random signals, this lower bound is usually attained at a
sub-Nyquist sampling rate, indicating that sub-Nyquist sampling is optimal for
this signal model under optimal quantization.[8]
***** Historical background[edit] *****
The sampling theorem was implied by the work of Harry_Nyquist in 1928,[9] in
which he showed that up to 2B independent pulse samples could be sent through a
system of bandwidth B; but he did not explicitly consider the problem of
sampling and reconstruction of continuous signals. About the same time, Karl
KÃ¼pfmÃ¼ller showed a similar result[10] and discussed the sinc-function
impulse response of a band-limiting filter, via its integral, the step-response
sine_integral; this bandlimiting and reconstruction filter that is so central
to the sampling theorem is sometimes referred to as a KÃ¼pfmÃ¼ller filter (but
seldom so in English).
The sampling theorem, essentially a dual of Nyquist's result, was proved by
Claude_E._Shannon.[2] V._A._Kotelnikov published similar results in 1933,[11]
as did the mathematician E._T._Whittaker in 1915,[12] J. M. Whittaker in 1935,
[13] and Gabor in 1946 ("Theory of communication"). In 1999, the Eduard_Rhein
Foundation awarded Kotelnikov their Basic Research Award "for the first
theoretically exact formulation of the sampling theorem".
In 1948 and 1949, Claude E. Shannon published the two revolutionary articles in
which he founded the information theory.[14][15][2] In Shannon_1948 the
sampling theorem is formulated as âTheorem 13â: Let f(t) contain no
frequencies over W. Then
         f ( t ) =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;    X  n      sin
      &#x2061; &#x03C0; ( 2 W t &#x2212; n )   &#x03C0; ( 2 W t &#x2212; n )
      ,   {\displaystyle f(t)=\sum _{n=-\infty }^{\infty }X_{n}{\frac {\sin \pi
      (2Wt-n)}{\pi (2Wt-n)}},}  [{\displaystyle f(t)=\sum _{n=-\infty }^{\infty
      }X_{n}{\frac {\sin \pi (2Wt-n)}{\pi (2Wt-n)}},}] where      X  n   = f
      (   n  2 W    )    {\displaystyle X_{n}=f\left({\frac {n}{2W}}\right)}  [
      {\displaystyle X_{n}=f\left({\frac {n}{2W}}\right)}].
It was not until these articles were published that the theorem known as
âShannonâs sampling theoremâ became common property among communication
engineers, although Shannon himself writes that this is a fact which is common
knowledge in the communication art.[note_2] A few lines further on, however, he
adds: "but in spite of its evident importance, [it] seems not to have appeared
explicitly in the literature of communication theory".
**** Other discoverers[edit] ****
Others who have independently discovered or played roles in the development of
the sampling theorem have been discussed in several historical articles, for
example, by Jerri[16] and by LÃ¼ke.[17] For example, LÃ¼ke points out that H.
Raabe, an assistant to KÃ¼pfmÃ¼ller, proved the theorem in his 1939 Ph.D.
dissertation; the term Raabe condition came to be associated with the criterion
for unambiguous representation (sampling rate greater than twice the
bandwidth). Meijering[18] mentions several other discoverers and names in a
paragraph and pair of footnotes:
     As pointed out by Higgins [135], the sampling theorem should really
     be considered in two parts, as done above: the first stating the fact
     that a bandlimited function is completely determined by its samples,
     the second describing how to reconstruct the function using its
     samples. Both parts of the sampling theorem were given in a somewhat
     different form by J. M. Whittaker [350, 351, 353] and before him also
     by Ogura [241, 242]. They were probably not aware of the fact that
     the first part of the theorem had been stated as early as 1897 by
     Borel [25].27 As we have seen, Borel also used around that time what
     became known as the cardinal series. However, he appears not to have
     made the link [135]. In later years it became known that the sampling
     theorem had been presented before Shannon to the Russian
     communication community by Kotel'nikov [173]. In more implicit,
     verbal form, it had also been described in the German literature by
     Raabe [257]. Several authors [33, 205] have mentioned that Someya
     [296] introduced the theorem in the Japanese literature parallel to
     Shannon. In the English literature, Weston [347] introduced it
     independently of Shannon around the same time.28
     27 Several authors, following Black [16], have claimed that this
     first part of the sampling theorem was stated even earlier by Cauchy,
     in a paper [41] published in 1841. However, the paper of Cauchy does
     not contain such a statement, as has been pointed out by Higgins
     [135].
     28 As a consequence of the discovery of the several independent
     introductions of the sampling theorem, people started to refer to the
     theorem by including the names of the aforementioned authors,
     resulting in such catchphrases as âthe
     WhittakerâKotelânikovâShannon (WKS) sampling theorem" [155] or
     even "the WhittakerâKotel'nikovâRaabeâShannonâSomeya sampling
     theorem" [33]. To avoid confusion, perhaps the best thing to do is to
     refer to it as the sampling theorem, "rather than trying to find a
     title that does justice to all claimants" [136].
**** Why Nyquist?[edit] ****
Exactly how, when, or why Harry_Nyquist had his name attached to the sampling
theorem remains obscure. The term Nyquist Sampling Theorem (capitalized thus)
appeared as early as 1959 in a book from his former employer, Bell_Labs,[19]
and appeared again in 1963,[20] and not capitalized in 1965.[21] It had been
called the Shannon Sampling Theorem as early as 1954,[22] but also just the
sampling theorem by several other books in the early 1950s.
In 1958, Blackman and Tukey cited Nyquist's 1928 article as a reference for the
sampling theorem of information theory,[23] even though that article does not
treat sampling and reconstruction of continuous signals as others did. Their
glossary of terms includes these entries:
  Sampling theorem (of information theory)
      Nyquist's result that equi-spaced data, with two or more points per cycle
      of highest frequency, allows reconstruction of band-limited functions.
      (See Cardinal theorem.)
  Cardinal theorem (of interpolation theory)
      A precise statement of the conditions under which values given at a
      doubly infinite set of equally spaced points can be interpolated to yield
      a continuous band-limited function with the aid of the function
                  sin &#x2061; ( x &#x2212;  x  i   )   x &#x2212;  x  i      .
            {\displaystyle {\frac {\sin(x-x_{i})}{x-x_{i}}}.}  [{\frac {\sin(x-
            x_{i})}{x-x_{i}}}.]
Exactly what "Nyquist's result" they are referring to remains mysterious.
When Shannon stated and proved the sampling theorem in his 1949 article,
according to Meijering,[18] "he referred to the critical sampling interval
T =   1  2 W      {\displaystyle T={\frac {1}{2W}}}  [{\displaystyle T={\frac
{1}{2W}}}] as the Nyquist interval corresponding to the band W, in recognition
of Nyquistâs discovery of the fundamental importance of this interval in
connection with telegraphy". This explains Nyquist's name on the critical
interval, but not on the theorem.
Similarly, Nyquist's name was attached to Nyquist_rate in 1953 by Harold_S.
Black:
     "If the essential frequency range is limited to B cycles per second,
     2B was given by Nyquist as the maximum number of code elements per
     second that could be unambiguously resolved, assuming the peak
     interference is less half a quantum step. This rate is generally
     referred to as signaling at the Nyquist rate and       1  2 B
     {\displaystyle {\frac {1}{2B}}}  [{\displaystyle {\frac {1}{2B}}}]
     has been termed a Nyquist interval."[24] (bold added for emphasis;
     italics as in the original)
According to the OED, this may be the origin of the term Nyquist rate. In
Black's usage, it is not a sampling rate, but a signaling rate.
***** See also[edit] *****
 Wikimedia Commons has media related to Nyquist_Shannon_theorem.
    * BalianâLow_theorem, a similar theoretical lower bound on sampling
      rates, but which applies to timeâfrequency_transforms.
    * The CheungâMarks_theorem specifies conditions where restoration of a
      signal by the sampling theorem can become ill-posed.
    * Hartley's_law
    * Nyquist_ISI_criterion
    * Reconstruction_from_zero_crossings
    * Zero-order_hold
***** Notes[edit] *****
   1. ^ The sinc function follows from rows 202 and 102 of the transform_tables
   2. ^ Shannon_1949, p 448.
***** References[edit] *****
   1. ^Nemirovsky, Jonathan; Shimron, Efrat (2015). "Utilizing Bochners Theorem
      for Constrained Evaluation of Missing Fourier Data". arXiv:1506.03300
      [physics.med-ph].
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
   3. ^ a b c dShannon,_Claude_E. (January 1949). "Communication in the
      presence of noise". Proceedings of the Institute of Radio Engineers. 37
      (1): 10â21. doi:10.1109/jrproc.1949.232969.
   4.  Reprint_as_classic_paper_in:_Proc._IEEE,_Vol._86,_No._2,_(Feb_1998)
      Archived 2010-02-08 at the Wayback_Machine
   5. ^Marvasti (ed), F. (2000). Nonuniform Sampling, Theory and Practice. New
      York: Kluwer Academic/Plenum Publishers.CS1 maint: Extra text: authors
      list (link)
   6. ^Landau, H. J. (1967). "Necessary density conditions for sampling and
      interpolation of certain entire functions". Acta Math. 117 (1): 37â52.
      doi:10.1007/BF02395039.
   7. ^ see, e.g.,Feng, P. (1997). Universal minimum-rate sampling and
      spectrum-blind reconstruction for multiband signals. Ph.D. dissertation,
      University of Illinois at Urbana-Champaign.
   8. ^Mishali, Moshe; Eldar, Yonina C. (March 2009). "Blind Multiband Signal
      Reconstruction: Compressed Sensing for Analog Signals". IEEE Trans.
      Signal Process. 57 (3). CiteSeerX 10.1.1.154.4255.
   9. ^Kipnis, Alon; Goldsmith, Andrea J.; Eldar, Yonina C.; Weissman, Tsachy
      (January 2016). "Distortion rate function of sub-Nyquist sampled Gaussian
      sources". IEEE Transactions on Information Theory. 62: 401â429. arXiv:
      1405.5329. doi:10.1109/tit.2015.2485271.
  10. ^Kipnis, Alon; Eldar, Yonina; Goldsmith, Andrea (26 April 2018). "Analog-
      to-Digital Compression: A New Paradigm for Converting Signals to Bits".
      IEEE Signal Processing Magazine. 35 (3): 16â39. arXiv:1801.06718.
      Bibcode:2018ISPM...35...16K. doi:10.1109/MSP.2017.2774249.
  11. ^Nyquist,_Harry (April 1928). "Certain topics in telegraph transmission
      theory". Trans. AIEE. 47 (2): 617â644. Bibcode:1928TAIEE..47..617N.
      doi:10.1109/t-aiee.1928.5055024.
  12.  Reprint_as_classic_paper_in:_Proc._IEEE,_Vol._90,_No._2,_Feb_2002
      Archived 2013-09-26 at the Wayback_Machine
  13. ^KÃ¼pfmÃ¼ller, Karl (1928). "Ãber die Dynamik der selbsttÃ¤tigen
      VerstÃ¤rkungsregler". Elektrische Nachrichtentechnik (in German). 5 (11):
      459â467.
  14.  (English_translation_2005).
  15. ^Kotelnikov,_V._A. (1933). "On the carrying capacity of the ether and
      wire in telecommunications". Material for the First All-Union Conference
      on Questions of Communication, Izd. Red. Upr. Svyazi RKKA (in Russian).
  16.  (English_translation,_PDF).
  17. ^Whittaker,_E._T. (1915). "On_the_Functions_Which_are_Represented_by_the
      Expansions_of_the_Interpolation_Theory". Proc. Royal Soc. Edinburgh. 35:
      181â194. doi:10.1017/s0370164600017806.
  18.  ("Theorie der Kardinalfunktionen").
  19. ^Whittaker,_J._M. (1935). Interpolatory Function Theory. Cambridge,
      England: Cambridge Univ. Press.
  20. .
  21. ^Shannon,_Claude_E. (July 1948). "A Mathematical Theory of
      Communication". Bell System Technical Journal. 27 (3): 379â423. doi:
      10.1002/j.1538-7305.1948.tb01338.x. hdl:11858/00-001M-0000-002C-4317-B.
  22. .
  23. ^Shannon,_Claude_E. (October 1948). "A Mathematical Theory of
      Communication". Bell System Technical Journal. 27 (4): 623â666. doi:
      10.1002/j.1538-7305.1948.tb00917.x. hdl:11858/00-001M-0000-002C-4314-2.
  24. ^Jerri,_Abdul (November 1977). "The_Shannon_Sampling_TheoremâIts
      Various_Extensions_and_Applications:_A_Tutorial_Review". Proceedings of
      the IEEE. 65 (11): 1565â1596. doi:10.1109/proc.1977.10771. Archived
      from the original on 2008-06-05.CS1 maint: BOT: original-url status
      unknown (link)
  25.  See alsoJerri, Abdul (April 1979). "Correction_to_"The_Shannon_sampling
      theoremâIts_various_extensions_and_applications:_A_tutorial_review"".
      Proceedings of the IEEE. 67 (4): 695. doi:10.1109/proc.1979.11307.
      Archived from the original on 2009-01-20.CS1 maint: BOT: original-url
      status unknown (link)
  26. ^LÃ¼ke, Hans Dieter (April 1999). "The_Origins_of_the_Sampling_Theorem"
      (PDF). IEEE Communications Magazine. 37 (4): 106â108.
      CiteSeerX 10.1.1.163.2887. doi:10.1109/35.755459.
  27. ^ a bMeijering, Erik (March 2002). "A_Chronology_of_Interpolation_From
      Ancient_Astronomy_to_Modern_Signal_and_Image_Processing" (PDF). Proc.
      IEEE. 90 (3): 319â342. doi:10.1109/5.993400.
  28. ^Members of the Technical Staff of Bell Telephone Lababoratories (1959).
      Transmission Systems for Communications. AT&T. pp. 26â4 (Vol.2).
  29. ^Guillemin, Ernst Adolph (1963). Theory_of_Linear_Physical_Systems.
      Wiley.
  30. ^Roberts, Richard A.; Barton, Ben F. (1965). Theory of Signal
      Detectability: Composite Deferred Decision Theory.
  31. ^Gray, Truman S. (1954). Applied Electronics: A First Course in
      Electronics, Electron Tubes, and Associated Circuits.
  32. ^Blackman, R. B.; Tukey, J. W. (1958). The_Measurement_of_Power_Spectra :
      From_the_Point_of_View_of_Communications_Engineering (PDF). New York:
      Dover.
  33. ^Black, Harold S. (1953). Modulation Theory.
***** Further reading[edit] *****
    * Higgins, J.R.: Five short stories about the cardinal series, Bulletin of
      the AMS 12(1985)
    * KÃ¼pfmÃ¼ller,_Karl, "UtjÃ¤mningsfÃ¶rlopp inom Telegraf- och
      Telefontekniken", ("Transients in telegraph and telephone engineering"),
      Teknisk_Tidskrift, no. 9 pp. 153â160 and 10 pp. 178â182, 1931. [1]
      [2]
    * Marks, R.J.(II): Introduction_to_Shannon_Sampling_and_Interpolation
      Theory, Springer-Verlag, 1991.
    * Marks, R.J.(II), Editor: Advanced_Topics_in_Shannon_Sampling_and
      Interpolation_Theory, Springer-Verlag, 1993.
    * Marks, R.J.(II), Handbook of Fourier Analysis and Its Applications,
      Oxford University Press, (2009), Chapters 5-8. Google_books
    * Press, WH; Teukolsky, SA; Vetterling, WT; Flannery, BP (2007), "Section
      13.11._Numerical_Use_of_the_Sampling_Theorem", Numerical Recipes: The Art
      of Scientific Computing (3rd ed.), New York: Cambridge University Press,
      ISBN 978-0-521-88068-8
Unser, Michael: Sampling-50_Years_after_Shannon, Proc. IEEE, vol. 88, no. 4,
pp. 569â587, April 2000
***** External links[edit] *****
 Wikimedia Commons has media related to Nyquist_Shannon_theorem.
    * Learning_by_Simulations Interactive simulation of the effects of
      inadequate sampling
    * Interactive_presentation_of_the_sampling_and_reconstruction_in_a_web-demo
      Institute of Telecommunications, University of Stuttgart
    * Undersampling_and_an_application_of_it
    * Sampling_Theory_For_Digital_Audio
    * Journal_devoted_to_Sampling_Theory
    * Sampling_Theorem_with_Constant_Amplitude_Variable_Width_Pulse
    * LÃ¼ke, Hans Dieter (April 1999). "The_Origins_of_the_Sampling_Theorem"
      (PDF). IEEE Communications Magazine. 37 (4): 106â108.
      CiteSeerX 10.1.1.163.2887. doi:10.1109/35.755459.
    * v
    * t
    * e
Digital_signal_processing
               * Detection_theory
Theory         * Discrete_signal
               * Estimation_theory
               * NyquistâShannon sampling theorem
               * Audio_signal_processing
Sub-fields     * Digital_image_processing
               * Speech_processing
               * Statistical_signal_processing
               * Advanced_Z-transform
               * Bilinear_transform
               * Constant-Q_transform
               * Discrete_Fourier_transform (DFT)
               * Discrete-time_Fourier_transform (DTFT)
               * Impulse_invariance
Techniques     * Integral_transform
               * Laplace_transform
               * Matched_Z-transform_method
               * Post's_inversion_formula
               * Starred_transform
               * Z-transform
               * Zak_transform
               * Aliasing
               * Anti-aliasing_filter
               * Downsampling
               * Nyquist_rate / frequency
Sampling       * Oversampling
               * Quantization
               * Sampling_rate
               * Undersampling
               * Upsampling
    * v
    * t
    * e
Data_compression methods
                             * Arithmetic
                             * Asymmetric_numeral_systems
                             * Golomb
                             * Huffman
                                   o Adaptive
                                   o Canonical
                                   o Modified
                             * Range
         Entropy_type        * Shannon
                             * ShannonâFano
                             * ShannonâFanoâElias
                             * Tunstall
                             * Unary
                             * Universal
                                   o Exp-Golomb
                                   o Fibonacci
                                   o Gamma
                                   o Levenshtein
                             * Byte_pair_encoding
                             * DEFLATE
                             * Snappy
Lossless                     * LempelâZiv
                                   o LZ77 /_LZ78_(LZ1 /_LZ2)
                                   o LZFSE
                                   o LZJB
                                   o LZMA
         Dictionary_type           o LZO
                                   o LZRW
                                   o LZS
                                   o LZSS
                                   o LZW
                                   o LZWL
                                   o LZX
                                   o LZ4
                                   o Brotli
                                   o Zstandard
                             * BWT
                             * CTW
                             * Delta
         Other types         * DMC
                             * MTF
                             * PAQ
                             * PPM
                             * RLE
                         * Bit_rate
                               o ABR
                               o CBR
                               o VBR
                         * Companding
                         * Convolution
         Concepts        * Dynamic_range
                         * Latency
                         * NyquistâShannon theorem
                         * Sampling
                         * Sound_quality
                         * Speech_coding
Audio                    * Sub-band_coding
                         * A-law
                         * Î¼-law
                         * ACELP
                         * ADPCM
                         * CELP
                         * DPCM
         Codec parts     * Fourier_transform
                         * LPC
                               o LAR
                               o LSP
                         * MDCT
                         * Psychoacoustic_model
                         * WLPC
                      * Chroma_subsampling
                      * Coding_tree_unit
                      * Color_space
                      * Compression_artifact
         Concepts     * Image_resolution
                      * Macroblock
                      * Pixel
                      * PSNR
                      * Quantization
Image                 * Standard_test_image
                      * Chain_code
                      * DCT
                      * EZW
                      * Fractal
         Methods      * KLT
                      * LP
                      * RLE
                      * SPIHT
                      * Wavelet
                         * Bit_rate
                               o ABR
                               o CBR
                               o VBR
                         * Display_resolution
         Concepts        * Frame
                         * Frame_rate
Video                    * Frame_types
                         * Interlace
                         * Video_characteristics
                         * Video_quality
                         * DCT
         Codec parts     * Deblocking_filter
                         * Lapped_transform
                         * Motion_compensation
             * Entropy
             * Information_theory
                   o Timeline
             * Kolmogorov_complexity
Theory       * Lossy
                   o DCT
             * Quantization
             * Rateâdistortion
             * Redundancy
    * [Template] Compression_formats
    * [Template] Compression_software_(codecs)

Retrieved from "https://en.wikipedia.org/w/
index.php?title=NyquistâShannon_sampling_theorem&oldid=909591526"
Categories:
    * Digital_signal_processing
    * Information_theory
    * Theorems_in_Fourier_analysis
    * Mathematical_theorems_in_theoretical_computer_science
    * Claude_Shannon
    * Telecommunication_theory
Hidden categories:
    * Webarchive_template_wayback_links
    * CS1_maint:_Extra_text:_authors_list
    * CS1_German-language_sources_(de)
    * CS1_Russian-language_sources_(ru)
    * CS1_maint:_BOT:_original-url_status_unknown
    * Use_American_English_from_March_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * All_articles_with_specifically_marked_weasel-worded_phrases
    * Articles_with_specifically_marked_weasel-worded_phrases_from_June_2017
    * Commons_category_link_is_on_Wikidata
    * Articles_containing_proofs
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Italiano
    * ×¢××¨××ª
    * à¤®à¤°à¤¾à¤ à¥
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Basa_Sunda
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 6 August 2019, at 10:43 (UTC).
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
