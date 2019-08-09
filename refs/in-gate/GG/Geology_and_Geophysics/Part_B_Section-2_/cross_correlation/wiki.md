The following text has been accessed from https://en.wikipedia.org/wiki/Cross-correlation at Thu Aug 8 23:25:18 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Cross-correlation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Part of a series on Statistics
Correlation and covariance
[CorrelationIcon.svg]
Correlation and covariance of random vectors
    * Autocorrelation_matrix
    * Cross-correlation_matrix
    * Auto-covariance_matrix
    * Cross-covariance_matrix
Correlation and covariance of stochastic processes
    * Autocorrelation_function
    * Cross-correlation_function
    * Autocovariance_function
    * Cross-covariance_function
Correlation and covariance of deterministic signals
    * Autocorrelation_function
    * Cross-correlation_function
    * Autocovariance function
    * Cross-covariance function
    * v
    * t
    * e
Visual comparison of convolution, cross-correlation and autocorrelation. For
the operations involving function f, and assuming the height of f is 1.0, the
value of the result at 5 different points is indicated by the shaded area below
each point. Also, the vertical symmetry of f is the reason     f &#x2217; g
{\displaystyle f*g}  [f*g] and     f &#x22C6; g   {\displaystyle f\star g}
[f\star g] are identical in this example.
In signal_processing, cross-correlation is a measure_of_similarity of two
series as a function of the displacement of one relative to the other. This is
also known as a sliding dot_product or sliding inner-product. It is commonly
used for searching a long signal for a shorter, known feature. It has
applications in pattern_recognition, single_particle_analysis, electron
tomography, averaging, cryptanalysis, and neurophysiology. The cross-
correlation is similar in nature to the convolution of two functions. In an
autocorrelation, which is the cross-correlation of a signal with itself, there
will always be a peak at a lag of zero, and its size will be the signal energy.
In probability and statistics, the term cross-correlations refers to the
correlations between the entries of two random_vectors      X    {\displaystyle
\mathbf {X} }  [\mathbf {X} ] and      Y    {\displaystyle \mathbf {Y} }
[\mathbf {Y} ], while the correlations of a random vector      X
{\displaystyle \mathbf {X} }  [\mathbf {X} ] are the correlations between the
entries of      X    {\displaystyle \mathbf {X} }  [\mathbf {X} ] itself, those
forming the correlation_matrix of      X    {\displaystyle \mathbf {X} }
[\mathbf {X} ]. If each of      X    {\displaystyle \mathbf {X} }  [\mathbf {X}
] and      Y    {\displaystyle \mathbf {Y} }  [\mathbf {Y} ] is a scalar random
variable which is realized repeatedly in a time_series, then the correlations
of the various temporal instances of      X    {\displaystyle \mathbf {X} }
[\mathbf {X} ] are known as autocorrelations of      X    {\displaystyle
\mathbf {X} }  [\mathbf {X} ], and the cross-correlations of      X
{\displaystyle \mathbf {X} }  [\mathbf {X} ] with      Y    {\displaystyle
\mathbf {Y} }  [\mathbf {Y} ] across time are temporal cross-correlations. In
probability and statistics, the definition of correlation always includes a
standardising factor in such a way that correlations have values between â1
and +1.
If     X   {\displaystyle X}  [X] and     Y   {\displaystyle Y}  [Y] are two
independent random_variables with probability_density_functions     f
{\displaystyle f}  [f] and     g   {\displaystyle g}  [g], respectively, then
the probability density of the difference     Y &#x2212; X   {\displaystyle Y-
X}  [Y-X] is formally given by the cross-correlation (in the signal-processing
sense)     f &#x22C6; g   {\displaystyle f\star g}  [f\star g]; however, this
terminology is not used in probability and statistics. In contrast, the
convolution     f &#x2217; g   {\displaystyle f*g}  [f*g] (equivalent to the
cross-correlation of     f ( t )   {\displaystyle f(t)}  [f(t)] and     g
( &#x2212; t )   {\displaystyle g(-t)}  [{\displaystyle g(-t)}]) gives the
probability density function of the sum     X + Y   {\displaystyle X+Y}  [X+Y].
⁰
***** Contents *****
    * 1_Cross-correlation_of_deterministic_signals
          o 1.1_Explanation
          o 1.2_Properties
          o 1.3_Definition_for_periodic_signals
    * 2_Cross-correlation_of_random_vectors
          o 2.1_Definition
          o 2.2_Example
          o 2.3_Definition_for_complex_random_vectors
    * 3_Cross-correlation_of_stochastic_processes
          o 3.1_Cross-correlation_function
          o 3.2_Cross-covariance_function
          o 3.3_Definition_for_wide-sense_stationary_stochastic_process
                # 3.3.1_Cross-correlation_function
                # 3.3.2_Cross-covariance_function
          o 3.4_Normalization
          o 3.5_Properties
                # 3.5.1_Symmetry_property
    * 4_Time_delay_analysis
    * 5_Terminology_in_image_processing
          o 5.1_Zero-normalized_cross-correlation_(ZNCC)
          o 5.2_Normalized_cross-correlation_(NCC)
    * 6_Nonlinear_systems
    * 7_See_also
    * 8_References
    * 9_Further_reading
    * 10_External_links
***** Cross-correlation of deterministic signals[edit] *****
For continuous functions     f   {\displaystyle f}  [f] and     g
{\displaystyle g}  [g], the cross-correlation is defined as:[1][2][3]
   ( f &#x22C6; g ) ( &#x03C4; ) &#xA0; &#x225C;  &#x222B;
&#x2212; &#x221E;   &#x221E;      f ( t )  &#x00AF;   g ( t +
&#x03C4; )  d t   {\displaystyle (f\star g)(\tau )\ \triangleq    (Eq.1)
\int _{-\infty }^{\infty }{\overline {f(t)}}g(t+\tau )\,dt}  [    
{\displaystyle (f\star g)(\tau )\ \triangleq \int _{-\infty }^
{\infty }{\overline {f(t)}}g(t+\tau )\,dt}]
which is equivalent to
         ( f &#x22C6; g ) ( &#x03C4; ) &#xA0; &#x225C;  &#x222B;  &#x2212;
      &#x221E;   &#x221E;      f ( t &#x2212; &#x03C4; )  &#x00AF;   g ( t )  d
      t   {\displaystyle (f\star g)(\tau )\ \triangleq \int _{-\infty }^{\infty
      }{\overline {f(t-\tau )}}g(t)\,dt}  [{\displaystyle (f\star g)(\tau )\
      \triangleq \int _{-\infty }^{\infty }{\overline {f(t-\tau )}}g(t)\,dt}]
where        f ( t )  &#x00AF;     {\displaystyle {\overline {f(t)}}}  [
{\displaystyle {\overline {f(t)}}}] denotes the complex_conjugate of     f ( t
)   {\displaystyle f(t)}  [f(t)], and     &#x03C4;   {\displaystyle \tau }
[\tau ] is the displacement, also known as lag (a feature in     f
{\displaystyle f}  [f] at     t   {\displaystyle t}  [t] occurs in     g
{\displaystyle g}  [g] at     t + &#x03C4;   {\displaystyle t+\tau }  [t+\tau
]).
Similarly, for discrete functions, the cross-correlation is defined as:[4][5]
   ( f &#x22C6; g ) [ n ] &#xA0; &#x225C;  &#x2211;  m = &#x2212;
&#x221E;   &#x221E;      f [ m ]  &#x00AF;   g [ m + n ]              
{\displaystyle (f\star g)[n]\ \triangleq \sum _{m=-\infty }^            (Eq.2)
{\infty }{\overline {f[m]}}g[m+n]}  [{\displaystyle (f\star g)[n]\
\triangleq \sum _{m=-\infty }^{\infty }{\overline {f[m]}}g[m+n]}]
which is equivalent to
         ( f &#x22C6; g ) [ n ] &#xA0; &#x225C;  &#x2211;  m = &#x2212;
      &#x221E;   &#x221E;      f [ m &#x2212; n ]  &#x00AF;   g [ m ]
      {\displaystyle (f\star g)[n]\ \triangleq \sum _{m=-\infty }^{\infty }
      {\overline {f[m-n]}}g[m]}  [{\displaystyle (f\star g)[n]\ \triangleq \sum
      _{m=-\infty }^{\infty }{\overline {f[m-n]}}g[m]}].
**** Explanation[edit] ****
As an example, consider two real valued functions     f   {\displaystyle f}
[f] and     g   {\displaystyle g}  [g] differing only by an unknown shift along
the x-axis. One can use the cross-correlation to find how much     g
{\displaystyle g}  [g] must be shifted along the x-axis to make it identical to
f   {\displaystyle f}  [f]. The formula essentially slides the     g
{\displaystyle g}  [g] function along the x-axis, calculating the integral of
their product at each position. When the functions match, the value of     ( f
&#x22C6; g )   {\displaystyle (f\star g)}  [(f\star g)] is maximized. This is
because when peaks (positive areas) are aligned, they make a large contribution
to the integral. Similarly, when troughs (negative areas) align, they also make
a positive contribution to the integral because the product of two negative
numbers is positive.
Animation displaying visually how cross correlation is calculated
With complex-valued_functions     f   {\displaystyle f}  [f] and     g
{\displaystyle g}  [g], taking the conjugate of     f   {\displaystyle f}  [f]
ensures that aligned peaks (or aligned troughs) with imaginary components will
contribute positively to the integral.
In econometrics, lagged cross-correlation is sometimes referred to as cross-
autocorrelation.[6]:p. 74
**** Properties[edit] ****
    * The cross-correlation of functions     f ( t )   {\displaystyle f(t)}  [f
      (t)] and     g ( t )   {\displaystyle g(t)}  [g(t)] is equivalent to the
      convolution (denoted by     &#x2217;   {\displaystyle *}  [*]) of
      f ( &#x2212; t )  &#x00AF;     {\displaystyle {\overline {f(-t)}}}  [
      {\displaystyle {\overline {f(-t)}}}] and     g ( t )   {\displaystyle g
      (t)}  [g(t)]. That is:
               [ f ( t ) &#x22C6; g ( t ) ] ( t ) = [    f ( &#x2212; t )
            &#x00AF;   &#x2217; g ( t ) ] ( t ) .   {\displaystyle [f(t)\star g
            (t)](t)=[{\overline {f(-t)}}*g(t)](t).}  [{\displaystyle [f(t)\star
            g(t)](t)=[{\overline {f(-t)}}*g(t)](t).}]
    *    [ f ( t ) &#x22C6; g ( t ) ] ( t ) = [    g ( t )  &#x00AF;   &#x22C6;
      f ( t )  &#x00AF;   ] ( &#x2212; t ) .   {\displaystyle [f(t)\star g(t)]
      (t)=[{\overline {g(t)}}\star {\overline {f(t)}}](-t).}  [{\displaystyle
      [f(t)\star g(t)](t)=[{\overline {g(t)}}\star {\overline {f(t)}}](-t).}]
    * If     f   {\displaystyle f}  [f] is a Hermitian_function, then     f
      &#x22C6; g = f &#x2217; g .   {\displaystyle f\star g=f*g.}  [
      {\displaystyle f\star g=f*g.}]
    * If both     f   {\displaystyle f}  [f] and     g   {\displaystyle g}  [g]
      are Hermitian, then     f &#x22C6; g = g &#x22C6; f   {\displaystyle
      f\star g=g\star f}  [f\star g=g\star f].
    *     (  f &#x22C6; g  )  &#x22C6;  (  f &#x22C6; g  )  =  (  f &#x22C6; f
      )  &#x22C6;  (  g &#x22C6; g  )    {\displaystyle \left(f\star
      g\right)\star \left(f\star g\right)=\left(f\star f\right)\star \left
      (g\star g\right)}  [{\displaystyle \left(f\star g\right)\star \left
      (f\star g\right)=\left(f\star f\right)\star \left(g\star g\right)}].
    * Analogous to the convolution_theorem, the cross-correlation satisfies
                 F    {  f &#x22C6; g  }  =      F    { f }   &#x00AF;
            &#x22C5;   F    { g }  ,   {\displaystyle {\mathcal {F}}\left\
            {f\star g\right\}={\overline {{\mathcal {F}}\left\{f\right\}}}\cdot
            {\mathcal {F}}\left\{g\right\},}  [{\displaystyle {\mathcal
            {F}}\left\{f\star g\right\}={\overline {{\mathcal {F}}\left\
            {f\right\}}}\cdot {\mathcal {F}}\left\{g\right\},}]
      where       F     {\displaystyle {\mathcal {F}}}  [{\mathcal {F}}]
      denotes the Fourier_transform, and an       f &#x00AF;     {\displaystyle
      {\overline {f}}}  [{\overline {f}}] again indicates the complex conjugate
      of     f   {\displaystyle f}  [f], since       F    {    f ( &#x2212; t )
      &#x00AF;   }  =      F    {  f ( t )  }   &#x00AF;     {\displaystyle
      {\mathcal {F}}\left\{{\overline {f(-t)}}\right\}={\overline {{\mathcal
      {F}}\left\{f(t)\right\}}}}  [{\displaystyle {\mathcal {F}}\left\{
      {\overline {f(-t)}}\right\}={\overline {{\mathcal {F}}\left\{f
      (t)\right\}}}}]. Coupled with fast_Fourier_transform algorithms, this
      property is often exploited for the efficient numerical computation of
      cross-correlations [7] (see circular_cross-correlation).
    * The cross-correlation is related to the spectral_density (see
      WienerâKhinchin_theorem).
    * The cross-correlation of a convolution of     f   {\displaystyle f}  [f]
      and     h   {\displaystyle h}  [h] with a function     g   {\displaystyle
      g}  [g] is the convolution of the cross-correlation of     g
      {\displaystyle g}  [g] and     f   {\displaystyle f}  [f] with the kernel
      h   {\displaystyle h}  [h]:
               g &#x22C6;  (  f &#x2217; h  )  =  (  g &#x22C6; f  )  &#x2217;
            h   {\displaystyle g\star \left(f*h\right)=\left(g\star f\right)*h}
            [{\displaystyle g\star \left(f*h\right)=\left(g\star f\right)*h}].
**** Definition for periodic signals[edit] ****
If     f   {\displaystyle f}  [f] and     g   {\displaystyle g}  [g] are both
continuous periodic functions of period     T   {\displaystyle T}  [T], the
integration from     &#x2212; &#x221E;   {\displaystyle -\infty }  [-\infty ]
to     &#x221E;   {\displaystyle \infty }  [\infty ] is replaced by integration
over any interval     [  t  0   ,  t  0   + T ]   {\displaystyle [t_{0},t_
{0}+T]}  [{\displaystyle [t_{0},t_{0}+T]}] of length     T   {\displaystyle T}
[T]:
         ( f &#x22C6; g ) ( &#x03C4; ) &#xA0; &#x225C;  &#x222B;   t  0      t
      0   + T      f ( t )  &#x00AF;   g ( t + &#x03C4; )  d t   {\displaystyle
      (f\star g)(\tau )\ \triangleq \int _{t_{0}}^{t_{0}+T}{\overline {f(t)}}g
      (t+\tau )\,dt}  [{\displaystyle (f\star g)(\tau )\ \triangleq \int _{t_
      {0}}^{t_{0}+T}{\overline {f(t)}}g(t+\tau )\,dt}]
which is equivalent to
         ( f &#x22C6; g ) ( &#x03C4; ) &#xA0; &#x225C;  &#x222B;   t  0      t
      0   + T      f ( t &#x2212; &#x03C4; )  &#x00AF;   g ( t )  d t
      {\displaystyle (f\star g)(\tau )\ \triangleq \int _{t_{0}}^{t_{0}+T}
      {\overline {f(t-\tau )}}g(t)\,dt}  [{\displaystyle (f\star g)(\tau )\
      \triangleq \int _{t_{0}}^{t_{0}+T}{\overline {f(t-\tau )}}g(t)\,dt}]
***** Cross-correlation of random vectors[edit] *****
Main article: Cross-correlation_matrix
**** Definition[edit] ****
For random_vectors      X  = (  X  1   , &#x2026; ,  X  m    )   T
{\displaystyle \mathbf {X} =(X_{1},\ldots ,X_{m})^{\rm {T}}}  [{\displaystyle
\mathbf {X} =(X_{1},\ldots ,X_{m})^{\rm {T}}}] and      Y  = (  Y  1   ,
&#x2026; ,  Y  n    )   T      {\displaystyle \mathbf {Y} =(Y_{1},\ldots ,Y_
{n})^{\rm {T}}}  [{\displaystyle \mathbf {Y} =(Y_{1},\ldots ,Y_{n})^{\rm
{T}}}], each containing random_elements whose expected_value and variance
exist, the cross-correlation matrix of      X    {\displaystyle \mathbf {X} }
[\mathbf {X} ] and      Y    {\displaystyle \mathbf {Y} }  [\mathbf {Y} ] is
defined by[8]:p.337
    R   X   Y    &#x225C; &#xA0; E &#x2061; [  X    Y    T    ]
{\displaystyle \operatorname {R} _{\mathbf {X} \mathbf {Y}
}\triangleq \ \operatorname {E} [\mathbf {X} \mathbf {Y} ^{\rm        (Eq.3)
{T}}]}  [{\displaystyle \operatorname {R} _{\mathbf {X} \mathbf       
{Y} }\triangleq \ \operatorname {E} [\mathbf {X} \mathbf {Y} ^{\rm
{T}}]}]
and has dimensions     m &#x00D7; n   {\displaystyle m\times n}  [m\times n].
Written component-wise:
          R   X   Y    =   [    E &#x2061; [  X  1    Y  1   ]   E &#x2061;
      [  X  1    Y  2   ]   &#x22EF;   E &#x2061; [  X  1    Y  n   ]        E
      &#x2061; [  X  2    Y  1   ]   E &#x2061; [  X  2    Y  2   ]   &#x22EF;
      E &#x2061; [  X  2    Y  n   ]        &#x22EE;   &#x22EE;   &#x22F1;
      &#x22EE;        E &#x2061; [  X  m    Y  1   ]   E &#x2061; [  X  m    Y
      2   ]   &#x22EF;   E &#x2061; [  X  m    Y  n   ]       ]
      {\displaystyle \operatorname {R} _{\mathbf {X} \mathbf {Y} }={\begin
      {bmatrix}\operatorname {E} [X_{1}Y_{1}]&\operatorname {E} [X_{1}Y_
      {2}]&\cdots &\operatorname {E} [X_{1}Y_{n}]\\\\\operatorname {E} [X_{2}Y_
      {1}]&\operatorname {E} [X_{2}Y_{2}]&\cdots &\operatorname {E} [X_{2}Y_
      {n}]\\\\\vdots &\vdots &\ddots &\vdots \\\\\operatorname {E} [X_{m}Y_
      {1}]&\operatorname {E} [X_{m}Y_{2}]&\cdots &\operatorname {E} [X_{m}Y_
      {n}]\\\\\end{bmatrix}}}  [{\displaystyle \operatorname {R} _{\mathbf {X}
      \mathbf {Y} }={\begin{bmatrix}\operatorname {E} [X_{1}Y_
      {1}]&\operatorname {E} [X_{1}Y_{2}]&\cdots &\operatorname {E} [X_{1}Y_
      {n}]\\\\\operatorname {E} [X_{2}Y_{1}]&\operatorname {E} [X_{2}Y_
      {2}]&\cdots &\operatorname {E} [X_{2}Y_{n}]\\\\\vdots &\vdots &\ddots
      &\vdots \\\\\operatorname {E} [X_{m}Y_{1}]&\operatorname {E} [X_{m}Y_
      {2}]&\cdots &\operatorname {E} [X_{m}Y_{n}]\\\\\end{bmatrix}}}]
The random vectors      X    {\displaystyle \mathbf {X} }  [\mathbf {X} ] and
Y    {\displaystyle \mathbf {Y} }  [\mathbf {Y} ] need not have the same
dimension, and either might be a scalar value.
**** Example[edit] ****
For example, if      X  =   (   X  1   ,  X  2   ,  X  3    )    T
{\displaystyle \mathbf {X} =\left(X_{1},X_{2},X_{3}\right)^{\rm {T}}}  [
{\displaystyle \mathbf {X} =\left(X_{1},X_{2},X_{3}\right)^{\rm {T}}}] and
Y  =   (   Y  1   ,  Y  2    )    T      {\displaystyle \mathbf {Y} =\left(Y_
{1},Y_{2}\right)^{\rm {T}}}  [{\displaystyle \mathbf {Y} =\left(Y_{1},Y_
{2}\right)^{\rm {T}}}] are random vectors, then      R   X   Y
{\displaystyle \operatorname {R} _{\mathbf {X} \mathbf {Y} }}  [{\displaystyle
\operatorname {R} _{\mathbf {X} \mathbf {Y} }}] is a     3 &#x00D7; 2
{\displaystyle 3\times 2}  [{\displaystyle 3\times 2}] matrix whose     ( i , j
)   {\displaystyle (i,j)}  [(i,j)]-th entry is     E &#x2061; [  X  i    Y  j
]   {\displaystyle \operatorname {E} [X_{i}Y_{j}]}  [{\displaystyle
\operatorname {E} [X_{i}Y_{j}]}].
**** Definition for complex random vectors[edit] ****
If      Z  = (  Z  1   , &#x2026; ,  Z  m    )   T      {\displaystyle \mathbf
{Z} =(Z_{1},\ldots ,Z_{m})^{\rm {T}}}  [{\displaystyle \mathbf {Z} =(Z_
{1},\ldots ,Z_{m})^{\rm {T}}}] and      W  = (  W  1   , &#x2026; ,  W  n    )
T      {\displaystyle \mathbf {W} =(W_{1},\ldots ,W_{n})^{\rm {T}}}  [
{\displaystyle \mathbf {W} =(W_{1},\ldots ,W_{n})^{\rm {T}}}] are complex
random_vectors, each containing random variables whose expected value and
variance exist, the cross-correlation matrix of      Z    {\displaystyle
\mathbf {Z} }  [\mathbf {Z} ] and      W    {\displaystyle \mathbf {W} }
[\mathbf {W} ] is defined by
          R   Z   W    &#x225C; &#xA0; E &#x2061; [  Z    W    H    ]
      {\displaystyle \operatorname {R} _{\mathbf {Z} \mathbf {W} }\triangleq \
      \operatorname {E} [\mathbf {Z} \mathbf {W} ^{\rm {H}}]}  [{\displaystyle
      \operatorname {R} _{\mathbf {Z} \mathbf {W} }\triangleq \ \operatorname
      {E} [\mathbf {Z} \mathbf {W} ^{\rm {H}}]}]
where          H      {\displaystyle {}^{\rm {H}}}  [{\displaystyle {}^{\rm
{H}}}] denotes Hermitian_transposition.
***** Cross-correlation of stochastic processes[edit] *****
In time_series_analysis and statistics, the cross-correlation of a pair of
random_process is the correlation between values of the processes at different
times, as a function of the two times. Let     (  X  t   ,  Y  t   )
{\displaystyle (X_{t},Y_{t})}  [{\displaystyle (X_{t},Y_{t})}] be a pair of
random processes, and     t   {\displaystyle t}  [t] be any point in time
(    t   {\displaystyle t}  [t] may be an integer for a discrete-time process
or a real_number for a continuous-time process). Then      X  t
{\displaystyle X_{t}}  [X_{t}] is the value (or realization) produced by a
given run of the process at time     t   {\displaystyle t}  [t].
**** Cross-correlation function[edit] ****
Suppose that the process has means      &#x03BC;  X   ( t )   {\displaystyle
\mu _{X}(t)}  [{\displaystyle \mu _{X}(t)}] and      &#x03BC;  Y   ( t )
{\displaystyle \mu _{Y}(t)}  [{\displaystyle \mu _{Y}(t)}] and variances
&#x03C3;  X   2   ( t )   {\displaystyle \sigma _{X}^{2}(t)}  [{\displaystyle
\sigma _{X}^{2}(t)}] and      &#x03C3;  Y   2   ( t )   {\displaystyle \sigma _
{Y}^{2}(t)}  [{\displaystyle \sigma _{Y}^{2}(t)}] at time     t
{\displaystyle t}  [t], for each     t   {\displaystyle t}  [t]. Then the
definition of the cross-correlation between times      t  1     {\displaystyle
t_{1}}  [t_{1}] and      t  2     {\displaystyle t_{2}}  [t_{2}] is[8]:p.392
    R  X Y   &#x2061; (  t  1   ,  t  2   ) = E &#x2061; [  X   t
