The following text has been accessed from https://en.wikipedia.org/wiki/Poisson_distribution at Thu Aug 8 22:52:14 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Poisson distribution ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
                                    Poisson
Probability mass function
[Poisson_pmf.svg]
The horizontal axis is the index k, the number of occurrences. Î» is the
expected number of occurrences, which need not be an integer. The vertical axis
is the probability of k occurrences given Î». The function is defined only at
integer values of k. The connecting lines are only guides for the eye.
Cumulative distribution function
[Poisson_cdf.svg]
The horizontal axis is the index k, the number of occurrences. The CDF is
discontinuous at the integers of k and flat everywhere else because a variable
that is Poisson distributed takes on only integer values.
Parameters            &#x03BB; > 0 ,   {\displaystyle \lambda >0,}  [
                   {\displaystyle \lambda >0,}] (real) â rate
Support               k &#x2208; { 0 , 1 , 2 , &#x2026; }   {\displaystyle k\in
                   \{0,1,2,\ldots \}}  [{\displaystyle k\in \{0,1,2,\ldots \}}]
                          &#x03BB;  k    e  &#x2212; &#x03BB;     k !
pmf                {\displaystyle {\frac {\lambda ^{k}e^{-\lambda }}{k!}}}  [
                   {\displaystyle {\frac {\lambda ^{k}e^{-\lambda }}{k!}}}]
                         &#x0393; ( &#x230A; k + 1 &#x230B; , &#x03BB; )
                   &#x230A; k &#x230B; !      {\displaystyle {\frac {\Gamma
                   (\lfloor k+1\rfloor ,\lambda )}{\lfloor k\rfloor !}}}  [
                   {\frac {\Gamma (\lfloor k+1\rfloor ,\lambda )}{\lfloor
                   k\rfloor !}}], or      e  &#x2212; &#x03BB;    &#x2211;  i =
                   0   &#x230A; k &#x230B;      &#x03BB;  i    i !    &#xA0;
                   {\displaystyle e^{-\lambda }\sum _{i=0}^{\lfloor k\rfloor }
                   {\frac {\lambda ^{i}}{i!}}\ }  [e^{-\lambda }\sum _{i=0}^
CDF                {\lfloor k\rfloor }{\frac {\lambda ^{i}}{i!}}\ ], or     Q
                   ( &#x230A; k + 1 &#x230B; , &#x03BB; )   {\displaystyle Q
                   (\lfloor k+1\rfloor ,\lambda )}  [Q(\lfloor k+1\rfloor
                   ,\lambda )] (for     k &#x2265; 0   {\displaystyle k\geq 0}
                   [k\geq 0], where     &#x0393; ( x , y )   {\displaystyle
                   \Gamma (x,y)}  [\Gamma (x,y)] is the upper_incomplete_gamma
                   function,     &#x230A; k &#x230B;   {\displaystyle \lfloor
                   k\rfloor }  [\lfloor k\rfloor ] is the floor_function, and Q
                   is the regularized_gamma_function)
Mean                  &#x03BB;   {\displaystyle \lambda }  [\lambda ]
                      &#x2248; &#x230A; &#x03BB; + 1  /  3 &#x2212; 0.02  /
Median             &#x03BB; &#x230B;   {\displaystyle \approx \lfloor \lambda
                   +1/3-0.02/\lambda \rfloor }  [\approx \lfloor \lambda +1/3-
                   0.02/\lambda \rfloor ]
                      &#x2308; &#x03BB; &#x2309; &#x2212; 1 , &#x230A; &#x03BB;
Mode               &#x230B;   {\displaystyle \lceil \lambda \rceil -1,\lfloor
                   \lambda \rfloor }  [\lceil \lambda \rceil -1,\lfloor \lambda
                   \rfloor ]
Variance              &#x03BB;   {\displaystyle \lambda }  [\lambda ]
Skewness               &#x03BB;  &#x2212; 1  /  2     {\displaystyle \lambda ^
                   {-1/2}}  [\lambda ^{-1/2}]
Ex._kurtosis           &#x03BB;  &#x2212; 1     {\displaystyle \lambda ^{-1}}
                   [\lambda ^{-1}]
                      &#x03BB; [ 1 &#x2212; log &#x2061; ( &#x03BB; ) ] +  e
                   &#x2212; &#x03BB;    &#x2211;  k = 0   &#x221E;
                   &#x03BB;  k   log &#x2061; ( k ! )   k !      {\displaystyle
                   \lambda [1-\log(\lambda )]+e^{-\lambda }\sum _{k=0}^{\infty
                   }{\frac {\lambda ^{k}\log(k!)}{k!}}}  [\lambda [1-\log
                   (\lambda )]+e^{-\lambda }\sum _{k=0}^{\infty }{\frac
                   {\lambda ^{k}\log(k!)}{k!}}]
                   (for large     &#x03BB;   {\displaystyle \lambda }  [\lambda
                   ])
Entropy                  1 2   log &#x2061; ( 2 &#x03C0; e &#x03BB; ) &#x2212;
                   1  12 &#x03BB;    &#x2212;   1  24  &#x03BB;  2
                   &#x2212;     {\displaystyle {\frac {1}{2}}\log(2\pi e\lambda
                   )-{\frac {1}{12\lambda }}-{\frac {1}{24\lambda ^{2}}}-{}}  [
                   {\displaystyle {\frac {1}{2}}\log(2\pi e\lambda )-{\frac {1}
                   {12\lambda }}-{\frac {1}{24\lambda ^{2}}}-{}}]
                         19  360  &#x03BB;  3      + O  (   1  &#x03BB;  4
                   )    {\displaystyle \qquad {\frac {19}{360\lambda ^
                   {3}}}+O\left({\frac {1}{\lambda ^{4}}}\right)}  [\qquad
                   {\frac {19}{360\lambda ^{3}}}+O\left({\frac {1}{\lambda ^
                   {4}}}\right)]
                      exp &#x2061; ( &#x03BB; (  e  t   &#x2212; 1 ) )
MGF                {\displaystyle \exp(\lambda (e^{t}-1))}  [\exp(\lambda (e^
                   {t}-1))]
                      exp &#x2061; ( &#x03BB; (  e  i t   &#x2212; 1 ) )
CF                 {\displaystyle \exp(\lambda (e^{it}-1))}  [\exp(\lambda (e^
                   {it}-1))]
PGF                   exp &#x2061; ( &#x03BB; ( z &#x2212; 1 ) )
                   {\displaystyle \exp(\lambda (z-1))}  [\exp(\lambda (z-1))]
Fisher_information      1 &#x03BB;     {\displaystyle {\frac {1}{\lambda }}}
                   [\frac{1}{\lambda}]
In probability_theory and statistics, the Poisson distribution (French
pronunciation: ​[pwasÉÌ]; in English often rendered /ËpwÉËsÉn/), named
after French mathematician SimÃ©on_Denis_Poisson, is a discrete_probability
distribution that expresses the probability of a given number of events
occurring in a fixed interval of time or space if these events occur with a
known constant rate and independently of the time since the last event.[1] The
Poisson distribution can also be used for the number of events in other
specified intervals such as distance, area or volume.
For instance, an individual keeping track of the amount of mail they receive
each day may notice that they receive an average number of 4 letters per day.
If receiving any particular piece of mail does not affect the arrival times of
future pieces of mail, i.e., if pieces of mail from a wide range of sources
arrive independently of one another, then a reasonable assumption is that the
number of pieces of mail received in a day obeys a Poisson distribution.[2]
Other examples that may follow a Poisson distribution include the number of
phone calls received by a call center per hour and the number of decay events
per second from a radioactive source.
⁰
***** Contents *****
    * 1_Basics
          o 1.1_Example
          o 1.2_Assumptions_and_validity
          o 1.3_Probability_of_events_for_a_Poisson_distribution
                # 1.3.1_Examples_of_probability_for_Poisson_distributions
                # 1.3.2_Once_in_an_interval_events:_The_special_case_of_λ_=_1
                  and_k_=_0
          o 1.4_Examples_that_violate_the_Poisson_assumptions
          o 1.5_Poisson_regression_and_negative_binomial_regression
    * 2_History
    * 3_Definition
    * 4_Properties
          o 4.1_Descriptive_statistics
          o 4.2_Median
          o 4.3_Higher_moments
          o 4.4_Sums_of_Poisson-distributed_random_variables
          o 4.5_Other_properties
          o 4.6_Poisson_races
          o 4.7_Poisson_Approximation
    * 5_Related_distributions
    * 6_Occurrence
          o 6.1_Law_of_rare_events
          o 6.2_Poisson_point_process
          o 6.3_Other_applications_in_science
    * 7_Generating_Poisson-distributed_random_variables
    * 8_Parameter_estimation
          o 8.1_Maximum_likelihood
          o 8.2_Confidence_interval
          o 8.3_Bayesian_inference
          o 8.4_Simultaneous_estimation_of_multiple_Poisson_means
    * 9_Bivariate_Poisson_distribution
    * 10_Computer_software_for_the_Poisson_distribution
          o 10.1_Evaluating_the_Poisson_distribution
          o 10.2_Random_drawing_from_the_Poisson_distribution
    * 11_See_also
    * 12_References
          o 12.1_Citations
          o 12.2_Sources
    * 13_Further_reading
***** Basics[edit] *****
The Poisson distribution is popular for modelling the number of times an event
occurs in an interval of time or space.
**** Example[edit] ****
The Poisson distribution may be useful to model events such as
    * The number of meteorites greater than 1 meter diameter that strike Earth
      in a year
    * The number of patients arriving in an emergency room between 10 and 11 pm
    * The number of photons hitting a detector in a particular time interval
**** Assumptions and validity[edit] ****
The Poisson distribution is an appropriate model if the following assumptions
are true.
    * k is the number of times an event occurs in an interval and k can take
      values 0, 1, 2, ....
    * The occurrence of one event does not affect the probability that a second
      event will occur. That is, events occur independently.
    * The average rate at which events occur is constant.
    * Two events cannot occur at exactly the same instant; instead, at each
      very small sub-interval exactly one event either occurs or does not
      occur.
      Or
    * The actual probability distribution is given by a binomial_distribution
      and the number of trials is sufficiently bigger than the number of
      successes one is asking about (see Related_distributions).
If these conditions are true, then k is a Poisson random variable, and the
distribution of k is a Poisson distribution.
**** Probability of events for a Poisson distribution[edit] ****
An event can occur 0, 1, 2, ... times in an interval. The average number of
events in an interval is designated     &#x03BB;   {\displaystyle \lambda }
[\lambda ] (lambda).     &#x03BB;   {\displaystyle \lambda }  [\lambda ] is the
event rate, also called the rate parameter. The probability of observing k
events in an interval is given by the equation
         P ( k  &#xA0;events in interval  ) =  e  &#x2212; &#x03BB;
      &#x03BB;  k    k !      {\displaystyle P(k{\text{ events in
      interval}})=e^{-\lambda }{\frac {\lambda ^{k}}{k!}}}  [{\displaystyle P(k
      {\text{ events in interval}})=e^{-\lambda }{\frac {\lambda ^{k}}{k!}}}]
