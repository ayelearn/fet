The following text has been accessed from https://en.wikipedia.org/wiki/Partial_molar_property at Fri Aug 9 02:03:44 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Partial molar property ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be challenged
 and removed.
 Find sources: "Partial_molar_property" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (September 2008)(Learn_how_and_when_to_remove_this_template_message)
A partial molar property is a thermodynamic quantity which indicates how an
extensive_property of a solution or mixture varies with changes in the molar
composition of the mixture at constant temperature and pressure. Essentially it
is the partial_derivative of the extensive property with respect to the amount
(number of moles) of the component of interest. Every extensive property of a
mixture has a corresponding partial molar property.
⁰
***** Contents *****
    * 1_Definition
    * 2_Applications
    * 3_Relationship_to_thermodynamic_potentials
    * 4_Differential_form_of_the_thermodynamic_potentials
    * 5_Measuring_partial_molar_properties
    * 6_Relation_to_apparent_molar_quantities
    * 7_See_also
    * 8_References
    * 9_Further_reading
    * 10_External_links
***** Definition[edit] *****
Water and ethanol always have negative excess volumes when mixed, indicating
the partial molar volume of each component is less when mixed than its molar
volume when pure.
The partial molar_volume is broadly understood as the contribution that a
component of a mixture makes to the overall volume of the solution. However,
there is more to it than this:
When one mole of water is added to a large volume of water at 25 Â°C, the
volume increases by 18 cm3. The molar volume of pure water would thus be
reported as 18 cm3 molâ1. However, addition of one mole of water to a large
volume of pure ethanol results in an increase in volume of only 14 cm3. The
reason that the increase is different is that the volume occupied by a given
number of water molecules depends upon the identity of the surrounding
molecules. The value 14 cm3 is said to be the partial molar volume of water in
ethanol.
In general, the partial molar volume of a substance X in a mixture is the
change in volume per mole of X added to the mixture.
The partial molar volumes of the components of a mixture vary with the
composition of the mixture, because the environment of the molecules in the
mixture changes with the composition. It is the changing molecular environment
(and the consequent alteration of the interactions between molecules) that
results in the thermodynamic properties of a mixture changing as its
composition is altered
If, by     Z   {\displaystyle Z}  [Z], one denotes a generic extensive property
of a mixture, it will always be true that it depends on the pressure (    P
{\displaystyle P}  [P]), temperature (    T   {\displaystyle T}  [T]), and the
amount of each component of the mixture (measured in moles, n). For a mixture
with q components, this is expressed as
         Z = Z ( T , P ,  n  1   ,  n  2   , &#x22EF; ) .   {\displaystyle Z=Z
      (T,P,n_{1},n_{2},\cdots ).}  [Z=Z(T,P,n_{1},n_{2},\cdots ).]
Now if temperature T and pressure P are held constant,     Z = Z (  n  1   ,  n
2   , &#x22EF; )   {\displaystyle Z=Z(n_{1},n_{2},\cdots )}  [Z=Z(n_{1},n_
{2},\cdots )] is a homogeneous_function of degree 1, since doubling the
quantities of each component in the mixture will double     Z   {\displaystyle
Z}  [Z]. More generally, for any     &#x03BB;   {\displaystyle \lambda }
[\lambda ]:
         Z ( &#x03BB;  n  1   , &#x03BB;  n  2   , &#x22EF; ) = &#x03BB; Z (  n
      1   ,  n  2   , &#x22EF; ) .   {\displaystyle Z(\lambda n_{1},\lambda n_
      {2},\cdots )=\lambda Z(n_{1},n_{2},\cdots ).}  [Z(\lambda n_{1},\lambda
      n_{2},\cdots )=\lambda Z(n_{1},n_{2},\cdots ).]
By Euler's_first_theorem_for_homogeneous_functions, this implies[1]
         Z =  &#x2211;  i = 1   q    n  i       Z  i   &#x00AF;    ,
      {\displaystyle Z=\sum _{i=1}^{q}n_{i}{\bar {Z_{i}}},}  [{\displaystyle
      Z=\sum _{i=1}^{q}n_{i}{\bar {Z_{i}}},}]
where         Z  i   &#x00AF;      {\displaystyle {\bar {Z_{i}}}}  [{\bar  {Z_
{i}}}] is the partial molar     Z   {\displaystyle Z}  [Z] of component     i
{\displaystyle i}  [i] defined as:
             Z  i   &#x00AF;    =   (    &#x2202; Z   &#x2202;  n  i      )   T
      , P ,  n  j &#x2260; i     .   {\displaystyle {\bar {Z_{i}}}=\left({\frac
      {\partial Z}{\partial n_{i}}}\right)_{T,P,n_{j\neq i}}.}  [{\bar  {Z_
      {i}}}=\left({\frac  {\partial Z}{\partial n_{i}}}\right)_{{T,P,n_{{j\neq
      i}}}}.]
