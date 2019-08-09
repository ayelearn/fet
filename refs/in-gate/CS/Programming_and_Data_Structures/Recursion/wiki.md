The following text has been accessed from https://en.wikipedia.org/wiki/Recursion at Fri Aug 9 01:07:43 IST 2019
Creative_Commons_Attribution-ShareAlike_License



















[Page_semi-protected]
****** Recursion ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other uses, see Recursion_(disambiguation).
 This article needs additional citations for verification. Please help improve_this_article by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and removed.
 Find sources: "Recursion" â news Â· newspapers Â· books Â· scholar Â· JSTOR (June 2012)(Learn
 how_and_when_to_remove_this_template_message)
A visual form of recursion known as the Droste_effect. The woman in this image
holds an object that contains a smaller image of her holding an identical
object, which in turn contains a smaller image of herself holding an identical
object, and so forth. 1904 Droste cocoa tin, designed by Jan Misset
Recursion (adjective: recursive) occurs when a thing is defined in terms of
itself or of its type. Recursion is used in a variety of disciplines ranging
from linguistics to logic. The most common application of recursion is in
mathematics and computer_science, where a function being defined is applied
within its own definition. While this apparently defines an infinite number of
instances (function values), it is often done in such a way that no loop or
infinite chain of references can occur.
⁰
***** Contents *****
    * 1_Formal_definitions
    * 2_Informal_definition
    * 3_In_language
          o 3.1_Recursive_humor
    * 4_In_mathematics
          o 4.1_Recursively_defined_sets
                # 4.1.1_Example:_the_natural_numbers
                # 4.1.2_Example:_Proof_procedure
          o 4.2_Finite_subdivision_rules
          o 4.3_Functional_recursion
          o 4.4_Proofs_involving_recursive_definitions
          o 4.5_Recursive_optimization
          o 4.6_The_recursion_theorem
                # 4.6.1_Proof_of_uniqueness
    * 5_In_computer_science
    * 6_In_art
    * 7_See_also
    * 8_References
    * 9_Bibliography
    * 10_External_links
***** Formal definitions *****
Ouroboros, an ancient symbol depicting a serpent or dragon eating its own tail.
In mathematics and computer science, a class of objects or methods exhibits
recursive behavior when it can be defined by two properties:
   1. A simple base case (or cases)âa terminating scenario that does not use
      recursion to produce an answer
   2. A set of rules that reduces all other cases toward the base case
For example, the following is a recursive definition of a person's ancestors:
    * One's parents are one's ancestors (base case).
    * The ancestors of one's ancestors are also one's ancestors (recursion
      step).
The Fibonacci_sequence is a classic example of recursion:
    Fib  ( 0 ) = 0  &#xA0;as base case 1,    {\displaystyle {\text{Fib}}(0)=0
{\text{ as base case 1,}}}  [\text{Fib}(0)=0\text{ as base case 1,}]
    Fib  ( 1 ) = 1  &#xA0;as base case 2,    {\displaystyle {\text{Fib}}(1)=1
{\text{ as base case 2,}}}  [\text{Fib}(1)=1\text{ as base case 2,}]
    For all integers&#xA0;  n > 1 , &#xA0;  &#xA0;Fib  ( n ) :=  Fib  ( n
