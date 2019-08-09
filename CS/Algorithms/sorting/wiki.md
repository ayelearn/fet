The following text has been accessed from https://en.wikipedia.org/wiki/Sorting at Fri Aug 9 01:10:00 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Sorting ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the process. For other uses, see Sort_(disambiguation).
On Wikipedia, SORTKEY may refer to Wikipedia:SORTKEY.
Sorting type
Sorting is any process of arranging items systematically, and has two common,
yet distinct meanings:
   1. ordering: arranging items in a sequence ordered by some criterion;
   2. categorizing: grouping items with similar properties.
⁰
***** Contents *****
    * 1_Sorting_information_or_data
          o 1.1_Common_sorting_algorithms
    * 2_Physical_sorting_processes
    * 3_See_also
    * 4_External_links
***** Sorting information or data[edit] *****
In computer_science, arranging in an ordered sequence is called "sorting".
Sorting is a common operation in many applications, and efficient algorithms to
perform it have been developed.
The most common uses of sorted sequences are:
    * making lookup_or_search efficient;
    * making merging_of_sequences efficient.
    * enable processing_of_data in a defined order.
The opposite of sorting, rearranging a sequence of items in a random or
meaningless order, is called shuffling.
For sorting, either a weak order, "should not come after", can be specified, or
a strict_weak_order, "should come before" (specifying one defines also the
other, the two are the complement of the inverse of each other, see operations
on_binary_relations). For the sorting to be unique, these two are restricted to
a total_order and a strict total order, respectively.
Sorting n-tuples (depending on context also called e.g. records consisting of
fields) can be done based on one or more of its components. More generally
objects can be sorted based on a property. Such a component or property is
called a sort key.
For example, the items are books, the sort key is the title, subject or author,
and the order is alphabetical.
A new sort key can be created from two or more sort keys by lexicographical
order. The first is then called the primary sort key, the second the secondary
sort key, etc.
For example, addresses could be sorted using the city as primary sort key, and
the street as secondary sort key.
If the sort key values are totally_ordered, the sort key defines a weak_order
of the items: items with the same sort key are equivalent with respect to
sorting. See also stable_sorting. If different items have different sort key
values then this defines a unique order of the items.
Workers sorting parcels in a postal facility
A standard order is often called ascending (corresponding to the fact that the
standard order of numbers is ascending, i.e. A to Z, 0 to 9), the reverse order
descending (Z to A, 9 to 0). For dates and times, ascending means that earlier
values precede later ones e.g. 1/1/2000 will sort ahead of 1/1/2001.
**** Common sorting algorithms[edit] ****
Main article: Sorting_algorithm
    * Bubble/Shell sort : Exchange two adjacent elements if they are out of
      order. Repeat until array is sorted.
    * Insertion sort : Scan successive elements for an out-of-order item, then
      insert the item in the proper place.
    * Selection sort : Find the smallest (or biggest) element in the array, and
      put it in the proper place. Swap it with the value in the first position.
      Repeat until array is sorted.
    * Quick sort : Partition the array into two segments. In the first segment,
      all elements are less than or equal to the pivot value. In the second
      segment, all elements are greater than or equal to the pivot value.
      Finally, sort the two segments recursively.
    * Merge sort : Divide the list of elements in two parts, sort the two parts
      individually and then merge it.
***** Physical sorting processes[edit] *****
A railroad classification_yard, used for sorting freight_cars
Various sorting tasks are essential in industrial processes. For example,
during the extraction of gold from ore, a device called a shaker_table uses
gravity, vibration, and flow to separate gold from lighter materials in the ore
(sorting by size and weight). Sorting is also a naturally occurring process
that results in the concentration of ore or sediment. Sorting results from the
application of some criterion or differential stressor to a mass to separate it
into its components based on some variable quality. Materials that are
different, but only slightly so, such as the isotopes of uranium, are very
difficult to separate.
Optical_sorting is an automated process of sorting solid products using cameras
and/or lasers and has widespread use in the food industry.[citation_needed]
Sensor-based_sorting is used in mineral processing.[1]
***** See also[edit] *****
    * Help:Sorting in Wikipedia tables. For sorting of categories, see
      Wikipedia:Categorization#Sort_keys and for sorting of article sections,
      see WP:ORDER
    * Collation
    * IBM_mainframe_sort/merge
    * Unicode_collation_algorithm
***** External links[edit] *****
 Look up sort or sorting in Wiktionary, the free dictionary.
    * Demonstration_of_Sorting_Algorithms (includes bubble and quicksort)
    * Animated_video explaining bubble sort and quick sort and compares their
      performance.
 Wikimedia Commons has media related to Sorting.
   1. ^Deepak Malhotra (2009). Recent_Advances_in_Mineral_Processing_Plant
      Design. SME. ISBN 978-0-87335-316-8.
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

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Sorting&oldid=909945462"
Categories:
    * Sorting_algorithms
    * Data_processing
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_August_2019
    * Commons_category_link_from_Wikidata
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * BÃ¢n-lÃ¢m-gÃº
    * ÄeÅ¡tina
    * ChiShona
    * Deutsch
    * ÙØ§Ø±Ø³Û
    * íêµ­ì´
    * Bahasa_Indonesia
    * Nederlands
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * TÃ¼rkÃ§e
Edit_links
    * This page was last edited on 8 August 2019, at 17:04 (UTC).
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
