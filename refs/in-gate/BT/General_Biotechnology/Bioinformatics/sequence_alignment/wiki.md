The following text has been accessed from https://en.wikipedia.org/wiki/Sequence_alignment at Fri Aug 9 02:18:49 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















[Listen_to_this_article]
****** Sequence alignment ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be
 challenged and removed.
 Find sources: "Sequence_alignment" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (March 2009)(Learn_how_and_when_to_remove_this_template_message)
In bioinformatics, a sequence alignment is a way of arranging the sequences of
DNA, RNA, or protein to identify regions of similarity that may be a
consequence of functional, structural, or evolutionary relationships between
the sequences.[1] Aligned sequences of nucleotide or amino_acid residues are
typically represented as rows within a matrix. Gaps are inserted between the
residues so that identical or similar characters are aligned in successive
columns. Sequence alignments are also used for non-biological sequences, such
as calculating the distance_cost between strings in a natural_language or in
financial data.
A sequence alignment, produced by ClustalO, of mammalian histone proteins.
Sequences are the amino_acids for residues 120-180 of the proteins. Residues
that are conserved across all sequences are highlighted in grey. Below the
protein sequences is a key denoting conserved_sequence (*), conservative
mutations (:), semi-conservative mutations (.), and non-conservative_mutations
( ).[2]
⁰
***** Contents *****
    * 1_Interpretation
    * 2_Alignment_methods
    * 3_Representations
    * 4_Global_and_local_alignments
    * 5_Pairwise_alignment
          o 5.1_Dot-matrix_methods
          o 5.2_Dynamic_programming
          o 5.3_Word_methods
    * 6_Multiple_sequence_alignment
          o 6.1_Dynamic_programming
          o 6.2_Progressive_methods
          o 6.3_Iterative_methods
          o 6.4_Motif_finding
          o 6.5_Techniques_inspired_by_computer_science
    * 7_Structural_alignment
          o 7.1_DALI
          o 7.2_SSAP
          o 7.3_Combinatorial_extension
    * 8_Phylogenetic_analysis
          o 8.1_Assessment_of_significance
          o 8.2_Assessment_of_credibility
          o 8.3_Scoring_functions
    * 9_Other_biological_uses
    * 10_Non-biological_uses
    * 11_Software
    * 12_See_also
    * 13_References
    * 14_External_links
