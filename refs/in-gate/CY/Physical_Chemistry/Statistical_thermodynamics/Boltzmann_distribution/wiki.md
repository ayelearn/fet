The following text has been accessed from https://en.wikipedia.org/wiki/Boltzmann_distribution at Fri Aug 9 02:04:39 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Boltzmann distribution ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Probability distribution of energy states of a system
This article is about system energy states. For particle energy levels and
velocities, see MaxwellâBoltzmann_distribution.
Boltzmann factor pi / pj (vertical axis) as a function of temperature T for
several energy differences Îµi â Îµj.
In statistical_mechanics and mathematics, a Boltzmann distribution (also called
Gibbs distribution[1]) is a probability_distribution or probability_measure
that gives the probability that a system will be in a certain state as a
function of that state's energy and the temperature of the system. It is also a
frequency_distribution of particles in a system.[citation_needed] The
distribution is expressed in the form:
          p  i   &#x221D;  e  &#x2212;    &#x03B5;  i    k T
      {\displaystyle p_{i}\propto e^{-{\frac {\varepsilon _{i}}{kT}}}}  [
      {\displaystyle p_{i}\propto e^{-{\frac {\varepsilon _{i}}{kT}}}}]
where pi is the probability of the system being in state i, Îµi is the energy
of that state, and a constant kT of the distribution is the product of
Boltzmann's_constant k and thermodynamic_temperature T. The symbol     &#x221D;
{\textstyle \propto }  [{\textstyle \propto }] denotes proportionality (see
Â§ The_distribution for the proportionality constant).
The term system here has a very wide meaning; it can range from a single atom
to a macroscopic system such as a natural_gas_storage_tank. Because of this the
Boltzmann distribution can be used to solve a very wide variety of problems.
The distribution shows that states with lower energy will always have a higher
probability of being occupied .
The ratio of probabilities of two states is known as the Boltzmann factor and
characteristically only depends on the states' energy difference:
            p  i    p  j     =  e     &#x03B5;  j   &#x2212;  &#x03B5;  i     k
      T       {\displaystyle {\frac {p_{i}}{p_{j}}}=e^{\frac {\varepsilon _{j}-
      \varepsilon _{i}}{kT}}}  [{\displaystyle {\frac {p_{i}}{p_{j}}}=e^{\frac
      {\varepsilon _{j}-\varepsilon _{i}}{kT}}}]
The Boltzmann distribution is named after Ludwig_Boltzmann who first formulated
it in 1868 during his studies of the statistical_mechanics of gases in thermal
equilibrium. Boltzmann's statistical work is borne out in his paper âOn the
Relationship between the Second Fundamental Theorem of the Mechanical Theory of
Heat and Probability Calculations Regarding the Conditions for Thermal
Equilibrium"[2] The distribution was later investigated extensively, in its
modern generic form, by Josiah_Willard_Gibbs in 1902.[3]:Ch.IV
The generalized Boltzmann distribution is a sufficient and necessary condition
for the equivalence between the statistical mechanics definition of entropy
(The Gibbs_entropy_formula     S = &#x2212;  k   B     &#x2211;  i    p  i
log &#x2061;  p  i     {\displaystyle S=-k_{\mathrm {B} }\sum _{i}p_{i}\log p_
{i}}  [{\displaystyle S=-k_{\mathrm {B} }\sum _{i}p_{i}\log p_{i}}]) and the
thermodynamic definition of entropy (    d S =    &#x03B4;  Q  rev    T
{\displaystyle dS={\frac {\delta Q_{\text{rev}}}{T}}}  [{\displaystyle dS=
{\frac {\delta Q_{\text{rev}}}{T}}}], and the fundamental_thermodynamic
relation)[4].
The Boltzmann distribution should not be confused with the MaxwellâBoltzmann
distribution. The former gives the probability that a system will be in a
certain state as a function of that state's energy;[5] in contrast, the latter
is used to describe particle speeds in idealized gases.
⁰
***** Contents *****
    * 1_The_distribution
    * 2_In_statistical_mechanics
    * 3_In_mathematics
    * 4_In_economics
    * 5_See_also
    * 6_References
