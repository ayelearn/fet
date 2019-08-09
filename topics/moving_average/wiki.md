The following text has been accessed from https://en.wikipedia.org/wiki/Moving_average at Fri Aug 9 03:46:12 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Moving average ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
type of statistical measure over subsets of a dataset
For the statistical process, see Moving_average_model.
For other uses, see Moving_average_(disambiguation).
An example of two moving average curves
In statistics, a moving average (rolling average or running average) is a
calculation to analyze data points by creating a series of averages of
different subsets of the full data set. It is also called a moving mean (MM)[1]
or rolling mean and is a type of finite_impulse_response filter. Variations
include: simple, and cumulative, or weighted forms (described below).
Given a series of numbers and a fixed subset size, the first element of the
moving average is obtained by taking the average of the initial fixed subset of
the number series. Then the subset is modified by "shifting forward"; that is,
excluding the first number of the series and including the next value in the
subset.
A moving average is commonly used with time_series data to smooth out short-
term fluctuations and highlight longer-term trends or cycles. The threshold
between short-term and long-term depends on the application, and the parameters
of the moving average will be set accordingly. For example, it is often used in
technical_analysis of financial data, like stock prices, returns or trading
volumes. It is also used in economics to examine gross domestic product,
employment or other macroeconomic time series. Mathematically, a moving average
is a type of convolution and so it can be viewed as an example of a low-pass
filter used in signal_processing. When used with non-time series data, a moving
average filters higher frequency components without any specific connection to
time, although typically some kind of ordering is implied. Viewed
simplistically it can be regarded as smoothing the data.
⁰
***** Contents *****
    * 1_Simple_moving_average
    * 2_Cumulative_moving_average
    * 3_Weighted_moving_average
    * 4_Exponential_moving_average
          o 4.1_Approximating_the_EMA_with_a_limited_number_of_terms
          o 4.2_Relationship_between_SMA_and_EMA
          o 4.3_Exponentially_weighted_moving_variance_and_standard_deviation
          o 4.4_Modified_moving_average
          o 4.5_Application_to_measuring_computer_performance
    * 5_Other_weightings
    * 6_Moving_median
    * 7_Moving_average_regression_model
    * 8_See_also
    * 9_Notes_and_references
    * 10_External_links
***** Simple moving average[edit] *****
[Moving_Average_Types_comparison_-_Simple_and_Exponential.png]
In financial applications a simple moving average (SMA) is the unweighted mean
of the previous n data. However, in science and engineering, the mean is
normally taken from an equal number of data on either side of a central value.
This ensures that variations in the mean are aligned with the variations in the
data rather than being shifted in time.  An example of a simple equally
weighted running mean for a n-day sample of closing price is the mean of the
previous n days' closing prices. If those prices are      p  M   ,  p  M
&#x2212; 1   , &#x2026; ,  p  M &#x2212; ( n &#x2212; 1 )     {\displaystyle p_
{M},p_{M-1},\dots ,p_{M-(n-1)}}  [{\displaystyle p_{M},p_{M-1},\dots ,p_{M-(n-
1)}}] then the formula is
                p &#x00AF;    SM      =     p  M   +  p  M &#x2212; 1   +
      &#x22EF; +  p  M &#x2212; ( n &#x2212; 1 )    n         =   1 n
      &#x2211;  i = 0   n &#x2212; 1    p  M &#x2212; i   .
      {\displaystyle {\begin{aligned}{\overline {p}}_{\text{SM}}&={\frac {p_
      {M}+p_{M-1}+\cdots +p_{M-(n-1)}}{n}}\\&={\frac {1}{n}}\sum _{i=0}^{n-1}p_
      {M-i}.\end{aligned}}}  [{\displaystyle {\begin{aligned}{\overline {p}}_
      {\text{SM}}&={\frac {p_{M}+p_{M-1}+\cdots +p_{M-(n-1)}}{n}}\\&={\frac {1}
      {n}}\sum _{i=0}^{n-1}p_{M-i}.\end{aligned}}}]
When calculating successive values, a new value comes into the sum, and the
oldest value drops out, meaning that a full summation each time is unnecessary
for this simple case:
            p &#x00AF;    SM   =    p &#x00AF;     SM  ,  prev    +   1 n
      (  p  M   &#x2212;  p  M &#x2212; n   ) .   {\displaystyle {\overline
      {p}}_{\text{SM}}={\overline {p}}_{{\text{SM}},{\text{prev}}}+{\frac {1}
      {n}}(p_{M}-p_{M-n}).}  [{\displaystyle {\overline {p}}_{\text{SM}}=
      {\overline {p}}_{{\text{SM}},{\text{prev}}}+{\frac {1}{n}}(p_{M}-p_{M-
      n}).}]
The period selected depends on the type of movement of interest, such as short,
intermediate, or long-term. In financial terms, moving-average levels can be
interpreted as support in a falling market or resistance in a rising market.
If the data used are not centered around the mean, a simple moving average lags
behind the latest datum point by half the sample width. An SMA can also be
disproportionately influenced by old datum points dropping out or new data
coming in. One characteristic of the SMA is that if the data have a periodic
fluctuation, then applying an SMA of that period will eliminate that variation
(the average always containing one complete cycle). But a perfectly regular
cycle is rarely encountered.[2]
For a number of applications, it is advantageous to avoid the shifting induced
by using only "past" data. Hence a central moving average can be computed,
using data equally spaced on either side of the point in the series where the
mean is calculated.[3] This requires using an odd number of datum points in the
sample window.
A major drawback of the SMA is that it lets through a significant amount of the
signal shorter than the window length. Worse, it actually inverts it. This can
lead to unexpected artifacts, such as peaks in the smoothed result appearing
where there were troughs in the data. It also leads to the result being less
smooth than expected, since some of the higher frequencies are not properly
removed.
***** Cumulative moving average[edit] *****
In a cumulative moving average (CMA), the data arrive in an ordered datum
stream, and the user would like to get the average of all of the data up until
the current datum point. For example, an investor may want the average price of
all of the stock transactions for a particular stock up until the current time.
As each new transaction occurs, the average price at the time of the
transaction can be calculated for all of the transactions up to that point
using the cumulative average, typically an equally weighted average of the
sequence of n values      x  1   . &#x2026; ,  x  n     {\displaystyle x_
{1}.\ldots ,x_{n}}  [x_{1}.\ldots ,x_{n}] up to the current time:
            CMA    n   =     x  1   + &#x22EF; +  x  n    n    .
      {\displaystyle {\textit {CMA}}_{n}={{x_{1}+\cdots +x_{n}} \over n}\,.}  [
      {\textit {CMA}}_{n}={{x_{1}+\cdots +x_{n}} \over n}\,.]
The brute-force method to calculate this would be to store all of the data and
calculate the sum and divide by the number of datum points every time a new
datum point arrived. However, it is possible to simply update cumulative
average as a new value,      x  n + 1     {\displaystyle x_{n+1}}  [x_{n+1}]
becomes available, using the formula
            CMA    n + 1   =     x  n + 1   + n &#x22C5;    CMA    n     n + 1
      .   {\displaystyle {\textit {CMA}}_{n+1}={{x_{n+1}+n\cdot {\textit
      {CMA}}_{n}} \over {n+1}}.}  [{\displaystyle {\textit {CMA}}_{n+1}={{x_
      {n+1}+n\cdot {\textit {CMA}}_{n}} \over {n+1}}.}]
