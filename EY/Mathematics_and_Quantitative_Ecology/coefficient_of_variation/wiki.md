The following text has been accessed from https://en.wikipedia.org/wiki/Coefficient_of_variation at Fri Aug 9 04:00:47 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Coefficient of variation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with Coefficient_of_determination.
Statistical parameter
In probability_theory and statistics, the coefficient of variation (CV), also
known as relative standard deviation (RSD), is a standardized measure of
dispersion of a probability_distribution or frequency_distribution. It is often
expressed as a percentage, and is defined as the ratio of the standard
deviation     &#xA0; &#x03C3;   {\displaystyle \ \sigma }  [\ \sigma ] to the
mean     &#xA0; &#x03BC;   {\displaystyle \ \mu }  [\ \mu ] (or its absolute
value,      |  &#x03BC;  |    {\displaystyle |\mu |}  [|\mu |]). The CV or RSD
is widely used in analytical_chemistry to express the precision and
repeatability of an assay. It is also commonly used in fields such as
engineering or physics when doing quality assurance studies and ANOVA_gauge
R&R.[citation_needed] In addition, CV is utilized by economists and investors
in economic_models and in determining the volatility of a security[citation
needed].
⁰
***** Contents *****
    * 1_Definition
    * 2_Examples
    * 3_Examples_of_misuse
    * 4_Estimation
          o 4.1_Log-normal_data
    * 5_Comparison_to_standard_deviation
          o 5.1_Advantages
          o 5.2_Disadvantages
    * 6_Applications
          o 6.1_Laboratory_measures_of_intra-assay_and_inter-assay_CVs
          o 6.2_As_a_measure_of_economic_inequality
    * 7_Distribution
          o 7.1_Alternative
    * 8_Similar_ratios
    * 9_See_also
    * 10_References
    * 11_External_links
***** Definition[edit] *****
The coefficient of variation (CV) is defined as the ratio of the standard
deviation     &#xA0; &#x03C3;   {\displaystyle \ \sigma }  [\ \sigma ] to the
mean     &#xA0; &#x03BC;   {\displaystyle \ \mu }  [\ \mu ]:[1]      c   v    =
&#x03C3; &#x03BC;   .   {\displaystyle c_{\rm {v}}={\frac {\sigma }{\mu }}.}  [
{\displaystyle c_{\rm {v}}={\frac {\sigma }{\mu }}.}] It shows the extent of
variability in relation to the mean of the population. The coefficient of
variation should be computed only for data measured on a ratio_scale, as these
are the measurements that allow the division operation. The coefficient of
variation may not have any meaning for data on an interval_scale.[2] For
example, most temperature scales (e.g., Celsius, Fahrenheit etc.) are interval
scales with arbitrary zeros, so the coefficient of variation would be different
depending on which scale you used. On the other hand, Kelvin temperature has a
meaningful zero, the complete absence of thermal energy, and thus is a ratio
scale. While the standard deviation (SD) can be meaningfully derived using
Kelvin, Celsius, or Fahrenheit, the CV is only valid as a measure of relative
variability for the Kelvin scale because its computation involves division.
Measurements that are log-normally distributed exhibit stationary CV; in
contrast, SD varies depending upon the expected value of measurements.
A more robust possibility is the quartile_coefficient_of_dispersion, half the
interquartile_range      (  Q  3   &#x2212;  Q  1   )  /  2    {\displaystyle {
(Q_{3}-Q_{1})/2}}  [{\displaystyle {(Q_{3}-Q_{1})/2}}] divided by the average
of the quartiles (the midhinge),      (  Q  1   +  Q  3   )  /  2
{\displaystyle {(Q_{1}+Q_{3})/2}}  [{\displaystyle {(Q_{1}+Q_{3})/2}}].
In most cases, a CV is computed for a single independent variable (e.g., a
single factory product) with numerous, repeated measures of a dependent
variable (e.g., error in the production process). However, data that are linear
or even logarithmically non-linear and include a continuous range for the
independent variable with sparse measurements across each value (e.g., scatter-
plot) may be amenable to single CV calculation using a maximum-likelihood
estimation approach.[3]
***** Examples[edit] *****
A data set of [100, 100, 100] has constant values. Its standard deviation is 0
and average is 100, giving the coefficient of variation as
      0 / 100 = 0%