where
    *    &#x03BB;   {\displaystyle \lambda }  [\lambda ] is the average number
      of events per interval
    * e is the number 2.71828... (Euler's_number) the base of the natural
      logarithms
    * k takes values 0, 1, 2, ...
    * k! = k Ã (k â 1) Ã (k â 2) Ã ... Ã 2 Ã 1 is the factorial of k.
This equation is the probability_mass_function (PMF) for a Poisson
distribution.
Notice that this equation can be adapted if, instead of the average number of
events     &#x03BB;   {\displaystyle \lambda }  [\lambda ], we are given a time
rate     r   {\displaystyle r}  [r] for the events to happen. Then     &#x03BB;
= r t   {\displaystyle \lambda =rt}  [{\displaystyle \lambda =rt}] (with     r
{\displaystyle r}  [ r] in units of 1/time), and
         P ( k  &#xA0;events in interval&#xA0;  t ) =  e  &#x2212; r t      ( r
      t  )  k     k !      {\displaystyle P(k{\text{ events in interval }}t)=e^
      {-rt}{\frac {(rt)^{k}}{k!}}}  [{\displaystyle P(k{\text{ events in
      interval }}t)=e^{-rt}{\frac {(rt)^{k}}{k!}}}]
*** Examples of probability for Poisson distributions[edit] ***
On a particular river, overflow floods occur once every 100 years on average.
Calculate the probability of k = 0, 1, 2, 3, 4, 5, or 6 overflow floods in a
100-year interval, assuming the Poisson model is appropriate.
Because the average event rate is one overflow flood per 100 years, λ = 1
         P ( k  &#xA0;overflow floods in 100 years  ) =     &#x03BB;  k    e
      &#x2212; &#x03BB;     k !    =     1  k    e  &#x2212; 1     k !
      {\displaystyle P(k{\text{ overflow floods in 100 years}})={\frac {\lambda
      ^{k}e^{-\lambda }}{k!}}={\frac {1^{k}e^{-1}}{k!}}}  [{\displaystyle P(k
      {\text{ overflow floods in 100 years}})={\frac {\lambda ^{k}e^{-\lambda
      }}{k!}}={\frac {1^{k}e^{-1}}{k!}}}]
         P ( k = 0  &#xA0;overflow floods in 100 years  ) =     1  0    e
      &#x2212; 1     0 !    =    e  &#x2212; 1   1   &#x2248; 0.368
      {\displaystyle P(k=0{\text{ overflow floods in 100 years}})={\frac {1^
      {0}e^{-1}}{0!}}={\frac {e^{-1}}{1}}\approx 0.368}  [{\displaystyle P(k=0
      {\text{ overflow floods in 100 years}})={\frac {1^{0}e^{-1}}{0!}}={\frac
      {e^{-1}}{1}}\approx 0.368}]
         P ( k = 1  &#xA0;overflow flood in 100 years  ) =     1  1    e
      &#x2212; 1     1 !    =    e  &#x2212; 1   1   &#x2248; 0.368
      {\displaystyle P(k=1{\text{ overflow flood in 100 years}})={\frac {1^
      {1}e^{-1}}{1!}}={\frac {e^{-1}}{1}}\approx 0.368}  [{\displaystyle P(k=1
      {\text{ overflow flood in 100 years}})={\frac {1^{1}e^{-1}}{1!}}={\frac
      {e^{-1}}{1}}\approx 0.368}]
         P ( k = 2  &#xA0;overflow floods in 100 years  ) =     1  2    e
      &#x2212; 1     2 !    =    e  &#x2212; 1   2   &#x2248; 0.184
      {\displaystyle P(k=2{\text{ overflow floods in 100 years}})={\frac {1^
      {2}e^{-1}}{2!}}={\frac {e^{-1}}{2}}\approx 0.184}  [{\displaystyle P(k=2
      {\text{ overflow floods in 100 years}})={\frac {1^{2}e^{-1}}{2!}}={\frac
      {e^{-1}}{2}}\approx 0.184}]
The table below gives the probability for 0 to 6 overflow floods in a 100-year
period.
k P(k overflow floods in 100 years)
0 0.368
1 0.368
2 0.184
3 0.061
4 0.015
5 0.003
6 0.0005
Ugarte and colleagues report that the average number of goals in a World Cup
soccer match is approximately 2.5 and the Poisson model is appropriate.[3]
Because the average event rate is 2.5 goals per match, λ = 2.5.
         P ( k  &#xA0;goals in a match  ) =     2.5  k    e  &#x2212; 2.5     k
      !      {\displaystyle P(k{\text{ goals in a match}})={\frac {2.5^{k}e^{-
      2.5}}{k!}}}  [{\displaystyle P(k{\text{ goals in a match}})={\frac {2.5^
      {k}e^{-2.5}}{k!}}}]
         P ( k = 0  &#xA0;goals in a match  ) =     2.5  0    e  &#x2212; 2.5
      0 !    =    e  &#x2212; 2.5   1   &#x2248; 0.082   {\displaystyle P(k=0
      {\text{ goals in a match}})={\frac {2.5^{0}e^{-2.5}}{0!}}={\frac {e^{-
      2.5}}{1}}\approx 0.082}  [{\displaystyle P(k=0{\text{ goals in a
      match}})={\frac {2.5^{0}e^{-2.5}}{0!}}={\frac {e^{-2.5}}{1}}\approx
      0.082}]
         P ( k = 1  &#xA0;goal in a match  ) =     2.5  1    e  &#x2212; 2.5
      1 !    =    2.5  e  &#x2212; 2.5    1   &#x2248; 0.205   {\displaystyle P
      (k=1{\text{ goal in a match}})={\frac {2.5^{1}e^{-2.5}}{1!}}={\frac
      {2.5e^{-2.5}}{1}}\approx 0.205}  [{\displaystyle P(k=1{\text{ goal in a
      match}})={\frac {2.5^{1}e^{-2.5}}{1!}}={\frac {2.5e^{-2.5}}{1}}\approx
      0.205}]
         P ( k = 2  &#xA0;goals in a match  ) =     2.5  2    e  &#x2212; 2.5
      2 !    =    6.25  e  &#x2212; 2.5    2   &#x2248; 0.257   {\displaystyle
      P(k=2{\text{ goals in a match}})={\frac {2.5^{2}e^{-2.5}}{2!}}={\frac
      {6.25e^{-2.5}}{2}}\approx 0.257}  [{\displaystyle P(k=2{\text{ goals in a
      match}})={\frac {2.5^{2}e^{-2.5}}{2!}}={\frac {6.25e^{-2.5}}{2}}\approx
      0.257}]
The table below gives the probability for 0 to 7 goals in a match.
k P(k goals in a World Cup soccer match)
0 0.082
1 0.205
2 0.257
3 0.213
4 0.133
5 0.067
6 0.028
7 0.010
*** Once in an interval events: The special case of λ = 1 and k = 0[edit] ***
Suppose that astronomers estimate that large meteorites (above a certain size)
hit the earth on average once every 100 years (λ = 1 event per 100 years), and
that the number of meteorite hits follows a Poisson distribution. What is the
probability of k = 0 meteorite hits in the next 100 years?
         P ( k =  0 meteorites hit in next 100 years  ) =     1  0    e
      &#x2212; 1     0 !    =   1 e   &#x2248; 0.37   {\displaystyle P(k={\text
      {0 meteorites hit in next 100 years}})={\frac {1^{0}e^{-1}}{0!}}={\frac
      {1}{e}}\approx 0.37}  [{\displaystyle P(k={\text{0 meteorites hit in next
      100 years}})={\frac {1^{0}e^{-1}}{0!}}={\frac {1}{e}}\approx 0.37}]
Under these assumptions, the probability that no large meteorites hit the earth
in the next 100 years is roughly 0.37. The remaining 1 â 0.37 = 0.63 is the
probability of 1, 2, 3, or more large meteorite hits in the next 100 years. In
an example above, an overflow flood occurred once every 100 years (λ = 1). The
probability of no overflow floods in 100 years was roughly 0.37, by the same
calculation.
In general, if an event occurs on average once per interval (λ = 1), and the
events follow a Poisson distribution, then P(0 events in next interval) = 0.37.
In addition, P(exactly one event in next interval) = 0.37, as shown in the
table for overflow floods.
**** Examples that violate the Poisson assumptions[edit] ****
The number of students who arrive at the student_union per minute will likely
not follow a Poisson distribution, because the rate is not constant (low rate
during class time, high rate between class times) and the arrivals of
individual students are not independent (students tend to come in groups).
The number of magnitude 5 earthquakes per year in a country may not follow a
Poisson distribution if one large earthquake increases the probability of
aftershocks of similar magnitude.
Among patients admitted to the intensive care unit of a hospital, the number of
days that the patients spend in the ICU is not Poisson distributed because the
number of days cannot be zero. The distribution may be modeled using a Zero-
truncated_Poisson_distribution.
Count distributions in which the number of intervals with zero events is higher
than predicted by a Poisson model may be modeled using a Zero-inflated_model.
**** Poisson regression and negative binomial regression[edit] ****
Poisson_regression and negative binomial regression are useful for analyses
where the dependent (response) variable is the count (0, 1, 2, ...) of the
number of events or occurrences in an interval.
***** History[edit] *****
The distribution was first introduced by SimÃ©on_Denis_Poisson (1781â1840)
and published, together with his probability theory, in 1837 in his work
Recherches sur la probabilitÃ© des jugements en matiÃ¨re criminelle et en
matiÃ¨re civile ("Research on the Probability of Judgments in Criminal and
Civil Matters").[4] The work theorized about the number of wrongful convictions
in a given country by focusing on certain random_variables N that count, among
other things, the number of discrete occurrences (sometimes called "events" or
"arrivals") that take place during a time-interval of given length. The result
had been given previously by Abraham_de_Moivre (1711) in De Mensura Sortis seu;
de Probabilitate Eventuum in Ludis a Casu Fortuito Pendentibus in Philosophical
Transactions of the Royal Society, p. 219.[5]:157 This makes it an example of
Stigler's_law and it has prompted some authors to argue that the Poisson
distribution should bear the name of de Moivre.[6][7]
A practical application of this distribution was made by Ladislaus_Bortkiewicz
in 1898 when he was given the task of investigating the number of soldiers in
the Prussian army killed accidentally by horse kicks; this experiment
introduced the Poisson distribution to the field of reliability_engineering.[8]
***** Definition[edit] *****
A discrete random_variable X  is said to have a Poisson distribution with
parameter Î» > 0, if, for k = 0, 1, 2, ..., the probability_mass_function of X 
is given by:[9]
          f ( k ; &#x03BB; ) = Pr ( X = k ) =     &#x03BB;  k    e  &#x2212;
      &#x03BB;     k !    ,   {\displaystyle \!f(k;\lambda )=\Pr(X=k)={\frac
      {\lambda ^{k}e^{-\lambda }}{k!}},}  [\!f(k;\lambda )=\Pr(X=k)={\frac
      {\lambda ^{k}e^{-\lambda }}{k!}},]
where
    * e is Euler's_number (e = 2.71828...)
    * k! is the factorial of k.
The positive real_number Î» is equal to the expected_value of X and also to its
variance[10]
         &#x03BB; = E &#x2061; ( X ) = Var &#x2061; ( X ) .   {\displaystyle
      \lambda =\operatorname {E} (X)=\operatorname {Var} (X).}  [\lambda
      =\operatorname {E} (X)=\operatorname {Var} (X).]
The Poisson distribution can be applied to systems with a large_number_of
possible_events,_each_of_which_is_rare. How many such events will occur during
a fixed time interval? Under the right circumstances, this is a random number
with a Poisson distribution.
The conventional definition of the Poisson distribution contains two terms that
can easily overflow on computers: Î»k and k!. The fraction of Î»k to k! can
also produce a rounding error that is very large compared to eâÎ», and
therefore give an erroneous result. For numerical stability the Poisson
probability mass function should therefore be evaluated as
          f ( k ; &#x03BB; ) = exp &#x2061;  {  k ln &#x2061; &#x03BB; &#x2212;
      &#x03BB; &#x2212; ln &#x2061; &#x0393; ( k + 1 )  }  ,   {\displaystyle
      \!f(k;\lambda )=\exp \left\{{k\ln \lambda -\lambda -\ln \Gamma
      (k+1)}\right\},}  [\!f(k;\lambda )=\exp \left\{{k\ln \lambda -\lambda -
      \ln \Gamma (k+1)}\right\},]
which is mathematically equivalent but numerically stable. The natural
logarithm of the Gamma_function can be obtained using the lgamma function in
the C_(programming_language) standard library (C99 version) or R_(programming
language), the gammaln function in MATLAB or SciPy, or the log_gamma function
in Fortran 2008 and later.
***** Properties[edit] *****
**** Descriptive statistics[edit] ****
    * The expected_value and variance of a Poisson-distributed random variable
      are both equal to Î».
    * The coefficient_of_variation is       &#x03BB;  &#x2212; 1  /  2
      {\displaystyle \textstyle \lambda ^{-1/2}}  [\textstyle \lambda ^{-1/2}],
      while the index_of_dispersion is 1.[5]:157
    * The mean_absolute_deviation about the mean is[5]:157
               E &#x2061;  |  X &#x2212; &#x03BB;  |  = 2 exp &#x2061;
            ( &#x2212; &#x03BB; )    &#x03BB;  &#x230A; &#x03BB; &#x230B; + 1
            &#x230A; &#x03BB; &#x230B; !    .   {\displaystyle \operatorname
            {E} |X-\lambda |=2\exp(-\lambda ){\frac {\lambda ^{\lfloor \lambda
            \rfloor +1}}{\lfloor \lambda \rfloor !}}.}  [\operatorname {E} |X-
            \lambda |=2\exp(-\lambda ){\frac {\lambda ^{\lfloor \lambda \rfloor
            +1}}{\lfloor \lambda \rfloor !}}.]
    * The mode of a Poisson-distributed random variable with non-integer Î» is
      equal to      &#x230A; &#x03BB; &#x230B;    {\displaystyle \scriptstyle
      \lfloor \lambda \rfloor }  [\scriptstyle \lfloor \lambda \rfloor ], which
      is the largest integer less than or equal to Î». This is also written as
      floor(Î»). When Î» is a positive integer, the modes are Î» and Î» â 1.
    * All of the cumulants of the Poisson distribution are equal to the
      expected value Î». The nth factorial_moment of the Poisson distribution
      is Î»n.
    * The expected_value of a Poisson_process is sometimes decomposed into the
      product of intensity and exposure (or more generally expressed as the
      integral of an "intensity function" over time or space, sometimes
      described as âexposureâ).[11][12]
**** Median[edit] ****
Bounds for the median (Î½) of the distribution are known and are sharp:[13]
         &#x03BB; &#x2212; ln &#x2061; 2 &#x2264; &#x03BD; < &#x03BB; +   1 3
      .   {\displaystyle \lambda -\ln 2\leq \nu <\lambda +{\frac {1}{3}}.}
      [\lambda -\ln 2\leq \nu <\lambda +{\frac {1}{3}}.]
**** Higher moments[edit] ****
    * The higher moments mk of the Poisson distribution about the origin are
      Touchard_polynomials in Î»:
                m  k   =  &#x2211;  i = 0   k    &#x03BB;  i    {     k     i
            }  ,   {\displaystyle m_{k}=\sum _{i=0}^{k}\lambda ^{i}\left\{
            {\begin{matrix}k\\i\end{matrix}}\right\},}  [{\displaystyle m_
            {k}=\sum _{i=0}^{k}\lambda ^{i}\left\{{\begin{matrix}k\\i\end
            {matrix}}\right\},}]
      where the {braces} denote Stirling_numbers_of_the_second_kind.[14] The
      coefficients of the polynomials have a combinatorial meaning. In fact,
      when the expected value of the Poisson distribution is 1, then Dobinski's
      formula says that the nth moment equals the number of partitions_of_a_set
      of size n.