Thus the current cumulative average for a new datum point is equal to the
previous cumulative average, times n, plus the latest datum point, all divided
by the number of points received so far, n+1. When all of the datum points
arrive (n = N), then the cumulative average will equal the final average. It is
also possible to store a running total of the datum point as well as the number
of points and dividing the total by the number of datum points to get the CMA
each time a new datum point arrives.
The derivation of the cumulative average formula is straightforward. Using
          x  1   + &#x22EF; +  x  n   = n &#x22C5;    CMA    n
      {\displaystyle x_{1}+\cdots +x_{n}=n\cdot {\textit {CMA}}_{n}}  [x_
      {1}+\cdots +x_{n}=n\cdot {\textit {CMA}}_{n}]
and similarly for n + 1, it is seen that
              x  n + 1      = (  x  1   + &#x22EF; +  x  n + 1   ) &#x2212;
      (  x  1   + &#x22EF; +  x  n   )       {\displaystyle {\begin{aligned}x_
      {n+1}&=(x_{1}+\cdots +x_{n+1})-(x_{1}+\cdots +x_{n})\\[6pt]\end
      {aligned}}}  [{\displaystyle {\begin{aligned}x_{n+1}&=(x_{1}+\cdots +x_
      {n+1})-(x_{1}+\cdots +x_{n})\\[6pt]\end{aligned}}}]
Solving this equation for        CMA    n + 1     {\displaystyle {\textit
{CMA}}_{n+1}}  [{\textit {CMA}}_{n+1}] results in
                CMA    n + 1      =     x  n + 1   + n &#x22C5;    CMA    n
      n + 1          =     x  n + 1   + ( n + 1 &#x2212; 1 ) &#x22C5;    CMA
      n     n + 1          =    ( n + 1 ) &#x22C5;    CMA    n   +  x  n + 1
      &#x2212;    CMA    n     n + 1          =     CMA    n    +     x  n + 1
      &#x2212;    CMA    n     n + 1          {\displaystyle {\begin{aligned}
      {\textit {CMA}}_{n+1}&={x_{n+1}+n\cdot {\textit {CMA}}_{n} \over {n+1}}\\
      [6pt]&={x_{n+1}+(n+1-1)\cdot {\textit {CMA}}_{n} \over {n+1}}\\[6pt]&={
      (n+1)\cdot {\textit {CMA}}_{n}+x_{n+1}-{\textit {CMA}}_{n} \over {n+1}}\\
      [6pt]&={{\textit {CMA}}_{n}}+{{x_{n+1}-{\textit {CMA}}_{n}} \over
      {n+1}}\end{aligned}}}  [{\displaystyle {\begin{aligned}{\textit {CMA}}_
      {n+1}&={x_{n+1}+n\cdot {\textit {CMA}}_{n} \over {n+1}}\\[6pt]&={x_{n+1}+
      (n+1-1)\cdot {\textit {CMA}}_{n} \over {n+1}}\\[6pt]&={(n+1)\cdot
      {\textit {CMA}}_{n}+x_{n+1}-{\textit {CMA}}_{n} \over {n+1}}\\[6pt]&={
      {\textit {CMA}}_{n}}+{{x_{n+1}-{\textit {CMA}}_{n}} \over {n+1}}\end
      {aligned}}}]
***** Weighted moving average[edit] *****
A weighted average is an average that has multiplying factors to give different
weights to data at different positions in the sample window. Mathematically,
the moving average is the convolution of the datum points with a fixed
weighting function. One application is removing pixelisation from a digital
graphical image.[citation_needed]
In technical_analysis of financial data, a weighted moving average (WMA) has
the specific meaning of weights that decrease in arithmetical progression.[4]
In an n-day WMA the latest day has weight n, the second latest n â 1, etc.,
down to one.
           WMA   M   =    n  p  M   + ( n &#x2212; 1 )  p  M &#x2212; 1   +
      &#x22EF; + 2  p  ( M &#x2212; n + 2 )   +  p  ( M &#x2212; n + 1 )     n
      + ( n &#x2212; 1 ) + &#x22EF; + 2 + 1      {\displaystyle {\text{WMA}}_
      {M}={np_{M}+(n-1)p_{M-1}+\cdots +2p_{(M-n+2)}+p_{(M-n+1)} \over n+(n-
      1)+\cdots +2+1}}  [{\text{WMA}}_{M}={np_{M}+(n-1)p_{M-1}+\cdots +2p_{(M-
      n+2)}+p_{(M-n+1)} \over n+(n-1)+\cdots +2+1}]
WMA weights n = 15
The denominator is a triangle_number equal to        n ( n + 1 )  2   .
{\displaystyle {\frac {n(n+1)}{2}}.}  [{\displaystyle {\frac {n(n+1)}{2}}.}] In
the more general case the denominator will always be the sum of the individual
weights.
When calculating the WMA across successive values, the difference between the
numerators of WMAM+1 and WMAM is npM+1 â pM â âââ â pMân+1. If we
denote the sum pM + âââ + pMân+1 by TotalM, then
               Total   M + 1      =   Total   M   +  p  M + 1   &#x2212;  p  M
      &#x2212; n + 1         Numerator   M + 1      =   Numerator   M   + n  p
      M + 1   &#x2212;   Total   M         WMA   M + 1      =     Numerator   M
      + 1    n + ( n &#x2212; 1 ) + &#x22EF; + 2 + 1          {\displaystyle
      {\begin{aligned}{\text{Total}}_{M+1}&={\text{Total}}_{M}+p_{M+1}-p_{M-
      n+1}\\[3pt]{\text{Numerator}}_{M+1}&={\text{Numerator}}_{M}+np_{M+1}-
      {\text{Total}}_{M}\\[3pt]{\text{WMA}}_{M+1}&={{\text{Numerator}}_{M+1}
      \over n+(n-1)+\cdots +2+1}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}{\text{Total}}_{M+1}&={\text{Total}}_{M}+p_{M+1}-p_{M-n+1}\\
      [3pt]{\text{Numerator}}_{M+1}&={\text{Numerator}}_{M}+np_{M+1}-{\text
      {Total}}_{M}\\[3pt]{\text{WMA}}_{M+1}&={{\text{Numerator}}_{M+1} \over n+
      (n-1)+\cdots +2+1}\end{aligned}}}]
