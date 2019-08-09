The following text has been accessed from https://en.wikipedia.org/wiki/Pulse-code_modulation at Fri Aug 9 01:22:58 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Pulse-code modulation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"PCM" redirects here. For other uses, see PCM_(disambiguation).
                            Pulse-code modulation
Filename_extension  .L16, .WAV, .AIFF, .AU, .PCM[1]
Internet_media typeaudio/L16, audio/L8,[2] audio/L20, audio/L24[3][4]
Type_code           "AIFF" for L16,[1] none[3]
Magic_number        Varies
Type of format      Uncompressed audio
Contained by       Audio_CD, AES3, WAV, AIFF, AU, M2TS, VOB, and many others
Extended from      PCM
Passband modulation
Analog_modulation
    * AM
    * FM
    * PM
    * QAM
    * SM
    * SSB
Digital_modulation
    * ASK
    * APSK
    * CPM
    * FSK
    * MFSK
    * MSK
    * OOK
    * PPM
    * PSK
    * QAM
    * SC-FDE
    * TCM
    * WDM
Hierarchical_modulation
    * QAM
    * WDM
Spread_spectrum
    * CSS
    * DSSS
    * FHSS
    * THSS
See also
    * Capacity-approaching_codes
    * Demodulation
    * Line_coding
    * Modem
    * AnM
    * PoM
    * PAM
    * PCM
    * PWM
    * ÎÎ£M
    * OFDM
    * FDM
    * Multiplexing
    * v
    * t
    * e
Pulse-code modulation (PCM) is a method used to digitally represent sampled
analog_signals. It is the standard form of digital_audio in computers, compact
discs, digital_telephony and other digital audio applications. In a PCM stream,
the amplitude of the analog signal is sampled regularly at uniform intervals,
and each sample is quantized to the nearest value within a range of digital
steps.
Linear pulse-code modulation (LPCM) is a specific type of PCM where the
quantization levels are linearly uniform.[5] This is in contrast to PCM
encodings where quantization levels vary as a function of amplitude (as with
the A-law_algorithm or the Î¼-law_algorithm). Though PCM is a more general
term, it is often used to describe data encoded as LPCM.
A PCM stream has two basic properties that determine the stream's fidelity to
the original analog signal: the sampling_rate, which is the number of times per
second that samples are taken; and the bit_depth, which determines the number
of possible digital values that can be used to represent each sample.
⁰
***** Contents *****
    * 1_History
    * 2_Implementations
    * 3_Modulation
    * 4_Demodulation
    * 5_Standard_sampling_precision_and_rates
    * 6_Limitations
    * 7_Processing_and_coding
    * 8_Encoding_for_serial_transmission
    * 9_Nomenclature
    * 10_See_also
    * 11_Notes
    * 12_References
    * 13_Further_reading
    * 14_External_links
