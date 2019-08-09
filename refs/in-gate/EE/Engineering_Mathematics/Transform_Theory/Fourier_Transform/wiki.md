The following text has been accessed from https://en.wikipedia.org/wiki/Fourier_transform at Thu Aug 8 22:50:17 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Fourier transform ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The Fourier transform (FT) decomposes a function of time (a signal) into its
constituent frequencies. This is similar to the way a musical chord can be
expressed in terms of the volumes and frequencies of its constituent notes. The
term Fourier transform refers to both the frequency_domain representation and
the mathematical operation that associates the frequency domain representation
to a function of time. The Fourier transform of a function of time is itself a
complex-valued function of frequency, whose magnitude (modulus) represents the
amount of that frequency present in the original function, and whose argument
is the phase_offset of the basic sinusoid in that frequency. The Fourier
transform is not limited to functions of time, but the domain_of_the_original
function is commonly referred to as the time_domain. There is also an inverse
Fourier transform that mathematically synthesizes the original function from
its frequency domain representation.
    * A sinusoidal curve, with peak amplitude (1), peak-to-peak (2), RMS (3),
      and wave period (4).
    * Illustration of phase shift Î¸.
    f ( t )    {\displaystyle \scriptstyle f(t)}  [\scriptstyle f(t)]
       f &#x005E;    ( &#x03C9; )    {\displaystyle \scriptstyle {\hat {f}}
(\omega )}  [\scriptstyle {\hat {f}}(\omega )]
    g ( t )    {\displaystyle \scriptstyle g(t)}  [\scriptstyle g(t)]
       g &#x005E;    ( &#x03C9; )    {\displaystyle \scriptstyle {\hat {g}}
(\omega )}  [\scriptstyle {\hat {g}}(\omega )]
    t    {\displaystyle \scriptstyle t}  [\scriptstyle t]
    &#x03C9;    {\displaystyle \scriptstyle \omega }  [\scriptstyle \omega ]
    t    {\displaystyle \scriptstyle t}  [\scriptstyle t]
    &#x03C9;    {\displaystyle \scriptstyle \omega }  [\scriptstyle \omega ]
In the first row of the figure is the graph of the unit_pulse function f (t)
and its Fourier transform fÌ (Ï), a function of frequency Ï. Translation
(that is, delay) in the time domain is interpreted as complex phase shifts in
the frequency domain. In the second row is shown g(t), a delayed unit pulse,
beside the real and imaginary parts of the Fourier transform. The Fourier
transform decomposes a function into eigenfunctions for the group of
translations.
Fourier transforms
Continuous Fourier transform
Fourier_series
Discrete-time_Fourier_transform
Discrete_Fourier_transform
Discrete_Fourier_transform_over_a_ring
Fourier_analysis
Related_transforms
Linear operations performed in one domain (time or frequency) have
corresponding operations in the other domain, which are sometimes easier to
perform. The operation of differentiation in the time domain corresponds to
multiplication by the frequency,[remark_1] so some differential_equations are
easier to analyze in the frequency domain. Also, convolution in the time domain
corresponds to ordinary multiplication in the frequency domain (see Convolution
theorem). After performing the desired operations, transformation of the result
can be made back to the time domain. Harmonic_analysis is the systematic study
of the relationship between the frequency and time domains, including the kinds
of functions or operations that are "simpler" in one or the other, and has deep
connections to many areas of modern mathematics.
Functions that are localized in the time domain have Fourier transforms that
are spread out across the frequency domain and vice versa, a phenomenon known
as the uncertainty_principle. The critical case for this principle is the
Gaussian_function, of substantial importance in probability_theory and
statistics as well as in the study of physical phenomena exhibiting normal
distribution (e.g., diffusion). The Fourier transform of a Gaussian function is
another Gaussian function. Joseph_Fourier introduced the transform in his study
of heat_transfer, where Gaussian functions appear as solutions of the heat
equation.
The Fourier transform can be formally defined as an improper Riemann_integral,
making it an integral_transform, although this definition is not suitable for
many applications requiring a more sophisticated integration theory.[remark_2]
For example, many relatively simple applications use the Dirac_delta_function,
which can be treated formally as if it were a function, but the justification
requires a mathematically more sophisticated viewpoint.[remark_3] The Fourier
transform can also be generalized to functions of several variables on
Euclidean space, sending a function of 3-dimensional 'position space' to a
function of 3-dimensional momentum (or a function of space and time to a
function of 4-momentum). This idea makes the spatial Fourier transform very
natural in the study of waves, as well as in quantum_mechanics, where it is
important to be able to represent wave solutions as functions of either
position or momentum and sometimes both. In general, functions to which Fourier
methods are applicable are complex-valued, and possibly vector-valued.[remark
4] Still further generalization is possible to functions on groups, which,
besides the original Fourier transform on â or ân (viewed as groups under
addition), notably includes the discrete-time_Fourier_transform (DTFT, group =
â¤), the discrete_Fourier_transform (DFT, group = â¤_mod_N) and the Fourier
series or circular Fourier transform (group = S1, the unit circle â closed
finite interval with endpoints identified). The latter is routinely employed to
handle periodic_functions. The fast_Fourier_transform (FFT) is an algorithm for
computing the DFT.
⁰
***** Contents *****
    * 1_Definition
    * 2_History
    * 3_Introduction
    * 4_Example
    * 5_Properties_of_the_Fourier_transform
          o 5.1_Basic_properties
                # 5.1.1_Linearity
                # 5.1.2_Translation_/_time_shifting
                # 5.1.3_Modulation_/_frequency_shifting
                # 5.1.4_Time_scaling
                # 5.1.5_Conjugation
                # 5.1.6_Real_and_imaginary_part_in_time
                # 5.1.7_Integration
          o 5.2_Invertibility_and_periodicity
          o 5.3_Units_and_duality
          o 5.4_Uniform_continuity_and_the_RiemannâLebesgue_lemma
          o 5.5_Plancherel_theorem_and_Parseval's_theorem
          o 5.6_Poisson_summation_formula
          o 5.7_Differentiation
          o 5.8_Convolution_theorem
          o 5.9_Cross-correlation_theorem
          o 5.10_Eigenfunctions
          o 5.11_Connection_with_the_Heisenberg_group
    * 6_Complex_domain
          o 6.1_Laplace_transform
          o 6.2_Inversion
    * 7_Fourier_transform_on_Euclidean_space
          o 7.1_Uncertainty_principle
          o 7.2_Sine_and_cosine_transforms
          o 7.3_Spherical_harmonics
          o 7.4_Restriction_problems
    * 8_Fourier_transform_on_function_spaces
          o 8.1_On_Lp_spaces
                # 8.1.1_On_L1
                # 8.1.2_On_L2
                # 8.1.3_On_other_Lp
          o 8.2_Tempered_distributions
    * 9_Generalizations
          o 9.1_FourierâStieltjes_transform
          o 9.2_Locally_compact_abelian_groups
          o 9.3_Gelfand_transform
          o 9.4_Compact_non-abelian_groups
    * 10_Alternatives
    * 11_Applications
          o 11.1_Analysis_of_differential_equations
          o 11.2_Fourier_transform_spectroscopy
          o 11.3_Quantum_mechanics
          o 11.4_Signal_processing
    * 12_Other_notations
    * 13_Other_conventions
    * 14_Computation_methods
          o 14.1_Numerical_integration_of_closed-form_functions
          o 14.2_Numerical_integration_of_a_series_of_ordered_pairs
          o 14.3_Discrete_Fourier_transforms_and_fast_Fourier_transforms
    * 15_Tables_of_important_Fourier_transforms
          o 15.1_Functional_relationships,_one-dimensional
          o 15.2_Square-integrable_functions,_one-dimensional
          o 15.3_Distributions,_one-dimensional
          o 15.4_Two-dimensional_functions
          o 15.5_Formulas_for_general_n-dimensional_functions
    * 16_See_also
    * 17_Remarks
    * 18_Notes
    * 19_References
    * 20_External_links
***** Definition[edit] *****
The Fourier transform of a function f is traditionally denoted        f
&#x005E;      {\displaystyle {\hat {f}}}  [{\hat {f}}], by adding a circumflex
to the symbol of the function. There are several common_conventions for
defining the Fourier transform of an integrable function     f :  R  &#x2192;
C    {\displaystyle f:\mathbb {R} \to \mathbb {C} }  [{\displaystyle f:\mathbb
{R} \to \mathbb {C} }].[1][2] One of them is
      f &#x005E;    ( &#x03BE; ) =  &#x222B;  &#x2212; &#x221E;
&#x221E;   f ( x ) &#xA0;  e  &#x2212; 2 &#x03C0; i x &#x03BE;      
d x ,   {\displaystyle {\hat {f}}(\xi )=\int _{-\infty }^{\infty      (Eq.1)
}f(x)\ e^{-2\pi ix\xi }\,dx,}  [{\displaystyle {\hat {f}}(\xi
)=\int _{-\infty }^{\infty }f(x)\ e^{-2\pi ix\xi }\,dx,}]
for any real_number Î¾.
A reason for the negative sign in the exponent is that it is common in
electrical_engineering to represent by     f ( x ) =  e  2 &#x03C0; i  &#x03BE;
0   x     {\displaystyle f(x)=e^{2\pi i\xi _{0}x}}  [{\displaystyle f(x)=e^
{2\pi i\xi _{0}x}}] a signal with zero initial phase and frequency
&#x03BE;  0   .   {\displaystyle \xi _{0}.}  [{\displaystyle \xi _{0}.}][3]
[remark_5] The negative sign convention causes the product      e  2 &#x03C0; i
&#x03BE;  0   x    e  &#x2212; 2 &#x03C0; i &#x03BE; x     {\displaystyle e^
{2\pi i\xi _{0}x}e^{-2\pi i\xi x}}  [{\displaystyle e^{2\pi i\xi _{0}x}e^{-2\pi
i\xi x}}] to be 1 (frequency zero) when     &#x03BE; =  &#x03BE;  0   ,
{\displaystyle \xi =\xi _{0},}  [{\displaystyle \xi =\xi _{0},}] causing the
integral to diverge. The result is a Dirac_delta_function at     &#x03BE; =
&#x03BE;  0     {\displaystyle \xi =\xi _{0}}  [{\displaystyle \xi =\xi _{0}}],
which is the only frequency component of the sinusoidal signal      e  2
&#x03C0; i  &#x03BE;  0   x   .   {\displaystyle e^{2\pi i\xi _{0}x}.}  [
{\displaystyle e^{2\pi i\xi _{0}x}.}]
When the independent variable x represents time, the transform variable Î¾
represents frequency (e.g. if time is measured in seconds, then frequency is in
hertz). Under suitable conditions, f is determined by        f &#x005E;
{\displaystyle {\hat {f}}}  [{\hat {f}}] via the inverse transform:
   f ( x ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;      f
&#x005E;    ( &#x03BE; ) &#xA0;  e  2 &#x03C0; i x &#x03BE;    d     
&#x03BE; ,   {\displaystyle f(x)=\int _{-\infty }^{\infty }{\hat       (Eq.2)
{f}}(\xi )\ e^{2\pi ix\xi }\,d\xi ,}  [{\displaystyle f(x)=\int _
{-\infty }^{\infty }{\hat {f}}(\xi )\ e^{2\pi ix\xi }\,d\xi ,}]
for any real number x.
The statement that f can be reconstructed from        f &#x005E;
{\displaystyle {\hat {f}}}  [{\hat {f}}] is known as the Fourier_inversion
theorem, and was first introduced in Fourier's Analytical Theory of Heat,[4][5]
although what would be considered a proof by modern standards was not given
until much later.[6][7] The functions f and        f &#x005E;
{\displaystyle {\hat {f}}}  [{\hat {f}}] often are referred to as a Fourier
integral pair or Fourier transform pair.[8]
For other common conventions and notations, including using the angular
frequency Ï instead of the frequency Î¾, see Other_conventions and Other
notations below. The Fourier_transform_on_Euclidean_space is treated
separately, in which the variable x often represents position and Î¾ momentum.
The conventions chosen in this article are those of harmonic_analysis, and are
characterized as the unique conventions such that the Fourier transform is both
unitary on L2 and an algebra homomorphism from L1 to Lâ, without
renormalizing the Lebesgue measure.[9]
Many other characterizations of the Fourier transform exist. For example, one
uses the Stoneâvon_Neumann_theorem: the Fourier transform is the unique
unitary intertwiner for the symplectic and Euclidean SchrÃ¶dinger
representations of the Heisenberg_group.
***** History[edit] *****
Main articles: Fourier_analysis_Â§ History, and Fourier_series_Â§ History
In 1822, Joseph_Fourier showed that some functions could be written as an
infinite sum of harmonics.[10]
***** Introduction[edit] *****
See also: Fourier_analysis
In the first frames of the animation, a function f is resolved into Fourier
series: a linear combination of sines and cosines (in blue). The component
frequencies of these sines and cosines spread across the frequency spectrum,
are represented as peaks in the frequency domain (actually Dirac_delta
functions, shown in the last frames of the animation). The frequency domain
representation of the function, fÌ, is the collection of these peaks at the
frequencies that appear in this resolution of the function.
One motivation for the Fourier transform comes from the study of Fourier
series. In the study of Fourier series, complicated but periodic functions are
written as the sum of simple waves mathematically represented by sines and
cosines. The Fourier transform is an extension of the Fourier series that
results when the period of the represented function is lengthened and allowed
to approach infinity.[11]
Due to the properties of sine and cosine, it is possible to recover the
amplitude of each wave in a Fourier series using an integral. In many cases it
is desirable to use Euler's_formula, which states that e2ÏiÎ¸ = cos(2ÏÎ¸) + i
sin(2ÏÎ¸), to write Fourier series in terms of the basic waves e2ÏiÎ¸. This
has the advantage of simplifying many of the formulas involved, and provides a
formulation for Fourier series that more closely resembles the definition
followed in this article. Re-writing sines and cosines as complex_exponentials
makes it necessary for the Fourier coefficients to be complex valued. The usual
interpretation of this complex number is that it gives both the amplitude (or
size) of the wave present in the function and the phase (or the initial angle)
of the wave. These complex exponentials sometimes contain negative
"frequencies". If Î¸ is measured in seconds, then the waves e2ÏiÎ¸ and
eâ2ÏiÎ¸ both complete one cycle per second, but they represent different
frequencies in the Fourier transform. Hence, frequency no longer measures the
number of cycles per unit time, but is still closely related.
There is a close connection between the definition of Fourier series and the
Fourier transform for functions f that are zero outside an interval. For such a
function, we can calculate its Fourier series on any interval that includes the
points where f is not identically zero. The Fourier transform is also defined
for such a function. As we increase the length of the interval in which we
calculate the Fourier series, then the Fourier series coefficients begin to
resemble the Fourier transform and the sum of the Fourier series of f begins to
resemble the inverse Fourier transform. More precisely, suppose T is large
enough that the interval [âT/2, T/2] contains the interval in which f is not
identically zero. Then, the nth series coefficient cn is given by:
          c  n   =   1 T    &#x222B;  &#x2212;   T 2      T 2    f ( x )   e
      &#x2212; 2 &#x03C0; i  (   n T   )  x    d x .   {\displaystyle c_{n}=
      {\frac {1}{T}}\int _{-{\frac {T}{2}}}^{\frac {T}{2}}f(x)\,e^{-2\pi i\left
      ({\frac {n}{T}}\right)x}\,dx.}  [{\displaystyle c_{n}={\frac {1}{T}}\int
      _{-{\frac {T}{2}}}^{\frac {T}{2}}f(x)\,e^{-2\pi i\left({\frac {n}
      {T}}\right)x}\,dx.}]
Comparing this to the definition of the Fourier transform, it follows that:
          c  n   =   1 T      f &#x005E;     (   n T   )    {\displaystyle c_
      {n}={\frac {1}{T}}{\hat {f}}\left({\frac {n}{T}}\right)}  [{\displaystyle
      c_{n}={\frac {1}{T}}{\hat {f}}\left({\frac {n}{T}}\right)}]
since f (x) is zero outside [âT/2, T/2]. Thus, the Fourier coefficients are
equal to the values of the Fourier transform sampled on a grid of width 1/T,
multiplied by the grid width 1/T.
Under appropriate conditions, the Fourier series of f will equal the function
f. In other words, f can be written:
         f ( x ) =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;    c  n     e  2
      &#x03C0; i  (   n T   )  x   =  &#x2211;  n = &#x2212; &#x221E;
      &#x221E;      f &#x005E;    (  &#x03BE;  n   ) &#xA0;  e  2 &#x03C0; i
      &#x03BE;  n   x   &#x0394; &#x03BE; ,   {\displaystyle f(x)=\sum _{n=-
      \infty }^{\infty }c_{n}\,e^{2\pi i\left({\frac {n}{T}}\right)x}=\sum _
      {n=-\infty }^{\infty }{\hat {f}}(\xi _{n})\ e^{2\pi i\xi _{n}x}\Delta \xi
      ,}  [{\displaystyle f(x)=\sum _{n=-\infty }^{\infty }c_{n}\,e^{2\pi
      i\left({\frac {n}{T}}\right)x}=\sum _{n=-\infty }^{\infty }{\hat {f}}(\xi
      _{n})\ e^{2\pi i\xi _{n}x}\Delta \xi ,}]
where the last sum is simply the first sum rewritten using the definitions Î¾n
= n/T, and ÎÎ¾ = n + 1/T â n/T = 1/T.
This second sum is a Riemann_sum. By letting T â â it will converge to the
integral for the inverse Fourier transform as expressed above. Under suitable
conditions, this argument may be made precise.[12]
In the study of Fourier series the numbers cn could be thought of as the
"amount" of the wave present in the Fourier series of f. Similarly, as seen
above, the Fourier transform can be thought of as a function that measures how
much of each individual frequency is present in our function f, and we can
recombine these waves by using an integral (or "continuous sum") to reproduce
the original function.
***** Example[edit] *****
The following figures provide a visual illustration how the Fourier transform
measures whether a frequency is present in a particular function. The depicted
function f (t) = cos(6Ït) eâÏt2 oscillates at 3 Hz (if t measures seconds)
and tends quickly to 0. (The second factor in this equation is an envelope
function that shapes the continuous sinusoid into a short pulse. Its general
form is a Gaussian_function). This function was specially chosen to have a real
Fourier transform that can be easily plotted. The first image contains its
graph. In order to calculate fÌ (3) we must integrate eâ2Ïi(3t)f (t). The
second image shows the plot of the real and imaginary parts of this function.
The real part of the integrand is almost always positive, because when f (t) is
negative, the real part of eâ2Ïi(3t) is negative as well. Because they
oscillate at the same rate, when f (t) is positive, so is the real part of
eâ2Ïi(3t). The result is that when you integrate the real part of the
integrand you get a relatively large number (in this case 1/2). On the other
hand, when you try to measure a frequency that is not present, as in the case
when we look at fÌ (5), you see that both real and imaginary component of this
function vary rapidly between positive and negative values, as plotted in the
third image. Therefore, in this case, the integrand oscillates fast enough so
that the integral is very small and the value for the Fourier transform for
that frequency is nearly zero.
The general situation may be a bit more complicated than this, but this in
spirit is how the Fourier transform measures how much of an individual
frequency is present in a function f (t).
    * Original function showing oscillation 3 Hz.
    * Real and imaginary parts of integrand for Fourier transform at 3 Hz
    * Real and imaginary parts of integrand for Fourier transform at 5 Hz
    * Magnitude of Fourier transform, with 3 and 5 Hz labeled.
***** Properties of the Fourier transform[edit] *****
Here we assume f (x), g(x) and h(x) are integrable functions: Lebesgue-
measurable on the real line satisfying:
          &#x222B;  &#x2212; &#x221E;   &#x221E;    |  f ( x )  |   d x <
      &#x221E; .   {\displaystyle \int _{-\infty }^{\infty }|f(x)|\,dx<\infty
      .}  [\int _{-\infty }^{\infty }|f(x)|\,dx<\infty .]
We denote the Fourier transforms of these functions as fÌ (Î¾), Ä(Î¾) and Ä¥
(Î¾) respectively.
**** Basic properties[edit] ****
The Fourier transform has the following basic properties:[13]
*** Linearity[edit] ***
      For any complex_numbers a and b, if h(x) = af (x) + bg(x), then Ä¥(Î¾) =
      a Â· fÌ (Î¾) + b Â· Ä(Î¾).
*** Translation / time shifting[edit] ***
Animation showing the Fourier Transform of a time shifted signal. [Top] the
original signal (orange), is continuously time shifted (blue). [Bottom] The
resultant Fourier Transform of the time shifted signal. Note how the higher
frequency components revolve in complex plane faster than the lower frequency
components
      For any real_number x0, if h(x) = f (x â x0), then Ä¥(Î¾) =
      eâ2Ïix0Î¾ fÌ (Î¾).
*** Modulation / frequency shifting[edit] ***
      For any real_number Î¾0, if h(x) = e2ÏixÎ¾0 f (x), then Ä¥(Î¾) = fÌ (Î¾
      â Î¾0).
*** Time scaling[edit] ***
      For a non-zero real_number a, if h(x) = f (ax), then
                  h &#x005E;    ( &#x03BE; ) =   1   |  a  |        f &#x005E;
            (   &#x03BE; a   )  .   {\displaystyle {\hat {h}}(\xi )={\frac {1}
            {|a|}}{\hat {f}}\left({\frac {\xi }{a}}\right).}  [{\hat {h}}(\xi
            )={\frac {1}{|a|}}{\hat {f}}\left({\frac {\xi }{a}}\right).]
      The case a = â1 leads to the time-reversal property, which states: if h
      (x) = f (âx), then Ä¥(Î¾) = fÌ (âÎ¾).
*** Conjugation[edit] ***
      If h(x) = f (x), then
                  h &#x005E;    ( &#x03BE; ) =       f &#x005E;    ( &#x2212;
            &#x03BE; )  &#x00AF;   .   {\displaystyle {\hat {h}}(\xi )=
            {\overline {{\hat {f}}(-\xi )}}.}  [{\hat {h}}(\xi )={\overline {
            {\hat {f}}(-\xi )}}.]
      In particular, if f is real, then one has the reality condition
                  f &#x005E;    ( &#x2212; &#x03BE; ) =       f &#x005E;
            ( &#x03BE; )  &#x00AF;   ,   {\displaystyle {\hat {f}}(-\xi )=
            {\overline {{\hat {f}}(\xi )}},}  [{\displaystyle {\hat {f}}(-\xi
            )={\overline {{\hat {f}}(\xi )}},}]
      that is, fÌ is a Hermitian_function. And if f is purely imaginary, then
                  f &#x005E;    ( &#x2212; &#x03BE; ) = &#x2212;       f
            &#x005E;    ( &#x03BE; )  &#x00AF;   .   {\displaystyle {\hat {f}}
            (-\xi )=-{\overline {{\hat {f}}(\xi )}}.}  [{\hat {f}}(-\xi )=-
            {\overline {{\hat {f}}(\xi )}}.]
*** Real and imaginary part in time[edit] ***
    * If     h ( x ) = &#x211C;  ( f ( x ) )    {\displaystyle h(x)=\Re {(f
      (x))}}  [{\displaystyle h(x)=\Re {(f(x))}}], then        h &#x005E;
      ( &#x03BE; ) =   1 2   (    f &#x005E;    ( &#x03BE; ) +       f &#x005E;
      ( &#x2212; &#x03BE; )  &#x00AF;   )   {\displaystyle {\hat {h}}(\xi )=
      {\frac {1}{2}}({\hat {f}}(\xi )+{\overline {{\hat {f}}(-\xi )}})}  [
      {\displaystyle {\hat {h}}(\xi )={\frac {1}{2}}({\hat {f}}(\xi )+
      {\overline {{\hat {f}}(-\xi )}})}].
    * If     h ( x ) = &#x2111;  ( f ( x ) )    {\displaystyle h(x)=\Im {(f
      (x))}}  [{\displaystyle h(x)=\Im {(f(x))}}], then        h &#x005E;
      ( &#x03BE; ) =   1  2 i    (    f &#x005E;    ( &#x03BE; ) &#x2212;
      f &#x005E;    ( &#x2212; &#x03BE; )  &#x00AF;   )   {\displaystyle {\hat
      {h}}(\xi )={\frac {1}{2i}}({\hat {f}}(\xi )-{\overline {{\hat {f}}(-\xi
      )}})}  [{\displaystyle {\hat {h}}(\xi )={\frac {1}{2i}}({\hat {f}}(\xi )-
      {\overline {{\hat {f}}(-\xi )}})}].
*** Integration[edit] ***
      Substituting Î¾ = 0 in the definition, we obtain
                  f &#x005E;    ( 0 ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;
            f ( x )  d x .   {\displaystyle {\hat {f}}(0)=\int _{-\infty }^
            {\infty }f(x)\,dx.}  [{\hat {f}}(0)=\int _{-\infty }^{\infty }f
            (x)\,dx.]
      That is, the evaluation of the Fourier transform at the origin (Î¾ = 0)
      equals the integral of f over all its domain.
**** Invertibility and periodicity[edit] ****
Further information: Fourier_inversion_theorem and Fractional_Fourier_transform
Under suitable conditions on the function f, it can be recovered from its
Fourier transform        f &#x005E;      {\displaystyle {\hat {f}}}  [{\hat
{f}}]. Indeed, denoting the Fourier transform operator by F, so F( f ) := fÌ,
then for suitable functions, applying the Fourier transform twice simply flips
the function: F2( f )(x) = f (âx), which can be interpreted as "reversing
time". Since reversing time is two-periodic, applying this twice yields F4( f )
= f, so the Fourier transform operator is four-periodic, and similarly the
inverse Fourier transform can be obtained by applying the Fourier transform
three times: F3( fÌ ) = f. In particular the Fourier transform is invertible
(under suitable conditions).
More precisely, defining the parity operator P that inverts time, P[ f ] : t
â¦ f (ât):
                F    0      =  I d  ,     F    1   =   F   ,        F    2
      =   P   ,     F    4   =  I d  ,        F    3      =    F    &#x2212; 1
      =   P   &#x2218;   F   =   F   &#x2218;   P         {\displaystyle
      {\begin{aligned}{\mathcal {F}}^{0}&=\mathrm {Id} ,\quad {\mathcal {F}}^
      {1}={\mathcal {F}},\\{\mathcal {F}}^{2}&={\mathcal {P}},\quad {\mathcal
      {F}}^{4}=\mathrm {Id} ,\\{\mathcal {F}}^{3}&={\mathcal {F}}^{-1}=
      {\mathcal {P}}\circ {\mathcal {F}}={\mathcal {F}}\circ {\mathcal {P}}\end
      {aligned}}}  [{\displaystyle {\begin{aligned}{\mathcal {F}}^{0}&=\mathrm
      {Id} ,\quad {\mathcal {F}}^{1}={\mathcal {F}},\\{\mathcal {F}}^{2}&=
      {\mathcal {P}},\quad {\mathcal {F}}^{4}=\mathrm {Id} ,\\{\mathcal {F}}^
      {3}&={\mathcal {F}}^{-1}={\mathcal {P}}\circ {\mathcal {F}}={\mathcal
      {F}}\circ {\mathcal {P}}\end{aligned}}}]
These equalities of operators require careful definition of the space of
functions in question, defining equality of functions (equality at every point?
equality almost_everywhere?) and defining equality of operators â that is,
defining the topology on the function space and operator space in question.
These are not true for all functions, but are true under various conditions,
which are the content of the various forms of the Fourier_inversion_theorem.
This fourfold periodicity of the Fourier transform is similar to a rotation of
the plane by 90Â°, particularly as the two-fold iteration yields a reversal,
and in fact this analogy can be made precise. While the Fourier transform can
simply be interpreted as switching the time domain and the frequency domain,
with the inverse Fourier transform switching them back, more geometrically it
can be interpreted as a rotation by 90Â° in the timeâfrequency_domain
(considering time as the x-axis and frequency as the y-axis), and the Fourier
transform can be generalized to the fractional_Fourier_transform, which
involves rotations by other angles. This can be further generalized to linear
canonical_transformations, which can be visualized as the action of the special
linear_group SL2(â) on the timeâfrequency plane, with the preserved
symplectic form corresponding to the uncertainty_principle, below. This
approach is particularly studied in signal_processing, under timeâfrequency
analysis.
**** Units and duality[edit] ****
In mathematics, one often does not think of any units as being attached to the
two variables t and Î¾. But in physical applications, Î¾ must have inverse
units to the units of t. For example, if t is measured in seconds, Î¾ should be
in cycles per second for the formulas here to be valid. If the scale of t is
changed and t is measured in units of 2Ï seconds, then either Î¾ must be in
the so-called "angular_frequency", or one must insert some constant scale
factor into some of the formulas. If t is measured in units of length, then Î¾
must be in inverse length, e.g., wavenumbers. That is to say, there are two
copies of the real line: one measured in one set of units, where t ranges, and
the other in inverse units to the units of t, and which is the range of Î¾. So
these are two distinct copies of the real line, and cannot be identified with
each other. Therefore, the Fourier transform goes from one space of functions
to a different space of functions: functions which have a different domain of
definition.
In general, Î¾ must always be taken to be a linear_form on the space of ts,
which is to say that the second real line is the dual space of the first real
line. See the article on linear_algebra for a more formal explanation and for
more details. This point of view becomes essential in generalisations of the
Fourier transform to general symmetry groups, including the case of Fourier
series.
That there is no one preferred way (often, one says "no canonical way") to
compare the two copies of the real line which are involved in the Fourier
transformâfixing the units on one line does not force the scale of the units
on the other lineâis the reason for the plethora of rival conventions on the
definition of the Fourier transform. The various definitions resulting from
different choices of units differ by various constants. If the units of t are
in seconds but the units of Î¾ are in angular frequency, then the angular
frequency variable is often denoted by one or another Greek letter, for
example, Ï = 2ÏÎ¾ is quite common. Thus (writing xÌ1 for the alternative
definition and xÌ for the definition adopted in this article)
             x &#x005E;     1   ( &#x03C9; ) =    x &#x005E;     (   &#x03C9;
      2 &#x03C0;    )  =  &#x222B;  &#x2212; &#x221E;   &#x221E;   x ( t )  e
      &#x2212; i &#x03C9; t    d t   {\displaystyle {\hat {x}}_{1}(\omega )=
      {\hat {x}}\left({\frac {\omega }{2\pi }}\right)=\int _{-\infty }^{\infty
      }x(t)e^{-i\omega t}\,dt}  [{\displaystyle {\hat {x}}_{1}(\omega )={\hat
      {x}}\left({\frac {\omega }{2\pi }}\right)=\int _{-\infty }^{\infty }x
      (t)e^{-i\omega t}\,dt}]
as before, but the corresponding alternative inversion formula would then have
to be
         x ( t ) =   1  2 &#x03C0;     &#x222B;  &#x2212; &#x221E;   &#x221E;
      x &#x005E;     1   ( &#x03C9; )  e  i t &#x03C9;    d &#x03C9; .
      {\displaystyle x(t)={\frac {1}{2\pi }}\int _{-\infty }^{\infty }{\hat
      {x}}_{1}(\omega )e^{it\omega }\,d\omega .}  [{\displaystyle x(t)={\frac
      {1}{2\pi }}\int _{-\infty }^{\infty }{\hat {x}}_{1}(\omega )e^{it\omega
      }\,d\omega .}]
To have something involving angular frequency but with greater symmetry between
the Fourier transform and the inversion formula, one very often sees still
another alternative definition of the Fourier transform, with a factor of √2Ï,
thus
             x &#x005E;     2   ( &#x03C9; ) =   1  2 &#x03C0;     &#x222B;
      &#x2212; &#x221E;   &#x221E;   x ( t )  e  &#x2212; i &#x03C9; t    d t ,
      {\displaystyle {\hat {x}}_{2}(\omega )={\frac {1}{\sqrt {2\pi }}}\int _{-
      \infty }^{\infty }x(t)e^{-i\omega t}\,dt,}  [{\hat {x}}_{2}(\omega )=
      {\frac {1}{\sqrt {2\pi }}}\int _{-\infty }^{\infty }x(t)e^{-i\omega
      t}\,dt,]
and the corresponding inversion formula then has to be
         x ( t ) =   1  2 &#x03C0;     &#x222B;  &#x2212; &#x221E;   &#x221E;
      x &#x005E;     2   ( &#x03C9; )  e  i t &#x03C9;    d &#x03C9; .
      {\displaystyle x(t)={\frac {1}{\sqrt {2\pi }}}\int _{-\infty }^{\infty }
      {\hat {x}}_{2}(\omega )e^{it\omega }\,d\omega .}  [{\displaystyle x(t)=
      {\frac {1}{\sqrt {2\pi }}}\int _{-\infty }^{\infty }{\hat {x}}_{2}(\omega
      )e^{it\omega }\,d\omega .}]
In some unusual conventions, such as those employed by the FourierTransform
command of the Wolfram_Language, the Fourier transform has i in the exponent
instead of âi, and vice versa for the inversion formula. Many of the
identities involving the Fourier transform remain valid in those conventions,
provided all terms that explicitly involve i have it replaced by −i.
For example, in probability theory, the characteristic function Ï of the
probability density function f of a random variable X of continuous type is
defined without a negative sign in the exponential, and since the units of x
are ignored, there is no 2Ï either:
         &#x03D5; ( &#x03BB; ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;   f
      ( x )  e  i &#x03BB; x    d x .   {\displaystyle \phi (\lambda )=\int _{-
      \infty }^{\infty }f(x)e^{i\lambda x}\,dx.}  [\phi (\lambda )=\int _{-
      \infty }^{\infty }f(x)e^{i\lambda x}\,dx.]
