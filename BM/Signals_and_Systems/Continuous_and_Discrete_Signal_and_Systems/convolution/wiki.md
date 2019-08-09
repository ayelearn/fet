The following text has been accessed from https://en.wikipedia.org/wiki/Convolution at Fri Aug 9 02:47:32 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Convolution ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For the usage in formal language theory, see Convolution_(computer_science).
For other uses, see Convolute.
Visual comparison of convolution, cross-correlation, and autocorrelation. For
the operations involving function f, and assuming the height of f is 1.0, the
value of the result at 5 different points is indicated by the shaded area below
each point. Also, the symmetry of f is the reason     f &#x2217; g
{\displaystyle f*g}  [f*g] and     f &#x22C6; g   {\displaystyle f\star g}
[f\star g] are identical in this example.
In mathematics (in particular, functional_analysis) convolution is a
mathematical_operation on two functions (f and g) to produce a third function
that expresses how the shape of one is modified by the other. The term
convolution refers to both the result function and to the process of computing
it. It is defined as the integral of the product of the two functions after one
is reversed and shifted.
Some features of convolution are similar to cross-correlation: for real-valued
functions, of a continuous or discrete variable, it differs from cross-
correlation only in that either f (x) or g(x) is reflected about the y-axis;
thus it is a cross-correlation of f (x) and g(âx), or f (âx) and g(x).[note
1]  For continuous functions, the cross-correlation operator is the adjoint of
the convolution operator.
Convolution has applications that include probability, statistics, computer
vision, natural_language_processing, image and signal_processing, engineering,
and differential_equations.[citation_needed]
The convolution can be defined for functions on Euclidean_space, and other
groups.[citation_needed] For example, periodic_functions, such as the discrete-
time_Fourier_transform, can be defined on a circle and convolved by periodic
convolution. (See row 18 at DTFT_§_Properties.) A discrete convolution can be
defined for functions on the set of integers.
Generalizations of convolution have applications in the field of numerical
analysis and numerical_linear_algebra, and in the design and implementation of
finite_impulse_response filters in signal processing.[citation_needed]
Computing the inverse of the convolution operation is known as deconvolution.
⁰
***** Contents *****
    * 1_Definition
          o 1.1_Notation
          o 1.2_Derivations
    * 2_Visual_explanation
    * 3_Historical_developments
    * 4_Circular_convolution
    * 5_Discrete_convolution
          o 5.1_Circular_discrete_convolution
          o 5.2_Fast_convolution_algorithms
    * 6_Domain_of_definition
          o 6.1_Compactly_supported_functions
          o 6.2_Integrable_functions
          o 6.3_Functions_of_rapid_decay
          o 6.4_Distributions
          o 6.5_Measures
    * 7_Properties
          o 7.1_Algebraic_properties
          o 7.2_Integration
          o 7.3_Differentiation
          o 7.4_Convolution_theorem
          o 7.5_Translational_equivariance
    * 8_Convolutions_on_groups
    * 9_Convolution_of_measures
    * 10_Bialgebras
    * 11_Applications
    * 12_See_also
    * 13_Notes
    * 14_References
    * 15_Further_reading
    * 16_External_links
***** Definition[edit] *****
The convolution of f and g is written fâg, using an asterisk. It is defined
as the integral of the product of the two functions after one is reversed and
shifted. As such, it is a particular kind of integral_transform:
   ( f &#x2217; g ) ( t ) &#x225C; &#xA0;  &#x222B;  &#x2212; &#x221E;
&#x221E;   f ( &#x03C4; ) g ( t &#x2212; &#x03C4; )  d &#x03C4; .
{\displaystyle (f*g)(t)\triangleq \ \int _{-\infty }^{\infty }f(\tau )g(t-\tau
)\,d\tau .}  [{\displaystyle (f*g)(t)\triangleq \ \int _{-\infty }^{\infty }f
(\tau )g(t-\tau )\,d\tau .}]
An equivalent definition is (see commutativity):
         ( f &#x2217; g ) ( t ) &#x225C; &#xA0;  &#x222B;  &#x2212; &#x221E;
      &#x221E;   f ( t &#x2212; &#x03C4; ) g ( &#x03C4; )  d &#x03C4; .
      {\displaystyle (f*g)(t)\triangleq \ \int _{-\infty }^{\infty }f(t-\tau )g
      (\tau )\,d\tau .}  [{\displaystyle (f*g)(t)\triangleq \ \int _{-\infty }^
      {\infty }f(t-\tau )g(\tau )\,d\tau .}]
While the symbol t is used above, it need not represent the time domain.  But
in that context, the convolution formula can be described as a weighted average
of the function f (Ï) at the moment t where the weighting is given by g(âÏ)
simply shifted by amount t.  As t changes, the weighting function emphasizes
different parts of the input function.
For functions f, g supported on only [0, â) (i.e., zero for negative
arguments), the integration limits can be truncated, resulting in:
         ( f &#x2217; g ) ( t ) =  &#x222B;  0   t   f ( &#x03C4; ) g ( t
      &#x2212; &#x03C4; )  d &#x03C4;  &#xA0;  for&#xA0;  f , g : [ 0 ,
      &#x221E; ) &#x2192;  R  .   {\displaystyle (f*g)(t)=\int _{0}^{t}f(\tau
      )g(t-\tau )\,d\tau \quad \ {\text{for }}f,g:[0,\infty )\to \mathbb {R} .}
      [{\displaystyle (f*g)(t)=\int _{0}^{t}f(\tau )g(t-\tau )\,d\tau \quad \
      {\text{for }}f,g:[0,\infty )\to \mathbb {R} .}]
For the multi-dimensional formulation of convolution, see domain_of_definition
(below).
**** Notation[edit] ****
A common engineering convention is:[1]
         f ( t ) &#x2217; g ( t )  &#x225C; &#xA0;      &#x222B;  &#x2212;
      &#x221E;   &#x221E;   f ( &#x03C4; ) g ( t &#x2212; &#x03C4; )  d
      &#x03C4;  &#x23DF;    ( f &#x2217; g ) ( t )   ,   {\displaystyle f(t)*g
      (t)\,\triangleq \ \underbrace {\int _{-\infty }^{\infty }f(\tau )g(t-\tau
      )\,d\tau } _{(f*g)(t)},}  [{\displaystyle f(t)*g(t)\,\triangleq \
      \underbrace {\int _{-\infty }^{\infty }f(\tau )g(t-\tau )\,d\tau } _{
      (f*g)(t)},}]
