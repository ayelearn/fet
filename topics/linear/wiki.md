The following text has been accessed from https://en.wikipedia.org/wiki/Linearity at Fri Aug 9 03:53:17 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Linearity ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Linear" redirects here. For other uses, see Linear_(disambiguation).
Not to be confused with Lineage_(disambiguation).
 This article needs additional citations for verification. Please help improve_this_article by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and removed.
 Find sources: "Linearity" â news Â· newspapers Â· books Â· scholar Â· JSTOR (December 2007)
 (Learn_how_and_when_to_remove_this_template_message)
Linearity is the property of a mathematical relationship or function which
means that it can be graphically represented as a straight line. Examples are
the relationship of voltage and current across a resistor (Ohm's_law), or the
mass and weight of an object. Proportionality implies linearity, but linearity
does not imply proportionality.
⁰
***** Contents *****
    * 1_In_mathematics
          o 1.1_Linear_polynomials
          o 1.2_Boolean_functions
    * 2_Physics
    * 3_Electronics
          o 3.1_Integral_linearity
    * 4_Military_tactical_formations
    * 5_Art
    * 6_Music
    * 7_Measurement
    * 8_See_also
    * 9_References
    * 10_External_links
***** In mathematics[edit] *****
In mathematics, a linear_map or linear_function f(x) is a function that
satisfies the following two properties:[1]
    * Additivity: f(x + y) = f(x) + f(y).
    * Homogeneity of degree 1: f(Î±x) = Î±f(x) for all Î±.
The homogeneity and additivity properties together are called the superposition
principle. It can be shown that additivity implies homogeneity in all cases
where Î± is rational; this is done by proving the case where Î± is a natural
number by mathematical_induction and then extending the result to arbitrary
rational numbers. If f is assumed to be continuous as well, then this can be
extended to show homogeneity for any real number Î±, using the fact that
rationals form a dense subset of the reals.
In this definition, x is not necessarily a real_number, but can in general be a
member of any vector_space. A more specific definition of linear_function, not
coinciding with the definition of linear map, is used in elementary
mathematics.
The concept of linearity can be extended to linear operators. Important
examples of linear operators include the derivative considered as a
differential_operator, and many constructed from it, such as del and the
Laplacian. When a differential_equation can be expressed in linear form, it is
generally straightforward to solve by breaking the equation up into smaller
pieces, solving each of those pieces, and summing the solutions.
Linear_algebra is the branch of mathematics concerned with the study of
vectors, vector spaces (also called linear spaces), linear transformations
(also called linear maps), and systems of linear equations.
The word linear comes from the Latin word linearis, which means pertaining to
or resembling a line. For a description of linear and nonlinear equations, see
linear_equation. Nonlinear equations and functions are of interest to
physicists and mathematicians because they can be used to represent many
natural phenomena, including chaos.
**** Linear polynomials[edit] ****
Main article: linear_equation
In a different usage to the above definition, a polynomial of degree 1 is said
to be linear, because the graph_of_a_function of that form is a line.[2]
Over the reals, a linear_equation is one of the forms:
         f ( x ) = m x + b &#xA0;   {\displaystyle f(x)=mx+b\ }  [f(x) = m x +
      b\ ]
where m is often called the slope or gradient; b the y-intercept, which gives
the point of intersection between the graph of the function and the y-axis.
Note that this usage of the term linear is not the same as in the section
above, because linear polynomials over the real numbers do not in general
satisfy either additivity or homogeneity. In fact, they do so if_and_only_if b
= 0. Hence, if b â  0, the function is often called an affine function (see in
greater generality affine_transformation).
**** Boolean functions[edit] ****
In Boolean_algebra, a linear function is a function     f   {\displaystyle f}
[f] for which there exist      a  0   ,  a  1   , &#x2026; ,  a  n   &#x2208;
{ 0 , 1 }   {\displaystyle a_{0},a_{1},\ldots ,a_{n}\in \{0,1\}}  [a_0, a_1,
\ldots, a_n \in \{0,1\}] such that
         f (  b  1   , &#x2026; ,  b  n   ) =  a  0   &#x2295; (  a  1
      &#x2227;  b  1   ) &#x2295; &#x22EF; &#x2295; (  a  n   &#x2227;  b  n
      )   {\displaystyle f(b_{1},\ldots ,b_{n})=a_{0}\oplus (a_{1}\land b_
      {1})\oplus \cdots \oplus (a_{n}\land b_{n})}  [f(b_1, \ldots, b_n) = a_0
      \oplus (a_1 \land b_1) \oplus \cdots \oplus (a_n \land b_n)], where
      b  1   , &#x2026; ,  b  n   &#x2208; { 0 , 1 } .   {\displaystyle b_
      {1},\ldots ,b_{n}\in \{0,1\}.}  [b_1, \ldots, b_n \in \{0,1\}.]
