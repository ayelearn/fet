The following text has been accessed from https://en.wikipedia.org/wiki/Signal_generator at Fri Aug 9 01:27:14 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Signal generator ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Tone generator" redirects here. For an electronic musical instrument, see
Sound_module.
A signal generator is an electronic device that generates repeating or non-
repeating electronic signals in either the analog or the digital domain. It is
generally used in designing, testing, troubleshooting, and repairing electronic
or electroacoustic devices, though it often has artistic uses as well.
There are many different types of signal generators with different purposes and
applications and at varying levels of expense. These types include function
generators, RF and microwave signal generators, pitch generators, arbitrary
waveform_generators, digital_pattern_generators and frequency generators. In
general, no device is suitable for all possible applications.
Traditionally, signal generators have been embedded hardware units, but since
the age of multimedia PCs, flexible, programmable software tone generators have
also been available.
⁰
***** Contents *****
    * 1_History
    * 2_General_purpose_signal_generators
          o 2.1_Function_generator
          o 2.2_Arbitrary_waveform_generator
                # 2.2.1_Technical_trends_driving_the_ARB_industry
          o 2.3_RF_and_microwave_signal_generators
                # 2.3.1_Analog_signal_generators
                # 2.3.2_Vector_signal_generator
                # 2.3.3_Digital_pattern_generator
    * 3_Special_purpose_signal_generators
          o 3.1_Pitch_generators_and_audio_generators
                # 3.1.1_Computer_programs
          o 3.2_Video_signal_generator
    * 4_See_also
    * 5_References
    * 6_External_links
***** History[edit] *****
In June 1928, the General_Radio 403, was the first commercial signal generator
ever marketed. It supported a frequency range of 500Hz to 1.5MHz.[1] Also, in
April 1929, the first commercial frequency standard was marketed by General
Radio with a frequency of 50KHz.[2]
***** General purpose signal generators[edit] *****
**** Function generator[edit] ****
Leader_Instruments LSG-15 signal generator
Main article: Function_generator
A function_generator is a device which produces simple repetitive waveforms.
Such devices contain an electronic_oscillator, a circuit that is capable of
creating a repetitive waveform. (Modern devices may use digital_signal
processing to synthesize waveforms, followed by a digital_to_analog_converter,
or DAC, to produce an analog output). The most common waveform is a sine_wave,
but sawtooth, step (pulse), square, and triangular waveform oscillators are
commonly available as are arbitrary_waveform_generators (AWGs). If the
oscillator operates above the audio_frequency range (>20 kHz), the generator
will often include some sort of modulation function such as amplitude
modulation (AM), frequency_modulation (FM), or phase_modulation (PM) as well as
a second oscillator that provides an audio_frequency modulation waveform.
**** Arbitrary waveform generator[edit] ****
Main article: Arbitrary_waveform_generator
An arbitrary waveform generator (AWG or ARB) is a sophisticated signal
generator that generates arbitrary waveforms within published limits of
frequency range, accuracy, and output level. Unlike a function generator that
produces a small set of specific waveforms, an AWG allows the user to specify a
source waveform in a variety of different ways. An AWG is generally more
expensive than a function generator and often has less bandwidth. An AWG is
used in higher-end design and test applications.
*** Technical trends driving the ARB industry[edit] ***
New high-speed DACs provide up to 16-bit resolution at sample rates in excess
of 1 GS/s. These devices provide the foundation for an AWG with the bandwidth
and dynamic range to address modern radio and communication applications. In
combination with a quadrature modulator and advanced digital signal processing,
high-speed DACs can be applied to create a full-featured vector signal
generator with very high modulation bandwidth. Example applications include
commercial wireless standards such as Wi-Fi (IEEE 802.11), WiMAX (IEEE 802.16)
and LTE, in addition to military standards such as those specified in the Joint
Tactical Radio System (JTRS) initiative. Also, broad modulation bandwidth
allows multi-carrier signal generation, necessary for testing receiver adjacent
channel rejection.
**** RF and microwave signal generators[edit] ****
RF_(radio_frequency) and microwave signal generators are used for testing
components, receivers and test systems in a wide variety of applications
including cellular communications, WiFi, WiMAX, GPS, audio and video
broadcasting, satellite communications, radar and electronic_warfare. RF and
microwave signal generators normally have similar features and capabilities,
but are differentiated by frequency range. RF signal generators typically range
from a few kHz to 6 GHz, while microwave signal generators cover a much wider
frequency range, from less than 1 MHz to at least 20 GHz. Some models go as
high as 70 GHz with a direct coaxial output, and up to hundreds of GHz when
used with external waveguide source modules. RF and microwave signal generators
can be classified further as analog or vector signal generators.
*** Analog signal generators[edit] ***
An analog RF signal generator
Analog signal generators based on a sine-wave oscillator were common before the
inception of digital electronics, and are still used. There was a sharp
distinction in purpose and design of radio-frequency and audio-frequency signal
generators.
  RF
