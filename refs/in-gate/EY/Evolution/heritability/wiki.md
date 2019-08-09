The following text has been accessed from https://en.wikipedia.org/wiki/Heritability at Fri Aug 9 04:02:42 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Heritability ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Estimation of effect of genetic variation on phenotypic variation of a trait
Studies of heritability ask questions such as how much genetic factors play a
role in differences in height between people. This is not the same as asking
how much genetic factors influence height in any one person.
Heritability is a statistic used in the fields of breeding and genetics that
estimates the degree of variation in a phenotypic_trait in a population that is
due to genetic variation between individuals in that population.[1] In other
words, the concept of heritability can alternately be expressed in the form of
the following question: "What is the proportion of the variation in a given
trait within a population that is not explained by the environment or random
chance?"[2]
Other causes of measured variation in a trait are characterized as
environmental_factors, including measurement error. In human studies of
heritability these are often apportioned into factors from "shared environment"
and "non-shared environment" based on whether they tend to result in persons
brought up in the same household being more or less similar to persons who were
not.
Heritability is estimated by comparing individual phenotypic variation among
related individuals in a population. Heritability is an important concept in
quantitative_genetics, particularly in selective_breeding and behavior_genetics
(for instance, twin_studies). It is the source of much confusion due to the
fact that its technical definition is different from its commonly-understood
folk definition. Therefore, its use conveys the incorrect impression that
behavioral traits are "inherited" or specifically passed down through the
genes.[3] Behavioral geneticists also conduct heritability analyses based on
the false assumption that genes and environments contribute in a separate,
additive manner to behavioral traits.[4]
⁰
***** Contents *****
    * 1_Overview
    * 2_Definition
          o 2.1_Example
          o 2.2_Assumptions
    * 3_Estimating_heritability
          o 3.1_Regression/correlation_methods_of_estimation
                # 3.1.1_Comparison_of_close_relatives
                      # 3.1.1.1_Parent-offspring_regression
                      # 3.1.1.2_Sibling_comparison
                      # 3.1.1.3_Twin_studies
          o 3.2_Analysis_of_variance_methods_of_estimation
                # 3.2.1_Basic_model
                      # 3.2.1.1_Intraclass_correlations
                      # 3.2.1.2_The_ANOVA
                # 3.2.2_Model_with_additive_and_dominance_terms
          o 3.3_Linear_mixed_models
          o 3.4_Genomic_heritability
    * 4_Response_to_selection
    * 5_Controversies
    * 6_See_also
    * 7_References
    * 8_Further_reading
    * 9_External_links
***** Overview[edit] *****
Heritability measures the fraction of phenotype variability that can be
attributed to genetic_variation. This is not the same as saying that this
fraction of an individual phenotype is caused by genetics. For example, it is
incorrect to say that since the heritability of personality traits is about .6,
that means that 60% of your personality is inherited from your parents and 40%
comes from the environment. In addition, heritability can change without any
genetic change occurring, such as when the environment starts contributing to
more variation. As a case in point, consider that both genes and environment
have the potential to influence intelligence. Heritability could increase if
genetic variation increases, causing individuals to show more phenotypic
variation, like showing different levels of intelligence. On the other hand,
heritability might also increase if the environmental variation decreases,
causing individuals to show less phenotypic variation, like showing more
similar levels of intelligence. Heritability increases when genetics are
contributing more variation or because non-genetic factors are contributing
less variation; what matters is the relative contribution. Heritability is
specific to a particular population in a particular environment. High
heritability of a trait, consequently, does not necessarily mean that the trait
is not very susceptible to environmental influences.[5] Heritability can also
change as a result of changes in the environment, migration, inbreeding, or the
way in which heritability itself is measured in the population under study.[6]
The heritability of a trait should not be interpreted as a measure of the
extent to which said trait is genetically determined in an individual.[7][8]
The extent of dependence of phenotype on environment can also be a function of
the genes involved. Matters of heritability are complicated because genes may
canalize a phenotype, making its expression almost inevitable in all occurring
environments. Individuals with the same genotype can also exhibit different
phenotypes through a mechanism called phenotypic_plasticity, which makes
heritability difficult to measure in some cases. Recent insights in molecular
biology have identified changes in transcriptional activity of individual genes
associated with environmental changes. However, there are a large number of
genes whose transcription is not affected by the environment.[9]
Estimates of heritability use statistical_analyses to help to identify the
causes of differences between individuals. Since heritability is concerned with
variance, it is necessarily an account of the differences between individuals
in a population. Heritability can be univariate â examining a single trait
â or multivariate â examining the genetic and environmental associations
between multiple traits at once. This allows a test of the genetic overlap
between different phenotypes: for instance hair_color and eye_color.
Environment and genetics may also interact, and heritability analyses can test
for and examine these interactions (GxE models).
A prerequisite for heritability analyses is that there is some population
variation to account for. This last point highlights the fact that heritability
cannot take into account the effect of factors which are invariant in the
population. Factors may be invariant if they are absent and do not exist in the
population, such as no one having access to a particular antibiotic, or because
they are omni-present, like if everyone is drinking coffee. In practice, all
human behavioral traits vary and almost all traits show some heritability.[10]
***** Definition[edit] *****
Heritability
Any particular phenotype can be modeled as the sum of genetic and environmental
effects:[11]
      Phenotype (P) = Genotype (G) + Environment (E).
Likewise the phenotypic variance in the trait â Var (P) â is the sum of
effects as follows:
      Var(P) = Var(G) + Var(E) + 2 Cov(G,E).