1        Y   t  2     &#x00AF;   ]   {\displaystyle \operatorname     
{R} _{XY}(t_{1},t_{2})=\operatorname {E} [X_{t_{1}}{\overline {Y_       (Eq.4)
{t_{2}}}}]}  [{\displaystyle \operatorname {R} _{XY}(t_{1},t_
{2})=\operatorname {E} [X_{t_{1}}{\overline {Y_{t_{2}}}}]}]
where     E   {\displaystyle \operatorname {E} }  [\operatorname {E} ] is the
expected_value operator. Note that this expression may be not defined.
**** Cross-covariance function[edit] ****
Subtracting the mean before multiplication yields the cross-covariance between
times      t  1     {\displaystyle t_{1}}  [t_{1}] and      t  2
{\displaystyle t_{2}}  [t_{2}]:[8]:p.392
    K  X Y   &#x2061; (  t  1   ,  t  2   ) = E &#x2061; [ (  X
t  1     &#x2212;  &#x03BC;  X   (  t  1   ) )    (  Y   t  2
&#x2212;  &#x03BC;  Y   (  t  2   ) )  &#x00AF;   ]
{\displaystyle \operatorname {K} _{XY}(t_{1},t_{2})=\operatorname     (Eq.5)
{E} [(X_{t_{1}}-\mu _{X}(t_{1})){\overline {(Y_{t_{2}}-\mu _{Y}(t_    
{2}))}}]}  [{\displaystyle \operatorname {K} _{XY}(t_{1},t_
{2})=\operatorname {E} [(X_{t_{1}}-\mu _{X}(t_{1})){\overline {(Y_
{t_{2}}-\mu _{Y}(t_{2}))}}]}]
Note that this expression is not well-defined for all-time series or processes,
because the mean may not exist, or the variance may not exist.
**** Definition for wide-sense stationary stochastic process[edit] ****
Let     (  X  t   ,  Y  t   )   {\displaystyle (X_{t},Y_{t})}  [{\displaystyle
(X_{t},Y_{t})}] represent a pair of stochastic_processes that are jointly_wide-
sense_stationary. Then the Cross-covariance_function and the cross-correlation
function are given as follows.
*** Cross-correlation function[edit] ***
    R  X Y   &#x2061; ( &#x03C4; ) = E &#x2061;  [   X  t      Y
