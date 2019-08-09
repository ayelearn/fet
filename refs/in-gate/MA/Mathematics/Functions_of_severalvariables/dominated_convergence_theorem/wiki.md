The following text has been accessed from https://en.wikipedia.org/wiki/Dominated_convergence_theorem at Fri Aug 9 02:34:03 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Dominated convergence theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In measure_theory, Lebesgue's dominated convergence theorem provides sufficient
conditions under which almost_everywhere convergence of a sequence of functions
implies convergence in the L1 norm. Its power and utility are two of the
primary theoretical advantages of Lebesgue_integration over Riemann
integration.
In addition to its frequent appearance in mathematical analysis and partial
differential equations, it is widely used in probability_theory, since it gives
a sufficient condition for the convergence of expected_values of random
variables.
⁰
***** Contents *****
    * 1_Statement_of_the_theorem
    * 2_Proof_of_the_theorem
    * 3_Discussion_of_the_assumptions
    * 4_Bounded_convergence_theorem
          o 4.1_Proof
    * 5_Dominated_convergence_in_Lp-spaces_(corollary)
    * 6_Extensions
    * 7_See_also
    * 8_References
***** Statement of the theorem[edit] *****
Lebesgue's Dominated Convergence Theorem. Let {fn} be a sequence of complex-
valued measurable_functions on a measure_space (S, Î£, Î¼). Suppose that the
sequence converges_pointwise to a function f and is dominated by some
integrable function g in the sense that
          |   f  n   ( x )  |  &#x2264; g ( x )   {\displaystyle |f_{n}(x)|\leq
      g(x)}  [    |f_n(x)| \le g(x)]
for all numbers n in the index set of the sequence and all points x â S. Then
f is integrable and
          lim  n &#x2192; &#x221E;    &#x222B;  S    |   f  n   &#x2212; f  |
      d &#x03BC; = 0   {\displaystyle \lim _{n\to \infty }\int _{S}|f_{n}-
      f|\,d\mu =0}  [ \lim_{n\to\infty} \int_S |f_n-f|\,d\mu = 0]
which also implies
          lim  n &#x2192; &#x221E;    &#x222B;  S    f  n    d &#x03BC; =
      &#x222B;  S   f  d &#x03BC;   {\displaystyle \lim _{n\to \infty }\int _
      {S}f_{n}\,d\mu =\int _{S}f\,d\mu }  [\lim_{n\to\infty} \int_S f_n\,d\mu =
      \int_S f\,d\mu]
Remark 1. The statement "g is integrable" means that measurable function g is
Lebesgue integrable; i.e.
          &#x222B;  S    |  g  |   d &#x03BC; < &#x221E; .   {\displaystyle
      \int _{S}|g|\,d\mu <\infty .}  [\int_S|g|\,d\mu < \infty.]
Remark 2. The convergence of the sequence and domination by g can be relaxed to
hold only Î¼-almost_everywhere provided the measure space (S, Î£, Î¼) is
complete or f is chosen as a measurable function which agrees Î¼-almost
everywhere with the Î¼-almost everywhere existing pointwise limit. (These
precautions are necessary, because otherwise there might exist a non-measurable
subset of a Î¼-null set N â Î£, hence f might not be measurable.)
Remark 3. If Î¼(S) < â, the condition that there is a dominating integrable
function g can be relaxed to uniform_integrability of the sequence {fn}, see
Vitali_convergence_theorem.
***** Proof of the theorem[edit] *****
Without_loss_of_generality, one can assume that f is real, because one can
split f into its real and imaginary parts (remember that a sequence of complex
numbers converges if_and_only_if both its real and imaginary counterparts
converge) and apply the triangle_inequality at the end.
Lebesgue's dominated convergence theorem is a special case of the
FatouâLebesgue_theorem. Below, however, is a direct proof that uses Fatouâs
lemma as the essential tool.
Since f is the pointwise limit of the sequence (fn) of measurable functions
that are dominated by g, it is also measurable and dominated by g, hence it is
integrable. Furthermore, (these will be needed later),
          |  f &#x2212;  f  n    |  &#x2264;  |  f  |  +  |   f  n    |
      &#x2264; 2 g   {\displaystyle |f-f_{n}|\leq |f|+|f_{n}|\leq 2g}  [    |f-
      f_n| \le |f| + |f_n| \leq 2g]
