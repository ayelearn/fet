The following text has been accessed from https://en.wikipedia.org/wiki/Species_diversity at Fri Aug 9 00:04:06 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Species diversity ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Species diversity is the number of different species that are represented in a
given community (a dataset). The effective number of species refers to the
number of equally abundant species needed to obtain the same mean proportional
species abundance as that observed in the dataset of interest (where all
species may not be equally abundant). Species diversity consists of three
components: species_richness, taxonomic or phylogenetic diversity and species
evenness. Species richness is a simple count of species, taxonomic or
phylogenetic diversity is the genetic relationship between different groups of
species,whereas species evenness quantifies how equal the abundances of the
species are.[1][2][3]
⁰
***** Contents *****
    * 1_Calculation_of_diversity
    * 2_Diversity_indices
    * 3_Sampling_considerations
    * 4_Trends
    * 5_See_also
    * 6_Notes
    * 7_External_links
***** Calculation of diversity[edit] *****
Species diversity in a dataset can be calculated by first taking the weighted
average of species proportional abundances in the dataset, and then taking the
inverse of this. The equation is:[1][2][3]
             q    D =   1     &#x2211;  i = 1   S    p  i    p  i   q &#x2212;
      1     q &#x2212; 1        {\displaystyle {}^{q}\!D={1 \over {\sqrt[{q-1}]
      {\sum _{i=1}^{S}p_{i}p_{i}^{q-1}}}}}  [{}^q\!D={1 \over \sqrt[q-1]{{\sum_
      {i=1}^S p_i p_i^{q-1}}}}]
The denominator equals mean proportional species abundance in the dataset as
calculated with the weighted generalized_mean with exponent q - 1. In the
equation, S is the total number of species (species richness) in the dataset,
and the proportional abundance of the ith species is      p  i
{\displaystyle p_{i}}  [p_{i}]. The proportional abundances themselves are used
as weights. The equation is often written in the equivalent form:
             q    D =   (   &#x2211;  i = 1   S    p  i   q    )   1  /  ( 1
      &#x2212; q )     {\displaystyle {}^{q}\!D=\left({\sum _{i=1}^{S}p_{i}^
      {q}}\right)^{1/(1-q)}}  [{}^q\!D=\left ( {\sum_{i=1}^S p_i^q} \right )^
      {1/(1-q)}]
The value of q defines which kind of mean is used. q = 0 corresponds to the
weighted harmonic_mean, which is 1/S because the      p  i     {\displaystyle
p_{i}}  [p_{i}] values cancel out. q = 1 is undefined, except that the limit as
q approaches 1 is well defined:
          lim  q &#x2192; 1       q    D = exp &#x2061;  (  &#x2212;  &#x2211;
      i = 1   S    p  i   ln &#x2061;  p  i    )    {\displaystyle \lim _
      {q\rightarrow 1}{}^{q}\!D=\exp \left(-\sum _{i=1}^{S}p_{i}\ln p_
      {i}\right)}  [\lim_{q \rightarrow 1} {}^q\!D = \exp\left(-\sum_{i=1}^S
      p_i \ln p_i\right)]
