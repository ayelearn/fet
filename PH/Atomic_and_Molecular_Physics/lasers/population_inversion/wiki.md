The following text has been accessed from https://en.wikipedia.org/wiki/Population_inversion at Fri Aug 9 03:08:07 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Population inversion ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In science, specifically statistical_mechanics, a population inversion occurs
while a system (such as a group of atoms or molecules) exists in a state in
which more members of the system are in higher, excited_states than in lower,
unexcited energy_states. It is called an "inversion" because in many familiar
and commonly encountered physical systems, this is not possible. This concept
is of fundamental importance in laser_science because the production of a
population inversion is a necessary step in the workings of a standard laser.
⁰
***** Contents *****
    * 1_Boltzmann_distributions_and_thermal_equilibrium
    * 2_The_interaction_of_light_with_matter
          o 2.1_Absorption
          o 2.2_Spontaneous_emission
          o 2.3_Stimulated_emission
    * 3_Selection_rules
    * 4_Creating_a_population_inversion
          o 4.1_Three-level_lasers
          o 4.2_Four-level_laser
    * 5_Other_methods_of_creating_a_population_inversion
    * 6_See_also
    * 7_References
***** Boltzmann distributions and thermal equilibrium[edit] *****
To understand the concept of a population inversion, it is necessary to
understand some thermodynamics and the way that light interacts with matter. To
do so, it is useful to consider a very simple assembly of atoms forming a laser
medium.
Assume there are a group of N atoms, each of which is capable of being in one
of two energy_states: either
   1. The ground state, with energy E1; or
   2. The excited state, with energy E2, with E2 > E1.
The number of these atoms which are in the ground_state is given by N1, and the
number in the excited state N2. Since there are N atoms in total,
          N  1   +  N  2   = N   {\displaystyle N_{1}+N_{2}=N}  [N_1+N_2 = N]
The energy difference between the two states, given by
         &#x0394;  E  12   =  E  2   &#x2212;  E  1   ,   {\displaystyle \Delta
      E_{12}=E_{2}-E_{1},}  [\Delta E_{12} = E_2-E_1,]
determines the characteristic frequency      &#x03BD;  12     {\textstyle \nu _
{12}}  [{\textstyle \nu _{{12}}}] of light which will interact with the atoms;
This is given by the relation
          E  2   &#x2212;  E  1   = &#x0394;  E  12   = h  &#x03BD;  12   ,
      {\displaystyle E_{2}-E_{1}=\Delta E_{12}=h\nu _{12},}  [{\displaystyle E_
      {2}-E_{1}=\Delta E_{12}=h\nu _{12},}]
h being Planck's_constant.
If the group of atoms is in thermal_equilibrium, it can be shown from
MaxwellâBoltzmann_statistics that the ratio of the number of atoms in each
state is given by the ratio of two Boltzmann_distributions, the Boltzmann
factor:
            N  2    N  1     = exp &#x2061;    &#x2212; (  E  2   &#x2212;  E
      1   )   k T    ,   {\displaystyle {\frac {N_{2}}{N_{1}}}=\exp {\frac {-
      (E_{2}-E_{1})}{kT}},}  [\frac{N_2}{N_1} = \exp{\frac{-(E_2-E_1)}{kT}},]