For the non-centered moments we define     B = k  /  &#x03BB;   {\displaystyle
B=k/\lambda }  [{\displaystyle B=k/\lambda }], then[15]
               E [  X  k    ]  1  /  k   &#x2264; C &#x22C5;   {    k  /  B
            if   B &#x2264; e     k  /  log &#x2061; B    if   B &#x2265; e
            {\displaystyle E[X^{k}]^{1/k}\leq C\cdot {\begin{cases}k/B&{\text
            {if}}\quad B\leq e\\k/\log B&{\text{if}}\quad B\geq e\end{cases}}}
            [{\displaystyle E[X^{k}]^{1/k}\leq C\cdot {\begin{cases}k/B&{\text
            {if}}\quad B\leq e\\k/\log B&{\text{if}}\quad B\geq e\end{cases}}}]
where     C   {\displaystyle C}  [C] is some absolute constant greater than 0.
**** Sums of Poisson-distributed random variables[edit] ****
      If      X  i   &#x223C; Pois &#x2061; (  &#x03BB;  i   )   {\displaystyle
      X_{i}\sim \operatorname {Pois} (\lambda _{i})}  [{\displaystyle X_{i}\sim
      \operatorname {Pois} (\lambda _{i})}] for     i = 1 , &#x2026; , n
      {\displaystyle i=1,\dotsc ,n}  [{\displaystyle i=1,\dotsc ,n}] are
      independent, and     &#x03BB; =  &#x2211;  i = 1   n    &#x03BB;  i
      {\displaystyle \lambda =\sum _{i=1}^{n}\lambda _{i}}  [\lambda =\sum _
      {i=1}^{n}\lambda _{i}], then     Y =  (   &#x2211;  i = 1   n    X  i
      )  &#x223C; Pois &#x2061; ( &#x03BB; )   {\displaystyle Y=\left(\sum _
      {i=1}^{n}X_{i}\right)\sim \operatorname {Pois} (\lambda )}  [Y=\left(\sum
      _{i=1}^{n}X_{i}\right)\sim \operatorname {Pois} (\lambda )].[16] A
      converse is Raikov's_theorem, which says that if the sum of two
      independent random variables is Poisson-distributed, then so are each of
      those two independent random variables.[17]
**** Other properties[edit] ****
    * The Poisson distributions are infinitely_divisible probability
      distributions.[18][5]:159
    * The directed KullbackâLeibler_divergence of Pois(Î»0) from Pois(Î») is
      given by
                D  KL   &#x2061; ( &#x03BB; &#x2223;  &#x03BB;  0   ) =
            &#x03BB;  0   &#x2212; &#x03BB; + &#x03BB; log &#x2061;   &#x03BB;
            &#x03BB;  0     .   {\displaystyle \operatorname {D} _{\text{KL}}
            (\lambda \mid \lambda _{0})=\lambda _{0}-\lambda +\lambda \log
            {\frac {\lambda }{\lambda _{0}}}.}  [{\displaystyle \operatorname
            {D} _{\text{KL}}(\lambda \mid \lambda _{0})=\lambda _{0}-\lambda
            +\lambda \log {\frac {\lambda }{\lambda _{0}}}.}]
    * Bounds for the tail probabilities of a Poisson random variable     X
      &#x223C; Pois &#x2061; ( &#x03BB; )   {\displaystyle X\sim \operatorname
      {Pois} (\lambda )}  [X\sim \operatorname {Pois} (\lambda )] can be
      derived using a Chernoff_bound argument.[19]
               P ( X &#x2265; x ) &#x2264;     e  &#x2212; &#x03BB;   ( e
            &#x03BB;  )  x     x  x     ,  &#xA0;for&#xA0;  x > &#x03BB;
            {\displaystyle P(X\geq x)\leq {\frac {e^{-\lambda }(e\lambda )^{x}}
            {x^{x}}},{\text{ for }}x>\lambda }  [P(X\geq x)\leq {\frac {e^{-
            \lambda }(e\lambda )^{x}}{x^{x}}},{\text{ for }}x>\lambda ],
               P ( X &#x2264; x ) &#x2264;     e  &#x2212; &#x03BB;   ( e
            &#x03BB;  )  x     x  x     ,  &#xA0;for&#xA0;  x < &#x03BB; .
            {\displaystyle P(X\leq x)\leq {\frac {e^{-\lambda }(e\lambda )^{x}}
            {x^{x}}},{\text{ for }}x<\lambda .}  [{\displaystyle P(X\leq x)\leq
            {\frac {e^{-\lambda }(e\lambda )^{x}}{x^{x}}},{\text{ for
            }}x<\lambda .}]
    * Inequalities that relate the distribution function of a Poisson random
      variable     X &#x223C; Pois &#x2061; ( &#x03BB; )   {\displaystyle X\sim
      \operatorname {Pois} (\lambda )}  [X\sim \operatorname {Pois} (\lambda )]
      to the standard Normal distribution function     &#x03A6; ( x )
      {\displaystyle \Phi (x)}  [\Phi (x)] are as follows:[20]
               &#x03A6;  (  sign &#x2061; ( k &#x2212; &#x03BB; )   2  D  KL
            &#x2061; ( k &#x2223; &#x03BB; )    )  < P ( X &#x2264; k ) <
            &#x03A6;  (  sign &#x2061; ( k &#x2212; &#x03BB; + 1 )   2  D  KL
            &#x2061; ( k + 1 &#x2223; &#x03BB; )    )  ,  &#xA0;for&#xA0;  k >
            0.   {\displaystyle \Phi \left(\operatorname {sign} (k-\lambda )
            {\sqrt {2\operatorname {D} _{\text{KL}}(k\mid \lambda )}}\right)<P
            (X\leq k)<\Phi \left(\operatorname {sign} (k-\lambda +1){\sqrt
            {2\operatorname {D} _{\text{KL}}(k+1\mid \lambda )}}\right),{\text
            { for }}k>0.}  [{\displaystyle \Phi \left(\operatorname {sign} (k-
            \lambda ){\sqrt {2\operatorname {D} _{\text{KL}}(k\mid \lambda
            )}}\right)<P(X\leq k)<\Phi \left(\operatorname {sign} (k-\lambda
            +1){\sqrt {2\operatorname {D} _{\text{KL}}(k+1\mid \lambda
            )}}\right),{\text{ for }}k>0.}]
            Where      D  KL   &#x2061; ( k &#x2223; &#x03BB; )
            {\displaystyle \operatorname {D} _{\text{KL}}(k\mid \lambda )}  [
            {\displaystyle \operatorname {D} _{\text{KL}}(k\mid \lambda )}] is
            the directed KullbackâLeibler_divergence, as described above.
**** Poisson races[edit] ****
Let     X &#x223C; Pois &#x2061; ( &#x03BB; )   {\displaystyle X\sim
\operatorname {Pois} (\lambda )}  [{\displaystyle X\sim \operatorname {Pois}
(\lambda )}] and     Y &#x223C; Pois &#x2061; ( &#x03BC; )   {\displaystyle
Y\sim \operatorname {Pois} (\mu )}  [{\displaystyle Y\sim \operatorname {Pois}
(\mu )}] be independent random variables, with     &#x03BB; < &#x03BC;
{\displaystyle \lambda <\mu }  [\lambda <\mu ], then we have that
            e  &#x2212; (   &#x03BC;   &#x2212;   &#x03BB;    )  2
      ( &#x03BB; + &#x03BC;  )  2      &#x2212;    e  &#x2212; ( &#x03BB; +
      &#x03BC; )    2   &#x03BB; &#x03BC;      &#x2212;    e  &#x2212;
      ( &#x03BB; + &#x03BC; )    4 &#x03BB; &#x03BC;    &#x2264; P ( X &#x2212;
      Y &#x2265; 0 ) &#x2264;  e  &#x2212; (   &#x03BC;   &#x2212;   &#x03BB;
      )  2       {\displaystyle {\frac {e^{-({\sqrt {\mu }}-{\sqrt {\lambda
      }})^{2}}}{(\lambda +\mu )^{2}}}-{\frac {e^{-(\lambda +\mu )}}{2{\sqrt
      {\lambda \mu }}}}-{\frac {e^{-(\lambda +\mu )}}{4\lambda \mu }}\leq P(X-
      Y\geq 0)\leq e^{-({\sqrt {\mu }}-{\sqrt {\lambda }})^{2}}}  [{\frac {e^{-
      ({\sqrt {\mu }}-{\sqrt {\lambda }})^{2}}}{(\lambda +\mu )^{2}}}-{\frac
      {e^{-(\lambda +\mu )}}{2{\sqrt {\lambda \mu }}}}-{\frac {e^{-(\lambda
      +\mu )}}{4\lambda \mu }}\leq P(X-Y\geq 0)\leq e^{-({\sqrt {\mu }}-{\sqrt
      {\lambda }})^{2}}]
The upper bound is proved using a standard Chernoff_bound.
The lower bound can be proved by noting that     P ( X &#x2212; Y &#x2265; 0
&#x2223; X + Y = i )   {\displaystyle P(X-Y\geq 0\mid X+Y=i)}  [{\displaystyle
P(X-Y\geq 0\mid X+Y=i)}] is the probability that     Z &#x2265;   i 2
{\displaystyle Z\geq {\frac {i}{2}}}  [Z\geq {\frac {i}{2}}], where     Z
&#x223C; Bin &#x2061;  (  i ,   &#x03BB;  &#x03BB; + &#x03BC;     )
{\displaystyle Z\sim \operatorname {Bin} \left(i,{\frac {\lambda }{\lambda +\mu
}}\right)}  [Z\sim \operatorname {Bin} \left(i,{\frac {\lambda }{\lambda +\mu
}}\right)], which is bounded below by       1  ( i + 1  )  2       e
(  &#x2212; i D  (  0.5 &#x2016;   &#x03BB;  &#x03BB; + &#x03BC;     )   )
{\displaystyle {\frac {1}{(i+1)^{2}}}e^{\left(-iD\left(0.5\|{\frac {\lambda }
{\lambda +\mu }}\right)\right)}}  [{\displaystyle {\frac {1}{(i+1)^{2}}}e^
{\left(-iD\left(0.5\|{\frac {\lambda }{\lambda +\mu }}\right)\right)}}], where
D   {\displaystyle D}  [D] is relative_entropy (See the entry on bounds_on
tails_of_binomial_distributions for details). Further noting that     X + Y
&#x223C; Pois &#x2061; ( &#x03BB; + &#x03BC; )   {\displaystyle X+Y\sim
\operatorname {Pois} (\lambda +\mu )}  [{\displaystyle X+Y\sim \operatorname
{Pois} (\lambda +\mu )}], and computing a lower bound on the unconditional
probability gives the result. More details can be found in the appendix of.[21]
**** Poisson Approximation[edit] ****
Assume      X  1   &#x223C; Pois &#x2061; (  &#x03BB;  1   ) ,  X  2   &#x223C;
Pois &#x2061; (  &#x03BB;  2   ) , &#x2026; ,  X  n   &#x223C; Pois &#x2061;
(  &#x03BB;  n   )   {\displaystyle X_{1}\sim \operatorname {Pois} (\lambda _
{1}),X_{2}\sim \operatorname {Pois} (\lambda _{2}),\dots ,X_{n}\sim
\operatorname {Pois} (\lambda _{n})}  [{\displaystyle X_{1}\sim \operatorname
{Pois} (\lambda _{1}),X_{2}\sim \operatorname {Pois} (\lambda _{2}),\dots ,X_
{n}\sim \operatorname {Pois} (\lambda _{n})}] where      &#x03BB;  1   +
&#x03BB;  2   + &#x22EF; +  &#x03BB;  n   = 1   {\displaystyle \lambda _
{1}+\lambda _{2}+\dots +\lambda _{n}=1}  [{\displaystyle \lambda _{1}+\lambda _
{2}+\dots +\lambda _{n}=1}], then[22]     (  X  1   ,  X  2   , &#x2026; ,  X
n   )   {\displaystyle (X_{1},X_{2},\dots ,X_{n})}  [{\displaystyle (X_{1},X_
{2},\dots ,X_{n})}] is Multinomially_Distributed     (  X  1   ,  X  2   ,
&#x2026; ,  X  n   ) &#x223C; Mult &#x2061; ( N ,  &#x03BB;  1   ,  &#x03BB;  2
, &#x2026; ,  &#x03BB;  n   )   {\displaystyle (X_{1},X_{2},\dots ,X_{n})\sim
\operatorname {Mult} (N,\lambda _{1},\lambda _{2},\dots ,\lambda _{n})}  [
{\displaystyle (X_{1},X_{2},\dots ,X_{n})\sim \operatorname {Mult} (N,\lambda _
{1},\lambda _{2},\dots ,\lambda _{n})}] conditioned on     N =  X  1   +  X  2
+ &#x2026;  X  n     {\displaystyle N=X_{1}+X_{2}+\dots X_{n}}  [{\displaystyle
N=X_{1}+X_{2}+\dots X_{n}}].
This means[23], among other things, that for any nonnegative function     f
(  x  1   ,  x  2   , &#x2026; ,  x  n   )   {\displaystyle f(x_{1},x_{2},\dots
,x_{n})}  [{\displaystyle f(x_{1},x_{2},\dots ,x_{n})}], if     (  Y  1   ,  Y
2   , &#x2026; ,  Y  n   ) &#x223C; Mult &#x2061; ( m ,  p  )   {\displaystyle
(Y_{1},Y_{2},\dots ,Y_{n})\sim \operatorname {Mult} (m,\mathbf {p} )}  [
{\displaystyle (Y_{1},Y_{2},\dots ,Y_{n})\sim \operatorname {Mult} (m,\mathbf
{p} )}] is multinomially distributed, then
         E &#x2061; [ f (  Y  1   ,  Y  2   , &#x2026; ,  Y  n   ) ] &#x2264; e
      m   E &#x2061; [ f (  X  1   ,  X  2   , &#x2026; ,  X  n   ) ]
      {\displaystyle \operatorname {E} [f(Y_{1},Y_{2},\dots ,Y_{n})]\leq e
      {\sqrt {m}}\operatorname {E} [f(X_{1},X_{2},\dots ,X_{n})]}  [
      {\displaystyle \operatorname {E} [f(Y_{1},Y_{2},\dots ,Y_{n})]\leq e
      {\sqrt {m}}\operatorname {E} [f(X_{1},X_{2},\dots ,X_{n})]}]
