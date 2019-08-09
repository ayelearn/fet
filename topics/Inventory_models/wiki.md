The following text has been accessed from https://en.wikipedia.org/wiki/Inventory_theory at Fri Aug 9 02:30:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Inventory theory ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Material theory (or more formally the mathematical theory of inventory and
production) is the sub-specialty within operations_research and operations
management that is concerned with the design of production/inventory systems to
minimize costs: it studies the decisions faced by firms and the military in
connection with manufacturing, warehousing, supply_chains, spare_part
allocation and so on and provides the mathematical foundation for logistics.
The inventory control problem is the problem faced by a firm that must decide
how much to order in each time period to meet demand for its products. The
problem can be modeled using mathematical techniques of optimal_control,
dynamic_programming and network_optimization. The study of such models is part
of inventory theory.
⁰
***** Contents *****
    * 1_Issues
    * 2_Inventory_models
          o 2.1_Classic_models
    * 3_See_also
    * 4_References
    * 5_Further_reading
***** Issues[edit] *****
 This section possibly contains original_research. Please improve_it by
 verifying the claims made and adding inline_citations. Statements consisting
 only of original research should be removed. (March 2016)(Learn_how_and_when
 to_remove_this_template_message)
One issue is infrequent large orders vs. frequent small orders. Large orders
will increase the amount of inventory on hand, which is costly, but may benefit
from volume discounts. Frequent orders are costly to process, and the resulting
small inventory levels may increase the probability of stockouts, leading to
loss of customers. In principle all these factors can be calculated
mathematically and the optimum found.
A second issue is related to changes in demand (predictable or random) for the
product. For example, having the needed merchandise on hand in order to make
sales during the appropriate buying season(s). A classic example is a toy_store
before Christmas: if the items are not on the shelves, they cannot be sold. And
the wholesale market is not perfect' there can be considerable delays,
particularly with the most popular toys. So, the entrepreneur or business
manager will buy speculatively. Another example is a furniture store. If there
is a six-week, or more, delay for customers to receive merchandise, some sales
will be lost. A further example is a restaurant, where a considerable
percentage of the sales are the value-added aspects of food preparation and
presentation, and so it is rational to buy and store somewhat more to reduce
the chances of running out of key ingredients. The situation often comes down
to two key questions: confidence in the merchandise selling, and the benefits
accruing if it does?
A third issue comes from the view that inventory also serves the function of
decoupling two separate operations. For example, work_in_process inventory
often accumulates between two departments because the consuming and the
producing department do not coordinate their work. With improved coordination
this buffer inventory could be eliminated. This leads to the whole philosophy
of Just_In_Time, which argues that the costs of carrying inventory have
typically been underestimated, both the direct, obvious costs of storage space
and insurance, but also the harder-to-measure costs of increased variables and
complexity, and thus decreased flexibility, for the business enterprise.
***** Inventory models[edit] *****
The mathematical approach is typically formulated as follows: a store has, at
time     k   {\displaystyle k}  [k],      x  k     {\displaystyle x_{k}}  [x_
{k}] items in stock. It then orders (and receives)      u  k     {\displaystyle
u_{k}}  [u_{k}] items, and sells      w  k     {\displaystyle w_{k}}  [w_k]
items, where     w   {\displaystyle w}  [w] follows a given probability
distribution. Thus:
          x  k + 1   =  x  k   +  u  k   &#x2212;  w  k     {\displaystyle x_
      {k+1}=x_{k}+u_{k}-w_{k}}  [{\displaystyle x_{k+1}=x_{k}+u_{k}-w_{k}}]
          u  k   &#x2265; 0   {\displaystyle u_{k}\geq 0}  [{\displaystyle u_
      {k}\geq 0}]
Whether      x  k     {\displaystyle x_{k}}  [x_{k}] is allowed to go negative,
corresponding to back-ordered items, will depend on the specific situation; if
allowed there will usually be a penalty for back orders. The store has costs
that are related to the number of items in store and the number of items
ordered:
          c  k   = c (  x  k   ,  u  k   )   {\displaystyle c_{k}=c(x_{k},u_
      {k})}  [{\displaystyle c_{k}=c(x_{k},u_{k})}]. Often this will be in
      additive form:      c  k   = p (  x  k   ) + h (  u  k   )
      {\displaystyle c_{k}=p(x_{k})+h(u_{k})}  [{\displaystyle c_{k}=p(x_{k})+h
      (u_{k})}]