***** History[edit] *****
Early electrical communications started to sample signals in order to multiplex
samples from multiple telegraphy sources and to convey them over a single
telegraph cable. The American inventor Moses_G._Farmer conveyed telegraph time-
division_multiplexing (TDM) as early as 1853. Electrical engineer W. M. Miner,
in 1903, used an electro-mechanical commutator for time-division multiplexing
multiple telegraph signals; he also applied this technology to telephony. He
obtained intelligible speech from channels sampled at a rate above
3500â4300 Hz; lower rates proved unsatisfactory.
In 1920, the Bartlane_cable_picture_transmission_system used telegraph
signaling of characters punched in paper tape to send samples of images
quantized to 5 levels.[6] In 1926, Paul M. Rainey of Western_Electric patented
a facsimile_machine which transmitted its signal using 5-bit PCM, encoded by an
opto-mechanical analog-to-digital_converter.[7] The machine did not go into
production.[8]
British engineer Alec_Reeves, unaware of previous work, conceived the use of
PCM for voice communication in 1937 while working for International_Telephone
and_Telegraph in France. He described the theory and advantages, but no
practical application resulted. Reeves filed for a French patent in 1938, and
his US patent was granted in 1943.[9] By this time Reeves had started working
at the Telecommunications_Research_Establishment.[8]
The first transmission of speech by digital techniques, the SIGSALY encryption
equipment, conveyed high-level Allied_communications during World_War_II. In
1943 the Bell_Labs researchers who designed the SIGSALY system became aware of
the use of PCM binary coding as already proposed by Reeves. In 1949, for the
Canadian Navy's DATAR system, Ferranti_Canada built a working PCM radio system
that was able to transmit digitized radar data over long distances.[10]
PCM in the late 1940s and early 1950s used a cathode-ray coding_tube with a
plate_electrode having encoding perforations.[11] As in an oscilloscope, the
beam was swept horizontally at the sample rate while the vertical deflection
was controlled by the input analog signal, causing the beam to pass through
higher or lower portions of the perforated plate. The plate collected or passed
the beam, producing current variations in binary code, one bit at a time.
Rather than natural binary, the grid of Goodall's later tube was perforated to
produce a glitch-free Gray_code, and produced all bits simultaneously by using
a fan beam instead of a scanning beam.[12]
In the United States, the National_Inventors_Hall_of_Fame has honored Bernard
M._Oliver[13] and Claude_Shannon[14] as the inventors of PCM,[15] as described
in "Communication System Employing Pulse Code Modulation", U.S._Patent
2,801,281 filed in 1946 and 1952, granted in 1956. Another patent by the same
title was filed by John_R._Pierce in 1945, and issued in 1948: U.S._Patent
2,437,707. The three of them published "The Philosophy of PCM" in 1948.[16]
The T-carrier system, introduced in 1961, uses two twisted-pair transmission
lines to carry 24 PCM telephone calls sampled at 8 kHz and 8-bit resolution.
This development improved capacity and call quality compared to the previous
frequency-division_multiplexing schemes.
In 1967, the first PCM recorder was developed by NHK's research facilities in
Japan.[17] The 30 kHz 12-bit device used a compander (similar to DBX_Noise
Reduction) to extend the dynamic range, and stored the signals on a video_tape
recorder. In 1969, NHK expanded the system's capabilities to 2-channel stereo
and 32 kHz 13-bit resolution. In January 1971, using NHK's PCM recording
system, engineers at Denon recorded the first commercial digital recordings.
[note_1][17]
In 1972, Denon unveiled the first 8-channel digital recorder, the DN-023R,
which used a 4-head open reel broadcast video_tape_recorder to record in 47.25
kHz, 13-bit PCM audio.[note_2] In 1977, Denon developed the portable PCM
recording system, the DN-034R. Like the DN-023R, it recorded 8 channels at
47.25 kHz, but it used 14-bits "with emphasis, making it equivalent to 15.5
bits."[17]
In 1973, adaptive_differential_pulse-code_modulation (ADPCM) was developed, by
P. Cummiskey, Nikil_Jayant and James_L._Flanagan.[18]
The compact_disc (CD) brought PCM to consumer audio applications with its
introduction in 1982. The CD uses a 44,100_Hz sampling frequency and 16-bit
resolution and stores up to 80 minutes of stereo audio per disc.
***** Implementations[edit] *****
PCM is the method of encoding typically used for uncompressed digital audio.
[note_3]
    * The 4ESS_switch introduced time-division switching into the US telephone
      system in 1976, based on medium scale integrated circuit technology.[19]
    * LPCM is used for the lossless encoding of audio data in the Compact disc
      Red_Book_standard (informally also known as Audio CD), introduced in
      1982.
    * AES3 (specified in 1985, upon which S/PDIF is based) is a particular
      format using LPCM.
    * LaserDiscs with digital sound have an LPCM track on the digital channel.
    * On PCs, PCM and LPCM often refer to the format used in WAV (defined in
      1991) and AIFF audio container formats (defined in 1988). LPCM data may
      also be stored in other formats such as AU, raw_audio_format (header-less
      file) and various multimedia container_formats.
    * LPCM has been defined as a part of the DVD (since 1995) and Blu-ray
      (since 2006) standards.[20][21][22] It is also defined as a part of
      various digital video and audio storage formats (e.g. DV since 1995,[23]
      AVCHD since 2006[24]).
    * LPCM is used by HDMI (defined in 2002), a single-cable digital audio/
      video connector interface for transmitting uncompressed digital data.
    * RF64 container format (defined in 2007) uses LPCM and also allows non-PCM
      bitstream storage: various compression formats contained in the RF64 file
      as data bursts (Dolby E, Dolby AC3, DTS, MPEG-1/MPEG-2 Audio) can be
      "disguised" as PCM linear.[25]
