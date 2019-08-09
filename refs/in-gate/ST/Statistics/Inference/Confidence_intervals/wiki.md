The following text has been accessed from https://en.wikipedia.org/wiki/Confidence_interval at Fri Aug 9 02:53:59 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Confidence interval ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article needs attention from an expert in Statistics. The specific
 problem is: Many reverts and fixes indicate the language of the article needs
 to be checked carefully. WikiProject_Statistics may be able to help recruit an
 expert. (November 2018)
In statistics, a confidence interval (CI) is a type of interval_estimate,
computed from the statistics of the observed data, that might contain the true
value of an unknown population_parameter. The interval has an associated
confidence level, or coverage that, loosely speaking, quantifies the level of
confidence that the deterministic parameter is captured by the interval. More
strictly speaking, the confidence level represents the frequency (i.e. the
proportion) of possible confidence intervals that contain the true value of the
unknown population parameter. In other words, if confidence intervals are
constructed using a given confidence level from an infinite number of
independent sample statistics, the proportion of those intervals that contain
the true value of the parameter will be equal to the confidence level.[1][2][3]
Confidence intervals consist of a range of potential values of the unknown
population_parameter. However, the interval computed from a particular sample
does not necessarily include the true value of the parameter. Based on the
(usually taken) assumption that observed data are random samples from a true
population, the confidence interval obtained from the data is also random.
The confidence level is designated prior to examining the data. Most commonly,
the 95% confidence level is used.[4] However, other confidence levels can be
used, for example, 90% and 99%.
Factors affecting the width of the confidence interval include the size of the
sample, the confidence level, and the variability in the sample. A larger
sample will tend to produce a better estimate of the population parameter, when
all other factors are equal. A higher confidence level will tend to produce a
broader confidence interval.
Confidence intervals were introduced to statistics by Jerzy_Neyman in a paper
published in 1937.[3]
⁰
***** Contents *****
    * 1_Conceptual_basis
          o 1.1_Introduction
          o 1.2_Meaning_and_interpretation
                # 1.2.1_Misunderstandings
          o 1.3_Philosophical_issues
          o 1.4_Relationship_with_other_statistical_topics
                # 1.4.1_Statistical_hypothesis_testing
                # 1.4.2_Confidence_region
                # 1.4.3_Confidence_band
    * 2_Basic_steps
    * 3_Statistical_theory
          o 3.1_Definition
                # 3.1.1_Approximate_confidence_intervals
          o 3.2_Desirable_properties
          o 3.3_Methods_of_derivation
    * 4_Examples
          o 4.1_Practical_example
                # 4.1.1_Interpretation
          o 4.2_Theoretical_example
    * 5_Alternatives_and_critiques
          o 5.1_Comparison_to_prediction_intervals
          o 5.2_Comparison_to_tolerance_intervals
          o 5.3_Comparison_to_Bayesian_interval_estimates
          o 5.4_Confidence_intervals_for_proportions_and_related_quantities
          o 5.5_Counter-examples
                # 5.5.1_Confidence_procedure_for_uniform_location
                # 5.5.2_Confidence_procedure_for_Ï2
    * 6_See_also
          o 6.1_Confidence_interval_for_specific_distributions
    * 7_References
    * 8_Bibliography
          o 8.1_External_links
          o 8.2_Online_calculators
***** Conceptual basis[edit] *****
In this bar_chart, the top ends of the brown bars indicate observed means and
the red line_segments ("error bars") represent the confidence intervals around
them. Although the error bars are shown as symmetric around the means, that is
not always the case. It is also important to note that in most graphs, the
error bars do not represent confidence intervals (e.g., they often represent
standard errors or standard_deviations)
**** Introduction[edit] ****
Interval_estimation can be contrasted with point_estimation. A point estimate
is a single value given as the estimate of a population parameter that is of
interest, for example, the mean of some quantity. An interval estimate
specifies instead a range within which the parameter is estimated to lie.
Confidence intervals are commonly reported in tables or graphs along with point
estimates of the same parameters, to show the reliability of the estimates.
For example, a confidence interval can be used to describe how reliable survey
results are. In a poll of electionâvoting intentions, the result might be
that 40% of respondents intend to vote for a certain party. A 99% confidence
interval for the proportion in the whole population having the same intention
on the survey might be 30% to 50%. From the same data one may calculate a 90%
confidence interval, which in this case might be 37% to 43%. A major factor
determining the length of a confidence interval is the size_of_the_sample used
in the estimation procedure, for example, the number of people taking part in a
survey.
**** Meaning and interpretation[edit] ****
See also: Â§ Practical_example_interpretation
Various interpretations of a confidence interval can be given (taking the 90%
confidence interval as an example in the following).
    * The confidence interval can be expressed in terms of samples (or repeated
      samples): "Were this procedure to be repeated on numerous samples, the
      fraction of calculated confidence intervals (which would differ for each
      sample) that encompass the true population parameter would tend toward
      90%."[1]
    * The confidence interval can be expressed in terms of a single sample:
      "There is a 90% probability that the calculated confidence interval from
      some future experiment encompasses the true value of the population
      parameter." Note this is a probability statement about the confidence
      interval, not the population parameter. This considers the probability
      associated with a confidence interval from a pre-experiment point of
      view, in the same context in which arguments for the random allocation of
      treatments to study items are made. Here the experimenter sets out the
      way in which they intend to calculate a confidence interval and to know,
      before they do the actual experiment, that the interval they will end up
      calculating has a particular chance of covering the true but unknown
      value.[3] This is very similar to the "repeated sample" interpretation
      above, except that it avoids relying on considering hypothetical repeats
      of a sampling procedure that may not be repeatable in any meaningful
      sense. See Neyman_construction.
    * The explanation of a confidence interval can amount to something like:
      "The confidence interval represents values for the population parameter
      for which the difference between the parameter and the observed estimate
      is not statistically_significant at the 10% level".[5] In fact, this
      relates to one particular way in which a confidence interval may be
      constructed.
In each of the above, the following applies: If the true value of the parameter
lies outside the 90% confidence interval, then a sampling event has occurred
(namely, obtaining a point estimate of the parameter at least this far from the
true parameter value) which had a probability of 10% (or less) of happening by
chance.
*** Misunderstandings[edit] ***
See also: Â§ Counter-examples, and Misunderstandings_of_p-values
Confidence intervals and levels are frequently misunderstood, and published
studies have shown that even professional scientists often misinterpret them.
[6][7][8][9]
    * A 95% confidence level does not mean that for a given realized interval
      there is a 95% probability that the population parameter lies within the
      interval (i.e., a 95% probability that the interval covers the population
      parameter).[10] According to the strict frequentist interpretation, once
      an interval is calculated, this interval either covers the parameter
      value or it does not; it is no longer a matter of probability. The 95%
      probability relates to the reliability of the estimation procedure, not
      to a specific calculated interval.[11] Neyman himself (the original
      proponent of confidence intervals) made this point in his original paper:
      [3]
           "It will be noticed that in the above description, the
           probability statements refer to the problems of estimation with
           which the statistician will be concerned in the future. In
           fact, I have repeatedly stated that the frequency of correct
           results will tend to Î±. Consider now the case when a sample is
           already drawn, and the calculations have given [particular
           limits]. Can we say that in this particular case the
           probability of the true value [falling between these limits] is
           equal to Î±? The answer is obviously in the negative. The
           parameter is an unknown constant, and no probability statement
           concerning its value may be made..."
      Deborah Mayo expands on this further as follows:[12]
           "It must be stressed, however, that having seen the value [of
           the data], Neyman-Pearson theory never permits one to conclude
           that the specific confidence interval formed covers the true
           value of 0 with either (1 â Î±)100% probability or (1 â
           Î±)100% degree of confidence. Seidenfeld's remark seems rooted
           in a (not uncommon) desire for Neyman-Pearson confidence
           intervals to provide something which they cannot legitimately
           provide; namely, a measure of the degree of probability,
           belief, or support that an unknown parameter value lies in a
           specific interval. Following Savage (1962), the probability
           that a parameter lies in a specific interval may be referred to
           as a measure of final precision. While a measure of final
           precision may seem desirable, and while confidence levels are
           often (wrongly) interpreted as providing such a measure, no
           such interpretation is warranted. Admittedly, such a
           misinterpretation is encouraged by the word 'confidence'."
    * A 95% confidence level does not mean that 95% of the sample data lie
      within the confidence interval.
    * A confidence interval is not a definitive range of plausible values for
      the sample parameter, though it may be understood as an estimate of
      plausible values for the population parameter.
    * A particular confidence level of 95% calculated from an experiment does
      not mean that there is a 95% probability of a sample parameter from a
      repeat of the experiment falling within this interval.
