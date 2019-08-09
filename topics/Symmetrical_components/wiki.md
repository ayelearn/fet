The following text has been accessed from https://en.wikipedia.org/wiki/Symmetrical_components at Thu Aug 8 22:53:17 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Symmetrical components ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In electrical_engineering, the method of symmetrical components simplifies
analysis of unbalanced three-phase power systems under both normal and abnormal
conditions. The basic idea is that an asymmetrical set of N phasors can be
expressed as a linear_combination of N symmetrical sets of phasors by means of
a complex linear_transformation.[1]
In the most common case of three-phase systems, the resulting "symmetrical"
components are referred to as direct (or positive), inverse (or negative) and
zero (or homopolar). The analysis of power system is much simpler in the domain
of symmetrical components, because the resulting equations are mutually
linearly_independent if the circuit itself is balanced.[citation_needed]
⁰
***** Contents *****
    * 1_Description
    * 2_The_three-phase_case
          o 2.1_A_matrix
          o 2.2_Decomposition
          o 2.3_Intuition
    * 3_Poly-phase_case
    * 4_Contribution_of_harmonics_to_symmetrical_components_in_3-phase_power
      systems
    * 5_Consequence_of_the_zero_sequence_component_in_power_systems
    * 6_See_also
    * 7_References
***** Description[edit] *****
Set of three unbalanced phasors, and the necessary symmetrical components that
sum up to the resulting plot at the bottom.
In 1918 Charles_Legeyt_Fortescue presented a paper[2] which demonstrated that
any set of N unbalanced phasors (that is, any such polyphase signal) could be
expressed as the sum of N symmetrical sets of balanced phasors, for values of N
that are prime. Only a single frequency component is represented by the
phasors.
In 1943 Edith_Clarke published a textbook giving a method of use of symmetrical
components for three-phase systems that greatly simplified calculations over
the original Fortescue paper. [3] In a three-phase system, one set of phasors
has the same phase_sequence as the system under study (positive sequence; say
ABC), the second set has the reverse phase sequence (negative sequence; ACB),
and in the third set the phasors A, B and C are in phase with each other (zero
sequence, the common-mode_signal). Essentially, this method converts three
unbalanced phases into three independent sources, which makes asymmetric_fault
analysis more tractable.
By expanding a one-line_diagram to show the positive sequence, negative
sequence, and zero sequence impedances of generators, transformers and other
devices including overhead_lines and cables, analysis of such unbalanced
conditions as a single line to ground short-circuit fault is greatly
simplified. The technique can also be extended to higher order phase systems.
Physically, in a three phase system, a positive sequence set of currents
produces a normal rotating field, a negative sequence set produces a field with
the opposite rotation, and the zero sequence set produces a field that
oscillates but does not rotate between phase windings. Since these effects can
be detected physically with sequence filters, the mathematical tool became the
basis for the design of protective_relays, which used negative-sequence
voltages and currents as a reliable indicator of fault conditions. Such relays
may be used to trip circuit_breakers or take other steps to protect electrical
systems.
The analytical technique was adopted and advanced by engineers at General
Electric and Westinghouse, and after World_War_II it became an accepted method
for asymmetric fault analysis.
As shown in the figure to the above right, the three sets of symmetrical
components (positive, negative, and zero sequence) add up to create the system
of three unbalanced phases as pictured in the bottom of the diagram. The
imbalance between phases arises because of the difference in magnitude and
phase shift between the sets of vectors. Notice that the colors (red, blue, and
yellow) of the separate sequence vectors correspond to three different phases
(A, B, and C, for example). To arrive at the final plot, the sum of vectors of
each phase is calculated. This resulting vector is the effective phasor
representation of that particular phase. This process, repeated, produces the
phasor for each of the three phases.
***** The three-phase case[edit] *****
Symmetrical components are most commonly used for analysis of three-phase
electrical_power_systems. The voltage or current of a three-phase system at
some point can be indicated by three phasors, called the three components of
the voltage or the current.
This article discusses voltage, however, the same considerations also apply to
current. In a perfectly balanced three-phase power system, the voltage phasor
components have equal magnitudes but are 120 degrees apart. In an unbalanced
system, the magnitudes and phases of the voltage phasor components are
different.
Decomposing the voltage phasor components into a set of symmetrical components
helps analyze the system as well as visualize any imbalances. If the three
voltage components are expressed as phasors (which are complex numbers), a
complex vector can be formed in which the three phase components are the
components of the vector. A vector for three phase voltage components can be
written as
           v   a b c   =   [     V  a        V  b        V  c      ]
      {\displaystyle \mathbf {v} _{abc}={\begin{bmatrix}V_{a}\\V_{b}\\V_{c}\end
      {bmatrix}}}  [{\displaystyle \mathbf {v} _{abc}={\begin{bmatrix}V_{a}\\V_
      {b}\\V_{c}\end{bmatrix}}}]