In a planned experiment Cov(G,E) can be controlled and held at 0. In this case,
heritability is defined as:
          H  2   =     V a r  ( G )    V a r  ( P )      {\displaystyle H^{2}=
      {\frac {\mathrm {Var} (G)}{\mathrm {Var} (P)}}}  [H^{2}={\frac  {{\mathrm
      {Var}}(G)}{{\mathrm  {Var}}(P)}}] .
H2 is the broad-sense heritability. This reflects all the genetic contributions
to a population's phenotypic variance including additive, dominant, and
epistatic (multi-genic interactions), as well as maternal_and_paternal_effects,
where individuals are directly affected by their parents' phenotype, such as
with milk production in mammals.
A particularly important component of the genetic variance is the additive
variance, Var(A), which is the variance due to the average effects (additive
effects) of the alleles. Since each parent passes a single allele per locus to
each offspring, parent-offspring resemblance depends upon the average effect of
single alleles. Additive variance represents, therefore, the genetic component
of variance responsible for parent-offspring resemblance. The additive genetic
portion of the phenotypic variance is known as Narrow-sense heritability and is
defined as
          h  2   =     V a r  ( A )    V a r  ( P )      {\displaystyle h^{2}=
      {\frac {\mathrm {Var} (A)}{\mathrm {Var} (P)}}}  [h^{2}={\frac  {{\mathrm
      {Var}}(A)}{{\mathrm  {Var}}(P)}}]
An upper case H2 is used to denote broad sense, and lower case h2 for narrow
sense.
For traits which are not continuous but dichotomous such as an additional toe
or certain diseases, the contribution of the various alleles can be considered
to be a sum, which past a threshold, manifests itself as the trait, giving the
liability_threshold_model in which heritability can be estimated and selection
modeled.
Additive variance is important for selection. If a selective pressure such as
improving livestock is exerted, the response of the trait is directly related
to narrow-sense heritability. The mean of the trait will increase in the next
generation as a function of how much the mean of the selected parents differs
from the mean of the population from which the selected parents were chosen.
The observed response to selection leads to an estimate of the narrow-sense
heritability (called realized heritability). This is the principle underlying
artificial_selection or breeding.
**** Example[edit] ****
Figure 1. Relationship of phenotypic values to additive and dominance effects
using a completely dominant locus.
The simplest genetic model involves a single locus with two alleles (b and B)
affecting one quantitative phenotype.
The number of B alleles can vary from 0, 1, or 2. For any genotype, BiBj, the
expected phenotype can then be written as the sum of the overall mean, a linear
effect, and a dominance deviation:
          P  i j   = &#x03BC; +  &#x03B1;  i   +  &#x03B1;  j   +  d  i j
      {\displaystyle P_{ij}=\mu +\alpha _{i}+\alpha _{j}+d_{ij}}  [P_{{ij}}=\mu
      +\alpha _{i}+\alpha _{j}+d_{{ij}}] = Population_mean + Additive Effect
      (     a  i j   =  &#x03B1;  i   +  &#x03B1;  j     {\displaystyle a_
      {ij}=\alpha _{i}+\alpha _{j}}  [a_{{ij}}=\alpha _{i}+\alpha _{j}]) +
      Dominance Deviation (     d  i j     {\displaystyle d_{ij}}  [d_{ij}]).
The additive genetic variance at this locus is the weighted_average of the
squares of the additive effects:
          V a r  ( A ) = f ( b b )  a  b b   2   + f ( B b )  a  B b   2   + f
      ( B B )  a  B B   2   ,   {\displaystyle \mathrm {Var} (A)=f(bb)a_{bb}^
      {2}+f(Bb)a_{Bb}^{2}+f(BB)a_{BB}^{2},}  [{\mathrm  {Var}}(A)=f(bb)a_{
      {bb}}^{2}+f(Bb)a_{{Bb}}^{2}+f(BB)a_{{BB}}^{2},]
where     f ( b b )  a  b b   + f ( B b )  a  B b   + f ( B B )  a  B B   = 0.
{\displaystyle f(bb)a_{bb}+f(Bb)a_{Bb}+f(BB)a_{BB}=0.}  [f(bb)a_{{bb}}+f(Bb)a_{
{Bb}}+f(BB)a_{{BB}}=0.]
There is a similar relationship for variance of dominance deviations:
          V a r  ( D ) = f ( b b )  d  b b   2   + f ( B b )  d  B b   2   + f
      ( B B )  d  B B   2   ,   {\displaystyle \mathrm {Var} (D)=f(bb)d_{bb}^
      {2}+f(Bb)d_{Bb}^{2}+f(BB)d_{BB}^{2},}  [{\mathrm  {Var}}(D)=f(bb)d_{
      {bb}}^{2}+f(Bb)d_{{Bb}}^{2}+f(BB)d_{{BB}}^{2},]
