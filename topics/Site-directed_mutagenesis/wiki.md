The following text has been accessed from https://en.wikipedia.org/wiki/Site-directed_mutagenesis at Fri Aug 9 02:21:14 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Site-directed mutagenesis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Site-directed mutagenesis is a molecular_biology method that is used to make
specific and intentional changes to the DNA_sequence of a gene and any gene
products. Also called site-specific mutagenesis or oligonucleotide-directed
mutagenesis, it is used for investigating the structure and biological activity
of DNA, RNA, and protein molecules, and for protein_engineering.
Site-directed mutagenesis is one of the most important techniques in laboratory
for introducing a mutation into a DNA sequence. There are numerous methods for
achieving site-directed mutagenesis, but with decreasing costs of
oligonucleotide_synthesis, artificial_gene_synthesis is now occasionally used
as an alternative to site-directed mutagenesis. Since 2013, the development of
the CRISPR/Cas9 technology, based on a prokaryotic viral defense system, has
also allowed for the editing_of_the_genome, and mutagenesis may be performed in
vivo with relative ease.[1]
⁰
***** Contents *****
    * 1_History
    * 2_Basic_mechanism
    * 3_Approaches
          o 3.1_Kunkel's_method
          o 3.2_Cassette_mutagenesis
          o 3.3_PCR_site-directed_mutagenesis
          o 3.4_Whole_plasmid_mutagenesis
          o 3.5_In_vivo_site-directed_mutagenesis_methods
          o 3.6_CRISPR
    * 4_Applications
    * 5_Gene_synthesis
    * 6_See_also
    * 7_References
    * 8_External_links