**** Philosophical issues[edit] ****
The principle behind confidence intervals was formulated to provide an answer
to the question raised in statistical_inference of how to deal with the
uncertainty inherent in results derived from data that are themselves only a
randomly selected subset of a population. There are other answers, notably that
provided by Bayesian_inference in the form of credible_intervals. Confidence
intervals correspond to a chosen rule for determining the confidence bounds,
where this rule is essentially determined before any data are obtained, or
before an experiment is done. The rule is defined such that over all possible
datasets that might be obtained, there is a high probability ("high" is
specifically quantified) that the interval determined by the rule will include
the true value of the quantity under consideration. The Bayesian approach
appears to offer intervals that can, subject to acceptance of an interpretation
of "probability" as Bayesian_probability, be interpreted as meaning that the
specific interval calculated from a given dataset has a particular probability
of including the true value, conditional on the data and other information
available. The confidence interval approach does not allow this since in this
formulation and at this same stage, both the bounds of the interval and the
true values are fixed values, and there is no randomness involved. On the other
hand, the Bayesian approach is only as valid as the prior probability used in
the computation, whereas the confidence interval does not depend on assumptions
about the prior probability.
The questions concerning how an interval expressing uncertainty in an estimate
might be formulated, and of how such intervals might be interpreted, are not
strictly mathematical problems and are philosophically problematic.[13]
Mathematics can take over once the basic principles of an approach to
'inference' have been established, but it has only a limited role in saying why
one approach should be preferred to another: For example, a confidence level of
95% is often used in the biological_sciences, but this is a matter of
convention or arbitration. In the physical_sciences, a much higher level may be
used.[14]
**** Relationship with other statistical topics[edit] ****
*** Statistical hypothesis testing[edit] ***
See also: Statistical_hypothesis_testing_Â§ Alternatives, and Estimation
statistics
Confidence intervals are closely related to statistical significance_testing.
For example, if for some estimated parameter Î¸ one wants to test the null
hypothesis that Î¸ = 0 against the alternative that Î¸ â  0, then this test
can be performed by determining whether the confidence interval for Î¸ contains
0.
More generally, given the availability of a hypothesis testing procedure that
can test the null hypothesis Î¸ = Î¸0 against the alternative that Î¸ â  Î¸0
for any value of Î¸0, then a confidence interval with confidence
level Î³ = 1 â Î± can be defined as containing any number Î¸0 for which the
corresponding null hypothesis is not rejected at significance level Î±.[15]
If the estimates of two parameters (for example, the mean values of a variable
in two independent groups) have confidence intervals that do not overlap, then
the difference between the two values is more significant than that indicated
by the individual values of Î±.[16] So, this "test" is too conservative and can
lead to a result that is more significant than the individual values of Î±
would indicate. If two confidence intervals overlap, the two means still may be
significantly different.[17][18][19] Accordingly, and consistent with the
Mantel-Haenszel Chi-squared_test, is a proposed fix whereby one reduces the
error bounds for the two means by multiplying them by the square root of Â½
(0.707107) before making the comparison.[20]
While the formulations of the notions of confidence intervals and of
statistical_hypothesis_testing are distinct, they are in some senses related
and to some extent complementary. While not all confidence intervals are
constructed in this way, one general purpose approach to constructing
confidence intervals is to define a 100(1 â Î±)% confidence interval to
consist of all those values Î¸0 for which a test of the hypothesis Î¸ = Î¸0 is
not rejected at a significance level of 100Î±%. Such an approach may not always
be available since it presupposes the practical availability of an appropriate
significance test. Naturally, any assumptions required for the significance
test would carry over to the confidence intervals.
It may be convenient to make the general correspondence that parameter values
within a confidence interval are equivalent to those values that would not be
rejected by a hypothesis test, but this would be dangerous. In many instances
the confidence intervals that are quoted are only approximately valid, perhaps
derived from "plus or minus twice the standard error," and the implications of
this for the supposedly corresponding hypothesis tests are usually unknown.
It is worth noting that the confidence interval for a parameter is not the same
as the acceptance region of a test for this parameter, as is sometimes thought.
The confidence interval is part of the parameter space, whereas the acceptance
region is part of the sample space. For the same reason, the confidence level
is not the same as the complementary probability of the level of significance.
[further_explanation_needed]
*** Confidence region[edit] ***
Main article: Confidence_region
Confidence_regions generalize the confidence interval concept to deal with
multiple quantities. Such regions can indicate not only the extent of likely
sampling_errors but can also reveal whether (for example) it is the case that
if the estimate for one quantity is unreliable, then the other is also likely
to be unreliable.
*** Confidence band[edit] ***
Main article: Confidence_band
A confidence_band is used in statistical_analysis to represent the uncertainty
in an estimate of a curve or function based on limited or noisy data.
Similarly, a prediction band is used to represent the uncertainty about the
value of a new data point on the curve, but subject to noise. Confidence and
prediction bands are often used as part of the graphical presentation of
results of a regression_analysis.
Confidence bands are closely related to confidence intervals, which represent
the uncertainty in an estimate of a single numerical value. "As confidence
intervals, by construction, only refer to a single point, they are narrower (at
this point) than a confidence band which is supposed to hold simultaneously at
many points."[21]
***** Basic steps[edit] *****
This example assumes that the samples are drawn from a Gaussian distribution.
The basic breakdown of how to calculate a confidence interval for a population
mean is as follows:
      1. Identify the sample mean,        x &#x00AF;      {\displaystyle {\bar
      {x}}}  [{\bar {x}}] .
      2. Identify whether the standard deviation is known,     &#x03C3;
      {\displaystyle \sigma }  [\sigma ], or unknown, s.
                * If standard deviation is known then      z  &#x2217;   =
                  &#x03A6;  &#x2212; 1    (  1 &#x2212;   &#x03B1; 2    )  =
                  &#x2212;  &#x03A6;  &#x2212; 1    (   &#x03B1; 2   )
                  {\displaystyle z^{*}=\Phi ^{-1}\left(1-{\frac {\alpha }
                  {2}}\right)=-\Phi ^{-1}\left({\frac {\alpha }{2}}\right)}  [
                  {\displaystyle z^{*}=\Phi ^{-1}\left(1-{\frac {\alpha }
                  {2}}\right)=-\Phi ^{-1}\left({\frac {\alpha }{2}}\right)}],
                  where     C = 100 ( 1 &#x2212; &#x03B1; ) &#x0025;
                  {\displaystyle C=100(1-\alpha )\%}  [{\displaystyle C=100(1-
                  \alpha )\%}] is the confidence level and     &#x03A6;
                  {\displaystyle \Phi }  [\Phi ] is the CDF of the standard
                  normal_distribution, used as the critical value. This value
                  is only dependent on the confidence level for the test.
                  Typical two sided confidence levels are:[22]
                  C   z*
                  99% 2.576
                  98% 2.326
                  95% 1.96
                  90% 1.645
                * If the standard deviation is unknown then Student's_t
                  distribution is used as the critical value. This value is
                  dependent on the confidence level (C) for the test and
                  degrees of freedom. The degrees of freedom are found by
                  subtracting one from the number of observations, n â 1. The
                  critical value is found from the t-distribution table. In
                  this table the critical value is written as tÎ±(r), where r
                  is the degrees of freedom and     &#x03B1; =    1 &#x2212; C
                  2     {\displaystyle \alpha ={1-C \over 2}}  [{\displaystyle
                  \alpha ={1-C \over 2}}].
      3. Plug the found values into the appropriate equations:
                * For a known standard deviation:      (     x &#x00AF;
                  &#x2212;  z  &#x2217;     &#x03C3;   n     ,    x &#x00AF;
                  +  z  &#x2217;     &#x03C3;   n      )    {\displaystyle
                  \left({\bar {x}}-z^{*}{\sigma \over {\sqrt {n}}},{\bar
                  {x}}+z^{*}{\sigma \over {\sqrt {n}}}\right)}  [{\displaystyle
                  \left({\bar {x}}-z^{*}{\sigma  \over {\sqrt {n}}},{\bar
                  {x}}+z^{*}{\sigma  \over {\sqrt {n}}}\right)}]
                * For an unknown standard deviation:      (     x &#x00AF;
                  &#x2212;  t  &#x2217;     s   n     ,    x &#x00AF;    +  t
                  &#x2217;     s   n      )    {\displaystyle \left({\bar {x}}-
                  t^{*}{s \over {\sqrt {n}}},{\bar {x}}+t^{*}{s \over {\sqrt
                  {n}}}\right)}  [{\displaystyle \left({\bar {x}}-t^{*}{s \over
                  {\sqrt {n}}},{\bar {x}}+t^{*}{s \over {\sqrt {n}}}\right)}]
                  [23]