where     (  X  1   ,  X  2   , &#x2026; ,  X  n   ) &#x223C; Pois &#x2061;
(  p  )   {\displaystyle (X_{1},X_{2},\dots ,X_{n})\sim \operatorname {Pois}
(\mathbf {p} )}  [{\displaystyle (X_{1},X_{2},\dots ,X_{n})\sim \operatorname
{Pois} (\mathbf {p} )}].
The factor of     e   m     {\displaystyle e{\sqrt {m}}}  [{\displaystyle e
{\sqrt {m}}}] can be removed if     f   {\displaystyle f}  [f] is further
assumed to be monotonically increasing or decreasing.
***** Related distributions[edit] *****
    * If      X  1   &#x223C;  P o i s  (  &#x03BB;  1   )    {\displaystyle X_
      {1}\sim \mathrm {Pois} (\lambda _{1})\,}  [X_{1}\sim \mathrm {Pois}
      (\lambda _{1})\,] and      X  2   &#x223C;  P o i s  (  &#x03BB;  2   )
      {\displaystyle X_{2}\sim \mathrm {Pois} (\lambda _{2})\,}  [X_{2}\sim
      \mathrm {Pois} (\lambda _{2})\,] are independent, then the difference
      Y =  X  1   &#x2212;  X  2     {\displaystyle Y=X_{1}-X_{2}}  [Y=X_{1}-X_
      {2}] follows a Skellam_distribution.
    * If      X  1   &#x223C;  P o i s  (  &#x03BB;  1   )    {\displaystyle X_
      {1}\sim \mathrm {Pois} (\lambda _{1})\,}  [X_{1}\sim \mathrm {Pois}
      (\lambda _{1})\,] and      X  2   &#x223C;  P o i s  (  &#x03BB;  2   )
      {\displaystyle X_{2}\sim \mathrm {Pois} (\lambda _{2})\,}  [X_{2}\sim
      \mathrm {Pois} (\lambda _{2})\,] are independent, then the distribution
      of      X  1     {\displaystyle X_{1}}  [X_{1}] conditional on      X  1
      +  X  2     {\displaystyle X_{1}+X_{2}}  [X_{1}+X_{2}] is a binomial
      distribution.
      Specifically, given      X  1   +  X  2   = k   {\displaystyle X_{1}+X_
      {2}=k}  [X_{1}+X_{2}=k],       X  1   &#x223C;  B i n o m  ( k ,
      &#x03BB;  1    /  (  &#x03BB;  1   +  &#x03BB;  2   ) )   {\displaystyle
      \!X_{1}\sim \mathrm {Binom} (k,\lambda _{1}/(\lambda _{1}+\lambda _{2}))}
      [\!X_{1}\sim \mathrm {Binom} (k,\lambda _{1}/(\lambda _{1}+\lambda _
      {2}))].
      More generally, if X1, X2,..., Xn are independent Poisson random
      variables with parameters Î»1, Î»2,..., Î»n then
            given      &#x2211;  j = 1   n    X  j   = k ,   {\displaystyle
            \sum _{j=1}^{n}X_{j}=k,}  [\sum _{j=1}^{n}X_{j}=k,]      X  i
            &#x223C;  B i n o m   (  k ,    &#x03BB;  i     &#x2211;  j = 1   n
            &#x03BB;  j       )    {\displaystyle X_{i}\sim \mathrm {Binom}
            \left(k,{\frac {\lambda _{i}}{\sum _{j=1}^{n}\lambda _{j}}}\right)}
            [X_{i}\sim \mathrm {Binom} \left(k,{\frac {\lambda _{i}}{\sum _
            {j=1}^{n}\lambda _{j}}}\right)]. In fact,     {  X  i   } &#x223C;
            M u l t i n o m   (  k ,  {    &#x03BB;  i     &#x2211;  j = 1   n
            &#x03BB;  j      }   )    {\displaystyle \{X_{i}\}\sim \mathrm
            {Multinom} \left(k,\left\{{\frac {\lambda _{i}}{\sum _{j=1}^
            {n}\lambda _{j}}}\right\}\right)}  [\{X_{i}\}\sim \mathrm
            {Multinom} \left(k,\left\{{\frac {\lambda _{i}}{\sum _{j=1}^
            {n}\lambda _{j}}}\right\}\right)].
    * If     X &#x223C;  P o i s  ( &#x03BB; )    {\displaystyle X\sim \mathrm
      {Pois} (\lambda )\,}  [X\sim \mathrm {Pois} (\lambda )\,] and the
      distribution of     Y   {\displaystyle Y}  [Y], conditional on X = k, is
      a binomial_distribution,     Y &#x2223; ( X = k ) &#x223C;  B i n o m
      ( k , p )   {\displaystyle Y\mid (X=k)\sim \mathrm {Binom} (k,p)}  [Y\mid
      (X=k)\sim \mathrm {Binom} (k,p)], then the distribution of Y follows a
      Poisson distribution     Y &#x223C;  P o i s  ( &#x03BB; &#x22C5; p )
      {\displaystyle Y\sim \mathrm {Pois} (\lambda \cdot p)\,}  [Y\sim \mathrm
      {Pois} (\lambda \cdot p)\,]. In fact, if     {  Y  i   }   {\displaystyle
      \{Y_{i}\}}  [\{Y_{i}\}], conditional on X = k, follows a multinomial
      distribution,     {  Y  i   } &#x2223; ( X = k ) &#x223C;  M u l t i n o
      m   (  k ,  p  i    )    {\displaystyle \{Y_{i}\}\mid (X=k)\sim \mathrm
      {Multinom} \left(k,p_{i}\right)}  [\{Y_{i}\}\mid (X=k)\sim \mathrm
      {Multinom} \left(k,p_{i}\right)], then each      Y  i     {\displaystyle
      Y_{i}}  [Y_{i}] follows an independent Poisson distribution      Y  i
      &#x223C;  P o i s  ( &#x03BB; &#x22C5;  p  i   ) , &#x03C1; (  Y  i   ,
      Y  j   ) = 0   {\displaystyle Y_{i}\sim \mathrm {Pois} (\lambda \cdot p_
      {i}),\rho (Y_{i},Y_{j})=0}  [Y_{i}\sim \mathrm {Pois} (\lambda \cdot p_
      {i}),\rho (Y_{i},Y_{j})=0].
    * The Poisson distribution can be derived as a limiting case to the
      binomial distribution as the number of trials goes to infinity and the
      expected number of successes remains fixed â see law_of_rare_events
      below. Therefore, it can be used as an approximation of the binomial
      distribution if n is sufficiently large and p is sufficiently small.
      There is a rule of thumb stating that the Poisson distribution is a good
      approximation of the binomial distribution if n is at least 20 and p is
      smaller than or equal to 0.05, and an excellent approximation if
      n â¥ 100 and np â¤ 10.[24]
                F   B i n o m i a l    ( k ; n , p ) &#x2248;  F   P o i s s o
            n    ( k ; &#x03BB; = n p )    {\displaystyle F_{\mathrm {Binomial}
            }(k;n,p)\approx F_{\mathrm {Poisson} }(k;\lambda =np)\,}  [F_
            {\mathrm {Binomial} }(k;n,p)\approx F_{\mathrm {Poisson} }
            (k;\lambda =np)\,]
    * The Poisson distribution is a special_case of the discrete compound
      Poisson distribution (or stuttering Poisson distribution) with only a
      parameter.[25][26] The discrete compound Poisson distribution can be
      deduced from the limiting distribution of univariate multinomial
      distribution. It is also a special_case of a compound_Poisson
      distribution.
    * For sufficiently large values of Î», (say Î»>1000), the normal
      distribution with mean Î» and variance Î» (standard deviation
      &#x03BB;     {\displaystyle {\sqrt {\lambda }}}  [{\sqrt {\lambda }}]) is
      an excellent approximation to the Poisson distribution. If Î» is greater
      than about 10, then the normal distribution is a good approximation if an
      appropriate continuity_correction is performed, i.e., if P(X â¤ x),
      where x is a non-negative integer, is replaced by P(X â¤ x + 0.5).
                F   P o i s s o n    ( x ; &#x03BB; ) &#x2248;  F   n o r m a l
            ( x ; &#x03BC; = &#x03BB; ,  &#x03C3;  2   = &#x03BB; )
            {\displaystyle F_{\mathrm {Poisson} }(x;\lambda )\approx F_{\mathrm
            {normal} }(x;\mu =\lambda ,\sigma ^{2}=\lambda )\,}  [F_{\mathrm
            {Poisson} }(x;\lambda )\approx F_{\mathrm {normal} }(x;\mu =\lambda
            ,\sigma ^{2}=\lambda )\,]
    * Variance-stabilizing_transformation: When a variable is Poisson
      distributed, its square root is approximately normally distributed with
      expected value of about       &#x03BB;     {\displaystyle {\sqrt {\lambda
      }}}  [{\sqrt {\lambda }}] and variance of about 1/4.[27][5]:163 Under
      this transformation, the convergence to normality (as Î» increases) is
      far faster than the untransformed variable.[citation_needed] Other,
      slightly more complicated, variance stabilizing transformations are
      available,[5]:163 one of which is Anscombe_transform. See Data
      transformation_(statistics) for more general uses of transformations.
    * If for every t > 0 the number of arrivals in the time interval [0, t]
      follows the Poisson distribution with mean Î»t, then the sequence of
      inter-arrival times are independent and identically distributed
      exponential random variables having mean 1/Î».[28]
    * The cumulative_distribution_functions of the Poisson and chi-squared
      distributions are related in the following ways:[5]:171
                F  Poisson   ( k ; &#x03BB; ) = 1 &#x2212;  F   &#x03C7;  2
            ( 2 &#x03BB; ; 2 ( k + 1 ) )    &#xA0;integer&#xA0;  k ,
            {\displaystyle F_{\text{Poisson}}(k;\lambda )=1-F_{\chi ^{2}}
            (2\lambda ;2(k+1))\quad \quad {\text{ integer }}k,}  [F_{\text
            {Poisson}}(k;\lambda )=1-F_{\chi ^{2}}(2\lambda ;2(k+1))\quad \quad
            {\text{ integer }}k,]
      and[5]:153
               Pr ( X = k ) =  F   &#x03C7;  2     ( 2 &#x03BB; ; 2 ( k + 1 ) )
            &#x2212;  F   &#x03C7;  2     ( 2 &#x03BB; ; 2 k ) .
            {\displaystyle \Pr(X=k)=F_{\chi ^{2}}(2\lambda ;2(k+1))-F_{\chi ^
            {2}}(2\lambda ;2k).}  [\Pr(X=k)=F_{\chi ^{2}}(2\lambda ;2(k+1))-F_
            {\chi ^{2}}(2\lambda ;2k).]
***** Occurrence[edit] *****
Applications of the Poisson distribution can be found in many fields related to
counting:[29]
    * Telecommunication example: telephone calls arriving in a system.
    * Astronomy example: photons arriving at a telescope.
    * Chemistry example: the molar_mass_distribution of a living_polymerization
      [30]
    * Biology example: the number of mutations on a strand of DNA per unit
      length.
    * Management example: customers arriving at a counter or call centre.
    * Finance_and_insurance example: number of losses or claims occurring in a
      given period of time.
    * Earthquake_seismology example: an asymptotic Poisson model of seismic
      risk for large earthquakes.[31]
    * Radioactivity example: number of decays in a given time interval in a
      radioactive sample.
The Poisson distribution arises in connection with Poisson_processes. It
applies to various phenomena of discrete properties (that is, those that may
happen 0, 1, 2, 3, ... times during a given period of time or in a given area)
whenever the probability of the phenomenon happening is constant in time or
space. Examples of events that may be modelled as a Poisson distribution
include:
    * The number of soldiers killed by horse-kicks each year in each corps in
      the Prussian cavalry. This example was used in a book by Ladislaus
      Bortkiewicz (1868â1931).
    * The number of yeast cells used when brewing Guinness beer. This example
      was used by William_Sealy_Gosset (1876â1937).[32]
    * The number of phone calls arriving at a call_centre within a minute. This
      example was described by A.K._Erlang (1878 â 1929).
    * Internet traffic.
    * The number of goals in sports involving two competing teams.[33]
    * The number of deaths per year in a given age group.
    * The number of jumps in a stock price in a given time interval.
    * Under an assumption of homogeneity, the number of times a web_server is
      accessed per minute.
    * The number of mutations in a given stretch of DNA after a certain amount
      of radiation.
    * The proportion of cells that will be infected at a given multiplicity_of
      infection.
    * The number of bacteria in a certain amount of liquid.[34]
    * The arrival of photons on a pixel circuit at a given illumination and
      over a given time period.
    * The targeting of V-1_flying_bombs on London during World War II
      investigated by R. D. Clarke in 1946.[35][36]
Gallagher in 1976 showed that the counts of prime_numbers in short intervals
obey a Poisson distribution provided a certain version of an unproved
conjecture of Hardy and Littlewood is true.[37]
**** Law of rare events[edit] ****
Main article: Poisson_limit_theorem
Comparison of the Poisson distribution (black lines) and the binomial
distribution with n = 10 (red circles), n = 20 (blue circles), n = 1000 (green
circles). All distributions have a mean of 5. The horizontal axis shows the
number of events k. Notice that as n gets larger, the Poisson distribution
becomes an increasingly better approximation for the binomial distribution with
the same mean.
The rate of an event is related to the probability of an event occurring in
some small subinterval (of time, space or otherwise). In the case of the
Poisson distribution, one assumes that there exists a small enough subinterval
for which the probability of an event occurring twice is "negligible". With
this assumption one can derive the Poisson distribution from the Binomial one,
given only the information of expected number of total events in the whole
interval. Let this total number be     &#x03BB;   {\displaystyle \lambda }
[\lambda ]. Divide the whole interval into     n   {\displaystyle n}  [n]
subintervals      I  1   , &#x2026; ,  I  n     {\displaystyle I_{1},\dots ,I_
{n}}  [I_{1},\dots ,I_{n}] of equal size, such that     n   {\displaystyle n}
[n] >     &#x03BB;   {\displaystyle \lambda }  [\lambda ] (since we are
interested in only very small portions of the interval this assumption is
meaningful). This means that the expected number of events in an interval
I  i     {\displaystyle I_{i}}  [I_{i}] for each     i   {\displaystyle i}  [i]
is equal to     &#x03BB;  /  n   {\displaystyle \lambda /n}  [\lambda /n]. Now
we assume that the occurrence of an event in the whole interval can be seen as
a Bernoulli_trial, where the      i  t h     {\displaystyle i^{th}}  [i^{th}]
trial corresponds to looking whether an event happens at the subinterval      I
i     {\displaystyle I_{i}}  [I_{i}] with probability     &#x03BB;  /  n
{\displaystyle \lambda /n}  [\lambda /n]. The expected number of total events
in     n   {\displaystyle n}  [n] such trials would be     &#x03BB;
{\displaystyle \lambda }  [\lambda ], the expected number of total events in
the whole interval. Hence for each subdivision of the interval we have
approximated the occurrence of the event as a Bernoulli process of the form
B   ( n , &#x03BB;  /  n )   {\displaystyle {\textrm {B}}(n,\lambda /n)}  [
{\textrm {B}}(n,\lambda /n)]. As we have noted before we want to consider only
very small subintervals. Therefore, we take the limit as     n   {\displaystyle
n}  [n] goes to infinity. In this case the binomial distribution converges to
what is known as the Poisson distribution by the Poisson_limit_theorem.
In several of the above examplesâsuch as, the number of mutations in a given
sequence of DNAâthe events being counted are actually the outcomes of
discrete trials, and would more precisely be modelled using the binomial
distribution, that is
         X &#x223C;   B   ( n , p ) .    {\displaystyle X\sim {\textrm {B}}
      (n,p).\,}  [X\sim {\textrm {B}}(n,p).\,]
