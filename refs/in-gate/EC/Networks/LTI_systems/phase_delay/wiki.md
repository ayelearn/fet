The following text has been accessed from https://en.wikipedia.org/wiki/Group_delay_and_phase_delay at Fri Aug 9 03:37:38 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Group delay and phase delay ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article needs additional citations for verification. Please help improve_this_article by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and removed.
 Find sources: "Group_delay_and_phase_delay" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (July 2011)(Learn_how_and_when_to_remove_this_template_message)
In signal_processing, group delay is the time delay of the amplitude envelopes
of the various sinusoidal components of a signal through a device_under_test,
and is a function of frequency for each component. Phase delay, in contrast, is
the time delay of the phase as opposed to the time delay of the amplitude
envelope.
All frequency components of a signal are delayed when passed through a device
such as an amplifier, a loudspeaker, or propagating through space or a medium,
such as air. This signal delay will be different for the various frequencies
unless the device has the property of being linear_phase. ("Linear phase" and
"minimum_phase" are often used interchangeably, but are actually quite
different.) The delay variation means that signals consisting of multiple
frequency components will suffer distortion because these components are not
delayed by the same amount of time at the output of the device. This changes
the shape of the signal in addition to any constant delay or scale change. A
sufficiently large delay variation can cause problems such as poor fidelity in
audio or intersymbol_interference (ISI) in the demodulation of digital
information from an analog carrier_signal. High speed modems use adaptive
equalizers to compensate for non-constant group delay.
⁰
***** Contents *****
    * 1_Introduction
    * 2_Group_delay_in_optics
    * 3_Group_delay_in_audio
    * 4_True_time_delay
    * 5_See_also
    * 6_References
    * 7_External_links