A data set of [90, 100, 110] has more variability. Its standard deviation is 10
and its average is 100, giving the coefficient of variation as
      10 / 100 = 10%
A data set of [1, 5, 6, 8, 10, 40, 65, 88] has still more variability. Its
standard deviation is 32.9 and its average is 27.9, giving a coefficient of
variation of
      32.9 / 27.9 = 118%
***** Examples of misuse[edit] *****
Comparing coefficients of variation between parameters using relative units can
result in differences that may not be real. If we compare the same set of
temperatures in Celsius and Fahrenheit (both relative units, where kelvin and
Rankine_scale are their associated absolute values):
Celsius: [0, 10, 20, 30, 40]
Fahrenheit: [32, 50, 68, 86, 104]
The sample_standard_deviations are 15.81 and 28.46, respectively. The CV of the
first set is 15.81/20 = 79%. For the second set (which are the same
temperatures) it is 28.46/68 = 42%.
If, for example, the data sets are temperature readings from two different
sensors (a Celsius sensor and a Fahrenheit sensor) and you want to know which
sensor is better by picking the one with the least variance, then you will be
misled if you use CV. The problem here is that you have divided by a relative
value rather than an absolute.
Comparing the same data set, now in absolute units:
Kelvin: [273.15, 283.15, 293.15, 303.15, 313.15]
Rankine: [491.67, 509.67, 527.67, 545.67, 563.67]
The sample_standard_deviations are still 15.81 and 28.46, respectively, because
the standard deviation is not affected by a constant offset. The coefficients
of variation, however, are now both equal to 5.39%.
***** Estimation[edit] *****
When only a sample of data from a population is available, the population CV
can be estimated using the ratio of the sample_standard_deviation     s
{\displaystyle s\,}  [s\,] to the sample mean        x &#x00AF;
{\displaystyle {\bar {x}}}  [{\bar {x}}]:
             c   v    &#x005E;    =   s   x &#x00AF;       {\displaystyle
      {\widehat {c_{\rm {v}}}}={\frac {s}{\bar {x}}}}  [{\displaystyle
      {\widehat {c_{\rm {v}}}}={\frac {s}{\bar {x}}}}]
But this estimator, when applied to a small or moderately sized sample, tends
to be too low: it is a biased_estimator. For normally_distributed data, an
unbiased estimator[4] for a sample of size n is:
              c   v    &#x005E;     &#x2217;   =   (   1 +   1  4 n      )
      c   v    &#x005E;      {\displaystyle {\widehat {c_{\rm {v}}}}^{*}={\bigg
      (}1+{\frac {1}{4n}}{\bigg )}{\widehat {c_{\rm {v}}}}}  [{\displaystyle
      {\widehat {c_{\rm {v}}}}^{*}={\bigg (}1+{\frac {1}{4n}}{\bigg )}{\widehat
      {c_{\rm {v}}}}}]
**** Log-normal data[edit] ****
In many applications, it can be assumed that data are log-normally distributed
(evidenced by the presence of skewness in the sampled data).[5] In such cases,
a more accurate estimate, derived from the properties of the log-normal
distribution,[6][7][8] is defined as:
              c   v    &#x005E;      l n    =     e    s   l n    2
      &#x2212; 1     {\displaystyle {\widehat {c_{\rm {v}}}}_{\rm {ln}}={\sqrt
      {\mathrm {e} ^{s_{\rm {ln}}^{2}}-1}}}  [{\displaystyle {\widehat {c_{\rm
      {v}}}}_{\rm {ln}}={\sqrt {\mathrm {e} ^{s_{\rm {ln}}^{2}}-1}}}]