The graph at the right shows how the weights decrease, from highest weight for
the most recent datum points, down to zero. It can be compared to the weights
in the exponential moving average which follows.
***** Exponential moving average[edit] *****
Further information: EWMA_chart and Exponential_smoothing
EMA weights N = 15
An exponential moving average (EMA), also known as an exponentially weighted
moving average (EWMA),[5] is a first-order infinite_impulse_response filter
that applies weighting factors which decrease exponentially. The weighting for
each older datum decreases exponentially, never reaching zero. The graph at
right shows an example of the weight decrease.
The EMA for a series Y may be calculated recursively:
          S  t   =   {     Y  1   ,   t = 1     &#x03B1; &#x22C5;  Y  t   + ( 1
      &#x2212; &#x03B1; ) &#x22C5;  S  t &#x2212; 1   ,   t > 1
      {\displaystyle S_{t}={\begin{cases}Y_{1},&t=1\\\alpha \cdot Y_{t}+(1-
      \alpha )\cdot S_{t-1},&t>1\end{cases}}}  [{\displaystyle S_{t}={\begin
      {cases}Y_{1},&t=1\\\alpha \cdot Y_{t}+(1-\alpha )\cdot S_{t-1},&t>1\end
      {cases}}}]
Where:
    * The coefficient Î± represents the degree of weighting decrease, a
      constant smoothing factor between 0 and 1. A higher Î± discounts older
      observations faster.
    * Yt is the value at a time period t.
    * St is the value of the EMA at any time period t.
S1 may be initialized in a number of different ways, most commonly by setting
S1 to Y1 as shown above, though other techniques exist, such as setting S1 to
an average of the first 4 or 5 observations. The importance of the S1
initialisations effect on the resultant moving average depends on Î±; smaller
Î± values make the choice of S1 relatively more important than larger Î±
values, since a higher Î± discounts older observations faster.
Whatever is done for S1 it assumes something about values prior to the
available data and is necessarily in error. In view of this, the early results
should be regarded as unreliable until the iterations have had time to
converge. This is sometimes called a 'spin-up' interval. One way to assess when
it can be regarded as reliable is to consider the required accuracy of the
result. For example, if 3% accuracy is required, initialising with Y1 and
taking data after five time constants (defined above) will ensure that the
calculation has converged to within 3% (only <3% of Y1 will remain in the
result ). Sometimes with very small alpha, this can mean little of the result
is useful. This is analogous to the problem of using a convolution filter (such
as a weighted average) with a very long window.
This formulation is according to Hunter (1986).[6] By repeated application of
this formula for different times, we can eventually write St as a weighted sum
of the datum points Yt, as:
              S  t   = &#x03B1;    [   Y  t   + ( 1 &#x2212; &#x03B1; )  Y  t
      &#x2212; 1   + ( 1 &#x2212; &#x03B1;  )  2    Y  t &#x2212; 2   +
      &#x22EF;            &#x22EF; + ( 1 &#x2212; &#x03B1;  )  k    Y  t
      &#x2212; k    ]  + ( 1 &#x2212; &#x03B1;  )  k + 1    S  t &#x2212; ( k +
      1 )         {\displaystyle {\begin{aligned}S_{t}=\alpha &\left[Y_{t}+(1-
      \alpha )Y_{t-1}+(1-\alpha )^{2}Y_{t-2}+\cdots \right.\\[6pt]&\left.\cdots
      +(1-\alpha )^{k}Y_{t-k}\right]+(1-\alpha )^{k+1}S_{t-(k+1)}\end
      {aligned}}}  [{\displaystyle {\begin{aligned}S_{t}=\alpha &\left[Y_{t}+
      (1-\alpha )Y_{t-1}+(1-\alpha )^{2}Y_{t-2}+\cdots \right.\\
      [6pt]&\left.\cdots +(1-\alpha )^{k}Y_{t-k}\right]+(1-\alpha )^{k+1}S_{t-
      (k+1)}\end{aligned}}}]
for any suitable k ∈ {0, 1, 2, â¦} The weight of the general datum point
Y  t &#x2212; i     {\displaystyle Y_{t-i}}  [Y_{t-i}] is     &#x03B1;   (  1
&#x2212; &#x03B1;  )   i     {\displaystyle \alpha \left(1-\alpha \right)^{i}}
[{\displaystyle \alpha \left(1-\alpha \right)^{i}}].
This formula can also be expressed in technical analysis terms as follows,
showing how the EMA steps towards the latest datum point, but only by a
proportion of the difference (each time):
           EMA   today   =   EMA   yesterday   + &#x03B1;  [    price   today
      &#x2212;   EMA   yesterday    ]    {\displaystyle {\text{EMA}}_{\text
      {today}}={\text{EMA}}_{\text{yesterday}}+\alpha \left[{\text{price}}_
      {\text{today}}-{\text{EMA}}_{\text{yesterday}}\right]}  [{\displaystyle
      {\text{EMA}}_{\text{today}}={\text{EMA}}_{\text{yesterday}}+\alpha \left[
      {\text{price}}_{\text{today}}-{\text{EMA}}_{\text{yesterday}}\right]}]
Expanding out       EMA   yesterday     {\displaystyle {\text{EMA}}_{\text
{yesterday}}}  [{\displaystyle {\text{EMA}}_{\text{yesterday}}}] each time
results in the following power series, showing how the weighting factor on each
datum point p1, p2, etc., decreases exponentially:
           EMA   today   =  &#x03B1;  [   p  1   + ( 1 &#x2212; &#x03B1; )  p
      2   + ( 1 &#x2212; &#x03B1;  )  2    p  3   + ( 1 &#x2212; &#x03B1;  )  3
      p  4   + &#x22EF;  ]     {\displaystyle {\text{EMA}}_{\text{today}}=
      {\alpha \left[p_{1}+(1-\alpha )p_{2}+(1-\alpha )^{2}p_{3}+(1-\alpha )^
      {3}p_{4}+\cdots \right]}}  [{\displaystyle {\text{EMA}}_{\text{today}}=
      {\alpha \left[p_{1}+(1-\alpha )p_{2}+(1-\alpha )^{2}p_{3}+(1-\alpha )^
      {3}p_{4}+\cdots \right]}}]
where
    *     p  1     {\displaystyle p_{1}}  [p_{1}] is       price   today
      {\displaystyle {\text{price}}_{\text{today}}}  [{\displaystyle {\text
      {price}}_{\text{today}}}]
    *     p  2     {\displaystyle p_{2}}  [p_{2}] is       price   yesterday
      {\displaystyle {\text{price}}_{\text{yesterday}}}  [{\displaystyle {\text
      {price}}_{\text{yesterday}}}]
    * and so on
           EMA   today   =     p  1   + ( 1 &#x2212; &#x03B1; )  p  2   + ( 1
      &#x2212; &#x03B1;  )  2    p  3   + ( 1 &#x2212; &#x03B1;  )  3    p  4
      + &#x22EF;   1 + ( 1 &#x2212; &#x03B1; ) + ( 1 &#x2212; &#x03B1;  )  2
      + ( 1 &#x2212; &#x03B1;  )  3   + &#x22EF;    ,   {\displaystyle {\text
      {EMA}}_{\text{today}}={\frac {p_{1}+(1-\alpha )p_{2}+(1-\alpha )^{2}p_
      {3}+(1-\alpha )^{3}p_{4}+\cdots }{1+(1-\alpha )+(1-\alpha )^{2}+(1-\alpha
      )^{3}+\cdots }},}  [{\displaystyle {\text{EMA}}_{\text{today}}={\frac {p_
      {1}+(1-\alpha )p_{2}+(1-\alpha )^{2}p_{3}+(1-\alpha )^{3}p_{4}+\cdots }
      {1+(1-\alpha )+(1-\alpha )^{2}+(1-\alpha )^{3}+\cdots }},}]