&#x2212; 1 ) +  Fib  ( n &#x2212; 2 ) .   {\displaystyle {\text{For all
integers }}n>1,~{\text{ Fib}}(n):={\text{Fib}}(n-1)+{\text{Fib}}(n-2).}  [\text
{For all integers }n>1,~\text{ Fib}(n):=\text{Fib}(n-1) + \text{Fib}(n-2).]
Many mathematical axioms are based upon recursive rules. For example, the
formal definition of the natural_numbers by the Peano_axioms can be described
as: 0 is a natural number, and each natural number has a successor, which is
also a natural number. By this base case and recursive rule, one can generate
the set of all natural numbers.
Recursively defined mathematical objects include functions, sets, and
especially fractals.
There are various more tongue-in-cheek "definitions" of recursion; see
recursive_humor.
***** Informal definition *****
Recently refreshed sourdough, bubbling through fermentation: the recipe calls
for some sourdough left over from the last time the same recipe was made.
Recursion is the process a procedure goes through when one of the steps of the
procedure involves invoking the procedure itself. A procedure that goes through
recursion is said to be 'recursive'.
To understand recursion, one must recognize the distinction between a procedure
and the running of a procedure. A procedure is a set of steps based on a set of
rules. The running of a procedure involves actually following the rules and
performing the steps. An analogy: a procedure is like a written recipe; running
a procedure is like actually preparing the meal.
Recursion is related to, but not the same as, a reference within the
specification of a procedure to the execution of some other procedure. For
instance, a recipe might refer to cooking vegetables, which is another
procedure that in turn requires heating water, and so forth. However, a
recursive procedure is where (at least) one of its steps calls for a new
instance of the very same procedure, like a sourdough recipe calling for some
dough left over from the last time the same recipe was made. This immediately
creates the possibility of an endless loop; recursion can only be properly used
in a definition if the step in question is skipped in certain cases so that the
procedure can complete, like a sourdough recipe that also tells you how to get
some starter dough in case you've never made it before. Even if properly
defined, a recursive procedure is not easy for humans to perform, as it
requires distinguishing the new from the old (partially executed) invocation of
the procedure; this requires some administration of how far various
simultaneous instances of the procedures have progressed. For this reason
recursive definitions are very rare in everyday situations. An example could be
the following procedure to find a way through a maze. Proceed forward until
reaching either an exit or a branching point (a dead end is considered a
branching point with 0 branches). If the point reached is an exit, terminate.
Otherwise try each branch in turn, using the procedure recursively; if every
trial fails by reaching only dead ends, return on the path that led to this
branching point and report failure. Whether this actually defines a terminating
procedure depends on the nature of the maze: it must not allow loops. In any
case, executing the procedure requires carefully recording all currently
explored branching points, and which of their branches have already been
exhaustively tried.
***** In language *****
Linguist Noam_Chomsky among many others has argued that the lack of an upper
bound on the number of grammatical sentences in a language, and the lack of an
upper bound on grammatical sentence length (beyond practical constraints such
as the time available to utter one), can be explained as the consequence of
recursion in natural language.[1][2] This can be understood in terms of a
recursive definition of a syntactic category, such as a sentence. A sentence
can have a structure in which what follows the verb is another sentence:
Dorothy thinks witches are dangerous, in which the sentence witches are
dangerous occurs in the larger one. So a sentence can be defined recursively
(very roughly) as something with a structure that includes a noun phrase, a
verb, and optionally another sentence. This is really just a special case of
the mathematical definition of recursion.
This provides a way of understanding the creativity of languageâthe unbounded
number of grammatical sentencesâbecause it immediately predicts that
sentences can be of arbitrary length: Dorothy thinks that Toto suspects that
Tin Man said that.... There are many structures apart from sentences that can
be defined recursively, and therefore many ways in which a sentence can embed
instances of one category inside another. Over the years, languages in general
have proved amenable to this kind of analysis.
Recently, however, the generally accepted idea that recursion is an essential
property of human language has been challenged by Daniel_Everett on the basis
of his claims about the PirahÃ£_language. Andrew Nevins, David Pesetsky and
Cilene Rodrigues are among many who have argued against this.[3] Literary self-
reference can in any case be argued to be different in kind from mathematical
or logical recursion.[4]
Recursion plays a crucial role not only in syntax, but also in natural_language
semantics. The word and, for example, can be construed as a function that can
apply to sentence meanings to create new sentences, and likewise for noun
phrase meanings, verb phrase meanings, and others. It can also apply to
intransitive verbs, transitive verbs, or ditransitive verbs. In order to
provide a single denotation for it that is suitably flexible, and is typically
defined so that it can take any of these different types of meanings as
arguments. This can be done by defining it for a simple case in which it
combines sentences, and then defining the other cases recursively in terms of
the simple one.[5]
A recursive_grammar is a formal grammar that contains recursive production
rules.[6]
**** Recursive humor ****
Recursion is sometimes used humorously in computer science, programming,
philosophy, or mathematics textbooks, generally by giving a circular_definition
or self-reference, in which the putative recursive step does not get closer to
a base case, but instead leads to an infinite_regress. It is not unusual for
such books to include a joke entry in their glossary along the lines of:
      Recursion, see Recursion.[7]