for all n and
          lim&#x2006;sup  n &#x2192; &#x221E;    |  f &#x2212;  f  n    |  = 0.
      {\displaystyle \limsup _{n\to \infty }|f-f_{n}|=0.}  [    \limsup_
      {n\to\infty} |f-f_n| = 0.]
The second of these is trivially true (by the very definition of f). Using
linearity_and_monotonicity_of_the_Lebesgue_integral,
          |   &#x222B;  S    f  d &#x03BC;  &#x2212;  &#x222B;  S     f  n    d
      &#x03BC;   |  =  |   &#x222B;  S    ( f &#x2212;  f  n   )  d &#x03BC;
      |  &#x2264;  &#x222B;  S     |  f &#x2212;  f  n    |   d &#x03BC;  .
      {\displaystyle \left|\int _{S}{f\,d\mu }-\int _{S}{f_{n}\,d\mu
      }\right|=\left|\int _{S}{(f-f_{n})\,d\mu }\right|\leq \int _{S}{|f-f_
      {n}|\,d\mu }.}  [    \left | \int_S{f\,d\mu} - \int_S{f_n\,d\mu} \right|=
      \left| \int_S{(f-f_n)\,d\mu} \right|\le \int_S{|f-f_n|\,d\mu}.]
By the reverse_Fatou_lemma (it is here that we use the fact that |fâfn| is
bounded above by an integrable function)
          lim&#x2006;sup  n &#x2192; &#x221E;    &#x222B;  S    |  f &#x2212;
      f  n    |   d &#x03BC; &#x2264;  &#x222B;  S    lim&#x2006;sup  n
      &#x2192; &#x221E;    |  f &#x2212;  f  n    |   d &#x03BC; = 0 ,
      {\displaystyle \limsup _{n\to \infty }\int _{S}|f-f_{n}|\,d\mu \leq \int
      _{S}\limsup _{n\to \infty }|f-f_{n}|\,d\mu =0,}  [\limsup_{n\to\infty}
      \int_S |f-f_n|\,d\mu \le \int_S \limsup_{n\to\infty} |f-f_n|\,d\mu = 0,]
which implies that the limit exists and vanishes i.e.
          lim  n &#x2192; &#x221E;    &#x222B;  S    |  f &#x2212;  f  n    |
      d &#x03BC; = 0.   {\displaystyle \lim _{n\to \infty }\int _{S}|f-f_
      {n}|\,d\mu =0.}  [\lim_{n\to\infty} \int_S |f-f_n|\,d\mu= 0.]
Finally, since
          lim  n &#x2192; &#x221E;    |   &#x222B;  S   f d &#x03BC; &#x2212;
      &#x222B;  S    f  n   d &#x03BC;  |  &#x2264;  lim  n &#x2192; &#x221E;
      &#x222B;  S    |  f &#x2212;  f  n    |   d &#x03BC; = 0.
      {\displaystyle \lim _{n\to \infty }\left|\int _{S}fd\mu -\int _{S}f_
      {n}d\mu \right|\leq \lim _{n\to \infty }\int _{S}|f-f_{n}|\,d\mu =0.}  [
      {\displaystyle \lim _{n\to \infty }\left|\int _{S}fd\mu -\int _{S}f_
      {n}d\mu \right|\leq \lim _{n\to \infty }\int _{S}|f-f_{n}|\,d\mu =0.}]
we have that
          lim  n &#x2192; &#x221E;    &#x222B;  S    f  n    d &#x03BC; =
      &#x222B;  S   f  d &#x03BC; .   {\displaystyle \lim _{n\to \infty }\int _
      {S}f_{n}\,d\mu =\int _{S}f\,d\mu .}  [{\displaystyle \lim _{n\to \infty
      }\int _{S}f_{n}\,d\mu =\int _{S}f\,d\mu .}]
