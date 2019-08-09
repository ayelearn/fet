The following text has been accessed from https://en.wikipedia.org/wiki/Deconvolution at Thu Aug 8 23:28:17 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Deconvolution ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, deconvolution is an algorithm-based process used to reverse the
effects of convolution on recorded data.[1] The concept of deconvolution is
widely used in the techniques of signal_processing and image_processing.
Because these techniques are in turn widely used in many scientific and
engineering disciplines, deconvolution finds many applications.
In general, the objective of deconvolution is to find the solution of a
convolution equation of the form:
         f &#x2217; g = h    {\displaystyle f*g=h\,}  [f * g = h \, ]
Usually, h is some recorded signal, and f is some signal that we wish to
recover, but has been convolved with some other signal g before we recorded it.
The function g might represent the transfer_function of an instrument or a
driving force that was applied to a physical system. If we know g, or at least
know the form of g, then we can perform deterministic deconvolution. However,
if we do not know g in advance, then we need to estimate it. This is most often
done using methods of statistical estimation.
In physical measurements, the situation is usually closer to
         ( f &#x2217; g ) + &#x03B5; = h    {\displaystyle (f*g)+\varepsilon
      =h\,}  [(f * g)  + \varepsilon  = h \, ]
In this case ε is noise that has entered our recorded signal. If we assume that
a noisy signal or image is noiseless when we try to make a statistical estimate
of g, our estimate will be incorrect. In turn, our estimate of ƒ will also be
incorrect. The lower the signal-to-noise_ratio, the worse our estimate of the
deconvolved signal will be. That is the reason why inverse_filtering the signal
is usually not a good solution. However, if we have at least some knowledge of
the type of noise in the data (for example, white_noise), we may be able to
improve the estimate of ƒ through techniques such as Wiener_deconvolution.
Deconvolution is usually performed by computing the Fourier_Transform of the
recorded signal h and the transfer_function g, apply deconvolution in the
Frequency domain, which in the case of absence of noise is merely:
         F = H  /  G    {\displaystyle F=H/G\,}  [{\displaystyle F=H/G\,}]
F, G, and H being the Fourier_Transforms of f, g, and h respectively. Finally
inverse Fourier_Transform F to find the estimated deconvolved signal f.
The foundations for deconvolution and time-series_analysis were largely laid by
Norbert_Wiener of the Massachusetts_Institute_of_Technology in his book
Extrapolation, Interpolation, and Smoothing of Stationary Time Series (1949).
[2] The book was based on work Wiener had done during World_War_II but that had
been classified at the time. Some of the early attempts to apply these theories
were in the fields of weather_forecasting and economics.
⁰
***** Contents *****
    * 1_Applications
          o 1.1_Seismology
          o 1.2_Optics_and_other_imaging
          o 1.3_Radio_astronomy
          o 1.4_Fourier_transform_aspects
    * 2_Absorption_spectra
    * 3_See_also
    * 4_References
***** Applications[edit] *****
**** Seismology[edit] ****
The concept of deconvolution had an early application in reflection_seismology.
In 1950, Enders_Robinson was a graduate student at MIT. He worked with others
at MIT, such as Norbert_Wiener, Norman_Levinson, and economist Paul_Samuelson,
to develop the "convolutional model" of a reflection seismogram. This model
assumes that the recorded seismogram s(t) is the convolution of an Earth-
reflectivity function e(t) and a seismic wavelet w(t) from a point_source,
where t represents recording time. Thus, our convolution equation is
         s ( t ) = ( e &#x2217; w ) ( t ) .    {\displaystyle s(t)=(e*w)(t).\,}
      [s(t) = (e * w)(t). \, ]
The seismologist is interested in e, which contains information about the
Earth's structure. By the convolution_theorem, this equation may be Fourier
transformed to
         S ( &#x03C9; ) = E ( &#x03C9; ) W ( &#x03C9; )    {\displaystyle S
      (\omega )=E(\omega )W(\omega )\,}  [S(\omega) = E(\omega)W(\omega) \, ]
in the frequency_domain. By assuming that the reflectivity is white, we can
assume that the power_spectrum of the reflectivity is constant, and that the
power spectrum of the seismogram is the spectrum of the wavelet multiplied by
that constant. Thus,
          |  S ( &#x03C9; )  |  &#x2248; k  |  W ( &#x03C9; )  |  .
      {\displaystyle |S(\omega )|\approx k|W(\omega )|.\,}  [|S(\omega)|
      \approx k|W(\omega)|. \, ]
If we assume that the wavelet is minimum_phase, we can recover it by
calculating the minimum phase equivalent of the power spectrum we just found.
The reflectivity may be recovered by designing and applying a Wiener_filter
that shapes the estimated wavelet to a Dirac_delta_function (i.e., a spike).
The result may be seen as a series of scaled, shifted delta functions (although
this is not mathematically rigorous):
         e ( t ) =  &#x2211;  i = 1   N    r  i   &#x03B4; ( t &#x2212;
      &#x03C4;  i   )   {\displaystyle e(t)=\sum _{i=1}^{N}r_{i}\delta (t-\tau
      _{i})}  [e(t)=\sum_{i=1}^N r_i\delta(t-\tau_i)],
