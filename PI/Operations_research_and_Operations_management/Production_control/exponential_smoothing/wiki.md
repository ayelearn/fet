The following text has been accessed from https://en.wikipedia.org/wiki/Exponential_smoothing at Fri Aug 9 03:46:15 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Exponential smoothing ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Generates a forecast of future values of a time series
Exponential smoothing is a rule_of_thumb technique for smoothing time_series
data using the exponential window_function. Whereas in the simple_moving
average the past observations are weighted equally, exponential functions are
used to assign exponentially decreasing weights over time. It is an easily
learned and easily applied procedure for making some determination based on
prior assumptions by the user, such as seasonality. Exponential smoothing is
often used for analysis of time-series data.
Exponential smoothing is one of many window_functions commonly applied to
smooth data in signal_processing, acting as low-pass_filters to remove high
frequency noise. This method is preceded by Poisson's use of recursive
exponential window functions in convolutions from the 19th century, as well as
Kolmogorov_and_Zurbenko's_use_of_recursive_moving_averages from their studies
of turbulence in the 1940s.
The raw data sequence is often represented by     {  x  t   }   {\displaystyle
\{x_{t}\}}  [\{x_{t}\}] beginning at time     t = 0   {\displaystyle t=0}
[t=0], and the output of the exponential smoothing algorithm is commonly
written as     {  s  t   }   {\displaystyle \{s_{t}\}}  [\{s_{t}\}], which may
be regarded as a best estimate of what the next value of     x   {\displaystyle
x}  [x] will be. When the sequence of observations begins at time     t = 0
{\displaystyle t=0}  [t=0], the simplest form of exponential smoothing is given
by the formulas:[1]
        s  0      =  x  0        s  t      = &#x03B1;  x  t   + ( 1 &#x2212;
&#x03B1; )  s  t &#x2212; 1   , &#xA0; t > 0       {\displaystyle {\begin
{aligned}s_{0}&=x_{0}\\s_{t}&=\alpha x_{t}+(1-\alpha )s_{t-1},\ t>0\end
{aligned}}}  [{\begin{aligned}s_{0}&=x_{0}\\s_{t}&=\alpha x_{t}+(1-\alpha )s_
{t-1},\ t>0\end{aligned}}]
where     &#x03B1;   {\displaystyle \alpha }  [\alpha ] is the smoothing
factor, and     0 < &#x03B1; < 1   {\displaystyle 0<\alpha <1}  [0<\alpha <1].
⁰
***** Contents *****
    * 1_Basic_exponential_smoothing
          o 1.1_Time_Constant
          o 1.2_Choosing_the_initial_smoothed_value
          o 1.3_Optimization
          o 1.4_âExponentialâ_naming
          o 1.5_Comparison_with_moving_average
    * 2_Double_exponential_smoothing
    * 3_Triple_exponential_smoothing
    * 4_Implementations_in_statistics_packages
    * 5_See_also
    * 6_Notes
    * 7_External_links
***** Basic exponential smoothing[edit] *****
The use of the exponential window function is first attributed to Poisson[2] as
an extension of a numerical analysis technique from the 17th century, and later
adopted by the signal_processing community in the 1940s. Here, exponential
smoothing is the application of the exponential, or Poisson, window_function.
Exponential smoothing was first suggested in the statistical literature without
citation to previous work by Robert_Goodell_Brown in 1956,[3] and then expanded
by Charles_C._Holt in 1957.[4] The formulation below, which is the one commonly
used, is attributed to Brown and is known as âBrownâs simple exponential
smoothingâ.[5] All the methods of Holt, Winters and Brown may be seen as a
simple application of recursive filtering, first found in the 1940s[2] to
convert FIR_filters to IIR_filters.
The simplest form of exponential smoothing is given by the formula:
          s  t   = &#x03B1; &#x22C5;  x  t   + ( 1 &#x2212; &#x03B1; ) &#x22C5;
      s  t &#x2212; 1   =  s  t &#x2212; 1   + &#x03B1; &#x22C5; (  x  t
      &#x2212;  s  t &#x2212; 1   )   {\displaystyle s_{t}=\alpha \cdot x_{t}+
      (1-\alpha )\cdot s_{t-1}=s_{t-1}+\alpha \cdot (x_{t}-s_{t-1})}  [
      {\displaystyle s_{t}=\alpha \cdot x_{t}+(1-\alpha )\cdot s_{t-1}=s_{t-
      1}+\alpha \cdot (x_{t}-s_{t-1})}].