***** History[edit] *****
Early attempts at mutagenesis using radiation or chemical mutagens were non-
site-specific, generating random mutations.[2] Analogs of nucleotides and other
chemicals were later used to generate localized point_mutations,[3] examples of
such chemicals are aminopurine,[4] nitrosoguanidine,[5] and bisulfite.[6] Site-
directed mutagenesis was achieved in 1974 in the laboratory of Charles
Weissmann using a nucleotide analogue N4-hydroxycytidine, which induces
transition of GC to AT.[7][8] These methods of mutagenesis, however, are
limited by the kind of mutation they can achieve, and they are not as specific
as later site-directed mutagenesis methods.
In 1971, Clyde_Hutchison and Marshall Edgell showed that it is possible to
produce mutants with small fragments of phage_ÏX174 and restriction_nucleases.
[9][10] Hutchison later produced with his collaborator Michael_Smith in 1978 a
more flexible approach to site-directed mutagenesis by using oligonucleotides
in a primer extension method with DNA polymerase.[11] For his part in the
development of this process, Michael Smith later shared the Nobel_Prize_in
Chemistry in October 1993 with Kary_B._Mullis, who invented polymerase_chain
reaction.
***** Basic mechanism[edit] *****
The basic procedure requires the synthesis of a short DNA primer. This
synthetic primer contains the desired mutation and is complementary to the
template DNA around the mutation site so it can hybridize with the DNA in the
gene of interest. The mutation may be a single base change (a point_mutation),
multiple base changes, deletion, or insertion. The single-strand primer is then
extended using a DNA_polymerase, which copies the rest of the gene. The gene
thus copied contains the mutated site, and is then introduced into a host cell
as a vector and cloned. Finally, mutants are selected by DNA_sequencing to
check that they contain the desired mutation.
The original method using single-primer extension was inefficient due to a low
yield of mutants. This resulting mixture contains both the original unmutated
template as well as the mutant strand, producing a mixed population of mutant
and non-mutant progenies. Furthermore, the template used is methylated while
the mutant strand is unmethylated, and the mutants may be counter-selected due
to presence of mismatch_repair system that favors the methylated template DNA,
resulting in fewer mutants. Many approaches have since been developed to
improve the efficiency of mutagenesis.
***** Approaches[edit] *****
A large number of methods are available to effect site-directed mutagenesis,
[12] although most of them are now rarely used in laboratories since the early
2000s, as newer techniques allow for simpler and easier ways of introducing
site-specific mutation into genes.
**** Kunkel's method[edit] ****
In 1985, Thomas_Kunkel introduced a technique that reduces the need to select
for the mutants.[13] The DNA fragment to be mutated is inserted into a phagemid
such as M13mp18/19 and is then transformed into an E._coli strain deficient in
two enzymes, dUTPase (dut) and uracil_deglycosidase (udg). Both enzymes are
part of a DNA_repair pathway that protects the bacterial chromosome from
mutations by the spontaneous deamination of dCTP to dUTP. The dUTPase
deficiency prevents the breakdown of dUTP, resulting in a high level of dUTP in
the cell. The uracil deglycosidase deficiency prevents the removal of uracil
from newly synthesized DNA. As the double-mutant E. coli replicates the phage
DNA, its enzymatic machinery may, therefore, misincorporate dUTP instead of
dTTP, resulting in single-strand DNA that contains some uracils (ssUDNA). The
ssUDNA is extracted from the bacteriophage that is released into the medium,
and then used as template for mutagenesis. An oligonucleotide containing the
desired mutation is used for primer extension. The heteroduplex DNA, that
forms, consists of one parental non-mutated strand containing dUTP and a
mutated strand containing dTTP. The DNA is then transformed into an E._coli
strain carrying the wildtype dut and udg genes. Here, the uracil-containing
parental DNA strand is degraded, so that nearly all of the resulting DNA
consists of the mutated strand.
**** Cassette mutagenesis[edit] ****
Unlike other methods, cassette mutagenesis need not involve primer extension
using DNA polymerase. In this method, a fragment of DNA is synthesized, and
then inserted into a plasmid.[14] It involves the cleavage by a restriction
enzyme at a site in the plasmid and subsequent ligation of a pair of
complementary oligonucleotides containing the mutation in the gene of interest
to the plasmid. Usually, the restriction enzymes that cut at the plasmid and
the oligonucleotide are the same, permitting sticky ends of the plasmid and
insert to ligate to one another. This method can generate mutants at close to
100% efficiency, but is limited by the availability of suitable restriction
sites flanking the site that is to be mutated.
**** PCR site-directed mutagenesis[edit] ****
The limitation of restriction sites in cassette mutagenesis may be overcome
using polymerase_chain_reaction with oligonucleotide "primers", such that a
larger fragment may be generated, covering two convenient restriction sites.
The exponential amplification in PCR produces a fragment containing the desired
mutation in sufficient quantity to be separated from the original, unmutated
plasmid by gel_electrophoresis, which may then be inserted in the original
context using standard recombinant molecular biology techniques. There are many
variations of the same technique. The simplest method places the mutation site
toward one of the ends of the fragment whereby one of two oligonucleotides used
for generating the fragment contains the mutation. This involves a single step
of PCR, but still has the inherent problem of requiring a suitable restriction
site near the mutation site unless a very long primer is used. Other
variations, therefore, employ three or four oligonucleotides, two of which may
be non-mutagenic oligonucleotides that cover two convenient restriction sites
and generate a fragment that can be digested and ligated into a plasmid,
whereas the mutagenic oligonucleotide may be complementary to a location within
that fragment well away from any convenient restriction site. These methods
require multiple steps of PCR so that the final fragment to be ligated can
contain the desired mutation. The design process for generating a fragment with
the desired mutation and relevant restriction sites can be cumbersome. Software
tools like SDM-Assist[15] can simplify the process.
**** Whole plasmid mutagenesis[edit] ****
For plasmid manipulations, other site-directed mutagenesis techniques have been
supplanted largely by techniques that are highly efficient but relatively
simple, easy to use, and commercially available as a kit. An example of these
techniques is the Quikchange method,[16] wherein a pair of complementary
mutagenic primers are used to amplify the entire plasmid in a thermocycling
reaction using a high-fidelity non-strand-displacing DNA polymerase such as pfu
polymerase. The reaction generates a nicked, circular DNA. The template DNA
must be eliminated by enzymatic digestion with a restriction_enzyme such as
DpnI, which is specific for methylated DNA. All DNA produced from most
Escherichia_coli strains would be methylated; the template plasmid that is
biosynthesized in E. coli will, therefore, be digested, while the mutated
plasmid, which is generated in vitro and is therefore unmethylated, would be
left undigested. Note that, in these double-strand plasmid mutagenesis methods,
while the thermocycling reaction may be used, the DNA need not be exponentially
amplified as in a PCR. Instead, the amplification is linear, and it is
therefore inaccurate to describe them as a PCR, since there is no chain
reaction.
Note that pfu polymerase can become strand-displacing at higher extension
temperature (â¥70 Â°C) which can result in the failure of the experiment,
therefore the extension reaction should be performed at the recommended
temperature of 68 Â°C. In some applications, this method has been observed to
lead to insertion of multiple copies of primers.[17] A variation of this
method, called SPRINP, prevents this artifact and has been used in different
types of site directed mutagenesis.[17]
**** In vivo site-directed mutagenesis methods[edit] ****
    * Delitto_perfetto[18]
    * Transplacement "pop-in pop-out"
    * Direct gene deletion and site-specific mutagenesis with PCR and one
      recyclable marker
    * Direct gene deletion and site-specific mutagenesis with PCR and one
      recyclable marker using long homologous regions
    * In vivo site-directed mutagenesis with synthetic oligonucleotides[19]