Note that if      a  0   = 1   {\displaystyle a_{0}=1}  [a_0 = 1], the above
function is considered affine in linear algebra (i.e. not linear).
A Boolean function is linear if one of the following holds for the function's
truth_table:
   1. In every row in which the truth value of the function is T, there are an
      odd number of Ts assigned to the arguments, and in every row in which the
      function is F there is an even number of Ts assigned to arguments.
      Specifically, f(F, F, ..., F) = F, and these functions correspond to
      linear_maps over the Boolean vector space.
   2. In every row in which the value of the function is T, there is an even
      number of Ts assigned to the arguments of the function; and in every row
      in which the truth_value of the function is F, there are an odd number of
      Ts assigned to arguments. In this case, f(F, F, ..., F) = T.
Another way to express this is that each variable always makes a difference in
the truth_value of the operation or it never makes a difference.
Negation, Logical_biconditional, exclusive_or, tautology, and contradiction are
linear functions.
***** Physics[edit] *****
In physics, linearity is a property of the differential_equations governing
many systems; for instance, the Maxwell_equations or the diffusion_equation.[3]
Linearity of a differential_equation means that if two functions f and g are
solutions of the equation, then any linear_combination af + bg is, too.
In instrumentation, linearity means that for every change in the variable you
are observing, you get the same change in the output of the measurement
apparatus - this is highly desirable in scientific work. In general,
instruments are close to linear over a useful certain range, and most useful
within that range. In contrast, human senses are highly nonlinear- for
instance, the brain totally ignores incoming light unless it exceeds a certain
absolute_threshold number of photons.
***** Electronics[edit] *****
In electronics, the linear operating region of a device, for example a
transistor, is where a dependent_variable (such as the transistor collector
current) is directly proportional to an independent_variable (such as the base
current). This ensures that an analog output is an accurate representation of
an input, typically with higher amplitude (amplified). A typical example of
linear equipment is a high_fidelity audio_amplifier, which must amplify a
signal without changing its waveform. Others are linear_filters, linear
regulators, and linear_amplifiers in general.
In most scientific and technological, as distinct from mathematical,
applications, something may be described as linear if the characteristic is
approximately but not exactly a straight line; and linearity may be valid only
within a certain operating regionâfor example, a high-fidelity amplifier may
distort a small signal, but sufficiently little to be acceptable (acceptable
but imperfect linearity); and may distort very badly if the input exceeds a
certain value, taking it away from the approximately linear part of the
transfer_function.[4]
**** Integral linearity[edit] ****
Main article: Integral_linearity
 This section contains overly_lengthy_quotations for an encyclopedic entry.
 Please help_improve_the_article by presenting facts as a neutrally-worded
 summary with appropriate_citations. Consider transferring direct quotations to
 Wikiquote. (September 2014)
For an electronic device (or other physical device) that converts a quantity to
another quantity, Bertram S. Kolts writes:[5][6]
     There are three basic definitions for integral linearity in common
     use: independent linearity, zero-based linearity, and terminal, or
     end-point, linearity. In each case, linearity defines how well the
     device's actual performance across a specified operating range
     approximates a straight line. Linearity is usually measured in terms
     of a deviation, or non-linearity, from an ideal straight line and it
     is typically expressed in terms of percent of full_scale, or in ppm
     (parts per million) of full scale. Typically, the straight line is
     obtained by performing a least-squares fit of the data. The three
     definitions vary in the manner in which the straight line is
     positioned relative to the actual device's performance. Also, all
     three of these definitions ignore any gain, or offset errors that may
     be present in the actual device's performance characteristics.
     Many times a device's specifications will simply refer to linearity,
     with no other explanation as to which type of linearity is intended.
     In cases where a specification is expressed simply as linearity, it
     is assumed to imply independent linearity.
     Independent linearity is probably the most commonly used linearity
     definition and is often found in the specifications for DMMs and
     ADCs, as well as devices like potentiometers. Independent linearity
     is defined as the maximum deviation of actual performance relative to
     a straight line, located such that it minimizes the maximum
     deviation. In that case there are no constraints placed upon the
     positioning of the straight line and it may be wherever necessary to
     minimize the deviations between it and the device's actual
     performance characteristic.
     Zero-based linearity forces the lower range value of the straight
     line to be equal to the actual lower range value of the device's
     characteristic, but it does allow the line to be rotated to minimize
     the maximum deviation. In this case, since the positioning of the
     straight line is constrained by the requirement that the lower range
     values of the line and the device's characteristic be coincident, the
     non-linearity based on this definition will generally be larger than
     for independent linearity.
     For terminal linearity, there is no flexibility allowed in the
     placement of the straight line in order to minimize the deviations.
     The straight line must be located such that each of its end-points
     coincides with the device's actual upper and lower range values. This
     means that the non-linearity measured by this definition will
     typically be larger than that measured by the independent, or the
     zero-based linearity definitions. This definition of linearity is
     often associated with ADCs, DACs and various sensors.
     A fourth linearity definition, absolute linearity, is sometimes also
     encountered. Absolute linearity is a variation of terminal linearity,
     in that it allows no flexibility in the placement of the straight
     line, however in this case the gain and offset errors of the actual
     device are included in the linearity measurement, making this the
     most difficult measure of a device's performance. For absolute
     linearity the end points of the straight line are defined by the
     ideal upper and lower range values for the device, rather than the
     actual values. The linearity error in this instance is the maximum
     deviation of the actual device's performance from ideal.
