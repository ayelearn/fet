The following text has been accessed from https://en.wikipedia.org/wiki/Data_assimilation at Fri Aug 9 01:58:18 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Data assimilation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article has multiple issues. Please help improve_it or discuss these issues on the talk_page.
 (Learn_how_and_when_to_remove_these_template_messages)
  This article needs additional citations for verification. Please help improve_this_article by adding_citations_to
  reliable_sources. Unsourced material may be challenged and removed.
  Find sources: "Data_assimilation" â news Â· newspapers Â· books Â· scholar Â· JSTOR (September 2011)(Learn_how
  and_when_to_remove_this_template_message)
  This article may be confusing_or_unclear to readers. In particular, complicated jargon is used
  throughout, lacking explanation. Please help us clarify_the_article. There might be a discussion
  about this on the_talk_page. (October 2013)(Learn_how_and_when_to_remove_this_template_message)
 (Learn_how_and_when_to_remove_this_template_message)
Data assimilation is a mathematical discipline that seeks to optimally combine
theory (usually in the form of a numerical model) with observations. There may
be a number of different goals sought, for exampleâto determine the optimal
state estimate of a system, to determine initial conditions for a numerical
forecast model, to interpolate sparse observation data using (e.g. physical)
knowledge of the system being observed, to train numerical model parameters
based on observed data. Depending on the goal, different solution methods may
be used. Data assimilation is distinguished from other forms of machine
learning, image analysis, and statistical methods in that it utilizes a
dynamical model of the system being analyzed.
Data assimilation initially developed in the field of numerical_weather
prediction. Numerical weather prediction models are equations describing the
dynamical behavior of the atmosphere, typically coded into a computer program.
In order to use these models to make forecasts, initial conditions are needed
for the model that closely resemble the current state of the atmosphere. Simply
inserting point-wise measurements into the numerical models did not provide a
satisfactory solution. Real world measurements contain errors both due to the
quality of the instrument and how accurately the position of the measurement is
known. These errors can cause instabilities in the models that eliminate any
level of skill in a forecast. Thus, more sophisticated methods were needed in
order to initialize a model using all available data while making sure to
maintain stability in the numerical model. Such data typically includes the
measurements as well as a previous forecast valid at the same time the
measurements are made. If applied iteratively, this process begins to
accumulate information from past observations into all subsequent forecasts.
Because data assimilation developed out of the field of numerical weather
prediction, it initially gained popularity amongst the geosciences. In fact,
one of the most cited publication in all of the geosciences is an application
of data assimilation to reconstruct the observed history of the atmosphere.[1]
⁰
***** Contents *****
    * 1_Details_of_the_Data_Assimilation_Process
    * 2_Data_assimilation_as_statistical_estimation
    * 3_Weather_forecasting_applications
          o 3.1_Why_it_is_necessary
          o 3.2_History
          o 3.3_Cost_function
                # 3.3.1_3D-Var
                # 3.3.2_4D-Var
          o 3.4_Future_development
    * 4_Other_applications
          o 4.1_Monitoring_water_and_energy_transfers
          o 4.2_Other_forecasting_applications
    * 5_References
    * 6_Further_reading
    * 7_External_links
