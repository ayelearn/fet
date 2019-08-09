The following text has been accessed from https://en.wikipedia.org/wiki/Consistency at Fri Aug 9 02:53:40 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Consistency ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other uses, see Consistency_(disambiguation).
In classical deductive_logic, a consistent theory is one that does not entail a
contradiction.[1][2] The lack of contradiction can be defined in either
semantic or syntactic terms. The semantic definition states that a theory is
consistent if it has a model, i.e., there exists an interpretation under which
all formulas in the theory are true. This is the sense used in traditional
Aristotelian_logic, although in contemporary mathematical logic the term
satisfiable is used instead. The syntactic definition states a theory     T
{\displaystyle T}  [T] is consistent if there is no formula     &#x03C6;
{\displaystyle \varphi }  [\varphi ] such that both     &#x03C6;
{\displaystyle \varphi }  [\varphi ] and its negation     &#x00AC; &#x03C6;
{\displaystyle \lnot \varphi }  [{\displaystyle \lnot \varphi }] are elements
of the set of consequences of     T   {\displaystyle T}  [T]. Let     A
{\displaystyle A}  [A] be a set of closed_sentences (informally "axioms") and
&#x27E8; A &#x27E9;   {\displaystyle \langle A\rangle }  [{\displaystyle
\langle A\rangle }] the set of closed sentences provable from     A
{\displaystyle A}  [A] under some (specified, possibly implicitly) formal
deductive system. The set of axioms     A   {\displaystyle A}  [A] is
consistent when     &#x03C6; , &#x00AC; &#x03C6; &#x2208; &#x27E8; A &#x27E9;
{\displaystyle \varphi ,\lnot \varphi \in \langle A\rangle }  [{\displaystyle
\varphi ,\lnot \varphi \in \langle A\rangle }] for no formula     &#x03C6;
{\displaystyle \varphi }  [\varphi ].[3]
If there exists a deductive system for which these semantic and syntactic
definitions are equivalent for any theory formulated in a particular deductive
logic, the logic is called complete.[citation_needed] The completeness of the
sentential_calculus was proved by Paul_Bernays in 1918[citation_needed][4] and
Emil_Post in 1921,[5] while the completeness of predicate_calculus was proved
by Kurt_GÃ¶del in 1930,[6] and consistency proofs for arithmetics restricted
with respect to the induction_axiom_schema were proved by Ackermann (1924), von
Neumann (1927) and Herbrand (1931).[7] Stronger logics, such as second-order
logic, are not complete.
A consistency proof is a mathematical_proof that a particular theory is
consistent.[8] The early development of mathematical proof_theory was driven by
the desire to provide finitary consistency proofs for all of mathematics as
part of Hilbert's_program. Hilbert's program was strongly impacted by
incompleteness_theorems, which showed that sufficiently strong proof theories
cannot prove their own consistency (provided that they are in fact consistent).
Although consistency can be proved by means of model theory, it is often done
in a purely syntactical way, without any need to reference some model of the
logic. The cut-elimination (or equivalently the normalization of the underlying
calculus if there is one) implies the consistency of the calculus: since there
is no cut-free proof of falsity, there is no contradiction in general.
⁰
***** Contents *****
    * 1_Consistency_and_completeness_in_arithmetic_and_set_theory
    * 2_First-order_logic
          o 2.1_Notation
          o 2.2_Definition
          o 2.3_Basic_results
          o 2.4_Henkin's_theorem
          o 2.5_Sketch_of_proof
    * 3_Model_theory
    * 4_See_also
    * 5_Footnotes
    * 6_References
    * 7_External_links
