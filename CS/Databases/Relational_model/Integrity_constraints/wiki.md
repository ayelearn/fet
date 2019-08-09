The following text has been accessed from https://en.wikipedia.org/wiki/Data_integrity at Fri Aug 9 01:11:31 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Data integrity ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Data integrity is the maintenance of, and the assurance of the accuracy and
consistency of, data over its entire life-cycle,[1] and is a critical aspect to
the design, implementation and usage of any system which stores, processes, or
retrieves data. The term is broad in scope and may have widely different
meanings depending on the specific context – even under the same general
umbrella of computing. It is at times used as a proxy term for data_quality,[2]
while data_validation is a pre-requisite for data integrity.[3] Data integrity
is the opposite of data_corruption.[4] The overall intent of any data integrity
technique is the same: ensure data is recorded exactly as intended (such as a
database correctly rejecting mutually exclusive possibilities,) and upon later
retrieval, ensure the data is the same as it was when it was originally
recorded. In short, data integrity aims to prevent unintentional changes to
information. Data integrity is not to be confused with data_security, the
discipline of protecting data from unauthorized parties.
Any unintended changes to data as the result of a storage, retrieval or
processing operation, including malicious intent, unexpected hardware failure,
and human_error, is failure of data integrity. If the changes are the result of
unauthorized access, it may also be a failure of data security. Depending on
the data involved this could manifest itself as benign as a single pixel in an
image appearing a different color than was originally recorded, to the loss of
vacation pictures or a business-critical database, to even catastrophic loss of
human life in a life-critical_system.
⁰
***** Contents *****
    * 1_Integrity_types
          o 1.1_Physical_integrity
          o 1.2_Logical_integrity
    * 2_Databases
          o 2.1_Types_of_integrity_constraints
          o 2.2_Examples
    * 3_File_systems
    * 4_Data_integrity_as_applied_to_various_industries
    * 5_See_also
    * 6_References
    * 7_Further_reading