(In probability theory, and in mathematical statistics, the use of the
FourierâStieltjes transform is preferred, because so many random variables
are not of continuous type, and do not possess a density function, and one must
treat discontinuous distribution functions, i.e., measures which possess
"atoms".)
From the higher point of view of group characters, which is much more abstract,
all these arbitrary choices disappear, as will be explained in the later
section of this article, on the notion of the Fourier transform of a function
on an Abelian locally compact group.
**** Uniform continuity and the RiemannâLebesgue lemma[edit] ****
The rectangular_function is Lebesgue_integrable.
The sinc_function, which is the Fourier transform of the rectangular function,
is bounded and continuous, but not Lebesgue integrable.
The Fourier transform may be defined in some cases for non-integrable
functions, but the Fourier transforms of integrable functions have several
strong properties.
The Fourier transform fÌ of any integrable function f is uniformly_continuous
and[14]
           &#x2016;    f &#x005E;    &#x2016;   &#x221E;   &#x2264;   &#x2016;
      f &#x2016;   1     {\displaystyle \left\|{\hat {f}}\right\|_{\infty }\leq
      \left\|f\right\|_{1}}  [{\displaystyle \left\|{\hat {f}}\right\|_{\infty
      }\leq \left\|f\right\|_{1}}]
By the RiemannâLebesgue_lemma,[15]
            f &#x005E;    ( &#x03BE; ) &#x2192; 0  &#xA0;as&#xA0;   |  &#x03BE;
      |  &#x2192; &#x221E; .   {\displaystyle {\hat {f}}(\xi )\to 0{\text{ as
      }}|\xi |\to \infty .}  [{\displaystyle {\hat {f}}(\xi )\to 0{\text{ as
      }}|\xi |\to \infty .}]
However,        f &#x005E;      {\displaystyle {\hat {f}}}  [{\hat {f}}] need
not be integrable. For example, the Fourier transform of the rectangular
function, which is integrable, is the sinc_function, which is not Lebesgue
integrable, because its improper_integrals behave analogously to the
alternating_harmonic_series, in converging to a sum without being absolutely
convergent.
It is not generally possible to write the inverse transform as a Lebesgue
integral. However, when both f and        f &#x005E;      {\displaystyle {\hat
{f}}}  [{\hat {f}}] are integrable, the inverse equality
         f ( x ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;      f &#x005E;
      ( &#x03BE; )  e  2 i &#x03C0; x &#x03BE;    d &#x03BE;   {\displaystyle f
      (x)=\int _{-\infty }^{\infty }{\hat {f}}(\xi )e^{2i\pi x\xi }\,d\xi }  [f
      (x)=\int _{-\infty }^{\infty }{\hat {f}}(\xi )e^{2i\pi x\xi }\,d\xi ]
holds almost_everywhere. That is, the Fourier transform is injective on L1
(â). (But if f is continuous, then equality holds for every x.)
**** Plancherel theorem and Parseval's theorem[edit] ****
Let f (x) and g(x) be integrable, and let fÌ (Î¾) and Ä(Î¾) be their Fourier
transforms. If f (x) and g(x) are also square-integrable, then the Parseval
formula follows:[16]
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x )    g ( x )  &#x00AF;
      d x =  &#x222B;  &#x2212; &#x221E;   &#x221E;      f &#x005E;
      ( &#x03BE; )       g &#x005E;    ( &#x03BE; )  &#x00AF;    d &#x03BE; ,
      {\displaystyle \int _{-\infty }^{\infty }f(x){\overline {g(x)}}\,dx=\int
      _{-\infty }^{\infty }{\hat {f}}(\xi ){\overline {{\hat {g}}(\xi )}}\,d\xi
      ,}  [{\displaystyle \int _{-\infty }^{\infty }f(x){\overline {g
      (x)}}\,dx=\int _{-\infty }^{\infty }{\hat {f}}(\xi ){\overline {{\hat
      {g}}(\xi )}}\,d\xi ,}]
where the bar denotes complex_conjugation.
The Plancherel_theorem, which follows from the above, states that[17]
          &#x222B;  &#x2212; &#x221E;   &#x221E;     |  f ( x )  |   2    d x =
      &#x222B;  &#x2212; &#x221E;   &#x221E;     |     f &#x005E;    ( &#x03BE;
      )  |   2    d &#x03BE; .   {\displaystyle \int _{-\infty }^{\infty
      }\left|f(x)\right|^{2}\,dx=\int _{-\infty }^{\infty }\left|{\hat {f}}(\xi
      )\right|^{2}\,d\xi .}  [\int _{-\infty }^{\infty }\left|f(x)\right|^
      {2}\,dx=\int _{-\infty }^{\infty }\left|{\hat {f}}(\xi )\right|^{2}\,d\xi
      .]
Plancherel's theorem makes it possible to extend the Fourier transform, by a
continuity argument, to a unitary_operator on L2(â). On L1(â) â© L2(â),
this extension agrees with original Fourier transform defined on L1(â), thus
enlarging the domain of the Fourier transform to L1(â) + L2(â) (and
consequently to Lp(â) for 1 â¤ p â¤ 2). Plancherel's theorem has the
interpretation in the sciences that the Fourier transform preserves the energy
of the original quantity. The terminology of these formulas is not quite
standardised. Parseval's theorem was proved only for Fourier series, and was
first proved by Lyapunov. But Parseval's formula makes sense for the Fourier
transform as well, and so even though in the context of the Fourier transform
it was proved by Plancherel, it is still often referred to as Parseval's
formula, or Parseval's relation, or even Parseval's theorem.
See Pontryagin_duality for a general formulation of this concept in the context
of locally compact abelian groups.
**** Poisson summation formula[edit] ****
Main article: Poisson_summation_formula
The Poisson summation formula (PSF) is an equation that relates the Fourier
series coefficients of the periodic_summation of a function to values of the
function's continuous Fourier transform. The Poisson summation formula says
that for sufficiently regular functions f,
          &#x2211;  n      f &#x005E;    ( n ) =  &#x2211;  n   f ( n ) .
      {\displaystyle \sum _{n}{\hat {f}}(n)=\sum _{n}f(n).}  [\sum _{n}{\hat
      {f}}(n)=\sum _{n}f(n).]
It has a variety of useful forms that are derived from the basic one by
application of the Fourier transform's scaling and time-shifting properties.
The formula has applications in engineering, physics, and number_theory. The
frequency-domain dual of the standard Poisson summation formula is also called
the discrete-time_Fourier_transform.
Poisson summation is generally associated with the physics of periodic media,
such as heat conduction on a circle. The fundamental solution of the heat
equation on a circle is called a theta_function. It is used in number_theory to
prove the transformation properties of theta functions, which turn out to be a
type of modular_form, and it is connected more generally to the theory of
automorphic_forms where it appears on one side of the Selberg_trace_formula.
**** Differentiation[edit] ****
Suppose f (x) is an absolutely continuous differentiable function, and both f
and its derivative f â² are integrable. Then the Fourier transform of the
derivative is given by
              f &#x2032;    &#x005E;    ( &#x03BE; ) = 2 &#x03C0; i &#x03BE;
      f &#x005E;    ( &#x03BE; ) .   {\displaystyle {\widehat {f'\;}}(\xi
      )=2\pi i\xi {\hat {f}}(\xi ).}  [{\widehat {f'\;}}(\xi )=2\pi i\xi {\hat
      {f}}(\xi ).]
More generally, the Fourier transformation of the nth derivative f(n) is given
by
             f  ( n )   &#x005E;    ( &#x03BE; ) = ( 2 &#x03C0; i &#x03BE;  )
      n      f &#x005E;    ( &#x03BE; ) .   {\displaystyle {\widehat {f^{(n)}}}
      (\xi )=(2\pi i\xi )^{n}{\hat {f}}(\xi ).}  [{\widehat {f^{(n)}}}(\xi )=
      (2\pi i\xi )^{n}{\hat {f}}(\xi ).]
By applying the Fourier transform and using these formulas, some ordinary
differential_equations can be transformed into algebraic equations, which are
much easier to solve. These formulas also give rise to the rule of thumb "f (x)
is smooth if_and_only_if fÌ (Î¾) quickly falls to 0 for |Î¾| â â." By
using the analogous rules for the inverse Fourier transform, one can also say
"f (x) quickly falls to 0 for |x| â â if and only if fÌ (Î¾) is smooth."
**** Convolution theorem[edit] ****
Main article: Convolution_theorem
The Fourier transform translates between convolution and multiplication of
functions. If f (x) and g(x) are integrable functions with Fourier transforms
fÌ (Î¾) and Ä(Î¾) respectively, then the Fourier transform of the convolution
is given by the product of the Fourier transforms fÌ (Î¾) and Ä(Î¾) (under
other conventions for the definition of the Fourier transform a constant factor
may appear).
This means that if:
         h ( x ) = ( f &#x2217; g ) ( x ) =  &#x222B;  &#x2212; &#x221E;
      &#x221E;   f ( y ) g ( x &#x2212; y )  d y ,   {\displaystyle h(x)=(f*g)
      (x)=\int _{-\infty }^{\infty }f(y)g(x-y)\,dy,}  [h(x)=(f*g)(x)=\int _{-
      \infty }^{\infty }f(y)g(x-y)\,dy,]
where â denotes the convolution operation, then:
            h &#x005E;    ( &#x03BE; ) =    f &#x005E;    ( &#x03BE; ) &#x22C5;
      g &#x005E;    ( &#x03BE; ) .   {\displaystyle {\hat {h}}(\xi )={\hat {f}}
      (\xi )\cdot {\hat {g}}(\xi ).}  [{\displaystyle {\hat {h}}(\xi )={\hat
      {f}}(\xi )\cdot {\hat {g}}(\xi ).}]
In linear_time_invariant_(LTI)_system_theory, it is common to interpret g(x) as
the impulse_response of an LTI system with input f (x) and output h(x), since
substituting the unit_impulse for f (x) yields h(x) = g(x). In this case, Ä
(Î¾) represents the frequency_response of the system.
Conversely, if f (x) can be decomposed as the product of two square integrable
functions p(x) and q(x), then the Fourier transform of f (x) is given by the
convolution of the respective Fourier transforms pÌ(Î¾) and qÌ(Î¾).
**** Cross-correlation theorem[edit] ****
Main article: Cross-correlation
In an analogous manner, it can be shown that if h(x) is the cross-correlation
of f (x) and g(x):
         h ( x ) = ( f &#x22C6; g ) ( x ) =  &#x222B;  &#x2212; &#x221E;
      &#x221E;      f ( y )  &#x00AF;   g ( x + y )  d y   {\displaystyle h(x)=
      (f\star g)(x)=\int _{-\infty }^{\infty }{\overline {f(y)}}g(x+y)\,dy}  [
      {\displaystyle h(x)=(f\star g)(x)=\int _{-\infty }^{\infty }{\overline {f
      (y)}}g(x+y)\,dy}]
then the Fourier transform of h(x) is:
            h &#x005E;    ( &#x03BE; ) =       f &#x005E;    ( &#x03BE; )
      &#x00AF;   &#x22C5;    g &#x005E;    ( &#x03BE; ) .   {\displaystyle
      {\hat {h}}(\xi )={\overline {{\hat {f}}(\xi )}}\cdot {\hat {g}}(\xi ).}
      [{\displaystyle {\hat {h}}(\xi )={\overline {{\hat {f}}(\xi )}}\cdot
      {\hat {g}}(\xi ).}]
As a special case, the autocorrelation of function f (x) is:
         h ( x ) = ( f &#x22C6; f ) ( x ) =  &#x222B;  &#x2212; &#x221E;
      &#x221E;      f ( y )  &#x00AF;   f ( x + y )  d y   {\displaystyle h(x)=
      (f\star f)(x)=\int _{-\infty }^{\infty }{\overline {f(y)}}f(x+y)\,dy}  [
      {\displaystyle h(x)=(f\star f)(x)=\int _{-\infty }^{\infty }{\overline {f
      (y)}}f(x+y)\,dy}]
for which
            h &#x005E;    ( &#x03BE; ) =       f &#x005E;    ( &#x03BE; )
      &#x00AF;      f &#x005E;    ( &#x03BE; ) =   |     f &#x005E;
      ( &#x03BE; )  |   2   .   {\displaystyle {\hat {h}}(\xi )={\overline {
      {\hat {f}}(\xi )}}{\hat {f}}(\xi )=\left|{\hat {f}}(\xi )\right|^{2}.}  [
      {\displaystyle {\hat {h}}(\xi )={\overline {{\hat {f}}(\xi )}}{\hat {f}}
      (\xi )=\left|{\hat {f}}(\xi )\right|^{2}.}]
**** Eigenfunctions[edit] ****
One important choice of an orthonormal basis for L2(â) is given by the
Hermite functions
          &#x03C8;  n   ( x ) =    2  4    n !     e  &#x2212; &#x03C0;  x  2
      H e   n    (  2 x   &#x03C0;    )  ,   {\displaystyle \psi _{n}(x)={\frac
      {\sqrt[{4}]{2}}{\sqrt {n!}}}e^{-\pi x^{2}}\mathrm {He} _{n}\left(2x{\sqrt
      {\pi }}\right),}  [{\displaystyle \psi _{n}(x)={\frac {\sqrt[{4}]{2}}
      {\sqrt {n!}}}e^{-\pi x^{2}}\mathrm {He} _{n}\left(2x{\sqrt {\pi
      }}\right),}]
where Hen(x) are the "probabilist's" Hermite_polynomials, defined as
           H e   n   ( x ) = ( &#x2212; 1  )  n    e    x  2   2      (   d  d
      x    )   n    e  &#x2212;    x  2   2       {\displaystyle \mathrm {He} _
      {n}(x)=(-1)^{n}e^{\frac {x^{2}}{2}}\left({\frac {d}{dx}}\right)^{n}e^{-
      {\frac {x^{2}}{2}}}}  [\mathrm {He} _{n}(x)=(-1)^{n}e^{\frac {x^{2}}
      {2}}\left({\frac {d}{dx}}\right)^{n}e^{-{\frac {x^{2}}{2}}}]
Under this convention for the Fourier transform, we have that
             &#x03C8; &#x005E;     n   ( &#x03BE; ) = ( &#x2212; i  )  n
      &#x03C8;  n   ( &#x03BE; )   {\displaystyle {\hat {\psi }}_{n}(\xi )=(-
      i)^{n}\psi _{n}(\xi )}  [{\displaystyle {\hat {\psi }}_{n}(\xi )=(-i)^
      {n}\psi _{n}(\xi )}].
In other words, the Hermite functions form a complete orthonormal system of
eigenfunctions for the Fourier transform on L2(â).[13] However, this choice
of eigenfunctions is not unique. There are only four different eigenvalues of
the Fourier transform (Â±1 and Â±i) and any linear combination of
eigenfunctions with the same eigenvalue gives another eigenfunction. As a
consequence of this, it is possible to decompose L2(â) as a direct sum of
four spaces H0, H1, H2, and H3 where the Fourier transform acts on Hek simply
by multiplication by ik.
Since the complete set of Hermite functions provides a resolution of the
identity, the Fourier transform can be represented by such a sum of terms
weighted by the above eigenvalues, and these sums can be explicitly summed.
This approach to define the Fourier transform was first done by Norbert_Wiener.
[18] Among other properties, Hermite functions decrease exponentially fast in
both frequency and time domains, and they are thus used to define a
generalization of the Fourier transform, namely the fractional_Fourier
transform used in time-frequency analysis.[19] In physics, this transform was
introduced by Edward_Condon.[20]
**** Connection with the Heisenberg group[edit] ****
The Heisenberg_group is a certain group of unitary_operators on the Hilbert
space L2(â) of square integrable complex valued functions f on the real line,
generated by the translations (Ty f )(x) = f (x + y) and multiplication by
e2ÏixÎ¾, (MÎ¾ f )(x) = e2ÏixÎ¾ f (x). These operators do not commute, as
their (group) commutator is
          (   M  &#x03BE;   &#x2212; 1    T  y   &#x2212; 1    M  &#x03BE;    T
      y   f  )  ( x ) =  e  2 &#x03C0; i y &#x03BE;   f ( x )   {\displaystyle
      \left(M_{\xi }^{-1}T_{y}^{-1}M_{\xi }T_{y}f\right)(x)=e^{2\pi iy\xi }f
      (x)}  [{\displaystyle \left(M_{\xi }^{-1}T_{y}^{-1}M_{\xi }T_{y}f\right)
      (x)=e^{2\pi iy\xi }f(x)}]
which is multiplication by the constant (independent of x) e2ÏiyÎ¾ â U(1)
(the circle_group of unit modulus complex numbers). As an abstract group, the
Heisenberg group is the three-dimensional Lie_group of triples (x, Î¾, z) â
â2 Ã U(1), with the group law
          (   x  1   ,  &#x03BE;  1   ,  t  1    )  &#x22C5;  (   x  2   ,
      &#x03BE;  2   ,  t  2    )  =  (   x  1   +  x  2   ,  &#x03BE;  1   +
      &#x03BE;  2   ,  t  1    t  2    e  2 &#x03C0; i  (   x  1    &#x03BE;  1
      +  x  2    &#x03BE;  2   +  x  1    &#x03BE;  2    )     )  .
      {\displaystyle \left(x_{1},\xi _{1},t_{1}\right)\cdot \left(x_{2},\xi _
      {2},t_{2}\right)=\left(x_{1}+x_{2},\xi _{1}+\xi _{2},t_{1}t_{2}e^{2\pi
      i\left(x_{1}\xi _{1}+x_{2}\xi _{2}+x_{1}\xi _{2}\right)}\right).}  [
      {\displaystyle \left(x_{1},\xi _{1},t_{1}\right)\cdot \left(x_{2},\xi _
      {2},t_{2}\right)=\left(x_{1}+x_{2},\xi _{1}+\xi _{2},t_{1}t_{2}e^{2\pi
      i\left(x_{1}\xi _{1}+x_{2}\xi _{2}+x_{1}\xi _{2}\right)}\right).}]
Denote the Heisenberg group by H1. The above procedure describes not only the
group structure, but also a standard unitary_representation of H1 on a Hilbert
space, which we denote by Ï : H1 â B(L2(â)). Define the linear
automorphism of â2 by
         J   (    x     &#x03BE;    )   =   (    &#x2212; &#x03BE;     x    )
      {\displaystyle J{\begin{pmatrix}x\\\xi \end{pmatrix}}={\begin{pmatrix}-
      \xi \\x\end{pmatrix}}}  [{\displaystyle J{\begin{pmatrix}x\\\xi \end
      {pmatrix}}={\begin{pmatrix}-\xi \\x\end{pmatrix}}}]
so that J2 = âI. This J can be extended to a unique automorphism of H1:
         j  (  x , &#x03BE; , t  )  =  (  &#x2212; &#x03BE; , x , t  e
      &#x2212; 2 &#x03C0; i x &#x03BE;    )  .   {\displaystyle j\left(x,\xi
      ,t\right)=\left(-\xi ,x,te^{-2\pi ix\xi }\right).}  [{\displaystyle
      j\left(x,\xi ,t\right)=\left(-\xi ,x,te^{-2\pi ix\xi }\right).}]
According to the Stoneâvon_Neumann_theorem, the unitary representations Ï
and Ï â j are unitarily equivalent, so there is a unique intertwiner W â U
(L2(â)) such that
         &#x03C1; &#x2218; j = W &#x03C1;  W  &#x2217;   .   {\displaystyle
      \rho \circ j=W\rho W^{*}.}  [{\displaystyle \rho \circ j=W\rho W^{*}.}]
This operator W is the Fourier transform.
Many of the standard properties of the Fourier transform are immediate
consequences of this more general framework.[21] For example, the square of the
Fourier transform, W2, is an intertwiner associated with J2 = âI, and so we
have (W2f )(x) = f (âx) is the reflection of the original function f.
***** Complex domain[edit] *****
The integral for the Fourier transform
            f &#x005E;    ( &#x03BE; ) =  &#x222B;  &#x2212; &#x221E;
      &#x221E;    e  &#x2212; 2 &#x03C0; i &#x03BE; t   f ( t )  d t
      {\displaystyle {\hat {f}}(\xi )=\int _{-\infty }^{\infty }e^{-2\pi i\xi
      t}f(t)\,dt}  [{\displaystyle {\hat {f}}(\xi )=\int _{-\infty }^{\infty
      }e^{-2\pi i\xi t}f(t)\,dt}]
can be studied for complex values of its argument Î¾. Depending on the
properties of f, this might not converge off the real axis at all, or it might
converge to a complex analytic_function for all values of Î¾ = Ï + iÏ, or
something in between.[22]
The PaleyâWiener_theorem says that f is smooth (i.e., n-times differentiable
for all positive integers n) and compactly supported if and only if fÌ (Ï +
iÏ) is a holomorphic_function for which there exists a constant a > 0 such
that for any integer n â¥ 0,
          |   &#x03BE;  n      f &#x005E;    ( &#x03BE; )  |  &#x2264; C  e  a
      | &#x03C4; |     {\displaystyle \left\vert \xi ^{n}{\hat {f}}(\xi
      )\right\vert \leq Ce^{a\vert \tau \vert }}  [{\displaystyle \left\vert
      \xi ^{n}{\hat {f}}(\xi )\right\vert \leq Ce^{a\vert \tau \vert }}]
for some constant C. (In this case, f is supported on [âa, a].) This can be
expressed by saying that fÌ is an entire_function which is rapidly_decreasing
in Ï (for fixed Ï) and of exponential growth in Ï (uniformly in Ï).[23]
(If f is not smooth, but only L2, the statement still holds provided n = 0.
[24]) The space of such functions of a complex_variable is called the
PaleyâWiener space. This theorem has been generalised to semisimple Lie
groups.[25]
If f is supported on the half-line t â¥ 0, then f is said to be "causal"
because the impulse_response_function of a physically realisable filter must
have this property, as no effect can precede its cause. Paley and Wiener showed
that then fÌ extends to a holomorphic_function on the complex lower half-plane
Ï < 0 which tends to zero as Ï goes to infinity.[26] The converse is false
and it is not known how to characterise the Fourier transform of a causal
function.[27]
**** Laplace transform[edit] ****
The Fourier transform fÌ (Î¾) is related to the Laplace_transform F(s), which
is also used for the solution of differential_equations and the analysis of
filters.
It may happen that a function f for which the Fourier integral does not
converge on the real axis at all, nevertheless has a complex Fourier transform
defined in some region of the complex_plane.
For example, if f (t) is of exponential growth, i.e.,
         | f ( t ) | < C  e  a | t |     {\displaystyle \vert f(t)\vert <Ce^
      {a\vert t\vert }}  [\vert f(t)\vert <Ce^{a\vert t\vert }]
for some constants C, a â¥ 0, then[28]
            f &#x005E;    ( i &#x03C4; ) =  &#x222B;  &#x2212; &#x221E;
      &#x221E;    e  2 &#x03C0; &#x03C4; t   f ( t )  d t ,   {\displaystyle
      {\hat {f}}(i\tau )=\int _{-\infty }^{\infty }e^{2\pi \tau t}f(t)\,dt,}  [
      {\displaystyle {\hat {f}}(i\tau )=\int _{-\infty }^{\infty }e^{2\pi \tau
      t}f(t)\,dt,}]
convergent for all 2ÏÏ < âa, is the two-sided_Laplace_transform of f.
The more usual version ("one-sided") of the Laplace transform is
         F ( s ) =  &#x222B;  0   &#x221E;   f ( t )  e  &#x2212; s t    d t .
      {\displaystyle F(s)=\int _{0}^{\infty }f(t)e^{-st}\,dt.}  [{\displaystyle
      F(s)=\int _{0}^{\infty }f(t)e^{-st}\,dt.}]
If f is also causal, then
            f &#x005E;    ( i &#x03C4; ) = F ( &#x2212; 2 &#x03C0; &#x03C4; ) .
      {\displaystyle {\hat {f}}(i\tau )=F(-2\pi \tau ).}  [{\hat {f}}(i\tau )=F
      (-2\pi \tau ).]
Thus, extending the Fourier transform to the complex domain means it includes
the Laplace transform as a special caseâthe case of causal functionsâbut
with the change of variable s = 2ÏiÎ¾.
**** Inversion[edit] ****
If fÌ is complex analytic for a â¤ Ï â¤ b, then
          &#x222B;  &#x2212; &#x221E;   &#x221E;      f &#x005E;    ( &#x03C3;
      + i a )  e  2 &#x03C0; i &#x03BE; t    d &#x03C3; =  &#x222B;  &#x2212;
      &#x221E;   &#x221E;      f &#x005E;    ( &#x03C3; + i b )  e  2 &#x03C0;
      i &#x03BE; t    d &#x03C3;   {\displaystyle \int _{-\infty }^{\infty }
      {\hat {f}}(\sigma +ia)e^{2\pi i\xi t}\,d\sigma =\int _{-\infty }^{\infty
      }{\hat {f}}(\sigma +ib)e^{2\pi i\xi t}\,d\sigma }  [{\displaystyle \int _
      {-\infty }^{\infty }{\hat {f}}(\sigma +ia)e^{2\pi i\xi t}\,d\sigma =\int
      _{-\infty }^{\infty }{\hat {f}}(\sigma +ib)e^{2\pi i\xi t}\,d\sigma }]
by Cauchy's_integral_theorem. Therefore, the Fourier inversion formula can use
integration along different lines, parallel to the real axis.[29]
Theorem: If f (t) = 0 for t < 0, and |f (t)| < Cea|t| for some constants C, a >
0, then
         f ( t ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;      f &#x005E;
      ( &#x03C3; + i &#x03C4; )  e  2 &#x03C0; i &#x03BE; t    d &#x03C3; ,
      {\displaystyle f(t)=\int _{-\infty }^{\infty }{\hat {f}}(\sigma +i\tau
      )e^{2\pi i\xi t}\,d\sigma ,}  [f(t)=\int _{-\infty }^{\infty }{\hat {f}}
      (\sigma +i\tau )e^{2\pi i\xi t}\,d\sigma ,]
for any Ï < âa/2Ï.
This theorem implies the Mellin_inversion_formula for the Laplace
transformation,[28]
         f ( t ) =   1  2 &#x03C0; i     &#x222B;  b &#x2212; i &#x221E;   b +
      i &#x221E;   F ( s )  e  s t    d s   {\displaystyle f(t)={\frac {1}{2\pi
      i}}\int _{b-i\infty }^{b+i\infty }F(s)e^{st}\,ds}  [{\displaystyle f(t)=
      {\frac {1}{2\pi i}}\int _{b-i\infty }^{b+i\infty }F(s)e^{st}\,ds}]
for any b > a, where F(s) is the Laplace transform of f (t).
The hypotheses can be weakened, as in the results of Carleman and Hunt, to f 
(t) eâat being L1, provided that f is of bounded variation in a closed
neighborhood of t (cf. Dirichlet-Dini_theorem), the value of f at t is taken to
be the arithmetic_mean of the left and right limits, and provided that the
integrals are taken in the sense of Cauchy principal values.[30]
L2 versions of these inversion formulas are also available.[31]
***** Fourier transform on Euclidean space[edit] *****
The Fourier transform can be defined in any arbitrary number of dimensions n.
As with the one-dimensional case, there are many conventions. For an integrable
function f (x), this article takes the definition:
            f &#x005E;    (  &#x03BE;  ) =   F   ( f ) (  &#x03BE;  ) =
      &#x222B;    R   n     f (  x  )  e  &#x2212; 2 &#x03C0; i  x  &#x22C5;
      &#x03BE;     d  x    {\displaystyle {\hat {f}}({\boldsymbol {\xi }})=
      {\mathcal {F}}(f)({\boldsymbol {\xi }})=\int _{\mathbb {R} ^{n}}f(\mathbf
      {x} )e^{-2\pi i\mathbf {x} \cdot {\boldsymbol {\xi }}}\,d\mathbf {x} }  [
      {\hat {f}}({\boldsymbol {\xi }})={\mathcal {F}}(f)({\boldsymbol {\xi
      }})=\int _{\mathbb {R} ^{n}}f(\mathbf {x} )e^{-2\pi i\mathbf {x} \cdot
      {\boldsymbol {\xi }}}\,d\mathbf {x} ]
where x and Î¾ are n-dimensional vectors, and x Â· Î¾ is the dot_product of the
vectors. The dot product is sometimes written as â¨x, Î¾â©.
All of the basic properties listed above hold for the n-dimensional Fourier
transform, as do Plancherel's and Parseval's theorem. When the function is
integrable, the Fourier transform is still uniformly continuous and the
RiemannâLebesgue_lemma holds.[15]
**** Uncertainty principle[edit] ****
Further information: Gabor_limit
Generally speaking, the more concentrated f (x) is, the more spread out its
Fourier transform fÌ (Î¾) must be. In particular, the scaling property of the
Fourier transform may be seen as saying: if we squeeze a function in x, its
Fourier transform stretches out in Î¾. It is not possible to arbitrarily
concentrate both a function and its Fourier transform.
The trade-off between the compaction of a function and its Fourier transform
can be formalized in the form of an uncertainty_principle by viewing a function
and its Fourier transform as conjugate_variables with respect to the symplectic
form on the timeâfrequency_domain: from the point of view of the linear
canonical_transformation, the Fourier transform is rotation by 90Â° in the
timeâfrequency domain, and preserves the symplectic_form.
Suppose f (x) is an integrable and square-integrable function. Without loss of
generality, assume that f (x) is normalized:
          &#x222B;  &#x2212; &#x221E;   &#x221E;    |  f ( x )   |   2    d x =
      1.   {\displaystyle \int _{-\infty }^{\infty }|f(x)|^{2}\,dx=1.}  [\int _
      {-\infty }^{\infty }|f(x)|^{2}\,dx=1.]
It follows from the Plancherel_theorem that fÌ (Î¾) is also normalized.
The spread around x = 0 may be measured by the dispersion about zero[32]
defined by
          D  0   ( f ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;    x  2    |
      f ( x )   |   2    d x .   {\displaystyle D_{0}(f)=\int _{-\infty }^
      {\infty }x^{2}|f(x)|^{2}\,dx.}  [D_{0}(f)=\int _{-\infty }^{\infty }x^
      {2}|f(x)|^{2}\,dx.]
In probability terms, this is the second_moment of |f (x)|2 about zero.
The uncertainty principle states that, if f (x) is absolutely continuous and
the functions xÂ·f (x) and f â²(x) are square integrable, then[13]
          D  0   ( f )  D  0    (    f &#x005E;    )  &#x2265;   1  16
      &#x03C0;  2        {\displaystyle D_{0}(f)D_{0}\left({\hat
      {f}}\right)\geq {\frac {1}{16\pi ^{2}}}}  [{\displaystyle D_{0}(f)D_
      {0}\left({\hat {f}}\right)\geq {\frac {1}{16\pi ^{2}}}}].
The equality is attained only in the case
             f ( x )    =  C  1     e  &#x2212; &#x03C0;    x  2    &#x03C3;  2
      &#x2234;    f &#x005E;    ( &#x03BE; )    = &#x03C3;  C  1     e
      &#x2212; &#x03C0;  &#x03C3;  2    &#x03BE;  2           {\displaystyle
      {\begin{aligned}f(x)&=C_{1}\,e^{-\pi {\frac {x^{2}}{\sigma ^
      {2}}}}\\\therefore {\hat {f}}(\xi )&=\sigma C_{1}\,e^{-\pi \sigma ^{2}\xi
      ^{2}}\end{aligned}}}  [{\displaystyle {\begin{aligned}f(x)&=C_{1}\,e^{-
      \pi {\frac {x^{2}}{\sigma ^{2}}}}\\\therefore {\hat {f}}(\xi )&=\sigma C_
      {1}\,e^{-\pi \sigma ^{2}\xi ^{2}}\end{aligned}}}]
where Ï > 0 is arbitrary and C1 = 4√2/√Ï so that f is L2-normalized.[13] In
other words, where f is a (normalized) Gaussian_function with variance Ï2,
centered at zero, and its Fourier transform is a Gaussian function with
variance Ïâ2.
In fact, this inequality implies that:
          (   &#x222B;  &#x2212; &#x221E;   &#x221E;   ( x &#x2212;  x  0    )
      2    |  f ( x )   |   2    d x  )   (   &#x222B;  &#x2212; &#x221E;
      &#x221E;   ( &#x03BE; &#x2212;  &#x03BE;  0    )  2     |     f &#x005E;
      ( &#x03BE; )  |   2    d &#x03BE;  )  &#x2265;   1  16  &#x03C0;  2
      {\displaystyle \left(\int _{-\infty }^{\infty }(x-x_{0})^{2}|f(x)|^
      {2}\,dx\right)\left(\int _{-\infty }^{\infty }(\xi -\xi _{0})^{2}\left|
      {\hat {f}}(\xi )\right|^{2}\,d\xi \right)\geq {\frac {1}{16\pi ^{2}}}}  [
      {\displaystyle \left(\int _{-\infty }^{\infty }(x-x_{0})^{2}|f(x)|^
      {2}\,dx\right)\left(\int _{-\infty }^{\infty }(\xi -\xi _{0})^{2}\left|
      {\hat {f}}(\xi )\right|^{2}\,d\xi \right)\geq {\frac {1}{16\pi ^{2}}}}]
for any x0, Î¾0 â â.[12]
In quantum_mechanics, the momentum and position wave_functions are Fourier
transform pairs, to within a factor of Planck's_constant. With this constant
properly taken into account, the inequality above becomes the statement of the
Heisenberg_uncertainty_principle.[33]
A stronger uncertainty principle is the Hirschman_uncertainty_principle, which
is expressed as:
         H  (   | f |   2   )  + H  (   |    f &#x005E;    |   2   )  &#x2265;
      log &#x2061;  (   e 2   )    {\displaystyle H\left(\left|f\right|^
      {2}\right)+H\left(\left|{\hat {f}}\right|^{2}\right)\geq \log \left(
      {\frac {e}{2}}\right)}  [{\displaystyle H\left(\left|f\right|^
      {2}\right)+H\left(\left|{\hat {f}}\right|^{2}\right)\geq \log \left(
      {\frac {e}{2}}\right)}]
where H(p) is the differential_entropy of the probability_density_function p
(x):
         H ( p ) = &#x2212;  &#x222B;  &#x2212; &#x221E;   &#x221E;   p ( x )
      log &#x2061;   (   p ( x )   )    d x   {\displaystyle H(p)=-\int _{-
      \infty }^{\infty }p(x)\log {\bigl (}p(x){\bigr )}\,dx}  [{\displaystyle H
      (p)=-\int _{-\infty }^{\infty }p(x)\log {\bigl (}p(x){\bigr )}\,dx}]
