The following text has been accessed from https://en.wikipedia.org/wiki/Tuple_relational_calculus at Fri Aug 9 01:11:33 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Tuple relational calculus ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Tuple calculus is a calculus that was created and introduced by Edgar_F._Codd
as part of the relational_model, in order to provide a declarative database-
query language for data manipulation in this data_model. It formed the
inspiration for the database-query languages QUEL and SQL, of which the latter,
although far less faithful to the original relational model and calculus, is
now the de facto standard database-query language; a dialect of SQL is used by
nearly every relational-database-management_system. Michel Lacroix and Alain
Pirotte proposed domain_calculus, which is closer to first-order_logic and
together with Codd showed that both of these calculi (as well as relational
algebra) are equivalent in expressive power. Subsequently, query languages for
the relational model were called relationally complete if they could express at
least all of these queries.
⁰
***** Contents *****
    * 1_Definition_of_the_calculus
          o 1.1_Relational_database
          o 1.2_Atoms
          o 1.3_Formulas
          o 1.4_Queries
    * 2_Semantic_and_syntactic_restriction_of_the_calculus
          o 2.1_Domain-independent_queries
          o 2.2_Safe_queries
    * 3_Systems
    * 4_See_also
    * 5_References
***** Definition of the calculus[edit] *****
**** Relational database[edit] ****
Since the calculus is a query language for relational_databases we first have
to define a relational database. The basic relational building block is the
domain (somewhat similar, but not equal to, a data_type). A tuple is a finite
sequence of attributes, which are ordered_pairs of domains and values. A
relation is a set of ordered pairs of domains and names; a relation serves as
the header for a relation[clarification_needed]. A relation is a set of
(compatible) tuples. Although these relational concepts are mathematically
defined, those definitions map loosely to traditional database concepts. A
table is an accepted visual representation of a relation; a tuple is similar to
the concept of a row.
We first assume the existence of a set C of column names, examples of which are
"name", "author", "address", etcetera. We define headers as finite subsets of
C. A relational database schema is defined as a tuple S = (D, R, h) where D is
the domain of atomic values (see relational_model for more on the notions of
domain and atomic value), R is a finite set of relation names, and
      h : R â 2C
a function that associates a header with each relation name in R. (Note that
this is a simplification from the full relational model where there is more
than one domain and a header is not just a set of column names but also maps
these column names to a domain.) Given a domain D we define a tuple over D as a
partial_function that maps some column names to an atomic value in D. An
example would be (name : "Harry", age : 25).
      t : C â¸ D
The set of all tuples over D is denoted as TD. The subset of C for which a
tuple t is defined is called the domain of t (not to be confused with the
domain in the schema) and denoted as dom(t).
Finally we define a relational database given a schema S = (D, R, h) as a
function
      db : R â 2TD
that maps the relation names in R to finite subsets of TD, such that for every
relation name r in R and tuple t in db(r) it holds that
      dom(t) = h(r).
The latter requirement simply says that all the tuples in a relation should
contain the same column names, namely those defined for it in the schema.
**** Atoms[edit] ****
For the construction of the formulas we will assume an infinite set V of tuple
variables. The formulas are defined given a database schema S = (D, R, h) and a
partial function type : V â¸ 2C, called at type assignment, that assigns
headers to some tuple variables. We then define the set of atomic_formulas A
[S,type] with the following rules:
   1. if v and w in V, a in type(v) and b in type(w) then the formula v.a = w.b
      is in A[S,type],
   2. if v in V, a in type(v) and k denotes a value in D then the formula v.a =
      k is in A[S,type], and
   3. if v in V, r in R and type(v) = h(r) then the formula r(v) is in A
      [S,type].
Examples of atoms are:
    * (t.age = s.age) â t has an age attribute and s has an age attribute
      with the same value
    * (t.name = "Codd") â tuple t has a name attribute and its value is
      "Codd"
    * Book(t) â tuple t is present in relation Book.
The formal semantics of such atoms is defined given a database db over S and a
tuple variable binding val : V â TD that maps tuple variables to tuples over
the domain in S:
   1. v.a = w.b is true if and only if val(v)(a) = val(w)(b)
   2. v.a = k is true if and only if val(v)(a) = k
   3. r(v) is true if and only if val(v) is in db(r)
