The following text has been accessed from https://en.wikipedia.org/wiki/Radiation_pattern at Fri Aug 9 03:42:56 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Radiation pattern ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Three-dimensional antenna radiation patterns. The radial distance from the
origin in any direction represents the strength of radiation emitted in that
direction. The top shows the directive pattern of a horn_antenna, the bottom
shows the omnidirectional pattern of a simple vertical_antenna.
Part of a_series on
Antennas
[Montage_of_the_typical_cellular_Antenna_at_the_top_of_the_tower]
Common types
    * Dipole
    * Fractal
    * Loop
    * Monopole
    * Satellite_dish
    * Television
    * Whip
Components
    * Balun
    * Block_upconverter
    * Coaxial_cable
    * Counterpoise_(ground_system)
    * Feed
    * Feed_line
    * Low-noise_block_downconverter
    * Passive_radiator
    * Receiver
    * Rotator
    * Stub
    * Transmitter
    * Tuner
    * Twin-lead
Systems
    * Antenna_farm
    * Amateur_radio
    * Cellular_network
    * Hotspot
    * Municipal_wireless_network
    * Radio
    * Radio_masts_and_towers
    * Wi-Fi
    * Wireless
Safety and regulation
    * Mobile_phone_radiation_and_health
    * Wireless_electronic_devices_and_health
    * International_Telecommunication_Union
      (Radio_Regulations)
    * World_Radiocommunication_Conference
Radiation sources / regions
    * Boresight
    * Focal_cloud
    * Ground_plane
    * Main_lobe
    * Near_and_far_field
    * Side_lobe
    * Vertical_plane
Characteristics
    * Array_gain
    * Directivity
    * Efficiency
    * Electrical_length
    * Equivalent_radius
    * Factor
    * Friis_transmission_equation
    * Gain
    * Height
    * Radiation pattern
    * Radiation_resistance
    * Radio_propagation
    * Radio_spectrum
    * Signal-to-noise_ratio
    * Spurious_emission
Techniques
    * Beam_steering
    * Beam_tilt
    * Beamforming
    * Small_cell
    * Bell_Laboratories_Layered
      Space-Time_(BLAST)
    * Massive Multiple-input_multiple-output_(MIMO)
    * Reconfiguration
    * Spread_spectrum
    * Wideband_Space_Division
      Multiple_Access_(WSDMA)
    * v
    * t
    * e
In the field of antenna design the term radiation pattern (or antenna pattern
or far-field pattern) refers to the directional (angular) dependence of the
strength of the radio_waves from the antenna or other source.[1][2][3]
Particularly in the fields of fiber_optics, lasers, and integrated_optics, the
term radiation pattern may also be used as a synonym for the near-field pattern
or Fresnel pattern.[4] This refers to the positional dependence of the
electromagnetic_field in the near-field, or Fresnel region of the source. The
near-field pattern is most commonly defined over a plane placed in front of the
source, or over a cylindrical or spherical surface enclosing it.[1][4]
The far-field pattern of an antenna may be determined experimentally at an
antenna_range, or alternatively, the near-field pattern may be found using a
near-field_scanner, and the radiation pattern deduced from it by computation.
[1] The far-field radiation pattern can also be calculated from the antenna
shape by computer programs such as NEC. Other software, like HFSS can also
compute the near field.
The far field radiation pattern may be represented graphically as a plot of one
of a number of related variables, including; the field_strength at a constant
(large) radius (an amplitude pattern or field pattern), the power per unit
solid angle (power pattern) and the directive_gain. Very often, only the
relative amplitude is plotted, normalized either to the amplitude on the
antenna boresight, or to the total radiated power. The plotted quantity may be
shown on a linear scale, or in dB. The plot is typically represented as a
three-dimensional graph (as at right), or as separate graphs in the vertical
plane and horizontal_plane. This is often known as a polar diagram.
⁰
***** Contents *****
    * 1_Reciprocity
    * 2_Typical_patterns
    * 3_Proof_of_reciprocity
          o 3.1_Practical_consequences
    * 4_See_also
    * 5_References
    * 6_External_links