***** Details of the Data Assimilation Process[edit] *****
Classically, data assimilation has been applied to chaotic dynamical systems
that are too difficult to predict using simple extrapolation methods. The cause
of this difficulty is that small changes in initial conditions can lead to
large changes in prediction accuracy. This is sometimes known as the butterfly
effect â the sensitive dependence on initial_conditions in which a small
change in one state of a deterministic nonlinear_system can result in large
differences in a later state.
At any update time, data assimilation usually takes a forecast (also known as
the first guess, or background information) and applies a correction to the
forecast based on a set of observed data and estimated errors that are present
in both the observations and the forecast itself. The difference between the
forecast and the observations at that time is called the departure or the
innovation (as it provides new information to the data assimilation process). A
weighting factor is applied to the innovation to determine how much of a
correction should be made to the forecast based on the new information from the
observations. The best estimate of the state of the system based on the
correction to the forecast determined by a weighting factor times the
innovation is called the analysis. In one dimension, computing the analysis
could be as simple as forming a weighted average of a forecasted and observed
value. In multiple dimensions the problem becomes more difficult. Much of the
work in data assimilation is focused on adequately estimating the appropriate
weighting factor based on intricate knowledge of the errors in the system.
The measurements are usually made of a real-world system, rather than of the
model's incomplete representation of that system, and so a special function
called the observation operator (usually depicted by h() for a nonlinear
operator or H for its linearization) is needed to map the modeled variable to a
form that can be directly compared with the observation.
***** Data assimilation as statistical estimation[edit] *****
One of the common mathematical philosophical perspectives is to view data
assimilation as a Bayesian estimation problem. From this perspective, the
analysis step is an application of Bayes'_theorem and the overall assimilation
procedure is an example of recursive_Bayesian_estimation. However, the
probabilistic analysis is usually simplified to a computationally feasible
form. Advancing the probability distribution in time would be done exactly in
the general case by the Fokker-Planck_equation, but that is not feasible for
high-dimensional systems, so various approximations operating on simplified
representations of the probability distributions are used instead. Often the
probability distributions are assumed Gaussian so that they can be represented
by their mean and covariance, which gives rise to the Kalman_filter.
Many methods represent the probability distributions only by the mean and input
some pre-calculated covariance. An example of a direct (or sequential) method
to compute this is called optimal statistical interpolation, or simply optimal
interpolation (OI). An alternative approach is to iteratively solve a cost
function that solves an identical problem. These are called variational
methods, such as 3D-Var and 4D-Var. Typical minimization algorithms are the
Conjugate_gradient_method or the Generalized_minimal_residual_method. The
Ensemble_Kalman_filter is sequential method that uses a Monte Carlo approach to
estimate both the mean and the covariance of a Gaussian probability
distribution by an ensemble of simulations. More recently, hybrid combinations
of ensemble approaches and variational methods have become more popular (e.g.
they are used for operational forecasts both at the European Centre for Medium-
Range Weather Forecasts (ECMWF) and at the NOAA National Centers for
Environmental Prediction (NCEP)).
***** Weather forecasting applications[edit] *****
In numerical weather prediction applications, data assimilation is most widely
known as a method for combining observations of meteorological variables such
as temperature and atmospheric_pressure with prior forecasts in order to
initialize numerical forecast models.
**** Why it is necessary[edit] ****
The atmosphere is a fluid. The idea of numerical weather prediction is to
sample the state of the fluid at a given time and use the equations of fluid
dynamics and thermodynamics to estimate the state of the fluid at some time in
the future. The process of entering observation data into the model to generate
initial_conditions is called initialization. On land, terrain maps available at
resolutions down to 1 kilometer (0.6 mi) globally are used to help model
atmospheric circulations within regions of rugged topography, in order to
better depict features such as downslope winds, mountain_waves and related
cloudiness that affects incoming solar radiation.[2] The main inputs from
country-based weather services are observations from devices (called
radiosondes) in weather balloons that measure various atmospheric parameters
and transmits them to a fixed receiver, as well as from weather_satellites. The
World_Meteorological_Organization acts to standardize the instrumentation,
observing practices and timing of these observations worldwide. Stations either
report hourly in METAR reports,[3] or every six hours in SYNOP reports.[4]
These observations are irregularly spaced, so they are processed by data
assimilation and objective analysis methods, which perform quality control and
obtain values at locations usable by the model's mathematical algorithms.[5]
Some global models use finite_differences, in which the world is represented as
discrete points on a regularly spaced grid of latitude and longitude;[6] other
models use spectral_methods that solve for a range of wavelengths. The data are
then used in the model as the starting point for a forecast.[7]
A variety of methods are used to gather observational data for use in numerical
models. Sites launch radiosondes in weather balloons which rise through the
troposphere and well into the stratosphere.[8] Information from weather
satellites is used where traditional data sources are not available. Commerce
provides pilot_reports along aircraft routes[9] and ship reports along shipping
routes.[10] Research projects use reconnaissance_aircraft to fly in and around
weather systems of interest, such as tropical_cyclones.[11][12] Reconnaissance
aircraft are also flown over the open oceans during the cold season into
systems which cause significant uncertainty in forecast guidance, or are
expected to be of high impact from three to seven days into the future over the
downstream continent.[13] Sea ice began to be initialized in forecast models in
1971.[14] Efforts to involve sea_surface_temperature in model initialization
began in 1972 due to its role in modulating weather in higher latitudes of the
Pacific.[15]
**** History[edit] ****
Lewis Fry Richardson
In 1922, Lewis_Fry_Richardson published the first attempt at forecasting the
weather numerically. Using a hydrostatic variation of Bjerknes's primitive
equations,[16] Richardson produced by hand a 6-hour forecast for the state of
the atmosphere over two points in central Europe, taking at least six weeks to
do so.[17] His forecast calculated that the change in surface_pressure would be
145 millibars (4.3 inHg), an unrealistic value incorrect by two orders of
magnitude. The large error was caused by an imbalance in the pressure and wind
velocity fields used as the initial conditions in his analysis,[16] indicating
the need for a data assimilation scheme.
Originally "subjective analysis" had been used in which NWP forecasts had been
adjusted by meteorologists using their operational expertise. Then "objective
analysis" (e.g. Cressman algorithm) was introduced for automated data
assimilation. These objective methods used simple interpolation approaches, and
thus were 3DDA methods.
Later, 4DDA methods, called "nudging", were developed, such as in the MM5
model. They are based on the simple idea of Newtonian relaxation (the 2nd axiom
of Newton). They introduce into the right part of dynamical equations of the
model a term that is proportional to the difference of the calculated
meteorological variable and the observed value. This term that has a negative
sign keeps the calculated state_vector closer to the observations. Nudging can
be interpreted as a variant of the Kalman-Bucy_filter (a continuous time
version of the Kalman_filter) with the gain matrix prescribed rather than
obtained from covariances.[citation_needed]
A major development was achieved by L. Gandin (1963) who introduced the
"statistical interpolation" (or "optimal interpolation") method, which
developed earlier ideas of Kolmogorov. This is a 3DDA method and is a type of
regression_analysis which utilizes information about the spatial distributions
of covariance functions of the errors of the "first guess" field (previous
forecast) and "true field". These functions are never known. However, the
different approximations were assumed.[citation_needed]
The optimal interpolation algorithm is the reduced version of the Kalman
filtering (KF) algorithm and in which the covariance matrices are not
calculated from the dynamical equations but are pre-determined in advance.
Attempts to introduce the KF algorithms as a 4DDA tool for NWP models came
later. However, this was (and remains) a difficult task because the full
version requires solution of the enormous number of additional equations
(~N*N~10**12, where N=Nx*Ny*Nz is the size of the state vector, Nx~100, Ny~100,
Nz~100 â the dimensions of the computational grid). To overcome this
difficulty, approximate or suboptimal Kalman filters were developed. These
include the Ensemble_Kalman_filter and the Reduced-Rank Kalman filters
(RRSQRT).[18]
Another significant advance in the development of the 4DDA methods was
utilizing the optimal_control theory (variational approach) in the works of Le
Dimet and Talagrand (1986), based on the previous works of G. Marchuk, who was
the first to apply that theory in the environmental modeling. The significant
advantage of the variational approaches is that the meteorological fields
satisfy the dynamical equations of the NWP model and at the same time they
minimize the functional, characterizing their difference from observations.
Thus, the problem of constrained minimization is solved. The 3DDA variational
methods were developed for the first time by Sasaki (1958).
As was shown by Lorenc (1986), all the above-mentioned 4DDA methods are in some
limit equivalent, i.e. under some assumptions they minimize the same cost
function. However, in practical applications these assumptions are never
fulfilled, the different methods perform differently and generally it is not
clear what approach (Kalman filtering or variational) is better. The
fundamental questions also arise in application of the advanced DA techniques
such as convergence of the computational method to the global minimum of the
functional to be minimised. For instance, cost function or the set in which the
solution is sought can be not convex. The 4DDA method which is currently most
successful[19][20] is hybrid incremental 4D-Var, where an ensemble is used to
augment the climatological background error covariances at the start of the
data assimilation time window, but the background error covariances are evolved
during the time window by a simplified version of the NWP forecast model. This
data assimilation method is used operationally at forecast centres such as the
Met_Office.[21][22]
**** Cost function[edit] ****
The process of creating the analysis in data assimilation often involves
minimization of a cost_function. A typical cost function would be the sum of
the squared deviations of the analysis values from the observations weighted by
the accuracy of the observations, plus the sum of the squared deviations of the
forecast fields and the analyzed fields weighted by the accuracy of the
forecast. This has the effect of making sure that the analysis does not drift
too far away from observations and forecasts that are known to usually be
reliable.[citation_needed]
*** 3D-Var[edit] ***
   J (  x  ) = (  x  &#x2212;   x   b    )   T      B   &#x2212; 1   (  x
&#x2212;   x   b   ) + (  y  &#x2212;   H   [  x  ]  )   T      R   &#x2212; 1
(  y  &#x2212;   H   [  x  ] ) ,   {\displaystyle J(\mathbf {x} )=(\mathbf {x}
-\mathbf {x} _{b})^{\mathrm {T} }\mathbf {B} ^{-1}(\mathbf {x} -\mathbf {x} _
{b})+(\mathbf {y} -{\mathit {H}}[\mathbf {x} ])^{\mathrm {T} }\mathbf {R} ^{-1}
(\mathbf {y} -{\mathit {H}}[\mathbf {x} ]),}  [J({\mathbf  {x}})=({\mathbf
{x}}-{\mathbf  {x}}_{{b}})^{{{\mathrm  {T}}}}{\mathbf  {B}}^{{-1}}({\mathbf
{x}}-{\mathbf  {x}}_{{b}})+({\mathbf  {y}}-{\mathit  {H}}[{\mathbf  {x}}])^{{
{\mathrm  {T}}}}{\mathbf  {R}}^{{-1}}({\mathbf  {y}}-{\mathit  {H}}[{\mathbf
{x}}]),]
where      B    {\displaystyle \mathbf {B} }  [\mathbf {B} ] denotes the
background error covariance,      R    {\displaystyle \mathbf {R} }  [\mathbf
{R} ] the observational error covariance.
   &#x2207; J (  x  ) = 2   B   &#x2212; 1   (  x  &#x2212;   x   b   )
