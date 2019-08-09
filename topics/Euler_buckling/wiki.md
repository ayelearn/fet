The following text has been accessed from https://en.wikipedia.org/wiki/Euler%27s_critical_load at Fri Aug 9 03:32:49 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Euler's critical load ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The critical load is the maximum load (unit: Newton, it is a force) which a
column can bear while staying straight. It is given by the formula:[1]
      Fig. 1: Column effective length factors for Euler's critical load. In
      practical design, it is recommended to increase the factors as shown
      above.
          P  c r   =     &#x03C0;  2   E I   ( K L  )  2        {\displaystyle
      P_{cr}={\frac {\pi ^{2}EI}{(KL)^{2}}}}  [{\displaystyle P_{cr}={\frac
      {\pi ^{2}EI}{(KL)^{2}}}}]
where
          P  c r     {\displaystyle P_{cr}}  [{\displaystyle P_{cr}}] = Euler's
      critical load (longitudinal compression load on column),
         E   {\displaystyle E}  [E] = modulus_of_elasticity of column material,
         I   {\displaystyle I}  [I] = minimum area_moment_of_inertia of the
      cross section of the column,
         L   {\displaystyle L}  [L] = unsupported length of column,
         K   {\displaystyle K}  [K] = column_effective_length_factor

This formula was derived in 1757, by the Swiss mathematician Leonhard_Euler.
The column will remain straight for loads less than the critical load. The
"critical load" is the greatest load that will not cause lateral deflection
(buckling). For loads greater than the critical load, the column will deflect
laterally. The critical load puts the column in a state of unstable
equilibrium. A load beyond the critical load causes the column to fail by
buckling. As the load is increased beyond the critical load the lateral
deflections increase, until it may fail in other modes such as yielding of the
material. Loading of columns beyond the critical load are not addressed in this
article.
Around 1900, J. B. Johnson showed that at low slenderness ratios an alternative
formula should be used.
⁰
***** Contents *****
    * 1_Assumptions_of_the_model
    * 2_Mathematical_derivation:_Pin_ended_column
    * 3_Mathematical_derivation:_General_approach
    * 4_See_also
    * 5_References
***** Assumptions of the model[edit] *****
The following assumptions are made while deriving Eulerâs formula:[2]
   1. The material of the column is homogeneous and isotropic.
   2. The compressive load on the column is axial only.
   3. The column is free from initial stress.
   4. The weight of the column is neglected.
   5. The column is initially straight (no eccentricity of the axial load).
   6. Pin joints are friction-less (no moment constraint) and fixed ends are
      rigid (no rotation deflection).
   7. The cross-section of the column is uniform throughout its length.
   8. The direct stress is very small as compared to the bending stress (the
      material is compressed only within the elastic range of strains).
   9. The length of the column is very large as compared to the cross-sectional
      dimensions of the column.
  10. The column fails only by buckling. This is true if the compressive stress
      in the column does not exceed the yield_strength      &#x03C3;  y
      {\displaystyle \sigma _{y}}  [\sigma_y] (see figure 2):
      Fig. 2: Critical stress vs slenderness ratio for steel, for E=200GPa,
      Yield strength=240MPa
         &#x03C3; =    P  c r   A   =     &#x03C0;  2   E   (  L  e    /  r  )
      2      <  &#x03C3;  y     {\displaystyle \sigma ={\frac {P_{cr}}{A}}=
      {\frac {\pi ^{2}E}{(L_{e}/r)^{2}}}<\sigma _{y}}  [{\displaystyle \sigma =
      {\frac {P_{cr}}{A}}={\frac {\pi ^{2}E}{(L_{e}/r)^{2}}}<\sigma _{y}}]
For slender columns, critical stress is usually lower than yield stress, and in
the elastic range. In contrast, a stocky column would have a critical buckling
stress higher than the yield, i.e. it yields in shortening prior the virtual
elastic buckling onset.

Where:
    L  e    /  r   {\displaystyle L_{e}/r}  [{\displaystyle L_{e}/r}] -
Slenderness ratio
    L  e     {\displaystyle L_{e}}  [L_{e}] - The effective length,      L  e
= K L   {\displaystyle L_{e}=KL}  [{\displaystyle L_{e}=KL}]
   r   {\displaystyle r}  [r] - Radius of gyration,     r =     I    A
{\displaystyle r={\sqrt {\operatorname {I} \! \over \operatorname {A} \!}}}  [
{\displaystyle r={\sqrt {\operatorname {I} \! \over \operatorname {A} \!}}}]
   I   {\displaystyle I}  [I] - Moment of inertia
   A   {\displaystyle A}  [A] - Area cross section
