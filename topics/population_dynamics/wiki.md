The following text has been accessed from https://en.wikipedia.org/wiki/Population_dynamics at Fri Aug 9 00:04:04 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Population dynamics ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (July 2012)(Learn_how_and_when
 to_remove_this_template_message)
Map of population trends of native and invasive species of jellyfish[1]
  Increase (high certainty)
  Increase (low certainty)
  Stable/variable
  Decrease
  No data
Population dynamics is the branch of life_sciences that studies the size and
age composition of populations as dynamical_systems, and the biological and
environmental processes driving them (such as birth and death_rates, and by
immigration and emigration). Example scenarios are ageing_populations,
population_growth, or population_decline.
⁰
***** Contents *****
    * 1_History
    * 2_Intrinsic_rate_of_increase
    * 3_Common_mathematical_models
          o 3.1_Exponential_population_growth
          o 3.2_Simple_discrete_time_exponential_model
          o 3.3_Continuous_time_version_of_exponential_growth
          o 3.4_Logistic_population_growth
          o 3.5_Continuous-time_model_of_logistic_growth
          o 3.6_Discrete_time_logistical_model
          o 3.7_Individual-based_models
    * 4_Fisheries_and_wildlife_management
    * 5_For_control_applications
    * 6_See_also
    * 7_References
    * 8_Further_reading
    * 9_External_links
***** History[edit] *****
Population dynamics has traditionally been the dominant branch of mathematical
biology, which has a history of more than 210 years, although more recently the
scope of mathematical biology has greatly expanded. The first principle of
population dynamics is widely regarded as the exponential law of Malthus, as
modeled by the Malthusian_growth_model. The early period was dominated by
demographic studies such as the work of Benjamin_Gompertz and Pierre_FranÃ§ois
Verhulst in the early 19th century, who refined and adjusted the Malthusian
demographic model.
A more general model formulation was proposed by F.J._Richards in 1959, further
expanded by Simon_Hopkins, in which the models of Gompertz, Verhulst and also
Ludwig_von_Bertalanffy are covered as special cases of the general formulation.
The LotkaâVolterra_predator-prey_equations are another famous example, as
well as the alternative ArditiâGinzburg_equations. The computer_game SimCity,
Sim_Earth and the MMORPG Ultima_Online, among others, tried to simulate some of
these population dynamics.
In the past 30 years, population dynamics has been complemented by evolutionary
game_theory, developed first by John_Maynard_Smith. Under these dynamics,
evolutionary biology concepts may take a deterministic mathematical form.
Population dynamics overlap with another active area of research in
mathematical biology: mathematical_epidemiology, the study of infectious
disease affecting populations. Various models of viral spread have been
proposed and analyzed, and provide important results that may be applied to
health policy decisions.
***** Intrinsic rate of increase[edit] *****
The rate at which a population increases in size if there are no density-
dependent forces regulating the population is known as the intrinsic rate of
increase. It is
             d N   d t        1 N    = r   {\displaystyle {\dfrac {dN}{dt}}
      {\dfrac {1}{N}}=r}  [{\dfrac {dN}{dt}}{\dfrac {1}{N}}=r]
where the derivative     d N  /  d t   {\displaystyle dN/dt}  [dN/dt] is the
rate of increase of the population, N is the population size, and r is the
intrinsic rate of increase. Thus r is the maximum theoretical rate of increase
of a population per individual â that is, the maximum population growth rate.
The concept is commonly used in insect population biology to determine how
environmental factors affect the rate at which pest populations increase. See
also exponential population growth and logistic population growth.[2]
***** Common mathematical models[edit] *****
**** Exponential population growth[edit] ****
Exponential growth describes unregulated reproduction. It is very unusual to
see this in nature. In the last 100 years, human_population_growth has appeared
to be exponential. In the long run, however, it is not likely. Thomas Malthus
believed that human population growth would lead to overpopulation and
starvation due to scarcity of resources. They believed that human population
would grow at rate in which they exceed the ability at which humans can find
food. In the future, humans would be unable to feed large populations. The
biological assumptions of exponential growth is that the per capita growth rate
is constant. Growth is not limited by resource scarcity or predation.[3]
**** Simple discrete time exponential model[edit] ****
          N  t + 1   = &#x03BB;  N  t     {\displaystyle N_{t+1}=\lambda N_{t}}
      [N_{t+1}=\lambda N_{t}]