***** Reciprocity[edit] *****
It is a fundamental property of antennas that the receiving pattern
(sensitivity as a function of direction) of an antenna when used for receiving
is identical to the far-field radiation pattern of the antenna when used for
transmitting. This is a consequence of the reciprocity_theorem of electro-
magnetics and is proved below. Therefore, in discussions of radiation patterns
the antenna can be viewed as either transmitting or receiving, whichever is
more convenient. Note however that this applies only to the passive antenna
elements. Active antennas that include amplifiers or other components are no
longer reciprocal devices.
***** Typical patterns[edit] *****
Typical polar radiation plot. Most antennas show a pattern of "lobes" or maxima
of radiation. In a directive_antenna, shown here, the largest lobe, in the
desired direction of propagation, is called the "main_lobe". The other lobes
are called "sidelobes" and usually represent radiation in unwanted directions.
Since electromagnetic_radiation is dipole_radiation, it is not possible to
build an antenna that radiates coherently equally in all directions, although
such a hypothetical isotropic_antenna is used as a reference to calculate
antenna_gain.
The simplest antennas, monopole and dipole_antennas, consist of one or two
straight metal rods along a common axis. These axially_symmetric antennas have
radiation patterns with a similar symmetry, called omnidirectional patterns;
they radiate equal power in all directions perpendicular to the antenna, with
the power varying only with the angle to the axis, dropping off to zero on the
antenna's axis. This illustrates the general principle that if the shape of an
antenna is symmetrical, its radiation pattern will have the same symmetry.
In most antennas, the radiation from the different parts of the antenna
interferes at some angles. This results in zero radiation at certain angles
where the radio waves from the different parts arrive out_of_phase, and local
maxima of radiation at other angles where the radio waves arrive in_phase.
Therefore, the radiation plot of most antennas shows a pattern of maxima called
"lobes" at various angles, separated by "nulls" at which the radiation goes to
zero.
A rectangular radiation plot, an alternative presentation method to a polar
plot.
The larger the antenna is compared to a wavelength, the more lobes there will
be. In a directive_antenna in which the objective is to direct the radio waves
in one particular direction, the lobe in that direction is larger than the
others; this is called the "main_lobe". The axis of maximum radiation, passing
through the center of the main lobe, is called the "beam axis" or boresight
axis". In some antennas, such as split-beam antennas, there may exist more than
one major lobe. A minor lobe is any lobe except a major lobe.
The other lobes, representing unwanted radiation in other directions, are
called "side_lobes". The side lobe in the opposite direction (180Â°) from the
main lobe is called the "back lobe".
Minor lobes usually represent radiation in undesired directions, so in
directional antennas a design goal is usually to reduce the minor lobes. Side
lobes are normally the largest of the minor lobes. The level of minor lobes is
usually expressed as a ratio of the power density in the lobe in question to
that of the major lobe. This ratio is often termed the side lobe ratio or side
lobe level. Side lobe levels of â20 dB or greater are usually not desirable
in many applications. Attainment of a side lobe level smaller than â30 dB
usually requires very careful design and construction. In most radar systems,
for example, low side lobe ratios are very important to minimize false target
indications through the side lobes.
***** Proof of reciprocity[edit] *****
For a complete proof, see the reciprocity_(electromagnetism) article. Here, we
present a common simple proof limited to the approximation of two antennas
separated by a large distance compared to the size of the antenna, in a
homogeneous medium. The first antenna is the test antenna whose patterns are to
be investigated; this antenna is free to point in any direction. The second
antenna is a reference antenna, which points rigidly at the first antenna.
Each antenna is alternately connected to a transmitter having a particular
source impedance, and a receiver having the same input impedance (the impedance
may differ between the two antennas).
It is assumed that the two antennas are sufficiently far apart that the
properties of the transmitting antenna are not affected by the load placed upon
it by the receiving antenna. Consequently, the amount of power transferred from
the transmitter to the receiver can be expressed as the product of two
independent factors; one depending on the directional properties of the
transmitting antenna, and the other depending on the directional properties of
the receiving antenna.
For the transmitting antenna, by the definition of gain,     G   {\displaystyle
G}  [G], the radiation power density at a distance     r   {\displaystyle r}
[r] from the antenna (i.e. the power passing through unit area) is
          W  ( &#x03B8; , &#x03A6; ) =     G  ( &#x03B8; , &#x03A6; )   4
      &#x03C0;  r  2       P  t     {\displaystyle \mathrm {W} (\theta ,\Phi )=
      {\frac {\mathrm {G} (\theta ,\Phi )}{4\pi r^{2}}}P_{t}}  [{\mathrm  {W}}
      (\theta ,\Phi )={\frac  {{\mathrm  {G}}(\theta ,\Phi )}{4\pi r^{{2}}}}P_{
      {t}}].