which has to be interpreted carefully to avoid confusion.  For instance, f
(t)âg(t â t0) is equivalent to (f âg)(t â t0),  but f (t â t0)âg(t
â t0) is in fact equivalent to (f âg)(t â 2t0).[2]
**** Derivations[edit] ****
Convolution describes the output (in terms of the input) of an important class
of operations known as linear time-invariant (LTI). See LTI_system_theory for a
derivation of convolution as the result of LTI constraints. In terms of the
Fourier_transforms of the input and output of an LTI operation, no new
frequency components are created. The existing ones are only modified
(amplitude and/or phase). In other words, the output transform is the pointwise
product of the input transform with a third transform (known as a transfer
function). See Convolution_theorem for a derivation of that property of
convolution. Conversely, convolution can be derived as the inverse Fourier
transform of the pointwise product of two Fourier transforms.
***** Visual explanation[edit] *****
Visual explanations of convolution
   1. Express each function in terms of a dummy_variable     &#x03C4; .
      {\displaystyle \tau .}  [\tau .]
   2. Reflect one of the functions:     g ( &#x03C4; )   {\displaystyle g(\tau )}
      [g(\tau )]â    g ( &#x2212; &#x03C4; ) .   {\displaystyle g(-\tau ).}  [g(-
      \tau ).]
   3. Add a time-offset, t, which allows     g ( t &#x2212; &#x03C4; )
      {\displaystyle g(t-\tau )}  [g(t-\tau )] to slide along the     &#x03C4;
      {\displaystyle \tau }  [\tau ]-axis.
   4. Start t at ââ and slide it all the way to +â. Wherever the two
      functions intersect, find the integral of their product. In other words,
      compute a sliding, weighted-sum of function     f ( &#x03C4; ) ,              [Convolution3.svg]
      {\displaystyle f(\tau ),}  [f(\tau ),] where the weighting function is     g
      ( &#x2212; &#x03C4; ) .   {\displaystyle g(-\tau ).}  [g(-\tau ).]
      The resulting waveform (not shown here) is the convolution of functions f and
      g.
      If f (t) is a unit_impulse, the result of this process is simply g(t).
      Formally:
                &#x222B;  &#x2212; &#x221E;   &#x221E;   &#x03B4; ( &#x03C4; ) g
            ( t &#x2212; &#x03C4; )  d &#x03C4; = g ( t )   {\displaystyle \int _{-
            \infty }^{\infty }\delta (\tau )g(t-\tau )\,d\tau =g(t)}  [
            {\displaystyle \int _{-\infty }^{\infty }\delta (\tau )g(t-\tau
            )\,d\tau =g(t)}]
      In this example, the red-colored "pulse",     &#xA0; g ( &#x03C4; ) ,
      {\displaystyle \ g(\tau ),}  [{\displaystyle \ g(\tau ),}] is an even
      function     ( &#xA0; g ( &#x2212; &#x03C4; ) = g ( &#x03C4; ) &#xA0; ) ,
      {\displaystyle (\ g(-\tau )=g(\tau )\ ),}  [(\ g(-\tau )=g(\tau )\ ),] so
      convolution is equivalent to correlation. A snapshot of this "movie" shows
      functions     g ( t &#x2212; &#x03C4; )   {\displaystyle g(t-\tau )}  [g(t-
      \tau )] and     f ( &#x03C4; )   {\displaystyle f(\tau )}  [f(\tau )] (in
      blue) for some value of parameter     t ,   {\displaystyle t,}  [t,] which is [Convolution_of
      arbitrarily defined as the distance from the     &#x03C4; = 0                 box_signal_with
      {\displaystyle \tau =0}  [\tau =0] axis to the center of the red pulse. The   itself2.gif]
      amount of yellow is the area of the product     f ( &#x03C4; ) &#x22C5; g ( t
      &#x2212; &#x03C4; ) ,   {\displaystyle f(\tau )\cdot g(t-\tau ),}  [f(\tau
      )\cdot g(t-\tau ),] computed by the convolution/correlation integral. The
      movie is created by continuously changing     t   {\displaystyle t}  [t] and
      recomputing the integral. The result (shown in black) is a function of     t
      ,   {\displaystyle t,}  [t,] but is plotted on the same axis as     &#x03C4;
      ,   {\displaystyle \tau ,}  [\tau ,] for convenience and comparison.
      In this depiction,     f ( &#x03C4; )   {\displaystyle f(\tau )}  [f(\tau )]
      could represent the response of an RC circuit to a narrow pulse that occurs
      at     &#x03C4; = 0.   {\displaystyle \tau =0.}  [\tau =0.] In other words,
      if     g ( &#x03C4; ) = &#x03B4; ( &#x03C4; ) ,   {\displaystyle g(\tau
      )=\delta (\tau ),}  [g(\tau )=\delta (\tau ),] the result of convolution is   [Convolution_of
      just     f ( t ) .   {\displaystyle f(t).}  [f(t).] But when     g ( &#x03C4; spiky_function
      )   {\displaystyle g(\tau )}  [g(\tau )] is the wider pulse (in red), the     with_box2.gif]
      response is a "smeared" version of     f ( t ) .   {\displaystyle f(t).}  [f
      (t).] It begins at     t = &#x2212; 0.5 ,   {\displaystyle t=-0.5,}  [t=-
      0.5,] because we defined     t   {\displaystyle t}  [t] as the distance from
      the     &#x03C4; = 0   {\displaystyle \tau =0}  [\tau =0] axis to the center
      of the wide pulse (instead of the leading edge).
***** Historical developments[edit] *****
One of the earliest uses of the convolution integral appeared in D'Alembert's
derivation of Taylor's_theorem in Recherches sur diffÃ©rents points importants
du systÃ¨me du monde, published in 1754.[3]
Also, an expression of the type:
         &#x222B; f ( u ) &#x22C5; g ( x &#x2212; u )  d u   {\displaystyle
      \int f(u)\cdot g(x-u)\,du}  [{\displaystyle \int f(u)\cdot g(x-u)\,du}]
is used by Sylvestre_FranÃ§ois_Lacroix on page 505 of his book entitled
Treatise on differences and series, which is the last of 3 volumes of the
encyclopedic series: TraitÃ© du calcul diffÃ©rentiel et du calcul intÃ©gral,
Chez Courcier, Paris, 1797â1800.[4] Soon thereafter, convolution operations
appear in the works of Pierre_Simon_Laplace, Jean-Baptiste_Joseph_Fourier,
SimÃ©on_Denis_Poisson, and others. The term itself did not come into wide use
until the 1950s or 60s. Prior to that it was sometimes known as Faltung (which
means folding in German), composition product, superposition integral, and
Carson's integral.[5] Yet it appears as early as 1903, though the definition is
rather unfamiliar in older uses.[6][7]
The operation:
          &#x222B;  0   t   &#x03C6; ( s ) &#x03C8; ( t &#x2212; s )  d s ,  0
      &#x2264; t < &#x221E; ,   {\displaystyle \int _{0}^{t}\varphi (s)\psi (t-
      s)\,ds,\qquad 0\leq t<\infty ,}  [{\displaystyle \int _{0}^{t}\varphi
      (s)\psi (t-s)\,ds,\qquad 0\leq t<\infty ,}]
