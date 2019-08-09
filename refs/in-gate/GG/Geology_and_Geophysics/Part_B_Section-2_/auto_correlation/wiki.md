The following text has been accessed from https://en.wikipedia.org/wiki/Autocorrelation at Thu Aug 8 23:23:12 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Autocorrelation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
correlation of a signal with a time-shifted copy of itself, as a function of
shift
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
Above: A plot of a series of 100 random numbers concealing a sine function.
Below: The sine function revealed in a correlogram produced by autocorrelation.
Visual comparison of convolution, cross-correlation and autocorrelation.
Autocorrelation, also known as serial correlation, is the correlation of a
signal with a delayed copy of itself as a function of delay. Informally, it is
the similarity between observations as a function of the time lag between them.
The analysis of autocorrelation is a mathematical tool for finding repeating
patterns, such as the presence of a periodic_signal obscured by noise, or
identifying the missing_fundamental_frequency in a signal implied by its
harmonic frequencies. It is often used in signal_processing for analyzing
functions or series of values, such as time_domain signals.
Different fields of study define autocorrelation differently, and not all of
these definitions are equivalent. In some fields, the term is used
interchangeably with autocovariance.
Unit_root processes, trend_stationary processes, autoregressive_processes, and
moving_average_processes are specific forms of processes with autocorrelation.
⁰
***** Contents *****
    * 1_Auto-correlation_of_stochastic_processes
          o 1.1_Definition_for_wide-sense_stationary_stochastic_process
          o 1.2_Normalization
          o 1.3_Properties
                # 1.3.1_Symmetry_property
                # 1.3.2_Maximum_at_zero
                # 1.3.3_CauchyâSchwarz_inequality
                # 1.3.4_Autocorrelation_of_white_noise
                # 1.3.5_WienerâKhinchin_theorem
    * 2_Auto-correlation_of_random_vectors
          o 2.1_Definition
          o 2.2_Example
    * 3_Auto-correlation_of_deterministic_signals
          o 3.1_Auto-correlation_of_continuous-time_signal
          o 3.2_Auto-correlation_of_discrete-time_signal
          o 3.3_Definition_for_periodic_signals
          o 3.4_Properties
    * 4_Multi-dimensional_autocorrelation
    * 5_Efficient_computation
    * 6_Estimation
    * 7_Regression_analysis
    * 8_Applications
    * 9_Serial_dependence
    * 10_See_also
    * 11_References
    * 12_Further_reading
    * 13_External_links
***** Auto-correlation of stochastic processes[edit] *****
In statistics, the autocorrelation of a real or complex random_process is the
Pearson_correlation between values of the process at different times, as a
function of the two times or of the time lag . Let      {  X  t   }
{\displaystyle \left\{X_{t}\right\}}  [{\displaystyle \left\{X_{t}\right\}}] be
a random process, and     t   {\displaystyle t}  [t] be any point in time
(    t   {\displaystyle t}  [t] may be an integer for a discrete-time process
or a real_number for a continuous-time process). Then      X  t
{\displaystyle X_{t}}  [X_{t}] is the value (or realization) produced by a
given run of the process at time     t   {\displaystyle t}  [t]. Suppose that
the process has mean      &#x03BC;  t     {\displaystyle \mu _{t}}  [\mu _{t}]
and variance      &#x03C3;  t   2     {\displaystyle \sigma _{t}^{2}}  [\sigma
_{t}^{2}] at time     t   {\displaystyle t}  [t], for each     t
{\displaystyle t}  [t]. Then the definition of the auto-correlation function
between times      t  1     {\displaystyle t_{1}}  [t_{1}] and      t  2
{\displaystyle t_{2}}  [t_{2}] is[1]:p.388[2]:p.165
    R  X X   &#x2061; (  t  1   ,  t  2   ) = E &#x2061; [  X   t
1        X   t  2     &#x00AF;   ]   {\displaystyle \operatorname     
{R} _{XX}(t_{1},t_{2})=\operatorname {E} [X_{t_{1}}{\overline {X_       (Eq.1)
{t_{2}}}}]}  [{\displaystyle \operatorname {R} _{XX}(t_{1},t_
{2})=\operatorname {E} [X_{t_{1}}{\overline {X_{t_{2}}}}]}]
where     E   {\displaystyle \operatorname {E} }  [\operatorname {E} ] is the
expected_value operator and the bar represents complex conjugation. Note that
the expectation may be not well defined.
Subtracting the mean before multiplication yields the auto-covariance function
between times      t  1     {\displaystyle t_{1}}  [t_{1}] and      t  2
{\displaystyle t_{2}}  [t_{2}]:[1]:p.392[2]:p.168
    K  X X   &#x2061; (  t  1   ,  t  2   ) = E &#x2061; [ (  X
t  1     &#x2212;  &#x03BC;   t  1     )    (  X   t  2
&#x2212;  &#x03BC;   t  2     )  &#x00AF;   ] = E &#x2061; [  X
t  1        X   t  2     &#x00AF;   ] &#x2212;  &#x03BC;   t  1
&#x03BC;   t  2     &#x00AF;     {\displaystyle \operatorname {K}
_{XX}(t_{1},t_{2})=\operatorname {E} [(X_{t_{1}}-\mu _{t_{1}})        (Eq.2)
{\overline {(X_{t_{2}}-\mu _{t_{2}})}}]=\operatorname {E} [X_{t_      
{1}}{\overline {X_{t_{2}}}}]-\mu _{t_{1}}{\overline {\mu _{t_
{2}}}}}  [{\displaystyle \operatorname {K} _{XX}(t_{1},t_
{2})=\operatorname {E} [(X_{t_{1}}-\mu _{t_{1}}){\overline {(X_{t_
{2}}-\mu _{t_{2}})}}]=\operatorname {E} [X_{t_{1}}{\overline {X_
{t_{2}}}}]-\mu _{t_{1}}{\overline {\mu _{t_{2}}}}}]
Note that this expression is not well-defined for all-time series or processes,
because the mean may not exist, or the variance may be zero (for a constant
process) or infinite (for processes with distribution lacking well-behaved
moments, such as certain types of power law).
**** Definition for wide-sense stationary stochastic process[edit] ****
If      {  X  t   }    {\displaystyle \left\{X_{t}\right\}}  [{\displaystyle
\left\{X_{t}\right\}}] is a wide-sense_stationary_process then the mean
&#x03BC;   {\displaystyle \mu }  [\mu ] and the variance      &#x03C3;  2
{\displaystyle \sigma ^{2}}  [\sigma ^{2}] are time-independent, and further
the autocovariance function depends only on the lag between      t  1
{\displaystyle t_{1}}  [t_{1}] and      t  2     {\displaystyle t_{2}}  [t_
{2}]: the autocovariance depends only on the time-distance between the pair of
values but not on their position in time. This further implies that the
autocovariance and auto-correlation can be expressed as a function of the time-
lag, and that this would be an even_function of the lag     &#x03C4; =  t  2
&#x2212;  t  1     {\displaystyle \tau =t_{2}-t_{1}}  [{\displaystyle \tau =t_
{2}-t_{1}}]. This gives the more familiar forms for the auto-correlation
function[1]:p.395
    R  X X   &#x2061; ( &#x03C4; ) = E &#x2061; [  X  t      X  t
