The following text has been accessed from https://en.wikipedia.org/wiki/Aliasing at Thu Aug 8 23:29:42 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Aliasing ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Effect that causes signals to become indistinguishable when sampled; often
producing detectable aberrations
This article is about aliasing in signal processing, including computer
graphics. For aliasing in computer programming, see aliasing_(computing).
Properly sampled image of a brick wall (requires screen of sufficient
resolution to prevent moirÃ©_pattern)
Spatial aliasing in the form of a moirÃ©_pattern
In signal_processing and related disciplines, aliasing is an effect that causes
different signals to become indistinguishable (or aliases of one another) when
sampled. It also refers to the distortion or artifact that results when the
signal reconstructed from samples is different from the original continuous
signal.
Aliasing can occur in signals sampled in time, for instance digital_audio, and
is referred to as temporal aliasing. Aliasing can also occur in spatially
sampled signals, for instance moirÃ©_patterns in digital_images. Aliasing in
spatially sampled signals is called spatial aliasing.
Aliasing is generally avoided by applying low_pass_filters or anti-aliasing
filters to the input signal before sampling. Suitable reconstruction_filters
should then be used when restoring the sampled signal to the continuous domain.
⁰
***** Contents *****
    * 1_Description
    * 2_Bandlimited_functions
    * 3_Bandpass_signals
    * 4_Sampling_sinusoidal_functions
          o 4.1_Folding
          o 4.2_Complex_sinusoids
          o 4.3_Sample_frequency
    * 5_Historical_usage
    * 6_Angular_aliasing
    * 7_More_examples
          o 7.1_Online_audio_example
          o 7.2_Direction_finding
    * 8_See_also
    * 9_Notes
    * 10_Citations
    * 11_Further_reading