where N is the number of reflection events, τ i τ i are the reflection times of
each event, and r i are the reflection_coefficients.
In practice, since we are dealing with noisy, finite bandwidth, finite length,
discretely_sampled datasets, the above procedure only yields an approximation
of the filter required to deconvolve the data. However, by formulating the
problem as the solution of a Toeplitz_matrix and using Levinson_recursion, we
can relatively quickly estimate a filter with the smallest mean_squared_error
possible. We can also do deconvolution directly in the frequency domain and get
similar results. The technique is closely related to linear_prediction.
**** Optics and other imaging[edit] ****
Example of a deconvolved microscope image.
In optics and imaging, the term "deconvolution" is specifically used to refer
to the process of reversing the optical_distortion that takes place in an
optical microscope, electron_microscope, telescope, or other imaging
instrument, thus creating clearer images. It is usually done in the digital
domain by a software algorithm, as part of a suite of microscope_image
processing techniques. Deconvolution is also practical to sharpen images that
suffer from fast motion or jiggles during capturing. Early Hubble_Space
Telescope images were distorted by a flawed_mirror and were sharpened by
deconvolution.
The usual method is to assume that the optical path through the instrument is
optically perfect, convolved with a point_spread_function (PSF), that is, a
mathematical_function that describes the distortion in terms of the pathway a
theoretical point_source of light (or other waves) takes through the
instrument.[3] Usually, such a point source contributes a small area of
fuzziness to the final image. If this function can be determined, it is then a
matter of computing its inverse or complementary function, and convolving the
acquired image with that. The result is the original, undistorted image.
In practice, finding the true PSF is impossible, and usually an approximation
of it is used, theoretically calculated[4] or based on some experimental
estimation by using known probes. Real optics may also have different PSFs at
different focal and spatial locations, and the PSF may be non-linear. The
accuracy of the approximation of the PSF will dictate the final result.
Different algorithms can be employed to give better results, at the price of
being more computationally intensive. Since the original convolution discards
data, some algorithms use additional data acquired at nearby focal points to
make up some of the lost information. Regularization in iterative algorithms
(as in expectation-maximization_algorithms) can be applied to avoid unrealistic
solutions.
Before and after deconvolution of an image of the lunar crater Copernicus using
the Lucy-Richardson algorithm. No other processing has been applied between the
two images.
When the PSF is unknown, it may be possible to deduce it by systematically
trying different possible PSFs and assessing whether the image has improved.
This procedure is called blind_deconvolution.[3] Blind deconvolution is a well-
established image restoration technique in astronomy, where the point nature of
the objects photographed exposes the PSF thus making it more feasible. It is
also used in fluorescence_microscopy for image restoration, and in fluorescence
spectral_imaging for spectral separation of multiple unknown fluorophores. The
most common iterative algorithm for the purpose is the RichardsonâLucy
deconvolution algorithm; the Wiener_deconvolution (and approximations) are the
most common non-iterative algorithms.
High Resolution THz image is achieved by deconvolution of the THz image and the
mathematically modeled THz PSF. (a) THz image of an integrated circuit (IC)
before enhancement; (b) Mathematically modeled THz PSF; (c) High resolution THz
image which is achieved as a result of deconvolution of the THz image shown in
(a) and the PSF which is shown in (b); (d) High resolution X-ray image confirms
the accuracy of the measured values.[5]
For some specific imaging systems such as laser pulsed terahertz systems, PSF
can be modeled mathematically.[6] As a result, as shown in the figure,
deconvolution of the modeled PSF and the terahertz image can give a higher
resolution representation of the terahertz image.
**** Radio astronomy[edit] ****
When performing image synthesis in radio interferometry, a specific kind of
radio_astronomy, one step consists of deconvolving the produced image with the
"dirty beam", which is a different name for the point_spread_function. A
commonly used method is the CLEAN_algorithm.
**** Fourier transform aspects[edit] ****
Deconvolution maps to division in the Fourier_co-domain. This allows
deconvolution to be easily applied with experimental data that are subject to a
Fourier_transform. An example is NMR_spectroscopy where the data are recorded
in the time domain, but analyzed in the frequency domain. Division of the time-
domain data by an exponential function has the effect of reducing the width of
Lorenzian lines in the frequency domain.
***** Absorption spectra[edit] *****
Deconvolution has been applied extensively to absorption spectra.[7] The Van
Cittert_algorithm (in German) may be used.[8]
***** See also[edit] *****
    * Convolution
    * Bit_plane
    * Digital_filter
    * Filter_(signal_processing)
    * Filter_design
    * Minimum_phase
    * Independent_component_analysis
    * Wiener_deconvolution
    * RichardsonâLucy_deconvolution
    * Digital_room_correction
    * Free_deconvolution
    * Point_spread_function
    * Deblurring
    * IVIVC
    * Unsharp_masking
