The following text has been accessed from https://en.wikipedia.org/wiki/Chemical_shift at Fri Aug 9 02:03:56 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Chemical shift ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In nuclear_magnetic_resonance (NMR) spectroscopy, the chemical shift is the
resonant_frequency of a nucleus relative to a standard in a magnetic field.
Often the position and number of chemical shifts are diagnostic of the
structure of a molecule.[1][2][3] Chemical shifts are also used to describe
signals in other forms of spectroscopy such as photoemission_spectroscopy.
Some atomic nuclei possess a magnetic moment (nuclear_spin), which gives rise
to different energy levels and resonance frequencies in a magnetic_field. The
total magnetic field experienced by a nucleus includes local magnetic fields
induced by currents of electrons in the molecular orbitals (note that electrons
have a magnetic moment themselves). The electron distribution of the same type
of nucleus (e.g. 1H, 13C, 15N) usually varies according to the local geometry
(binding partners, bond lengths, angles between bonds, and so on), and with it
the local magnetic field at each nucleus. This is reflected in the spin energy
levels (and resonance frequencies). The variations of nuclear magnetic
resonance frequencies of the same kind of nucleus, due to variations in the
electron distribution, is called the chemical shift. The size of the chemical
shift is given with respect to a reference frequency or reference sample (see
also chemical_shift_referencing), usually a molecule with a barely distorted
electron distribution.
⁰
***** Contents *****
    * 1_Operating_frequency
    * 2_Chemical_shift_referencing
          o 2.1_Referencing_Methods
    * 3_The_induced_magnetic_field
    * 4_Diamagnetic_shielding
    * 5_Factors_causing_chemical_shifts
    * 6_Magnetic_properties_of_most_common_nuclei
    * 7_Chemical_Shift_Manipulation
    * 8_Other_chemical_shifts
    * 9_See_also
    * 10_References
    * 11_External_links
***** Operating frequency[edit] *****
The operating (or Larmor) frequency Ï0 of a magnet is calculated from the
Larmor_equation[4]
          &#x03C9;  0   = &#x03B3;  B  0    ,   {\displaystyle \omega _
      {0}=\gamma B_{0}\,,}  [{\displaystyle \omega _{0}=\gamma B_{0}\,,}]
where B0 is the actual strength of the magnet in units like Teslas or Gauss,
and Î³ is the gyromagnetic_ratio of the nucleus being tested which is in turn
calculated from its magnetic_moment Î¼ and spin_number I with the nuclear
magneton Î¼N and the Planck_constant h:[citation_needed]
         &#x03B3; =    &#x03BC;   &#x03BC;   N      h I     .   {\displaystyle
      \gamma ={\frac {\mu \,\mu _{\mathrm {N} }}{hI}}\,.}  [{\displaystyle
      \gamma ={\frac {\mu \,\mu _{\mathrm {N} }}{hI}}\,.}]
Thus for example, the proton operating frequency for a 1 T magnet is calculated
as:
          &#x03C9;  0   = &#x03B3;  B  0   =    2.79 &#x00D7; 5.05 &#x00D7;  10
      &#x2212; 27      J  /  T     6.62 &#x00D7;  10  &#x2212; 34      J s
      &#x00D7;    1 2       &#x00D7; 1    T   = 42.5    M H z    .
      {\displaystyle \omega _{0}=\gamma B_{0}={\frac {2.79\times 5.05\times 10^
      {-27}\,{\rm {J/T}}}{6.62\times 10^{-34}\,{\rm {Js}}\times {\tfrac {1}
      {2}}}}\times 1\,{\rm {T}}=42.5\,{\rm {MHz}}\,.}  [{\displaystyle \omega _
      {0}=\gamma B_{0}={\frac {2.79\times 5.05\times 10^{-27}\,{\rm {J/T}}}
      {6.62\times 10^{-34}\,{\rm {Js}}\times {\tfrac {1}{2}}}}\times 1\,{\rm
      {T}}=42.5\,{\rm {MHz}}\,.}]