***** Modulation[edit] *****
Sampling and quantization of a signal (red) for 4-bit LPCM
In the diagram, a sine_wave (red curve) is sampled and quantized for PCM. The
sine wave is sampled at regular intervals, shown as vertical lines. For each
sample, one of the available values (on the y-axis) is chosen. The PCM process
is commonly implemented on a single integrated_circuit called an analog-to-
digital_converter (ADC). This produces a fully discrete representation of the
input signal (blue points) that can be easily encoded as digital data for
storage or manipulation. Several PCM streams could also be multiplexed into a
larger aggregate data_stream, generally for transmission of multiple streams
over a single physical link. One technique is called time-division_multiplexing
(TDM) and is widely used, notably in the modern public telephone system.
***** Demodulation[edit] *****
The electronics involved in producing an accurate analog signal from the
discrete data are similar to those used for generating the digital signal.
These devices are digital-to-analog_converters (DACs). They produce a voltage
or current (depending on type) that represents the value presented on their
digital inputs. This output would then generally be filtered and amplified for
use.
To recover the original signal from the sampled data, a demodulator can apply
the procedure of modulation in reverse. After each sampling period, the
demodulator reads the next value and transitions the output signal to the new
value. As a result of these transitions, the signal gains a significant amount
of high-frequency energy due to aliasing effects. To remove these undesirable
frequencies, the demodulator passes the signal through a reconstruction_filter
that suppress energy outside the expected frequency range (greater than the
Nyquist_frequency      f  s    /  2   {\displaystyle f_{s}/2}  [f_s / 2 ]).
[note_4]
***** Standard sampling precision and rates[edit] *****
Common sample depths for LPCM are 8, 16, 20 or 24 bits per sample.[1][2][3][26]
LPCM encodes a single sound channel. Support for multichannel audio depends on
file format and relies on synchronization of multiple LPCM streams.[5][27]
While two channels (stereo) is the most common format, systems can support up
to 8 audio channels (7.1 surround)[2][3] or more.
Common sampling frequencies are 48 kHz as used with DVD format videos, or
44.1 kHz as used in Compact_discs. Sampling frequencies of 96 kHz or 192 kHz
can be used on some equipment, but the benefits have been debated.[28]
***** Limitations[edit] *****
The NyquistâShannon_sampling_theorem shows PCM devices can operate without
introducing distortions within their designed frequency bands if they provide a
sampling frequency at least twice that of the highest frequency contained in
the input signal. For example, in telephony, the usable voice_frequency band
ranges from approximately 300 Hz to 3400 Hz. For effective reconstruction of
the voice signal, telephony applications therefore typically uses an 8000 Hz
sampling frequency which is more than twice the highest usable voice frequency.
Regardless, there are potential sources of impairment implicit in any PCM
system:
    * Choosing a discrete value that is near but not exactly at the analog
      signal level for each sample leads to quantization_error.[note_5]
    * Between samples no measurement of the signal is made; the sampling
      theorem guarantees non-ambiguous representation and recovery of the
      signal only if it has no energy at frequency fs/2 or higher (one half the
      sampling frequency, known as the Nyquist_frequency); higher frequencies
      will not be correctly represented or recovered and add aliasing
      distortion to the signal below the Nyquist frequency.
    * As samples are dependent on time, an accurate clock is required for
      accurate reproduction. If either the encoding or decoding clock is not
      stable, these imperfections will directly affect the output quality of
      the device.[note_6]
