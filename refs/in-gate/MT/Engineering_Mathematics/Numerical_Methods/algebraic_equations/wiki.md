The following text has been accessed from https://en.wikipedia.org/wiki/Algebraic_equation at Fri Aug 9 03:26:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Algebraic equation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article may be expanded with text translated from the corresponding_article
 in French. (August 2013) Click [show] for important translation instructions.
     * View a machine-translated version of the French article.
     * Machine translation like Deepl or Google_Translate is a useful starting
       point for translations, but translators must revise errors as necessary
       and confirm that the translation is accurate, rather than simply copy-
       pasting machine-translated text into the English Wikipedia.
     * Do not translate text that appears unreliable or low-quality. If possible,
       verify the text with references provided in the foreign-language article.
     * You must provide copyright_attribution in the edit_summary accompanying
       your translation by providing an interlanguage_link to the source of your
       translation. A model attribution edit summary (using German): Content in
       this edit is translated from the existing German Wikipedia article at [[:
       de:Exact name of German article]]; see its history for attribution.
     * You should also add the template {{Translated|fr|Ãquation polynomiale}}
       to the talk_page.
     * For more guidance, see Wikipedia:Translation.
 This article needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be
 challenged and removed.
 Find sources: "Algebraic_equation" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (January 2010)(Learn_how_and_when_to_remove_this_template_message)
In mathematics, an algebraic equation or polynomial equation is an equation of
the form
         P = Q   {\displaystyle P=Q}  [P=Q]
where P and Q are polynomials with coefficients in some field, often the field
of the rational_numbers. For most authors, an algebraic equation is univariate,
which means that it involves only one variable. On the other hand, a polynomial
equation may involve several variables, in which case it is called multivariate
and the term polynomial equation is usually preferred to algebraic equation.
For example,
          x  5   &#x2212; 3 x + 1 = 0   {\displaystyle x^{5}-3x+1=0}  [x^{5}-
      3x+1=0]
is an algebraic equation with integer coefficients and
          y  4   +    x y  2   =    x  3   3   &#x2212; x  y  2   +  y  2
      &#x2212;   1 7     {\displaystyle y^{4}+{\frac {xy}{2}}={\frac {x^{3}}
      {3}}-xy^{2}+y^{2}-{\frac {1}{7}}}  [y^{4}+{\frac {xy}{2}}={\frac {x^{3}}
      {3}}-xy^{2}+y^{2}-{\frac {1}{7}}]
is a multivariate polynomial equation over the rationals.
Some but not all polynomial equations with rational_coefficients have a
solution that is an algebraic_expression that can be found using a finite
number of operations that involve only those same types of coefficients (that
is, can be solved_algebraically). This can be done for all such equations of
degree one, two, three, or four; but for degree five or more it can only be
done for some equations, not_for_all. A large amount of research has been
devoted to compute efficiently accurate approximations of the real or complex
solutions of a univariate algebraic equation (see Root-finding_algorithm) and
of the common solutions of several multivariate polynomial equations (see
System_of_polynomial_equations).
⁰
***** Contents *****
    * 1_History
    * 2_Areas_of_study
    * 3_Solutions
    * 4_See_also
    * 5_References
