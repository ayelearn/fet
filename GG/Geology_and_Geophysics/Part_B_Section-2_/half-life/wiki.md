The following text has been accessed from https://en.wikipedia.org/wiki/Half-life at Thu Aug 8 23:26:52 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Half-life ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the scientific and mathematical concept. For the video
game, see Half-Life_(video_game). For other uses, see Half-Life_
(disambiguation).
                    This article is missing information about the history of
[Wiki_letter_w.svg] the term half-life. Please expand the article to include
                    this information. Further details may exist on the talk
                    page. (July 2019)
                                                Number of  Fraction  Percentage
                                                half-lives remaining remaining
                                                elapsed
                                                0          1â1  100
                                                1          1â2   50
                                                2          1â4   25
                                                3          1â8   12 .5
                                                4          1â16   6 .25
                                                5          1â32   3 .125
                                                6          1â64   1 .563
                                                7          1â128  0 .781
                                                ...        ...       ...
                                                n          1/2n      100/2n
Half-life (symbol t1â2) is the time required for a quantity to reduce to half
of its initial value. The term is commonly used in nuclear_physics to describe
how quickly unstable atoms undergo, or how long stable atoms survive,
radioactive_decay. The term is also used more generally to characterize any
type of exponential or non-exponential decay. For example, the medical sciences
refer to the biological_half-life of drugs and other chemicals in the human
body. The converse of half-life is doubling_time.
The original term, half-life period, dating to Ernest_Rutherford's discovery of
the principle in 1907, was shortened to half-life in the early 1950s.[1]
Rutherford applied the principle of a radioactive element's half-life to
studies of age determination of rocks by measuring the decay period of radium
to lead-206.
Half-life is constant over the lifetime of an exponentially decaying quantity,
and it is a characteristic_unit for the exponential decay equation. The
accompanying table shows the reduction of a quantity as a function of the
number of half-lives elapsed.
⁰
***** Contents *****
    * 1_Probabilistic_nature
    * 2_Formulas_for_half-life_in_exponential_decay
          o 2.1_Decay_by_two_or_more_processes
          o 2.2_Examples
    * 3_In_non-exponential_decay
    * 4_In_biology_and_pharmacology
    * 5_See_also
    * 6_References
    * 7_External_links
***** Probabilistic nature[edit] *****
Simulation of many identical atoms undergoing radioactive decay, starting with
either 4 atoms per box (left) or 400 (right). The number at the top is how many
half-lives have elapsed. Note the consequence of the law_of_large_numbers: with
more atoms, the overall decay is more regular and more predictable.
A half-life usually describes the decay of discrete entities, such as
radioactive atoms. In that case, it does not work to use the definition that
states "half-life is the time required for exactly half of the entities to
decay". For example, if there is just one radioactive atom, and its half-life
is one second, there will not be "half of an atom" left after one second.
Instead, the half-life is defined in terms of probability: "Half-life is the
time required for exactly half of the entities to decay on_average". In other
words, the probability of a radioactive atom decaying within its half-life is
50%.[2]
For example, the image on the right is a simulation of many identical atoms
undergoing radioactive decay. Note that after one half-life there are not
exactly one-half of the atoms remaining, only approximately, because of the
random variation in the process. Nevertheless, when there are many identical
atoms decaying (right boxes), the law_of_large_numbers suggests that it is a
very good approximation to say that half of the atoms remain after one half-
life.
There are various simple exercises that demonstrate probabilistic decay, for
example involving flipping coins or running a statistical computer_program.[3]
[4][5]
***** Formulas for half-life in exponential decay[edit] *****
Main article: Exponential_decay
An exponential decay can be described by any of the following three equivalent
formulas:[6]:109â112
       N ( t )    =  N  0     (   1 2   )    t  t  1  /  2          N ( t )