is a particular case of composition products considered by the Italian
mathematician Vito_Volterra in 1913.[8]
***** Circular convolution[edit] *****
Main article: Circular_convolution
When a function gT is periodic, with period T, then for functions, f, such that
f â gT exists, the convolution is also periodic and identical to:
         ( f &#x2217;  g  T   ) ( t ) &#x2261;  &#x222B;   t  0      t  0   + T
      [   &#x2211;  k = &#x2212; &#x221E;   &#x221E;   f ( &#x03C4; + k T )  ]
      g  T   ( t &#x2212; &#x03C4; )  d &#x03C4; ,   {\displaystyle (f*g_{T})
      (t)\equiv \int _{t_{0}}^{t_{0}+T}\left[\sum _{k=-\infty }^{\infty }f(\tau
      +kT)\right]g_{T}(t-\tau )\,d\tau ,}  [(f*g_{T})(t)\equiv \int _{t_{0}}^
      {t_{0}+T}\left[\sum _{k=-\infty }^{\infty }f(\tau +kT)\right]g_{T}(t-\tau
      )\,d\tau ,]
where t0 is an arbitrary choice. The summation is called a periodic_summation
of the function f.
When gT is a periodic summation of another function, g, then f â gT is known
as a circular or cyclic convolution of f and g.
And if the periodic summation above is replaced by fT, the operation is called
a periodic convolution of fT and gT.
***** Discrete convolution[edit] *****
For complex-valued functions f, g defined on the set Z of integers, the
discrete convolution of f and g is given by:[9]
   ( f &#x2217; g ) [ n ] =  &#x2211;  m = &#x2212; &#x221E;   &#x221E;   f [ m
] g [ n &#x2212; m ]   {\displaystyle (f*g)[n]=\sum _{m=-\infty }^{\infty }f
[m]g[n-m]}  [{\displaystyle (f*g)[n]=\sum _{m=-\infty }^{\infty }f[m]g[n-m]}]
or equivalently (see commutativity) by:
         ( f &#x2217; g ) [ n ] =  &#x2211;  m = &#x2212; &#x221E;   &#x221E;
      f [ n &#x2212; m ] g [ m ] .   {\displaystyle (f*g)[n]=\sum _{m=-\infty
      }^{\infty }f[n-m]g[m].}  [{\displaystyle (f*g)[n]=\sum _{m=-\infty }^
      {\infty }f[n-m]g[m].}]
The convolution of two finite sequences is defined by extending the sequences
to finitely supported functions on the set of integers. When the sequences are
the coefficients of two polynomials, then the coefficients of the ordinary
product of the two polynomials are the convolution of the original two
sequences. This is known as the Cauchy_product of the coefficients of the
sequences.
Thus when g has finite support in the set     { &#x2212; M , &#x2212; M + 1 ,
&#x2026; , M &#x2212; 1 , M }   {\displaystyle \{-M,-M+1,\dots ,M-1,M\}}  [\{-
M,-M+1,\dots ,M-1,M\}] (representing, for instance, a finite_impulse_response),
a finite summation may be used:[10]
         ( f &#x2217; g ) [ n ] =  &#x2211;  m = &#x2212; M   M   f [ n
      &#x2212; m ] g [ m ] .   {\displaystyle (f*g)[n]=\sum _{m=-M}^{M}f[n-m]g
      [m].}  [{\displaystyle (f*g)[n]=\sum _{m=-M}^{M}f[n-m]g[m].}]
**** Circular discrete convolution[edit] ****
When a function gN is periodic, with period N, then for functions, f, such that
fâgN exists, the convolution is also periodic and identical to:
         ( f &#x2217;  g  N   ) [ n ] &#x2261;  &#x2211;  m = 0   N &#x2212; 1
      (   &#x2211;  k = &#x2212; &#x221E;   &#x221E;    f  [ m + k N ]  )   g
      N   [ n &#x2212; m ] .   {\displaystyle (f*g_{N})[n]\equiv \sum _{m=0}^
      {N-1}\left(\sum _{k=-\infty }^{\infty }{f}[m+kN]\right)g_{N}[n-m].}  [
      {\displaystyle (f*g_{N})[n]\equiv \sum _{m=0}^{N-1}\left(\sum _{k=-\infty
      }^{\infty }{f}[m+kN]\right)g_{N}[n-m].}]
The summation on k is called a periodic_summation of the function f.
If gN is a periodic summation of another function, g, then fâgN is known as a
circular_convolution of f and g.
When the non-zero durations of both f and g are limited to the interval [0,
Nâ1],  fâgN reduces to these common forms:
             ( f &#x2217;  g  N   ) [ n ]    =  &#x2211;  m = 0
      N &#x2212; 1   f [ m ]  g  N   [ n &#x2212; m ]       =
      &#x2211;  m = 0   n   f [ m ] g [ n &#x2212; m ] +  &#x2211;
      m = n + 1   N &#x2212; 1   f [ m ] g [ N + n &#x2212; m ]
      =  &#x2211;  m = 0   N &#x2212; 1   f [ m ] g [ ( n &#x2212;
      m  )  mod  N    ] &#x225C; ( f  &#x2217;     N     g ) [ n ]
      {\displaystyle {\begin{aligned}(f*g_{N})[n]&=\sum _{m=0}^{N-    (Eq.1)
      1}f[m]g_{N}[n-m]\\&=\sum _{m=0}^{n}f[m]g[n-m]+\sum _{m=n+1}^    
      {N-1}f[m]g[N+n-m]\\&=\sum _{m=0}^{N-1}f[m]g[(n-m)_{\bmod
      {N}}]\triangleq (f*_{_{N}}g)[n]\end{aligned}}}  [
      {\displaystyle {\begin{aligned}(f*g_{N})[n]&=\sum _{m=0}^{N-
      1}f[m]g_{N}[n-m]\\&=\sum _{m=0}^{n}f[m]g[n-m]+\sum _{m=n+1}^
      {N-1}f[m]g[N+n-m]\\&=\sum _{m=0}^{N-1}f[m]g[(n-m)_{\bmod
      {N}}]\triangleq (f*_{_{N}}g)[n]\end{aligned}}}]
The notation (f âN g) for cyclic convolution denotes convolution over the
cyclic_group of integers_modulo_N.
Circular convolution arises most often in the context of fast convolution with
a fast_Fourier_transform (FFT) algorithm.
**** Fast convolution algorithms[edit] ****
In many situations, discrete convolutions can be converted to circular
convolutions so that fast transforms with a convolution property can be used to
implement the computation. For example, convolution of digit sequences is the
kernel operation in multiplication of multi-digit numbers, which can therefore
be efficiently implemented with transform techniques (Knuth_1997, Â§4.3.3.C;
von_zur_Gathen_&_Gerhard_2003, Â§8.2).
Eq.1 requires N arithmetic operations per output value and N2 operations for N
outputs. That can be significantly reduced with any of several fast algorithms.
Digital_signal_processing and other applications typically use fast convolution
algorithms to reduce the cost of the convolution to O(N log N) complexity.
The most common fast convolution algorithms use fast_Fourier_transform (FFT)
algorithms via the circular_convolution_theorem. Specifically, the circular
convolution of two finite-length sequences is found by taking an FFT of each
sequence, multiplying pointwise, and then performing an inverse FFT.
Convolutions of the type defined above are then efficiently implemented using
that technique in conjunction with zero-extension and/or discarding portions of
the output. Other fast convolution algorithms, such as the
SchÃ¶nhageâStrassen_algorithm or the Mersenne transform,[11] use fast Fourier
transforms in other rings.
If one sequence is much longer than the other, zero-extension of the shorter
sequence and fast circular convolution is not the most computationally
efficient method available.[12] Instead, decomposing the longer sequence into
blocks and convolving each block allows for faster algorithms such as the
Overlapâsave_method and Overlapâadd_method.[13] A hybrid convolution method
that combines block and FIR algorithms allows for a zero input-output latency
that is useful for real-time convolution computations.[14]
***** Domain of definition[edit] *****
The convolution of two complex-valued functions on Rd is itself a complex-
valued function on Rd, defined by:
         ( f &#x2217; g ) ( x ) =  &#x222B;    R   d     f ( y ) g ( x &#x2212;
      y )  d y =  &#x222B;    R   d     f ( x &#x2212; y ) g ( y )  d y ,
      {\displaystyle (f*g)(x)=\int _{\mathbf {R} ^{d}}f(y)g(x-y)\,dy=\int _
      {\mathbf {R} ^{d}}f(x-y)g(y)\,dy,}  [(f*g)(x)=\int _{\mathbf {R} ^{d}}f
      (y)g(x-y)\,dy=\int _{\mathbf {R} ^{d}}f(x-y)g(y)\,dy,]
is well-defined only if f and g decay sufficiently rapidly at infinity in order
for the integral to exist. Conditions for the existence of the convolution may
be tricky, since a blow-up in g at infinity can be easily offset by
sufficiently rapid decay in f. The question of existence thus may involve
different conditions on f and g:
**** Compactly supported functions[edit] ****
If f and g are compactly_supported continuous_functions, then their convolution
exists, and is also compactly supported and continuous (HÃ¶rmander_1983,
Chapter 1). More generally, if either function (say f) is compactly supported
and the other is locally_integrable, then the convolution fâg is well-defined
and continuous.
Convolution of f and g is also well defined when both functions are locally
square integrable on R and supported on an interval of the form [a, +â) (or
both supported on [ââ, a]).
**** Integrable functions[edit] ****
The convolution of f and g exists if f and g are both Lebesgue_integrable
functions in L1(Rd), and in this case fâg is also integrable (Stein_&_Weiss
1971, Theorem 1.3). This is a consequence of Tonelli's_theorem. This is also
true for functions in L1, under the discrete convolution, or more generally for
the convolution_on_any_group.
Likewise, if f â L1(Rd)  and  g â Lp(Rd)  where 1 â¤ p â¤ â,  then
 fâg â Lp(Rd),  and
         &#x2016;  f  &#x2217; g  &#x2016;  p   &#x2264; &#x2016; f  &#x2016;
      1   &#x2016; g  &#x2016;  p   .   {\displaystyle \|{f}*g\|_{p}\leq \|f\|_
      {1}\|g\|_{p}.}  [{\displaystyle \|{f}*g\|_{p}\leq \|f\|_{1}\|g\|_{p}.}]
In the particular case p = 1, this shows that L1 is a Banach_algebra under the
convolution (and equality of the two sides holds if f and g are non-negative
almost everywhere).
More generally, Young's_inequality implies that the convolution is a continuous
bilinear map between suitable Lp spaces. Specifically, if  1 â¤ p, q, r â¤
â  satisfy:
           1 p   +   1 q   =   1 r   + 1 ,   {\displaystyle {\frac {1}{p}}+
      {\frac {1}{q}}={\frac {1}{r}}+1,}  [{\frac {1}{p}}+{\frac {1}{q}}={\frac
      {1}{r}}+1,]
then
           &#x2016;  f &#x2217; g  &#x2016;   r   &#x2264;   &#x2016; f
      &#x2016;   p     &#x2016; g &#x2016;   q   ,  f &#x2208;    L    p   ,
      &#xA0; g &#x2208;    L    q   ,   {\displaystyle \left\Vert
      f*g\right\Vert _{r}\leq \left\Vert f\right\Vert _{p}\left\Vert
      g\right\Vert _{q},\quad f\in {\mathcal {L}}^{p},\ g\in {\mathcal {L}}^
      {q},}  [{\displaystyle \left\Vert f*g\right\Vert _{r}\leq \left\Vert
      f\right\Vert _{p}\left\Vert g\right\Vert _{q},\quad f\in {\mathcal {L}}^
      {p},\ g\in {\mathcal {L}}^{q},}]