***** Statistical theory[edit] *****
**** Definition[edit] ****
Let X be a random_sample from a probability_distribution with statistical
parameters Î¸, which is a quantity to be estimated, and Ï, representing
quantities that are not of immediate interest. A confidence interval for the
parameter Î¸, with confidence level or confidence coefficient Î³, is an
interval with random endpoints (u(X), v(X)), determined by the pair of random
variables u(X) and v(X), with the property:
           Pr   &#x03B8; , &#x03C6;   ( u ( X ) < &#x03B8; < v ( X ) ) =
      &#x03B3;  &#xA0;for all&#xA0;  ( &#x03B8; , &#x03C6; ) .   {\displaystyle
      {\Pr }_{\theta ,\varphi }(u(X)<\theta <v(X))=\gamma {\text{ for all }}
      (\theta ,\varphi ).}  [{\displaystyle {\Pr }_{\theta ,\varphi }(u
      (X)<\theta <v(X))=\gamma {\text{ for all }}(\theta ,\varphi ).}]
The quantities Ï in which there is no immediate interest are called nuisance
parameters, as statistical theory still needs to find some way to deal with
them. The number Î³, with typical values close to but not greater than 1, is
sometimes given in the form 1 â Î± (or as a percentage 100%Â·(1 â Î±)),
where Î± is a small non-negative number, close to 0.
Here PrÎ¸,Ï indicates the probability_distribution of X characterised by 
(Î¸, Ï). An important part of this specification is that the random interval
(u(X), v(X)) covers the unknown value Î¸ with a high probability no matter what
the true value of Î¸ actually is.
Note that here PrÎ¸,Ï need not refer to an explicitly given parameterized
family of distributions, although it often does. Just as the random variable X
notionally corresponds to other possible realizations of x from the same
population or from the same version of reality, the parameters (Î¸, Ï)
indicate that we need to consider other versions of reality in which the
distribution of X might have different characteristics.
In a specific situation, when x is the outcome of the sample X, the interval (u
(x), v(x)) is also referred to as a confidence interval for Î¸. Note that it is
no longer possible to say that the (observed) interval (u(x), v(x)) has
probability Î³ to contain the parameter Î¸. This observed interval is just one
realization of all possible intervals for which the probability statement
holds.
*** Approximate confidence intervals[edit] ***
In many applications, confidence intervals that have exactly the required
confidence level are hard to construct. But practically useful intervals can
still be found: the rule for constructing the interval may be accepted as
providing a confidence interval at level Î³ if
           Pr   &#x03B8; , &#x03C6;   ( u ( X ) < &#x03B8; < v ( X ) ) &#x2248;
      &#x03B3;  &#xA0;for all&#xA0;  ( &#x03B8; , &#x03C6; )    {\displaystyle
      {\Pr }_{\theta ,\varphi }(u(X)<\theta <v(X))\approx \gamma {\text{ for
      all }}(\theta ,\varphi )\,}  [{\displaystyle {\Pr }_{\theta ,\varphi }(u
      (X)<\theta <v(X))\approx \gamma {\text{ for all }}(\theta ,\varphi )\,}]
to an acceptable level of approximation. Alternatively, some authors[24] simply
require that
           Pr   &#x03B8; , &#x03C6;   ( u ( X ) < &#x03B8; < v ( X ) ) &#x2265;
      &#x03B3;  &#xA0;for all&#xA0;  ( &#x03B8; , &#x03C6; )    {\displaystyle
      {\Pr }_{\theta ,\varphi }(u(X)<\theta <v(X))\geq \gamma {\text{ for all
      }}(\theta ,\varphi )\,}  [{\displaystyle {\Pr }_{\theta ,\varphi }(u
      (X)<\theta <v(X))\geq \gamma {\text{ for all }}(\theta ,\varphi )\,}]
which is useful if the probabilities are only partially identified, or
imprecise.
**** Desirable properties[edit] ****
When applying standard statistical procedures, there will often be standard
ways of constructing confidence intervals. These will have been devised so as
to meet certain desirable properties, which will hold given that the
assumptions on which the procedure rely are true. These desirable properties
may be described as: validity, optimality, and invariance. Of these "validity"
is most important, followed closely by "optimality". "Invariance" may be
considered as a property of the method of derivation of a confidence interval
rather than of the rule for constructing the interval. In non-standard
applications, the same desirable properties would be sought.
    * Validity. This means that the nominal coverage_probability (confidence
      level) of the confidence interval should hold, either exactly or to a
      good approximation.
    * Optimality. This means that the rule for constructing the confidence
      interval should make as much use of the information in the data-set as
      possible. Recall that one could throw away half of a dataset and still be
      able to derive a valid confidence interval. One way of assessing
      optimality is by the length of the interval so that a rule for
      constructing a confidence interval is judged better than another if it
      leads to intervals whose lengths are typically shorter.
    * Invariance. In many applications, the quantity being estimated might not
      be tightly defined as such. For example, a survey might result in an
      estimate of the median income in a population, but it might equally be
      considered as providing an estimate of the logarithm of the median
      income, given that this is a common scale for presenting graphical
      results. It would be desirable that the method used for constructing a
      confidence interval for the median income would give equivalent results
      when applied to constructing a confidence interval for the logarithm of
      the median income: specifically the values at the ends of the latter
      interval would be the logarithms of the values at the ends of former
      interval.