MRI_scanners are often referred to by their field strengths B0 (eg "a 7T
scanner"), whereas NMR_spectrometers are commonly referred to by the
corresponding proton Larmor frequency (eg "a 300 MHz spectrometer; which has a
7T B0). While chemical shift is referenced in order that the units are
equivalent across different field strengths, the actual frequency separation in
Hertz scales with field strength (B0), meaning that larger B0 machines give
spectra with peaks that are less likely to be overlapping, a significant
advantage for analysis. (Larger field machines are also favoured on account of
having intrinsically higher signal arising from the Boltzmann_distribution of
magnetic_spin_states.)
***** Chemical shift referencing[edit] *****
Chemical shift Î´ is usually expressed in parts_per_million (ppm) by frequency,
because it is calculated from:[5]
         &#x03B4; =     &#x03BD;   s a m p l e    &#x2212;  &#x03BD;   r e f
      &#x03BD;   r e f       ,   {\displaystyle \delta ={\frac {\nu _{\mathrm
      {sample} }-\nu _{\mathrm {ref} }}{\nu _{\mathrm {ref} }}}\,,}  [
      {\displaystyle \delta ={\frac {\nu _{\mathrm {sample} }-\nu _{\mathrm
      {ref} }}{\nu _{\mathrm {ref} }}}\,,}]
where Î½sample is the absolute resonance frequency of the sample and Î½ref is
the absolute resonance frequency of a standard reference compound, measured in
the same applied magnetic field B0. Since the numerator is usually expressed in
hertz, and the denominator in megahertz, Î´ is expressed in ppm.
The detected frequencies (in Hz) for 1H, 13C, and 29Si nuclei are usually
referenced against TMS (tetramethylsilane), TSP (Trimethylsilylpropanoic_acid),
or DSS, which by the definition above have a chemical shift of zero if chosen
as the reference. Other standard materials are used for setting the chemical
shift for other nuclei.
Thus, an NMR signal observed at a frequency 300 Hz higher than the signal from
TMS, where the TMS resonance frequency is 300 MHz, has a chemical shift of:
            300    H z     300 &#x00D7;  10  6      H z      = 1 &#x00D7;  10
      &#x2212; 6   = 1    p p m  .     {\displaystyle {\frac {300\,{\rm {Hz}}}
      {300\times 10^{6}\,{\rm {Hz}}}}=1\times 10^{-6}=1\,{\rm {ppm\,.}}}  [
      {\displaystyle {\frac {300\,{\rm {Hz}}}{300\times 10^{6}\,{\rm
      {Hz}}}}=1\times 10^{-6}=1\,{\rm {ppm\,.}}}]
Although the absolute resonance frequency depends on the applied magnetic
field, the chemical shift is independent of external magnetic field strength.
On the other hand, the resolution of NMR will increase with applied magnetic
field.
**** Referencing Methods[edit] ****
Practically speaking, diverse methods may be used to reference chemical shifts
in a NMR experiment, which can be subdivided into indirect and direct
referencing methods.[5] Indirect referencing uses a channel other than the one
of interest to adjust chemical shift scale correctly, i.e. the solvent signal
in the deuterium (lock) channel can be used to reference the a 1H NMR spectrum.
[5] Both indirect and direct referencing can be done as three different
procedures:
   1. "Internal referencing, where the reference compound is added directly to
      the system under study."[5] In this common practice, users adjust
      residual solvent signals of 1H or 13C NMR spectra with calibrated
      spectral tables.[6][7] If substances other than the solvent itself are
      used for internal referencing, the sample has to be combined with the
      reference compound, which may affect the chemical shifts.
   2. "External referencing, involving sample and reference contained
      separately in coaxial cylindrical tubes."[5] With this procedure, the
      reference signal is still visible in the spectrum of interest, although
      the reference and the sample are physically separated by a glass wall.
      Magnetic susceptibility differences between the sample and the reference
      phase need to corrected theoretically,[5] which lowers the practicality
      of this procedure.
   3. "Substitution method: The use of separate cylindrical tubes for the
      sample and the reference compound, with (in principle) spectra recorded
      individually for each."[5] Similar to external referencing, this method
      allows referencing without sample contamination. If field/frequency
      locking via the 2H signal of the deutarated solvent is used and the
      solvents of reference and analyte are the same, the use of this methods
      is straightforward. Problems may arise if different solvents are used for
      the reference compound and the sample as (just like for external
      referencing) magnetic susceptibility differences need to be corrected
      theoretically.[5][8] If this method is used without field/frequency
      locking, shimming procedures between the sample and the reference need to
      be avoided as they change the applied magnetic field (and thereby
      influence the chemical shift).[5]
