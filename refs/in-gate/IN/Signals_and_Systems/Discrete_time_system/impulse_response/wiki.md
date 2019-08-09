The following text has been accessed from https://en.wikipedia.org/wiki/Impulse_response at Fri Aug 9 01:31:39 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Impulse response ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The Impulse response from a simple audio system. Showing, from top to bottom,
the original impulse, the response after high frequency boosting, and the
response after low frequency boosting.
In signal_processing, the impulse response, or impulse response function (IRF),
of a dynamic_system is its output when presented with a brief input signal,
called an impulse. More generally, an impulse response is the reaction of any
dynamic system in response to some external change. In both cases, the impulse
response describes the reaction of the system as a function of time (or
possibly as a function of some other independent_variable that parameterizes
the dynamic behavior of the system).
In all these cases, the dynamic system and its impulse response may be actual
physical objects, or may be mathematical systems of equations describing such
objects.
Since the impulse function contains all frequencies, the impulse response
defines the response of a linear_time-invariant_system for all frequencies.
⁰
***** Contents *****
    * 1_Mathematical_considerations
    * 2_Practical_applications
          o 2.1_Loudspeakers
          o 2.2_Electronic_processing
          o 2.3_Control_systems
          o 2.4_Acoustic_and_audio_applications
          o 2.5_Economics
    * 3_See_also
    * 4_References