t + &#x03C4;   &#x00AF;    ]    {\displaystyle \operatorname {R} _    
{XY}(\tau )=\operatorname {E} \left[X_{t}{\overline {Y_{t+\tau          (Eq.6)
}}}\right]}  [{\displaystyle \operatorname {R} _{XY}(\tau
)=\operatorname {E} \left[X_{t}{\overline {Y_{t+\tau }}}\right]}]
or equivalently
          R  X Y   &#x2061; ( &#x03C4; ) = E &#x2061;  [   X  t &#x2212;
      &#x03C4;      Y  t   &#x00AF;    ]    {\displaystyle \operatorname {R} _
      {XY}(\tau )=\operatorname {E} \left[X_{t-\tau }{\overline {Y_
      {t}}}\right]}  [{\displaystyle \operatorname {R} _{XY}(\tau
      )=\operatorname {E} \left[X_{t-\tau }{\overline {Y_{t}}}\right]}]
*** Cross-covariance function[edit] ***
    K  X Y   &#x2061; ( &#x03C4; ) = E &#x2061;  [   (   X  t
&#x2212;  &#x03BC;  X    )     (   Y  t + &#x03C4;   &#x2212;
&#x03BC;  Y    )  &#x00AF;    ]    {\displaystyle \operatorname
{K} _{XY}(\tau )=\operatorname {E} \left[\left(X_{t}-\mu _            (Eq.7)
{X}\right){\overline {\left(Y_{t+\tau }-\mu _{Y}\right)}}\right]}     
[{\displaystyle \operatorname {K} _{XY}(\tau )=\operatorname {E}
\left[\left(X_{t}-\mu _{X}\right){\overline {\left(Y_{t+\tau }-\mu
_{Y}\right)}}\right]}]
or equivalently
          K  X Y   &#x2061; ( &#x03C4; ) = E &#x2061;  [   (   X  t &#x2212;
      &#x03C4;   &#x2212;  &#x03BC;  X    )     (   Y  t   &#x2212;  &#x03BC;
      Y    )  &#x00AF;    ]    {\displaystyle \operatorname {K} _{XY}(\tau
      )=\operatorname {E} \left[\left(X_{t-\tau }-\mu _{X}\right){\overline
      {\left(Y_{t}-\mu _{Y}\right)}}\right]}  [{\displaystyle \operatorname {K}
      _{XY}(\tau )=\operatorname {E} \left[\left(X_{t-\tau }-\mu _{X}\right)
      {\overline {\left(Y_{t}-\mu _{Y}\right)}}\right]}]