where       s   l n        {\displaystyle {s_{\rm {ln}}}\,}  [{\displaystyle
{s_{\rm {ln}}}\,}] is the sample standard deviation of the data after a natural
log transformation. (In the event that measurements are recorded using any
other logarithmic base, b, their standard deviation      s  b
{\displaystyle s_{b}\,}  [s_b \,] is converted to base e using      s   l n
=  s  b   ln &#x2061; ( b )    {\displaystyle s_{\rm {ln}}=s_{b}\ln(b)\,}  [
{\displaystyle s_{\rm {ln}}=s_{b}\ln(b)\,}], and the formula for          c   v
&#x005E;      l n       {\displaystyle {\widehat {c_{\rm {v}}}}_{\rm {ln}}\,}
[{\displaystyle {\widehat {c_{\rm {v}}}}_{\rm {ln}}\,}] remains the same.[9])
This estimate is sometimes referred to as the "geometric CV"[10][11] in order
to distinguish it from the simple estimate above. However, "geometric
coefficient of variation" has also been defined by Kirkwood[12] as:
          G C  V  K    =    e    s   l n        &#x2212; 1    {\displaystyle
      \mathrm {GCV_{K}} ={\mathrm {e} ^{s_{\rm {ln}}}\!\!-1}}  [{\displaystyle
      \mathrm {GCV_{K}} ={\mathrm {e} ^{s_{\rm {ln}}}\!\!-1}}]
This term was intended to be analogous to the coefficient of variation, for
describing multiplicative variation in log-normal data, but this definition of
GCV has no theoretical basis as an estimate of      c   v       {\displaystyle
c_{\rm {v}}\,}  [{\displaystyle c_{\rm {v}}\,}] itself.
For many practical purposes (such as sample_size_determination and calculation
of confidence_intervals) it is      s  l n      {\displaystyle s_{ln}\,}  [s_
{ln} \,] which is of most use in the context of log-normally distributed data.
If necessary, this can be derived from an estimate of      c   v
{\displaystyle c_{\rm {v}}\,}  [{\displaystyle c_{\rm {v}}\,}] or GCV by
inverting the corresponding formula.
***** Comparison to standard deviation[edit] *****
**** Advantages[edit] ****
The coefficient of variation is useful because the standard deviation of data
must always be understood in the context of the mean of the data. In contrast,
the actual value of the CV is independent of the unit in which the measurement
has been taken, so it is a dimensionless_number. For comparison between data
sets with different units or widely different means, one should use the
coefficient of variation instead of the standard deviation.
**** Disadvantages[edit] ****
    * When the mean value is close to zero, the coefficient of variation will
      approach infinity and is therefore sensitive to small changes in the
      mean. This is often the case if the values do not originate from a ratio
      scale.
    * Unlike the standard deviation, it cannot be used directly to construct
      confidence_intervals for the mean.
    * CVs are not an ideal index of the certainty of measurement when the
      number of replicates varies across samples because CV is invariant to the
      number of replicates while the certainty of the mean improves with
      increasing replicates. In this case, standard error in percent is
      suggested to be superior.[13]