***** Mathematical derivation: Pin ended column[edit] *****
The following model applies to columns simply supported at each end (    K = 1
{\displaystyle K=1}  [K=1]).
Firstly, we will put attention to the fact there are no reactions in the hinged
ends, so we also have no shear force in any cross-section of the column. The
reason for no reactions can be obtained from symmetry (so the reactions should
be in the same direction) and from moment equilibrium (so the reactions should
be in opposite directions).
Using the free_body_diagram in the right side of figure 3, and making a
summation of moments about point A:
         &#x03A3; M = 0 &#x21D2; M ( x ) + P w = 0   {\displaystyle \Sigma
      M=0\Rightarrow M(x)+Pw=0}  [{\displaystyle \Sigma M=0\Rightarrow M
      (x)+Pw=0}]
where w is the lateral deflection.
According to EulerâBernoulli_beam_theory, the deflection of a beam is related
with its bending_moment by:
         M = &#x2212; E I           d   2   w           d   x  2
      {\displaystyle M=-EI{\cfrac {\mathrm {d} ^{2}w}{\mathrm {d} x^{2}}}}  [
      {\displaystyle M=-EI{\cfrac {\mathrm {d} ^{2}w}{\mathrm {d} x^{2}}}}],
so:
Fig. 3: Pin ended column under the effect of Buckling load
         E I     d  2   w   d  x  2      + P w = 0   {\displaystyle EI{\frac
      {d^{2}w}{dx^{2}}}+Pw=0}  [{\displaystyle EI{\frac {d^{2}w}{dx^
      {2}}}+Pw=0}]
Let      &#x03BB;  2   =   P  E I      {\displaystyle \lambda ^{2}={\frac {P}
{EI}}}  [{\displaystyle \lambda ^{2}={\frac {P}{EI}}}], so:
             d  2   w   d  x  2      +  &#x03BB;  2   w = 0   {\displaystyle
      {\frac {d^{2}w}{dx^{2}}}+\lambda ^{2}w=0}  [{\displaystyle {\frac {d^
      {2}w}{dx^{2}}}+\lambda ^{2}w=0}]
We get a classical homogeneous second-order ordinary_differential_equation.
The general solutions of this equation is:     w ( x ) = A cos &#x2061;
( &#x03BB; x ) + B sin &#x2061; ( &#x03BB; x )   {\displaystyle w(x)=A\cos
(\lambda x)+B\sin(\lambda x)}  [{\displaystyle w(x)=A\cos(\lambda x)+B\sin
(\lambda x)}], where     A   {\displaystyle A}  [A] and     B   {\displaystyle
B}  [B] are constants to be determined by boundary_conditions, which are:
    * Left end pinned     &#x2192; w ( 0 ) = 0 &#x2192; A = 0   {\displaystyle
      \rightarrow w(0)=0\rightarrow A=0}  [{\displaystyle \rightarrow w
      (0)=0\rightarrow A=0}]
    * Right end pinned     &#x2192; w ( l ) = 0 &#x2192; B sin &#x2061;
      ( &#x03BB; l ) = 0   {\displaystyle \rightarrow w(l)=0\rightarrow B\sin
      (\lambda l)=0}  [{\displaystyle \rightarrow w(l)=0\rightarrow B\sin
      (\lambda l)=0}]
Fig. 4: First three modes of buckling loads
If     B = 0   {\displaystyle B=0}  [{\displaystyle B=0}], no bending moment
exists and we get the trivial_solution of     w ( x ) = 0   {\displaystyle w
(x)=0}  [{\displaystyle w(x)=0}].
However, from the other solution     sin &#x2061; ( &#x03BB; l ) = 0
{\displaystyle \sin(\lambda l)=0}  [{\displaystyle \sin(\lambda l)=0}] we get
&#x03BB;  n   l = n &#x03C0;   {\displaystyle \lambda _{n}l=n\pi }  [
{\displaystyle \lambda _{n}l=n\pi }], for     n = 0 , 1 , 2...   {\displaystyle
n=0,1,2...}  [{\displaystyle n=0,1,2...}]
Together with      &#x03BB;  2   =   P  E I      {\displaystyle \lambda ^{2}=
{\frac {P}{EI}}}  [{\displaystyle \lambda ^{2}={\frac {P}{EI}}}] as defined
before, the various critical loads are:
          P  n   =     n  2    &#x03C0;  2   E I   l  2       {\displaystyle P_
      {n}={\frac {n^{2}\pi ^{2}EI}{l^{2}}}}  [{\displaystyle P_{n}={\frac {n^
      {2}\pi ^{2}EI}{l^{2}}}}], for     n = 0 , 1 , 2...   {\displaystyle
      n=0,1,2...}  [{\displaystyle n=0,1,2...}]
and depending upon the value of     n   {\displaystyle n}  [{\displaystyle n}],
different buckling modes are produced[3] as shown in figure 4. The load and
mode for n=0 is the nonbuckled mode.
Theoretically, any buckling mode is possible, but in the case of a slowly
applied load only the first modal shape is likely to be produced.
The critical load of Euler for a pin ended column is therefore:
          P  c r   =     &#x03C0;  2   E I   l  2       {\displaystyle P_{cr}=
      {\frac {\pi ^{2}EI}{l^{2}}}}  [{\displaystyle P_{cr}={\frac {\pi ^{2}EI}
      {l^{2}}}}]