***** Consistency and completeness in arithmetic and set theory[edit] *****
In theories of arithmetic, such as Peano_arithmetic, there is an intricate
relationship between the consistency of the theory and its completeness. A
theory is complete if, for every formula Ï in its language, at least one of Ï
or Â¬Ï is a logical consequence of the theory.
Presburger_arithmetic is an axiom system for the natural numbers under
addition. It is both consistent and complete.
GÃ¶del's_incompleteness_theorems show that any sufficiently strong recursively
enumerable theory of arithmetic cannot be both complete and consistent.
GÃ¶del's theorem applies to the theories of Peano_arithmetic (PA) and primitive
recursive_arithmetic (PRA), but not to Presburger_arithmetic.
Moreover, GÃ¶del's second incompleteness theorem shows that the consistency of
sufficiently strong recursively enumerable theories of arithmetic can be tested
in a particular way. Such a theory is consistent if and only if it does not
prove a particular sentence, called the GÃ¶del sentence of the theory, which is
a formalized statement of the claim that the theory is indeed consistent. Thus
the consistency of a sufficiently strong, recursively enumerable, consistent
theory of arithmetic can never be proven in that system itself. The same result
is true for recursively enumerable theories that can describe a strong enough
fragment of arithmetic—including set theories such as ZermeloâFraenkel_set
theory. These set theories cannot prove their own GÃ¶del sentenceâprovided
that they are consistent, which is generally believed.
Because consistency of ZF is not provable in ZF, the weaker notion relative
consistency is interesting in set theory (and in other sufficiently expressive
axiomatic systems). If T is a theory and A is an additional axiom, T + A is
said to be consistent relative to T (or simply that A is consistent with T) if
it can be proved that if T is consistent then T + A is consistent. If both A
and Â¬A are consistent with T, then A is said to be independent of T.
***** First-order logic[edit] *****
**** Notation[edit] ****
   &#x22A2;   {\displaystyle \vdash }  [\vdash ] (Turnstile symbol) in the
following context of mathematical_logic, means "provable from". That is,     a
&#x22A2; b   {\displaystyle a\vdash b}  [{\displaystyle a\vdash b}] reads: b is
provable from a (in some specified formal system). See List_of_logic_symbols.
In other cases, the turnstile symbol may mean implies; permits the derivation
of. See: List_of_mathematical_symbols.
**** Definition[edit] ****
    * A set of formulas     &#x03A6;   {\displaystyle \Phi }  [\Phi ] in first-
      order logic is consistent (written     Con &#x2061; &#x03A6;
      {\displaystyle \operatorname {Con} \Phi }  [{\displaystyle \operatorname
      {Con} \Phi }]) if there is no formula     &#x03C6;   {\displaystyle
      \varphi }  [\varphi ] such that     &#x03A6; &#x22A2; &#x03C6;
      {\displaystyle \Phi \vdash \varphi }  [{\displaystyle \Phi \vdash \varphi
      }] and     &#x03A6; &#x22A2; &#x00AC; &#x03C6;   {\displaystyle \Phi
      \vdash \lnot \varphi }  [{\displaystyle \Phi \vdash \lnot \varphi }].
      Otherwise     &#x03A6;   {\displaystyle \Phi }  [\Phi ] is inconsistent
      (written     Inc &#x2061; &#x03A6;   {\displaystyle \operatorname {Inc}
      \Phi }  [{\displaystyle \operatorname {Inc} \Phi }]).
    *    &#x03A6;   {\displaystyle \Phi }  [\Phi ] is said to be simply
      consistent if for no formula     &#x03C6;   {\displaystyle \varphi }
      [\varphi ] of     &#x03A6;   {\displaystyle \Phi }  [\Phi ], both
      &#x03C6;   {\displaystyle \varphi }  [\varphi ] and the negation of
      &#x03C6;   {\displaystyle \varphi }  [\varphi ] are theorems of
      &#x03A6;   {\displaystyle \Phi }  [\Phi ].[clarification_needed]
    *    &#x03A6;   {\displaystyle \Phi }  [\Phi ] is said to be absolutely
      consistent or Post consistent if at least one formula in the language of
      &#x03A6;   {\displaystyle \Phi }  [\Phi ] is not a theorem of
      &#x03A6;   {\displaystyle \Phi }  [\Phi ].
    *    &#x03A6;   {\displaystyle \Phi }  [\Phi ] is said to be maximally
      consistent if for every formula     &#x03C6;   {\displaystyle \varphi }
      [\varphi ], if     Con &#x2061; ( &#x03A6; &#x222A; &#x03C6; )
      {\displaystyle \operatorname {Con} (\Phi \cup \varphi )}  [{\displaystyle
      \operatorname {Con} (\Phi \cup \varphi )}] implies     &#x03C6; &#x2208;
      &#x03A6;   {\displaystyle \varphi \in \Phi }  [{\displaystyle \varphi \in
      \Phi }].
    *    &#x03A6;   {\displaystyle \Phi }  [\Phi ] is said to contain witnesses
      if for every formula of the form     &#x2203; x  &#x03C6;
      {\displaystyle \exists x\,\varphi }  [{\displaystyle \exists x\,\varphi
      }] there exists a term     t   {\displaystyle t}  [t] such that
      ( &#x2203; x  &#x03C6; &#x2192; &#x03C6;   t x   ) &#x2208; &#x03A6;
      {\displaystyle (\exists x\,\varphi \to \varphi {t \over x})\in \Phi }  [
      {\displaystyle (\exists x\,\varphi \to \varphi {t \over x})\in \Phi }],
      where     &#x03C6;   t x     {\displaystyle \varphi {t \over x}}  [
      {\displaystyle \varphi {t \over x}}] denotes the substitution of each
      x   {\displaystyle x}  [x] in     &#x03C6;   {\displaystyle \varphi }
      [\varphi ] by a     t   {\displaystyle t}  [t]; see also First-order
      logic.[citation_needed]