***** Mathematical considerations[edit] *****
See also: Vector_autoregression_Â§ Impulse_response, and Moving_average_model
Â§ Interpretation
Mathematically, how the impulse is described depends on whether the system is
modeled in discrete or continuous time. The impulse can be modeled as a Dirac
delta_function for continuous-time systems, or as the Kronecker_delta for
discrete-time systems. The Dirac delta represents the limiting case of a pulse
made very short in time while maintaining its area or integral (thus giving an
infinitely high peak). While this is impossible in any real system, it is a
useful idealisation. In Fourier_analysis theory, such an impulse comprises
equal portions of all possible excitation frequencies, which makes it a
convenient test probe.
Any system in a large class known as linear, time-invariant (LTI) is completely
characterized by its impulse response. That is, for any input, the output can
be calculated in terms of the input and the impulse response. (See LTI_system
theory.) The impulse response of a linear_transformation is the image of
Dirac's_delta_function under the transformation, analogous to the fundamental
solution of a partial_differential_operator.
It is usually easier to analyze systems using transfer_functions as opposed to
impulse responses. The transfer function is the Laplace_transform of the
impulse response. The Laplace transform of a system's output may be determined
by the multiplication of the transfer function with the input's Laplace
transform in the complex_plane, also known as the frequency_domain. An inverse
Laplace_transform of this result will yield the output in the time_domain.
To determine an output directly in the time domain requires the convolution of
the input with the impulse response. When the transfer function and the Laplace
transform of the input are known, this convolution may be more complicated than
the alternative of multiplying two functions in the frequency_domain.
The impulse response, considered as a Green's_function, can be thought of as an
"influence function": how a point of input influences output.
***** Practical applications[edit] *****
In practical systems, it is not possible to produce a perfect impulse to serve
as input for testing; therefore, a brief pulse is sometimes used as an
approximation of an impulse. Provided that the pulse is short enough compared
to the impulse response, the result will be close to the true, theoretical,
impulse response. In many systems, however, driving with a very short strong
pulse may drive the system into a nonlinear regime, so instead the system is
driven with a pseudo-random sequence, and the impulse response is computed from
the input and output signals.[1]
**** Loudspeakers[edit] ****
An application that demonstrates this idea was the development of impulse
response loudspeaker testing in the 1970s. Loudspeakers suffer from phase
inaccuracy, a defect unlike other measured properties such as frequency
response. Phase inaccuracy is caused by (slightly) delayed frequencies/octaves
that are mainly the result of passive cross overs (especially higher order
filters) but are also caused by resonance, energy storage in the cone, the
internal volume, or the enclosure panels vibrating.[citation_needed] Measuring
the impulse response, which is a direct plot of this "time-smearing," provided
a tool for use in reducing resonances by the use of improved materials for
cones and enclosures, as well as changes to the speaker crossover. The need to
limit input amplitude to maintain the linearity of the system led to the use of
inputs such as pseudo-random maximum_length_sequences, and to the use of
computer processing to derive the impulse response.[2]
**** Electronic processing[edit] ****
Impulse response analysis is a major facet of radar, ultrasound_imaging, and
many areas of digital_signal_processing. An interesting example would be
broadband internet connections. DSL/Broadband services use adaptive
equalisation techniques to help compensate for signal distortion and
interference introduced by the copper phone lines used to deliver the service.
**** Control systems[edit] ****
In control_theory the impulse response is the response of a system to a Dirac
delta input. This proves useful in the analysis of dynamic_systems; the Laplace
transform of the delta function is 1, so the impulse response is equivalent to
the inverse_Laplace_transform of the system's transfer_function.
**** Acoustic and audio applications[edit] ****
In acoustic and audio applications, impulse responses enable the acoustic
characteristics of a location, such as a concert hall, to be captured. Various
packages are available containing impulse responses from specific locations,
ranging from small rooms to large concert halls. These impulse responses can
then be utilized in convolution_reverb applications to enable the acoustic
characteristics of a particular location to be applied to target audio.[3]
**** Economics[edit] ****
In economics, and especially in contemporary macroeconomic_modeling, impulse
response functions are used to describe how the economy reacts over time to
exogenous impulses, which economists usually call shocks, and are often modeled
in the context of a vector_autoregression. Impulses that are often treated as
exogenous from a macroeconomic point of view include changes in government
spending, tax_rates, and other fiscal_policy parameters; changes in the
monetary_base or other monetary_policy parameters; changes in productivity or
other technological parameters; and changes in preferences, such as the degree
of impatience. Impulse response functions describe the reaction of endogenous
macroeconomic variables such as output, consumption, investment, and employment
at the time of the shock and over subsequent points in time.[4][5] Recently,
asymmetric impulse response functions have been suggested in the literature
that separate the impact of a positive shock from a negative one. [6]
***** See also[edit] *****
    * Convolution_reverb
    * Dirac_delta_function
    * Dynamic_stochastic_general_equilibrium
    * Duhamel's_principle
    * Frequency_response
    * Gibbs_phenomenon
    * LTI_system_theory
    * Pre-echo
    * System_analysis
    * Step_response
    * Time_constant
    * Linear_response_function
    * Transient
    * Transient_response
    * Unit_impulse_function
    * Point_spread_function
    * KÃ¼ssner_effect
    * Variation_of_parameters
    *  Media related to Impulse_response at Wikimedia Commons
***** References[edit] *****
   1. ^F._Alton_Everest (2000). Master_Handbook_of_Acoustics (Fourth ed.).
      McGraw-Hill Professional. ISBN 0-07-136097-2.
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
   3. ^"Monitor". 9 April 1976. Retrieved 9 April 2018 – via Google Books.
   4. ^ http://www.acoustics.hut.fi/projects/poririrs/ the Concert Hall Impulse
      Responses from Pori, Finland
   5. ^LÃ¼tkepohl,_Helmut (2008). "Impulse response function". The New Palgrave
      Dictionary of Economics (2nd ed.).
   6. ^Hamilton,_James_D. (1994). "Difference Equations". Time Series Analysis.
      Princeton University Press. p. 5. ISBN 0-691-04289-6.
   7. ^Hatemi-J, A. (2014). "Asymmetric_generalized_impulse_responses_with_an
      application_in_finance". Economic_Modelling. 36: 18â2.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Impulse_response&oldid=890888372"
Categories:
    * Control_theory
    * Time_domain_analysis
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_July_2011
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
    * á áá­á
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Basa_Sunda
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 4 April 2019, at 06:16 (UTC).
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
