The following text has been accessed from https://en.wikipedia.org/wiki/In-phase_and_quadrature_components at Thu Aug 8 23:23:03 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** In-phase and quadrature components ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For the colourspace components, see YIQ.
Graphic example of the formula        cos &#x2061; ( 2 &#x03C0; f t + &#x03D5;
( t ) )   &#xA0; = &#xA0;   cos &#x2061; ( 2 &#x03C0; f t ) cos &#x2061;
( &#x03D5; ( t ) )   &#xA0; + &#xA0;   cos &#x2061; ( 2 &#x03C0; f t + &#x03C0;
/  2 ) sin &#x2061; ( &#x03D5; ( t ) )   .    {\displaystyle \scriptstyle
{\color {Green}\cos(2\pi ft+\phi (t))}\ =\ {\color {Blue}\cos(2\pi ft)\cos(\phi
(t))}\ +\ {\color {Red}\cos(2\pi ft+\pi /2)\sin(\phi (t))}.}  [{\displaystyle
\scriptstyle {\color {Green}\cos(2\pi ft+\phi (t))}\ =\ {\color {Blue}\cos(2\pi
ft)\cos(\phi (t))}\ +\ {\color {Red}\cos(2\pi ft+\pi /2)\sin(\phi (t))}.}] The
phase modulation (Ï(t), not shown) is a non-linearly increasing function from
0 to Ï/2 over the interval 0 < t < 16. The two amplitude-modulated components
are known as the in-phase component (I, thin blue, decreasing) and the
quadrature component (Q, thin red, increasing).
In electrical_engineering, a sinusoid with angle_modulation can be decomposed
into, or synthesized from, two amplitude-modulated sinusoids that are offset in
phase by one-quarter cycle (Ï/2 radians). All three functions have the same
frequency. The amplitude modulated sinusoids are known as in-phase and
quadrature components.[1]  In some contexts it is more convenient to refer to
only the amplitude modulation (baseband) itself by those terms.[2]
⁰
***** Contents *****
    * 1_Concept
          o 1.1_Alternating_current_(AC)_circuits
          o 1.2_Narrowband_signal_model
    * 2_See_also
    * 3_References
    * 4_Further_reading
    * 5_External_links
***** Concept[edit] *****
See also: List_of_trigonometric_identities_Â§ Linear_combinations
In vector analysis, a vector with polar coordinates A,Ï and Cartesian
coordinates x = A cos(Ï), y = A sin(Ï), can be represented as the sum of
orthogonal "components": [x,0] + [0,y]. Similarly in trigonometry, the
expression sin(x + Ï) can be represented by sin(x) cos(Ï) + sin(x + Ï/2) sin
(Ï). And in functional analysis, when x is a linear function of some variable,
such as time, these components are sinusoids, and they are orthogonal
functions. When Ï = 0, sin(x + Ï) reduces to just the in-phase component, sin
(x) cos(Ï), and the quadrature component, sin(x + Ï/2) sin(Ï), is zero. A
phase-shift of x â x + Ï/2 changes the identity to cos(x + Ï) = cos(x) cos
(Ï) + cos(x + Ï/2) sin(Ï), in which case cos(x) cos(Ï) is the in-phase
component. In both conventions cos(Ï) is the in-phase amplitude modulation,
which explains why some authors refer to it as the actual in-phase component.
We can also observe that in both conventions the quadrature component leads the
in-phase component by one-quarter cycle.
When a sinusoidal voltage is applied to either a simple capacitor or inductor,
the resultant current that flows is "in quadrature" with the voltage.
**** Alternating current (AC) circuits[edit] ****
The term alternating current applies to a voltage vs. time function that is
sinusoidal with a frequency f.  When it is applied to a typical circuit or
device, it causes a current that is also sinusoidal. In general there is a
constant phase difference, Ï, between any two sinusoids. The input sinusoidal
voltage is usually defined to have zero phase, meaning that it is arbitrarily
chosen as a convenient time reference. So the phase difference is attributed to
the current function, e.g. sin(2Ïft + Ï), whose orthogonal components are sin
(2Ïft) cos(Ï) and sin(2Ïft + Ï/2) sin(Ï), as we have seen. When Ï happens
to be such that the in-phase component is zero, the current and voltage
sinusoids are said to be in quadrature, which means they are orthogonal to each
other. In that case, no electrical power is consumed. Rather it is temporarily
stored by the device and given back, once every &#x200b;1⁄f  seconds. Note that
the term in quadrature only implies that two sinusoids are orthogonal, not that
they are components of another sinusoid.
**** Narrowband signal model[edit] ****
In an angle modulation application, with carrier_frequency f, Ï is also a
time-variant function, giving:
         sin &#x2061; [ 2 &#x03C0; f t + &#x03D5; ( t ) ] &#xA0; = &#xA0;
      sin &#x2061; ( 2 &#x03C0; f t ) &#x22C5; cos &#x2061; [ &#x03D5; ( t ) ]
      &#x23DF;    in-phase    +          sin &#x2061;  (  2 &#x03C0; f t +
      &#x03C0; 2     )   &#x23DE;    cos &#x2061; ( 2 &#x03C0; f t )   &#x22C5;
      sin &#x2061; [ &#x03D5; ( t ) ]  &#x23DF;    quadrature   .
      {\displaystyle \sin[2\pi ft+\phi (t)]\ =\ \underbrace {\sin(2\pi ft)\cdot
      \cos[\phi (t)]} _{\text{in-phase}}\,+\,\underbrace {\overbrace {\sin
      \left(2\pi ft+{\tfrac {\pi }{2}}\right)} ^{\cos(2\pi ft)}\cdot \sin[\phi
      (t)]} _{\text{quadrature}}.}  [{\displaystyle \sin[2\pi ft+\phi (t)]\ =\
      \underbrace {\sin(2\pi ft)\cdot \cos[\phi (t)]} _{\text{in-
      phase}}\,+\,\underbrace {\overbrace {\sin \left(2\pi ft+{\tfrac {\pi }
      {2}}\right)} ^{\cos(2\pi ft)}\cdot \sin[\phi (t)]} _{\text
      {quadrature}}.}]