***** Processing and coding[edit] *****
Some forms of PCM combine signal processing with coding. Older versions of
these systems applied the processing in the analog domain as part of the
analog-to-digital process; newer implementations do so in the digital domain.
These simple techniques have been largely rendered obsolete by modern
transform-based audio_compression techniques.
    * Linear_PCM (LPCM) is PCM with linear quantization.[29]
    * DPCM encodes the PCM values as differences between the current and the
      predicted value. An algorithm predicts the next sample based on the
      previous samples, and the encoder stores only the difference between this
      prediction and the actual value. If the prediction is reasonable, fewer
      bits can be used to represent the same information. For audio, this type
      of encoding reduces the number of bits required per sample by about 25%
      compared to PCM.
    * Adaptive_DPCM (ADPCM) is a variant of DPCM that varies the size of the
      quantization step, to allow further reduction of the required bandwidth
      for a given signal-to-noise_ratio.
    * Delta_modulation is a form of DPCM which uses one bit per sample.
In telephony, a standard audio signal for a single phone call is encoded as
8,000 samples_per_second, of 8 bits each, giving a 64 kbit/s digital signal
known as DS0. The default signal_compression encoding on a DS0 is either Î¼-law
(mu-law) PCM (North America and Japan) or A-law PCM (Europe and most of the
rest of the world). These are logarithmic compression systems where a 12- or
13-bit linear PCM sample number is mapped into an 8-bit value. This system is
described by international standard G.711.
Where circuit costs are high and loss of voice quality is acceptable, it
sometimes makes sense to compress the voice signal even further. An ADPCM
algorithm is used to map a series of 8-bit Âµ-law or A-law PCM samples into a
series of 4-bit ADPCM samples. In this way, the capacity of the line is
doubled. The technique is detailed in the G.726 standard.
Later it was found that even further compression was possible and additional
standards were published. Some of these international standards describe
systems and ideas which are covered by privately owned patents and thus use of
these standards requires payments to the patent holders.
Some ADPCM techniques are used in Voice_over_IP communications.
***** Encoding for serial transmission[edit] *****
Main article: Line_code
See also: T-carrier and E-carrier
PCM can be either return-to-zero (RZ) or non-return-to-zero (NRZ). For a NRZ
system to be synchronized using in-band information, there must not be long
sequences of identical symbols, such as ones or zeroes. For binary PCM systems,
the density of 1-symbols is called ones-density.[30]
Ones-density is often controlled using precoding techniques such as Run_Length
Limited encoding, where the PCM code is expanded into a slightly longer code
with a guaranteed bound on ones-density before modulation into the channel. In
other cases, extra framing_bits are added into the stream which guarantee at
least occasional symbol transitions.
Another technique used to control ones-density is the use of a scrambler
polynomial on the raw_data which will tend to turn the raw data stream into a
stream that looks pseudo-random, but where the raw stream can be recovered
exactly by reversing the effect of the polynomial. In this case, long runs of
zeroes or ones are still possible on the output, but are considered unlikely
enough to be within normal engineering tolerance.
In other cases, the long term DC value of the modulated signal is important, as
building up a DC offset will tend to bias detector circuits out of their
operating range. In this case special measures are taken to keep a count of the
cumulative DC offset, and to modify the codes if necessary to make the DC
offset always tend back to zero.
Many of these codes are bipolar_codes, where the pulses can be positive,
negative or absent. In the typical alternate_mark_inversion code, non-zero
pulses alternate between being positive and negative. These rules may be
violated to generate special symbols used for framing or other special
purposes.
***** Nomenclature[edit] *****
The word pulse in the term pulse-code modulation refers to the "pulses" to be
found in the transmission line. This perhaps is a natural consequence of this
technique having evolved alongside two analog methods, pulse_width_modulation
and pulse_position_modulation, in which the information to be encoded is
represented by discrete signal pulses of varying width or position,
respectively.[citation_needed] In this respect, PCM bears little resemblance to
these other forms of signal encoding, except that all can be used in time
division multiplexing, and the numbers of the PCM codes are represented as
electrical pulses. The device that performs the coding and decoding function in
a telephone (or other circuit) is called a codec.
***** See also[edit] *****
    * Beta_encoder
    * Equivalent_pulse_code_modulation_noise
    * Signal-to-quantization-noise_ratio (SQNR) â One method of measuring
      quantization error.