**** Basic results[edit] ****
   1. The following are equivalent:
         1.    Inc &#x2061; &#x03A6;   {\displaystyle \operatorname {Inc} \Phi
            }  [{\displaystyle \operatorname {Inc} \Phi }]
         2. For all     &#x03C6; ,  &#x03A6; &#x22A2; &#x03C6; .
            {\displaystyle \varphi ,\;\Phi \vdash \varphi .}  [{\displaystyle
            \varphi ,\;\Phi \vdash \varphi .}]
   2. Every satisfiable set of formulas is consistent, where a set of formulas
      &#x03A6;   {\displaystyle \Phi }  [\Phi ] is satisfiable if and only if
      there exists a model       I     {\displaystyle {\mathfrak {I}}}  [
      {\mathfrak {I}}] such that       I   &#x22A8; &#x03A6;   {\displaystyle
      {\mathfrak {I}}\vDash \Phi }  [\mathfrak{I} \vDash \Phi ].
   3. For all     &#x03A6;   {\displaystyle \Phi }  [\Phi ] and     &#x03C6;
      {\displaystyle \varphi }  [\varphi ]:
         1. if not     &#x03A6; &#x22A2; &#x03C6;   {\displaystyle \Phi \vdash
            \varphi }  [{\displaystyle \Phi \vdash \varphi }], then     Con
            &#x2061;  (  &#x03A6; &#x222A; { &#x00AC; &#x03C6; }  )
            {\displaystyle \operatorname {Con} \left(\Phi \cup \{\lnot \varphi
            \}\right)}  [{\displaystyle \operatorname {Con} \left(\Phi \cup \
            {\lnot \varphi \}\right)}];
         2. if     Con &#x2061; &#x03A6;   {\displaystyle \operatorname {Con}
            \Phi }  [{\displaystyle \operatorname {Con} \Phi }] and
            &#x03A6; &#x22A2; &#x03C6;   {\displaystyle \Phi \vdash \varphi }
            [{\displaystyle \Phi \vdash \varphi }], then     Con &#x2061;
            (  &#x03A6; &#x222A; { &#x03C6; }  )    {\displaystyle
            \operatorname {Con} \left(\Phi \cup \{\varphi \}\right)}  [
            {\displaystyle \operatorname {Con} \left(\Phi \cup \{\varphi
            \}\right)}];
         3. if     Con &#x2061; &#x03A6;   {\displaystyle \operatorname {Con}
            \Phi }  [{\displaystyle \operatorname {Con} \Phi }], then     Con
            &#x2061;  (  &#x03A6; &#x222A; { &#x03C6; }  )    {\displaystyle
            \operatorname {Con} \left(\Phi \cup \{\varphi \}\right)}  [
            {\displaystyle \operatorname {Con} \left(\Phi \cup \{\varphi
            \}\right)}] or     Con &#x2061;  (  &#x03A6; &#x222A; { &#x00AC;
            &#x03C6; }  )    {\displaystyle \operatorname {Con} \left(\Phi \cup
            \{\lnot \varphi \}\right)}  [{\displaystyle \operatorname {Con}
            \left(\Phi \cup \{\lnot \varphi \}\right)}].
   4. Let     &#x03A6;   {\displaystyle \Phi }  [\Phi ] be a maximally
      consistent set of formulas and suppose it contains witnesses. For all
      &#x03C6;   {\displaystyle \varphi }  [\varphi ] and     &#x03C8;
      {\displaystyle \psi }  [\psi ]:
         1. if     &#x03A6; &#x22A2; &#x03C6;   {\displaystyle \Phi \vdash
            \varphi }  [{\displaystyle \Phi \vdash \varphi }], then
            &#x03C6; &#x2208; &#x03A6;   {\displaystyle \varphi \in \Phi }  [
            {\displaystyle \varphi \in \Phi }],
         2. either     &#x03C6; &#x2208; &#x03A6;   {\displaystyle \varphi \in
            \Phi }  [{\displaystyle \varphi \in \Phi }] or     &#x00AC;
            &#x03C6; &#x2208; &#x03A6;   {\displaystyle \lnot \varphi \in \Phi
            }  [{\displaystyle \lnot \varphi \in \Phi }],
         3.    ( &#x03C6; &#x2228; &#x03C8; ) &#x2208; &#x03A6;
            {\displaystyle (\varphi \lor \psi )\in \Phi }  [{\displaystyle
            (\varphi \lor \psi )\in \Phi }] if and only if     &#x03C6;
            &#x2208; &#x03A6;   {\displaystyle \varphi \in \Phi }  [
            {\displaystyle \varphi \in \Phi }] or     &#x03C8; &#x2208;
            &#x03A6;   {\displaystyle \psi \in \Phi }  [\psi \in \Phi],
         4. if     ( &#x03C6; &#x2192; &#x03C8; ) &#x2208; &#x03A6;
            {\displaystyle (\varphi \to \psi )\in \Phi }  [{\displaystyle
            (\varphi \to \psi )\in \Phi }] and     &#x03C6; &#x2208; &#x03A6;
            {\displaystyle \varphi \in \Phi }  [{\displaystyle \varphi \in \Phi
            }], then     &#x03C8; &#x2208; &#x03A6;   {\displaystyle \psi \in
            \Phi }  [\psi \in \Phi],
         5.    &#x2203; x  &#x03C6; &#x2208; &#x03A6;   {\displaystyle \exists
            x\,\varphi \in \Phi }  [{\displaystyle \exists x\,\varphi \in \Phi
            }] if and only if there is a term     t   {\displaystyle t}  [t]
            such that     &#x03C6;   t x   &#x2208; &#x03A6;   {\displaystyle
            \varphi {t \over x}\in \Phi }  [{\displaystyle \varphi {t \over
            x}\in \Phi }].[citation_needed]