so that the convolution is a continuous bilinear mapping from LpÃLq to Lr. The
Young inequality for convolution is also true in other contexts (circle group,
convolution on Z). The preceding inequality is not sharp on the real line: when
1 < p, q, r < â, there exists a constant Bp,q < 1 such that:
           &#x2016;  f &#x2217; g  &#x2016;   r   &#x2264;  B  p , q
      &#x2016; f &#x2016;   p     &#x2016; g &#x2016;   q   ,  f &#x2208;    L
      p   , &#xA0; g &#x2208;    L    q   .   {\displaystyle \left\Vert
      f*g\right\Vert _{r}\leq B_{p,q}\left\Vert f\right\Vert _{p}\left\Vert
      g\right\Vert _{q},\quad f\in {\mathcal {L}}^{p},\ g\in {\mathcal {L}}^
      {q}.}  [{\displaystyle \left\Vert f*g\right\Vert _{r}\leq B_
      {p,q}\left\Vert f\right\Vert _{p}\left\Vert g\right\Vert _{q},\quad f\in
      {\mathcal {L}}^{p},\ g\in {\mathcal {L}}^{q}.}]
The optimal value of Bp,q was discovered in 1975.[15]
A stronger estimate is true provided  1 < p, q, r < â :
         &#x2016; f &#x2217; g  &#x2016;  r   &#x2264;  C  p , q   &#x2016; f
      &#x2016;  p   &#x2016; g  &#x2016;  q , w     {\displaystyle \|f*g\|_
      {r}\leq C_{p,q}\|f\|_{p}\|g\|_{q,w}}  [{\displaystyle \|f*g\|_{r}\leq C_
      {p,q}\|f\|_{p}\|g\|_{q,w}}]
where     &#x2016; g  &#x2016;  q , w     {\displaystyle \|g\|_{q,w}}  [\|g\|_
{q,w}] is the weak_Lq norm. Convolution also defines a bilinear continuous map
L  p , w   &#x00D7;  L  q , w   &#x2192;  L  r , w     {\displaystyle L^
{p,w}\times L^{q,w}\to L^{r,w}}  [{\displaystyle L^{p,w}\times L^{q,w}\to L^
{r,w}}] for     1 < p , q , r < &#x221E;   {\displaystyle 1<p,q,r<\infty }
[1<p,q,r<\infty ], owing to the weak Young inequality:[16]
         &#x2016; f &#x2217; g  &#x2016;  r , w   &#x2264;  C  p , q   &#x2016;
      f  &#x2016;  p , w   &#x2016; g  &#x2016;  r , w   .   {\displaystyle
      \|f*g\|_{r,w}\leq C_{p,q}\|f\|_{p,w}\|g\|_{r,w}.}  [{\displaystyle
      \|f*g\|_{r,w}\leq C_{p,q}\|f\|_{p,w}\|g\|_{r,w}.}]
**** Functions of rapid decay[edit] ****
In addition to compactly supported functions and integrable functions,
functions that have sufficiently rapid decay at infinity can also be convolved.
An important feature of the convolution is that if f and g both decay rapidly,
then fâg also decays rapidly. In particular, if f and g are rapidly
decreasing_functions, then so is the convolution fâg. Combined with the fact
that convolution commutes with differentiation (see #Properties), it follows
that the class of Schwartz_functions is closed under convolution (Stein_&_Weiss
1971, Theorem 3.3).
**** Distributions[edit] ****
Main article: Distribution_(mathematics)
Under some circumstances, it is possible to define the convolution of a
function with a distribution, or of two distributions. If f is a compactly
supported function and g is a distribution, then fâg is a smooth function
defined by a distributional formula analogous to
          &#x222B;    R   d      f  ( y ) g ( x &#x2212; y )  d y .
      {\displaystyle \int _{\mathbf {R} ^{d}}{f}(y)g(x-y)\,dy.}  [\int _
      {\mathbf {R} ^{d}}{f}(y)g(x-y)\,dy.]
More generally, it is possible to extend the definition of the convolution in a
unique way so that the associative law
         f &#x2217; ( g &#x2217; &#x03C6; ) = ( f &#x2217; g ) &#x2217;
      &#x03C6;   {\displaystyle f*(g*\varphi )=(f*g)*\varphi }  [{\displaystyle
      f*(g*\varphi )=(f*g)*\varphi }]
remains valid in the case where f is a distribution, and g a compactly
supported distribution (HÃ¶rmander_1983, Â§4.2).
**** Measures[edit] ****
The convolution of any two Borel_measures Î¼ and Î½ of bounded_variation is the
measure Î» defined by (Rudin_1962)
          &#x222B;    R   d     f ( x )  d &#x03BB; ( x ) =  &#x222B;    R   d
      &#x222B;    R   d     f ( x + y )  d &#x03BC; ( x )  d &#x03BD; ( y ) .
      {\displaystyle \int _{\mathbf {R} ^{d}}f(x)\,d\lambda (x)=\int _{\mathbf
      {R} ^{d}}\int _{\mathbf {R} ^{d}}f(x+y)\,d\mu (x)\,d\nu (y).}  [
      {\displaystyle \int _{\mathbf {R} ^{d}}f(x)\,d\lambda (x)=\int _{\mathbf
      {R} ^{d}}\int _{\mathbf {R} ^{d}}f(x+y)\,d\mu (x)\,d\nu (y).}]
This agrees with the convolution defined above when Î¼ and Î½ are regarded as
distributions, as well as the convolution of L1 functions when Î¼ and Î½ are
absolutely continuous with respect to the Lebesgue measure.
The convolution of measures also satisfies the following version of Young's
inequality
         &#x2016; &#x03BC; &#x2217; &#x03BD; &#x2016; &#x2264; &#x2016;
      &#x03BC; &#x2016; &#x2016; &#x03BD; &#x2016;   {\displaystyle \|\mu *\nu
      \|\leq \|\mu \|\|\nu \|}  [{\displaystyle \|\mu *\nu \|\leq \|\mu \|\|\nu
      \|}]
where the norm is the total_variation of a measure. Because the space of
measures of bounded variation is a Banach_space, convolution of measures can be
treated with standard methods of functional_analysis that may not apply for the
convolution of distributions.
***** Properties[edit] *****
**** Algebraic properties[edit] ****
See also: Convolution_algebra
The convolution defines a product on the linear_space of integrable functions.
This product satisfies the following algebraic properties, which formally mean
that the space of integrable functions with the product given by convolution is
a commutative associative_algebra without identity (Strichartz_1994, Â§3.3).
Other linear spaces of functions, such as the space of continuous functions of
compact support, are closed under the convolution, and so also form commutative
associative algebras.
  Commutativity
         f &#x2217; g = g &#x2217; f   {\displaystyle f*g=g*f}  [{\displaystyle
      f*g=g*f}]