+ &#x03C4;   &#x00AF;   ]   {\displaystyle \operatorname {R} _{XX}    
(\tau )=\operatorname {E} [X_{t}{\overline {X_{t+\tau }}}]}  [          (Eq.3)
{\displaystyle \operatorname {R} _{XX}(\tau )=\operatorname {E}
[X_{t}{\overline {X_{t+\tau }}}]}]
and the auto-covariance function:
    K  X X   &#x2061; ( &#x03C4; ) = E &#x2061; [ (  X  t
&#x2212; &#x03BC; )    (  X  t + &#x03C4;   &#x2212; &#x03BC; )
&#x00AF;   ] = E &#x2061; [  X  t      X  t + &#x03C4;   &#x00AF;
] &#x2212; &#x03BC;   &#x03BC; &#x00AF;     {\displaystyle
\operatorname {K} _{XX}(\tau )=\operatorname {E} [(X_{t}-\mu )       (Eq.4)
{\overline {(X_{t+\tau }-\mu )}}]=\operatorname {E} [X_{t}           
{\overline {X_{t+\tau }}}]-\mu {\overline {\mu }}}  [
{\displaystyle \operatorname {K} _{XX}(\tau )=\operatorname {E} [
(X_{t}-\mu ){\overline {(X_{t+\tau }-\mu )}}]=\operatorname {E}
[X_{t}{\overline {X_{t+\tau }}}]-\mu {\overline {\mu }}}]
**** Normalization[edit] ****
It is common practice in some disciplines (e.g. statistics and time_series
analysis) to normalize the autocovariance function to get a time-dependent
Pearson_correlation_coefficient. However, in other disciplines (e.g.
engineering) the normalization is usually dropped and the terms
"autocorrelation" and "autocovariance" are used interchangeably.
The definition of the auto-correlation coefficient of a stochastic process is
[2]:p.169
          &#x03C1;  X X   (  t  1   ,  t  2   ) =     K  X X   &#x2061; (  t  1
      ,  t  2   )    &#x03C3;   t  1      &#x03C3;   t  2        =    E
      &#x2061; [ (  X   t  1     &#x2212;  &#x03BC;   t  1     )    (  X   t  2
      &#x2212;  &#x03BC;   t  2     )  &#x00AF;   ]    &#x03C3;   t  1
      &#x03C3;   t  2          {\displaystyle \rho _{XX}(t_{1},t_{2})={\frac
      {\operatorname {K} _{XX}(t_{1},t_{2})}{\sigma _{t_{1}}\sigma _{t_{2}}}}=
      {\frac {\operatorname {E} [(X_{t_{1}}-\mu _{t_{1}}){\overline {(X_{t_
      {2}}-\mu _{t_{2}})}}]}{\sigma _{t_{1}}\sigma _{t_{2}}}}}  [{\displaystyle
      \rho _{XX}(t_{1},t_{2})={\frac {\operatorname {K} _{XX}(t_{1},t_{2})}
      {\sigma _{t_{1}}\sigma _{t_{2}}}}={\frac {\operatorname {E} [(X_{t_{1}}-
      \mu _{t_{1}}){\overline {(X_{t_{2}}-\mu _{t_{2}})}}]}{\sigma _{t_
      {1}}\sigma _{t_{2}}}}}].
If the function      &#x03C1;  X X     {\displaystyle \rho _{XX}}  [
{\displaystyle \rho _{XX}}] is well-defined, its value must lie in the range
[ &#x2212; 1 , 1 ]   {\displaystyle [-1,1]}  [[-1,1]], with 1 indicating
perfect correlation and â1 indicating perfect anti-correlation.
For a weak-sense stationarity,_wide-sense_stationarity (WSS) process, the
definition is
          &#x03C1;  X X   ( &#x03C4; ) =     K  X X   &#x2061; ( &#x03C4; )
      &#x03C3;  2     =    E &#x2061; [ (  X  t   &#x2212; &#x03BC; )    (  X
      t + &#x03C4;   &#x2212; &#x03BC; )  &#x00AF;   ]   &#x03C3;  2
      {\displaystyle \rho _{XX}(\tau )={\frac {\operatorname {K} _{XX}(\tau )}
      {\sigma ^{2}}}={\frac {\operatorname {E} [(X_{t}-\mu ){\overline {(X_
      {t+\tau }-\mu )}}]}{\sigma ^{2}}}}  [{\displaystyle \rho _{XX}(\tau )=
      {\frac {\operatorname {K} _{XX}(\tau )}{\sigma ^{2}}}={\frac
      {\operatorname {E} [(X_{t}-\mu ){\overline {(X_{t+\tau }-\mu )}}]}{\sigma
      ^{2}}}}]
where
          K  X X   &#x2061; ( 0 ) =  &#x03C3;  2     {\displaystyle
      \operatorname {K} _{XX}(0)=\sigma ^{2}}  [{\displaystyle \operatorname
      {K} _{XX}(0)=\sigma ^{2}}].
The normalization is important both because the interpretation of the
autocorrelation as a correlation provides a scale-free measure of the strength
of statistical_dependence, and because the normalization has an effect on the
statistical properties of the estimated autocorrelations.
**** Properties[edit] ****
*** Symmetry property[edit] ***
The fact that the auto-correlation function      R  X X     {\displaystyle
\operatorname {R} _{XX}}  [{\displaystyle \operatorname {R} _{XX}}] this is an
even_function can be stated as[2]:p.171
          R  X X   &#x2061; (  t  1   ,  t  2   ) =     R  X X   &#x2061; (  t
      2   ,  t  1   )  &#x00AF;     {\displaystyle \operatorname {R} _{XX}(t_
      {1},t_{2})={\overline {\operatorname {R} _{XX}(t_{2},t_{1})}}}  [
      {\displaystyle \operatorname {R} _{XX}(t_{1},t_{2})={\overline
      {\operatorname {R} _{XX}(t_{2},t_{1})}}}]
