The following text has been accessed from https://en.wikipedia.org/wiki/Relational_model at Fri Aug 9 01:11:26 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Relational model ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The relational model (RM) for database management is an approach to managing
data using a structure and language consistent with first-order_predicate
logic, first described in 1969 by English computer scientist Edgar_F._Codd,[1]
[2] where all data is represented in terms of tuples, grouped into relations. A
database organized in terms of the relational model is a relational_database.
Diagram of an example database according to the relational model[3]
In the relational model, related records are linked together with a "key".
The purpose of the relational model is to provide a declarative method for
specifying data and queries: users directly state what information the database
contains and what information they want from it, and let the database
management system software take care of describing data structures for storing
the data and retrieval procedures for answering queries.
Most relational databases use the SQL data definition and query language; these
systems implement what can be regarded as an engineering approximation to the
relational model. A table in an SQL database schema corresponds to a predicate
variable; the contents of a table to a relation; key constraints, other
constraints, and SQL queries correspond to predicates. However, SQL databases
deviate_from_the_relational_model_in_many_details, and Codd fiercely argued
against deviations that compromise the original principles.[4]
⁰
***** Contents *****
    * 1_Overview
          o 1.1_Alternatives
          o 1.2_Implementation
    * 2_History
          o 2.1_Controversies
    * 3_Topics
          o 3.1_Interpretation
          o 3.2_Application_to_databases
          o 3.3_SQL_and_the_relational_model
          o 3.4_Relational_operations
          o 3.5_Database_normalization
    * 4_Examples
          o 4.1_Database
          o 4.2_Customer_relation
    * 5_Set-theoretic_formulation
          o 5.1_Key_constraints_and_functional_dependencies
          o 5.2_Algorithm_to_derive_candidate_keys_from_functional_dependencies
    * 6_See_also
    * 7_References
    * 8_Further_reading
    * 9_External_links
