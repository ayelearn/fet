The following text has been accessed from https://en.wikipedia.org/wiki/Frequency_response at Fri Aug 9 01:31:34 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Frequency response ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This introduction and first section needs additional citations for verification.
 Please help improve_this_article by adding_citations_to_reliable_sources. Unsourced
 material may be challenged and removed.
 Find sources: "Frequency_response" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (September 2011)(Learn_how_and_when_to_remove_this_template_message)
Frequency response is the quantitative measure of the output spectrum of a
system or device in response to a stimulus, and is used to characterize the
dynamics of the system. It is a measure of magnitude and phase of the output as
a function of frequency, in comparison to the input. In simplest terms, if a
sine_wave is injected into a system at a given frequency, a linear_system will
respond at that same frequency with a certain magnitude and a certain phase
angle relative to the input. Also for a linear system, doubling the amplitude
of the input will double the amplitude of the output. In addition, if the
system is time-invariant (so LTI), then the frequency response also will not
vary with time. Thus for LTI systems, the frequency response can be seen as
applying the system's transfer_function to a purely_imaginary_number argument
representing_the_frequency of the sinusoidal excitation.[1]
Two applications of frequency response analysis are related but have different
objectives.
For an audio system, the objective may be to reproduce the input signal with no
distortion. That would require a uniform (flat) magnitude of response up to the
bandwidth limitation of the system, with the signal delayed by precisely the
same amount of time at all frequencies. That amount of time could be seconds,
or weeks or months in the case of recorded media.
In contrast, for a feedback apparatus used to control a dynamic system, the
objective is to give the closed-loop system improved response as compared to
the uncompensated system. The feedback generally needs to respond to system
dynamics within a very small number of cycles of oscillation (usually less than
one full cycle), and with a definite phase angle relative to the commanded
control input. For feedback of sufficient amplification, getting the phase
angle wrong can lead to instability for an open-loop stable system, or failure
to stabilize a system that is open-loop unstable.
Digital filters may be used for both audio systems and feedback control
systems, but since the objectives are different, generally the phase
characteristics of the filters will be significantly different for the two
applications.
⁰
***** Contents *****
    * 1_Estimation_and_plotting
          o 1.1_Nonlinear_frequency_response
    * 2_Applications
    * 3_See_also
    * 4_References
    * 5_External_links
***** Estimation and plotting[edit] *****
Frequency response of a low pass filter with 6 dB per octave or 20 dB per
decade
Estimating the frequency response for a physical system generally involves
exciting the system with an input signal, measuring both input and output time
histories, and comparing the two through a process such as the Fast_Fourier
Transform (FFT). One thing to keep in mind for the analysis is that the
frequency content of the input signal must cover the frequency range of
interest because the results will not be valid for the portion of the frequency
range not covered.
The frequency response of a system can be measured by applying a test signal,
for example:
    * applying an impulse to the system and measuring its response (see impulse
      response)
    * sweeping a constant-amplitude pure tone through the bandwidth of interest
      and measuring the output level and phase shift relative to the input
    * applying a signal with a wide frequency spectrum (for example
      multifrequency signals [2] (nonorthogonal frequency-discrete multiplexing
      of signals (N-OFDM [3][4] or as the same SEFDM[5]) and OFDM), digitally-
      generated maximum_length_sequence noise, or analog filtered white_noise
      equivalent, like pink_noise), and calculating the impulse response by
      deconvolution of this input signal and the output signal of the system.