**** Henkin's theorem[edit] ****
Let     S   {\displaystyle S}  [S] be a symbol_set. Let     &#x03A6;
{\displaystyle \Phi }  [\Phi ] be a maximally consistent set of     S
{\displaystyle S}  [S]-formulas containing witnesses.
Define an equivalence relation     &#x223C;   {\displaystyle \sim }  [\sim ] on
the set of     S   {\displaystyle S}  [S]-terms by      t  0   &#x223C;  t  1
{\displaystyle t_{0}\sim t_{1}}  [t_0 \sim t_1] if       t  0   &#x2261;  t  1
&#x2208; &#x03A6;   {\displaystyle \;t_{0}\equiv t_{1}\in \Phi }  [\; t_0
\equiv t_1 \in \Phi], where     &#x2261;   {\displaystyle \equiv }  [\equiv ]
denotes equality. Let       t &#x00AF;     {\displaystyle {\overline {t}}}  [
{\displaystyle {\overline {t}}}] denote the equivalence class of terms
containing     t   {\displaystyle t}  [t]; and let      T  &#x03A6;   := {    t
&#x00AF;   &#x2223; t &#x2208;  T  S   }   {\displaystyle T_{\Phi }:=\{\;
{\overline {t}}\mid t\in T^{S}\}}  [{\displaystyle T_{\Phi }:=\{\;{\overline
{t}}\mid t\in T^{S}\}}] where      T  S     {\displaystyle T^{S}}  [
{\displaystyle T^{S}}] is the set of terms based on the symbol set     S
{\displaystyle S}  [S ].
Define the     S   {\displaystyle S}  [S]-structure        T    &#x03A6;
{\displaystyle {\mathfrak {T}}_{\Phi }}  [{\displaystyle {\mathfrak {T}}_{\Phi
}}] over      T  &#x03A6;     {\displaystyle T_{\Phi }}  [{\displaystyle T_
{\Phi }}], also called the term-structure corresponding to     &#x03A6;
{\displaystyle \Phi }  [\Phi ], by:
   1. for each     n   {\displaystyle n}  [n]-ary relation symbol     R
      &#x2208; S   {\displaystyle R\in S}  [R \in S], define      R     T
      &#x03A6;        t  0   &#x00AF;   &#x2026;    t  n &#x2212; 1   &#x00AF;
      {\displaystyle R^{{\mathfrak {T}}_{\Phi }}{\overline {t_{0}}}\ldots
      {\overline {t_{n-1}}}}  [{\displaystyle R^{{\mathfrak {T}}_{\Phi }}
      {\overline {t_{0}}}\ldots {\overline {t_{n-1}}}}] if      R  t  0
      &#x2026;  t  n &#x2212; 1   &#x2208; &#x03A6; ;   {\displaystyle \;Rt_
      {0}\ldots t_{n-1}\in \Phi ;}  [{\displaystyle \;Rt_{0}\ldots t_{n-1}\in
      \Phi ;}][9]
   2. for each     n   {\displaystyle n}  [n]-ary function symbol     f
      &#x2208; S   {\displaystyle f\in S}  [f \in S], define      f     T
      &#x03A6;     (    t  0   &#x00AF;   &#x2026;    t  n &#x2212; 1
      &#x00AF;   ) :=    f  t  0   &#x2026;  t  n &#x2212; 1    &#x00AF;   ;
      {\displaystyle f^{{\mathfrak {T}}_{\Phi }}({\overline {t_{0}}}\ldots
      {\overline {t_{n-1}}}):={\overline {ft_{0}\ldots t_{n-1}}};}  [
      {\displaystyle f^{{\mathfrak {T}}_{\Phi }}({\overline {t_{0}}}\ldots
      {\overline {t_{n-1}}}):={\overline {ft_{0}\ldots t_{n-1}}};}]
   3. for each constant symbol     c &#x2208; S   {\displaystyle c\in S}  [c
      \in S], define      c     T    &#x03A6;     :=   c &#x00AF;   .
      {\displaystyle c^{{\mathfrak {T}}_{\Phi }}:={\overline {c}}.}  [
      {\displaystyle c^{{\mathfrak {T}}_{\Phi }}:={\overline {c}}.}]