where      &#x03BC;  X     {\displaystyle \mu _{X}}  [\mu _{X}] and
&#x03C3;  X     {\displaystyle \sigma _{X}}  [\sigma _{X}] are the mean and
standard deviation of the process     (  X  t   )   {\displaystyle (X_{t})}  [
(X_{t})], which are constant over time due to stationarity; and similarly for
(  Y  t   )   {\displaystyle (Y_{t})}  [(Y_{t})], respectively.     E &#x2061;
[ &#xA0; ]   {\displaystyle \operatorname {E} [\ ]}  [\operatorname {E} [\ ]]
indicates the expected_value. That the cross-covariance and cross-correlation
are independent of     t   {\displaystyle t}  [t] is precisely the additional
information (beyond being individually wide-sense stationary) conveyed by the
requirement that     (  X  t   ,  Y  t   )   {\displaystyle (X_{t},Y_{t})}  [
{\displaystyle (X_{t},Y_{t})}] are jointly wide-sense stationary.
The cross-correlation of a pair of jointly wide_sense_stationary stochastic
processes can be estimated by averaging the product of samples measured from
one process and samples measured from the other (and its time shifts). The
samples included in the average can be an arbitrary subset of all the samples
in the signal (e.g., samples within a finite time window or a sub-sampling
[which?] of one of the signals). For a large number of samples, the average
converges to the true cross-correlation.
**** Normalization[edit] ****
It is common practice in some disciplines (e.g. statistics and time_series
analysis) to normalize the cross-correlation function to get a time-dependent
Pearson_correlation_coefficient. However, in other disciplines (e.g.
engineering) the normalization is usually dropped and the terms "cross-
correlation" and "cross-covariance" are used interchangeably.
The definition of the normalized cross-correlation of a stochastic process is
          &#x03C1;  X X   (  t  1   ,  t  2   ) =     K  X X   &#x2061; (  t  1
      ,  t  2   )    &#x03C3;  X   (  t  1   )  &#x03C3;  X   (  t  2   )    =
      E &#x2061; [ (  X   t  1     &#x2212;  &#x03BC;   t  1     )    (  X   t
      2     &#x2212;  &#x03BC;   t  2     )  &#x00AF;   ]    &#x03C3;  X   (  t
      1   )  &#x03C3;  X   (  t  2   )      {\displaystyle \rho _{XX}(t_{1},t_
      {2})={\frac {\operatorname {K} _{XX}(t_{1},t_{2})}{\sigma _{X}(t_
      {1})\sigma _{X}(t_{2})}}={\frac {\operatorname {E} [(X_{t_{1}}-\mu _{t_
      {1}}){\overline {(X_{t_{2}}-\mu _{t_{2}})}}]}{\sigma _{X}(t_{1})\sigma _
      {X}(t_{2})}}}  [{\displaystyle \rho _{XX}(t_{1},t_{2})={\frac
      {\operatorname {K} _{XX}(t_{1},t_{2})}{\sigma _{X}(t_{1})\sigma _{X}(t_
      {2})}}={\frac {\operatorname {E} [(X_{t_{1}}-\mu _{t_{1}}){\overline {(X_
      {t_{2}}-\mu _{t_{2}})}}]}{\sigma _{X}(t_{1})\sigma _{X}(t_{2})}}}].