***** The distribution[edit] *****
The Boltzmann distribution is a probability_distribution that gives the
probability of a certain state as a function of that state's energy and
temperature of the system to which the distribution is applied.[6] It is given
as
           p  i   =   1 Q       e  &#x2212;   &#x03B5;   i    /  k T   =    e
      &#x2212;   &#x03B5;   i    /  k T     &#x2211;  j = 1   M     e  &#x2212;
      &#x03B5;   j    /  k T         {\displaystyle p_{i}={\frac {1}{Q}}}{e^{-
      {\varepsilon }_{i}/kT}={\frac {e^{-{\varepsilon }_{i}/kT}}{\sum _{j=1}^
      {M}{e^{-{\varepsilon }_{j}/kT}}}}}  [{\displaystyle p_{i}={\frac {1}{Q}}}
      {e^{-{\varepsilon }_{i}/kT}={\frac {e^{-{\varepsilon }_{i}/kT}}{\sum _
      {j=1}^{M}{e^{-{\varepsilon }_{j}/kT}}}}}]
where pi is the probability of state i, Îµi the energy of state i, k the
Boltzmann constant, T the temperature of the system and M is the number of all
states accessible to the system of interest.[6][5] Implied parentheses around
the denominator kT are omitted for brevity. The normalization denominator Q
(denoted by some authors by Z) is the canonical_partition_function
         Q =   &#x2211;  i = 1   M     e  &#x2212;   &#x03B5;   i    /  k T
      {\displaystyle Q={\sum _{i=1}^{M}{e^{-{\varepsilon }_{i}/kT}}}}  [Q={\sum
      _{{i=1}}^{{M}}{e^{{-{\varepsilon }_{i}/kT}}}}]
It results from the constraint that the probabilities of all accessible states
must add up to 1.
The Boltzmann distribution is the distribution that maximizes the entropy
         H (  p  1   ,  p  2   , &#x22EF; ,  p  M   ) = &#x2212;  &#x2211;  i =
      1   M    p  i    log  2   &#x2061;  p  i     {\displaystyle H(p_{1},p_
      {2},\cdots ,p_{M})=-\sum _{i=1}^{M}p_{i}\log _{2}p_{i}}  [{\displaystyle
      H(p_{1},p_{2},\cdots ,p_{M})=-\sum _{i=1}^{M}p_{i}\log _{2}p_{i}}]
subject to the constraint that      &#x2211;   p  i     &#x03B5;   i
{\textstyle {\sum {p_{i}{\varepsilon }_{i}}}}  [{\textstyle {\sum {p_{i}
{\varepsilon }_{i}}}}] equals a particular mean energy value (which can be
proven using Lagrange_multipliers).
The partition function can be calculated if we know the energies of the states
accessible to the system of interest. For atoms the partition function values
can be found in the NIST Atomic Spectra Database.[7]
The distribution shows that states with lower energy will always have a higher
probability of being occupied than the states with higher energy. It can also
give us the quantitative relationship between the probabilities of the two
states being occupied. The ratio of probabilities for states i and j is given
as
            p  i    p  j     =  e  (   &#x03B5;   j   &#x2212;   &#x03B5;   i
      )  /  k T     {\displaystyle {\frac {p_{i}}{p_{j}}}=e^{({\varepsilon }_
      {j}-{\varepsilon }_{i})/kT}}  [{{\frac  {p_{i}}{p_{j}}}}=e^{{(
      {\varepsilon }_{j}-{\varepsilon }_{i})/kT}}]
where pi is the probability of state i, pj the probability of state j, and Îµi
and Îµj are the energies of states i and j, respectively.
The Boltzmann distribution is often used to describe the distribution of
particles, such as atoms or molecules, over energy states accessible to them.
If we have a system consisting of many particles, the probability of a particle
being in state i is practically the probability that, if we pick a random
particle from that system and check what state it is in, we will find it is in
state i. This probability is equal to the number of particles in state i
divided by the total number of particles in the system, that is the fraction of
particles that occupy state i.
          p  i   =    N  i   N     {\displaystyle p_{i}={\frac {N_{i}}{N}}}
      [p_{i}={{\frac  {N_{i}}{N}}}]