RF signal generators are capable of producing CW_(continuous_wave) tones. The
output frequency can usually be tuned anywhere in their frequency range. Many
models offer various types of analog modulation, either as standard equipment
or as an optional capability to the base unit. This could include AM, FM, Î¦M_
(phase_modulation) and pulse_modulation. Another common feature is a built-in
attenuator which makes it possible to vary the signalâs output power.
Depending on the manufacturer and model, output powers can range from -135 to
+30 dBm. A wide range of output power is desirable, since different
applications require different amounts of signal power. For example, if a
signal has to travel through a very long cable out to an antenna, a high output
signal may be needed to overcome the losses through the cable and still have
sufficient power at the antenna. But when testing receiver sensitivity, a low
signal level is required to see how the receiver behaves under low signal-to-
noise conditions.
RF signal generators are available as benchtop instruments, rackmount
instruments, embeddable modules and in card-level formats. Mobile, field-
testing and airborne applications benefit from lighter, battery-operated
platforms. In automated and production testing, web-browser access, which
allows multi-source control, and faster frequency switching speeds improve test
times and throughput.
RF signal generators are required for servicing and setting up analog radio
receivers, and are used for professional RF applications.
  AF
Audio-frequency signal generators generate signals in the audio-frequency range
and above. An early example was the HP200A Audio Oscillator, the first product
sold by the Hewlett-Packard_Company in 1939. Applications include checking
frequency response of audio equipment, and many uses in the electronic
laboratory.
Equipment distortion can be measured using a very-low-distortion audio
generator as the signal source, with appropriate equipment to measure output
distortion harmonic-by-harmonic with a wave_analyser, or simply total_harmonic
distortion. A distortion of 0.0001% can be achieved by an audio signal
generator with a relatively simple circuit.[3]
*** Vector signal generator[edit] ***
A vector signal generator
With the advent of digital communications systems, it is no longer possible to
adequately test these systems with traditional analog signal generators. This
has led to the development of the vector signal generator, which is also known
as a digital signal generator. These signal generators are capable of
generating digitally-modulated radio signals that may use any of a large number
of digital_modulation formats such as QAM, QPSK, FSK, BPSK, and OFDM. In
addition, since modern commercial digital communication systems are almost all
based on well-defined industry standards, many vector signal generators can
generate signals based on these standards. Examples include GSM, W-CDMA_(UMTS),
CDMA2000, LTE, Wi-Fi_(IEEE_802.11), and WiMAX_(IEEE_802.16). In contrast,
military communication systems such as JTRS, which place a great deal of
importance on robustness and information security, typically use very
proprietary methods. To test these types of communication systems, users will
often create their own custom waveforms and download them into the vector
signal generator to create the desired test signal.
*** Digital pattern generator[edit] ***
Main article: Digital_pattern_generator
A logic signal generator or data pattern generator or digital_pattern_generator
produces logic signals - that is logical 1s and 0s in the form of conventional
voltage levels. The usual voltage standards are: LVTTL, LVCMOS. It is different
from a "pulse/pattern generator", which refers to signal generators able to
generate logic pulses with different analog characteristics (such as pulse
rise/fall time, high level length, ...).
A digital pattern generator is used as stimulus source for digital integrated
circuits and embedded systems - for functional validation and testing.
***** Special purpose signal generators[edit] *****
A pitch generator and a probe for locating a specific pair of wires amongst
many, for example in a punch_block.
In addition to the above general-purpose devices, there are several classes of
signal generators designed for specific applications.
**** Pitch generators and audio generators[edit] ****
A pitch generator is a type of signal generator optimized for use in audio and
acoustics applications. Pitch generators typically include sine waves over the
audio_frequency range (20 Hz–20 kHz). Sophisticated pitch generators will also
include sweep generators (a function which varies the output frequency over a
range, in order to make frequency-domain measurements), multipitch generators
(which output several pitches simultaneously, and are used to check for
intermodulation_distortion and other non-linear effects), and tone bursts (used
to measure response to transients). Pitch generators are typically used in
conjunction with sound_level_meters, when measuring the acoustics of a room or
a sound reproduction system, and/or with oscilloscopes or specialized audio
analyzers.
Many pitch generators operate in the digital domain, producing output in
various digital audio formats such as AES3, or SPDIF. Such generators may
include special signals to stimulate various digital effects and problems, such
as clipping, jitter, bit_errors; they also often provide ways to manipulate the
metadata associated with digital audio formats.
The term synthesizer is used for a device that generates audio signals for
music, or that uses slightly more intricate methods.
*** Computer programs[edit] ***
Computer_programs can be used to generate arbitrary waveforms on a general-
purpose computer and output the waveform via an output interface. Such programs
may be provided commercially or be freeware. Simple systems use a standard
computer sound_card as output device, limiting the accuracy of the output
waveform and limiting frequency to lie within the audio-frequency band.
**** Video signal generator[edit] ****
Main article: Video_signal_generator
A video signal generator is a device which outputs predetermined video and/or
television waveforms, and other signals used to stimulate faults in, or aid in
parametric measurements of, television and video systems. There are several
different types of video signal generators in widespread use. Regardless of the
specific type, the output of a video generator will generally contain
synchronization signals appropriate for television, including horizontal and
vertical sync pulses (in analog) or sync words (in digital). Generators of
composite video signals (such as NTSC and PAL) will also include a colorburst
signal as part of the output. Video signal generators are available for a wide
variety of applications, and for a wide variety of digital formats; many of
these also include audio generation capability (as the audio track is an
important part of any video or television program or motion picture).
***** See also[edit] *****
    * A/N_URM-25D_Signal_Generator, 1950s hardware still in use today.
    * Digital_Pattern_Generator, for generating digital (logic) type of signals