Respectively for WSS a process:[2]:p.173
          R  X X   &#x2061; ( &#x03C4; ) =     R  X X   &#x2061; ( &#x2212;
      &#x03C4; )  &#x00AF;     {\displaystyle \operatorname {R} _{XX}(\tau )=
      {\overline {\operatorname {R} _{XX}(-\tau )}}}  [{\displaystyle
      \operatorname {R} _{XX}(\tau )={\overline {\operatorname {R} _{XX}(-\tau
      )}}}].
*** Maximum at zero[edit] ***
For a WSS process:[2]:p.174
          |   R  X X   &#x2061; ( &#x03C4; )  |  &#x2264;  R  X X   &#x2061;
      ( 0 )   {\displaystyle \left|\operatorname {R} _{XX}(\tau )\right|\leq
      \operatorname {R} _{XX}(0)}  [{\displaystyle \left|\operatorname {R} _
      {XX}(\tau )\right|\leq \operatorname {R} _{XX}(0)}]
Notice that      R  X X   &#x2061; ( 0 )   {\displaystyle \operatorname {R} _
{XX}(0)}  [{\displaystyle \operatorname {R} _{XX}(0)}] is always real.
*** CauchyâSchwarz inequality[edit] ***
The CauchyâSchwarz_inequality, inequality for stochastic processes:[1]:p.392
           |   R  X X   &#x2061; (  t  1   ,  t  2   )  |   2   &#x2264; E
      &#x2061; [  |   X   t  1       |   2   ] E &#x2061; [  |   X   t  2
      |   2   ]   {\displaystyle \left|\operatorname {R} _{XX}(t_{1},t_
      {2})\right|^{2}\leq \operatorname {E} [|X_{t_{1}}|^{2}]\operatorname {E}
      [|X_{t_{2}}|^{2}]}  [{\displaystyle \left|\operatorname {R} _{XX}(t_
      {1},t_{2})\right|^{2}\leq \operatorname {E} [|X_{t_{1}}|^
      {2}]\operatorname {E} [|X_{t_{2}}|^{2}]}]
*** Autocorrelation of white noise[edit] ***
The autocorrelation of a continuous-time white_noise signal will have a strong
peak (represented by a Dirac_delta_function) at     &#x03C4; = 0
{\displaystyle \tau =0}  [\tau =0] and will be exactly 0 for all other
&#x03C4;   {\displaystyle \tau }  [\tau ].
*** WienerâKhinchin theorem[edit] ***
The WienerâKhinchin_theorem relates the autocorrelation function      R  X X
{\displaystyle \operatorname {R} _{XX}}  [{\displaystyle \operatorname {R} _
{XX}}] to the power_spectral_density      S  X X     {\displaystyle S_{XX}}  [
{\displaystyle S_{XX}}] via the Fourier_transform:
          R  X X   &#x2061; ( &#x03C4; ) =  &#x222B;  &#x2212; &#x221E;
      &#x221E;    S  X X   ( f )  e  i 2 &#x03C0; f &#x03C4;      d   f
      {\displaystyle \operatorname {R} _{XX}(\tau )=\int _{-\infty }^{\infty
      }S_{XX}(f)e^{i2\pi f\tau }\,{\rm {d}}f}  [{\displaystyle \operatorname
      {R} _{XX}(\tau )=\int _{-\infty }^{\infty }S_{XX}(f)e^{i2\pi f\tau }\,
      {\rm {d}}f}]
          S  X X   ( f ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;    R  X X
      &#x2061; ( &#x03C4; )  e  &#x2212; i 2 &#x03C0; f &#x03C4;      d
      &#x03C4;   {\displaystyle S_{XX}(f)=\int _{-\infty }^{\infty
      }\operatorname {R} _{XX}(\tau )e^{-i2\pi f\tau }\,{\rm {d}}\tau }  [
      {\displaystyle S_{XX}(f)=\int _{-\infty }^{\infty }\operatorname {R} _
      {XX}(\tau )e^{-i2\pi f\tau }\,{\rm {d}}\tau }].
For real-valued functions, the symmetric autocorrelation function has a real
symmetric transform, so the WienerâKhinchin_theorem can be re-expressed in
terms of real cosines only:
          R  X X   &#x2061; ( &#x03C4; ) =  &#x222B;  &#x2212; &#x221E;
      &#x221E;    S  X X   ( f ) cos &#x2061; ( 2 &#x03C0; f &#x03C4; )    d
      f   {\displaystyle \operatorname {R} _{XX}(\tau )=\int _{-\infty }^
      {\infty }S_{XX}(f)\cos(2\pi f\tau )\,{\rm {d}}f}  [{\displaystyle
      \operatorname {R} _{XX}(\tau )=\int _{-\infty }^{\infty }S_{XX}(f)\cos
      (2\pi f\tau )\,{\rm {d}}f}]
          S  X X   ( f ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;    R  X X
      &#x2061; ( &#x03C4; ) cos &#x2061; ( 2 &#x03C0; f &#x03C4; )    d
      &#x03C4;   {\displaystyle S_{XX}(f)=\int _{-\infty }^{\infty
      }\operatorname {R} _{XX}(\tau )\cos(2\pi f\tau )\,{\rm {d}}\tau }  [
      {\displaystyle S_{XX}(f)=\int _{-\infty }^{\infty }\operatorname {R} _
      {XX}(\tau )\cos(2\pi f\tau )\,{\rm {d}}\tau }].