where T is the thermodynamic_temperature of the group of atoms, and k is
Boltzmann's_constant.
We may calculate the ratio of the populations of the two states at room
temperature (T â 300 K) for an energy difference ÎE that corresponds to
light of a frequency corresponding to visible light (Î½ â 5Ã1014 Hz). In
this case ÎE = E2 - E1 â 2.07 eV, and kT â 0.026 eV. Since E2 - E1 â« kT,
it follows that the argument of the exponential in the equation above is a
large negative number, and as such N2/N1 is vanishingly small; i.e., there are
almost no atoms in the excited state. When in thermal equilibrium, then, it is
seen that the lower energy state is more populated than the higher energy
state, and this is the normal state of the system. As T increases, the number
of electrons in the high-energy state (N2) increases, but N2 never exceeds N1
for a system at thermal equilibrium; rather, at infinite temperature, the
populations N2 and N1 become equal. In other words, a population inversion (N2/
N1 > 1) can never exist for a system at thermal equilibrium. To achieve
population inversion therefore requires pushing the system into a non-
equilibrated state.
***** The interaction of light with matter[edit] *****
There are three types of possible interactions between a system of atoms and
light that are of interest:
**** Absorption[edit] ****
Main article: Absorption_(optics)
If light (photons) of frequency Î½12 passes through the group of atoms, there
is a possibility of the light being absorbed by electrons which are in the
ground state, which will cause them to be excited to the higher energy state.
The rate of absorption is proportional to the radiation intensity of the light,
and also to the number of atoms currently in the ground state, N1.
**** Spontaneous emission[edit] ****
Main article: Spontaneous_emission
If atoms are in the excited state, spontaneous decay events to the ground state
will occur at a rate proportional to N2, the number of atoms in the excited
state. The energy difference between the two states ÎE21 is emitted from the
atom as a photon of frequency Î½21 as given by the frequency-energy relation
above.
The photons are emitted stochastically, and there is no fixed phase
relationship between photons emitted from a group of excited atoms; in other
words, spontaneous emission is incoherent. In the absence of other processes,
the number of atoms in the excited state at time t, is given by
          N  2   ( t ) =  N  2   ( 0 ) exp &#x2061;    &#x2212; t   &#x03C4;
      21     ,   {\displaystyle N_{2}(t)=N_{2}(0)\exp {\frac {-t}{\tau _
      {21}}},}  [N_2(t) = N_2(0) \exp{\frac{-t}{\tau_{21}}},]