**** Methods of derivation[edit] ****
For non-standard applications, there are several routes that might be taken to
derive a rule for the construction of confidence intervals. Established rules
for standard procedures might be justified or explained via several of these
routes. Typically a rule for constructing confidence intervals is closely tied
to a particular way of finding a point_estimate of the quantity being
considered.
  Summary_statistics
      This is closely related to the method_of_moments for estimation. A simple
      example arises where the quantity to be estimated is the mean, in which
      case a natural estimate is the sample mean. The usual arguments indicate
      that the sample variance can be used to estimate the variance of the
      sample mean. A confidence interval for the true mean can be constructed
      centered on the sample mean with a width which is a multiple of the
      square root of the sample variance.
  Likelihood theory
      Where estimates are constructed using the maximum_likelihood_principle,
      the theory for this provides two ways of constructing confidence
      intervals or confidence regions for the estimates.[clarification_needed]
      One way is by using Wilks's_theorem to find all the possible values of
      &#x03B8;   {\displaystyle \theta }  [\theta ] that fulfill the following
      restriction:[25]
               ln &#x2061; ( L ( &#x03B8; ) ) &#x2265; ln &#x2061; ( L
            (    &#x03B8; &#x005E;    ) ) &#x2212;   1 2    &#x03C7;  1 , 1
            &#x2212; &#x03B1;   2     {\displaystyle \ln(L(\theta ))\geq \ln(L(
            {\hat {\theta }}))-{\frac {1}{2}}\chi _{1,1-\alpha }^{2}}  [
            {\displaystyle \ln(L(\theta ))\geq \ln(L({\hat {\theta }}))-{\frac
            {1}{2}}\chi _{1,1-\alpha }^{2}}]
  Estimating equations
      The estimation approach here can be considered as both a generalization
      of the method of moments and a generalization of the maximum likelihood
      approach. There are corresponding generalizations of the results of
      maximum likelihood theory that allow confidence intervals to be
      constructed based on estimates derived from estimating_equations.
      [clarification_needed]
  Hypothesis_testing
      If significance tests are available for general values of a parameter,
      then confidence intervals/regions can be constructed by including in the
      100p% confidence region all those points for which the significance test
      of the null hypothesis that the true value is the given value is not
      rejected at a significance level of (1 â p).[15]
  Bootstrapping
      In situations where the distributional assumptions for that above methods
      are uncertain or violated, resampling methods allow construction of
      confidence intervals or prediction intervals. The observed data
      distribution and the internal correlations are used as the surrogate for
      the correlations in the wider population.
***** Examples[edit] *****
**** Practical example[edit] ****
[Margarinefilling.png]
A machine fills cups with a liquid, and is supposed to be adjusted so that the
content of the cups is 250 g of liquid. As the machine cannot fill every cup
with exactly 250.0 g, the content added to individual cups shows some
variation, and is considered a random variable X. This variation is assumed to
be normally_distributed around the desired average of 250 g, with a standard
deviation, Ï, of 2.5 g. To determine if the machine is adequately calibrated,
a sample of n = 25 cups of liquid is chosen at random and the cups are weighed.
The resulting measured masses of liquid are X1, ..., X25, a random sample
from X.
To get an impression of the expectation Î¼, it is sufficient to give an
estimate. The appropriate estimator is the sample mean:
            &#x03BC; &#x005E;    =    X &#x00AF;    =   1 n    &#x2211;  i = 1
      n    X  i   .   {\displaystyle {\hat {\mu }}={\bar {X}}={\frac {1}
      {n}}\sum _{i=1}^{n}X_{i}.}  [{\displaystyle {\hat {\mu }}={\bar {X}}=
      {\frac {1}{n}}\sum _{i=1}^{n}X_{i}.}]
The sample shows actual weights x1, ..., x25, with mean:
            x &#x00AF;    =   1 25    &#x2211;  i = 1   25    x  i   = 250.2
      &#xA0;grams  .   {\displaystyle {\bar {x}}={\frac {1}{25}}\sum _{i=1}^
      {25}x_{i}=250.2{\text{ grams}}.}  [{\displaystyle {\bar {x}}={\frac {1}
      {25}}\sum _{i=1}^{25}x_{i}=250.2{\text{ grams}}.}]
If we take another sample of 25 cups, we could easily expect to find mean
values like 250.4 or 251.1 grams. A sample mean value of 280 grams however
would be extremely rare if the mean content of the cups is in fact close to
250 grams. There is a whole interval around the observed value 250.2 grams of
the sample mean within which, if the whole population mean actually takes a
value in this range, the observed data would not be considered particularly
unusual. Such an interval is called a confidence interval for the parameter Î¼.
How do we calculate such an interval? The endpoints of the interval have to be
calculated from the sample, so they are statistics, functions of the sample
X1, ..., X25 and hence random variables themselves.
In our case we may determine the endpoints by considering that the sample mean
X from a normally distributed sample is also normally distributed, with the
same expectation Î¼, but with a standard_error of:
           &#x03C3;  n    =    2.5  &#xA0;g    25    = 0.5  &#xA0;grams
      {\displaystyle {\frac {\sigma }{\sqrt {n}}}={\frac {2.5{\text{ g}}}{\sqrt
      {25}}}=0.5{\text{ grams}}}  [{\displaystyle {\frac {\sigma }{\sqrt {n}}}=
      {\frac {2.5{\text{ g}}}{\sqrt {25}}}=0.5{\text{ grams}}}]
By standardizing, we get a random variable:
         Z =       X &#x00AF;    &#x2212; &#x03BC;   &#x03C3;  /    n      =
      X &#x00AF;    &#x2212; &#x03BC;  0.5     {\displaystyle Z={\frac {{\bar
      {X}}-\mu }{\sigma /{\sqrt {n}}}}={\frac {{\bar {X}}-\mu }{0.5}}}  [Z=
      {\frac {{\bar {X}}-\mu }{\sigma /{\sqrt {n}}}}={\frac {{\bar {X}}-\mu }
      {0.5}}]
dependent on the parameter Î¼ to be estimated, but with a standard normal
distribution independent of the parameter Î¼. Hence it is possible to find
numbers âz and z, independent of Î¼, between which Z lies with probability
1 â Î±, a measure of how confident we want to be.
We take 1 â Î± = 0.95, for example. So we have:
         P ( &#x2212; z &#x2264; Z &#x2264; z ) = 1 &#x2212; &#x03B1; = 0.95.
      {\displaystyle P(-z\leq Z\leq z)=1-\alpha =0.95.}  [{\displaystyle P(-
      z\leq Z\leq z)=1-\alpha =0.95.}]
The number z follows from the cumulative_distribution_function, in this case
the cumulative_normal_distribution_function:
             &#x03A6; ( z )    = P ( Z &#x2264; z ) = 1 &#x2212;    &#x03B1; 2
      = 0.975 ,     z    =  &#x03A6;  &#x2212; 1   ( &#x03A6; ( z ) ) =
      &#x03A6;  &#x2212; 1   ( 0.975 ) = 1.96 ,       {\displaystyle {\begin
      {aligned}\Phi (z)&=P(Z\leq z)=1-{\tfrac {\alpha }{2}}=0.975,\\
      [6pt]z&=\Phi ^{-1}(\Phi (z))=\Phi ^{-1}(0.975)=1.96,\end{aligned}}}  [
      {\begin{aligned}\Phi (z)&=P(Z\leq z)=1-{\tfrac {\alpha }{2}}=0.975,\\
      [6pt]z&=\Phi ^{-1}(\Phi (z))=\Phi ^{-1}(0.975)=1.96,\end{aligned}}]
and we get:
             0.95    = 1 &#x2212; &#x03B1; = P ( &#x2212; z &#x2264; Z &#x2264;
      z ) = P  (  &#x2212; 1.96 &#x2264;       X &#x00AF;    &#x2212; &#x03BC;
      &#x03C3;  /    n      &#x2264; 1.96  )        = P  (     X &#x00AF;
      &#x2212; 1.96   &#x03C3;  n    &#x2264; &#x03BC; &#x2264;    X &#x00AF;
      + 1.96   &#x03C3;  n     )  .       {\displaystyle {\begin
      {aligned}0.95&=1-\alpha =P(-z\leq Z\leq z)=P\left(-1.96\leq {\frac {{\bar
      {X}}-\mu }{\sigma /{\sqrt {n}}}}\leq 1.96\right)\\[6pt]&=P\left({\bar
      {X}}-1.96{\frac {\sigma }{\sqrt {n}}}\leq \mu \leq {\bar {X}}+1.96{\frac
      {\sigma }{\sqrt {n}}}\right).\end{aligned}}}  [{\displaystyle {\begin
      {aligned}0.95&=1-\alpha =P(-z\leq Z\leq z)=P\left(-1.96\leq {\frac {{\bar
      {X}}-\mu }{\sigma /{\sqrt {n}}}}\leq 1.96\right)\\[6pt]&=P\left({\bar
      {X}}-1.96{\frac {\sigma }{\sqrt {n}}}\leq \mu \leq {\bar {X}}+1.96{\frac
      {\sigma }{\sqrt {n}}}\right).\end{aligned}}}]