**** Formulas[edit] ****
The atoms can be combined into formulas, as is usual in first-order logic, with
the logical operators â§ (and), â¨ (or) and Â¬ (not), and we can use the
existential quantifier (â) and the universal quantifier (â) to bind the
variables. We define the set of formulas F[S,type] inductively with the
following rules:
   1. every atom in A[S,type] is also in F[S,type]
   2. if f1 and f2 are in F[S,type] then the formula f1 â§ f2 is also in F
      [S,type]
   3. if f1 and f2 are in F[S,type] then the formula f1 â¨ f2 is also in F
      [S,type]
   4. if f is in F[S,type] then the formula Â¬ f is also in F[S,type]
   5. if v in V, H a header and f a formula in F[S,type[v->H]] then the formula
      â v : H ( f ) is also in F[S,type], where type[v->H] denotes the
      function that is equal to type except that it maps v to H,
   6. if v in V, H a header and f a formula in F[S,type[v->H]] then the formula
      â v : H ( f ) is also in F[S,type]
Examples of formulas:
    * t.name = "C. J. Date" â¨ t.name = "H. Darwen"
    * Book(t) â¨ Magazine(t)
    * â t : {author, title, subject} ( Â¬ ( Book(t) â§ t.author = "C. J.
      Date" â§ Â¬ ( t.subject = "relational model")))
Note that the last formula states that all books that are written by C. J. Date
have as their subject the relational model. As usual we omit brackets if this
causes no ambiguity about the semantics of the formula.
We will assume that the quantifiers quantify over the universe of all tuples
over the domain in the schema. This leads to the following formal semantics for
formulas given a database db over S and a tuple variable binding val : V -> TD:
   1. f1 â§ f2 is true if and only if f1 is true and f2 is true,
   2. f1 â¨ f2 is true if and only if f1 is true or f2 is true or both are
      true,
   3. Â¬ f is true if and only if f is not true,
   4. â v : H ( f ) is true if and only if there is a tuple t over D such
      that dom(t) = H and the formula f is true for val[v->t], and
   5. â v : H ( f ) is true if and only if for all tuples t over D such that
      dom(t) = H the formula f is true for val[v->t].
**** Queries[edit] ****
Finally we define what a query expression looks like given a schema S = (D, R,
h):
      { v : H | f(v) }
where v is a tuple variable, H a header and f(v) a formula in F[S,type] where
type = { (v, H) } and with v as its only free variable. The result of such a
query for a given database db over S is the set of all tuples t over D with dom
(t) = H such that f is true for db and val = { (v, t) }.
Examples of query expressions are:
    * { t : {name} | â s : {name, wage} ( Employee(s) â§ s.wage = 50.000 â§
      t.name = s.name ) }
    * { t : {supplier, article} | â s : {s#, sname} ( Supplier(s) â§ s.sname
      = t.supplier â§ â p : {p#, pname} ( Product(p) â§ p.pname = t.article
      â§ â a : {s#, p#} ( Supplies(a) â§ s.s# = a.s# â§ a.p# = p.p# ) }
***** Semantic and syntactic restriction of the calculus[edit] *****
**** Domain-independent queries[edit] ****
Because the semantics of the quantifiers is such that they quantify over all
the tuples over the domain in the schema it can be that a query may return a
different result for a certain database if another schema is presumed. For
example, consider the two schemas S1 = ( D1, R, h ) and S2 = ( D2, R, h ) with
domains D1 = { 1 }, D2 = { 1, 2 }, relation names R = { "r1" } and headers h =
{ ("r1", {"a"}) }. Both schemas have a common instance:
      db = { ( "r1", { ("a", 1) } ) }
If we consider the following query expression
      { t : {a} | t.a = t.a }
then its result on db is either { (a : 1) } under S1 or { (a : 1), (a : 2) }
under S2. It will also be clear that if we take the domain to be an infinite
set, then the result of the query will also be infinite. To solve these
problems we will restrict our attention to those queries that are domain
independent, i.e., the queries that return the same result for a database under
all of its schemas.
An interesting property of these queries is that if we assume that the tuple
variables range over tuples over the so-called active domain of the database,
which is the subset of the domain that occurs in at least one tuple in the
database or in the query expression, then the semantics of the query
expressions does not change. In fact, in many definitions of the tuple calculus
this is how the semantics of the quantifiers is defined, which makes all
queries by definition domain independent.
**** Safe queries[edit] ****
In order to limit the query expressions such that they express only domain-
independent queries a syntactical notion of safe query is usually introduced.
To determine whether a query expression is safe we will derive two types of
information from a query. The first is whether a variable-column pair t.a is
bound to the column of a relation or a constant, and the second is whether two
variable-column pairs are directly or indirectly equated (denoted t.v == s.w).
For deriving boundedness we introduce the following reasoning rules:
   1. in " v.a = w.b " no variable-column pair is bound,
   2. in " v.a = k " the variable-column pair v.a is bound,
   3. in " r(v) " all pairs v.a are bound for a in type(v),
   4. in " f1 â§ f2 " all pairs are bound that are bound either in f1 or in
      f2,
   5. in " f1 â¨ f2 " all pairs are bound that are bound both in f1 and in f2,
   6. in " Â¬ f " no pairs are bound,
   7. in " â v : H ( f ) " a pair w.a is bound if it is bound in f and w <>
      v, and
   8. in " â v : H ( f ) " a pair w.a is bound if it is bound in f and w <>
      v.
For deriving equatedness we introduce the following reasoning rules (next to
the usual reasoning rules for equivalence relations: reflexivity, symmetry and
transitivity):
   1. in " v.a = w.b " it holds that v.a == w.b,
   2. in " v.a = k " no pairs are equated,
   3. in " r(v) " no pairs are equated,
   4. in " f1 â§ f2 " it holds that v.a == w.b if it holds either in f1 or in
      f2,
   5. in " f1 â¨ f2 " it holds that v.a == w.b if it holds both in f1 and in
      f2,
   6. in " Â¬ f " no pairs are equated,
   7. in " â v : H ( f ) " it holds that w.a == x.b if it holds in f and w<>v
      and x<>v, and
   8. in " â v : H ( f ) " it holds that w.a == x.b if it holds in f and w<>v
      and x<>v.
We then say that a query expression { v : H | f(v) } is safe if
    * for every column name a in H we can derive that v.a is equated with a
      bound pair in f,
    * for every subexpression of f of the form " â w : G ( g ) " we can
      derive that for every column name a in G we can derive that w.a is
      equated with a bound pair in g, and
    * for every subexpression of f of the form " â w : G ( g ) " we can
      derive that for every column name a in G we can derive that w.a is
      equated with a bound pair in g.
The restriction to safe query expressions does not limit the expressiveness
since all domain-independent queries that could be expressed can also be
expressed by a safe query expression. This can be proven by showing that for a
schema S = (D, R, h), a given set K of constants in the query expression, a
tuple variable v and a header H we can construct a safe formula for every pair
v.a with a in H that states that its value is in the active domain. For
example, assume that K={1,2}, R={"r"} and h = { ("r", {"a, "b"}) } then the
corresponding safe formula for v.b is:
      v.b = 1 â¨ v.b = 2 â¨ â w ( r(w) â§ ( v.b = w.a â¨ v.b = w.b ) )
This formula, then, can be used to rewrite any unsafe query expression to an
equivalent safe query expression by adding such a formula for every variable v
and column name a in its type where it is used in the expression. Effectively
this means that we let all variables range over the active domain, which, as
was already explained, does not change the semantics if the expressed query is
domain independent.
***** Systems[edit] *****
    * DES_â_An_educational_tool_for_working_with_Tuple_Relational_Calculus
      and_other_formal_languages
    * WinRDBI_â_An_educational_tool_for_working_with_Tuple_Relational
      Calculus_and_other_formal_languages
***** See also[edit] *****
    * Relational_algebra
    * Relational_calculus
          o Domain_relational_calculus (DRC)
***** References[edit] *****
    * Edgar_F._Codd: A_Relational_Model_of_Data_for_Large_Shared_Data_Banks.
      Communications_of_the_ACM, 13(6):377â387, 1970.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Tuple_relational_calculus&oldid=898633110"
Categories:
    * Relational_model
    * Logical_calculi
Hidden categories:
    * Wikipedia_articles_needing_clarification_from_May_2019
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
    * Deutsch
    * EspaÃ±ol
    * Italiano
    * Ð ÑÑÑÐºÐ¸Ð¹
    * ä¸­æ
Edit_links
    * This page was last edited on 24 May 2019, at 22:43 (UTC).
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