Define a variable assignment      &#x03B2;  &#x03A6;     {\displaystyle \beta _
{\Phi }}  [{\displaystyle \beta _{\Phi }}] by      &#x03B2;  &#x03A6;   ( x ) :
=    x &#x00AF;      {\displaystyle \beta _{\Phi }(x):={\bar {x}}}  [
{\displaystyle \beta _{\Phi }(x):={\bar {x}}}] for each variable     x
{\displaystyle x}  [x]. Let        I    &#x03A6;   := (    T    &#x03A6;   ,
&#x03B2;  &#x03A6;   )   {\displaystyle {\mathfrak {I}}_{\Phi }:=({\mathfrak
{T}}_{\Phi },\beta _{\Phi })}  [{\displaystyle {\mathfrak {I}}_{\Phi }:=(
{\mathfrak {T}}_{\Phi },\beta _{\Phi })}] be the term interpretation associated
with     &#x03A6;   {\displaystyle \Phi }  [\Phi ].
Then for each     S   {\displaystyle S}  [S]-formula     &#x03C6;
{\displaystyle \varphi }  [\varphi ]:
      I    &#x03A6;   &#x22A8; &#x03C6;   {\displaystyle {\mathfrak {I}}_{\Phi
}\vDash \varphi }  [{\displaystyle {\mathfrak {I}}_{\Phi }\vDash \varphi }] if
 and only if      &#x03C6; &#x2208; &#x03A6; .   {\displaystyle \;\varphi \in
       \Phi .}  [{\displaystyle \;\varphi \in \Phi .}][citation_needed]