q = 2 corresponds to the arithmetic_mean. As q approaches infinity, the
generalized mean approaches the maximum      p  i     {\displaystyle p_{i}}
[p_{i}] value. In practice, q modifies species weighting, such that increasing
q increases the weight given to the most abundant species, and fewer equally
abundant species are hence needed to reach mean proportional abundance.
Consequently, large values of q lead to smaller species diversity than small
values of q for the same dataset. If all species are equally abundant in the
dataset, changing the value of q has no effect, but species diversity at any
value of q equals species richness.
Negative values of q are not used, because then the effective number of species
(diversity) would exceed the actual number of species (richness). As q
approaches negative infinity, the generalized mean approaches the minimum
p  i     {\displaystyle p_{i}}  [p_{i}] value. In many real datasets, the least
abundant species is represented by a single individual, and then the effective
number of species would equal the number of individuals in the dataset.[2][3]
The same equation can be used to calculate the diversity in relation to any
classification, not only species. If the individuals are classified into genera
or functional types,      p  i     {\displaystyle p_{i}}  [p_{i}] represents
the proportional abundance of the ith genus or functional type, and qD equals
genus diversity or functional type diversity, respectively.
***** Diversity indices[edit] *****
Often researchers have used the values given by one or more diversity indices
to quantify species diversity. Such indices include species_richness, the
Shannon_index, the Simpson_index, and the complement of the Simpson index (also
known as the Gini-Simpson index).[4][5][6]
When interpreted in ecological terms, each one of these indices corresponds to
a different thing, and their values are therefore not directly comparable.
Species richness quantifies the actual rather than effective number of species.
The Shannon index equals log(qD), and in practice quantifies the uncertainty in
the species identity of an individual that is taken at random from the dataset.
The Simpson index equals 1/qD and quantifies the probability that two
individuals taken at random from the dataset (with replacement of the first
individual before taking the second) represent the same species. The Gini-
Simpson index equals 1 - 1/qD and quantifies the probability that the two
randomly taken individuals represent different species.[1][2][3][6][7]
***** Sampling considerations[edit] *****
Depending on the purposes of quantifying species diversity, the data set used
for the calculations can be obtained in different ways. Although species
diversity can be calculated for any data-set where individuals have been
identified to species, meaningful ecological interpretations require that the
dataset is appropriate for the questions at hand. In practice, the interest is
usually in the species diversity of areas so large that not all individuals in
them can be observed and identified to species, but a sample of the relevant
individuals has to be obtained. Extrapolation from the sample to the underlying
population of interest is not straightforward, because the species diversity of
the available sample generally gives an underestimation of the species
diversity in the entire population. Applying different sampling_methods will
lead to different sets of individuals being observed for the same area of
interest, and the species diversity of each set may be different. When a new
individual is added to a dataset, it may introduce a species that was not yet
represented. How much this increases species diversity depends on the value of
q: when q = 0, each new actual species causes species diversity to increase by
one effective species, but when q is large, adding a rare species to a dataset
has little effect on its species diversity.[8]
In general, sets with many individuals can be expected to have higher species
diversity than sets with fewer individuals. When species diversity values are
compared among sets, sampling efforts need to be standardised in an appropriate
way for the comparisons to yield ecologically meaningful results. Resampling
methods can be used to bring samples of different sizes to a common footing.[9]
Species_discovery_curves and the number of species only represented by one or a
few individuals can be used to help in estimating how representative the
available sample is of the population from which it was drawn.[10][11]
***** Trends[edit] *****
The observed species diversity is affected not only by the number of
individuals but also by the heterogeneity of the sample. If individuals are
drawn from different environmental conditions (or different habitats), the
species diversity of the resulting set can be expected to be higher than if all
individuals are drawn from a similar environment. Increasing the area sampled
increases observed species diversity both because more individuals get included
in the sample and because large areas are environmentally more heterogeneous
than small areas.
***** See also[edit] *****
    * [icon]Environment_portal
    * [icon]Ecology_portal
    * Earth_sciences_portal
    * [icon]Sustainable_development_portal
    * Alpha_diversity
    * Beta_diversity
    * Biodiversity
          o Diversity_index
          o Measurement_of_biodiversity
    * Dark_diversity
    * Gamma_diversity
    * Genetic_diversity
    * Latitudinal_gradients_in_species_diversity
    * Relative_species_abundance
    * Speciesâarea_relationship
***** Notes[edit] *****
   1. ^ a b c Hill, M. O. (1973) Diversity and evenness: a unifying notation
      and its consequences. Ecology, 54, 427â432
   2. ^ a b c d Tuomisto, H. (2010) A diversity of beta diversities:
      straightening up a concept gone awry. Part 1. Defining beta diversity as
      a function of alpha and gamma diversity. Ecography, 33, 2-22. doi:
      10.1111/j.1600-0587.2009.05880.x
   3. ^ a b c d Tuomisto, H. 2010. A consistent terminology for quantifying
      species diversity? Yes, it does exist. Oecologia 4: 853â860. doi:
      10.1007/s00442-010-1812-0
   4. ^ Krebs, C. J. (1999) Ecological Methodology. Second edition. Addison-
      Wesley, California.
   5. ^ Magurran, A. E. (2004) Measuring biological diversity. Blackwell
      Publishing, Oxford.
   6. ^ a b Jost, L. (2006) Entropy and diversity. Oikos, 113, 363â375
   7. ^ Jost, L. (2007) Partitioning diversity into independent alpha and beta
      components. Ecology, 88, 2427â2439.
   8. ^ Tuomisto, H. (2010) A diversity of beta diversities: straightening up a
      concept gone awry. Part 2. Quantifying beta diversity and related
      phenomena. Ecography, 33, 23-45. doi:10.1111/j.1600-0587.2009.06148.x
   9. ^ Colwell, R. K. and Coddington, J. A. (1994) Estimating terrestrial
      biodiversity through extrapolation. Philosophical Transactions:
      Biological Sciences, 345, 101-118.
  10. ^ Good, I. J. and Toulmin, G. H. (1956) The number of new species, and
      the increase in population coverage, when a sample is increased.
      Biometrika, 43, 45-63.
  11. ^ Chao,_A. (2005) Species richness estimation. Pages 7909-7916 in N.
      Balakrishnan, C. B. Read, and B. Vidakovic, eds. Encyclopedia of
      Statistical Sciences. New York, Wiley.
***** External links[edit] *****
    * Harrison, Ian; Laverty, Melina; Sterling, Eleanor. "Species_Diversity".
      Connexions (cnx.org). William and Flora Hewlett Foundation, the Maxfield
      Foundation, and the Connexions Consortium. Retrieved 1 February 2011.
 (Licensed under Creative_Commons_1.0_Attribution_Generic).
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
                * Species diversity
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
index.php?title=Species_diversity&oldid=904153243"
Categories:
    * Ecological_metrics
    * Habitat
    * Environmental_terminology
    * Measurement_of_biodiversity
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
    * ÄeÅ¡tina
    * Deutsch
    * Esperanto
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * ×¢××¨××ª
    * æ¥æ¬èª
    * à¨ªà©°à¨à¨¾à¨¬à©
    * PortuguÃªs
    * SlovenÅ¡Äina
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 30 June 2019, at 09:22 (UTC).
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