If the function      &#x03C1;  X X     {\displaystyle \rho _{XX}}  [
{\displaystyle \rho _{XX}}] is well-defined, its value must lie in the range
[ &#x2212; 1 , 1 ]   {\displaystyle [-1,1]}  [[-1,1]], with 1 indicating
perfect correlation and â1 indicating perfect anti-correlation.
For jointly wide-sense stationary stochastic processes, the definition is
          &#x03C1;  X Y   ( &#x03C4; ) =     K  X Y   &#x2061; ( &#x03C4; )
      &#x03C3;  X    &#x03C3;  Y      =    E &#x2061; [  (   X  t   &#x2212;
      &#x03BC;  X    )     (   Y  t + &#x03C4;   &#x2212;  &#x03BC;  Y    )
      &#x00AF;   ]    &#x03C3;  X    &#x03C3;  Y        {\displaystyle \rho _
      {XY}(\tau )={\frac {\operatorname {K} _{XY}(\tau )}{\sigma _{X}\sigma _
      {Y}}}={\frac {\operatorname {E} [\left(X_{t}-\mu _{X}\right){\overline
      {\left(Y_{t+\tau }-\mu _{Y}\right)}}]}{\sigma _{X}\sigma _{Y}}}}  [
      {\displaystyle \rho _{XY}(\tau )={\frac {\operatorname {K} _{XY}(\tau )}
      {\sigma _{X}\sigma _{Y}}}={\frac {\operatorname {E} [\left(X_{t}-\mu _
      {X}\right){\overline {\left(Y_{t+\tau }-\mu _{Y}\right)}}]}{\sigma _
      {X}\sigma _{Y}}}}].