where the logarithms may be in any base that is consistent. The equality is
attained for a Gaussian, as in the previous case.
**** Sine and cosine transforms[edit] ****
Main article: Sine_and_cosine_transforms
Fourier's original formulation of the transform did not use complex numbers,
but rather sines and cosines. Statisticians and others still use this form. An
absolutely integrable function f for which Fourier inversion holds good can be
expanded in terms of genuine frequencies (avoiding negative frequencies, which
are sometimes considered hard to interpret physically[34]) Î» by
         f ( t ) =  &#x222B;  0   &#x221E;     (   a ( &#x03BB; ) cos &#x2061;
      ( 2 &#x03C0; &#x03BB; t ) + b ( &#x03BB; ) sin &#x2061; ( 2 &#x03C0;
      &#x03BB; t )   )    d &#x03BB; .   {\displaystyle f(t)=\int _{0}^{\infty
      }{\bigl (}a(\lambda )\cos(2\pi \lambda t)+b(\lambda )\sin(2\pi \lambda t)
      {\bigr )}\,d\lambda .}  [{\displaystyle f(t)=\int _{0}^{\infty }{\bigl
      (}a(\lambda )\cos(2\pi \lambda t)+b(\lambda )\sin(2\pi \lambda t){\bigr
      )}\,d\lambda .}]
This is called an expansion as a trigonometric integral, or a Fourier integral
expansion. The coefficient functions a and b can be found by using variants of
the Fourier cosine transform and the Fourier sine transform (the normalisations
are, again, not standardised):
         a ( &#x03BB; ) = 2  &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( t )
      cos &#x2061; ( 2 &#x03C0; &#x03BB; t )  d t   {\displaystyle a(\lambda
      )=2\int _{-\infty }^{\infty }f(t)\cos(2\pi \lambda t)\,dt}  [
      {\displaystyle a(\lambda )=2\int _{-\infty }^{\infty }f(t)\cos(2\pi
      \lambda t)\,dt}]
and
         b ( &#x03BB; ) = 2  &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( t )
      sin &#x2061; ( 2 &#x03C0; &#x03BB; t )  d t .   {\displaystyle b(\lambda
      )=2\int _{-\infty }^{\infty }f(t)\sin(2\pi \lambda t)\,dt.}  [
      {\displaystyle b(\lambda )=2\int _{-\infty }^{\infty }f(t)\sin(2\pi
      \lambda t)\,dt.}]
Older literature refers to the two transform functions, the Fourier cosine
transform, a, and the Fourier sine transform, b.
The function f can be recovered from the sine and cosine transform using
         f ( t ) = 2  &#x222B;  0   &#x221E;    &#x222B;  &#x2212; &#x221E;
      &#x221E;   f ( &#x03C4; ) cos &#x2061;   (   2 &#x03C0; &#x03BB;
      ( &#x03C4; &#x2212; t )   )    d &#x03C4;  d &#x03BB; .   {\displaystyle
      f(t)=2\int _{0}^{\infty }\int _{-\infty }^{\infty }f(\tau )\cos {\bigl
      (}2\pi \lambda (\tau -t){\bigr )}\,d\tau \,d\lambda .}  [{\displaystyle f
      (t)=2\int _{0}^{\infty }\int _{-\infty }^{\infty }f(\tau )\cos {\bigl
      (}2\pi \lambda (\tau -t){\bigr )}\,d\tau \,d\lambda .}]
together with trigonometric identities. This is referred to as Fourier's
integral formula.[28][35][36][37]
**** Spherical harmonics[edit] ****
Let the set of homogeneous harmonic polynomials of degree k on ân be denoted
by Ak. The set Ak consists of the solid_spherical_harmonics of degree k. The
solid spherical harmonics play a similar role in higher dimensions to the
Hermite polynomials in dimension one. Specifically, if f (x) = eâÏ|x|2P(x)
for some P(x) in Ak, then fÌ (Î¾) = iâk f (Î¾). Let the set Hk be the
closure in L2(ân) of linear combinations of functions of the form f (|x|)P(x)
where P(x) is in Ak. The space L2(ân) is then a direct sum of the spaces Hk
and the Fourier transform maps each space Hk to itself and is possible to
characterize the action of the Fourier transform on each space Hk.[15]
Let f (x) = f0(|x|)P(x) (with P(x) in Ak), then
            f &#x005E;    ( &#x03BE; ) =  F  0   (  |  &#x03BE;  |  ) P
      ( &#x03BE; )   {\displaystyle {\hat {f}}(\xi )=F_{0}(|\xi |)P(\xi )}  [
      {\hat {f}}(\xi )=F_{0}(|\xi |)P(\xi )]
where
          F  0   ( r ) = 2 &#x03C0;  i  &#x2212; k    r  &#x2212;    n + 2 k
      &#x2212; 2  2      &#x222B;  0   &#x221E;    f  0   ( s )  J    n + 2 k
      &#x2212; 2  2    ( 2 &#x03C0; r s )  s    n + 2 k  2     d s .
      {\displaystyle F_{0}(r)=2\pi i^{-k}r^{-{\frac {n+2k-2}{2}}}\int _{0}^
      {\infty }f_{0}(s)J_{\frac {n+2k-2}{2}}(2\pi rs)s^{\frac {n+2k}{2}}\,ds.}
      [{\displaystyle F_{0}(r)=2\pi i^{-k}r^{-{\frac {n+2k-2}{2}}}\int _{0}^
      {\infty }f_{0}(s)J_{\frac {n+2k-2}{2}}(2\pi rs)s^{\frac {n+2k}{2}}\,ds.}]
Here Jn + 2k â 2/2 denotes the Bessel_function of the first kind with order n
+ 2k â 2/2. When k = 0 this gives a useful formula for the Fourier transform
of a radial function.[38] Note that this is essentially the Hankel_transform.
Moreover, there is a simple recursion relating the cases n + 2 and n[39]
allowing to compute, e.g., the three-dimensional Fourier transform of a radial
function from the one-dimensional one.
**** Restriction problems[edit] ****
In higher dimensions it becomes interesting to study restriction problems for
the Fourier transform. The Fourier transform of an integrable function is
continuous and the restriction of this function to any set is defined. But for
a square-integrable function the Fourier transform could be a general class of
square integrable functions. As such, the restriction of the Fourier transform
of an L2(ân) function cannot be defined on sets of measure 0. It is still an
active area of study to understand restriction problems in Lp for 1 < p < 2.
Surprisingly, it is possible in some cases to define the restriction of a
Fourier transform to a set S, provided S has non-zero curvature. The case when
S is the unit sphere in ân is of particular interest. In this case the
TomasâStein restriction theorem states that the restriction of the Fourier
transform to the unit sphere in ân is a bounded operator on Lp provided 1 â¤
p â¤ 2n + 2/n + 3.
One notable difference between the Fourier transform in 1 dimension versus
higher dimensions concerns the partial sum operator. Consider an increasing
collection of measurable sets ER indexed by R â (0,â): such as balls of
radius R centered at the origin, or cubes of side 2R. For a given integrable
function f, consider the function fR defined by:
          f  R   ( x ) =  &#x222B;   E  R        f &#x005E;    ( &#x03BE; )  e
      2 &#x03C0; i x &#x22C5; &#x03BE;    d &#x03BE; ,  x &#x2208;   R   n   .
      {\displaystyle f_{R}(x)=\int _{E_{R}}{\hat {f}}(\xi )e^{2\pi ix\cdot \xi
      }\,d\xi ,\quad x\in \mathbb {R} ^{n}.}  [{\displaystyle f_{R}(x)=\int _
      {E_{R}}{\hat {f}}(\xi )e^{2\pi ix\cdot \xi }\,d\xi ,\quad x\in \mathbb
      {R} ^{n}.}]
Suppose in addition that f â Lp(ân). For n = 1 and 1 < p < â, if one
takes ER = (âR, R), then fR converges to f in Lp as R tends to infinity, by
the boundedness of the Hilbert_transform. Naively one may hope the same holds
true for n > 1. In the case that ER is taken to be a cube with side length R,
then convergence still holds. Another natural candidate is the Euclidean ball
ER = {Î¾ : |Î¾| < R}. In order for this partial sum operator to converge, it is
necessary that the multiplier for the unit ball be bounded in Lp(ân). For n
â¥ 2 it is a celebrated theorem of Charles_Fefferman that the multiplier for
the unit ball is never bounded unless p = 2.[18] In fact, when p â  2, this
shows that not only may fR fail to converge to f in Lp, but for some functions
f â Lp(ân), fR is not even an element of Lp.
***** Fourier transform on function spaces[edit] *****
**** On Lp spaces[edit] ****
*** On L1[edit] ***
The definition of the Fourier transform by the integral formula
            f &#x005E;    ( &#x03BE; ) =  &#x222B;    R   n     f ( x )  e
      &#x2212; 2 &#x03C0; i &#x03BE; &#x22C5; x    d x   {\displaystyle {\hat
      {f}}(\xi )=\int _{\mathbb {R} ^{n}}f(x)e^{-2\pi i\xi \cdot x}\,dx}  [
      {\displaystyle {\hat {f}}(\xi )=\int _{\mathbb {R} ^{n}}f(x)e^{-2\pi i\xi
      \cdot x}\,dx}]
is valid for Lebesgue integrable functions f; that is, f â L1(ân).
The Fourier transform F : L1(ân) â Lâ(ân) is a bounded_operator. This
follows from the observation that
          |     f &#x005E;    ( &#x03BE; )  |  &#x2264;  &#x222B;    R   n
      | f ( x ) |  d x ,   {\displaystyle \left\vert {\hat {f}}(\xi
      )\right\vert \leq \int _{\mathbb {R} ^{n}}\vert f(x)\vert \,dx,}  [
      {\displaystyle \left\vert {\hat {f}}(\xi )\right\vert \leq \int _{\mathbb
      {R} ^{n}}\vert f(x)\vert \,dx,}]
which shows that its operator_norm is bounded by 1. Indeed, it equals 1, which
can be seen, for example, from the transform_of_the_rect_function. The image of
L1 is a subset of the space C0(ân) of continuous functions that tend to zero
at infinity (the RiemannâLebesgue_lemma), although it is not the entire
space. Indeed, there is no simple characterization of the image.
*** On L2[edit] ***
Since compactly supported smooth functions are integrable and dense in L2
(ân), the Plancherel_theorem allows us to extend the definition of the
Fourier transform to general functions in L2(ân) by continuity arguments. The
Fourier transform in L2(ân) is no longer given by an ordinary Lebesgue
integral, although it can be computed by an improper_integral, here meaning
that for an L2 function f,
            f &#x005E;    ( &#x03BE; ) =  lim  R &#x2192; &#x221E;    &#x222B;
      |  x  |  &#x2264; R   f ( x )  e  &#x2212; 2 &#x03C0; i x &#x22C5;
      &#x03BE;    d x   {\displaystyle {\hat {f}}(\xi )=\lim _{R\to \infty
      }\int _{|x|\leq R}f(x)e^{-2\pi ix\cdot \xi }\,dx}  [{\hat {f}}(\xi )=\lim
      _{R\to \infty }\int _{|x|\leq R}f(x)e^{-2\pi ix\cdot \xi }\,dx]
where the limit is taken in the L2 sense. (More generally, you can take a
sequence of functions that are in the intersection of L1 and L2 and that
converges to f in the L2-norm, and define the Fourier transform of f as the L2
-limit of the Fourier transforms of these functions.[40])
Many of the properties of the Fourier transform in L1 carry over to L2, by a
suitable limiting argument.
Furthermore, F : L2(ân) â L2(ân) is a unitary_operator.[41] For an
operator to be unitary it is sufficient to show that it is bijective and
preserves the inner product, so in this case these follow from the Fourier
inversion theorem combined with the fact that for any f, g â L2(ân) we have
          &#x222B;    R   n     f ( x )   F   g ( x )  d x =  &#x222B;    R   n
      F   f ( x ) g ( x )  d x .   {\displaystyle \int _{\mathbb {R} ^{n}}f(x)
      {\mathcal {F}}g(x)\,dx=\int _{\mathbb {R} ^{n}}{\mathcal {F}}f(x)g
      (x)\,dx.}  [{\displaystyle \int _{\mathbb {R} ^{n}}f(x){\mathcal {F}}g
      (x)\,dx=\int _{\mathbb {R} ^{n}}{\mathcal {F}}f(x)g(x)\,dx.}]
In particular, the image of L2(ân) is itself under the Fourier transform.
*** On other Lp[edit] ***
The definition of the Fourier transform can be extended to functions in Lp
(ân) for 1 â¤ p â¤ 2 by decomposing such functions into a fat tail part in
L2 plus a fat body part in L1. In each of these spaces, the Fourier transform
of a function in Lp(ân) is in Lq(ân), where q = p/p â 1 is the HÃ¶lder
conjugate of p (by the HausdorffâYoung_inequality). However, except for p =
2, the image is not easily characterized. Further extensions become more
technical. The Fourier transform of functions in Lp for the range 2 < p < â
requires the study of distributions.[14] In fact, it can be shown that there
are functions in Lp with p > 2 so that the Fourier transform is not defined as
a function.[15]
**** Tempered distributions[edit] ****
Main article: Distribution_(mathematics)_Â§ Tempered_distributions_and_Fourier
transform
One might consider enlarging the domain of the Fourier transform from L1 + L2
by considering generalized_functions, or distributions. A distribution on ân
is a continuous linear functional on the space Cc(ân) of compactly supported
smooth functions, equipped with a suitable topology. The strategy is then to
consider the action of the Fourier transform on Cc(ân) and pass to
distributions by duality. The obstruction to doing this is that the Fourier
transform does not map Cc(ân) to Cc(ân). In fact the Fourier transform of
an element in Cc(ân) can not vanish on an open set; see the above discussion
on the uncertainty principle. The right space here is the slightly larger space
of Schwartz_functions. The Fourier transform is an automorphism on the Schwartz
space, as a topological vector space, and thus induces an automorphism on its
dual, the space of tempered distributions.[15] The tempered distributions
include all the integrable functions mentioned above, as well as well-behaved
functions of polynomial growth and distributions of compact support.
For the definition of the Fourier transform of a tempered distribution, let f
and g be integrable functions, and let fÌ and Ä be their Fourier transforms
respectively. Then the Fourier transform obeys the following multiplication
formula,[15]
          &#x222B;    R   n        f &#x005E;    ( x ) g ( x )  d x =  &#x222B;
      R   n     f ( x )    g &#x005E;    ( x )  d x .   {\displaystyle \int _
      {\mathbb {R} ^{n}}{\hat {f}}(x)g(x)\,dx=\int _{\mathbb {R} ^{n}}f(x){\hat
      {g}}(x)\,dx.}  [{\displaystyle \int _{\mathbb {R} ^{n}}{\hat {f}}(x)g
      (x)\,dx=\int _{\mathbb {R} ^{n}}f(x){\hat {g}}(x)\,dx.}]
Every integrable function f defines (induces) a distribution Tf by the relation
          T  f   ( &#x03C6; ) =  &#x222B;    R   n     f ( x ) &#x03C6; ( x )
      d x   {\displaystyle T_{f}(\varphi )=\int _{\mathbb {R} ^{n}}f(x)\varphi
      (x)\,dx}  [{\displaystyle T_{f}(\varphi )=\int _{\mathbb {R} ^{n}}f
      (x)\varphi (x)\,dx}]
for all Schwartz functions Ï. So it makes sense to define Fourier transform
TÌf of Tf by
             T &#x005E;     f   ( &#x03C6; ) =  T  f    (    &#x03C6; &#x005E;
      )    {\displaystyle {\hat {T}}_{f}(\varphi )=T_{f}\left({\hat {\varphi
      }}\right)}  [{\displaystyle {\hat {T}}_{f}(\varphi )=T_{f}\left({\hat
      {\varphi }}\right)}]
for all Schwartz functions Ï. Extending this to all tempered distributions T
gives the general definition of the Fourier transform.
Distributions can be differentiated and the above-mentioned compatibility of
the Fourier transform with differentiation and convolution remains true for
tempered distributions.
***** Generalizations[edit] *****
**** FourierâStieltjes transform[edit] ****
The Fourier transform of a finite Borel measure Î¼ on ân is given by:[42]
            &#x03BC; &#x005E;    ( &#x03BE; ) =  &#x222B;    R   n      e
      &#x2212; 2 &#x03C0; i x &#x22C5; &#x03BE;    d &#x03BC; .
      {\displaystyle {\hat {\mu }}(\xi )=\int _{\mathbb {R} ^{n}}e^{-2\pi
      ix\cdot \xi }\,d\mu .}  [{\displaystyle {\hat {\mu }}(\xi )=\int _
      {\mathbb {R} ^{n}}e^{-2\pi ix\cdot \xi }\,d\mu .}]
This transform continues to enjoy many of the properties of the Fourier
transform of integrable functions. One notable difference is that the
RiemannâLebesgue_lemma fails for measures.[14] In the case that dÎ¼ = f (x)
dx, then the formula above reduces to the usual definition for the Fourier
transform of f. In the case that Î¼ is the probability distribution associated
to a random variable X, the FourierâStieltjes transform is closely related to
the characteristic_function, but the typical conventions in probability theory
take eixÎ¾ instead of eâ2ÏixÎ¾.[13] In the case when the distribution has a
probability_density_function this definition reduces to the Fourier transform
applied to the probability density function, again with a different choice of
constants.
The Fourier transform may be used to give a characterization of measures.
Bochner's_theorem characterizes which functions may arise as the
FourierâStieltjes transform of a positive measure on the circle.[14]
Furthermore, the Dirac_delta_function, although not a function, is a finite
Borel_measure. Its Fourier transform is a constant function (whose specific
value depends upon the form of the Fourier transform used).
**** Locally compact abelian groups[edit] ****
Main article: Pontryagin_duality
The Fourier transform may be generalized to any locally compact abelian group.
A locally compact abelian group is an abelian_group that is at the same time a
locally_compact Hausdorff_topological_space so that the group operation is
continuous. If G is a locally compact abelian group, it has a translation
invariant measure Î¼, called Haar_measure. For a locally compact abelian group
G, the set of irreducible, i.e. one-dimensional, unitary representations are
called its characters. With its natural group structure and the topology of
pointwise convergence, the set of characters Ä is itself a locally compact
abelian group, called the Pontryagin dual of G. For a function f in L1(G), its
Fourier transform is defined by[14]
            f &#x005E;    ( &#x03BE; ) =  &#x222B;  G   &#x03BE; ( x ) f ( x )
      d &#x03BC;   for any&#xA0;  &#x03BE; &#x2208;    G &#x005E;    .
      {\displaystyle {\hat {f}}(\xi )=\int _{G}\xi (x)f(x)\,d\mu \qquad {\text
      {for any }}\xi \in {\hat {G}}.}  [{\hat {f}}(\xi )=\int _{G}\xi (x)f
      (x)\,d\mu \qquad {\text{for any }}\xi \in {\hat {G}}.]
The RiemannâLebesgue lemma holds in this case; fÌ (Î¾) is a function
vanishing at infinity on Ä.
**** Gelfand transform[edit] ****
Main article: Gelfand_representation
The Fourier transform is also a special case of Gelfand_transform. In this
particular context, it is closely related to the Pontryagin duality map defined
above.
Given an abelian locally_compact Hausdorff topological_group G, as before we
consider space L1(G), defined using a Haar measure. With convolution as
multiplication, L1(G) is an abelian Banach_algebra. It also has an involution *
given by
          f  &#x2217;   ( g ) =    f  (  g  &#x2212; 1   )   &#x00AF;   .
      {\displaystyle f^{*}(g)={\overline {f\left(g^{-1}\right)}}.}  [
      {\displaystyle f^{*}(g)={\overline {f\left(g^{-1}\right)}}.}]
Taking the completion with respect to the largest possibly C*-norm gives its
enveloping C*-algebra, called the group C*-algebra C*(G) of G. (Any C*-norm on
L1(G) is bounded by the L1 norm, therefore their supremum exists.)
Given any abelian C*-algebra A, the Gelfand transform gives an isomorphism
between A and C0(A^), where A^ is the multiplicative linear functionals, i.e.
one-dimensional representations, on A with the weak-* topology. The map is
simply given by
         a &#x21A6;   (   &#x03C6; &#x21A6; &#x03C6; ( a )   )
      {\displaystyle a\mapsto {\bigl (}\varphi \mapsto \varphi (a){\bigr )}}  [
      {\displaystyle a\mapsto {\bigl (}\varphi \mapsto \varphi (a){\bigr )}}]
It turns out that the multiplicative linear functionals of C*(G), after
suitable identification, are exactly the characters of G, and the Gelfand
transform, when restricted to the dense subset L1(G) is the
FourierâPontryagin transform.
**** Compact non-abelian groups[edit] ****
The Fourier transform can also be defined for functions on a non-abelian group,
provided that the group is compact. Removing the assumption that the underlying
group is abelian, irreducible unitary representations need not always be one-
dimensional. This means the Fourier transform on a non-abelian group takes
values as Hilbert space operators.[43] The Fourier transform on compact groups
is a major tool in representation_theory[44] and non-commutative_harmonic
analysis.
Let G be a compact Hausdorff topological_group. Let Î£ denote the collection of
all isomorphism classes of finite-dimensional irreducible unitary
representations, along with a definite choice of representation U(Ï) on the
Hilbert_space HÏ of finite dimension dÏ for each Ï â Î£. If Î¼ is a finite
Borel_measure on G, then the FourierâStieltjes transform of Î¼ is the
operator on HÏ defined by
           &#x27E8;     &#x03BC; &#x005E;    &#x03BE; , &#x03B7;  &#x27E9;    H
      &#x03C3;     =  &#x222B;  G    &#x27E8;     U &#x00AF;    g   ( &#x03C3;
      )   &#x03BE; , &#x03B7;  &#x27E9;   d &#x03BC; ( g )   {\displaystyle
      \left\langle {\hat {\mu }}\xi ,\eta \right\rangle _{H_{\sigma }}=\int _
      {G}\left\langle {\overline {U}}_{g}^{(\sigma )}\xi ,\eta \right\rangle
      \,d\mu (g)}  [{\displaystyle \left\langle {\hat {\mu }}\xi ,\eta
      \right\rangle _{H_{\sigma }}=\int _{G}\left\langle {\overline {U}}_{g}^{
      (\sigma )}\xi ,\eta \right\rangle \,d\mu (g)}]
where U(Ï) is the complex-conjugate representation of U(Ï) acting on HÏ. If
Î¼ is absolutely_continuous with respect to the left-invariant_probability
measure Î» on G, represented as
         d &#x03BC; = f  d &#x03BB;   {\displaystyle d\mu =f\,d\lambda }  [d\mu
      =f\,d\lambda ]
for some f â L1(Î»), one identifies the Fourier transform of f with the
FourierâStieltjes transform of Î¼.
The mapping
         &#x03BC; &#x21A6;    &#x03BC; &#x005E;      {\displaystyle \mu \mapsto
      {\hat {\mu }}}  [\mu \mapsto {\hat {\mu }}]
defines an isomorphism between the Banach_space M(G) of finite Borel measures
(see rca_space) and a closed subspace of the Banach space Câ(Î£) consisting
of all sequences E = (EÏ) indexed by Î£ of (bounded) linear operators EÏ :
HÏ â HÏ for which the norm
         &#x2016; E &#x2016; =  sup  &#x03C3; &#x2208; &#x03A3;    &#x2016;  E
      &#x03C3;   &#x2016;    {\displaystyle \|E\|=\sup _{\sigma \in \Sigma
      }\left\|E_{\sigma }\right\|}  [{\displaystyle \|E\|=\sup _{\sigma \in
      \Sigma }\left\|E_{\sigma }\right\|}]
is finite. The "convolution_theorem" asserts that, furthermore, this
isomorphism of Banach spaces is in fact an isometric isomorphism of C*_algebras
into a subspace of Câ(Î£). Multiplication on M(G) is given by convolution of
measures and the involution * defined by
          f  &#x2217;   ( g ) =    f  (  g  &#x2212; 1   )   &#x00AF;   ,
      {\displaystyle f^{*}(g)={\overline {f\left(g^{-1}\right)}},}  [
      {\displaystyle f^{*}(g)={\overline {f\left(g^{-1}\right)}},}]
and Câ(Î£) has a natural C*-algebra structure as Hilbert space operators.
The PeterâWeyl_theorem holds, and a version of the Fourier inversion formula
(Plancherel's_theorem) follows: if f â L2(G), then
         f ( g ) =  &#x2211;  &#x03C3; &#x2208; &#x03A3;    d  &#x03C3;   tr
      &#x2061;  (     f &#x005E;    ( &#x03C3; )  U  g   ( &#x03C3; )    )
      {\displaystyle f(g)=\sum _{\sigma \in \Sigma }d_{\sigma }\operatorname
      {tr} \left({\hat {f}}(\sigma )U_{g}^{(\sigma )}\right)}  [{\displaystyle
      f(g)=\sum _{\sigma \in \Sigma }d_{\sigma }\operatorname {tr} \left({\hat
      {f}}(\sigma )U_{g}^{(\sigma )}\right)}]
where the summation is understood as convergent in the L2 sense.
The generalization of the Fourier transform to the noncommutative situation has
also in part contributed to the development of noncommutative_geometry.
[citation_needed] In this context, a categorical generalization of the Fourier
transform to noncommutative groups is TannakaâKrein_duality, which replaces
the group of characters with the category of representations. However, this
loses the connection with harmonic functions.
***** Alternatives[edit] *****
In signal_processing terms, a function (of time) is a representation of a
signal with perfect time resolution, but no frequency information, while the
Fourier transform has perfect frequency resolution, but no time information:
the magnitude of the Fourier transform at a point is how much frequency content
there is, but location is only given by phase (argument of the Fourier
transform at a point), and standing waves are not localized in time â a sine
wave continues out to infinity, without decaying. This limits the usefulness of
the Fourier transform for analyzing signals that are localized in time, notably
transients, or any signal of finite extent.
As alternatives to the Fourier transform, in time-frequency_analysis, one uses
time-frequency transforms or time-frequency distributions to represent signals
in a form that has some time information and some frequency information â by
the uncertainty principle, there is a trade-off between these. These can be
generalizations of the Fourier transform, such as the short-time_Fourier
transform or fractional_Fourier_transform, or other functions to represent
signals, as in wavelet_transforms and chirplet_transforms, with the wavelet
analog of the (continuous) Fourier transform being the continuous_wavelet
transform.[19]
***** Applications[edit] *****
See also: Spectral_density_Â§ Applications
Some problems, such as certain differential equations, become easier to solve
when the Fourier transform is applied. In that case the solution to the
original problem is recovered using the inverse Fourier transform.
**** Analysis of differential equations[edit] ****
Perhaps the most important use of the Fourier transformation is to solve
partial_differential_equations. Many of the equations of the mathematical
physics of the nineteenth century can be treated this way. Fourier studied the
heat equation, which in one dimension and in dimensionless units is
             &#x2202;  2   y ( x , t )    &#x2202;  2   x    =    &#x2202; y
      ( x , t )   &#x2202; t    .   {\displaystyle {\frac {\partial ^{2}y(x,t)}
      {\partial ^{2}x}}={\frac {\partial y(x,t)}{\partial t}}.}  [
      {\displaystyle {\frac {\partial ^{2}y(x,t)}{\partial ^{2}x}}={\frac
      {\partial y(x,t)}{\partial t}}.}]
The example we will give, a slightly more difficult one, is the wave equation
in one dimension,
             &#x2202;  2   y ( x , t )    &#x2202;  2   x    =     &#x2202;  2
      y ( x , t )    &#x2202;  2   t    .   {\displaystyle {\frac {\partial ^
      {2}y(x,t)}{\partial ^{2}x}}={\frac {\partial ^{2}y(x,t)}{\partial ^
      {2}t}}.}  [{\displaystyle {\frac {\partial ^{2}y(x,t)}{\partial ^{2}x}}=
      {\frac {\partial ^{2}y(x,t)}{\partial ^{2}t}}.}]
As usual, the problem is not to find a solution: there are infinitely many. The
problem is that of the so-called "boundary problem": find a solution which
satisfies the "boundary conditions"
         y ( x , 0 ) = f ( x ) ,     &#x2202; y ( x , 0 )   &#x2202; t    = g
      ( x ) .   {\displaystyle y(x,0)=f(x),\qquad {\frac {\partial y(x,0)}
      {\partial t}}=g(x).}  [{\displaystyle y(x,0)=f(x),\qquad {\frac {\partial
      y(x,0)}{\partial t}}=g(x).}]
Here, f and g are given functions. For the heat equation, only one boundary
condition can be required (usually the first one). But for the wave equation,
there are still infinitely many solutions y which satisfy the first boundary
condition. But when one imposes both conditions, there is only one possible
solution.
It is easier to find the Fourier transform Å· of the solution than to find the
solution directly. This is because the Fourier transformation takes
differentiation into multiplication by the variable, and so a partial
differential equation applied to the original function is transformed into
multiplication by polynomial functions of the dual variables applied to the
transformed function. After Å· is determined, we can apply the inverse Fourier
transformation to find y.
Fourier's method is as follows. First, note that any function of the forms
         cos &#x2061;   (   2 &#x03C0; &#x03BE; ( x &#x00B1; t )   )
      &#xA0;or&#xA0;   sin &#x2061;   (   2 &#x03C0; &#x03BE; ( x &#x00B1; t )
      )     {\displaystyle \cos {\bigl (}2\pi \xi (x\pm t){\bigr )}{\mbox{ or
      }}\sin {\bigl (}2\pi \xi (x\pm t){\bigr )}}  [{\displaystyle \cos {\bigl
      (}2\pi \xi (x\pm t){\bigr )}{\mbox{ or }}\sin {\bigl (}2\pi \xi (x\pm t)
      {\bigr )}}]