where Î± is the smoothing factor, and 0 < Î± < 1. In other words, the smoothed
statistic st' is a simple weighted average of the current observation xt and
the previous smoothed statistic stâ1. The term smoothing factor applied to Î±
here is something of a misnomer, as larger values of Î± actually reduce the
level of smoothing, and in the limiting case with Î± = 1 the output series is
just the current observation. Simple exponential smoothing is easily applied,
and it produces a smoothed statistic as soon as two observations are available.
Values of Î± close to one have less of a smoothing effect and give greater
weight to recent changes in the data, while values of Î± closer to zero have a
greater smoothing effect and are less responsive to recent changes. There is no
formally correct procedure for choosing Î±. Sometimes the statistician's
judgment is used to choose an appropriate factor. Alternatively, a statistical
technique may be used to optimize the value of Î±. For example, the method_of
least_squares might be used to determine the value of Î± for which the sum of
the quantities     (  s  t   &#x2212;  x  t + 1    )  2     {\displaystyle (s_
{t}-x_{t+1})^{2}}  [{\displaystyle (s_{t}-x_{t+1})^{2}}] is minimized.[6]
Unlike some other smoothing methods, such as the simple moving average, this
technique does not require any minimum number of observations to be made before
it begins to produce results. In practice, however, a âgood averageâ will
not be achieved until several samples have been averaged together; for example,
a constant signal will take approximately 3/Î± stages to reach 95% of the
actual value. To accurately reconstruct the original signal without information
loss all stages of the exponential moving average must also be available,
because older samples decay in weight exponentially. This is in contrast to a
simple moving average, in which some samples can be skipped without as much
loss of information due to the constant weighting of samples within the
average. If a known number of samples will be missed, one can adjust a weighted
average for this as well, by giving equal weight to the new sample and all
those to be skipped.
This simple form of exponential smoothing is also known as an exponentially
weighted_moving_average (EWMA). Technically it can also be classified as an
autoregressive_integrated_moving_average (ARIMA) (0,1,1) model with no constant
term.[7]
**** Time Constant[edit] ****
The time_constant of an exponential moving average is the amount of time for
the smoothed response of a unit set function to reach     1 &#x2212; 1  /  e
&#x2248; 63.2  &#x0025;   {\displaystyle 1-1/e\approx 63.2\,\%}  [1-1/e\approx
63.2\,\%] of the original signal. The relationship between this time constant,
&#x03C4;   {\displaystyle \tau }  [\tau ], and the smoothing factor,
&#x03B1;   {\displaystyle \alpha }  [\alpha ], is given by the formula:
         &#x03B1; = 1 &#x2212;  e    &#x2212; &#x0394; T  &#x03C4;
      {\displaystyle \alpha =1-e^{-\Delta T \over \tau }}  [\alpha =1-e^{-
      \Delta T \over \tau }]
Where     &#x0394; T   {\displaystyle \Delta T}  [\Delta T] is the sampling
time interval of the discrete time implementation. If the sampling time is fast
compared to the time constant (    &#x0394; T &#x226A; &#x03C4;
{\displaystyle \Delta T\ll \tau }  [{\displaystyle \Delta T\ll \tau }]) then
         &#x03B1; &#x2248;    &#x0394; T  &#x03C4;     {\displaystyle \alpha
      \approx {\Delta T \over \tau }}  [{\displaystyle \alpha \approx {\Delta T
      \over \tau }}]