The normalization is important both because the interpretation of the
autocorrelation as a correlation provides a scale-free measure of the strength
of statistical_dependence, and because the normalization has an effect on the
statistical properties of the estimated autocorrelations.
**** Properties[edit] ****
*** Symmetry property[edit] ***
For jointly wide-sense stationary stochastic processes, the cross-correlation
function has the following symmetry property:[9]:p.173
          R  X Y   &#x2061; (  t  1   ,  t  2   ) =     R  Y X   &#x2061; (  t
      2   ,  t  1   )  &#x00AF;     {\displaystyle \operatorname {R} _{XY}(t_
      {1},t_{2})={\overline {\operatorname {R} _{YX}(t_{2},t_{1})}}}  [
      {\displaystyle \operatorname {R} _{XY}(t_{1},t_{2})={\overline
      {\operatorname {R} _{YX}(t_{2},t_{1})}}}]
Respectively for jointly WSS processes:
          R  X Y   &#x2061; ( &#x03C4; ) =     R  Y X   &#x2061; ( &#x2212;
      &#x03C4; )  &#x00AF;     {\displaystyle \operatorname {R} _{XY}(\tau )=
      {\overline {\operatorname {R} _{YX}(-\tau )}}}  [{\displaystyle
      \operatorname {R} _{XY}(\tau )={\overline {\operatorname {R} _{YX}(-\tau
      )}}}]
***** Time delay analysis[edit] *****
Cross-correlations are useful for determining the time delay between two
signals, e.g., for determining time delays for the propagation of acoustic
signals across a microphone array.[10][11][clarification_needed] After
calculating the cross-correlation between the two signals, the maximum (or
minimum if the signals are negatively correlated) of the cross-correlation
function indicates the point in time where the signals are best aligned; i.e.,
the time delay between the two signals is determined by the argument of the
maximum, or arg_max of the cross-correlation, as in
          &#x03C4;   d e l a y    =    a r g  m a x   t &#x2208;  R     ( ( f
      &#x22C6; g ) ( t ) )   {\displaystyle \tau _{\mathrm {delay} }={\underset
      {t\in \mathbb {R} }{\operatorname {arg\,max} }}((f\star g)(t))}  [
      {\displaystyle \tau _{\mathrm {delay} }={\underset {t\in \mathbb {R} }
      {\operatorname {arg\,max} }}((f\star g)(t))}]
***** Terminology in image processing[edit] *****
**** Zero-normalized cross-correlation (ZNCC)[edit] ****
For image-processing applications in which the brightness of the image and
template can vary due to lighting and exposure conditions, the images can be
first normalized. This is typically done at every step by subtracting the mean
and dividing by the standard_deviation. That is, the cross-correlation of a
template,     t ( x , y )   {\displaystyle t(x,y)}  [t(x,y)] with a subimage
f ( x , y )   {\displaystyle f(x,y)}  [f(x,y)] is
           1 n    &#x2211;  x , y     1   &#x03C3;  f    &#x03C3;  t       (  f
      ( x , y ) &#x2212;  &#x03BC;  f    )   (  t ( x , y ) &#x2212;  &#x03BC;
      t    )    {\displaystyle {\frac {1}{n}}\sum _{x,y}{\frac {1}{\sigma _
      {f}\sigma _{t}}}\left(f(x,y)-\mu _{f}\right)\left(t(x,y)-\mu _{t}\right)}
      [{\displaystyle {\frac {1}{n}}\sum _{x,y}{\frac {1}{\sigma _{f}\sigma _
      {t}}}\left(f(x,y)-\mu _{f}\right)\left(t(x,y)-\mu _{t}\right)}].
where     n   {\displaystyle n}  [n] is the number of pixels in     t ( x , y )
{\displaystyle t(x,y)}  [t(x,y)] and     f ( x , y )   {\displaystyle f(x,y)}
[f(x,y)],      &#x03BC;  f     {\displaystyle \mu _{f}}  [{\displaystyle \mu _
{f}}] is the average of     f   {\displaystyle f}  [f] and      &#x03C3;  f
{\displaystyle \sigma _{f}}  [\sigma _{f}] is standard_deviation of     f
{\displaystyle f}  [f].
In functional_analysis terms, this can be thought of as the dot product of two
normalized_vectors. That is, if
         F ( x , y ) = f ( x , y ) &#x2212;  &#x03BC;  f     {\displaystyle F
      (x,y)=f(x,y)-\mu _{f}}  [{\displaystyle F(x,y)=f(x,y)-\mu _{f}}]
and
         T ( x , y ) = t ( x , y ) &#x2212;  &#x03BC;  t     {\displaystyle T
      (x,y)=t(x,y)-\mu _{t}}  [{\displaystyle T(x,y)=t(x,y)-\mu _{t}}]
then the above sum is equal to
          &#x27E8;    F  &#x2016; F &#x2016;    ,   T  &#x2016; T &#x2016;
      &#x27E9;    {\displaystyle \left\langle {\frac {F}{\|F\|}},{\frac {T}
      {\|T\|}}\right\rangle }  [\left\langle {\frac {F}{\|F\|}},{\frac {T}
      {\|T\|}}\right\rangle ]
where     &#x27E8; &#x22C5; , &#x22C5; &#x27E9;   {\displaystyle \langle \cdot
,\cdot \rangle }  [\langle \cdot ,\cdot \rangle ] is the inner_product and
&#x2016; &#x22C5; &#x2016;   {\displaystyle \|\cdot \|}  [\|\cdot \|] is the
LÂ²_norm.
Thus, if     f   {\displaystyle f}  [f] and     t   {\displaystyle t}  [t] are
real matrices, their normalized cross-correlation equals the cosine of the
angle between the unit vectors     F   {\displaystyle F}  [F] and     T
{\displaystyle T}  [T], being thus     1   {\displaystyle 1}  [1] if and only
if     F   {\displaystyle F}  [F] equals     T   {\displaystyle T}  [T]
multiplied by a positive scalar.
Normalized correlation is one of the methods used for template_matching, a
process used for finding incidences of a pattern or object within an image. It
is also the 2-dimensional version of Pearson_product-moment_correlation
coefficient.
**** Normalized cross-correlation (NCC)[edit] ****
NCC is similar to ZNCC with the only difference of not subtracting the local
mean value of intensities:
           1 n    &#x2211;  x , y     1   &#x03C3;  f    &#x03C3;  t      f ( x
      , y ) t ( x , y )   {\displaystyle {\frac {1}{n}}\sum _{x,y}{\frac {1}
      {\sigma _{f}\sigma _{t}}}f(x,y)t(x,y)}  [{\displaystyle {\frac {1}
      {n}}\sum _{x,y}{\frac {1}{\sigma _{f}\sigma _{t}}}f(x,y)t(x,y)}]