***** Applications[edit] *****
The coefficient of variation is also common in applied probability fields such
as renewal_theory, queueing_theory, and reliability_theory. In these fields,
the exponential_distribution is often more important than the normal
distribution. The standard deviation of an exponential_distribution is equal to
its mean, so its coefficient of variation is equal to 1. Distributions with CV
< 1 (such as an Erlang_distribution) are considered low-variance, while those
with CV > 1 (such as a hyper-exponential_distribution) are considered high-
variance[citation_needed]. Some formulas in these fields are expressed using
the squared coefficient of variation, often abbreviated SCV. In modeling, a
variation of the CV is the CV(RMSD). Essentially the CV(RMSD) replaces the
standard deviation term with the Root_Mean_Square_Deviation_(RMSD). While many
natural processes indeed show a correlation between the average value and the
amount of variation around it, accurate sensor devices need to be designed in
such a way that the coefficient of variation is close to zero, i.e., yielding a
constant absolute_error over their working range.
In actuarial_science, the CV is known as unitized risk.[14]
In Industrial Solids Processing, CV is particularly important to measure the
degree of homogeneity of a powder mixture. Comparing the calculated CV to a
specification will allow to define if a sufficient degree of mixing has been
reached.[15]
**** Laboratory measures of intra-assay and inter-assay CVs[edit] ****
CV measures are often used as quality controls for quantitative laboratory
assays. While intra-assay and inter-assay CVs might be assumed to be calculated
by simply averaging CV values across CV values for multiple samples within one
assay or by averaging multiple inter-assay CV estimates, it has been suggested
that these practices are incorrect and that a more complex computational
process is required.[16] It has also been noted that CV values are not an ideal
index of the certainty of a measurement when the number of replicates varies
across samples â in this case standard error in percent is suggested to be
superior.[13] If measurements do not have a natural zero point then the CV is
not a valid measurement and alternative measures such as the intraclass
correlation coefficient are recommended.[17]
**** As a measure of economic inequality[edit] ****
The coefficient of variation fulfills the requirements_for_a_measure_of
economic_inequality.[18][19][20] If x (with entries xi) is a list of the values
of an economic indicator (e.g. wealth), with xi being the wealth of agent i,
then the following requirements are met:
    * Anonymity â cv is independent of the ordering of the list x. This
      follows from the fact that the variance and mean are independent of the
      ordering of x.
    * Scale invariance: cv(x)=cv(αx) where α is a real number.[20]
    * Population independence â If {x,x} is the list x appended to itself,
      then cv({x,x})=cv(x). This follows from the fact that the variance and
      mean both obey this principle.
    * Pigou-Dalton transfer principle: when wealth is transferred from a
      wealthier agent i to a poorer agent j (i.e. xi > xj) without altering
      their rank, then cv decreases and vice versa.[20]