***** Military tactical formations[edit] *****
In military_tactical_formations, "linear formations" were adapted from phalanx-
like formations of pike protected by handgunners towards shallow formations of
handgunners protected by progressively fewer pikes. This kind of formation
would get thinner until its extreme in the age of Wellington with the 'Thin_Red
Line'. It would eventually be replaced by skirmish_order at the time of the
invention of the breech-loading rifle that allowed soldiers to move and fire
independently of the large-scale formations and fight in small, mobile units.
***** Art[edit] *****
Linear is one of the five categories proposed by Swiss art historian Heinrich
WÃ¶lfflin to distinguish "Classic", or Renaissance_art, from the Baroque.
According to WÃ¶lfflin, painters of the fifteenth and early sixteenth centuries
(Leonardo_da_Vinci, Raphael or Albrecht_DÃ¼rer) are more linear than
"painterly" Baroque painters of the seventeenth century (Peter_Paul_Rubens,
Rembrandt, and VelÃ¡zquez) because they primarily use outline to create shape.
[7] Linearity in art can also be referenced in digital_art. For example,
hypertext_fiction can be an example of nonlinear_narrative, but there are also
websites designed to go in a specified, organized manner, following a linear
path.
***** Music[edit] *****
In music the linear aspect is succession, either intervals or melody, as
opposed to simultaneity or the vertical aspect.
***** Measurement[edit] *****
In measurement, the term "linear foot" refers to the number of feet in a
straight line of material (such as lumber or fabric) generally without regard
to the width. It is sometimes incorrectly referred to as "lineal feet";
however, "lineal" is typically reserved for usage when referring to ancestry or
heredity.[1] The words "linear"[2] & "lineal" [3] both descend from the same
root meaning, the Latin word for line, which is "linea".
[[icon]] This section needs expansion. You can help by adding_to_it. (March
         2013)
***** See also[edit] *****
    * Linear_actuator
    * Linear_element
    * Linear_system
    * Linear_medium
    * Linear_programming
    * Linear_differential_equation
    * Bilinear
    * Multilinear
    * Linear_motor
    * Linear_A and Linear_B scripts.
    * Linear_interpolation
***** References[edit] *****
   1. ^Edwards, Harold M. (1995). Linear_Algebra. Springer. p. 78.
      ISBN 9780817637316.
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
   3. ^ Stewart,_James (2008). Calculus: Early Transcendentals, 6th ed., Brooks
      Cole Cengage Learning.
   4. ISBN 978-0-495-01166-8, Section 1.2
   5. ^Evans, Lawrence C. (2010) [1998], Partial_differential_equations (PDF),
      Graduate_Studies_in_Mathematics, 19 (2nd ed.), Providence, R.I.: American
      Mathematical_Society, doi:10.1090/gsm/019, ISBN 978-0-8218-4974-3,
      MR 2597943
   6. ^Whitaker, Jerry C. (2002). The_RF_transmission_systems_handbook. CRC
      Press. ISBN 978-0-8493-0973-1.
   7. ^Kolts, Bertram S. (2005). "Understanding_Linearity_and_Monotonicity"
      (PDF). analogZONE. Archived from the_original (PDF) on February 4, 2012.
      Retrieved September 24, 2014.
   8. ^Kolts, Bertram S. (2005). "Understanding_Linearity_and_Monotonicity".
      Foreign Electronic Measurement Technology. 24 (5): 30â31. Retrieved
      September 25, 2014.
   9. ^WÃ¶lfflin, Heinrich (1950). Hottinger, M.D. (ed.). Principles of Art
      History: The Problem of the Development of Style in Later Art. New York:
      Dover. pp. 18â72.
***** External links[edit] *****
    *  The dictionary definition of linearity at Wiktionary

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Linearity&oldid=889739587"
Categories:
    * Elementary_algebra
    * Concepts_in_physics
Hidden categories:
    * Articles_needing_additional_references_from_December_2007
    * All_articles_needing_additional_references
    * Wikipedia_articles_with_style_issues_from_September_2014
    * All_articles_with_style_issues
    * Articles_to_be_expanded_from_March_2013
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
    * Broad-concept_articles
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
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Svenska
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 27 March 2019, at 16:58 (UTC).
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
