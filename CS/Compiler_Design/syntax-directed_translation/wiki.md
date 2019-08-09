The following text has been accessed from https://en.wikipedia.org/wiki/Syntax-directed_translation at Fri Aug 9 01:12:25 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Syntax-directed translation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Syntax-directed translation refers to a method of compiler implementation where
the source language translation is completely driven by the parser.
A common method of syntax-directed translation is translating a string into a
sequence of actions by attaching one such action to each rule of a grammar.[1]
Thus, parsing a string of the grammar produces a sequence of rule applications.
SDT provides a simple way to attach semantics to any such syntax.
⁰
***** Contents *****
    * 1_Overview
    * 2_Metacompilers
    * 3_See_also
    * 4_References
***** Overview[edit] *****
Syntax-directed translation fundamentally works by adding actions to the
productions in a context-free_grammar, resulting in a Syntax-Directed
Definition (SDD).[2] Actions are steps or procedures that will be carried out
when that production is used in a derivation. A grammar specification embedded
with actions to be performed is called a syntax-directed translation scheme[1]
(sometimes simply called a 'translation scheme'.)
Each symbol in the grammar can have an attribute, which is a value that is to
be associated with the symbol. Common attributes could include a variable type,
the value of an expression, etc. Given a symbol X, with an attribute t, that
attribute is referred to as X.t
Thus, given actions and attributes, the grammar can be used for translating
strings from its language by applying the actions and carrying information
through each symbol's attribute.
***** Metacompilers[edit] *****
Early metacompilers use the terms syntax-driven and syntax-directed translation
in their descriptions. They have metaprogramming language features for
outputing code.
See metacompiler, META_II, and TREE-META.
***** See also[edit] *****
    * Attribute_grammar
***** References[edit] *****
   1. ^ a bGurari, Eitan M. "Syntax-Directed_Translation_Schemes_(SDTS's)".
      Archived from the_original on 28 July 2012.
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
   3. ^ Aho, Alfred V. Compilers:_Principles,_Techniques,_&_Tools. Boston:
      Pearson/Addison Wesley, 2007.

Retrieved from "https://en.wikipedia.org/w/index.php?title=Syntax-
directed_translation&oldid=863676621"
Categories:
    * Compiler_construction
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
    * Norsk
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * ä¸­æ
Edit_links
    * This page was last edited on 12 October 2018, at 08:30 (UTC).
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