***** Notes[edit] *****
   1. ^ Among the first recordings was Uzu: The World Of Stomu Yamash'ta 2 by
      Stomu_Yamashta.
   2. ^ The first recording with this new system was recorded in Tokyo during
      April 24â26, 1972.
   3. ^ Other methods exist such as pulse-density_modulation used also on Super
      Audio_CD.
   4. ^ Some systems use digital_filtering to remove some of the aliasing,
      converting the signal from digital to analog at a higher sample rate such
      that the analog anti-aliasing_filter is much simpler. In some systems, no
      explicit filtering is done at all; as it's impossible for any system to
      reproduce a signal with infinite bandwidth, inherent losses in the system
      compensate for the artifacts â or the system simply does not require
      much precision.
   5. ^ Quantization error swings between -q/2 and q/2. In the ideal case (with
      a fully linear ADC and signal level >> q) it is uniformly_distributed
      over this interval, with zero mean and variance of q2/12.
   6. ^ A slight difference between the encoding and decoding clock frequencies
      is not generally a major concern; a small constant error is not
      noticeable. Clock error does become a major issue if the clock contains
      significant jitter, however.
***** References[edit] *****
   1. ^ a b cAlvestrand, Harald Tveit; Salsman, James (May 1999). "RFC_2586_â
      The_Audio/L16_MIME_content_type". The Internet Society. Retrieved March
      16, 2010.
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
   3. ^ a b cCasner, S. (March 2007). "RFC_4856_â_Media_Type_Registration_of
      Payload_Formats_in_the_RTP_Profile_for_Audio_and_Video_Conferences_â
      Registration_of_Media_Type_audio/L8". The IETF Trust. Retrieved March 16,
      2010.
   4. ^ a b c dBormann, C.; Casner, S.; Kobayashi, K.; Ogawa, A. (January
      2002). "RFC_3190_â_RTP_Payload_Format_for_12-bit_DAT_Audio_and_20-_and
      24-bit_Linear_Sampled_Audio". The Internet Society. Retrieved March 16,
      2010.
   5. ^"Audio_Media_Types". Internet Assigned Numbers Authority. Retrieved
      March 16, 2010.
   6. ^ a b"Linear_Pulse_Code_Modulated_Audio_(LPCM)". Library_of_Congress.
      February 19, 2008. Retrieved March 21, 2010.
   7. ^"The_Bartlane_Transmission_System". DigicamHistory.com. Archived from
      the_original on February 10, 2010. Retrieved January 7, 2010.
   8. ^ U.S. patent number 1,608,527; also see p. 8, Data conversion handbook,
      Walter Allan Kester, ed., Newnes, 2005,
   9. ISBN 0-7506-7841-0.
  10. ^ a bJohn Vardalas (June 2013), Pulse_Code_Modulation:_It_all_Started_75
      Years_Ago_with_Alec_Reeves, IEEE
  11. ^ US_2272070 
  12. ^Porter, Arthur (2004). So Many Hills to Climb. Beckham Publications
      Group. ISBN 9780931761188.
  13. [page needed]
  14. ^Sears, R. W. (January 1948). Electron_Beam_Deflection_Tube_for_Pulse
      Code_Modulation. Bell Systems Technical Journal. 27. Bell_Labs.
      pp. 44â57. Retrieved May 14, 2017.
  15. ^Goodall, W. M. (January 1951). Television_by_Pulse_Code_Modulation. Bell
      Systems Technical Journal. 30. Bell_Labs. pp. 33â49. Retrieved May 14,
      2017.
  16. ^ "Bernard_Oliver". National Inventor's Hall of Fame. Archived from the
      original on December 5, 2010. Retrieved February 6, 2011.
  17. ^ "Claude_Shannon". National Inventor's Hall of Fame. Archived from the
      original on December 6, 2010. Retrieved February 6, 2011.
  18. ^ "National_Inventors_Hall_of_Fame_announces_2004_class_of_inventors".
      Science Blog. February 11, 2004. Retrieved February 6, 2011.
  19. ^ B. M. Oliver; J. R. Pierce & C. E. Shannon (November 1948). "The
      Philosophy of PCM". Proceedings of the IRE. 36 (11): 1324â1331. doi:
      10.1109/JRPROC.1948.231941. ISSN 0096-8390.
  20. ^ a b cThomas Fine (2008). "The_dawn_of_commercial_digital_recording"
      (PDF). ARSC_Journal. 39 (1): 1â17.
  21. ^ P. Cummiskey, N. S. Jayant, and J. L. Flanagan, "Adaptive quantization
      in differential PCM coding of speech," Bell Syst. Tech. J., vol. 52, pp.
      1105â1118, Sept. 1973.
  22. ^Cambron, G. Keith (October 17, 2012). Global Networks: Engineering,
      Operations and Design. John Wiley & Sons. p. 345.
  23. ^Blu-ray Disc Association (March 2005), White_paper_Blu-ray_Disc_Format
      â_2.B_Audio_Visual_Application_Format_Specifications_for_BD-ROM (PDF),
      retrieved July 26, 2009
  24. ^"DVD_Technical_Notes_(DVD_Video_â_"Book_B")_â_Audio_data
      specifications". July 21, 1996. Retrieved March 16, 2010.
  25. ^Jim Taylor. "DVD_Frequently_Asked_Questions_(and_Answers)_â_Audio
      details_of_DVD-Video". Retrieved March 20, 2010.
  26. ^"How_DV_works". Archived from the_original on December 6, 2007.
      Retrieved March 21, 2010.
  27. ^"AVCHD_Information_Website_â_AVCHD_format_specification_overview".
      Retrieved March 21, 2010.
  28. ^EBU (July 2009), EBU_Tech_3306_â_MBWF_/_RF64:_An_Extended_File_Format
      for_Audio (PDF), retrieved January 19, 2010
  29. ^"RFC_3108_â_Conventions_for_the_use_of_the_Session_Description
      Protocol_(SDP)_for_ATM_Bearer_Connections". May 2001. Retrieved March 16,
      2010.
  30. ^"PCM,_Pulse_Code_Modulated_Audio". Library of Congress. Retrieved July
      18, 2009.
  31. ^"24/192_Music_Downloads,_and_why_they_do_not_make_sense". Chris "Monty"
      Montgomery. Retrieved March 16, 2013.
  32. ^"Linear_Pulse_Code_Modulated_Audio_(LPCM)". The Library of Congress.
      February 19, 2008. Retrieved March 21, 2010.
  33. ^ Stallings, William, Digital_Signaling_Techniques, December 1984, Vol.
      22, No. 12, IEEE Communications_Magazine