**** CRISPR[edit] ****
Since 2013, the development of CRISPR-Cas9 technology has allowed for the
efficient introduction of point mutations into the genome of a wide variety of
organisms. The method does not require a transposon insertion site, leaves no
marker, and its efficiency and simplicity has made it the preferred method for
genome_editing.[20][21]
***** Applications[edit] *****
Site-directed mutagenesis is used to generate mutations that may produce a
rationally_designed protein that has improved or special properties
(i.e.protein engineering).
Investigative tools â specific mutations in DNA allow the function and
properties of a DNA sequence or a protein to be investigated in a rational
approach. Furthermore, single amino-acid changes by site-directed mutagenesis
in proteins can help understand the importance of post-translational
modifications. For instance changing a particular serine (phosphoacceptor) to
an alanine (phospho-non-acceptor) in a substrate protein blocks the attachement
of a phosphate group, thereby allows the phosphorylation to be investigated.
This approach has been used to uncover the phosphorylation of the protein CBP
by the kinase HIPK2 [22]
Commercial applications â Proteins may be engineered to produce mutant forms
that are tailored for a specific application. For example, commonly used
laundry detergents may contain subtilisin, whose wild-type form has a
methionine that can be oxidized by bleach, significantly reducing the activity
the protein in the process.[23] This methionine may be replaced by alanine or
other residues, making it resistant to oxidation thereby keeping the protein
active in the presence of bleach.[24]
***** Gene synthesis[edit] *****
As the cost of DNA oligonucleotides synthesis falls, artificial_synthesis_of_a
complete_gene is now a viable method for introducing mutation into gene. This
method allows for extensive mutagenesis over multiples sites, including the
complete redesign of the codon usage of gene to optimise it for a particular
organism.[25]
***** See also[edit] *****
    * Directed_mutagenesis