Proof: By definition
         ( f &#x2217; g ) ( t ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;   f
      ( &#x03C4; ) g ( t &#x2212; &#x03C4; )  d &#x03C4;   {\displaystyle (f*g)
      (t)=\int _{-\infty }^{\infty }f(\tau )g(t-\tau )\,d\tau }  [
      {\displaystyle (f*g)(t)=\int _{-\infty }^{\infty }f(\tau )g(t-\tau
      )\,d\tau }]
Changing the variable of integration to     u = t &#x2212; &#x03C4;
{\displaystyle u=t-\tau }  [{\displaystyle u=t-\tau }] the result follows.
  Associativity
         f &#x2217; ( g &#x2217; h ) = ( f &#x2217; g ) &#x2217; h
      {\displaystyle f*(g*h)=(f*g)*h}  [{\displaystyle f*(g*h)=(f*g)*h}]
Proof: This follows from using Fubini's_theorem (i.e., double integrals can be
evaluated as iterated integrals in either order).
  Distributivity
         f &#x2217; ( g + h ) = ( f &#x2217; g ) + ( f &#x2217; h )
      {\displaystyle f*(g+h)=(f*g)+(f*h)}  [{\displaystyle f*(g+h)=(f*g)+
      (f*h)}]
Proof: This follows from linearity of the integral.
  Associativity with scalar multiplication
         a ( f &#x2217; g ) = ( a f ) &#x2217; g   {\displaystyle a(f*g)=
      (af)*g}  [{\displaystyle a(f*g)=(af)*g}]
for any real (or complex) number     a   {\displaystyle a}  [a].
  Multiplicative_identity
No algebra of functions possesses an identity for the convolution. The lack of
identity is typically not a major inconvenience, since most collections of
functions on which the convolution is performed can be convolved with a delta
distribution or, at the very least (as is the case of L1) admit approximations
to_the_identity. The linear space of compactly supported distributions does,
however, admit an identity under the convolution. Specifically,
         f &#x2217; &#x03B4; = f   {\displaystyle f*\delta =f}  [{\displaystyle
      f*\delta =f}]
where Î´ is the delta distribution.
  Inverse element
Some distributions have an inverse_element for the convolution, S(−1), which is
defined by
          S  ( &#x2212; 1 )   &#x2217; S = &#x03B4; .   {\displaystyle S^{(-
      1)}*S=\delta .}  [{\displaystyle S^{(-1)}*S=\delta .}]
The set of invertible distributions forms an abelian_group under the
convolution.
  Complex conjugation
            f &#x2217; g  &#x00AF;   =   f &#x00AF;   &#x2217;   g &#x00AF;
      {\displaystyle {\overline {f*g}}={\overline {f}}*{\overline {g}}}  [
      {\displaystyle {\overline {f*g}}={\overline {f}}*{\overline {g}}}]
  Relationship with differentiation
         ( f &#x2217; g  ) &#x2032;  =  f &#x2032;  &#x2217; g = f &#x2217;  g
      &#x2032;    {\displaystyle (f*g)'=f'*g=f*g'}  [{\displaystyle
      (f*g)'=f'*g=f*g'}]
Proof:
             ( f &#x2217; g  ) &#x2032;     =   d  d t     &#x222B;  &#x2212;
      &#x221E;   &#x221E;   f ( &#x03C4; ) g ( t &#x2212; &#x03C4; )  d
      &#x03C4;       =  &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( &#x03C4; )
      &#x2202;  &#x2202; t    g ( t &#x2212; &#x03C4; )  d &#x03C4;       =
      &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( &#x03C4; )  g &#x2032;  ( t
      &#x2212; &#x03C4; )  d &#x03C4; = f &#x2217;  g &#x2032;  .
      {\displaystyle {\begin{aligned}(f*g)'&={\frac {d}{dt}}\int _{-\infty }^
      {\infty }f(\tau )g(t-\tau )\,d\tau \\[4pt]&=\int _{-\infty }^{\infty }f
      (\tau ){\frac {\partial }{\partial t}}g(t-\tau )\,d\tau \\[4pt]&=\int _{-
      \infty }^{\infty }f(\tau )g'(t-\tau )\,d\tau =f*g'.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}(f*g)'&={\frac {d}{dt}}\int _{-\infty }^
      {\infty }f(\tau )g(t-\tau )\,d\tau \\[4pt]&=\int _{-\infty }^{\infty }f
      (\tau ){\frac {\partial }{\partial t}}g(t-\tau )\,d\tau \\[4pt]&=\int _{-
      \infty }^{\infty }f(\tau )g'(t-\tau )\,d\tau =f*g'.\end{aligned}}}]
  Relationship with integration
      If     F ( t ) =  &#x222B;  &#x2212; &#x221E;   t   f ( &#x03C4; ) d
      &#x03C4; ,   {\displaystyle F(t)=\int _{-\infty }^{t}f(\tau )d\tau ,}  [
      {\displaystyle F(t)=\int _{-\infty }^{t}f(\tau )d\tau ,}] and     G ( t )
      =  &#x222B;  &#x2212; &#x221E;   t   g ( &#x03C4; )  d &#x03C4; ,
      {\displaystyle G(t)=\int _{-\infty }^{t}g(\tau )\,d\tau ,}  [
      {\displaystyle G(t)=\int _{-\infty }^{t}g(\tau )\,d\tau ,}] then
         ( F &#x2217; g ) ( t ) = ( f &#x2217; G ) ( t ) =  &#x222B;  &#x2212;
      &#x221E;   t   ( f &#x2217; g ) ( &#x03C4; )  d &#x03C4; .
      {\displaystyle (F*g)(t)=(f*G)(t)=\int _{-\infty }^{t}(f*g)(\tau )\,d\tau
      .}  [{\displaystyle (F*g)(t)=(f*G)(t)=\int _{-\infty }^{t}(f*g)(\tau
      )\,d\tau .}]
**** Integration[edit] ****
If f and g are integrable functions, then the integral of their convolution on
the whole space is simply obtained as the product of their integrals:
          &#x222B;    R   d     ( f &#x2217; g ) ( x )  d x =  (   &#x222B;
      R   d     f ( x )  d x  )   (   &#x222B;    R   d     g ( x )  d x  )  .
      {\displaystyle \int _{\mathbf {R} ^{d}}(f*g)(x)\,dx=\left(\int _{\mathbf
      {R} ^{d}}f(x)\,dx\right)\left(\int _{\mathbf {R} ^{d}}g(x)\,dx\right).}
      [{\displaystyle \int _{\mathbf {R} ^{d}}(f*g)(x)\,dx=\left(\int _{\mathbf
      {R} ^{d}}f(x)\,dx\right)\left(\int _{\mathbf {R} ^{d}}g(x)\,dx\right).}]
This follows from Fubini's_theorem. The same result holds if f and g are only
assumed to be nonnegative measurable functions, by Tonelli's_theorem.
**** Differentiation[edit] ****
In the one-variable case,
           d  d x    ( f &#x2217; g ) =    d f   d x    &#x2217; g = f &#x2217;
      d g   d x      {\displaystyle {\frac {d}{dx}}(f*g)={\frac {df}{dx}}*g=f*
      {\frac {dg}{dx}}}  [{\displaystyle {\frac {d}{dx}}(f*g)={\frac {df}
      {dx}}*g=f*{\frac {dg}{dx}}}]
where d/dx is the derivative. More generally, in the case of functions of
several variables, an analogous formula holds with the partial_derivative:
           &#x2202;  &#x2202;  x  i      ( f &#x2217; g ) =    &#x2202; f
      &#x2202;  x  i      &#x2217; g = f &#x2217;    &#x2202; g   &#x2202;  x
      i      .   {\displaystyle {\frac {\partial }{\partial x_{i}}}(f*g)={\frac
      {\partial f}{\partial x_{i}}}*g=f*{\frac {\partial g}{\partial x_{i}}}.}
      [{\frac {\partial }{\partial x_{i}}}(f*g)={\frac {\partial f}{\partial x_
      {i}}}*g=f*{\frac {\partial g}{\partial x_{i}}}.]
A particular consequence of this is that the convolution can be viewed as a
"smoothing" operation: the convolution of f and g is differentiable as many
times as f and g are in total.
These identities hold under the precise condition that f and g are absolutely
integrable and at least one of them has an absolutely integrable (L1) weak
derivative, as a consequence of Young's_convolution_inequality. For instance,
when f is continuously differentiable with compact support, and g is an
arbitrary locally integrable function,
           d  d x    ( f &#x2217; g ) =    d f   d x    &#x2217; g .
      {\displaystyle {\frac {d}{dx}}(f*g)={\frac {df}{dx}}*g.}  [{\displaystyle
      {\frac {d}{dx}}(f*g)={\frac {df}{dx}}*g.}]
These identities also hold much more broadly in the sense of tempered
distributions if one of f or g is a compactly supported distribution or a
Schwartz function and the other is a tempered distribution. On the other hand,
two positive integrable and infinitely differentiable functions may have a
nowhere continuous convolution.
In the discrete case, the difference_operator D f(n) = f(n + 1) − f(n)
satisfies an analogous relationship:
         D ( f &#x2217; g ) = ( D f ) &#x2217; g = f &#x2217; ( D g ) .
      {\displaystyle D(f*g)=(Df)*g=f*(Dg).}  [{\displaystyle D(f*g)=(Df)*g=f*
      (Dg).}]
**** Convolution theorem[edit] ****
The convolution_theorem states that
           F   { f &#x2217; g } = k &#x22C5;   F   { f } &#x22C5;   F   { g }
      {\displaystyle {\mathcal {F}}\{f*g\}=k\cdot {\mathcal {F}}\{f\}\cdot
      {\mathcal {F}}\{g\}}  [{\mathcal {F}}\{f*g\}=k\cdot {\mathcal {F}}\
      {f\}\cdot {\mathcal {F}}\{g\}]
where       F   { f }   {\displaystyle {\mathcal {F}}\{f\}}  [{\displaystyle
{\mathcal {F}}\{f\}}] denotes the Fourier_transform of     f   {\displaystyle
f}  [f], and     k   {\displaystyle k}  [k] is a constant that depends on the
specific normalization of the Fourier transform. Versions of this theorem also
hold for the Laplace_transform, two-sided_Laplace_transform, Z-transform and
Mellin_transform.
See also the less trivial Titchmarsh_convolution_theorem.
**** Translational equivariance[edit] ****
The convolution commutes with translations, meaning that
          &#x03C4;  x   ( f &#x2217; g ) = (  &#x03C4;  x   f ) &#x2217; g =  f
      &#x2217; (  &#x03C4;  x   g )   {\displaystyle \tau _{x}(f*g)=(\tau _
      {x}f)*g={f}*(\tau _{x}g)}  [{\displaystyle \tau _{x}(f*g)=(\tau _{x}f)*g=
      {f}*(\tau _{x}g)}]
where Ïxf is the translation of the function f by x defined by
         (  &#x03C4;  x   f ) ( y ) = f ( y &#x2212; x ) .   {\displaystyle
      (\tau _{x}f)(y)=f(y-x).}  [{\displaystyle (\tau _{x}f)(y)=f(y-x).}]
If f is a Schwartz_function, then Ïxf is the convolution with a translated
Dirac delta function Ïxf = f â Ïx Î´. So translation invariance of the
convolution of Schwartz functions is a consequence of the associativity of
convolution.
Furthermore, under certain conditions, convolution is the most general
translation invariant operation. Informally speaking, the following holds
    * Suppose that S is a bounded linear_operator acting on functions which
      commutes with translations: S(Ïxf) = Ïx(Sf) for all x. Then S is given
      as convolution with a function (or distribution) gS; that is Sf = gS â
      f.
Thus some translation invariant operations can be represented as convolution.
Convolutions play an important role in the study of time-invariant_systems, and
especially LTI_system_theory. The representing function gS is the impulse
response of the transformation S.
A more precise version of the theorem quoted above requires specifying the
class of functions on which the convolution is defined, and also requires
assuming in addition that S must be a continuous_linear_operator with respect
to the appropriate topology. It is known, for instance, that every continuous
translation invariant continuous linear operator on L1 is the convolution with
a finite Borel_measure. More generally, every continuous translation invariant
continuous linear operator on Lp for 1 â¤ p < â is the convolution with a
tempered_distribution whose Fourier_transform is bounded. To wit, they are all
given by bounded Fourier_multipliers.
***** Convolutions on groups[edit] *****
If G is a suitable group endowed with a measure Î», and if f and g are real or
complex valued integrable functions on G, then we can define their convolution
by
         ( f &#x2217; g ) ( x ) =  &#x222B;  G   f ( y ) g (  y  &#x2212; 1   x
      )  d &#x03BB; ( y ) .   {\displaystyle (f*g)(x)=\int _{G}f(y)g(y^{-
      1}x)\,d\lambda (y).}  [{\displaystyle (f*g)(x)=\int _{G}f(y)g(y^{-
      1}x)\,d\lambda (y).}]