where Î» is the discrete-time per capita growth rate. At Î» = 1, we get a
linear line and a discrete-time per capita growth rate of zero. At Î» < 1, we
get a decrease in per capita growth rate. At Î» > 1, we get an increase in per
capita growth rate. At Î» = 0, we get extinction of the species.[3]
**** Continuous time version of exponential growth[edit] ****
Some species have continuous reproduction.
             d N   d T     = r N   {\displaystyle {\dfrac {dN}{dT}}=rN}  [
      {\dfrac {dN}{dT}}=rN]
where         d N   d T       {\displaystyle {\dfrac {dN}{dT}}}  [{\dfrac {dN}
{dT}}] is the rate of population growth per unit time, r is the maximum per
capita growth rate, and N is the population size.
At r > 0, there is an increase in per capita growth rate. At r = 0, the per
capita growth rate is zero. At r < 0, there is a decrease in per capita growth
rate.
**** Logistic population growth[edit] ****
âLogisticsâ comes from the French word logistique, which means âto
computeâ. Population regulation is a density-dependent process, meaning that
population growth rates are regulated by the density of a population. Consider
an analogy with a thermostat. When the temperature is too hot, the thermostat
turns on the air conditioning to decrease the temperature back to homeostasis.
When the temperature is too cold, the thermostat turns on the heater to
increase the temperature back to homeostasis. Likewise with density dependence,
whether the population density is high or low, population dynamics returns the
population density to homeostasis. Homeostasis is the set point, or carrying
capacity, defined as K.[3]
**** Continuous-time model of logistic growth[edit] ****
             d N   d T     = r N   (   1 &#x2212;    N K      )
      {\displaystyle {\dfrac {dN}{dT}}=rN{\Big (}1-{\dfrac {N}{K}}{\Big )}}  [
      {\dfrac {dN}{dT}}=rN{\Big (}1-{\dfrac {N}{K}}{\Big )}]
where       (   1 &#x2212;    N K      )     {\displaystyle {\Big (}1-{\dfrac
{N}{K}}{\Big )}}  [{\Big (}1-{\dfrac {N}{K}}{\Big )}] is the density
dependence, N is the number in the population, K is the set point for
homeostasis and the carrying capacity. In this logistic_model, population
growth rate is highest at 1/2 K and the population growth rate is zero around
K. The optimum harvesting rate is a close rate to 1/2 K where population will
grow the fastest. Above K, the population growth rate is negative. The logistic
models also show density dependence, meaning the per capita population growth
rates decline as the population density increases. In the wild, you can't get
these patterns to emerge without simplification. Negative density dependence
allows for a population that overshoots the carrying capacity to decrease back
to the carrying capacity, K.[3]
According to r/K_selection_theory organisms may be specialised for rapid
growth, or stability closer to carrying capacity.
**** Discrete time logistical model[edit] ****
          N  t + 1   =  N  t   + r  N  t   ( 1 &#x2212;   N  t    /  K  )
      {\displaystyle N_{t+1}=N_{t}+rN_{t}(1-{N_{t}/K})}  [N_{t+1}=N_{t}+rN_{t}
      (1-{N_{t}/K})]
This equation uses r instead of Î» because per capita growth rate is zero when
r = 0. As r gets very high, there are oscillations and deterministic_chaos.[3]
Deterministic chaos is large changes in population dynamics when there is a
very small change in r. This makes it hard to make predictions at high o values
because a very small r error results in a massive error in population dynamics.
Population is always density dependent. Even a severe density independent event
cannot regulate populate, although it may cause it to go extinct.
Not all population models are necessarily negative density dependent. The Allee
effect allows for a positive correlation between population density and per
capita growth rate in communities with very small populations. For example, a
fish swimming on its own is more likely to be eaten than the same fish swimming
among a school of fish, because the pattern of movement of the school of fish
is more likely to confuse and stun the predator.[3]
**** Individual-based models[edit] ****
Cellular automata are used to investigate mechanisms of population dynamics.
Here are relatively simple models with one and two species.
Logical deterministic individual-based cellular_automata model of single
species population growth
Logical deterministic individual-based cellular_automata model of interspecific
competition for a single limited resource
***** Fisheries and wildlife management[edit] *****
See also: Population_dynamics_of_fisheries and Matrix_population_models
In fisheries and wildlife_management, population is affected by three dynamic
rate functions.
    * Natality or birth_rate, often recruitment, which means reaching a certain
      size or reproductive stage. Usually refers to the age a fish can be
      caught and counted in nets.
    * Population_growth_rate, which measures the growth of individuals in size
      and length. More important in fisheries, where population is often
      measured in biomass.
    * Mortality, which includes harvest mortality and natural mortality.
      Natural mortality includes non-human predation, disease and old age.
If N1 is the number of individuals at time 1 then
                            N  1   =  N  0   + B &#x2212; D + I &#x2212; E
                        {\displaystyle N_{1}=N_{0}+B-D+I-E}  [N_{1}=N_{0}+B-
                        D+I-E]
where N0 is the number of individuals at time 0, B is the number of individuals
born, D the number that died, I the number that immigrated, and E the number
that emigrated between time 0 and time 1.
If we measure these rates over many time intervals, we can determine how a
population's density changes over time. Immigration and emigration are present,
but are usually not measured.
All of these are measured to determine the harvestable surplus, which is the
number of individuals that can be harvested from a population without affecting
long-term population stability or average population size. The harvest within
the harvestable surplus is termed "compensatory" mortality, where the harvest
deaths are substituted for the deaths that would have occurred naturally.
Harvest above that level is termed "additive" mortality, because it adds to the
number of deaths that would have occurred naturally. These terms are not
necessarily judged as "good" and "bad," respectively, in population management.
For example, a fish & game agency might aim to reduce the size of a deer
population through additive mortality. Bucks might be targeted to increase buck
competition, or does might be targeted to reduce reproduction and thus overall
population size.
For the management of many fish and other wildlife populations, the goal is
often to achieve the largest possible long-run sustainable harvest, also known
as maximum_sustainable_yield (or MSY). Given a population dynamic model, such
as any of the ones above, it is possible to calculate the population size that
produces the largest harvestable surplus at equilibrium.[4] While the use of
population dynamic models along with statistics and optimization to set harvest
limits for fish and game is controversial among scientists,[5] it has been
shown to be more effective than the use of human judgment in computer
experiments where both incorrect models and natural resource management
students competed to maximize yield in two hypothetical fisheries.[6][7] To
give an example of a non-intuitive result, fisheries produce more fish when
there is a nearby refuge from human predation in the form of a nature_reserve,
resulting in higher catches than if the whole area was open to fishing.[8][9]
***** For control applications[edit] *****
See also: Evolutionary_game_theory
Population dynamics have been widely used in several control_theory
applications. With the use of evolutionary_game_theory, population games are
broadly implemented for different industrial and daily-life contexts. Mostly
used in multiple-input-multiple-output (MIMO) systems, although they can be
adapted for use in single-input-single-output (SISO) systems. Some examples of
applications are military campaigns, resource allocation for water
distribution, dispatch_of_distributed_generators, lab experiments, transport
problems, communication problems, among others. Furthermore, with the adequate
contextualization of industrial problems, population dynamics can be an
efficient and easy-to-implement solution for control-related problems. Multiple
academic research has been and is continuously carried out.
***** See also[edit] *****
    * Delayed_density_dependence
    * Demography
    * Holocene_extinction
    * Lotka-Volterra_equations
    * Minimum_viable_population
    * Maximum_sustainable_yield
    * NicholsonâBailey_model
    * Overshoot_(population)
    * Pest_insect_population_dynamics
    * Population_cycle
    * Population_dynamics_of_fisheries
    * Population_ecology
    * Population_genetics
    * Population_modeling
    * Ricker_model
    * r/K_selection_theory
    * Sigmoid_curve
    * Societal_collapse
    * System_dynamics
***** References[edit] *****
   1. ^Brotz, Lucas; Cheung, William W. L; Kleisner, Kristin; Pakhomov, Evgeny;
      Pauly, Daniel (2012). "Increasing jellyfish populations: Trends in Large
      Marine Ecosystems". Hydrobiologia. 690 (1): 3â20. doi:10.1007/s10750-
      012-1039-7.
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
   3. ^Jahn, Gary C; Almazan, Liberty P; Pacia, Jocelyn B (2005). "Effect of
      Nitrogen Fertilizer on the Intrinsic Rate of Increase of Hysteroneura
      setariae(Thomas) (Homoptera: Aphididae) on Rice (Oryza sativaL.)".
      Environmental Entomology. 34 (4): 938â43. doi:10.1603/0046-225X-
      34.4.938.
   4. ^ a b c d e f Yang, Louie. Population Dynamics. Davis: UC Davis, 2014.
      [page needed]
   5. ^Clark, Colin (1990). Mathematical bioeconomics : the optimal management
      of renewable resources. New York: Wiley. ISBN 978-0471508830.
   6. [page needed]
   7. ^Finley, C; Oreskes, N (2013). "Maximum sustained yield: A policy
      disguised as science". ICES Journal of Marine Science. 70 (2): 245â50.
      doi:10.1093/icesjms/fss192.
   8. ^Holden, Matthew H; Ellner, Stephen P (2016). "Human judgment vs.
      Quantitative models for the management of ecological resources".
      Ecological Applications. 26 (5): 1553â1565. arXiv:1603.04518. doi:
      10.1890/15-1295. PMID 27755756.
   9. ^Standard, Pacific (2016-03-11). "Sometimes,_Even_Bad_Models_Make_Better
      Decisions_Than_People". Pacific Standard. Retrieved 2017-01-28.
  10. [permanent_dead_link]
  11. ^Chakraborty, Kunal; Das, Kunal; Kar, T. K (2013). "An_ecological
      perspective_on_marine_reserves_in_preyâpredator_dynamics". Journal of
      Biological Physics. 39 (4): 749â76. doi:10.1007/s10867-013-9329-5.
      PMC 3758828. PMID 23949368.
  12. ^Lv, Yunfei; Yuan, Rong; Pei, Yongzhen (2013). "A prey-predator model
      with harvesting for fishery resource with reserve area". Applied
      Mathematical Modelling. 37 (5): 3048â62. doi:10.1016/j.apm.2012.07.030.
***** Further reading[edit] *****
    * Andrey_Korotayev, Artemy Malkov, and Daria Khaltourina. Introduction to
      Social Macrodynamics: Compact Macromodels of the World System Growth.
ISBN 5-484-00414-4
Turchin,_P. 2003. Complex Population Dynamics: a Theoretical/Empirical
Synthesis. Princeton, NJ: Princeton University Press.
Weiss, Volkmar (2007). "The_Population_Cycle_Drives_Human_History_-_from_a
Eugenic_Phase_into_a_Dysgenic_Phase_and_Eventual_Collapse". The Journal of
Social, Political, and Economic Studies. 32 (3): 327â58.
***** External links[edit] *****
    * The_Virtual_Handbook_on_Population_Dynamics. An online compilation of
      state-ot-the-art basic tools for the analysis of population dynamics with
      emphasis on benthic invertebrates.
    * v
    * t
    * e
Human_impact_on_the_environment
               * Environmental_issues
                     o list_of_issues
General        * Human_impact
               * Impact_assessment
               * Planetary_boundaries
               * Agriculture
                     o fishing
                     o irrigation
                     o meat_production
                     o cocoa_production
                     o palm_oil
               * Energy_industry
                     o biofuels
                     o biodiesel
                     o coal
                     o electricity_generation
                     o nuclear_power
                     o oil_shale
                     o petroleum
                     o reservoirs
                     o wind_power
               * Genetic_pollution
               * Industrialisation
               * Land_use
               * Manufacturing
                     o cleaning_agents
                     o concrete
Causes               o plastics
                     o nanotechnology
                     o paint
                     o paper
                     o pesticides
                     o pharmaceuticals_and_personal_care
               * Mining
               * Overdrafting
               * Overfishing
               * Overgrazing
               * Overexploitation
               * Overpopulation
               * Particulates
               * Pollution
               * Quarrying
               * Reservoirs
               * Tourism
               * Transport
                     o aviation
                     o roads
                     o shipping                          [Planetary_boundaries]
               * Urbanization
                     o urban_sprawl
               * War
               * Biodiversity_threats
                     o biodiversity_loss
                     o decline_in_amphibian_populations
                     o decline_in_insect_populations
               * Climate_change
                     o global_warming
                     o runaway_climate_change
               * Coral_reefs
               * Deforestation
               * Defaunation
               * Desertification
               * Ecocide
               * Erosion
Effects        * Environmental_degradation
               * Freshwater_cycle
               * Habitat_destruction
               * Holocene_extinction
               * Nitrogen_cycle
               * Land_degradation
               * Land_consumption
               * Land_surface_effects_on_climate
               * Loss_of_green_belts
               * Phosphorus_cycle
               * Ocean_acidification
               * Ozone_depletion
               * Resource_depletion
               * Water_degradation
               * Water_scarcity
               * Birth_control
               * Cleaner_production
               * Climate_change_mitigation
               * Climate_engineering
               * Community_resilience
               * Decoupling
               * Ecological_engineering
               * Environmental_engineering
Mitigation     * Environmental_mitigation
               * Industrial_ecology
               * Mitigation_banking
               * Organic_farming
               * Reforestation
                     o urban
               * Restoration_ecology
               * Sustainable_consumption
               * Waste_minimization
    *  [Commons page] Commons
    *  [Category] Category
    * by_country
    * assessment
    * mitigation
    * v
    * t
    * e
Global_human_population
                    * Biocapacity
                    * Optimum_population
                    * Overpopulation
                          o Malthusian_catastrophe
Major topics        * Population
                    * Population_ethics
                    * Population_momentum
                    * Sustainable_development
                    * Women's_reproductive_rights
                    * Zero_population_growth
                    * Family_planning
                          o Pledge_two_or_fewer
                    * Human_population_planning
                          o One-child_policy
                          o Two-child_policy
                    * Population_biology
Biological and      * Population_decline
related topics      * Population_density
                          o Physiological_density
                    * Population dynamics
                    * Population_growth
                    * Population_model
                    * Population_pyramid
                    * Projections_of_population_growth
                    * Deforestation
                    * Desalination
                    * Desertification
                    * Environmental_impact
                          o of_agriculture
                          o of_aviation
                          o of_biodiesel
                          o of_concrete
                          o of_electricity_generation
                          o of_the_energy_industry
                          o of_fishing
                          o of_irrigation
                          o of_mining
                          o of_off-roading
                          o of_oil_shale_industry
Human_impact_on           o of_palm_oil
the_environment           o of_paper
                          o of_the_petroleum_industry
                          o of_reservoirs
                          o of_shipping
                          o of_war
                    * Industrialisation
                    * Land_degradation
                    * Land_reclamation
                    * Overconsumption
                    * Pollution
                    * Quarrying
                    * Urbanization
                          o Loss_of_green_belts
                          o Urban_sprawl
                    * Waste
                    * Water_scarcity
                          o Overdrafting
                    * Carrying_capacity
                    * Deep_ecology
                    * Earth's_energy_budget
                    * Food_security
                    * Habitat_destruction
Population          * I_=_P_Ã_Aâ_Ã_T
ecology             * Kaya_identity
                    * Malthusian_growth_model
                    * Overshoot_(population)
                    * World_energy_consumption
                    * World_energy_resources
                    * World3_model
                    * A_Modest_Proposal
                    * Observations_Concerning_the_Increase_of_Mankind,_Peopling
                      of_Countries,_etc.
                    * An_Essay_on_the_Principle_of_Population
                    * "How_Much_Land_Does_a_Man_Need?"
Literature          * Operating_Manual_for_Spaceship_Earth
                    * Population_Control:_Real_Costs,_Illusory_Benefits
                    * The_Limits_to_Growth
                    * The_Population_Bomb
                    * The_Skeptical_Environmentalist
                    * The_Ultimate_Resource
Publications        * Population_and_Environment
                    * Population_and_Development_Review
                    * Population_and_housing_censuses_by_country
Lists               * Metropolitan_areas_by_population
                    * Population_milestone_babies
                    * 7_Billion_Actions
                    * Extinction_Rebellion
                    * International_Conference_on_Population_and_Development
                    * Population_Action_International
Events and          * Population_Connection
organizations       * Population_Matters
                    * Population_Research_Institute
                    * United_Nations_Population_Fund
                    * Voluntary_Human_Extinction_Movement
                    * World_Population_Day
                    * World_Population_Foundation
                    * Classic_Maya_collapse
                    * Fertility_and_intelligence
Related topics      * Green_Revolution
                    * Holocene_extinction
                    * Migration
    * [Commons page] Commons
    * [Category] Human_overpopulation
    * Human_activities_with_impact_on_the_environment
    * Human_migration
    * v
    * t
    * e
Lists_of_countries by population_statistics
Global                   * Current_population
                         * Africa
                         * Asia
                         * Europe
(Sub-)continents         * North_America
                               o Caribbean
                         * Oceania
                         * South_America
                         * Americas
                         * Arab_world
                         * Commonwealth_of_Nations
Intercontinental         * Eurasia
                         * European_Union
                         * Islands
                         * Latin_America
                         * Middle_East
                         * National_capitals
                         * Cities_proper
Cities/urban regions     * Metropolitan_areas
                         * Urban_areas
                         * Megacities
                         * Megalopolises
                         * Past_and_future_population
                         * World_population_estimates
                         * 0
                         * 1
                         * 1000
                         * 1500
                         * 1600
                         * 1700
Past and future          * 1800
                         * 1900
                         * 1907
                         * 1939
                         * 1989
                         * 2000
                         * 2005
                         * 2010
                         * Population_milestones
                         * Current_density
Population_density       * Past_and_future_population_density
                         * Current_real_density_based_on_food_growing_capacity
                         * Population_growth_rate
                         * Natural_increase
Growth indicators        * Birth_rate
                         * Mortality_rate
                         * Fertility_rate
                         * Past_fertility_rate
                         * Age_at_first_marriage
                         * Age_structure
                         * Dependency_ratio
                         * Divorce_rate
                         * Ethnic_and_cultural_diversity_level
Other                    * Immigrant_population
demographics             * Linguistic_diversity
                         * Median_age
                         * Net_migration_rate
                         * Number_of_households
                         * Sex_ratio
                         * Urban_population
                         * Urbanization
                         * Antidepressant_consumption
                         * Antiviral_medications_for_pandemic_influenza
                         * HIV/AIDS_adult_prevalence_rate
                         * Infant_and_under-five_mortality_rates
                         * Maternal_mortality_rate
Health                   * Life_expectancy
                         * Past_life_expectancy
                         * Percentage_suffering_from_undernourishment
                         * Health_expenditure_covered_by_government
                         * Suicide_rate
                         * Total_health_expenditure_per_capita
                         * Body_Mass_Index_(BMI)
                         * Bloomberg_Innovation_Index
                         * Education_Index
                         * International_Innovation_Index
                         * Innovation_Union_Scoreboard
                         * Literacy_rate
                         * Programme_for_the_International_Assessment_of_Adult
Education                  Competencies
and innovation           * Progress_in_International_Reading_Literacy_Study
                         * Student_skills
                         * Tertiary_education_attainment
                         * Trends_in_International_Mathematics_and_Science
                           Study
                         * Women's_average_years_in_school
                         * World_Intellectual_Property_Indicators
                         * Development_aid_given
                               o Official_Development_Assistance_received
                         * Employment_rate
                         * Irrigated_land_area
                         * Human_Development_Index
                               o by_country
                               o inequality-adjusted
                         * Human_Poverty_Index
Economic                 * Imports
                         * Income_equality
                         * Labour_force
                         * Number_of_millionaires_(US_dollars)
                         * Number_of_billionaires_(US_dollars)
                         * Percentage_living_in_poverty
                         * Public_sector
                         * Sen_social_welfare_function
                         * Unemployment_rate
    * List_of_international_rankings
    * List_of_top_international_rankings_by_country
    * Lists_by_country
    * v
    * t
    * e
Hierarchy_of_life
    * Biosphere > Biome > Ecosystem > Biocenosis > Population > Organism >
      Organ_system > Organ > Tissue > Cell > Organelle > Biomolecular
      complex > Macromolecule > Biomolecule

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Population_dynamics&oldid=907604442"
Categories:
    * Fisheries_science
    * Human_overpopulation
    * Population_ecology
    * Environmental_controversies
    * Population_models
    * Social_dynamics
Hidden categories:
    * Wikipedia_articles_needing_page_number_citations_from_November_2017
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_December_2017
    * Articles_with_permanently_dead_external_links
    * Articles_lacking_in-text_citations_from_July_2012
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * CatalÃ 
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * á¥áá áá£áá
    * Magyar
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Suomi
    * Svenska
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 24 July 2019, at 01:40 (UTC).
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