**** Choosing the initial smoothed value[edit] ****
Note that in the definition above, s0 is being initialized to x0. Because
exponential smoothing requires that at each stage we have the previous
forecast, it is not obvious how to get the method started. We could assume that
the initial forecast is equal to the initial value of demand; however, this
approach has a serious drawback. Exponential smoothing puts substantial weight
on past observations, so the initial value of demand will have an unreasonably
large effect on early forecasts. This problem can be overcome by allowing the
process to evolve for a reasonable number of periods (10 or more) and using the
average of the demand during those periods as the initial forecast. There are
many other ways of setting this initial value, but it is important to note that
the smaller the value of Î±, the more sensitive your forecast will be on the
selection of this initial smoother value s1.[8]
**** Optimization[edit] ****
For every exponential smoothing method we also need to choose the value for the
smoothing parameters. For simple exponential smoothing, there is only one
smoothing parameter (Î±), but for the methods that follow there is usually more
than one smoothing parameter.
There are cases where the smoothing parameters may be chosen in a subjective
manner â the forecaster specifies the value of the smoothing parameters based
on previous experience. However, a more robust and objective way to obtain
values for the unknown parameters included in any exponential smoothing method
is to estimate them from the observed data.
The unknown parameters and the initial values for any exponential smoothing
method can be estimated by minimizing the sum_of_squared_errors (SSE). The
errors are specified as      e  t   =  y  t   &#x2212;     y &#x005E;     t  |
t &#x2212; 1     {\displaystyle e_{t}=y_{t}-{\hat {y}}_{t|t-1}}  [
{\displaystyle e_{t}=y_{t}-{\hat {y}}_{t|t-1}}] for t=1,...,T (the one-step-
ahead within-sample forecast errors). Hence we find the values of the unknown
parameters and the initial values that minimize
   S S E =  &#x2211;  t = 1   T   (  y  t   &#x2212;     y &#x005E;     t  |  t