In other words, the lower endpoint of the 95% confidence interval is:
          Lower endpoint  =    X &#x00AF;    &#x2212; 1.96   &#x03C3;  n    ,
      {\displaystyle {\text{Lower endpoint}}={\bar {X}}-1.96{\frac {\sigma }
      {\sqrt {n}}},}  [{\displaystyle {\text{Lower endpoint}}={\bar {X}}-1.96
      {\frac {\sigma }{\sqrt {n}}},}]
and the upper endpoint of the 95% confidence interval is:
          Upper endpoint  =    X &#x00AF;    + 1.96   &#x03C3;  n    .
      {\displaystyle {\text{Upper endpoint}}={\bar {X}}+1.96{\frac {\sigma }
      {\sqrt {n}}}.}  [{\displaystyle {\text{Upper endpoint}}={\bar {X}}+1.96
      {\frac {\sigma }{\sqrt {n}}}.}]
With the values in this example, the confidence interval is:
             0.95    = Pr (    X &#x00AF;    &#x2212; 1.96 &#x00D7; 0.5
      &#x2264; &#x03BC; &#x2264;    X &#x00AF;    + 1.96 &#x00D7; 0.5 )       =
      Pr (    X &#x00AF;    &#x2212; 0.98 &#x2264; &#x03BC; &#x2264;    X
      &#x00AF;    + 0.98 ) .       {\displaystyle {\begin{aligned}0.95&=\Pr(
      {\bar {X}}-1.96\times 0.5\leq \mu \leq {\bar {X}}+1.96\times 0.5)\\
      [6pt]&=\Pr({\bar {X}}-0.98\leq \mu \leq {\bar {X}}+0.98).\end{aligned}}}
      [{\displaystyle {\begin{aligned}0.95&=\Pr({\bar {X}}-1.96\times 0.5\leq
      \mu \leq {\bar {X}}+1.96\times 0.5)\\[6pt]&=\Pr({\bar {X}}-0.98\leq \mu
      \leq {\bar {X}}+0.98).\end{aligned}}}]
As the standard deviation of the population Ï is known in this case, the
distribution of the sample mean        X &#x00AF;      {\displaystyle {\bar
{X}}}  [{\bar {X}}] is a normal_distribution with     &#x03BC;   {\displaystyle
\mu }  [\mu ] the only unknown parameter. In the theoretical example below, the
parameter Ï is also unknown, which calls for using the Student's_t-
distribution.
*** Interpretation[edit] ***
This might be interpreted as: with probability 0.95 we will find a confidence
interval in which the value of parameter Î¼ will be between the stochastic
endpoints
             X &#x00AF;    &#x2212; 0  .  98   {\displaystyle \!{\bar {X}}-0
      {.}98}  [\!{\bar {X}}-0{.}98]
and
             X &#x00AF;    + 0.98.   {\displaystyle \!{\bar {X}}+0.98.}  [\!
      {\bar {X}}+0.98.]
This does not mean there is 0.95 probability that the value of parameter Î¼ is
in the interval obtained by using the currently computed value of the sample
mean,
         (    x &#x00AF;    &#x2212; 0.98 ,     x &#x00AF;    + 0.98 ) .
      {\displaystyle ({\bar {x}}-0.98,\,{\bar {x}}+0.98).}  [({\bar {x}}-
      0.98,\,{\bar {x}}+0.98).]
Instead, every time the measurements are repeated, there will be another value
for the mean X of the sample. In 95% of the cases Î¼ will be between the
endpoints calculated from this mean, but in 5% of the cases it will not be. The
actual confidence interval is calculated by entering the measured masses in the
formula. Our 0.95 confidence interval becomes:
         (    x &#x00AF;    &#x2212; 0.98 ;    x &#x00AF;    + 0.98 ) = ( 250.2
      &#x2212; 0.98 ; 250.2 + 0.98 ) = ( 249.22 ; 251.18 ) .    {\displaystyle
      ({\bar {x}}-0.98;{\bar {x}}+0.98)=(250.2-0.98;250.2+0.98)=
      (249.22;251.18).\,}  [({\bar {x}}-0.98;{\bar {x}}+0.98)=(250.2-
      0.98;250.2+0.98)=(249.22;251.18).\,]
The blue vertical line_segments represent 50 realizations of a confidence
interval for the population mean Î¼, represented as a red horizontal dashed
line; note that some confidence intervals do not contain the population mean,
as expected.
In other words, the 95% confidence interval is between the lower endpoint
249.22 g and the upper endpoint 251.18 g.
As the desired value 250 of Î¼ is within the resulted confidence interval,
there is no reason to believe the machine is wrongly calibrated.
The calculated interval has fixed endpoints, where Î¼ might be in between (or
not). Thus this event has probability either 0 or 1. One cannot say: "with
probability (1 â Î±) the parameter Î¼ lies in the confidence interval." One
only knows that by repetition in 100(1 â Î±)% of the cases, Î¼ will be in the
calculated interval. In 100Î±% of the cases however it does not. And
unfortunately one does not know in which of the cases this happens. That is
(instead of using the term "probability") why one can say: "with confidence
level 100(1 â Î±) %, Î¼ lies in the confidence interval."
The maximum error is calculated to be 0.98 since it is the difference between
the value that we are confident of with upper or lower endpoint.
The figure on the right shows 50 realizations of a confidence interval for a
given population mean Î¼. If we randomly choose one realization, the
probability is 95% we end up having chosen an interval that contains the
parameter; however, we may be unlucky and have picked the wrong one. We will
never know; we are stuck with our interval.
**** Theoretical example[edit] ****
Suppose {X1, ..., Xn} is an independent sample from a normally_distributed
population with unknown (parameters) mean Î¼ and variance Ï2. Let
            X &#x00AF;    = (  X  1   + &#x22EF; +  X  n   )  /  n  ,
      {\displaystyle {\bar {X}}=(X_{1}+\cdots +X_{n})/n\,,}  [{\bar {X}}=(X_
      {1}+\cdots +X_{n})/n\,,]
          S  2   =   1  n &#x2212; 1     &#x2211;  i = 1   n   (  X  i
      &#x2212;    X &#x00AF;      )  2   .   {\displaystyle S^{2}={\frac {1}{n-
      1}}\sum _{i=1}^{n}(X_{i}-{\bar {X}}\,)^{2}.}  [{\displaystyle S^{2}=
      {\frac {1}{n-1}}\sum _{i=1}^{n}(X_{i}-{\bar {X}}\,)^{2}.}]
Where X is the sample_mean, and S2 is the sample_variance. Then
         T =       X &#x00AF;    &#x2212; &#x03BC;   S  /    n
      {\displaystyle T={\frac {{\bar {X}}-\mu }{S/{\sqrt {n}}}}}  [T={\frac {
      {\bar {X}}-\mu }{S/{\sqrt {n}}}}]
has a Student's_t-distribution with n â 1 degrees of freedom.[26] Note that
the distribution of T does not depend on the values of the unobservable
parameters Î¼ and Ï2; i.e., it is a pivotal_quantity. Suppose we wanted to
calculate a 95% confidence interval for Î¼. Then, denoting c as the 97.5th
percentile of this distribution,
         Pr ( &#x2212; c &#x2264; T &#x2264; c ) = 0.95    {\displaystyle \Pr(-
      c\leq T\leq c)=0.95\,}  [{\displaystyle \Pr(-c\leq T\leq c)=0.95\,}]