=  N  0    e  &#x2212;   t &#x03C4;         N ( t )    =  N  0    e  &#x2212;
&#x03BB; t         {\displaystyle {\begin{aligned}N(t)&=N_{0}\left({\frac {1}
{2}}\right)^{\frac {t}{t_{1/2}}}\\N(t)&=N_{0}e^{-{\frac {t}{\tau }}}\\N(t)&=N_
{0}e^{-\lambda t}\end{aligned}}}  [{\displaystyle {\begin{aligned}N(t)&=N_
{0}\left({\frac {1}{2}}\right)^{\frac {t}{t_{1/2}}}\\N(t)&=N_{0}e^{-{\frac {t}
{\tau }}}\\N(t)&=N_{0}e^{-\lambda t}\end{aligned}}}]
where
    * N0 is the initial quantity of the substance that will decay (this
      quantity may be measured in grams, moles, number of atoms, etc.),
    * N(t) is the quantity that still remains and has not yet decayed after a
      time t,
    * t1â2 is the half-life of the decaying quantity,
    * Ï is a positive_number called the mean_lifetime of the decaying
      quantity,
    * Î» is a positive number called the decay_constant of the decaying
      quantity.
The three parameters t1â2, Ï, and Î» are all directly related in the
following way:
    t  1  /  2   =    ln &#x2061; ( 2 )  &#x03BB;   = &#x03C4; ln &#x2061; ( 2
)   {\displaystyle t_{1/2}={\frac {\ln(2)}{\lambda }}=\tau \ln(2)}  [
{\displaystyle t_{1/2}={\frac {\ln(2)}{\lambda }}=\tau \ln(2)}]
where ln(2) is the natural_logarithm_of_2 (approximately 0.693).[6]:112
**** Decay by two or more processes[edit] ****
Some quantities decay by two exponential-decay processes simultaneously. In
this case, the actual half-life T1â2 can be related to the half-lives t1 and
t2 that the quantity would have if each of the decay processes acted in
isolation:
           1  T  1  /  2     =   1  t  1     +   1  t  2       {\displaystyle
      {\frac {1}{T_{1/2}}}={\frac {1}{t_{1}}}+{\frac {1}{t_{2}}}}  [
      {\displaystyle {\frac {1}{T_{1/2}}}={\frac {1}{t_{1}}}+{\frac {1}{t_
      {2}}}}]
For three or more processes, the analogous formula is:
           1  T  1  /  2     =   1  t  1     +   1  t  2     +   1  t  3     +
      &#x22EF;   {\displaystyle {\frac {1}{T_{1/2}}}={\frac {1}{t_{1}}}+{\frac
      {1}{t_{2}}}+{\frac {1}{t_{3}}}+\cdots }  [{\displaystyle {\frac {1}{T_{1/
      2}}}={\frac {1}{t_{1}}}+{\frac {1}{t_{2}}}+{\frac {1}{t_{3}}}+\cdots }]
For a proof of these formulas, see Exponential_decay_Â§_Decay_by_two_or_more
processes.
**** Examples[edit] ****
Half life demonstrated using dice in a classroom_experiment
Further information: Exponential_decay_Â§ Applications_and_examples
There is a half-life describing any exponential-decay process. For example:
    * As noted above, in radioactive_decay the half-life is the length of time
      after which there is a 50% chance that an atom will have undergone
      nuclear decay. It varies depending on the atom type and isotope, and is
      usually determined experimentally. See List_of_nuclides.
    * The current flowing through an RC_circuit or RL_circuit decays with a
      half-life of ln(2)RC or ln(2)L/R, respectively. For this example the term
      half_time tends to be used, rather than "half life", but they mean the
      same thing.
    * In a chemical_reaction, the half-life of a species is the time it takes
      for the concentration of that substance to fall to half of its initial
      value. In a first-order reaction the half-life of the reactant is ln(2)/
      Î», where Î» is the reaction_rate_constant.