By Euler's_second_theorem_for_homogeneous_functions,         Z  i   &#x00AF;
{\displaystyle {\bar {Z_{i}}}}  [{\bar  {Z_{i}}}] is a homogeneous function of
degree 0 which means that for any     &#x03BB;   {\displaystyle \lambda }
[\lambda ]:
             Z  i   &#x00AF;    ( &#x03BB;  n  1   , &#x03BB;  n  2   ,
      &#x22EF; ) =     Z  i   &#x00AF;    (  n  1   ,  n  2   , &#x22EF; ) .
      {\displaystyle {\bar {Z_{i}}}(\lambda n_{1},\lambda n_{2},\cdots )={\bar
      {Z_{i}}}(n_{1},n_{2},\cdots ).}  [{\bar  {Z_{i}}}(\lambda n_{1},\lambda
      n_{2},\cdots )={\bar  {Z_{i}}}(n_{1},n_{2},\cdots ).]
In particular, taking     &#x03BB; = 1  /   n  T     {\displaystyle \lambda =1/
n_{T}}  [\lambda =1/n_{T}] where      n  T   =  n  1   +  n  2   + &#x22EF;
{\displaystyle n_{T}=n_{1}+n_{2}+\cdots }  [n_{T}=n_{1}+n_{2}+\cdots ], one has
             Z  i   &#x00AF;    (  x  1   ,  x  2   , &#x22EF; ) =     Z  i
      &#x00AF;    (  n  1   ,  n  2   , &#x22EF; ) ,   {\displaystyle {\bar {Z_
      {i}}}(x_{1},x_{2},\cdots )={\bar {Z_{i}}}(n_{1},n_{2},\cdots ),}  [{\bar
      {Z_{i}}}(x_{1},x_{2},\cdots )={\bar  {Z_{i}}}(n_{1},n_{2},\cdots ),]
where      x  i   =    n  i    n  T       {\displaystyle x_{i}={\frac {n_{i}}
{n_{T}}}}  [x_{i}={\frac  {n_{i}}{n_{T}}}] is the concentration expressed as
the mole_fraction of component     i   {\displaystyle i}  [i]. Since the molar
fractions satisfy the relation
          &#x2211;  i = 1   q    x  i   = 1 ,   {\displaystyle \sum _{i=1}^
      {q}x_{i}=1,}  [{\displaystyle \sum _{i=1}^{q}x_{i}=1,}]
the xi are not independent, and the partial molar property is a function of
only     q &#x2212; 1   {\displaystyle q-1}  [q-1] mole fractions:
             Z  i   &#x00AF;    =     Z  i   &#x00AF;    (  x  1   ,  x  2   ,
      &#x22EF; ,  x  q &#x2212; 1   ) .   {\displaystyle {\bar {Z_{i}}}={\bar
      {Z_{i}}}(x_{1},x_{2},\cdots ,x_{q-1}).}  [{\displaystyle {\bar {Z_{i}}}=
      {\bar {Z_{i}}}(x_{1},x_{2},\cdots ,x_{q-1}).}]
The partial molar property is thus an intensive_property - it does not depend
on the size of the system.
The partial volume is not the partial molar volume.
***** Applications[edit] *****
Partial molar properties are useful because chemical mixtures are often
maintained at constant temperature and pressure and under these conditions, the
value of any extensive_property can be obtained from its partial molar
property. They are especially useful when considering specific_properties of
pure_substances (that is, properties of one mole of pure substance) and
properties of mixing (such as the heat_of_mixing or entropy_of_mixing). By
definition, properties of mixing are related to those of the pure substances
by:
         &#x0394;  z  M   = z &#x2212;  &#x2211;  i    x  i    z  i   &#x2217;
      .   {\displaystyle \Delta z^{M}=z-\sum _{i}x_{i}z_{i}^{*}.}  [\Delta z^
      {M}=z-\sum _{i}x_{i}z_{i}^{*}.]
Here     &#x2217;   {\displaystyle *}  [*] denotes a pure substance,     M
{\displaystyle M}  [M] the mixing property, and     z   {\displaystyle z}  [z]
corresponds to the specific property under consideration. From the definition
of partial molar properties,
         z =  &#x2211;  i    x  i       Z  i   &#x00AF;    ,   {\displaystyle
      z=\sum _{i}x_{i}{\bar {Z_{i}}},}  [z=\sum _{i}x_{i}{\bar  {Z_{i}}},]