**** Sketch of proof[edit] ****
There are several things to verify. First, that     &#x223C;   {\displaystyle
\sim }  [\sim ] is in fact an equivalence_relation. Then, it needs to be
verified that (1), (2), and (3) are well defined. This falls out of the fact
that     &#x223C;   {\displaystyle \sim }  [\sim ] is an equivalence relation
and also requires a proof that (1) and (2) are independent of the choice of
t  0   , &#x2026; ,  t  n &#x2212; 1     {\displaystyle t_{0},\ldots ,t_{n-1}}
[ t_0, \ldots ,t_{n-1} ] class representatives. Finally,        I    &#x03A6;
&#x22A8; &#x03C6;   {\displaystyle {\mathfrak {I}}_{\Phi }\vDash \varphi }  [
{\displaystyle {\mathfrak {I}}_{\Phi }\vDash \varphi }] can be verified by
induction on formulas.
***** Model theory[edit] *****
In ZFC_set_theory with classical first-order_logic,[10] an inconsistent theory
T   {\displaystyle T}  [T] is one such that there exists a closed sentence
&#x03C6;   {\displaystyle \varphi }  [\varphi ] such that     T
{\displaystyle T}  [T] contains both     &#x03C6;   {\displaystyle \varphi }
[\varphi ] and its negation      &#x03C6; &#x2032;    {\displaystyle \varphi '}
[\varphi ']. A consistent theory is one such that the following logically
equivalent conditions hold
   1.    { &#x03C6; ,  &#x03C6; &#x2032;  } &#x2288; T   {\displaystyle \
      {\varphi ,\varphi '\}\not \subseteq T}  [{\displaystyle \{\varphi
      ,\varphi '\}\not \subseteq T}][11]
   2.     &#x03C6; &#x2032;  &#x2209; T &#x2228; &#x03C6; &#x2209; T
      {\displaystyle \varphi '\not \in T\lor \varphi \not \in T}  [
      {\displaystyle \varphi '\not \in T\lor \varphi \not \in T}]
***** See also[edit] *****
    * [icon]Logic_portal
 Wikiquote has quotations related to: Consistency
 Look up consistency in Wiktionary, the free dictionary.
    * Equiconsistency
    * Hilbert's_problems
    * Hilbert's_second_problem
    * Jan_Åukasiewicz
    * Paraconsistent_logic
    * Ï-consistency
    * Gentzen's_consistency_proof
    * Proof_by_contradiction
***** Footnotes[edit] *****
   1. ^ Tarski 1946 states it this way: "A deductive theory is called
      CONSISTENT or NON-CONTRADICTORY if no two asserted statements of this
      theory contradict each other, or in other words, if of any two
      contradictory sentences . . . at least one cannot be proved," (p. 135)
      where Tarski defines contradictory as follows: "With the help of the word
      not one forms the NEGATION of any sentence; two sentences, of which the
      first is a negation of the second, are called CONTRADICTORY SENTENCES"
      (p. 20). This definition requires a notion of "proof". GÃ¶del in his 1931
      defines the notion this way: "The class of provable formulas is defined
      to be the smallest class of formulas that contains the axioms and is
      closed under the relation "immediate consequence", i.e., formula c of a
      and b is defined as an immediate consequence in terms of modus ponens or
      substitution; cf GÃ¶del 1931 van Heijenoort 1967:601. Tarski defines
      "proof" informally as "statements follow one another in a definite order
      according to certain principles . . . and accompanied by considerations
      intended to establish their validity[true conclusion for all true
      premises -- Reichenbach 1947:68]" cf Tarski 1946:3. Kleene 1952 defines
      the notion with respect to either an induction or as to paraphrase) a
      finite sequence of formulas such that each formula in the sequence is
      either an axiom or an "immediate consequence" of the preceding formulas;
      "A proof is said to be a proofofits last formula, and this formula is
      said to be(formally) provableor be a(formal) theorem" cf Kleene 1952:83.
   2. ^ see Paraconsistent_logic
   3. ^
           Let     L   {\displaystyle L}  [L] be a signature,     T
           {\displaystyle T}  [T] a theory in      L  &#x221E; &#x03C9;
           {\displaystyle L_{\infty \omega }}  [{\displaystyle L_{\infty
           \omega }}] and     &#x03C6;   {\displaystyle \varphi }
           [\varphi ] a sentence in      L  &#x221E; &#x03C9;
           {\displaystyle L_{\infty \omega }}  [L_{{\infty \omega }}]. We
           say that     &#x03C6;   {\displaystyle \varphi }  [\varphi ] is
           a consequence of     T   {\displaystyle T}  [T], or that     T
           {\displaystyle T}  [T] entails     &#x03C6;   {\displaystyle
           \varphi }  [\varphi ], in symbols     T &#x22A2; &#x03C6;
           {\displaystyle T\vdash \varphi }  [T \vdash \varphi], if every
           model of     T   {\displaystyle T}  [T] is a model of
           &#x03C6;   {\displaystyle \varphi }  [\varphi ]. (In particular
           if     T   {\displaystyle T}  [T] has no models then     T
           {\displaystyle T}  [T] entails     &#x03C6;   {\displaystyle
           \varphi }  [\varphi ].)
           Warning: we don't require that if     T &#x22A2; &#x03C6;
           {\displaystyle T\vdash \varphi }  [T \vdash \varphi] then there
           is a proof of     &#x03C6;   {\displaystyle \varphi }  [\varphi
           ] from     T   {\displaystyle T}  [T]. In any case, with
           infinitary languages it's not always clear what would
           constitute a proof. Some writers use     T &#x22A2; &#x03C6;
           {\displaystyle T\vdash \varphi }  [{\displaystyle T\vdash
           \varphi }] to mean that     &#x03C6;   {\displaystyle \varphi }
           [\varphi ] is deducible from     T   {\displaystyle T}  [T] in
           some particular formal proof calculus, and they write     T
           &#x22A8; &#x03C6;   {\displaystyle T\models \varphi }  [
           {\displaystyle T\models \varphi }] for our notion of entailment
           (a notation which clashes with our     A &#x22A8; &#x03C6;
           {\displaystyle A\models \varphi }  [{\displaystyle A\models
           \varphi }]). For first-order logic the two kinds of entailment
           coincide by the completeness theorem for the proof calculus in
           question. We say that     &#x03C6;   {\displaystyle \varphi }
           [\varphi ] is valid, or is a logical theorem, in symbols
           &#x22A2; &#x03C6;   {\displaystyle \vdash \varphi }  [
           {\displaystyle \vdash \varphi }], if     &#x03C6;
           {\displaystyle \varphi }  [\varphi ] is true in every     L
           {\displaystyle L}  [L]-structure. We say that     &#x03C6;
           {\displaystyle \varphi }  [\varphi ] is consistent if
           &#x03C6;   {\displaystyle \varphi }  [\varphi ] is true in some
           L   {\displaystyle L}  [L]-structure. Likewise we say that a
           theory     T   {\displaystyle T}  [T] is consistent if it has a
           model.
           We say that two theories S and T in L infinity omega are
           equivalent if they have the same models, i.e. if Mod(S) = Mod
           (T). (Please note definition of Mod(T) on p. 30 ...)
      A Shorter Model Theory by Wilfrid Hodges, p. 37
   4. ^ van Heijenoort 1967:265 states that Bernays determined the independence
      of the axioms of Principia Mathematica, a result not published until
      1926, but he says nothing about Bernays proving their consistency.
   5. ^ Post proves both consistency and completeness of the propositional
      calculus of PM, cf van Heijenoort's commentary and Post's 1931
      Introduction to a general theory of elementary propositions in van
      Heijenoort 1967:264ff. Also Tarski 1946:134ff.
   6. ^ cf van Heijenoort's commentary and GÃ¶del's 1930 The completeness of
      the axioms of the functional calculus of logic in van Heijenoort 1967:
      582ff
   7. ^ cf van Heijenoort's commentary and Herbrand's 1930 On the consistency
      of arithmetic in van Heijenoort 1967:618ff.
   8. ^ Informally, ZermeloâFraenkel_set_theory is ordinarily assumed; some
      dialects of informal mathematics customarily assume the axiom_of_choice
      in addition.
   9. ^ This definition is indepentent of the choice of      t  i
      {\displaystyle t_{i}}  [t_{i}] due to the substitutivity properties of
      &#x2261;   {\displaystyle \equiv }  [\equiv ] and the maximal consistency
      of     &#x03A6;   {\displaystyle \Phi }  [\Phi ].
  10. ^ the common case in many applications to other areas of mathematics as
      well as the ordinary mode of reasoning of informal_mathematics in
      calculus and applications to physics, chemistry, engineering
  11. ^ according to De_Morgan's_laws