The store wants to select      u  k     {\displaystyle u_{k}}  [u_{k}] in an
optimal way, i.e. to minimize
          &#x2211;  k = 0   T    c  k   .   {\displaystyle \sum _{k=0}^{T}c_
      {k}.}  [{\displaystyle \sum _{k=0}^{T}c_{k}.}]
Many other features can be added to the model, including multiple products
(denoted      x  i k     {\displaystyle x_{ik}}  [{\displaystyle x_{ik}}]),
upper bounds on inventory and so on. Inventory models can be based on different
assumptions:[1][2]
    * Nature of demand: constant, deterministically time-varying or stochastic
    * Costs: variable versus fixed
    * Flow of time: discrete versus continuous
    * Lead_time: deterministic or stochastic
    * Time_horizon: finite versus infinite (T=+â)
    * Presence or absence of back-ordering
    * Production_rate: infinite, deterministic or random
    * Presence or absence of quantity discounts
    * Imperfect quality
    * Capacity: infinite or limited
    * Products: one or many
    * Location: one or many
    * Echelons: one or many
**** Classic models[edit] ****
Although the number of models described in the literature is immense, the
following is a list of classics:
    * Infinite fill rate for the part being produced: Economic_order_quantity
      model, a.k.a. Wilson EOQ Model
    * Constant fill rate for the part being produced: Economic_production
      quantity model
    * Demand is random, only one replenishment: classical Newsvendor_model
    * Demand is random, continuous replenishment: Base_stock_model
    * Demand varies deterministically over time: Dynamic_lot_size_model or
      Wagner-Whitin model
    * Demand varies deterministically over time: SilverâMeal_heuristic
    * Several products produced on the same machine: Economic_lot_scheduling
      problem
***** See also[edit] *****
    * Safety_stock
    * Inventory_optimization
    * Inventory_management_software
    * Supply_chain_management
    * Warehouse_management_system
***** References[edit] *****
   1. ^ Zipkin Paul H., Foundations of Inventory Management, Boston: McGraw
      Hill, 2000,
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
   3. ISBN 0-256-11379-3
   4. ^ W. Hopp, M. Spearman, Factory Physics, 3rd ed. Waveland Press, 2011
***** Further reading[edit] *****
    * International Journal of Inventory Research is an academic_journal on
      inventory theory publishing current research.
Classic books that established the field are:
    * Kenneth J. Arrow, Samuel Karlin, and Herbert E. Scarf: Studies in the
      Mathematical Theory of Inventory and Production, Stanford University
      Press, 1958
    * Thomson M. Whitin, G. Hadley, Analysis of Inventory Systems, Englewood
      Cliffs: Prentice-Hall 1963
Many university courses in inventory theory use one or more of the following
current textbooks:
    * Axsaeter, Sven. Inventory Control. Norwell, MA: Kluwer, 2000.
ISBN 0-387-33250-2
Porteus, Evan L. Foundations of Stochastic Inventory Theory. Stanford, CA:
Stanford University Press, 2002.
ISBN 0-8047-4399-1
Silver, Edward A., David F. Pyke, and Rein Peterson. Inventory Management and
Production Planning and Scheduling, 3rd ed. Hoboken, NJ: Wiley, 1998.
ISBN 0-471-11947-4
Simchi-Levi, David, Xin Chen, and Julien Bramel. The Logic of Logistics:
Theory, Algorithms, and Applications for Logistics Management, 2nd ed. New
York: Springer Verlag, 2004.
ISBN 0-387-22199-9
Tempelmeier, Horst. Inventory Management in Supply Networks, 3rd. Edition,
Norderstedt (Books on Demand) 2011,
ISBN 3-8423-4677-8
Zipkin, Paul H. Foundations of Inventory Management. Boston: McGraw Hill, 2000.
ISBN 0-256-11379-3

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Inventory_theory&oldid=846789673"
Categories:
    * Inventory_optimization
Hidden categories:
    * Articles_that_may_contain_original_research_from_March_2016
    * All_articles_that_may_contain_original_research
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
    * This page was last edited on 20 June 2018, at 22:19 (UTC).
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