***** Further reading[edit] *****
    * Franklin_S._Cooper; Ignatius Mattingly (1969). "Computer-controlled PCM
      system for investigation of dichotic speech perception". Journal of the
      Acoustical Society of America. 46: 115. doi:10.1121/1.1972688.
Ken C. Pohlmann (1985). Principles of Digital Audio (2nd ed.). Carmel, Indiana:
Sams/Prentice-Hall Computer Publishing. ISBN 978-0-672-22634-2.
D._H._Whalen, E. R. Wiley, Philip_E._Rubin, and Franklin_S._Cooper (1990). "The
Haskins_Laboratories_pulse_code_modulation_(PCM)_system". Behavior Research
Methods, Instruments, and Computers. 22 (6): 550â559. doi:10.3758/
BF03204440.CS1 maint: Multiple names: authors list (link)
Bill Waggener (1995). Pulse Code Modulation Techniques (1st ed.). New York, NY:
Van Nostrand Reinhold. ISBN 978-0-442-01436-0.
Bill Waggener (1999). Pulse Code Modulation Systems Design (1st ed.). Boston,
MA: Artech House. ISBN 978-0-89006-776-5.
***** External links[edit] *****
 Wikimedia Commons has media related to Pulse-code_modulation.
    * PCM_description_on_MultimediaWiki
    * Ralph_Miller and Bob Badgley invented multi-level PCM independently in
      their work at Bell Labs on SIGSALY: U.S._Patent_3,912,868 filed in 1943:
      N-ary Pulse Code Modulation.
    * Information_about_PCM: A description of PCM with links to information
      about subtypes of this format (for example Linear_Pulse_Code_Modulation),
      and references to their specifications.
    * Summary_of_LPCM â Contains links to information about implementations
      and their specifications.
    * How_to_control_internal/external_hardware_using_Microsoft's_Media_Control
      Interface â Contains information about, and specifications for the
      implementation of LPCM used in WAV files.
    * RFC_4856_â_Media_Type_Registration_of_Payload_Formats_in_the_RTP
      Profile_for_Audio_and_Video_Conferences â audio/L8 and audio/L16 (March
      2007)
    * RFC_3190_â_RTP_Payload_Format_for_12-bit_DAT_Audio_and_20-_and_24-bit
      Linear_Sampled_Audio (January 2002)
    * RFC_3551_â_RTP_Profile_for_Audio_and_Video_Conferences_with_Minimal
      Control â L8 and L16 (July 2003)
    * v
    * t
    * e