&#x2212; 2    H    T     R   &#x2212; 1   (  y  &#x2212;   H   [  x  ] )
{\displaystyle \nabla J(\mathbf {x} )=2\mathbf {B} ^{-1}(\mathbf {x} -\mathbf
{x} _{b})-2{\mathit {H}}^{T}\mathbf {R} ^{-1}(\mathbf {y} -{\mathit {H}}
[\mathbf {x} ])}  [\nabla J({\mathbf  {x}})=2{\mathbf  {B}}^{{-1}}({\mathbf
{x}}-{\mathbf  {x}}_{{b}})-2{\mathit  {H}}^{T}{\mathbf  {R}}^{{-1}}({\mathbf
{y}}-{\mathit  {H}}[{\mathbf  {x}}])]
*** 4D-Var[edit] ***
   J (  x  ) = (  x  &#x2212;   x   b    )   T      B   &#x2212; 1   (  x
&#x2212;   x   b   ) +  &#x2211;  i = 0   n   (   y   i   &#x2212;    H    i
[   x   i   ]  )   T      R   i   &#x2212; 1   (   y   i   &#x2212;    H    i
[   x   i   ] )   {\displaystyle J(\mathbf {x} )=(\mathbf {x} -\mathbf {x} _
{b})^{\mathrm {T} }\mathbf {B} ^{-1}(\mathbf {x} -\mathbf {x} _{b})+\sum _
{i=0}^{n}(\mathbf {y} _{i}-{\mathit {H}}_{i}[\mathbf {x} _{i}])^{\mathrm {T}
}\mathbf {R} _{i}^{-1}(\mathbf {y} _{i}-{\mathit {H}}_{i}[\mathbf {x} _{i}])}
[J({\mathbf  {x}})=({\mathbf  {x}}-{\mathbf  {x}}_{{b}})^{{{\mathrm  {T}}}}
{\mathbf  {B}}^{{-1}}({\mathbf  {x}}-{\mathbf  {x}}_{{b}})+\sum _{{i=0}}^{{n}}(
{\mathbf  {y}}_{{i}}-{\mathit  {H}}_{{i}}[{\mathbf  {x}}_{{i}}])^{{{\mathrm
{T}}}}{\mathbf  {R}}_{{i}}^{{-1}}({\mathbf  {y}}_{{i}}-{\mathit  {H}}_{{i}}[
{\mathbf  {x}}_{{i}}])]
provided that       H     {\displaystyle {\mathit {H}}}  [{\mathit  {H}}] is a
linear operator (matrix).
**** Future development[edit] ****
Factors driving the rapid development of data assimilation methods for NWP
models include:
    * Utilizing the observations currently offers promising improvement in
      forecast_skill at a variety of spatial scales (from global to highly
      local) and time scales.
    * The number of different kinds of available observations (sodars, radars,
      satellite) is rapidly growing.