where     f ( b b )  d  b b   + f ( B b )  d  B b   + f ( B B )  d  B B   = 0.
{\displaystyle f(bb)d_{bb}+f(Bb)d_{Bb}+f(BB)d_{BB}=0.}  [f(bb)d_{{bb}}+f(Bb)d_{
{Bb}}+f(BB)d_{{BB}}=0.]
The linear_regression of phenotype on genotype is shown in Figure 1.
**** Assumptions[edit] ****
Estimates of the total heritability of human traits assume the absence of
epistasis, which has been called the "assumption of additivity". Although some
researchers have cited such estimates in support of the existence of "missing
heritability" unaccounted for by known genetic loci, the assumption of
additivity may render these estimates invalid.[12] There is also empirical
evidence that the additivity assumption is frequently violated in behavior
genetic studies of adolescent intelligence and academic_achievement.[13]
***** Estimating heritability[edit] *****
Since only P can be observed or measured directly, heritability must be
estimated from the similarities observed in subjects varying in their level of
genetic or environmental similarity. The statistical analyses required to
estimate the genetic and environmental components of variance depend on the
sample characteristics. Briefly, better estimates are obtained using data from
individuals with widely varying levels of genetic relationship - such as twins,
siblings, parents and offspring, rather than from more distantly related (and
therefore less similar) subjects. The standard_error for heritability estimates
is improved with large sample sizes.
In non-human populations it is often possible to collect information in a
controlled way. For example, among farm animals it is easy to arrange for a
bull to produce offspring from a large number of cows and to control
environments. Such experimental_control is generally not possible when
gathering human data, relying on naturally occurring relationships and
environments.
In classical quantitative genetics, there were two schools of thought regarding
estimation of heritability.
One school_of_thought was developed by Sewall_Wright at The_University_of
Chicago, and further popularized by C._C._Li (University_of_Chicago) and J._L.
Lush (Iowa_State_University). It is based on the analysis of correlations and,
by extension, regression. Path_Analysis was developed by Sewall_Wright as a way
of estimating heritability.
The second was originally developed by R._A._Fisher and expanded at The
University_of_Edinburgh, Iowa_State_University, and North_Carolina_State
University, as well as other schools. It is based on the analysis_of_variance
of breeding studies, using the intraclass correlation of relatives. Various
methods of estimating components of variance (and, hence, heritability) from
ANOVA are used in these analyses.
Today, heritability can be estimated from general pedigrees using linear_mixed
models and from genomic_relatedness estimated from genetic markers.
Studies of human heritability often utilize adoption study designs, often with
identical_twins who have been separated early in life and raised in different
environments. Such individuals have identical genotypes and can be used to
separate the effects of genotype and environment. A limit of this design is the
common prenatal environment and the relatively low numbers of twins reared
apart. A second and more common design is the twin_study in which the
similarity of identical and fraternal twins is used to estimate heritability.
These studies can be limited by the fact that identical twins are not
completely_genetically_identical, potentially resulting in an underestimation
of heritability.
In observational_studies, or because of evocative effects (where a genome
evokes environments by its effect on them), G and E may covary: gene
environment_correlation. Depending on the methods used to estimate
heritability, correlations between genetic factors and shared or non-shared
environments may or may not be confounded with heritability.[14]
**** Regression/correlation methods of estimation[edit] ****
The first school of estimation uses regression and correlation to estimate
heritability.
*** Comparison of close relatives[edit] ***
In the comparison of relatives, we find that in general,
          h  2   =   b r   =   t r     {\displaystyle h^{2}={\frac {b}{r}}=
      {\frac {t}{r}}}  [{\displaystyle h^{2}={\frac {b}{r}}={\frac {t}{r}}}]
where r can be thought of as the coefficient_of_relatedness, b is the
coefficient of regression and t is the coefficient of correlation.
** Parent-offspring regression[edit] **
Figure 2. Sir Francis_Galton's (1889) data showing the relationship between
offspring height (928 individuals) as a function of mean parent height (205
sets of parents).
Heritability may be estimated by comparing parent and offspring traits (as in
Fig. 2). The slope of the line (0.57) approximates the heritability of the
trait when offspring values are regressed against the average trait in the
parents. If only one parent's value is used then heritability is twice the
slope. (Note that this is the source of the term "regression," since the
offspring values always tend to regress_to_the_mean value for the population,
i.e., the slope is always less than one). This regression effect also underlies
the DeFries Fulker method for analyzing twins selected for one member being
affected.[15]
** Sibling comparison[edit] **
A basic approach to heritability can be taken using full-Sib designs: comparing
similarity between siblings who share both a biological mother and a father.
[16] When there is only additive gene action, this sibling phenotypic
correlation is an index of familiarity â the sum of half the additive genetic
variance plus full effect of the common environment. It thus places an upper-
limit on additive heritability of twice the full-Sib phenotypic correlation.
Half-Sib designs compare phenotypic traits of siblings that share one parent
with other sibling groups.
** Twin studies[edit] **
Main article: Twin_study
Figure 3. Twin concordances for seven psychological traits (sample size shown
inside bars), with DZ being fraternal and MZ being identical twins.
Heritability for traits in humans is most frequently estimated by comparing
resemblances between twins. "The advantage of twin studies, is that the total
variance can be split up into genetic, shared or common environmental, and
unique environmental components, enabling an accurate estimation of
heritability".[17] Fraternal or dizygotic (DZ) twins on average share half
their genes (assuming there is no assortative_mating for the trait), and so
identical or monozygotic (MZ) twins on average are twice as genetically similar
as DZ twins. A crude estimate of heritability, then, is approximately twice the
difference in correlation between MZ and DZ twins, i.e. Falconer's_formula H2=2
(r(MZ)-r(DZ)).
The effect of shared environment, c2, contributes to similarity between
siblings due to the commonality of the environment they are raised in. Shared
environment is approximated by the DZ correlation minus half heritability,
which is the degree to which DZ twins share the same genes, c2=DZ-1/2h2. Unique
environmental variance, e2, reflects the degree to which identical twins raised
together are dissimilar, e2=1-r(MZ).
**** Analysis of variance methods of estimation[edit] ****
The second set of methods of estimation of heritability involves ANOVA and
estimation of variance components.
*** Basic model[edit] ***
We use the basic discussion of Kempthorne.[11] Considering only the most basic
of genetic models, we can look at the quantitative contribution of a single
locus with genotype Gi as
          y  i   = &#x03BC; +  g  i   + e   {\displaystyle y_{i}=\mu +g_{i}+e}
      [y_{i}=\mu +g_{i}+e]
