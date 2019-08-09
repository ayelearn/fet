The following text has been accessed from https://en.wikipedia.org/wiki/Accuracy_and_precision at Thu Aug 8 23:40:55 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Accuracy and precision ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Precision is a description of random_errors, a measure of statistical
variability.
Accuracy has two definitions:
   1. More commonly, it is a description of systematic_errors, a measure of
      statistical_bias; low accuracy causes a difference between a result and a
      "true" value. ISO calls this trueness.
   2. Alternatively, ISO defines accuracy as describing a combination of both
      types of observational_error above (random and systematic), so high
      accuracy requires both high precision and high trueness.
In simplest terms, given a set of data points from repeated measurements of the
same quantity, the set can be said to be precise if the values are close to
each other, while the set can be said to be accurate if their average is close
to the true value of the quantity being measured. In the first, more common
definition above, the two concepts are independent of each other, so a
particular set of data can be said to be either accurate, or precise, or both,
or neither.
⁰
***** Contents *****
    * 1_Common_technical_definition
          o 1.1_Quantification
    * 2_ISO_definition_(ISO_5725)
    * 3_In_binary_classification
    * 4_In_psychometrics_and_psychophysics
    * 5_In_logic_simulation
    * 6_In_information_systems
    * 7_See_also
    * 8_References
    * 9_External_links