***** Nonlinear systems[edit] *****
Caution must be applied when using cross correlation for nonlinear systems. In
certain circumstances, which depend on the properties of the input, cross
correlation between the input and output of a system with nonlinear dynamics
can be completely blind to certain nonlinear effects.[12] This problem arises
because some quadratic moments can equal zero and this can incorrectly suggest
that there is little "correlation" (in the sense of statistical dependence)
between two signals, when in fact the two signals are strongly related by
nonlinear dynamics.
***** See also[edit] *****
    * Autocorrelation
    * Autocovariance
    * Coherence
    * Convolution
    * Correlation
    * Correlation_function
    * Cross-correlation_matrix
    * Cross-covariance
    * Cross-spectrum
    * Digital_image_correlation
    * Phase_correlation
    * Scaled_correlation
    * Spectral_density
    * WienerâKhinchin_theorem
***** References[edit] *****
   1. ^ Bracewell, R. "Pentagram Notation for Cross Correlation." The Fourier
      Transform and Its Applications. New York: McGraw-Hill, pp. 46 and 243,
      1965.
   2. ^  Papoulis, A. The Fourier Integral and Its Applications. New York:
      McGraw-Hill, pp. 244â245 and 252-253, 1962.
   3. ^ Weisstein, Eric W. "Cross-Correlation." From MathWorld--A Wolfram Web
      Resource. http://mathworld.wolfram.com/Cross-Correlation.html
   4. ^Rabiner, L.R.; Schafer, R.W. (1978). Digital Processing of Speech
      Signals. Signal Processing Series. Upper Saddle River, NJ: Prentice Hall.
      pp. 147â148. ISBN 0132136031.
   5. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   6. ^Rabiner, Lawrence R.; Gold, Bernard (1975). Theory and Application of
      Digital Signal Processing. Englewood Cliffs, NJ: Prentice-Hall. p. 401.
      ISBN 0139141014.
   7. ^Campbell; Lo; MacKinlay (1996). The Econometrics of Financial Markets.
      NJ: Princeton University Press. ISBN 0691043019.
   8. ^Kapinchev, Konstantin; Bradu, Adrian; Barnes, Frederick; Podoleanu,
      Adrian (2015). "GPU implementation of cross-correlation for image
      generation in real time". 2015 9th International Conference on Signal
      Processing and Communication Systems (ICSPCS). pp. 1â6. doi:10.1109/
      ICSPCS.2015.7391783. ISBN 978-1-4673-8118-5.
   9. ^ a b cGubner, John A. (2006). Probability and Random Processes for
      Electrical and Computer Engineers. Cambridge University Press. ISBN 978-
      0-521-86470-1.
  10. ^ Kun Il Park, Fundamentals of Probability and Stochastic Processes with
      Applications to Communications, Springer, 2018, 978-3-319-68074-3
  11. ^Rhudy, Matthew; Brian Bucci; Jeffrey Vipperman; Jeffrey Allanach; Bruce
      Abraham (November 2009). "Microphone Array Analysis Methods Using Cross-
      Correlations". Proceedings of 2009 ASME International Mechanical
      Engineering Congress, Lake Buena Vista, FL: 281â288. doi:10.1115/
      IMECE2009-10798. ISBN 978-0-7918-4388-8.
  12. ^Rhudy, Matthew (November 2009). "Real_Time_Implementation_of_a_Military
      Impulse_Classifier". University of Pittsburgh, Master's Thesis.
  13. ^Billings, S. A. (2013). Nonlinear System Identification: NARMAX Methods
      in the Time, Frequency, and Spatio-Temporal Domains. Wiley. ISBN 978-1-
      118-53556-1.
***** Further reading[edit] *****
    * Tahmasebi, Pejman; Hezarkhani, Ardeshir; Sahimi, Muhammad (2012).
      "Multiple-point geostatistical modeling based on the cross-correlation
      functions". Computational Geosciences. 16 (3): 779â797. doi:10.1007/
      s10596-012-9287-1.
***** External links[edit] *****
    * Cross_Correlation_from_Mathworld
    * http://scribblethink.org/Work/nvisionInterface/nip.html
    * http://www.phys.ufl.edu/LIGO/stochastic/sign05.pdf
    * http://www.staff.ncl.ac.uk/oliver.hinton/eee305/Chapter6.pdf
    * v
    * t
    * e
Statistics
    * Outline
    * Index
Descriptive_statistics
                               * Mean
                                     o arithmetic
                Center               o geometric
                                     o harmonic
                               * Median
                               * Mode
                               * Variance
                               * Standard_deviation
Continuous_data Dispersion     * Coefficient_of_variation
                               * Percentile
                               * Range
                               * Interquartile_range
                               * Central_limit_theorem
                               * Moments
                Shape                o Skewness
                                     o Kurtosis
                                     o L-moments
Count_data          * Index_of_dispersion
                    * Grouped_data
Summary tables      * Frequency_distribution
                    * Contingency_table
                    * Pearson_product-moment_correlation
                    * Rank_correlation
Dependence                o Spearman's_rho
                          o Kendall's_tau
                    * Partial_correlation
                    * Scatter_plot
                    * Bar_chart
                    * Biplot
                    * Box_plot
                    * Control_chart
                    * Correlogram
                    * Fan_chart
Graphics            * Forest_plot
                    * Histogram
                    * Pie_chart
                    * QâQ_plot
                    * Run_chart
                    * Scatter_plot
                    * Stem-and-leaf_display
                    * Radar_chart
Data_collection
                           * Population
                           * Statistic
                           * Effect_size
Study_design               * Statistical_power
                           * Optimal_design
                           * Sample_size_determination
                           * Replication
                           * Missing_data
                           * Sampling
                                 o stratified
Survey_methodology               o cluster
                           * Standard_error
                           * Opinion_poll
                           * Questionnaire
                           * Scientific_control
                           * Randomized_experiment
                           * Randomized_controlled_trial
Controlled_experiments     * Random_assignment
                           * Blocking
                           * Interaction
                           * Factorial_experiment
                           * Adaptive_clinical_trial
Adaptive Designs           * Up-and-Down_Designs
                           * Stochastic_approximation
                           * Cross-sectional_study
Observational_Studies      * Cohort_study
                           * Natural_experiment
                           * Quasi-experiment