where      g  i     {\displaystyle g_{i}}  [g_{i}] is the effect of genotype Gi
and     e   {\displaystyle e}  [e] is the environmental effect.
Consider an experiment with a group of sires and their progeny from random
dams. Since the progeny get half of their genes from the father and half from
their (random) mother, the progeny equation is
          z  i   = &#x03BC; +   1 2    g  i   + e   {\displaystyle z_{i}=\mu +
      {\frac {1}{2}}g_{i}+e}  [z_{i}=\mu +{\frac  {1}{2}}g_{i}+e]
** Intraclass correlations[edit] **
Consider the experiment above. We have two groups of progeny we can compare.
The first is comparing the various progeny for an individual sire (called
within sire group). The variance will include terms for genetic variance (since
they did not all get the same genotype) and environmental variance. This is
thought of as an error term.
The second group of progeny are comparisons of means of half sibs with each
other (called among sire group). In addition to the error_term as in the within
sire groups, we have an addition term due to the differences among different
means of half sibs. The intraclass correlation is
          c o r r  ( z ,  z &#x2032;  ) =  c o r r  ( &#x03BC; +   1 2   g + e
      , &#x03BC; +   1 2   g +  e &#x2032;  ) =   1 4    V  g
      {\displaystyle \mathrm {corr} (z,z')=\mathrm {corr} (\mu +{\frac {1}
      {2}}g+e,\mu +{\frac {1}{2}}g+e')={\frac {1}{4}}V_{g}}  [{\mathrm  {corr}}
      (z,z')={\mathrm  {corr}}(\mu +{\frac  {1}{2}}g+e,\mu +{\frac  {1}
      {2}}g+e')={\frac  {1}{4}}V_{g}] ,
since environmental effects are independent of each other.
** The ANOVA[edit] **
In an experiment with     n   {\displaystyle n}  [n] sires and     r
{\displaystyle r}  [r] progeny per sire, we can calculate the following ANOVA,
using      V  g     {\displaystyle V_{g}}  [V_{g}] as the genetic variance and
V  e     {\displaystyle V_{e}}  [V_{e}] as the environmental variance:
                      Table 1: ANOVA for Sire experiment
Source             d.f.                Mean Square         Expected Mean Square
                                                                3 4    V  g   +
                                                           V  e   + r (    1 4
                                                           V  g    )
                      n &#x2212; 1        S                {\displaystyle
Among sire groups  {\displaystyle n-1} {\displaystyle S}   {\frac {3}{4}}V_
                   [n-1]               [S]                 {g}+V_{e}+r({{\frac
                                                           {1}{4}}V_{g}})}  [
                                                           {\frac  {3}{4}}V_
                                                           {g}+V_{e}+r({{\frac
                                                           {1}{4}}V_{g}})]
                                                                3 4    V  g   +
                      n ( r &#x2212; 1    W                V  e
Within sire groups )   {\displaystyle  {\displaystyle W}   {\displaystyle
                   n(r-1)}  [n(r-1)]   [W]                 {\frac {3}{4}}V_
                                                           {g}+V_{e}}  [{\frac
                                                           {3}{4}}V_{g}+V_{e}]
The       1 4    V  g     {\displaystyle {\frac {1}{4}}V_{g}}  [{\frac  {1}
{4}}V_{g}] term is the intraclass_correlation among half sibs. We can easily
calculate      H  2   =    V  g     V  g   +  V  e      =    4 ( S &#x2212; W )
S + ( r &#x2212; 1 ) W      {\displaystyle H^{2}={\frac {V_{g}}{V_{g}+V_{e}}}=
{\frac {4(S-W)}{S+(r-1)W}}}  [H^{2}={\frac  {V_{g}}{V_{g}+V_{e}}}={\frac  {4(S-
W)}{S+(r-1)W}}]. The Expected Mean Square is calculated from the relationship
of the individuals (progeny within a sire are all half-sibs, for example), and
an understanding of intraclass correlations.
The use of ANOVA to calculate heritability often fails to account for the
presence of gene-environment_interactions, because ANOVA has a much lower
statistical_power for testing for interaction effects than for direct effects.
[18]
*** Model with additive and dominance terms[edit] ***
For a model with additive and dominance terms, but not others, the equation for
a single locus is
          y  i j   = &#x03BC; +  &#x03B1;  i   +  &#x03B1;  j   +  d  i j   + e
      ,   {\displaystyle y_{ij}=\mu +\alpha _{i}+\alpha _{j}+d_{ij}+e,}  [y_{
      {ij}}=\mu +\alpha _{i}+\alpha _{j}+d_{{ij}}+e,]
where
    &#x03B1;  i     {\displaystyle \alpha _{i}}  [\alpha _{i}] is the additive
effect of the ith allele,      &#x03B1;  j     {\displaystyle \alpha _{j}}
[\alpha _{j}] is the additive effect of the jth allele,      d  i j
{\displaystyle d_{ij}}  [d_{ij}] is the dominance deviation for the ijth
genotype, and     e   {\displaystyle e}  [e] is the environment.
Experiments can be run with a similar setup to the one given in Table 1. Using
different relationship groups, we can evaluate different intraclass
correlations. Using      V  a     {\displaystyle V_{a}}  [V_{a}] as the
additive genetic variance and      V  d     {\displaystyle V_{d}}  [V_{d}] as
the dominance deviation variance, intraclass correlations become linear
functions of these parameters. In general,
      Intraclass correlation    = r  V  a   + &#x03B8;  V  d   ,
      {\displaystyle =rV_{a}+\theta V_{d},}  [=rV_{a}+\theta V_{d},]
where     r   {\displaystyle r}  [r] and     &#x03B8;   {\displaystyle \theta }
[\theta ] are found as
   r =   {\displaystyle r=}  [r=]P[ alleles drawn at random from the
relationship pair are identical_by_descent], and
   &#x03B8; =   {\displaystyle \theta =}  [\theta =]P[ genotypes drawn at
random from the relationship pair are identical_by_descent].
Some common relationships and their coefficients are given in Table 2.
           Table 2: Coefficients for calculating variance components
Relationship            r   {\displaystyle r}        &#x03B8;   {\displaystyle
                     [r]                          \theta }  [\theta ]