Modern NMR spectrometers commonly make use of the absolute scale,[8][5] which
defines the 1H signal of TMS as 0 ppm in proton NMR and the center frequencies
of all other nuclei as percentage of the TMS resonance frequency:[5][8]
   &#x039E; [ &#x0025; ] = 100 (  &#x03C5;  X   o b s    /   &#x03C5;  T M S
o b s   )   {\displaystyle \Xi [\%]=100(\upsilon _{X}^{obs}/\upsilon _{TMS}^
{obs})}  [{\displaystyle \Xi [\%]=100(\upsilon _{X}^{obs}/\upsilon _{TMS}^
{obs})}]
The use of the deuterium (lock) channel, so the 2H signal of the deuterated
solvent, and the Î value of the absolute scale is a form of internal
referencing and is particularly useful in heteronuclear NMR spectroscopy as
local reference compounds may not be always be available or easily used (i.e.
liquid NH3 for 15N NMR spectroscopy). This system, however, relies on
accurately determined 2H NMR chemical shifts enlisted in the spectrometer
software and correctly determined Î values by IUPAC.[5][8] A recent study for
19F_NMR_spectroscopy reveiled that the use of the absolute scale and lock-based
internal referencing led to errors in chemical shifts.[9][10] These may be
negated by inclusion of calibrated reference compounds.[9][10]
***** The induced magnetic field[edit] *****
The electrons around a nucleus will circulate in a magnetic field and create a
secondary induced_magnetic_field. This field opposes the applied field as
stipulated by Lenz's_law and atoms with higher induced fields (i.e., higher
electron density) are therefore called shielded, relative to those with lower
electron density. The chemical milieu of an atom can influence its electron
density through the polar_effect. Electron-donating alkyl groups, for example,
lead to increased shielding while electron-withdrawing substituents such as
nitro_groups lead to deshielding of the nucleus. Not only substituents cause
local induced fields. Bonding electrons can also lead to shielding and
deshielding effects. A striking example of this is the pi_bonds in benzene.
Circular current through the hyperconjugated system causes a shielding effect
at the molecule's center and a deshielding effect at its edges. Trends in
chemical shift are explained based on the degree of shielding or deshielding.
Nuclei are found to resonate in a wide range to the left (or more rare to the
right) of the internal standard. When a signal is found with a higher chemical
shift:
    * the applied effective magnetic field is lower, if the resonance frequency
      is fixed (as in old traditional CW spectrometers)
    * the frequency is higher, when the applied magnetic field is static
      (normal case in FT spectrometers)
    * the nucleus is more deshielded
    * the signal or shift is downfield or at low field or paramagnetic