***** Auto-correlation of random vectors[edit] *****
Main article: Autocorrelation_matrix
**** Definition[edit] ****
For a random_vector      X  = (  X  1   , &#x2026; ,  X  n    )   T
{\displaystyle \mathbf {X} =(X_{1},\ldots ,X_{n})^{\rm {T}}}  [{\displaystyle
\mathbf {X} =(X_{1},\ldots ,X_{n})^{\rm {T}}}] containing random_elements whose
expected_value and variance exist, the auto-correlation matrix is defined by
    R   X   X    &#x225C; &#xA0; E &#x2061; [  X    X    T    ]
{\displaystyle \operatorname {R} _{\mathbf {X} \mathbf {X}
}\triangleq \ \operatorname {E} [\mathbf {X} \mathbf {X} ^{\rm        (Eq.5)
{T}}]}  [{\displaystyle \operatorname {R} _{\mathbf {X} \mathbf       
{X} }\triangleq \ \operatorname {E} [\mathbf {X} \mathbf {X} ^{\rm
{T}}]}]
and has dimensions     n &#x00D7; n   {\displaystyle n\times n}  [n\times n].
If      Z    {\displaystyle \mathbf {Z} }  [\mathbf {Z} ] is a complex_random
vector, the autocorrelation is instead defined by
          R   Z   Z    &#x225C; &#xA0; E &#x2061; [  Z    Z    H    ]
      {\displaystyle \operatorname {R} _{\mathbf {Z} \mathbf {Z} }\triangleq \
      \operatorname {E} [\mathbf {Z} \mathbf {Z} ^{\rm {H}}]}  [{\displaystyle
      \operatorname {R} _{\mathbf {Z} \mathbf {Z} }\triangleq \ \operatorname
      {E} [\mathbf {Z} \mathbf {Z} ^{\rm {H}}]}].
**** Example[edit] ****
For example, if      X  =   (   X  1   ,  X  2   ,  X  3    )    T
{\displaystyle \mathbf {X} =\left(X_{1},X_{2},X_{3}\right)^{\rm {T}}}  [
{\displaystyle \mathbf {X} =\left(X_{1},X_{2},X_{3}\right)^{\rm {T}}}] is a
random vector, then      R   X   X      {\displaystyle \operatorname {R} _
{\mathbf {X} \mathbf {X} }}  [{\displaystyle \operatorname {R} _{\mathbf {X}
\mathbf {X} }}] is a     3 &#x00D7; 3   {\displaystyle 3\times 3}  [3 \times 3]
matrix whose     ( i , j )   {\displaystyle (i,j)}  [(i,j)]-th entry is     E
&#x2061; [  X  i    X  j   ]   {\displaystyle \operatorname {E} [X_{i}X_{j}]}
[{\displaystyle \operatorname {E} [X_{i}X_{j}]}].
***** Auto-correlation of deterministic signals[edit] *****
In signal_processing, the above definition is often used without the
normalization, that is, without subtracting the mean and dividing by the
variance. When the autocorrelation function is normalized by mean and variance,
it is sometimes referred to as the autocorrelation coefficient[3] or
autocovariance function.
**** Auto-correlation of continuous-time signal[edit] ****
Given a signal     f ( t )   {\displaystyle f(t)}  [f(t)], the continuous
autocorrelation      R  f f   ( &#x03C4; )   {\displaystyle R_{ff}(\tau )}  [R_
{ff}(\tau )] is most often defined as the continuous cross-correlation integral
of     f ( t )   {\displaystyle f(t)}  [f(t)] with itself, at lag     &#x03C4;
{\displaystyle \tau }  [\tau ].[1]:p.411
    R  f f   ( &#x03C4; ) =  &#x222B;  &#x2212; &#x221E;
&#x221E;   f ( t + &#x03C4; )    f ( t )  &#x00AF;      d   t =
&#x222B;  &#x2212; &#x221E;   &#x221E;   f ( t )    f ( t &#x2212;
&#x03C4; )  &#x00AF;      d   t   {\displaystyle R_{ff}(\tau          
)=\int _{-\infty }^{\infty }f(t+\tau ){\overline {f(t)}}\,{\rm          (Eq.6)
{d}}t=\int _{-\infty }^{\infty }f(t){\overline {f(t-\tau )}}\,{\rm
{d}}t}  [{\displaystyle R_{ff}(\tau )=\int _{-\infty }^{\infty }f
(t+\tau ){\overline {f(t)}}\,{\rm {d}}t=\int _{-\infty }^{\infty
}f(t){\overline {f(t-\tau )}}\,{\rm {d}}t}]
where        f ( t )  &#x00AF;     {\displaystyle {\overline {f(t)}}}  [
{\displaystyle {\overline {f(t)}}}] represents the complex_conjugate of     f
( t )   {\displaystyle f(t)}  [f(t)]. Note that the parameter     t
{\displaystyle t}  [t] in the integral is a dummy variable and is only
necessary to calculate the integral. It has no specific meaning.
**** Auto-correlation of discrete-time signal[edit] ****
The discrete autocorrelation     R   {\displaystyle R}  [R] at lag     &#x2113;
{\displaystyle \ell }  [\ell ] for a discrete-time signal     y ( n )
{\displaystyle y(n)}  [y(n)] is
    R  y y   ( &#x2113; ) =  &#x2211;  n &#x2208; Z   y ( n )
y ( n &#x2212; &#x2113; )  &#x00AF;     {\displaystyle R_{yy}(\ell    (Eq.7)
)=\sum _{n\in Z}y(n)\,{\overline {y(n-\ell )}}}  [{\displaystyle      
R_{yy}(\ell )=\sum _{n\in Z}y(n)\,{\overline {y(n-\ell )}}}]
The above definitions work for signals that are square integrable, or square
summable, that is, of finite energy. Signals that "last forever" are treated
instead as random processes, in which case different definitions are needed,
based on expected values. For wide-sense-stationary_random_processes, the
autocorrelations are defined as
          R  f f   ( &#x03C4; ) = E &#x2061;  [  f ( t )    f ( t &#x2212;
      &#x03C4; )  &#x00AF;    ]    {\displaystyle R_{ff}(\tau )=\operatorname
      {E} \left[f(t){\overline {f(t-\tau )}}\right]}  [{\displaystyle R_{ff}
      (\tau )=\operatorname {E} \left[f(t){\overline {f(t-\tau )}}\right]}]
          R  y y   ( &#x2113; ) = E &#x2061;  [  y ( n )     y ( n &#x2212;
      &#x2113; )  &#x00AF;    ]  .   {\displaystyle R_{yy}(\ell )=\operatorname
      {E} \left[y(n)\,{\overline {y(n-\ell )}}\right].}  [{\displaystyle R_{yy}
      (\ell )=\operatorname {E} \left[y(n)\,{\overline {y(n-\ell )}}\right].}]