In such cases n is very large and p is very small (and so the expectation np is
of intermediate magnitude). Then the distribution may be approximated by the
less cumbersome Poisson distribution[citation_needed]
         X &#x223C;   Pois   ( n p ) .    {\displaystyle X\sim {\textrm {Pois}}
      (np).\,}  [X\sim {\textrm {Pois}}(np).\,]
This approximation is sometimes known as the law of rare events,[38] since each
of the n individual Bernoulli_events rarely occurs. The name may be misleading
because the total count of success events in a Poisson process need not be rare
if the parameter np is not small. For example, the number of telephone calls to
a busy switchboard in one hour follows a Poisson distribution with the events
appearing frequent to the operator, but they are rare from the point of view of
the average member of the population who is very unlikely to make a call to
that switchboard in that hour.
The word law is sometimes used as a synonym of probability_distribution, and
convergence in law means convergence in distribution. Accordingly, the Poisson
distribution is sometimes called the "law of small numbers" because it is the
probability distribution of the number of occurrences of an event that happens
rarely but has very many opportunities to happen. The Law of Small Numbers is a
book by Ladislaus_Bortkiewicz (Bortkevitch)[39] about the Poisson distribution,
published in 1898.
**** Poisson point process[edit] ****
Main article: Poisson_point_process
The Poisson distribution arises as the number of points of a Poisson_point
process located in some finite region. More specifically, if D is some region
space, for example Euclidean space Rd, for which |D|, the area, volume or, more
generally, the Lebesgue measure of the region is finite, and if N(D) denotes
the number of points in D, then
         P ( N ( D ) = k ) =    ( &#x03BB;  |  D  |   )  k    e  &#x2212;
      &#x03BB;  |  D  |      k !    .   {\displaystyle P(N(D)=k)={\frac {
      (\lambda |D|)^{k}e^{-\lambda |D|}}{k!}}.}  [P(N(D)=k)={\frac {(\lambda
      |D|)^{k}e^{-\lambda |D|}}{k!}}.]
**** Other applications in science[edit] ****
In a Poisson process, the number of observed occurrences fluctuates about its
mean Î» with a standard_deviation      &#x03C3;  k   =   &#x03BB;
{\displaystyle \sigma _{k}={\sqrt {\lambda }}}  [\sigma _{k}={\sqrt {\lambda
}}]. These fluctuations are denoted as Poisson noise or (particularly in
electronics) as shot_noise.
The correlation of the mean and standard deviation in counting independent
discrete occurrences is useful scientifically. By monitoring how the
fluctuations vary with the mean signal, one can estimate the contribution of a
single occurrence, even if that contribution is too small to be detected
directly. For example, the charge e on an electron can be estimated by
correlating the magnitude of an electric_current with its shot_noise. If N
electrons pass a point in a given time t on the average, the mean current is
I = e N  /  t   {\displaystyle I=eN/t}  [I=eN/t]; since the current
fluctuations should be of the order      &#x03C3;  I   = e   N    /  t
{\displaystyle \sigma _{I}=e{\sqrt {N}}/t}  [\sigma _{I}=e{\sqrt {N}}/t] (i.e.,
the standard deviation of the Poisson_process), the charge     e
{\displaystyle e}  [e] can be estimated from the ratio     t  &#x03C3;  I   2
/  I   {\displaystyle t\sigma _{I}^{2}/I}  [t\sigma _{I}^{2}/I].[citation
needed]
An everyday example is the graininess that appears as photographs are enlarged;
the graininess is due to Poisson fluctuations in the number of reduced silver
grains, not to the individual grains themselves. By correlating the graininess
with the degree of enlargement, one can estimate the contribution of an
individual grain (which is otherwise too small to be seen unaided).[citation
needed] Many other molecular applications of Poisson noise have been developed,
e.g., estimating the number density of receptor molecules in a cell_membrane.
         Pr (  N  t   = k ) = f ( k ; &#x03BB; t ) =     e  &#x2212; &#x03BB; t
      ( &#x03BB; t  )  k     k !    .   {\displaystyle \Pr(N_{t}=k)=f(k;\lambda
      t)={\frac {e^{-\lambda t}(\lambda t)^{k}}{k!}}.}  [{\displaystyle \Pr(N_
      {t}=k)=f(k;\lambda t)={\frac {e^{-\lambda t}(\lambda t)^{k}}{k!}}.}]
In Causal_Set theory the discrete elements of spacetime follow a Poisson
distribution in the volume.
***** Generating Poisson-distributed random variables[edit] *****
A simple algorithm to generate random Poisson-distributed numbers (pseudo-
random_number_sampling) has been given by Knuth (see References below):
algorithm poisson random number (Knuth):
    init:
         Let L â eâÎ», k â 0 and p â 1.
    do:
         k â k + 1.
         Generate uniform random number u in [0,1] and let p â p Ã u.
    while p > L.
    return k â 1.
The complexity is linear in the returned value k, which is Î» on average. There
are many other algorithms to improve this. Some are given in Ahrens & Dieter,
see Â§ References below.
For large values of Î», the value of L = eâÎ» may be so small that it is hard
to represent. This can be solved by a change to the algorithm which uses an
additional parameter STEP such that eâSTEP does not underflow:[citation
needed]
algorithm poisson random number (Junhao, based on Knuth):
    init:
         Let Î»Left â Î», k â 0 and p â 1.
    do:
         k â k + 1.
         Generate uniform random number u in (0,1) and let p â p Ã u.
         while p < 1 and Î»Left > 0:
              if Î»Left > STEP:
                   p â p Ã eSTEP
                   Î»Left â Î»Left â STEP
              else:
                   p â p Ã eÎ»Left
                   Î»Left â 0
    while p > 1.
    return k â 1.
The choice of STEP depends on the threshold of overflow. For double precision
floating point format, the threshold is near e700, so 500 shall be a safe STEP.
Other solutions for large values of Î» include rejection_sampling and using
Gaussian approximation.
Inverse_transform_sampling is simple and efficient for small values of Î», and
requires only one uniform random number u per sample. Cumulative probabilities
are examined in turn until one exceeds u.
algorithm Poisson generator based upon the inversion by sequential search:[40]
    init:
         Let x â 0, p â eâÎ», s â p.
         Generate uniform random number u in [0,1].
    while u > s do:
         x â x + 1.
         p â p * Î» / x.
         s â s + p.
    return x.
***** Parameter estimation[edit] *****
See also: Poisson_regression
**** Maximum likelihood[edit] ****
Given a sample of n measured values      k  i   &#x2208; { 0 , 1 , . . . }
{\displaystyle k_{i}\in \{0,1,...\}}  [{\displaystyle k_{i}\in \{0,1,...\}}],
for i = 1, ..., n, we wish to estimate the value of the parameter Î» of the
Poisson population from which the sample was drawn. The maximum_likelihood
estimate is [41]
             &#x03BB; &#x005E;      M L E    =   1 n    &#x2211;  i = 1   n
      k  i   .    {\displaystyle {\widehat {\lambda }}_{\mathrm {MLE} }={\frac
      {1}{n}}\sum _{i=1}^{n}k_{i}.\!}  [{\widehat {\lambda }}_{\mathrm {MLE} }=
      {\frac {1}{n}}\sum _{i=1}^{n}k_{i}.\!]
Since each observation has expectation Î» so does this sample mean. Therefore,
the maximum likelihood estimate is an unbiased_estimator of Î». It is also an
efficient estimator, i.e. its estimation variance achieves the CramÃ©râRao
lower_bound (CRLB).[citation_needed] Hence it is minimum-variance_unbiased.
Also it can be proven that the sum (and hence the sample mean as it is a one-
to-one function of the sum) is a complete and sufficient statistic for Î».
To prove sufficiency we may use the factorization_theorem. Consider
partitioning the probability mass function of the joint Poisson distribution
for the sample into two parts: one that depends solely on the sample      x
{\displaystyle \mathbf {x} }  [\mathbf {x} ] (called     h (  x  )
{\displaystyle h(\mathbf {x} )}  [h(\mathbf {x} )]) and one that depends on the
parameter     &#x03BB;   {\displaystyle \lambda }  [\lambda ] and the sample
x    {\displaystyle \mathbf {x} }  [\mathbf {x} ] only through the function
T (  x  )   {\displaystyle T(\mathbf {x} )}  [T(\mathbf {x} )]. Then     T (  x
)   {\displaystyle T(\mathbf {x} )}  [T(\mathbf {x} )] is a sufficient
statistic for     &#x03BB;   {\displaystyle \lambda }  [\lambda ].
         P (  x  ) =  &#x220F;  i = 1   n       &#x03BB;   x  i      e
      &#x2212; &#x03BB;      x  i   !    =   1   &#x220F;  i = 1   n    x  i
      !    &#x00D7;  &#x03BB;   &#x2211;  i = 1   n    x  i      e  &#x2212; n
      &#x03BB;     {\displaystyle P(\mathbf {x} )=\prod _{i=1}^{n}{\frac
      {\lambda ^{x_{i}}e^{-\lambda }}{x_{i}!}}={\frac {1}{\prod _{i=1}^{n}x_
      {i}!}}\times \lambda ^{\sum _{i=1}^{n}x_{i}}e^{-n\lambda }}  [
      {\displaystyle P(\mathbf {x} )=\prod _{i=1}^{n}{\frac {\lambda ^{x_{i}}e^
      {-\lambda }}{x_{i}!}}={\frac {1}{\prod _{i=1}^{n}x_{i}!}}\times \lambda ^
      {\sum _{i=1}^{n}x_{i}}e^{-n\lambda }}]