and decomposing the vector into three symmetrical components gives
           [     V  a        V  b        V  c      ]   =   [     V  a , 0
      V  b , 0        V  c , 0      ]   +   [     V  a , 1        V  b , 1
      V  c , 1      ]   +   [     V  a , 2        V  b , 2        V  c , 2
      ]     {\displaystyle {\begin{bmatrix}V_{a}\\V_{b}\\V_{c}\end{bmatrix}}=
      {\begin{bmatrix}V_{a,0}\\V_{b,0}\\V_{c,0}\end{bmatrix}}+{\begin
      {bmatrix}V_{a,1}\\V_{b,1}\\V_{c,1}\end{bmatrix}}+{\begin{bmatrix}V_
      {a,2}\\V_{b,2}\\V_{c,2}\end{bmatrix}}}  [{\displaystyle {\begin
      {bmatrix}V_{a}\\V_{b}\\V_{c}\end{bmatrix}}={\begin{bmatrix}V_{a,0}\\V_
      {b,0}\\V_{c,0}\end{bmatrix}}+{\begin{bmatrix}V_{a,1}\\V_{b,1}\\V_
      {c,1}\end{bmatrix}}+{\begin{bmatrix}V_{a,2}\\V_{b,2}\\V_{c,2}\end
      {bmatrix}}}]
where the subscripts 0, 1, and 2 refer respectively to the zero, positive, and
negative sequence components. The sequence components differ only by their
phase angles, which are symmetrical and so are        2 3   &#x03C0;
{\displaystyle \scriptstyle {\frac {2}{3}}\pi }  [\scriptstyle {\frac {2}
{3}}\pi ] radians or 120Â°.
**** A matrix[edit] ****
Define a phasor rotation operator alpha, which rotates a phasor vector
counterclockwise by 120 degrees:
         &#x03B1; &#x2261;  e    2 3   &#x03C0; i     {\displaystyle \alpha
      \equiv e^{{\frac {2}{3}}\pi i}}  [\alpha \equiv e^{{\frac {2}{3}}\pi i}].
Note that α3 = 1 so that α−1 = α2.
The zero sequence components have equal magnitude and in phase with each other,
therefore:
          V  0   &#x2261;  V  a , 0   =  V  b , 0   =  V  c , 0
      {\displaystyle V_{0}\equiv V_{a,0}=V_{b,0}=V_{c,0}}  [V_{0}\equiv V_
      {a,0}=V_{b,0}=V_{c,0}],
and the other phase sequences have the same magnitude, but their phases differ
by 120Â°:
              V  1      &#x2261;  V  a , 1   =  &#x03B1;  2    V  b , 1   =
      &#x03B1;  V  c , 1        V  2      &#x2261;  V  a , 2   = &#x03B1;  V  b
      , 2   =  &#x03B1;  2    V  c , 2         {\displaystyle {\begin
      {aligned}V_{1}&\equiv V_{a,1}=\alpha ^{2}V_{b,1}=\alpha V_{c,1}\\V_
      {2}&\equiv V_{a,2}=\alpha V_{b,2}=\alpha ^{2}V_{c,2}\\\end{aligned}}}  [
      {\displaystyle {\begin{aligned}V_{1}&\equiv V_{a,1}=\alpha ^{2}V_
      {b,1}=\alpha V_{c,1}\\V_{2}&\equiv V_{a,2}=\alpha V_{b,2}=\alpha ^{2}V_
      {c,2}\\\end{aligned}}}]