For processes that are not stationary, these will also be functions of     t
{\displaystyle t}  [t], or     n   {\displaystyle n}  [n].
For processes that are also ergodic, the expectation can be replaced by the
limit of a time average. The autocorrelation of an ergodic process is sometimes
defined as or equated to[3]
          R  f f   ( &#x03C4; ) =  lim  T &#x2192; &#x221E;     1 T    &#x222B;
      0   T   f ( t + &#x03C4; )    f ( t )  &#x00AF;      d   t
      {\displaystyle R_{ff}(\tau )=\lim _{T\rightarrow \infty }{\frac {1}
      {T}}\int _{0}^{T}f(t+\tau ){\overline {f(t)}}\,{\rm {d}}t}  [
      {\displaystyle R_{ff}(\tau )=\lim _{T\rightarrow \infty }{\frac {1}
      {T}}\int _{0}^{T}f(t+\tau ){\overline {f(t)}}\,{\rm {d}}t}]
          R  y y   ( &#x2113; ) =  lim  N &#x2192; &#x221E;     1 N    &#x2211;
      n = 0   N &#x2212; 1   y ( n )     y ( n &#x2212; &#x2113; )  &#x00AF;
      .   {\displaystyle R_{yy}(\ell )=\lim _{N\rightarrow \infty }{\frac {1}
      {N}}\sum _{n=0}^{N-1}y(n)\,{\overline {y(n-\ell )}}.}  [{\displaystyle R_
      {yy}(\ell )=\lim _{N\rightarrow \infty }{\frac {1}{N}}\sum _{n=0}^{N-1}y
      (n)\,{\overline {y(n-\ell )}}.}]
These definitions have the advantage that they give sensible well-defined
single-parameter results for periodic functions, even when those functions are
not the output of stationary ergodic processes.
Alternatively, signals that last forever can be treated by a short-time
autocorrelation function analysis, using finite time integrals. (See short-time
Fourier_transform for a related process.)
**** Definition for periodic signals[edit] ****
If     f   {\displaystyle f}  [f] is a continuous periodic functions of period
T   {\displaystyle T}  [T], the integration from     &#x2212; &#x221E;
{\displaystyle -\infty }  [-\infty ] to     &#x221E;   {\displaystyle \infty }
[\infty ] is replaced by integration over any interval     [  t  0   ,  t  0
+ T ]   {\displaystyle [t_{0},t_{0}+T]}  [{\displaystyle [t_{0},t_{0}+T]}] of
length     T   {\displaystyle T}  [T]:
          R  f f   ( &#x03C4; ) &#x225C;  &#x222B;   t  0      t  0   + T   f
      ( t + &#x03C4; )    f ( t )  &#x00AF;    d t   {\displaystyle R_{ff}(\tau
      )\triangleq \int _{t_{0}}^{t_{0}+T}f(t+\tau ){\overline {f(t)}}\,dt}  [
      {\displaystyle R_{ff}(\tau )\triangleq \int _{t_{0}}^{t_{0}+T}f(t+\tau )
      {\overline {f(t)}}\,dt}]
which is equivalent to
          R  f f   ( &#x03C4; ) &#x225C;  &#x222B;   t  0      t  0   + T   f
      ( t )    f ( t &#x2212; &#x03C4; )  &#x00AF;    d t   {\displaystyle R_
      {ff}(\tau )\triangleq \int _{t_{0}}^{t_{0}+T}f(t){\overline {f(t-\tau
      )}}\,dt}  [{\displaystyle R_{ff}(\tau )\triangleq \int _{t_{0}}^{t_
      {0}+T}f(t){\overline {f(t-\tau )}}\,dt}]
**** Properties[edit] ****
In the following, we will describe properties of one-dimensional
autocorrelations only, since most properties are easily transferred from the
one-dimensional case to the multi-dimensional cases. These properties hold for
wide-sense_stationary_processes.[4]
    * A fundamental property of the autocorrelation is symmetry,      R  f f
      ( &#x03C4; ) =  R  f f   ( &#x2212; &#x03C4; )   {\displaystyle R_{ff}
      (\tau )=R_{ff}(-\tau )}  [{\displaystyle R_{ff}(\tau )=R_{ff}(-\tau )}],
      which is easy to prove from the definition. In the continuous case,
      the autocorrelation is an even_function
                R  f f   ( &#x2212; &#x03C4; ) =  R  f f   ( &#x03C4; )
            {\displaystyle R_{ff}(-\tau )=R_{ff}(\tau )\,}  [{\displaystyle R_
            {ff}(-\tau )=R_{ff}(\tau )\,}] when     f   {\displaystyle f}  [f]
            is a real function,
      and the autocorrelation is a Hermitian_function
                R  f f   ( &#x2212; &#x03C4; ) =  R  f f   &#x2217;
            ( &#x03C4; )    {\displaystyle R_{ff}(-\tau )=R_{ff}^{*}(\tau )\,}
            [{\displaystyle R_{ff}(-\tau )=R_{ff}^{*}(\tau )\,}] when     f
            {\displaystyle f}  [f] is a complex_function.
    * The continuous autocorrelation function reaches its peak at the origin,
      where it takes a real value, i.e. for any delay     &#x03C4;
      {\displaystyle \tau }  [\tau ],      |   R  f f   ( &#x03C4; )  |
      &#x2264;  R  f f   ( 0 )   {\displaystyle |R_{ff}(\tau )|\leq R_{ff}(0)}
      [{\displaystyle |R_{ff}(\tau )|\leq R_{ff}(0)}].[1]:p.410 This is a
      consequence of the rearrangement_inequality. The same result holds in the
      discrete case.
    * The autocorrelation of a periodic_function is, itself, periodic with the
      same period.
    * The autocorrelation of the sum of two completely uncorrelated functions
      (the cross-correlation is zero for all     &#x03C4;   {\displaystyle \tau
      }  [\tau ]) is the sum of the autocorrelations of each function
      separately.
    * Since autocorrelation is a specific type of cross-correlation, it
      maintains all the properties of cross-correlation.
    * By using the symbol     &#x2217;   {\displaystyle *}  [*] to represent
      convolution and      g  &#x2212; 1     {\displaystyle g_{-1}}  [g_{-1}]
      is a function which manipulates the function     f   {\displaystyle f}
      [f] and is defined as      g  &#x2212; 1   ( f ) ( t ) = f ( &#x2212; t )
      {\displaystyle g_{-1}(f)(t)=f(-t)}  [{\displaystyle g_{-1}(f)(t)=f(-t)}],
      the definition for      R  f f   ( &#x03C4; )   {\displaystyle R_{ff}
      (\tau )}  [R_{ff}(\tau )] may be written as:
                R  f f   ( &#x03C4; ) = ( f &#x2217;  g  &#x2212; 1   (   f
            &#x00AF;   ) ) ( &#x03C4; )   {\displaystyle R_{ff}(\tau )=(f*g_{-
            1}({\overline {f}}))(\tau )}  [{\displaystyle R_{ff}(\tau )=(f*g_{-
            1}({\overline {f}}))(\tau )}]
***** Multi-dimensional autocorrelation[edit] *****
Multi-dimensional autocorrelation is defined similarly. For example, in three
dimensions the autocorrelation of a square-summable discrete_signal would be
         R ( j , k , &#x2113; ) =  &#x2211;  n , q , r    x  n , q , r     x  n
      &#x2212; j , q &#x2212; k , r &#x2212; &#x2113;     {\displaystyle R
      (j,k,\ell )=\sum _{n,q,r}x_{n,q,r}\,x_{n-j,q-k,r-\ell }}  [{\displaystyle
      R(j,k,\ell )=\sum _{n,q,r}x_{n,q,r}\,x_{n-j,q-k,r-\ell }}].
When mean values are subtracted from signals before computing an
autocorrelation function, the resulting function is usually called an auto-
covariance function.
***** Efficient computation[edit] *****
For data expressed as a discrete sequence, it is frequently necessary to
compute the autocorrelation with high computational_efficiency. A brute force
method based on the signal processing definition      R  x x   ( j ) =
&#x2211;  n    x  n       x &#x00AF;    n &#x2212; j     {\displaystyle R_{xx}
(j)=\sum _{n}x_{n}\,{\overline {x}}_{n-j}}  [R_{xx}(j)=\sum _{n}x_{n}\,
{\overline {x}}_{n-j}] can be used when the signal size is small. For example,
to calculate the autocorrelation of the real signal sequence     x = ( 2 , 3 ,
&#x2212; 1 )   {\displaystyle x=(2,3,-1)}  [{\displaystyle x=(2,3,-1)}] (i.e.
x  0   = 2 ,  x  1   = 3 ,  x  2   = &#x2212; 1   {\displaystyle x_{0}=2,x_
{1}=3,x_{2}=-1}  [{\displaystyle x_{0}=2,x_{1}=3,x_{2}=-1}], and      x  i   =
0   {\displaystyle x_{i}=0}  [x_{i}=0] for all other values of i) by hand, we
first recognize that the definition just given is same as the "usual"
multiplication, but with right shifts, where each vertical addition gives the
autocorrelation for particular lag values:
              2   3   &#x2212; 1     &#x00D7;   2   3   &#x2212; 1
      &#x2212; 2   &#x2212; 3   1       6   9   &#x2212; 3     +     4   6
      &#x2212; 2      &#x2212; 2   3   14   3   &#x2212; 2       {\displaystyle
      {\begin{array}{rrrrrr}&2&3&-1\\\times &2&3&-1\\\hline &-2&-3&1\\&&6&9&-
      3\\+&&&4&6&-2\\\hline &-2&3&14&3&-2\end{array}}}  [{\displaystyle {\begin
      {array}{rrrrrr}&2&3&-1\\\times &2&3&-1\\\hline &-2&-3&1\\&&6&9&-
      3\\+&&&4&6&-2\\\hline &-2&3&14&3&-2\end{array}}}]
Thus the required autocorrelation sequence is      R  x x   = ( &#x2212; 2 , 3
, 14 , 3 , &#x2212; 2 )   {\displaystyle R_{xx}=(-2,3,14,3,-2)}  [
{\displaystyle R_{xx}=(-2,3,14,3,-2)}], where      R  x x   ( 0 ) = 14 ,
{\displaystyle R_{xx}(0)=14,}  [R_{xx}(0)=14,]      R  x x   ( &#x2212; 1 ) =
R  x x   ( 1 ) = 3 ,   {\displaystyle R_{xx}(-1)=R_{xx}(1)=3,}  [{\displaystyle
R_{xx}(-1)=R_{xx}(1)=3,}] and      R  x x   ( &#x2212; 2 ) =  R  x x   ( 2 ) =
&#x2212; 2 ,   {\displaystyle R_{xx}(-2)=R_{xx}(2)=-2,}  [{\displaystyle R_{xx}
(-2)=R_{xx}(2)=-2,}] the autocorrelation for other lag values being zero. In
this calculation we do not perform the carry-over operation during addition as
is usual in normal multiplication. Note that we can halve the number of
operations required by exploiting the inherent symmetry of the autocorrelation.
If the signal happens to be periodic, i.e.     x = ( &#x2026; , 2 , 3 ,
&#x2212; 1 , 2 , 3 , &#x2212; 1 , &#x2026; ) ,   {\displaystyle x=(\ldots
,2,3,-1,2,3,-1,\ldots ),}  [{\displaystyle x=(\ldots ,2,3,-1,2,3,-1,\ldots ),}]
then we get a circular autocorrelation (similar to circular_convolution) where
the left and right tails of the previous autocorrelation sequence will overlap
and give      R  x x   = ( &#x2026; , 14 , 1 , 1 , 14 , 1 , 1 , &#x2026; )
{\displaystyle R_{xx}=(\ldots ,14,1,1,14,1,1,\ldots )}  [{\displaystyle R_{xx}=
(\ldots ,14,1,1,14,1,1,\ldots )}] which has the same period as the signal
sequence     x .   {\displaystyle x.}  [x.] The procedure can be regarded as an
application of the convolution property of z-transform of a discrete signal.
While the brute force algorithm is order n2, several efficient algorithms exist
which can compute the autocorrelation in order n log(n). For example, the
WienerâKhinchin_theorem allows computing the autocorrelation from the raw
data X(t) with two fast_Fourier_transforms (FFT):[5]
              F  R   ( f )    = FFT &#x2061; [ X ( t ) ]     S ( f )    =  F  R
      ( f )  F  R   &#x2217;   ( f )     R ( &#x03C4; )    = IFFT &#x2061; [ S
      ( f ) ]       {\displaystyle {\begin{aligned}F_{R}(f)&=\operatorname
      {FFT} [X(t)]\\S(f)&=F_{R}(f)F_{R}^{*}(f)\\R(\tau )&=\operatorname {IFFT}
      [S(f)]\end{aligned}}}  [{\displaystyle {\begin{aligned}F_{R}
      (f)&=\operatorname {FFT} [X(t)]\\S(f)&=F_{R}(f)F_{R}^{*}(f)\\R(\tau
      )&=\operatorname {IFFT} [S(f)]\end{aligned}}}]
where IFFT denotes the inverse fast_Fourier_transform. The asterisk denotes
complex_conjugate.
Alternatively, a multiple Ï correlation can be performed by using brute force
calculation for low Ï values, and then progressively binning the X(t) data
with a logarithmic density to compute higher values, resulting in the same n
log(n) efficiency, but with lower memory requirements.[6][7]
***** Estimation[edit] *****
For a discrete process with known mean and variance for which we observe     n
{\displaystyle n}  [n] observations     {  X  1   ,   X  2   ,  &#x2026; ,   X
n   }   {\displaystyle \{X_{1},\,X_{2},\,\ldots ,\,X_{n}\}}  [\{X_{1},\,X_
{2},\,\ldots ,\,X_{n}\}], an estimate of the autocorrelation may be obtained as
            R &#x005E;    ( k ) =   1  ( n &#x2212; k )  &#x03C3;  2
      &#x2211;  t = 1   n &#x2212; k   (  X  t   &#x2212; &#x03BC; ) (  X  t +
      k   &#x2212; &#x03BC; )   {\displaystyle {\hat {R}}(k)={\frac {1}{(n-
      k)\sigma ^{2}}}\sum _{t=1}^{n-k}(X_{t}-\mu )(X_{t+k}-\mu )}  [{\hat {R}}
      (k)={\frac {1}{(n-k)\sigma ^{2}}}\sum _{t=1}^{n-k}(X_{t}-\mu )(X_{t+k}-
      \mu )]