***** Introduction[edit] *****
Group delay is a useful measure of time distortion, and is calculated by
differentiating, with respect to frequency, the phase_response of the device
under test (DUT): the group delay is a measure of the slope of the phase
response at any given frequency. Variations in group delay cause signal
distortion, just as deviations from linear phase cause distortion.
In linear_time-invariant_(LTI)_system_theory, control_theory, and in digital or
analog signal_processing, the relationship between the input signal,      x ( t
)    {\displaystyle \displaystyle x(t)}  [\displaystyle x(t)], to output
signal,      y ( t )    {\displaystyle \displaystyle y(t)}  [\displaystyle y
(t)], of an LTI system is governed by a convolution operation:
         y ( t ) = ( h &#x2217; x ) ( t ) &#xA0;     =    d e f      &#xA0;
      &#x222B;  &#x2212; &#x221E;   &#x221E;   x ( u ) h ( t &#x2212; u )  d u
      {\displaystyle y(t)=(h*x)(t)\ {\stackrel {\mathrm {def} }{=}}\ \int _{-
      \infty }^{\infty }x(u)h(t-u)\,du}  [y(t)=(h*x)(t)\ {\stackrel  {{\mathrm
      {def}}}{=}}\ \int _{{-\infty }}^{{\infty }}x(u)h(t-u)\,du]
Or, in the frequency_domain,
         Y ( s ) = H ( s ) X ( s )    {\displaystyle Y(s)=H(s)X(s)\,}  [ Y(s) =
      H(s) X(s)  \, ]
where
         X ( s ) =   L     {   x ( t )   }   &#xA0;     =    d e f      &#xA0;
      &#x222B;  &#x2212; &#x221E;   &#x221E;   x ( t )  e  &#x2212; s t    d t
      {\displaystyle X(s)={\mathcal {L}}{\Big \{}x(t){\Big \}}\ {\stackrel
      {\mathrm {def} }{=}}\ \int _{-\infty }^{\infty }x(t)e^{-st}\,dt}  [
      {\displaystyle X(s)={\mathcal {L}}{\Big \{}x(t){\Big \}}\ {\stackrel
      {\mathrm {def} }{=}}\ \int _{-\infty }^{\infty }x(t)e^{-st}\,dt}]
         Y ( s ) =   L     {   y ( t )   }   &#xA0;     =    d e f      &#xA0;
      &#x222B;  &#x2212; &#x221E;   &#x221E;   y ( t )  e  &#x2212; s t    d t
      {\displaystyle Y(s)={\mathcal {L}}{\Big \{}y(t){\Big \}}\ {\stackrel
      {\mathrm {def} }{=}}\ \int _{-\infty }^{\infty }y(t)e^{-st}\,dt}  [
      {\displaystyle Y(s)={\mathcal {L}}{\Big \{}y(t){\Big \}}\ {\stackrel
      {\mathrm {def} }{=}}\ \int _{-\infty }^{\infty }y(t)e^{-st}\,dt}]
and
         H ( s ) =   L     {   h ( t )   }   &#xA0;     =    d e f      &#xA0;
      &#x222B;  &#x2212; &#x221E;   &#x221E;   h ( t )  e  &#x2212; s t    d t
      {\displaystyle H(s)={\mathcal {L}}{\Big \{}h(t){\Big \}}\ {\stackrel
      {\mathrm {def} }{=}}\ \int _{-\infty }^{\infty }h(t)e^{-st}\,dt}  [
      {\displaystyle H(s)={\mathcal {L}}{\Big \{}h(t){\Big \}}\ {\stackrel
      {\mathrm {def} }{=}}\ \int _{-\infty }^{\infty }h(t)e^{-st}\,dt}].
Here      h ( t )    {\displaystyle \displaystyle h(t)}  [\displaystyle h(t)]
is the time-domain impulse_response of the LTI system and      X ( s )
{\displaystyle \displaystyle X(s)}  [\displaystyle X(s)],      Y ( s )
{\displaystyle \displaystyle Y(s)}  [\displaystyle Y(s)],      H ( s )
{\displaystyle \displaystyle H(s)}  [\displaystyle H(s)], are the Laplace
transforms of the input      x ( t )    {\displaystyle \displaystyle x(t)}
[\displaystyle x(t)], output      y ( t )    {\displaystyle \displaystyle y(t)}
[\displaystyle y(t)], and impulse response      h ( t )    {\displaystyle
\displaystyle h(t)}  [\displaystyle h(t)], respectively.      H ( s )
{\displaystyle \displaystyle H(s)}  [\displaystyle H(s)] is called the transfer
function of the LTI system and, like the impulse response      h ( t )
{\displaystyle \displaystyle h(t)}  [\displaystyle h(t)], fully defines the
input-output characteristics of the LTI system.
Suppose that such a system is driven by a quasi-sinusoidal signal, that is a
sinusoid having an amplitude envelope      a ( t ) > 0    {\displaystyle
\displaystyle a(t)>0}  [{\displaystyle \displaystyle a(t)>0}] that is slowly
changing relative to the frequency      &#x03C9;    {\displaystyle
\displaystyle \omega }  [\displaystyle \omega] of the sinusoid. Mathematically,
this means that the quasi-sinusoidal driving signal has the form
         x ( t ) = a ( t ) cos &#x2061; ( &#x03C9; t + &#x03B8; ) &#xA0;
      {\displaystyle x(t)=a(t)\cos(\omega t+\theta )\ }  [x(t)=a(t)\cos(\omega
      t+\theta )\ ]
and the slowly changing amplitude envelope      a ( t )    {\displaystyle
\displaystyle a(t)}  [\displaystyle a(t)] means that
          |    d  d t    log &#x2061;   (   a ( t )   )    |  &#x226A; &#x03C9;
      &#xA0; .   {\displaystyle \left|{\frac {d}{dt}}\log {\big (}a(t){\big
      )}\right|\ll \omega \ .}  [{\displaystyle \left|{\frac {d}{dt}}\log {\big
      (}a(t){\big )}\right|\ll \omega \ .}]