It is not commutative in general. In typical cases of interest G is a locally
compact Hausdorff topological_group and Î» is a (left-) Haar_measure. In that
case, unless G is unimodular, the convolution defined in this way is not the
same as       &#x222B; f ( x  y  &#x2212; 1   ) g ( y )  d &#x03BB; ( y )
{\displaystyle \textstyle {\int f(xy^{-1})g(y)\,d\lambda (y)}}  [\textstyle
{\int f(xy^{-1})g(y)\,d\lambda (y)}]. The preference of one over the other is
made so that convolution with a fixed function g commutes with left translation
in the group:
          L  h   ( f &#x2217; g ) = (  L  h   f ) &#x2217; g .   {\displaystyle
      L_{h}(f*g)=(L_{h}f)*g.}  [{\displaystyle L_{h}(f*g)=(L_{h}f)*g.}]
Furthermore, the convention is also required for consistency with the
definition of the convolution of measures given below. However, with a right
instead of a left Haar measure, the latter integral is preferred over the
former.
On locally compact abelian_groups, a version of the convolution_theorem holds:
the Fourier transform of a convolution is the pointwise product of the Fourier
transforms. The circle_group T with the Lebesgue measure is an immediate
example. For a fixed g in L1(T), we have the following familiar operator acting
on the Hilbert_space L2(T):
         T  f  ( x ) =   1  2 &#x03C0;     &#x222B;   T     f  ( y ) g ( x
      &#x2212; y )  d y .   {\displaystyle T{f}(x)={\frac {1}{2\pi }}\int _
      {\mathbf {T} }{f}(y)g(x-y)\,dy.}  [{\displaystyle T{f}(x)={\frac {1}{2\pi
      }}\int _{\mathbf {T} }{f}(y)g(x-y)\,dy.}]
The operator T is compact. A direct calculation shows that its adjoint T* is
convolution with
            g &#x00AF;    ( &#x2212; y ) .   {\displaystyle {\bar {g}}(-y).}  [
      {\displaystyle {\bar {g}}(-y).}]
By the commutativity property cited above, T is normal: T* T = TT* . Also, T
commutes with the translation operators. Consider the family S of operators
consisting of all such convolutions and the translation operators. Then S is a
commuting family of normal operators. According to spectral_theory, there
exists an orthonormal basis {hk} that simultaneously diagonalizes S. This
characterizes convolutions on the circle. Specifically, we have
          h  k   ( x ) =  e  i k x   ,  k &#x2208;  Z  ,    {\displaystyle h_
      {k}(x)=e^{ikx},\quad k\in \mathbb {Z} ,\;}  [h_{k}(x)=e^{ikx},\quad k\in
      \mathbb {Z} ,\;]
which are precisely the characters of T. Each convolution is a compact
multiplication_operator in this basis. This can be viewed as a version of the
convolution theorem discussed above.
A discrete example is a finite cyclic_group of order n. Convolution operators
are here represented by circulant_matrices, and can be diagonalized by the
discrete_Fourier_transform.
A similar result holds for compact groups (not necessarily abelian): the matrix
coefficients of finite-dimensional unitary_representations form an orthonormal
basis in L2 by the PeterâWeyl_theorem, and an analog of the convolution
theorem continues to hold, along with many other aspects of harmonic_analysis
that depend on the Fourier transform.
***** Convolution of measures[edit] *****
Let G be a (multiplicatively written) topological group. If Î¼ and Î½ are
finite Borel_measures on G, then their convolution Î¼âÎ½ is defined as the
pushforward_measure of the group_action and can be written as
         ( &#x03BC; &#x2217; &#x03BD; ) ( E ) = &#x222C;  1  E   ( x y )  d
      &#x03BC; ( x )  d &#x03BD; ( y )   {\displaystyle (\mu *\nu )(E)=\iint 1_
      {E}(xy)\,d\mu (x)\,d\nu (y)}  [{\displaystyle (\mu *\nu )(E)=\iint 1_{E}
      (xy)\,d\mu (x)\,d\nu (y)}]