***** Integrity types[edit] *****
**** Physical integrity[edit] ****
Physical integrity deals with challenges associated with correctly storing and
fetching the data itself. Challenges with physical integrity may include
electromechanical faults, design flaws, material fatigue, corrosion, power
outages, natural disasters, acts of war and terrorism, and other special
environmental hazards such as ionizing radiation, extreme temperatures,
pressures and g-forces. Ensuring physical integrity includes methods such as
redundant hardware, an uninterruptible_power_supply, certain types of RAID
arrays, radiation_hardened chips, error-correcting_memory, use of a clustered
file_system, using file systems that employ block level checksums such as ZFS,
storage arrays that compute parity calculations such as exclusive_or or use a
cryptographic_hash_function and even having a watchdog_timer on critical
subsystems.
Physical integrity often makes extensive use of error detecting algorithms
known as error-correcting_codes. Human-induced data integrity errors are often
detected through the use of simpler checks and algorithms, such as the Damm
algorithm or Luhn_algorithm. These are used to maintain data integrity after
manual transcription from one computer system to another by a human
intermediary (e.g. credit card or bank routing numbers). Computer-induced
transcription errors can be detected through hash_functions.
In production systems, these techniques are used together to ensure various
degrees of data integrity. For example, a computer file_system may be
configured on a fault-tolerant RAID array, but might not provide block-level
checksums to detect and prevent silent_data_corruption. As another example, a
database management system might be compliant with the ACID properties, but the
RAID controller or hard disk drive's internal write cache might not be.
**** Logical integrity[edit] ****
See also: Mutex and Copy-on-write
This type of integrity is concerned with the correctness or rationality of a
piece of data, given a particular context. This includes topics such as
referential_integrity and entity_integrity in a relational_database or
correctly ignoring impossible sensor data in robotic systems. These concerns
involve ensuring that the data "makes sense" given its environment. Challenges
include software_bugs, design flaws, and human errors. Common methods of
ensuring logical integrity include things such as a check_constraints, foreign
key_constraints, program assertions, and other run-time sanity checks.
Both physical and logical integrity often share many common challenges such as
human errors and design flaws, and both must appropriately deal with concurrent
requests to record and retrieve data, the latter of which is entirely a subject
on its own.
***** Databases[edit] *****
Data integrity contains guidelines for data_retention, specifying or
guaranteeing the length of time data can be retained in a particular database.
To achieve data integrity, these rules are consistently and routinely applied
to all data entering the system, and any relaxation of enforcement could cause
errors in the data. Implementing checks on the data as close as possible to the
source of input (such as human data entry), causes less erroneous data to enter
the system. Strict enforcement of data integrity rules results in lower error
rates, and time saved troubleshooting and tracing erroneous data and the errors
it causes to algorithms.
Data integrity also includes rules defining the relations a piece of data can
have, to other pieces of data, such as a Customer record being allowed to link
to purchased Products, but not to unrelated data such as Corporate Assets. Data
integrity often includes checks and correction for invalid data, based on a
fixed schema or a predefined set of rules. An example being textual data
entered where a date-time value is required. Rules for data derivation are also
applicable, specifying how a data value is derived based on algorithm,
contributors and conditions. It also specifies the conditions on how the data
value could be re-derived.
**** Types of integrity constraints[edit] ****
Data integrity is normally enforced in a database_system by a series of
integrity constraints or rules. Three types of integrity constraints are an
inherent part of the relational data model: entity integrity, referential
integrity and domain integrity.
    * Entity_integrity concerns the concept of a primary_key. Entity integrity
      is an integrity rule which states that every table must have a primary
      key and that the column or columns chosen to be the primary key should be
      unique and not null.
    * Referential_integrity concerns the concept of a foreign_key. The
      referential integrity rule states that any foreign-key value can only be
      in one of two states. The usual state of affairs is that the foreign-key
      value refers to a primary key value of some table in the database.
      Occasionally, and this will depend on the rules of the data owner, a
      foreign-key value can be null. In this case, we are explicitly saying
      that either there is no relationship between the objects represented in
      the database or that this relationship is unknown.
    * Domain integrity specifies that all columns in a relational database must
      be declared upon a defined domain. The primary unit of data in the
      relational data model is the data item. Such data items are said to be
      non-decomposable or atomic. A domain is a set of values of the same type.
      Domains are therefore pools of values from which actual values appearing
      in the columns of a table are drawn.
    * User-defined integrity refers to a set of rules specified by a user,
      which do not belong to the entity, domain and referential integrity
      categories.
If a database supports these features, it is the responsibility of the database
to ensure data integrity as well as the consistency_model for the data storage
and retrieval. If a database does not support these features, it is the
responsibility of the applications to ensure data integrity while the database
supports the consistency_model for the data storage and retrieval.
Having a single, well-controlled, and well-defined data-integrity system
increases
    * stability (one centralized system performs all data integrity operations)
    * performance (all data integrity operations are performed in the same tier
      as the consistency model)
    * re-usability (all applications benefit from a single centralized data
      integrity system)
    * maintainability (one centralized system for all data integrity
      administration).