substitution yields:
         &#x0394;  z  M   =  &#x2211;  i    x  i   (     Z  i   &#x00AF;
      &#x2212;  z  i   &#x2217;   ) .   {\displaystyle \Delta z^{M}=\sum _{i}x_
      {i}({\bar {Z_{i}}}-z_{i}^{*}).}  [\Delta z^{M}=\sum _{i}x_{i}({\bar  {Z_
      {i}}}-z_{i}^{*}).]
So from knowledge of the partial molar properties, deviation of properties of
mixing from single components can be calculated.
***** Relationship to thermodynamic potentials[edit] *****
Partial molar properties satisfy relations analogous to those of the extensive
properties. For the internal_energy U, enthalpy H, Helmholtz_free_energy A, and
Gibbs_free_energy G, the following hold:
             H  i   &#x00AF;    =     U  i   &#x00AF;    + P     V  i
      &#x00AF;    ,   {\displaystyle {\bar {H_{i}}}={\bar {U_{i}}}+P{\bar {V_
      {i}}},}  [{\bar  {H_{i}}}={\bar  {U_{i}}}+P{\bar  {V_{i}}},]
             A  i   &#x00AF;    =     U  i   &#x00AF;    &#x2212; T     S  i
      &#x00AF;    ,   {\displaystyle {\bar {A_{i}}}={\bar {U_{i}}}-T{\bar {S_
      {i}}},}  [{\bar  {A_{i}}}={\bar  {U_{i}}}-T{\bar  {S_{i}}},]
             G  i   &#x00AF;    =     H  i   &#x00AF;    &#x2212; T     S  i
      &#x00AF;    ,   {\displaystyle {\bar {G_{i}}}={\bar {H_{i}}}-T{\bar {S_
      {i}}},}  [{\bar  {G_{i}}}={\bar  {H_{i}}}-T{\bar  {S_{i}}},]
where     P   {\displaystyle P}  [P] is the pressure,     V   {\displaystyle V}
[V] the volume,     T   {\displaystyle T}  [T] the temperature, and     S
{\displaystyle S}  [S] the entropy.
***** Differential form of the thermodynamic potentials[edit] *****
The thermodynamic potentials also satisfy
         d U = T d S &#x2212; P d V +  &#x2211;  i    &#x03BC;  i   d  n  i   ,
      {\displaystyle dU=TdS-PdV+\sum _{i}\mu _{i}dn_{i},\,}  [dU=TdS-PdV+\sum _
      {i}\mu _{i}dn_{i},\,]
         d H = T d S + V d P +  &#x2211;  i    &#x03BC;  i   d  n  i   ,
      {\displaystyle dH=TdS+VdP+\sum _{i}\mu _{i}dn_{i},\,}  [dH=TdS+VdP+\sum _
      {i}\mu _{i}dn_{i},\,]
         d A = &#x2212; S d T &#x2212; P d V +  &#x2211;  i    &#x03BC;  i   d
      n  i   ,    {\displaystyle dA=-SdT-PdV+\sum _{i}\mu _{i}dn_{i},\,}  [dA=-
      SdT-PdV+\sum _{i}\mu _{i}dn_{i},\,]
         d G = &#x2212; S d T + V d P +  &#x2211;  i    &#x03BC;  i   d  n  i
      ,    {\displaystyle dG=-SdT+VdP+\sum _{i}\mu _{i}dn_{i},\,}  [dG=-
      SdT+VdP+\sum _{i}\mu _{i}dn_{i},\,]
where      &#x03BC;  i     {\displaystyle \mu _{i}}  [\mu _{i}] is the chemical
potential defined as (for constant nj with jâ i):
          &#x03BC;  i   =   (    &#x2202; U   &#x2202;  n  i      )   S , V   =
      (    &#x2202; H   &#x2202;  n  i      )   S , P   =   (    &#x2202; A
      &#x2202;  n  i      )   T , V   =   (    &#x2202; G   &#x2202;  n  i
      )   T , P   .   {\displaystyle \mu _{i}=\left({\frac {\partial U}
      {\partial n_{i}}}\right)_{S,V}=\left({\frac {\partial H}{\partial n_
      {i}}}\right)_{S,P}=\left({\frac {\partial A}{\partial n_{i}}}\right)_
      {T,V}=\left({\frac {\partial G}{\partial n_{i}}}\right)_{T,P}.}  [\mu _
      {i}=\left({\frac  {\partial U}{\partial n_{i}}}\right)_{{S,V}}=\left(
      {\frac  {\partial H}{\partial n_{i}}}\right)_{{S,P}}=\left({\frac
      {\partial A}{\partial n_{i}}}\right)_{{T,V}}=\left({\frac  {\partial G}
      {\partial n_{i}}}\right)_{{T,P}}.]