where Ni is the number of particles in state i and N is the total number of
particles in the system. We may use the Boltzmann distribution to find this
probability that is, as we have seen, equal to the fraction of particles that
are in state i. So the equation that gives the fraction of particles in state i
as a function of the energy of that state is [5]
            N  i   N   =    e  &#x2212;   &#x03B5;   i    /  k T     &#x2211;
      j = 1   M     e  &#x2212;   &#x03B5;   j    /  k T         {\displaystyle
      {\frac {N_{i}}{N}}={\frac {e^{-{\varepsilon }_{i}/kT}}{\sum _{j=1}^{M}{e^
      {-{\varepsilon }_{j}/kT}}}}}  [{\displaystyle {\frac {N_{i}}{N}}={\frac
      {e^{-{\varepsilon }_{i}/kT}}{\sum _{j=1}^{M}{e^{-{\varepsilon }_{j}/
      kT}}}}}]
This equation is of great importance to spectroscopy. In spectroscopy we
observe a spectral_line of atoms or molecules that we are interested in going
from one state to another.[5][8] In order for this to be possible, there must
be some particles in the first state to undergo the transition. We may find
that this condition is fulfilled by finding the fraction of particles in the
first state. If it is negligible, the transition is very likely not to be
observed at the temperature for which the calculation was done. In general, a
larger fraction of molecules in the first state means a higher number of
transitions to the second state.[9] This gives a stronger spectral line.
However, there are other factors that influence the intensity of a spectral
line, such as whether it is caused by an allowed or a forbidden_transition.
The Boltzmann distribution is related to the softmax_function commonly used in
machine learning.
***** In statistical mechanics[edit] *****
Main articles: Canonical_ensemble and MaxwellâBoltzmann_statistics
The Boltzmann distribution appears in statistical_mechanics when considering
isolated (or nearly-isolated) systems of fixed composition that are in thermal
equilibrium (equilibrium with respect to energy exchange). The most general
case is the probability distribution for the canonical ensemble, but also some
special cases (derivable from the canonical ensemble) also show the Boltzmann
distribution in different aspects:
  Canonical_ensemble (general case)
      The canonical_ensemble gives the probabilities of the various possible
      states of a closed system of fixed volume, in thermal equilibrium with a
      heat_bath. The canonical ensemble is a probability distribution with the
      Boltzmann form.
  Statistical frequencies of subsystems' states (in a non-interacting
  collection)
      When the system of interest is a collection of many non-interacting
      copies of a smaller subsystem, it is sometimes useful to find the
      statistical_frequency of a given subsystem state, among the collection.
      The canonical ensemble has the property of separability when applied to
      such a collection: as long as the non-interacting subsystems have fixed
      composition, then each subsystem's state is independent of the others and
      is also characterized by a canonical ensemble. As a result, the expected
      statistical frequency distribution of subsystem states has the Boltzmann
      form.
  MaxwellâBoltzmann_statistics of classical gases (systems of non-interacting
  particles)
      In particle systems, many particles share the same space and regularly
      change places with each other; the single-particle state space they
      occupy is a shared space. MaxwellâBoltzmann_statistics give the
      expected number of particles found in a given single-particle state, in a
      classical gas of non-interacting particles at equilibrium. This expected
      number distribution has the Boltzmann form.
Although these cases have strong similarities, it is helpful to distinguish
them as they generalize in different ways when the crucial assumptions are
changed:
    * When a system is in thermodynamic equilibrium with respect to both energy
      exchange and particle exchange, the requirement of fixed composition is
      relaxed and a grand_canonical_ensemble is obtained rather than canonical
      ensemble. On the other hand, if both composition and energy are fixed,
      then a microcanonical_ensemble applies instead.
    * If the subsystems within a collection do interact with each other, then
      the expected frequencies of subsystem states no longer follow a Boltzmann
      distribution, and even may not have an analytical_solution.[10] The
      canonical ensemble can however still be applied to the collective states
      of the entire system considered as a whole, provided the entire system is
      isolated and in thermal equilibrium.
    * With quantum gases of non-interacting particles in equilibrium, the
      number of particles found in a given single-particle state does not
      follow MaxwellâBoltzmann statistics, and there is no simple closed form
      expression for quantum gases in the canonical ensemble. In the grand
      canonical ensemble the state-filling statistics of quantum gases are
      described by FermiâDirac_statistics or BoseâEinstein_statistics,
      depending on whether the particles are fermions or bosons respectively.