***** Overview[edit] *****
The relational model's central idea is to describe a database as a collection
of predicates over a finite set of predicate variables, describing constraints
on the possible values and combinations of values. The content of the database
at any given time is a finite (logical) model of the database, i.e. a set of
relations, one per predicate variable, such that all predicates are satisfied.
A request for information from the database (a database_query) is also a
predicate.
Relational model concepts.
**** Alternatives[edit] ****
Other models are the hierarchical_model and network_model. Some systems using
these older architectures are still in use today in data_centers with high data
volume needs, or where existing systems are so complex and abstract that it
would be cost-prohibitive to migrate to systems employing the relational model.
Also of note are newer object-oriented_databases.
**** Implementation[edit] ****
There have been several attempts to produce a true implementation of the
relational database model as originally defined by Codd and explained by Date,
Darwen and others, but none have been popular successes so far. As of
October 2015[update] Rel is one of the more recent attempts to do this.
The relational model was the first database model to be described in formal
mathematical terms. Hierarchical and network databases existed before
relational databases, but their specifications were relatively informal. After
the relational model was defined, there were many attempts to compare and
contrast the different models, and this led to the emergence of more rigorous
descriptions of the earlier models; though the procedural nature of the data
manipulation interfaces for hierarchical and network databases limited the
scope for formalization.[citation_needed]
***** History[edit] *****
The relational model was invented by Edgar_F._Codd as a general model of data,
and subsequently promoted by Chris_Date and Hugh_Darwen among others. In The
Third_Manifesto (first published in 1995) Date and Darwen attempt to show how
the relational model can allegedly accommodate certain "desired" object-
oriented features.
**** Controversies[edit] ****
Codd himself, some years after publication of his 1970 model, proposed a three-
valued_logic (True, False, Missing/NULL) version of it to deal with missing
information, and in his The Relational Model for Database Management Version 2
(1990) he went a step further with a four-valued logic (True, False, Missing
but Applicable, Missing but Inapplicable) version.[5] But these have never been
implemented, presumably because of attending complexity. SQL's NULL construct
was intended to be part of a three-valued logic system, but fell short of that
due to logical errors in the standard and in its implementations.[6]
***** Topics[edit] *****
The fundamental assumption of the relational model is that all data is
represented as mathematical n-ary relations, an n-ary relation being a subset
of the Cartesian_product of n domains. In the mathematical model, reasoning
about such data is done in two-valued predicate_logic, meaning there are two
possible evaluations for each proposition: either true or false (and in
particular no third value such as unknown, or not applicable, either of which
are often associated with the concept of NULL). Data are operated upon by means
of a relational_calculus or relational_algebra, these being equivalent in
expressive_power.
The relational model of data permits the database designer to create a
consistent, logical representation of information. Consistency is achieved by
including declared constraints in the database design, which is usually
referred to as the logical schema. The theory includes a process of database
normalization whereby a design with certain desirable properties can be
selected from a set of logically_equivalent alternatives. The access_plans and
other implementation and operation details are handled by the DBMS engine, and
are not reflected in the logical model. This contrasts with common practice for
SQL DBMSs in which performance_tuning often requires changes to the logical
model.
The basic relational building block is the domain or data_type, usually
abbreviated nowadays to type. A tuple is an ordered set of attribute values. An
attribute is an ordered pair of attribute name and type name. An attribute
value is a specific valid value for the type of the attribute. This can be
either a scalar value or a more complex type.
A relation consists of a heading and a body. A heading is a set of attributes.
A body (of an n-ary relation) is a set of n-tuples. The heading of the relation
is also the heading of each of its tuples.
A relation is defined as a set of n-tuples. In both mathematics and the
relational database model, a set is an unordered collection of unique, non-
duplicated items, although some DBMSs impose an order to their data. In
mathematics, a tuple has an order, and allows for duplication. E. F._Codd
originally defined tuples using this mathematical definition.[2] Later, it was
one of E. F._Codd's great insights that using attribute names instead of an
ordering would be so much more convenient (in general) in a computer language
based on relations[citation_needed]. This insight is still being used today.
Though the concept has changed, the name "tuple" has not. An immediate and
important consequence of this distinguishing feature is that in the relational
model the Cartesian_product becomes commutative.
A table is an accepted visual representation of a relation; a tuple is similar
to the concept of a row.
A relvar is a named variable of some specific relation type, to which at all
times some relation of that type is assigned, though the relation may contain
zero tuples.
The basic principle of the relational model is the Information_Principle: all
information is represented by data values in relations. In accordance with this
Principle, a relational_database is a set of relvars and the result of every
query is presented as a relation.
The consistency of a relational database is enforced, not by rules built into
the applications that use it, but rather by constraints, declared as part of
the logical schema and enforced by the DBMS for all applications. In general,
constraints are expressed using relational comparison operators, of which just
one, "is subset of" (â), is theoretically sufficient[citation_needed]. In
practice, several useful shorthands are expected to be available, of which the
most important are candidate_key (really, superkey) and foreign_key
constraints.
**** Interpretation[edit] ****
To fully appreciate the relational model of data it is essential to understand
the intended interpretation of a relation.
The body of a relation is sometimes called its extension. This is because it is
to be interpreted as a representation of the extension of some predicate, this
being the set of true propositions that can be formed by replacing each free
variable in that predicate by a name (a term that designates something).
There is a one-to-one_correspondence between the free variables of the
predicate and the attribute names of the relation heading. Each tuple of the
relation body provides attribute values to instantiate the predicate by
substituting each of its free variables. The result is a proposition that is
deemed, on account of the appearance of the tuple in the relation body, to be
true. Contrariwise, every tuple whose heading conforms to that of the relation,
but which does not appear in the body is deemed to be false. This assumption is
known as the closed_world_assumption: it is often violated in practical
databases, where the absence of a tuple might mean that the truth of the
corresponding proposition is unknown. For example, the absence of the tuple
('John', 'Spanish') from a table of language skills cannot necessarily be taken
as evidence that John does not speak Spanish.
For a formal exposition of these ideas, see the section Set-theoretic
Formulation, below.
**** Application to databases[edit] ****
A data_type as used in a typical relational database might be the set of
integers, the set of character strings, the set of dates, or the two boolean
values true and false, and so on. The corresponding type names for these types
might be the strings "int", "char", "date", "boolean", etc. It is important to
understand, though, that relational theory does not dictate what types are to
be supported; indeed, nowadays provisions are expected to be available for
user-defined types in addition to the built-in ones provided by the system.
Attribute is the term used in the theory for what is commonly referred to as a
column. Similarly, table is commonly used in place of the theoretical term
relation (though in SQL the term is by no means synonymous with relation). A
table data structure is specified as a list of column definitions, each of
which specifies a unique column name and the type of the values that are
permitted for that column. An attribute value is the entry in a specific column
and row, such as "John Doe" or "35".
A tuple is basically the same thing as a row, except in an SQL DBMS, where the
column values in a row are ordered. (Tuples are not ordered; instead, each
attribute value is identified solely by the attribute name and never by its
ordinal position within the tuple.) An attribute name might be "name" or "age".
A relation is a table structure definition (a set of column definitions) along
with the data appearing in that structure. The structure definition is the
heading and the data appearing in it is the body, a set of rows. A database
relvar (relation variable) is commonly known as a base table. The heading of
its assigned value at any time is as specified in the table declaration and its
body is that most recently assigned to it by invoking some update operator
(typically, INSERT, UPDATE, or DELETE). The heading and body of the table
resulting from evaluation of some query are determined by the definitions of
the operators used in the expression of that query. (Note that in SQL the
heading is not always a set of column definitions as described above, because
it is possible for a column to have no name and also for two or more columns to
have the same name. Also, the body is not always a set of rows because in SQL
it is possible for the same row to appear more than once in the same body.)
**** SQL and the relational model[edit] ****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (February 2013)(Learn_how_and_when_to_remove_this_template_message)
SQL, initially pushed as the standard language for relational_databases,
deviates from the relational model in several places. The current ISO SQL
standard doesn't mention the relational model or use relational terms or
concepts. However, it is possible to create a database conforming to the
relational model using SQL if one does not use certain SQL features.
The following deviations from the relational model have been noted[who?] in
SQL. Note that few database servers implement the entire SQL standard and in
particular do not allow some of these deviations. Whereas NULL is ubiquitous,
for example, allowing duplicate column names within a table or anonymous
columns is uncommon.
  Duplicate rows
      The same row can appear more than once in an SQL table. The same tuple
      cannot appear more than once in a relation.
  Anonymous columns
      A column in an SQL table can be unnamed and thus unable to be referenced
      in expressions. The relational model requires every attribute to be named
      and referenceable.
  Duplicate column names
      Two or more columns of the same SQL table can have the same name and
      therefore cannot be referenced, on account of the obvious ambiguity. The
      relational model requires every attribute to be referenceable.
  Column order significance
      The order of columns in an SQL table is defined and significant, one
      consequence being that SQL's implementations of Cartesian product and
      union are both noncommutative. The relational model requires there to be
      no significance to any ordering of the attributes of a relation.
  Views without CHECK OPTION
      Updates to a view defined without CHECK OPTION can be accepted but the
      resulting update to the database does not necessarily have the expressed
      effect on its target. For example, an invocation of INSERT can be
      accepted but the inserted rows might not all appear in the view, or an
      invocation of UPDATE can result in rows disappearing from the view. The
      relational model requires updates to a view to have the same effect as if
      the view were a base relvar.
  Columnless tables unrecognized
      SQL requires every table to have at least one column, but there are two
      relations of degree zero (of cardinality one and zero) and they are
      needed to represent extensions of predicates that contain no free
      variables.
  NULL
      This special mark can appear instead of a value wherever a value can
      appear in SQL, in particular in place of a column value in some row. The
      deviation from the relational model arises from the fact that the
      implementation of this ad hoc concept in SQL involves the use of three-
      valued_logic, under which the comparison of NULL with itself does not
      yield true but instead yields the third truth_value, unknown; similarly
      the comparison NULL with something other than itself does not yield false
      but instead yields unknown. It is because of this behavior in comparisons
      that NULL is described as a mark rather than a value. The relational
      model depends on the law_of_excluded_middle under which anything that is
      not true is false and anything that is not false is true; it also
      requires every tuple in a relation body to have a value for every
      attribute of that relation. This particular deviation is disputed by some
      if only because E. F. Codd himself eventually advocated the use of
      special marks and a 4-valued logic, but this was based on his observation
      that there are two distinct reasons why one might want to use a special
      mark in place of a value, which led opponents of the use of such logics
      to discover more distinct reasons and at least as many as 19 have been
      noted, which would require a 21-valued logic.[citation_needed] SQL itself
      uses NULL for several purposes other than to represent "value unknown".
      For example, the sum of the empty set is NULL, meaning zero, the average
      of the empty set is NULL, meaning undefined, and NULL appearing in the
      result of a LEFT JOIN can mean "no value because there is no matching row
      in the right-hand operand". There are ways to design tables to avoid the
      need for NULL, typically what may be considered or resemble high degrees
      of database_normalization, but many find such impractical. It can be a
      hotly debated topic.