Identical Twins         1   {\displaystyle 1}        1   {\displaystyle 1}  [1]
                     [1]
                          1 2     {\displaystyle     0   {\displaystyle 0}  [
Parent-Offspring     {\frac {1}{2}}}  [{\frac {1} {\displaystyle 0}]
                     {2}}]
                          1 4     {\displaystyle     0   {\displaystyle 0}  [
Half Siblings        {\frac {1}{4}}}  [\frac{1}   {\displaystyle 0}]
                     {4}]
                          1 2     {\displaystyle       1 4     {\displaystyle
Full Siblings        {\frac {1}{2}}}  [{\frac {1} {\frac {1}{4}}}  [\frac{1}
                     {2}}]                        {4}]
                          1 8     {\displaystyle     0   {\displaystyle 0}  [
First Cousins        {\frac {1}{8}}}  [{\frac     {\displaystyle 0}]
                     {1}{8}}]
                          1 4     {\displaystyle       1 16     {\displaystyle
Double First Cousins {\frac {1}{4}}}  [\frac{1}   {\frac {1}{16}}}  [{\frac
                     {4}]                         {1}{16}}]
**** Linear mixed models[edit] ****
A wide variety approaches using linear mixed models have been reported in
literature. Via these methods, phenotypic variance is partitioned into genetic,
environmental and experimental design variances to estimate heritability.
Environmental variance can be explicitly modeled by studying individuals across
a broad range of environments, although inference of genetic variance from
phenotypic and environmental variance may lead to underestimation of
heritability due to the challenge of capturing the full range of environmental
influence affecting a trait. Other methods for calculating heritability use
data from genome-wide_association_studies to estimate the influence on a trait
by genetic factors, which is reflected by the rate and influence of putatively
associated genetic loci (usually single-nucleotide_polymorphisms) on the trait.
This can lead to underestimation of heritability, however. This discrepancy is
referred to as "missing heritability" and reflects the challenge of accurately
modeling both genetic and environmental variance in heritability models.[19]
When a large, complex pedigree or another aforementioned type of data is
available, heritability and other quantitative genetic parameters can be
estimated by restricted_maximum_likelihood (REML) or Bayesian_methods. The raw
data will usually have three or more data points for each individual: a code
for the sire, a code for the dam and one or several trait values. Different
trait values may be for different traits or for different time points of
measurement.
The currently popular methodology relies on high degrees of certainty over the
identities of the sire and dam; it is not common to treat the sire identity
probabilistically. This is not usually a problem, since the methodology is
rarely applied to wild populations (although it has been used for several wild
ungulate and bird populations), and sires are invariably known with a very high
degree of certainty in breeding programmes. There are also algorithms that
account for uncertain paternity.
The pedigrees can be viewed using programs such as Pedigree Viewer [1], and
analyzed with programs such as ASReml, VCE [2], WOMBAT [3] or the BLUPF90
family of programs [4].
Pedigree models are helpful for untangling confounds such as reverse_causality,
maternal_effects such as the prenatal_environment, and confounding of genetic
dominance, shared environment, and maternal gene effects.[20][21]
**** Genomic heritability[edit] ****
When genome-wide genotype data and phenotypes from large population samples are
available, one can estimate the relationships between individuals based on
their genotypes and use a linear mixed model to estimate the variance explained
by the genetic markers. This gives a genomic heritability estimate based on the
variance captured by common genetic variants.[22] There are multiple methods
that make different adjustments for allele frequency and linkage
disequilibrium.
***** Response to selection[edit] *****
Figure 4. Strength of selection (S) and response to selection (R) in an
artificial selection experiment, h2=R/S.
In selective_breeding of plants and animals, the expected response to selection
of a trait with known narrow-sense heritability     (  h  2   )
{\displaystyle (h^{2})}  [{\displaystyle (h^{2})}] can be estimated using the
breeder's equation:[23]
         R =  h  2   S   {\displaystyle R=h^{2}S}  [R=h^{2}S]