Note that the first term,     h (  x  )   {\displaystyle h(\mathbf {x} )}  [h
(\mathbf {x} )], depends only on      x    {\displaystyle \mathbf {x} }
[\mathbf {x} ]. The second term,     g ( T (  x  )  |  &#x03BB; )
{\displaystyle g(T(\mathbf {x} )|\lambda )}  [g(T(\mathbf {x} )|\lambda )],
depends on the sample only through     T (  x  ) =  &#x2211;  i = 1   n    x  i
{\displaystyle T(\mathbf {x} )=\sum _{i=1}^{n}x_{i}}  [T(\mathbf {x} )=\sum _
{i=1}^{n}x_{i}]. Thus,     T (  x  )   {\displaystyle T(\mathbf {x} )}  [T
(\mathbf {x} )] is sufficient.
To find the parameter Î» that maximizes the probability function for the
Poisson population, we can use the logarithm of the likelihood function:
             &#x2113; ( &#x03BB; )    = ln &#x2061;  &#x220F;  i = 1   n   f
      (  k  i   &#x2223; &#x03BB; )       =  &#x2211;  i = 1   n   ln   (     e
      &#x2212; &#x03BB;    &#x03BB;   k  i        k  i   !    )        =
      &#x2212; n &#x03BB; +  (   &#x2211;  i = 1   n    k  i    )  ln &#x2061;
      ( &#x03BB; ) &#x2212;  &#x2211;  i = 1   n   ln &#x2061; (  k  i   ! ) .
      {\displaystyle {\begin{aligned}\ell (\lambda )&=\ln \prod _{i=1}^{n}f(k_
      {i}\mid \lambda )\\&=\sum _{i=1}^{n}\ln \!\left({\frac {e^{-\lambda
      }\lambda ^{k_{i}}}{k_{i}!}}\right)\\&=-n\lambda +\left(\sum _{i=1}^{n}k_
      {i}\right)\ln(\lambda )-\sum _{i=1}^{n}\ln(k_{i}!).\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\ell (\lambda )&=\ln \prod _{i=1}^{n}f(k_
      {i}\mid \lambda )\\&=\sum _{i=1}^{n}\ln \!\left({\frac {e^{-\lambda
      }\lambda ^{k_{i}}}{k_{i}!}}\right)\\&=-n\lambda +\left(\sum _{i=1}^{n}k_
      {i}\right)\ln(\lambda )-\sum _{i=1}^{n}\ln(k_{i}!).\end{aligned}}}]
We take the derivative of    &#x2113;   {\displaystyle \ell }  [\ell ] with
respect to Î» and compare it to zero:
            d    d  &#x03BB;    &#x2113; ( &#x03BB; ) = 0  &#x27FA;  &#x2212; n
      +  (   &#x2211;  i = 1   n    k  i    )    1 &#x03BB;   = 0.
      {\displaystyle {\frac {\mathrm {d} }{\mathrm {d} \lambda }}\ell (\lambda
      )=0\iff -n+\left(\sum _{i=1}^{n}k_{i}\right){\frac {1}{\lambda }}=0.\!}
      [{\displaystyle {\frac {\mathrm {d} }{\mathrm {d} \lambda }}\ell (\lambda
      )=0\iff -n+\left(\sum _{i=1}^{n}k_{i}\right){\frac {1}{\lambda }}=0.\!}]
Solving for Î» gives a stationary point.
         &#x03BB; =     &#x2211;  i = 1   n    k  i    n     {\displaystyle
      \lambda ={\frac {\sum _{i=1}^{n}k_{i}}{n}}}  [\lambda ={\frac {\sum _
      {i=1}^{n}k_{i}}{n}}]
So Î» is the average of the ki values. Obtaining the sign of the second
derivative of L at the stationary point will determine what kind of extreme
value Î» is.
             &#x2202;  2   &#x2113;   &#x2202;  &#x03BB;  2      = &#x2212;
      &#x03BB;  &#x2212; 2    &#x2211;  i = 1   n    k  i     {\displaystyle
      {\frac {\partial ^{2}\ell }{\partial \lambda ^{2}}}=-\lambda ^{-2}\sum _
      {i=1}^{n}k_{i}}  [{\displaystyle {\frac {\partial ^{2}\ell }{\partial
      \lambda ^{2}}}=-\lambda ^{-2}\sum _{i=1}^{n}k_{i}}]
Evaluating the second derivative at the stationary point gives:
             &#x2202;  2   &#x2113;   &#x2202;  &#x03BB;  2      = &#x2212;
      n  2     &#x2211;  i = 1   n    k  i        {\displaystyle {\frac
      {\partial ^{2}\ell }{\partial \lambda ^{2}}}=-{\frac {n^{2}}{\sum _{i=1}^
      {n}k_{i}}}}  [{\displaystyle {\frac {\partial ^{2}\ell }{\partial \lambda
      ^{2}}}=-{\frac {n^{2}}{\sum _{i=1}^{n}k_{i}}}}]
which is the negative of n times the reciprocal of the average of the ki. This
expression is negative when the average is positive. If this is satisfied, then
the stationary point maximizes the probability function.
For completeness, a family of distributions is said to be complete if and only
if     E ( g ( T ) ) = 0   {\displaystyle E(g(T))=0}  [E(g(T))=0] implies that
P  &#x03BB;   ( g ( T ) = 0 ) = 1   {\displaystyle P_{\lambda }(g(T)=0)=1}  [P_
{\lambda }(g(T)=0)=1] for all     &#x03BB;   {\displaystyle \lambda }  [\lambda
]. If the individual      X  i     {\displaystyle X_{i}}  [X_{i}] are iid
P o  ( &#x03BB; )   {\displaystyle \mathrm {Po} (\lambda )}  [\mathrm {Po}
(\lambda )], then     T (  x  ) =  &#x2211;  i = 1   n    X  i   &#x223C;  P o
( n &#x03BB; )   {\displaystyle T(\mathbf {x} )=\sum _{i=1}^{n}X_{i}\sim
\mathrm {Po} (n\lambda )}  [T(\mathbf {x} )=\sum _{i=1}^{n}X_{i}\sim \mathrm
{Po} (n\lambda )]. Knowing the distribution we want to investigate, it is easy
to see that the statistic is complete.
         E ( g ( T ) ) =  &#x2211;  t = 0   &#x221E;   g ( t )    ( n &#x03BB;
      )  t    e  &#x2212; n &#x03BB;     t !    = 0   {\displaystyle E(g
      (T))=\sum _{t=0}^{\infty }g(t){\frac {(n\lambda )^{t}e^{-n\lambda }}
      {t!}}=0}  [E(g(T))=\sum _{t=0}^{\infty }g(t){\frac {(n\lambda )^{t}e^{-
      n\lambda }}{t!}}=0]
For this equality to hold,     g ( t )   {\displaystyle g(t)}  [g(t)] must be
0. This follows from the fact that none of the other terms will be 0 for all
t   {\displaystyle t}  [t] in the sum and for all possible values of
&#x03BB;   {\displaystyle \lambda }  [\lambda ]. Hence,     E ( g ( T ) ) = 0
{\displaystyle E(g(T))=0}  [E(g(T))=0] for all     &#x03BB;   {\displaystyle
\lambda }  [\lambda ] implies that      P  &#x03BB;   ( g ( T ) = 0 ) = 1
{\displaystyle P_{\lambda }(g(T)=0)=1}  [P_{\lambda }(g(T)=0)=1], and the
statistic has been shown to be complete.
**** Confidence interval[edit] ****
The confidence_interval for the mean of a Poisson distribution can be expressed
using the relationship between the cumulative distribution functions of the
Poisson and chi-squared_distributions. The chi-squared distribution is itself
closely related to the gamma_distribution, and this leads to an alternative
expression. Given an observation k from a Poisson distribution with mean Î¼, a
confidence interval for Î¼ with confidence level 1 â Î± is
            1 2     &#x03C7;  2   ( &#x03B1;  /  2 ; 2 k ) &#x2264; &#x03BC;
      &#x2264;    1 2     &#x03C7;  2   ( 1 &#x2212; &#x03B1;  /  2 ; 2 k + 2 )
      ,   {\displaystyle {\tfrac {1}{2}}\chi ^{2}(\alpha /2;2k)\leq \mu \leq
      {\tfrac {1}{2}}\chi ^{2}(1-\alpha /2;2k+2),}  [{\tfrac {1}{2}}\chi ^{2}
      (\alpha /2;2k)\leq \mu \leq {\tfrac {1}{2}}\chi ^{2}(1-\alpha /2;2k+2),]
or equivalently,
          F  &#x2212; 1   ( &#x03B1;  /  2 ; k , 1 ) &#x2264; &#x03BC; &#x2264;
      F  &#x2212; 1   ( 1 &#x2212; &#x03B1;  /  2 ; k + 1 , 1 ) ,
      {\displaystyle F^{-1}(\alpha /2;k,1)\leq \mu \leq F^{-1}(1-\alpha /
      2;k+1,1),}  [F^{-1}(\alpha /2;k,1)\leq \mu \leq F^{-1}(1-\alpha /
      2;k+1,1),]
where      &#x03C7;  2   ( p ; n )   {\displaystyle \chi ^{2}(p;n)}  [\chi ^{2}
(p;n)] is the quantile_function (corresponding to a lower tail area p) of the
chi-squared distribution with n degrees of freedom and      F  &#x2212; 1   ( p
; n , 1 )   {\displaystyle F^{-1}(p;n,1)}  [F^{-1}(p;n,1)] is the quantile
function of a Gamma_distribution with shape parameter n and scale parameter 1.
[5]:171[42] This interval is 'exact' in the sense that its coverage_probability
is never less than the nominal 1 â Î±.
When quantiles of the Gamma distribution are not available, an accurate
approximation to this exact interval has been proposed (based on the
WilsonâHilferty_transformation):[43]
         k   (  1 &#x2212;   1  9 k    &#x2212;    z  &#x03B1;  /  2    3   k
      )   3   &#x2264; &#x03BC; &#x2264; ( k + 1 )   (  1 &#x2212;   1  9 ( k +
      1 )    +    z  &#x03B1;  /  2    3   k + 1       )   3   ,
      {\displaystyle k\left(1-{\frac {1}{9k}}-{\frac {z_{\alpha /2}}{3{\sqrt
      {k}}}}\right)^{3}\leq \mu \leq (k+1)\left(1-{\frac {1}{9(k+1)}}+{\frac
      {z_{\alpha /2}}{3{\sqrt {k+1}}}}\right)^{3},}  [k\left(1-{\frac {1}{9k}}-
      {\frac {z_{\alpha /2}}{3{\sqrt {k}}}}\right)^{3}\leq \mu \leq (k+1)\left
      (1-{\frac {1}{9(k+1)}}+{\frac {z_{\alpha /2}}{3{\sqrt {k+1}}}}\right)^
      {3},]
where      z  &#x03B1;  /  2     {\displaystyle z_{\alpha /2}}  [z_{\alpha /2}]
denotes the standard_normal_deviate with upper tail area Î± / 2.
For application of these formulae in the same context as above (given a sample
of n measured values ki each drawn from a Poisson distribution with mean Î»),
one would set
         k =  &#x2211;  i = 1   n    k  i   ,    {\displaystyle k=\sum _{i=1}^
      {n}k_{i},\!}  [k=\sum _{i=1}^{n}k_{i},\!]
calculate an interval for Î¼ = nÎ», and then derive the interval for Î».
**** Bayesian inference[edit] ****
In Bayesian_inference, the conjugate_prior for the rate parameter Î» of the
Poisson distribution is the gamma_distribution.[44] Let
         &#x03BB; &#x223C;  G a m m a  ( &#x03B1; , &#x03B2; )
      {\displaystyle \lambda \sim \mathrm {Gamma} (\alpha ,\beta )\!}  [\lambda
      \sim \mathrm {Gamma} (\alpha ,\beta )\!]
denote that Î» is distributed according to the gamma density g parameterized in
terms of a shape_parameter Î± and an inverse scale_parameter Î²:
         g ( &#x03BB; &#x2223; &#x03B1; , &#x03B2; ) =    &#x03B2;  &#x03B1;
      &#x0393; ( &#x03B1; )      &#x03BB;  &#x03B1; &#x2212; 1     e  &#x2212;
      &#x03B2;  &#x03BB;     &#xA0;for&#xA0;  &#x03BB; > 0   .   {\displaystyle
      g(\lambda \mid \alpha ,\beta )={\frac {\beta ^{\alpha }}{\Gamma (\alpha
      )}}\;\lambda ^{\alpha -1}\;e^{-\beta \,\lambda }\qquad {\text{ for
      }}\lambda >0\,\!.}  [g(\lambda \mid \alpha ,\beta )={\frac {\beta ^
      {\alpha }}{\Gamma (\alpha )}}\;\lambda ^{\alpha -1}\;e^{-\beta \,\lambda
      }\qquad {\text{ for }}\lambda >0\,\!.]
Then, given the same sample of n measured values ki as_before, and a prior of
Gamma(Î±, Î²), the posterior distribution is
         &#x03BB; &#x223C;  G a m m a   (  &#x03B1; +  &#x2211;  i = 1   n    k
      i   , &#x03B2; + n  )  .    {\displaystyle \lambda \sim \mathrm {Gamma}
      \left(\alpha +\sum _{i=1}^{n}k_{i},\beta +n\right).\!}  [\lambda \sim
      \mathrm {Gamma} \left(\alpha +\sum _{i=1}^{n}k_{i},\beta +n\right).\!]