satisfies the wave equation. These are called the elementary solutions.
Second, note that therefore any integral
         y ( x , t ) =  &#x222B;  0   &#x221E;    a  +   ( &#x03BE; ) cos
      &#x2061;   (   2 &#x03C0; &#x03BE; ( x + t )   )   +  a  &#x2212;
      ( &#x03BE; ) cos &#x2061;   (   2 &#x03C0; &#x03BE; ( x &#x2212; t )   )
      +  b  +   ( &#x03BE; ) sin &#x2061;   (   2 &#x03C0; &#x03BE; ( x + t )
      )   +  b  &#x2212;   ( &#x03BE; ) sin &#x2061;  (  2 &#x03C0; &#x03BE;
      ( x &#x2212; t )  )   d &#x03BE;   {\displaystyle y(x,t)=\int _{0}^
      {\infty }a_{+}(\xi )\cos {\bigl (}2\pi \xi (x+t){\bigr )}+a_{-}(\xi )\cos
      {\bigl (}2\pi \xi (x-t){\bigr )}+b_{+}(\xi )\sin {\bigl (}2\pi \xi (x+t)
      {\bigr )}+b_{-}(\xi )\sin \left(2\pi \xi (x-t)\right)\,d\xi }  [
      {\displaystyle y(x,t)=\int _{0}^{\infty }a_{+}(\xi )\cos {\bigl (}2\pi
      \xi (x+t){\bigr )}+a_{-}(\xi )\cos {\bigl (}2\pi \xi (x-t){\bigr )}+b_{+}
      (\xi )\sin {\bigl (}2\pi \xi (x+t){\bigr )}+b_{-}(\xi )\sin \left(2\pi
      \xi (x-t)\right)\,d\xi }]
(for arbitrary a+, aâ, b+, bâ) satisfies the wave equation. (This integral
is just a kind of continuous linear combination, and the equation is linear.)
Now this resembles the formula for the Fourier synthesis of a function. In
fact, this is the real inverse Fourier transform of aÂ± and bÂ± in the variable
x.
The third step is to examine how to find the specific unknown coefficient
functions aÂ± and bÂ± that will lead to y satisfying the boundary conditions.
We are interested in the values of these solutions at t = 0. So we will set t =
0. Assuming that the conditions needed for Fourier inversion are satisfied, we
can then find the Fourier sine and cosine transforms (in the variable x) of
both sides and obtain
         2  &#x222B;  &#x2212; &#x221E;   &#x221E;   y ( x , 0 ) cos &#x2061;
      ( 2 &#x03C0; &#x03BE; x )  d x =  a  +   +  a  &#x2212;
      {\displaystyle 2\int _{-\infty }^{\infty }y(x,0)\cos(2\pi \xi x)\,dx=a_
      {+}+a_{-}}  [{\displaystyle 2\int _{-\infty }^{\infty }y(x,0)\cos(2\pi
      \xi x)\,dx=a_{+}+a_{-}}]
and
         2  &#x222B;  &#x2212; &#x221E;   &#x221E;   y ( x , 0 ) sin &#x2061;
      ( 2 &#x03C0; &#x03BE; x )  d x =  b  +   +  b  &#x2212;   .
      {\displaystyle 2\int _{-\infty }^{\infty }y(x,0)\sin(2\pi \xi x)\,dx=b_
      {+}+b_{-}.}  [{\displaystyle 2\int _{-\infty }^{\infty }y(x,0)\sin(2\pi
      \xi x)\,dx=b_{+}+b_{-}.}]
Similarly, taking the derivative of y with respect to t and then applying the
Fourier sine and cosine transformations yields
         2  &#x222B;  &#x2212; &#x221E;   &#x221E;      &#x2202; y ( u , 0 )
      &#x2202; t    sin &#x2061; ( 2 &#x03C0; &#x03BE; x )  d x = ( 2 &#x03C0;
      &#x03BE; )  (  &#x2212;  a  +   +  a  &#x2212;    )    {\displaystyle
      2\int _{-\infty }^{\infty }{\frac {\partial y(u,0)}{\partial t}}\sin(2\pi
      \xi x)\,dx=(2\pi \xi )\left(-a_{+}+a_{-}\right)}  [{\displaystyle 2\int _
      {-\infty }^{\infty }{\frac {\partial y(u,0)}{\partial t}}\sin(2\pi \xi
      x)\,dx=(2\pi \xi )\left(-a_{+}+a_{-}\right)}]
and
         2  &#x222B;  &#x2212; &#x221E;   &#x221E;      &#x2202; y ( u , 0 )
      &#x2202; t    cos &#x2061; ( 2 &#x03C0; &#x03BE; x )  d x = ( 2 &#x03C0;
      &#x03BE; )  (   b  +   &#x2212;  b  &#x2212;    )  .   {\displaystyle
      2\int _{-\infty }^{\infty }{\frac {\partial y(u,0)}{\partial t}}\cos(2\pi
      \xi x)\,dx=(2\pi \xi )\left(b_{+}-b_{-}\right).}  [{\displaystyle 2\int _
      {-\infty }^{\infty }{\frac {\partial y(u,0)}{\partial t}}\cos(2\pi \xi
      x)\,dx=(2\pi \xi )\left(b_{+}-b_{-}\right).}]
These are four linear equations for the four unknowns aÂ± and bÂ±, in terms of
the Fourier sine and cosine transforms of the boundary conditions, which are
easily solved by elementary algebra, provided that these transforms can be
found.
In summary, we chose a set of elementary solutions, parametrised by Î¾, of
which the general solution would be a (continuous) linear combination in the
form of an integral over the parameter Î¾. But this integral was in the form of
a Fourier integral. The next step was to express the boundary conditions in
terms of these integrals, and set them equal to the given functions f and g.
But these expressions also took the form of a Fourier integral because of the
properties of the Fourier transform of a derivative. The last step was to
exploit Fourier inversion by applying the Fourier transformation to both sides,
thus obtaining expressions for the coefficient functions aÂ± and bÂ± in terms
of the given boundary conditions f and g.
From a higher point of view, Fourier's procedure can be reformulated more
conceptually. Since there are two variables, we will use the Fourier
transformation in both x and t rather than operate as Fourier did, who only
transformed in the spatial variables. Note that Å· must be considered in the
sense of a distribution since y(x, t) is not going to be L1: as a wave, it will
persist through time and thus is not a transient phenomenon. But it will be
bounded and so its Fourier transform can be defined as a distribution. The
operational properties of the Fourier transformation that are relevant to this
equation are that it takes differentiation in x to multiplication by 2ÏiÎ¾ and
differentiation with respect to t to multiplication by 2Ïif where f is the
frequency. Then the wave equation becomes an algebraic equation in Å·:
          &#x03BE;  2      y &#x005E;    ( &#x03BE; , f ) =  f  2      y
      &#x005E;    ( &#x03BE; , f ) .   {\displaystyle \xi ^{2}{\hat {y}}(\xi
      ,f)=f^{2}{\hat {y}}(\xi ,f).}  [\xi ^{2}{\hat {y}}(\xi ,f)=f^{2}{\hat
      {y}}(\xi ,f).]
This is equivalent to requiring Å·(Î¾, f ) = 0 unless Î¾ = Â±f. Right away,
this explains why the choice of elementary solutions we made earlier worked so
well: obviously fÌ = Î´(Î¾ Â± f ) will be solutions. Applying Fourier
inversion to these delta functions, we obtain the elementary solutions we
picked earlier. But from the higher point of view, one does not pick elementary
solutions, but rather considers the space of all distributions which are
supported on the (degenerate) conic Î¾2 â f2 = 0.
We may as well consider the distributions supported on the conic that are given
by distributions of one variable on the line Î¾ = f plus distributions on the
line Î¾ = âf as follows: if Ï is any test function,
         &#x222C;    y &#x005E;    &#x03D5; ( &#x03BE; , f )  d &#x03BE;  d f =
      &#x222B;  s  +   &#x03D5; ( &#x03BE; , &#x03BE; )  d &#x03BE; + &#x222B;
      s  &#x2212;   &#x03D5; ( &#x03BE; , &#x2212; &#x03BE; )  d &#x03BE; ,
      {\displaystyle \iint {\hat {y}}\phi (\xi ,f)\,d\xi \,df=\int s_{+}\phi
      (\xi ,\xi )\,d\xi +\int s_{-}\phi (\xi ,-\xi )\,d\xi ,}  [{\displaystyle
      \iint {\hat {y}}\phi (\xi ,f)\,d\xi \,df=\int s_{+}\phi (\xi ,\xi )\,d\xi
      +\int s_{-}\phi (\xi ,-\xi )\,d\xi ,}]
where s+, and sâ, are distributions of one variable.
Then Fourier inversion gives, for the boundary conditions, something very
similar to what we had more concretely above (put Ï(Î¾, f ) = e2Ïi(xÎ¾+tf ),
which is clearly of polynomial growth):
         y ( x , 0 ) = &#x222B;   {    s  +   ( &#x03BE; ) +  s  &#x2212;
      ( &#x03BE; )   }    e  2 &#x03C0; i &#x03BE; x + 0    d &#x03BE;
      {\displaystyle y(x,0)=\int {\bigl \{}s_{+}(\xi )+s_{-}(\xi ){\bigr \}}e^
      {2\pi i\xi x+0}\,d\xi }  [{\displaystyle y(x,0)=\int {\bigl \{}s_{+}(\xi
      )+s_{-}(\xi ){\bigr \}}e^{2\pi i\xi x+0}\,d\xi }]
and
            &#x2202; y ( x , 0 )   &#x2202; t    = &#x222B;   {    s  +
      ( &#x03BE; ) &#x2212;  s  &#x2212;   ( &#x03BE; )   }   2 &#x03C0; i
      &#x03BE;  e  2 &#x03C0; i &#x03BE; x + 0    d &#x03BE; .   {\displaystyle
      {\frac {\partial y(x,0)}{\partial t}}=\int {\bigl \{}s_{+}(\xi )-s_{-}
      (\xi ){\bigr \}}2\pi i\xi e^{2\pi i\xi x+0}\,d\xi .}  [{\displaystyle
      {\frac {\partial y(x,0)}{\partial t}}=\int {\bigl \{}s_{+}(\xi )-s_{-}
      (\xi ){\bigr \}}2\pi i\xi e^{2\pi i\xi x+0}\,d\xi .}]
Now, as before, applying the one-variable Fourier transformation in the
variable x to these functions of x yields two equations in the two unknown
distributions sÂ± (which can be taken to be ordinary functions if the boundary
conditions are L1 or L2).
From a calculational point of view, the drawback of course is that one must
first calculate the Fourier transforms of the boundary conditions, then
assemble the solution from these, and then calculate an inverse Fourier
transform. Closed form formulas are rare, except when there is some geometric
symmetry that can be exploited, and the numerical calculations are difficult
because of the oscillatory nature of the integrals, which makes convergence
slow and hard to estimate. For practical calculations, other methods are often
used.
The twentieth century has seen the extension of these methods to all linear
partial differential equations with polynomial coefficients, and by extending
the notion of Fourier transformation to include Fourier integral operators,
some non-linear equations as well.
**** Fourier transform spectroscopy[edit] ****
Main article: Fourier_transform_spectroscopy
The Fourier transform is also used in nuclear_magnetic_resonance (NMR) and in
other kinds of spectroscopy, e.g. infrared (FTIR). In NMR an exponentially
shaped free induction decay (FID) signal is acquired in the time domain and
Fourier-transformed to a Lorentzian line-shape in the frequency domain. The
Fourier transform is also used in magnetic_resonance_imaging (MRI) and mass
spectrometry.
**** Quantum mechanics[edit] ****
The Fourier transform is useful in quantum_mechanics in two different ways. To
begin with, the basic conceptual structure of Quantum Mechanics postulates the
existence of pairs of complementary variables, connected by the Heisenberg
uncertainty principle. For example, in one dimension, the spatial variable q
of, say, a particle, can only be measured by the quantum mechanical "position
operator" at the cost of losing information about the momentum p of the
particle. Therefore, the physical state of the particle can either be described
by a function, called "the wave function", of q or by a function of p but not
by a function of both variables. The variable p is called the conjugate
variable to q. In Classical Mechanics, the physical state of a particle
(existing in one dimension, for simplicity of exposition) would be given by
assigning definite values to both p and q simultaneously. Thus, the set of all
possible physical states is the two-dimensional real vector space with a p-axis
and a q-axis called the phase space.
In contrast, quantum mechanics chooses a polarisation of this space in the
sense that it picks a subspace of one-half the dimension, for example, the q-
axis alone, but instead of considering only points, takes the set of all
complex-valued "wave functions" on this axis. Nevertheless, choosing the p-axis
is an equally valid polarisation, yielding a different representation of the
set of possible physical states of the particle which is related to the first
representation by the Fourier transformation
         &#x03D5; ( p ) = &#x222B; &#x03C8; ( q )  e  2 &#x03C0; i    p q  h
      d q .   {\displaystyle \phi (p)=\int \psi (q)e^{2\pi i{\frac {pq}
      {h}}}\,dq.}  [{\displaystyle \phi (p)=\int \psi (q)e^{2\pi i{\frac {pq}
      {h}}}\,dq.}]
Physically realisable states are L2, and so by the Plancherel theorem, their
Fourier transforms are also L2. (Note that since q is in units of distance and
p is in units of momentum, the presence of Planck's constant in the exponent
makes the exponent dimensionless, as it should be.)
Therefore, the Fourier transform can be used to pass from one way of
representing the state of the particle, by a wave function of position, to
another way of representing the state of the particle: by a wave function of
momentum. Infinitely many different polarisations are possible, and all are
equally valid. Being able to transform states from one representation to
another is sometimes convenient.
The other use of the Fourier transform in both quantum mechanics and quantum
field_theory is to solve the applicable wave equation. In non-relativistic
quantum mechanics, SchrÃ¶dinger's_equation for a time-varying wave function in
one-dimension, not subject to external forces, is
            &#x2202;  2    &#x2202;  x  2      &#x03C8; ( x , t ) = i   h  2
      &#x03C0;      &#x2202;  &#x2202; t    &#x03C8; ( x , t ) .
      {\displaystyle {\frac {\partial ^{2}}{\partial x^{2}}}\psi (x,t)=i{\frac
      {h}{2\pi }}{\frac {\partial }{\partial t}}\psi (x,t).}  [{\displaystyle
      {\frac {\partial ^{2}}{\partial x^{2}}}\psi (x,t)=i{\frac {h}{2\pi }}
      {\frac {\partial }{\partial t}}\psi (x,t).}]
This is the same as the heat equation except for the presence of the imaginary
unit i. Fourier methods can be used to solve this equation.
In the presence of a potential, given by the potential energy function V(x),
the equation becomes
            &#x2202;  2    &#x2202;  x  2      &#x03C8; ( x , t ) + V ( x )
      &#x03C8; ( x , t ) = i   h  2 &#x03C0;      &#x2202;  &#x2202; t
      &#x03C8; ( x , t ) .   {\displaystyle {\frac {\partial ^{2}}{\partial x^
      {2}}}\psi (x,t)+V(x)\psi (x,t)=i{\frac {h}{2\pi }}{\frac {\partial }
      {\partial t}}\psi (x,t).}  [{\displaystyle {\frac {\partial ^{2}}
      {\partial x^{2}}}\psi (x,t)+V(x)\psi (x,t)=i{\frac {h}{2\pi }}{\frac
      {\partial }{\partial t}}\psi (x,t).}]
The "elementary solutions", as we referred to them above, are the so-called
"stationary states" of the particle, and Fourier's algorithm, as described
above, can still be used to solve the boundary value problem of the future
evolution of Ï given its values for t = 0. Neither of these approaches is of
much practical use in quantum mechanics. Boundary value problems and the time-
evolution of the wave function is not of much practical interest: it is the
stationary states that are most important.
In relativistic quantum mechanics, SchrÃ¶dinger's equation becomes a wave
equation as was usual in classical physics, except that complex-valued waves
are considered. A simple example, in the absence of interactions with other
particles or fields, is the free one-dimensional
KleinâGordonâSchrÃ¶dingerâFock equation, this time in dimensionless
units,
          (     &#x2202;  2    &#x2202;  x  2      + 1  )  &#x03C8; ( x , t ) =
      &#x2202;  2    &#x2202;  t  2      &#x03C8; ( x , t ) .   {\displaystyle
      \left({\frac {\partial ^{2}}{\partial x^{2}}}+1\right)\psi (x,t)={\frac
      {\partial ^{2}}{\partial t^{2}}}\psi (x,t).}  [{\displaystyle \left(
      {\frac {\partial ^{2}}{\partial x^{2}}}+1\right)\psi (x,t)={\frac
      {\partial ^{2}}{\partial t^{2}}}\psi (x,t).}]
This is, from the mathematical point of view, the same as the wave equation of
classical physics solved above (but with a complex-valued wave, which makes no
difference in the methods). This is of great use in quantum field theory: each
separate Fourier component of a wave can be treated as a separate harmonic
oscillator and then quantized, a procedure known as "second quantization".
Fourier methods have been adapted to also deal with non-trivial interactions.
**** Signal processing[edit] ****
The Fourier transform is used for the spectral analysis of time-series. The
subject of statistical signal processing does not, however, usually apply the
Fourier transformation to the signal itself. Even if a real signal is indeed
transient, it has been found in practice advisable to model a signal by a
function (or, alternatively, a stochastic process) which is stationary in the
sense that its characteristic properties are constant over all time. The
Fourier transform of such a function does not exist in the usual sense, and it
has been found more useful for the analysis of signals to instead take the
Fourier transform of its autocorrelation function.
The autocorrelation function R of a function f is defined by
          R  f   ( &#x03C4; ) =  lim  T &#x2192; &#x221E;     1  2 T
      &#x222B;  &#x2212; T   T   f ( t ) f ( t + &#x03C4; )  d t .
      {\displaystyle R_{f}(\tau )=\lim _{T\rightarrow \infty }{\frac {1}
      {2T}}\int _{-T}^{T}f(t)f(t+\tau )\,dt.}  [{\displaystyle R_{f}(\tau
      )=\lim _{T\rightarrow \infty }{\frac {1}{2T}}\int _{-T}^{T}f(t)f(t+\tau
      )\,dt.}]
This function is a function of the time-lag Ï elapsing between the values of f
to be correlated.
For most functions f that occur in practice, R is a bounded even function of
the time-lag Ï and for typical noisy signals it turns out to be uniformly
continuous with a maximum at Ï = 0.
The autocorrelation function, more properly called the autocovariance function
unless it is normalized in some appropriate fashion, measures the strength of
the correlation between the values of f separated by a time lag. This is a way
of searching for the correlation of f with its own past. It is useful even for
other statistical tasks besides the analysis of signals. For example, if f (t)
represents the temperature at time t, one expects a strong correlation with the
temperature at a time lag of 24 hours.
It possesses a Fourier transform,
          P  f   ( &#x03BE; ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;    R  f
      ( &#x03C4; )  e  &#x2212; 2 &#x03C0; i &#x03BE; &#x03C4;    d &#x03C4; .
      {\displaystyle P_{f}(\xi )=\int _{-\infty }^{\infty }R_{f}(\tau )e^{-2\pi
      i\xi \tau }\,d\tau .}  [{\displaystyle P_{f}(\xi )=\int _{-\infty }^
      {\infty }R_{f}(\tau )e^{-2\pi i\xi \tau }\,d\tau .}]
This Fourier transform is called the power spectral density function of f.
(Unless all periodic components are first filtered out from f, this integral
will diverge, but it is easy to filter out such periodicities.)
The power spectrum, as indicated by this density function P, measures the
amount of variance contributed to the data by the frequency Î¾. In electrical
signals, the variance is proportional to the average power (energy per unit
time), and so the power spectrum describes how much the different frequencies
contribute to the average power of the signal. This process is called the
spectral analysis of time-series and is analogous to the usual analysis of
variance of data that is not a time-series (ANOVA).
Knowledge of which frequencies are "important" in this sense is crucial for the
proper design of filters and for the proper evaluation of measuring
apparatuses. It can also be useful for the scientific analysis of the phenomena
responsible for producing the data.
The power spectrum of a signal can also be approximately measured directly by
measuring the average power that remains in a signal after all the frequencies
outside a narrow band have been filtered out.
Spectral analysis is carried out for visual signals as well. The power spectrum
ignores all phase relations, which is good enough for many purposes, but for
video signals other types of spectral analysis must also be employed, still
using the Fourier transform as a tool.
***** Other notations[edit] *****
Other common notations for fÌ (Î¾) include:
            f &#x007E;    ( &#x03BE; ) , &#xA0;    f &#x007E;    ( &#x03C9; ) ,
      &#xA0; F ( &#x03BE; ) , &#xA0;   F    ( f )  ( &#x03BE; ) , &#xA0;
      (    F   f  )  ( &#x03BE; ) , &#xA0;   F   ( f ) , &#xA0;   F
      ( &#x03C9; ) , &#xA0; F ( &#x03C9; ) , &#xA0;   F   ( j &#x03C9; ) ,
      &#xA0;   F   { f } , &#xA0;   F     (   f ( t )   )   , &#xA0;   F
      {   f ( t )   }   .   {\displaystyle {\tilde {f}}(\xi ),\ {\tilde {f}}
      (\omega ),\ F(\xi ),\ {\mathcal {F}}\left(f\right)(\xi ),\ \left(
      {\mathcal {F}}f\right)(\xi ),\ {\mathcal {F}}(f),\ {\mathcal {F}}(\omega
      ),\ F(\omega ),\ {\mathcal {F}}(j\omega ),\ {\mathcal {F}}\{f\},\
      {\mathcal {F}}{\bigl (}f(t){\bigr )},\ {\mathcal {F}}{\bigl \{}f(t){\bigr
      \}}.}  [{\displaystyle {\tilde {f}}(\xi ),\ {\tilde {f}}(\omega ),\ F(\xi
      ),\ {\mathcal {F}}\left(f\right)(\xi ),\ \left({\mathcal {F}}f\right)(\xi
      ),\ {\mathcal {F}}(f),\ {\mathcal {F}}(\omega ),\ F(\omega ),\ {\mathcal
      {F}}(j\omega ),\ {\mathcal {F}}\{f\},\ {\mathcal {F}}{\bigl (}f(t){\bigr
      )},\ {\mathcal {F}}{\bigl \{}f(t){\bigr \}}.}]
Denoting the Fourier transform by a capital letter corresponding to the letter
of function being transformed (such as f (x) and F(Î¾)) is especially common in
the sciences and engineering. In electronics, omega (Ï) is often used instead
of Î¾ due to its interpretation as angular frequency, sometimes it is written
as F( jÏ), where j is the imaginary_unit, to indicate its relationship with
the Laplace_transform, and sometimes it is written informally as F(2Ïf ) in
order to use ordinary frequency. In some contexts such as particle physics, the
same symbol     f   {\displaystyle f}  [f] may be used for both for a function
as well as it Fourier transform, with the two only distinguished by their
argument:     f (  k  1   +  k  2   )   {\displaystyle f(k_{1}+k_{2})}  [
{\displaystyle f(k_{1}+k_{2})}] would refer to the Fourier transform because of
the momentum argument, while     f (  x  0   + &#x03C0;    r &#x2192;    )
{\displaystyle f(x_{0}+\pi {\vec {r}})}  [{\displaystyle f(x_{0}+\pi {\vec
{r}})}] would refer to the original function because of the positional
argument. Although tildes may be used as in        f &#x007E;
{\displaystyle {\tilde {f}}}  [{\tilde {f}}] to indicate Fourier transforms,
tildes may also be used to indicate a modification of a quantity with a more
Lorentz_invariant form, such as         d k  &#x007E;    =    d k   ( 2
&#x03C0;  )  3   2 &#x03C9;      {\displaystyle {\tilde {dk}}={\frac {dk}{(2\pi
)^{3}2\omega }}}  [{\displaystyle {\tilde {dk}}={\frac {dk}{(2\pi )^{3}2\omega
}}}], so care must be taken.
The interpretation of the complex function fÌ (Î¾) may be aided by expressing
it in polar_coordinate form
            f &#x005E;    ( &#x03BE; ) = A ( &#x03BE; )  e  i &#x03C6;
      ( &#x03BE; )     {\displaystyle {\hat {f}}(\xi )=A(\xi )e^{i\varphi (\xi
      )}}  [{\hat {f}}(\xi )=A(\xi )e^{i\varphi (\xi )}]
in terms of the two real functions A(Î¾) and Ï(Î¾) where:
         A ( &#x03BE; ) =  |     f &#x005E;    ( &#x03BE; )  |  ,
      {\displaystyle A(\xi )=\left|{\hat {f}}(\xi )\right|,}  [{\displaystyle A
      (\xi )=\left|{\hat {f}}(\xi )\right|,}]
is the amplitude and
         &#x03C6; ( &#x03BE; ) = arg &#x2061;  (     f &#x005E;    ( &#x03BE; )
      )  ,   {\displaystyle \varphi (\xi )=\arg \left({\hat {f}}(\xi )\right),}
      [{\displaystyle \varphi (\xi )=\arg \left({\hat {f}}(\xi )\right),}]
is the phase (see arg_function).
Then the inverse transform can be written:
         f ( x ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;   A ( &#x03BE; )
      &#xA0;  e  i   (   2 &#x03C0; &#x03BE; x + &#x03C6; ( &#x03BE; )   )
      d &#x03BE; ,   {\displaystyle f(x)=\int _{-\infty }^{\infty }A(\xi )\ e^
      {i{\bigl (}2\pi \xi x+\varphi (\xi ){\bigr )}}\,d\xi ,}  [{\displaystyle
      f(x)=\int _{-\infty }^{\infty }A(\xi )\ e^{i{\bigl (}2\pi \xi x+\varphi
      (\xi ){\bigr )}}\,d\xi ,}]
which is a recombination of all the frequency components of f (x). Each
component is a complex sinusoid of the form e2ÏixÎ¾ whose amplitude is A(Î¾)
and whose initial phase_angle (at x = 0) is Ï(Î¾).
The Fourier transform may be thought of as a mapping on function spaces. This
mapping is here denoted F and F( f ) is used to denote the Fourier transform of
the function f. This mapping is linear, which means that F can also be seen as
a linear transformation on the function space and implies that the standard
notation in linear algebra of applying a linear transformation to a vector
(here the function f ) can be used to write F f instead of F( f ). Since the
result of applying the Fourier transform is again a function, we can be
interested in the value of this function evaluated at the value Î¾ for its
variable, and this is denoted either as F f (Î¾) or as ( F f )(Î¾). Notice that
in the former case, it is implicitly understood that F is applied first to f
and then the resulting function is evaluated at Î¾, not the other way around.
In mathematics and various applied sciences, it is often necessary to
distinguish between a function f and the value of f when its variable equals x,
denoted f (x). This means that a notation like F( f (x)) formally can be
interpreted as the Fourier transform of the values of f at x. Despite this
flaw, the previous notation appears frequently, often when a particular
function or a function of a particular variable is to be transformed. For
example,
           F     (   rect &#x2061; ( x )   )   = sinc &#x2061; ( &#x03BE; )
      {\displaystyle {\mathcal {F}}{\bigl (}\operatorname {rect} (x){\bigr
      )}=\operatorname {sinc} (\xi )}  [{\displaystyle {\mathcal {F}}{\bigl
      (}\operatorname {rect} (x){\bigr )}=\operatorname {sinc} (\xi )}]
is sometimes used to express that the Fourier transform of a rectangular
function is a sinc_function, or
           F     (   f ( x +  x  0   )   )   =   F     (   f ( x )   )    e  2
      &#x03C0; i &#x03BE;  x  0       {\displaystyle {\mathcal {F}}{\bigl (}f
      (x+x_{0}){\bigr )}={\mathcal {F}}{\bigl (}f(x){\bigr )}e^{2\pi i\xi x_
      {0}}}  [{\displaystyle {\mathcal {F}}{\bigl (}f(x+x_{0}){\bigr )}=
      {\mathcal {F}}{\bigl (}f(x){\bigr )}e^{2\pi i\xi x_{0}}}]
is used to express the shift property of the Fourier transform.
Notice, that the last example is only correct under the assumption that the
transformed function is a function of x, not of x0.
***** Other conventions[edit] *****
The Fourier transform can also be written in terms of angular_frequency:
         &#x03C9; = 2 &#x03C0; &#x03BE; ,   {\displaystyle \omega =2\pi \xi ,}
      [\omega =2\pi \xi ,]
whose units are radians per second.
The substitution Î¾ = Ï/2Ï into the formulas above produces this convention:
            f &#x005E;    ( &#x03C9; ) =  &#x222B;    R   n     f ( x )  e
      &#x2212; i &#x03C9; &#x22C5; x    d x .   {\displaystyle {\hat {f}}
      (\omega )=\int _{\mathbb {R} ^{n}}f(x)e^{-i\omega \cdot x}\,dx.}  [
      {\displaystyle {\hat {f}}(\omega )=\int _{\mathbb {R} ^{n}}f(x)e^{-
      i\omega \cdot x}\,dx.}]