&#x2212; 1    )  2   =  &#x2211;  t = 1   T    e  t   2     {\displaystyle
SSE=\sum _{t=1}^{T}(y_{t}-{\hat {y}}_{t|t-1})^{2}=\sum _{t=1}^{T}e_{t}^{2}}  [
{\displaystyle SSE=\sum _{t=1}^{T}(y_{t}-{\hat {y}}_{t|t-1})^{2}=\sum _{t=1}^
{T}e_{t}^{2}}] [9]
Unlike the regression case (where we have formulae to directly compute the
regression coefficients which minimize the SSE) this involves a non-linear
minimization problem and we need to use an optimization tool to perform this.
**** âExponentialâ naming[edit] ****
The name 'exponential smoothing' is attributed to the use of the exponential
window function during convolution. It is no longer attributed to Holt, Winters
& Brown.
By direct substitution of the defining equation for simple exponential
smoothing back into itself we find that
              s  t      = &#x03B1;  x  t   + ( 1 &#x2212; &#x03B1; )  s  t
      &#x2212; 1         = &#x03B1;  x  t   + &#x03B1; ( 1 &#x2212; &#x03B1; )
      x  t &#x2212; 1   + ( 1 &#x2212; &#x03B1;  )  2    s  t &#x2212; 2
      = &#x03B1;  [   x  t   + ( 1 &#x2212; &#x03B1; )  x  t &#x2212; 1   + ( 1
      &#x2212; &#x03B1;  )  2    x  t &#x2212; 2   + ( 1 &#x2212; &#x03B1;  )
      3    x  t &#x2212; 3   + &#x22EF; + ( 1 &#x2212; &#x03B1;  )  t &#x2212;
      1    x  1    ]  + ( 1 &#x2212; &#x03B1;  )  t    x  0   .
      {\displaystyle {\begin{aligned}s_{t}&=\alpha x_{t}+(1-\alpha )s_{t-1}\\
      [3pt]&=\alpha x_{t}+\alpha (1-\alpha )x_{t-1}+(1-\alpha )^{2}s_{t-2}\\
      [3pt]&=\alpha \left[x_{t}+(1-\alpha )x_{t-1}+(1-\alpha )^{2}x_{t-2}+(1-
      \alpha )^{3}x_{t-3}+\cdots +(1-\alpha )^{t-1}x_{1}\right]+(1-\alpha )^
      {t}x_{0}.\end{aligned}}}  [{\displaystyle {\begin{aligned}s_{t}&=\alpha
      x_{t}+(1-\alpha )s_{t-1}\\[3pt]&=\alpha x_{t}+\alpha (1-\alpha )x_{t-1}+
      (1-\alpha )^{2}s_{t-2}\\[3pt]&=\alpha \left[x_{t}+(1-\alpha )x_{t-1}+(1-
      \alpha )^{2}x_{t-2}+(1-\alpha )^{3}x_{t-3}+\cdots +(1-\alpha )^{t-1}x_
      {1}\right]+(1-\alpha )^{t}x_{0}.\end{aligned}}}]
In other words, as time passes the smoothed statistic st becomes the weighted
average of a greater and greater number of the past observations xtân, and
the weights assigned to previous observations are in general proportional to
the terms of the geometric progression {1, (1 â Î±), (1 â Î±)2, 
(1 â Î±)3, ...}. A geometric_progression is the discrete version of an
exponential_function, so this is where the name for this smoothing method
originated according to Statistics lore.
**** Comparison with moving average[edit] ****
Exponential smoothing and moving average have similar defects of introducing a
lag relative to the input data. While this can be corrected by shifting the
result by half the window length for a symmetrical kernel, such as a moving
average or gaussian, it is unclear how appropriate this would be for
exponential smoothing. They also both have roughly the same distribution of
forecast error when Î± = 2/(k+1). They differ in that exponential smoothing
takes into account all past data, whereas moving average only takes into
account k past data points. Computationally speaking, they also differ in that
moving average requires that the past k data points, or the data point at lag
k+1 plus the most recent forecast value, to be kept, whereas exponential
smoothing only needs the most recent forecast value to be kept.[10]
In the signal_processing literature, the use of non-causal (symmetric) filters
is commonplace, and the exponential window_function is broadly used in this
fashion, but a different terminology is used: exponential smoothing is
equivalent to a first-order Infinite Impulse Response or IIR_filter and moving
average is equivalent to a Finite Impulse Response or FIR_filter with equal
weighting factors.
***** Double exponential smoothing[edit] *****
Simple exponential smoothing does not do well when there is a trend in the
data, which is inconvenient.[1] In such situations, several methods were
devised under the name "double exponential smoothing" or "second-order
exponential smoothing.", which is the recursive application of an exponential
filter twice, thus being termed "double exponential smoothing". This
nomenclature is similar to quadruple exponential smoothing, which also
references its recursion depth.[11] The basic idea behind double exponential
smoothing is to introduce a term to take into account the possibility of a
series exhibiting some form of trend. This slope component is itself updated
via exponential smoothing.
One method, sometimes referred to as "Holt-Winters double exponential
smoothing" works as follows:[12]
Again, the raw data sequence of observations is represented by {xt}, beginning
at time t = 0. We use {st} to represent the smoothed value for time t, and {bt}
is our best estimate of the trend at time t. The output of the algorithm is now
written as Ft+m, an estimate of the value of x at time t + m for m > 0 based on
the raw data up to time t. Double exponential smoothing is given by the
formulas
              s  1      =  x  1        b  1      =  x  1   &#x2212;  x  0
      {\displaystyle {\begin{aligned}s_{1}&=x_{1}\\b_{1}&=x_{1}-x_{0}\\\end
      {aligned}}}  [{\begin{aligned}s_{1}&=x_{1}\\b_{1}&=x_{1}-x_{0}\\\end
      {aligned}}]
And for t > 1 by
              s  t      = &#x03B1;  x  t   + ( 1 &#x2212; &#x03B1; ) (  s  t
      &#x2212; 1   +  b  t &#x2212; 1   )      b  t      = &#x03B2; (  s  t
      &#x2212;  s  t &#x2212; 1   ) + ( 1 &#x2212; &#x03B2; )  b  t &#x2212; 1
      {\displaystyle {\begin{aligned}s_{t}&=\alpha x_{t}+(1-\alpha )(s_{t-1}+b_
      {t-1})\\b_{t}&=\beta (s_{t}-s_{t-1})+(1-\beta )b_{t-1}\\\end{aligned}}}
      [{\begin{aligned}s_{t}&=\alpha x_{t}+(1-\alpha )(s_{t-1}+b_{t-1})\\b_
      {t}&=\beta (s_{t}-s_{t-1})+(1-\beta )b_{t-1}\\\end{aligned}}]
where Î± is the data smoothing factor, 0 < Î± < 1, and Î² is the trend
smoothing factor, 0 < Î² < 1.
To forecast beyond xt
              F  t + m      =  s  t   + m  b  t         {\displaystyle {\begin
      {aligned}F_{t+m}&=s_{t}+mb_{t}\end{aligned}}}  [{\begin{aligned}F_
      {t+m}&=s_{t}+mb_{t}\end{aligned}}]
Setting the initial value b0 is a matter of preference. An option other than
the one listed above is (xn - x0)/n for some n > 1.
Note that F0 is undefined (there is no estimation for time 0), and according to
the definition F1=s0+b0, which is well defined, thus further values can be
evaluated.
A second method, referred to as either Brown's linear exponential smoothing
(LES) or Brown's double exponential smoothing works as follows.[13]
              s  0  &#x2032;     =  x  0        s  0  &#x2033;     =  x  0
      s  t  &#x2032;     = &#x03B1;  x  t   + ( 1 &#x2212; &#x03B1; )  s  t
      &#x2212; 1  &#x2032;       s  t  &#x2033;     = &#x03B1;  s  t  &#x2032;
      + ( 1 &#x2212; &#x03B1; )  s  t &#x2212; 1  &#x2033;       F  t + m
      =  a  t   + m  b  t   ,       {\displaystyle {\begin{aligned}s'_{0}&=x_
      {0}\\s''_{0}&=x_{0}\\s'_{t}&=\alpha x_{t}+(1-\alpha )s'_{t-1}\\s''_
      {t}&=\alpha s'_{t}+(1-\alpha )s''_{t-1}\\F_{t+m}&=a_{t}+mb_{t},\end
      {aligned}}}  [{\begin{aligned}s'_{0}&=x_{0}\\s''_{0}&=x_{0}\\s'_
      {t}&=\alpha x_{t}+(1-\alpha )s'_{t-1}\\s''_{t}&=\alpha s'_{t}+(1-\alpha
      )s''_{t-1}\\F_{t+m}&=a_{t}+mb_{t},\end{aligned}}]
where at, the estimated level at time t and bt, the estimated trend at time t
are:
              a  t      = 2  s  t  &#x2032;  &#x2212;  s  t  &#x2033;       b
      t      =   &#x03B1;  1 &#x2212; &#x03B1;    (  s  t  &#x2032;  &#x2212;
      s  t  &#x2033;  ) .       {\displaystyle {\begin{aligned}a_{t}&=2s'_{t}-
      s''_{t}\\b_{t}&={\frac {\alpha }{1-\alpha }}(s'_{t}-s''_{t}).\end
      {aligned}}}  [{\begin{aligned}a_{t}&=2s'_{t}-s''_{t}\\b_{t}&={\frac
      {\alpha }{1-\alpha }}(s'_{t}-s''_{t}).\end{aligned}}]
***** Triple exponential smoothing[edit] *****
Triple exponential smoothing applies exponential smoothing three times, which
is commonly used when there are three high frequency signals to be removed from
a time series under study. There are different types of seasonality:
'multiplicative' and 'additive' in nature, much like addition and
multiplication are basic operations in mathematics.
If every month of December we sell 10,000 more apartments than we do in
November the seasonality is additive in nature. However, if we sell 10% more
apartments in the summer months than we do in the winter months the seasonality
is multiplicative in nature. Multiplicative seasonality can be represented as a
constant factor, not an absolute amount. [14]
Triple exponential smoothing was first suggested by Holt's student, Peter
Winters, in 1960 after reading a signal processing book from the 1940s on
exponential smoothing.[15] Holt's novel idea was to repeat filtering an odd
number of times greater than 1 and less than 5, which was popular with scholars
of previous eras.[15] While recursive filtering had been used previously, it
was applied twice and four times to coincide with the Hadamard_conjecture,
while triple application required more than double the operations of singular
convolution. The use of a triple application is considered a rule_of_thumb
technique, rather than one based on theoretical foundations and has often been
over-emphasized by practitioners.
Suppose we have a sequence of observations {xt}, beginning at time t = 0 with a
cycle of seasonal change of length L.
The method calculates a trend line for the data as well as seasonal indices
that weight the values in the trend line based on where that time point falls
in the cycle of length L.
{st} represents the smoothed value of the constant part for time t. {bt}
represents the sequence of best estimates of the linear trend that are
superimposed on the seasonal changes. {ct} is the sequence of seasonal
correction factors. ct is the expected proportion of the predicted trend at any
time t mod L in the cycle that the observations take on. As a rule of thumb, a
minimum of two full seasons (or 2L periods) of historical data is needed to
initialize a set of seasonal factors.
The output of the algorithm is again written as Ft+m, an estimate of the value
of x at time t+m, m>0 based on the raw data up to time t. Triple exponential
smoothing with multiplicative seasonality is given by the formulas[1]
              s  0      =  x  0        s  t      = &#x03B1;    x  t    c  t
      &#x2212; L     + ( 1 &#x2212; &#x03B1; ) (  s  t &#x2212; 1   +  b  t
      &#x2212; 1   )      b  t      = &#x03B2; (  s  t   &#x2212;  s  t
      &#x2212; 1   ) + ( 1 &#x2212; &#x03B2; )  b  t &#x2212; 1        c  t
      = &#x03B3;    x  t    s  t     + ( 1 &#x2212; &#x03B3; )  c  t &#x2212; L
      F  t + m      = (  s  t   + m  b  t   )  c  t &#x2212; L + 1 + ( m
      &#x2212; 1 )  mod   L   ,       {\displaystyle {\begin{aligned}s_{0}&=x_
      {0}\\s_{t}&=\alpha {\frac {x_{t}}{c_{t-L}}}+(1-\alpha )(s_{t-1}+b_{t-
      1})\\b_{t}&=\beta (s_{t}-s_{t-1})+(1-\beta )b_{t-1}\\c_{t}&=\gamma {\frac
      {x_{t}}{s_{t}}}+(1-\gamma )c_{t-L}\\F_{t+m}&=(s_{t}+mb_{t})c_{t-L+1+(m-
      1)\mod L},\end{aligned}}}  [{\begin{aligned}s_{0}&=x_{0}\\s_{t}&=\alpha
      {\frac {x_{t}}{c_{t-L}}}+(1-\alpha )(s_{t-1}+b_{t-1})\\b_{t}&=\beta (s_
      {t}-s_{t-1})+(1-\beta )b_{t-1}\\c_{t}&=\gamma {\frac {x_{t}}{s_{t}}}+(1-
      \gamma )c_{t-L}\\F_{t+m}&=(s_{t}+mb_{t})c_{t-L+1+(m-1)\mod L},\end
      {aligned}}]
where Î± is the data smoothing factor, 0 < Î± < 1, Î² is the trend smoothing
factor, 0 < Î² < 1, and Î³ is the seasonal change smoothing factor, 0 < Î³ < 1.
The general formula for the initial trend estimate b0 is:
              b  0      =   1 L    (      x  L + 1   &#x2212;  x  1    L   +
      x  L + 2   &#x2212;  x  2    L   + &#x2026; +     x  L + L   &#x2212;  x
      L    L    )        {\displaystyle {\begin{aligned}b_{0}&={\frac {1}
      {L}}\left({\frac {x_{L+1}-x_{1}}{L}}+{\frac {x_{L+2}-x_{2}}{L}}+\ldots +
      {\frac {x_{L+L}-x_{L}}{L}}\right)\end{aligned}}}  [{\begin{aligned}b_
      {0}&={\frac {1}{L}}\left({\frac {x_{L+1}-x_{1}}{L}}+{\frac {x_{L+2}-x_
      {2}}{L}}+\ldots +{\frac {x_{L+L}-x_{L}}{L}}\right)\end{aligned}}]
Setting the initial estimates for the seasonal indices ci for i = 1,2,...,L is
a bit more involved. If N is the number of complete cycles present in your
data, then:
                 c  i      =   1 N    &#x2211;  j = 1   N      x  L ( j
      &#x2212; 1 ) + i    A  j      &#x2200; i   = 1 , 2 , &#x2026; , L
      {\displaystyle {\begin{aligned}\\c_{i}&={\frac {1}{N}}\sum _{j=1}^{N}
      {\frac {x_{L(j-1)+i}}{A_{j}}}\quad \forall i&=1,2,\ldots ,L\\\end
      {aligned}}}  [{\begin{aligned}\\c_{i}&={\frac {1}{N}}\sum _{j=1}^{N}
      {\frac {x_{L(j-1)+i}}{A_{j}}}\quad \forall i&=1,2,\ldots ,L\\\end
      {aligned}}]
where
              A  j      =     &#x2211;  i = 1   L    x  L ( j &#x2212; 1 ) + i
      L    &#x2200; j   = 1 , 2 , &#x2026; , N       {\displaystyle {\begin
      {aligned}A_{j}&={\frac {\sum _{i=1}^{L}x_{L(j-1)+i}}{L}}\quad \forall
      j&=1,2,\ldots ,N\end{aligned}}}  [{\begin{aligned}A_{j}&={\frac {\sum _
      {i=1}^{L}x_{L(j-1)+i}}{L}}\quad \forall j&=1,2,\ldots ,N\end{aligned}}]