**** Relational operations[edit] ****
Users (or programs) request data from a relational database by sending it a
query that is written in a special language, usually a dialect of SQL. Although
SQL was originally intended for end-users, it is much more common for SQL
queries to be embedded into software that provides an easier user interface.
Many Web sites, such as Wikipedia, perform SQL queries when generating pages.
In response to a query, the database returns a result set, which is just a list
of rows containing the answers. The simplest query is just to return all the
rows from a table, but more often, the rows are filtered in some way to return
just the answer wanted.
Often, data from multiple tables are combined into one, by doing a join.
Conceptually, this is done by taking all possible combinations of rows (the
Cartesian_product), and then filtering out everything except the answer. In
practice, relational database management systems rewrite ("optimize") queries
to perform faster, using a variety of techniques.
There are a number of relational operations in addition to join. These include
project (the process of eliminating some of the columns), restrict (the process
of eliminating some of the rows), union (a way of combining two tables with
similar structures), difference (that lists the rows in one table that are not
found in the other), intersect (that lists the rows found in both tables), and
product (mentioned above, which combines each row of one table with each row of
the other). Depending on which other sources you consult, there are a number of
other operators â many of which can be defined in terms of those listed
above. These include semi-join, outer operators such as outer join and outer
union, and various forms of division. Then there are operators to rename
columns, and summarizing or aggregating operators, and if you permit relation
values as attributes (relation-valued attribute), then operators such as group
and ungroup. The SELECT statement in SQL serves to handle all of these except
for the group and ungroup operators.
The flexibility of relational databases allows programmers to write queries
that were not anticipated by the database designers. As a result, relational
databases can be used by multiple applications in ways the original designers
did not foresee, which is especially important for databases that might be used
for a long time (perhaps several decades). This has made the idea and
implementation of relational databases very popular with businesses.
**** Database normalization[edit] ****
Main article: Database_normalization
Relations are classified based upon the types of anomalies to which they're
vulnerable. A database that's in the first normal form is vulnerable to all
types of anomalies, while a database that's in the domain/key normal form has
no modification anomalies. Normal forms are hierarchical in nature. That is,
the lowest level is the first normal form, and the database cannot meet the
requirements for higher level normal forms without first having met all the
requirements of the lesser normal forms.[7]
***** Examples[edit] *****
**** Database[edit] ****
An idealized, very simple example of a description of some relvars (relation
variables) and their attributes:
    * Customer (Customer_ID, Tax ID, Name, Address, City, State, Zip, Phone,
      Email, Sex)
    * Order (Order_No, Customer_ID, Invoice_No, Date Placed, Date Promised,
      Terms, Status)
    * Order Line (Order_No, Order_Line_No, Product_Code, Qty)
    * Invoice (Invoice_No, Customer_ID, Order_No, Date, Status)
    * Invoice Line (Invoice_No, Invoice_Line_No, Product_Code, Qty Shipped)
    * Product (Product_Code, Product Description)