and the obtained shape of the buckled column in the first mode is:
         w ( x ) = B sin &#x2061;   (     &#x03C0; l   x   )     {\displaystyle
      w(x)=B\sin {\Bigl (}{\pi \over l}x{\Bigr )}}  [{\displaystyle w(x)=B\sin
      {\Bigl (}{\pi  \over l}x{\Bigr )}}].
***** Mathematical derivation: General approach[edit] *****
Fig. 5: forces and moments acting on a column
The differential equation of the axis of a beam[4] is:
             d  4   w   d  x  4      +   P  E I        d  2   w   d  x  2
      =   q  E I      {\displaystyle {\frac {d^{4}w}{dx^{4}}}+{\frac {P}{EI}}
      {\frac {d^{2}w}{dx^{2}}}={\frac {q}{EI}}}  [{\displaystyle {\frac {d^
      {4}w}{dx^{4}}}+{\frac {P}{EI}}{\frac {d^{2}w}{dx^{2}}}={\frac {q}{EI}}}]
For a column with axial load only, the lateral load     q ( x )
{\displaystyle q(x)}  [q(x)] vanishes and substituting      &#x03BB;  2   =   P
E I      {\displaystyle \lambda ^{2}={\frac {P}{EI}}}  [{\displaystyle \lambda
^{2}={\frac {P}{EI}}}] , we get:
             d  4   w   d  x  4      +  &#x03BB;  2       d  2   w   d  x  2
      = 0   {\displaystyle {\frac {d^{4}w}{dx^{4}}}+\lambda ^{2}{\frac {d^{2}w}
      {dx^{2}}}=0}  [{\displaystyle {\frac {d^{4}w}{dx^{4}}}+\lambda ^{2}{\frac
      {d^{2}w}{dx^{2}}}=0}]
This is a homogeneous fourth-order differential equation and its general
solution is     w ( x ) = A sin &#x2061; ( &#x03BB; x ) + B cos &#x2061;
( &#x03BB; x ) + C x + D   {\displaystyle w(x)=A\sin(\lambda x)+B\cos(\lambda
x)+Cx+D}  [{\displaystyle w(x)=A\sin(\lambda x)+B\cos(\lambda x)+Cx+D}]
The four constants     A , B , C , D   {\displaystyle A,B,C,D}  [{\displaystyle
A,B,C,D}] are determined by the boundary conditions (end constraints) on     w
( x )   {\displaystyle w(x)}  [w(x) ], at each end. There are three cases:
   1. Pinned end:     w = 0   {\displaystyle w=0}  [{\displaystyle w=0}] and
      M = 0 &#x2192;     d  2   w   d  x  2      = 0   {\displaystyle
      M=0\rightarrow {d^{2}w \over dx^{2}}=0}  [{\displaystyle M=0\rightarrow
      {d^{2}w \over dx^{2}}=0}]
   2. Fixed end:     w = 0   {\displaystyle w=0}  [{\displaystyle w=0}] and
      d w   d x    = 0   {\displaystyle {dw \over dx}=0}  [{\displaystyle {dw
      \over dx}=0}]
   3. Free end:     M = 0 &#x2192;     d  2   w   d  x  2      = 0
      {\displaystyle M=0\rightarrow {d^{2}w \over dx^{2}}=0}  [{\displaystyle
      M=0\rightarrow {d^{2}w \over dx^{2}}=0}] and     V = 0 &#x2192;     d  3
      w   d  x  3      +  &#x03BB;  2      d w   d x    = 0   {\displaystyle
      V=0\rightarrow {d^{3}w \over dx^{3}}+\lambda ^{2}{dw \over dx}=0}  [
      {\displaystyle V=0\rightarrow {d^{3}w \over dx^{3}}+\lambda ^{2}{dw \over
      dx}=0}]
Using each time a different combination of these BCs, eigenvalue_problems are
obtained. Solving those, we get the values of Euler's critical load for each
one of the cases presented in Figure 1.
***** See also[edit] *****
    * Buckling
    * Bending_moment
    * Bending
    * EulerâBernoulli_beam_theory
***** References[edit] *****
   1. ^"Column_Buckling".
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
   3. ^"Questions_on_Columns_and_Struts".
   4. ^"Buckling_of_Columns" (PDF).
   5. ^Timoshenko, S. P. & Gere, J. M. (1961). Theory of Elastic Stability, 2
      ed., McGraw-Hill.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Euler%27s_critical_load&oldid=888477989"
Categories:
    * Elasticity_(physics)
    * Materials_science
    * Mechanical_failure_modes
    * Structural_analysis
    * Mechanics
    * Leonhard_Euler
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
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 19 March 2019, at 12:50 (UTC).
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