Note that Aj is the average value of x in the jth cycle of your data.
Triple exponential smoothing with additive seasonality is given by:
        s  0      =  x  0        s  t      = &#x03B1; (  x  t   &#x2212;  c  t
&#x2212; L   ) + ( 1 &#x2212; &#x03B1; ) (  s  t &#x2212; 1   +  b  t &#x2212;
1   )      b  t      = &#x03B2; (  s  t   &#x2212;  s  t &#x2212; 1   ) + ( 1
&#x2212; &#x03B2; )  b  t &#x2212; 1        c  t      = &#x03B3; (  x  t
&#x2212;  s  t &#x2212; 1   &#x2212;  b  t &#x2212; 1   ) + ( 1 &#x2212;
&#x03B3; )  c  t &#x2212; L        F  t + m      =  s  t   + m  b  t   +  c  t
&#x2212; L + 1 + ( m &#x2212; 1 )  mod   L   ,       {\displaystyle {\begin
{aligned}s_{0}&=x_{0}\\s_{t}&=\alpha (x_{t}-c_{t-L})+(1-\alpha )(s_{t-1}+b_{t-
1})\\b_{t}&=\beta (s_{t}-s_{t-1})+(1-\beta )b_{t-1}\\c_{t}&=\gamma (x_{t}-s_{t-
1}-b_{t-1})+(1-\gamma )c_{t-L}\\F_{t+m}&=s_{t}+mb_{t}+c_{t-L+1+(m-1)\mod
L},\end{aligned}}}  [{\displaystyle {\begin{aligned}s_{0}&=x_{0}\\s_{t}&=\alpha
(x_{t}-c_{t-L})+(1-\alpha )(s_{t-1}+b_{t-1})\\b_{t}&=\beta (s_{t}-s_{t-1})+(1-
\beta )b_{t-1}\\c_{t}&=\gamma (x_{t}-s_{t-1}-b_{t-1})+(1-\gamma )c_{t-L}\\F_
{t+m}&=s_{t}+mb_{t}+c_{t-L+1+(m-1)\mod L},\end{aligned}}}]
***** Implementations in statistics packages[edit] *****
    * R: the HoltWinters function in the stats package[16] and ets function in
      the forecast package[17] (a more complete implementation, generally
      resulting in a better performance[18]).
    * IBM SPSS includes Simple, Simple Seasonal, Holt's Linear Trend, Brown's
      Linear Trend, Damped Trend, Winters' Additive, and Winters'
      Multiplicative in the Time-Series modeling procedure within its
      Statistics and Modeler statistical packages. The default Expert Modeler
      feature evaluates all seven exponential smoothing models and ARIMA models
      with a range of nonseasonal and seasonal p, d, and q values, and selects
      the model with the lowest Bayesian Information Criterion statistic.
    * Stata: tssmooth command[19]
    * LibreOffice 5.2[20]
    * Microsoft_Excel 2016[21]