for each measurable subset E of G. The convolution is also a finite measure,
whose total_variation satisfies
         &#x2016; &#x03BC; &#x2217; &#x03BD; &#x2016; &#x2264; &#x2016;
      &#x03BC; &#x2016; &#x2016; &#x03BD; &#x2016; .   {\displaystyle \|\mu
      *\nu \|\leq \|\mu \|\|\nu \|.}  [{\displaystyle \|\mu *\nu \|\leq \|\mu
      \|\|\nu \|.}]
In the case when G is locally_compact with (left-)Haar_measure Î», and Î¼ and
Î½ are absolutely_continuous with respect to a Î», so_that_each_has_a_density
function, then the convolution Î¼âÎ½ is also absolutely continuous, and its
density function is just the convolution of the two separate density functions.
If Î¼ and Î½ are probability_measures on the topological group (R,+), then the
convolution Î¼âÎ½ is the probability_distribution of the sum X + Y of two
independent random_variables X and Y whose respective distributions are Î¼ and
Î½.
***** Bialgebras[edit] *****
Let (X, Î, â, Îµ, Î·) be a bialgebra with comultiplication Î,
multiplication â, unit Î·, and counit Îµ. The convolution is a product
defined on the endomorphism_algebra End(X) as follows. Let Ï, Ï â End(X),
that is, Ï,Ï : X â X are functions that respect all algebraic structure of
X, then the convolution ÏâÏ is defined as the composition
         X   &#x2192;  &#x0394;    X &#x2297; X   &#x2192;  &#x03D5; &#x2297;
      &#x03C8;    X &#x2297; X   &#x2192;  &#x2207;    X .   {\displaystyle X
      {\xrightarrow {\Delta }}X\otimes X{\xrightarrow {\phi \otimes \psi
      }}X\otimes X{\xrightarrow {\nabla }}X.}  [{\displaystyle X{\xrightarrow
      {\Delta }}X\otimes X{\xrightarrow {\phi \otimes \psi }}X\otimes X
      {\xrightarrow {\nabla }}X.}]
The convolution appears notably in the definition of Hopf_algebras (Kassel
1995, Â§III.3). A bialgebra is a Hopf algebra if and only if it has an
antipode: an endomorphism S such that
         S &#x2217;  id  X   =  id  X   &#x2217; S = &#x03B7; &#x2218; &#x03B5;
      .   {\displaystyle S*\operatorname {id} _{X}=\operatorname {id} _
      {X}*S=\eta \circ \varepsilon .}  [S*\operatorname {id} _{X}=\operatorname
      {id} _{X}*S=\eta \circ \varepsilon .]
***** Applications[edit] *****
Gaussian_blur can be used to obtain a smooth grayscale digital image of a
halftone print.
Convolution and related operations are found in many applications in science,
engineering and mathematics.
    * In image_processing
            In digital_image_processing convolutional filtering plays an
            important role in many important algorithms in edge_detection and
            related processes.
            In optics, an out-of-focus photograph is a convolution of the sharp
            image with a lens function. The photographic term for this is
            bokeh.
            In image processing applications such as adding blurring.
    * In digital data processing
            In analytical_chemistry, SavitzkyâGolay_smoothing_filters are
            used for the analysis of spectroscopic data. They can improve
            signal-to-noise_ratio with minimal distortion of the spectra
            In statistics, a weighted moving_average is a convolution.
    * In acoustics, reverberation is the convolution of the original sound with
      echoes from objects surrounding the sound source.
            In digital signal processing, convolution is used to map the
            impulse_response of a real room on a digital audio signal.
            In electronic_music convolution is the imposition of a spectral or
            rhythmic structure on a sound. Often this envelope or structure is
            taken from another sound. The convolution of two signals is the
            filtering of one through the other.[17]
    * In electrical_engineering, the convolution of one function (the input
      signal) with a second function (the impulse response) gives the output of
      a linear_time-invariant_system (LTI). At any given moment, the output is
      an accumulated effect of all the prior values of the input function, with
      the most recent values typically having the most influence (expressed as
      a multiplicative factor). The impulse response function provides that
      factor as a function of the elapsed time since each input value occurred.
    * In physics, wherever there is a linear_system with a "superposition
      principle", a convolution operation makes an appearance. For instance, in
      spectroscopy line broadening due to the Doppler effect on its own gives a
      Gaussian spectral_line_shape and collision broadening alone gives a
      Lorentzian line shape. When both effects are operative, the line shape is
      a convolution of Gaussian and Lorentzian, a Voigt_function.
            In time-resolved_fluorescence_spectroscopy, the excitation signal
            can be treated as a chain of delta pulses, and the measured
            fluorescence is a sum of exponential decays from each delta pulse.
            In computational_fluid_dynamics, the large_eddy_simulation (LES)
            turbulence_model uses the convolution operation to lower the range
            of length scales necessary in computation thereby reducing
            computational cost.
    * In probability_theory, the probability_distribution of the sum of two
      independent random_variables is the convolution of their individual
      distributions.
            In kernel_density_estimation, a distribution is estimated from
            sample points by convolution with a kernel, such as an isotropic
            Gaussian. (Diggle_1995).
    * In radiotherapy treatment planning systems, most part of all modern codes
      of calculation applies a convolution-superposition_algorithm.
      [clarification_needed]
    * Convolutional_neural_networks apply multiple cascaded convolution kernels
      with applications in machine_vision and artificial_intelligence
    * In structural reliability, the reliability index can be defined based on
      the convolution theorem.
            The definition of reliability index for limit state functions with
            nonnormal distributions can be established corresponding to the
            joint_distribution_function. In fact, the joint distribution
            function can be obtained using the convolution theory. (Ghasemi-
            Nowak_2017).
***** See also[edit] *****
    * Analog_signal_processing
    * Circulant_matrix
    * Convolution_for_optical_broad-beam_responses_in_scattering_media
    * Convolution_power
    * Dirichlet_convolution
    * Generalized_signal_averaging
    * Jan_Mikusinski
    * List_of_convolutions_of_probability_distributions
    * LTI_system_theory#Impulse_response_and_convolution
    * Multidimensional_discrete_convolution
    * Scaled_correlation
    * Titchmarsh_convolution_theorem
    * Toeplitz_matrix (convolutions can be considered a Toeplitz matrix
      operation where each row is a shifted copy of the convolution kernel)
***** Notes[edit] *****
   1. ^ Reasons for the reflection include:
          o It is necessary to implement the equivalent of the pointwise
            product of the Fourier transforms of f and g.
          o When the convolution is viewed as a moving_weighted_average, the
            weighting function, g(âx), is often specified in terms of another
            function, g(x), called the impulse_response of a linear_time-
            invariant_system.