Then the output of such an LTI system is very well approximated as
         y ( t ) =   |   H ( i &#x03C9; )   |   &#xA0; a ( t &#x2212;  &#x03C4;
      g   ) cos &#x2061;   (   &#x03C9; ( t &#x2212;  &#x03C4;  &#x03D5;   ) +
      &#x03B8;   )    .   {\displaystyle y(t)={\big |}H(i\omega ){\big |}\ a(t-
      \tau _{g})\cos {\big (}\omega (t-\tau _{\phi })+\theta {\big )}\;.}  [
      {\displaystyle y(t)={\big |}H(i\omega ){\big |}\ a(t-\tau _{g})\cos {\big
      (}\omega (t-\tau _{\phi })+\theta {\big )}\;.}]
Here       &#x03C4;  g      {\displaystyle \displaystyle \tau _{g}}
[\displaystyle \tau _{g}] and       &#x03C4;  &#x03D5;      {\displaystyle
\displaystyle \tau _{\phi }}  [\displaystyle \tau _{\phi }], the group delay
and phase delay respectively, are given by the expressions below (and
potentially are functions of the angular_frequency      &#x03C9;
{\displaystyle \displaystyle \omega }  [\displaystyle \omega]). The sinusoid,
as indicated by the zero crossings, is delayed in time by phase delay,
&#x03C4;  &#x03D5;      {\displaystyle \displaystyle \tau _{\phi }}
[\displaystyle \tau _{\phi }]. The envelope of the sinusoid is delayed in time
by the group delay,       &#x03C4;  g      {\displaystyle \displaystyle \tau _
{g}}  [\displaystyle \tau _{g}].
In a linear_phase system (with non-inverting gain), both       &#x03C4;  g
{\displaystyle \displaystyle \tau _{g}}  [\displaystyle \tau _{g}] and
&#x03C4;  &#x03D5;      {\displaystyle \displaystyle \tau _{\phi }}
[\displaystyle \tau _{\phi }] are constant (i.e. independent of      &#x03C9;
{\displaystyle \displaystyle \omega }  [\displaystyle \omega]) and equal, and
their common value equals the overall delay of the system; and the unwrapped
phase_shift of the system (namely      &#x2212; &#x03C9;  &#x03C4;  &#x03D5;
{\displaystyle \displaystyle -\omega \tau _{\phi }}  [{\displaystyle
\displaystyle -\omega \tau _{\phi }}]) is negative, with magnitude increasing
linearly with frequency      &#x03C9;    {\displaystyle \displaystyle \omega }
[\displaystyle \omega].
More generally, it can be shown that for an LTI system with transfer function
H ( s )    {\displaystyle \displaystyle H(s)}  [\displaystyle H(s)] driven by a
complex_sinusoid of unit amplitude,
         x ( t ) =  e  i &#x03C9; t   &#xA0;   {\displaystyle x(t)=e^{i\omega
      t}\ }  [x(t)=e^{{i\omega t}}\ ]