In this design we have six relvars: Customer, Order, Order Line, Invoice,
Invoice Line and Product. The bold, underlined attributes are candidate_keys.
The non-bold, underlined attributes are foreign_keys.
Usually one candidate_key is chosen to be called the primary_key and used in
preference over the other candidate keys, which are then called alternate_keys.
A candidate key is a unique identifier enforcing that no tuple will be
duplicated; this would make the relation into something else, namely a bag, by
violating the basic definition of a set. Both foreign keys and superkeys (that
includes candidate keys) can be composite, that is, can be composed of several
attributes. Below is a tabular depiction of a relation of our example Customer
relvar; a relation can be thought of as a value that can be attributed to a
relvar.
**** Customer relation[edit] ****
Customer ID Tax ID      Name     Address                 [More fields…]
1234567890  555-5512222 Ramesh   323 Southern Avenue     …
2223344556  555-5523232 Adam     1200 Main Street        …
3334445563  555-5533323 Shweta   871 Rani Jhansi Road    …
4232342432  555-5325523 Sarfaraz 123 Maulana Azad Sarani …
If we attempted to insert a new customer with the ID 1234567890, this would
violate the design of the relvar since Customer_ID is a primary key and we
already have a customer 1234567890. The DBMS must reject a transaction such as
this that would render the database inconsistent by a violation of an integrity
constraint.
Foreign_keys are integrity_constraints enforcing that the value of the
attribute_set is drawn from a candidate_key in another relation. For example,
in the Order relation the attribute Customer_ID is a foreign key. A join is the
operation that draws on information from several relations at once. By joining
relvars from the example above we could query the database for all of the
Customers, Orders, and Invoices. If we only wanted the tuples for a specific
customer, we would specify this using a restriction_condition.
If we wanted to retrieve all of the Orders for Customer 1234567890, we could
query the database to return every row in the Order table with Customer_ID
1234567890 and join the Order table to the Order Line table based on Order_No.
There is a flaw in our database_design above. The Invoice relvar contains an
Order No attribute. So, each tuple in the Invoice relvar will have one Order
No, which implies that there is precisely one Order for each Invoice. But in
reality an invoice can be created against many orders, or indeed for no
particular order. Additionally the Order relvar contains an Invoice No
attribute, implying that each Order has a corresponding Invoice. But again this
is not always true in the real world. An order is sometimes paid through
several invoices, and sometimes paid without an invoice. In other words, there
can be many Invoices per Order and many Orders per Invoice. This is a many-to-
many relationship between Order and Invoice (also called a non-specific
relationship). To represent this relationship in the database a new relvar
should be introduced whose role is to specify the correspondence between Orders
and Invoices:
OrderInvoice (Order_No, Invoice_No)
Now, the Order relvar has a one-to-many_relationship to the OrderInvoice table,
as does the Invoice relvar. If we want to retrieve every Invoice for a
particular Order, we can query for all orders where Order_No in the Order
relation equals the Order_No in OrderInvoice, and where Invoice_No in
OrderInvoice equals the Invoice_No in Invoice.
***** Set-theoretic formulation[edit] *****
Basic notions in the relational model are relation names and attribute names.
We will represent these as strings such as "Person" and "name" and we will
usually use the variables     r , s , t , &#x2026;   {\displaystyle
r,s,t,\ldots }  [r, s, t, \ldots] and     a , b , c   {\displaystyle a,b,c}
[a,b,c] to range over them. Another basic notion is the set of atomic values
that contains values such as numbers and strings.
Our first definition concerns the notion of tuple, which formalizes the notion
of row or record in a table:
  Tuple
      A tuple is a partial_function from attribute names to atomic values.
  Header
      A header is a finite set of attribute names.
  Projection
      The projection of a tuple     t   {\displaystyle t}  [t] on a finite_set
      of attributes     A   {\displaystyle A}  [A] is     t [ A ] = { ( a , v )
      : ( a , v ) &#x2208; t , a &#x2208; A }   {\displaystyle t[A]=\{(a,v):
      (a,v)\in t,a\in A\}}  [t[A] = \{ (a, v) : (a, v) \in t, a \in A \}].