cv assumes its minimum value of zero for complete equality (all xi are equal).
[20] Its most notable drawback is that it is not bounded from above, so it
cannot be normalized to be within a fixed range (e.g. like the Gini_coefficient
which is constrained to be between 0 and 1).[20] It is, however, more
mathematically tractable than the Gini Coefficient.
***** Distribution[edit] *****
Provided that negative and small positive values of the sample mean occur with
negligible frequency, the probability_distribution of the coefficient of
variation for a sample of size n has been shown by Hendricks and Robey[21] to
be
          d   F   c   v      =   2   &#x03C0;  1  /  2   &#x0393;  (    n
      &#x2212; 1  2   )        e   &#x2212;   n  2   (   &#x03C3; &#x03BC;   )
      2           c   v      2    1 +    c   v      2             c   v      n
      &#x2212; 2    ( 1 +    c   v      2    )  n  /  2             &#x2211;
      &#x2211;   &#x2032;     i = 0   n &#x2212; 1   &#x2061;    ( n &#x2212; 1
      ) !  &#x0393;  (    n &#x2212; i  2   )    ( n &#x2212; 1 &#x2212; i ) !
      i !        n  i  /  2     2  i  /  2     (   &#x03C3; &#x03BC;   )   i
      1  ( 1 +    c   v      2    )  i  /  2        d   c   v    ,
      {\displaystyle \mathrm {d} F_{c_{\rm {v}}}={\frac {2}{\pi ^{1/2}\Gamma
      \left({\frac {n-1}{2}}\right)}}\;\mathrm {e} ^{-{\frac {n}{2\left({\frac
      {\sigma }{\mu }}\right)^{2}}}{\frac {{c_{\rm {v}}}^{2}}{1+{c_{\rm {v}}}^
      {2}}}}{\frac {{c_{\rm {v}}}^{n-2}}{(1+{c_{\rm {v}}}^{2})^{n/2}}}\sideset
      {}{^{\prime }}\sum _{i=0}^{n-1}{\frac {(n-1)!\,\Gamma \left({\frac {n-i}
      {2}}\right)}{(n-1-i)!\,i!\,}}{\frac {n^{i/2}}{2^{i/2}\left({\frac {\sigma
      }{\mu }}\right)^{i}}}{\frac {1}{(1+{c_{\rm {v}}}^{2})^{i/2}}}\,\mathrm
      {d} c_{\rm {v}},}  [{\displaystyle \mathrm {d} F_{c_{\rm {v}}}={\frac {2}
      {\pi ^{1/2}\Gamma \left({\frac {n-1}{2}}\right)}}\;\mathrm {e} ^{-{\frac
      {n}{2\left({\frac {\sigma }{\mu }}\right)^{2}}}{\frac {{c_{\rm {v}}}^{2}}
      {1+{c_{\rm {v}}}^{2}}}}{\frac {{c_{\rm {v}}}^{n-2}}{(1+{c_{\rm {v}}}^
      {2})^{n/2}}}\sideset {}{^{\prime }}\sum _{i=0}^{n-1}{\frac {(n-
      1)!\,\Gamma \left({\frac {n-i}{2}}\right)}{(n-1-i)!\,i!\,}}{\frac {n^{i/
      2}}{2^{i/2}\left({\frac {\sigma }{\mu }}\right)^{i}}}{\frac {1}{(1+{c_
      {\rm {v}}}^{2})^{i/2}}}\,\mathrm {d} c_{\rm {v}},}]
where the symbol           &#x2211;         &#x2211;   &#x2032;
{\displaystyle \sideset {}{^{\prime }}\sum }  [\sideset{}{^\prime}\sum]
indicates that the summation is over only even values of n-1-i, i.e., if n is
odd, sum over even values of i and if n is even, sum only over odd values of i.
This is useful, for instance, in the construction of hypothesis_tests or
confidence_intervals. Statistical inference for the coefficient of variation in
normally distributed data is often based on McKay's_chi-square_approximation
for the coefficient of variation [22][23][24][25][26][27]
**** Alternative[edit] ****
According to Liu (2012),[28] Lehmann (1986).[29] "also derived the sample
distribution of CV in order to give an exact method for the construction of a
confidence interval for CV;" it is based on a non-central_t-distribution.
***** Similar ratios[edit] *****
Standardized_moments are similar ratios,       &#x03BC;  k     /    &#x03C3;  k
{\displaystyle {\mu _{k}}/{\sigma ^{k}}}  [{\mu_k}/{\sigma^k}] where
&#x03BC;  k     {\displaystyle \mu _{k}}  [\mu _{k}] is the kth moment about
the mean, which are also dimensionless and scale invariant. The variance-to-
mean_ratio,      &#x03C3;  2    /  &#x03BC;   {\displaystyle \sigma ^{2}/\mu }
[\sigma^2/\mu], is another similar ratio, but is not dimensionless, and hence
not scale invariant. See Normalization_(statistics) for further ratios.
In signal_processing, particularly image_processing, the reciprocal ratio
&#x03BC;  /  &#x03C3;   {\displaystyle \mu /\sigma }  [\mu/\sigma] is referred
to as the signal_to_noise_ratio in general and signal-to-noise_ratio_(imaging)
in particular.
    * Efficiency,      &#x03C3;  2    /   &#x03BC;  2     {\displaystyle \sigma
      ^{2}/\mu ^{2}}  [\sigma^2 / \mu^2]
    * Standardized_moment,      &#x03BC;  k    /   &#x03C3;  k
      {\displaystyle \mu _{k}/\sigma ^{k}}  [\mu_k/\sigma^k]
    * Variance-to-mean_ratio (or relative variance),      &#x03C3;  2    /
      &#x03BC;   {\displaystyle \sigma ^{2}/\mu }  [\sigma^2/\mu]
    * Fano_factor,      &#x03C3;  W   2    /   &#x03BC;  W     {\displaystyle
      \sigma _{W}^{2}/\mu _{W}}  [\sigma^2_W/\mu_W] (windowed VMR)
    * Relative_Standard_Error
***** See also[edit] *****
    * Omega_ratio
    * Sampling_(statistics)