for any positive integer     k < n   {\displaystyle k<n}  [k<n]. When the true
mean     &#x03BC;   {\displaystyle \mu }  [\mu ] and variance      &#x03C3;  2
{\displaystyle \sigma ^{2}}  [\sigma ^{2}] are known, this estimate is
unbiased. If the true mean and variance of the process are not known there are
a several possibilities:
    * If     &#x03BC;   {\displaystyle \mu }  [\mu ] and      &#x03C3;  2
      {\displaystyle \sigma ^{2}}  [\sigma ^{2}] are replaced by the standard
      formulae for sample mean and sample variance, then this is a biased
      estimate.
    * A periodogram-based estimate replaces     n &#x2212; k   {\displaystyle
      n-k}  [n-k] in the above formula with     n   {\displaystyle n}  [n].
      This estimate is always biased; however, it usually has a smaller mean
      squared error.[8][9]
    * Other possibilities derive from treating the two portions of data
      {  X  1   ,   X  2   ,  &#x2026; ,   X  n &#x2212; k   }   {\displaystyle
      \{X_{1},\,X_{2},\,\ldots ,\,X_{n-k}\}}  [\{X_{1},\,X_{2},\,\ldots ,\,X_
      {n-k}\}] and     {  X  k + 1   ,   X  k + 2   ,  &#x2026; ,   X  n   }
      {\displaystyle \{X_{k+1},\,X_{k+2},\,\ldots ,\,X_{n}\}}  [\{X_{k+1},\,X_
      {k+2},\,\ldots ,\,X_{n}\}] separately and calculating separate sample
      means and/or sample variances for use in defining the estimate.
The advantage of estimates of the last type is that the set of estimated
autocorrelations, as a function of     k   {\displaystyle k}  [k], then form a
function which is a valid autocorrelation in the sense that it is possible to
define a theoretical process having exactly that autocorrelation. Other
estimates can suffer from the problem that, if they are used to calculate the
variance of a linear combination of the     X   {\displaystyle X}  [X]'s, the
variance calculated may turn out to be negative.
***** Regression analysis[edit] *****
In regression_analysis using time_series_data, autocorrelation in a variable of
interest is typically modeled either with an autoregressive_model (AR), a
moving_average_model (MA), their combination as an autoregressive-moving-
average_model (ARMA), or an extension of the latter called an autoregressive
integrated_moving_average_model (ARIMA). With multiple interrelated data
series, vector_autoregression (VAR) or its extensions are used.
In ordinary_least_squares (OLS), the adequacy of a model specification can be
checked in part by establishing whether there is autocorrelation of the
regression_residuals. Problematic autocorrelation of the errors, which
themselves are unobserved, can generally be detected because it produces
autocorrelation in the observable residuals. (Errors are also known as "error
terms" in econometrics.) Autocorrelation of the errors violates the ordinary
least squares assumption that the error terms are uncorrelated, meaning that
the Gauss_Markov_theorem does not apply, and that OLS estimators are no longer
the Best Linear Unbiased Estimators (BLUE). While it does not bias the OLS
coefficient estimates, the standard_errors tend to be underestimated (and the
t-scores overestimated) when the autocorrelations of the errors at low lags are
positive.
The traditional test for the presence of first-order autocorrelation is the
DurbinâWatson_statistic or, if the explanatory variables include a lagged
dependent variable, Durbin's_h_statistic. The Durbin-Watson can be linearly
mapped however to the Pearson correlation between values and their lags.[10] A
more flexible test, covering autocorrelation of higher orders and applicable
whether or not the regressors include lags of the dependent variable, is the
BreuschâGodfrey_test. This involves an auxiliary regression, wherein the
residuals obtained from estimating the model of interest are regressed on (a)
the original regressors and (b) k lags of the residuals, where 'k' is the order
of the test. The simplest version of the test statistic from this auxiliary
regression is TR2, where T is the sample size and R2 is the coefficient_of
determination. Under the null hypothesis of no autocorrelation, this statistic
is asymptotically distributed as      &#x03C7;  2     {\displaystyle \chi ^{2}}
[\chi ^{2}] with k degrees of freedom.
Responses to nonzero autocorrelation include generalized_least_squares and the
NeweyâWest_HAC_estimator (Heteroskedasticity and Autocorrelation Consistent).
[11]
In the estimation of a moving_average_model (MA), the autocorrelation function
is used to determine the appropriate number of lagged error terms to be
included. This is based on the fact that for an MA process of order q, we have
R ( &#x03C4; ) &#x2260; 0   {\displaystyle R(\tau )\neq 0}  [{\displaystyle R
(\tau )\neq 0}], for     &#x03C4; = 0 , 1 , &#x2026; , q   {\displaystyle \tau
=0,1,\ldots ,q}  [{\displaystyle \tau =0,1,\ldots ,q}], and     R ( &#x03C4; )
= 0   {\displaystyle R(\tau )=0}  [{\displaystyle R(\tau )=0}], for
&#x03C4; > q   {\displaystyle \tau >q}  [{\displaystyle \tau >q}].
***** Applications[edit] *****
    * Autocorrelation analysis is used heavily in fluorescence_correlation
      spectroscopy.
    * Another application of autocorrelation is the measurement of optical
      spectra and the measurement of very-short-duration light pulses produced
      by lasers, both using optical_autocorrelators.
    * Autocorrelation is used to analyze dynamic_light_scattering data, which
      notably enables determination of the particle_size_distributions of
      nanometer-sized particles or micelles suspended in a fluid. A laser
      shining into the mixture produces a speckle_pattern that results from the
      motion of the particles. Autocorrelation of the signal can be analyzed in
      terms of the diffusion of the particles. From this, knowing the viscosity
      of the fluid, the sizes of the particles can be calculated.
    * The small-angle_X-ray_scattering intensity of a nanostructured system is
      the Fourier transform of the spatial autocorrelation function of the
      electron density.
    * In optics, normalized autocorrelations and cross-correlations give the
      degree_of_coherence of an electromagnetic field.
    * In signal_processing, autocorrelation can give information about
      repeating events like musical beats (for example, to determine tempo) or
      pulsar frequencies, though it cannot tell the position in time of the
      beat. It can also be used to estimate_the_pitch_of_a_musical_tone.
    * In music_recording, autocorrelation is used as a pitch_detection
      algorithm prior to vocal processing, as a distortion effect or to
      eliminate undesired mistakes and inaccuracies.[12]
    * Autocorrelation in space rather than time, via the Patterson_function, is
      used by X-ray diffractionists to help recover the "Fourier phase
      information" on atom positions not available through diffraction alone.
    * In statistics, spatial autocorrelation between sample locations also
      helps one estimate mean_value_uncertainties when sampling a heterogeneous
      population.
    * The SEQUEST algorithm for analyzing mass_spectra makes use of
      autocorrelation in conjunction with cross-correlation to score the
      similarity of an observed spectrum to an idealized spectrum representing
      a peptide.
    * In astrophysics, autocorrelation is used to study and characterize the
      spatial distribution of galaxies in the universe and in multi-wavelength
      observations of low mass X-ray_binaries.
    * In panel_data, spatial autocorrelation refers to correlation of a
      variable with itself through space.
    * In analysis of Markov_chain_Monte_Carlo data, autocorrelation must be
      taken into account for correct error determination.
    * In geosciences (specifically in geophysics) it can be used to compute an
      autocorrelation seismic attribute, out of a 3D seismic survey of the
      underground.
    * In medical_ultrasound imaging, autocorrelation is used to visualize blood
      flow.
    * In intertemporal_portfolio_choice, the presence or absence of
      autocorrelation in an asset's rate_of_return can affect the optimal
      portion of the portfolio to hold in that asset.
***** Serial dependence[edit] *****
Serial dependence is closely linked to the notion of autocorrelation, but
represents a distinct concept (see Correlation_and_dependence). In particular,
it is possible to have serial dependence but no (linear) correlation. In some
fields however, the two terms are used as synonyms.
A time_series of a random_variable has serial dependence if the value at some
time     t   {\displaystyle t}  [t] in the series is statistically_dependent on
the value at another time     s   {\displaystyle s}  [s]. A series is serially
independent if there is no dependence between any pair.
If a time series      {  X  t   }    {\displaystyle \left\{X_{t}\right\}}  [
{\displaystyle \left\{X_{t}\right\}}] is stationary, then statistical
dependence between the pair     (  X  t   ,  X  s   )   {\displaystyle (X_
{t},X_{s})}  [{\displaystyle (X_{t},X_{s})}] would imply that there is
statistical dependence between all pairs of values at the same lag     &#x03C4;
= s &#x2212; t   {\displaystyle \tau =s-t}  [{\displaystyle \tau =s-t}].
***** See also[edit] *****
    * Autocorrelation_matrix
    * Autocorrelation_technique
    * Autocorrelation_of_a_formal_word
    * Autocorrelator
    * Correlation_function
    * Correlogram
    * Cross-correlation
    * Galton's_problem
    * Partial_autocorrelation_function
    * Fluorescence_correlation_spectroscopy
    * Optical_autocorrelation
    * Pitch_detection_algorithm
    * Triple_correlation
    * Variance
    * CUSUM
    * CochraneâOrcutt_estimation (transformation for autocorrelated error
      terms)
    * PraisâWinsten_transformation
    * Scaled_Correlation
    * Unbiased_estimation_of_standard_deviation
***** References[edit] *****
   1. ^ a b c d e fGubner, John A. (2006). Probability and Random Processes for
      Electrical and Computer Engineers. Cambridge University Press. ISBN 978-
      0-521-86470-1.
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
   3. ^ a b c d e f Kun Il Park, Fundamentals of Probability and Stochastic
      Processes with Applications to Communications, Springer, 2018,
   4. ISBN 978-3-319-68074-3
   5. ^ a bDunn, Patrick F. (2005). Measurement and Data Analysis for
      Engineering and Science. New York: McGrawâHill. ISBN 978-0-07-282538-1.
   6. ^Proakis, John (August 31, 2001). Communication Systems Engineering (2nd
      Edition) (2 ed.). Pearson. p. 168. ISBN 978-0130617934.
   7. ^Box, G. E. P.; Jenkins, G. M.; Reinsel, G. C. (1994). Time Series
      Analysis: Forecasting and Control (3rd ed.). Upper Saddle River, NJ:
      PrenticeâHall. ISBN 978-0130607744.
   8. [page needed]
   9. ^Frenkel, D.; Smit, B. (2002). "chap. 4.4.2". Understanding Molecular
      Simulation (2nd ed.). London: Academic Press. ISBN 978-0122673511.
  10. ^Colberg, P.; HÃ¶fling, F. (2011). "Highly accelerated simulations of
      glassy dynamics using GPUs: caveats on limited floating-point precision".
      Comp._Phys._Comm. 182 (5): 1120â1129. arXiv:0912.3824. Bibcode:
      2011CoPhC.182.1120C. doi:10.1016/j.cpc.2011.01.009.
  11. ^Priestley, M. B. (1982). Spectral analysis and time series. London, New
      York: Academic Press. ISBN 978-0125649018.
  12. ^Percival, Donald B.; Andrew T. Walden (1993). Spectral Analysis for
      Physical Applications: Multitaper and Conventional Univariate Techniques.
      Cambridge University Press. pp. 190â195. ISBN 978-0-521-43541-3.
  13. ^"Serial_correlation_techniques". Statistical Ideas. 26 May 2014.
  14. ^Baum, Christopher F. (2006). An Introduction to Modern Econometrics
      Using Stata. Stata Press. ISBN 978-1-59718-013-9.
  15. ^Tyrangiel, Josh (2009-02-05). "Auto-Tune:_Why_Pop_Music_Sounds_Perfect".
      Time Magazine.
***** Further reading[edit] *****
    * Kmenta,_Jan (1986). Elements of Econometrics (Second ed.). New York:
      Macmillan. pp. 298â334. ISBN 978-0-02-365070-3.
Marno Verbeek (10 August 2017). A_Guide_to_Modern_Econometrics. Wiley.
ISBN 978-1-119-40110-0.
Mojtaba Soltanalian, and Petre Stoica. "Computational_design_of_sequences_with
good_correlation_properties." IEEE Transactions on Signal Processing, 60.5
(2012): 2180â2193.
Solomon W. Golomb, and Guang Gong. Signal_design_for_good_correlation:_for
wireless_communication,_cryptography,_and_radar. Cambridge University Press,
2005.
***** External links[edit] *****
    * Weisstein,_Eric_W. "Autocorrelation". MathWorld.
Autocorrelation_articles_in_Comp.DSP_(DSP_usenet_group).
GPU_accelerated_calculation_of_autocorrelation_function.
Econometrics_lecture_(topic:_autocorrelation) on YouTube by Mark_Thoma
Autocorrelation_Time_Series_data_by_itfeature
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
                                  * Autocorrelation (ACF)
                                        o partial_(PACF)
                                  * Cross-correlation_(XCF)
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

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Autocorrelation&oldid=907260569"
Categories:
    * Autocorrelation
    * Signal_processing
    * Time_domain_analysis
Hidden categories:
    * Wikipedia_articles_needing_page_number_citations_from_March_2013
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * Bahasa_Indonesia
    * Italiano
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Basa_Sunda
    * Suomi
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 21 July 2019, at 17:31 (UTC).
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