Under this convention, the inverse transform becomes:
         f ( x ) =   1  ( 2 &#x03C0;  )  n       &#x222B;    R   n        f
      &#x005E;    ( &#x03C9; )  e  i &#x03C9; &#x22C5; x    d &#x03C9; .
      {\displaystyle f(x)={\frac {1}{(2\pi )^{n}}}\int _{\mathbb {R} ^{n}}{\hat
      {f}}(\omega )e^{i\omega \cdot x}\,d\omega .}  [{\displaystyle f(x)={\frac
      {1}{(2\pi )^{n}}}\int _{\mathbb {R} ^{n}}{\hat {f}}(\omega )e^{i\omega
      \cdot x}\,d\omega .}]
Unlike the convention followed in this article, when the Fourier transform is
defined this way, it is no longer a unitary_transformation on L2(ân). There
is also less symmetry between the formulas for the Fourier transform and its
inverse.
Another convention is to split the factor of (2Ï)n evenly between the Fourier
transform and its inverse, which leads to definitions:
                f &#x005E;    ( &#x03C9; )    =   1  ( 2 &#x03C0;  )   n 2
      &#x222B;    R   n     f ( x )  e  &#x2212; i &#x03C9; &#x22C5; x    d x ,
      f ( x )    =   1  ( 2 &#x03C0;  )   n 2        &#x222B;    R   n        f
      &#x005E;    ( &#x03C9; )  e  i &#x03C9; &#x22C5; x    d &#x03C9; .
      {\displaystyle {\begin{aligned}{\hat {f}}(\omega )&={\frac {1}{(2\pi )^
      {\frac {n}{2}}}}\int _{\mathbb {R} ^{n}}f(x)e^{-i\omega \cdot x}\,dx,\\f
      (x)&={\frac {1}{(2\pi )^{\frac {n}{2}}}}\int _{\mathbb {R} ^{n}}{\hat
      {f}}(\omega )e^{i\omega \cdot x}\,d\omega .\end{aligned}}}  [
      {\displaystyle {\begin{aligned}{\hat {f}}(\omega )&={\frac {1}{(2\pi )^
      {\frac {n}{2}}}}\int _{\mathbb {R} ^{n}}f(x)e^{-i\omega \cdot x}\,dx,\\f
      (x)&={\frac {1}{(2\pi )^{\frac {n}{2}}}}\int _{\mathbb {R} ^{n}}{\hat
      {f}}(\omega )e^{i\omega \cdot x}\,d\omega .\end{aligned}}}]
Under this convention, the Fourier transform is again a unitary transformation
on L2(ân). It also restores the symmetry between the Fourier transform and
its inverse.
Variations of all three conventions can be created by conjugating the complex-
exponential kernel of both the forward and the reverse transform. The signs
must be opposites. Other than that, the choice is (again) a matter of
convention.
      Summary of popular forms of the Fourier transform, one-dimensional
                                                    f &#x005E;     1
                                         ( &#x03BE; ) &#xA0;        =    d e f
                                         &#xA0;  &#x222B;  &#x2212; &#x221E;
                                         &#x221E;   f ( x ) &#x22C5;  e
                                         &#x2212; 2 &#x03C0; i x &#x22C5;
                                         &#x03BE;    d x =   2 &#x03C0;
                                         &#x22C5;     f &#x005E;     2   ( 2
                                         &#x03C0; &#x03BE; ) =     f &#x005E;
                                         3   ( 2 &#x03C0; &#x03BE; )     f ( x
                                         )    =  &#x222B;  &#x2212; &#x221E;
                                         &#x221E;       f &#x005E;     1
                                         ( &#x03BE; ) &#x22C5;  e  2 &#x03C0; i
                                         x &#x22C5; &#x03BE;    d &#x03BE;
                                         {\displaystyle {\begin{aligned}{\hat
                                         {f}}_{1}(\xi )\ &{\stackrel {\mathrm
ordinary frequency Î¾ (Hz) unitary     {def} }{=}}\ \int _{-\infty }^{\infty
                                         }f(x)\cdot e^{-2\pi ix\cdot \xi }\,dx=
                                         {\sqrt {2\pi }}\cdot {\hat {f}}_{2}
                                         (2\pi \xi )={\hat {f}}_{3}(2\pi \xi
                                         )\\f(x)&=\int _{-\infty }^{\infty }
                                         {\hat {f}}_{1}(\xi )\cdot e^{2\pi
                                         ix\cdot \xi }\,d\xi \end{aligned}}}  [
                                         {\displaystyle {\begin{aligned}{\hat
                                         {f}}_{1}(\xi )\ &{\stackrel {\mathrm
                                         {def} }{=}}\ \int _{-\infty }^{\infty
                                         }f(x)\cdot e^{-2\pi ix\cdot \xi }\,dx=
                                         {\sqrt {2\pi }}\cdot {\hat {f}}_{2}
                                         (2\pi \xi )={\hat {f}}_{3}(2\pi \xi
                                         )\\f(x)&=\int _{-\infty }^{\infty }
                                         {\hat {f}}_{1}(\xi )\cdot e^{2\pi
                                         ix\cdot \xi }\,d\xi \end{aligned}}}]
                                                    f &#x005E;     2
                                         ( &#x03C9; ) &#xA0;        =    d e f
                                         &#xA0;   1  2 &#x03C0;     &#x222B;
                                         &#x2212; &#x221E;   &#x221E;   f ( x )
                                         &#x22C5;  e  &#x2212; i &#x03C9;
                                         &#x22C5; x    d x =   1  2 &#x03C0;
                                         &#x22C5;     f &#x005E;     1
                                         (   &#x03C9;  2 &#x03C0;    )  =   1
                                         2 &#x03C0;    &#x22C5;     f &#x005E;
                                         3   ( &#x03C9; )     f ( x )    =   1
                                         2 &#x03C0;     &#x222B;  &#x2212;
                                         &#x221E;   &#x221E;       f &#x005E;
                                         2   ( &#x03C9; ) &#x22C5;  e  i
                                         &#x03C9; &#x22C5; x    d &#x03C9;
                                         {\displaystyle {\begin{aligned}{\hat
                                         {f}}_{2}(\omega )\ &{\stackrel
                                         {\mathrm {def} }{=}}\ {\frac {1}{\sqrt
                                         {2\pi }}}\int _{-\infty }^{\infty }f
                                         (x)\cdot e^{-i\omega \cdot x}\,dx=
                             unitary     {\frac {1}{\sqrt {2\pi }}}\cdot {\hat
                                         {f}}_{1}\!\left({\frac {\omega }{2\pi
                                         }}\right)={\frac {1}{\sqrt {2\pi
                                         }}}\cdot {\hat {f}}_{3}(\omega )\\f
                                         (x)&={\frac {1}{\sqrt {2\pi }}}\int _
                                         {-\infty }^{\infty }{\hat {f}}_{2}
                                         (\omega )\cdot e^{i\omega \cdot
                                         x}\,d\omega \end{aligned}}}  [
                                         {\displaystyle {\begin{aligned}{\hat
                                         {f}}_{2}(\omega )\ &{\stackrel
                                         {\mathrm {def} }{=}}\ {\frac {1}{\sqrt
                                         {2\pi }}}\int _{-\infty }^{\infty }f
                                         (x)\cdot e^{-i\omega \cdot x}\,dx=
                                         {\frac {1}{\sqrt {2\pi }}}\cdot {\hat
                                         {f}}_{1}\!\left({\frac {\omega }{2\pi
                                         }}\right)={\frac {1}{\sqrt {2\pi
                                         }}}\cdot {\hat {f}}_{3}(\omega )\\f
                                         (x)&={\frac {1}{\sqrt {2\pi }}}\int _
angular frequency Ï (rad/s)           {-\infty }^{\infty }{\hat {f}}_{2}
                                         (\omega )\cdot e^{i\omega \cdot
                                         x}\,d\omega \end{aligned}}}]
                                                    f &#x005E;     3
                                         ( &#x03C9; ) &#xA0;        =    d e f
                                         &#xA0;  &#x222B;  &#x2212; &#x221E;
                                         &#x221E;   f ( x ) &#x22C5;  e
                                         &#x2212; i &#x03C9; &#x22C5; x    d x
                                         =     f &#x005E;     1    (   &#x03C9;
                                         2 &#x03C0;    )  =   2 &#x03C0;
                                         &#x22C5;     f &#x005E;     2
                                         ( &#x03C9; )     f ( x )    =   1  2
                                         &#x03C0;     &#x222B;  &#x2212;
                                         &#x221E;   &#x221E;       f &#x005E;
                                         3   ( &#x03C9; ) &#x22C5;  e  i
                                         &#x03C9; &#x22C5; x    d &#x03C9;
                                         {\displaystyle {\begin{aligned}{\hat
                                         {f}}_{3}(\omega )\ &{\stackrel
                                         {\mathrm {def} }{=}}\ \int _{-\infty
                                         }^{\infty }f(x)\cdot e^{-i\omega \cdot
                             non-unitary x}\,dx={\hat {f}}_{1}\left({\frac
                                         {\omega }{2\pi }}\right)={\sqrt {2\pi
                                         }}\cdot {\hat {f}}_{2}(\omega )\\f
                                         (x)&={\frac {1}{2\pi }}\int _{-\infty
                                         }^{\infty }{\hat {f}}_{3}(\omega
                                         )\cdot e^{i\omega \cdot x}\,d\omega
                                         \end{aligned}}}  [{\displaystyle
                                         {\begin{aligned}{\hat {f}}_{3}(\omega
                                         )\ &{\stackrel {\mathrm {def} }{=}}\
                                         \int _{-\infty }^{\infty }f(x)\cdot e^
                                         {-i\omega \cdot x}\,dx={\hat {f}}_
                                         {1}\left({\frac {\omega }{2\pi
                                         }}\right)={\sqrt {2\pi }}\cdot {\hat
                                         {f}}_{2}(\omega )\\f(x)&={\frac {1}
                                         {2\pi }}\int _{-\infty }^{\infty }
                                         {\hat {f}}_{3}(\omega )\cdot e^
                                         {i\omega \cdot x}\,d\omega \end
                                         {aligned}}}]
                  Generalization for n-dimensional functions
                                                    f &#x005E;     1
                                         ( &#x03BE; ) &#xA0;        =    d e f
                                         &#xA0;  &#x222B;    R   n     f ( x )
                                         e  &#x2212; 2 &#x03C0; i x &#x22C5;
                                         &#x03BE;    d x = ( 2 &#x03C0;  )   n
                                         2        f &#x005E;     2   ( 2
                                         &#x03C0; &#x03BE; ) =     f &#x005E;
                                         3   ( 2 &#x03C0; &#x03BE; )     f ( x
                                         )    =  &#x222B;    R   n         f
                                         &#x005E;     1   ( &#x03BE; )  e  2
                                         &#x03C0; i x &#x22C5; &#x03BE;    d
                                         &#x03BE;       {\displaystyle {\begin
                                         {aligned}{\hat {f}}_{1}(\xi )\ &
                                         {\stackrel {\mathrm {def} }{=}}\ \int
ordinary frequency Î¾ (Hz) unitary     _{\mathbb {R} ^{n}}f(x)e^{-2\pi
                                         ix\cdot \xi }\,dx=(2\pi )^{\frac {n}
                                         {2}}{\hat {f}}_{2}(2\pi \xi )={\hat
                                         {f}}_{3}(2\pi \xi )\\f(x)&=\int _
                                         {\mathbb {R} ^{n}}{\hat {f}}_{1}(\xi
                                         )e^{2\pi ix\cdot \xi }\,d\xi \end
                                         {aligned}}}  [{\displaystyle {\begin
                                         {aligned}{\hat {f}}_{1}(\xi )\ &
                                         {\stackrel {\mathrm {def} }{=}}\ \int
                                         _{\mathbb {R} ^{n}}f(x)e^{-2\pi
                                         ix\cdot \xi }\,dx=(2\pi )^{\frac {n}
                                         {2}}{\hat {f}}_{2}(2\pi \xi )={\hat
                                         {f}}_{3}(2\pi \xi )\\f(x)&=\int _
                                         {\mathbb {R} ^{n}}{\hat {f}}_{1}(\xi
                                         )e^{2\pi ix\cdot \xi }\,d\xi \end
                                         {aligned}}}]
                                                    f &#x005E;     2
                                         ( &#x03C9; ) &#xA0;        =    d e f
                                         &#xA0;   1  ( 2 &#x03C0;  )   n 2
                                         &#x222B;    R   n     f ( x )  e
                                         &#x2212; i &#x03C9; &#x22C5; x    d x
                                         =   1  ( 2 &#x03C0;  )   n 2
                                         f &#x005E;     1     (   &#x03C9;  2
                                         &#x03C0;    )  =   1  ( 2 &#x03C0;  )
                                         n 2           f &#x005E;     3
                                         ( &#x03C9; )     f ( x )    =   1  ( 2
                                         &#x03C0;  )   n 2        &#x222B;    R
                                         n         f &#x005E;     2
                                         ( &#x03C9; )  e  i &#x03C9; &#x22C5; x
                                         d &#x03C9;       {\displaystyle
                                         {\begin{aligned}{\hat {f}}_{2}(\omega
                                         )\ &{\stackrel {\mathrm {def} }{=}}\
                                         {\frac {1}{(2\pi )^{\frac {n}
                                         {2}}}}\int _{\mathbb {R} ^{n}}f(x)e^{-
                                         i\omega \cdot x}\,dx={\frac {1}{(2\pi
                             unitary     )^{\frac {n}{2}}}}{\hat {f}}_
                                         {1}\!\left({\frac {\omega }{2\pi
                                         }}\right)={\frac {1}{(2\pi )^{\frac
                                         {n}{2}}}}{\hat {f}}_{3}(\omega )\\f
                                         (x)&={\frac {1}{(2\pi )^{\frac {n}
                                         {2}}}}\int _{\mathbb {R} ^{n}}{\hat
                                         {f}}_{2}(\omega )e^{i\omega \cdot
                                         x}\,d\omega \end{aligned}}}  [
                                         {\displaystyle {\begin{aligned}{\hat
                                         {f}}_{2}(\omega )\ &{\stackrel
                                         {\mathrm {def} }{=}}\ {\frac {1}{(2\pi
                                         )^{\frac {n}{2}}}}\int _{\mathbb {R} ^
                                         {n}}f(x)e^{-i\omega \cdot x}\,dx=
                                         {\frac {1}{(2\pi )^{\frac {n}{2}}}}
                                         {\hat {f}}_{1}\!\left({\frac {\omega }
                                         {2\pi }}\right)={\frac {1}{(2\pi )^
angular frequency Ï (rad/s)           {\frac {n}{2}}}}{\hat {f}}_{3}(\omega
                                         )\\f(x)&={\frac {1}{(2\pi )^{\frac {n}
                                         {2}}}}\int _{\mathbb {R} ^{n}}{\hat
                                         {f}}_{2}(\omega )e^{i\omega \cdot
                                         x}\,d\omega \end{aligned}}}]
                                                    f &#x005E;     3
                                         ( &#x03C9; ) &#xA0;        =    d e f
                                         &#xA0;  &#x222B;    R   n     f ( x )
                                         e  &#x2212; i &#x03C9; &#x22C5; x    d
                                         x =     f &#x005E;     1
                                         (   &#x03C9;  2 &#x03C0;    )  = ( 2
                                         &#x03C0;  )   n 2        f &#x005E;
                                         2   ( &#x03C9; )     f ( x )    =   1
                                         ( 2 &#x03C0;  )  n       &#x222B;    R
                                         n         f &#x005E;     3
                                         ( &#x03C9; )  e  i &#x03C9; &#x22C5; x
                                         d &#x03C9;       {\displaystyle
                                         {\begin{aligned}{\hat {f}}_{3}(\omega
                                         )\ &{\stackrel {\mathrm {def} }{=}}\
                                         \int _{\mathbb {R} ^{n}}f(x)e^{-
                             non-unitary i\omega \cdot x}\,dx={\hat {f}}_
                                         {1}\left({\frac {\omega }{2\pi
                                         }}\right)=(2\pi )^{\frac {n}{2}}{\hat
                                         {f}}_{2}(\omega )\\f(x)&={\frac {1}{
                                         (2\pi )^{n}}}\int _{\mathbb {R} ^{n}}
                                         {\hat {f}}_{3}(\omega )e^{i\omega
                                         \cdot x}\,d\omega \end{aligned}}}  [
                                         {\displaystyle {\begin{aligned}{\hat
                                         {f}}_{3}(\omega )\ &{\stackrel
                                         {\mathrm {def} }{=}}\ \int _{\mathbb
                                         {R} ^{n}}f(x)e^{-i\omega \cdot x}\,dx=
                                         {\hat {f}}_{1}\left({\frac {\omega }
                                         {2\pi }}\right)=(2\pi )^{\frac {n}{2}}
                                         {\hat {f}}_{2}(\omega )\\f(x)&={\frac
                                         {1}{(2\pi )^{n}}}\int _{\mathbb {R} ^
                                         {n}}{\hat {f}}_{3}(\omega )e^{i\omega
                                         \cdot x}\,d\omega \end{aligned}}}]
As discussed above, the characteristic_function of a random variable is the
same as the FourierâStieltjes_transform of its distribution measure, but in
this context it is typical to take a different convention for the constants.
Typically characteristic function is defined
         E  (  e  i t &#x22C5; X   )  = &#x222B;  e  i t &#x22C5; x    d
      &#x03BC;  X   ( x ) .   {\displaystyle E\left(e^{it\cdot X}\right)=\int
      e^{it\cdot x}\,d\mu _{X}(x).}  [{\displaystyle E\left(e^{it\cdot
      X}\right)=\int e^{it\cdot x}\,d\mu _{X}(x).}]
As in the case of the "non-unitary angular frequency" convention above, the
factor of 2Ï appears in neither the normalizing constant nor the exponent.
Unlike any of the conventions appearing above, this convention takes the
opposite sign in the exponent.
***** Computation methods[edit] *****
The appropriate computation method largely depends how the original
mathematical function is represented and the desired form of the output
function.
Since the fundamental definition of a Fourier transform is an integral,
functions that can be expressed as closed-form_expressions are commonly
computed by working the integral analytically to yield a closed-form expression
in the Fourier transform conjugate variable as the result. This is the method
used to generate tables of Fourier transforms,[45] including those found in the
table below (Fourier_transform#Tables_of_important_Fourier_transforms).
Many computer algebra systems such as Matlab and Mathematica that are capable
of symbolic_integration are capable of computing Fourier transforms
analytically. For example, to compute the Fourier transform of f (t) = cos
(6Ït) eâÏt2 one might enter the command integrate cos(6*pi*t) exp
(âpi*t^2) exp(-i*2*pi*f*t) from -inf to inf into Wolfram_Alpha.
**** Numerical integration of closed-form functions[edit] ****
If the input function is in closed-form and the desired output function is a
series of ordered pairs (for example a table of values from which a graph can
be generated) over a specified domain, then the Fourier transform can be
generated by numerical_integration at each value of the Fourier conjugate
variable (frequency, for example) for which a value of the output variable is
desired.[46] Note that this method requires computing a separate numerical
integration for each value of frequency for which a value of the Fourier
transform is desired.[47][48] The numerical integration approach works on a
much broader class of functions than the analytic approach, because it yields
results for functions that do not have closed form Fourier transform integrals.
**** Numerical integration of a series of ordered pairs[edit] ****
If the input function is a series of ordered pairs (for example, a time series
from measuring an output variable repeatedly over a time interval) then the
output function must also be a series of ordered pairs (for example, a complex
number vs. frequency over a specified domain of frequencies), unless certain
assumptions and approximations are made allowing the output function to be
approximated by a closed-form expression. In the general case where the
available input series of ordered pairs are assumed be samples representing a
continuous function over an interval (amplitude vs. time, for example), the
series of ordered pairs representing the desired output function can be
obtained by numerical integration of the input data over the available interval
at each value of the Fourier conjugate variable (frequency, for example) for
which the value of the Fourier transform is desired.[49]
Explicit numerical integration over the ordered pairs can yield the Fourier
transform output value for any desired value of the conjugate Fourier transform
variable (frequency, for example), so that a spectrum can be produced at any
desired step size and over any desired variable range for accurate
determination of amplitudes, frequencies, and phases corresponding to isolated
peaks. Unlike limitations in DFT and FFT methods, explicit numerical
integration can have any desired step size and compute the Fourier transform
over any desired range of the conjugate Fourier transform variable (for
example, frequency).
**** Discrete Fourier transforms and fast Fourier transforms[edit] ****
If the ordered pairs representing the original input function are equally
spaced in their input variable (for example, equal time steps), then the
Fourier transform is known as a discrete_Fourier_transform (DFT), which can be
computed either by explicit numerical integration, by explicit evaluation of
the DFT definition, or by fast_Fourier_transform (FFT) methods. In contrast to
explicit integration of input data, use of the DFT and FFT methods produces
Fourier transforms described by ordered pairs of step size equal to the
reciprocal of the original sampling interval. For example, if the input data is
sampled every 10 seconds, the output of DFT and FFT methods will have a 0.1 Hz
frequency spacing.
***** Tables of important Fourier transforms[edit] *****
The following tables record some closed-form Fourier transforms. For functions
f (x), g(x) and h(x) denote their Fourier transforms by fÌ, Ä, and Ä¥
respectively. Only the three most common conventions are included. It may be
useful to notice that entry 105 gives a relationship between the Fourier
transform of a function and the original function, which can be seen as
relating the Fourier transform and its inverse.
**** Functional relationships, one-dimensional[edit] ****
The Fourier transforms in this table may be found in ErdÃ©lyi_(1954) or Kammler
(2000, appendix).
                                Fourier         Fourier
                                transform       transform       Fourier transform
    Function                    unitary,        unitary,        non-unitary, angular    Remarks
                                ordinary        angular         frequency
                                frequency       frequency
                                                           f
                                                &#x005E;
                                                ( &#x03C9; )
                                           f    =   1  2
                                &#x005E;        &#x03C0;
                                ( &#x03BE; )    &#x222B;
                                =  &#x222B;     &#x2212;
                                &#x2212;        &#x221E;
                                &#x221E;        &#x221E;   f
                                &#x221E;   f    ( x )  e                   f &#x005E;
                                ( x )  e        &#x2212; i      ( &#x03BD; )       =
                                &#x2212; 2      &#x03C9; x    d &#x222B;  &#x2212;
                                &#x03C0; i x    x               &#x221E;   &#x221E;   f
                                &#x03BE;    d x {\displaystyle  ( x )  e  &#x2212; i
                                {\displaystyle  {\begin         &#x03BD; x    d x
                                {\begin         {aligned}&{\hat {\displaystyle {\begin
                                {aligned}&{\hat {f}}(\omega     {aligned}&{\hat {f}}
       f ( x )                  {f}}(\xi        )\\&={\frac {1} (\nu )\\&=\int _{-
    {\displaystyle f(x)\,}  [   )\\&=\int _{-   {\sqrt {2\pi    \infty }^{\infty }f     Definition
    {\displaystyle f(x)\,}]     \infty }^       }}}\int _{-     (x)e^{-i\nu x}\,dx\end
                                {\infty }f(x)e^ \infty }^       {aligned}}}  [
                                {-2\pi ix\xi    {\infty }f(x)e^ {\displaystyle {\begin
                                }\,dx\end       {-i\omega       {aligned}&{\hat {f}}
                                {aligned}}}  [  x}\,dx\end      (\nu )\\&=\int _{-
                                {\displaystyle  {aligned}}}  [  \infty }^{\infty }f
                                {\begin         {\displaystyle  (x)e^{-i\nu x}\,dx\end
                                {aligned}&{\hat {\begin         {aligned}}}]
                                {f}}(\xi        {aligned}&{\hat
                                )\\&=\int _{-   {f}}(\omega
                                \infty }^       )\\&={\frac {1}
                                {\infty }f(x)e^ {\sqrt {2\pi
                                {-2\pi ix\xi    }}}\int _{-
                                }\,dx\end       \infty }^
                                {aligned}}}]    {\infty }f(x)e^
                                                {-i\omega
                                                x}\,dx\end
                                                {aligned}}}]
                                                   a &#x22C5;
                                   a &#x22C5;   f &#x005E;
                                f &#x005E;      ( &#x03C9; ) +
                                ( &#x03BE; ) +  b &#x22C5;    g    a &#x22C5;    f
                                b &#x22C5;    g &#x005E;        &#x005E;    ( &#x03BD;
                                &#x005E;        ( &#x03C9; )    ) + b &#x22C5;    g
       a &#x22C5; f ( x ) + b   ( &#x03BE; )    {\displaystyle  &#x005E;    ( &#x03BD;
    &#x22C5; g ( x )            {\displaystyle  a\cdot {\hat    )    {\displaystyle
101 {\displaystyle a\cdot f     a\cdot {\hat    {f}}(\omega     a\cdot {\hat {f}}(\nu   Linearity
    (x)+b\cdot g(x)\,}  [       {f}}(\xi        )+b\cdot {\hat  )+b\cdot {\hat {g}}(\nu
    {\displaystyle a\cdot f     )+b\cdot {\hat  {g}}(\omega     )\,}  [{\displaystyle
    (x)+b\cdot g(x)\,}]         {g}}(\xi )\,}   )\,}  [         a\cdot {\hat {f}}(\nu
                                [{\displaystyle {\displaystyle  )+b\cdot {\hat {g}}(\nu
                                a\cdot {\hat    a\cdot {\hat    )\,}]
                                {f}}(\xi        {f}}(\omega
                                )+b\cdot {\hat  )+b\cdot {\hat
                                {g}}(\xi )\,}]  {g}}(\omega
                                                )\,}]
                                    e  &#x2212;     e  &#x2212;
                                2 &#x03C0; i a  i a &#x03C9;
                                &#x03BE;      f f &#x005E;          e  &#x2212; i a
                                &#x005E;        ( &#x03C9; )    &#x03BD;      f
                                ( &#x03BE; )    {\displaystyle  &#x005E;    ( &#x03BD;
       f ( x &#x2212; a )       {\displaystyle  e^{-ia\omega }  )    {\displaystyle e^
102 {\displaystyle f(x-a)\,}  [ e^{-2\pi ia\xi  {\hat {f}}      {-ia\nu }{\hat {f}}(\nu Shift in time domain
    {\displaystyle f(x-a)\,}]   }{\hat {f}}(\xi (\omega )\,}  [ )\,}  [{\displaystyle
                                )\,}  [         {\displaystyle  e^{-ia\nu }{\hat {f}}
                                {\displaystyle  e^{-ia\omega }  (\nu )\,}]
                                e^{-2\pi ia\xi  {\hat {f}}
                                }{\hat {f}}(\xi (\omega )\,}]
                                )\,}]
                                      f
                                &#x005E;
                                (  &#x03BE;           f
                                &#x2212;   a  2 &#x005E;
                                &#x03C0;     )  ( &#x03C9;            f &#x005E;
       f ( x )  e  i a x        {\displaystyle  &#x2212; a )    ( &#x03BD; &#x2212; a )
    {\displaystyle f(x)e^       {\hat {f}}\left {\displaystyle  {\displaystyle {\hat
103 {iax}\,}  [{\displaystyle f (\xi -{\frac    {\hat {f}}      {f}}(\nu -a)\,}  [      Shift in frequency domain, dual of 102
    (x)e^{iax}\,}]              {a}{2\pi        (\omega -a)\,}  {\displaystyle {\hat
                                }}\right)\,}  [ [{\displaystyle {f}}(\nu -a)\,}]
                                {\displaystyle  {\hat {f}}
                                {\hat {f}}\left (\omega -a)\,}]
                                (\xi -{\frac
                                {a}{2\pi
                                }}\right)\,}]
                                     1   |  a        1   |  a
                                |        f      |        f
                                &#x005E;        &#x005E;
                                (   &#x03BE; a  (   &#x03C9; a       1   |  a  |
                                )               )               f &#x005E;
                                {\displaystyle  {\displaystyle  (   &#x03BD; a   )
                                {\frac {1}      {\frac {1}      {\displaystyle {\frac   Scaling in the time domain. If |a| is large, then f (ax) is concentrated
       f ( a x )                {|a|}}{\hat     {|a|}}{\hat     {1}{|a|}}{\hat          around 0 and
104 {\displaystyle f(ax)\,}  [  {f}}\left(      {f}}\left(      {f}}\left({\frac {\nu }      1   |  a  |        f &#x005E;     (   &#x03C9; a   )     {\displaystyle
    {\displaystyle f(ax)\,}]    {\frac {\xi }   {\frac {\omega  {a}}\right)\,}  [       {\frac {1}{|a|}}{\hat {f}}\left({\frac {\omega }{a}}\right)\,}  [
                                {a}}\right)\,}  }{a}}\right)\,} {\displaystyle {\frac   {\displaystyle {\frac {1}{|a|}}{\hat {f}}\left({\frac {\omega }{a}}\right)\,}]
                                [{\displaystyle [{\displaystyle {1}{|a|}}{\hat          spreads out and flattens.
                                {\frac {1}      {\frac {1}      {f}}\left({\frac {\nu }
                                {|a|}}{\hat     {|a|}}{\hat     {a}}\right)\,}]
                                {f}}\left(      {f}}\left(
                                {\frac {\xi }   {\frac {\omega
                                {a}}\right)\,}] }
                                                {a}}\right)\,}]
                                   f ( &#x2212;    f ( &#x2212;    2 &#x03C0; f
          f &#x005E;    ( x )   &#x03BE; )      &#x03C9; )      ( &#x2212; &#x03BD; )   Duality. Here fÌ needs to be calculated using the same method as Fourier
105 {\displaystyle {\hat {f}}   {\displaystyle  {\displaystyle  {\displaystyle 2\pi f(- transform column. Results from swapping "dummy" variables of x and Î¾ or Ï or
    (x)\,}  [{\displaystyle     f(-\xi )\,}  [  f(-\omega )\,}  \nu )\,}  [             Î½.
    {\hat {f}}(x)\,}]           {\displaystyle  [{\displaystyle {\displaystyle 2\pi f(-
                                f(-\xi )\,}]    f(-\omega )\,}] \nu )\,}]
                                   ( 2 &#x03C0;    ( i &#x03C9;
                                i &#x03BE;  )   )  n      f
                                n      f        &#x005E;           ( i &#x03BD;  )  n
           d  n   f ( x )   d   &#x005E;        ( &#x03C9; )    f &#x005E;
    x  n         {\displaystyle ( &#x03BE; )    {\displaystyle  ( &#x03BD; )
    {\frac {d^{n}f(x)}{dx^      {\displaystyle  (i\omega )^{n}  {\displaystyle (i\nu )^
106 {n}}}\,}  [{\displaystyle   (2\pi i\xi )^   {\hat {f}}      {n}{\hat {f}}(\nu )\,}
    {\frac {d^{n}f(x)}{dx^      {n}{\hat {f}}   (\omega )\,}  [ [{\displaystyle (i\nu
    {n}}}\,}]                   (\xi )\,}  [    {\displaystyle  )^{n}{\hat {f}}(\nu
                                {\displaystyle  (i\omega )^{n}  )\,}]
                                (2\pi i\xi )^   {\hat {f}}
                                {n}{\hat {f}}   (\omega )\,}]
                                (\xi )\,}]
                                     (   i  2
                                &#x03C0;    )
                                n       d  n        i  n
                                f &#x005E;      d  n      f
                                ( &#x03BE; )    &#x005E;
                                d  &#x03BE;  n  ( &#x03C9; )
                                {\displaystyle  d  &#x03C9;  n      i  n       d  n
                                \left({\frac    {\displaystyle  f &#x005E;
                                {i}{2\pi        i^{n}{\frac {d^ ( &#x03BD; )   d
        x  n   f ( x )          }}\right)^{n}   {n}{\hat {f}}   &#x03BD;  n
107 {\displaystyle x^{n}f(x)\,} {\frac {d^{n}   (\omega )}      {\displaystyle i^{n}    This is the dual of 106
    [{\displaystyle x^{n}f      {\hat {f}}(\xi  {d\omega ^      {\frac {d^{n}{\hat {f}}
    (x)\,}]                     )}{d\xi ^       {n}}}}  [       (\nu )}{d\nu ^{n}}}}  [
                                {n}}}\,}  [     {\displaystyle  {\displaystyle i^{n}
                                {\displaystyle  i^{n}{\frac {d^ {\frac {d^{n}{\hat {f}}
                                \left({\frac    {n}{\hat {f}}   (\nu )}{d\nu ^{n}}}}]
                                {i}{2\pi        (\omega )}
                                }}\right)^{n}   {d\omega ^
                                {\frac {d^{n}   {n}}}}]
                                {\hat {f}}(\xi
                                )}{d\xi ^
                                {n}}}\,}]
                                                     2 &#x03C0;
                                                f &#x005E;
                                      f         ( &#x03C9; )
                                &#x005E;        g &#x005E;
                                ( &#x03BE; )    ( &#x03C9; )          f &#x005E;
                                g &#x005E;      {\displaystyle  ( &#x03BD; )    g
       ( f &#x2217; g ) ( x )   ( &#x03BE; )    {\sqrt {2\pi }} &#x005E;    ( &#x03BD;
    {\displaystyle (f*g)(x)\,}  {\displaystyle  {\hat {f}}      )    {\displaystyle     The notation f â g denotes the convolution of f and g â this rule is the
108 [{\displaystyle (f*g)       {\hat {f}}(\xi  (\omega ){\hat  {\hat {f}}(\nu ){\hat   convolution_theorem
    (x)\,}]                     ){\hat {g}}(\xi {g}}(\omega     {g}}(\nu )\,}  [
                                )\,}  [         )\,}  [         {\displaystyle {\hat
                                {\displaystyle  {\displaystyle  {f}}(\nu ){\hat {g}}
                                {\hat {f}}(\xi  {\sqrt {2\pi }} (\nu )\,}]
                                ){\hat {g}}(\xi {\hat {f}}
                                )\,}]           (\omega ){\hat
                                                {g}}(\omega
                                                )\,}]
                                                     1  2
                                                &#x03C0;
                                                (     f
                                    (     f     &#x005E;
                                &#x005E;        &#x2217;    g        1  2 &#x03C0;
                                &#x2217;    g   &#x005E;     )  (     f &#x005E;
                                &#x005E;     )  ( &#x03C9; )    &#x2217;    g &#x005E;
                                ( &#x03BE; )    {\displaystyle  )  ( &#x03BD; )
       f ( x ) g ( x )          {\displaystyle  {\frac {1}      {\displaystyle {\frac
    {\displaystyle f(x)g(x)\,}  \left({\hat     {\sqrt {2\pi    {1}{2\pi }}\left({\hat
109 [{\displaystyle f(x)g       {f}}*{\hat      }}}\left({\hat  {f}}*{\hat {g}}\right)  This is the dual of 108
    (x)\,}]                     {g}}\right)(\xi {f}}*{\hat      (\nu )\,}  [
                                )\,}  [         {g}}\right)     {\displaystyle {\frac
                                {\displaystyle  (\omega )\,}  [ {1}{2\pi }}\left({\hat
                                \left({\hat     {\displaystyle  {f}}*{\hat {g}}\right)
                                {f}}*{\hat      {\frac {1}      (\nu )\,}]
                                {g}}\right)(\xi {\sqrt {2\pi
                                )\,}]           }}}\left({\hat
                                                {f}}*{\hat
                                                {g}}\right)
                                                (\omega )\,}]
                                                      f
                                      f         &#x005E;
                                &#x005E;        ( &#x2212;
                                ( &#x2212;      &#x03C9; ) =
                                &#x03BE; ) =    f &#x005E;            f &#x005E;
                                f &#x005E;      ( &#x03C9; )    ( &#x2212; &#x03BD; ) =
                                ( &#x03BE; )    &#x00AF;        f &#x005E;
                                &#x00AF;        {\displaystyle  ( &#x03BD; )  &#x00AF;
                                {\displaystyle  {\hat {f}}(-    {\displaystyle {\hat
110 For f (x) purely real     {\hat {f}}(-\xi \omega )=       {f}}(-\nu )={\overline  Hermitian symmetry. z indicates the complex_conjugate.
                                )={\overline {  {\overline {    {{\hat {f}}(\nu )}}\,}
                                {\hat {f}}(\xi  {\hat {f}}      [{\displaystyle {\hat
                                )}}\,}  [       (\omega )}}\,}  {f}}(-\nu )={\overline
                                {\displaystyle  [{\displaystyle {{\hat {f}}(\nu )}}\,}]
                                {\hat {f}}(-\xi {\hat {f}}(-
                                )={\overline {  \omega )=
                                {\hat {f}}(\xi  {\overline {
                                )}}\,}]         {\hat {f}}
                                                (\omega )}}\,}]
111 For f (x) purely real and  fÌ (Î¾), fÌ (Ï) and fÌ (Î½) are purely real even
    even                                              functions.
112 For f (x) purely real and  fÌ (Î¾), fÌ (Ï) and fÌ (Î½) are purely imaginary
    odd                                             odd_functions.
                                                      f
                                      f         &#x005E;
                                &#x005E;        ( &#x2212;
                                ( &#x2212;      &#x03C9; ) =
                                &#x03BE; ) =    &#x2212;              f &#x005E;
                                &#x2212;        f &#x005E;      ( &#x2212; &#x03BD; ) =
                                f &#x005E;      ( &#x03C9; )    &#x2212;       f
                                ( &#x03BE; )    &#x00AF;        &#x005E;    ( &#x03BD;
                                &#x00AF;        {\displaystyle  )  &#x00AF;
113 For f (x) purely imaginary{\displaystyle  {\hat {f}}(-    {\displaystyle {\hat    z indicates the complex_conjugate.
                                {\hat {f}}(-\xi \omega )=-      {f}}(-\nu )=-{\overline
                                )=-{\overline { {\overline {    {{\hat {f}}(\nu )}}\,}
                                {\hat {f}}(\xi  {\hat {f}}      [{\displaystyle {\hat
                                )}}\,}  [       (\omega )}}\,}  {f}}(-\nu )=-{\overline
                                {\displaystyle  [{\displaystyle {{\hat {f}}(\nu )}}\,}]
                                {\hat {f}}(-\xi {\hat {f}}(-
                                )=-{\overline { \omega )=-
                                {\hat {f}}(\xi  {\overline {
                                )}}\,}]         {\hat {f}}
                                                (\omega )}}\,}]
                                         f               f
                                &#x005E;        &#x005E;
                                ( &#x2212;      ( &#x2212;               f &#x005E;
                                &#x03BE; )      &#x03C9; )      ( &#x2212; &#x03BD; )
          f ( x )  &#x00AF;     &#x00AF;        &#x00AF;        &#x00AF;
    {\displaystyle {\overline   {\displaystyle  {\displaystyle  {\displaystyle
114 {f(x)}}}  [{\displaystyle   {\overline {    {\overline {    {\overline {{\hat {f}}  Complex_conjugation, generalization of 110 and 113
    {\overline {f(x)}}}]        {\hat {f}}(-\xi {\hat {f}}(-    (-\nu )}}}  [
                                )}}}  [         \omega )}}}  [  {\displaystyle
                                {\displaystyle  {\displaystyle  {\overline {{\hat {f}}
                                {\overline {    {\overline {    (-\nu )}}}]
                                {\hat {f}}(-\xi {\hat {f}}(-
                                )}}}]           \omega )}}}]
                                         f
                                &#x005E;
                                (  &#x03BE;
                                &#x2212;   a  2          f
                                &#x03C0;     )  &#x005E;
                                +    f &#x005E; ( &#x03C9;
                                (  &#x03BE; +   &#x2212; a ) +
                                a  2 &#x03C0;   f &#x005E;               f &#x005E;
                                )   2           ( &#x03C9; + a  ( &#x03BD; &#x2212; a )
                                {\displaystyle  )  2            +    f &#x005E;
       f ( x ) cos &#x2061; ( a {\frac {{\hat   {\displaystyle  ( &#x03BD; + a )  2
    x )   {\displaystyle f      {f}}\left(\xi - {\frac {{\hat   {\displaystyle {\frac { This follows from rules 101 and 103 using Euler's_formula:
115 (x)\cos(ax)}  [             {\frac {a}{2\pi {f}}(\omega -   {\hat {f}}(\nu -a)+        cos &#x2061; ( a x ) =     e  i a x   +  e  &#x2212; i a x    2   .
    {\displaystyle f(x)\cos     }}\right)+{\hat a)+{\hat {f}}   {\hat {f}}(\nu +a)}     {\displaystyle \cos(ax)={\frac {e^{iax}+e^{-iax}}{2}}.}  [{\displaystyle \cos
    (ax)}]                      {f}}\left(\xi + (\omega +a)}    {2}}}  [{\displaystyle  (ax)={\frac {e^{iax}+e^{-iax}}{2}}.}]
                                {\frac {a}{2\pi {2}}\,}  [      {\frac {{\hat {f}}(\nu
                                }}\right)}{2}}} {\displaystyle  -a)+{\hat {f}}(\nu +a)}
                                [{\displaystyle {\frac {{\hat   {2}}}]
                                {\frac {{\hat   {f}}(\omega -
                                {f}}\left(\xi - a)+{\hat {f}}
                                {\frac {a}{2\pi (\omega +a)}
                                }}\right)+{\hat {2}}\,}]
                                {f}}\left(\xi +
                                {\frac {a}{2\pi
                                }}\right)}
                                {2}}}]
                                         f
                                &#x005E;
                                (  &#x03BE;
                                &#x2212;   a  2
                                &#x03C0;     )           f
                                &#x2212;    f   &#x005E;
                                &#x005E;        ( &#x03C9;
                                (  &#x03BE; +   &#x2212; a )
                                a  2 &#x03C0;   &#x2212;    f            f &#x005E;
                                )    2 i        &#x005E;        ( &#x03BD; &#x2212; a )
                                {\displaystyle  ( &#x03C9; + a  &#x2212;    f &#x005E;
       f ( x ) sin &#x2061; ( a {\frac {{\hat   )   2 i         ( &#x03BD; + a )   2 i
    x )   {\displaystyle f      {f}}\left(\xi - {\displaystyle  {\displaystyle {\frac { This follows from 101 and 103 using Euler's_formula:
116 (x)\sin(ax)}  [             {\frac {a}{2\pi {\frac {{\hat   {\hat {f}}(\nu -a)-        sin &#x2061; ( a x ) =     e  i a x   &#x2212;  e  &#x2212; i a x     2 i
    {\displaystyle f(x)\sin     }}\right)-{\hat {f}}(\omega -   {\hat {f}}(\nu +a)}     .   {\displaystyle \sin(ax)={\frac {e^{iax}-e^{-iax}}{2i}}.}  [{\displaystyle
    (ax)}]                      {f}}\left(\xi + a)-{\hat {f}}   {2i}}}  [{\displaystyle \sin(ax)={\frac {e^{iax}-e^{-iax}}{2i}}.}]
                                {\frac {a}{2\pi (\omega +a)}    {\frac {{\hat {f}}(\nu
                                }}\right)}      {2i}}}  [       -a)-{\hat {f}}(\nu +a)}
                                {2i}}}  [       {\displaystyle  {2i}}}]
                                {\displaystyle  {\frac {{\hat
                                {\frac {{\hat   {f}}(\omega -
                                {f}}\left(\xi - a)-{\hat {f}}
                                {\frac {a}{2\pi (\omega +a)}
                                }}\right)-{\hat {2i}}}]
                                {f}}\left(\xi +
                                {\frac {a}{2\pi
                                }}\right)}
                                {2i}}}]
**** Square-integrable functions, one-dimensional[edit] ****
The Fourier transforms in this table may be found in Campbell_&_Foster_(1948),
ErdÃ©lyi_(1954), or Kammler_(2000, appendix).
                   Fourier transform Fourier transform  Fourier transform
    Function                         unitary, angular                     Remarks
                   unitary, ordinary frequency          non-unitary,
                   frequency                            angular frequency
                                                f
                                     &#x005E;
                              f      ( &#x03C9; )                  f
                   &#x005E;          =   1  2 &#x03C0;  &#x005E;
                   ( &#x03BE; )      &#x222B;  &#x2212; ( &#x03BD; )
                   =  &#x222B;       &#x221E;           =  &#x222B;
                   &#x2212; &#x221E; &#x221E;   f ( x ) &#x2212; &#x221E;
                   &#x221E;   f ( x  e  &#x2212; i      &#x221E;   f ( x
                   )  e  &#x2212; 2  &#x03C9; x    d x  )  e  &#x2212; i
                   &#x03C0; i x      {\displaystyle     &#x03BD; x    d x
                   &#x03BE;    d x   {\begin{aligned}&  {\displaystyle
                   {\displaystyle    {\hat {f}}(\omega  {\begin{aligned}&
       f ( x )     {\begin{aligned}& )\\&={\frac {1}    {\hat {f}}(\nu
    {\displaystyle {\hat {f}}(\xi    {\sqrt {2\pi       )\\&=\int _{-
    f(x)\,}  [     )\\&=\int _{-     }}}\int _{-\infty  \infty }^{\infty
    {\displaystyle \infty }^{\infty  }^{\infty }f(x)e^  }f(x)e^{-i\nu
    f(x)\,}]       }f(x)e^{-2\pi     {-i\omega          x}\,dx\end
                   ix\xi }\,dx\end   x}\,dx\end         {aligned}}}  [
                   {aligned}}}  [    {aligned}}}  [     {\displaystyle
                   {\displaystyle    {\displaystyle     {\begin{aligned}&
                   {\begin{aligned}& {\begin{aligned}&  {\hat {f}}(\nu
                   {\hat {f}}(\xi    {\hat {f}}(\omega  )\\&=\int _{-
                   )\\&=\int _{-     )\\&={\frac {1}    \infty }^{\infty
                   \infty }^{\infty  {\sqrt {2\pi       }f(x)e^{-i\nu
                   }f(x)e^{-2\pi     }}}\int _{-\infty  x}\,dx\end
                   ix\xi }\,dx\end   }^{\infty }f(x)e^  {aligned}}}]
                   {aligned}}}]      {-i\omega
                                     x}\,dx\end
                                     {aligned}}}]
                                          1  2 &#x03C0;      1   |  a  |
                        1   |  a  |  a  2      &#x22C5; &#x22C5; sinc
                   &#x22C5; sinc     sinc &#x2061;      &#x2061;
                   &#x2061;          (   &#x03C9;  2    (   &#x03BD;  2
                   (   &#x03BE; a    &#x03C0; a    )    &#x03C0; a    )
       rect        )                 {\displaystyle     {\displaystyle
    &#x2061; ( a x {\displaystyle    {\frac {1}{\sqrt   {\frac {1}
    )              {\frac {1}        {2\pi a^           {|a|}}\cdot
    {\displaystyle {|a|}}\cdot       {2}}}}\cdot        \operatorname
    \operatorname  \operatorname     \operatorname      {sinc} \left(     The rectangular_pulse and the normalized sinc_function, here defined as sinc(x)
201 {rect} (ax)\,} {sinc} \left(     {sinc} \left(      {\frac {\nu }     = sin(Ïx)/Ïx
    [              {\frac {\xi }     {\frac {\omega }   {2\pi a}}\right)}
    {\displaystyle {a}}\right)}  [   {2\pi a}}\right)}  [{\displaystyle
    \operatorname  {\displaystyle    [{\displaystyle    {\frac {1}
    {rect}         {\frac {1}        {\frac {1}{\sqrt   {|a|}}\cdot
    (ax)\,}]       {|a|}}\cdot       {2\pi a^           \operatorname
                   \operatorname     {2}}}}\cdot        {sinc} \left(
                   {sinc} \left(     \operatorname      {\frac {\nu }
                   {\frac {\xi }     {sinc} \left(      {2\pi
                   {a}}\right)}]     {\frac {\omega }   a}}\right)}]
                                     {2\pi a}}\right)}]
                                          1  2 &#x03C0;      1   |  a  |
                        1   |  a  |  a  2      &#x22C5; &#x22C5; rect
                   &#x22C5; rect     rect &#x2061;      &#x2061;
                   &#x2061;          (   &#x03C9;  2    (   &#x03BD;  2
                   (   &#x03BE; a    &#x03C0; a    )    &#x03C0; a    )
       sinc        )                 {\displaystyle     {\displaystyle
    &#x2061; ( a x {\displaystyle    {\frac {1}{\sqrt   {\frac {1}
    )              {\frac {1}        {2\pi a^           {|a|}}\cdot
    {\displaystyle {|a|}}\cdot       {2}}}}\cdot        \operatorname
    \operatorname  \operatorname     \operatorname      {rect} \left(     Dual of rule 201. The rectangular_function is an ideal low-pass_filter, and the
202 {sinc} (ax)\,} {rect} \left(     {rect} \left(      {\frac {\nu }     sinc_function is the non-causal impulse response of such a filter. The sinc
    [              {\frac {\xi }     {\frac {\omega }   {2\pi a}}\right)} function is defined here as sinc(x) = sin(Ïx)/Ïx
    {\displaystyle {a}}\right)\,}  [ {2\pi a}}\right)}  [{\displaystyle
    \operatorname  {\displaystyle    [{\displaystyle    {\frac {1}
    {sinc}         {\frac {1}        {\frac {1}{\sqrt   {|a|}}\cdot
    (ax)\,}]       {|a|}}\cdot       {2\pi a^           \operatorname
                   \operatorname     {2}}}}\cdot        {rect} \left(
                   {rect} \left(     \operatorname      {\frac {\nu }
                   {\frac {\xi }     {rect} \left(      {2\pi
                   {a}}\right)\,}]   {\frac {\omega }   a}}\right)}]
                                     {2\pi a}}\right)}]
                                          1  2 &#x03C0;      1   |  a  |
                        1   |  a  |  a  2      &#x22C5; &#x22C5; tri
                   &#x22C5; tri      tri &#x2061;       &#x2061;
                   &#x2061;          (   &#x03C9;  2    (   &#x03BD;  2
                   (   &#x03BE; a    &#x03C0; a    )    &#x03C0; a    )
        sinc  2    )                 {\displaystyle     {\displaystyle
    &#x2061; ( a x {\displaystyle    {\frac {1}{\sqrt   {\frac {1}
    )              {\frac {1}        {2\pi a^           {|a|}}\cdot
    {\displaystyle {|a|}}\cdot       {2}}}}\cdot        \operatorname
    \operatorname  \operatorname     \operatorname      {tri} \left(
203 {sinc} ^{2}    {tri} \left(      {tri} \left({\frac {\frac {\nu }     The function tri(x) is the triangular_function
    (ax)}  [       {\frac {\xi }     {\omega }{2\pi     {2\pi a}}\right)}
    {\displaystyle {a}}\right)}  [   a}}\right)}  [     [{\displaystyle
    \operatorname  {\displaystyle    {\displaystyle     {\frac {1}
    {sinc} ^{2}    {\frac {1}        {\frac {1}{\sqrt   {|a|}}\cdot
    (ax)}]         {|a|}}\cdot       {2\pi a^           \operatorname
                   \operatorname     {2}}}}\cdot        {tri} \left(
                   {tri} \left(      \operatorname      {\frac {\nu }
                   {\frac {\xi }     {tri} \left({\frac {2\pi
                   {a}}\right)}]     {\omega }{2\pi     a}}\right)}]
                                     a}}\right)}]
                                          1  2 &#x03C0;      1   |  a  |
                        1   |  a  |  a  2      &#x22C5; &#x22C5;  sinc  2
                   &#x22C5;  sinc  2 sinc  2   &#x2061; &#x2061;
                   &#x2061;          (   &#x03C9;  2    (   &#x03BD;  2
                   (   &#x03BE; a    &#x03C0; a    )    &#x03C0; a    )
                   )                 {\displaystyle     {\displaystyle
       tri         {\displaystyle    {\frac {1}{\sqrt   {\frac {1}
    &#x2061; ( a x {\frac {1}        {2\pi a^           {|a|}}\cdot
    )              {|a|}}\cdot       {2}}}}\cdot        \operatorname
    {\displaystyle \operatorname     \operatorname      {sinc} ^{2}\left(
204 \operatorname  {sinc} ^{2}\left( {sinc} ^{2}\left(  {\frac {\nu }     Dual of rule 203.
    {tri} (ax)}  [ {\frac {\xi }     {\frac {\omega }   {2\pi a}}\right)}
    {\displaystyle {a}}\right)\,}  [ {2\pi a}}\right)}  [{\displaystyle
    \operatorname  {\displaystyle    [{\displaystyle    {\frac {1}
    {tri} (ax)}]   {\frac {1}        {\frac {1}{\sqrt   {|a|}}\cdot
                   {|a|}}\cdot       {2\pi a^           \operatorname
                   \operatorname     {2}}}}\cdot        {sinc} ^{2}\left(
                   {sinc} ^{2}\left( \operatorname      {\frac {\nu }
                   {\frac {\xi }     {sinc} ^{2}\left(  {2\pi
                   {a}}\right)\,}]   {\frac {\omega }   a}}\right)}]
                                     {2\pi a}}\right)}]
                                          1    2
        e               1  a + 2     &#x03C0;   ( a + i      1  a + i
    &#x2212; a x   &#x03C0; i        &#x03C9; )         &#x03BD;
    u ( x )        &#x03BE;          {\displaystyle     {\displaystyle
    {\displaystyle {\displaystyle    {\frac {1}{{\sqrt  {\frac {1}{a+i\nu
205 e^{-ax}u(x)\,} {\frac {1}{a+2\pi {2\pi }}(a+i\omega }}}  [            The function u(x) is the Heaviside_unit_step_function and a > 0.
    [              i\xi }}}  [       )}}}  [            {\displaystyle
    {\displaystyle {\displaystyle    {\displaystyle     {\frac {1}{a+i\nu
    e^{-ax}u       {\frac {1}{a+2\pi {\frac {1}{{\sqrt  }}}]
    (x)\,}]        i\xi }}}]         {2\pi }}(a+i\omega
                                     )}}}]
                         &#x03C0;
                   &#x03B1;                                   &#x03C0;
                   &#x22C5;  e            1  2 &#x03B1; &#x03B1;
                   &#x2212;          &#x22C5;  e        &#x22C5;  e
                   ( &#x03C0;        &#x2212;           &#x2212;
                   &#x03BE;  )  2    &#x03C9;  2    4   &#x03BD;  2    4
        e          &#x03B1;          &#x03B1;           &#x03B1;
    &#x2212;       {\displaystyle    {\displaystyle     {\displaystyle
    &#x03B1;  x  2 {\sqrt {\frac     {\frac {1}{\sqrt   {\sqrt {\frac
    {\displaystyle {\pi }{\alpha     {2\alpha }}}\cdot  {\pi }{\alpha     This shows that, for the unitary Fourier transforms, the Gaussian_function
206 e^{-\alpha x^  }}}\cdot e^{-     e^{-{\frac {\omega }}}\cdot e^{-     eâÎ±x2 is its own Fourier transform for some choice of Î±. For this to be
    {2}}\,}  [     {\frac {(\pi \xi  ^{2}}{4\alpha }}}} {\frac {\nu ^{2}} integrable we must have Re(Î±) > 0.
    {\displaystyle )^{2}}{\alpha     [{\displaystyle    {4\alpha }}}}  [
    e^{-\alpha x^  }}}}  [           {\frac {1}{\sqrt   {\displaystyle
    {2}}\,}]       {\displaystyle    {2\alpha }}}\cdot  {\sqrt {\frac
                   {\sqrt {\frac     e^{-{\frac {\omega {\pi }{\alpha
                   {\pi }{\alpha     ^{2}}{4\alpha      }}}\cdot e^{-
                   }}}\cdot e^{-     }}}}]              {\frac {\nu ^{2}}
                   {\frac {(\pi \xi                     {4\alpha }}}}]
                   )^{2}}{\alpha
                   }}}}]
        e                2 a    a  2       2 &#x03C0;
    &#x2212; a  |  + 4  &#x03C0;  2  &#x22C5;   a   a
    x  |           &#x03BE;  2       2   +  &#x03C9;  2       2 a    a  2
    {\displaystyle {\displaystyle    {\displaystyle     +  &#x03BD;  2
    \operatorname  {\frac {2a}{a^    {\sqrt {\frac {2}  {\displaystyle
207 {e} ^{-        {2}+4\pi ^{2}\xi  {\pi }}}\cdot      {\frac {2a}{a^    For Re(a) > 0. That is, the Fourier transform of a two-sided_decaying
    a|x|}\,}  [    ^{2}}}}  [        {\frac {a}{a^      {2}+\nu ^{2}}}}   exponential_function is a Lorentzian_function.
    {\displaystyle {\displaystyle    {2}+\omega ^{2}}}} [{\displaystyle
    \operatorname  {\frac {2a}{a^    [ \sqrt{\frac{2}   {\frac {2a}{a^
    {e} ^{-        {2}+4\pi ^{2}\xi  {\pi}} \cdot \frac {2}+\nu ^{2}}}}]
    a|x|}\,}]      ^{2}}}}]          {a}{a^2 +
                                     \omega^2} ]
                                          1 a
                                     &#x03C0; 2    sech
                                     &#x2061;
                        &#x03C0; a   (    &#x03C0;  2 a      &#x03C0; a
                   sech &#x2061;     &#x03C9;  )        sech &#x2061;
                   (     &#x03C0;  2 {\displaystyle     (    &#x03C0;  2
       sech        a   &#x03BE;  )   {\frac {1}{a}}     a    &#x03BD;  )
    &#x2061; ( a x {\displaystyle    {\sqrt {\frac {\pi {\displaystyle
    )              {\frac {\pi }     }                  {\frac {\pi }
    {\displaystyle {a}}\operatorname {2}}}\operatorname {a}}\operatorname
    \operatorname  {sech} \left(     {sech} \left(      {sech} \left(
208 {sech} (ax)\,} {\frac {\pi ^{2}} {\frac {\pi }      {\frac {\pi }     Hyperbolic_secant is its own Fourier transform
    [              {a}}\xi \right)}  {2a}}\omega        {2a}}\nu \right)}
    {\displaystyle [{\displaystyle   \right)}  [        [{\displaystyle
    \operatorname  {\frac {\pi }     {\displaystyle     {\frac {\pi }
    {sech}         {a}}\operatorname {\frac {1}{a}}     {a}}\operatorname
    (ax)\,}]       {sech} \left(     {\sqrt {\frac {\pi {sech} \left(
                   {\frac {\pi ^{2}} }                  {\frac {\pi }
                   {a}}\xi \right)}] {2}}}\operatorname {2a}}\nu
                                     {sech} \left(      \right)}]
                                     {\frac {\pi }
                                     {2a}}\omega
                                     \right)}]
                           2
                   &#x03C0;
                   ( &#x2212; i  )                            ( &#x2212;
                   n    a    e                          i  )  n     2
                   &#x2212;    2           ( &#x2212; i &#x03C0;    a
                   &#x03C0;  2       )  n    a    e     e  &#x2212;
                   &#x03BE;  2     a &#x2212;           &#x03BD;  2    2
        e          2        H  n     &#x03C9;  2    2   a  2         H  n
    &#x2212;     a (    2 &#x03C0;   a  2         H  n  (   &#x03BD; a
    2    x  2    2 &#x03BE;  a   )   (   &#x03C9; a   ) )
    H  n   ( a x ) {\displaystyle    {\displaystyle     {\displaystyle
    {\displaystyle {\frac {{\sqrt    {\frac {(-i)^{n}}  {\frac {(-i)^{n}
    e^{-{\frac {a^ {2\pi }}(-i)^{n}} {a}}e^{-{\frac     {\sqrt {2\pi }}}  Hn is the nth-order Hermite_polynomial. If a = 1 then the GaussâHermite
209 {2}x^{2}}      {a}}e^{-{\frac    {\omega ^{2}}{2a^  {a}}e^{-{\frac    functions are eigenfunctions of the Fourier transform operator. For a
    {2}}}H_{n}     {2\pi ^{2}\xi ^   {2}}}}H_{n}\left(  {\nu ^{2}}{2a^    derivation, see Hermite_polynomial. The formula reduces to 206 for n = 0.
    (ax)\,}  [     {2}}{a^{2}}}}H_   {\frac {\omega }   {2}}}}H_{n}\left(
    {\displaystyle {n}\left({\frac   {a}}\right)}  [    {\frac {\nu }
    e^{-{\frac {a^ {2\pi \xi }       {\displaystyle     {a}}\right)}  [
    {2}x^{2}}      {a}}\right)}  [   {\frac {(-i)^{n}}  {\displaystyle
    {2}}}H_{n}     {\displaystyle    {a}}e^{-{\frac     {\frac {(-i)^{n}
    (ax)\,}]       {\frac {{\sqrt    {\omega ^{2}}{2a^  {\sqrt {2\pi }}}
                   {2\pi }}(-i)^{n}} {2}}}}H_{n}\left(  {a}}e^{-{\frac
                   {a}}e^{-{\frac    {\frac {\omega }   {\nu ^{2}}{2a^
                   {2\pi ^{2}\xi ^   {a}}\right)}]      {2}}}}H_{n}\left(
                   {2}}{a^{2}}}}H_                      {\frac {\nu }
                   {n}\left({\frac                      {a}}\right)}]
                   {2\pi \xi }
                   {a}}\right)}]