Statistical_inference
                * Population
                * Statistic
                * Probability_distribution
                * Sampling_distribution
                      o Order_statistic
                * Empirical_distribution
                      o Density_estimation
                * Statistical_model
                      o Model_specification
                      o Lp_space
                * Parameter
                      o location
                      o scale
                      o shape
Statistical     * Parametric_family
theory                o Likelihood (monotone)
                      o Locationâscale_family
                      o Exponential_family
                * Completeness
                * Sufficiency
                * Statistical_functional
                      o Bootstrap
                      o U
                      o V
                * Optimal_decision
                      o loss_function
                * Efficiency
                * Statistical_distance
                      o divergence
                * Asymptotics
                * Robustness
                                    * Estimating_equations
                                          o Maximum_likelihood
                                          o Method_of_moments
                                          o M-estimator
                                          o Minimum_distance
            Point_estimation        * Unbiased_estimators
                                          o Mean-unbiased_minimum-variance
                                                # RaoâBlackwellization
                                                # LehmannâScheffÃ©_theorem
                                          o Median_unbiased
                                    * Plug-in
                                    * Confidence_interval
                                    * Pivot
Frequentist                         * Likelihood_interval
inference   Interval_estimation     * Prediction_interval
                                    * Tolerance_interval
                                    * Resampling
                                          o Bootstrap
                                          o Jackknife
                                    * 1-_&_2-tails
                                    * Power
            Testing_hypotheses            o Uniformly_most_powerful_test
                                    * Permutation_test
                                          o Randomization_test
                                    * Multiple_comparisons
                                    * Likelihood-ratio
            Parametric_tests        * Score/Lagrange_multiplier
                                    * Wald
                * Z-test_(normal)
                * Student's_t-test
                * F-test
                           * Chi-squared
                           * G-test
                           * KolmogorovâSmirnov
                           * AndersonâDarling
                           * Lilliefors
            Goodness       * JarqueâBera
            of_fit         * Normality_(ShapiroâWilk)
                           * Likelihood-ratio_test
Specific                   * Model_selection
tests                            o Cross_validation
                                 o AIC
                                 o BIC
                           * Sign
                                 o Sample_median
                           * Signed_rank_(Wilcoxon)
            Rank                 o HodgesâLehmann_estimator
            statistics     * Rank_sum_(MannâWhitney)
                           * Nonparametric anova
                                 o 1-way_(KruskalâWallis)
                                 o 2-way_(Friedman)
                                 o Ordered_alternative_(JonckheereâTerpstra)
                * Bayesian_probability
                      o prior
Bayesian              o posterior
inference       * Credible_interval
                * Bayes_factor
                * Bayesian_estimator
                      o Maximum_posterior_estimator
    * Correlation
    * Regression_analysis
                       * Pearson_product-moment
Correlation            * Partial_correlation
                       * Confounding_variable
                       * Coefficient_of_determination
                       * Errors_and_residuals
Regression             * Regression_validation
analysis               * Mixed_effects_models
                       * Simultaneous_equations_models
                       * Multivariate_adaptive_regression_splines_(MARS)
                       * Simple_linear_regression
Linear_regression      * Ordinary_least_squares
                       * General_linear_model
                       * Bayesian_regression
                       * Nonlinear_regression
                       * Nonparametric
Non-standard           * Semiparametric
predictors             * Isotonic
                       * Robust
                       * Heteroscedasticity
                       * Homoscedasticity
Generalized_linear     * Exponential_families
model                  * Logistic_(Bernoulli) / Binomial / Poisson_regressions
                       * Analysis_of_variance_(ANOVA,_anova)
Partition_of           * Analysis_of_covariance
variance               * Multivariate_ANOVA
                       * Degrees_of_freedom
Categorical / Multivariate / Time-series / Survival_analysis
                 * Cohen's_kappa
                 * Contingency_table
Categorical      * Graphical_model
                 * Log-linear_model
                 * McNemar's_test
                 * Regression
                 * Manova
                 * Principal_components
                 * Canonical_correlation
                 * Discriminant_analysis
Multivariate     * Cluster_analysis
                 * Classification
                 * Structural_equation_model
                       o Factor_analysis
                 * Multivariate_distributions
                       o Elliptical_distributions
                             # Normal
                                  * Decomposition
                                  * Trend
                                  * Stationarity
             General              * Seasonal_adjustment
                                  * Exponential_smoothing
                                  * Cointegration
                                  * Structural_break
                                  * Granger_causality
                                  * DickeyâFuller
                                  * Johansen
             Specific tests       * Q-statistic_(LjungâBox)
                                  * DurbinâWatson
Time-series                       * BreuschâGodfrey
                                  * Autocorrelation_(ACF)
                                        o partial_(PACF)
                                  * Cross-correlation (XCF)
             Time_domain          * ARMA_model
                                  * ARIMA_model_(BoxâJenkins)
                                  * Autoregressive_conditional
                                    heteroskedasticity_(ARCH)
                                  * Vector_autoregression_(VAR)
                                  * Spectral_density_estimation
             Frequency_domain     * Fourier_analysis
                                  * Wavelet
                                  * Whittle_likelihood
                                   * KaplanâMeier_estimator_(product_limit)
             Survival_function     * Proportional_hazards_models
Survival                           * Accelerated_failure_time_(AFT)_model
                                   * First_hitting_time
             Hazard_function       * NelsonâAalen_estimator
             Test                  * Log-rank_test
Applications
                           * Bioinformatics
Biostatistics              * Clinical_trials / studies
                           * Epidemiology
                           * Medical_statistics
                           * Chemometrics
                           * Methods_engineering
Engineering_statistics     * Probabilistic_design
                           * Process / quality_control
                           * Reliability
                           * System_identification
                           * Actuarial_science
                           * Census
                           * Crime_statistics
                           * Demography
Social_statistics          * Econometrics
                           * National_accounts
                           * Official_statistics
                           * Population_statistics
                           * Psychometrics
                           * Cartography
                           * Environmental_statistics
Spatial_statistics         * Geographic_information_system
                           * Geostatistics
                           * Kriging
    * [Category]Category
    * [Portal]Portal
    * [Commons page]Commons
    * [WikiProject] WikiProject

Retrieved from "https://en.wikipedia.org/w/index.php?title=Cross-
correlation&oldid=908671343"
Categories:
    * Bilinear_operators
    * Covariance_and_correlation
    * Signal_processing
    * Time_domain_analysis
Hidden categories:
    * All_articles_with_specifically_marked_weasel-worded_phrases
    * Articles_with_specifically_marked_weasel-worded_phrases_from_May_2015
    * Wikipedia_articles_needing_clarification_from_May_2015
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
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * ä¸­æ
Edit_links
    * This page was last edited on 31 July 2019, at 06:49 (UTC).
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