***** In non-exponential decay[edit] *****
The term "half-life" is almost exclusively used for decay processes that are
exponential (such as radioactive decay or the other examples above), or
approximately exponential (such as biological_half-life discussed below). In a
decay process that is not even close to exponential, the half-life will change
dramatically while the decay is happening. In this situation it is generally
uncommon to talk about half-life in the first place, but sometimes people will
describe the decay in terms of its "first half-life", "second half-life", etc.,
where the first half-life is defined as the time required for decay from the
initial value to 50%, the second half-life is from 50% to 25%, and so on.[7]
***** In biology and pharmacology[edit] *****
See also: Biological_half-life
A biological half-life or elimination half-life is the time it takes for a
substance (drug, radioactive nuclide, or other) to lose one-half of its
pharmacologic, physiologic, or radiological activity. In a medical context, the
half-life may also describe the time that it takes for the concentration of a
substance in blood_plasma to reach one-half of its steady-state value (the
"plasma half-life").
The relationship between the biological and plasma half-lives of a substance
can be complex, due to factors including accumulation in tissues, active
metabolites, and receptor interactions.[8]
While a radioactive isotope decays almost perfectly according to so-called
"first order kinetics" where the rate constant is a fixed number, the
elimination of a substance from a living organism usually follows more complex
chemical kinetics.
For example, the biological half-life of water in a human being is about 9 to
10 days,[9] though this can be altered by behavior and various other
conditions. The biological half-life of caesium in human beings is between one
and four months.
The concept of a half-life has also been utilized for pesticides in plants,[10]
and certain authors maintain that pesticide_risk_and_impact_assessment_models
rely on and are sensitive to information describing dissipation from plants.
[11]
***** See also[edit] *****
    * Half_time_(physics)
    * List_of_isotopes_by_half-life
    * Mean_lifetime
***** References[edit] *****
   1. ^ John Ayto, 20th Century Words (1989), Cambridge University Press.
   2. ^Muller,_Richard_A. (April 12, 2010). Physics and Technology for Future
      Presidents. Princeton_University_Press. pp. 128â129.
      ISBN 9780691135045.
   3. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   4. ^Chivers, Sidney (March 16, 2003). "Re:_What_happens_durring_half_lifes_
      [sic]_when_there_is_only_one_atom_left?". MADSCI.org.
   5. ^ "Radioactive-Decay_Model". Exploratorium.edu. Retrieved 2012-04-25.
   6. ^ Wallin, John (September 1996). "Assignment_#2:_Data,_Simulations,_and
      Analytic_Science_in_Decay". Astro.GLU.edu. Archived from the original on
      2011-09-29.CS1 maint: BOT: original-url status unknown (link)
   7. ^ a bRÃ¶sch, Frank (September 12, 2014). Nuclear- and Radiochemistry:
      Introduction. 1. Walter_de_Gruyter. ISBN 978-3-11-022191-6.
   8. ^Jonathan Crowe, Tony Bradshaw (2014). Chemistry_for_the_Biosciences:_The
      Essential_Concepts. p. 568. ISBN 9780199662883.CS1 maint: Uses authors
      parameter (link)
   9. ^Lin VW; Cardenas DD (2003). Spinal_cord_medicine. Demos Medical
      Publishing, LLC. p. 251. ISBN 978-1-888799-61-3.
  10. ^Pang, Xiao-Feng (2014). Water: Molecular Structure and Properties. New
      Jersey: World Scientific. p. 451. ISBN 9789814440424.
  11. ^Australian Pesticides and Veterinary Medicines Authority (31 March
      2015). "Tebufenozide_in_the_product_Mimic_700_WP_Insecticide,_Mimic_240
      SC_Insecticide". Australian Government. Retrieved 30 April 2018.
  12. ^Fantke, Peter; Gillespie, Brenda W.; Juraske, Ronnie; Jolliet, Olivier
      (11 July 2014). "Estimating Half-Lives for Pesticide Dissipation from
      Plants". Environmental Science & Technology. 48 (15): 8588â8602.
      Bibcode:2014EnST...48.8588F. doi:10.1021/es500434p. PMID 24968074.