**** Distributions, one-dimensional[edit] ****
The Fourier transforms in this table may be found in ErdÃ©lyi_(1954) or Kammler
(2000, appendix).
                     Fourier transform  Fourier transform  Fourier transform
    Function         unitary, ordinary  unitary, angular   non-unitary,       Remarks
                     frequency          frequency          angular frequency
                                                   f
                                f       &#x005E;
                     &#x005E;           ( &#x03C9; ) =   1            f
                     ( &#x03BE; ) =     2 &#x03C0;         &#x005E;
                     &#x222B;  &#x2212; &#x222B;  &#x2212; ( &#x03BD; ) =
                     &#x221E;           &#x221E;           &#x222B;  &#x2212;
                     &#x221E;   f ( x ) &#x221E;   f ( x ) &#x221E;
                     e  &#x2212; 2      e  &#x2212; i      &#x221E;   f ( x )
                     &#x03C0; i x       &#x03C9; x    d x  e  &#x2212; i
                     &#x03BE;    d x    {\displaystyle     &#x03BD; x    d x
                     {\displaystyle     {\begin{aligned}&  {\displaystyle
       f ( x )       {\begin{aligned}&  {\hat {f}}(\omega  {\begin{aligned}&
    {\displaystyle f {\hat {f}}(\xi     )={\frac {1}{\sqrt {\hat {f}}(\nu
    (x)\,}  [        )=\int _{-\infty   {2\pi }}}\int _{-  )=\int _{-\infty
    {\displaystyle f }^{\infty }f(x)e^  \infty }^{\infty   }^{\infty }f(x)e^
    (x)\,}]          {-2\pi ix\xi       }f(x)e^{-i\omega   {-i\nu x}\,dx\end
                     }\,dx\end          x}\,dx\end         {aligned}}}  [
                     {aligned}}}  [     {aligned}}}  [     {\displaystyle
                     {\displaystyle     {\displaystyle     {\begin{aligned}&
                     {\begin{aligned}&  {\begin{aligned}&  {\hat {f}}(\nu
                     {\hat {f}}(\xi     {\hat {f}}(\omega  )=\int _{-\infty
                     )=\int _{-\infty   )={\frac {1}{\sqrt }^{\infty }f(x)e^
                     }^{\infty }f(x)e^  {2\pi }}}\int _{-  {-i\nu x}\,dx\end
                     {-2\pi ix\xi       \infty }^{\infty   {aligned}}}]
                     }\,dx\end          }f(x)e^{-i\omega
                     {aligned}}}]       x}\,dx\end
                                        {aligned}}}]
                                             2 &#x03C0;
                                        &#x22C5; &#x03B4;     2 &#x03C0;
                        &#x03B4;        ( &#x03C9; )       &#x03B4;
                     ( &#x03BE; )       {\displaystyle     ( &#x03BD; )
       1             {\displaystyle     {\sqrt {2\pi       {\displaystyle
301 {\displaystyle   \delta (\xi )}  [  }}\cdot \delta     2\pi \delta (\nu   The distribution Î´(Î¾) denotes the Dirac_delta_function.
    1}  [ 1]         {\displaystyle     (\omega )}  [      )}  [
                     \delta (\xi )}]    {\displaystyle     {\displaystyle
                                        {\sqrt {2\pi       2\pi \delta (\nu
                                        }}\cdot \delta     )}]
                                        (\omega )}]
       &#x03B4; ( x                          1  2 &#x03C0;
    )                                   {\displaystyle
    {\displaystyle      1               {\frac {1}{\sqrt      1
302 \delta (x)\,}  [ {\displaystyle 1}  {2\pi }}}\,}  [    {\displaystyle 1}  Dual of rule 301.
    {\displaystyle   [ 1]               {\displaystyle     [ 1]
    \delta (x)\,}]                      {\frac {1}{\sqrt
                                        {2\pi }}}\,}]
                        &#x03B4;             2 &#x03C0;
                     (  &#x03BE;        &#x22C5; &#x03B4;     2 &#x03C0;
                     &#x2212;   a  2    ( &#x03C9;         &#x03B4;
        e  i a x     &#x03C0;     )     &#x2212; a )       ( &#x03BD;
    {\displaystyle   {\displaystyle     {\displaystyle     &#x2212; a )
303 e^{iax}}  [      \delta \left(\xi - {\sqrt {2\pi       {\displaystyle     This follows from 103 and 301.
    {\displaystyle   {\frac {a}{2\pi    }}\cdot \delta     2\pi \delta (\nu -
    e^{iax}}]        }}\right)}  [      (\omega -a)}  [    a)}  [
                     {\displaystyle     {\displaystyle     {\displaystyle
                     \delta \left(\xi - {\sqrt {2\pi       2\pi \delta (\nu -
                     {\frac {a}{2\pi    }}\cdot \delta     a)}]
                     }}\right)}]        (\omega -a)}]
                           &#x03B4;
                     (  &#x03BE;
                     &#x2212;   a  2         2 &#x03C0;
                     &#x03C0;     )  +  &#x22C5;
                     &#x03B4;           &#x03B4;              &#x03C0;
                     (  &#x03BE; +   a  ( &#x03C9;         (  &#x03B4;
                     2 &#x03C0;     )   &#x2212; a ) +     ( &#x03BD;
                     2                  &#x03B4;           &#x2212; a ) +
                     {\displaystyle     ( &#x03C9; + a )   &#x03B4;
       cos &#x2061;  {\frac {\delta     2                  ( &#x03BD; + a )
    ( a x )          \left(\xi -{\frac  {\displaystyle     )                  This follows from rules 101 and 303 using Euler's_formula:
304 {\displaystyle   {a}{2\pi           {\sqrt {2\pi       {\displaystyle \pi    cos &#x2061; ( a x ) =     e  i a x   +  e  &#x2212; i a x    2   .
    \cos(ax)}  [     }}\right)+\delta   }}\cdot {\frac     \left(\delta (\nu  {\displaystyle \cos(ax)={\frac {e^{iax}+e^{-iax}}{2}}.}  [{\displaystyle \cos
    {\displaystyle   \left(\xi +{\frac  {\delta (\omega -  -a)+\delta (\nu    (ax)={\frac {e^{iax}+e^{-iax}}{2}}.}]
    \cos(ax)}]       {a}{2\pi           a)+\delta (\omega  +a)\right)}  [
                     }}\right)}{2}}}  [ +a)}{2}}\,}  [     {\displaystyle \pi
                     {\displaystyle     {\displaystyle     \left(\delta (\nu
                     {\frac {\delta     {\sqrt {2\pi       -a)+\delta (\nu
                     \left(\xi -{\frac  }}\cdot {\frac     +a)\right)}]
                     {a}{2\pi           {\delta (\omega -
                     }}\right)+\delta   a)+\delta (\omega
                     \left(\xi +{\frac  +a)}{2}}\,}]
                     {a}{2\pi
                     }}\right)}{2}}}]
                           &#x03B4;
                     (  &#x03BE;
                     &#x2212;   a  2         2 &#x03C0;
                     &#x03C0;     )     &#x22C5;              &#x2212; i
                     &#x2212; &#x03B4;  &#x03B4;           &#x03C0;
                     (  &#x03BE; +   a  ( &#x03C9;         (   &#x03B4;
                     2 &#x03C0;     )   &#x2212; a )       ( &#x03BD;
                     2 i                &#x2212; &#x03B4;  &#x2212; a )
                     {\displaystyle     ( &#x03C9; + a )   &#x2212; &#x03B4;
       sin &#x2061;  {\frac {\delta     2 i                ( &#x03BD; + a )
    ( a x )          \left(\xi -{\frac  {\displaystyle     )                  This follows from 101 and 303 using
305 {\displaystyle   {a}{2\pi           {\sqrt {2\pi       {\displaystyle -      sin &#x2061; ( a x ) =     e  i a x   &#x2212;  e  &#x2212; i a x     2 i    .
    \sin(ax)}  [     }}\right)-\delta   }}\cdot {\frac     i\pi {\bigl        {\displaystyle \sin(ax)={\frac {e^{iax}-e^{-iax}}{2i}}.}  [{\displaystyle \sin
    {\displaystyle   \left(\xi +{\frac  {\delta (\omega -  (}\delta (\nu -a)- (ax)={\frac {e^{iax}-e^{-iax}}{2i}}.}]
    \sin(ax)}]       {a}{2\pi           a)-\delta (\omega  \delta (\nu +a)
                     }}\right)}{2i}}}   +a)}{2i}}}  [      {\bigr )}}  [
                     [{\displaystyle    {\displaystyle     {\displaystyle -
                     {\frac {\delta     {\sqrt {2\pi       i\pi {\bigl
                     \left(\xi -{\frac  }}\cdot {\frac     (}\delta (\nu -a)-
                     {a}{2\pi           {\delta (\omega -  \delta (\nu +a)
                     }}\right)-\delta   a)-\delta (\omega  {\bigr )}}]
                     \left(\xi +{\frac  +a)}{2i}}}]
                     {a}{2\pi
                     }}\right)}{2i}}}]
                           &#x03C0; a
                     cos &#x2061;                                &#x03C0; a
                     (      &#x03C0;  2      1  2 a    cos cos &#x2061;
                     &#x03BE;  2    a   &#x2061;           (     &#x03BD;  2
                     &#x2212;           (     &#x03C9;  2  4 a    &#x2212;
                     &#x03C0; 4    )    4 a    &#x2212;    &#x03C0; 4    )
       cos &#x2061;  {\displaystyle     &#x03C0; 4    )    {\displaystyle
    (  a  x  2    )  {\sqrt {\frac {\pi {\displaystyle     {\sqrt {\frac {\pi
    {\displaystyle   }{a}}}\cos \left(  {\frac {1}{\sqrt   }{a}}}\cos \left(
306 \cos \left(ax^   {\frac {\pi ^      {2a}}}\cos \left(  {\frac {\nu ^{2}}
    {2}\right)}  [   {2}\xi ^{2}}{a}}-  {\frac {\omega ^   {4a}}-{\frac {\pi
    {\displaystyle   {\frac {\pi }      {2}}{4a}}-{\frac   }{4}}\right)}  [
    \cos \left(ax^   {4}}\right)}  [    {\pi }{4}}\right)} {\displaystyle
    {2}\right)}]     {\displaystyle     [ \frac{1}{\sqrt{2 {\sqrt {\frac {\pi
                     {\sqrt {\frac {\pi a}} \cos \left     }{a}}}\cos \left(
                     }{a}}}\cos \left(  ( \frac{\omega^2}  {\frac {\nu ^{2}}
                     {\frac {\pi ^      {4 a} - \frac{\pi} {4a}}-{\frac {\pi
                     {2}\xi ^{2}}{a}}-  {4} \right) ]      }{4}}\right)}]
                     {\frac {\pi }
                     {4}}\right)}]
                        &#x2212;
                     &#x03C0; a    sin                        &#x2212;
                     &#x2061;                 &#x2212; 1   &#x03C0; a    sin
                     (      &#x03C0;  2 2 a    sin         &#x2061;
                     &#x03BE;  2    a   &#x2061;           (     &#x03BD;  2
                     &#x2212;           (     &#x03C9;  2  4 a    &#x2212;
       sin &#x2061;  &#x03C0; 4    )    4 a    &#x2212;    &#x03C0; 4    )
    (  a  x  2    )  {\displaystyle -   &#x03C0; 4    )    {\displaystyle -
    {\displaystyle   {\sqrt {\frac {\pi {\displaystyle     {\sqrt {\frac {\pi
    \sin \left(ax^   }{a}}}\sin \left(  {\frac {-1}{\sqrt  }{a}}}\sin \left(
307 {2}\right)\,}  [ {\frac {\pi ^      {2a}}}\sin \left(  {\frac {\nu ^{2}}
    {\displaystyle   {2}\xi ^{2}}{a}}-  {\frac {\omega ^   {4a}}-{\frac {\pi
    \sin \left(ax^   {\frac {\pi }      {2}}{4a}}-{\frac   }{4}}\right)}  [
    {2}\right)\,}]   {4}}\right)}  [    {\pi }{4}}\right)} {\displaystyle -
                     {\displaystyle -   [ \frac{-1}{\sqrt  {\sqrt {\frac {\pi
                     {\sqrt {\frac {\pi {2 a}} \sin \left  }{a}}}\sin \left(
                     }{a}}}\sin \left(  ( \frac{\omega^2}  {\frac {\nu ^{2}}
                     {\frac {\pi ^      {4 a} - \frac{\pi} {4a}}-{\frac {\pi
                     {2}\xi ^{2}}{a}}-  {4} \right) ]      }{4}}\right)}]
                     {\frac {\pi }
                     {4}}\right)}]
                          (   i  2
                     &#x03C0;    )   n      i  n     2
                     &#x03B4;  ( n )    &#x03C0;              2 &#x03C0;  i
                     ( &#x03BE; )       &#x03B4;  ( n )    n    &#x03B4;  ( n
        x  n         {\displaystyle     ( &#x03C9; )       )   ( &#x03BD; )
    {\displaystyle   \left({\frac {i}   {\displaystyle i^  {\displaystyle     Here, n is a natural_number and Î´(n)(Î¾) is the nth distribution derivative of
308 x^{n}\,}  [      {2\pi }}\right)^   {n}{\sqrt {2\pi    2\pi i^{n}\delta ^ the Dirac delta function. This rule follows from rules 107 and 301. Combining
    {\displaystyle   {n}\delta ^{(n)}   }}\delta ^{(n)}    {(n)}(\nu )\,}  [  this rule with 101, we can transform all polynomials.
    x^{n}\,}]        (\xi )\,}  [       (\omega )\,}  [    {\displaystyle
                     {\displaystyle     {\displaystyle i^  2\pi i^{n}\delta ^
                     \left({\frac {i}   {n}{\sqrt {2\pi    {(n)}(\nu )\,}]
                     {2\pi }}\right)^   }}\delta ^{(n)}
                     {n}\delta ^{(n)}   (\omega )\,}]
                     (\xi )\,}]
                                              ( i &#x03C9;
        &#x03B4;        ( 2 &#x03C0; i  )  n     2
    ( n )   ( x )    &#x03BE;  )  n     &#x03C0;              ( i &#x03BD;  )
    {\displaystyle   {\displaystyle     {\displaystyle     n
    \delta ^{(n)}    (2\pi i\xi )^      {\frac {(i\omega   {\displaystyle     Dual of rule 308. Î´(n)(Î¾) is the nth distribution derivative of the Dirac delta
    (x)\,}  [        {n}\,}  [          )^{n}}{\sqrt {2\pi (i\nu )^{n}\,}  [  function. This rule follows from 106 and 302.
    {\displaystyle   {\displaystyle     }}}\,}  [          {\displaystyle
    \delta ^{(n)}    (2\pi i\xi )^      {\displaystyle     (i\nu )^{n}\,}]
    (x)\,}]          {n}\,}]            {\frac {(i\omega
                                        )^{n}}{\sqrt {2\pi
                                        }}}\,}]
                                           &#x2212; i
                                        &#x03C0; 2    sgn
                        &#x2212; i      &#x2061;              &#x2212; i
                     &#x03C0; sgn       ( &#x03C9; )       &#x03C0; sgn
         1 x         &#x2061;           {\displaystyle -i  &#x2061;
    {\displaystyle   ( &#x03BE; )       {\sqrt {\frac {\pi ( &#x03BD; )       Here sgn(Î¾) is the sign_function. Note that 1/x is not a distribution. It is
309 {\frac {1}{x}}}  {\displaystyle -   }                  {\displaystyle -   necessary to use the Cauchy_principal_value when testing against Schwartz
    [{\displaystyle  i\pi \operatorname {2}}}\operatorname i\pi \operatorname functions. This rule is useful in studying the Hilbert_transform.
    {\frac {1}{x}}}] {sgn}(\xi )}  [    {sgn}(\omega )}  [ {sgn}(\nu )}  [
                     {\displaystyle -   {\displaystyle -i  {\displaystyle -
                     i\pi \operatorname {\sqrt {\frac {\pi i\pi \operatorname
                     {sgn}(\xi )}]      }                  {sgn}(\nu )}]
                                        {2}}}\operatorname
                                        {sgn}(\omega )}]
              1  x
    n           :
    =    ( &#x2212;
    1  )  n &#x2212;                       &#x2212; i
    1     ( n           &#x2212; i      &#x03C0; 2
    &#x2212; 1 ) !   &#x03C0;           &#x22C5;              &#x2212; i
    d  n    d  x  n  ( &#x2212; 2       ( &#x2212; i       &#x03C0;
    log &#x2061;  |  &#x03C0; i         &#x03C9;  )  n     ( &#x2212; i
    x  |             &#x03BE;  )  n     &#x2212; 1     ( n &#x03BD;  )  n
    {\displaystyle   &#x2212; 1     ( n &#x2212; 1 ) !     &#x2212; 1     ( n
    {\begin          &#x2212; 1 ) !     sgn &#x2061;       &#x2212; 1 ) !
    {aligned}&{\frac sgn &#x2061;       ( &#x03C9; )       sgn &#x2061;
    {1}{x^{n}}}\\&:= ( &#x03BE; )       {\displaystyle -i  ( &#x03BD; )       1/xn is the homogeneous_distribution defined by the distributional derivative
    {\frac {(-1)^{n- {\displaystyle -   {\sqrt {\frac {\pi {\displaystyle -         ( &#x2212; 1  )  n &#x2212; 1     ( n &#x2212; 1 ) !       d  n    d  x  n
310 1}}{(n-1)!}}     i\pi {\frac {(-    }{2}}}\cdot {\frac i\pi {\frac {(-    log &#x2061;  |  x  |    {\displaystyle {\frac {(-1)^{n-1}}{(n-1)!}}{\frac {d^
    {\frac {d^{n}}   2\pi i\xi )^{n-1}} {(-i\omega )^{n-   i\nu )^{n-1}}{(n-  {n}}{dx^{n}}}\log |x|}  [{\displaystyle {\frac {(-1)^{n-1}}{(n-1)!}}{\frac {d^
    {dx^{n}}}\log    {(n-               1}}{(n-            1)!}}\operatorname {n}}{dx^{n}}}\log |x|}]
    |x|\end          1)!}}\operatorname 1)!}}\operatorname {sgn}(\nu )}  [
    {aligned}}}  [   {sgn}(\xi )}  [    {sgn}(\omega )}  [ {\displaystyle -
    {\displaystyle   {\displaystyle -   {\displaystyle -i  i\pi {\frac {(-
    {\begin          i\pi {\frac {(-    {\sqrt {\frac {\pi i\nu )^{n-1}}{(n-
    {aligned}&{\frac 2\pi i\xi )^{n-1}} }{2}}}\cdot {\frac 1)!}}\operatorname
    {1}{x^{n}}}\\&:= {(n-               {(-i\omega )^{n-   {sgn}(\nu )}]
    {\frac {(-1)^{n- 1)!}}\operatorname 1}}{(n-
    1}}{(n-1)!}}     {sgn}(\xi )}]      1)!}}\operatorname
    {\frac {d^{n}}                      {sgn}(\omega )}]
    {dx^{n}}}\log
    |x|\end
    {aligned}}}]
                                              &#x2212; 2
                                        2 &#x03C0;
                        &#x2212;    2   &#x22C5;    sin
                     sin &#x2061;       &#x2061;
                     (    &#x03C0;      (    &#x03C0;         &#x2212;    2
                     &#x03B1;  2   )    &#x03B1;  2   )    sin &#x2061;
                     &#x0393;           &#x0393;           (    &#x03C0;
                     ( &#x03B1; + 1 )   ( &#x03B1; + 1 )   &#x03B1;  2   )
                     |  2 &#x03C0;      |  &#x03C9;   |    &#x0393;
                     &#x03BE;   |       &#x03B1; + 1       ( &#x03B1; + 1 )
                     &#x03B1; + 1       {\displaystyle     |  &#x03BD;   |
        |  x   |     {\displaystyle -   {\frac {-2}{\sqrt  &#x03B1; + 1       This formula is valid for 0 > Î± > â1. For Î± > 0 some singular terms arise at
    &#x03B1;         {\frac {2\sin      {2\pi }}}\cdot     {\displaystyle -   the origin that can be found by differentiating 318. If Re Î± > â1, then |x|Î±
    {\displaystyle   \left({\frac {\pi  {\frac {\sin \left {\frac {2\sin      is a locally integrable function, and so a tempered distribution. The function Î±
311 |x|^{\alpha }\,} \alpha }           ({\frac {\pi       \left({\frac {\pi  â¦ |x|Î± is a holomorphic function from the right half-plane to the space of
    [{\displaystyle  {2}}\right)\Gamma  \alpha }           \alpha }           tempered distributions. It admits a unique meromorphic extension to a tempered
    |x|^{\alpha      (\alpha +1)}{|2\pi {2}}\right)\Gamma  {2}}\right)\Gamma  distribution, also denoted |x|Î± for Î± â  â2, â4,... (See homogeneous
    }\,}]            \xi |^{\alpha      (\alpha +1)}       (\alpha +1)}{|\nu  distribution.)
                     +1}}}}  [          {|\omega |^{\alpha |^{\alpha +1}}}}
                     {\displaystyle -   +1}}}}  [          [{\displaystyle -
                     {\frac {2\sin      {\displaystyle     {\frac {2\sin
                     \left({\frac {\pi  {\frac {-2}{\sqrt  \left({\frac {\pi
                     \alpha }           {2\pi }}}\cdot     \alpha }
                     {2}}\right)\Gamma  {\frac {\sin \left {2}}\right)\Gamma
                     (\alpha +1)}{|2\pi ({\frac {\pi       (\alpha +1)}{|\nu
                     \xi |^{\alpha      \alpha }           |^{\alpha +1}}}}]
                     +1}}}}]            {2}}\right)\Gamma
                                        (\alpha +1)}
                                        {|\omega |^{\alpha
                                        +1}}}}]
                                                                 2 &#x03C0;
         1   |  x  |      1   |              1   |         |  &#x03BD;  |
    {\displaystyle   &#x03BE;  |        &#x03C9;  |        {\displaystyle
    {\frac {1}{\sqrt {\displaystyle     {\displaystyle     {\frac {\sqrt
    {|x|}}}\,}  [    {\frac {1}{\sqrt   {\frac {1}{\sqrt   {2\pi }}{\sqrt     Special case of 311.
    {\frac {1}{\sqrt {|\xi |}}}}  [     {|\omega |}}}}  [  {|\nu |}}}}  [
    {|x|}}}\,]       {\frac {1}{\sqrt   {\frac {1}{\sqrt   {\frac {\sqrt
                     {|\xi |}}}]        {|\omega |}}}]     {2\pi }}{\sqrt
                                                           {|\nu |}}}]
                                              2 &#x03C0;
       sgn &#x2061;       1  i &#x03C0; 1  i &#x03C9;           2  i &#x03BD;
    ( x )            &#x03BE;           {\displaystyle     {\displaystyle
    {\displaystyle   {\displaystyle     {\sqrt {\frac {2}  {\frac {2}{i\nu
312 \operatorname    {\frac {1}{i\pi    {\pi }}}{\frac {1} }}}  [             The dual of rule 309. This time the Fourier transforms need to be considered as a
    {sgn}(x)}  [     \xi }}}  [         {i\omega }}}  [    {\displaystyle     Cauchy_principal_value.
    {\displaystyle   {\displaystyle     {\displaystyle     {\frac {2}{i\nu
    \operatorname    {\frac {1}{i\pi    {\sqrt {\frac {2}  }}}]
    {sgn}(x)}]       \xi }}}]           {\pi }}}{\frac {1}
                                        {i\omega }}}]
                          1 2    (    1       &#x03C0; 2
                     i &#x03C0;         (    1  i &#x03C0;    &#x03C0;
                     &#x03BE;    +      &#x03C9;    +      (    1  i &#x03C0;
                     &#x03B4;           &#x03B4;           &#x03BD;    +
                     ( &#x03BE; )  )    ( &#x03C9; )  )    &#x03B4;
                     {\displaystyle     {\displaystyle     ( &#x03BD; )  )
       u ( x )       {\frac {1}         {\sqrt {\frac {\pi {\displaystyle \pi
    {\displaystyle u {2}}\left({\frac   }{2}}}\left({\frac \left({\frac {1}   The function u(x) is the Heaviside unit_step_function; this follows from rules
313 (x)}  [          {1}{i\pi \xi       {1}{i\pi \omega    {i\pi \nu          101, 301, and 312.
    {\displaystyle u }}+\delta (\xi     }}+\delta (\omega  }}+\delta (\nu
    (x)}]            )\right)}  [       )\right)}  [       )\right)}  [
                     {\displaystyle     {\displaystyle     {\displaystyle \pi
                     {\frac {1}         {\sqrt {\frac {\pi \left({\frac {1}
                     {2}}\left({\frac   }{2}}}\left({\frac {i\pi \nu
                     {1}{i\pi \xi       {1}{i\pi \omega    }}+\delta (\nu
                     }}+\delta (\xi     }}+\delta (\omega  )\right)}]
                     )\right)}]         )\right)}]
                                              2 &#x03C0;
                                        T    &#x2211;  k =       2 &#x03C0;
                          1 T           &#x2212; &#x221E;  T    &#x2211;  k =
                     &#x2211;  k =      &#x221E;           &#x2212; &#x221E;
                     &#x2212; &#x221E;  &#x03B4;           &#x221E;
        &#x2211;  n  &#x221E;           (  &#x03C9;        &#x03B4;
    = &#x2212;       &#x03B4;           &#x2212;    2      (  &#x03BD;
    &#x221E;         (  &#x03BE;        &#x03C0; k  T    ) &#x2212;    2
    &#x221E;         &#x2212;   k T     {\displaystyle     &#x03C0; k  T    ) This function is known as the Dirac_comb function. This result can be derived
    &#x03B4; ( x     )                  {\frac {\sqrt      {\displaystyle     from 302 and 102, together with the fact that
    &#x2212; n T )   {\displaystyle     {2\pi }}{T}}\sum _ {\frac {2\pi }         &#x2211;  n = &#x2212; &#x221E;   &#x221E;    e  i n x   = 2 &#x03C0;
314 {\displaystyle   {\frac {1}{T}}\sum {k=-\infty }^      {T}}\sum _{k=-     &#x2211;  k = &#x2212; &#x221E;   &#x221E;   &#x03B4; ( x + 2 &#x03C0; k )
    \sum _{n=-\infty _{k=-\infty }^     {\infty }\delta    \infty }^{\infty   {\displaystyle \sum _{n=-\infty }^{\infty }e^{inx}=2\pi \sum _{k=-\infty }^
    }^{\infty        {\infty }\delta    \left(\omega -     }\delta \left(\nu  {\infty }\delta (x+2\pi k)}  [{\displaystyle \sum _{n=-\infty }^{\infty }e^
    }\delta (x-nT)}  \left(\xi -{\frac  {\frac {2\pi k}    -{\frac {2\pi k}   {inx}=2\pi \sum _{k=-\infty }^{\infty }\delta (x+2\pi k)}]
    [{\displaystyle  {k}{T}}\right)}  [ {T}}\right)}  [    {T}}\right)}  [    as distributions.
    \sum _{n=-\infty {\displaystyle     {\displaystyle     {\displaystyle
    }^{\infty        {\frac {1}{T}}\sum {\frac {\sqrt      {\frac {2\pi }
    }\delta (x-nT)}] _{k=-\infty }^     {2\pi }}{T}}\sum _ {T}}\sum _{k=-
                     {\infty }\delta    {k=-\infty }^      \infty }^{\infty
                     \left(\xi -{\frac  {\infty }\delta    }\delta \left(\nu
                     {k}{T}}\right)}]   \left(\omega -     -{\frac {2\pi k}
                                        {\frac {2\pi k}    {T}}\right)}]
                                        {T}}\right)}]
                                              2 &#x03C0;
                                        &#x22C5;    rect
                                        &#x2061;
                           2  rect      (   &#x03C9; 2   )       2  rect
                     &#x2061;           1 &#x2212;         &#x2061;
                     ( &#x03C0;         &#x03C9;  2        (   &#x03BD; 2   )
                     &#x03BE; )   1     {\displaystyle     1 &#x2212;
                     &#x2212; 4         {\sqrt {\frac {2}  &#x03BD;  2
                     &#x03C0;  2        {\pi }}}\cdot      {\displaystyle
                     &#x03BE;  2        {\frac             {\frac
        J  0   ( x ) {\displaystyle     {\operatorname     {2\,\operatorname
    {\displaystyle   {\frac             {rect} \left(      {rect} \left(
315 J_{0}(x)}  [     {2\,\operatorname  {\frac {\omega }   {\frac {\nu }      The function J0(x) is the zeroth order Bessel_function of first kind.
    {\displaystyle   {rect} (\pi \xi )} {2}}\right)}{\sqrt {2}}\right)}{\sqrt
    J_{0}(x)}]       {\sqrt {1-4\pi ^   {1-\omega ^{2}}}}} {1-\nu ^{2}}}}}  [
                     {2}\xi ^{2}}}}}  [ [{\displaystyle    {\displaystyle
                     {\displaystyle     {\sqrt {\frac {2}  {\frac
                     {\frac             {\pi }}}\cdot      {2\,\operatorname
                     {2\,\operatorname  {\frac             {rect} \left(
                     {rect} (\pi \xi )} {\operatorname     {\frac {\nu }
                     {\sqrt {1-4\pi ^   {rect} \left(      {2}}\right)}{\sqrt
                     {2}\xi ^{2}}}}}]   {\frac {\omega }   {1-\nu ^{2}}}}}]
                                        {2}}\right)}{\sqrt
                                        {1-\omega ^
                                        {2}}}}}]
                                              2 &#x03C0;
                           2 ( &#x2212; ( &#x2212; i  )  n       2 ( &#x2212;
                     i  )  n    T  n    T  n   ( &#x03C9;  i  )  n    T  n
                     ( 2 &#x03C0;       ) rect &#x2061;    ( &#x03BD; ) rect
                     &#x03BE; ) rect    (   &#x03C9; 2   ) &#x2061;
                     &#x2061;           1 &#x2212;         (   &#x03BD; 2   )
                     ( &#x03C0;         &#x03C9;  2        1 &#x2212;
                     &#x03BE; )   1     {\displaystyle     &#x03BD;  2
                     &#x2212; 4         {\sqrt {\frac {2}  {\displaystyle
                     &#x03C0;  2        {\pi }}}{\frac {(- {\frac {2(-i)^
        J  n   ( x ) &#x03BE;  2        i)^{n}T_{n}(\omega {n}T_{n}(\nu
    {\displaystyle   {\displaystyle     )\operatorname     )\operatorname     This is a generalization of 315. The function Jn(x) is the nth order Bessel
316 J_{n}(x)}  [     {\frac {2(-i)^     {rect} \left(      {rect} \left(      function of first kind. The function Tn(x) is the Chebyshev_polynomial_of_the
    {\displaystyle   {n}T_{n}(2\pi \xi  {\frac {\omega }   {\frac {\nu }      first_kind.
    J_{n}(x)}]       )\operatorname     {2}}\right)}{\sqrt {2}}\right)}{\sqrt
                     {rect} (\pi \xi )} {1-\omega ^{2}}}}} {1-\nu ^{2}}}}}  [
                     {\sqrt {1-4\pi ^   [{\displaystyle    {\displaystyle
                     {2}\xi ^{2}}}}}  [ {\sqrt {\frac {2}  {\frac {2(-i)^
                     {\displaystyle     {\pi }}}{\frac {(- {n}T_{n}(\nu
                     {\frac {2(-i)^     i)^{n}T_{n}(\omega )\operatorname
                     {n}T_{n}(2\pi \xi  )\operatorname     {rect} \left(
                     )\operatorname     {rect} \left(      {\frac {\nu }
                     {rect} (\pi \xi )} {\frac {\omega }   {2}}\right)}{\sqrt
                     {\sqrt {1-4\pi ^   {2}}\right)}{\sqrt {1-\nu ^{2}}}}}]
                     {2}\xi ^{2}}}}}]   {1-\omega ^
                                        {2}}}}}]
                                           &#x2212;
                                        &#x03C0; 2    |       &#x2212;
                        &#x2212;   1 2  &#x03C9; |         &#x03C0;  |
                     1  | &#x03BE; |    &#x2212;   2       &#x03BD; |
                     &#x2212; &#x03B3;  &#x03C0;           &#x2212; 2
                     &#x03B4;           &#x03B3; &#x03B4;  &#x03C0; &#x03B3;
                     ( &#x03BE; )       ( &#x03C9; )       &#x03B4;
       log &#x2061;  {\displaystyle -   {\displaystyle -   ( &#x03BD; )
    | x |            {\frac {1}{2}}     {\frac {\sqrt      {\displaystyle -
    {\displaystyle   {\frac {1}         {\frac {\pi }{2}}} {\frac {\pi }
    \log             {\left|\xi         {\left|\omega      {\left|\nu
317 \left|x\right|}  \right|}}-\gamma   \right|}}-{\sqrt   \right|}}-2\pi     Î³ is the EulerâMascheroni_constant.
    [{\displaystyle  \delta \left(\xi   {2\pi }}\gamma     \gamma \delta
    \log             \right)}  [        \delta \left       \left(\nu \right)}
    \left|x\right|}] {\displaystyle -   (\omega \right)}   [{\displaystyle -
                     {\frac {1}{2}}     [{\displaystyle -  {\frac {\pi }
                     {\frac {1}         {\frac {\sqrt      {\left|\nu
                     {\left|\xi         {\frac {\pi }{2}}} \right|}}-2\pi
                     \right|}}-\gamma   {\left|\omega      \gamma \delta
                     \delta \left(\xi   \right|}}-{\sqrt   \left(\nu
                     \right)}]          {2\pi }}\gamma     \right)}]
                                        \delta \left
                                        (\omega \right)}]
                            (  2
                     &#x03C0;  )
                     &#x03B1;                 2 &#x03C0;         2 &#x03C0;
                     &#x0393;           &#x0393;           &#x0393;
                     ( &#x03B1; )     u ( &#x03B1; )     u ( &#x03B1; )     u
                     (  &#x00B1;        (  &#x00B1;        (  &#x00B1;
                     &#x03BE;  )        &#x03C9;  )        &#x03BD;  )
                     (  &#x00B1;        (  &#x00B1;        (  &#x00B1;
                     &#x03BE;  )        &#x03C9;  )        &#x03BD;  )
         (  &#x2213; &#x03B1; &#x2212;  &#x03B1; &#x2212;  &#x03B1; &#x2212;
    i x  )           1                  1                  1
    &#x2212;         {\displaystyle     {\displaystyle     {\displaystyle
    &#x03B1;         {\frac {\left(2\pi {\frac {\sqrt      {\frac {2\pi }
    {\displaystyle   \right)^{\alpha }} {2\pi }}{\Gamma    {\Gamma \left
    \left(\mp        {\Gamma \left      \left(\alpha       (\alpha            This formula is valid for 1 > Î± > 0. Use differentiation to derive formula for
318 ix\right)^{-     (\alpha            \right)}}u\left    \right)}}u\left    higher exponents. u is the Heaviside function.
    \alpha }}  [     \right)}}u\left    (\pm \omega        (\pm \nu
    {\displaystyle   (\pm \xi           \right)\left(\pm   \right)\left(\pm
    \left(\mp        \right)\left(\pm   \omega \right)^    \nu \right)^
    ix\right)^{-     \xi \right)^       {\alpha -1}}  [    {\alpha -1}}  [
    \alpha }}]       {\alpha -1}}  [    {\displaystyle     {\displaystyle
                     {\displaystyle     {\frac {\sqrt      {\frac {2\pi }
                     {\frac {\left(2\pi {2\pi }}{\Gamma    {\Gamma \left
                     \right)^{\alpha }} \left(\alpha       (\alpha
                     {\Gamma \left      \right)}}u\left    \right)}}u\left
                     (\alpha            (\pm \omega        (\pm \nu
                     \right)}}u\left    \right)\left(\pm   \right)\left(\pm
                     (\pm \xi           \omega \right)^    \nu \right)^
                     \right)\left(\pm   {\alpha -1}}]      {\alpha -1}}]
                     \xi \right)^
                     {\alpha -1}}]
