The following text has been accessed from https://en.wikipedia.org/wiki/Population_ecology at Fri Aug 9 03:59:07 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Population ecology ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Study of the dynamics of species populations and how these populations interact
with the environment
The_human_population_is_growing at a logistic rate and has been affecting the
populations of other species in return. Chemical_pollution, deforestation, and
population are very big problems. Irrigation are examples of means by which
humans may influence the population ecology of other species. As the human
population increases, its effect on the populations of other species may also
increase.
Populations cannot grow indefinitely. Population ecology involves studying
factors that affect population growth and survival. Mass_extinctions are
examples of factors that have radically reduced populations' sizes and
populations' survivability. The survivability of populations is critical to
maintaining high levels of biodiversity on Earth.
Population ecology is a sub-field of ecology that deals with the dynamics of
species populations and how these populations interact with the environment.[1]
It is the study of how the population_sizes of species change over time and
space. The term population ecology is often used interchangeably with
population_biology or population_dynamics.
The development of population ecology owes much to demography and actuarial
life_tables. Population ecology is important in conservation_biology,
especially in the development of population_viability_analysis (PVA) which
makes it possible to predict the long-term probability of a species persisting
in a given habitat patch. Although population ecology is a subfield of biology,
it provides interesting problems for mathematicians and statisticians who work
in population_dynamics.
⁰
***** Contents *****
    * 1_Fundamentals
    * 2_Geometric_populations
          o 2.1_Doubling_time_of_geometric_populations
          o 2.2_Half-life_of_geometric_populations
          o 2.3_Geometric_(R)_and_finite_(Î»)_growth_constants
                # 2.3.1_Geometric_(R)_growth_constant
                # 2.3.2_Finite_(Î»)_growth_constant
          o 2.4_Mathematical_relationship_between_geometric_and_exponential
            populations
    * 3_r/K_selection
    * 4_Metapopulation
    * 5_History
    * 6_Journals
    * 7_See_also
    * 8_References
    * 9_Further_reading
    * 10_External_links
***** Fundamentals[edit] *****
 Terms used to describe natural groups of individuals in ecological studies[2]
Term               Definition
Species population All individuals of a species.
Metapopulation     A set of spatially disjunct populations, among which there
                   is some immigration.
Population         A group of conspecific individuals that is demographically,
                   genetically, or spatially disjunct from other groups of
                   individuals.
Aggregation        A spatially clustered group of individuals.
Deme               A group of individuals more genetically similar to each
                   other than to other individuals, usually with some degree of
                   spatial isolation as well.
Local population   A group of individuals within an investigator-delimited area
                   smaller than the geographic range of the species and often
                   within a population (as defined above). A local population
                   could be a disjunct population as well.
Subpopulation      An arbitrary spatially delimited subset of individuals from
                   within a population (as defined above).
The most fundamental law of population ecology is Thomas_Malthus' exponential
law of population growth.[3]
     A population will grow (or decline) exponentially as long as the
     environment experienced by all individuals in the population remains
     constant.[3]:18
Thomas_Robert_Malthus
This principle in population ecology provides the basis for formulating
predictive theories and tests that follow:
Simplified population models usually start with four key variables (four
demographic processes) including death, birth, immigration, and emigration.
Mathematical models used to calculate changes in population demographics and
evolution hold the assumption (or null_hypothesis) of no external influence.
Models can be more mathematically complex where "...several competing
hypotheses are simultaneously confronted with the data."[4] For example, in a
closed system where immigration and emigration does not take place, the rate of
change in the number of individuals in a population can be described as:
            d N   d T    = B &#x2212; D = b N &#x2212; d N = ( b &#x2212; d ) N
      = r N ,   {\displaystyle {\frac {dN}{dT}}=B-D=bN-dN=(b-d)N=rN,}  [{\frac
      {dN}{dT}}=B-D=bN-dN=(b-d)N=rN,]