***** See also[edit] *****
    * Autoregressive_moving_average_model (ARMA)
    * Errors_and_residuals_in_statistics
    * Moving_average
    * Continued_fraction
***** Notes[edit] *****
   1. ^ a b c"NIST/SEMATECH_e-Handbook_of_Statistical_Methods". NIST. Retrieved
      23 May 2010.
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
   3. ^ a bOppenheim, Alan V.; Schafer, Ronald W. (1975). Digital Signal
      Processing. Prentice_Hall. p. 5. ISBN 0-13-214635-5.
   4. ^Brown, Robert G. (1956). Exponential_Smoothing_for_Predicting_Demand.
      Cambridge, Massachusetts: Arthur D. Little Inc. p. 15.
   5. ^Holt,_Charles_C. (1957). "Forecasting Trends and Seasonal by
      Exponentially Weighted Averages". Office of Naval Research Memorandum.
      52.
   6.  reprinted inHolt,_Charles_C. (January â March 2004). "Forecasting
      Trends_and_Seasonal_by_Exponentially_Weighted_Averages". International
      Journal_of_Forecasting. 20 (1): 5â10.
   7. ^Brown, Robert Goodell (1963). Smoothing_Forecasting_and_Prediction_of
      Discrete_Time_Series. Englewood Cliffs, NJ: Prentice-Hall.
   8. ^"NIST/SEMATECH_e-Handbook_of_Statistical_Methods,_6.4.3.1._Single
      Exponential_Smoothing". NIST. Retrieved 5 July 2017.
   9. ^Nau, Robert. "Averaging_and_Exponential_Smoothing_Models". Retrieved 26
      July 2010.
  10. ^ "Production and Operations Analysis" Nahmias. 2009.
  11. ^ https://www.otexts.org/fpp/7/1
  12. ^Nahmias, Steven. Production and Operations Analysis (6th ed.). ISBN 0-
      07-337785-6.
  13. [page needed]
  14. ^"Model:_Second-Order_Exponential_Smoothing". SAP_AG. Retrieved 23
      January 2013.
  15. ^"6.4.3.3._Double_Exponential_Smoothing". itl.nist.gov. Retrieved 25
      September 2011.
  16. ^"Averaging_and_Exponential_Smoothing_Models". duke.edu. Retrieved 25
      September 2011.
  17. ^Kalehar, Prajakta S. "Time_series_Forecasting_using_Holt-Winters
      Exponential_Smoothing" (PDF). Retrieved 23 June 2014.
  18. ^ a bWinters, P. R. (April 1960). "Forecasting_Sales_by_Exponentially
      Weighted_Moving_Averages". Management_Science. 6 (3): 324â342. doi:
      10.1287/mnsc.6.3.324.
  19. ^"R:_Holt-Winters_Filtering". stat.ethz.ch. Retrieved 5 June 2016.
  20. ^"ets_{forecast}_|_inside-R_|_A_Community_Site_for_R". www.inside-r.org.
      Archived from the_original on 16 July 2016. Retrieved 5 June 2016.
  21. ^"Comparing_HoltWinters()_and_ets()". Hyndsight. 29 May 2011. Retrieved 5
      June 2016.
  22. ^ tssmooth in Stata manual
  23. ^ https://wiki.documentfoundation.org/ReleaseNotes/
      5.2#New_spreadsheet_functions
  24. ^ http://www.real-statistics.com/time-series-analysis/basic-time-series-
      forecasting/excel-2016-forecasting-functions/