***** In mathematics[edit] *****
Main articles: Gibbs_measure, Log-linear_model, and Boltzmann_machine
In more general mathematical settings, the Boltzmann distribution is also known
as the Gibbs_measure. In statistics and machine_learning, it is called a log-
linear_model. In deep_learning, the Boltzmann distribution is used in the
sampling_distribution of stochastic_neural_networks such as the Boltzmann
machine , Restricted_Boltzmann_machine and deep_Boltzmann_machine.
***** In economics[edit] *****
The Boltzmann distribution can be introduced to allocate permits in emissions
trading.[11][12] The new allocation method using the Boltzmann distribution can
describe the most probable, natural, and unbiased distribution of emissions
permits among multiple countries. Simple and versatile, this new method holds
potential for many economic and environmental applications.
The Boltzmann distribution has the same form as the multinomial_logit model. As
a discrete_choice model, this is very well known in economics since Daniel
McFadden made the connection to random utility maximization.
***** See also[edit] *****
    * BoseâEinstein_statistics
    * FermiâDirac_statistics
    * Negative_temperature
    * Softmax_function
***** References[edit] *****
   1. ^Landau,_Lev_Davidovich & Lifshitz,_Evgeny_Mikhailovich (1980) [1976].
      Statistical Physics. Course of Theoretical Physics. 5 (3 ed.). Oxford:
      Pergamon Press. ISBN 0-7506-3372-7.
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
   3. Translated by J.B. Sykes and M.J. Kearsley. See section 28
   4. ^ http://crystal.med.upenn.edu/sharp-lab-pdfs/
      2015SharpMatschinsky_Boltz1877_Entropy17.pdf
   5. ^Gibbs,_Josiah_Willard (1902). Elementary_Principles_in_Statistical
      Mechanics. New York: Charles_Scribner's_Sons.
   6. ^Gao, Xiang; Gallicchio, Emilio; Roitberg, Adrian (2019). "The
      generalized_Boltzmann_distribution_is_the_only_distribution_in_which_the
      Gibbs-Shannon_entropy_equals_the_thermodynamic_entropy". The Journal of
      Chemical Physics. 151 (3): 034113. doi:10.1063/1.5111333.
   7. ^ a b c d Atkins, P. W. (2010) Quanta, W. H. Freeman and Company, New
      York
   8. ^ a b McQuarrie, A. (2000) Statistical Mechanics, University Science
      Books, California
   9. ^ NIST_Atomic_Spectra_Database_Levels_Form at nist.gov
  10. ^ Atkins, P. W.; de Paula J. (2009) Physical Chemistry, 9th edition,
      Oxford University Press, Oxford, UK
  11. ^ Skoog, D. A.; Holler, F. J.; Crouch, S. R. (2006) Principles of
      Instrumental Analysis, Brooks/Cole, Boston, MA
  12. ^ A classic example of this is magnetic_ordering. Systems of non-
      interacting spins show paramagnetic behaviour that can be understood with
      a single-particle canonical ensemble (resulting in the Brillouin
      function). Systems of interacting spins can show much more complex
      behaviour such as ferromagnetism or antiferromagnetism.
  13. ^ Park, J.-W., Kim, C. U. and Isard, W. (2012) Permit allocation in
      emissions trading using the Boltzmann distribution. Physica A 391:
      4883â4890
  14. ^ The_Thorny_Problem_Of_Fair_Allocation. Technology Review blog. August
      17, 2011. Cites and summarizes Park, Kim and Isard (2012).
    * Boltzmann,_Ludwig (1868). "Studien Ã¼ber das Gleichgewicht der lebendigen
      Kraft zwischen bewegten materiellen Punkten" [Studies on the balance of
      living force between moving material points]. Wiener Berichte. 58:
      517â560.
Gibbs,_Josiah_Willard (1902). Elementary_Principles_in_Statistical_Mechanics.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Boltzmann_distribution&oldid=907922101"
Categories:
    * Statistical_mechanics
Hidden categories:
    * Use_American_English_from_March_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_December_2018
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
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * SlovenÄina
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Svenska
    * TÃ¼rkÃ§e
    * ä¸­æ
Edit_links
    * This page was last edited on 26 July 2019, at 06:25 (UTC).
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