where N is the total number of individuals in the population, B is the raw
number of births, D is the raw number of deaths, b and d are the per capita
rates of birth and death respectively, and r is the per capita average number
of surviving offspring each individual has. This formula can be read as the
rate of change in the population (dN/dT) is equal to births minus deaths (B -
D).[3][5]
Using these techniques, Malthus' population principle of growth was later
transformed into a mathematical model known as the logistic_equation:
            d N   d T    = a N  (  1 &#x2212;   N K    )  ,   {\displaystyle
      {\frac {dN}{dT}}=aN\left(1-{\frac {N}{K}}\right),}  [{\frac {dN}
      {dT}}=aN\left(1-{\frac {N}{K}}\right),]
where N is the biomass density, a is the maximum per-capita rate of change, and
K is the carrying_capacity of the population. The formula can be read as
follows: the rate of change in the population (dN/dT) is equal to growth (aN)
that is limited by carrying capacity (1-N/K). From these basic mathematical
principles the discipline of population ecology expands into a field of
investigation that queries the demographics of real populations and tests these
results against the statistical models. The field of population ecology often
uses data on life history and matrix algebra to develop projection matrices on
fecundity and survivorship. This information is used for managing wildlife
stocks and setting harvest quotas [5][6]
***** Geometric populations[edit] *****
Operophtera brumata (Winter moth) populations are geometric.[7]
The population model below can be manipulated to mathematically infer certain
properties of geometric populations. A population with a size that increases
geometrically is a population where generations of reproduction do not overlap.
[8] In each generation there is an effective_population_size denoted as Ne
which constitutes the number of individuals in the population that are able to
reproduce and will reproduce in any reproductive generation in concern.[9] In
the population model below it is assumed that N is the effective population
size.[8]
Assumption 01: Ne = N
Nt+1 = Nt + Bt + It - Dt - Et
Term Definition
     Population size in the generation after generation t. This may be the current
Nt+1 generation or the next (upcoming) generation depending on the situation in which
     the population model is used.
Nt   Population size in generation t.
Bt   Sum (Î£) of births in the population between generations t and t+1. Also known
     as raw birth rate.
It   Sum (Î£) of immigrants moving into the population between generations t and t+1.
     Also known as raw immigration rate.
Dt   Sum (Î£) of deaths in the population between generations t and t+1. Also known
     as raw death rate.
Et   Sum (Î£) of emigrants moving out of the population between generations t and
     t+1. Also known as raw emigration rate.