***** References[edit] *****
   1. ^Burke, Charles (March 1930). "The_Standard-Signal_Method_of_Measuring
      Receiver_Characteristics" (PDF). General_Radio. Archived (PDF) from the
      original on December 18, 2018. Experimenter - Issue Vol. IV, No. 10
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
   3. ^Thiessen, Arthur (1965). "A_History_of_the_General_Radio_Company_1915-
      1965" (PDF). General_Radio. Archived (PDF) from the original on December
      18, 2018.
   4. ^ Capacitor_Sounds_1_-_Low_Distortion_(sub_1PPM_)_1_kHz_Test_Oscillator,
      C_Bateman,_Electronics_World_July_2002,_expanded_March_2003. Description,
      measurements, circuit, and PCB layout
***** External links[edit] *****
 Wikimedia Commons has media related to Signal_generators.
    * Function_Generator_&_Arbitrary_Waveform_Generator_Guidebook
    * Understanding_signal_generator_specifications
    * Waveform_Generator_Fundamentals at Archive.today (archived 2012-12-08)
    * Blog_Post:_All_About_ABRS_(Waveform_Generators) at the Wayback_Machine
      (archived 2011-07-18)
    * v
    * t
    * e
Electrical_and_electronic_measuring_equipment
               * Ammeter
               * Capacitance_meter
               * Distortionmeter
               * Electricity_meter
               * Frequency_counter
               * Galvanometer
               * LCR_meter
               * Microwave_power_meter
               * Multimeter
               * Megohmmeter
Metering       * Ohmmeter
               * Peak_meter
               * Peak_programme_meter
               * Psophometer
               * Q_meter
               * Time-domain_reflectometer
               * Time-to-digital_converter
               * Transistor_tester
               * Tube_tester
               * Wattmeter
               * Voltmeter
               * VU_meter
               * Bus_analyzer
               * Logic_analyzer
               * Network_analyzer
               * Oscilloscope
Analysis       * Signal_analyzer
               * Spectrum_analyzer
               * Waveform_monitor
               * Vectorscope
               * Videoscope
               * Arbitrary_waveform_generator
               * Digital_pattern_generator
Generation     * Function_generator
               * Sweep_generator
               * Signal generator
               * Video-signal_generator
Authority_control [Edit_this_at_Wikidata]     * GND: 4181270-0

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Signal_generator&oldid=878195557"
Categories:
    * Laboratory_equipment
    * Electronic_test_equipment
Hidden categories:
    * Commons_category_link_is_on_Wikidata
    * Webarchive_template_archiveis_links
    * Webarchive_template_wayback_links
    * Wikipedia_articles_with_GND_identifiers
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
    * Eesti
    * EspaÃ±ol
    * Italiano
    * Nederlands
    * æ¥æ¬èª
    * PortuguÃªs
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * ä¸­æ
Edit_links
    * This page was last edited on 13 January 2019, at 16:40 (UTC).
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