Thus,
               v   a b c      =   [     V  0        V  0        V  0      ]   +
      [     V  1        &#x03B1;  2    V  1       &#x03B1;  V  1      ]   +
      [     V  2       &#x03B1;  V  2        &#x03B1;  2    V  2      ]
      =   [    1   1   1     1    &#x03B1;  2     &#x03B1;     1   &#x03B1;
      &#x03B1;  2      ]     [     V  0        V  1        V  2      ]
      =   A     v   012         {\displaystyle {\begin{aligned}\mathbf {v} _
      {abc}&={\begin{bmatrix}V_{0}\\V_{0}\\V_{0}\end{bmatrix}}+{\begin
      {bmatrix}V_{1}\\\alpha ^{2}V_{1}\\\alpha V_{1}\end{bmatrix}}+{\begin
      {bmatrix}V_{2}\\\alpha V_{2}\\\alpha ^{2}V_{2}\end{bmatrix}}\\&={\begin
      {bmatrix}1&1&1\\1&\alpha ^{2}&\alpha \\1&\alpha &\alpha ^{2}\end
      {bmatrix}}{\begin{bmatrix}V_{0}\\V_{1}\\V_{2}\end{bmatrix}}\\&={\textbf
      {A}}\mathbf {v} _{012}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}\mathbf {v} _{abc}&={\begin{bmatrix}V_{0}\\V_{0}\\V_{0}\end
      {bmatrix}}+{\begin{bmatrix}V_{1}\\\alpha ^{2}V_{1}\\\alpha V_{1}\end
      {bmatrix}}+{\begin{bmatrix}V_{2}\\\alpha V_{2}\\\alpha ^{2}V_{2}\end
      {bmatrix}}\\&={\begin{bmatrix}1&1&1\\1&\alpha ^{2}&\alpha \\1&\alpha
      &\alpha ^{2}\end{bmatrix}}{\begin{bmatrix}V_{0}\\V_{1}\\V_{2}\end
      {bmatrix}}\\&={\textbf {A}}\mathbf {v} _{012}\end{aligned}}}]
where
           v   012   =   [     V  0        V  1        V  2      ]   ,   A   =
      [    1   1   1     1    &#x03B1;  2     &#x03B1;     1   &#x03B1;
      &#x03B1;  2      ]     {\displaystyle \mathbf {v} _{012}={\begin
      {bmatrix}V_{0}\\V_{1}\\V_{2}\end{bmatrix}},{\textbf {A}}={\begin
      {bmatrix}1&1&1\\1&\alpha ^{2}&\alpha \\1&\alpha &\alpha ^{2}\end
      {bmatrix}}}  [{\displaystyle \mathbf {v} _{012}={\begin{bmatrix}V_{0}\\V_
      {1}\\V_{2}\end{bmatrix}},{\textbf {A}}={\begin{bmatrix}1&1&1\\1&\alpha ^
      {2}&\alpha \\1&\alpha &\alpha ^{2}\end{bmatrix}}}]
In reverse phase rotation systems, the following matrix can be similarly
derived
           Aacb   =   [    1   1   1     1   &#x03B1;    &#x03B1;  2       1
      &#x03B1;  2     &#x03B1;    ]     {\displaystyle {\textbf {Aacb}}={\begin
      {bmatrix}1&1&1\\1&\alpha &\alpha ^{2}\\1&\alpha ^{2}&\alpha \end
      {bmatrix}}}  [{\displaystyle {\textbf {Aacb}}={\begin
      {bmatrix}1&1&1\\1&\alpha &\alpha ^{2}\\1&\alpha ^{2}&\alpha \end
      {bmatrix}}}]