The theorem now follows.
If the assumptions hold only Î¼-almost everywhere, then there exists a Î¼-null
set N â Î£ such that the functions fn 1Sâ\âN satisfy the assumptions
everywhere on S. Then the function f(x) defined as the pointwise limit of fn(x)
for x â Sâ\âN and by f(x) = 0 for x â N, is measurable and is the
pointwise limit of this modified function sequence. The values of these
integrals are not influenced by these changes to the integrands on this Î¼-null
set N, so the theorem continues to hold.
DCT holds even if fn converges to f in measure (finite measure) and the
dominating function is non-negative almost everywhere.
***** Discussion of the assumptions[edit] *****
The assumption that the sequence is dominated by some integrable g cannot be
dispensed with. This may be seen as follows: define fn(x) = n for x in the
interval (0, 1/n] and fn(x) = 0 otherwise. Any g which dominates the sequence
must also dominate the pointwise supremum h = supn fn. Observe that
          &#x222B;  0   1   h ( x )  d x &#x2265;  &#x222B;   1 m    1    h ( x
      )  d x  =  &#x2211;  n = 1   m &#x2212; 1    &#x222B;   (    1  n + 1
      ,   1 n    ]     h ( x )  d x  &#x2265;  &#x2211;  n = 1   m &#x2212; 1
      &#x222B;   (    1  n + 1    ,   1 n    ]     n  d x  =  &#x2211;  n = 1
      m &#x2212; 1     1  n + 1    &#x2192; &#x221E;   as&#xA0;  m &#x2192;
      &#x221E;   {\displaystyle \int _{0}^{1}h(x)\,dx\geq \int _{\frac {1}{m}}^
      {1}{h(x)\,dx}=\sum _{n=1}^{m-1}\int _{\left({\frac {1}{n+1}},{\frac {1}
      {n}}\right]}{h(x)\,dx}\geq \sum _{n=1}^{m-1}\int _{\left({\frac {1}
      {n+1}},{\frac {1}{n}}\right]}{n\,dx}=\sum _{n=1}^{m-1}{\frac {1}{n+1}}\to
      \infty \qquad {\text{as }}m\to \infty }  [\int_0^1 h(x)\,dx \ge \int_
      {\frac{1}{m}}^1{h(x)\,dx} = \sum_{n=1}^{m-1} \int_{\left(\frac{1}
      {n+1},\frac{1}{n}\right]}{h(x)\,dx} \ge \sum_{n=1}^{m-1} \int_{\left
      (\frac{1}{n+1},\frac{1}{n}\right]}{n\,dx}=\sum_{n=1}^{m-1} \frac{1}{n+1}
      \to \infty \qquad \text{as }m\to\infty  ]
by the divergence of the harmonic_series. Hence, the monotonicity of the
Lebesgue integral tells us that there exists no integrable function which
dominates the sequence on [0,1]. A direct calculation shows that integration
and pointwise limit do not commute for this sequence:
          &#x222B;  0   1    lim  n &#x2192; &#x221E;    f  n   ( x )  d x = 0
      &#x2260; 1 =  lim  n &#x2192; &#x221E;    &#x222B;  0   1    f  n   ( x )
      d x ,   {\displaystyle \int _{0}^{1}\lim _{n\to \infty }f_{n}
      (x)\,dx=0\neq 1=\lim _{n\to \infty }\int _{0}^{1}f_{n}(x)\,dx,}
      [\int_0^1 \lim_{n\to\infty} f_n(x)\,dx = 0 \neq 1 = \lim_
      {n\to\infty}\int_0^1 f_n(x)\,dx,]
because the pointwise limit of the sequence is the zero_function. Note that the
sequence {fn} is not even uniformly_integrable, hence also the Vitali
convergence_theorem is not applicable.
***** Bounded convergence theorem[edit] *****
One corollary to the dominated convergence theorem is the bounded convergence
theorem, which states that if {fn} is a sequence of uniformly_bounded complex-
valued measurable_functions which converges pointwise on a bounded measure
space (S, Î£, Î¼) (i.e. one in which Î¼(S) is finite) to a function f, then the
limit f is an integrable function and
          lim  n &#x2192; &#x221E;    &#x222B;  S     f  n    d &#x03BC;  =
      &#x222B;  S    f  d &#x03BC;  .   {\displaystyle \lim _{n\to \infty }\int
      _{S}{f_{n}\,d\mu }=\int _{S}{f\,d\mu }.}  [\lim_{n\to\infty} \int_S
      {f_n\,d\mu} = \int_S{f\,d\mu}.]