The posterior mean E[Î»] approaches the maximum likelihood estimate
&#x03BB; &#x005E;      M L E      {\displaystyle {\widehat {\lambda }}_{\mathrm
{MLE} }}  [{\widehat {\lambda }}_{\mathrm {MLE} }] in the limit as     &#x03B1;
&#x2192; 0 , &#xA0; &#x03B2; &#x2192; 0   {\displaystyle \alpha \to 0,\ \beta
\to 0}  [\alpha \to 0,\ \beta \to 0], which follows immediately from the
general expression of the mean of the gamma_distribution.
The posterior_predictive_distribution for a single additional observation is a
negative_binomial_distribution,[45] sometimes called a GammaâPoisson
distribution.
**** Simultaneous estimation of multiple Poisson means[edit] ****
Suppose      X  1   ,  X  2   , &#x2026; ,  X  p     {\displaystyle X_{1},X_
{2},\dots ,X_{p}}  [X_{1},X_{2},\dots ,X_{p}] is a set of independent random
variables from a set of     p   {\displaystyle p}  [p] Poisson distributions,
each with a parameter      &#x03BB;  i     {\displaystyle \lambda _{i}}
[\lambda _{i}],     i = 1 , &#x2026; , p   {\displaystyle i=1,\dots ,p}
[i=1,\dots ,p], and we would like to estimate these parameters. Then, Clevenson
and Zidek show that under the normalized squared error loss     L ( &#x03BB; ,
&#x03BB; &#x005E;    ) =  &#x2211;  i = 1   p    &#x03BB;  i   &#x2212; 1
(     &#x03BB; &#x005E;     i   &#x2212;  &#x03BB;  i    )  2
{\displaystyle L(\lambda ,{\hat {\lambda }})=\sum _{i=1}^{p}\lambda _{i}^{-1}(
{\hat {\lambda }}_{i}-\lambda _{i})^{2}}  [L(\lambda ,{\hat {\lambda }})=\sum _
{i=1}^{p}\lambda _{i}^{-1}({\hat {\lambda }}_{i}-\lambda _{i})^{2}], when     p
> 1   {\displaystyle p>1}  [p>1], then, similar as in Stein's_example for the
Normal means, the MLE estimator         &#x03BB; &#x005E;     i   =  X  i
{\displaystyle {\hat {\lambda }}_{i}=X_{i}}  [{\hat {\lambda }}_{i}=X_{i}] is
inadmissible.[46]
In this case, a family of minimax_estimators is given for any     0 < c
&#x2264; 2 ( p &#x2212; 1 )   {\displaystyle 0<c\leq 2(p-1)}  [0<c\leq 2(p-1)]
and     b &#x2265; ( p &#x2212; 2 +  p  &#x2212; 1   )   {\displaystyle b\geq
(p-2+p^{-1})}  [b\geq (p-2+p^{-1})] as[47]
             &#x03BB; &#x005E;     i   =  (  1 &#x2212;   c  b +  &#x2211;  i =
      1   p    X  i       )   X  i   ,  i = 1 , &#x2026; , p .   {\displaystyle
      {\hat {\lambda }}_{i}=\left(1-{\frac {c}{b+\sum _{i=1}^{p}X_
      {i}}}\right)X_{i},\qquad i=1,\dots ,p.}  [{\hat {\lambda }}_{i}=\left(1-
      {\frac {c}{b+\sum _{i=1}^{p}X_{i}}}\right)X_{i},\qquad i=1,\dots ,p.]
***** Bivariate Poisson distribution[edit] *****
This distribution has been extended to the bivariate case.[48] The generating
function for this distribution is
         g ( u , v ) = exp &#x2061; [ (  &#x03B8;  1   &#x2212;  &#x03B8;  12
      ) ( u &#x2212; 1 ) + (  &#x03B8;  2   &#x2212;  &#x03B8;  12   ) ( v
      &#x2212; 1 ) +  &#x03B8;  12   ( u v &#x2212; 1 ) ]   {\displaystyle g
      (u,v)=\exp[(\theta _{1}-\theta _{12})(u-1)+(\theta _{2}-\theta _{12})(v-
      1)+\theta _{12}(uv-1)]}  [g(u,v)=\exp[(\theta _{1}-\theta _{12})(u-1)+
      (\theta _{2}-\theta _{12})(v-1)+\theta _{12}(uv-1)]]
with
          &#x03B8;  1   ,  &#x03B8;  2   >  &#x03B8;  12   > 0
      {\displaystyle \theta _{1},\theta _{2}>\theta _{12}>0\,}  [\theta _
      {1},\theta _{2}>\theta _{12}>0\,]
The marginal distributions are Poisson(Î¸1) and Poisson(Î¸2) and the
correlation coefficient is limited to the range
         0 &#x2264; &#x03C1; &#x2264; min  {     &#x03B8;  1    &#x03B8;  2
      ,    &#x03B8;  2    &#x03B8;  1      }    {\displaystyle 0\leq \rho \leq
      \min \left\{{\frac {\theta _{1}}{\theta _{2}}},{\frac {\theta _{2}}
      {\theta _{1}}}\right\}}  [0\leq \rho \leq \min \left\{{\frac {\theta _
      {1}}{\theta _{2}}},{\frac {\theta _{2}}{\theta _{1}}}\right\}]
A simple way to generate a bivariate Poisson distribution      X  1   ,  X  2
{\displaystyle X_{1},X_{2}}  [X_{1},X_{2}] is to take three independent Poisson
distributions      Y  1   ,  Y  2   ,  Y  3     {\displaystyle Y_{1},Y_{2},Y_
{3}}  [Y_{1},Y_{2},Y_{3}] with means      &#x03BB;  1   ,  &#x03BB;  2   ,
&#x03BB;  3     {\displaystyle \lambda _{1},\lambda _{2},\lambda _{3}}
[\lambda _{1},\lambda _{2},\lambda _{3}] and then set      X  1   =  Y  1   +
Y  3   ,  X  2   =  Y  2   +  Y  3     {\displaystyle X_{1}=Y_{1}+Y_{3},X_
{2}=Y_{2}+Y_{3}}  [X_{1}=Y_{1}+Y_{3},X_{2}=Y_{2}+Y_{3}]. The probability
function of the bivariate Poisson distribution is
               Pr (  X  1   =  k  1   ,  X  2   =  k  2   )     =     exp
      &#x2061;  (  &#x2212;  &#x03BB;  1   &#x2212;  &#x03BB;  2   &#x2212;
      &#x03BB;  3    )     &#x03BB;  1    k  1       k  1   !       &#x03BB;  2
      k  2       k  2   !     &#x2211;  k = 0   min (  k  1   ,  k  2   )
      (    k  1   k   )       (    k  2   k   )    k !   (    &#x03BB;  3
      &#x03BB;  1    &#x03BB;  2      )   k         {\displaystyle {\begin
      {aligned}&\Pr(X_{1}=k_{1},X_{2}=k_{2})\\={}&\exp \left(-\lambda _{1}-
      \lambda _{2}-\lambda _{3}\right){\frac {\lambda _{1}^{k_{1}}}{k_{1}!}}
      {\frac {\lambda _{2}^{k_{2}}}{k_{2}!}}\sum _{k=0}^{\min(k_{1},k_{2})}
      {\binom {k_{1}}{k}}{\binom {k_{2}}{k}}k!\left({\frac {\lambda _{3}}
      {\lambda _{1}\lambda _{2}}}\right)^{k}\end{aligned}}}  [{\begin
      {aligned}&\Pr(X_{1}=k_{1},X_{2}=k_{2})\\={}&\exp \left(-\lambda _{1}-
      \lambda _{2}-\lambda _{3}\right){\frac {\lambda _{1}^{k_{1}}}{k_{1}!}}
      {\frac {\lambda _{2}^{k_{2}}}{k_{2}!}}\sum _{k=0}^{\min(k_{1},k_{2})}
      {\binom {k_{1}}{k}}{\binom {k_{2}}{k}}k!\left({\frac {\lambda _{3}}
      {\lambda _{1}\lambda _{2}}}\right)^{k}\end{aligned}}]
***** Computer software for the Poisson distribution[edit] *****
The Poisson distribution poses two different tasks for dedicated software
libraries: Evaluating the distribution     P ( k ; &#x03BB; )   {\displaystyle
P(k;\lambda )}  [{\displaystyle P(k;\lambda )}], and drawing random numbers
according to that distribution.
**** Evaluating the Poisson distribution[edit] ****
Computing     P ( k ; &#x03BB; )   {\displaystyle P(k;\lambda )}  [
{\displaystyle P(k;\lambda )}] for given     k   {\displaystyle k}  [k] and
&#x03BB;   {\displaystyle \lambda }  [\lambda ] is a trivial task that can be
accomplished by using the standard definition of     P ( k ; &#x03BB; )
{\displaystyle P(k;\lambda )}  [{\displaystyle P(k;\lambda )}] in terms of
exponential, power, and factorial functions — expect for large values of     k
{\displaystyle k}  [k] that entail risk of cancellation. To avoid cancellation,
it is advisable to use the math.h standard library function lgamma.
Some computing languages provide built-in Poisson distributions, namely
    * R: function dpois(x, lambda);
    * Excel: function POISSON( x, mean, cumulative), with a flag to specify the
      cumulative distribution;
    * Mathematica: univariate Poisson distribution as PoissonDistribution
      [    &#x03BB;   {\displaystyle \lambda }  [\lambda ]],[49] bivariate
      Poisson distribution as MultivariatePoissonDistribution[     &#x03B8;  12
      {\displaystyle \theta _{12}}  [{\displaystyle \theta _{12}}],
      {      &#x03B8;  1   &#x2212;  &#x03B8;  12     {\displaystyle \theta _
      {1}-\theta _{12}}  [{\displaystyle \theta _{1}-\theta _{12}}],
      &#x03B8;  2   &#x2212;  &#x03B8;  12     {\displaystyle \theta _{2}-
      \theta _{12}}  [{\displaystyle \theta _{2}-\theta _{12}}]}],.[50]
**** Random drawing from the Poisson distribution[edit] ****
The less trivial task is to draw random integers from the Poisson distribution
with given     &#x03BB;   {\displaystyle \lambda }  [\lambda ].
Solutions are provided by:
    * GNU_Scientific_Library (GSL): function gsl_ran_poisson
    * R: function rpois(n, lambda);
***** See also[edit] *****
    * Compound_Poisson_distribution
    * ConwayâMaxwellâPoisson_distribution
    * Erlang_distribution
    * Hermite_distribution
    * Index_of_dispersion
    * Negative_binomial_distribution
    * Poisson_clumping
    * Poisson_point_process
    * Poisson_regression
    * Poisson_sampling
    * Poisson_wavelet
    * Queueing_theory
    * Renewal_theory
    * Robbins_lemma
    * Skellam_distribution
    * Tweedie_distribution
    * Zero-inflated_model
    * Zero-truncated_Poisson_distribution