where N2(0) is the number of excited atoms at time t = 0, and Ï21 is the mean
lifetime of the transition between the two states.
**** Stimulated emission[edit] ****
Main article: Stimulated_emission
If an atom is already in the excited state, it may be agitated by the passage
of a photon that has a frequency Î½21 corresponding to the energy gap ÎE of
the excited state to ground state transition. In this case, the excited atom
relaxes to the ground state, and it produces a second photon of frequency Î½21.
The original photon is not absorbed by the atom, and so the result is two
photons of the same frequency. This process is known as stimulated emission.
Specifically, an excited atom will act like a small electric dipole which will
oscillate with the external field provided. One of the consequences of this
oscillation is that it encourages electrons to decay to the lowest energy
state. When this happens due to the presence of the electromagnetic field from
a photon, a photon is released in the same phase and direction as the
"stimulating" photon, and is called stimulated emission.
[Stimulated_Emission.svg]
The rate at which stimulated emission occurs is proportional to the number of
atoms N2 in the excited state, and the radiation density of the light. The base
probability of a photon causing stimulated emission in a single excited atom
was shown by Albert_Einstein to be exactly equal to the probability of a photon
being absorbed by an atom in the ground state. Therefore, when the numbers of
atoms in the ground and excited states are equal, the rate of stimulated
emission is equal to the rate of absorption for a given radiation density.
The critical detail of stimulated emission is that the induced photon has the
same frequency and phase as the incident photon. In other words, the two
photons are coherent. It is this property that allows optical_amplification,
and the production of a laser system. During the operation of a laser, all
three light-matter interactions described above are taking place. Initially,
atoms are energized from the ground state to the excited state by a process
called pumping, described below. Some of these atoms decay via spontaneous
emission, releasing incoherent light as photons of frequency, Î½. These photons
are fed back into the laser medium, usually by an optical_resonator. Some of
these photons are absorbed by the atoms in the ground state, and the photons
are lost to the laser process. However, some photons cause stimulated emission
in excited-state atoms, releasing another coherent photon. In effect, this
results in optical amplification.
If the number of photons being amplified per unit time is greater than the
number of photons being absorbed, then the net result is a continuously
increasing number of photons being produced; the laser medium is said to have a
gain of greater than unity.
Recall from the descriptions of absorption and stimulated emission above that
the rates of these two processes are proportional to the number of atoms in the
ground and excited states, N1 and N2, respectively. If the ground state has a
higher population than the excited state (N1 > N2), then the absorption process
dominates, and there is a net attenuation of photons. If the populations of the
two states are the same (N1 = N2), the rate of absorption of light exactly
balances the rate of emission; the medium is then said to be optically
transparent.
If the higher energy state has a greater population than the lower energy state
(N1 < N2), then the emission process dominates, and light in the system
undergoes a net increase in intensity. It is thus clear that to produce a
faster rate of stimulated emissions than absorptions, it is required that the
ratio of the populations of the two states is such that N2/N1 > 1; In other
words, a population inversion is required for laser operation.
***** Selection rules[edit] *****
Main article: Selection_rule
Many transitions involving electromagnetic radiation are strictly forbidden
under quantum mechanics. The allowed transitions are described by so-called
selection_rules, which describe the conditions under which a radiative
transition is allowed. For instance, transitions are only allowed if ÎS = 0, S
being the total spin angular momentum of the system. In real materials other
effects, such as interactions with the crystal lattice, intervene to circumvent
the formal rules by providing alternate mechanisms. In these systems the
forbidden transitions can occur, but usually at slower rates than allowed
transitions. A classic example is phosphorescence where a material has a ground
state with S = 0, an excited state with S = 0, and an intermediate state with
S = 1. The transition from the intermediate state to the ground state by
emission of light is slow because of the selection rules. Thus emission may
continue after the external illumination is removed. In contrast fluorescence
in materials is characterized by emission which ceases when the external
illumination is removed.
Transitions which do not involve the absorption or emission of radiation are
not affected by selection rules. Radiationless transition between levels, such
as between the excited S = 0 and S = 1 states, may proceed quickly enough to
siphon off a portion of the S = 0 population before it spontaneously returns to
the ground state.
The existence of intermediate states in materials is essential to the technique
of optical pumping of lasers (see below).
***** Creating a population inversion[edit] *****
As described above, a population inversion is required for laser operation, but
cannot be achieved in our theoretical group of atoms with two energy-levels
when they are in thermal equilibrium. In fact, any method by which the atoms
are directly and continuously excited from the ground state to the excited
state (such as optical absorption) will eventually reach equilibrium with the
de-exciting processes of spontaneous and stimulated emission. At best, an equal
population of the two states, N1 = N2 = N/2, can be achieved, resulting in
optical transparency but no net optical gain.
**** Three-level lasers[edit] ****
A three-level laser energy diagram.
To achieve non-equilibrium conditions, an indirect method of populating the
excited state must be used. To understand how this is done, we may use a
slightly more realistic model, that of a three-level laser. Again consider a
group of N atoms, this time with each atom able to exist in any of three energy
states, levels 1, 2 and 3, with energies E1, E2, and E3, and populations N1,
N2, and N3, respectively.
We assume that E1 < E2 < E3; that is, the energy of level 2 lies between that
of the ground state and level 3.
Initially, the system of atoms is at thermal equilibrium, and the majority of
the atoms will be in the ground state, i.e., N1 â N, N2 â N3 â 0. If we
now subject the atoms to light of a frequency       &#x03BD;  13    =    1 h
(   E  3   &#x2212;  E  1    )     {\displaystyle \scriptstyle \nu _{13}\,=\,
{\frac {1}{h}}\left(E_{3}-E_{1}\right)}  [\scriptstyle\nu_{13} \,=\, \frac{1}
{h}\left(E_3 - E_1\right)], the process of optical absorption will excite
electrons from the ground state to level 3. This process is called pumping, and
does not necessarily always directly involve light absorption; other methods of
exciting the laser medium, such as electrical discharge or chemical reactions,
may be used. The level 3 is sometimes referred to as the pump level or pump
band, and the energy transition E1 â E3 as the pump transition, which is
shown as the arrow marked P in the diagram on the right.
If we continuously pump electrons, we will excite an appreciable number of them
into level 3, such that N3 > 0. To have a medium suitable for laser operation,
it is necessary that these excited atoms quickly decay to level 2. The energy
released in this transition may be emitted as a photon (spontaneous emission),
however in practice the 3â2 transition (labeled R in the diagram) is usually
radiationless, with the energy being transferred to vibrational motion (heat)
of the host material surrounding the atoms, without the generation of a photon.
An electron in level 2 may decay by spontaneous emission to the ground state,
releasing a photon of frequency Î½12 (given by E2 â E1 = hÎ½12), which is
shown as the transition L, called the laser transition in the diagram. If the
lifetime of this transition, Ï21 is much longer than the lifetime of the
radiationless 3 â 2 transition Ï32 (if Ï21 â« Ï32, known as a favourable
lifetime ratio), the population of the E3 will be essentially zero (N3 â 0)
and a population of excited state atoms will accumulate in level 2 (N2 > 0). If
over half the N atoms can be accumulated in this state, this will exceed the
population of the ground state N1. A population inversion (N2 > N1 ) has thus
been achieved between level 1 and 2, and optical amplification at the frequency
Î½21 can be obtained.
Because at least half the population of atoms must be excited from the ground
state to obtain a population inversion, the laser medium must be very strongly
pumped. This makes three-level lasers rather inefficient, despite being the
first type of laser to be discovered (based on a ruby laser medium, by Theodore
Maiman in 1960). A three-level system could also have a radiative transition
between level 3 and 2, and a non-radiative transition between 2 and 1. In this
case, the pumping requirements are weaker. In practice, most lasers are four-
level lasers, described below.
**** Four-level laser[edit] ****
A four-level laser energy diagram.
Here, there are four energy levels, energies E1, E2, E3, E4, and populations
N1, N2, N3, N4, respectively. The energies of each level are such that E1 < E2
< E3 < E4.
In this system, the pumping transition P excites the atoms in the ground state
(level 1) into the pump band (level 4). From level 4, the atoms again decay by
a fast, non-radiative transition Ra into the level 3. Since the lifetime of the
laser transition L is long compared to that of Ra (Ï32 â« Ï43), a population
accumulates in level 3 (the upper laser level), which may relax by spontaneous
or stimulated emission into level 2 (the lower laser level). This level
likewise has a fast, non-radiative decay Rb into the ground state.
As before, the presence of a fast, radiationless decay transition results in
the population of the pump band being quickly depleted (N4 â 0). In a four-
level system, any atom in the lower laser level E2 is also quickly de-excited,
leading to a negligible population in that state (N2 â 0). This is important,
since any appreciable population accumulating in level 3, the upper laser
level, will form a population inversion with respect to level 2. That is, as
long as N3 > 0, then N3 > N2, and a population inversion is achieved. Thus
optical amplification, and laser operation, can take place at a frequency of
Î½32 (E3-E2 = hÎ½32).
Since only a few atoms must be excited into the upper laser level to form a
population inversion, a four-level laser is much more efficient than a three-
level one, and most practical lasers are of this type. In reality, many more
than four energy levels may be involved in the laser process, with complex
excitation and relaxation processes involved between these levels. In
particular, the pump band may consist of several distinct energy levels, or a
continuum of levels, which allow optical pumping of the medium over a wide
range of wavelengths.
Note that in both three- and four-level lasers, the energy of the pumping
transition is greater than that of the laser transition. This means that, if
the laser is optically pumped, the frequency of the pumping light must be
greater than that of the resulting laser light. In other words, the pump
wavelength is shorter than the laser wavelength. It is possible in some media
to use multiple photon absorptions between multiple lower-energy transitions to
reach the pump level; such lasers are called up-conversion lasers.
While in many lasers the laser process involves the transition of atoms between
different electronic energy states, as described in the model above, this is
not the only mechanism that can result in laser action. For example, there are
many common lasers (e.g., dye_lasers, carbon_dioxide_lasers) where the laser
medium consists of complete molecules, and energy states correspond to
vibrational and rotational modes of oscillation of the molecules. This is the
case with water masers, that occur in nature.
In some media it is possible, by imposing an additional optical or microwave
field, to use quantum_coherence effects to reduce the likelihood of an excited-
state to ground-state transition. This technique, known as lasing_without
inversion, allows optical amplification to take place without producing a
population inversion between the two states.
***** Other methods of creating a population inversion[edit] *****
Stimulated emission was first observed in the microwave region of the
electromagnetic spectrum, giving rise to the acronym MASER for Microwave
Amplification by Stimulated Emission of Radiation. In the microwave region, the
Boltzmann distribution of molecules among energy states is such that, at room
temperature all states are populated almost equally.
To create a population inversion under these conditions, it is necessary to
selectively remove some atoms or molecules from the system based on differences
in properties. For instance, in a hydrogen_maser, the well-known 21cm_wave
transition_in_atomic_hydrogen, where the lone electron flips its spin state
from parallel to the nuclear spin to antiparallel, can be used to create a
population inversion because the parallel state has a magnetic moment and the
antiparallel state does not. A strong_inhomogeneous_magnetic_field will
separate out atoms in the higher energy state from a beam of mixed state atoms.
The separated population represents a population inversion which can exhibit
stimulated emissions.
***** See also[edit] *****
    * Laser_construction
    * Negative_temperature
    * Quantum_electronics
***** References[edit] *****
    * Svelto, Orazio (1998). Principles of Lasers, 4th ed. (trans. David
      Hanna), Springer.
ISBN 0-306-45748-2

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Population_inversion&oldid=900076139"
Categories:
    * Laser_science
    * Statistical_mechanics
Hidden categories:
    * Use_dmy_dates_from_September_2010
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
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 3 June 2019, at 08:12 (UTC).
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