**** Two-dimensional functions[edit] ****
                   Fourier transform  Fourier transform  Fourier transform
    Function       unitary, ordinary  unitary, angular   non-unitary,       Remarks
                   frequency          frequency          angular frequency
                                                 f
                              f       &#x005E;                      f
                   &#x005E;           (  &#x03C9;  x   , &#x005E;
                   (  &#x03BE;  x   , &#x03C9;  y   )    (  &#x03BD;  x   ,
                   &#x03BE;  y   )    =   1  2 &#x03C0;  &#x03BD;  y   )
                   = &#x222C; f ( x , &#x222C; f ( x , y = &#x222C; f ( x ,
                   y )  e  &#x2212; 2 )  e  &#x2212; i   y )  e  &#x2212; i
                   &#x03C0; i         (  &#x03C9;  x   x (  &#x03BD;  x   x
                   (  &#x03BE;  x   x +  &#x03C9;  y   y +  &#x03BD;  y   y
                   +  &#x03BE;  y   y )    d x  d y      )    d x  d y
                   )    d x  d y      {\displaystyle     {\displaystyle
                   {\displaystyle     {\begin{aligned}&  {\begin{aligned}&
       f ( x , y ) {\begin{aligned}&  {\hat {f}}(\omega  {\hat {f}}(\nu _
    {\displaystyle {\hat {f}}(\xi _   _{x},\omega _      {x},\nu _
400 f(x,y)}  [     {x},\xi _          {y})\\&={\frac {1} {y})\\&=\iint f    The variables Î¾x, Î¾y, Ïx, Ïy, Î½x, Î½y are real numbers. The integrals are taken
    {\displaystyle {y})\\&=\iint f    {2\pi }}\iint f    (x,y)e^{-i(\nu _   over the entire plane.
    f(x,y)}]       (x,y)e^{-2\pi i    (x,y)e^{-i(\omega  {x}x+\nu _
                   (\xi _{x}x+\xi _   _{x}x+\omega _     {y}y)}\,dx\,dy\end
                   {y}y)}\,dx\,dy\end {y}y)}\,dx\,dy\end {aligned}}}  [
                   {aligned}}}  [     {aligned}}}  [     {\displaystyle
                   {\displaystyle     {\displaystyle     {\begin{aligned}&
                   {\begin{aligned}&  {\begin{aligned}&  {\hat {f}}(\nu _
                   {\hat {f}}(\xi _   {\hat {f}}(\omega  {x},\nu _
                   {x},\xi _          _{x},\omega _      {y})\\&=\iint f
                   {y})\\&=\iint f    {y})\\&={\frac {1} (x,y)e^{-i(\nu _
                   (x,y)e^{-2\pi i    {2\pi }}\iint f    {x}x+\nu _
                   (\xi _{x}x+\xi _   (x,y)e^{-i(\omega  {y}y)}\,dx\,dy\end
                   {y}y)}\,dx\,dy\end _{x}x+\omega _     {aligned}}}]
                   {aligned}}}]       {y}y)}\,dx\,dy\end
                                      {aligned}}}]
                                           1  2 &#x03C0;      1   |  a b  |
                        1   |  a b  | &#x22C5;  |  a b   e  &#x2212;   1  4
                   e  &#x2212;        |      e  &#x2212; &#x03C0;
                   &#x03C0;           1  4 &#x03C0;      (     &#x03BD;  x
        e          (     &#x03BE;  x  (     &#x03C9;  x  2    a  2     +
    &#x2212;       2    a  2     +    2    a  2     +    &#x03BD;  y   2
    &#x03C0;       &#x03BE;  y   2    &#x03C9;  y   2    b  2      )
    (   a  2    x  b  2      )        b  2      )        {\displaystyle
    2   +  b  2    {\displaystyle     {\displaystyle     {\frac {1}
    y  2    )      {\frac {1}         {\frac {1}{2\pi    {|ab|}}e^{-{\frac
    {\displaystyle {|ab|}}e^{-\pi     \cdot |ab|}}e^{-   {1}{4\pi }}\left(
    e^{-\pi \left  \left({\frac {\xi  {\frac {1}{4\pi    {\frac {\nu _{x}^
401 (a^{2}x^{2}+b^ _{x}^{2}}{a^{2}}}+ }}\left({\frac     {2}}{a^{2}}}+      Both functions are Gaussians, which may not have unit volume.
    {2}y^          {\frac {\xi _{y}^  {\omega _{x}^{2}}  {\frac {\nu _{y}^
    {2}\right)}}   {2}}{b^            {a^{2}}}+{\frac    {2}}{b^
    [              {2}}}\right)}}  [  {\omega _{y}^{2}}  {2}}}\right)}}  [
    {\displaystyle {\displaystyle     {b^{2}}}\right)}}  {\displaystyle
    e^{-\pi \left  {\frac {1}         [{\displaystyle    {\frac {1}
    (a^{2}x^{2}+b^ {|ab|}}e^{-\pi     {\frac {1}{2\pi    {|ab|}}e^{-{\frac
    {2}y^          \left({\frac {\xi  \cdot |ab|}}e^{-   {1}{4\pi }}\left(
    {2}\right)}}]  _{x}^{2}}{a^{2}}}+ {\frac {1}{4\pi    {\frac {\nu _{x}^
                   {\frac {\xi _{y}^  }}\left({\frac     {2}}{a^{2}}}+
                   {2}}{b^            {\omega _{x}^{2}}  {\frac {\nu _{y}^
                   {2}}}\right)}}]    {a^{2}}}+{\frac    {2}}{b^
                                      {\omega _{y}^{2}}  {2}}}\right)}}]
                                      {b^{2}}}\right)}}]
                          J  1               J  1              2 &#x03C0;
                   (  2 &#x03C0;      (    &#x03C9;  x   J  1
                   &#x03BE;  x   2    2   +  &#x03C9;  y (    &#x03BD;  x
       circ        +  &#x03BE;  y   2 2     )            2   +  &#x03BD;  y
    &#x2061;       )     &#x03BE;  x  &#x03C9;  x   2    2     )
    (    x  2   +  2   +  &#x03BE;  y +  &#x03C9;  y   2 &#x03BD;  x   2
    y  2     )     2                  {\displaystyle     +  &#x03BD;  y   2
    {\displaystyle {\displaystyle     {\frac {J_{1}\left {\displaystyle
    \operatorname  {\frac {J_{1}\left ({\sqrt {\omega _  {\frac {2\pi J_
    {circ} \left(  (2\pi {\sqrt {\xi  {x}^{2}+\omega _   {1}\left({\sqrt
    {\sqrt {x^     _{x}^{2}+\xi _{y}^ {y}^{2}}}\right)}  {\nu _{x}^{2}+\nu  The function is defined by circ(r) = 1 for 0 â¤ r â¤ 1, and is 0 otherwise. The
402 {2}+y^         {2}}}\right)}      {\sqrt {\omega _   _{y}^{2}}}\right)} result is the amplitude distribution of the Airy_disk, and is expressed using J1 (the
    {2}}}\right)}  {\sqrt {\xi _{x}^  {x}^{2}+\omega _   {\sqrt {\nu _{x}^  order-1 Bessel_function of the first kind).[50]
    [              {2}+\xi _{y}^      {y}^{2}}}}}  [     {2}+\nu _{y}^
    {\displaystyle {2}}}}}  [         {\displaystyle     {2}}}}}  [
    \operatorname  {\displaystyle     {\frac {J_{1}\left {\displaystyle
    {circ} \left(  {\frac {J_{1}\left ({\sqrt {\omega _  {\frac {2\pi J_
    {\sqrt {x^     (2\pi {\sqrt {\xi  {x}^{2}+\omega _   {1}\left({\sqrt
    {2}+y^         _{x}^{2}+\xi _{y}^ {y}^{2}}}\right)}  {\nu _{x}^{2}+\nu
    {2}}}\right)}] {2}}}\right)}      {\sqrt {\omega _   _{y}^{2}}}\right)}
                   {\sqrt {\xi _{x}^  {x}^{2}+\omega _   {\sqrt {\nu _{x}^
                   {2}+\xi _{y}^      {y}^{2}}}}}]       {2}+\nu _{y}^
                   {2}}}}}]                              {2}}}}}]
**** Formulas for general n-dimensional functions[edit] ****
                    Fourier        Fourier        Fourier
                    transform      transform      transform
    Function        unitary,       unitary,       non-unitary,   Remarks
                    ordinary       angular        angular
                    frequency      frequency      frequency
                                              f
                                   &#x005E;
                                   (  &#x03C9;  )
                               f   =   1   ( 2
                    &#x005E;       &#x03C0; )                f
                    (  &#x03BE;  ) n 2            &#x005E;
                    =  &#x222B;    &#x222B;    R  (  &#x03BD;  )
                    R   n     f    n     f (  x   =  &#x222B;
                    (  x  )  e     )  e  &#x2212; R   n     f
                    &#x2212; 2     i  &#x03C9;    (  x  )  e
                    &#x03C0; i  x  &#x22C5;  x    &#x2212; i  x
                    &#x22C5;       d  x           &#x22C5;
                    &#x03BE;     d {\displaystyle &#x03BD;     d
                    x              {\begin        x
                    {\displaystyle {aligned}&     {\displaystyle
                    {\begin        {\hat {f}}(    {\begin
                    {aligned}&     {\boldsymbol   {aligned}&
                    {\hat {f}}(    {\omega        {\hat {f}}(
                    {\boldsymbol   }})\\&={\frac  {\boldsymbol
                    {\xi           {1}{{(2\pi )}^ {\nu
                    }})\\&=\int _  {\frac {n}     }})\\&=\int _
                    {\mathbb {R} ^ {2}}}}\int _   {\mathbb {R} ^
       f (  x  )    {n}}f(\mathbf  {\mathbb {R} ^ {n}}f(\mathbf
    {\displaystyle  {x} )e^{-2\pi  {n}}f(\mathbf  {x} )e^{-
    f(\mathbf {x}   i\mathbf {x}   {x} )e^{-i     i\mathbf {x}
500 )\,}  [         \cdot          {\boldsymbol   \cdot
    {\displaystyle  {\boldsymbol   {\omega        {\boldsymbol
    f(\mathbf {x}   {\xi           }}\cdot        {\nu
    )\,}]           }}}\,d\mathbf  \mathbf {x}    }}}\,d\mathbf
                    {x} \end       }\,d\mathbf    {x} \end
                    {aligned}}}  [ {x} \end       {aligned}}}  [
                    {\displaystyle {aligned}}}  [ {\displaystyle
                    {\begin        {\displaystyle {\begin
                    {aligned}&     {\begin        {aligned}&
                    {\hat {f}}(    {aligned}&     {\hat {f}}(
                    {\boldsymbol   {\hat {f}}(    {\boldsymbol
                    {\xi           {\boldsymbol   {\nu
                    }})\\&=\int _  {\omega        }})\\&=\int _
                    {\mathbb {R} ^ }})\\&={\frac  {\mathbb {R} ^
                    {n}}f(\mathbf  {1}{{(2\pi )}^ {n}}f(\mathbf
                    {x} )e^{-2\pi  {\frac {n}     {x} )e^{-
                    i\mathbf {x}   {2}}}}\int _   i\mathbf {x}
                    \cdot          {\mathbb {R} ^ \cdot
                    {\boldsymbol   {n}}f(\mathbf  {\boldsymbol
                    {\xi           {x} )e^{-i     {\nu
                    }}}\,d\mathbf  {\boldsymbol   }}}\,d\mathbf
                    {x} \end       {\omega        {x} \end
                    {aligned}}}]   }}\cdot        {aligned}}}]
                                   \mathbf {x}
                                   }\,d\mathbf
                                   {x} \end
                                   {aligned}}}]
                                                      &#x03C0;
                                       2          &#x2212;
                        &#x03C0;   &#x2212;       &#x03B4;
                    &#x2212;       &#x03B4;       &#x0393;
                    &#x03B4;       &#x0393;       ( &#x03B4; + 1
                    &#x0393;       ( &#x03B4; + 1 )   |
                    ( &#x03B4; + 1 )   |          &#x03BD;  2
                    )  |           &#x03C9;  |    &#x03C0;    |
                    &#x03BE;    |  &#x2212;   n 2 &#x2212;   n 2
                    &#x2212;   n 2 &#x2212;       &#x2212;
                    &#x2212;       &#x03B4;    J  &#x03B4;    J
                    &#x03B4;    J  n 2   +        n 2   +
                    n 2   +        &#x03B4;       &#x03B4;
        &#x03C7;    &#x03B4;   ( 2 (  |           (  |
    [ 0 , 1 ]       &#x03C0;  |    &#x03C9;   |   &#x03BD;   |
    (  |   x   |  ) &#x03BE;   |   )              )
    (  1 &#x2212;   )              {\displaystyle {\displaystyle
    |   x    |   2  {\displaystyle 2^{-\delta     \pi ^{-\delta
    )   &#x03B4;    \pi ^{-\delta  }\Gamma        }\Gamma
    {\displaystyle  }\Gamma        (\delta        (\delta
    \chi _{[0,1]}   (\delta +1)|   +1)\left|      +1)\left|
    (|\mathbf {x}   {\boldsymbol   {\boldsymbol   {\frac         The function Ï[0, 1] is the indicator_function of the interval [0, 1]. The function
501 |)\left(1-      {\xi }}|^{-    {\omega        {\boldsymbol   Î(x) is the gamma function. The function Jn/2 + Î´ is a Bessel function of the first
    |\mathbf {x} |^ {\frac {n}     }}\right|^{-   {\nu }}{2\pi   kind, with order n/2 + Î´. Taking n = 2 and Î´ = 0 produces 402.[51]
    {2}\right)^     {2}}-\delta    {\frac {n}     }}\right|^{-
    {\delta }}  [   }J_{{\frac {n} {2}}-\delta    {\frac {n}
    {\displaystyle  {2}}+\delta }  }J_{{\frac {n} {2}}-\delta
    \chi _{[0,1]}   (2\pi |        {2}}+\delta }  }J_{{\frac {n}
    (|\mathbf {x}   {\boldsymbol   (|{\boldsymbol {2}}+\delta }
    |)\left(1-      {\xi }}|)}  [  {\omega }}|)}  (|{\boldsymbol
    |\mathbf {x} |^ {\displaystyle [              {\nu }}|)}  [
    {2}\right)^     \pi ^{-\delta  {\displaystyle {\displaystyle
    {\delta }}]     }\Gamma        2^{-\delta     \pi ^{-\delta
                    (\delta +1)|   }\Gamma        }\Gamma
                    {\boldsymbol   (\delta        (\delta
                    {\xi }}|^{-    +1)\left|      +1)\left|
                    {\frac {n}     {\boldsymbol   {\frac
                    {2}}-\delta    {\omega        {\boldsymbol
                    }J_{{\frac {n} }}\right|^{-   {\nu }}{2\pi
                    {2}}+\delta }  {\frac {n}     }}\right|^{-
                    (2\pi |        {2}}-\delta    {\frac {n}
                    {\boldsymbol   }J_{{\frac {n} {2}}-\delta
                    {\xi }}|)}]    {2}}+\delta }  }J_{{\frac {n}
                                   (|{\boldsymbol {2}}+\delta }
                                   {\omega }}|)}] (|{\boldsymbol
                                                  {\nu }}|)}]
                          ( 2            ( 2
                    &#x03C0;  )    &#x03C0;  )          ( 2
                    &#x03B1;     c n 2      c  n  &#x03C0;  )  n
        |   x    |  n , &#x03B1;   , &#x03B1;     c  n ,
    &#x2212;        |   &#x03BE;   |   &#x03C9;   &#x03B1;
    &#x03B1;   ,  0 |   &#x2212;   |   &#x2212;   |   &#x03BD;
    < Re &#x2061;   ( n &#x2212;   ( n &#x2212;   |   &#x2212;
    &#x03B1; < n .  &#x03B1; )     &#x03B1; )     ( n &#x2212;   See Riesz_potential where the constant is given by
    {\displaystyle  {\displaystyle {\displaystyle &#x03B1; )         c  n , &#x03B1;   =  &#x03C0;   n 2     2  &#x03B1;      &#x0393;  (   &#x03B1; 2
    |\mathbf {x} |^ {\frac {(2\pi  {\frac {(2\pi  {\displaystyle )    &#x0393;  (    n &#x2212; &#x03B1;  2   )     .   {\displaystyle c_{n,\alpha
    {-\alpha        )^{\alpha }}   )^{\frac {n}   {\frac {(2\pi  }=\pi ^{\frac {n}{2}}2^{\alpha }{\frac {\Gamma \left({\frac {\alpha }{2}}\right)}
    },\quad         {c_{n,\alpha   {2}}}{c_       )^{n}}{c_      {\Gamma \left({\frac {n-\alpha }{2}}\right)}}.}  [{\displaystyle c_{n,\alpha }=\pi ^
502 0<\operatorname }}}|           {n,\alpha }}}| {n,\alpha }}}| {\frac {n}{2}}2^{\alpha }{\frac {\Gamma \left({\frac {\alpha }{2}}\right)}{\Gamma
    {Re} \alpha     {\boldsymbol   {\boldsymbol   {\boldsymbol   \left({\frac {n-\alpha }{2}}\right)}}.}]
    <n.}  [         {\xi }}|^{-(n- {\omega }}|^{- {\nu }}|^{-(n- The formula also holds for all Î± â  ân, ân â 1, ... by analytic continuation,
    {\displaystyle  \alpha )}}  [  (n-\alpha )}}  \alpha )}}  [  but then the function and its Fourier transforms need to be understood as suitably
    |\mathbf {x} |^ {\displaystyle [              {\displaystyle regularized tempered distributions. See homogeneous_distribution.[52]
    {-\alpha        {\frac {(2\pi  {\displaystyle {\frac {(2\pi
    },\quad         )^{\alpha }}   {\frac {(2\pi  )^{n}}{c_
    0<\operatorname {c_{n,\alpha   )^{\frac {n}   {n,\alpha }}}|
    {Re} \alpha     }}}|           {2}}}{c_       {\boldsymbol
    <n.}]           {\boldsymbol   {n,\alpha }}}| {\nu }}|^{-(n-
                    {\xi }}|^{-(n- {\boldsymbol   \alpha )}}]
                    \alpha )}}]    {\omega }}|^{-
                                   (n-\alpha )}}]
         1   |
    &#x03C3;  |
    (  2 &#x03C0;
    )    n 2
    e  &#x2212;   1                   ( 2
    2     x    T                   &#x03C0;  )
    &#x03C3;                       &#x2212;   n 2
    &#x2212;  T                    e  &#x2212;
    &#x03C3;            e          1 2                e
    &#x2212; 1    x &#x2212; 2     &#x03C9;    T  &#x2212;   1 2
    {\displaystyle  &#x03C0;  2    &#x03C3;       &#x03BD;    T
    {\frac {1}      &#x03BE;    T  &#x03C3;    T  &#x03C3;
    {\left|         &#x03C3;       &#x03C9;       &#x03C3;    T
    {\boldsymbol    &#x03C3;    T  {\displaystyle &#x03BD;
    {\sigma         &#x03BE;       (2\pi )^{-     {\displaystyle
    }}\right|\left  {\displaystyle {\frac {n}     e^{-{\frac {1}
    (2\pi \right)^  e^{-2\pi ^{2}  {2}}}e^{-      {2}}
    {\frac {n}      {\boldsymbol   {\frac {1}{2}} {\boldsymbol
    {2}}}}e^{-      {\xi }}^       {\boldsymbol   {\nu }}^
    {\frac {1}      {\mathrm {T} } {\omega }}^    {\mathrm {T} }
    {2}}\mathbf {x} {\boldsymbol   {\mathrm {T} } {\boldsymbol
    ^{\mathrm {T} } {\sigma }}     {\boldsymbol   {\sigma }}
    {\boldsymbol    {\boldsymbol   {\sigma }}     {\boldsymbol   This is the formula for a multivariate_normal_distribution normalized to 1 with a
503 {\sigma }}^{-   {\sigma }}^    {\boldsymbol   {\sigma }}^    mean of 0. Bold variables are vectors or matrices. Following the notation of the
    \mathrm {T} }   {\mathrm {T} } {\sigma }}^    {\mathrm {T} } aforementioned page, Î£ = Ï ÏT and Î£â1 = ÏâT Ïâ1
    {\boldsymbol    {\boldsymbol   {\mathrm {T} } {\boldsymbol
    {\sigma }}^{-   {\xi }}}}  [   {\boldsymbol   {\nu }}}}  [
    1}\mathbf {x}   {\displaystyle {\omega }}}}   {\displaystyle
    }}  [           e^{-2\pi ^{2}  [              e^{-{\frac {1}
    {\displaystyle  {\boldsymbol   {\displaystyle {2}}
    {\frac {1}      {\xi }}^       (2\pi )^{-     {\boldsymbol
    {\left|         {\mathrm {T} } {\frac {n}     {\nu }}^
    {\boldsymbol    {\boldsymbol   {2}}}e^{-      {\mathrm {T} }
    {\sigma         {\sigma }}     {\frac {1}{2}} {\boldsymbol
    }}\right|\left  {\boldsymbol   {\boldsymbol   {\sigma }}
    (2\pi \right)^  {\sigma }}^    {\omega }}^    {\boldsymbol
    {\frac {n}      {\mathrm {T} } {\mathrm {T} } {\sigma }}^
    {2}}}}e^{-      {\boldsymbol   {\boldsymbol   {\mathrm {T} }
    {\frac {1}      {\xi }}}}]     {\sigma }}     {\boldsymbol
    {2}}\mathbf {x}                {\boldsymbol   {\nu }}}}]
    ^{\mathrm {T} }                {\sigma }}^
    {\boldsymbol                   {\mathrm {T} }
    {\sigma }}^{-                  {\boldsymbol
    \mathrm {T} }                  {\omega }}}}]
    {\boldsymbol
    {\sigma }}^{-
    1}\mathbf {x}
    }}]
                                          c  n
                                   ( 2 &#x03C0;          c  n
                                   )    n + 2  2  ( 2 &#x03C0;
                                   &#x03B1;       )  n + 1
                           c  n    (  4  &#x03C0; &#x03B1;
                    &#x03B1;       2    &#x03B1;  (  4  &#x03C0;
                    (   &#x03B1;   2   +  |       2    &#x03B1;
                    2   +  |       &#x03C9;    |  2   +  |
                    &#x03BE;    |  2    )     n + &#x03BD;    |
                    2    )     n + 1  2           2    )     n +
                    1  2           {\displaystyle 1  2
                    {\displaystyle {\frac {c_{n}  {\displaystyle
        e  &#x2212; {\frac {c_     (2\pi )^{\frac {\frac {c_{n}
    2 &#x03C0;      {n}\alpha }    {n+2}          (2\pi )^
    &#x03B1;  |   x {\left(\alpha  {2}}\alpha }   {n+1}\alpha }
    |               ^{2}+|         {\left(4\pi ^  {\left(4\pi ^  Here[53]
    {\displaystyle  {\boldsymbol   {2}\alpha ^    {2}\alpha ^        c  n   =    &#x0393;  (    n + 1  2   )    &#x03C0;    n + 1  2      .
504 e^{-2\pi \alpha {\xi }}|^      {2}+|          {2}+|          {\displaystyle c_{n}={\frac {\Gamma \left({\frac {n+1}{2}}\right)}{\pi ^{\frac {n+1}
    |\mathbf {x}    {2}\right)^    {\boldsymbol   {\boldsymbol   {2}}}}.}  [{\displaystyle c_{n}={\frac {\Gamma \left({\frac {n+1}{2}}\right)}{\pi ^
    |}}  [          {\frac {n+1}   {\omega }}|^   {\nu }}|^      {\frac {n+1}{2}}}}.}]
    {\displaystyle  {2}}}}}  [     {2}\right)^    {2}\right)^
    e^{-2\pi \alpha {\displaystyle {\frac {n+1}   {\frac {n+1}
    |\mathbf {x}    {\frac {c_     {2}}}}}  [     {2}}}}}  [
    |}}]            {n}\alpha }    {\displaystyle {\displaystyle
                    {\left(\alpha  {\frac {c_{n}  {\frac {c_{n}
                    ^{2}+|         (2\pi )^{\frac (2\pi )^
                    {\boldsymbol   {n+2}          {n+1}\alpha }
                    {\xi }}|^      {2}}\alpha }   {\left(4\pi ^
                    {2}\right)^    {\left(4\pi ^  {2}\alpha ^
                    {\frac {n+1}   {2}\alpha ^    {2}+|
                    {2}}}}}]       {2}+|          {\boldsymbol
                                   {\boldsymbol   {\nu }}|^
                                   {\omega }}|^   {2}\right)^
                                   {2}\right)^    {\frac {n+1}
                                   {\frac {n+1}   {2}}}}}]
                                   {2}}}}}]