The next definition defines relation that formalizes the contents of a table as
it is defined in the relational model.
  Relation
      A relation is a tuple     ( H , B )   {\displaystyle (H,B)}  [(H, B)]
      with     H   {\displaystyle H}  [H], the header, and     B
      {\displaystyle B}  [B], the body, a set of tuples that all have the
      domain     H   {\displaystyle H}  [H].
Such a relation closely corresponds to what is usually called the extension of
a predicate in first-order_logic except that here we identify the places in the
predicate with attribute names. Usually in the relational model a database
schema is said to consist of a set of relation names, the headers that are
associated with these names and the constraints that should hold for every
instance of the database schema.
  Relation universe
      A relation universe     U   {\displaystyle U}  [U] over a header     H
      {\displaystyle H}  [H] is a non-empty set of relations with header     H
      {\displaystyle H}  [H].
  Relation schema
      A relation schema     ( H , C )   {\displaystyle (H,C)}  [(H, C)]
      consists of a header     H   {\displaystyle H}  [H] and a predicate     C
      ( R )   {\displaystyle C(R)}  [C(R)] that is defined for all relations
      R   {\displaystyle R}  [R] with header     H   {\displaystyle H}  [H]. A
      relation satisfies a relation schema     ( H , C )   {\displaystyle
      (H,C)}  [(H, C)] if it has header     H   {\displaystyle H}  [H] and
      satisfies     C   {\displaystyle C}  [C].
**** Key constraints and functional dependencies[edit] ****
One of the simplest and most important types of relation constraints is the key
constraint. It tells us that in every instance of a certain relational schema
the tuples can be identified by their values for certain attributes.
  Superkey
A superkey is a set of column headers for which the values of those columns
concatenated are unique across all rows. Formally:
      A superkey is written as a finite set of attribute names.
      A superkey     K   {\displaystyle K}  [K] holds in a relation     ( H , B
      )   {\displaystyle (H,B)}  [(H, B)] if:
          *    K &#x2286; H   {\displaystyle K\subseteq H}  [K \subseteq H] and
          * there exist no two distinct tuples      t  1   ,  t  2   &#x2208; B
            {\displaystyle t_{1},t_{2}\in B}  [t_1, t_2 \in B] such that      t
            1   [ K ] =  t  2   [ K ]   {\displaystyle t_{1}[K]=t_{2}[K]}  [t_1
            [K] = t_2[K]].
      A superkey holds in a relation universe     U   {\displaystyle U}  [U] if
      it holds in all relations in     U   {\displaystyle U}  [U].
      Theorem: A superkey     K   {\displaystyle K}  [K] holds in a relation
      universe     U   {\displaystyle U}  [U] over     H   {\displaystyle H}
      [H] if and only if     K &#x2286; H   {\displaystyle K\subseteq H}  [K
      \subseteq H] and     K &#x2192; H   {\displaystyle K\rightarrow H}  [K
      \rightarrow H] holds in     U   {\displaystyle U}  [U].
  Candidate_key