***** Description[edit] *****
Left: An aliased image of the letter A in Times New Roman. Right: An anti-
aliased image. (See also: Font_rasterization)
When a digital image is viewed, a reconstruction is performed by a display or
printer device, and by the eyes and the brain. If the image data is processed
in some way during sampling or reconstruction, the reconstructed image will
differ from the original image, and an alias is seen.
An example of spatial aliasing is the moirÃ©_pattern observed in a poorly
pixelized image of a brick wall. Spatial_anti-aliasing techniques avoid such
poor pixelizations. Aliasing can be caused either by the sampling stage or the
reconstruction stage; these may be distinguished by calling sampling aliasing
prealiasing and reconstruction aliasing  postaliasing.[1]
Temporal aliasing is a major concern in the sampling of video and audio
signals. Music, for instance, may contain high-frequency components that are
inaudible to humans. If a piece of music is sampled at 32000 samples_per_second
(Hz), any frequency components at or above 16000 Hz (the Nyquist_frequency for
this sampling rate) will cause aliasing when the music is reproduced by a
digital-to-analog_converter (DAC). To prevent this, an anti-aliasing_filter is
used to remove components above the Nyquist frequency prior to sampling.
In video or cinematography, temporal aliasing results from the limited frame
rate, and causes the wagon-wheel_effect, whereby a spoked wheel appears to
rotate too slowly or even backwards. Aliasing has changed its apparent
frequency of rotation. A reversal of direction can be described as a negative
frequency. Temporal aliasing frequencies in video and cinematography are
determined by the frame rate of the camera, but the relative intensity of the
aliased frequencies is determined by the shutter timing (exposure time) or the
use of a temporal aliasing reduction filter during filming.[2][unreliable
source?]
Like the video camera, most sampling schemes are periodic; that is, they have a
characteristic sampling_frequency in time or in space. Digital cameras provide
a certain number of samples (pixels) per degree or per radian, or samples per
mm in the focal plane of the camera. Audio signals are sampled (digitized) with
an analog-to-digital_converter, which produces a constant number of samples per
second. Some of the most dramatic and subtle examples of aliasing occur when
the signal being sampled also has periodic content.
***** Bandlimited functions[edit] *****
Main article: NyquistâShannon_sampling_theorem
Actual signals have a finite duration and their frequency content, as defined
by the Fourier_transform, has no upper bound. Some amount of aliasing always
occurs when such functions are sampled. Functions whose frequency content is
bounded (bandlimited) have an infinite duration in the time domain. If sampled
at a high enough rate, determined by the bandwidth, the original function can,
in theory, be perfectly reconstructed from the infinite set of samples.
***** Bandpass signals[edit] *****
Main article: Undersampling
Sometimes aliasing is used intentionally on signals with no low-frequency
content, called bandpass signals. Undersampling, which creates low-frequency
aliases, can produce the same result, with less effort, as frequency-shifting
the signal to lower frequencies before sampling at the lower rate. Some digital
channelizers[3] exploit aliasing in this way for computational efficiency. See
Sampling_(signal_processing), Nyquist_rate_(relative_to_sampling), and Filter
bank.
***** Sampling sinusoidal functions[edit] *****
Sinusoids are an important type of periodic function, because realistic signals
are often modeled as the summation of many sinusoids of different frequencies
and different amplitudes (for example, with a Fourier_series or transform).
Understanding what aliasing does to the individual sinusoids is useful in
understanding what happens to their sum.
When sampling a function at frequency fs (intervals 1/fs), the following
functions yield identical sets of samples: {sin(2Ï( f+Nfs) t + Ï), N = 0,
Â±1, Â±2, Â±3,...}. A frequency_spectrum of the samples produces equally strong
responses at all those frequencies. Without collateral information, the
frequency of the original function is ambiguous. So the functions and their
frequencies are said to be aliases of each other. Noting the trigonometric
identity:
         sin &#x2061; ( 2 &#x03C0; ( f + N  f  s   ) t + &#x03D5; ) =  {     +
      sin &#x2061; ( 2 &#x03C0; ( f + N  f  s   ) t + &#x03D5; ) ,   f + N  f
      s   &#x2265; 0     &#x2212; sin &#x2061; ( 2 &#x03C0;  |  f + N  f  s
      |  t &#x2212; &#x03D5; ) ,   f + N  f  s   < 0         {\displaystyle
      \sin(2\pi (f+Nf_{s})t+\phi )=\left\{{\begin{array}{ll}+\sin(2\pi (f+Nf_
      {s})t+\phi ),&f+Nf_{s}\geq 0\\-\sin(2\pi |f+Nf_{s}|t-\phi ),&f+Nf_
      {s}<0\\\end{array}}\right.}  [{\displaystyle \sin(2\pi (f+Nf_{s})t+\phi
      )=\left\{{\begin{array}{ll}+\sin(2\pi (f+Nf_{s})t+\phi ),&f+Nf_{s}\geq
      0\\-\sin(2\pi |f+Nf_{s}|t-\phi ),&f+Nf_{s}<0\\\end{array}}\right.}]
we can write all the alias frequencies as positive values:  fN(f) Î= |f+N fs|
.
Two different sinusoids that fit the same set of samples.
For example, here a plot depicts a set of samples with parameter fs = 1, and
two different sinusoids that could have produced the samples. Nine cycles of
the red sinusoid and one cycle of the blue sinusoid span an interval of 10
samples. The corresponding number of cycles per sample are  fred = 0.9fs  and
 fblue = 0.1fs.  So the N = â1  alias of  fred  is  fblue  (and vice versa).
Aliasing matters when one attempts to reconstruct the original waveform from
its samples. The most common reconstruction technique produces the smallest of
the  fN(f)  frequencies. So it is usually important that  f0(f)  be the unique
minimum.  A necessary and sufficient condition for that is  fs/2 > |f|,  where
 fs/2  is commonly called the Nyquist_frequency of a system that samples at
rate  fs.  In our example, the Nyquist condition is satisfied if the original
signal is the blue sinusoid (f = fblue).  But if  f = fred = 0.9fs,  the usual
reconstruction method will produce the blue sinusoid instead of the red one.
**** Folding[edit] ****
In the example above,  fred  and  fblue  are symmetrical around the frequency
 fs/2.  And in general, as  f  increases from 0 to  fs/2,   fâ1(f)  decreases
from  fs  to  fs/2.  Similarly, as  f  increases from  fs/2  to  fs,   fâ1
(f)  continues decreasing from  fs/2  to 0.
A graph of amplitude vs frequency for a single sinusoid at frequency  0.6 fs 
and some of its aliases at  0.4 fs,  1.4 fs,  and  1.6 fs  would look like the
4 black dots in the first figure below. The red lines depict the paths (loci)
of the 4 dots if we were to adjust the frequency and amplitude of the sinusoid
along the solid red segment (between  fs/2  and  fs).  No matter what function
we choose to change the amplitude vs frequency, the graph will exhibit symmetry
between 0 and  fs.  This symmetry is commonly referred to as folding, and
another name for  fs/2  (the Nyquist frequency) is folding frequency. Folding
is often observed in practice when viewing the frequency_spectrum of real-
valued samples, such as the second figure below.
The black dots are aliases The Fourier transform of Graph of frequency
of each other. The solid   music sampled at 44100   aliasing, showing folding
red line is an example of  samples/sec exhibits     frequency and periodicity.
amplitude varying with     symmetry (called         Frequencies above fs/2 have
frequency. The dashed red  "folding") around the    an alias below fs/2, whose
lines are the              Nyquist frequency (22050 value is given by this
corresponding paths of the Hz).                     graph.
aliases.
Two complex sinusoids, colored gold and cyan, that fit the same sets of real
and imaginary sample points when sampled at the rate (fs) indicated by the grid
lines. The case shown here is: fcyan = fâ1(fgold) = fgold â fs
**** Complex sinusoids[edit] ****
Complex_sinusoids are waveforms whose samples are complex_numbers, and the
concept of negative_frequency is necessary to distinguish them. In that case,
the frequencies of the aliases are given by just:  fN(f) = f + N fs. 
Therefore, as  f  increases from  fs/2  to  fs,   fâ1(f)  goes from  âfs/2 
up to 0.  Consequently, complex sinusoids do not exhibit folding. Complex
samples of real-valued sinusoids have zero-valued imaginary parts and do
exhibit folding.
**** Sample frequency[edit] ****
Illustration of 4 waveforms reconstructed from samples taken at six different
rates. Two of the waveforms are sufficiently sampled to avoid aliasing at all
six rates. The other two illustrate increasing distortion (aliasing) at the
lower rates.
When the condition  fs/2 > f  is met for the highest frequency component of the
original signal, then it is met for all the frequency components, a condition
called the Nyquist_criterion. That is typically approximated by filtering the
original signal to attenuate high frequency components before it is sampled.
These attenuated high frequency components still generate low-frequency
aliases, but typically at low enough amplitudes that they do not cause
problems. A filter chosen in anticipation of a certain sample frequency is
called an anti-aliasing_filter.
The filtered signal can subsequently be reconstructed, by interpolation
algorithms, without significant additional distortion. Most sampled signals are
not simply stored and reconstructed. But the fidelity of a theoretical
reconstruction (via the WhittakerâShannon_interpolation_formula) is a
customary measure of the effectiveness of sampling.
***** Historical usage[edit] *****
Historically the term aliasing evolved from radio engineering because of the
action of superheterodyne_receivers. When the receiver shifts multiple signals
down to lower frequencies, from RF to IF by heterodyning, an unwanted signal,
from an RF frequency equally far from the local_oscillator (LO) frequency as
the desired signal, but on the wrong side of the LO, can end up at the same IF
frequency as the wanted one. If it is strong enough it can interfere with
reception of the desired signal. This unwanted signal is known as an image or
alias of the desired signal.
***** Angular aliasing[edit] *****
Aliasing occurs whenever the use of discrete elements to capture or produce a
continuous signal causes frequency ambiguity.
Spatial aliasing, particular of angular frequency, can occur when reproducing a
light_field[4] or sound field with discrete elements, as in 3D_displays or wave
field_synthesis of sound.
This aliasing is visible in images such as posters with lenticular_printing: if
they have low angular resolution, then as one moves past them, say from left-
to-right, the 2D image does not initially change (so it appears to move left),
then as one moves to the next angular image, the image suddenly changes (so it
jumps right) â and the frequency and amplitude of this side-to-side movement
corresponds to the angular resolution of the image (and, for frequency, the
speed of the viewer's lateral movement), which is the angular aliasing of the
4D light field.
The lack of parallax on viewer movement in 2D images and in 3-D_film produced
by stereoscopic glasses (in 3D films the effect is called "yawing", as the
image appears to rotate on its axis) can similarly be seen as loss of angular
resolution, all angular frequencies being aliased to 0 (constant).
***** More examples[edit] *****
**** Online audio example[edit] ****
The qualitative effects of aliasing can be heard in the following audio
demonstration. Six sawtooth_waves are played in succession, with the first two
sawtooths having a fundamental_frequency of 440 Hz (A4), the second two having
fundamental frequency of 880 Hz (A5), and the final two at 1760 Hz (A6). The
sawtooths alternate between bandlimited (non-aliased) sawtooths and aliased
sawtooths and the sampling rate is 22.05 kHz. The bandlimited sawtooths are
synthesized from the sawtooth waveform's Fourier_series such that no harmonics
above the Nyquist_frequency are present.
The aliasing distortion in the lower frequencies is increasingly obvious with
higher fundamental frequencies, and while the bandlimited sawtooth is still
clear at 1760 Hz, the aliased sawtooth is degraded and harsh with a buzzing
audible at frequencies lower than the fundamental.
 Sawtooth_aliasing_demo
 440 Hz bandlimited, 440 Hz aliased, 880 Hz bandlimited, 880 Hz aliased, 1760
 Hz bandlimited, 1760 Hz aliased
==============================================================================
Problems playing this file? See media_help.
**** Direction finding[edit] ****
A form of spatial aliasing can also occur in antenna arrays or microphone
arrays used to estimate the direction of arrival of a wave signal, as in
geophysical exploration by seismic waves. Waves must be sampled at more than
two points per wavelength, or the wave arrival direction becomes ambiguous.[5]
***** See also[edit] *****
 Wikimedia Commons has media related to Aliasing.
    * Brillouin_zone
    * Glossary_of_video_terms
    * Jaggies
    * Kell_factor
    * Sinc_filter
    * Sinc_function
    * Stroboscopic_effect
    * Wagon-wheel_effect
    * NyquistâShannon_sampling_theorem#Critical_frequency
***** Notes[edit] *****
***** Citations[edit] *****
   1. ^Mitchell, Don P.; Netravali, Arun N. (August 1988). Reconstruction
      filters_in_computer-graphics (PDF). ACM_SIGGRAPH_International_Conference
      on_Computer_Graphics_and_Interactive_Techniques. 22. pp. 221â228. doi:
      10.1145/54852.378514. ISBN 0-89791-275-6.
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
   3. ^ Tessive, LLC (2010)."Time_Filter_Technical_Explanation"
   4. ^harris, frederic j. (Aug 2006). Multirate Signal Processing for
      Communication Systems. Upper Saddle River, NJ: Prentice Hall PTR.
      ISBN 978-0-13-146511-4.
   5. ^ The_(New)_Stanford_Light_Field_Archive
   6. ^ Flanagan J.L., âBeamwidth and useable bandwidth of delay- steered
      microphone arraysâ, AT&T Tech. J., 1985, 64, pp. 983â995
***** Further reading[edit] *****
    * Matt Pharr; Greg Humphreys (28 June 2010). Physically_Based_Rendering:
      From_Theory_to_Implementation. Morgan Kaufmann.
ISBN 978-0-12-375079-2. Chapter_7_(Sampling_and_reconstruction). Retrieved 3
March 2013.
    * Aliasing_by_a_sampling_oscilloscope on YouTube by Tektronix Application
      Engineer
    * Anti-Aliasing_Filter_Primer by La Vida Leica discusses its purpose and
      effect on the image recorded.
    * Interactive_examples_demonstrating_the_aliasing_effect
    * v
    * t
    * e
Digital_signal_processing
               * Detection_theory
Theory         * Discrete_signal
               * Estimation_theory
               * NyquistâShannon_sampling_theorem
               * Audio_signal_processing
Sub-fields     * Digital_image_processing
               * Speech_processing
               * Statistical_signal_processing
               * Advanced_Z-transform
               * Bilinear_transform
               * Constant-Q_transform
               * Discrete_Fourier_transform (DFT)
               * Discrete-time_Fourier_transform (DTFT)
               * Impulse_invariance
Techniques     * Integral_transform
               * Laplace_transform
               * Matched_Z-transform_method
               * Post's_inversion_formula
               * Starred_transform
               * Z-transform
               * Zak_transform
               * Aliasing
               * Anti-aliasing_filter
               * Downsampling
               * Nyquist_rate / frequency
Sampling       * Oversampling
               * Quantization
               * Sampling_rate
               * Undersampling
               * Upsampling

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Aliasing&oldid=900450440"
Categories:
    * Digital_signal_processing
    * Signal_processing
Hidden categories:
    * Use_American_English_from_March_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * All_articles_lacking_reliable_references
    * Articles_lacking_reliable_references_from_July_2018
    * Articles_with_hAudio_microformats
    * Commons_category_link_is_on_Wikidata
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
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Italiano
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 5 June 2019, at 19:20 (UTC).
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