***** External links[edit] *****
 Look up half-life in Wiktionary, the free dictionary.
 Wikimedia Commons has media related to Half_times.
    * Nucleonica.net, Nuclear Science Portal
    * Nucleonica.net, wiki: Decay Engine
    * Bucknell.edu, System Dynamics â Time Constants
    * [1] Researchers Nikhef and UvA measure slowest radioactive decay ever:
      Xe-124 with 18 billion trillion years.
    * Subotex.com, Half-Life elimination of drugs in blood plasma â Simple
      Charting Tool
    * v
    * t
    * e
Radiation (physics and health)
                                            * Acoustic_radiation_force
                                            * Infrared
                                            * Light
                 Non-ionizing_radiation     * Starlight
                                            * Sunlight
                                            * Microwave
                                            * Radio_waves
                                            * Ultraviolet
                                            * Radioactive_decay
                                            * Cluster_decay
                                            * Background_radiation
                                            * Alpha_particle
                                            * Beta_particle
                                            * Gamma_ray
                                            * Cosmic_ray
                 Ionizing_radiation         * Neutron_radiation
                                            * Nuclear_fission
Main articles                               * Nuclear_fusion
                                            * Nuclear_reactors
                                            * Nuclear_weapons
                                            * Particle_accelerators
                                            * Radioactive_materials
                                            * X-ray
                     * Earth's_energy_budget
                     * Electromagnetic_radiation
                     * Synchrotron_radiation
                     * Thermal_radiation
                     * Black-body_radiation
                     * Particle_radiation
                     * Gravitational_Radiation
                     * Cosmic_background_radiation
                     * Cherenkov_radiation
                     * Askaryan_radiation
                     * Bremsstrahlung
                     * Unruh_radiation
                     * Dark_radiation
                     * Radiation syndrome
                           o acute
                           o chronic
                     * Health_physics
                     * Dosimetry
                     * Electromagnetic_radiation_and_health
                     * Laser_safety
                     * Lasers_and_aviation_safety
Radiation            * Medical_radiography
and health           * Mobile_phone_radiation_and_health
                     * Radiation_protection
                     * Radiation_therapy
                     * Radioactivity_in_the_life_sciences
                     * Radioactive_contamination
                     * Radiobiology
                     * Biological_dose_units_and_quantities
                     * Wireless_electronic_devices_and_health
                     * Radiation_Heat-transfer
                     * Half-life
                     * Nuclear_physics
                     * Radioactive_source
                     * Radiation_hardening
Related articles     * List_of_civilian_radiation_accidents
                     * 1996_Costa_Rica_accident
                     * 1987_GoiÃ¢nia_accident
                     * 1984_Moroccan_accident
                     * 1990_Zaragoza_accident
See also: the categories Radiation_effects, Radioactivity, Radiobiology, and
Radiation_protection.
Authority_control [Edit_this_at_Wikidata]     * GND: 4258821-2
                                              * LCCN: sh85058421

Retrieved from "https://en.wikipedia.org/w/index.php?title=Half-
life&oldid=907034765"
Categories:
    * Radioactivity
    * Exponentials
    * Chemical_kinetics
Hidden categories:
    * CS1_maint:_BOT:_original-url_status_unknown
    * CS1_maint:_Uses_authors_parameter
    * Articles_to_be_expanded_from_July_2019
    * Commons_category_link_is_on_Wikidata
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AragonÃ©s
    * Asturianu
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * à¤­à¥à¤à¤ªà¥à¤°à¥
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * Ð§ÓÐ²Ð°ÑÐ»Ð°
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * è´èª
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * à²à²¨à³à²¨à²¡
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * KreyÃ²l_ayisyen
    * LatvieÅ¡u
    * LietuviÅ³
    * Limburgs
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Nordfriisk
    * Norsk
    * Norsk_nynorsk
    * Occitan
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Ù¾ÙØ¬Ø§Ø¨Û
    * PlattdÃ¼Ã¼tsch
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Runa_Simi
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * à°¤à±à°²à±à°à±
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 20 July 2019, at 00:35 (UTC).
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