High-definition (HD)
                        * High-definition_television
Concepts                * High-definition_video
                        * Ultra-high-definition_television
Analog_broadcast        * 819_line_system
(All defunct)           * HD_MAC
                        * MUSE_(Hi-Vision)
                        * ATSC
                        * DMB-T/H
Digital broadcast       * DVB
                        * ISDB
                        * SBTVD
                        * Dolby_Digital
                        * Surround_sound
Audio                   * DSD
                        * DXD
                        * DTS
Filming and storage     * DCI
                        * HDV
                        * Archival_Disc
                        * Blu-ray
                        * CBHD
                        * D-VHS
                        * DVD-Audio
                        * H.264
HD_media_and            * H.265
compression             * HD_DVD
                        * HD_VMD
                        * MPEG-2
                        * MVC
                        * Super_Audio_CD
                        * Ultra_HD_Blu-ray
                        * Uncompressed
                        * VC-1
                        * Component
                        * DisplayPort
Connectors              * DVI
                        * HDMI
                        * VGA
Deployments             * List_of_digital_television_deployments_by_country
    * v
    * t
    * e
Line_coding (digital baseband transmission)
                     * Unipolar_encoding
Main articles        * Bipolar_encoding
                     * On-off_keying
                     * Return_to_zero_(RZ)
                     * Non-return-to-zero,_level_(NRZ/NRZ-L)
Basic line_codes     * Non-return-to-zero,_inverted_(NRZ-I)
                     * Non-return-to-zero,_space_(NRZ-S)
                     * Manchester
                     * Differential_Manchester/biphase_(Bi-Ï)
                     * Conditioned_Diphase
                     * 4B3T
                     * 4B5B
                     * 2B1Q                                      [Biphase_Mark
                     * Alternate_mark_inversion                  Code.svg]
                     * Modified_AMI_code
Extended line        * Coded_mark_inversion
codes                * MLT-3_encoding
                     * Hybrid_ternary_code
                     * 6b/8b_encoding
                     * 8b/10b_encoding
                     * 64b/66b_encoding
                     * Eight-to-fourteen_modulation
                     * Delay/Miller_encoding
                     * TC-PAM
Optical line         * Carrier-suppressed_return-to-zero
codes                * Alternate-phase_return-to-zero
    * See also: Baseband
    * Baud
    * Bit_rate
    * Digital_signal
    * Digital_transmission
    * Ethernet_physical_layer
    * Pulse_modulation_methods
    * Pulse-amplitude_modulation (PAM)
    * Pulse_code_modulation (PCM)
    * Serial_communication
    * Category:Line_codes
    * v
    * t
    * e