A variation is found on page 269 in the index of some editions of Brian
Kernighan and Dennis_Ritchie's book The_C_Programming_Language; the index entry
recursively references itself ("recursion 86, 139, 141, 182, 202, 269"). Early
versions of this joke can be fund in "Let's talk Lisp" by Laurent SiklÃ³ssy
(published by Prentice Hall PTR on December, 1, 1975 with a copyright date of
1976) and in "Software Tools" by Kernighan and Plauger (published by Addison-
Wesley Professional on January, 11, 1976). The joke also appears in "The UNIX
Programming Environment" by Kernighan and Pike. It did not appear in the first
edition of The C Programming Language. The joke is part of the Functional
programming folklore and was already widespread in the functional programming
community before the publication of the afore-mentioned books.
Another joke is that "To understand recursion, you must understand recursion."
[7] In the English-language version of the Google web search engine, when a
search for "recursion" is made, the site suggests "Did you mean: recursion." An
alternative form is the following, from Andrew_Plotkin: "If you already know
what recursion is, just remember the answer. Otherwise, find someone who is
standing closer to Douglas_Hofstadter than you are; then ask him or her what
recursion is."
Recursive_acronyms are other examples of recursive humor. PHP, for example,
stands for "PHP Hypertext Preprocessor", WINE stands for "WINE Is Not an
Emulator" GNU stands for "GNU's not Unix", and SPARQL denotes the "SPARQL
Protocol and RDF Query Language".
***** In mathematics *****
The Sierpinski_triangleâa confined recursion of triangles that form a fractal
**** Recursively defined sets ****
Main article: Recursive_definition
*** Example: the natural numbers ***
See also: Closure_(mathematics)
The canonical example of a recursively defined set is given by the natural
numbers:
      0 is in      N    {\displaystyle \mathbb {N} }  [\mathbb {N} ]
      if n is in      N    {\displaystyle \mathbb {N} }  [\mathbb {N} ], then n
      + 1 is in      N    {\displaystyle \mathbb {N} }  [\mathbb {N} ]
      The set of natural numbers is the smallest set satisfying the previous
      two properties.
In mathematical logic, the Peano_axioms (or Peano postulates or
DedekindâPeano axioms), are axioms for the natural numbers presented in the
19th century by the German mathematician Richard_Dedekind and by the Italian
mathematician Giuseppe_Peano. The Peano Axioms define the natural numbers
referring to a recursive successor function and addition and multiplication as
recursive functions.
*** Example: Proof procedure ***
Another interesting example is the set of all "provable" propositions in an
axiomatic_system that are defined in terms of a prof_procedure which is
inductively (or recursively) defined as follows:
    * If a proposition is an axiom, it is a provable proposition.
    * If a proposition can be derived from true reachable propositions by means
      of inference rules, it is a provable proposition.
    * The set of provable propositions is the smallest set of propositions
      satisfying these conditions.