This last partial_derivative is the same as         G  i   &#x00AF;
{\displaystyle {\bar {G_{i}}}}  [{\bar  {G_{i}}}], the partial molar Gibbs_free
energy. This means that the partial molar Gibbs free energy and the chemical
potential, one of the most important properties in thermodynamics and
chemistry, are the same quantity. Under isobaric (constant P) and isothermal
(constant T) conditions, knowledge of the chemical potentials,      &#x03BC;  i
(  x  1   ,  x  2   , &#x22EF; ,  x  m   )   {\displaystyle \mu _{i}(x_{1},x_
{2},\cdots ,x_{m})}  [\mu _{i}(x_{1},x_{2},\cdots ,x_{m})], yields every
property of the mixture as they completely determine the Gibbs free energy.
***** Measuring partial molar properties[edit] *****
To measure the partial molar property         Z  1   &#x00AF;
{\displaystyle {\bar {Z_{1}}}}  [{\bar  {Z_{1}}}] of a binary solution, one
begins with the pure component denoted as     2   {\displaystyle 2}  [2] and,
keeping the temperature and pressure constant during the entire process, add
small quantities of component     1   {\displaystyle 1}  [1]; measuring     Z
{\displaystyle Z}  [Z] after each addition. After sampling the compositions of
interest one can fit a curve to the experimental data. This function will be
Z (  n  1   )   {\displaystyle Z(n_{1})}  [Z(n_{1})]. Differentiating with
respect to      n  1     {\displaystyle n_{1}}  [n_{1}] will give         Z  1
&#x00AF;      {\displaystyle {\bar {Z_{1}}}}  [{\bar  {Z_{1}}}].         Z  2
&#x00AF;      {\displaystyle {\bar {Z_{2}}}}  [{\bar  {Z_{2}}}] is then
obtained from the relation:
         Z =     Z  1   &#x00AF;     n  1   +     Z  2   &#x00AF;     n  2   .
      {\displaystyle Z={\bar {Z_{1}}}n_{1}+{\bar {Z_{2}}}n_{2}.}  [Z={\bar  {Z_
      {1}}}n_{1}+{\bar  {Z_{2}}}n_{2}.]
***** Relation to apparent molar quantities[edit] *****
The relation between partial molar properties and the apparent ones can be
derived from the definition of the apparent quantities and of the molality.
             V  1   &#x00AF;    =     &#x03D5;       V &#x007E;     1   + b
      &#x2202;     &#x03D5;       V &#x007E;     1     &#x2202; b    .
      {\displaystyle {\bar {V_{1}}}={}^{\phi }{\tilde {V}}_{1}+b{\frac
      {\partial {}^{\phi }{\tilde {V}}_{1}}{\partial b}}.}  [{\bar  {V_{1}}}=
      {}^{\phi }{\tilde  {V}}_{1}+b{\frac  {\partial {}^{\phi }{\tilde  {V}}_
      {1}}{\partial b}}.]
The relation holds also for multicomponent mixtures, just that in this case
subscript i is required.
***** See also[edit] *****
    * Apparent_molar_property
    * Ideal_solution
    * Excess_molar_quantity
    * Partial_specific_volume
    * Thermodynamic_activity
***** References[edit] *****
   1. ^ Wolfram_Mathworld:_Euler's_homogeneous_function_theorem
***** Further reading[edit] *****
    * P. Atkins and J. de Paula, "Atkins' Physical Chemistry" (8th edition,
      Freeman 2006), chap.5
    * T. Engel and P. Reid, "Physical Chemistry" (Pearson Benjamin-Cummings
      2006), p. 210
    * K.J. Laidler and J.H. Meiser, "Physical Chemistry" (Benjamin-Cummings
      1982), p. 184-189
    * P. Rock, "Chemical Thermodynamics" (MacMillan 1969), chap.9
    * Ira.Levine, "Physical Chemistry" (6th edition,McGraw Hill 2009),p.125-128
***** External links[edit] *****
 Wikimedia Commons has media related to Excess_volume_diagrams.
    * Lecture notes from the University of Arizona detailing mixtures,_partial
      molar_quantities,_and_ideal_solutions
    * On-line_calculator_for_densities_and_partial_molar_volumes_of_aqueous
      solutions_of_some_common_electrolytes_and_their_mixtures,_at_temperatures
      up_to_323.15_K.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Partial_molar_property&oldid=898038308"
Categories:
    * Physical_chemistry
    * Thermodynamic_properties
    * Chemical_thermodynamics
Hidden categories:
    * Articles_needing_additional_references_from_September_2008
    * All_articles_needing_additional_references
    * Commons_category_link_is_on_Wikidata
    * Commons_category_link_is_on_Wikidata_using_P373
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
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * Italiano
    * Nederlands
    * RomÃ¢nÄ
    * Suomi
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 21 May 2019, at 00:01 (UTC).
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