The general difference between populations that grow exponentially and
geometrically. Geometric populations grow in reproductive generations between
intervals of abstinence from reproduction. Exponential populations grow without
designated periods for reproduction. Reproduction is a continuous process and
generations of reproduction overlap. This graph illustrates two hypothetical
populations - one population growing periodically (and therefore geometrically)
and the other population growing continuously (and therefore exponentially).
The populations in the graph have a doubling time of 1 year. The populations in
the graph are hypothetical. In reality, the doubling times differ between
populations.
Assumption 02: There is no migration to or from the population (N)
It = Et = 0
Nt+1 = Nt + Bt - Dt
The raw birth and death rates are related to the per capita birth and death
rates:
Bt = bt Ã Nt
Dt = dt Ã Nt
bt = Bt / Nt
dt = Dt / Nt
Term Definition
bt   Per capita birth rate.
dt   Per capita death rate.
Therefore:
Nt+1 = Nt + (bt Ã Nt) - (dt Ã Nt)
Assumption 03: bt and dt are constant (i.e. they don't change each generation).
Nt+1 = Nt + (bNt) - (dNt)
Term Definition
b    Constant per capita birth rate.
d    Constant per capita death rate.
Take the term Nt out of the brackets.
Nt+1 = Nt + (b - d)Nt
b - d = R
Term Definition
R    Geometric rate of increase.
Nt+1 = Nt + RNt
Nt+1 = (Nt + RNt)
Take the term Nt out of the brackets again.
Nt+1 = (1 + R)Nt
1 + R = Î»
Term Definition
Î» Finite rate of increase.
Nt+1 = Î»Nt
At  Nt+1 = Î»Nt
t+1
At  Nt+2 = Î»Nt+1 = Î»Î»Nt = Î»2Nt
t+2
At  Nt+3 = Î»Nt+2 = Î»Î»Nt+1 = Î»Î»Î»Nt = Î»3Nt
t+3
At  Nt+4 = Î»Nt+3 = Î»Î»Nt+2 = Î»Î»Î»Nt+1 = Î»Î»Î»Î»Nt = Î»4Nt
t+4
At  Nt+5 = Î»Nt+4 = Î»Î»Nt+3 = Î»Î»Î»Nt+2 = Î»Î»Î»Î»Nt+1 = Î»Î»Î»Î»Î»Nt = Î»5Nt
t+5
Therefore:
Nt+1 = Î»tNt
Term Definition
     Finite rate of increase raised to the power of the number of generations (e.g. for t+2
Î»t[two generations] â Î»2 , for t+1 [one generation] â Î»1 = Î», and for t [before any
     generations - at time zero] â Î»0 = 1
**** Doubling time of geometric populations[edit] ****
G. stearothermophilus has a shorter doubling time (td) than E. coli and N.
meningitidis. Growth rates of 2 bacterial species will differ by unexpected
orders of magnitude if the doubling times of the 2 species differ by even as
little as 10 minutes. In eukaryotes such as animals, fungi, plants, and
protists, doubling times are much longer than in bacteria. This reduces the
growth rates of eukaryotes in comparison to Bacteria. G._stearothermophilus, E.
coli, and N._meningitidis have 20 minute,[10] 30 minute,[11] and 40 minute[12]
doubling times under optimal conditions respectively. If bacterial populations
could grow indefinitely (which they do not) then the number of bacteria in each
species would approach infinity (â). However, the percentage of G.
stearothermophilus bacteria out of all the bacteria would approach 100% whilst
the percentage of E. coli and N. meningitidis combined out of all the bacteria
would approach 0%. This graph is a simulation of this hypothetical scenario. In
reality, bacterial populations do not grow indefinitely in size and the 3
species require different optimal conditions to bring their doubling times to
minima.
Time in minutes % that is G. stearothermophilus
30              44.4%
60              53.3%
90              64.9%
120             72.7%
ââ    100%
Time in minutes % that is E. coli
30              29.6%
60              26.7%
90              21.6%
120             18.2%
ââ    0.00%
Time in minutes % that is N. meningitidis
30              25.9%
60              20.0%
90              13.5%
120             9.10%
ââ    0.00%
Disclaimer: Bacterial populations are exponential (or, more correctly,
logistic) instead of geometric. Nevertheless, doubling times are applicable to
both types of populations.
The doubling_time of a population is the time required for the population to
grow to twice its size.[13] We can calculate the doubling_time of a geometric
population using the equation: Nt+1 = Î»tNt by exploiting our knowledge of the
fact that the population (N) is twice its size (2N) after the doubling time.[8]
2Ntd = Î»td Ã Nt
Term Definition
td   Doubling time.
Î»td = 2Ntd / Nt
Î»td = 2
The doubling time can be found by taking logarithms. For instance:
td Ã log2(Î») = log2(2)
log2(2) = 1
td Ã log2(Î») = 1
td = 1 / log2(Î»)
Or:
td Ã ln(Î») = ln(2)
td = ln(2) / ln(Î»)
td = 0.693... / ln(Î»)
Therefore:
td = 1 / log2(Î») = 0.693... / ln(Î»)
**** Half-life of geometric populations[edit] ****
The half-life of a population is the time taken for the population to decline
to half its size. We can calculate the half-life of a geometric population
using the equation: Nt+1 = Î»tNt by exploiting our knowledge of the fact that
the population (N) is half its size (0.5N) after a half-life.[8]
0.5Nt1/2 = Î»t1/2 Ã Nt
Term Definition
t1/2 Half-life.
Î»t1/2 = 0.5Nt1/2 / Nt
Î»t1/2 = 0.5
The half-life can be calculated by taking logarithms (see above).
t1/2 = 1 / log0.5(Î») = ln(0.5) / ln(Î»)
**** Geometric (R) and finite (Î») growth constants[edit] ****
*** Geometric (R) growth constant[edit] ***
R = b - d
Nt+1 = Nt + RNt
Nt+1 - Nt = RNt
Nt+1 - Nt = ÎN
Term Definition
ÎNChange in population size between two generations (between generation t+1
     and t).
ÎN = RNt
ÎN/Nt = R
*** Finite (Î») growth constant[edit] ***
1 + R = Î»
Nt+1 = Î»Nt
Î» = Nt+1 / Nt
**** Mathematical relationship between geometric and exponential populations
[edit] ****
In geometric populations, R and Î» represent growth constants (see 2 and 2.3).
In exponential populations however, the intrinsic_growth_rate, also known as
intrinsic_rate_of_increase (r) is the relevant growth constant. Since
generations of reproduction in a geometric population do not overlap (e.g.
reproduce once a year) but do in an exponential population, geometric and
exponential populations are usually considered to be mutually exclusive.[14]
However, geometric constants and exponential constants share the mathematical
relationship below.[8]
The growth equation for exponential populations is
Nt = N0ert
Term Definition
e    Euler's_number - A universal_constant often applicable in exponential
     equations.
r    intrinsic_growth_rate - also known as intrinsic_rate_of_increase.
Leonhard_Euler was the mathematician who established the universal constant
2.71828... also known as Euler's_number or e.
Assumption: Nt (of a geometric population) = Nt (of an exponential population).
Therefore:
N0ert = N0Î»t
N0 cancels on both sides.
N0ert / N0 = Î»t
ert = Î»t
Take the natural_logarithms of the equation. Using natural logarithms instead
of base 10 or base 2 logarithms simplifies the final equation as ln(e) = 1.
rt Ã ln(e) = t Ã ln(Î»)
Term Definition
     natural_logarithm - in other words ln(y) = loge(y) = x = the power (x)
ln   that e needs to be raised to (ex) to give the answer y.
     In this case, e1 = e therefore ln(e) = 1.
rt Ã 1 = t Ã ln(Î»)
rt = t Ã ln(Î»)
t cancels on both sides.
rt / t = ln(Î»)
The results:
r = ln(Î»)
and
er = Î»
***** r/K selection[edit] *****
Main article: r/K_selection
At its most elementary level, interspecific competition involves two species
utilizing a similar resource. It rapidly gets more complicated, but stripping
the phenomenon of all its complications, this is the basic principle: two
consumers consuming the same resource.[5]:222
An important concept in population ecology is the r/K_selection theory. The
first variable is r (the intrinsic rate of natural increase in population size,
density independent) and the second variable is K (the carrying capacity of a
population, density dependent).[15] An r-selected species (e.g., many kinds of
insects, such as aphids[16]) is one that has high rates of fecundity, low
levels of parental investment in the young, and high rates of mortality before
individuals reach maturity. Evolution favors productivity in r-selected
species. In contrast, a K-selected species (such as humans) has low rates of
fecundity, high levels of parental investment in the young, and low rates of
mortality as individuals mature. Evolution in K-selected species favors
efficiency in the conversion of more resources into fewer offspring.[17][18]
***** Metapopulation[edit] *****
Main article: Metapopulation
Populations are also studied and conceptualized through the "metapopulation"
concept. The metapopulation concept was introduced in 1969:[19]
     "as a population of populations which go extinct locally and
     recolonize."[20]:105
Metapopulation ecology is a simplified model of the landscape into patches of
varying levels of quality.[21] Patches are either occupied or they are not.
Migrants moving among the patches are structured into metapopulations either as
sources or sinks. Source patches are productive sites that generate a seasonal
supply of migrants to other patch locations. Sink patches are unproductive
sites that only receive migrants. In metapopulation terminology there are
emigrants (individuals that leave a patch) and immigrants (individuals that
move into a patch). Metapopulation models examine patch dynamics over time to
answer questions about spatial and demographic ecology. An important concept in
metapopulation ecology is the rescue effect, where small patches of lower
quality (i.e., sinks) are maintained by a seasonal influx of new immigrants.
Metapopulation structure evolves from year to year, where some patches are
sinks, such as dry years, and become sources when conditions are more
favorable. Ecologists utilize a mixture of computer models and field studies to
explain metapopulation structure.[22]
***** History[edit] *****
The older term, autecology (from Greek: Î±á½ÏÎ¿, auto, "self"; Î¿Î¯ÎºÎ¿Ï,
oikos, "household"; and Î»ÏÎ³Î¿Ï, logos, "knowledge"), refers to roughly the
same field of study as population ecology. It derives from the division of
ecology into autecologyâthe study of individual species in relation to the
environmentâand synecologyâthe study of groups of organisms in relation to
the environmentâor community ecology. Odum (1959, p. 8) considered that
synecology should be divided into population ecology, community ecology, and
ecosystem ecology, defining autecology as essentially "species ecology."[1]
However, for some time biologists have recognized that the more significant
level of organization of a species is a population, because at this level the
species gene pool is most coherent. In fact, Odum regarded "autecology" as no
longer a "present tendency" in ecology (i.e., an archaic term), although
included "species ecology"âstudies emphasizing life_history and behavior as
adaptations to the environment of individual organisms or speciesâas one of
four subdivisions of ecology.
***** Journals[edit] *****
The first journal publication of the Society of Population Ecology, titled
Population Ecology (originally called Researches on Population Ecology) was
released in 1952.[23]
Scientific articles on population ecology can also be found in the Journal_of
Animal_Ecology, Oikos and other journals.
***** See also[edit] *****
    * Deep_ecology
    * Density-dependent_inhibition
    * Irruptive_growth
    * Lists_of_organisms_by_population
    * Overpopulation
    * Overpopulation_in_companion_animals
    * Overshoot_(population)
    * Population_density
    * Population_distribution
    * Population_dynamics
    * Population_dynamics_of_fisheries
    * Population_genetics
    * Population_growth
    * Theoretical_ecology
***** References[edit] *****
   1. ^ a bOdum,_Eugene_P. (1959). Fundamentals of Ecology (Second ed.).
      Philadelphia and London: W. B. Saunders Co. p. 546 p. ISBN 9780721669410.
      OCLC 554879.
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
   3. ^Wells, J. V.; Richmond, M. E. (1995). "Populations,_metapopulations,_and
      species_populations:_What_are_they_and_who_should_care?" (PDF). Wildlife
      Society Bulletin. 23 (3): 458â462. Archived from the_original (PDF) on
      November 4, 2005.
   4. ^ a b cTurchin, P. (2001). "Does Population Ecology Have General Laws?".
      Oikos. 94 (1): 17â26. doi:10.1034/j.1600-0706.2001.11310.x.
   5. ^Johnson, J. B.; Omland, K. S. (2004). "Model_selection_in_ecology_and
      evolution" (PDF). Trends in Ecology and Evolution. 19 (2): 101â108.
      CiteSeerX 10.1.1.401.777. doi:10.1016/j.tree.2003.10.013. PMID 16701236.
   6. ^ a b cVandermeer, J. H.; Goldberg, D. E. (2003). Population ecology:
      First principles. Woodstock, Oxfordshire: Princeton University Press.
      ISBN 978-0-691-11440-8.
   7. ^Berryman, A. A. (1992). "The Origins and Evolution of Predator-Prey
      Theory". Ecology. 73 (5): 1530â1535. doi:10.2307/1940005.
      JSTOR 1940005.
   8. ^Hassell, Michael P. (June 1980). "Foraging Strategies, Population Models
      and Biological Control: A Case Study". The Journal of Animal Ecology. 49
      (2): 603â628. doi:10.2307/4267. JSTOR 4267.
   9. ^ a b c d e"GEOMETRIC_AND_EXPONENTIAL_POPULATION_MODELS" (PDF).
  10. ^Holsinger, Kent (2008-08-26). "Effective_Population_Size".
  11. ^"Bacillus_stearothermophilus_NEUF2011". Microbe wiki.
  12. ^Chandler, M.; Bird, R.E.; Caro, L. (May 1975). "The replication time of
      the Escherichia coli K12 chromosome as a function of cell doubling time".
      Journal of Molecular Biology. 94 (1): 127â132. doi:10.1016/0022-2836
      (75)90410-6.
  13. ^Tobiason, D. M.; Seifert, H. S. (19 February 2010). "Genomic_Content_of
      Neisseria_Species". Journal of Bacteriology. 192 (8): 2160â2168. doi:
      10.1128/JB.01593-09. PMC 2849444. PMID 20172999.
  14. ^Boucher, Lauren (24 March 2015). "What_is_Doubling_Time_and_How_is_it
      Calculated?". Population Education.
  15. ^"Population_Growth" (PDF). University_of_Alberta.
  16. ^Begon, M.; Townsend, C. R.; Harper, J. L. (2006). Ecology:_From
      Individuals_to_Ecosystems (4th ed.). Oxford, UK: Blackwell Publishing.
      ISBN 978-1-4051-1117-1.
  17. ^Whitham, T. G. (1978). "Habitat Selection by Pemphigus Aphids in
      Response to Response Limitation and Competition". Ecology. 59 (6):
      1164â1176. doi:10.2307/1938230. JSTOR 1938230.
  18. ^MacArthur, R.; Wilson, E. O. (1967). "The Theory of Island
      Biogeography". Princeton, NJ: Princeton University Press.
  19. ^Pianka, E. R. (1972). "r and K Selection or b and d Selection?". The
      American Naturalist. 106 (951): 581â588. doi:10.1086/282798.
  20. ^Levins, R. (1969). Some_demographic_and_genetic_consequences_of
      environmental_heterogeneity_for_biological_control. Bulletin of the
      Entomological Society of America. 15. Columbia University Press.
      pp. 237â240. doi:10.1093/besa/15.3.237. ISBN 978-0-231-12680-9.
  21. ^Levins, R. (1970). Gerstenhaber, M. (ed.). Extinction._In:_Some
      Mathematical_Questions_in_Biology. AMS Bookstore. pp. 77â107. ISBN 978-
      0-8218-1152-8.
  22. ^Hanski, I. (1998). "Metapopulation_dynamics" (PDF). Nature. 396 (6706):
      41â49. doi:10.1038/23876. Archived from the_original (PDF) on 2010-12-
      31.
  23. ^Hanski, I.; Gaggiotti, O. E., eds. (2004). Ecology,_genetics_and
      evolution_of_metapopulations. Burlington, MA: Elsevier Academic Press.
      ISBN 978-0-12-323448-3.
  24. ^"Population_Ecology". John Wiley & Sons.
***** Further reading[edit] *****
    * Kareiva, Peter (1989). "Renewing the Dialogue between Theory and
      Experiments in Population Ecology". In Roughgarden J., R.M. May and S. A.
      Levin (ed.). Perspectives in ecological theory. New Jersey: Princeton
      University Press. p. 394 p.
Odum,_Eugene_P. (1959). Fundamentals of Ecology (Second ed.). Philadelphia and
London: W. B. Saunders Co. p. 546 p. ISBN 9780721669410. OCLC 554879.
Smith, Frederick E. (1952). "Experimental methods in population dynamics: a
critique". Ecology. 33 (4): 441â450. doi:10.2307/1931519. JSTOR 1931519.
***** External links[edit] *****
    * AAAS_Atlas_of_Population_and_Environment
    * v
    * t
    * e
Ecology: Modelling_ecosystems: Trophic components
                   * Abiotic_component
                   * Abiotic_stress
                   * Behaviour
                   * Biogeochemical_cycle
                   * Biomass
                   * Biotic_component
                   * Biotic_stress
                   * Carrying_capacity
General            * Competition
                   * Ecosystem
                   * Ecosystem_ecology
                   * Ecosystem_model
                   * Keystone_species
                   * List_of_feeding_behaviours
                   * Metabolic_theory_of_ecology
                   * Productivity
                   * Resource
                   * Autotrophs
                   * Chemosynthesis
                   * Chemotrophs
                   * Foundation_species
                   * Mixotrophs
                   * Myco-heterotrophy
Producers          * Mycotroph
                   * Organotrophs
                   * Photoheterotrophs
                   * Photosynthesis
                   * Photosynthetic_efficiency
                   * Phototrophs
                   * Primary_nutritional_groups
                   * Primary_production
                   * Apex_predator
                   * Bacterivore
                   * Carnivores
                   * Chemoorganotroph
                   * Foraging
                   * Generalist_and_specialist_species
                   * Intraguild_predation
                   * Herbivores
Consumers          * Heterotroph
                   * Heterotrophic_nutrition
                   * Insectivore
                   * Mesopredators
                   * Mesopredator_release_hypothesis
                   * Omnivores
                   * Optimal_foraging_theory
                   * Planktivore
                   * Predation
                   * Prey_switching
                   * Chemoorganoheterotrophy
Decomposers        * Decomposition
                   * Detritivores
                   * Detritus
                   * Archaea
                   * Bacteriophage
                   * Environmental_microbiology
                   * Lithoautotroph
                   * Lithotrophy
                   * Microbial_cooperation
Microorganisms     * Microbial_ecology
                   * Microbial_food_web
                   * Microbial_intelligence
                   * Microbial_loop
                   * Microbial_mat
                   * Microbial_metabolism
                   * Phage_ecology
                   * Biomagnification
                   * Ecological_efficiency
Food_webs          * Ecological_pyramid
                   * Energy_flow
                   * Food_chain
                   * Trophic_level
                   * Cold_seeps
                   * Hydrothermal_vents
                   * Intertidal
                   * Kelp_forests
Example webs       * Lakes
                   * North_Pacific_Subtropical_Gyre
                   * Rivers
                   * San_Francisco_Estuary
                   * Soil
                   * Tide_pool
                   * Ascendency
                   * Bioaccumulation
                   * Cascade_effect
                   * Climax_community
                   * Competitive_exclusion_principle
                   * Consumer-resource_systems
                   * Copiotrophs
                   * Dominance
                   * Ecological_network
                   * Ecological_succession
Processes          * Energy_quality
                   * Energy_Systems_Language
                   * f-ratio
                   * Feed_conversion_ratio
                   * Feeding_frenzy
                   * Mesotrophic_soil
                   * Nutrient_cycle
                   * Oligotroph
                   * Paradox_of_the_plankton
                   * Trophic_cascade
                   * Trophic_mutualism
                   * Trophic_state_index
                   * Animal_coloration
                   * Antipredator_adaptations
                   * Camouflage
Defense,           * Deimatic_behaviour
counter            * Herbivore_adaptations_to_plant_defense
                   * Mimicry
                   * Plant_defense_against_herbivory
                   * Predator_avoidance_in_schooling_fish
    * v
    * t
    * e
Ecology: Modelling_ecosystems: Other components
                * Abundance
                * Allee_effect
                * Depensation
                * Ecological_yield
                * Effective_population_size
                * Intraspecific_competition
                * Logistic_function
                * Malthusian_growth_model
                * Maximum_sustainable_yield
Population      * Overpopulation_in_wild_animals
ecology         * Overexploitation
                * Population_cycle
                * Population_dynamics
                * Population_modeling
                * Population_size
                * Predatorâprey_(LotkaâVolterra)_equations
                * Recruitment
                * Resilience
                * Small_population_size
                * Stability
                * Biodiversity
                * Density-dependent_inhibition
                * Ecological_effects_of_biodiversity
                * Ecological_extinction
                * Endemic_species
                * Flagship_species
                * Gradient_analysis
                * Indicator_species
                * Introduced_species
                * Invasive_species
                * Latitudinal_gradients_in_species_diversity
                * Minimum_viable_population
Species         * Neutral_theory
                * Occupancyâabundance_relationship
                * Population_viability_analysis
                * Priority_effect
                * Rapoport's_rule
                * Relative_abundance_distribution
                * Relative_species_abundance
                * Species_diversity
                * Species_homogeneity
                * Species_richness
                * Species_distribution
                * Species-area_curve
                * Umbrella_species
                * Antibiosis
                * Biological_interaction
                * Commensalism
                * Community_ecology
Species         * Ecological_facilitation
interaction     * Interspecific_competition
                * Mutualism
                * Parasitism
                * Storage_effect
                * Symbiosis
                * Biogeography
                * Cross-boundary_subsidy
                * Ecocline
                * Ecotone
                * Ecotype
                * Disturbance
                * Edge_effects
                * Foster's_rule
                * Habitat_fragmentation
Spatial         * Ideal_free_distribution
ecology         * Intermediate_Disturbance_Hypothesis
                * Island_biogeography
                * Landscape_ecology
                * Landscape_epidemiology
                * Landscape_limnology
                * Metapopulation
                * Patch_dynamics
                * r/K_selection_theory
                * Resource_selection_function
                * Sourceâsink_dynamics
                * Ecological_niche
                * Ecological_trap
                * Ecosystem_engineer
                * Environmental_niche_modelling
                * Guild
Niche           * Habitat
                * Marine_habitats
                * Limiting_similarity
                * Niche_apportionment_models
                * Niche_construction
                * Niche_differentiation
                * Assembly_rules
                * Bateman's_principle
                * Bioluminescence
                * Ecological_collapse
                * Ecological_debt
                * Ecological_deficit
                * Ecological_energetics
Other           * Ecological_indicator
networks        * Ecological_threshold
                * Ecosystem_diversity
                * Emergence
                * Extinction_debt
                * Kleiber's_law
                * Liebig's_law_of_the_minimum
                * Marginal_value_theorem
                * Thorson's_rule
                * Xerosere
                * Allometry
                * Alternative_stable_state
                * Balance_of_nature
                * Biological_data_visualization
                * Ecocline
                * Ecological_economics
                * Ecological_footprint
                * Ecological_forecasting
                * Ecological_humanities
                * Ecological_stoichiometry
                * Ecopath
Other           * Ecosystem_based_fisheries
                * Endolith
                * Evolutionary_ecology
                * Functional_ecology
                * Industrial_ecology
                * Macroecology
                * Microecosystem
                * Natural_environment
                * Regime_shift
                * Systems_ecology
                * Urban_ecology
                * Theoretical_ecology
List_of_ecology_topics

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Population_ecology&oldid=908625327"
Categories:
    * Population_ecology
    * Applied_statistics
    * Population
    * Subfields_of_ecology
Hidden categories:
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
**** In other projects ****
    * Wikimedia_Commons
    * Wikiquote
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * Bosanski
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Bahasa_Indonesia
    * Italiano
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Suomi
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 30 July 2019, at 22:26 (UTC).
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