Modern databases support these features (see Comparison_of_relational_database
management_systems), and it has become the de facto responsibility of the
database to ensure data integrity. Companies, and indeed many database systems,
offer products and services to migrate legacy systems to modern databases.
**** Examples[edit] ****
An example of a data-integrity mechanism is the parent-and-child relationship
of related records. If a parent record owns one or more related child records
all of the referential integrity processes are handled by the database itself,
which automatically ensures the accuracy and integrity of the data so that no
child record can exist without a parent (also called being orphaned) and that
no parent loses their child records. It also ensures that no parent record can
be deleted while the parent record owns any child records. All of this is
handled at the database level and does not require coding integrity checks into
each application.
***** File systems[edit] *****
Various research results show that neither widespread filesystems (including
UFS, Ext, XFS, JFS and NTFS) nor hardware_RAID solutions provide sufficient
protection against data integrity problems.[5][6][7][8][9]
Some filesystems (including Btrfs and ZFS) provide internal data and metadata
checksumming that is used for detecting silent_data_corruption and improving
data integrity. If a corruption is detected that way and internal RAID
mechanisms provided by those filesystems are also used, such filesystems can
additionally reconstruct corrupted data in a transparent way.[10] This approach
allows improved data integrity protection covering the entire data paths, which
is usually known as end-to-end_data_protection.[11]
***** Data integrity as applied to various industries[edit] *****
    * The U.S. Food_and_Drug_Administration has created draft guidance on data
      integrity for the pharmaceutical manufacturers required to adhere to U.S.
      Code of Federal Regulations 21 CFR Parts 210â212.[12] Outside the U.S.,
      similar data integrity guidance has been issued by the United Kingdom
      (2015), Switzerland (2016), and Australia (2017).[13]
    * Various standards for the manufacture of medical devices address data
      integrity either directly or indirectly, including ISO_13485, ISO_14155,
      and ISO 5840.[14]
    * Consumer healthcare companies producing over-the-counter therapies must
      also put safeguards in place to manage data_integrity. In addition to
      compliance with FDA regulations, there is a significant risk to brand and
      reputation.[15]
    * In early 2017, the Financial Industry Regulatory Authority (FINRA),
      noting data integrity problems with automated trading and money movement
      surveillance systems, stated it would make "the development of a data
      integrity program to monitor the accuracy of the submitted data" a
      priority.[16] In early 2018, FINRA said it would expand its approach on
      data integrity to firms' "technology change management policies and
      procedures" and Treasury securities reviews.[17]
    * Other sectors such as mining[18] and product manufacturing[19] are
      increasingly focusing on the importance of data integrity in associated
      automation and production monitoring assets.
    * Cloud storage providers have long faced significant challenges ensuring
      the integrity or provenance of customer data and tracking violations.[20]
      [21][22]
***** See also[edit] *****
    * End-to-end_data_integrity
    * Message_authentication
    * National_Information_Systems_Security_Glossary
    * Single_version_of_the_truth