***** References[edit] *****
   1. ^ Smith, Stephen W (1997). "13.Convolution". The Scientist and Engineer's
      Guide to Digital Signal Processing (1 ed.). California Technical
      Publishing. ISBN 0966017633. Retrieved 22 April 2016.
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
   3. ^Irwin, J. David (1997). "4.3". The Industrial Electronics Handbook (1
      ed.). Boca Raton, FL: CRC Press. p. 75. ISBN 0849383439.
   4. ^ Dominguez-Torres, p 2
   5. ^ Dominguez-Torres, p 4
   6. ^ R. N. Bracewell (2005), "Early_work_on_imaging_theory_in_radio
      astronomy", in W. T. Sullivan (ed.), The Early Years of Radio Astronomy:
      Reflections Fifty Years After Jansky's Discovery, Cambridge University
      Press, p. 172, ISBN 978-0-521-61602-7
   7. ^ John Hilton Grace and Alfred Young (1903), The_algebra_of_invariants,
      Cambridge University Press, p. 40
   8. ^ Leonard Eugene Dickson (1914), Algebraic_invariants, J. Wiley, p. 85
   9. ^  According to [Lothar von Wolfersdorf (2000), "Einige Klassen
      quadratischer Integralgleichungen", Sitzungsberichte der SÃ¤chsischen
      Akademie der Wissenschaften zu Leipzig, Mathematisch-
      naturwissenschaftliche Klasse, volume 128, number 2, 6â7], the source
      is Volterra, Vito (1913), "LeÃ§ons sur les fonctions de linges".
      Gauthier-Villars, Paris 1913.
  10. ^ Damelin_&_Miller_2011, p. 232
  11. ^Press, William H.; Flannery, Brian P.; Teukolsky, Saul A.; Vetterling,
      William T. (1989). Numerical Recipes in Pascal. Cambridge University
      Press. p. 450. ISBN 0-521-37516-9.
  12. ^Rader, C.M. (December 1972). "Discrete Convolutions via Mersenne
      Transforms". IEEE Transactions on Computers. 21 (12): 1269â1273. doi:
      10.1109/T-C.1972.223497.
  13. ^Madisetti, Vijay K. (1999). "Fast_Convolution_and_Filtering"_in_the
      "Digital_Signal_Processing_Handbook" (PDF). CRC Press LLC. p. Section 8.
      ISBN 9781420045635.
  14. ^Juang, B.H. "Lecture_21:_Block_Convolution" (PDF). EECS at the Georgia
      Institute of Technology. Retrieved 17 May 2013.
  15. ^Gardner, William G. (November 1994). "Efficient_Convolution_without
      Input/Output_Delay" (PDF). Audio Engineering Society Convention 97. Paper
      3897. Retrieved 17 May 2013.
  16. ^  Beckner,_William (1975), "Inequalities in Fourier analysis", Ann. of
      Math. (2) 102: 159–182. Independently, Brascamp, Herm J. and Lieb,
      Elliott_H. (1976), "Best constants in Young's inequality, its converse,
      and its generalization to more than three functions", Advances in Math.
      20: 151–173. See BrascampâLieb_inequality
  17. ^ Reed_&_Simon_1975, IX.4
  18. ^ ZÃ¶lzer, Udo, ed. (2002). DAFX:Digital Audio Effects, p.48â49.
  19. ISBN 0471490784.
***** Further reading[edit] *****
    * Bracewell, R. (1986), The Fourier Transform and Its Applications (2nd
      ed.), McGrawâHill, ISBN 0-07-116043-4
.
Damelin, S.; Miller, W. (2011), The Mathematics of Signal Processing, Cambridge
University Press, ISBN 978-1107601048
Diggle, P. J. (1985), "A kernel method for smoothing point process data",
Journal of the Royal Statistical Society, Series C, 34 (2): 138â147, doi:
10.2307/2347366, JSTOR 2347366
Dominguez-Torres, Alejandro (Nov 2, 2010). "Origin and history of convolution".
41 pgs. http://www.slideshare.net/Alexdfar/origin-adn-history-of-convolution.
Cranfield, Bedford MK43 OAL, UK. Retrieved Mar 13, 2013.
Diggle, P. J. (1985), "A kernel method for smoothing point process data",
Journal of the Royal Statistical Society, Series C, 34 (2): 138â147, doi:
10.2307/2347366, JSTOR 2347366
Ghasemi, S. Hooman; Nowak, Andrzej S. (2017), "Reliability Index for Non-normal
Distributions of Limit State Functions", Structural Engineering and Mechanics,
62 (3): 365â372, doi:10.12989/sem.2017.62.3.365
Grinshpan, A. Z. (2017), "An inequality for multiple convolutions with respect
to Dirichlet probability measure", Advances in Applied Mathematics, 82 (1):
102â119, doi:10.1016/j.aam.2016.08.001
Hewitt, Edwin; Ross, Kenneth A. (1979), Abstract harmonic analysis. Vol. I,
Grundlehren der Mathematischen Wissenschaften [Fundamental Principles of
Mathematical Sciences], 115 (2nd ed.), Berlin, New York: Springer-Verlag,
ISBN 978-3-540-09434-0, MR 0551496
.
Hewitt, Edwin; Ross, Kenneth A. (1970), Abstract harmonic analysis. Vol. II:
Structure and analysis for compact groups. Analysis on locally compact Abelian
groups, Die Grundlehren der mathematischen Wissenschaften, Band 152, Berlin,
New York: Springer-Verlag, MR 0262773
.
HÃ¶rmander,_L. (1983), The analysis of linear partial differential operators I,
Grundl. Math. Wissenschaft., 256, Springer, doi:10.1007/978-3-642-96750-4,
ISBN 3-540-12104-8, MR 0717035
.
Kassel, Christian (1995), Quantum groups, Graduate Texts in Mathematics, 155,
Berlin, New York: Springer-Verlag, doi:10.1007/978-1-4612-0783-2, ISBN 978-0-
387-94370-1, MR 1321145
.
Knuth,_Donald (1997), Seminumerical Algorithms (3rd. ed.), Reading,
Massachusetts: AddisonâWesley, ISBN 0-201-89684-2
.
Reed, Michael; Simon,_Barry (1975), Methods of modern mathematical physics. II.
Fourier analysis, self-adjointness, New York-London: Academic Press Harcourt
Brace Jovanovich, Publishers, pp. xv+361, ISBN 0-12-585002-6, MR 0493420
Rudin,_Walter (1962), Fourier analysis on groups, Interscience Tracts in Pure
and Applied Mathematics, 12, New YorkâLondon: Interscience Publishers,
ISBN 0-471-52364-X, MR 0152834
.
Sobolev, V.I. (2001) [1994], "Convolution_of_functions", in Hazewinkel,_Michiel
(ed.), Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
Kluwer Academic Publishers, ISBN 978-1-55608-010-4
.
Stein,_Elias; Weiss, Guido (1971), Introduction to Fourier Analysis on
Euclidean Spaces, Princeton University Press, ISBN 0-691-08078-X
.
Strichartz, R. (1994), A Guide to Distribution Theory and Fourier Transforms,
CRC Press, ISBN 0-8493-8273-4
.
Titchmarsh,_E (1948), Introduction to the theory of Fourier integrals (2nd
ed.), New York, N.Y.: Chelsea Pub. Co. (published 1986), ISBN 978-0-8284-0324-5
.
Uludag,_A._M. (1998), "On possible deterioration of smoothness under the
operation of convolution", J. Math. Anal. Appl., 227 (2): 335â358, doi:
10.1006/jmaa.1998.6091
Treves, FranÃ§ois (1967), Topological Vector Spaces, Distributions and Kernels,
Academic Press, ISBN 0-486-45352-9
.
von zur Gathen, J.; Gerhard, J. (2003), Modern Computer Algebra, Cambridge
University Press, ISBN 0-521-82646-2
.
***** External links[edit] *****
 Look up convolution in Wiktionary, the free dictionary.
 Wikimedia Commons has media related to Convolution.
    * Earliest_Uses:_The_entry_on_Convolution_has_some_historical_information.
    * Convolution, on The_Data_Analysis_BriefBook
    * http://www.jhu.edu/~signals/convolve/index.html Visual convolution Java
      Applet
    * http://www.jhu.edu/~signals/discreteconv2/index.html Visual convolution
      Java Applet for discrete-time functions
    * Lectures_on_Image_Processing:_A_collection_of_18_lectures_in_pdf_format
      from_Vanderbilt_University._Lecture_7_is_on_2-D_convolution., by Alan
      Peters
    * * https://archive.org/details/Lectures_on_Image_Processing
    * Convolution_Kernel_Mask_Operation_Interactive_tutorial
    * Convolution at MathWorld
    * Freeverb3_Impulse_Response_Processor: Opensource zero latency impulse
      response processor with VST plugins
    * Stanford University CS 178 interactive_Flash_demo showing how spatial
      convolution works.
    * A_video_lecture_on_the_subject_of_convolution given by Salman_Khan
    * Example_of_FFT_convolution_for_pattern-recognition_(image_processing)

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Convolution&oldid=909221093"
Categories:
    * Functional_analysis
    * Image_processing
    * Binary_operations
    * Fourier_analysis
    * Bilinear_operators
    * Feature_detection_(computer_vision)
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_October_2017
    * Wikipedia_articles_needing_clarification_from_May_2013
    * Commons_category_link_is_on_Wikidata
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ø³ÙÚÙ
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 3 August 2019, at 23:46 (UTC).
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