***** References[edit] *****
   1. ^Everitt, Brian (1998). The Cambridge Dictionary of Statistics.
      Cambridge, UK New York: Cambridge University Press. ISBN 978-0521593465.
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
   3. ^"What_is_the_difference_between_ordinal,_interval_and_ratio_variables?
      Why_should_I_care?". GraphPad Software Inc. Archived from the original on
      15 December 2008. Retrieved 22 February 2008.
   4. ^Odic, Darko; Im, Hee Yeon; Eisinger, Robert; Ly, Ryan; Halberda, Justin
      (June 2016). "PsiMLE: A maximum-likelihood estimation approach to
      estimating psychophysical scaling and variability more reliably,
      efficiently, and flexibly". Behavior Research Methods. 48 (2): 445â462.
      doi:10.3758/s13428-015-0600-5. ISSN 1554-3528. PMID 25987306.
   5. ^ Sokal RR & Rohlf FJ. Biometry (3rd Ed). New York: Freeman, 1995. p. 58.
   6. ISBN 0-7167-2411-1
   7. ^Limpert, Eckhard; Stahel, Werner A.; Abbt, Markus (2001). "Log-normal
      Distributions across the Sciences: Keys and Clues". BioScience. 51 (5):
      341â352. doi:10.1641/0006-3568(2001)051[0341:LNDATS]2.0.CO;2.
   8. ^Koopmans, L. H.; Owen, D. B.; Rosenblatt, J. I. (1964). "Confidence
      intervals for the coefficient of variation for the normal and log normal
      distributions". Biometrika. 51: 25â32. doi:10.1093/biomet/51.1-2.25.
   9. ^Diletti, E; Hauschke, D; Steinijans, VW (1992). "Sample size
      determination for bioequivalence assessment by means of confidence
      intervals". International Journal of Clinical Pharmacology, Therapy, and
      Toxicology. 30 Suppl 1: S51â8. PMID 1601532.
  10. ^Julious, Steven A.; Debarnot, Camille A. M. (2000). "Why Are
      Pharmacokinetic Data Summarized by Arithmetic Means?". Journal of
      Biopharmaceutical Statistics. 10 (1): 55â71. doi:10.1081/BIP-100101013.
      PMID 10709801.
  11. ^Reed, JF; Lynn, F; Meade, BD (2002). "Use_of_Coefficient_of_Variation_in
      Assessing_Variability_of_Quantitative_Assays". Clin Diagn Lab Immunol. 9
      (6): 1235â1239. doi:10.1128/CDLI.9.6.1235-1239.2002. PMC 130103.
      PMID 12414755.
  12. ^ Sawant,S.; Mohan, N. (2011) "FAQ:_Issues_with_Efficacy_Analysis_of
      Clinical_Trial_Data_Using_SAS" Archived 24 August 2011 at the Wayback
      Machine, PharmaSUG2011, Paper PO08
  13. ^Schiff, MH; et al. (2014). "Head-to-head,_randomised,_crossover_study_of
      oral_versus_subcutaneous_methotrexate_in_patients_with_rheumatoid
      arthritis:_drug-exposure_limitations_of_oral_methotrexate_at_doses_>=15
      mg_may_be_overcome_with_subcutaneous_administration". Ann Rheum Dis. 73
      (8): 1â3. doi:10.1136/annrheumdis-2014-205228. PMC 4112421.
      PMID 24728329.
  14. ^Kirkwood, TBL (1979). "Geometric means and measures of dispersion".
      Biometrics. 35 (4): 908â9. JSTOR 2530139.
  15. ^ a bEisenberg, Dan (2015). "Improving_qPCR_telomere_length_assays:
      Controlling_for_well_position_effects_increases_statistical_power".
      American Journal of Human Biology. 27 (4): 570â5. doi:10.1002/
      ajhb.22690. PMC 4478151. PMID 25757675.
  16. ^Broverman, Samuel A. (2001). Actex_study_manual,_Course_1,_Examination
      of_the_Society_of_Actuaries,_Exam_1_of_the_Casualty_Actuarial_Society
      (2001 ed.). Winsted, CT: Actex Publications. p. 104. ISBN 9781566983969.
      Retrieved 7 June 2014.
  17. ^"Measuring_Degree_of_Mixing_-_Homogeneity_of_powder_mix_-_Mixture
      quality_-_PowderProcess.net". www.powderprocess.net. Archived from the
      original on 14 November 2017. Retrieved 2 May 2018.
  18. ^Rodbard, D (October 1974). "Statistical quality control and routine data
      processing for radioimmunoassays and immunoradiometric assays". Clinical
      Chemistry. 20 (10): 1255â70. PMID 4370388.
  19. ^Eisenberg, Dan T. A. (30 August 2016). "Telomere_length_measurement
      validity:_the_coefficient_of_variation_is_invalid_and_cannot_be_used_to
      compare_quantitative_polymerase_chain_reaction_and_Southern_blot_telomere
      length_measurement_technique". International Journal of Epidemiology. 45
      (4): 1295â1298. doi:10.1093/ije/dyw191. ISSN 0300-5771. PMID 27581804.
  20. ^Champernowne, D. G.; Cowell, F. A. (1999). Economic Inequality and
      Income Distribution. Cambridge University Press.
  21. ^Campano, F.; Salvatore, D. (2006). Income distribution. Oxford
      University Press.
  22. ^ a b c d eBellu, Lorenzo Giovanni; Liberati, Paolo (2006). "Policy
      Impacts_on_Inequality_â_Simple_Inequality_Measures" (PDF). EASYPol,
      Analytical tools. Policy Support Service, Policy Assistance Division,
      FAO. Archived (PDF) from the original on 5 August 2016. Retrieved 13 June
      2016.
  23. ^Hendricks, Walter A.; Robey, Kate W. (1936). "The Sampling Distribution
      of the Coefficient of Variation". The Annals of Mathematical Statistics.
      7 (3): 129â32. doi:10.1214/aoms/1177732503. JSTOR 2957564.
  24. ^Iglevicz, Boris; Myers, Raymond (1970). "Comparisons of approximations
      to the percentage points of the sample coefficient of variation".
      Technometrics. 12 (1): 166â169. doi:10.2307/1267363. JSTOR 1267363.
  25. ^Bennett, B. M. (1976). "On an approximate test for homogeneity of
      coefficients of variation". Contributions to Applied Statistics Dedicated
      to A. Linder. Experentia Suppl. 22: 169â171.
  26. ^Vangel, Mark G. (1996). "Confidence intervals for a normal coefficient
      of variation". The American Statistician. 50 (1): 21â26. doi:10.1080/
      00031305.1996.10473537. JSTOR 2685039.
  27. .
  28. ^Feltz, Carol J; Miller, G. Edward (1996). "An asymptotic test for the
      equality of coefficients of variation from k populations". Statistics in
      Medicine. 15 (6): 647. doi:10.1002/(SICI)1097-0258(19960330)15:6<647::
      AID-SIM184>3.0.CO;2-P.
  29. ^Forkman, Johannes (2009). "Estimator_and_tests_for_common_coefficients
      of_variation_in_normal_distributions" (PDF). Communications in Statistics
      â Theory and Methods. 38 (2): 21â26. doi:10.1080/03610920802187448.
      Archived (PDF) from the original on 6 December 2013. Retrieved 23
      September 2013.
  30. ^Krishnamoorthy, K; Lee, Meesook (2013). "Improved tests for the equality
      of normal coefficients of variation". Computational Statistics. 29:
      215â232. doi:10.1007/s00180-013-0445-2.
  31. ^Liu, Shuang (2012). Confidence_Interval_Estimation_for_Coefficient_of
      Variation (Thesis). Georgia State University. p.3. Archived from the
      original on 1 March 2014. Retrieved 25 February 2014.
  32. ^ Lehmann, E. L. (1986). Testing Statistical Hypothesis. 2nd ed. New
      York: Wiley.
***** External links[edit] *****
    * cvequality: R package to test for significant differences between
      multiple coefficients of variation
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
Continuous_data Dispersion     * Coefficient of variation
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

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Coefficient_of_variation&oldid=900098611"
Categories:
    * Statistical_deviation_and_dispersion
    * Statistical_ratios
Hidden categories:
    * CS1:_long_volume_value
    * Webarchive_template_wayback_links
    * Use_American_English_from_January_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * Use_dmy_dates_from_October_2017
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2016
    * Articles_with_unsourced_statements_from_February_2018
    * Articles_with_unsourced_statements_from_June_2019
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
    * AragonÃ©s
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Italiano
    * LietuviÅ³
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * SlovenÅ¡Äina
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 3 June 2019, at 12:25 (UTC).
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