**** Finite subdivision rules ****
Main article: Finite_subdivision_rule
Finite subdivision rules are a geometric form of recursion, which can be used
to create fractal-like images. A subdivision rule starts with a collection of
polygons labelled by finitely many labels, and then each polygon is subdivided
into smaller labelled polygons in a way that depends only on the labels of the
original polygon. This process can be iterated. The standard `middle thirds'
technique for creating the Cantor_set is a subdivision rule, as is barycentric
subdivision.
**** Functional recursion ****
A function may be recursively defined in terms of itself. A familiar example is
the Fibonacci_number sequence: F(n) = F(n â 1) + F(n â 2). For such a
definition to be useful, it must lead to non-recursively defined values, in
this case F(0) = 0 and F(1) = 1.
A famous recursive function is the Ackermann_function, which, unlike the
Fibonacci sequence, cannot be expressed without recursion.
**** Proofs involving recursive definitions ****
Applying the standard technique of proof_by_cases to recursively defined sets
or functions, as in the preceding sections, yields structural_induction, a
powerful generalization of mathematical_induction widely used to derive proofs
in mathematical_logic and computer science.
**** Recursive optimization ****
Dynamic_programming is an approach to optimization that restates a multiperiod
or multistep optimization problem in recursive form. The key result in dynamic
programming is the Bellman_equation, which writes the value of the optimization
problem at an earlier time (or earlier step) in terms of its value at a later
time (or later step).
**** The recursion theorem ****
In set_theory, this is a theorem guaranteeing that recursively defined
functions exist. Given a set X, an element a of X and a function     f : X
&#x2192; X   {\displaystyle f:X\rightarrow X}  [f: X \rightarrow X], the
theorem states that there is a unique function     F :  N  &#x2192; X
{\displaystyle F:\mathbb {N} \rightarrow X}  [F: \mathbb{N} \rightarrow X]
(where      N    {\displaystyle \mathbb {N} }  [\mathbb {N} ] denotes the set
of natural numbers including zero) such that
         F ( 0 ) = a   {\displaystyle F(0)=a}  [F(0) = a]
         F ( n + 1 ) = f ( F ( n ) )   {\displaystyle F(n+1)=f(F(n))}  [F(n +
      1) = f(F(n))]
for any natural number n.
*** Proof of uniqueness ***
Take two functions     F :  N  &#x2192; X   {\displaystyle F:\mathbb {N}
\rightarrow X}  [F: \mathbb{N} \rightarrow X] and     G :  N  &#x2192; X
{\displaystyle G:\mathbb {N} \rightarrow X}  [G: \mathbb{N} \rightarrow X] such
that:
         F ( 0 ) = a   {\displaystyle F(0)=a}  [F(0) = a]
         G ( 0 ) = a   {\displaystyle G(0)=a}  [G(0) = a]
         F ( n + 1 ) = f ( F ( n ) )   {\displaystyle F(n+1)=f(F(n))}  [F(n +
      1) = f(F(n))]
         G ( n + 1 ) = f ( G ( n ) )   {\displaystyle G(n+1)=f(G(n))}  [G(n +
      1) = f(G(n))]
where a is an element of X.
It can be proved by mathematical_induction that     F ( n ) = G ( n )
{\displaystyle F(n)=G(n)}  [F(n) = G(n)] for all natural numbers n:
      Base Case:     F ( 0 ) = a = G ( 0 )   {\displaystyle F(0)=a=G(0)}  [F(0)
      = a = G(0)] so the equality holds for     n = 0   {\displaystyle n=0}
      [n=0].
      Inductive Step: Suppose     F ( k ) = G ( k )   {\displaystyle F(k)=G(k)}
      [F(k) = G(k)] for some     k &#x2208;  N    {\displaystyle k\in \mathbb
      {N} }  [k\in \mathbb {N} ]. Then     F ( k + 1 ) = f ( F ( k ) ) = f ( G
      ( k ) ) = G ( k + 1 ) .   {\displaystyle F(k+1)=f(F(k))=f(G(k))=G(k+1).}
      [F(k+1) = f(F(k)) = f(G(k)) = G(k+1).]
            Hence F(k) = G(k) implies F(k+1) = G(k+1).
By induction,     F ( n ) = G ( n )   {\displaystyle F(n)=G(n)}  [F(n) = G(n)]
for all     n &#x2208;  N    {\displaystyle n\in \mathbb {N} }  [n\in \mathbb
{N} ].
***** In computer science *****
Main article: Recursion_(computer_science)
A common method of simplification is to divide a problem into subproblems of
the same type. As a computer_programming technique, this is called divide_and
conquer and is key to the design of many important algorithms. Divide and
conquer serves as a top-down approach to problem solving, where problems are
solved by solving smaller and smaller instances. A contrary approach is dynamic
programming. This approach serves as a bottom-up approach, where problems are
solved by solving larger and larger instances, until the desired size is
reached.
A classic example of recursion is the definition of the factorial function,
given here in C code:
unsigned int factorial(unsigned int n) {
    if (n == 0) {
        return 1;
    } else {
        return n * factorial(n - 1);
    }
}
The function calls itself recursively on a smaller version of the input (n - 1)
and multiplies the result of the recursive call by n, until reaching the base
case, analogously to the mathematical definition of factorial.
Recursion in computer programming is exemplified when a function is defined in
terms of simpler, often smaller versions of itself. The solution to the problem
is then devised by combining the solutions obtained from the simpler versions
of the problem. One example application of recursion is in parsers for
programming languages. The great advantage of recursion is that an infinite set
of possible sentences, designs or other data can be defined, parsed or produced
by a finite computer program.
Recurrence_relations are equations to define one or more sequences recursively.
Some specific kinds of recurrence relation can be "solved" to obtain a non-
recursive definition.
Use of recursion in an algorithm has both advantages and disadvantages. The
main advantage is usually simplicity. The main disadvantage is that the memory
usage of recursive algorithms may grow very quickly, rendering them
impractical.
***** In art *****
Recursive dolls: the original set of Matryoshka_dolls by Zvyozdochkin and
Malyutin, 1892
Front face of Giotto's Stefaneschi_Triptych, 1320, recursively contains an
image of itself (held up by the kneeling figure in the central panel).
See also: Mathematics_and_art and Infinity_mirror
The Russian Doll or Matryoshka_Doll is a physical artistic example of the
recursive concept.[8]
Recursion has been used in paintings since Giotto's Stefaneschi_Triptych, made
in 1320. Its central panel contains the kneeling figure of Cardinal
Stefaneschi, holding up the triptych itself as an offering.[9]
M._C._Escher's Print_Gallery (1956) is a print which depicts a distorted city
which contains a gallery which recursively contains the picture, and so ad
infinitum.[10]
***** See also *****
    * Corecursion
    * Course-of-values_recursion
    * Digital_infinity
    * Fixed_point_combinator
    * Infinite_compositions_of_analytic_functions
    * Infinite_loop
    * Infinitism
    * Iterated_function
    * Mise_en_abyme
    * Reentrant_(subroutine)
    * Self-reference
    * Strange_loop
    * Tail_recursion
    * Tupper's_self-referential_formula
    * Turtles_all_the_way_down
***** References *****
   1. ^Pinker, Steven (1994). The Language Instinct. William Morrow.
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
   3. ^Pinker, Steven; Jackendoff, Ray (2005). "The faculty of language: What's
      so special about it?". Cognition. 95 (2): 201â236.
      CiteSeerX 10.1.1.116.7784. doi:10.1016/j.cognition.2004.08.004.
      PMID 15694646.
   4. ^Nevins, Andrew; Pesetsky, David; Rodrigues, Cilene (2009). "Evidence_and
      argumentation:_A_reply_to_Everett_(2009)" (PDF). Language. 85 (3):
      671â681. doi:10.1353/lan.0.0140. Archived from the_original (PDF) on
      2012-01-06.
   5. ^Drucker, Thomas (4 January 2008). Perspectives_on_the_History_of
      Mathematical_Logic. Springer Science & Business Media. p. 110. ISBN 978-
      0-8176-4768-1.
   6. ^ Barbara Partee and Mats Rooth. 1983. In Rainer BÃ¤uerle et al.,
      Meaning, Use, and Interpretation of Language. Reprinted in Paul Portner
      and Barbara Partee, eds. 2002. Formal Semantics: The Essential Readings.
      Blackwell.
   7. ^Nederhof, Mark-Jan; Satta, Giorgio (2002), "Parsing Non-recursive
      Context-free Grammars", Proceedings of the 40th Annual Meeting on
      Association for Computational Linguistics (ACL '02), Stroudsburg, PA,
      USA: Association for Computational Linguistics, pp. 112â119, doi:
      10.3115/1073083.1073104
   8. .
   9. ^ a bHunter, David (2011). Essentials_of_Discrete_Mathematics. Jones and
      Bartlett. p. 494. ISBN 9781449604424.
  10. ^Tang, Daisy. "Recursion". Retrieved 24 September 2015. More examples of
      recursion: Russian Matryoshka dolls. Each doll is made of solid wood or
      is hollow and contains another Matryoshka doll inside it.
  11. ^"Giotto_di_Bondone_and_assistants:_Stefaneschi_triptych". The Vatican.
      Retrieved 16 September 2015.
  12. ^Cooper, Jonathan (5 September 2007). "Art_and_Mathematics". Retrieved 5
      September 2015.
***** Bibliography *****
    * Dijkstra,_Edsger_W. (1960). "Recursive Programming". Numerische
      Mathematik. 2 (1): 312â318. doi:10.1007/BF01386232.
Johnsonbaugh,_Richard (2004). Discrete Mathematics. Prentice Hall. ISBN 978-0-
13-117686-7.
Hofstadter,_Douglas (1999). GÃ¶del, Escher, Bach: an Eternal Golden Braid.
Basic Books. ISBN 978-0-465-02656-2.
Shoenfield,_Joseph_R. (2000). Recursion Theory. A K Peters Ltd. ISBN 978-1-
56881-149-9.
Causey, Robert L. (2001). Logic, Sets, and Recursion. Jones & Bartlett.
ISBN 978-0-7637-1695-0.
Cori, Rene; Lascar, Daniel; Pelletier, Donald H. (2001). Recursion Theory,
GÃ¶del's Theorems, Set Theory, Model Theory. Oxford University Press. ISBN 978-
0-19-850050-6.
Barwise,_Jon; Moss, Lawrence S. (1996). Vicious Circles. Stanford Univ Center
for the Study of Language and Information. ISBN 978-0-19-850050-6.
 - offers a treatment of corecursion.
Rosen, Kenneth H. (2002). Discrete Mathematics and Its Applications. McGraw-
Hill College. ISBN 978-0-07-293033-7.
Cormen, Thomas H., Charles E. Leiserson, Ronald L. Rivest, Clifford Stein
(2001). Introduction to Algorithms. Mit Pr. ISBN 978-0-262-03293-3.CS1 maint:
Multiple names: authors list (link)
Kernighan, B.; Ritchie, D. (1988). The C programming Language. Prentice Hall.
ISBN 978-0-13-110362-7.
Stokey, Nancy; Robert Lucas; Edward Prescott (1989). Recursive Methods in
Economic Dynamics. Harvard University Press. ISBN 978-0-674-75096-8.
Hungerford (1980). Algebra. Springer. ISBN 978-0-387-90518-1.
, first chapter on set theory.
***** External links *****
 Wikimedia Commons has media related to Recursion.
 Look up recursion or recursivity in Wiktionary, the free dictionary.
    * Recursion - tutorial by Alan Gauld
    * Zip_Files_All_The_Way_Down
    * Nevins,_Andrew_and_David_Pesetsky_and_Cilene_Rodrigues._Evidence_and
      Argumentation:_A_Reply_to_Everett_(2009)._Language_85.3:_671--681_(2009)
    * v
    * t
    * e
Fractals
                         * Fractal_dimensions
                               o Assouad
                               o Box-counting
                               o Correlation
Characteristics                o Hausdorff
                               o Packing
                               o Topological
                         * Recursion
                         * Self-similarity
                         * Barnsley_fern
                         * Cantor_set
                         * Koch_snowflake
                         * Menger_sponge
                         * Sierpinski_carpet
                         * Sierpinski_triangle
                         * Space-filling_curve
Iterated_function_             o Blancmange_curve
system                         o De_Rham_curve
                               o Dragon_curve
                               o Koch_curve
                               o LÃ©vy_C_curve
                               o Peano_curve
                               o SierpiÅski_curve
                         * T-square
                         * n-flake
Strange_attractor        * Multifractal_system
                         * Fractal_canopy
L-system                 * Space-filling_curve
                               o H_tree
                         * Burning_Ship_fractal
                         * Julia_set
                               o Filled
Escape-time_             * Lyapunov_fractal
fractals                 * Mandelbrot_set
                         * Newton_fractal            [Partial_view_of_the
                         * Tricorn                   Mandelbrot_set.]
                         * Mandelbox
                         * Mandelbulb
                         * Buddhabrot
Rendering techniques     * Orbit_trap
                         * Pickover_stalk
                         * Brownian_motion
                               o Brownian_tree
Random fractals          * Fractal_landscape
                         * LÃ©vy_flight
                         * Percolation_theory
                         * Self-avoiding_walk
                         * Georg_Cantor
                         * Felix_Hausdorff
                         * Gaston_Julia
                         * Helge_von_Koch
People                   * Paul_LÃ©vy
                         * Aleksandr_Lyapunov
                         * Benoit_Mandelbrot
                         * Lewis_Fry_Richardson
                         * WacÅaw_SierpiÅski
                         * "How_Long_Is_the_Coast_of
                           Britain?"
                               o Coastline_paradox
                         * List_of_fractals_by
                           Hausdorff_dimension
                         * The_Beauty_of_Fractals
Other                      (1986 book)
                         * Fractal_art
                         * Chaos:_Making_a_New
                           Science (1987 book)
                         * The_Fractal_Geometry_of
                           Nature (1982 book)
                         * Kaleidoscope
                         * Chaos_theory
    * v
    * t
    * e
Mathematical_logic
                           * Formal_language
                           * Formation_rule
                           * Formal_proof
                           * Formal_semantics
                           * Well-formed_formula
                           * Set
                           * Element
                           * Class
General                    * Classical_logic
                           * Axiom
                           * Rule_of_inference
                           * Relation
                           * Theorem
                           * Logical_consequence
                           * Type_theory
                           * Symbol
                           * Syntax
                           * Theory
                           * Formal_system
                           * Deductive_system
Systems                    * Axiomatic_system
                           * Hilbert_style_systems
                           * Natural_deduction
                           * Sequent_calculus
                           * Proposition
                           * Inference
                           * Argument
Traditional_logic          * Validity
                           * Cogency
                           * Syllogism
                           * Square_of_opposition
                           * Venn_diagram
                           * Boolean_functions
                           * Propositional_calculus
Propositional_calculus     * Propositional_formula
and Boolean_logic          * Logical_connectives
                           * Truth_tables
                           * Many-valued_logic
                           * First-order
                           * Quantifiers
Predicate_logic            * Predicate
                           * Second-order
                           * Monadic_predicate_calculus
                           * Set
                           * Empty_set
                           * Element
                           * Enumeration
                           * Extensionality
                           * Finite_set
                           * Infinite_set
                           * Subset
                           * Power_set
Naive_set_theory           * Countable_set
                           * Uncountable_set
                           * Recursive_set
                           * Domain
                           * Codomain
                           * Image
                           * Map
                           * Function
                           * Relation
                           * Ordered_pair
                           * Foundations_of_mathematics
                           * ZermeloâFraenkel_set_theory
                           * Axiom_of_choice
Set_theory                 * General_set_theory
                           * KripkeâPlatek_set_theory
                           * Von_NeumannâBernaysâGÃ¶del_set_theory
                           * MorseâKelley_set_theory
                           * TarskiâGrothendieck_set_theory
                           * Model
                           * Interpretation
Model_theory               * Non-standard_model
                           * Finite_model_theory
                           * Truth_value
                           * Validity
                           * Formal_proof
                           * Deductive_system
                           * Formal_system
Proof_theory               * Theorem
                           * Logical_consequence
                           * Rule_of_inference
                           * Syntax
                           * Recursion
                           * Recursive_set
Computability_             * Recursively_enumerable_set
theory                     * Decision_problem
                           * ChurchâTuring_thesis
                           * Computable_function
                           * Primitive_recursive_function

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Recursion&oldid=901212161"
Categories:
    * Theory_of_computation
    * Recursion
    * Self-reference
    * Feedback
Hidden categories:
    * Wikipedia_pages_semi-protected_against_vandalism
    * Articles_needing_additional_references_from_June_2012
    * All_articles_needing_additional_references
    * CS1_maint:_Multiple_names:_authors_list
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
    * View_source
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Ido
    * Bahasa_Indonesia
    * Interlingua
    * Ãslenska
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * Nederlands
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÐ¸Ð½ÑÑÐºÑÐ¹
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à¤¸à¤à¤¸à¥à¤à¥à¤¤à¤®à¥
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 10 June 2019, at 11:30 (UTC).
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