Here, the angles     &#x03B8;   {\displaystyle \theta }  [\theta ] and
&#x03A6;   {\displaystyle \Phi }  [\Phi ] indicate a dependence on direction
from the antenna, and      P  t     {\displaystyle P_{t}}  [P_{{t}}] stands for
the power the transmitter would deliver into a matched load. The gain     G
{\displaystyle G}  [G] may be broken down into three factors; the antenna_gain
(the directional redistribution of the power), the radiation_efficiency
(accounting for ohmic losses in the antenna), and lastly the loss due to
mismatch between the antenna and transmitter. Strictly, to include the
mismatch, it should be called the realized gain,[4] but this is not common
usage.
For the receiving antenna, the power delivered to the receiver is
          P  r   =  A  ( &#x03B8; , &#x03A6; ) W    {\displaystyle P_
      {r}=\mathrm {A} (\theta ,\Phi )W\,}  [P_{{r}}={\mathrm  {A}}(\theta ,\Phi
      )W\,].
Here     W   {\displaystyle W}  [W] is the power density of the incident
radiation, and     A   {\displaystyle A}  [A] is the antenna_aperture or
effective area of the antenna (the area the antenna would need to occupy in
order to intercept the observed captured power). The directional arguments are
now relative to the receiving antenna, and again     A   {\displaystyle A}  [A]
is taken to include ohmic and mismatch losses.
Putting these expressions together, the power transferred from transmitter to
receiver is
          P  r   = A   G  4 &#x03C0;  r  2       P  t     {\displaystyle P_
      {r}=A{\frac {G}{4\pi r^{2}}}P_{t}}  [P_{{r}}=A{\frac  {G}{4\pi r^{
      {2}}}}P_{{t}}],