A candidate key is a superkey cannot be further subdivided to form another
superkey.
      A superkey     K   {\displaystyle K}  [K] holds as a candidate key for a
      relation universe     U   {\displaystyle U}  [U] if it holds as a
      superkey for     U   {\displaystyle U}  [U] and there is no proper_subset
      of     K   {\displaystyle K}  [K] that also holds as a superkey for     U
      {\displaystyle U}  [U].
  Functional_dependency
Functional dependency is the property that a value in a tuple may be derived
from another value in that tuple.
      A functional dependency (FD for short) is written as     X &#x2192; Y
      {\displaystyle X\rightarrow Y}  [X \rightarrow Y] for     X , Y
      {\displaystyle X,Y}  [X,Y] finite sets of attribute names.
      A functional dependency     X &#x2192; Y   {\displaystyle X\rightarrow Y}
      [X \rightarrow Y] holds in a relation     ( H , B )   {\displaystyle
      (H,B)}  [(H, B)] if:
          *    X , Y &#x2286; H   {\displaystyle X,Y\subseteq H}  [X, Y
            \subseteq H] and
          *    &#x2200;   {\displaystyle \forall }  [\forall ] tuples      t  1
            ,  t  2   &#x2208; B   {\displaystyle t_{1},t_{2}\in B}  [t_1, t_2
            \in B],      t  1   [ X ] =  t  2   [ X ] &#xA0; &#x21D2; &#xA0;  t
            1   [ Y ] =  t  2   [ Y ]   {\displaystyle t_{1}[X]=t_{2}
            [X]~\Rightarrow ~t_{1}[Y]=t_{2}[Y]}  [t_1[X] = t_2
            [X]~\Rightarrow~t_1[Y] = t_2[Y]]
      A functional dependency     X &#x2192; Y   {\displaystyle X\rightarrow Y}
      [X \rightarrow Y] holds in a relation universe     U   {\displaystyle U}
      [U] if it holds in all relations in     U   {\displaystyle U}  [U].
  Trivial functional dependency
      A functional dependency is trivial under a header     H   {\displaystyle
      H}  [H] if it holds in all relation universes over     H   {\displaystyle
      H}  [H].
      Theorem: An FD     X &#x2192; Y   {\displaystyle X\rightarrow Y}  [X
      \rightarrow Y] is trivial under a header     H   {\displaystyle H}  [H]
      if and only if     Y &#x2286; X &#x2286; H   {\displaystyle Y\subseteq
      X\subseteq H}  [Y \subseteq X \subseteq H].
  Closure
      Armstrong's_axioms: The closure of a set of FDs     S   {\displaystyle S}
      [S] under a header     H   {\displaystyle H}  [H], written as      S  +
      {\displaystyle S^{+}}  [S^+], is the smallest superset of     S
      {\displaystyle S}  [S] such that:
          *    Y &#x2286; X &#x2286; H &#xA0; &#x21D2; &#xA0; X &#x2192; Y
            &#x2208;  S  +     {\displaystyle Y\subseteq X\subseteq
            H~\Rightarrow ~X\rightarrow Y\in S^{+}}  [Y \subseteq X \subseteq
            H~\Rightarrow~X \rightarrow Y \in S^+] (reflexivity)
          *    X &#x2192; Y &#x2208;  S  +   &#x2227; Y &#x2192; Z &#x2208;  S
            +   &#xA0; &#x21D2; &#xA0; X &#x2192; Z &#x2208;  S  +
            {\displaystyle X\rightarrow Y\in S^{+}\land Y\rightarrow Z\in S^
            {+}~\Rightarrow ~X\rightarrow Z\in S^{+}}  [X \rightarrow Y \in S^+
            \land Y \rightarrow Z \in S^+~\Rightarrow~X \rightarrow Z \in S^+]
            (transitivity) and
          *    X &#x2192; Y &#x2208;  S  +   &#x2227; Z &#x2286; H &#xA0;
            &#x21D2; &#xA0; ( X &#x222A; Z ) &#x2192; ( Y &#x222A; Z ) &#x2208;
            S  +     {\displaystyle X\rightarrow Y\in S^{+}\land Z\subseteq
            H~\Rightarrow ~(X\cup Z)\rightarrow (Y\cup Z)\in S^{+}}  [X
            \rightarrow Y \in S^+ \land Z \subseteq H~\Rightarrow~(X \cup Z)
            \rightarrow (Y \cup Z) \in S^+] (augmentation)
      Theorem: Armstrong's axioms are sound and complete; given a header     H
      {\displaystyle H}  [H] and a set     S   {\displaystyle S}  [S] of FDs
      that only contain subsets of     H   {\displaystyle H}  [H],     X
      &#x2192; Y &#x2208;  S  +     {\displaystyle X\rightarrow Y\in S^{+}}  [X
      \rightarrow Y \in S^+] if and only if     X &#x2192; Y   {\displaystyle
      X\rightarrow Y}  [X \rightarrow Y] holds in all relation universes over
      H   {\displaystyle H}  [H] in which all FDs in     S   {\displaystyle S}
      [S] hold.
  Completion
      The completion of a finite set of attributes     X   {\displaystyle X}
      [X] under a finite set of FDs     S   {\displaystyle S}  [S], written as
      X  +     {\displaystyle X^{+}}  [X^+], is the smallest superset of     X
      {\displaystyle X}  [X] such that:
          *    Y &#x2192; Z &#x2208; S &#x2227; Y &#x2286;  X  +   &#xA0;
            &#x21D2; &#xA0; Z &#x2286;  X  +     {\displaystyle Y\rightarrow
            Z\in S\land Y\subseteq X^{+}~\Rightarrow ~Z\subseteq X^{+}}  [Y
            \rightarrow Z \in S \land Y \subseteq X^+~\Rightarrow~Z \subseteq
            X^+]
      The completion of an attribute set can be used to compute if a certain
      dependency is in the closure of a set of FDs.
      Theorem: Given a set     S   {\displaystyle S}  [S] of FDs,     X
      &#x2192; Y &#x2208;  S  +     {\displaystyle X\rightarrow Y\in S^{+}}  [X
      \rightarrow Y \in S^+] if and only if     Y &#x2286;  X  +
      {\displaystyle Y\subseteq X^{+}}  [Y \subseteq X^+].
  Irreducible cover
      An irreducible cover of a set     S   {\displaystyle S}  [S] of FDs is a
      set     T   {\displaystyle T}  [T] of FDs such that:
          *     S  +   =  T  +     {\displaystyle S^{+}=T^{+}}  [S^+ = T^+]
          * there exists no     U &#x2282; T   {\displaystyle U\subset T}  [U
            \subset T] such that      S  +   =  U  +     {\displaystyle S^
            {+}=U^{+}}  [S^+ = U^+]
          *    X &#x2192; Y &#x2208; T &#xA0; &#x21D2; Y   {\displaystyle
            X\rightarrow Y\in T~\Rightarrow Y}  [X \rightarrow Y \in
            T~\Rightarrow Y] is a singleton set and
          *    X &#x2192; Y &#x2208; T &#x2227; Z &#x2282; X &#xA0; &#x21D2;
            &#xA0; Z &#x2192; Y &#x2209;  S  +     {\displaystyle X\rightarrow
            Y\in T\land Z\subset X~\Rightarrow ~Z\rightarrow Y\notin S^{+}}  [X
            \rightarrow Y \in T \land Z \subset X~\Rightarrow~Z \rightarrow Y
            \notin S^+].
