The following text has been accessed from https://en.wikipedia.org/wiki/State-transition_matrix at Thu Aug 8 22:54:26 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** State-transition matrix ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article has multiple issues. Please help improve_it or discuss these
 issues on the talk_page. (Learn_how_and_when_to_remove_these_template
 messages)
  This article may be too technical for most readers to understand. Please help
  improve_it to make_it_understandable_to_non-experts, without removing the
  technical details. (December 2018)(Learn_how_and_when_to_remove_this_template
  message)
  It has been suggested that this article be merged with Stochastic_matrix.
  (Discuss)Proposed since December 2018.
 (Learn_how_and_when_to_remove_this_template_message)
In control_theory, the state-transition matrix is a matrix whose product with
the state vector     x   {\displaystyle x}  [x] at an initial time      t  0
{\displaystyle t_{0}}  [t_{0}] gives     x   {\displaystyle x}  [x] at a later
time     t   {\displaystyle t}  [t]. The state-transition matrix can be used to
obtain the general solution of linear dynamical systems.
⁰
***** Contents *****
    * 1_Linear_systems_solutions
    * 2_Peano-Baker_series
    * 3_Other_properties
    * 4_See_also
    * 5_References
    * 6_Further_reading
***** Linear systems solutions[edit] *****
The state-transition matrix is used to find the solution to a general state-
space_representation of a linear_system in the following form
             x  &#x02D9;    ( t ) =  A  ( t )  x  ( t ) +  B  ( t )  u  ( t ) ,
      x  (  t  0   ) =   x   0     {\displaystyle {\dot {\mathbf {x} }}
      (t)=\mathbf {A} (t)\mathbf {x} (t)+\mathbf {B} (t)\mathbf {u}
      (t),\;\mathbf {x} (t_{0})=\mathbf {x} _{0}}  [{\displaystyle {\dot
      {\mathbf {x} }}(t)=\mathbf {A} (t)\mathbf {x} (t)+\mathbf {B} (t)\mathbf
      {u} (t),\;\mathbf {x} (t_{0})=\mathbf {x} _{0}}],
where      x  ( t )   {\displaystyle \mathbf {x} (t)}  [\mathbf {x} (t)] are
the states of the system,      u  ( t )   {\displaystyle \mathbf {u} (t)}  [
{\mathbf  {u}}(t)] is the input signal, and       x   0     {\displaystyle
\mathbf {x} _{0}}  [\mathbf {x} _{0}] is the initial condition at      t  0
{\displaystyle t_{0}}  [t_{0}]. Using the state-transition matrix      &#x03A6;
( t , &#x03C4; )   {\displaystyle \mathbf {\Phi } (t,\tau )}  [{\mathbf  {\Phi
}}(t,\tau )], the solution is given by:[1][2]
          x  ( t ) =  &#x03A6;  ( t ,  t  0   )  x  (  t  0   ) +  &#x222B;   t
      0     t    &#x03A6;  ( t , &#x03C4; )  B  ( &#x03C4; )  u  ( &#x03C4; ) d
      &#x03C4;   {\displaystyle \mathbf {x} (t)=\mathbf {\Phi } (t,t_
      {0})\mathbf {x} (t_{0})+\int _{t_{0}}^{t}\mathbf {\Phi } (t,\tau )\mathbf
      {B} (\tau )\mathbf {u} (\tau )d\tau }  [{\mathbf  {x}}(t)={\mathbf  {\Phi
      }}(t,t_{0}){\mathbf  {x}}(t_{0})+\int _{{t_{0}}}^{t}{\mathbf  {\Phi }}
      (t,\tau ){\mathbf  {B}}(\tau ){\mathbf  {u}}(\tau )d\tau ]