***** Common technical definition[edit] *****
Accuracy is the proximity of measurement results to the true value; precision
is the degree to which repeated (or reproducible) measurements under unchanged
conditions show the same results.
In the fields of science and engineering, the accuracy of a measurement system
is the degree of closeness of measurements of a quantity to that quantity's
true value.[1] The precision of a measurement system, related to
reproducibility and repeatability, is the degree to which repeated measurements
under unchanged conditions show the same results.[1][2] Although the two words
precision and accuracy can be synonymous in colloquial use, they are
deliberately contrasted in the context of the scientific_method.
The field of statistics, where the interpretation of measurements plays a
central role, prefers to use the terms bias and variability instead of accuracy
and precision: bias is the amount of inaccuracy and variability is the amount
of imprecision.
A measurement system can be accurate but not precise, precise but not accurate,
neither, or both. For example, if an experiment contains a systematic_error,
then increasing the sample_size generally increases precision but does not
improve accuracy. The result would be a consistent yet inaccurate string of
results from the flawed experiment. Eliminating the systematic error improves
accuracy but does not change precision.
A measurement system is considered valid if it is both accurate and precise.
Related terms include bias (non-random or directed effects caused by a factor
or factors unrelated to the independent_variable) and error (random
variability).
The terminology is also applied to indirect measurementsâthat is, values
obtained by a computational procedure from observed data.
In addition to accuracy and precision, measurements may also have a measurement
resolution, which is the smallest change in the underlying physical quantity
that produces a response in the measurement.
In numerical_analysis, accuracy is also the nearness of a calculation to the
true value; while precision is the resolution of the representation, typically
defined by the number of decimal or binary digits.
In military terms, accuracy refers primarily to the accuracy of fire (or
"justesse de tir"), the precision of fire expressed by the closeness of a
grouping of shots at and around the centre of the target.[3]
**** Quantification[edit] ****
See also: False_precision
In industrial instrumentation, accuracy is the measurement tolerance, or
transmission of the instrument and defines the limits of the errors made when
the instrument is used in normal operating conditions.[4]
Ideally a measurement device is both accurate and precise, with measurements
all close to and tightly clustered around the true value. The accuracy and
precision of a measurement process is usually established by repeatedly
measuring some traceable reference standard. Such standards are defined in the
International_System_of_Units (abbreviated SI from French: SystÃ¨me
international d'unitÃ©s) and maintained by national standards_organizations
such as the National_Institute_of_Standards_and_Technology in the United
States.
This also applies when measurements are repeated and averaged. In that case,
the term standard_error is properly applied: the precision of the average is
equal to the known standard deviation of the process divided by the square root
of the number of measurements averaged. Further, the central_limit_theorem
shows that the probability_distribution of the averaged measurements will be
closer to a normal distribution than that of individual measurements.
With regard to accuracy we can distinguish:
    * the difference between the mean of the measurements and the reference
      value, the bias. Establishing and correcting for bias is necessary for
      calibration.
    * the combined effect of that and precision.
A common convention in science and engineering is to express accuracy and/or
precision implicitly by means of significant_figures. Here, when not explicitly
stated, the margin of error is understood to be one-half the value of the last
significant place. For instance, a recording of 843.6 m, or 843.0 m, or 800.0 m
would imply a margin of 0.05 m (the last significant place is the tenths
place), while a recording of 8436 m would imply a margin of error of 0.5 m (the
last significant digits are the units).
A reading of 8,000 m, with trailing zeroes and no decimal point, is ambiguous;
the trailing zeroes may or may not be intended as significant figures. To avoid
this ambiguity, the number could be represented in scientific notation:
8.0 × 103 m indicates that the first zero is significant (hence a margin of
50 m) while 8.000 × 103 m indicates that all three zeroes are significant,
giving a margin of 0.5 m. Similarly, it is possible to use a multiple of the
basic measurement unit: 8.0 km is equivalent to 8.0 × 103 m. In fact, it
indicates a margin of 0.05 km (50 m). However, reliance on this convention can
lead to false_precision errors when accepting data from sources that do not
obey it. For example, a source reporting a number like 153,753 with precision
+/- 5,000 looks like it has precision +/- 0.5. Under the convention it would
have been rounded to 154,000.
Precision includes:
    * repeatability — the variation arising when all efforts are made to keep
      conditions constant by using the same instrument and operator, and
      repeating during a short time period; and
    * reproducibility — the variation arising using the same measurement
      process among different instruments and operators, and over longer time
      periods.
***** ISO definition (ISO 5725)[edit] *****
According to ISO 5725-1, Accuracy consists of trueness (proximity of
measurement results to the true value) and precision (repeatability or
reproducibility of the measurement)
A shift in the meaning of these terms appeared with the publication of the ISO
5725 series of standards in 1994, which is also reflected in the 2008 issue of
the "BIPM International Vocabulary of Metrology" (VIM), items 2.13 and 2.14.[1]
According to ISO 5725-1,[5] the general term "accuracy" is used to describe the
closeness of a measurement to the true value. When the term is applied to sets
of measurements of the same measurand, it involves a component of random error
and a component of systematic error. In this case trueness is the closeness of
the mean of a set of measurement results to the actual (true) value and
precision is the closeness of agreement among a set of results.
ISO 5725-1 and VIM also avoid the use of the term "bias", previously specified
in BS 5497-1,[6] because it has different connotations outside the fields of
science and engineering, as in medicine and law.
Accuracy of a target_grouping according to BIPM and ISO 5725
    * Low accuracy due to poor precision
    * Low accuracy due to poor trueness
***** In binary classification[edit] *****
Main article: Evaluation_of_binary_classifiers
Accuracy is also used as a statistical measure of how well a binary
classification test correctly identifies or excludes a condition. That is, the
accuracy is the proportion of true results (both true_positives and true
negatives) among the total number of cases examined.[7] To make the context
clear by the semantics, it is often referred to as the "Rand accuracy" or "Rand
index".[8][9][10] It is a parameter of the test. The formula for quantifying
binary accuracy is:
Accuracy = (TP+TN)/(TP+TN+FP+FN)
where: TP = True positive; FP = False positive; TN = True negative; FN = False
negative
The formula for quantifying binary precision is: Precision = (TP) / (TP+FP)
***** In psychometrics and psychophysics[edit] *****
In psychometrics and psychophysics, the term accuracy is interchangeably used
with validity and constant error. Precision is a synonym for reliability and
variable error. The validity of a measurement instrument or psychological test
is established through experiment or correlation with behavior. Reliability is
established with a variety of statistical techniques, classically through an
internal consistency test like Cronbach's_alpha to ensure sets of related
questions have related responses, and then comparison of those related question
between reference and target population.[citation_needed]
***** In logic simulation[edit] *****
In logic_simulation, a common mistake in evaluation of accurate models is to
compare a logic_simulation_model to a transistor circuit_simulation_model. This
is a comparison of differences in precision, not accuracy. Precision is
measured with respect to detail and accuracy is measured with respect to
reality.[11][12]
***** In information systems[edit] *****
Information retrieval systems, such as databases and web_search_engines, are
evaluated by many_different_metrics, some of which are derived from the
confusion_matrix, which divides results into true positives (documents
correctly retrieved), true negatives (documents correctly not retrieved), false
positives (documents incorrectly retrieved), and false negatives (documents
incorrectly not retrieved). Commonly used metrics include the notions of
precision_and_recall. In this context, precision is defined as the fraction of
retrieved documents which are relevant to the query (true positives divided by
true+false positives), using a set of ground_truth relevant results selected by
humans. Recall is defined as the fraction of relevant documents retrieved
compared to the total number of relevant documents (true positives divided by
true positives+false negatives). Less commonly, the metric of accuracy is used,
is defined as the total number of correct classifications (true positives plus
true negatives) divided by the total number of documents.
None of these metrics take into account the ranking of results. Ranking is very
important for web search engines because readers seldom go past the first page
of results, and there are too many documents on the web to manually classify
all of them as to whether they should be included or excluded from a given
search. Adding a cutoff at a particular number of results takes ranking into
account to some degree. The measure precision_at_k, for example, is a measure
of precision looking only at the top ten (k=10) search results. More
sophisticated metrics, such as discounted_cumulative_gain, take into account
each individual ranking, and are more commonly used where this is important.
***** See also[edit] *****
    * Bias-variance_tradeoff in statistics and machine learning
    * Accepted_and_experimental_value
    * Data_quality
    * Engineering_tolerance
    * Exactness
    * Experimental_uncertainty_analysis
    * F-score
    * Information_quality
    * Measurement_uncertainty
    * Precision_(statistics)
    * Probability
    * Random_and_systematic_errors
    * Sensitivity_and_specificity
    * Significant_figures
    * Statistical_significance
***** References[edit] *****
   1. ^ a b c JCGM_200:2008_International_vocabulary_of_metrology â Basic and
      general concepts and associated terms (VIM)
   2. ^Taylor, John Robert (1999). An_Introduction_to_Error_Analysis:_The_Study
      of_Uncertainties_in_Physical_Measurements. University Science Books.
      pp. 128â129. ISBN 0-935702-75-X.
   3. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   4. ^ North Atlantic Treaty Organization, Nato Standardization Agency AAP-6 -
      Glossary of terms and definitions, p 43.
   5. ^ Creus, Antonio. InstrumentaciÃ³n Industrial[citation_needed]
   6. ^ BS ISO 5725-1: "Accuracy (trueness and precision) of measurement
      methods and results - Part 1: General principles and definitions.", p.1
      (1994)
   7. ^ BS 5497-1: "Precision of test methods. Guide for the determination of
      repeatability and reproducibility for a standard test method." (1979)
   8. ^Metz, CE (October 1978). "Basic_principles_of_ROC_analysis" (PDF). Semin
      Nucl Med. 8 (4): 283â98. PMID 112681.
   9. ^"Archived_copy" (PDF). Archived from the_original (PDF) on 2015-03-11.
      Retrieved 2015-08-09.CS1 maint: Archived copy as title (link)
  10. ^Powers, David M. W (2015). "What the F-measure doesn't measure". arXiv:
      1503.06410 [cs.IR].
  11. ^David M W Powers. "The_Problem_with_Kappa" (PDF). Anthology.aclweb.org.
      Retrieved 11 December 2017.
  12. ^Acken, John M. (1997). "none". Encyclopedia of Computer Science and
      Technology. 36: 281â306.
  13. ^Glasser, Mark; Mathews, Rob; Acken, John M. (June 1990). "1990 Workshop
      on Logic-Level Modelling for ASICS". SIGDA Newsletter. 20 (1).
***** External links[edit] *****
 Look up accuracy, or precision in Wiktionary, the free dictionary.
 Wikimedia Commons has media related to Accuracy_and_precision.
    * BIPM_-_Guides_in_metrology, Guide to the Expression of Uncertainty in
      Measurement (GUM) and International Vocabulary of Metrology (VIM)
    * "Beyond_NIST_Traceability:_What_really_creates_accuracy", Controlled
      Environments magazine
    * Precision_and_Accuracy_with_Three_Psychophysical_Methods
    * Appendix_D.1:_Terminology, Guidelines for Evaluating and Expressing the
      Uncertainty of NIST Measurement Results
    * Accuracy_and_Precision
    * Accuracy_vs_Precision â a brief video by Matt Parker
    * What's_the_difference_between_accuracy_and_precision? by Matt Anticole at
      TED-Ed
    * v
    * t
    * e
ISO standards
by standard number
List of ISO_standards / ISO_romanizations / IEC_standards
                  * 1
                  * 2
                  * 3
                  * 4
                  * 5
                  * 6
                  * 7
                  * 9
                  * 16
                  * 17
                  * 31
                        o -0
                        o -1
                        o -2
                        o -3
                        o -4
                        o -5
                        o -6
                        o -7
                        o -8
                        o -9
                        o -10
                        o -11
                        o -12
                        o -13
                  * 128
                  * 216
                  * 217
                  * 226
                  * 228
                  * 233
                  * 259
                  * 269
                  * 302
                  * 306
                  * 361
                  * 428
                  * 500
                  * 518
                  * 519
                  * 639
                        o -1
                        o -2
                        o -3
                        o -5
                        o -6
                  * 646
                  * 657
                  * 668
                  * 690
                  * 704
                  * 732
                  * 764
                  * 838
                  * 843
                  * 860
                  * 898
                  * 965
                  * 999
                  * 1000
                  * 1004
                  * 1007
                  * 1073-1
                  * 1155
                  * 1413
                  * 1538
                  * 1629
                  * 1745
                  * 1989
                  * 2014
                  * 2015
                  * 2022
                  * 2033
                  * 2047
                  * 2108
                  * 2145
                  * 2146
                  * 2240
                  * 2281
                  * 2533
                  * 2709
                  * 2711
                  * 2720
                  * 2788
                  * 2848
                  * 2852
                  * 3029
                  * 3103
                  * 3166
                        o -1
                        o -2
                        o -3
                  * 3297
                  * 3307
                  * 3601
                  * 3602
                  * 3864
                  * 3901
                  * 3950
                  * 3977
                  * 4031
1â9999       * 4157
                  * 4165
                  * 4217
                  * 4909
                  * 5218
                  * 5426
                  * 5427
                  * 5428
                  * 5725
                  * 5775
                  * 5776
                  * 5800
                  * 5807
                  * 5964
                  * 6166
                  * 6344
                  * 6346
                  * 6385
                  * 6425
                  * 6429
                  * 6438
                  * 6523
                  * 6709
                  * 6943
                  * 7001
                  * 7002
                  * 7010
                  * 7027
                  * 7064
                  * 7098
                  * 7185
                  * 7200
                  * 7498
                        o -1
                  * 7637
                  * 7736
                  * 7810
                  * 7811
                  * 7812
                  * 7813
                  * 7816
                  * 7942
                  * 8000
                  * 8093
                  * 8178
                  * 8217
                  * 8373
                  * 8501-1
                  * 8571
                  * 8583
                  * 8601
                  * 8613
                  * 8632
                  * 8651
                  * 8652
                  * 8691
                  * 8805/8806
                  * 8807
                  * 8820-5
                  * 8859
                        o -1
                        o -2
                        o -3
                        o -4
                        o -5
                        o -6
                        o -7
                        o -8
                        o -8-I
                        o -9
                        o -10
                        o -11
                        o -12
                        o -13
                        o -14
                        o -15
                        o -16
                  * 8879
                  * 9000/9001
                  * 9036
                  * 9075
                  * 9126
                  * 9141
                  * 9227
                  * 9241
                  * 9293
                  * 9314
                  * 9362
                  * 9407
                  * 9506
                  * 9529
                  * 9564
                  * 9592/9593
                  * 9594
                  * 9660
                  * 9797-1
                  * 9897
                  * 9899
                  * 9945
                  * 9984
                  * 9985
                  * 9995
                  * 10005
                  * 10006
                  * 10007
                  * 10116
                  * 10118-3
                  * 10160
                  * 10161
                  * 10165
                  * 10179
                  * 10206
                  * 10218
                  * 10303
                        o -11
                        o -21
                        o -22
                        o -28
                        o -238
                  * 10383
                  * 10487
                  * 10585
                  * 10589
                  * 10646
                  * 10664
                  * 10746
                  * 10861
                  * 10957
                  * 10962
                  * 10967
                  * 11073
                  * 11170
                  * 11179
                  * 11404
                  * 11544
                  * 11783
                  * 11784
                  * 11785
                  * 11801
                  * 11898
                  * 11940 (-2)
                  * 11941
                  * 11941_(TR)
                  * 11992
                  * 12006
                  * 12182
                  * 12207
                  * 12234-2
                  * 13211
                        o -1
                        o -2
                  * 13216
                  * 13250
                  * 13399
                  * 13406-2
                  * 13450
                  * 13485
                  * 13490
                  * 13567
                  * 13568
                  * 13584
                  * 13616
                  * 14000
                  * 14031
                  * 14224
                  * 14289
                  * 14396
                  * 14443
                  * 14496
                        o -2
                        o -3
                        o -6
                        o -10
                        o -11
                        o -12
                        o -14
                        o -17
                        o -20
10000â199    * 14644
                  * 14649
                  * 14651
                  * 14698
                  * 14750
                  * 14764
                  * 14882
                  * 14971
                  * 15022
                  * 15189
                  * 15288
                  * 15291
                  * 15292
                  * 15398
                  * 15408
                  * 15444
                        o -3
                  * 15445
                  * 15438
                  * 15504
                  * 15511
                  * 15686
                  * 15693
                  * 15706
                        o -2
                  * 15707
                  * 15897
                  * 15919
                  * 15924
                  * 15926
                  * 15926_WIP
                  * 15930
                  * 16023
                  * 16262
                  * 16355-1
                  * 16612-2
                  * 16750
                  * 16949_(TS)
                  * 17024
                  * 17025
                  * 17100
                  * 17203
                  * 17369
                  * 17442
                  * 17799
                  * 18000
                  * 18004
                  * 18014
                  * 18245
                  * 18629
                  * 18916
                  * 19005
                  * 19011
                  * 19092_(-1
                  * -2)
                  * 19114
                  * 19115
                  * 19125
                  * 19136
                  * 19407
                  * 19439
                  * 19500
                  * 19501
                  * 19502
                  * 19503
                  * 19505
                  * 19506
                  * 19507
                  * 19508
                  * 19509
                  * 19510
                  * 19600
                  * 19752
                  * 19757
                  * 19770
                  * 19775-1
                  * 19794-5
                  * 19831
                  * 20000
                  * 20022
                  * 20121
                  * 20400
                  * 21000
                  * 21047
                  * 21500
                  * 21827:2002
                  * 22000
                  * 23270
                  * 23271
                  * 23360
                  * 24517
                  * 24613
                  * 24617
                  * 24707
                  * 25178
                  * 25964
                  * 26000
                  * 26262
                  * 26300
                  * 26324
                  * 27000_series
20000+            * 27000
                  * 27001
                  * 27002
                  * 27006
                  * 27729
                  * 28000
                  * 29110
                  * 29148
                  * 29199-2
                  * 29500
                  * 30170
                  * 31000
                  * 32000
                  * 37001
                  * 38500
                  * 40500
                  * 42010
                  * 45001
                  * 50001
                  * 55000
                  * 80000
                        o -1
                        o -2
                        o -3
    * [Category] Category

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Accuracy_and_precision&oldid=903429731"
Categories:
    * Accuracy_and_precision
    * Biostatistics
    * Metrology
    * Psychometrics
    * ISO_standards
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_February_2015
    * CS1_maint:_Archived_copy_as_title
    * Articles_with_unsourced_statements_from_July_2009
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
    * AzÉrbaycanca
    * BÃ¢n-lÃ¢m-gÃº
    * CatalÃ 
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Basa_Sunda
    * Suomi
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 25 June 2019, at 17:07 (UTC).
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