**** Decomposition[edit] ****
The sequence components are derived from the analysis equation
           v   012   =    A    &#x2212; 1     v   a b c     {\displaystyle
      \mathbf {v} _{012}={\textbf {A}}^{-1}\mathbf {v} _{abc}}  [{\displaystyle
      \mathbf {v} _{012}={\textbf {A}}^{-1}\mathbf {v} _{abc}}]
where
            A    &#x2212; 1   =   1 3     [    1   1   1     1   &#x03B1;
      &#x03B1;  2       1    &#x03B1;  2     &#x03B1;    ]     {\displaystyle
      {\textbf {A}}^{-1}={\frac {1}{3}}{\begin{bmatrix}1&1&1\\1&\alpha &\alpha
      ^{2}\\1&\alpha ^{2}&\alpha \end{bmatrix}}}  [{\textbf {A}}^{-1}={\frac
      {1}{3}}{\begin{bmatrix}1&1&1\\1&\alpha &\alpha ^{2}\\1&\alpha ^{2}&\alpha
      \end{bmatrix}}]
The above two equations tell how to derive symmetrical components corresponding
to an asymmetrical set of three phasors:
    * Sequence 0 is one-third the sum of the original three phasors.
    * Sequence 1 is one-third the sum of the original three phasors rotated
      counterclockwise 0Â°, 120Â°, and 240Â°.
    * Sequence 2 is one-third the sum of the original three phasors rotated
      clockwise 0Â°, 240Â°, and 120Â°.
Visually, if the original components are symmetrical, sequences 1 and 2 will
each form a triangle, summing to zero, and sequence 0 components will sum to a
straight line.
**** Intuition[edit] ****
Napoleon's theorem: If the triangles centered on L, M, and N are equilateral,
then so is the green triangle.
The phasors       V  ( a b )   =  V  ( a )   &#x2212;  V  ( b )   ;   V  ( b c
)   =  V  ( b )   &#x2212;  V  ( c )   ;   V  ( c a )   =  V  ( c )   &#x2212;
V  ( a )      {\displaystyle \scriptstyle V_{(ab)}=V_{(a)}-V_{(b)};\;V_{
(bc)}=V_{(b)}-V_{(c)};\;V_{(ca)}=V_{(c)}-V_{(a)}}  [\scriptstyle V_{(ab)}=V_{
(a)}-V_{(b)};\;V_{(bc)}=V_{(b)}-V_{(c)};\;V_{(ca)}=V_{(c)}-V_{(a)}] form a
closed triangle (e.g., outer voltages or line to line voltages). To find the
synchronous and inverse components of the phases, take any side of the outer
triangle and draw the two possible equilateral triangles sharing the selected
side as base. These two equilateral triangles represent a synchronous and an
inverse system.
If the phasors V were a perfectly synchronous system, the vertex of the outer
triangle not on the base line would be at the same position as the
corresponding vertex of the equilateral triangle representing the synchronous
system. Any amount of inverse component would mean a deviation from this
position. The deviation is exactly 3 times the inverse phase component.
The synchronous component is in the same manner 3 times the deviation from the
"inverse equilateral triangle". The directions of these components are correct
for the relevant phase. It seems counter intuitive that this works for all
three phases regardless of the side chosen but that is the beauty of this
illustration. The graphic is from Napoleon's_Theorem, which matches a graphical
calculation technique that sometimes appears in older references books.[4]
***** Poly-phase case[edit] *****
It can be seen that the transformation matrix above is a discrete_Fourier
transform, and as such, symmetrical components can be calculated for any poly-
phase system.
***** Contribution of harmonics to symmetrical components in 3-phase power
systems[edit] *****
Harmonics often occur in power systems as a consequence of non-linear loads.
Each order of harmonics contributes to different sequence components. Harmonics
of order      2 n    {\displaystyle \scriptstyle 2n}  [\scriptstyle 2n] make no
contribution. Harmonics of order      3 + 6 n    {\displaystyle \scriptstyle
3+6n}  [{\displaystyle \scriptstyle 3+6n}] contribute to the zero sequence.
Harmonics of order      5 + 6 n    {\displaystyle \scriptstyle 5+6n}  [
{\displaystyle \scriptstyle 5+6n}] contribute to the negative sequence.
Harmonics of order      7 + 6 n    {\displaystyle \scriptstyle 7+6n}  [
{\displaystyle \scriptstyle 7+6n}] contribute to the positive sequence.
Note that the rules above are only applicable if the phase values (or
distortion) are exactly the same.
***** Consequence of the zero sequence component in power systems[edit] *****
The zero sequence represents the component of the unbalanced phasors that is
equal in magnitude and phase. Because they are in phase, zero sequence currents
flowing through an n-phase network will sum to n times the magnitude of the
individual zero sequence currents components. Under normal operating conditions
this sum is small enough to be negligible. However, during large zero sequence
events such as lightning strikes, this nonzero sum of currents can lead to a
larger current flowing through the neutral conductor than the individual phase
conductors. Because neutral conductors are typically not larger than individual
phase conductors, and are often smaller than these conductors, a large zero
sequence component can lead to overheating of neutral conductors and to fires.
One way to prevent large zero sequence currents is to use a delta connection,
which appears as an open circuit to zero sequence currents. For this reason,
most transmission, and much sub-transmission is implemented using delta. Much
distribution is also implemented using delta, although "old work" distribution
systems have occasionally been "wyed-up" (converted from delta to wye) so as to
increase the line's capacity at a low converted cost, but at the expense of a
higher central station protective relay cost.
***** See also[edit] *****
    * Symmetry
    * Dqo_transformation
    * Alphaâbeta_transformation