In this equation, the Response to Selection (R) is defined as the realized
average difference between the parent generation and the next generation, and
the Selection Differential (S) is defined as the average difference between the
parent generation and the selected parents.[11]:1957[24]
For example, imagine that a plant breeder is involved in a selective breeding
project with the aim of increasing the number of kernels per ear of corn. For
the sake of argument, let us assume that the average ear of corn in the parent
generation has 100 kernels. Let us also assume that the selected parents
produce corn with an average of 120 kernels per ear. If h2 equals 0.5, then the
next generation will produce corn with an average of 0.5(120-100) = 10
additional kernels per ear. Therefore, the total number of kernels per ear of
corn will equal, on average, 110.
Observing the response to selection in an artificial selection experiment will
allow calculation of realized heritability as in Fig. 5.
Note that heritability in the above equation is equal to the ratio      V a r
( A )  /   V a r  ( P )   {\displaystyle \mathrm {Var} (A)/\mathrm {Var} (P)}
[{\mathrm  {Var}}(A)/{\mathrm  {Var}}(P)] only if the genotype and the
environmental noise follow Gaussian_distributions.
***** Controversies[edit] *****
                   This section's representation of one or more viewpoints
[Ambox scales.svg] about a controversial issue may be unbalanced or inaccurate.
                   Please improve_the_article or discuss the issue on the talk
                   page. (August 2016)
Heritability estimates' prominent critics, such as Steven_Rose,[25] Jay_Joseph,
[26] and Richard_Bentall, focus largely on heritability estimates in behavioral
sciences and social_sciences. Bentall has claimed that such heritability scores
are typically calculated counterintuitively to derive numerically high scores,
that heritability is misinterpreted as genetic_determination, and that this
alleged bias distracts from other factors that researches have found more
causally important, such as childhood abuse causing later psychosis.[27][28]
Heritability estimates are also inherently limited because they do not convey
any information regarding whether genes or environment play a larger role in
the development of the trait under study. For this reason, David_Moore and
David_Shenk describe the term "heritability" in the context of behavior
genetics as "...one of the most misleading in the history of science" and argue
that it has no value except in very rare cases.[29] When studying complex human
traits, it is impossible to use heritability analysis to determine the relative
contributions of genes and environment, as such traits result from multiple
causes interacting.[30]
The controversy over heritability estimates is largely via their basis in twin
studies. The scarce success of molecular-genetic studies to corroborate such
population-genetic studies' conclusions is the missing_heritability_problem.
[31] Eric Turkheimer has argued that newer molecular methods have vindicated
the conventional interpretation of twin studies,[31] although it remains mostly
unclear how to explain the relations between genes and behaviors.[32] According
to Turkheimer, both genes and environment are heritable, genetic contribution
varies by environment, and a focus on heritability distracts from other
important factors.[33] Overall, however, heritability is a concept widely
applicable.[21]
***** See also[edit] *****
    * Behavioral_genetics
    * Heredity
    * Heritability_of_IQ