**** Algorithm to derive candidate keys from functional dependencies[edit] ****
:INPUT: a set S of FDs that contain only subsets of a header H
      OUTPUT: the set C of superkeys that hold as candidate keys in
              all relation universes over H in which all FDs in S hold
      begin
        C := â;          // found candidate keys
        Q := { H };      // superkeys that contain candidate keys
        while Q <> â do
          let K be some element from Q;
          Q := Q â { K };
          minimal := true;
          for each X->Y in S do
            K' := (K â Y) âª X;   // derive new superkey
            if K' â K then
              minimal := false;
              Q := Q âª { K' };
            end if
          end for
          if minimal and there is not a subset of K in C then
            remove all supersets of K from C;
            C := C âª { K };
          end if
        end while
      end
***** See also[edit] *****
    * Domain_relational_calculus            * Relation
    * List_of_relational_database           * Relational_database
      management_systems                    * Relational_database_management
    * Query_language                          system
          o Database_query_language         * The_Third_Manifesto (TTM)
          o Information_retrieval_query     * Tuple-versioning
            language
***** References[edit] *****
   1. ^Codd, E.F (1969), Derivability, Redundancy, and Consistency of Relations
      Stored in Large Data Banks, Research Report, IBM
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
   3. .
   4. ^ a bCodd, E.F (1970). "A_Relational_Model_of_Data_for_Large_Shared_Data
      Banks". Communications_of_the_ACM. Classics. 13 (6): 377â87. doi:
      10.1145/362384.362685. Archived from the_original on 2007-06-12.
   5. ^Data_Integration_Glossary (PDF), US: Department of Transportation,
      August 2001, archived from the_original (PDF) on 2012-02-18
   6. .
   7. ^Codd, E. F (1990), The Relational Model for Database Management,
      Addison-Wesley, pp. 371â388, ISBN 978-0-201-14192-4
   8. .
   9. ^Date, C.J (2006). "18. Why Three- and Four-Valued Logic Don't Work".
      Date on Database: Writings 2000â2006. Apress. pp. 329â41. ISBN 978-1-
      59059-746-0.
  10. ^Date, C.J (2004). An Introduction to Database Systems (8 ed.). Addison
      Wesley. pp. 592â97. ISBN 978-0-321-19784-9.
  11. ^ David M. Kroenke, Database Processing: Fundamentals, Design, and
      Implementation (1997), Prentice-Hall, Inc., pages 130â144
***** Further reading[edit] *****
    * Date, C. J.; Darwen, Hugh (2000). Foundation for future database systems:
      the third manifesto; a detailed study of the impact of type theory on the
      relational model of data, including a comprehensive model of type
      inheritance (2 ed.). Reading, MA: Addison-Wesley. ISBN 978-0-201-70928-5.
——— (2007). An Introduction to Database Systems (8 ed.). Boston: Pearson
Education. ISBN 978-0-321-19784-9.
***** External links[edit] *****
 Wikimedia Commons has media related to Relational_models.
    * Childs (1968), Feasibility of a set-theoretic data structure: a general
      structure based on a reconstituted definition of relation (research),
      Handle, hdl:2027.42/4164
 cited in Codd's 1970 paper.
Darwen, Hugh, The_Third_Manifesto_(TTM)
.
Relational_Databases at Curlie
"Relational_Model", C2
.
Binary_relations_and_tuples_compared_with_respect_to_the_semantic_web (World
Wide_Web log), Sun
.
    * v
    * t
    * e
Database_models
                    * Flat
                    * Hierarchical
                    * Dimensional
                    * Network
Common models       * Relational
                    * Entityârelationship
                          o Enhanced
                    * Graph
                    * Object-oriented
                    * Entityâattributeâvalue
                    * Associative
                    * Correlational
                    * Multidimensional
Other models        * Array
                    * Semantic
                    * Star_schema
                    * XML_database
                    * Flat_file
                    * Column-oriented
                    * Document-oriented
                    * Object-relational
Implementations     * Deductive
                    * Temporal
                    * XML_data_store
                    * Key-value_store
                    * Triplestore
    * v
    * t
    * e
Database_management_systems
                   * Object-oriented
                         o comparison
                   * Relational
Types                    o comparison
                   * Document-oriented
                   * Graph
                   * NoSQL
                   * NewSQL
                   * Database
                   * ACID
                   * Armstrong's_axioms
                   * CAP_theorem
                   * CRUD
Concepts           * Null
                   * Candidate_key
                   * Foreign_key
                   * Superkey
                   * Surrogate_key
                   * Unique_key
                   * Relation
                         o table
                         o column
                         o row
                   * View
Objects            * Transaction
                   * Transaction_log
                   * Trigger
                   * Index
                   * Stored_procedure
                   * Cursor
                   * Partition
                   * Concurrency_control
                   * Data_dictionary
                   * JDBC
Components         * XQJ
                   * ODBC
                   * Query_language
                   * Query_optimizer
                   * Query_plan
                   * Administration
Functions          * Query_optimization
                   * Replication
                   * Database_models
                   * Database_normalization
                   * Database_storage
                   * Distributed_database
                   * Federated_database_system
Related topics     * Referential_integrity
                   * Relational_algebra
                   * Relational_calculus
                   * Relational_database
                   * Relational model
                   * Object-relational_database
                   * Transaction_processing

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Relational_model&oldid=907337803"
Categories:
    * Database_management_systems
    * Relational_model
    * 1969_in_computer_science
    * Programming_paradigms
Hidden categories:
    * Articles_containing_potentially_dated_statements_from_October_2015
    * All_articles_containing_potentially_dated_statements
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_August_2016
    * Articles_with_unsourced_statements_from_February_2007
    * Articles_with_unsourced_statements_from_August_2010
    * Articles_needing_additional_references_from_February_2013
    * All_articles_needing_additional_references
    * All_articles_with_specifically_marked_weasel-worded_phrases
    * Articles_with_specifically_marked_weasel-worded_phrases_from_September
      2011
    * Articles_with_unsourced_statements_from_July_2009
    * Commons_category_link_is_on_Wikidata
    * Articles_with_Curlie_links
    * Articles_with_example_pseudocode
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
    * AzÉrbaycanca
    * CatalÃ 
    * ÄeÅ¡tina
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * íêµ­ì´
    * Interlingua
    * Italiano
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * LietuviÅ³
    * Magyar
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 22 July 2019, at 06:49 (UTC).
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