***** External links[edit] *****
    * Lecture_notes_on_exponential_smoothing_(Robert_Nau,_Duke_University)
    * Data_Smoothing by Jon McLoone, The_Wolfram_Demonstrations_Project
    * The_Holt-Winters_Approach_to_Exponential_Smoothing:_50_Years_Old_and
      Going_Strong by Paul Goodwin (2010) Foresight:_The_International_Journal
      of_Applied_Forecasting
    * Algorithms_for_Unevenly_Spaced_Time_Series:_Moving_Averages_and_Other
      Rolling_Operators by Andreas Eckner
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
                                  * Exponential smoothing
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
    * v
    * t
    * e
Quantitative forecasting methods
Historical data forecasts
    * Moving_average
    * Exponential smoothing
    * Trend_analysis
    * Decomposition_of_time_series
    * NaÃ¯ve_approach
Associative (causal) forecasts
Moving_average
Simple_linear_regression
Regression_analysis
Econometric_model

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Exponential_smoothing&oldid=908868898"
Categories:
    * Time_series
Hidden categories:
    * Wikipedia_articles_needing_page_number_citations_from_September_2011
    * Articles_with_short_description
    * Use_dmy_dates_from_September_2011
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
    * Deutsch
    * EspaÃ±ol
    * Euskara
    * FranÃ§ais
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 1 August 2019, at 14:55 (UTC).
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