***** References[edit] *****
   1. ^Wray N, Visscher P (2008). "Estimating_Trait_Heritability". Nature
      Education. 1 (1): 29. Retrieved 24 July 2015.
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
   3. ^Gazzaniga MS, Heatherton TF, Halpern DF. Psychological science (5th
      ed.). New York. ISBN 978-0-393-26313-8. OCLC 908409996.
   4. ^Stoltenberg, Scott F. (June 1997). "Coming_to_terms_with_heritability".
      Genetica. 99 (2â3): 89â96. doi:10.1007/BF02259512. ISSN 0016-6707.
   5. ^Wahlsten, Douglas (1994). "The_intelligence_of_heritability". Canadian
      Psychology. 35 (3): 244â260. doi:10.1037/0708-5591.35.3.244. ISSN 1878-
      7304.
   6. ^Maccoby EE (February 2000). "Parenting and its effects on children: on
      reading and misreading behavior genetics". Annual Review of Psychology.
      51 (1): 1â27. doi:10.1146/annurev.psych.51.1.1. PMID 10751963.
   7. ^Visscher PM, Hill WG, Wray NR (2008-03-04). "Heritability_in_the
      genomics_era_â_concepts_and_misconceptions". Nature Reviews Genetics. 9
      (4): 255â266. doi:10.1038/nrg2322. ISSN 1471-0056. PMID 18319743.
   8. ^Sauce B, Matzel LD (January 2018). "The_paradox_of_intelligence:
      Heritability_and_malleability_coexist_in_hidden_gene-environment
      interplay". Psychological Bulletin. 144 (1): 26â47. doi:10.1037/
      bul0000131. PMC 5754247. PMID 29083200.
   9. ^Block N (August 1995). "How heritability misleads about race".
      Cognition. 56 (2): 99â128. doi:10.1016/0010-0277(95)00678-r.
      PMID 7554794.
  10. ^Wills C (2007). "Principles_of_Population_Genetics,_4th_edition" (PDF).
      Journal_of_Heredity (Book Review). 98 (4): 382. doi:10.1093/jhered/
      esm035.
          o review of:Hartl DL, Clark AG (2007). Principles of Population
            Genetics. Sunderland, MA: Sinauer and Associates. pp. xv + 652.
            ISBN 978-0-87893-308-2.
  11. ^Turkheimer E (October 2000). "Three_Laws_of_Behavior_Genetics_and_What
      They_Mean" (PDF). Current Directions in Psychological Science. 9 (5):
      160â164. doi:10.1111/1467-8721.00084. ISSN 0963-7214. Retrieved 29
      October 2013.
  12. ^ a b cKempthorne O (1957). An introduction to genetic statistics (1st
      ed.). Ames, Iowa: Iowa State Univ. Press. OCLC 422371269.
  13. ^Zuk O, Hechter E, Sunyaev SR, Lander ES (January 2012). "The_mystery_of
      missing_heritability:_Genetic_interactions_create_phantom_heritability".
      Proceedings of the National Academy of Sciences of the United States of
      America. 109 (4): 1193â8. doi:10.1073/pnas.1119675109. PMC 3268279.
      PMID 22223662.
  14. ^Daw J, Guo G, Harris KM (July 2015). "Nurture_net_of_nature:_Re-
      evaluating_the_role_of_shared_environments_in_academic_achievement_and
      verbal_intelligence". Social Science Research. 52: 422â39. doi:10.1016/
      j.ssresearch.2015.02.011. PMC 4888873. PMID 26004471.
  15. ^Cattell RB (November 1960). "The multiple abstract variance analysis
      equations and solutions: for nature-nurture research on continuous
      variables". Psychological Review. 67 (6): 353â72. doi:10.1037/h0043487.
      PMID 13691636.
  16. ^DeFries JC, Fulker DW (September 1985). "Multiple regression analysis of
      twin data". Behavior Genetics. 15 (5): 467â73. doi:10.1007/BF01066239.
      PMID 4074272.
  17. ^Falconer DS, Mackay TF (December 1995). Introduction to Quantitative
      Genetics (4th ed.). Longman. ISBN 978-0582243026.
  18. ^Gielen M, Lindsey PJ, Derom C, Smeets HJ, Souren NY, Paulussen AD, Derom
      R, Nijhuis JG (January 2008). "Modeling_genetic_and_environmental_factors
      to_increase_heritability_and_ease_the_identification_of_candidate_genes
      for_birth_weight:_a_twin_study". Behavior Genetics. 38 (1): 44â54. doi:
      10.1007/s10519-007-9170-3. PMC 2226023. PMID 18157630.
  19. ^Wahlsten, Douglas (March 1990). "Insensitivity_of_the_analysis_of
      variance_to_heredity-environment_interaction". Behavioral and Brain
      Sciences. 13 (1): 109â120. doi:10.1017/S0140525X00077797. ISSN 1469-
      1825.
  20. ^Heckerman D, Gurdasani D, Kadie C, Pomilla C, Carstensen T, Martin H,
      Ekoru K, Nsubuga RN, Ssenyomo G, Kamali A, Kaleebu P, Widmer C, Sandhu MS
      (July 2016). "Linear_mixed_model_for_heritability_estimation_that
      explicitly_addresses_environmental_variation". Proceedings of the
      National Academy of Sciences of the United States of America. 113 (27):
      7377â82. doi:10.1073/pnas.1510497113. PMC 4941438. PMID 27382152.
  21. ^Hill WG, Goddard_ME, Visscher PM (February 2008). MacKay TF (ed.). "Data
      and_theory_point_to_mainly_additive_genetic_variance_for_complex_traits".
      PLoS Genetics. 4 (2): e1000008. doi:10.1371/journal.pgen.1000008.
      PMC 2265475. PMID 18454194.
  22.  [open_access]
  23. ^ a bVisscher PM, Hill_WG, Wray NR (April 2008). "Heritability_in_the
      genomics_era--concepts_and_misconceptions" (PDF). Nature Reviews.
      Genetics. 9 (4): 255â66. doi:10.1038/nrg2322. PMID 18319743.
  24. ^Yang J, Zeng J, Goddard ME, Wray NR, Visscher PM (August 2017).
      "Concepts,_estimation_and_interpretation_of_SNP-based_heritability".
      Nature Genetics. 49 (9): 1304â1310. doi:10.1038/ng.3941. PMID 28854176.
  25. ^Plomin R, DeFries JC, McClearn GE, McGuffin P (2017). Behavioral
      Genetics: A Primer (2nd ed.). New York: W.H. Freeman. ISBN 978-0-7167-
      2056-0.
  26. ^Falconer DS, Mackay TF (1998). Introduction to quantitative genetics
      (4th ed.). Essex: Longman. ISBN 978-0-582-24302-6.
  27. ^Rose_SP (June 2006). "Commentary: heritability estimates--long past
      their sell-by date". International Journal of Epidemiology. 35 (3):
      525â7. doi:10.1093/ije/dyl064. PMID 16645027.
  28. ^Joseph J (2004). "Chapter_5". The_Gene_Illusion. New York: Algora.
      p. 141. ISBN 978-1-898059-47-9.
  29. ^Bentall RP (2009). Doctoring_the_Mind:_Is_Our_Current_Treatment_of
      Mental_Illness_Really_Any_Good?. New York: New_York_University_Press.
      pp. 123â127. ISBN 978-0-8147-8723-6.
  30. ^McGrath M (5 July 2009). "Doctoring_the_Mind:_Review". The_Telegraph.
  31. ^Moore DS, Shenk D (January 2017). "The heritability fallacy". Wiley
      Interdisciplinary Reviews: Cognitive Science. 8 (1â2): e1400. doi:
      10.1002/wcs.1400. PMID 27906501.
  32. ^Feldman MW, Ramachandran S (April 2018). "Missing_compared_to_what?
      Revisiting_heritability,_genes_and_culture". Philosophical Transactions
      of the Royal Society of London. Series B, Biological Sciences. 373
      (1743): 20170064. doi:10.1098/rstb.2017.0064. PMC 5812976. PMID 29440529.
      ...all complex human traits result from a combination of causes. If these
      causes interact, it is impossible to assign quantitative values to the
      fraction of a trait due to each, just as we cannot say how much of the
      area of a rectangle is due, separately, to each of its two dimensions.
      Thus, in the analyses of complex human phenotypes...we cannot actually
      find âthe relative importance of genes and environment in the
      determination of phenotypeâ.
  33. ^ a bTurkheimer E (2011). "Still missing". Research in Human Development.
      8 (3â4): 227â241. doi:10.1080/15427609.2011.625321.
  34. ^Turkheimer E (2015). "Genetic Prediction". The Hastings Center Report.
      45 (5 Suppl): S32â8. doi:10.1002/hast.496. PMID 26413946.
  35. ^Joseph J (2014). The_Trouble_with_Twin_Studies:_A_Reassessment_of_Twin
      Research_in_the_Social_and_Behavioral_Sciences (PDF). New York:
      Routledge. p. 81. ISBN 978-1-317-60590-4.