since     1  /  &#x03B1; = 1 + ( 1 &#x2212; &#x03B1; ) + ( 1 &#x2212; &#x03B1;
)  2   + &#x22EF;   {\displaystyle 1/\alpha =1+(1-\alpha )+(1-\alpha )^
{2}+\cdots }  [{\displaystyle 1/\alpha =1+(1-\alpha )+(1-\alpha )^{2}+\cdots
}].
It can also be calculated recursively without introducing the error when
initializing the first estimate (n starts from 1):
           EMA   n   =     WeightedSum   n     WeightedCount   n
      {\displaystyle {\text{EMA}}_{n}={\frac {{\text{WeightedSum}}_{n}}{{\text
      {WeightedCount}}_{n}}}}  [{\displaystyle {\text{EMA}}_{n}={\frac {{\text
      {WeightedSum}}_{n}}{{\text{WeightedCount}}_{n}}}}]
           WeightedSum   n   =  p  n   + ( 1 &#x2212; &#x03B1; )   WeightedSum
      n &#x2212; 1     {\displaystyle {\text{WeightedSum}}_{n}=p_{n}+(1-\alpha
      ){\text{WeightedSum}}_{n-1}}  [{\displaystyle {\text{WeightedSum}}_{n}=p_
      {n}+(1-\alpha ){\text{WeightedSum}}_{n-1}}]
           WeightedCount   n   = 1 + ( 1 &#x2212; &#x03B1; )   WeightedCount
      n &#x2212; 1   =    1 &#x2212; ( 1 &#x2212; &#x03B1;  )  n     1 &#x2212;
      ( 1 &#x2212; &#x03B1; )      {\displaystyle {\text{WeightedCount}}_{n}=1+
      (1-\alpha ){\text{WeightedCount}}_{n-1}={\frac {1-(1-\alpha )^{n}}{1-(1-
      \alpha )}}}  [{\displaystyle {\text{WeightedCount}}_{n}=1+(1-\alpha )
      {\text{WeightedCount}}_{n-1}={\frac {1-(1-\alpha )^{n}}{1-(1-\alpha )}}}]
      Assume       WeightedSum   0   =   WeightedCount   0   = 0
      {\displaystyle {\text{WeightedSum}}_{0}={\text{WeightedCount}}_{0}=0}  [
      {\displaystyle {\text{WeightedSum}}_{0}={\text{WeightedCount}}_{0}=0}]
This is an infinite_sum with decreasing terms.
**** Approximating the EMA with a limited number of terms[edit] ****
The question of how far back to go for an initial value depends, in the worst
case, on the data. Large price values in old data will affect the total even if
their weighting is very small. If prices have small variations then just the
weighting can be considered. The power_formula above gives a starting value for
a particular day, after which the successive days formula shown first can be
applied. The weight omitted by stopping after k terms is
         &#x03B1;  [  ( 1 &#x2212; &#x03B1;  )  k   + ( 1 &#x2212; &#x03B1;  )
      k + 1   + ( 1 &#x2212; &#x03B1;  )  k + 2   + &#x22EF;  ]  ,
      {\displaystyle \alpha \left[(1-\alpha )^{k}+(1-\alpha )^{k+1}+(1-\alpha
      )^{k+2}+\cdots \right],}  [{\displaystyle \alpha \left[(1-\alpha )^{k}+
      (1-\alpha )^{k+1}+(1-\alpha )^{k+2}+\cdots \right],}]
which is
         &#x03B1; ( 1 &#x2212; &#x03B1;  )  k    [  1 + ( 1 &#x2212; &#x03B1; )
      + ( 1 &#x2212; &#x03B1;  )  2   + &#x22EF;  ]  ,   {\displaystyle \alpha
      (1-\alpha )^{k}\left[1+(1-\alpha )+(1-\alpha )^{2}+\cdots \right],}  [
      {\displaystyle \alpha (1-\alpha )^{k}\left[1+(1-\alpha )+(1-\alpha )^
      {2}+\cdots \right],}]
i.e. a fraction
                  weight omitted by stopping after&#xA0;  k  &#xA0;terms
      total weight       =        &#x03B1;  [  ( 1 &#x2212; &#x03B1;  )  k   +
      ( 1 &#x2212; &#x03B1;  )  k + 1   + ( 1 &#x2212; &#x03B1;  )  k + 2   +
      &#x22EF;  ]    &#x03B1;  [  1 + ( 1 &#x2212; &#x03B1; ) + ( 1 &#x2212;
      &#x03B1;  )  2   + &#x22EF;  ]         =        &#x03B1; ( 1 &#x2212;
      &#x03B1;  )  k     1  1 &#x2212; ( 1 &#x2212; &#x03B1; )      &#x03B1;  1
      &#x2212; ( 1 &#x2212; &#x03B1; )         =      ( 1 &#x2212; &#x03B1;  )
      k         {\displaystyle {\begin{aligned}&{\frac {{\text{weight omitted
      by stopping after }}k{\text{ terms}}}{\text{total weight}}}\\[6pt]={}&
      {\frac {\alpha \left[(1-\alpha )^{k}+(1-\alpha )^{k+1}+(1-\alpha )^
      {k+2}+\cdots \right]}{\alpha \left[1+(1-\alpha )+(1-\alpha )^{2}+\cdots
      \right]}}\\[6pt]={}&{\frac {\alpha (1-\alpha )^{k}{\frac {1}{1-(1-\alpha
      )}}}{\frac {\alpha }{1-(1-\alpha )}}}\\[6pt]={}&(1-\alpha )^{k}\end
      {aligned}}}  [{\displaystyle {\begin{aligned}&{\frac {{\text{weight
      omitted by stopping after }}k{\text{ terms}}}{\text{total weight}}}\\
      [6pt]={}&{\frac {\alpha \left[(1-\alpha )^{k}+(1-\alpha )^{k+1}+(1-\alpha
      )^{k+2}+\cdots \right]}{\alpha \left[1+(1-\alpha )+(1-\alpha )^{2}+\cdots
      \right]}}\\[6pt]={}&{\frac {\alpha (1-\alpha )^{k}{\frac {1}{1-(1-\alpha
      )}}}{\frac {\alpha }{1-(1-\alpha )}}}\\[6pt]={}&(1-\alpha )^{k}\end
      {aligned}}}][7]
out of the total weight.
For example, to have 99.9% of the weight, set above ratio equal to 0.1% and
solve for k:
         k =    log &#x2061; ( 0.001 )   log &#x2061; ( 1 &#x2212; &#x03B1; )
      {\displaystyle k={\log(0.001) \over \log(1-\alpha )}}  [{\displaystyle k=
      {\log(0.001) \over \log(1-\alpha )}}]
to determine how many terms should be used. Since     &#x03B1; &#x2192; 0
{\displaystyle \alpha \to 0}  [\alpha \to 0] as     N &#x2192; &#x221E;
{\displaystyle N\to \infty }  [N\to \infty ], we know     log  ( 1 &#x2212;
&#x03B1; )   {\displaystyle \log \,(1-\alpha )}  [\log \,(1-\alpha )]
approaches     &#x2212; &#x03B1;   {\displaystyle -\alpha }  [-\alpha ] as N
increases [8]. This gives:
         k &#x2248;    log &#x2061; ( 0.001 )   &#x2212; &#x03B1;
      {\displaystyle k\approx {\log(0.001) \over {-\alpha }}}  [{\displaystyle
      k\approx {\log(0.001) \over {-\alpha }}}]
When     &#x03B1;   {\displaystyle \alpha }  [\alpha ] is related to N via to
&#x03B1; =   2  N + 1      {\displaystyle \alpha ={2 \over N+1}}  [
{\displaystyle \alpha ={2 \over N+1}}], this simplifies to approximately[9],
         k &#x2248; 3.45 ( N + 1 )    {\displaystyle k\approx 3.45(N+1)\,}  [
      {\displaystyle k\approx 3.45(N+1)\,}]
for this example (99.9% weight).
**** Relationship between SMA and EMA[edit] ****
Note that there is no "accepted" value that should be chosen for     &#x03B1;
{\displaystyle \alpha }  [\alpha ], although there are some recommended values
based on the application. A commonly used value for     &#x03B1;
{\displaystyle \alpha }  [\alpha ] is     &#x03B1; = 2  /  ( N + 1 )
{\displaystyle \alpha =2/(N+1)}  [\alpha =2/(N+1)]. This is because the weights
of an SMA and EMA have the same "center of mass" when      &#x03B1;   R M A
= 2  /   (   N   S M A    + 1  )    {\displaystyle \alpha _{\mathrm {RMA} }=2/
\left(N_{\mathrm {SMA} }+1\right)}  [{\displaystyle \alpha _{\mathrm {RMA} }=2/
\left(N_{\mathrm {SMA} }+1\right)}].
[Proof]
The weights of an     N   {\displaystyle N}  [N]-day SMA have a "center of
mass" on the      R   t h      {\displaystyle R^{\mathrm {th} }}  [
{\displaystyle R^{\mathrm {th} }}] day, where



        R
        =



              N
              +
              1

            2




    {\displaystyle R={\frac {N+1}{2}}}

[{\displaystyle R={\frac {N+1}{2}}}]
(or     R =  (  N &#x2212; 1  )   /  2   {\displaystyle R=\left(N-1\right)/2}
[{\displaystyle R=\left(N-1\right)/2}], if we use zero-based indexing)
For the remainder of this proof we will use one-based indexing.

Now meanwhile, the weights of an EMA have center of mass




          R


              E
              M
              A



        =
        &#x03B1;

          [

            1
            +
            2
            &#x2217;
            (
            1
            &#x2212;
            &#x03B1;
            )
            +
            3
            &#x2217;
            (
            1
            &#x2212;
            &#x03B1;

              )

                2


            +
            .
            .
            .
            +
            k
            &#x2217;
            (
            1
            &#x2212;
            &#x03B1;

              )

                k
                &#x2212;
                1



          ]



    {\displaystyle R_{\mathrm {EMA} }=\alpha \left[1+2*(1-\alpha )+3*(1-\alpha
)^{2}+...+k*(1-\alpha )^{k-1}\right]}

[{\displaystyle R_{\mathrm {EMA} }=\alpha \left[1+2*(1-\alpha )+3*(1-\alpha )^
{2}+...+k*(1-\alpha )^{k-1}\right]}]
That is,




          R


              E
              M
              A



        =
        &#x03B1;

          &#x2211;

            k
            =
            1


            k
            =
            &#x221E;




        k
        &#x2217;


            (

              1
              &#x2212;
              &#x03B1;

            )


            k
            &#x2212;
            1




    {\displaystyle R_{\mathrm {EMA} }=\alpha \sum _{k=1}^{k=\infty }\!\,k*\left
(1-\alpha \right)^{k-1}}

[{\displaystyle R_{\mathrm {EMA} }=\alpha \sum _{k=1}^{k=\infty }\!\,k*\left(1-
\alpha \right)^{k-1}}]

We also know the Maclaurin Series



        1

          /

        (
        1
        &#x2212;
        x
        )
        =

          &#x2211;

            k
            =
            0


            k
            =
            &#x221E;





          x

            k




    {\displaystyle 1/(1-x)=\sum _{k=0}^{k=\infty }\!\,x^{k}}

[{\displaystyle 1/(1-x)=\sum _{k=0}^{k=\infty }\!\,x^{k}}]
Taking derivatives of both sides with respect to     x   {\displaystyle x}  [x]
gives:




        (
        x
        &#x2212;
        1

          )

            &#x2212;
            2


        =

          &#x2211;

            k
            =
            0


            k
            =
            &#x221E;




        k
        &#x2217;

          x

            k
            &#x2212;
            1




    {\displaystyle (x-1)^{-2}=\sum _{k=0}^{k=\infty }\!\,k*x^{k-1}}

[{\displaystyle (x-1)^{-2}=\sum _{k=0}^{k=\infty }\!\,k*x^{k-1}}]
or




        (
        x
        &#x2212;
        1

          )

            &#x2212;
            2


        =
        0
        +

          &#x2211;

            k
            =
            1


            k
            =
            &#x221E;




        k
        &#x2217;

          x

            k
            &#x2212;
            1




    {\displaystyle (x-1)^{-2}=0+\sum _{k=1}^{k=\infty }\!\,k*x^{k-1}}

[{\displaystyle (x-1)^{-2}=0+\sum _{k=1}^{k=\infty }\!\,k*x^{k-1}}]


Substituting     x = 1 &#x2212; &#x03B1;   {\displaystyle x=1-\alpha }  [
{\displaystyle x=1-\alpha }], we get




          R


              E
              M
              A



        =
        &#x03B1;


            (
            &#x03B1;
            )


            &#x2212;
            2




    {\displaystyle R_{\mathrm {EMA} }=\alpha \left(\alpha \right)^{-2}}

[{\displaystyle R_{\mathrm {EMA} }=\alpha \left(\alpha \right)^{-2}}]
or




          R


              E
              M
              A



        =


            (
            &#x03B1;
            )


            &#x2212;
            1




    {\displaystyle R_{\mathrm {EMA} }=\left(\alpha \right)^{-1}}

[{\displaystyle R_{\mathrm {EMA} }=\left(\alpha \right)^{-1}}]

So the value of     &#x03B1;   {\displaystyle \alpha }  [\alpha ] that sets
R   S M A    =  R   R M A      {\displaystyle R_{\mathrm {SMA} }=R_{\mathrm
{RMA} }}  [{\displaystyle R_{\mathrm {SMA} }=R_{\mathrm {RMA} }}] is, in fact:







                N


                    S
                    M
                    A



              +
              1

            2


        =


            (

              &#x03B1;


                  E
                  M
                  A



            )


            &#x2212;
            1




    {\displaystyle {\frac {N_{\mathrm {SMA} }+1}{2}}=\left(\alpha _{\mathrm
{EMA} }\right)^{-1}}

[{\displaystyle {\frac {N_{\mathrm {SMA} }+1}{2}}=\left(\alpha _{\mathrm {EMA}
}\right)^{-1}}]
or





            2


                N


                    S
                    M
                    A



              +
              1



        =

          &#x03B1;


              E
              M
              A





    {\displaystyle {\frac {2}{N_{\mathrm {SMA} }+1}}=\alpha _{\mathrm {EMA} }}

[{\displaystyle {\frac {2}{N_{\mathrm {SMA} }+1}}=\alpha _{\mathrm {EMA} }}]
And so     2  /   (  N + 1  )    {\displaystyle 2/\left(N+1\right)}  [
{\displaystyle 2/\left(N+1\right)}] is the value of     &#x03B1;
{\displaystyle \alpha }  [\alpha ] that creates an EMA whose weights have the
same center of gravity as would the equivalent N-day SMA

This is also why sometimes an EMA is referred to as an N-day EMA. Despite the
name suggesting there are N periods, the terminology only specifies the Î±
factor. N is not a stopping point for the calculation in the way it is in an
SMA or WMA. For sufficiently large N, the first N datum points in an EMA
represent about 86% of the total weight in the calculation when     &#x03B1; =
2  /  ( N + 1 )   {\displaystyle \alpha =2/(N+1)}  [\alpha =2/(N+1)]:

[Proof]
The sum of the weights of all the terms (i.e., infinite number of terms) in an
exponential moving average is 1. The sum of the weights of     N
{\displaystyle N}  [N] terms is     1 &#x2212; ( 1 &#x2212; &#x03B1;  )  N + 1
{\displaystyle 1-(1-\alpha )^{N+1}}  [1-(1-\alpha )^{N+1}]. Both of these sums
can be derived by using the formula for the sum of a geometric series. The
weight omitted after     N   {\displaystyle N}  [N] terms is given by
subtracting this from 1, and you get     1 &#x2212;  [  1 &#x2212; ( 1 &#x2212;
&#x03B1;  )  N + 1    ]  = ( 1 &#x2212; &#x03B1;  )  N + 1     {\displaystyle
1-\left[1-(1-\alpha )^{N+1}\right]=(1-\alpha )^{N+1}}  [{\displaystyle 1-\left
[1-(1-\alpha )^{N+1}\right]=(1-\alpha )^{N+1}}] (this is essentially the
formula given previously for the weight omitted).
We now substitute the commonly used value for     &#x03B1; = 2  /  ( N + 1 )
{\displaystyle \alpha =2/(N+1)}  [\alpha =2/(N+1)] in the formula for the
weight of     N   {\displaystyle N}  [N] terms. If you make this substitution,
and you make use of[10]      lim  n &#x2192; &#x221E;     (  1 +   a n    )   n
=  e  a     {\displaystyle \lim _{n\to \infty }\left(1+{a \over n}\right)^
{n}=e^{a}}  [{\displaystyle \lim _{n\to \infty }\left(1+{a \over n}\right)^
{n}=e^{a}}], then you get
            &#x03B1;  [  1 + ( 1 &#x2212; &#x03B1; ) + ( 1 &#x2212; &#x03B1;  )
      2   + &#x22EF; + ( 1 &#x2212; &#x03B1;  )  N    ]    &#x03B1;  [  1 + ( 1
      &#x2212; &#x03B1; ) + ( 1 &#x2212; &#x03B1;  )  2   + &#x22EF;  ]  )    =
      1 &#x2212;    (  1 &#x2212;   2  N + 1     )    N + 1     {\displaystyle
      {\frac {\alpha \left[1+(1-\alpha )+(1-\alpha )^{2}+\cdots +(1-\alpha )^
      {N}\right]}{\alpha \left[1+(1-\alpha )+(1-\alpha )^{2}+\cdots
      \right])}}=1-{\left(1-{2 \over N+1}\right)}^{N+1}}  [{\displaystyle
      {\frac {\alpha \left[1+(1-\alpha )+(1-\alpha )^{2}+\cdots +(1-\alpha )^
      {N}\right]}{\alpha \left[1+(1-\alpha )+(1-\alpha )^{2}+\cdots
      \right])}}=1-{\left(1-{2 \over N+1}\right)}^{N+1}}][11]
      i.e.      lim  N &#x2192; &#x221E;    [  1 &#x2212;    (  1 &#x2212;   2
      N + 1     )    N + 1    ]    {\displaystyle \lim _{N\to \infty }\left[1-
      {\left(1-{2 \over N+1}\right)}^{N+1}\right]}  [{\displaystyle \lim _{N\to
      \infty }\left[1-{\left(1-{2 \over N+1}\right)}^{N+1}\right]}] simplified,
      [12] tends to     1 &#x2212;  e  &#x2212; 2   &#x2248; 0.8647
      {\displaystyle 1-e^{-2}\approx 0.8647}  [{\displaystyle 1-e^{-2}\approx
      0.8647}].