The frequency response is characterized by the magnitude of the system's
response, typically measured in decibels (dB) or as a decimal, and the phase,
measured in radians or degrees, versus frequency in radians/sec or Hertz (Hz).
These response measurements can be plotted in three ways: by plotting the
magnitude and phase measurements on two rectangular plots as functions of
frequency to obtain a Bode_plot; by plotting the magnitude and phase angle on a
single polar plot with frequency as a parameter to obtain a Nyquist_plot; or by
plotting magnitude and phase on a single rectangular plot with frequency as a
parameter to obtain a Nichols_plot.
For audio systems with nearly uniform time delay at all frequencies, the
magnitude versus frequency portion of the Bode plot may be all that is of
interest. For design of control systems, any of the three types of plots [Bode,
Nyquist, Nichols] can be used to infer closed-loop stability and stability
margins (gain and phase margins) from the open-loop frequency response,
provided that for the Bode analysis the phase-versus-frequency plot is
included.
The form of frequency response for digital systems (as example FFT filters )
are periodical with multiple main lobes and sidelobes.[6]
**** Nonlinear frequency response[edit] ****
If the system under investigation is nonlinear then applying purely linear
frequency domain analysis will not reveal all the nonlinear characteristics. To
overcome these limitations, generalized frequency response functions and
nonlinear output frequency response functions have been defined that allow the
user to analyze complex nonlinear dynamic effects.[7] The nonlinear frequency
response methods reveal complex resonance, inter modulation, and energy
transfer effects that cannot be seen using a purely linear analysis and are
becoming increasingly important in a nonlinear world.
***** Applications[edit] *****
In electronics this stimulus would be an input signal.[8] In the audible range
it is usually referred to in connection with electronic_amplifiers, microphones
and loudspeakers. Radio spectrum frequency response can refer to measurements
of coaxial_cable, twisted-pair_cable, video_switching equipment, wireless
communications devices, and antenna systems. Infrasonic frequency response
measurements include earthquakes and electroencephalography (brain waves).
Frequency response requirements differ depending on the application.[9] In high
fidelity audio, an amplifier requires a frequency response of at least
20â20,000 Hz, with a tolerance as tight as Â±0.1 dB in the mid-range
frequencies around 1000 Hz, however, in telephony, a frequency response of
400â4,000 Hz, with a tolerance of Â±1 dB is sufficient for intelligibility of
speech.[9]
Frequency response curves are often used to indicate the accuracy of electronic
components or systems.[8] When a system or component reproduces all desired
input signals with no emphasis or attenuation of a particular frequency band,
the system or component is said to be "flat", or to have a flat frequency
response curve.[8] In other case can be use 3D-form of frequency response
surface.
Once a frequency response has been measured (e.g., as an impulse response),
provided the system is linear_and_time-invariant, its characteristic can be
approximated with arbitrary accuracy by a digital_filter. Similarly, if a
system is demonstrated to have a poor frequency response, a digital or analog
filter can be applied to the signals prior to their reproduction to compensate
for these deficiencies.
The form of a frequency response curve is very important for anti-jamming
protection of radars, communications and other systems.
***** See also[edit] *****
    * Audio_system_measurements
    * Bandwidth_(signal_processing)
    * Bode_plot
    * Frequency response
    * Impulse_response
    * Spectral_sensitivity
    * Steady_state_(electronics)
    * Transient_response
    * Universal_dielectric_response
***** References[edit] *****
  Notes
   1. ^Dennis L. Feucht (1990). Handbook of Analog Circuit Design. Elsevier
      Science. p. 192. ISBN 978-1-4832-5938-3.
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
   3. ^ RU2054684 (C1) G01R 23/16. Amplitude-frequency response measurement
      technique// Slyusar V. â Appl. Number SU 19925055759, Priority Data:
      19920722. â Official Publication Data: 1996-02-20 [1]
   4. ^ Slyusar, V. I. Smolyar, V. G. The method of nonorthogonal frequency-
      discrete modulation of signals for narrow-band communication channels/
      / Radio electronics and communications systems c/c of Izvestiia- vysshie
      uchebnye zavedeniia radioelektronika. â 2004, volume 47; part 4, pages
      40â44. â Allerton press Inc. (USA)[2]
   5. ^ Slyusar, V. I. Smolyar, V. G. Multifrequency operation of communication
      channels based on super-Rayleigh resolution of signals// Radio
      electronics and communications systems c/c of Izvestiia- vysshie uchebnye
      zavedeniia radioelektronika.. â 2003, volume 46; part 7, pages 22â27.
      â Allerton press Inc. (USA)[3]
   6. ^ M. R. D. Rodrigues and I. Darwazeh. A Spectrally Efficient Frequency
      Division Multiplexing Based Communications System.// InOWo'03, 8th
      International OFDM-Workshop, Proceedings, Hamburg, DE, September 24â25,
      2003. â https://www.researchgate.net/publication/309373002
   7. ^ L. R. Rabiner and B. Gold. Theory and Application of Digital Signal
      Processing. â Englewood Cliffs, NJ: Prentice-Hall, 1975. â 720 pp
   8. ^ Billings S.A. "Nonlinear System Identification: NARMAX Methods in the
      Time, Frequency, and Spatio-Temporal Domains". Wiley, 2013
   9. ^ a b c Stark, 2002, p. 51.
  10. ^ a b Luther, 1999, p. 141.
  Bibliography
    * Luther, Arch C.; Inglis, Andrew F. Video_engineering, McGraw-Hill, 1999.
ISBN 0-07-135017-9
Stark, Scott Hunter. Live_Sound_Reinforcement, Vallejo, California,
Artistpro.com, 1996â2002.
ISBN 0-918371-07-4
L. R. Rabiner and B. Gold. Theory and Application of Digital Signal Processing.
â Englewood Cliffs, NJ: Prentice-Hall, 1975. â 720 pp
***** External links[edit] *****
    * University_of_Michigan: Frequency_Response_Analysis_and_Design_Tutorial
    * Smith, Julius O. III: Introduction_to_Digital_Filters_with_Audio
      Applications has a nice chapter on Frequency_Response

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Frequency_response&oldid=881250825"
Categories:
    * Signal_processing
    * Control_theory
    * Audio_amplifier_specifications
Hidden categories:
    * Articles_needing_additional_references_from_September_2011
    * All_articles_needing_additional_references
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
    * Dansk
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * Nederlands
    * æ¥æ¬èª
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 1 February 2019, at 10:44 (UTC).
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