***** Interpretation[edit] *****
If two sequences in an alignment share a common ancestor, mismatches can be
interpreted as point_mutations and gaps as indels (that is, insertion or
deletion mutations) introduced in one or both lineages in the time since they
diverged from one another. In sequence alignments of proteins, the degree of
similarity between amino_acids occupying a particular position in the sequence
can be interpreted as a rough measure of how conserved a particular region or
sequence_motif is among lineages. The absence of substitutions, or the presence
of only very conservative substitutions (that is, the substitution of amino
acids whose side_chains have similar biochemical properties) in a particular
region of the sequence, suggest [3] that this region has structural or
functional importance. Although DNA and RNA nucleotide bases are more similar
to each other than are amino acids, the conservation of base pairs can indicate
a similar functional or structural role.
***** Alignment methods[edit] *****
Very short or very similar sequences can be aligned by hand. However, most
interesting problems require the alignment of lengthy, highly variable or
extremely numerous sequences that cannot be aligned solely by human effort.
Instead, human knowledge is applied in constructing algorithms to produce high-
quality sequence alignments, and occasionally in adjusting the final results to
reflect patterns that are difficult to represent algorithmically (especially in
the case of nucleotide sequences). Computational approaches to sequence
alignment generally fall into two categories: global alignments and local
alignments. Calculating a global alignment is a form of global_optimization
that "forces" the alignment to span the entire length of all query sequences.
By contrast, local alignments identify regions of similarity within long
sequences that are often widely divergent overall. Local alignments are often
preferable, but can be more difficult to calculate because of the additional
challenge of identifying the regions of similarity.[4] A variety of
computational algorithms have been applied to the sequence alignment problem.
These include slow but formally correct methods like dynamic_programming. These
also include efficient, heuristic_algorithms or probabilistic methods designed
for large-scale database search, that do not guarantee to find best matches.
***** Representations[edit] *****
Alignments are commonly represented both graphically and in text format. In
almost all sequence alignment representations, sequences are written in rows
arranged so that aligned residues appear in successive columns. In text
formats, aligned columns containing identical or similar characters are
indicated with a system of conservation symbols. As in the image above, an
asterisk or pipe symbol is used to show identity between two columns; other
less common symbols include a colon for conservative substitutions and a period
for semiconservative substitutions. Many sequence visualization programs also
use color to display information about the properties of the individual
sequence elements; in DNA and RNA sequences, this equates to assigning each
nucleotide its own color. In protein alignments, such as the one in the image
above, color is often used to indicate amino acid properties to aid in judging
the conservation of a given amino acid substitution. For multiple sequences the
last row in each column is often the consensus_sequence determined by the
alignment; the consensus sequence is also often represented in graphical format
with a sequence_logo in which the size of each nucleotide or amino acid letter
corresponds to its degree of conservation.[5]
Sequence alignments can be stored in a wide variety of text-based file formats,
many of which were originally developed in conjunction with a specific
alignment program or implementation. Most web-based tools allow a limited
number of input and output formats, such as FASTA_format and GenBank format and
the output is not easily editable. Several conversion programs that provide
graphical and/or command line interfaces are available[dead_link], such as
READSEQ and EMBOSS. There are also several programming packages which provide
this conversion functionality, such as BioPython, BioRuby and BioPerl. The SAM/
BAM_files use the CIGAR (Compact Idiosyncratic Gapped Alignment Report) string
format to represent an alignment of a sequence to a reference by encoding a
sequence of events (e.g. match/mismatch, insertions, deletions).[6]
***** Global and local alignments[edit] *****
Global alignments, which attempt to align every residue in every sequence, are
most useful when the sequences in the query set are similar and of roughly
equal size. (This does not mean global alignments cannot start and/or end in
gaps.) A general global alignment technique is the NeedlemanâWunsch
algorithm, which is based on dynamic programming. Local alignments are more
useful for dissimilar sequences that are suspected to contain regions of
similarity or similar sequence motifs within their larger sequence context. The
SmithâWaterman_algorithm is a general local alignment method based on the
same dynamic programming scheme but with additional choices to start and end at
any place.[4]
Hybrid methods, known as semi-global or "glocal" (short for global-local)
methods, search for the best possible partial alignment of the two sequences
(in other words, a combination of one or both starts and one or both ends is
stated to be aligned). This can be especially useful when the downstream part
of one sequence overlaps with the upstream part of the other sequence. In this
case, neither global nor local alignment is entirely appropriate: a global
alignment would attempt to force the alignment to extend beyond the region of
overlap, while a local alignment might not fully cover the region of overlap.
[7] Another case where semi-global alignment is useful is when one sequence is
short (for example a gene sequence) and the other is very long (for example a
chromosome sequence). In that case, the short sequence should be globally
(fully) aligned but only a local (partial) alignment is desired for the long
sequence.
***** Pairwise alignment[edit] *****
Pairwise sequence alignment methods are used to find the best-matching
piecewise (local or global) alignments of two query sequences. Pairwise
alignments can only be used between two sequences at a time, but they are
efficient to calculate and are often used for methods that do not require
extreme precision (such as searching a database for sequences with high
similarity to a query). The three primary methods of producing pairwise
alignments are dot-matrix methods, dynamic programming, and word methods;[1]
however, multiple sequence alignment techniques can also align pairs of
sequences. Although each method has its individual strengths and weaknesses,
all three pairwise methods have difficulty with highly repetitive sequences of
low information_content - especially where the number of repetitions differ in
the two sequences to be aligned. One way of quantifying the utility of a given
pairwise alignment is the 'maximum unique match' (MUM), or the longest
subsequence that occurs in both query sequences. Longer MUM sequences typically
reflect closer relatedness.
**** Dot-matrix methods[edit] ****
Self comparison of a part of a mouse strain genome. The dot-plot shows a
patchwork of lines, demonstrating duplicated segments of DNA.
See main article on dot_plots_(bioinformatics).
A DNA dot_plot of a human zinc_finger transcription_factor (GenBank ID
NM_002383), showing regional self-similarity. The main diagonal represents the
sequence's alignment with itself; lines off the main diagonal represent similar
or repetitive patterns within the sequence. This is a typical example of a
recurrence_plot.
The dot-matrix approach, which implicitly produces a family of alignments for
individual sequence regions, is qualitative and conceptually simple, though
time-consuming to analyze on a large scale. In the absence of noise, it can be
easy to visually identify certain sequence featuresâsuch as insertions,
deletions, repeats, or inverted_repeatsâfrom a dot-matrix plot. To construct
a dot-matrix_plot, the two sequences are written along the top row and leftmost
column of a two-dimensional matrix and a dot is placed at any point where the
characters in the appropriate columns matchâthis is a typical recurrence
plot. Some implementations vary the size or intensity of the dot depending on
the degree of similarity of the two characters, to accommodate conservative
substitutions. The dot plots of very closely related sequences will appear as a
single line along the matrix's main_diagonal.
Problems with dot plots as an information display technique include: noise,
lack of clarity, non-intuitiveness, difficulty extracting match summary
statistics and match positions on the two sequences. There is also much wasted
space where the match data is inherently duplicated across the diagonal and
most of the actual area of the plot is taken up by either empty space or noise,
and, finally, dot-plots are limited to two sequences. None of these limitations
apply to Miropeats alignment diagrams but they have their own particular flaws.
Dot plots can also be used to assess repetitiveness in a single sequence. A
sequence can be plotted against itself and regions that share significant
similarities will appear as lines off the main diagonal. This effect can occur
when a protein consists of multiple similar structural_domains.
**** Dynamic programming[edit] ****
The technique of dynamic_programming can be applied to produce global
alignments via the Needleman-Wunsch_algorithm, and local alignments via the
Smith-Waterman_algorithm. In typical usage, protein alignments use a
substitution_matrix to assign scores to amino-acid matches or mismatches, and a
gap_penalty for matching an amino acid in one sequence to a gap in the other.
DNA and RNA alignments may use a scoring matrix, but in practice often simply
assign a positive match score, a negative mismatch score, and a negative gap
penalty. (In standard dynamic programming, the score of each amino acid
position is independent of the identity of its neighbors, and therefore base
stacking effects are not taken into account. However, it is possible to account
for such effects by modifying the algorithm.) A common extension to standard
linear gap costs, is the usage of two different gap penalties for opening a gap
and for extending a gap. Typically the former is much larger than the latter,
e.g. -10 for gap open and -2 for gap extension. Thus, the number of gaps in an
alignment is usually reduced and residues and gaps are kept together, which
typically makes more biological sense. The Gotoh algorithm implements affine
gap costs by using three matrices.
Dynamic programming can be useful in aligning nucleotide to protein sequences,
a task complicated by the need to take into account frameshift mutations
(usually insertions or deletions). The framesearch method produces a series of
global or local pairwise alignments between a query nucleotide sequence and a
search set of protein sequences, or vice versa. Its ability to evaluate
frameshifts offset by an arbitrary number of nucleotides makes the method
useful for sequences containing large numbers of indels, which can be very
difficult to align with more efficient heuristic methods. In practice, the
method requires large amounts of computing power or a system whose architecture
is specialized for dynamic programming. The BLAST and EMBOSS suites provide
basic tools for creating translated alignments (though some of these approaches
take advantage of side-effects of sequence searching capabilities of the
tools). More general methods are available from both commercial sources, such
as FrameSearch, distributed as part of the Accelrys GCG_package, and open-
source_software such as Genewise.
The dynamic programming method is guaranteed to find an optimal alignment given
a particular scoring function; however, identifying a good scoring function is
often an empirical rather than a theoretical matter. Although dynamic
programming is extensible to more than two sequences, it is prohibitively slow
for large numbers of sequences or extremely long sequences.
**** Word methods[edit] ****
Word methods, also known as k-tuple methods, are heuristic methods that are not
guaranteed to find an optimal alignment solution, but are significantly more
efficient than dynamic programming. These methods are especially useful in
large-scale database searches where it is understood that a large proportion of
the candidate sequences will have essentially no significant match with the
query sequence. Word methods are best known for their implementation in the
database search tools FASTA and the BLAST family.[1] Word methods identify a
series of short, nonoverlapping subsequences ("words") in the query sequence
that are then matched to candidate database sequences. The relative positions
of the word in the two sequences being compared are subtracted to obtain an
offset; this will indicate a region of alignment if multiple distinct words
produce the same offset. Only if this region is detected do these methods apply
more sensitive alignment criteria; thus, many unnecessary comparisons with
sequences of no appreciable similarity are eliminated.
In the FASTA method, the user defines a value k to use as the word length with
which to search the database. The method is slower but more sensitive at lower
values of k, which are also preferred for searches involving a very short query
sequence. The BLAST family of search methods provides a number of algorithms
optimized for particular types of queries, such as searching for distantly
related sequence matches. BLAST was developed to provide a faster alternative
to FASTA without sacrificing much accuracy; like FASTA, BLAST uses a word
search of length k, but evaluates only the most significant word matches,
rather than every word match as does FASTA. Most BLAST implementations use a
fixed default word length that is optimized for the query and database type,
and that is changed only under special circumstances, such as when searching
with repetitive or very short query sequences. Implementations can be found via
a number of web portals, such as EMBL_FASTA and NCBI_BLAST.
***** Multiple sequence alignment[edit] *****
Main article: Multiple_sequence_alignment
Alignment of 27 avian_influenza hemagglutinin protein sequences colored by
residue conservation (top) and residue properties (bottom)
Multiple_sequence_alignment is an extension of pairwise alignment to
incorporate more than two sequences at a time. Multiple alignment methods try
to align all of the sequences in a given query set. Multiple alignments are
often used in identifying conserved sequence regions across a group of
sequences hypothesized to be evolutionarily related. Such conserved sequence
motifs can be used in conjunction with structural and mechanistic information
to locate the catalytic active_sites of enzymes. Alignments are also used to
aid in establishing evolutionary relationships by constructing phylogenetic
trees. Multiple sequence alignments are computationally difficult to produce
and most formulations of the problem lead to NP-complete combinatorial
optimization problems.[8][9] Nevertheless, the utility of these alignments in
bioinformatics has led to the development of a variety of methods suitable for
aligning three or more sequences.
**** Dynamic programming[edit] ****
The technique of dynamic programming is theoretically applicable to any number
of sequences; however, because it is computationally expensive in both time and
memory, it is rarely used for more than three or four sequences in its most
basic form. This method requires constructing the n-dimensional equivalent of
the sequence matrix formed from two sequences, where n is the number of
sequences in the query. Standard dynamic programming is first used on all pairs
of query sequences and then the "alignment space" is filled in by considering
possible matches or gaps at intermediate positions, eventually constructing an
alignment essentially between each two-sequence alignment. Although this
technique is computationally expensive, its guarantee of a global optimum
solution is useful in cases where only a few sequences need to be aligned
accurately. One method for reducing the computational demands of dynamic
programming, which relies on the "sum of pairs" objective_function, has been
implemented in the MSA software package.[10]
**** Progressive methods[edit] ****
Progressive, hierarchical, or tree methods generate a multiple sequence
alignment by first aligning the most similar sequences and then adding
successively less related sequences or groups to the alignment until the entire
query set has been incorporated into the solution. The initial tree describing
the sequence relatedness is based on pairwise comparisons that may include
heuristic pairwise alignment methods similar to FASTA. Progressive alignment
results are dependent on the choice of "most related" sequences and thus can be
sensitive to inaccuracies in the initial pairwise alignments. Most progressive
multiple sequence alignment methods additionally weight the sequences in the
query set according to their relatedness, which reduces the likelihood of
making a poor choice of initial sequences and thus improves alignment accuracy.
Many variations of the Clustal progressive implementation[11][12][13] are used
for multiple sequence alignment, phylogenetic tree construction, and as input
for protein_structure_prediction. A slower but more accurate variant of the
progressive method is known as T-Coffee.[14]
**** Iterative methods[edit] ****
Iterative methods attempt to improve on the heavy dependence on the accuracy of
the initial pairwise alignments, which is the weak point of the progressive
methods. Iterative methods optimize an objective_function based on a selected
alignment scoring method by assigning an initial global alignment and then
realigning sequence subsets. The realigned subsets are then themselves aligned
to produce the next iteration's multiple sequence alignment. Various ways of
selecting the sequence subgroups and objective function are reviewed in.[15]
**** Motif finding[edit] ****
Motif finding, also known as profile analysis, constructs global multiple
sequence alignments that attempt to align short conserved sequence_motifs among
the sequences in the query set. This is usually done by first constructing a
general global multiple sequence alignment, after which the highly conserved
regions are isolated and used to construct a set of profile matrices. The
profile matrix for each conserved region is arranged like a scoring matrix but
its frequency counts for each amino acid or nucleotide at each position are
derived from the conserved region's character distribution rather than from a
more general empirical distribution. The profile matrices are then used to
search other sequences for occurrences of the motif they characterize. In cases
where the original data_set contained a small number of sequences, or only
highly related sequences, pseudocounts are added to normalize the character
distributions represented in the motif.
**** Techniques inspired by computer science[edit] ****
A variety of general optimization algorithms commonly used in computer science
have also been applied to the multiple sequence alignment problem. Hidden
Markov_models have been used to produce probability scores for a family of
possible multiple sequence alignments for a given query set; although early
HMM-based methods produced underwhelming performance, later applications have
found them especially effective in detecting remotely related sequences because
they are less susceptible to noise created by conservative or semiconservative
substitutions.[16] Genetic_algorithms and simulated_annealing have also been
used in optimizing multiple sequence alignment scores as judged by a scoring
function like the sum-of-pairs method. More complete details and software
packages can be found in the main article multiple_sequence_alignment.
The BurrowsâWheeler_transform has been successfully applied to fast short
read alignment in popular tools such as Bowtie and BWA. See FM-index.
***** Structural alignment[edit] *****
Main article: Structural_alignment
Structural alignments, which are usually specific to protein and sometimes RNA
sequences, use information about the secondary and tertiary_structure of the
protein or RNA molecule to aid in aligning the sequences. These methods can be
used for two or more sequences and typically produce local alignments; however,
because they depend on the availability of structural information, they can
only be used for sequences whose corresponding structures are known (usually
through X-ray_crystallography or NMR_spectroscopy). Because both protein and
RNA structure is more evolutionarily conserved than sequence,[17] structural
alignments can be more reliable between sequences that are very distantly
related and that have diverged so extensively that sequence comparison cannot
reliably detect their similarity.
Structural alignments are used as the "gold standard" in evaluating alignments
for homology-based protein_structure_prediction[18] because they explicitly
align regions of the protein sequence that are structurally similar rather than
relying exclusively on sequence information. However, clearly structural
alignments cannot be used in structure prediction because at least one sequence
in the query set is the target to be modeled, for which the structure is not
known. It has been shown that, given the structural alignment between a target
and a template sequence, highly accurate models of the target protein sequence
can be produced; a major stumbling block in homology-based structure prediction
is the production of structurally accurate alignments given only sequence
information.[18]
**** DALI[edit] ****
The DALI method, or distance_matrix alignment, is a fragment-based method for
constructing structural alignments based on contact similarity patterns between
successive hexapeptides in the query sequences.[19] It can generate pairwise or
multiple alignments and identify a query sequence's structural neighbors in the
Protein_Data_Bank (PDB). It has been used to construct the FSSP structural
alignment database (Fold classification based on Structure-Structure alignment
of Proteins, or Families of Structurally Similar Proteins). A DALI webserver
can be accessed at DALI and the FSSP is located at The_Dali_Database.
**** SSAP[edit] ****
SSAP (sequential structure alignment program) is a dynamic programming-based
method of structural alignment that uses atom-to-atom vectors in structure
space as comparison points. It has been extended since its original description
to include multiple as well as pairwise alignments,[20] and has been used in
the construction of the CATH (Class, Architecture, Topology, Homology)
hierarchical database classification of protein folds.[21] The CATH database
can be accessed at CATH_Protein_Structure_Classification.
**** Combinatorial extension[edit] ****
The combinatorial extension method of structural alignment generates a pairwise
structural alignment by using local geometry to align short fragments of the
two proteins being analyzed and then assembles these fragments into a larger
alignment.[22] Based on measures such as rigid-body root_mean_square_distance,
residue distances, local secondary structure, and surrounding environmental
features such as residue neighbor hydrophobicity, local alignments called
"aligned fragment pairs" are generated and used to build a similarity matrix
representing all possible structural alignments within predefined cutoff
criteria. A path from one protein structure state to the other is then traced
through the matrix by extending the growing alignment one fragment at a time.
The optimal such path defines the combinatorial-extension alignment. A web-
based server implementing the method and providing a database of pairwise
alignments of structures in the Protein Data Bank is located at the
Combinatorial_Extension website.
***** Phylogenetic analysis[edit] *****
Main article: Computational_phylogenetics
Phylogenetics and sequence alignment are closely related fields due to the
shared necessity of evaluating sequence relatedness.[23] The field of
phylogenetics makes extensive use of sequence alignments in the construction
and interpretation of phylogenetic_trees, which are used to classify the
evolutionary relationships between homologous genes represented in the genomes
of divergent species. The degree to which sequences in a query set differ is
qualitatively related to the sequences' evolutionary distance from one another.
Roughly speaking, high sequence identity suggests that the sequences in
question have a comparatively young most_recent_common_ancestor, while low
identity suggests that the divergence is more ancient. This approximation,
which reflects the "molecular_clock" hypothesis that a roughly constant rate of
evolutionary change can be used to extrapolate the elapsed time since two genes
first diverged (that is, the coalescence time), assumes that the effects of
mutation and selection are constant across sequence lineages. Therefore, it
does not account for possible difference among organisms or species in the
rates of DNA_repair or the possible functional conservation of specific regions
in a sequence. (In the case of nucleotide sequences, the molecular clock
hypothesis in its most basic form also discounts the difference in acceptance
rates between silent_mutations that do not alter the meaning of a given codon
and other mutations that result in a different amino_acid being incorporated
into the protein). More statistically accurate methods allow the evolutionary
rate on each branch of the phylogenetic tree to vary, thus producing better
estimates of coalescence times for genes.
Progressive multiple alignment techniques produce a phylogenetic tree by
necessity because they incorporate sequences into the growing alignment in
order of relatedness. Other techniques that assemble multiple sequence
alignments and phylogenetic trees score and sort trees first and calculate a
multiple sequence alignment from the highest-scoring tree. Commonly used
methods of phylogenetic tree construction are mainly heuristic because the
problem of selecting the optimal tree, like the problem of selecting the
optimal multiple sequence alignment, is NP-hard.[24]
**** Assessment of significance[edit] ****
Sequence alignments are useful in bioinformatics for identifying sequence
similarity, producing phylogenetic trees, and developing homology models of
protein structures. However, the biological relevance of sequence alignments is
not always clear. Alignments are often assumed to reflect a degree of
evolutionary change between sequences descended from a common ancestor;
however, it is formally possible that convergent_evolution can occur to produce
apparent similarity between proteins that are evolutionarily unrelated but
perform similar functions and have similar structures.
In database searches such as BLAST, statistical methods can determine the
likelihood of a particular alignment between sequences or sequence regions
arising by chance given the size and composition of the database being
searched. These values can vary significantly depending on the search space. In
particular, the likelihood of finding a given alignment by chance increases if
the database consists only of sequences from the same organism as the query
sequence. Repetitive sequences in the database or query can also distort both
the search results and the assessment of statistical significance; BLAST
automatically filters such repetitive sequences in the query to avoid apparent
hits that are statistical artifacts.
Methods of statistical significance estimation for gapped sequence alignments
are available in the literature.[23][25][26][27][28][29][30][31]
**** Assessment of credibility[edit] ****
Statistical significance indicates the probability that an alignment of a given
quality could arise by chance, but does not indicate how much superior a given
alignment is to alternative alignments of the same sequences. Measures of
alignment credibility indicate the extent to which the best scoring alignments
for a given pair of sequences are substantially similar. Methods of alignment
credibility estimation for gapped sequence alignments are available in the
literature.[32]
**** Scoring functions[edit] ****
The choice of a scoring function that reflects biological or statistical
observations about known sequences is important to producing good alignments.
Protein sequences are frequently aligned using substitution_matrices that
reflect the probabilities of given character-to-character substitutions. A
series of matrices called PAM_matrices (Point Accepted Mutation matrices,
originally defined by Margaret_Dayhoff and sometimes referred to as "Dayhoff
matrices") explicitly encode evolutionary approximations regarding the rates
and probabilities of particular amino acid mutations. Another common series of
scoring matrices, known as BLOSUM (Blocks Substitution Matrix), encodes
empirically derived substitution probabilities. Variants of both types of
matrices are used to detect sequences with differing levels of divergence, thus
allowing users of BLAST or FASTA to restrict searches to more closely related
matches or expand to detect more divergent sequences. Gap_penalties account for
the introduction of a gap - on the evolutionary model, an insertion or deletion
mutation - in both nucleotide and protein sequences, and therefore the penalty
values should be proportional to the expected rate of such mutations. The
quality of the alignments produced therefore depends on the quality of the
scoring function.
It can be very useful and instructive to try the same alignment several times
with different choices for scoring matrix and/or gap penalty values and compare
the results. Regions where the solution is weak or non-unique can often be
identified by observing which regions of the alignment are robust to variations
in alignment parameters.
***** Other biological uses[edit] *****
Sequenced RNA, such as expressed_sequence_tags and full-length mRNAs, can be
aligned to a sequenced genome to find where there are genes and get information
about alternative_splicing[33] and RNA_editing.[34] Sequence alignment is also
a part of genome_assembly, where sequences are aligned to find overlap so that
contigs (long stretches of sequence) can be formed.[35] Another use is SNP
analysis, where sequences from different individuals are aligned to find single
basepairs that are often different in a population.[36]
***** Non-biological uses[edit] *****
The methods used for biological sequence alignment have also found applications
in other fields, most notably in natural_language_processing and in social
sciences, where the Needleman-Wunsch_algorithm is usually referred to as
Optimal_matching.[37] Techniques that generate the set of elements from which
words will be selected in natural-language generation algorithms have borrowed
multiple sequence alignment techniques from bioinformatics to produce
linguistic versions of computer-generated mathematical proofs.[38] In the field
of historical and comparative linguistics, sequence alignment has been used to
partially automate the comparative_method by which linguists traditionally
reconstruct languages.[39] Business and marketing research has also applied
multiple sequence alignment techniques in analyzing series of purchases over
time.[40]
***** Software[edit] *****
Main article: Sequence_alignment_software
A more complete list of available software categorized by algorithm and
alignment type is available at sequence_alignment_software, but common software
tools used for general sequence alignment tasks include ClustalW2[41] and T-
coffee[42] for alignment, and BLAST[43] and FASTA3x[44] for database searching.
Commercial tools such as DNASTAR_Lasergene, Geneious, and PatternHunter are
also available. Tools annotated as performing sequence_alignment are listed in
the bio.tools registry.
Alignment algorithms and software can be directly compared to one another using
a standardized set of benchmark reference multiple sequence alignments known as
BAliBASE.[45] The data set consists of structural alignments, which can be
considered a standard against which purely sequence-based methods are compared.
The relative performance of many common alignment methods on frequently
encountered alignment problems has been tabulated and selected results
published online at BAliBASE.[46][47] A comprehensive list of BAliBASE scores
for many (currently 12) different alignment tools can be computed within the
protein workbench STRAP.[48]
***** See also[edit] *****
    * Sequence_homology
    * Sequence_mining
    * BLAST
    * String_searching_algorithm
    * Alignment-free_sequence_analysis
    * UGENE
    * NeedlemanâWunsch_algorithm
***** References[edit] *****
   1. ^ a b cMount DM. (2004). Bioinformatics: Sequence and Genome Analysis
      (2nd ed.). Cold Spring Harbor Laboratory Press: Cold Spring Harbor, NY.
      ISBN 978-0-87969-608-5.
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
   3. ^"Clustal_FAQ_#Symbols". Clustal. Retrieved 8 December 2014.
   4. ^Ng PC; Henikoff S (May 2001). "Predicting_deleterious_amino_acid
      substitutions". Genome Res. 11 (5): 863â74. doi:10.1101/gr.176601.
      PMC 311071. PMID 11337480.
   5. ^ a bPolyanovsky, V. O.; Roytberg, M. A.; Tumanyan, V. G. (2011).
      "Comparative_analysis_of_the_quality_of_a_global_algorithm_and_a_local
      algorithm_for_alignment_of_two_sequences". Algorithms for Molecular
      Biology. 6 (1): 25. doi:10.1186/1748-7188-6-25. PMC 3223492.
      PMID 22032267.
   6. ^Schneider TD; Stephens RM (1990). "Sequence_logos:_a_new_way_to_display
      consensus_sequences". Nucleic Acids Res. 18 (20): 6097â6100. doi:
      10.1093/nar/18.20.6097. PMC 332411. PMID 2172928.
   7. ^"Sequence_Alignment/Map_Format_Specification" (PDF).
   8. ^Brudno M; Malde S; Poliakov A; Do CB; Couronne O; Dubchak I; Batzoglou S
      (2003). "Glocal_alignment:_finding_rearrangements_during_alignment".
      Bioinformatics. 19. Suppl 1 (90001): i54â62. doi:10.1093/
      bioinformatics/btg1005. PMID 12855437.
   9. ^Wang L; Jiang T. (1994). "On the complexity of multiple sequence
      alignment". J Comput Biol. 1 (4): 337â48. CiteSeerX 10.1.1.408.894.
      doi:10.1089/cmb.1994.1.337. PMID 8790475.
  10. ^Elias, Isaac (2006). "Settling the intractability of multiple
      alignment". J Comput Biol. 13 (7): 1323â1339. CiteSeerX 10.1.1.6.256.
      doi:10.1089/cmb.2006.13.1323. PMID 17037961.
  11. ^Lipman DJ; Altschul SF; Kececioglu JD (1989). "A_tool_for_multiple
      sequence_alignment". Proc Natl Acad Sci USA. 86 (12): 4412â5. Bibcode:
      1989PNAS...86.4412L. doi:10.1073/pnas.86.12.4412. PMC 287279.
      PMID 2734293.
  12. ^Higgins_DG, Sharp PM (1988). "CLUSTAL: a package for performing multiple
      sequence alignment on a microcomputer". Gene. 73 (1): 237â44. doi:
      10.1016/0378-1119(88)90330-7. PMID 3243435.
  13. ^Thompson JD; Higgins_DG; Gibson TJ. (1994). "CLUSTAL_W:_improving_the
      sensitivity_of_progressive_multiple_sequence_alignment_through_sequence
      weighting,_position-specific_gap_penalties_and_weight_matrix_choice".
      Nucleic Acids Res. 22 (22): 4673â80. doi:10.1093/nar/22.22.4673.
      PMC 308517. PMID 7984417.
  14. ^Chenna R; Sugawara H; Koike T; Lopez R; Gibson TJ; Higgins DG; Thompson
      JD. (2003). "Multiple_sequence_alignment_with_the_Clustal_series_of
      programs". Nucleic Acids Res. 31 (13): 3497â500. doi:10.1093/nar/
      gkg500. PMC 168907. PMID 12824352.
  15. ^Notredame C; Higgins_DG; Heringa J. (2000). "T-Coffee: A novel method
      for fast and accurate multiple sequence alignment". J Mol Biol. 302 (1):
      205â17. doi:10.1006/jmbi.2000.4042. PMID 10964570.
  16. ^Hirosawa M; Totoki Y; Hoshida M; Ishikawa M. (1995). "Comprehensive
      study_on_iterative_algorithms_of_multiple_sequence_alignment". Comput
      Appl Biosci. 11 (1): 13â8. doi:10.1093/bioinformatics/11.1.13.
      PMID 7796270.
  17. ^Karplus K; Barrett C; Hughey R. (1998). "Hidden_Markov_models_for
      detecting_remote_protein_homologies". Bioinformatics. 14 (10): 846â856.
      doi:10.1093/bioinformatics/14.10.846. PMID 9927713.
  18. ^Chothia C; Lesk AM. (April 1986). "The_relation_between_the_divergence
      of_sequence_and_structure_in_proteins". EMBO J. 5 (4): 823â6. doi:
      10.1002/j.1460-2075.1986.tb04288.x. PMC 1166865. PMID 3709526.
  19. ^ a bZhang Y; Skolnick J. (2005). "The_protein_structure_prediction
      problem_could_be_solved_using_the_current_PDB_library". Proc Natl Acad
      Sci USA. 102 (4): 1029â34. Bibcode:2005PNAS..102.1029Z. doi:10.1073/
      pnas.0407152101. PMC 545829. PMID 15653774.
  20. ^Holm L; Sander C (1996). "Mapping the protein universe". Science. 273
      (5275): 595â603. Bibcode:1996Sci...273..595H. doi:10.1126/
      science.273.5275.595. PMID 8662544.
  21. ^Taylor WR; Flores TP; Orengo CA. (1994). "Multiple_protein_structure
      alignment". Protein Sci. 3 (10): 1858â70. doi:10.1002/pro.5560031025.
      PMC 2142613. PMID 7849601.
  22. [permanent_dead_link]
  23. ^Orengo CA; Michie AD; Jones S; Jones DT; Swindells MB; Thornton JM
      (1997). "CATH--a hierarchic classification of protein domain structures".
      Structure. 5 (8): 1093â108. doi:10.1016/S0969-2126(97)00260-8.
      PMID 9309224.
  24. ^Shindyalov IN; Bourne PE. (1998). "Protein_structure_alignment_by
      incremental_combinatorial_extension_(CE)_of_the_optimal_path". Protein
      Eng. 11 (9): 739â47. doi:10.1093/protein/11.9.739. PMID 9796821.
  25. ^ a bOrtet P; Bastien O (2010). "Where_Does_the_Alignment_Score
      Distribution_Shape_Come_from?". Evolutionary Bioinformatics. 6:
      159â187. doi:10.4137/EBO.S5875. PMC 3023300. PMID 21258650.
  26. ^Felsenstein J. (2004). Inferring Phylogenies. Sinauer Associates:
      Sunderland, MA. ISBN 978-0-87893-177-4.
  27. ^Altschul SF; Gish W (1996). Local Alignment Statistics. Meth.Enz.
      Methods in Enzymology. 266. pp. 460â480. doi:10.1016/S0076-6879
      (96)66029-7. ISBN 9780121821678. PMID 8743700.
  28. ^Hartmann AK (2002). "Sampling rare events: statistics of local sequence
      alignments". Phys. Rev. E. 65 (5): 056102. arXiv:cond-mat/0108201.
      Bibcode:2002PhRvE..65e6102H. doi:10.1103/PhysRevE.65.056102.
      PMID 12059642.
  29. ^Newberg LA (2008). "Significance_of_gapped_sequence_alignments". J
      Comput Biol. 15 (9): 1187â1194. doi:10.1089/cmb.2008.0125. PMC 2737730.
      PMID 18973434.
  30. ^Eddy SR; Rost, Burkhard (2008). Rost, Burkhard (ed.). "A_probabilistic
      model_of_local_sequence_alignment_that_simplifies_statistical
      significance_estimation". PLoS Comput Biol. 4 (5): e1000069. Bibcode:
      2008PLSCB...4E0069E. doi:10.1371/journal.pcbi.1000069. PMC 2396288.
      PMID 18516236.
  31. ^Bastien O; Aude JC; Roy S; Marechal E (2004). "Fundamentals_of_massive
      automatic_pairwise_alignments_of_protein_sequences:_theoretical
      significance_of_Z-value_statistics". Bioinformatics. 20 (4): 534â537.
      doi:10.1093/bioinformatics/btg440. PMID 14990449.
  32. ^Agrawal A; Huang X (2011). "Pairwise Statistical Significance of Local
      Sequence Alignment Using Sequence-Specific and Position-Specific
      Substitution Matrices". IEEE/ACM Transactions on Computational Biology
      and Bioinformatics. 8 (1): 194â205. doi:10.1109/TCBB.2009.69.
      PMID 21071807.
  33. ^Agrawal A; Brendel VP; Huang X (2008). "Pairwise_statistical
      significance_and_empirical_determination_of_effective_gap_opening
      penalties_for_protein_local_sequence_alignment". International Journal of
      Computational Biology and Drug Design. 1 (4): 347â367. doi:10.1504/
      IJCBDD.2008.022207. Archived from the_original on 28 January 2013.
  34. ^Newberg LA; Lawrence CE (2009). "Exact_Calculation_of_Distributions_on
      Integers,_with_Application_to_Sequence_Alignment". J Comput Biol. 16 (1):
      1â18. doi:10.1089/cmb.2008.0137. PMC 2858568. PMID 19119992.
  35. ^Kim N; Lee C (2008). Bioinformatics detection of alternative splicing.
      Methods Mol. Biol. Methods in Molecular Biologyâ¢. 452. pp. 179â97.
      doi:10.1007/978-1-60327-159-2_9. ISBN 978-1-58829-707-5. PMID 18566765.
  36. ^Li JB, Levanon EY, Yoon JK, et al. (May 2009). "Genome-wide
      identification of human RNA editing sites by parallel DNA capturing and
      sequencing". Science. 324 (5931): 1210â3. Bibcode:2009Sci...324.1210L.
      doi:10.1126/science.1170995. PMID 19478186.
  37. ^Blazewicz J, Bryja M, Figlerowicz M, et al. (June 2009). "Whole genome
      assembly from 454 sequencing output via modified DNA graph concept".
      Comput Biol Chem. 33 (3): 224â30. doi:10.1016/
      j.compbiolchem.2009.04.005. PMID 19477687.
  38. ^Duran C; Appleby N; Vardy M; Imelfort M; Edwards D; Batley J (May 2009).
      "Single nucleotide polymorphism discovery in barley using autoSNPdb".
      Plant Biotechnol. J. 7 (4): 326â33. doi:10.1111/j.1467-
      7652.2009.00407.x. PMID 19386041.
  39. ^Abbott A.; Tsay A. (2000). "Sequence Analysis and Optimal Matching
      Methods in Sociology, Review and Prospect". Sociological Methods and
      Research. 29 (1): 3â33. doi:10.1177/0049124100029001001.
  40. ^Barzilay R; Lee L. (2002). "Bootstrapping_Lexical_Choice_via_Multiple-
      Sequence_Alignment" (PDF). Proceedings of the Conference on Empirical
      Methods in Natural Language Processing (EMNLP). 10: 164â171. arXiv:cs/
      0205065. doi:10.3115/1118693.1118715.
  41. ^Kondrak, Grzegorz (2002). "Algorithms_for_Language_Reconstruction"
      (PDF). University of Toronto, Ontario. Retrieved 21 January 2007.
  42. ^Prinzie A.; D. Van den Poel (2006). "Incorporating_sequential
      information_into_traditional_classification_models_by_using_an_element/
      position-sensitive_SAM". Decision Support Systems. 42 (2): 508â526.
      doi:10.1016/j.dss.2005.02.004.
  43.  See also Prinzie and Van den Poel's paperPrinzie, A; Vandenpoel, D
      (2007). "Predicting_home-appliance_acquisition_sequences:_Markov/Markov
      for_Discrimination_and_survival_analysis_for_modeling_sequential
      information_in_NPTB_models". Decision Support Systems. 44 (1): 28â45.
      doi:10.1016/j.dss.2007.02.008.
  44. ^EMBL-EBI. "ClustalW2_<_Multiple_Sequence_Alignment_<_EMBL-EBI".
      www.EBI.ac.uk. Retrieved 12 June 2017.
  45. ^ T-coffee
  46. ^"BLAST:_Basic_Local_Alignment_Search_Tool". blast.ncbi.nlm.NIH.gov.
      Retrieved 12 June 2017.
  47. ^"UVA_FASTA_Server". fasta.bioch.Virginia.edu. Retrieved 12 June 2017.
  48. ^Thompson JD; Plewniak F; Poch O (1999). "BAliBASE:_a_benchmark_alignment
      database_for_the_evaluation_of_multiple_alignment_programs".
      Bioinformatics. 15 (1): 87â8. doi:10.1093/bioinformatics/15.1.87.
      PMID 10068696.
  49. ^ BAliBASE
  50. ^Thompson JD; Plewniak F; Poch O. (1999). "A_comprehensive_comparison_of
      multiple_sequence_alignment_programs". Nucleic Acids Res. 27 (13):
      2682â90. doi:10.1093/nar/27.13.2682. PMC 148477. PMID 10373585.
  51. ^"Multiple_sequence_alignment:_Strap". 3d-alignment.eu. Retrieved 12 June
      2017.
***** External links[edit] *****
 Wikiversity has learning resources about Dot-matrix_methods
Listen to this article (info/dl)

This audio file was created from a revision of the article "Sequence alignment"
dated 2012-06-05, and does not reflect subsequent edits to the article. (Audio
help)
More_spoken_articles
    *  Media related to Sequence_alignment at Wikimedia Commons
    * v
    * t
    * e
Bioinformatics
                   * Sequence databases: GenBank, European_Nucleotide_Archive
                     and DNA_Data_Bank_of_Japan
                   * Secondary databases: UniProt, database of protein
                     sequences grouping together Swiss-Prot, TrEMBL and Protein
Databases            Information_Resource
                   * Other databases: Protein_Data_Bank, Ensembl and InterPro
                   * Specialised genomic databases: BOLD, Saccharomyces_Genome
                     Database, FlyBase, VectorBase, WormBase, PHI-base,
                     Arabidopsis_Information_Resource and Zebrafish_Information
                     Network
                   * BLAST
                   * Bowtie
                   * Clustal
Software           * HMMER
                   * MUSCLE
                   * SAMtools
                   * TopHat
Other              * Server: ExPASy
                   * Ontology: Gene_Ontology
                   * European_Bioinformatics_Institute
                   * US_National_Center_for_Biotechnology_Information
                   * Swiss_Institute_of_Bioinformatics
Institutions       * Japanese_Institute_of_Genetics
                   * Philippine_Genome_Center
                   * Broad_Institute
                   * Wellcome_Sanger_Institute
                   * International_Society_for_Computational_Biology (ISCB)
                   * European_Molecular_Biology_network (EMBnet)
Organizations      * African_Society_for_Bioinformatics_and_Computational
                     Biology (ASBCB)
                   * Japanese_Society_for_Bioinformatics (JSBi)
                   * Intelligent_Systems_for_Molecular_Biology (ISMB)
                   * Research_in_Computational_Molecular_Biology (RECOMB)
                   * European_Conference_on_Computational_Biology (ECCB)
Meetings           * Pacific_Symposium_on_Biocomputing (PSB)
                   * ISCB_Africa_ASBCB_Conference_on_Bioinformatics
                   * Basel_Computational_Biology_Conferenceâ ([BC2])
                   * International_Conference_on_Bioinformatics (InCoB)
                   * Computational_biology
                   * List_of_biological_databases
Related topics     * Sequencing
                   * Sequence_database
                   * Sequence alignment
                   * Molecular_phylogenetics
    * [Category] Category
    * [Commons page] Commons

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Sequence_alignment&oldid=909273712"
Categories:
    * Spoken_articles
    * Bioinformatics
    * Computational_phylogenetics
    * Sequence_alignment_algorithms
    * Evolutionary_developmental_biology
Hidden categories:
    * CS1:_long_volume_value
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_September_2016
    * Articles_with_permanently_dead_external_links
    * Articles_needing_additional_references_from_March_2009
    * All_articles_needing_additional_references
    * Articles_with_dead_external_links_from_August_2009
    * Articles_with_hAudio_microformats
    * Commons_category_link_from_Wikidata
    * Use_dmy_dates_from_April_2017
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
    * Asturianu
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Occitan
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 4 August 2019, at 09:54 (UTC).
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