Conversely a lower chemical shift is called a diamagnetic shift, and is upfield
and more shielded.
***** Diamagnetic shielding[edit] *****
In real molecules protons are surrounded by a cloud of charge due to adjacent
bonds and atoms. In an applied magnetic field (B0) electrons circulate and
produce an induced field (Bi) which opposes the applied field. The effective
field at the nucleus will be B = B0 â Bi. The nucleus is said to be
experiencing a diamagnetic shielding.
***** Factors causing chemical shifts[edit] *****
Important factors influencing chemical shift are electron density,
electronegativity of neighboring groups and anisotropic induced magnetic field
effects.
Electron density shields a nucleus from the external field. For example, in
proton NMR the electron-poor tropylium ion has its protons downfield at
9.17 ppm, those of the electron-rich cyclooctatetraenyl anion move upfield to
6.75 ppm and its dianion even more upfield to 5.56 ppm.
A nucleus in the vicinity of an electronegative atom experiences reduced
electron density and the nucleus is therefore deshielded. In proton_NMR of
methyl_halides (CH3X) the chemical shift of the methyl protons increase in the
order I < Br < Cl < F from 2.16 ppm to 4.26 ppm reflecting this trend. In
carbon_NMR the chemical shift of the carbon nuclei increase in the same order
from around â10 ppm to 70 ppm. Also when the electronegative atom is removed
further away the effect diminishes until it can be observed no longer.
Anisotropic induced magnetic field effects are the result of a local induced
magnetic field experienced by a nucleus resulting from circulating electrons
that can either be paramagnetic when it is parallel to the applied field or
diamagnetic when it is opposed to it. It is observed in alkenes where the
double bond is oriented perpendicular to the external field with pi electrons
likewise circulating at right angles. The induced magnetic field lines are
parallel to the external field at the location of the alkene protons which
therefore shift downfield to a 4.5 ppm to 7.5 ppm range. The three-dimensional
space where a diamagnetic shift is called the shielding zone with a cone-like
shape aligned with the external field.
      Induced magnetic field of alkenes in external magnetic fields, field
      lines in grey.
The protons in aromatic compounds are shifted downfield even further with a
signal for benzene at 7.73 ppm as a consequence of a diamagnetic_ring_current.
Alkyne protons by contrast resonate at high field in a 2â3 ppm range. For
alkynes the most effective orientation is the external field in parallel with
electrons circulation around the triple bond. In this way the acetylenic
protons are located in the cone-shaped shielding zone hence the upfield shift.
      Induced magnetic field of alkynes in external magnetic fields, field
      lines in grey.
***** Magnetic properties of most common nuclei[edit] *****
1H and 13C are not the only nuclei susceptible to NMR experiments. A number of
different nuclei can also be detected, although the use of such techniques is
generally rare due to small relative sensitivities in NMR experiments (compared
to 1H) of the nuclei in question, the other factor for rare use being their
slender representation in nature and organic compounds.
                                Magnetic properties of common nuclei[11]
        Occurrence Spin   Magnetic    Electric quadrupole moment Operating_frequency at 7 T Relative
Isotope in_nature  number moment Î¼ (e Ã 10â24 cm2) (MHz)                       sensitivity
        (%)        I      (Î¼N)
1H      099.984    1/2    â2.7962â0                    300.13                      1
2H      000.016    1      â0.8573â0.0028               046.07                      0.0964
10B     018.8      3      â1.8005â0.074                032.25                      0.0199
11B     081.2      3/2    â2.6880â0.026                096.29                      0.165
12C     098.9      0      â0     â0                    000                         0
13C     001.1      1/2    â0.7022â0                    075.47                      0.0159
14N     099.64     1      â0.4035â0.071                021.68                      0.00101
15N     000.37     1/2    â0.2830â0                    030.41                      0.00104
16O     099.76     0      â0     â0                    000                         0
17O     000.0317   5/2    â1.8930â0.0040               040.69                      0.0291
19F     100        1/2    â2.6273â0                    282.40                      0.834
28Si    092.28     0      â0     â0                    000                         0
29Si    004.70     1/2    â0.5548â0                    059.63                      0.0785
31P     100        1/2    â1.1205â0                    121.49                      0.0664
35Cl    075.4      3/2    â0.9209â0.079                029.41                      0.0047
37Cl    024.6      3/2    â0.6833â0.062                024.48                      0.0027
1H, 13C, 15N, 19F and 31P are the five nuclei that have the greatest importance
in NMR experiments:
    * 1H because of high sensitivity and vast occurrence in organic compounds
    * 13C because of being the key component of all organic compounds despite
      occurring at a low abundance (1.1%) compared to the major isotope of
      carbon 12C, which has a spin of 0 and therefore is NMR-inactive.
    * 15N because of being a key component of important biomolecules such as
      proteins and DNA
    * 19F because of high relative sensitivity
    * 31P because of frequent occurrence in organic compounds and moderate
      relative sensitivity