("97.5th" and "0.95" are correct in the preceding expressions. There is a 2.5%
chance that T will be less than âc and a 2.5% chance that it will be larger
than +c. Thus, the probability that T will be between âc and +c is 95%.)
Consequently,
         Pr  (     X &#x00AF;    &#x2212;    c S   n    &#x2264; &#x03BC;
      &#x2264;    X &#x00AF;    +    c S   n     )  = 0.95    {\displaystyle
      \Pr \left({\bar {X}}-{\frac {cS}{\sqrt {n}}}\leq \mu \leq {\bar {X}}+
      {\frac {cS}{\sqrt {n}}}\right)=0.95\,}  [\Pr \left({\bar {X}}-{\frac {cS}
      {\sqrt {n}}}\leq \mu \leq {\bar {X}}+{\frac {cS}{\sqrt
      {n}}}\right)=0.95\,]
and we have a theoretical (stochastic) 95% confidence interval for Î¼.
After observing the sample we find values x for X and s for S, from which we
compute the confidence interval
          [     x &#x00AF;    &#x2212;    c s   n    ,    x &#x00AF;    +    c
      s   n     ]  ,    {\displaystyle \left[{\bar {x}}-{\frac {cs}{\sqrt
      {n}}},{\bar {x}}+{\frac {cs}{\sqrt {n}}}\right],\,}  [\left[{\bar {x}}-
      {\frac {cs}{\sqrt {n}}},{\bar {x}}+{\frac {cs}{\sqrt {n}}}\right],\,]
an interval with fixed numbers as endpoints, of which we can no longer say
there is a certain probability it contains the parameter Î¼; either Î¼ is in
this interval or isn't.
***** Alternatives and critiques[edit] *****
Main article: Interval_estimation
Confidence intervals are one method of interval_estimation, and the most widely
used in frequentist_statistics. An analogous concept in Bayesian_statistics is
credible_intervals, while an alternative frequentist method is that of
prediction_intervals which, rather than estimating parameters, estimate the
outcome of future samples. For other approaches to expressing uncertainty using
intervals, see interval_estimation.
**** Comparison to prediction intervals[edit] ****
Main article: Prediction_interval
A prediction_interval for a random_variable is defined similarly to a
confidence interval for a statistical_parameter. Consider an additional random
variable Y which may or may not be statistically dependent on the random_sample
X. Then (u(X), v(X)) provides a prediction_interval for the as-yet-to-be
observed value y of Y if
           Pr   &#x03B8; , &#x03C6;   ( u ( X ) < Y < v ( X ) ) = &#x03B3;
      &#xA0;for all&#xA0;  ( &#x03B8; , &#x03C6; ) .    {\displaystyle {\Pr }_
      {\theta ,\varphi }(u(X)<Y<v(X))=\gamma {\text{ for all }}(\theta ,\varphi
      ).\,}  [{\displaystyle {\Pr }_{\theta ,\varphi }(u(X)<Y<v(X))=\gamma
      {\text{ for all }}(\theta ,\varphi ).\,}]
Here PrÎ¸,Ï indicates the joint_probability_distribution of the random
variables (X, Y), where this distribution depends on the statistical
parameters (Î¸, Ï).
**** Comparison to tolerance intervals[edit] ****
Main article: Tolerance_interval
[[icon]] This section needs expansion. You can help by adding_to_it. (September
         2014)
**** Comparison to Bayesian interval estimates[edit] ****
See also: Credible_interval_Â§ Confidence_interval
A Bayesian interval estimate is called a credible_interval. Using much of the
same notation as above, the definition of a credible interval for the unknown
true value of Î¸ is, for a given Î³,[27]
         Pr ( u ( x ) < &#x0398; < v ( x ) &#x2223; X = x ) = &#x03B3; .
      {\displaystyle \Pr(u(x)<\Theta <v(x)\mid X=x)=\gamma .\,}  [
      {\displaystyle \Pr(u(x)<\Theta <v(x)\mid X=x)=\gamma .\,}]
Here Î is used to emphasize that the unknown value of Î¸ is being treated as a
random variable. The definitions of the two types of intervals may be compared
as follows.
    * The definition of a confidence interval involves probabilities calculated
      from the distribution of X for a given (Î¸, Ï) (or conditional on these
      values) and the condition needs to hold for all values of (Î¸, Ï).
    * The definition of a credible interval involves probabilities calculated
      from the distribution of Î conditional on the observed values of X = x
      and marginalised (or averaged) over the values of Î¦, where this last
      quantity is the random variable corresponding to the uncertainty about
      the nuisance_parameters in Ï.
Note that the treatment of the nuisance_parameters above is often omitted from
discussions comparing confidence and credible intervals but it is markedly
different between the two cases.
In some simple standard cases, the intervals produced as confidence and
credible intervals from the same data set can be identical. They are very
different if informative prior_information is included in the Bayesian
analysis, and may be very different for some parts of the space of possible
data even if the Bayesian prior is relatively uninformative.
There is disagreement about which of these methods produces the most useful
results: the mathematics of the computations are rarely in
questionâconfidence intervals being based on sampling distributions, credible
intervals being based on Bayes'_theoremâbut the application of these methods,
the utility and interpretation of the produced statistics, is debated.
**** Confidence intervals for proportions and related quantities[edit] ****
See also: Margin_of_error and Binomial_proportion_confidence_interval
An approximate confidence interval for a population mean can be constructed for
random variables that are not normally distributed in the population, relying
on the central_limit_theorem, if the sample_sizes and counts are big enough.
The formulae are identical to the case above (where the sample mean is actually
normally distributed about the population mean). The approximation will be
quite good with only a few dozen observations in the sample if the probability
distribution of the random variable is not too different from the normal
distribution (e.g. its cumulative_distribution_function does not have any
discontinuities and its skewness is moderate).
One type of sample mean is the mean of an indicator_variable, which takes on
the value 1 for true and the value 0 for false. The mean of such a variable is
equal to the proportion that has the variable equal to one (both in the
population and in any sample). This is a useful property of indicator
variables, especially for hypothesis testing. To apply the central_limit
theorem, one must use a large enough sample. A rough rule of thumb is that one
should see at least 5 cases in which the indicator is 1 and at least 5 in which
it is 0. Confidence intervals constructed using the above formulae may include
negative numbers or numbers greater than 1, but proportions obviously cannot be
negative or exceed 1. Additionally, sample proportions can only take on a
finite number of values, so the central_limit_theorem and the normal
distribution are not the best tools for building a confidence interval. See
"Binomial_proportion_confidence_interval" for better methods which are specific
to this case.
**** Counter-examples[edit] ****
Since confidence interval theory was proposed, a number of counter-examples to
the theory have been developed to show how the interpretation of confidence
intervals can be problematic, at least if one interprets them naÃ¯vely.
*** Confidence procedure for uniform location[edit] ***
Welch [28] presented an example which clearly shows the difference between the
theory of confidence intervals and other theories of interval estimation
(including Fisher's fiducial intervals and objective Bayesian intervals).
Robinson [29] called this example "[p]ossibly the best known counterexample for
Neyman's version of confidence interval theory." To Welch, it showed the
superiority of confidence interval theory; to critics of the theory, it shows a
deficiency. Here we present a simplified version.
Suppose that      X  1   ,  X  2     {\displaystyle X_{1},X_{2}}  [X_{1},X_{2}]
are independent observations from a Uniform(Î¸ â 1/2, Î¸ + 1/2) distribution.
Then the optimal 50% confidence procedure[30] is
            X &#x00AF;    &#x00B1;   {         |   X  1   &#x2212;  X  2    |
      2       if&#xA0;   |   X  1   &#x2212;  X  2    |  < 1  /  2         1
      &#x2212;  |   X  1   &#x2212;  X  2    |   2       if&#xA0;   |   X  1
      &#x2212;  X  2    |  &#x2265; 1  /  2.         {\displaystyle {\bar
      {X}}\pm {\begin{cases}{\dfrac {|X_{1}-X_{2}|}{2}}&{\text{if }}|X_{1}-X_
      {2}|<1/2\\[8pt]{\dfrac {1-|X_{1}-X_{2}|}{2}}&{\text{if }}|X_{1}-X_
      {2}|\geq 1/2.\end{cases}}}  [{\displaystyle {\bar {X}}\pm {\begin{cases}
      {\dfrac {|X_{1}-X_{2}|}{2}}&{\text{if }}|X_{1}-X_{2}|<1/2\\[8pt]{\dfrac
      {1-|X_{1}-X_{2}|}{2}}&{\text{if }}|X_{1}-X_{2}|\geq 1/2.\end{cases}}}]