***** History[edit] *****
The study of algebraic equations is probably as old as mathematics: the
Babylonian_mathematicians, as early as 2000 BC could solve some kinds of
quadratic_equations (displayed on Old_Babylonian clay_tablets).
Univariate algebraic equations over the rationals (i.e., with rational
coefficients) have a very long history. Ancient mathematicians wanted the
solutions in the form of radical_expressions, like     x =    1 +   5    2
{\displaystyle x={\frac {1+{\sqrt {5}}}{2}}}  [x={\frac  {1+{\sqrt  {5}}}{2}}]
for the positive solution of      x  2   &#x2212; x &#x2212; 1 = 0
{\displaystyle x^{2}-x-1=0}  [x^{2}-x-1=0]. The ancient Egyptians knew how to
solve equations of degree 2 in this manner. The Indian mathematician
Brahmagupta (597â668 AD) explicitly described the quadratic formula in his
treatise BrÄhmasphuá¹­asiddhÄnta published in 628 AD, but written in words
instead of symbols. In the 9th century Muhammad_ibn_Musa_al-Khwarizmi and other
Islamic mathematicians derived the quadratic_formula, the general solution of
equations of degree 2, and recognized the importance of the discriminant.
During the Renaissance in 1545, Gerolamo_Cardano published the solution of
Scipione_del_Ferro and NiccolÃ²_Fontana_Tartaglia to equations_of_degree_3 and
that of Lodovico_Ferrari for equations_of_degree_4. Finally Niels_Henrik_Abel
proved, in 1824, that equations_of_degree_5 and higher do not have general
solutions using radicals. Galois_theory, named after Ãvariste_Galois, showed
that some equations of at least degree 5 do not even have an idiosyncratic
solution in radicals, and gave criteria for deciding if an equation is in fact
solvable using radicals.
***** Areas of study[edit] *****
The algebraic equations are the basis of a number of areas of modern
mathematics: Algebraic_number_theory is the study of (univariate) algebraic
equations over the rationals (that is, with rational coefficients). Galois
theory was introduced by Ãvariste_Galois to specify criteria for deciding if
an algebraic equation may be solved in terms of radicals. In field_theory, an
algebraic_extension is an extension such that every element is a root of an
algebraic equation over the base field. Transcendental_number_theory is the
study of the real numbers which are not solutions to an algebraic equation over
the rationals. A Diophantine_equation is a (usually multivariate) polynomial
equation with integer coefficients for which one is interested in the integer
solutions. Algebraic_geometry is the study of the solutions in an algebraically
closed_field of multivariate polynomial equations.
Two equations are equivalent if they have the same set of solutions. In
particular the equation     P = Q   {\displaystyle P=Q}  [P=Q] is equivalent to
P &#x2212; Q = 0   {\displaystyle P-Q=0}  [P-Q=0]. It follows that the study of
algebraic equations is equivalent to the study of polynomials.
A polynomial equation over the rationals can always be converted to an
equivalent one in which the coefficients are integers. For example, multiplying
through by 42 = 2Â·3Â·7 and grouping its terms in the first member, the
previously mentioned polynomial equation      y  4   +    x y  2   =    x  3
3   &#x2212; x  y  2   +  y  2   &#x2212;   1 7     {\displaystyle y^{4}+{\frac
{xy}{2}}={\frac {x^{3}}{3}}-xy^{2}+y^{2}-{\frac {1}{7}}}  [y^{4}+{\frac {xy}
{2}}={\frac {x^{3}}{3}}-xy^{2}+y^{2}-{\frac {1}{7}}] becomes
         42  y  4   + 21 x y &#x2212; 14  x  3   + 42 x  y  2   &#x2212; 42  y
      2   + 6 = 0.   {\displaystyle 42y^{4}+21xy-14x^{3}+42xy^{2}-42y^{2}+6=0.}
      [42y^{4}+21xy-14x^{3}+42xy^{2}-42y^{2}+6=0.]
Because sine, exponentiation, and 1/T are not polynomial functions,
          e  T    x  2   +   1 T   x y + sin &#x2061; ( T ) z &#x2212; 2 = 0
      {\displaystyle e^{T}x^{2}+{\frac {1}{T}}xy+\sin(T)z-2=0}  [e^{T}x^{2}+
      {\frac  {1}{T}}xy+\sin(T)z-2=0]
is not a polynomial equation in the four variables x, y, z, and T over the
rational numbers. However, it is a polynomial equation in the three variables
x, y, and z over the field of the elementary_functions in the variable T.
***** Solutions[edit] *****
Main article: Polynomial_Â§ Solving_polynomial_equations
As for any equation, the solutions of an equation are the values of the
variables for which the equation is true. For univariate algebraic equations
these are also called roots, even if, properly speaking, one should say the
solutions of the algebraic equation P=0 are the roots of the polynomial P. When
solving an equation, it is important to specify in which set the solutions are
allowed. For example, for an equation over the rationals one may look for
solutions in which all the variables are integers. In this case the equation is
a Diophantine_equation. One may also be interested only in the real solutions.
However, for univariate algebraic equations, the number of solutions is finite,
and all solutions are contained in any algebraically_closed_field containing
the coefficients—for example, the field of complex numbers in the case of
equations over the rationals. It follows that without precision "root" and
"solution" usually mean "solution in an algebraically closed field".
***** See also[edit] *****
    * Algebraic_function
    * Algebraic_number
    * Root_finding
    * Linear_equation (degree = 1)
    * Quadratic_equation (degree = 2)
    * Cubic_equation (degree = 3)
    * Quartic_equation (degree = 4)
    * Quintic_equation (degree = 5)
    * Sextic_equation (degree = 6)
    * Septic_equation (degree = 7)
    * System_of_linear_equations
    * System_of_polynomial_equations
    * Linear_Diophantine_equation
    * Linear_equation_over_a_ring
    * Cramer's_theorem_(algebraic_curves), on the number of points usually
      sufficient to determine a bivariate n-th degree curve
***** References[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Algebraic_equation",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
Weisstein,_Eric_W. "Algebraic_Equation". MathWorld.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Algebraic_equation&oldid=902799358"
Categories:
    * Polynomials
    * Equations
Hidden categories:
    * Articles_to_be_expanded_from_August_2013
    * All_articles_to_be_expanded
    * Science_articles_needing_translation_from_French_Wikipedia
    * Articles_needing_additional_references_from_January_2010
    * All_articles_needing_additional_references
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * LietuviÅ³
    * æ¥æ¬èª
    * Norsk_nynorsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * Simple_English
    * SlovenÄina
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 21 June 2019, at 10:12 (UTC).
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