When all three terms above are multiplied by an optional amplitude function, A
(t) > 0, the left-hand side of the equality is known as the amplitude/phase
form, and the right-hand side is the quadrature-carrier or IQ form. Because of
the modulation, the components are no longer completely orthogonal functions.
But when A(t) and Ï(t) are slowly varying functions compared to 2Ïft, the
assumption of orthogonality is a common one. Authors often call it a narrowband
assumption, or a narrowband signal model.[3][4]  Orthogonality is important in
many applications, including demodulation, direction-finding, and bandpass
sampling.
***** See also[edit] *****
    * IQ_imbalance
    * Constellation_diagram
    * Phasor
    * Polar_modulation
    * Quadrature_amplitude_modulation
    * Single-sideband_modulation
***** References[edit] *****
   1. ^Gast, Matthew (2005-05-02). 802.11 Wireless Networks: The Definitive
      Guide. 1 (2 ed.). Sebastopol,CA: O'Reilly Media. p. 284. ISBN 0596100523.
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
   3. ^ Franks, L.E. (September 1969). Signal Theory. Information theory.
      Englewood Cliffs, NJ: Prentice Hall. p. 82. ISBN 0138100772.
   4. ^ Wade, Graham (1994-09-30). Signal Coding and Processing. 1 (2 ed.).
      Cambridge University Press. p. 10. ISBN 0521412307.
   5. ^ Naidu, Prabhakar S. (November 2003). Modern Digital Signal Processing:
      An Introduction. Pangbourne RG8 8UT, UK: Alpha Science Intl Ltd.
      pp. 29â31. ISBN 1842651331.
***** Further reading[edit] *****
    * Steinmetz, Charles Proteus (2003-02-20). Lectures on Electrical
      Engineering. 3 (1 ed.). Mineola,NY: Dover Publications. ISBN 0486495388.
Steinmetz, Charles Proteus (1917). Theory and Calculations of Electrical
Apparatus 6 (1 ed.). New York: McGraw-Hill Book Company. B004G3ZGTM.
***** External links[edit] *****
    * I/Q_Data_for_Dummies
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

Retrieved from "https://en.wikipedia.org/w/index.php?title=In-
phase_and_quadrature_components&oldid=876639964"
Categories:
    * Signal_processing
    * Radio_electronics
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
    * Deutsch
    * EspaÃ±ol
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 3 January 2019, at 15:17 (UTC).
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