***** References[edit] *****
   1. ^Boritz, J. "IS_Practitioners'_Views_on_Core_Concepts_of_Information
      Integrity". International Journal of Accounting Information Systems.
      Elsevier. Archived from the_original on 5 October 2011. Retrieved 12
      August 2011.
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
   3. ^ What_is_Data_Integrity?_Learn_How_to_Ensure_Database_Data_Integrity_via
      Checks,_Tests,_&_Best_Practices
   4. ^ What_is_Data_Integrity?_Data_Protection_101
   5. ^ From_the_book:_Uberveillance_and_the_Social_Implications_of_Microchip
      Implants:_Emerging_Page_40
   6. ^ Vijayan Prabhakaran (2006). "IRON_FILE_SYSTEMS" (PDF). Doctor of
      Philosophy in Computer Sciences. University of Wisconsin-Madison.
      Retrieved 9 June 2012.
   7. ^ "Parity_Lost_and_Parity_Regained".
   8. ^ "An_Analysis_of_Data_Corruption_in_the_Storage_Stack" (PDF).
   9. ^ "Impact_of_Disk_Corruption_on_Open-Source_DBMS" (PDF).
  10. ^ "Baarf.com". Baarf.com. Retrieved November 4, 2011.
  11. ^Bierman, Margaret; Grimmer, Lenz (August 2012). "How_I_Use_the_Advanced
      Capabilities_of_Btrfs". Retrieved 2014-01-02.
  12. ^Yupu Zhang; Abhishek Rajimwale; Andrea C. Arpaci-Dusseau; Remzi H.
      Arpaci-Dusseau. "End-to-end_Data_Integrity_for_File_Systems:_A_ZFS_Case
      Study" (PDF). Computer Sciences Department, University of Wisconsin.
      Retrieved 2014-01-02.
  13. ^"Data_Integrity_and_Compliance_with_CGMP:_Guidance_for_Industry" (PDF).
      U.S. Food and Drug Administration. April 2016. Retrieved 20 January 2018.
  14. ^Davidson, J. (18 July 2017). "Data_Integrity_Guidance_Around_the_World".
      Contract Pharma. Rodman Media. Retrieved 20 January 2018.
  15. ^Scannel, P. (12 May 2015). "Data_Integrity:_A_perspective_from_the
      medical_device_regulatory_and_standards_framework" (PDF). Data Integrity
      Seminar. Parenteral Drug Association. pp. 10â57. Retrieved 20 January
      2018.
  16. ^"New_Risks_of_Data_Integrity_in_Consumer_Healthcare_|_Clarkston
      Consulting". Clarkston Consulting. 2018-09-10. Retrieved 2018-09-11.
  17. ^Cook, R. (4 January 2017). "2017_Regulatory_and_Examination_Priorities
      Letter". Financial Industry Regulatory Authority. Retrieved 20 January
      2018.
  18. ^Cook, R. (8 January 2018). "2018_Regulatory_and_Examination_Priorities
      Letter". Financial Industry Regulatory Authority. Retrieved 20 January
      2018.
  19. ^"Data_Integrity:_Enabling_Effective_Decisions_in_Mining_Operations"
      (PDF). Accenture. 2016. Retrieved 20 January 2018.
  20. ^"Industry_4.0_and_Cyber-Physical_Systems_Raise_the_Data_Integrity
      Imperative". Nymi Blog. Nymi, Inc. 24 October 2017. Retrieved 20 January
      2018.
  21. ^Priyadharshini, B.; Parvathi, P. (2012). "Data integrity in cloud
      storage". Proceedings from the 2012 International Conference on Advances
      in Engineering, Science and Management. ISBN 9788190904223.
  22. ^Zafar, F.; Khan, A.; Malik, S.U.R.; et al. (2017). "A survey of cloud
      computing data integrity schemes: Design challenges, taxonomy and future
      trends". Computers & Security. 65 (3): 29â49. doi:10.1016/
      j.cose.2016.10.006.
  23. ^Imran, M.; Hlavacs, H.; Haq, I.U.I.; et al. (2017). "Provenance_based
      data_integrity_checking_and_verification_in_cloud_environments". PLOS
      One. 12 (5): e0177576. doi:10.1371/journal.pone.0177576. PMC 5435237.
      PMID 28545151.
***** Further reading[edit] *****
    *  This article incorporates public_domain_material from the General
      Services_Administration document "Federal_Standard_1037C" (in support of
      MIL-STD-188).
    * Xiaoyun Wang; Hongbo Yu (2005). "How_to_Break_MD5_and_Other_Hash
      Functions" (PDF). EUROCRYPT. ISBN 3-540-25910-4. Archived from the
      original (PDF) on 2009-05-21. Retrieved 2009-05-10.
Authority_control [Edit_this_at_Wikidata]     * GND: 4214306-8
    * v
    * t
    * e
Data
    * Analysis
    * Archaeology
    * Cleansing
    * Collection
    * Compression
    * Corruption
    * Curation
    * Degradation
    * Editing
    * Farming
    * Format_management
    * Fusion
    * Integration
    * Integrity
    * Library
    * Loss
    * Management
    * Migration
    * Mining
    * Pre-processing
    * Preservation
    * Protection_(privacy)
    * Recovery
    * Reduction
    * Retention
    * Quality
    * Science
    * Scraping
    * Scrubbing
    * Security
    * Stewardship
    * Storage
    * Validation
    * Warehouse
    * Wrangling/munging

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Data_integrity&oldid=908854062"
Categories:
    * Data_quality
    * Transaction_processing
Hidden categories:
    * Wikipedia_articles_incorporating_text_from_the_Federal_Standard_1037C
    * Wikipedia_articles_incorporating_text_from_MIL-STD-188
    * Wikipedia_articles_with_GND_identifiers
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
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Hrvatski
    * Italiano
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Suomi
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 1 August 2019, at 12:47 (UTC).
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