***** Chemical Shift Manipulation[edit] *****
In general, the associated increased signal-to-noise and resolution has driven
a move towards increasingly high field strengths. In limited cases, however,
lower fields are preferred; examples are for systems in chemical exchange,
where the speed of the exchange relative to the NMR experiment can cause
additional and confounding linewidth broadening. Similarly, while avoidance of
second_order_coupling is generally preferred, this information can be useful
for elucidation of chemical structures. Using refocussing pulses placed between
recording of successive points of the Free_Induction_Decay, in an analogous
fashion to the Spin_Echo technique in MRI, the chemical shift evolution can be
scaled to provide apparent low-field spectra on a high-field spectrometer[12].
In a similar fashion, it is possible to upscale the effect of J-coupling
relative to the chemical shift using pulse sequences that include additional J-
coupling evolution periods interspersed with conventional spin evolutions[13].
***** Other chemical shifts[edit] *****
The related Knight_shift (first reported in 1949) is observed with pure metals.
The NMR chemical shift in its present-day meaning first appeared in journals in
1950. Chemical shifts with a different meaning appear in X-ray_photoelectron
spectroscopy as the shift in atomic core-level energy due to a specific
chemical environment. The term is also used in MÃ¶ssbauer_spectroscopy, where
similarly to NMR it refers to a shift in peak position due to the local
chemical bonding environment. As is the case for NMR the chemical shift
reflects the electron density at the atomic nucleus.[14]
***** See also[edit] *****
    * EuFOD, a shift agent
    * MRI
    * Nuclear_magnetic_resonance
    * Nuclear_magnetic_resonance_spectroscopy_of_carbohydrates
    * Nuclear_magnetic_resonance_spectroscopy_of_nucleic_acids
    * Nuclear_magnetic_resonance_spectroscopy_of_proteins
    * Protein_NMR
    * Random_coil_index
    * Relaxation_(NMR)
    * Solid-state_NMR
    * TRISPHAT, a chiral shift reagent for cations
    * Zeeman_effect