the output is
             y ( t )    = H ( i &#x03C9; ) &#xA0;  e  i &#x03C9; t   &#xA0;
      =  (    |   H ( i &#x03C9; )   |    e  i &#x03D5; ( &#x03C9; )    )
      &#xA0;  e  i &#x03C9; t   &#xA0;       =   |   H ( i &#x03C9; )   |
      &#xA0;  e  i  (  &#x03C9; t + &#x03D5; ( &#x03C9; )  )    &#xA0;
      &#xA0;   {\displaystyle {\begin{aligned}y(t)&=H(i\omega )\ e^{i\omega t}\
      \\&=\left({\big |}H(i\omega ){\big |}e^{i\phi (\omega )}\right)\ e^
      {i\omega t}\ \\&={\big |}H(i\omega ){\big |}\ e^{i\left(\omega t+\phi
      (\omega )\right)}\ \\\end{aligned}}\ }  [{\displaystyle {\begin{aligned}y
      (t)&=H(i\omega )\ e^{i\omega t}\ \\&=\left({\big |}H(i\omega ){\big |}e^
      {i\phi (\omega )}\right)\ e^{i\omega t}\ \\&={\big |}H(i\omega ){\big |}\
      e^{i\left(\omega t+\phi (\omega )\right)}\ \\\end{aligned}}\ }]
where the phase shift      &#x03D5;    {\displaystyle \displaystyle \phi }
[\displaystyle \phi] is
         &#x03D5; ( &#x03C9; ) &#xA0;     =    d e f      &#xA0; arg &#x2061;
      {  H ( i &#x03C9; )  }   .   {\displaystyle \phi (\omega )\ {\stackrel
      {\mathrm {def} }{=}}\ \arg \left\{H(i\omega )\right\}\;.}  [\phi (\omega
      )\ {\stackrel  {{\mathrm  {def}}}{=}}\ \arg \left\{H(i\omega
      )\right\}\;.]
Additionally, it can be shown that the group delay,       &#x03C4;  g
{\displaystyle \displaystyle \tau _{g}}  [\displaystyle \tau _{g}], and phase
delay,       &#x03C4;  &#x03D5;      {\displaystyle \displaystyle \tau _{\phi
}}  [\displaystyle \tau _{\phi }], are frequency-dependent, and they can be
computed from the phase shift      &#x03D5;    {\displaystyle \displaystyle
\phi }  [\displaystyle \phi] by
          &#x03C4;  g   ( &#x03C9; ) = &#x2212;    d &#x03D5; ( &#x03C9; )   d
      &#x03C9;    &#xA0;   {\displaystyle \tau _{g}(\omega )=-{\frac {d\phi
      (\omega )}{d\omega }}\ }  [\tau _{g}(\omega )=-{\frac  {d\phi (\omega )}
      {d\omega }}\ ]
          &#x03C4;  &#x03D5;   ( &#x03C9; ) = &#x2212;    &#x03D5; ( &#x03C9; )
      &#x03C9;   &#xA0;   {\displaystyle \tau _{\phi }(\omega )=-{\frac {\phi
      (\omega )}{\omega }}\ }  [\tau _{\phi }(\omega )=-{\frac  {\phi (\omega
      )}{\omega }}\ ] .
***** Group delay in optics[edit] *****
In physics, and in particular in optics, the term group delay has the following
meanings:
      1. The rate of change of the total phase shift with respect to angular
      frequency,
                &#x03C4;  g   = &#x2212;    d &#x03D5;   d &#x03C9;
            {\displaystyle \tau _{g}=-{\frac {d\phi }{d\omega }}}  [\tau _{g}=-
            {\frac  {d\phi }{d\omega }}]
      through a device or transmission_medium, where     &#x03D5; &#xA0;
      {\displaystyle \phi \ }  [\phi \ ] is the total phase shift in radians,
      and     &#x03C9; &#xA0;   {\displaystyle \omega \ }  [\omega \ ] is the
      angular_frequency in radians per unit time, equal to     2 &#x03C0; f
      &#xA0;   {\displaystyle 2\pi f\ }  [2\pi f\ ], where     f &#xA0;
      {\displaystyle f\ }  [ f \ ] is the frequency (hertz if group delay is
      measured in seconds).
      2. In an optical_fiber, the transit time required for optical power,
      traveling at a given mode's group_velocity, to travel a given distance.
      Note: For optical fiber dispersion measurement purposes, the quantity of
      interest is group delay per unit length, which is the reciprocal of the
      group velocity of a particular mode. The measured group delay of a signal
      through an optical fiber exhibits a wavelength dependence due to the
      various dispersion mechanisms present in the fiber.