***** References[edit] *****
    * Stephen_Kleene, 1952 10th impression 1991, Introduction to
      Metamathematics, North-Holland Publishing Company, Amsterday, New York,
ISBN 0-7204-2103-9.
Hans_Reichenbach, 1947, Elements of Symbolic Logic, Dover Publications, Inc.
New York,
ISBN 0-486-24004-5,
Alfred_Tarski, 1946, Introduction to Logic and to the Methodology of Deductive
Sciences, Second Edition, Dover Publications, Inc., New York,
ISBN 0-486-28462-X.
Jean_van_Heijenoort, 1967, From Frege to GÃ¶del: A Source Book in Mathematical
Logic, Harvard University Press, Cambridge, MA,
ISBN 0-674-32449-8 (pbk.)
The_Cambridge_Dictionary_of_Philosophy, consistency
H.D. Ebbinghaus, J. Flum, W. Thomas, Mathematical Logic
Jevons, W.S., 1870, Elementary Lessons in Logic
***** External links[edit] *****
    * Chris Mortensen, Inconsistent_Mathematics, Stanford_Encyclopedia_of
      Philosophy
    * v
    * t
    * e
âLogical_truth â¤
                * truth_value
Functional:     * truth_function
                * ⊨ tautology
                * theory
Formal:         * formal_proof   [Venn1001.svg]
                * theorem
                * â¥ false
Negation       * contradiction
                * inconsistency
    * v
    * t
    * e
    * Metalogic
    * Metamathematics
    * Cantor's_theorem
    * Entscheidungsproblem
    * ChurchâTuring_thesis
    * Consistency
    * Effective_method
    * Foundations_of_mathematics
          o of_geometry
    * GÃ¶del's_completeness_theorem
    * GÃ¶del's_incompleteness_theorems
    * Soundness
    * Completeness
    * Decidability
    * Interpretation
    * LÃ¶wenheimâSkolem_theorem
    * Metatheorem
    * Satisfiability
    * Independence
    * Typeâtoken_distinction
    * Useâmention_distinction

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Consistency&oldid=896689960"
Categories:
    * Proof_theory
    * Hilbert's_problems
    * Metalogic
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2012
    * Articles_with_unsourced_statements_from_October_2009
    * Wikipedia_articles_needing_clarification_from_September_2018
    * Articles_with_unsourced_statements_from_September_2018
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
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Italiano
    * ×¢××¨××ª
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 12 May 2019, at 07:30 (UTC).
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