***** References[edit] *****
   1. ^Silverstein; Bassler; Morrill (1981). Spectrometric Identification of
      organic Compounds (4th ed.). ISBN 978-0-471-09070-0.
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
   3. ^Kemp, William (1 January 1987). Organic Spectroscopy (3rd ed.).
      ISBN 978-0-333-41767-6.
   4. ^Balei, Metin. Basic 1H and 13C-NMR spectroscopy. ISBN 978-0-444-51811-8.
   5. ^"Chemical_Shift". NMRCentral. Archived from the_original on 26 September
      2011.
   6. ^ a b c d e f g h i j k lHarris, R. K.; Becker, E. D.; Cabral de Menezes,
      S. M.; Goodfellow, R.; Granger, P. (2001). "NMR nomenclature. Nuclear
      spin properties and conventions for chemical shifts (IUPAC
      Recommendations 2001)". Pure_Appl._Chem. 73 (11): 1795â1818. doi:
      10.1351/pac200173111795.
   7. ^Gottlieb, Hugo E.; Kotlyar, Vadim; Nudelman, Abraham (1997). "NMR
      Chemical Shifts of Common Laboratory Solvents as Trace Impurities". The
      Journal of Organic Chemistry. 62 (21): 7512â7515. Bibcode:
      2007JOCh...72.1134P. doi:10.1021/jo971176v. ISSN 0022-3263.
      PMID 11671879.
   8. ^Fulmer, Gregory R.; Miller, Alexander J. M.; Sherden, Nathaniel H.;
      Gottlieb, Hugo E.; Nudelman, Abraham; Stoltz, Brian M.; Bercaw, John E.;
      Goldberg, Karen I. (10 May 2010). "NMR Chemical Shifts of Trace
      Impurities: Common Laboratory Solvents, Organics, and Gases in Deuterated
      Solvents Relevant to the Organometallic Chemist". Organometallics. 29
      (9): 2176â2179. doi:10.1021/om100106e. ISSN 0276-7333.
   9. ^ a b c dHarris, Robin K.; Becker, Edwin D.; Menezes, Cabral de; M,
      Sonia; Granger, Pierre; Hoffman, Roy E.; Zilm, Kurt W. (2008). "Further
      conventions_for_NMR_shielding_and_chemical_shifts_(IUPAC_Recommendations
      2008)". Pure and Applied Chemistry. 80 (1): 59â84. doi:10.1351/
      pac200880010059. ISSN 0033-4545.
  10. ^ a bRosenau, Carl Philipp; Jelier, Benson J.; Gossert, Alvar D.; Togni,
      Antonio (16 May 2018). "Exposing the Origins of Irreproducibility in
      Fluorine NMR Spectroscopy". Angewandte Chemie International Edition. 51
      (30): 9528â9533. Bibcode:2012AnChe..51.3695M. doi:10.1002/
      anie.201802620. ISSN 1433-7851. PMID 29663671.
  11. ^ a bRosenau, Carl Philipp; Jelier, Benson J.; Gossert, Alvar D.; Togni,
      Antonio (16 May 2018). "Fluor-NMR-Spektroskopie rekalibriert". Angewandte
      Chemie (in German). 130 (30): 9672â9677. doi:10.1002/ange.201802620.
      ISSN 0044-8249.
  12. ^CRC_Handbook_of_Chemistry_and_Physics (65th ed.).
  13. ^Morris, Gareth A.; Jerome, Neil P.; Lian, Lu-Yun (17 February 2003).
      "RealâTime ChemicalâShift Scaling in HighâResolution NMR
      Spectroscopy". Angewandte Chemie (in German). 115 (7): 847â849. doi:
      10.1002/ange.200390189.
  14. ^Glanzer, Simon; Zangger, Klaus (13 April 2015). "Visualizing_Unresolved
      Scalar_Couplings_by_Real-Time-Upscaled_NMR". Journal of the American
      Chemical Society. 137 (15): 5163â5169. doi:10.1021/jacs.5b01687.
      PMC 4415032. PMID 25837306.
  15. ^Nagaoka, Shin'ichi (May 2007). "A Short History of Three Chemical
      Shifts". J._Chem._Educ. 84 (5): 801. Bibcode:2007JChEd..84..801N. doi:
      10.1021/ed084p801.
***** External links[edit] *****
    * chem.wisc.edu
    * BioMagResBank
    * chem.csustan.edu[dead_link]
    * Proton_chemical_shifts
    * Carbon_chemical_shifts
    * Online tutorials (these generally involve combined use of IR, 1H_NMR, 13C
      NMR and mass_spectrometry)
          o Problem_set_1 (see also this link for more background information
            on spin-spin coupling)
          o Problem_set_2
          o Problem_set_4
          o Problem_set_5
          o Combined solutions to problem set 5 (Problems_1–32) and (Problems
            33–64)

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Chemical_shift&oldid=908584978"
Categories:
    * Nuclear_chemistry
    * Nuclear_physics
    * Nuclear_magnetic_resonance_spectroscopy
Hidden categories:
    * CS1_German-language_sources_(de)
    * Use_dmy_dates_from_July_2013
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_January_2017
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_January_2016
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
    * CatalÃ 
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * Italiano
    * LatvieÅ¡u
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 30 July 2019, at 17:13 (UTC).
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