It is often desirable for the group delay to be constant across all
frequencies; otherwise there is temporal smearing of the signal. Because group
delay is      &#x03C4;  g   ( &#x03C9; ) = &#x2212;    d &#x03D5;   d &#x03C9;
{\displaystyle \tau _{g}(\omega )=-{\frac {d\phi }{d\omega }}}  [\tau _{g}
(\omega )=-{\frac  {d\phi }{d\omega }}], as defined in (1), it therefore
follows that a constant group delay can be achieved if the transfer_function of
the device or medium has a linear phase response (i.e.,     &#x03D5; ( &#x03C9;
) = &#x03D5; ( 0 ) &#x2212;  &#x03C4;  g   &#x03C9; &#xA0;   {\displaystyle
\phi (\omega )=\phi (0)-\tau _{g}\omega \ }  [\phi (\omega )=\phi (0)-\tau _
{g}\omega \ ] where the group delay      &#x03C4;  g   &#xA0;   {\displaystyle
\tau _{g}\ }  [\tau _{g}\ ] is a constant). The degree of nonlinearity of the
phase indicates the deviation of the group delay from a constant.
***** Group delay in audio[edit] *****
Group delay has some importance in the audio field and especially in the sound
reproduction field. Many components of an audio reproduction chain, notably
loudspeakers and multiway loudspeaker crossover_networks, introduce group delay
in the audio signal. It is therefore important to know the threshold of
audibility of group delay with respect to frequency, especially if the audio
chain is supposed to provide high_fidelity reproduction. The best thresholds of
audibility table has been provided by Blauert_&_Laws_(1978).
Frequency Threshold Periods (Cycles)
500 Hz    3.2 ms    1.6
1 kHz     2 ms      2
2 kHz    1 ms      2
4 kHz    1.5 ms    6
8 kHz    2 ms      16
Flanagan, Moore and Stone conclude that at 1, 2 and 4 kHz, a group delay of
about 1.6 ms is audible with headphones in a non-reverberant condition.[1]
***** True time delay[edit] *****
A transmitting apparatus is said to have true time delay (TTD) if the time
delay is independent of the frequency of the electrical signal.[2][3] TTD is an
important characteristic of lossless and low-loss, dispersion free,
transmission lines. TTD allows for a wide instantaneous signal bandwidth with
virtually no signal distortion such as pulse broadening during pulsed
operation.
***** See also[edit] *****
    * Audio_system_measurements
    * Bessel_filter
    * Eye_pattern
    * Group_velocity -- "The group velocity of light in a medium is the inverse
      of the group delay per unit length."[4]
    * Spectral_phase -- "The group delay can be defined as the derivative of
      the spectral phase with respect to angular frequency."[5]
***** References[edit] *****
 This article incorporates public_domain_material from the General_Services
Administration document "Federal_Standard_1037C".
   1. ^Flanagan, Sheila; Moore, Brian C. J.; Stone, Michael A. (2005),
      "Discrimination_of_Group_Delay_in_Clicklike_Signals_Presented_via
      Headphones_and_Loudspeakers", Journal of the Audio Engineering Society,
      53 (7/8): 593â611
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
   3. ^"True_Time_Delay". Microwaves101, IEEE.
   4. ^Julius O. Smith III. "Phase_Delay_and_Group_Delay". Department of
      Electrical Engineering, Stanford_University.
   5. ^ https://www.rp-photonics.com/group_delay.html
   6. ^ https://www.rp-photonics.com/spectral_phase.html
    * Blauert, J.; Laws, P. (May 1978), "Group Delay Distortions in
      Electroacoustical Systems", Journal of the Acoustical Society of America,
      63 (5): 1478â1483, Bibcode:1978ASAJ...63.1478B, doi:10.1121/1.381841
***** External links[edit] *****
    * Discussion_of_Group_Delay_in_Loudspeakers
    * Group_Delay_Explanations_and_Applications
    * Blauert,_J.;_Laws,_P._(May_1978),_"Group_Delay_Distortions_in
      Electroacoustical_Systems",_Journal_of_the_Acoustical_Society_of_America
      63_(5):_1478â1483
    * "Introduction_to_Digital_Filters_with_Audio_Applications",_Julius_O.
      Smith_III,_(September_2007_Edition).

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Group_delay_and_phase_delay&oldid=886587453"
Categories:
    * Optics
    * Waves
    * Signal_processing
    * Electrical_engineering
Hidden categories:
    * Articles_needing_additional_references_from_July_2011
    * All_articles_needing_additional_references
    * Wikipedia_articles_incorporating_text_from_the_Federal_Standard_1037C
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
    * Deutsch
    * Esperanto
    * FranÃ§ais
    * æ¥æ¬èª
    * ä¸­æ
Edit_links
    * This page was last edited on 7 March 2019, at 05:46 (UTC).
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