the 0.8647 approximation. Intuitively, what this is telling us is that the
weight after     N   {\displaystyle N}  [N] terms of an ``    N
{\displaystyle N}  [N]-period" exponential moving average converges to 0.8647.
The designation of     &#x03B1; = 2  /   (  N + 1  )    {\displaystyle \alpha
=2/\left(N+1\right)}  [{\displaystyle \alpha =2/\left(N+1\right)}] is not a
requirement. (For example, a similar proof could be used to just as easily
determine that the EMA with the same half-life as an N-day SMA is     &#x03B1;
= 1 &#x2212;  0.5  1  /  ( 0.5 N )     {\displaystyle \alpha =1-0.5^{1/(0.5N)}}
[{\displaystyle \alpha =1-0.5^{1/(0.5N)}}]). In fact, 2/(N+1) is merely a
common convention to form an intuitive understanding of the relationship
between EMAs and SMAs, for industries where both are commonly used together on
the same datasets. In reality, an EMA with any value of     &#x03B1;
{\displaystyle \alpha }  [\alpha ] can be used, and can be named either by
stating the value of     &#x03B1;   {\displaystyle \alpha }  [\alpha ], or with
the more familiar N-day EMA terminology letting     N =  (  2  /  &#x03B1;  )
&#x2212; 1   {\displaystyle N=\left(2/\alpha \right)-1}  [{\displaystyle
N=\left(2/\alpha \right)-1}].
**** Exponentially weighted moving variance and standard deviation[edit] ****
In addition to the mean, we may also be interested in the variance and in the
standard_deviation to evaluate the statistical_significance of a deviation from
the mean.
EWMVar can be computed easily along with the moving average. The starting
values are       EMA   1   =  x  1     {\displaystyle {\text{EMA}}_{1}=x_{1}}
[{\displaystyle {\text{EMA}}_{1}=x_{1}}] and       EMVar   1   = 0
{\displaystyle {\text{EMVar}}_{1}=0}  [{\displaystyle {\text{EMVar}}_{1}=0}],
and we then compute the subsequent values using:[13]
        &#x03B4;  i      =  x  i   &#x2212;   EMA   i &#x2212; 1         EMA