A fiducial or objective Bayesian argument can be used to derive the interval
estimate
            X &#x00AF;    &#x00B1;    1 &#x2212;  |   X  1   &#x2212;  X  2
      |   4   ,   {\displaystyle {\bar {X}}\pm {\frac {1-|X_{1}-X_{2}|}{4}},}
      [{\displaystyle {\bar {X}}\pm {\frac {1-|X_{1}-X_{2}|}{4}},}]
which is also a 50% confidence procedure. Welch showed that the first
confidence procedure dominates the second, according to desiderata from
confidence interval theory; for every      &#x03B8;  1   &#x2260; &#x03B8;
{\displaystyle \theta _{1}\neq \theta }  [{\displaystyle \theta _{1}\neq \theta
}], the probability that the first procedure contains      &#x03B8;  1
{\displaystyle \theta _{1}}  [\theta _{1}] is less than or equal to the
probability that the second procedure contains      &#x03B8;  1
{\displaystyle \theta _{1}}  [\theta _{1}]. The average width of the intervals
from the first procedure is less than that of the second. Hence, the first
procedure is preferred under classical confidence interval theory.
However, when      |   X  1   &#x2212;  X  2    |  &#x2265; 1  /  2
{\displaystyle |X_{1}-X_{2}|\geq 1/2}  [{\displaystyle |X_{1}-X_{2}|\geq 1/2}],
intervals from the first procedure are guaranteed to contain the true value
&#x03B8;   {\displaystyle \theta }  [\theta ]: Therefore, the nominal 50%
confidence coefficient is unrelated to the uncertainty we should have that a
specific interval contains the true value. The second procedure does not have
this property.
Moreover, when the first procedure generates a very short interval, this
indicates that      X  1   ,  X  2     {\displaystyle X_{1},X_{2}}  [X_{1},X_
{2}] are very close together and hence only offer the information in a single
data point. Yet the first interval will exclude almost all reasonable values of
the parameter due to its short width. The second procedure does not have this
property.
The two counter-intuitive properties of the first procedureâ100% coverage
when      X  1   ,  X  2     {\displaystyle X_{1},X_{2}}  [X_{1},X_{2}] are far
apart and almost 0% coverage when      X  1   ,  X  2     {\displaystyle X_
{1},X_{2}}  [X_{1},X_{2}] are close togetherâbalance out to yield 50%
coverage on average. However, despite the first procedure being optimal, its
intervals offer neither an assessment of the precision of the estimate nor an
assessment of the uncertainty one should have that the interval contains the
true value.
This counter-example is used to argue against naÃ¯ve interpretations of
confidence intervals. If a confidence procedure is asserted to have properties
beyond that of the nominal coverage (such as relation to precision, or a
relationship with Bayesian inference), those properties must be proved; they do
not follow from the fact that a procedure is a confidence procedure.
*** Confidence procedure for Ï2[edit] ***
Steiger[31] suggested a number of confidence procedures for common effect_size
measures in ANOVA. Morey et al.[10] point out that several of these confidence
procedures, including the one for Ï2, have the property that as the F
statistic becomes increasingly smallâindicating misfit with all possible
values of Ï2âthe confidence interval shrinks and can even contain only the
single value Ï2 = 0; that is, the CI is infinitesimally narrow (this occurs
when     p &#x2265; 1 &#x2212; &#x03B1;  /  2   {\displaystyle p\geq 1-\alpha /
2}  [{\displaystyle p\geq 1-\alpha /2}] for a     100 ( 1 &#x2212; &#x03B1; )
&#x0025;   {\displaystyle 100(1-\alpha )\%}  [100(1-\alpha)\%] CI).
This behavior is consistent with the relationship between the confidence
procedure and significance testing: as F becomes so small that the group means
are much closer together than we would expect by chance, a significance test
might indicate rejection for most or all values of Ï2. Hence the interval will
be very narrow or even empty (or, by a convention suggested by Steiger,
containing only 0). However, this does not indicate that the estimate of Ï2 is
very precise. In a sense, it indicates the opposite: that the trustworthiness
of the results themselves may be in doubt. This is contrary to the common
interpretation of confidence intervals that they reveal the precision of the
estimate.
***** See also[edit] *****
    * Cumulative_distribution_function-based_nonparametric_confidence_interval
    * CLs_upper_limits_(particle_physics)
    * Confidence_distribution
    * Credence_(statistics)
    * Error_bar
    * Estimation_statistics
    * p-value
    * Robust_confidence_intervals
    * Confidence_region
    * Credible_interval
**** Confidence interval for specific distributions[edit] ****
    * Confidence_interval_for_binomial_distribution
    * Confidence_interval_for_exponent_of_the_power_law_distribution
    * Confidence_interval_for_mean_of_the_exponential_distribution
    * Confidence_interval_for_mean_of_the_Poisson_distribution
    * Confidence_intervals_for_mean_and_variance_of_the_normal_distribution
***** References[edit] *****
   1. ^ a b Cox D.R., Hinkley D.V. (1974) Theoretical Statistics, Chapman &
      Hall, p49, p209
   2. ^ Kendall, M.G. and Stuart, D.G. (1973) The Advanced Theory of
      Statistics. Vol 2: Inference and Relationship, Griffin, London. Section
      20.4
   3. ^ a b c dNeyman,_J. (1937). "Outline of a Theory of Statistical
      Estimation Based on the Classical Theory of Probability". Philosophical
      Transactions_of_the_Royal_Society_A. 236 (767): 333â380. Bibcode:
      1937RSPTA.236..333N. doi:10.1098/rsta.1937.0005. JSTOR 91337.
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
   5. ^Zar, Jerrold H. (199). Biostatistical Analysis (4th ed.). Upper Saddle
      River, N.J.: Prentice Hall. pp. 43â45. ISBN 978-0130815422.
      OCLC 39498633.
   6. ^ Cox D.R., Hinkley D.V. (1974) Theoretical Statistics, Chapman & Hall,
      pp 214, 225, 233
   7. ^ [1]
   8. ^"Archived_copy" (PDF). Archived from the_original (PDF) on 2016-03-04.
      Retrieved 2014-09-16.CS1 maint: Archived copy as title (link)
   9. ^ Hoekstra, R., R. D. Morey, J. N. Rouder, and E-J. Wagenmakers, 2014.
      Robust misinterpretation of confidence intervals. Psychonomic Bulletin
      Review, in press. [2]
  10. ^ Scientistsâ_grasp_of_confidence_intervals_doesnât_inspire
      confidence, Science_News, July 3, 2014
  11. ^ a bMorey, R. D.; Hoekstra, R.; Rouder, J. N.; Lee, M. D.; Wagenmakers,
      E.-J. (2016). "The_Fallacy_of_Placing_Confidence_in_Confidence
      Intervals". Psychonomic Bulletin & Review. 23 (1): 103â123. doi:
      10.3758/s13423-015-0947-8. PMC 4742505. PMID 26450628.
  12. ^"1.3.5.2._Confidence_Limits_for_the_Mean". nist.gov. Archived from the
      original on 2008-02-05. Retrieved 2014-09-16.
  13. ^ Mayo, D. G. (1981) "In_defence_of_the_Neyman-Pearson_theory_of
      confidence_intervals", Philosophy of Science, 48 (2), 269â280.
      JSTOR 187185
  14. ^ T. Seidenfeld, Philosophical Problems of Statistical Inference:
      Learning from R.A. Fisher, Springer-Verlag, 1979
  15. ^"Statistical_significance_defined_using_the_five_sigma_standard".
  16. ^ a b Cox D.R., Hinkley D.V. (1974) Theoretical Statistics, Chapman &
      Hall, Section 7.2(iii)
  17. ^ Pav Kalinowski, "Understanding_Confidence_Intervals_(CIs)_and_Effect
      Size_Estimation", Observer Vol.23, No.4 April 2010.
  18. ^ Andrea Knezevic, "Overlapping_Confidence_Intervals_and_Statistical
      Significance", StatNews # 73: Cornell Statistical Consulting Unit,
      October 2008.
  19. ^Goldstein, H.; Healey, M.J.R. (1995). "The graphical presentation of a
      collection of means". Journal of the Royal Statistical Society. 158 (1):
      175â77. CiteSeerX 10.1.1.649.5259. doi:10.2307/2983411. JSTOR 2983411.
  20. ^Wolfe R, Hanley J (Jan 2002). "If_we're_so_different,_why_do_we_keep
      overlapping?_When_1_plus_1_doesn't_make_2". CMAJ. 166 (1): 65â6.
      PMC 99228. PMID 11800251.
  21. ^ Daniel Smith, "Overlapping_confidence_intervals_are_not_a_statistical
      test", California Dept of Health Services, 26th Annual Institute on
      Research and Statistics, Sacramento, CA, March, 2005.
  22. ^ p.65 in W. HÃ¤rdle, M. MÃ¼ller, S. Sperlich, A. Werwatz (2004),
      Nonparametric and Semiparametric Models, Springer,
  23. ISBN 3-540-20722-8
  24. ^"Checking_Out_Statistical_Confidence_Interval_Critical_Values_â_For
      Dummies". www.dummies.com. Retrieved 2016-02-11.
  25. ^"Confidence_Intervals". www.stat.yale.edu. Retrieved 2016-02-11.
  26. ^ George G. Roussas (1997) A Course in Mathematical Statistics, 2nd
      Edition, Academic Press, p397
  27. ^ Abramovich, Felix, and Ya'acov Ritov. Statistical Theory: A Concise
      Introduction. CRC Press, 2013. Pages 121â122
  28. ^ Rees. D.G. (2001) Essential Statistics, 4th Edition, Chapman and Hall/
      CRC.
  29. ISBN 1-58488-007-4 (Section 9.5)
  30. ^Bernardo JE, Smith, Adrian (2000). Bayesian theory. New York: Wiley.
      p. 259. ISBN 978-0-471-49464-5.CS1 maint: Multiple names: authors list
      (link)
  31. ^Welch, B. L. (1939). "On Confidence Limits and Sufficiency, with
      Particular Reference to Parameters of Location". The Annals of
      Mathematical Statistics. 10 (1): 58â69. doi:10.1214/aoms/1177732246.
      JSTOR 2235987.
  32. ^Robinson, G. K. (1975). "Some Counterexamples to the Theory of
      Confidence Intervals". Biometrika. 62 (1): 155â161. doi:10.2307/
      2334498. JSTOR 2334498.
  33. ^Pratt, J. W. (1961). "Book Review: Testing Statistical Hypotheses. by E.
      L. Lehmann". Journal of the American Statistical Association. 56 (293):
      163â167. doi:10.1080/01621459.1961.10482103. JSTOR 2282344.
  34. ^Steiger, J. H. (2004). "Beyond_the_F_test:_Effect_size_confidence
      intervals_and_tests_of_close_fit_in_the_analysis_of_variance_and_contrast
      analysis". Psychological Methods. 9 (2): 164â182. doi:10.1037/1082-
      989x.9.2.164. PMID 15137887.
***** Bibliography[edit] *****
    * Fisher,_R.A. (1956) Statistical Methods and Scientific Inference. Oliver
      and Boyd, Edinburgh. (See p. 32.)
    * Freund, J.E. (1962) Mathematical Statistics Prentice Hall, Englewood
      Cliffs, NJ. (See pp. 227â228.)
    * Hacking,_I. (1965) Logic of Statistical Inference. Cambridge University
      Press, Cambridge.
ISBN 0-521-05165-7
Keeping, E.S. (1962) Introduction to Statistical Inference. D. Van Nostrand,
Princeton, NJ.
Kiefer,_J. (1977). "Conditional Confidence Statements and Confidence Estimators
(with discussion)". Journal of the American Statistical Association. 72 (360a):
789â827. doi:10.1080/01621459.1977.10479956. JSTOR 2286460.
Mayo, D. G. (1981) "In_defence_of_the_Neyman-Pearson_theory_of_confidence
intervals", Philosophy of Science, 48 (2), 269â280. JSTOR 187185
Neyman,_J. (1937) "Outline_of_a_Theory_of_Statistical_Estimation_Based_on_the
Classical_Theory_of_Probability" Philosophical Transactions of the Royal
Society of London A, 236, 333â380. (Seminal work.)
Robinson, G.K. (1975). "Some Counterexamples to the Theory of Confidence
Intervals". Biometrika. 62 (1): 155â161. doi:10.1093/biomet/62.1.155.
JSTOR 2334498.
Savage, L. J. (1962), The Foundations of Statistical Inference. Methuen,
London.
Smithson, M. (2003) Confidence intervals. Quantitative Applications in the
Social Sciences Series, No. 140. Belmont, CA: SAGE Publications.
ISBN 978-0-7619-2499-9.
    * Mehta,_S. (2014) Statistics Topics
ISBN 978-1-4992-7353-3
Hazewinkel,_Michiel, ed. (2001) [1994], "Confidence_estimation", Encyclopedia
of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
Publishers, ISBN 978-1-55608-010-4
Morey, R. D.; Hoekstra, R.; Rouder, J. N.; Lee, M. D.; Wagenmakers, E.-J.
(2016). "The_fallacy_of_placing_confidence_in_confidence_intervals".
Psychonomic Bulletin & Review. 23 (1): 103â123. doi:10.3758/s13423-015-0947-
8. PMC 4742505. PMID 26450628.
**** External links[edit] ****
 Wikimedia Commons has media related to Confidence_interval.
    * The_Exploratory_Software_for_Confidence_Intervals_tutorial_programs_that
      run_under_Excel
    * Confidence interval calculators for R-Squares, Regression_Coefficients,
      and Regression_Intercepts
    * Weisstein,_Eric_W. "Confidence_Interval". MathWorld.
CAUSEweb.org Many resources for teaching statistics including Confidence
Intervals.
An_interactive_introduction_to_Confidence_Intervals
Confidence_Intervals:_Confidence_Level,_Sample_Size,_and_Margin_of_Error by
Eric Schulz, the Wolfram_Demonstrations_Project.
Confidence_Intervals_in_Public_Health. Straightforward description with
examples and what to do about small sample sizes or rates near 0.
**** Online calculators[edit] ****
    * GraphPad_QuickCalcs
    * TAMU's_Confidence_Interval_Calculators
    * MBAStats_confidence_interval_and_hypothesis_test_calculators
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
                                    * Confidence interval
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

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Confidence_interval&oldid=909434076"
Categories:
    * Quantitative_marketing_research
    * Psephology
    * Biostatistics
    * Statistical_intervals
Hidden categories:
    * CS1_maint:_Archived_copy_as_title
    * CS1_maint:_Multiple_names:_authors_list
    * Articles_needing_expert_attention_from_November_2018
    * All_articles_needing_expert_attention
    * Statistics_articles_needing_expert_attention
    * Wikipedia_articles_needing_clarification_from_November_2013
    * Wikipedia_articles_needing_clarification_from_July_2014
    * Articles_to_be_expanded_from_September_2014
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
    * Commons_category_link_from_Wikidata
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
    * AzÉrbaycanca
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
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
    * à²à²¨à³à²¨à²¡
    * LietuviÅ³
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Basa_Sunda
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ä¸­æ
Edit_links
    * This page was last edited on 5 August 2019, at 11:57 (UTC).
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