The first term is known as the zero-input response and the second term is known
as the zero-state response.
***** Peano-Baker series[edit] *****
The most general transition matrix is given by the Peano-Baker series
          &#x03A6;  ( t , &#x03C4; ) =  I  +  &#x222B;  &#x03C4;   t    A
      (  &#x03C3;  1   )  d  &#x03C3;  1   +  &#x222B;  &#x03C4;   t    A
      (  &#x03C3;  1   )  &#x222B;  &#x03C4;    &#x03C3;  1      A  (  &#x03C3;
      2   )  d  &#x03C3;  2    d  &#x03C3;  1   +  &#x222B;  &#x03C4;   t    A
      (  &#x03C3;  1   )  &#x222B;  &#x03C4;    &#x03C3;  1      A  (  &#x03C3;
      2   )  &#x222B;  &#x03C4;    &#x03C3;  2      A  (  &#x03C3;  3   )  d
      &#x03C3;  3    d  &#x03C3;  2    d  &#x03C3;  1   + . . .
      {\displaystyle \mathbf {\Phi } (t,\tau )=\mathbf {I} +\int _{\tau }^
      {t}\mathbf {A} (\sigma _{1})\,d\sigma _{1}+\int _{\tau }^{t}\mathbf {A}
      (\sigma _{1})\int _{\tau }^{\sigma _{1}}\mathbf {A} (\sigma _
      {2})\,d\sigma _{2}\,d\sigma _{1}+\int _{\tau }^{t}\mathbf {A} (\sigma _
      {1})\int _{\tau }^{\sigma _{1}}\mathbf {A} (\sigma _{2})\int _{\tau }^
      {\sigma _{2}}\mathbf {A} (\sigma _{3})\,d\sigma _{3}\,d\sigma _
      {2}\,d\sigma _{1}+...}  [{\mathbf  {\Phi }}(t,\tau )={\mathbf  {I}}+\int
      _{\tau }^{t}{\mathbf  {A}}(\sigma _{1})\,d\sigma _{1}+\int _{\tau }^{t}
      {\mathbf  {A}}(\sigma _{1})\int _{\tau }^{{\sigma _{1}}}{\mathbf  {A}}
      (\sigma _{2})\,d\sigma _{2}\,d\sigma _{1}+\int _{\tau }^{t}{\mathbf  {A}}
      (\sigma _{1})\int _{\tau }^{{\sigma _{1}}}{\mathbf  {A}}(\sigma _{2})\int
      _{\tau }^{{\sigma _{2}}}{\mathbf  {A}}(\sigma _{3})\,d\sigma _
      {3}\,d\sigma _{2}\,d\sigma _{1}+...]
where      I    {\displaystyle \mathbf {I} }  [\mathbf {I} ] is the identity
matrix. This matrix converges uniformly and absolutely to a solution that
exists and is unique.[2]
***** Other properties[edit] *****
The state-transition matrix      &#x03A6;  ( t , &#x03C4; )   {\displaystyle
\mathbf {\Phi } (t,\tau )}  [{\mathbf  {\Phi }}(t,\tau )], given by
          &#x03A6;  ( t , &#x03C4; ) &#x2261;  U  ( t )   U   &#x2212; 1
      ( &#x03C4; )   {\displaystyle \mathbf {\Phi } (t,\tau )\equiv \mathbf {U}
      (t)\mathbf {U} ^{-1}(\tau )}  [{\mathbf  {\Phi }}(t,\tau )\equiv {\mathbf
      {U}}(t){\mathbf  {U}}^{{-1}}(\tau )]
where      U  ( t )   {\displaystyle \mathbf {U} (t)}  [{\mathbf  {U}}(t)] is
the fundamental_solution_matrix that satisfies
             U  &#x02D9;    ( t ) =  A  ( t )  U  ( t )   {\displaystyle {\dot
      {\mathbf {U} }}(t)=\mathbf {A} (t)\mathbf {U} (t)}  [{\dot  {{\mathbf
      {U}}}}(t)={\mathbf  {A}}(t){\mathbf  {U}}(t)]
is a     n &#x00D7; n   {\displaystyle n\times n}  [n\times n] matrix that is a
linear mapping onto itself, i.e., with      u  ( t ) = 0   {\displaystyle
\mathbf {u} (t)=0}  [{\mathbf  {u}}(t)=0], given the state      x  ( &#x03C4; )
{\displaystyle \mathbf {x} (\tau )}  [\mathbf{x}(\tau)] at any time
&#x03C4;   {\displaystyle \tau }  [\tau ], the state at any other time     t
{\displaystyle t}  [t] is given by the mapping
          x  ( t ) =  &#x03A6;  ( t , &#x03C4; )  x  ( &#x03C4; )
      {\displaystyle \mathbf {x} (t)=\mathbf {\Phi } (t,\tau )\mathbf {x} (\tau
      )}  [{\mathbf  {x}}(t)={\mathbf  {\Phi }}(t,\tau ){\mathbf  {x}}(\tau )]
The state transition matrix must always satisfy the following relationships:
            &#x2202;  &#x03A6;  ( t ,  t  0   )   &#x2202; t    =  A  ( t )
      &#x03A6;  ( t ,  t  0   )   {\displaystyle {\frac {\partial \mathbf {\Phi
      } (t,t_{0})}{\partial t}}=\mathbf {A} (t)\mathbf {\Phi } (t,t_{0})}  [
      {\frac  {\partial {\mathbf  {\Phi }}(t,t_{0})}{\partial t}}={\mathbf
      {A}}(t){\mathbf  {\Phi }}(t,t_{0})] and
          &#x03A6;  ( &#x03C4; , &#x03C4; ) = I   {\displaystyle \mathbf {\Phi
      } (\tau ,\tau )=I}  [{\mathbf  {\Phi }}(\tau ,\tau )=I] for all
      &#x03C4;   {\displaystyle \tau }  [\tau ] and where     I
      {\displaystyle I}  [I] is the identity matrix.[3]