Remark: The pointwise convergence and uniform boundedness of the sequence can
be relaxed to hold only Î¼-almost_everywhere, provided the measure space (S,
Î£, Î¼) is complete or f is chosen as a measurable function which agrees Î¼-
almost everywhere with the Î¼-almost everywhere existing pointwise limit.
**** Proof[edit] ****
Since the sequence is uniformly bounded, there is a real number M such that |fn
(x)| â¤ M for all x â S and for all n. Define g(x) = M for all x â S. Then
the sequence is dominated by g. Furthermore, g is integrable since it is a
constant function on a set of finite measure. Therefore, the result follows
from the dominated convergence theorem.
If the assumptions hold only Î¼-almost everywhere, then there exists a Î¼-null
set N â Î£ such that the functions fn1S\N satisfy the assumptions everywhere
on S.
***** Dominated convergence in Lp-spaces (corollary)[edit] *****
Let     ( &#x03A9; ,   A   , &#x03BC; )   {\displaystyle (\Omega ,{\mathcal
{A}},\mu )}  [(\Omega,\mathcal{A},\mu)] be a measure_space,  1 â¤ p < â a
real number and {fn} a sequence of       A     {\displaystyle {\mathcal {A}}}
[{\mathcal {A}}]-measurable functions      f  n   : &#x03A9; &#x2192;  C
&#x222A; { &#x221E; }   {\displaystyle f_{n}:\Omega \to \mathbb {C} \cup \
{\infty \}}  [{\displaystyle f_{n}:\Omega \to \mathbb {C} \cup \{\infty \}}].
Assume the sequence {fn} converges Î¼-almost everywhere to an       A
{\displaystyle {\mathcal {A}}}  [{\mathcal {A}}]-measurable function f, and is
dominated by a     g &#x2208;  L  p     {\displaystyle g\in L^{p}}  [g \in L^p]
(cf. Lp_space), i.e., for every natural number n we have: |fn| â¤ g, Î¼-almost
everywhere.
Then all fn as well as f are in      L  p     {\displaystyle L^{p}}  [L^{p}]
and the sequence {fn} converges to f in the_sense_of______L__p_____
{\displaystyle_L^{p}}__[L^{p}], i.e.:
          lim  n &#x2192; &#x221E;   &#x2016;  f  n   &#x2212; f  &#x2016;  p
      =  lim  n &#x2192; &#x221E;     (   &#x222B;  &#x03A9;    |   f  n
      &#x2212; f   |   p    d &#x03BC;  )    1 p    = 0.   {\displaystyle \lim
      _{n\to \infty }\|f_{n}-f\|_{p}=\lim _{n\to \infty }\left(\int _{\Omega
      }|f_{n}-f|^{p}\,d\mu \right)^{\frac {1}{p}}=0.}  [\lim_{n \to
      \infty}\|f_n-f\|_p =\lim_{n \to \infty}\left(\int_\Omega |f_n-f|^p
      \,d\mu\right)^{\frac{1}{p}} = 0.]
Idea of the proof: Apply the original theorem to the function sequence      h
n   =  |   f  n   &#x2212; f   |   p     {\displaystyle h_{n}=|f_{n}-f|^{p}}
[h_n = |f_n-f|^p] with the dominating function     ( 2 g  )  p
{\displaystyle (2g)^{p}}  [(2g)^p].
***** Extensions[edit] *****
The dominated convergence theorem applies also to measurable functions with
values in a Banach_space, with the dominating function still being non-negative
and integrable as above. The assumption of convergence almost everywhere can be
weakened to require only convergence_in_measure.
***** See also[edit] *****
    * Convergence_of_random_variables, Convergence_in_mean
    * Monotone_convergence_theorem (does not require domination by an
      integrable function but assumes monotonicity of the sequence instead)
    * ScheffÃ©âs_lemma
    * Uniform_integrability
    * Vitali_convergence_theorem (a generalization of Lebesgue's dominated
      convergence theorem)
***** References[edit] *****
    * Bartle, R.G. (1995). The_Elements_of_Integration_and_Lebesgue_Measure.
      Wiley Interscience.
Royden, H.L. (1988). Real_Analysis. Prentice Hall.
Weir, Alan J. (1973). "The Convergence Theorems". Lebesgue Integration and
Measure. Cambridge: Cambridge University Press. pp. 93â118. ISBN 0-521-08728-
7.
Williams,_D. (1991). Probability with martingales. Cambridge University Press.
ISBN 0-521-40605-6.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Dominated_convergence_theorem&oldid=904336373"
Categories:
    * Theorems_in_real_analysis
    * Theorems_in_measure_theory
    * Probability_theorems
Hidden categories:
    * Articles_containing_proofs
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
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÄina
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 1 July 2019, at 13:47 (UTC).
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
