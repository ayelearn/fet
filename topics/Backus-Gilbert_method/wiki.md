The following text has been accessed from https://en.wikipedia.org/wiki/Backus%E2%80%93Gilbert_method at Thu Aug 8 23:28:20 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** BackusâGilbert method ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, the BackusâGilbert method, also known as the optimally
localized average (OLA) method is named for its discoverers, geophysicists
George_E._Backus and James_Freeman_Gilbert. It is a regularization method for
obtaining meaningful solutions to ill-posed inverse_problems. Where other
regularization methods, such as the frequently used Tikhonov_regularization
method, seek to impose smoothness constraints on the solution, BackusâGilbert
instead seeks to impose stability constraints, so that the solution would vary
as little as possible if the input data were resampled multiple times. In
practice, and to the extent that is justified by the data, smoothness results
from this.
Given a data array X, the basic Backus-Gilbert inverse is:
           H   &#x03B8;   =      C   &#x2212; 1     G   &#x03B8;       G
      &#x03B8;   T     C   &#x2212; 1     G   &#x03B8;        {\displaystyle
      \mathbf {H} _{\theta }={\frac {\mathbf {C} ^{-1}\mathbf {G} _{\theta }}
      {\mathbf {G} _{\theta }^{T}\mathbf {C} ^{-1}\mathbf {G} _{\theta }}}}  [
      {\displaystyle \mathbf {H} _{\theta }={\frac {\mathbf {C} ^{-1}\mathbf
      {G} _{\theta }}{\mathbf {G} _{\theta }^{T}\mathbf {C} ^{-1}\mathbf {G} _
      {\theta }}}}]
where C is the covariance_matrix of the data, and GÎ¸ is an a priori constraint
representing the source Î¸ for which a solution is sought. Regularization is
implemented by "whitening" the covariance matrix:
           C     &#x2032;    =  C  + &#x03BB;  I    {\displaystyle \mathbf {C}
      ^{'}=\mathbf {C} +\lambda \mathbf {I} }  [{\displaystyle \mathbf {C} ^
      {'}=\mathbf {C} +\lambda \mathbf {I} }]
with Câ² replacing C in the equation for HÎ¸. Then,
           H   &#x03B8;   T    X    {\displaystyle \mathbf {H} _{\theta }^
      {T}\mathbf {X} }  [{\displaystyle \mathbf {H} _{\theta }^{T}\mathbf {X}
      }]
is an estimate of the activity of the source Î¸.
***** References[edit] *****
    * Backus, G.E., and Gilbert, F. 1968, "The Resolving power of Gross Earth
      Data", Geophysical_Journal_of_the_Royal_Astronomical_Society, vol. 16,
      pp. 169â205.
    * Backus, G.E., and Gilbert, F. 1970, "Uniqueness in the Inversion of
      inaccurate Gross Earth Data", Philosophical Transactions of the Royal
      Society of London A, vol. 266, pp. 123â192.
    * Press, WH; Teukolsky, SA; Vetterling, WT; Flannery, BP (2007). "Section
      19.6._BackusâGilbert_Method". Numerical_Recipes (3rd ed.). Cambridge
      University_Press. ISBN 978-0-521-88068-8.

            This statistics-related article is a stub. You can help Wikipedia
            by expanding_it.
[Stub_icon]     * v
                * t
                * e

Retrieved from "https://en.wikipedia.org/w/
index.php?title=BackusâGilbert_method&oldid=816775613"
Categories:
    * Inverse_problems
    * Linear_algebra
    * Statistics_stubs
Hidden categories:
    * All_stub_articles
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
Add_links
    * This page was last edited on 23 December 2017, at 16:23 (UTC).
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