where     G   {\displaystyle G}  [G] and     A   {\displaystyle A}  [A] are
directionally dependent properties of the transmitting and receiving antennas
respectively. For transmission from the reference antenna (2), to the test
antenna (1), that is
          P  1 r   =   A  1    ( &#x03B8; , &#x03A6; )    G  2    4 &#x03C0;  r
      2       P  2 t     {\displaystyle P_{1r}=\mathrm {A_{1}} (\theta ,\Phi )
      {\frac {G_{2}}{4\pi r^{2}}}P_{2t}}  [P_{{1r}}={\mathrm  {A_{{1}}}}(\theta
      ,\Phi ){\frac  {G_{{2}}}{4\pi r^{{2}}}}P_{{2t}}],
and for transmission in the opposite direction
          P  2 r   =  A  2        G  1    ( &#x03B8; , &#x03A6; )   4 &#x03C0;
      r  2       P  1 t     {\displaystyle P_{2r}=A_{2}{\frac {\mathrm {G_{1}}
      (\theta ,\Phi )}{4\pi r^{2}}}P_{1t}}  [P_{{2r}}=A_{{2}}{\frac  {{\mathrm
      {G_{{1}}}}(\theta ,\Phi )}{4\pi r^{{2}}}}P_{{1t}}].
Here, the gain      G  2     {\displaystyle G_{2}}  [G_{{2}}] and effective
area      A  2     {\displaystyle A_{2}}  [A_{2}] of antenna 2 are fixed,
because the orientation of this antenna is fixed with respect to the first.
Now for a given disposition of the antennas, the reciprocity_theorem requires
that the power transfer is equally effective in each direction, i.e.
            P  1 r    P  2 t     =    P  2 r    P  1 t       {\displaystyle
      {\frac {P_{1r}}{P_{2t}}}={\frac {P_{2r}}{P_{1t}}}}  [{\frac  {P_{{1r}}}
      {P_{{2t}}}}={\frac  {P_{{2r}}}{P_{{1t}}}}],
whence
              A  1    ( &#x03B8; , &#x03A6; )     G  1    ( &#x03B8; , &#x03A6;
      )    =    A  2    G  2       {\displaystyle {\frac {\mathrm {A_{1}}
      (\theta ,\Phi )}{\mathrm {G_{1}} (\theta ,\Phi )}}={\frac {A_{2}}{G_
      {2}}}}  [{\frac  {{\mathrm  {A_{{1}}}}(\theta ,\Phi )}{{\mathrm  {G_{
      {1}}}}(\theta ,\Phi )}}={\frac  {A_{{2}}}{G_{{2}}}}].
But the right hand side of this equation is fixed (because the orientation of
antenna 2 is fixed), and so
              A  1    ( &#x03B8; , &#x03A6; )     G  1    ( &#x03B8; , &#x03A6;
      )    =  c o n s t a n t    {\displaystyle {\frac {\mathrm {A_{1}} (\theta
      ,\Phi )}{\mathrm {G_{1}} (\theta ,\Phi )}}=\mathrm {constant} }  [{\frac
      {{\mathrm  {A_{{1}}}}(\theta ,\Phi )}{{\mathrm  {G_{{1}}}}(\theta ,\Phi
      )}}={\mathrm  {constant}}],
i.e. the directional dependence of the (receiving) effective aperture and the
(transmitting) gain are identical (QED). Furthermore, the constant of
proportionality is the same irrespective of the nature of the antenna, and so
must be the same for all antennas. Analysis of a particular antenna (such as a
Hertzian_dipole), shows that this constant is        &#x03BB;  2    4 &#x03C0;
{\displaystyle {\frac {\lambda ^{2}}{4\pi }}}  [{\frac  {\lambda ^{{2}}}{4\pi
}}], where     &#x03BB;   {\displaystyle \lambda }  [\lambda ] is the free-
space wavelength. Hence, for any antenna the gain and the effective aperture
are related by
          A  ( &#x03B8; , &#x03A6; ) =     &#x03BB;  2    G  ( &#x03B8; ,
      &#x03A6; )   4 &#x03C0;      {\displaystyle \mathrm {A} (\theta ,\Phi )=
      {\frac {\lambda ^{2}\mathrm {G} (\theta ,\Phi )}{4\pi }}}  [{\mathrm
      {A}}(\theta ,\Phi )={\frac  {\lambda ^{{2}}{\mathrm  {G}}(\theta ,\Phi )}
      {4\pi }}].
Even for a receiving antenna, it is more usual to state the gain than to
specify the effective aperture. The power delivered to the receiver is
therefore more usually written as
          P  r   =     &#x03BB;  2    G  r    G  t     ( 4 &#x03C0; r  )  2
      P  t     {\displaystyle P_{r}={\frac {\lambda ^{2}G_{r}G_{t}}{(4\pi r)^
      {2}}}P_{t}}  [P_{{r}}={\frac  {\lambda ^{{2}}G_{{r}}G_{{t}}}{(4\pi r)^{
      {2}}}}P_{{t}}]
(see link_budget). The effective aperture is however of interest for comparison
with the actual physical size of the antenna.
**** Practical consequences[edit] ****
    * When determining the pattern of a receiving antenna by computer
      simulation, it is not necessary to perform a calculation for every
      possible angle of incidence. Instead, the radiation pattern of the
      antenna is determined by a single simulation, and the receiving pattern
      inferred by reciprocity.
    * When determining the pattern of an antenna_by_measurement, the antenna
      may be either receiving or transmitting, whichever is more convenient.
    * For a practical antenna, the side lobe level should be minimum, it is
      necessary to have the maximum directivity[5].
***** See also[edit] *****
    * E-plane_and_H-plane
***** References[edit] *****
   1. ^ a b c Constantine A. Balanis: âAntenna Theory, Analysis and
      Designâ, John Wiley & Sons, Inc., 2nd ed. 1982
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
   3. ISBN 0-471-59268-4
   4. ^ David K Cheng: âField and Wave Electromagneticsâ, Addison-Wesley
      Publishing Company Inc., Edition 2, 1998.
   5. ISBN 0-201-52820-7
   6. ^ Edward C. Jordan & Keith G. Balmain; âElectromagnetic Waves and
      Radiating Systemsâ (2nd ed. 1968) Prentice-Hall.
   7. ISBN 81-203-0054-8
   8. ^ a b c Institute of Electrical and Electronics Engineers , âThe IEEE
      standard dictionary of electrical and electronics termsâ; 6th ed. New
      York, N.Y., Institute of Electrical and Electronics Engineers, c1997.
      IEEE Std 100-1996.
   9. ISBN 1-55937-833-6 [ed. Standards Coordinating Committee 10, Terms and
      Definitions; Jane Radatz, (chair)]
  10. ^Singh, Urvinder; Salgotra, Rohit (20 July 2016). "Synthesis of linear
      antenna array using flower pollination algorithm". Neural Computing and
      Applications. 29 (2): 435â445. doi:10.1007/s00521-016-2457-7.
 This article incorporates public_domain_material from the General_Services
Administration document "Federal_Standard_1037C" (in support of MIL-STD-188).
***** External links[edit] *****
    * Understanding_and_Using_Antenna_Radiation_Patterns_By_Joseph_H._Reisert

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Radiation_pattern&oldid=889615663"
Categories:
    * Antennas_(radio)
    * Fiber_optics
Hidden categories:
    * Wikipedia_articles_incorporating_text_from_the_Federal_Standard_1037C
    * Wikipedia_articles_incorporating_text_from_MIL-STD-188
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
    * Deutsch
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Italiano
    * ×¢××¨××ª
    * Polski
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à·à·à¶à·à¶½
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 26 March 2019, at 20:48 (UTC).
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