***** Further reading[edit] *****
    * Lynch M, Walsh B (1998). Genetics and analysis of quantitative traits.
      Sunderland, Mass.: Sinauer Assoc. ISBN 978-0-87893-481-2.
Johnson W, Penke L, Spinath FM (2011). "Understanding Heritability: What it is
and What it is Not". European Journal of Personality. 25 (4): 287â294. doi:
10.1002/per.835. ISSN 0890-2070.
***** External links[edit] *****
    * Stanford_Encyclopedia_of_Philosophy_entry_on_Heredity_and_Heritability
    * Quantitative_Genetics_Resources_website,_including_the_two_volume_book_by
      Lynch_and_Walsh._Free_access
    * v
    * t
    * e
Genetics: Quantitative_genetics
                                      * Heritability
Concepts in Quantitative Genetics     * Quantitative_trait_locus
                                      * Candidate_gene
                                      * Effective_population_size
                                      * Population_genetics
Related Topics                        * Genomics
                                      * Evolutionary_biology
                                      * Heredity
    * [Category] Category
    * v
    * t
    * e
The development of phenotype
                                 * Genotypeâphenotype_distinction
                                 * Norms_of_reaction
                                 * Geneâenvironment_interaction
                                 * Geneâenvironment_correlation
Key concepts                     * Operon
                                 * Heritability
                                 * Quantitative_genetics
                                 * Heterochrony
                                       o Neoteny
                                 * Heterotopy
                                 * Canalisation
                                 * Genetic_assimilation
                                 * Dominance
                                 * Epistasis
Genetic_architecture             * Fitness_landscape/evolutionary_landscape
                                 * Pleiotropy
                                 * Plasticity
                                 * Polygenic_inheritance
                                 * Transgressive_segregation
                                 * Sequence_space
                                 * Epigenetics
                                 * Maternal_effect
Non-genetic influences           * Genomic_imprinting
                                 * Dual_inheritance_theory
                                 * Polyphenism
                                 * Developmental_biology
                                 * Morphogenesis
                                       o Eyespot
Developmental architecture             o Pattern_formation
                                 * Segmentation
                                 * Metamerism
                                 * Modularity
                                 * Evolvability
Evolution of genetic systems     * Mutational_robustness
                                 * Neutral_networks
                                 * Evolution_of_sexual_reproduction
                                          * Regulation_of_gene_expression
                                          * Gene_regulatory_network
                                          * Developmental-genetic_toolkit
                             Systems      * Evolutionary_developmental_biology
                                          * Homeobox
                                          * Hedgehog_signaling_pathway
                                          * Notch_signaling_pathway
                                          * Homeotic_gene
Control of development                    * Hox_gene
                                          * Pax_genes
                                                o eyeless_gene
                                          * Distal-less
                             Elements     * Engrailed
                                          * cis-regulatory_element
                                          * Ligand
                                          * Morphogen
                                          * Cell_surface_receptor
                                          * Transcription_factor
                                 * C._H._Waddington
                                 * Richard_Lewontin
                                 * FranÃ§ois_Jacob + Jacques_Monod
                                       o Lac_operon
Influential figures              * Eric_F._Wieschaus
                                 * Christiane_NÃ¼sslein-Volhard
                                 * William_McGinnis
                                 * Mike_Levine
                                 * Sean_B._Carroll
                                       o Endless_Forms_Most_Beautiful
Debates                          * Nature_versus_nurture
                                 * Morphogenetic_field
Index_of_evolutionary_biology_articles
    * v
    * t
    * e
Lysenkoism
                    * Trofim_Lysenko
                    * Nikita_Khrushchev
Lysenkoists         * Ivan_Vladimirovich_Michurin
                    * Joseph_Stalin
                    * VASKhNIL
                    * WacÅaw_Gajewski
                    * Tan_Jiazhen
Dissidents          * Georgii_Karpechenko
                    * Zhores_Medvedev
                    * Georgii_Nadson
                    * Nikolai_Vavilov
                    * Heredity
                    * Heritability
                    * Hybridization
Concepts            * Inheritance_of_acquired_characteristics
                    * Lamarckism
                    * Mendelian_inheritance
                    * Vernalization
                    * Bourgeois_pseudoscience
                    * Collectivization_in_the_Soviet_Union
                    * Pavlovian_session
Soviet policies     * Socialist_realism
                    * Suppressed_research_in_the_Soviet_Union
                    * Wrecking
                    * Politicization_of_science
    * [Wikipedia book] Book
Authority_control [Edit_this_at_Wikidata]     * GND: 4311919-0

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Heritability&oldid=908677522"
Categories:
    * Genetics
Hidden categories:
    * Articles_with_short_description
    * Articles_needing_more_viewpoints_from_August_2016
    * Wikipedia_articles_with_GND_identifiers
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
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * FranÃ§ais
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Bahasa_Melayu
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 31 July 2019, at 08:01 (UTC).
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