***** References[edit] *****
  Notes
   1. ^HadjsaÃ¯d, Nouredine; SabonnadiÃ¨re, Jean-Claude (2013). Power_Systems
      and_Restructuring. John Wiley & Sons. p. 244. ISBN 9781118599921.
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
   3. ^ Charles L. Fortescue, "Method_of_Symmetrical_Co-Ordinates_Applied_to
      the_Solution_of_Polyphase_Networks". Presented at the 34th annual
      convention of the AIEE (American Institute of Electrical Engineers) in
      Atlantic City, N.J. on 28 June 1918. Published in: AIEE Transactions,
      vol. 37, part II, pages 1027â1140 (1918). For a brief history of the
      early years of symmetrical component theory, see: J. Lewis Blackburn,
      Symmetrical Components for Power Engineering (Boca Raton, Florida: CRC
      Press, 1993), pages 3â4.
   4. ^  Gabriele Kass-Simon, Patricia Farnes, Deborah Nash (ed), Women of
      Science: Righting the Record , Indiana University Press, 1993,
   5. ISBN 0253208130. pages 164-168
   6. ^Wagner, C. F.; Evans, R. D. (1933). Symmetrical Components. New York and
      London: McGraw Hill. p. 265.
  Bibliography
    * J. Lewis Blackburn Symmetrical Components for Power Systems Engineering,
      Marcel Dekker, New York (1993).
ISBN 0-8247-8767-6
William D. Stevenson, Jr. Elements of Power System Analysis Third Edition,
McGraw-Hill, New York (1975).
ISBN 0-07-061285-4.
History_article from IEEE on early development of symmetrical components,
retrieved May 12, 2005.
Westinghouse Corporation, Applied Protective Relaying, 1976, Westinghouse
Corporation, no ISBN, Library of Congress card no. 76-8060 - a standard
reference on electromechanical protective relays

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Symmetrical_components&oldid=909032745"
Categories:
    * Electrical_engineering
    * Three-phase_AC_power
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_November_2016
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
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Nederlands
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
Edit_links
    * This page was last edited on 2 August 2019, at 16:12 (UTC).
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
