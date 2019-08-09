The following text has been accessed from https://en.wikipedia.org/wiki/Nyquist_frequency at Thu Aug 8 23:22:57 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Nyquist frequency ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Important in signal processing and sampling
Not to be confused with Nyquist_rate.
Fig 1. The black dots are aliases of each other. The solid red line is an
example of adjusting amplitude vs frequency. The dashed red lines are the
corresponding paths of the aliases.
The Nyquist frequency, named after electronic engineer Harry_Nyquist, is half
of the sampling_rate of a discrete_signal processing system.[1][2] It is
sometimes known as the folding_frequency of a sampling system.[3]  An example
of folding is depicted in Figure 1, where fs is the sampling rate and 0.5 fs is
the corresponding Nyquist frequency.[note_1]  The black dot plotted at 0.6 fs
represents the amplitude and frequency of a sinusoidal function whose frequency
is 60% of the sample-rate (fs). The other three dots indicate the frequencies
and amplitudes of three other sinusoids that would produce the same set of
samples as the actual sinusoid that was sampled. The symmetry about 0.5 fs is
referred to as folding.
The Nyquist frequency should not be confused with the Nyquist_rate, the latter
is the minimum sampling rate that satisfies the Nyquist_sampling_criterion for
a given signal or family of signals. The Nyquist rate is twice the maximum
component frequency of the function being sampled. For example, the Nyquist
rate for the sinusoid at 0.6 fs is 1.2 fs, which means that at the fs rate, it
is being undersampled. Thus, Nyquist rate is a property of a continuous-time
signal, whereas Nyquist frequency is a property of a discrete-time system.[4]
[5]
When the function domain is time, sample rates are usually expressed in samples
per_second, and the unit of Nyquist frequency is cycles_per_second (hertz).
When the function domain is distance, as in an image sampling system, the
sample rate might be dots per inch and the corresponding Nyquist frequency
would be in cycles/inch.
⁰
***** Contents *****
    * 1_Aliasing
    * 2_Other_meanings
    * 3_Notes
    * 4_Citations
***** Aliasing[edit] *****
Main article: Aliasing
Referring again to Figure 1, undersampling of the sinusoid at 0.6 fs is what
allows there to be a lower-frequency alias, which is a different function that
produces the same set of samples. That condition is usually described as
aliasing. The mathematical algorithms that are typically used to recreate a
continuous function from its samples will misinterpret the contributions of
undersampled frequency components, which causes distortion. Samples of a pure
0.6 fs sinusoid would produce a 0.4 fs sinusoid instead. If the true frequency
was 0.4 fs, there would still be aliases at 0.6, 1.4, 1.6, etc.,[note_2] but
the reconstructed frequency would be correct.
In a typical application of sampling, one first chooses the highest frequency
to be preserved and recreated, based on the expected content (voice, music,
etc.) and desired fidelity. Then one inserts an anti-aliasing_filter ahead of
the sampler. Its job is to attenuate the frequencies above that limit. Finally,
based on the characteristics of the filter, one chooses a sample-rate (and
corresponding Nyquist frequency) that will provide an acceptably small amount
of aliasing.
In applications where the sample-rate is pre-determined, the filter is chosen
based on the Nyquist frequency, rather than vice versa. For example, audio CDs
have a sampling rate of 44100 samples/sec. The Nyquist frequency is therefore
22050 Hz. The anti-aliasing filter must adequately suppress any higher
frequencies but negligibly affect the frequencies within the human hearing
range. A filter that preserves 0â20 kHz is more than adequate for that.
***** Other meanings[edit] *****
Early uses of the term Nyquist frequency, such as those cited above, are all
consistent with the definition presented in this article. Some later
publications, including some respectable textbooks, call twice the signal
bandwidth the Nyquist frequency;[6][7] this is a distinctly minority usage, and
the frequency at twice the signal bandwidth is otherwise commonly referred to
as the Nyquist_rate.
***** Notes[edit] *****
   1. ^ In this context, the factor of Â½ has units of cycles per sample, as
      explained at Aliasing#Sampling_sinusoidal_functions.
   2. ^ As previously mentioned, these are the frequencies of other sinusoids
      that would produce the same set of samples as the one that was actually
      sampled.
***** Citations[edit] *****
   1. ^Grenander,_Ulf (1959). Probability_and_Statistics:_The_Harald_CramÃ©r
      Volume. Wiley. The Nyquist frequency is that frequency whose period is
      two sampling intervals.
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
   3. ^Harry L. Stiltz (1961). Aerospace_Telemetry. Prentice-Hall. the
      existence of power in the continuous signal spectrum at frequencies
      higher than the Nyquist frequency is the cause of aliasing error
   4. ^Thomas Zawistowski; Paras Shah. "An_Introduction_to_Sampling_Theory".
      Retrieved 17 April 2010. Frequencies "fold" around half the sampling
      frequency - which is why [the Nyquist] frequency is often referred to as
      the folding frequency.
   5. ^James J. Condon & Scott M. Ransom (2016). Essential_Radio_Astronomy.
      Princeton University Press. pp. 280â281. ISBN 9781400881161.
   6. ^John W. Leis (2011). Digital_Signal_Processing_Using_MATLAB_for_Students
      and_Researchers. John Wiley & Sons. p. 82. ISBN 9781118033807. The
      Nyquist rate is twice the bandwidth of the signal ... The Nyquist
      frequency or folding frequency is half the sampling rate and corresponds
      to the highest frequency which a sampled data system can reproduce
      without error.
   7. ^Jonathan M. Blackledge (2003). Digital_Signal_Processing:_Mathematical
      and_Computational_Methods,_Software_Development_and_Applications. Horwood
      Publishing. ISBN 1-898563-48-9.
   8. ^Paulo Sergio Ramirez Diniz, Eduardo A. B. Da Silva, Sergio L. Netto
      (2002). Digital_Signal_Processing:_System_Analysis_and_Design. Cambridge
      University Press. ISBN 0-521-78175-2.CS1 maint: Multiple names: authors
      list (link)
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
index.php?title=Nyquist_frequency&oldid=885610729"
Categories:
    * Digital_signal_processing
Hidden categories:
    * CS1_maint:_Multiple_names:_authors_list
    * Use_American_English_from_March_2019
    * All_Wikipedia_articles_written_in_American_English
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * AzÉrbaycanca
    * Dansk
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * ×¢××¨××ª
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 1 March 2019, at 03:51 (UTC).
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