Telecommunications
                     * Beacon
                     * Broadcasting
                     * Cable_protection_system
                     * Cable_TV
                     * Communications_satellite
                     * Computer_network
                     * Drums
                     * Electrical_telegraph
                     * Fax
                     * Heliographs
                     * Hydraulic_telegraph
                     * Internet
                     * Mass_media
                     * Mobile_phone
                     * Optical_telecommunication
                     * Optical_telegraphy
                     * Pager
                     * Photophone
History              * Prepaid_mobile_phone
                     * Radio
                     * Radiotelephone
                     * Satellite_communications
                     * Semaphore
                     * Smartphone
                     * Smoke_signals
                     * Telecommunications_history
                     * Telautograph
                     * Telegraphy
                     * Teleprinter (teletype)
                     * Telephone
                     * The_Telephone_Cases
                     * Television
                     * Undersea_telegraph_line
                     * Videoconferencing
                     * Videophone
                     * Videotelephony
                     * Whistled_language
                     * Edwin_Howard_Armstrong
                     * John_Logie_Baird
                     * Paul_Baran
                     * Alexander_Graham_Bell
                     * Tim_Berners-Lee
                     * Jagadish_Chandra_Bose
                     * Vint_Cerf
                     * Claude_Chappe
                     * Donald_Davies
                     * Lee_de_Forest
                     * Philo_Farnsworth
                     * Reginald_Fessenden
                     * Elisha_Gray
Pioneers             * Erna_Schneider_Hoover
                     * Charles_K._Kao
                     * Hedy_Lamarr                      [Telecom-icon.svg]
                     * Innocenzo_Manzetti
                     * Guglielmo_Marconi
                     * Antonio_Meucci
                     * Radia_Perlman
                     * Alexander_Stepanovich_Popov
                     * Johann_Philipp_Reis
                     * Henry_Sutton
                     * Nikola_Tesla
                     * Camille_Tissot
                     * Alfred_Vail
                     * Charles_Wheatstone
                     * Vladimir_K._Zworykin
                     * Coaxial_cable
                     * Fiber-optic_communication
Transmission               o Optical_fiber
media                * Free-space_optical_communication
                     * Molecular_communication
                     * Radio_waves
                     * Transmission_line
                     * Links
                     * Nodes
Network_topology     * Terminal_node
and switching        * Network_switching (circuit
                     * packet)
                     * Telephone_exchange
                     * Space-division
                     * Frequency-division
Multiplexing         * Time-division
                     * Polarization-division
                     * Orbital_angular-momentum
                     * Code-division
                     * ARPANET
                     * BITNET
                     * Cellular_network
                     * Computer
                     * CYCLADES
                     * Ethernet
                     * FidoNet
                     * Internet
                     * ISDN
                     * LAN
Networks             * Mobile
                     * NGN
                     * NPL_network
                     * Public_Switched_Telephone
                     * Radio
                     * Telecommunications_equipment
                     * Television
                     * Telex
                     * WAN
                     * Wireless_network
                     * World_Wide_Web
    * [Category] Category
    * [List-Class article] Outline
    * [Portal] Portal
    * [Commons page] Commons
Authority_control [Edit_this_at_Wikidata]     * NDL: 00569065

Retrieved from "https://en.wikipedia.org/w/index.php?title=Pulse-
code_modulation&oldid=897114695"
Categories:
    * Quantized_radio_modulation_modes
    * Digital_audio
    * Digital_audio_recording
    * Audio_codecs
    * Computer_file_formats
    * Multiplexing
    * Telephony_signals
Hidden categories:
    * Wikipedia_articles_needing_page_number_citations_from_September_2017
    * Use_mdy_dates_from_July_2013
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_November_2016
    * CS1_maint:_Multiple_names:_authors_list
    * Commons_category_link_from_Wikidata
    * Wikipedia_articles_with_NDL_identifiers
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Basa_Sunda
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 14 May 2019, at 21:27 (UTC).
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