i      =   EMA   i &#x2212; 1   + &#x03B1; &#x22C5;  &#x03B4;  i         EMVar
i      =  (  1 &#x2212; &#x03B1;  )  &#x22C5;  (    EMVar   i &#x2212; 1   +
&#x03B1; &#x22C5;  &#x03B4;  i   2    )        {\displaystyle {\begin
{aligned}\delta _{i}&=x_{i}-{\text{EMA}}_{i-1}\\{\text{EMA}}_{i}&={\text{EMA}}_
{i-1}+\alpha \cdot \delta _{i}\\{\text{EMVar}}_{i}&=\left(1-\alpha \right)\cdot
\left({\text{EMVar}}_{i-1}+\alpha \cdot \delta _{i}^{2}\right)\end{aligned}}}
[{\displaystyle {\begin{aligned}\delta _{i}&=x_{i}-{\text{EMA}}_{i-1}\\{\text
{EMA}}_{i}&={\text{EMA}}_{i-1}+\alpha \cdot \delta _{i}\\{\text{EMVar}}_
{i}&=\left(1-\alpha \right)\cdot \left({\text{EMVar}}_{i-1}+\alpha \cdot \delta
_{i}^{2}\right)\end{aligned}}}]
From this, the exponentially weighted moving standard deviation can be computed
as       EWSD   i   =     EMVar   i       {\displaystyle {\text{EWSD}}_{i}=
{\sqrt {{\text{EMVar}}_{i}}}}  [{\displaystyle {\text{EWSD}}_{i}={\sqrt {{\text
{EMVar}}_{i}}}}]. We can then use the standard_score to normalize data with
respect to the moving average and variance. This algorithm is based on
Welford's_algorithm_for_computing_the_variance.
**** Modified moving average[edit] ****
A modified moving average (MMA), running moving average (RMA), or smoothed
moving average (SMMA) is defined as:
            p &#x00AF;    M M ,  today    =    ( N &#x2212; 1 )    p &#x00AF;
      M M ,  yesterday    +  p  today    N     {\displaystyle {\overline {p}}_
      {MM,{\text{today}}}={\frac {(N-1){\overline {p}}_{MM,{\text
      {yesterday}}}+p_{\text{today}}}{N}}}  [{\displaystyle {\overline {p}}_
      {MM,{\text{today}}}={\frac {(N-1){\overline {p}}_{MM,{\text
      {yesterday}}}+p_{\text{today}}}{N}}}]