***** References[edit] *****
   1. ^O'Haver T. "Intro_to_Signal_Processing_-_Deconvolution". University of
      Maryland at College Park. Retrieved 2007-08-15.
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
   3. ^Wiener N (1964). Extrapolation, Interpolation, and Smoothing of
      Stationary Time Series. Cambridge, Mass: MIT Press. ISBN 0-262-73005-7.
   4. ^ a bCheng PC (2006). "The Contrast Formation in Optical Microscopy".
      Handbook of Biological Confocal Microscopy (Pawley JB, ed.) (3rd ed.).
      Berlin: Springer. pp. 189â90. ISBN 0-387-25921-X.
   5. ^Nasse M. J., Woehl J. C. (2010). "Realistic modeling of the illumination
      point spread function in confocal scanning optical microscopy". J. Opt.
      Soc. Am. A. 27 (2): 295â302. doi:10.1364/JOSAA.27.000295.
      PMID 20126241.
   6. ^Ahi, Kiarash; Anwar, Mehdi (May 26, 2016). "Developing_terahertz_imaging
      equation_and_enhancement_of_the_resolution_of_terahertz_images_using
      deconvolution". Proc. SPIE 9856, Terahertz Physics, Devices, and Systems
      X: Advanced Applications in Industry and Defense, 98560N. doi:10.1117/
      12.2228680.
   7. ^Sung, Shijun (2013). Terahertz Imaging and Remote Sensing Design for
      Applications in Medical Imaging. UCLA Electronic Theses and
      Dissertations.
   8. ^Blass, W.E.; Halsey, G.W. (1981). Deconvolution of Absorption Spectra.
      Academic Press. ISBN 0121046508.
   9. ^Wu, Chengqi; Aissaoui, Idriss; Jacquey, Serge (1994). "Algebraic
      analysis of the Van Cittert iterative method of deconvolution with a
      general relaxation factor". J. Opt. Soc. Am. A. 11 (11): 2804â2808.
      doi:10.1364/JOSAA.11.002804.
    * v
    * t
    * e
Optical microscopy
    * Microscope
    * Optical_microscopy
                         * Bright-field_microscopy
                         * KÃ¶hler_illumination
                         * Dark-field_microscopy
                         * Phase_contrast
                         * Quantitative_phase-
                           contrast_microscopy
Illumination and         * Differential_interference
contrast methods           contrast_(DIC)
                         * Dispersion_staining
                         * Second_harmonic_imaging_
                           (SHIM)
                         * 4Pi_microscope
                         * Structured_illumination
                         * Sarfus
                         * Fluorescence_microscopy
                         * Confocal_microscopy       [Loupe-binoculaire-
                         * Two-photon_excitation     p1030891.jpg]
                           microscopy
                         * Multiphoton_microscopy
Fluorescence methods     * Image_deconvolution
                         * Total_internal_reflection
                           fluorescence_microscopy_
                           (TIRF)
                         * Lightsheet_microscopy_
                           (LSFM/SPIM)
                         * Diffraction_limit
                         * Stimulated_emission
Sub-diffraction            depletion_(STED)
limit techniques         * Photo-activated
                           localization_microscopy_
                           (PALM/STORM)
                         * Near-field_(NSOM/SNOM)

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Deconvolution&oldid=891454792"
Categories:
    * Signal_processing
    * Image_processing
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
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 8 April 2019, at 01:59 (UTC).
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