***** See also[edit] *****
    * Analog_signal_processing
    * BeeversâLipson_strip
    * Discrete_Fourier_transform
          o DFT_matrix
    * Fast_Fourier_transform
    * Fourier_integral_operator
    * Fourier_inversion_theorem
    * Fourier_multiplier
    * Fourier_series
    * Fourier_sine_transform
    * FourierâDeligne_transform
    * FourierâMukai_transform
    * Fractional_Fourier_transform
    * Indirect_Fourier_transform
    * Integral_transform
          o Hankel_transform
          o Hartley_transform
    * Laplace_transform
    * Linear_canonical_transform
    * Mellin_transform
    * Multidimensional_transform
    * NGC_4622, especially the image NGC 4622 Fourier transform m = 2.
    * Short-time_Fourier_transform
    * Space-time_Fourier_transform
    * Spectral_density
          o Spectral_density_estimation
    * Symbolic_integration
    * Time_stretch_dispersive_Fourier_transform
    * Transform_(mathematics)
***** Remarks[edit] *****
   1. ^ Up to an imaginary constant factor whose magnitude depends on what
      Fourier transform convention is used.
   2. ^ Depending on the application a Lebesgue_integral, distributional, or
      other approach may be most appropriate.
   3. ^ Vretblad_(2000) provides solid justification for these formal
      procedures without going too deeply into functional_analysis or the
      theory_of_distributions.
   4. ^ In relativistic_quantum_mechanics one encounters vector-valued Fourier
      transforms of multi-component wave functions. In quantum_field_theory,
      operator-valued Fourier transforms of operator-valued functions of
      spacetime are in frequent use, see for example Greiner_&_Reinhardt_
      (1996).
   5. ^ The function     f ( x ) = cos &#x2061; ( 2 &#x03C0;  &#x03BE;  0   x )
      &#x2261; cos &#x2061; ( &#x2212; 2 &#x03C0;  &#x03BE;  0   x )
      {\displaystyle f(x)=\cos(2\pi \xi _{0}x)\equiv \cos(-2\pi \xi _{0}x)}  [
      {\displaystyle f(x)=\cos(2\pi \xi _{0}x)\equiv \cos(-2\pi \xi _{0}x)}] is
      also a signal with frequency      &#x03BE;  0     {\displaystyle \xi _
      {0}}  [{\displaystyle \xi _{0}}], but the integral obviously produces
      identical responses at both      &#x03BE;  0     {\displaystyle \xi _{0}}
      [{\displaystyle \xi _{0}}] and     &#x2212;  &#x03BE;  0
      {\displaystyle -\xi _{0}}  [{\displaystyle -\xi _{0}}], which is also
      consistent with Euler's_formula:     cos &#x2061; ( 2 &#x03C0;  &#x03BE;
      0   x ) &#x2261;    1 2     e  i 2 &#x03C0;  &#x03BE;  0   x   +    1 2
      e  &#x2212; i 2 &#x03C0;  &#x03BE;  0   x   .   {\displaystyle \cos(2\pi
      \xi _{0}x)\equiv {\tfrac {1}{2}}e^{i2\pi \xi _{0}x}+{\tfrac {1}{2}}e^{-
      i2\pi \xi _{0}x}.}  [{\displaystyle \cos(2\pi \xi _{0}x)\equiv {\tfrac
      {1}{2}}e^{i2\pi \xi _{0}x}+{\tfrac {1}{2}}e^{-i2\pi \xi _{0}x}.}]
***** Notes[edit] *****
   1. ^ Kaiser_1994, p. 29.
   2. ^ Rahman_2011, p. 11.
   3. ^"Sign_Conventions_in_Electromagnetic_(EM)_Waves" (PDF).
   4. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   5. ^ Fourier_1822, p. 525.
   6. ^ Fourier_1878, p. 408.
   7. ^ (Jordan_1883) proves on pp. 216â226 the Fourier_integral_theorem
      before studying Fourier series.
   8. ^ Titchmarsh_1986, p. 1.
   9. ^ Rahman_2011, p. 10.
  10. ^ Folland_1989.
  11. ^ Fourier_1822.
  12. ^ Taneja_2008, p. 192.
  13. ^ a b Stein_&_Shakarchi_2003.
  14. ^ a b c d e Pinsky_2002.
  15. ^ a b c d e Katznelson_1976.
  16. ^ a b c d e f Stein_&_Weiss_1971.
  17. ^ Rudin_1987, p. 187.
  18. ^ Rudin_1987, p. 186.
  19. ^ a b Duoandikoetxea_2001.
  20. ^ a b Boashash_2003.
  21. ^ Condon_1937.
  22. ^ Howe_1980.
  23. ^ Paley_&_Wiener_1934.
  24. ^ Gelfand_&_Vilenkin_1964.
  25. ^ Kirillov_&_Gvishiani_1982.
  26. ^ Clozel_&_Delorme_1985, pp. 331â333.
  27. ^ de_Groot_&_Mazur_1984, p. 146.
  28. ^ Champeney_1987, p. 80.
  29. ^ a b c Kolmogorov_&_Fomin_1999.
  30. ^ Wiener_1949.
  31. ^ Champeney_1987, p. 63.
  32. ^ Widder_&_Wiener_1938, p. 537.
  33. ^ Pinsky_2002, p. 131.
  34. ^ Stein_&_Shakarchi_2003, p. 158.
  35. ^ Chatfield_2004, p. 113.
  36. ^ Fourier_1822, p. 441.
  37. ^ PoincarÃ©_1895, p. 102.
  38. ^ Whittaker_&_Watson_1927, p. 188.
  39. ^ Grafakos_2004.
  40. ^ Grafakos_&_Teschl_2013.
  41. ^ [1]
  42. ^ Stein_&_Weiss_1971, Thm. 2.3.
  43. ^ Pinsky_2002, p. 256.
  44. ^ Hewitt_&_Ross_1970, Chapter 8.
  45. ^ Knapp_2001.
  46. ^ Gradshteyn_et_al._2015.
  47. ^ Press_et_al._1992.
  48. ^ Bailey_&_Swarztrauber_1994.
  49. ^ Lado_1971.
  50. ^ Simonen_&_Olkkonen_1985.
  51. ^ Stein_&_Weiss_1971, Thm. IV.3.3.
  52. ^ Stein_&_Weiss_1971, Thm. 4.15.
  53. ^ In Gelfand_&_Shilov_1964, p. 363, with the non-unitary conventions of
      this table, the transform of      |   x    |   &#x03BB;
      {\displaystyle |\mathbf {x} |^{\lambda }}  [{\displaystyle |\mathbf {x}
      |^{\lambda }}] is given to be      2  &#x03BB; + n    &#x03C0;     1 2
      n      &#x0393;  (    &#x03BB; + n  2   )    &#x0393;  (  &#x2212;
      &#x03BB; 2    )      |   &#x03BD;    |   &#x2212; &#x03BB; &#x2212; n
      {\displaystyle 2^{\lambda +n}\pi ^{{\tfrac {1}{2}}n}{\frac {\Gamma \left(
      {\frac {\lambda +n}{2}}\right)}{\Gamma \left(-{\frac {\lambda }
      {2}}\right)}}|{\boldsymbol {\nu }}|^{-\lambda -n}}  [{\displaystyle 2^
      {\lambda +n}\pi ^{{\tfrac {1}{2}}n}{\frac {\Gamma \left({\frac {\lambda
      +n}{2}}\right)}{\Gamma \left(-{\frac {\lambda }{2}}\right)}}|{\boldsymbol
      {\nu }}|^{-\lambda -n}}] from which this follows, with     &#x03BB; =
      &#x2212; &#x03B1;   {\displaystyle \lambda =-\alpha }  [{\displaystyle
      \lambda =-\alpha }].
  54. ^ Stein_&_Weiss_1971, p. 6.
***** References[edit] *****
    * Bailey, David H.; Swarztrauber, Paul N. (1994), "A_fast_method_for_the
      numerical_evaluation_of_continuous_Fourier_and_Laplace_transforms" (PDF),
      SIAM_Journal_on_Scientific_Computing, 15 (5): 1105â1110,
      CiteSeerX 10.1.1.127.1534, doi:10.1137/0915067
.
    * Boashash, B., ed. (2003), Time-Frequency Signal Analysis and Processing:
      A Comprehensive Reference, Oxford: Elsevier Science, ISBN 978-0-08-
      044335-5
.
    * Bochner,_S.; Chandrasekharan,_K. (1949), Fourier Transforms, Princeton
      University_Press
.
    * Bracewell, R. N. (2000), The Fourier Transform and Its Applications (3rd
      ed.), Boston: McGraw-Hill, ISBN 978-0-07-116043-8
.
    * Campbell, George; Foster, Ronald (1948), Fourier Integrals for Practical
      Applications, New York: D. Van Nostrand Company, Inc.
.
    * Champeney, D.C. (1987), A Handbook of Fourier Theorems, Cambridge
      University_Press
.
    * Chatfield, Chris (2004), The_Analysis_of_Time_Series:_An_Introduction,
      Texts in Statistical Science (6th ed.), London: Chapman & Hall/CRC
.
    * Clozel, Laurent; Delorme, Patrice (1985), "Sur le thÃ©orÃ¨me de Paley-
      Wiener invariant pour les groupes de Lie rÃ©ductifs rÃ©els", Comptes
      Rendus de l'AcadÃ©mie des Sciences, SÃ©rie I, 300: 331â333
.
    * Condon,_E._U. (1937), "Immersion of the Fourier transform in a continuous
      group of functional transformations", Proc._Natl._Acad._Sci., 23 (3):
      158â164, Bibcode:1937PNAS...23..158C, doi:10.1073/pnas.23.3.158,
      PMC 1076889, PMID 16588141
.
    * de Groot, Sybren R.; Mazur, Peter (1984), Non-Equilibrium Thermodynamics
      (2nd ed.), New York: Dover
.
    * Duoandikoetxea, Javier (2001), Fourier Analysis, American_Mathematical
      Society, ISBN 978-0-8218-2172-5
.
    * Dym,_H.; McKean, H. (1985), Fourier Series and Integrals, Academic_Press,
      ISBN 978-0-12-226451-1
.
    * ErdÃ©lyi, Arthur, ed. (1954), Tables of Integral Transforms, Vol. 1,
      McGraw-Hill
.
    * Feller,_William (1971), An Introduction to Probability Theory and Its
      Applications, Vol. II (2nd ed.), New York: Wiley, MR 0270403
.
    * Folland, Gerald (1989), Harmonic analysis in phase space, Princeton
      University_Press
.
    * Fourier,_J.B._Joseph (1822), ThÃ©orie_analytique_de_la_chaleur (in
      French), Paris: Firmin Didot, pÃ¨re et fils, OCLC 2688081
.
    * Fourier,_J.B._Joseph (1878) [1822], The_Analytical_Theory_of_Heat,
      translated by Alexander Freeman, The University Press
 (translated from French).
    * Gradshteyn,_Izrail_Solomonovich; Ryzhik,_Iosif_Moiseevich; Geronimus,
      Yuri_Veniaminovich; Tseytlin,_Michail_Yulyevich; Jeffrey, Alan (2015),
      Zwillinger, Daniel; Moll, Victor Hugo (eds.), Table_of_Integrals,_Series,
      and_Products, translated by Scripta Technica, Inc. (8th ed.), Academic
      Press, ISBN 978-0-12-384933-5
.
    * Grafakos, Loukas (2004), Classical and Modern Fourier Analysis, Prentice-
      Hall, ISBN 978-0-13-035399-3
.
    * Grafakos, Loukas; Teschl,_Gerald (2013), "On Fourier transforms of radial
      functions and distributions", J. Fourier Anal. Appl., 19: 167â179,
      arXiv:1112.5469, doi:10.1007/s00041-012-9242-5
.
    * Greiner, W.; Reinhardt, J. (1996), Field Quantization, Springer,
      ISBN 978-3-540-59179-5
.
    * Gelfand,_I.M.; Shilov,_G.E. (1964), Generalized Functions, Vol. 1, New
      York: Academic_Press
 (translated from Russian).
    * Gelfand,_I.M.; Vilenkin,_N.Y. (1964), Generalized Functions, Vol. 4, New
      York: Academic_Press
 (translated from Russian).
    * Hewitt, Edwin; Ross, Kenneth A. (1970), Abstract harmonic analysis, Die
      Grundlehren der mathematischen Wissenschaften, Band 152, Vol. II:
      Structure and analysis for compact groups. Analysis on locally compact
      Abelian groups, Springer, MR 0262773
.
    * HÃ¶rmander,_L. (1976), Linear Partial Differential Operators, Vol. 1,
      Springer, ISBN 978-3-540-00662-6
.
    * Howe, Roger (1980), "On the role of the Heisenberg group in harmonic
      analysis", Bulletin_of_the_American_Mathematical_Society, 3 (2):
      821â844, Bibcode:1994BAMaS..30..205W, doi:10.1090/S0273-0979-1980-
      14825-9, MR 0578375
.
    * James, J.F. (2011), A Student's Guide to Fourier Transforms (3rd ed.),
      Cambridge_University_Press, ISBN 978-0-521-17683-5
.
    * Jordan,_Camille (1883), Cours d'Analyse de l'Ãcole Polytechnique, Vol.
      II, Calcul IntÃ©gral: IntÃ©grales dÃ©finies et indÃ©finies (2nd ed.),
      Paris
.
    * Kaiser, Gerald (1994), "A_Friendly_Guide_to_Wavelets", Physics Today, 48
      (7): 57â58, Bibcode:1995PhT....48g..57K, doi:10.1063/1.2808105,
      ISBN 978-0-8176-3711-8
.
    * Kammler, David (2000), A First Course in Fourier Analysis, Prentice Hall,
      ISBN 978-0-13-578782-3
.
    * Katznelson, Yitzhak (1976), An Introduction to Harmonic Analysis, Dover,
      ISBN 978-0-486-63331-2
.
    * Kirillov,_Alexandre; Gvishiani, Alexei D. (1982) [1979], Theorems and
      Problems in Functional Analysis, Springer
 (translated from Russian).
    * Knapp, Anthony W. (2001), Representation_Theory_of_Semisimple_Groups:_An
      Overview_Based_on_Examples, Princeton_University_Press, ISBN 978-0-691-
      09089-4
.
    * Kolmogorov,_Andrey_Nikolaevich; Fomin,_Sergei_Vasilyevich (1999) [1957],
      Elements_of_the_Theory_of_Functions_and_Functional_Analysis, Dover
 (translated from Russian).
    * Lado, F. (1971), "Numerical_Fourier_transforms_in_one,_two,_and_three
      dimensions_for_liquid_state_calculations", Journal_of_Computational
      Physics, 8 (3): 417â433, Bibcode:1971JCoPh...8..417L, doi:10.1016/0021-
      9991(71)90021-0
.
    * MÃ¼ller, Meinard (2015), The_Fourier_Transform_in_a_Nutshell. (PDF), In
      Fundamentals_of_Music_Processing, Section 2.1, pages 40-56: Springer,
      doi:10.1007/978-3-319-21945-5, ISBN 978-3-319-21944-8
.
    * Paley,_R.E.A.C.; Wiener,_Norbert (1934), Fourier Transforms in the
      Complex Domain, American Mathematical Society Colloquium Publications
      (19), Providence, Rhode Island: American_Mathematical_Society
.
    * Pinsky, Mark (2002), Introduction_to_Fourier_Analysis_and_Wavelets,
      Brooks/Cole, ISBN 978-0-534-37660-4
.
    * PoincarÃ©,_Henri (1895), ThÃ©orie_analytique_de_la_propagation_de_la
      chaleur, Paris: CarrÃ©
.
    * Polyanin, A. D.; Manzhirov, A. V. (1998), Handbook of Integral Equations,
      Boca Raton: CRC_Press, ISBN 978-0-8493-2876-3
.
    * Press, William H.; Flannery, Brian P.; Teukolsky, Saul A.; Vetterling,
      William T. (1992), Numerical Recipes in C: The Art of Scientific
      Computing, Second Edition (2nd ed.), Cambridge_University_Press
.
    * Rahman, Matiur (2011), Applications_of_Fourier_Transforms_to_Generalized
      Functions, WIT Press, ISBN 978-1-84564-564-9
.
    * Rudin, Walter (1987), Real and Complex Analysis (3rd ed.), Singapore:
      McGraw Hill, ISBN 978-0-07-100276-9
.
    * Simonen, P.; Olkkonen, H. (1985), "Fast method for computing the Fourier
      integral transform via Simpson's numerical integration", Journal of
      Biomedical Engineering, 7 (4): 337â340, doi:10.1016/0141-5425(85)90067-
      6
.
    * Stein, Elias; Shakarchi, Rami (2003), Fourier_Analysis:_An_introduction,
      Princeton_University_Press, ISBN 978-0-691-11384-5
.
    * Stein,_Elias; Weiss,_Guido (1971), Introduction_to_Fourier_Analysis_on
      Euclidean_Spaces, Princeton, N.J.: Princeton_University_Press, ISBN 978-
      0-691-08078-9
.
    * Taneja, H.C. (2008), "Chapter_18:_Fourier_integrals_and_Fourier
      transforms", Advanced Engineering Mathematics, Vol. 2, New Delhi, India:
      I. K. International Pvt Ltd, ISBN 978-8189866563
.
    * Titchmarsh,_E. (1986) [1948], Introduction to the theory of Fourier
      integrals (2nd ed.), Oxford University: Clarendon_Press, ISBN 978-0-8284-
      0324-5
.
    * Vretblad, Anders (2000), Fourier Analysis and its Applications, Graduate
      Texts_in_Mathematics, 223, New York: Springer, ISBN 978-0-387-00836-3
.
    * Whittaker,_E._T.; Watson,_G._N. (1927), A_Course_of_Modern_Analysis (4th
      ed.), Cambridge_University_Press
.
    * Widder, David Vernon; Wiener,_Norbert (August 1938), "Remarks on the
      Classical Inversion Formula for the Laplace Integral", Bulletin of the
      American Mathematical Society, 44 (8): 573â575, Bibcode:
      1994BAMaS..30..205W, doi:10.1090/s0002-9904-1938-06812-7
.
    * Wiener,_Norbert (1949), Extrapolation, Interpolation, and Smoothing of
      Stationary Time Series With Engineering Applications, Cambridge, Mass.:
      Technology Press and John Wiley & Sons and Chapman & Hall
.
    * Wilson, R. G. (1995), Fourier Series and Optical Transform Techniques in
      Contemporary Optics, New York: Wiley, ISBN 978-0-471-30357-2
.
    * Yosida,_K. (1968), Functional Analysis, Springer, ISBN 978-3-540-58654-8
.
***** External links[edit] *****
    * Encyclopedia_of_Mathematics
    * Weisstein,_Eric_W. "Fourier_Transform". MathWorld.
                                              * GND: 4018014-1
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85051094
                                              * NDL: 00562090

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Fourier_transform&oldid=907515227"
Categories:
    * Fourier_analysis
    * Integral_transforms
    * Unitary_operators
    * Joseph_Fourier
    * Mathematical_physics
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2009
    * CS1:_long_volume_value
    * CS1_French-language_sources_(fr)
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
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
    * á áá­á
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Boarisch
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LietuviÅ³
    * Magyar
    * Malti
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * áá¼ááºáá¬áá¬áá¬
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 23 July 2019, at 12:45 (UTC).
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