In short, this is an exponential moving average, with     &#x03B1; = 1  /  N
{\displaystyle \alpha =1/N}  [{\displaystyle \alpha =1/N}].
**** Application to measuring computer performance[edit] ****
Some computer performance metrics, e.g. the average process queue length, or
the average CPU utilization, use a form of exponential moving average.
          S  n   = &#x03B1; (  t  n   &#x2212;  t  n &#x2212; 1   )  Y  n   +
      [  1 &#x2212; &#x03B1; (  t  n   &#x2212;  t  n &#x2212; 1   )  ]   S  n
      &#x2212; 1   .   {\displaystyle S_{n}=\alpha (t_{n}-t_{n-1})Y_{n}+\left
      [1-\alpha (t_{n}-t_{n-1})\right]S_{n-1}.}  [{\displaystyle S_{n}=\alpha
      (t_{n}-t_{n-1})Y_{n}+\left[1-\alpha (t_{n}-t_{n-1})\right]S_{n-1}.}]
Here α is defined as a function of time between two readings. An example of a
coefficient giving bigger weight to the current reading, and smaller weight to
the older readings is
         &#x03B1; (  t  n   &#x2212;  t  n &#x2212; 1   ) = 1 &#x2212; exp
      &#x2061;  (  &#x2212;     t  n   &#x2212;  t  n &#x2212; 1     W &#x22C5;
      60     )    {\displaystyle \alpha (t_{n}-t_{n-1})=1-\exp \left({-{\frac
      {t_{n}-t_{n-1}}{W\cdot 60}}}\right)}  [{\displaystyle \alpha (t_{n}-t_{n-
      1})=1-\exp \left({-{\frac {t_{n}-t_{n-1}}{W\cdot 60}}}\right)}]
where exp() is the exponential_function, time for readings tn is expressed in
seconds, and W is the period of time in minutes over which the reading is said
to be averaged (the mean lifetime of each reading in the average). Given the
above definition of α, the moving average can be expressed as
          S  n   =  [  1 &#x2212; exp &#x2061;  (  &#x2212;     t  n   &#x2212;
      t  n &#x2212; 1     W &#x22C5; 60     )   ]   Y  n   + exp &#x2061;
      (  &#x2212;     t  n   &#x2212;  t  n &#x2212; 1     W &#x22C5; 60     )
      S  n &#x2212; 1     {\displaystyle S_{n}=\left[1-\exp \left(-{{t_{n}-t_
      {n-1}} \over {W\cdot 60}}\right)\right]Y_{n}+\exp \left(-{{t_{n}-t_{n-1}}
      \over {W\cdot 60}}\right)S_{n-1}}  [{\displaystyle S_{n}=\left[1-\exp
      \left(-{{t_{n}-t_{n-1}} \over {W\cdot 60}}\right)\right]Y_{n}+\exp \left
      (-{{t_{n}-t_{n-1}} \over {W\cdot 60}}\right)S_{n-1}}]
For example, a 15-minute average L of a process queue length Q, measured every
5 seconds (time difference is 5 seconds), is computed as
              L  n      =  [  1 &#x2212; exp &#x2061;  (  &#x2212;   5  15
      &#x22C5; 60     )   ]   Q  n   +  e  &#x2212;   5  15 &#x22C5; 60       L
      n &#x2212; 1         =  [  1 &#x2212; exp &#x2061;  (  &#x2212;   1 180
      )   ]   Q  n   +  e  &#x2212;   1 180      L  n &#x2212; 1         =  Q
      n   +  e  &#x2212;   1 180      (   L  n &#x2212; 1   &#x2212;  Q  n    )
      {\displaystyle {\begin{aligned}L_{n}&=\left[1-\exp \left({-{\frac {5}
      {15\cdot 60}}}\right)\right]Q_{n}+e^{-{\frac {5}{15\cdot 60}}}L_{n-1}\\
      [6pt]&=\left[1-\exp \left({-{\frac {1}{180}}}\right)\right]Q_{n}+e^{-
      {\frac {1}{180}}}L_{n-1}\\[6pt]&=Q_{n}+e^{-{\frac {1}{180}}}\left(L_{n-
      1}-Q_{n}\right)\end{aligned}}}  [{\displaystyle {\begin{aligned}L_
      {n}&=\left[1-\exp \left({-{\frac {5}{15\cdot 60}}}\right)\right]Q_{n}+e^
      {-{\frac {5}{15\cdot 60}}}L_{n-1}\\[6pt]&=\left[1-\exp \left({-{\frac {1}
      {180}}}\right)\right]Q_{n}+e^{-{\frac {1}{180}}}L_{n-1}\\[6pt]&=Q_{n}+e^
      {-{\frac {1}{180}}}\left(L_{n-1}-Q_{n}\right)\end{aligned}}}]
***** Other weightings[edit] *****
Other weighting systems are used occasionally â for example, in share trading
a volume weighting will weight each time period in proportion to its trading
volume.
A further weighting, used by actuaries, is Spencer's 15-Point Moving Average
[14] (a central moving average). The symmetric weight coefficients are â3,
â6, â5, 3, 21, 46, 67, 74, 67, 46, 21, 3, â5, â6, â3.
Outside the world of finance, weighted running means have many forms and
applications. Each weighting function or "kernel" has its own characteristics.
In engineering and science the frequency and phase response of the filter is
often of primary importance in understanding the desired and undesired
distortions that a particular filter will apply to the data.
A mean does not just "smooth" the data. A mean is a form of low-pass filter.
The effects of the particular filter used should be understood in order to make
an appropriate choice. On this point, the French version of this article
discusses the spectral effects of 3 kinds of means (cumulative, exponential,
Gaussian).
***** Moving median[edit] *****
From a statistical point of view, the moving average, when used to estimate the
underlying trend in a time series, is susceptible to rare events such as rapid
shocks or other anomalies. A more robust estimate of the trend is the simple
moving median over n time points:
             p &#x007E;     SM   =  Median  (  p  M   ,  p  M &#x2212; 1   ,
      &#x2026; ,  p  M &#x2212; n + 1   )   {\displaystyle {\widetilde {p}}_
      {\text{SM}}={\text{Median}}(p_{M},p_{M-1},\ldots ,p_{M-n+1})}  [
      {\displaystyle {\widetilde {p}}_{\text{SM}}={\text{Median}}(p_{M},p_{M-
      1},\ldots ,p_{M-n+1})}]