[[icon]] This section needs expansion. You can help by adding_to_it. (June
         2008)
***** Other applications[edit] *****
[[icon]] This section needs expansion. You can help by adding_to_it. (June
         2008)
**** Monitoring water and energy transfers[edit] ****
General Data Assimilation diagram (Alpilles-ReSeDA)[23]
Data assimilation has been used, in the 1980s and 1990s, in several HAPEX
(Hydrologic and Atmospheric Pilot Experiment) projects for monitoring energy
transfers between the soil, vegetation and atmosphere. For instance:
- HAPEX-MobilHy,[24] HAPEX-Sahel,[25]
- the "Alpilles-ReSeDA" (Remote Sensing Data Assimilation) experiment[26][27],
a European project in the FP4-ENV program[28] which took place in the Alpilles
region, South-East of France (1996â97). The Flow-chart diagram (right),
excerpted from the final report of that project[23], shows how to infer
variables of interest such as canopy state, radiative fluxes, environmental
budget, production in quantity and quality, from remote sensing data and
ancillary information. In that diagram, the small blue-green arrows indicate
the direct way the models actually run.[citation_needed][29]
**** Other forecasting applications[edit] ****
Data assimilation methods are currently also used in other environmental
forecasting problems, e.g. in hydrological forecasting. Basically, the same
types of data assimilation methods as those described above are in use there.
An example of chemical data assimilation using Autochem can be found at
CDACentral.[citation_needed]
Given the abundance of spacecraft data for other planets in the solar system,
data assimilation is now also applied beyond the Earth to obtain re-analyses of
the atmospheric state of extraterrestrial planets. Mars is the only
extraterrestrial planet to which data assimilation has been applied so far.
Available spacecraft data include, in particular, retrievals of temperature and
dust/water ice optical ticknesses from the Thermal_Emission_Spectrometer
onboard NASA's Mars_Global_Surveyor and the Mars Climate Sounder onboard NASA's
Mars_Reconnaissance_Orbiter. Two methods of data assimilation have been applied
to these datasets: an Analysis Correction scheme [30] and two Ensemble Kalman
Filter schemes,[31][32] both using a global circulation model of the martian
atmosphere as forward model. The Mars Analysis Correction Data Assimilation
(MACDA) dataset is publicly available from the British Atmospheric Data Centre.
[33]
Data assimilation is a part of the challenge for every forecasting problem.
Dealing with biased data is a serious challenge in data assimilation. Further
development of methods to deal with biases will be of particular use. If there
are several instruments observing the same variable then intercomparing them
using probability_distribution_functions can be instructive.[citation_needed]
The numerical forecast models are becoming of higher resolution due to the
increase of computational_power, with operational atmospheric models now
running with horizontal resolutions of order of 1 km (e.g. at the German
National Meteorological Service, the Deutscher_Wetterdienst_(DWD) and Met
Office in the UK). This increase in horizontal resolutions is starting to allow
us to resolve more chaotic features of our non-linear models, e.g. resolve
convection on the grid scale, clouds, in the atmospheric models. This
increasing non-linearity in the models and observation_operators poses a new
problem in the data assimilation. The existing data assimilation methods such
as many variants of ensemble_Kalman_filters and variational methods, well
established with linear or near-linear models, are being assessed on non-linear
models, as well as many new methods are being developed e.g. particle_filters
for high-dimensional problems, hybrids data assimilation methods.[34]
Other uses include trajectory estimation for the Apollo_program, GPS, and
atmospheric_chemistry.
***** References[edit] *****
   1. ^Kalnay, Eugenia; and coauthors (1996). "The NCEP/NCAR 40-Year Reanalysis
      Project". BAMS. 77 (March): 437. Bibcode:1996BAMS...77..437K. doi:
      10.1175/1520-0477(1996)077<0437:TNYRP>2.0.CO;2.
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
   3. ^Stensrud, David J. (2007). Parameterization_schemes:_keys_to
      understanding_numerical_weather_prediction_models. Cambridge University
      Press. p. 56. ISBN 978-0-521-86540-1.
   4. ^National_Climatic_Data_Center (2008-08-20). "Key_to_METAR_Surface
      Weather_Observations". National_Oceanic_and_Atmospheric_Administration.
      Retrieved 2011-02-11.
   5. ^"SYNOP_Data_Format_(FM-12):_Surface_Synoptic_Observations". UNISYS.
      2008-05-25. Archived from the_original on 2007-12-30.
   6. ^Krishnamurti, T N (1995). "Numerical Weather Prediction". Annual Review
      of Fluid Mechanics. 27: 195â225. Bibcode:1995AnRFM..27..195K. doi:
      10.1146/annurev.fl.27.010195.001211.
   7. ^Chaudhari, H. S.; Lee, K. M.; Oh, J. H. (2007). "Weather_prediction_and
      computational_aspects_of_icosahedral-hexagonal_gridpoint_model_GME". In
      Kwon, Jang-Hyuk; Periaux, Jacques; Fox, Pat; Satofuka, N.; Ecer, A.
      (eds.). Parallel computational fluid dynamics: parallel computings and
      its applications : proceedings of the Parallel CFD 2006 Conference, Busan
      city, Korea (May 15â18, 2006). Elsevier. pp. 223â30. ISBN 978-0-444-
      53035-6. Retrieved 2011-01-06.
   8. ^"The_WRF_Variational_Data_Assimilation_System_(WRF-Var)". University
      Corporation_for_Atmospheric_Research. 2007-08-14. Archived from the
      original on 2007-08-14.
   9. ^Gaffen, Dian J. (2007-06-07). "Radiosonde_Observations_and_Their_Use_in
      SPARC-Related_Investigations". Archived from the_original on 2007-06-07.
  10. ^Ballish, Bradley A; Kumar, V. Krishna (2008). "Systematic Differences in
      Aircraft and Radiosonde Temperatures". Bulletin of the American
      Meteorological Society. 89 (11): 1689. Bibcode:2008BAMS...89.1689B. doi:
      10.1175/2008BAMS2332.1.
  11. ^National Data Buoy Center (2009-01-28). "The_WMO_Voluntary_Observing
      Ships_(VOS)_Scheme". National_Oceanic_and_Atmospheric_Administration.
      Retrieved 2011-02-15.
  12. ^403rd Wing (2011). "The_Hurricane_Hunters". 53rd_Weather_Reconnaissance
      Squadron. Retrieved 2006-03-30.
  13. ^Lee, Christopher (2007-10-08). "Drone,_Sensors_May_Open_Path_Into_Eye_of
      Storm". The Washington Post. Retrieved 2008-02-22.
  14. ^National_Oceanic_and_Atmospheric_Administration (2010-11-12). "NOAA
      Dispatches_High-Tech_Research_Plane_to_Improve_Winter_Storm_Forecasts".
      Retrieved 2010-12-22.
  15. ^Stensrud, David J. (2007). Parameterization_schemes:_keys_to
      understanding_numerical_weather_prediction_models. Cambridge_University
      Press. p. 137. ISBN 978-0-521-86540-1.
  16. ^Houghton, John Theodore (1985). The_Global_Climate. Cambridge University
      Press archive. pp. 49â50. ISBN 978-0-521-31256-1.
  17. ^ a bLynch, Peter (2008). "The_origins_of_computer_weather_prediction_and
      climate_modeling". Journal of Computational Physics. 227 (7):
      3431â3444. Bibcode:2008JCoPh.227.3431L. doi:10.1016/j.jcp.2007.02.034.
  18. ^Lynch, Peter (2006). "Weather Prediction by Numerical Process". The
      Emergence of Numerical Weather Prediction. Cambridge_University_Press.
      pp. 1â27. ISBN 978-0-521-85729-1.
  19. ^ Todling and Cohn, 1994[full_citation_needed]
  20. ^"Abstract:_Mesoscale_ensemble_4DVAR_and_its_comparison_with_EnKF_and
      4DVAR_(91st_American_Meteorological_Society_Annual_Meeting)".
  21. ^ http://hfip.psu.edu/EDA2010/MZhang.pdf
  22. ^Barker, Dale; Lorenc, Andrew; Clayton, Adam (September 2011). "Hybrid
      Variational/Ensemble_Data_Assimilation" (PDF).
  23. ^ http://www.metoffice.gov.uk/research/modelling-systems/unified-model/
      weather-forecasting[full_citation_needed]
  24. ^ a bBaret, Frederic (June 2000). "ReSeDA:_Assimilation_of_Multi-Sensor_&
      Multi-Temporal_Remote_Sensing_Data_to_Monitor_Soil_&_Vegetation
      Functioning" (PDF) (final report, European contract number ENV4CT960326).
      Avignon: Institut_national_de_la_recherche_agronomique. p. 59. Retrieved
      8 July 2019.
  25. ^AndrÃ©, Jean-Claude; Goutorbe, Jean-Paul; Perrier, Alain (1986).
      "HAPEXâMOBLIHY: A Hydrologic Atmospheric Experiment for the Study of
      Water Budget and Evaporation Flux at the Climatic Scale". Bulletin of the
      American Meteorological Society. 67 (2): 138. Bibcode:
      1986BAMS...67..138A. doi:10.1175/1520-0477(1986)067<0138:HAHAEF>2.0.CO;2.
  26. ^Goutorbe, J.P; Lebel, T; Dolman, A.J; Gash, J.H.C; Kabat, P; Kerr, Y.H;
      Monteny, B; Prince, S.D; Stricker, J.N.M; Tinga, A; Wallace, J.S (1997).
      "An overview of HAPEX-Sahel: A study in climate and desertification".
      Journal of Hydrology. 188-189: 4â17. Bibcode:1997JHyd..188....4G. doi:
      10.1016/S0022-1694(96)03308-2.
  27. ^Prevot L, Baret F, Chanzy A, Olioso A, Wigneron JP, Autret H, Baudin F,
      Bessemoulin P, Bethenod O, Blamont D, Blavoux B, Bonnefond JM, Boubkraoui
      S, Bouman BA, Braud I, Bruguier N, Calvet JC, Caselles V, Chauki H,
      Clevers JG, Coll C, Company A, Courault D, Dedieu G, Degenne P, Delecolle
      R, Denis H, Desprats JF, Ducros Y, Dyer D, Fies JC, Fischer A, Francois
      C, Gaudu JC, Gonzalez E, Goujet R, Gu XF, Guerif M, Hanocq JF, Hautecoeur
      O, Haverkamp R, Hobbs S, Jacob F, Jeansoulin R, Jongschaap RE, Kerr Y,
      King C, Laborie P, Lagouarde JP, Laques AE, et al. (July 1998).
      "Assimilation_of_Multi-Sensor_and_Multi-Temporal_Remote_Sensing_Data,_to
      Monitor_Vegetation_and_Soil:_the_Alpilles-ReSeDA_project" (pdf). Seattle,
      WA, USA: IGARSS'98, International Geoscience and Remote Sensing
      Symposium. Retrieved 8 July 2019.
  28. ^Eibl, B; Mauser, W; Moulin, S; Noilhan, J; Ottle, C; Paloscia, S;
      Pampaloni, P; Podvin, T; Quaracino, F; Roujean, J.L; Rozier, C; Ruisi, R;
      Susini, C; Taconet, O; Tallet, N; Thony, J.L; Travi, Y; Van Leewen, H;
      Vauclin, M; Vidal-Madjar, D; Vonder, O.W (1998). "Comparison of the
      albedo derived from MOS-B and WIFS with NOAA-AVHRR". IGARSS '98. Sensing
      and Managing the Environment. 1998 IEEE International Geoscience and
      Remote Sensing. Symposium Proceedings. (Cat. No.98CH36174). pp. 2402â4.
      doi:10.1109/IGARSS.1998.702226. ISBN 978-0-7803-4403-7.
  29. ^"ReSeDA". cordis.europa.eu. Retrieved 8 July 2019.
  30. ^Olioso A, Prevot L, Baret F, Chanzy A, Braud I, Autret H, Baudin F,
      Bessemoulin P, Bethenod O, Blamont D, Blavoux B, Bonnefond JM, Boubkraoui
      S, Bouman BA, Bruguier N, Calvet JC, Caselles V, Chauki H, Clevers JW,
      Coll C, Company A, Courault D, Dedieu G, Degenne P, Delecolle R, Denis H,
      Desprats JF, Ducros Y, Dyer D, Fies JC, Fischer A, Francois C, Gaudu JC,
      Gonzalez E, Gouget R, Gu XF, Guerif M, Hanocq JF, Hautecoeur O, Haverkamp
      R, Hobbs S, Jacob F, Jeansoulin R, Jongschaap RE, Kerr Y, King C, Laborie
      P, Lagouarde JP, Laques AE, Larcena D, Laurent G, Laurent JP, Leroy M,
      McAneney J, Macelloni G, Moulin S, Noilhan J, Ottle C, Paloscia S,
      Pampaloni P, Podvin T, Quaracino F, Roujean JL, Rozier C, Ruisi R, Susini
      C, Taconet O, Tallet N, Thony JL, Travi Y, van Leewen H, Vauclin M,
      Vidal-Madjar D, Vonder OW, Weiss M, Wigneron JP (19â21 March 1998). D.
      Marceau (ed.). Spatial_Aspects_in_the_Alpilles-ReSeDA_Project (PDF).
      International Workshop on Scaling and Modelling in Forestry: Applications
      in Remote Sensing and GIS. University of Montreal, MontrÃ©al, QuÃ©bec,
      Canada. pp. 93â102. Retrieved 8 July 2019.CS1 maint: Date format (link)
  31. ^ {{Cite web |url=http://www.atm.ox.ac.uk/group/gpfd/
      research.html#marsgcm{{full |title=Archived copy |access-date=2011-08-19
      |archive-url=https://web.archive.org/web/20110928051446/http://
      www.atm.ox.ac.uk/group/gpfd/research.html#marsgcm[full_citation_needed]
  32. ^ http://www.eps.jhu.edu/~mjhoffman/pages/research.html[full_citation
      needed]
  33. ^ http://www.marsclimatecenter.com
  34. ^ http://badc.nerc.ac.uk/home/[full_citation_needed]
  35. ^Vetra-Carvalho, Sanita; P. J. van Leeuwen; L. Nerger; A. Barth; A.M.
      Umer; P. Brasseur; P. Kirchgessner; J-M. Beckers (2018). "State-of-the-
      art stochastic data assimilation methods for high-dimensional non-
      Gaussian problems". Tellus A. 70 (1): 1445364. Bibcode:
      2018TellA..7045364V. doi:10.1080/16000870.2018.1445364.
***** Further reading[edit] *****
    * Daley,_R. (1991). Atmospheric Data Analysis. Cambridge University Press.
      ISBN 978-0-521-38215-1.
"MM5_community_model_homepage".
"ECMWF_Data_Assimilation_Lecture_notes".
Ide, Kayo; Courtier, Philippe; Ghil,_Michael; Lorenc, Andrew C (1997). "Unified
Notation for Data Assimilation : Operational, Sequential and Variational
(gtSpecial IssueltData Assimilation in Meteology and Oceanography: Theory and
Practice)". Journal of the Meteorological Society of Japan. Ser. II. 75 (1B):
181â9. doi:10.2151/jmsj1965.75.1B_181.
"Understanding_Data_Assimilation". COMET module.
Evensen, Geir (2009). Data Assimilation. The Ensemble Kalman Filter (Second
ed.). Springer. ISBN 978-3-642-03710-8.
Lewis, John M.; Lakshmivarahan, S.; Dhall, Sudarshan (2006). "Dynamic Data
Assimilation : A Least Squares Approach". Encyclopedia of Mathematics and its
Applications. 104. Cambridge University Press. ISBN 978-0-521-85155-8.
Asch, Mark; Bocquet, Marc; Nodet, MaÃ«lle (2016). Data Assimilation: Methods,
Algorithms, and Applications. Society for Industrial and Applied Mathematics.
ISBN 978-1-61197-453-9.
Kalnay,_Eugenia (2002). Atmospheric Modeling, Data Assimilation and
Predictability. Atmospheric Modeling. Cambridge University Press. p. 364.
Bibcode:2002amda.book.....K. ISBN 978-0-521-79179-3.
Vetra-Carvalho, S.; van Leeuwen, P. J.; Nerger, L.; Barth, A.; Umer Altat, M.;
Brasseur, P.; Kirchgessner, P.; Beckers, J-M. (2018). "State-of-the-art
stochastic data assimilation methods for high-dimensional non-Gaussian
problems". Tellus A: Dynamic Meteorology and Oceanography. 70 (1): 1445364.
Bibcode:2018TellA..7045364V. doi:10.1080/16000870.2018.1445364.
***** External links[edit] *****
Examples of how variational assimilation is implemented weather forecasting at:
    * Data_Assimilation. ECMWF. IFS Documentation. ECMWF. 2010.
"Data_Assimilation". Met_Office.
Other examples of assimilation:
    * CDACentral_(an_example_analysis_from_Chemical_Data_Assimilation)
    * PDFCentral_(using_PDFs_to_examine_biases_and_representativeness)
    * OpenDA_â_Open_Source_Data_Assimilation_package
    * PDAF_â_open-source_Parallel_Data_Assimilation_Framework
    * SANGOMA_New_Data_Assimilation_techniques

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Data_assimilation&oldid=907756654"
Categories:
    * Weather_forecasting
    * Numerical_climate_and_weather_models
    * Estimation_theory
    * Control_theory
    * Bayesian_statistics
    * Climate_and_weather_statistics
    * Statistical_forecasting
Hidden categories:
    * Articles_with_incomplete_citations_from_January_2018
    * CS1:_long_volume_value
    * CS1_maint:_Date_format
    * Articles_with_incomplete_citations_from_July_2019
    * Articles_needing_additional_references_from_September_2011
    * All_articles_needing_additional_references
    * Wikipedia_articles_needing_clarification_from_October_2013
    * All_Wikipedia_articles_needing_clarification
    * Articles_with_multiple_maintenance_issues
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_January_2018
    * Articles_to_be_expanded_from_June_2008
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
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
    * CatalÃ 
    * Deutsch
    * FranÃ§ais
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 25 July 2019, at 02:15 (UTC).
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