And      &#x03A6;    {\displaystyle \mathbf {\Phi } }  [{\mathbf  {\Phi }}]
also must have the following properties:
             &#x03A6;  (  t  2   ,  t  1   )  &#x03A6;  (  t  1   ,  t  0   ) =
         &#x03A6;  (  t  2   ,  t  0   )   {\displaystyle \mathbf {\Phi } (t_
      1. {2},t_{1})\mathbf {\Phi } (t_{1},t_{0})=\mathbf {\Phi } (t_{2},t_{0})}
         [{\displaystyle \mathbf {\Phi } (t_{2},t_{1})\mathbf {\Phi } (t_{1},t_
         {0})=\mathbf {\Phi } (t_{2},t_{0})}]
              &#x03A6;   &#x2212; 1   ( t , &#x03C4; ) =  &#x03A6;  ( &#x03C4;
      2. , t )   {\displaystyle \mathbf {\Phi } ^{-1}(t,\tau )=\mathbf {\Phi }
         (\tau ,t)}  [{\displaystyle \mathbf {\Phi } ^{-1}(t,\tau )=\mathbf
         {\Phi } (\tau ,t)}]
              &#x03A6;   &#x2212; 1   ( t , &#x03C4; )  &#x03A6;  ( t ,
      3. &#x03C4; ) = I   {\displaystyle \mathbf {\Phi } ^{-1}(t,\tau )\mathbf
         {\Phi } (t,\tau )=I}  [{\displaystyle \mathbf {\Phi } ^{-1}(t,\tau
         )\mathbf {\Phi } (t,\tau )=I}]
               d  &#x03A6;  ( t ,  t  0   )   d t    =  A  ( t )  &#x03A6;  ( t
         ,  t  0   )   {\displaystyle {\frac {d\mathbf {\Phi } (t,t_{0})}
      4. {dt}}=\mathbf {A} (t)\mathbf {\Phi } (t,t_{0})}  [{\displaystyle
         {\frac {d\mathbf {\Phi } (t,t_{0})}{dt}}=\mathbf {A} (t)\mathbf {\Phi
         } (t,t_{0})}]
If the system is time-invariant, we can define      &#x03A6;    {\displaystyle
\mathbf {\Phi } }  [{\mathbf  {\Phi }}]; as:
          &#x03A6;  ( t ,  t  0   ) =  e   A  ( t &#x2212;  t  0   )
      {\displaystyle \mathbf {\Phi } (t,t_{0})=e^{\mathbf {A} (t-t_{0})}}  [
      {\mathbf  {\Phi }}(t,t_{0})=e^{{{\mathbf  {A}}(t-t_{0})}}]
In the time-variant case, there are many different functions that may satisfy
these requirements, and the solution is dependent on the structure of the
system. The state-transition matrix must be determined before analysis on the
time-varying solution can continue.
***** See also[edit] *****
    * Magnus_expansion
***** References[edit] *****
   1. ^Baake, Michael; Schlaegel, Ulrike (2011). "The Peano Baker Series".
      Proceedings of the Steklov Institute of Mathematics. 275: 155â159.
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
   3. ^ a bRugh, Wilson (1996). Linear System Theory. Upper Saddle River, NJ:
      Prentice Hall. ISBN 0-13-441205-2.
   4. ^Brockett, Roger W. (1970). Finite Dimensional Linear Systems. John Wiley
      & Sons. ISBN 978-0-471-10585-5.
***** Further reading[edit] *****
    * Baake, M.; Schlaegel, U. (2011). "The Peano Baker Series". Proceedings of
      the Steklov Institute of Mathematics. 275: 155â159.
Brogan, W.L. (1991). Modern Control Theory. Prentice Hall. ISBN 0-13-589763-7.
 Wikibooks has a book on the topic of: Control_Systems/Time_Variant_System
 Solutions

Retrieved from "https://en.wikipedia.org/w/index.php?title=State-
transition_matrix&oldid=908470876"
Categories:
    * Classical_control_theory
Hidden categories:
    * Wikipedia_articles_that_are_too_technical_from_December_2018
    * All_articles_that_are_too_technical
    * Articles_needing_expert_attention_from_December_2018
    * All_articles_needing_expert_attention
    * Articles_to_be_merged_from_December_2018
    * All_articles_to_be_merged
    * Articles_with_multiple_maintenance_issues
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
    * Polski
    * ä¸­æ
Edit_links
    * This page was last edited on 29 July 2019, at 23:01 (UTC).
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