where the median is found by, for example, sorting the values inside the
brackets and finding the value in the middle. For larger values of n, the
median can be efficiently computed by updating an indexable_skiplist.[15]
Statistically, the moving average is optimal for recovering the underlying
trend of the time series when the fluctuations about the trend are normally
distributed. However, the normal distribution does not place high probability
on very large deviations from the trend which explains why such deviations will
have a disproportionately large effect on the trend estimate. It can be shown
that if the fluctuations are instead assumed to be Laplace_distributed, then
the moving median is statistically optimal.[16] For a given variance, the
Laplace distribution places higher probability on rare events than does the
normal, which explains why the moving median tolerates shocks better than the
moving mean.
When the simple moving median above is central, the smoothing is identical to
the median_filter which has applications in, for example, image signal
processing.
***** Moving average regression model[edit] *****
Main article: Moving-average_model
In a moving_average_regression_model, a variable of interest is assumed to be a
weighted moving average of unobserved independent error terms; the weights in
the moving average are parameters to be estimated.
Those two concepts are often confused due to their name, but while they share
many similarities, they represent distinct methods and are used in very
different contexts.
***** See also[edit] *****
 Wikimedia Commons has media related to Moving_averages.
    * Exponential_smoothing
    * Moving_average_convergence/divergence_indicator
    * Window_function
    * Moving_average_crossover
    * Rising_moving_average
    * Running_total
    * Local_regression
    * Kernel_smoothing
    * Moving_least_squares
    * Zero_lag_exponential_moving_average
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (February 2010)(Learn_how_and
 when_to_remove_this_template_message)
***** Notes and references[edit] *****
   1. ^ Hydrologic_Variability_of_the_Cosumnes_River_Floodplain (Booth et al.,
      San Francisco Estuary and Watershed Science, Volume 4, Issue 2, 2006)
   2. ^ Statistical Analysis, Ya-lun Chou, Holt International, 1975,
   3. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   4. ISBN 0-03-089422-0, section 17.9.
   5. ^ The derivation and properties of the simple central moving average are
      given in full at SavitzkyâGolay_filter.
   6. ^"Weighted_Moving_Averages:_The_Basics". Investopedia.
   7. ^"Archived_copy". Archived from the_original on 2010-03-29. Retrieved
      2010-10-26.CS1 maint: Archived copy as title (link)
   8. ^ NIST/SEMATECH_e-Handbook_of_Statistical_Methods:_Single_Exponential
      Smoothing at the National_Institute_of_Standards_and_Technology
   9. ^  The Maclaurin_Series for     1  /  ( 1 &#x2212; x )   {\displaystyle
      1/(1-x)}  [{\displaystyle 1/(1-x)}] is     1 + x +  x  2   + &#x22EF;
      {\displaystyle 1+x+x^{2}+\cdots }  [{\displaystyle 1+x+x^{2}+\cdots }]
  10. ^ It means     &#x03B1; &#x2192; 0   {\displaystyle \alpha \to 0}
      [\alpha \to 0], and the Taylor_series of     log &#x2061; ( 1 &#x2212;
      &#x03B1; ) = &#x2212; &#x03B1; &#x2212;  &#x03B1;  2    /  2 &#x2212;
      &#x22EF;   {\displaystyle \log(1-\alpha )=-\alpha -\alpha ^{2}/2-\cdots }
      [{\displaystyle \log(1-\alpha )=-\alpha -\alpha ^{2}/2-\cdots }]
      approaches     &#x2212; &#x03B1;   {\displaystyle -\alpha }  [-\alpha ].
  11. ^ loge(0.001) / 2 = â3.45
  12. ^ See the following link for a proof.
  13. ^ The denominator on the left-hand side should be unity, and the
      numerator will become the right-hand side (geometric_series),
      &#x03B1;  [    1 &#x2212; ( 1 &#x2212; &#x03B1;  )  N + 1     1 &#x2212;
      ( 1 &#x2212; &#x03B1; )    ]    {\displaystyle \alpha \left[{1-(1-\alpha
      )^{N+1} \over 1-(1-\alpha )}\right]}  [{\displaystyle \alpha \left[{1-(1-
      \alpha )^{N+1} \over 1-(1-\alpha )}\right]}].
  14. ^ Because (1 + x/n)n tends to the limit ex for large n.
  15. ^Finch, Tony. "Incremental_calculation_of_weighted_mean_and_variance"
      (PDF). University of Cambridge. Retrieved 28 March 2018.
  16. ^ Spencer's_15-Point_Moving_Average_â_from_Wolfram_MathWorld
  17. ^ http://code.activestate.com/recipes/576930/
  18. ^ G.R. Arce, "Nonlinear Signal Processing: A Statistical Approach",
      Wiley:New Jersey, USA, 2005.
***** External links[edit] *****
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
Technical_analysis
               * Breakout
               * Dead_cat_bounce
Concepts       * Dow_theory
               * Elliott_wave_principle
               * Market_trend
               * Candlestick
               * Renko
Charts         * Kagi
               * Line
               * Open-high-low-close
               * Point_and_figure
                           * Broadening_top
                           * Cup_and_handle
                           * Double_top_and_double_bottom
                           * Flag_and_pennant
                           * Gap
           Chart           * Head_and_shoulders
                           * Island_reversal
                           * Price_channels
                           * Triangle
                           * Triple_top_and_triple_bottom
Patterns                   * Wedge_pattern
                                   * Doji
                                   * Hammer
                                   * Hanging_man
                       Simple      * Inverted_hammer
                                   * Marubozu
           Candlestick             * Shooting_star
                                   * Spinning_top
                                   * Hikkake_pattern
                       Complex     * Morning_star
                                   * Three_black_crows
                                   * Three_white_soldiers
                          * Bottom
           Support_&      * Fibonacci_retracement
           resistance     * Pivot_point (PP)
                          * Top
                          * Average_directional_index (A.D.X.)
                          * Commodity_channel_index (CCI)
                          * Detrended_price_oscillator (DPO)
                          * Know_sure_thing_oscillator (KST)
                          * Ichimoku_KinkÅ_HyÅ
                          * Moving_average_convergence/divergence (MACD)
           Trend          * Mass_index
                          * Moving average (MA)
                          * Parabolic_SAR (SAR)
                          * Smart_money_index (SMI)
                          * Trend_line
                          * Trix
                          * Vortex_indicator (VI)
                          * Money_flow_index (MFI)
                          * Relative_strength_index (RSI)
           Momentum       * Stochastic_oscillator
Indicators                * True_strength_index (TSI)
                          * Ultimate_oscillator
                          * Williams_%R (%R)
                          * Accumulation/distribution_line
                          * Ease_of_movement (EMV)
                          * Force_index (FI)
           Volume         * Negative_volume_index (NVI)
                          * On-balance_volume (OBV)
                          * Put/call_ratio (PCR)
                          * Volumeâprice_trend (VPT)
                          * Average_true_range (ATR)
                          * Bollinger_Bands (BB)
           Volatility     * Donchian_channel
                          * Keltner_channel
                          * CBOE_Market_Volatility_Index (VIX)
                          * Standard_deviation (Ï)
                          * Advanceâdecline_line (ADL)
           Breadth        * Arms_index (TRIN)
                          * McClellan_oscillator
           Other          * Coppock_curve
                          * Ulcer_index
    * v
    * t
    * e
Quantitative forecasting methods
Historical data forecasts
    * Moving average
    * Exponential_smoothing
    * Trend_analysis
    * Decomposition_of_time_series
    * NaÃ¯ve_approach
Associative (causal) forecasts
Moving average
Simple_linear_regression
Regression_analysis
Econometric_model

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Moving_average&oldid=909561999"
Categories:
    * Statistical_charts_and_diagrams
    * Time_series
    * Chart_overlays
    * Technical_analysis
Hidden categories:
    * CS1_maint:_Archived_copy_as_title
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_February_2018
    * Commons_category_link_is_on_Wikidata
    * Articles_lacking_in-text_citations_from_February_2010
    * All_articles_lacking_in-text_citations
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * ×¢××¨××ª
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * Tagalog
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 6 August 2019, at 05:39 (UTC).
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