***** References[edit] *****
   1. ^Hsu PD, Lander ES, Zhang F (June 2014). "Development_and_applications_of
      CRISPR-Cas9_for_genome_engineering". Cell. 157 (6): 1262â78. doi:
      10.1016/j.cell.2014.05.010. PMC 4343198. PMID 24906146.
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
   3. ^Kilbey, B. J. (1995). "Charlotte_Auerbach_(1899-1994)". Genetics. 141
      (1): 1â5. PMC 1206709. PMID 8536959.
   4. ^Shortle, D.; Dimaio, D.; Nathans, D. (1981). "Directed Mutagenesis".
      Annual Review of Genetics. 15: 265â294. doi:10.1146/
      annurev.ge.15.120181.001405. PMID 6279018.
   5. ^Caras, I. W.; MacInnes, M. A.; Persing, D. H.; Coffino, P.; Martin Jr,
      D. W. (1982). "Mechanism_of_2-aminopurine_mutagenesis_in_mouse_T-
      lymphosarcoma_cells". Molecular and Cellular Biology. 2 (9): 1096â1103.
      doi:10.1128/MCB.2.9.1096. PMC 369902. PMID 6983647.
   6. ^McHugh, G. L.; Miller, C. G. (1974). "Isolation_and_Characterization_of
      Proline_Peptidase_Mutants_of_Salmonella_typhimurium". Journal of
      Bacteriology. 120 (1): 364â371. PMC 245771. PMID 4607625.
   7. ^D Shortle & D Nathans (1978). "Local_mutagenesis:_a_method_for
      generating_viral_mutants_with_base_substitutions_in_preselected_regions
      of_the_viral_genome". Proceedings of the National Academy of Sciences. 75
      (5): 2170â2174. doi:10.1073/pnas.75.5.2170. PMC 392513. PMID 209457.
   8. ^R A Flavell; D L Sabo; E F Bandle & C Weissmann (1975). "Site-directed
      mutagenesis:_effect_of_an_extracistronic_mutation_on_the_in_vitro
      propagation_of_bacteriophage_Qbeta_RNA". Proc Natl Acad Sci U S A. 72
      (1): 367â371. doi:10.1073/pnas.72.1.367. PMC 432306. PMID 47176.
   9. ^Willi MÃ¼ller; Hans Weber; FranÃ§ois Meyer; Charles Weissmann (1978).
      "Site-directed mutagenesis in DNA: Generation of point mutations in
      cloned Î² globin complementary DNA at the positions corresponding to
      amino acids 121 to 123". Journal of Molecular Biology. 124 (2):
      343â358. doi:10.1016/0022-2836(78)90303-0. PMID 712841.
  10. ^Hutchison Ca, 3.; Edgell, M. H. (1971). "Genetic_Assay_for_Small
      Fragments_of_Bacteriophage_ÏX174_Deoxyribonucleic_Acid". Journal of
      Virology. 8 (2): 181â189. PMC 356229. PMID 4940243.
  11. ^Marshall H. Edgell, Clyde A. Hutchison, III, and Morton Sclair (1972).
      "Specific_Endonuclease_R_Fragments_of_Bacteriophage_X174_Deoxyribonucleic
      Acid". Journal of Virology. 9 (4): 574â582. PMC 356341.
      PMID 4553678.CS1 maint: Multiple names: authors list (link)
  12. ^Hutchison CA, Phillips S, Edgell MH, Gillam S, Jahnke P, Smith M
      (September 1978). "Mutagenesis_at_a_specific_position_in_a_DNA_sequence"
      (PDF). J. Biol. Chem. 253 (18): 6551â60. PMID 681366.
  13. ^Braman, Jeff, ed. (2002). In Vitro Mutagenesis Protocols. Methods in
      Molecular Biology. 182 (2nd ed.). Humana Press. ISBN 978-0896039100.
  14. ^Kunkel TA. (1985). "Rapid_and_efficient_site-specific_mutagenesis
      without_phenotypic_selection". Proceedings of the National Academy of
      Sciences. 82 (2): 488â92. doi:10.1073/pnas.82.2.488. PMC 397064.
      PMID 3881765.
  15. ^Wells, J. A.; Estell, D. A. (1988). "Subtilisin--an enzyme designed to
      be engineered". Trends in Biochemical Sciences. 13 (8): 291â297. doi:
      10.1016/0968-0004(88)90121-1. PMID 3154281.
  16. ^Karnik, Abhijit; Karnik, Rucha; Grefen, Christopher (2013). "SDM-Assist
      software_to_design_site-directed_mutagenesis_primers_introducing_"silent"
      restriction_sites". BMC Bioinformatics. 14 (1): 105. doi:10.1186/1471-
      2105-14-105. ISSN 1471-2105. PMC 3644487. PMID 23522286.
  17. ^Papworth, C., Bauer, J. C., Braman, J. and Wright, D. A. (1996). "Site-
      directed mutagenesis in one day with >80% efficiency". Strategies. 9 (3):
      3â4.CS1 maint: Multiple names: authors list (link)
  18. ^ a bEdelheit, O; Hanukoglu, A; Hanukoglu, I (2009). "Simple_and
      efficient_site-directed_mutagenesis_using_two_single-primer_reactions_in
      parallel_to_generate_mutants_for_protein_structure-function_studies". BMC
      Biotechnol. 9: 61. doi:10.1186/1472-6750-9-61. PMC 2711942.
      PMID 19566935.
  19. ^Storici F.; Resnick MA. (2006). The delitto perfetto approach to in vivo
      site-directed mutagenesis and chromosome rearrangements with synthetic
      oligonucleotides in yeast. Methods in Enzymology. 409. pp. 329â45. doi:
      10.1016/S0076-6879(05)09019-1. ISBN 9780121828141. PMID 16793410.
  20. ^Storici F.; Resnick MA (2003). "Delitto perfetto targeted mutagenesis in
      yeast with oligonucleotides". Genetic Engineering. 25: 189â207.
      PMID 15260239.
  21. ^Damien Biot-Pelletier and Vincent J. J. Martin (2016). "Seamless_site-
      directed_mutagenesis_of_the_Saccharomyces_cerevisiae_genome_using_CRISPR-
      Cas9". Journal of Biological Engineering. 10: 6. doi:10.1186/s13036-016-
      0028-1. PMC 4850645. PMID 27134651.CS1 maint: Uses authors parameter
      (link)
  22. ^Xu S (20 August 2015). "The_application_of_CRISPR-Cas9_genome_editing_in
      Caenorhabditis_elegans". J Genet Genomics. 42 (8): 413â21. doi:10.1016/
      j.jgg.2015.06.005. PMC 4560834. PMID 26336798.
  23. ^KovÃ¡cs KA, Steinmann M, Halfon O, Magistretti PJ, Cardinaux JR
      (November 2015). "Complex regulation of CREB-binding protein by
      homeodomain-interacting protein kinase 2". Cellular Signalling. 27 (11):
      2252â60. doi:10.1016/j.cellsig.2015.08.001. PMID 26247811.
  24. ^Stauffer CE, Etson D (October 10, 1969). "The_effect_on_subtilisin
      activity_of_oxidizing_a_methionine_residue". Journal of Biological
      Chemistry. 244 (19): 5333â8. PMID 5344139.
  25. ^Estell DA, Graycar TP, Wells JA (10 June 1985). "Engineering_an_enzyme
      by_site-directed_mutagenesis_to_be_resistant_to_chemical_oxidation".
      Journal of Biological Chemistry. 260 (11): 6518â21. PMID 3922976.
  26. ^Yury E. Khudyakov, Howard A. Fields, ed. (25 September 2002). Artificial
      DNA:_Methods_and_Applications. CRC Press. p. 13. ISBN 9781420040166.
***** External links[edit] *****
Library_resources about
Site-directed mutagenesis
===============================================================================
    * Resources_in_your_library
    * Resources_in_other_libraries
    * Nobel_Lecture_on_Invention_of_Site-Directed_Mutagenesis
    * OpenWetWare
    * Diagram_summarizing_site-directed_mutagenesis

Retrieved from "https://en.wikipedia.org/w/index.php?title=Site-
directed_mutagenesis&oldid=886975165"
Categories:
    * Molecular_genetics
    * Mutagenesis
    * Protein_engineering
Hidden categories:
    * CS1_maint:_Multiple_names:_authors_list
    * CS1_maint:_Uses_authors_parameter
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
    * EspaÃ±ol
    * FranÃ§ais
    * Italiano
    * PortuguÃªs
    * ä¸­æ
Edit_links
    * This page was last edited on 9 March 2019, at 19:58 (UTC).
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