***** References[edit] *****
**** Citations[edit] ****
   1. ^Frank A. Haight (1967). Handbook of the Poisson Distribution. New York:
      John Wiley & Sons.
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
   3. ^"Statistics_|_The_Poisson_Distribution". Umass.edu. 2007-08-24.
      Retrieved 2014-04-18.
   4. ^Ugarte, MD; Militino, AF; Arnholt, AT (2016), Probability and Statistics
      with R (Second ed.), CRC Press, ISBN 978-1-4665-0439-4
   5. ^ S.D. Poisson, ProbabilitÃ© des jugements en matiÃ¨re criminelle et en
      matiÃ¨re civile, prÃ©cÃ©dÃ©es des rÃ¨gles gÃ©nÃ©rales du calcul des
      probabilitiÃ©s (Paris, France: Bachelier, 1837), page_206.
   6. ^ a b c d e f g h i Johnson, N. L.; Kotz, S.; Kemp, A. W. (1993).
      Univariate Discrete distributions (2nd ed.). Wiley. ISBN 0-471-54897-9.
   7. ^Stigler, Stephen M. (1982). "Poisson on the poisson distribution".
      Statistics & Probability Letters. 1: 33â35. doi:10.1016/0167-7152
      (82)90010-4.
   8. ^Hald, A.; de Moivre, Abraham; McClintock, Bruce (1984). "A. de Moivre:
      'De Mensura Sortis' or 'On the Measurement of Chance'". International
      Statistical Review / Revue Internationale de Statistique. 52 (3):
      229â262. doi:10.2307/1403045. JSTOR 1403045.
   9. ^ Ladislaus von Bortkiewicz, Das Gesetz der kleinen Zahlen [The law of
      small numbers] (Leipzig, Germany: B.G. Teubner, 1898). On page_1,
      Bortkiewicz presents the Poisson distribution. On pages_23â25,
      Bortkiewicz presents his analysis of "4. Beispiel: Die durch Schlag eines
      Pferdes im preussischen Heere GetÃ¶teten." (4. Example: Those killed in
      the Prussian army by a horse's kick.).
  10. ^ Probability and Stochastic Processes: A Friendly Introduction for
      Electrical and Computer Engineers, Roy D. Yates, David Goodman, page 60.
  11. ^ For the proof, see : Proof_wiki:_expectation and Proof_wiki:_variance
  12. ^Some_Poisson_models, Vose Software, retrieved 2016-01-18
  13. ^Helske, Jouni (2015-06-25), KFAS:_Exponential_family_state_space_models
      in_R (PDF), Comprehensive_R_Archive_Network, arXiv:1612.01907, Bibcode:
      2016arXiv161201907H, retrieved 2016-01-18
  14. ^ Choi KP (1994) On the medians of Gamma distributions and an equation of
      Ramanujan. Proc Amer Math Soc 121 (1) 245â251
  15. ^Riordan, John (1937). "Moment recurrence relations for binomial, Poisson
      and hypergeometric frequency distributions". Annals of Mathematical
      Statistics. 8 (2): 103â111. doi:10.1214/aoms/1177732430.
  16.  Also see Haight (1967), p. 6.
  17. ^ Jagadeesan, Meena. "Simple analysis of sparse, sign-consistent JL."
      arXiv preprint arXiv:1708.02966 (2017).
  18. ^E. L. Lehmann (1986). Testing Statistical Hypotheses (second ed.). New
      York: Springer Verlag. ISBN 978-0-387-94919-2.
  19.  page 65.
  20. ^ Raikov, D. (1937). On the decomposition of Poisson laws. Comptes Rendus
      de l'AcadÃ©mie des Sciences de l'URSS, 14, 9â11. (The proof is also
      given invon Mises, Richard (1964). Mathematical Theory of Probability and
      Statistics. New York: Academic Press.
  21. )
  22. ^Laha, R. G. & Rohatgi, V. K. (1979-05-01). Probability Theory. New York:
      John Wiley & Sons. p. 233. ISBN 978-0-471-03262-5.
  23. ^Michael Mitzenmacher & Eli Upfal (2005-01-31). Probability and
      Computing: Randomized Algorithms and Probabilistic Analysis. Cambridge
      University Press. p. 97. ISBN 978-0521835404.
  24. ^ http://downloads.hindawi.com/archive/2013/412958.pdf
  25. ^ "Optimal_Haplotype_Assembly_from_High-Throughput_Mate-Pair_Reads,
      published_in_ISIT_2015"
  26. ^ https://newonlinecourses.science.psu.edu/stat504/node/48/
  27. ^ Mitzenmacher, Michael, and Eli Upfal. Probability and computing:
      randomization and probabilistic techniques in algorithms and data
      analysis. Cambridge university press, 2017.
  28. ^ NIST/SEMATECH, '6.3.3.1._Counts_Control_Charts', e-Handbook of
      Statistical Methods, accessed 25 October 2006
  29. ^Huiming, Zhang; Yunxiao Liu; Bo Li (2014). "Notes on discrete compound
      Poisson model with applications to risk theory". Insurance: Mathematics
      and Economics. 59: 325â336. doi:10.1016/j.insmatheco.2014.09.012.
  30. ^Huiming, Zhang; Bo Li (2016). "Characterizations of discrete compound
      Poisson distributions". Communications in Statistics - Theory and
      Methods. 45 (22): 6789â6802. doi:10.1080/03610926.2014.901375.
  31. ^McCullagh,_Peter; Nelder,_John (1989). Generalized Linear Models.
      London: Chapman and Hall. ISBN 978-0-412-31760-6.
  32.  page 196 gives the approximation and higher order terms.
  33. ^S. M. Ross (2007). Introduction to Probability Models (ninth ed.).
      Boston: Academic Press. ISBN 978-0-12-598062-3.
  34.  pp. 307â308.
  35. ^ "The_Poisson_Process_as_a_Model_for_a_Diversity_of_Behavioural
      Phenomena"
  36. ^Paul J. Flory (1940). "Molecular Size Distribution in Ethylene Oxide
      Polymers". Journal of the American Chemical Society. 62 (6): 1561â1565.
      doi:10.1021/ja01863a066.
  37. ^Lomnitz, Cinna (1994). Fundamentals of earthquake prediction. New York:
      John Wiley & Sons. ISBN 0-471-57419-8. OCLC 647404423.
  38. ^Philip J. Boland (1984). "A Biographical Glimpse of William Sealy
      Gosset". The American Statistician. 38 (3): 179â183. doi:10.1080/
      00031305.1984.10483195.
  39. ^ Dave Hornby. "Football_Prediction_Model:_Poisson_Distribution".
      calculate the probability of outcomes for a football match, which in turn
      can be turned into odds that we can use to identify value in the market.
  40. ^Koyama, Kento; Hokunan, Hidekazu; Hasegawa, Mayumi; Kawamura, Shuso;
      Koseki, Shigenobu (2016-12-01). "Do bacterial cell numbers follow a
      theoretical Poisson distribution? Comparison of experimentally obtained
      numbers of single cells with random number generation via computer
      simulation". Food Microbiology. 60: 49â53. doi:10.1016/
      j.fm.2016.05.019. ISSN 0740-0020.
  41. ^Clarke, R. D. (1946). "An application of the Poisson distribution".
      Journal of the Institute of Actuaries. 72 (3): 481. doi:10.1017/
      S0020268100035435.
  42. ^ Aatish Bhatia (2012-12-21). "What_does_randomness_look_like?". Wired.
      Within a large area of London, the bombs werenât being targeted. They
      rained down at random in a devastating, city-wide game of Russian
      roulette.
  43. ^Gallagher,_P._X. (1976). "On the distribution of primes in short
      intervals". Mathematika. 23: 4â9. doi:10.1112/s0025579300016442.
  44. ^A. Colin Cameron; Pravin K. Trivedi (1998). Regression_Analysis_of_Count
      Data. ISBN 9780521635677. Retrieved 2013-01-30. (p.5) The law of rare
      events states that the total number of events will follow, approximately,
      the Poisson distribution if an event may occur in any of a large number
      of trials but the probability of occurrence in any given trial is small.
  45. ^Edgeworth,_F._Y. (1913). "On the use of the theory of probabilities in
      statistics relating to society". Journal_of_the_Royal_Statistical
      Society. 76 (2): 165â193. doi:10.2307/2340091. JSTOR 2340091.
  46. ^Devroye,_Luc (1986). "Discrete_Univariate_Distributions" (PDF). Non-
      Uniform_Random_Variate_Generation. New York: Springer-Verlag. p. 505.
  47. ^Paszek, Ewa. "Maximum_Likelihood_Estimation_â_Examples".
  48. ^ Garwood, F. (1936). "Fiducial Limits for the Poisson Distribution".
      Biometrika. 28 (3/4): 437â442. doi:10.1093/biomet/28.3-4.437.
  49. ^Breslow,_NE; Day,_NE (1987). Statistical_Methods_in_Cancer_Research:
      Volume_2âThe_Design_and_Analysis_of_Cohort_Studies. Paris:
      International_Agency_for_Research_on_Cancer. ISBN 978-92-832-0182-3.
  50. ^Fink, Daniel (1997). A Compendium of Conjugate Priors.
  51. ^Gelman; et al. (2005). Bayesian Data Analysis (2nd ed.). p. 60.
  52. ^Clevenson, M. L.; Zidek, J. V. (1975). "Simultaneous Estimation of the
      Means of Independent Poisson Laws". Journal of the American Statistical
      Association. 70 (351a): 698â705. doi:10.1080/01621459.1975.10482497.
  53. ^Berger, J. O. (1985). Statistical Decision Theory and Bayesian Analysis
      (2nd ed.). Springer. Bibcode:1985sdtb.book.....B.
  54. ^Loukas, S.; Kemp, C. D. (1986). "The Index of Dispersion Test for the
      Bivariate Poisson Distribution". Biometrics. 42 (4): 941â948. doi:
      10.2307/2530708. JSTOR 2530708.
  55. ^"Wolfram_Language:_PoissonDistribution_reference_page". wolfram.com.
      Retrieved 2016-04-08.
  56. ^"Wolfram_Language:_MultivariatePoissonDistribution_reference_page".
      wolfram.com. Retrieved 2016-04-08.
**** Sources[edit] ****
    * Ahrens, Joachim H.; Dieter, Ulrich (1974). "Computer Methods for Sampling
      from Gamma, Beta, Poisson and Binomial Distributions". Computing. 12 (3):
      223â246. doi:10.1007/BF02293108.
Ahrens, Joachim H.; Dieter, Ulrich (1982). "Computer Generation of Poisson
Deviates". ACM Transactions on Mathematical Software. 8 (2): 163â179. doi:
10.1145/355993.355997.
Evans, Ronald J.; Boersma, J.; Blachman, N. M.; Jagers, A. A. (1988). "The
Entropy of a Poisson Distribution: Problem 87-6". SIAM Review. 30 (2):
314â317. doi:10.1137/1030059.
Knuth, Donald E. (1969). Seminumerical Algorithms. The_Art_of_Computer
Programming. 2. Addison_Wesley.
***** Further reading[edit] *****
    * Shanmugam, Ramalingam (2013). "Informatics about fear to report rapes
      using bumped-up Poisson model". American Journal of Biostatistics. 3 (1):
      17â29. doi:10.3844/amjbsp.2013.17.29.
Clarke, R. D., F.I.A. "An_Application_of_the_Poisson_Distribution" (PDF).
Institute_and_Faculty_of_Actuaries. Retrieved 7 July 2019.
    * v
    * t
    * e
Probability_distributions
List
                                          * Benford
                                          * Bernoulli
                                          * beta-binomial
                                          * binomial
                                          * categorical
Discrete univariate                       * hypergeometric
with finite support                       * Poisson_binomial
                                          * Rademacher
                                          * soliton
                                          * discrete_uniform
                                          * Zipf
                                          * ZipfâMandelbrot
                                          * beta_negative_binomial
                                          * Borel
                                          * ConwayâMaxwellâPoisson
                                          * discrete_phase-type
                                          * Delaporte
                                          * extended_negative_binomial
Discrete univariate                       * GaussâKuzmin
with infinite support                     * geometric
                                          * logarithmic
                                          * negative_binomial
                                          * parabolic_fractal
                                          * Poisson
                                          * Skellam
                                          * YuleâSimon
                                          * zeta
                                          * arcsine
                                          * ARGUS
                                          * BaldingâNichols
                                          * Bates
                                          * beta
                                          * beta_rectangular
                                          * IrwinâHall
Continuous univariate                     * Kumaraswamy
supported on a bounded interval           * logit-normal
                                          * noncentral_beta
                                          * raised_cosine
                                          * reciprocal
                                          * triangular
                                          * U-quadratic
                                          * uniform
                                          * Wigner_semicircle
                                          * Benini
                                          * Benktander_1st_kind
                                          * Benktander_2nd_kind
                                          * beta_prime
                                          * Burr
                                          * chi-squared
                                          * chi
                                          * Dagum
                                          * Davis
                                          * exponential-logarithmic
                                          * Erlang
                                          * exponential
                                          * F
                                          * folded_normal
                                          * FloryâSchulz
                                          * FrÃ©chet
                                          * gamma
                                          * gamma/Gompertz
                                          * generalized_inverse_Gaussian
                                          * Gompertz
                                          * half-logistic
                                          * half-normal
                                          * Hotelling's_T-squared
                                          * hyper-Erlang
                                          * hyperexponential
                                          * hypoexponential
Continuous univariate                     * inverse_chi-squared
supported on a semi-infinite interval           o scaled_inverse_chi-squared
                                          * inverse_Gaussian
                                          * inverse_gamma
                                          * Kolmogorov
                                          * LÃ©vy
                                          * log-Cauchy
                                          * log-Laplace
                                          * log-logistic
                                          * log-normal
                                          * Lomax
                                          * matrix-exponential
                                          * MaxwellâBoltzmann
                                          * MaxwellâJÃ¼ttner
                                          * Mittag-Leffler
                                          * Nakagami
                                          * noncentral_chi-squared
                                          * Pareto
                                          * phase-type
                                          * poly-Weibull
                                          * Rayleigh
                                          * relativistic_BreitâWigner
                                          * Rice
                                          * shifted_Gompertz
                                          * truncated_normal
                                          * type-2_Gumbel
                                          * Weibull
                                                o Discrete_Weibull
                                          * Wilks's_lambda
                                          * Cauchy
                                          * exponential_power
                                          * Fisher's_z
                                          * Gaussian_q
                                          * generalized_normal
                                          * generalized_hyperbolic
                                          * geometric_stable
                                          * Gumbel
                                          * Holtsmark
                                          * hyperbolic_secant
                                          * Johnson's_SU
                                          * Landau
Continuous univariate                     * Laplace
supported on the whole real line          * asymmetric_Laplace
                                          * logistic
                                          * noncentral_t
                                          * normal_(Gaussian)
                                          * normal-inverse_Gaussian
                                          * skew_normal
                                          * slash
                                          * stable
                                          * Student's_t
                                          * type-1_Gumbel
                                          * TracyâWidom
                                          * variance-gamma
                                          * Voigt
                                          * generalized_extreme_value
                                          * generalized_Pareto
                                          * MarchenkoâPastur
Continuous univariate                     * q-exponential
with support whose type varies            * q-Gaussian
                                          * q-Weibull
                                          * shifted_log-logistic
                                          * Tukey_lambda
Mixed continuous-discrete univariate      * rectified_Gaussian
                                            inverse_matrix_gamma
                                            inverse-Wishart
                                            matrix_normal
Multivariate_(joint)                        matrix_t
                                            matrix_gamma
                                            normal-inverse-Wishart
                                            normal-Wishart
                                            Wishart
Directional                                 von_MisesâFisher
                                            Bingham
Degenerate and singular                     Cantor
                                          * Circular
                                          * compound_Poisson
                                          * elliptical
                                          * exponential
                                          * natural_exponential
Families                                  * locationâscale
                                          * maximum_entropy
                                          * mixture
                                          * Pearson
                                          * Tweedie
                                          * wrapped
                                              * GND: 4253010-6
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85103956
                                              * NDL: 00569122

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Poisson_distribution&oldid=909659012"
Categories:
    * Conjugate_prior_distributions
    * Factorial_and_binomial_topics
    * Poisson_distribution
    * Infinitely_divisible_probability_distributions
Hidden categories:
    * Pages_using_deprecated_image_syntax
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2012
    * Articles_with_unsourced_statements_from_April_2012
    * Articles_with_unsourced_statements_from_March_2019
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
    * Articles_with_example_pseudocode
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
    * Asturianu
    * ØªÛØ±Ú©Ø¬Ù
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Basa_Sunda
    * Suomi
    * Svenska
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 6 August 2019, at 19:54 (UTC).
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
