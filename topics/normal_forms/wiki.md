The following text has been accessed from https://en.wikipedia.org/wiki/Database_normalization at Fri Aug 9 01:11:45 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Database normalization ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Reduction of data redundancy
 This article needs attention from an expert in Databases. See the talk_page
 for details. WikiProject_Databases may be able to help recruit an expert.
 (March 2018)
Database normalization is the process of structuring a relational_database
[clarification_needed] in accordance with a series of so-called normal_forms in
order to reduce data_redundancy and improve data_integrity. It was first
proposed by Edgar_F._Codd as an integral part of his relational_model.
Normalization entails organizing the columns (attributes) and tables
(relations) of a database to ensure that their dependencies are properly
enforced by database integrity constraints. It is accomplished by applying some
formal rules either by a process of synthesis (creating a new database design)
or decomposition (improving an existing database design).
⁰
***** Contents *****
    * 1_Objectives
          o 1.1_Minimize_redesign_when_extending_the_database_structure
          o 1.2_Example
    * 2_Normal_forms
    * 3_Example_of_a_step_by_step_normalization
          o 3.1_Initial_data
          o 3.2_Satisfying_1NF
          o 3.3_Satisfying_2NF
          o 3.4_Satisfying_3NF
          o 3.5_Satisfying_EKNF
          o 3.6_Satisfying_BCNF
          o 3.7_Satisfying_4NF
          o 3.8_Satisfying_ETNF
          o 3.9_Satisfying_5NF
          o 3.10_Satisfying_DKNF
          o 3.11_Satisfying_6NF
    * 4_See_also
    * 5_Notes_and_references
    * 6_Further_reading
    * 7_External_links
***** Objectives[edit] *****
A basic objective of the first normal form defined by Codd in 1970 was to
permit data to be queried and manipulated using a "universal data sub-language"
grounded in first-order_logic.[1] (SQL is an example of such a data sub-
language, albeit one that Codd regarded as seriously flawed.[2])
The objectives of normalization beyond 1NF (first normal form) were stated as
follows by Codd:
        1. To free the collection of relations from undesirable insertion,
           update and deletion dependencies.
        2. To reduce the need for restructuring the collection of
           relations, as new types of data are introduced, and thus
           increase the life span of application programs.
        3. To make the relational model more informative to users.
        4. To make the collection of relations neutral to the query
           statistics, where these statistics are liable to change as time
           goes by.
           â E.F. Codd, "Further Normalization of the Data Base
           Relational Model"[3]
An update anomaly. Employee 519 is shown as having different addresses on
different records.
An insertion anomaly. Until the new faculty member, Dr. Newsome, is assigned to
teach at least one course, his or her details cannot be recorded.
A deletion anomaly. All information about Dr. Giddens is lost if he or she
temporarily ceases to be assigned to any courses.
When an attempt is made to modify (update, insert into, or delete from) a
relation, the following undesirable side-effects may arise in relations that
have not been sufficiently normalized:
    * Update anomaly. The same information can be expressed on multiple rows;
      therefore updates to the relation may result in logical inconsistencies.
      For example, each record in an "Employees' Skills" relation might contain
      an Employee ID, Employee Address, and Skill; thus a change of address for
      a particular employee may need to be applied to multiple records (one for
      each skill). If the update is only partially successful â the
      employee's address is updated on some records but not others â then the
      relation is left in an inconsistent state. Specifically, the relation
      provides conflicting answers to the question of what this particular
      employee's address is. This phenomenon is known as an update anomaly.
    * Insertion anomaly. There are circumstances in which certain facts cannot
      be recorded at all. For example, each record in a "Faculty and Their
      Courses" relation might contain a Faculty ID, Faculty Name, Faculty Hire
      Date, and Course Code. Therefore, we can record the details of any
      faculty member who teaches at least one course, but we cannot record a
      newly hired faculty member who has not yet been assigned to teach any
      courses, except by setting the Course Code to null. This phenomenon is
      known as an insertion anomaly.
    * Deletion anomaly. Under certain circumstances, deletion of data
      representing certain facts necessitates deletion of data representing
      completely different facts. The "Faculty and Their Courses" relation
      described in the previous example suffers from this type of anomaly, for
      if a faculty member temporarily ceases to be assigned to any courses, we
      must delete the last of the records on which that faculty member appears,
      effectively also deleting the faculty member, unless we set the Course
      Code to null. This phenomenon is known as a deletion anomaly.
**** Minimize redesign when extending the database structure[edit] ****
A fully normalized database allows its structure to be extended to accommodate
new types of data without changing existing structure too much. As a result,
applications interacting with the database are minimally affected.
Normalized relations, and the relationship between one normalized relation and
another, mirror real-world concepts and their interrelationships.
**** Example[edit] ****
Querying and manipulating the data within a data structure that is not
normalized, such as the following non-1NF representation of customers, credit
card transactions, involves more complexity than is really necessary:
Customer Cust. ID Transactions
                  Tr. ID Date        Amount
Abraham  1        12890  14-Oct-2003 −87
                  12904  15-Oct-2003 −50
Issac    2        Tr. ID Date        Amount
                  12898  14-Oct-2003 −21
                  Tr. ID Date        Amount
Jacob    3        12907  15-Oct-2003 −18
                  14920  20-Nov-2003 −70
                  15003  27-Nov-2003 −60

To each customer corresponds a 'repeating group' of transactions. The automated
evaluation of any query relating to customers' transactions, therefore, would
broadly involve two stages:
   1. Unpacking one or more customers' groups of transactions allowing the
      individual transactions in a group to be examined, and
   2. Deriving a query result based on the results of the first stage
For example, in order to find out the monetary sum of all transactions that
occurred in October 2003 for all customers, the system would have to know that
it must first unpack the Transactions group of each customer, then sum the
Amounts of all transactions thus obtained where the Date of the transaction
falls in October 2003.
One of Codd's important insights was that structural complexity can be reduced.
Reduced structural complexity gives users, application, and DBMS more power and
flexibility to formulate and evaluate the queries. A more normalized equivalent
of the structure above might look like this:
Customer Cust. ID
Abraham  1
Issac    2
Jacob    3
Cust. ID Tr. ID Date        Amount
1        12890  14-Oct-2003 −87
1        12904  15-Oct-2003 −50
2        12898  14-Oct-2003 −21
3        12907  15-Oct-2003 −18
3        14920  20-Nov-2003 −70
3        15003  27-Nov-2003 −60
In the modified structure, the key is {Cust. ID} in the first relation, {Cust.
ID, Tr ID} in the second relation.
Now each row represents an individual credit card transaction, and the DBMS can
obtain the answer of interest, simply by finding all rows with a Date falling
in October, and summing their Amounts. The data structure places all of the
values on an equal footing, exposing each to the DBMS directly, so each can
potentially participate directly in queries; whereas in the previous situation
some values were embedded in lower-level structures that had to be handled
specially. Accordingly, the normalized design lends itself to general-purpose
query processing, whereas the unnormalized design does not. The normalized
version also allows the user to change the customer name in one place and
guards against errors that arise if the customer name is misspelled on some
records.
***** Normal forms[edit] *****
Codd introduced the concept of normalization and what is now known as the first
normal_form (1NF) in 1970.[4] Codd went on to define the second_normal_form
(2NF) and third_normal_form (3NF) in 1971,[5] and Codd and Raymond_F._Boyce
defined the Boyce-Codd_normal_form (BCNF) in 1974.[6]
Informally, a relational database relation is often described as "normalized"
if it meets third normal form.[7] Most 3NF relations are free of insertion,
update, and deletion anomalies.
The normal forms (from least normalized to most normalized) are:
    * UNF: Unnormalized_form
    * 1NF: First_normal_form
    * 2NF: Second_normal_form
    * 3NF: Third_normal_form
    * EKNF: Elementary_key_normal_form
    * BCNF: BoyceâCodd_normal_form
    * 4NF: Fourth_normal_form
    * ETNF: Essential_tuple_normal_form
    * 5NF: Fifth_normal_form
    * DKNF: Domain-key_normal_form
    * 6NF: Sixth_normal_form
             UNF     1NF    2NF    3NF    EKNF   BCNF   4NF    ETNF   5NF    DKNF   6NF
             (1970)  (1970) (1971) (1971) (1982) (1974) (1977) (2012) (1979) (1981) (2003)
Primary_key
(no          [Maybe] [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]
duplicate
tuples)
No repeating [Maybe] [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]
groups
Atomic
columns
(cells have  [No]    [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]
single
value)
No partial
dependencies
(values
depend on    [No]    [No]   [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]
the whole of
every
Candidate
key)
No
transitive
dependencies
(values      [No]    [No]   [No]   [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]
depend only
on Candidate
keys)
Every non-
trivial
functional
dependency
involves     [No]    [No]   [No]   [No]   [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  N/A
either a
superkey or
an
elementary
key's subkey
No
redundancy
from any     [No]    [No]   [No]   [No]   [No]   [Yes]  [Yes]  [Yes]  [Yes]  [Yes]  N/A
functional
dependency
Every non-
trivial,
multi-value  [No]    [No]   [No]   [No]   [No]   [No]   [Yes]  [Yes]  [Yes]  [Yes]  N/A
dependency
has a
superkey
A component
of every
explicit
join         [No]    [No]   [No]   [No]   [No]   [No]   [No]   [Yes]  [Yes]  [Yes]  N/A
dependency
is a
superkey[8]
Every non-
trivial join
dependency
is implied   [No]    [No]   [No]   [No]   [No]   [No]   [No]   [No]   [Yes]  [Yes]  N/A
by a
candidate
key
Every
constraint
is a
consequence  [No]    [No]   [No]   [No]   [No]   [No]   [No]   [No]   [No]   [Yes]  N/A
of domain
constraints
and key
constraints
Every join
dependency   [No]    [No]   [No]   [No]   [No]   [No]   [No]   [No]   [No]   [No]   [Yes]
is trivial
***** Example of a step by step normalization[edit] *****
Normalization is a database design technique, which is used to design a
relational_database table up to higher normal form. [9] The process is
progressive, and a higher level of database normalization cannot be achieved
unless the previous levels have been satisfied. [10]
That means that, having data in unnormalized_form (the least normalized) and
aiming to achieve the highest level of normalization, the first step would be
to ensure compliance to first_normal_form, the second step would be to ensure
second_normal_form is satisfied, and so forth in order mentioned above, until
the data conform to sixth_normal_form.
However, it is worth noting that normal forms beyond 4NF are mainly of academic
interest, as the problems they exist to solve rarely appear in practice [11]
Please note that the data in the following example were intentionally designed
to contradict most of the normal forms. In real life, it's quite possible to be
able to skip some of the normalization steps because the table doesn't contain
anything contradicting the given normal form. It also commonly occurs that
fixing a violation of one normal form also fixes a violation of a higher normal
form in the process. Also one table has been chosen for normalization at each
step, meaning that at the end of this example process, there might still be
some tables not satisfying the highest normal form.
**** Initial data[edit] ****
Let a database table with the following structure: [10]
Title        Author  Author      Format    Price Subject   Pages Thickness Publisher Publisher Publication Genre Genre
                     Nationality                                                     Country   Type        ID    Name
Beginning
MySQL        Chad                                MySQL,
Database     Russell American    Hardcover 49.99 Database, 520   Thick     Apress    USA       E-book      1     Tutorial
Design and                                       Design
Optimization
We assume in this example that each book has only one author.
**** Satisfying 1NF[edit] ****
To satisfy 1NF, we need to ensure that the values in each column of a table are
atomic. In the initial table, Subject contains a set of values, meaning it does
not comply.
One way to achieve the first_normal_form would be to separate the duplicities
into multiple columns:
Title        Format    Author  Author      Price Subject Subject  Subject Pages Thickness Publisher Publisher Genre Genre
                               Nationality       1       2        3                                 country   ID    Name
Beginning
MySQL                  Chad
Database     Hardcover Russell American    49.99 MySQL   Database Design  520   Thick     Apress    USA       1     Tutorial
Design and
Optimization
Although now the table formally complies to the 1NF (is atomic), the problem
with this solution is obvious - if a book has more than three subjects, it
cannot be added to the database without altering its structure.
To solve the problem in a more elegant way, it is necessary to identify
entities represented in the table and separate them into their own respective
tables. In this case, it would result in Book, Subject and Publisher tables:
[10]
                                          Book
Title        Format    Author  Author      Price Pages Thickness Genre Genre    Publisher
                               Nationality                       ID    Name     ID
Beginning
MySQL                  Chad
Database     Hardcover Russell American    49.99 520   Thick     1     Tutorial 1
Design and
Optimization
        Subject
Subject_ID Subject name          Publisher
1          MySQL        Publisher_ID Name   Country
2          Database     1            Apress USA
3          Design
Simply separating the initial data into multiple tables would break the
connection between the data. That means we also need to determine the
relationships between the newly introduced tables. You might have noticed the
Publisher ID column in the Book's table - it is a foreign_key realizing many-
to-one relation between a book and a publisher.
A book can fit many subjects, as well as a subject may correspond to many
books. That means we also need to define a many-to-many relationship. We
achieve that by creating a link_table: [10]
                      Title - Subject
Title                                            Subject ID
Beginning MySQL Database Design and Optimization 1
Beginning MySQL Database Design and Optimization 2
Beginning MySQL Database Design and Optimization 3

Instead of one table in unnormalized_form, we now have 4 tables conforming to
the 1NF.
**** Satisfying 2NF[edit] ****
The Book table has one candidate_key, the compound_key {Title , Format}.[12]
Consider the following table fragment:
                                           Book
Title        Format    Author   Author      Price Pages Thickness Genre Genre    Publisher
                                Nationality                       ID    Name     ID
Beginning
MySQL                  Chad
Database     Hardcover Russell  American    49.99 520   Thick     1     Tutorial 1
Design and
Optimization
Beginning
MySQL                  Chad
Database     E-book    Russell  American    22.34 520   Thick     1     Tutorial 1
Design and
Optimization
The
Relational
Model for    E-book    E.F.Codd British     13.88 538   Thick     2     Popular  2
Database                                                                science
Management:
Version 2
The
Relational
Model for    Paperback E.F.Codd British     39.99 538   Thick     2     Popular  2
Database                                                                science
Management:
Version 2
All of the attributes that are not part of the key depend on Title, but only
Price also depends on Format. To conform to 2NF and remove duplicities, every
non-key attribute must depend on the whole key, not just part of it.
To normalize this table, make {Title} the (simple) key so that every non-key
attribute depends upon the whole key, and remove Price into a separate table so
that its dependency on Format can be preserved:
                                                                                 Format - Prices
                                                                           Title        Format    Price
                                                                           Beginning
                                                                           MySQL
                                                                           Database     Hardcover 49.99
                                   Book                                    Design and
Title        Author   Author      Pages Thickness Genre Genre    Publisher Optimization
                      Nationality                 ID    Name     ID        Beginning
Beginning                                                                  MySQL
MySQL        Chad                                                          Database     E-book    22.34
Database     Russell  American    520   Thick     1     Tutorial 1         Design and
Design and                                                                 Optimization
Optimization                                                               The
The                                                                        Relational
Relational                                                                 Model for    E-book    13.88
Model for    E.F.Codd British     538   Thick     2     Popular  2         Database
Database                                                science            Management:
Management:                                                                Version 2
Version 2                                                                  The
                                                                           Relational
                                                                           Model for    Paperback 39.99
                                                                           Database
                                                                           Management:
                                                                           Version 2
Now, the book table conforms to 2NF.
**** Satisfying 3NF[edit] ****
A table in third_normal_form (3NF) is a table in 2NF that has no transitive
dependencies. Note the book table with more rows (previously omitted for
brevity):
                                     Book
Title        Author   Author      Pages Thickness Genre ID Genre Name Publisher
                      Nationality                                     ID
Beginning
MySQL        Chad
Database     Russell  American    520   Thick     1        Tutorial   1
Design and
Optimization
The
Relational
Model for    E.F.Codd British     538   Thick     2        Popular    2
Database                                                   science
Management:
Version 2
Learning SQL Alan     American    338   Slim      1        Tutorial   3
             Beaulieu
SQL Cookbook Anthony  American    636   Thick     1        Tutorial   3
             Molinaro
Genre ID and Genre Name both depend upon the primary key {Title}, but they are
not independent of one another. The dependency of, say, Genre Name on the
primary key can be deduced from the dependency of Genre Name on Genre ID and of
Genre ID on the primary key. Since there are more titles than genres, that
dependency introduces redundant data into the Book table which can be
eliminated by abstracting the dependency of Genre Name on Genre ID into its own
table:
                              Book
Title        Author   Author      Pages Thickness Genre Publisher
                      Nationality                 ID    ID
Beginning
MySQL        Chad
Database     Russell  American    520   Thick     1     1
Design and                                                         Book Genres
Optimization                                                      Genre Genre
The                                                               ID    Name
Relational                                                        1     Tutorial
Model for    E.F.Codd British     538   Thick     2     2         2     Popular
Database                                                                science
Management:
Version 2
Learning SQL Alan     American    338   Slim      1     3
             Beaulieu
SQL Cookbook Anthony  American    636   Thick     1     3
             Molinaro
The Book table is now in third normal form. Although tables in 1NF are by
definition normalized, "normalized" is commonly used to mean 3NF.[7]
**** Satisfying EKNF[edit] ****
EKNF falls strictly between 3NF and BCNF and isn't much discussed in the
literature. It is intended âto capture the salient qualities of both 3NF and
BCNFâ while avoiding the problems of both (namely, that 3NF is âtoo
forgivingâ and BCNF is âprone to computational complexityâ). Since it is
rarely mentioned in literature, it is not included in this example. [13] For
more information on the EKNF, see its own Wikipedia_page.
**** Satisfying BCNF[edit] ****
A relational schema R is considered to be in BoyceâCodd normal form (BCNF)
if, for every one of its dependencies X â Y, one of the following conditions
hold true:
    * X â Y is a trivial functional dependency (i.e., Y is a subset of X)
    * X is a superkey for schema R
Consider the table in 3NF from the previous step:
                                     Book
Title           Author        Author      Pages Thickness Genre ID Publisher ID
                              Nationality
Beginning MySQL
Database Design Chad Russell  American    520   Thick     1        1
and
Optimization
The Relational
Model for
Database        E.F.Codd      British     538   Thick     2        2
Management:
Version 2
Learning SQL    Alan Beaulieu American    338   Slim      1        3
SQL Cookbook    Anthony       American    636   Thick     1        3
                Molinaro
There is a non-trivial dependency violating BCNF - {Author} â {Author
Nationality}. Therefore, the table should be decomposed:
                        Book
Title        Author   Pages Thickness Genre Publisher
                                      ID    ID
Beginning
MySQL        Chad                                       Author - Nationality
Database     Russell  520   Thick     1     1         Author       Author
Design and                                                         Nationality
Optimization                                          Chad Russell American
The                                                   E.F.Codd     British
Relational                                            Alan         American
Model for    E.F.Codd 538   Thick     2     2         Beaulieu
Database                                              Anthony      American
Management:                                           Molinaro
Version 2
Learning SQL Alan     338   Slim      1     3
             Beaulieu
SQL Cookbook Anthony  636   Thick     1     3
             Molinaro
Now, each attribute represents a fact about the key, the whole key, and nothing
but the key. Therefore BCNF has been achieved. [14]
**** Satisfying 4NF[edit] ****
Assume the database is owned by a book retailer franchise that has several
franchisees that own shops in different locations. And therefore the retailer
decided to add a table that contains data about availability of the books at
different locations:
                          Franchisee - Book Location
Franchisee_ID Title                                                 Location
1             Beginning MySQL Database Design and Optimization      California
1             Beginning MySQL Database Design and Optimization      Florida
1             Beginning MySQL Database Design and Optimization      Texas
1             The Relational Model for Database Management: Version California
              2
1             The Relational Model for Database Management: Version Florida
              2
1             The Relational Model for Database Management: Version Texas
              2
2             Beginning MySQL Database Design and Optimization      California
2             Beginning MySQL Database Design and Optimization      Florida
2             Beginning MySQL Database Design and Optimization      Texas
2             The Relational Model for Database Management: Version California
              2
2             The Relational Model for Database Management: Version Florida
              2
2             The Relational Model for Database Management: Version Texas
              2
3             Beginning MySQL Database Design and Optimization      Texas
As this table structure consists of a compound_primary_key, it doesn't contain
any non-key attributes and it's already in BCNF (and therefore also satisfies
all the previous normal_forms). However, if we assume that all available books
are offered in each area, we might notice that the Title is not unambiguously
bound to a certain Location and therefore the table doesn't satisfy 4NF.
That means that, to satisfy the fourth_normal_form, this table needs to be
decomposed as well:
                Franchisee - Book
Franchisee_ID Title                                Franchisee - Location
1             Beginning MySQL Database Design and Franchisee_ID Location
              Optimization                        1             California
1             The Relational Model for Database   1             Florida
              Management: Version 2               1             Texas
2             Beginning MySQL Database Design and 2             California
              Optimization                        2             Florida
2             The Relational Model for Database   2             Texas
              Management: Version 2               3             Texas
3             Beginning MySQL Database Design and
              Optimization
Now, every record is unambiguously identified by a superkey, therefore 4NF is
satisfied. [15]
**** Satisfying ETNF[edit] ****
Suppose the franchisees can also order books from different suppliers. Let the
relation also be subject to the following constraint:
    * If a certain supplier supplies a certain title
    * and the title is supplied to the franchisee
    * and the franchisee is being supplied by the supplier,
    * then the supplier supplies the title to the franchisee. [16]
                         Supplier - Book - Franchisee
Supplier_ID Title                                                 Franchisee_ID
1           Beginning MySQL Database Design and Optimization      1
2           The Relational Model for Database Management: Version 2
            2
3           Learning SQL                                          3
This table is in 4NF, but the Supplier ID is equal to the join of its
projections: { { Supplier ID , Book } , { Book, Franchisee ID } , { Franchisee
ID , Supplier ID } }. No component of that join dependency is a superkey (the
sole superkey being the entire heading), so the table does not satisfy the ETNF
and can be further decomposed: [16]
                               Book - Franchisee
     Supplier - Book       Title        Franchisee_ID
Supplier_ID Title          Beginning
            Beginning      MySQL
1           MySQL Database Database     1               Franchisee - Supplier
            Design and     Design and                 Supplier_ID Franchisee_ID
            Optimization   Optimization               1           1
            The Relational The                        2           2
            Model for      Relational                 3           3
2           Database       Model for    2
            Management:    Database
            Version 2      Management:
3           Learning SQL   Version 2
                           Learning SQL 3
After the decomposition, compliance to ETNF is ensured.
**** Satisfying 5NF[edit] ****
To spot a table not satisfying the 5NF, it is usually necessary to examine the
data thoroughly. Suppose the table from 4NF_example with a little modification
in data and let's examine if it satisfies 5NF:
                          Franchisee - Book Location
Franchisee_ID Title                                                 Location
1             Beginning MySQL Database Design and Optimization      California
1             Learning SQL                                          California
1             The Relational Model for Database Management: Version Texas
              2
2             The Relational Model for Database Management: Version California
              2
If we decompose this table, we lower redundancies and get the following two
tables:
                Franchisee - Book
Franchisee_ID Title
1             Beginning MySQL Database Design and  Franchisee - Location
              Optimization                        Franchisee_ID Location
1             Learning SQL                        1             California
1             The Relational Model for Database   1             Texas
              Management: Version 2               2             California
2             The Relational Model for Database
              Management: Version 2
What happens if we try to join these tables? The query would return the
following data:
                     Franchisee - Book - Location JOINed
Franchisee_ID Title                                                 Location
1             Beginning MySQL Database Design and Optimization      California
1             Learning SQL                                          California
1             The Relational Model for Database Management: Version California
              2
1             The Relational Model for Database Management: Version Texas
              2
1             Learning SQL                                          Texas
1             Beginning MySQL Database Design and Optimization      Texas
2             The Relational Model for Database Management: Version California
              2
Apparently, the JOIN returns three more rows than it should - let's try to add
another table to clarify the relation. We end up with three separate tables:
    Franchisee - Book
Franchisee_ID Title
              Beginning                                   Location - Book
              MySQL                                 Location   Title
1             Database                                         Beginning MySQL
              Design and                            California Database Design
              Optimization                                     and Optimization
1             Learning SQL  Franchisee - Location   California Learning SQL
              The          Franchisee_ID Location              The Relational
              Relational   1             California            Model for
1             Model for    1             Texas      California Database
              Database     2             California            Management:
              Management:                                      Version 2
              Version 2                                        The Relational
              The                                              Model for
              Relational                            Texas      Database
2             Model for                                        Management:
              Database                                         Version 2
              Management:
              Version 2
What will the JOIN return now? It actually is not possible to join these three
tables. That means it wasn't possible to decompose the Franchisee - Book
Location without data loss, therefore the table already satisfies 5NF. [15]
C.J. Date has argued that only a database in 5NF is truly "normalized".[17]
**** Satisfying DKNF[edit] ****
Let's have a look at the Book table from previous examples and see if it
satisfies the Domain_Key_Normal_Form:
                                  Book
Title                               Pages Thickness Genre ID Publisher ID
Beginning MySQL Database Design and 520   Thick     1        1
Optimization
The Relational Model for Database   538   Thick     2        2
Management: Version 2
Learning SQL                        338   Slim      1        3
SQL Cookbook                        636   Thick     1        3
Logically, Thickness is determined by number of pages. That means it depends on
Pages which is not a key. Let's set an example convention saying a book up to
350 pages is considered "slim" and a book over 350 pages is considered "thick".
This convention is technically a constraint but it is neither a domain
constraint nor a key constraint; therefore we cannot rely on domain constraints
and key constraints to keep the data integrity.
In other words - nothing prevents us from putting, for example, "Thick" for a
book with only 50 pages - and this makes the table violate DKNF.
To solve this, we can create a table holding enumeration that defines the
Thickness and remove that column from the original table:
                                         Book - Pages - Genre - Publisher
                                    Title           Pages Genre ID Publisher ID
                                    Beginning MySQL
                                    Database Design 520   1        1
          Thickness Enum            and
Thickness Min pages Max pages       Optimization
Slim      1         350             The Relational
Thick     351       999,999,999,999 Model for
                                    Database        538   2        2
                                    Management:
                                    Version 2
                                    Learning SQL    338   1        3
                                    SQL Cookbook    636   1        3
That way, the domain integrity violation has been eliminated, and the table is
in DKNF.
**** Satisfying 6NF[edit] ****
A simple and intuitive definition of the sixth_normal_form is that "a table is
in 6NF when the row contains the Primary Key, and at most one other attribute".
[18]
That means, for example, the Publishers table designed while creating_the_1NF
         Publisher
Publisher_ID Name   Country
1            Apress USA
needs to be further decomposed into two tables:
     Publisher       Publisher country
Publisher_ID Name   Publisher_ID Country
1            Apress 1            USA
Such normalization to 6NF is mostly used in data warehouses where the benefits
outweigh the drawbacks. [19]
***** See also[edit] *****
    * Denormalization
    * Database_refactoring
***** Notes and references[edit] *****
   1. ^ "The adoption of a relational model of data ... permits the development
      of a universal data sub-language based on an applied predicate calculus.
      A first-order predicate calculus suffices if the collection of relations
      is in first normal form. Such a language would provide a yardstick of
      linguistic power for all other proposed data languages, and would itself
      be a strong candidate for embedding (with appropriate syntactic
      modification) in a variety of host languages (programming, command- or
      problem-oriented)." Codd, "A_Relational_Model_of_Data_for_Large_Shared
      Data_Banks" Archived June 12, 2007, at the Wayback_Machine, p. 381
   2. ^ Codd, E.F. Chapter 23, "Serious Flaws in SQL", in The Relational Model
      for Database Management: Version 2. Addison-Wesley (1990), pp. 371â389
   3. ^ Codd, E.F. "Further Normalization of the Data Base Relational Model",
      p. 34
   4. ^Codd,_E._F. (June 1970). "A_Relational_Model_of_Data_for_Large_Shared
      Data_Banks". Communications_of_the_ACM. 13 (6): 377â387. doi:10.1145/
      362384.362685. Archived from the_original on June 12, 2007. Retrieved
      August 25, 2005.
   5. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   6. ^ Codd, E. F. "Further Normalization of the Data Base Relational Model".
      (Presented at Courant Computer Science Symposia Series 6, "Data Base
      Systems", New York City, May 24â25, 1971.) IBM Research Report RJ909
      (August 31, 1971). Republished in Randall J. Rustin (ed.), Data Base
      Systems: Courant Computer Science Symposia Series 6. Prentice-Hall, 1972.
   7. ^ Codd, E. F. "Recent Investigations into Relational Data Base Systems".
      IBM Research Report RJ1385 (April 23, 1974). Republished in Proc. 1974
      Congress (Stockholm, Sweden, 1974), N.Y.: North-Holland (1974).
   8. ^ a bDate, C. J. (1999). An Introduction to Database Systems. Addison-
      Wesley. p. 290.
   9. ^Darwen, Hugh; Date, C. J.; Fagin, Ronald (2012). "A_Normal_Form_for
      Preventing_Redundant_Tuples_in_Relational_Databases" (PDF). Proceedings
      of the 15th International Conference on Database Theory. EDBT/ICDT_2012
      Joint_Conference. ACM International Conference Proceeding Series.
      Association_for_Computing_Machinery. p. 114. doi:10.1145/2274576.2274589.
      ISBN 978-1-4503-0791-8. OCLC 802369023. Retrieved May 22, 2018.
  10. ^Kumar, Kunal; Azad, S. K. (October 2017). Database normalization design
      pattern. 2017 4th IEEE Uttar Pradesh Section International Conference on
      Electrical, Computer and Electronics (UPCON). IEEE. doi:10.1109/
      upcon.2017.8251067. ISBN 9781538630044.
  11. ^ a b c d"Database_normalization_in_MySQL:_Four_quick_and_easy_steps".
      ComputerWeekly.com. Retrieved January 21, 2019.
  12. ^"Database_Normalization:_5th_Normal_Form_and_Beyond". MariaDB
      KnowledgeBase. Retrieved January 23, 2019.
  13. ^ The table fragment itself has several candidate keys (simple key Price,
      and compound keys of Format together with any column except Price or
      Thickness), but we assume that in the complete table only {Title, Format}
      will be unique.
  14. ^"Additional_Normal_Forms_-_Database_Design_and_Relational_Theory_-_page
      151". what-when-how.com. Retrieved January 22, 2019.
  15. ^Kozubek, Agnieszka (April 3, 2014). "The_Boyce-Codd_Normal_Form_(BCNF)".
      vertabelo. Retrieved January 22, 2019.
  16. ^ a b"Normalizace_databÃ¡ze", Wikipedie (in Czech), November 7, 2018,
      retrieved January 22, 2019
  17. ^ a bDate, C. J. (December 21, 2015). The_New_Relational_Database
      Dictionary:_Terms,_Concepts,_and_Examples. "O'Reilly Media, Inc.".
      p. 138. ISBN 9781491951699.
  18. ^Date, C. J. (December 21, 2015). The_New_Relational_Database_Dictionary:
      Terms,_Concepts,_and_Examples. "O'Reilly Media, Inc.". p. 163.
      ISBN 9781491951699.
  19. ^"normalization_-_Would_like_to_Understand_6NF_with_an_Example". Stack
      Overflow. Retrieved January 23, 2019.
  20. ^"Sixth_normal_form", Wikipedia, December 10, 2018, retrieved January 23,
      2019
***** Further reading[edit] *****
    * Date, C. J. (1999), An_Introduction_to_Database_Systems (8th ed.).
      Addison-Wesley Longman.
ISBN 0-321-19784-4.
Kent, W. (1983) A_Simple_Guide_to_Five_Normal_Forms_in_Relational_Database
Theory, Communications of the ACM, vol. 26, pp. 120â125
H.-J. Schek, P. Pistor Data Structures for an Integrated Data Base Management
and Information Retrieval System
***** External links[edit] *****
    * Kent, William (February 1983). "A_Simple_Guide_to_Five_Normal_Forms_in
      Relational_Database_Theory". Communications of the ACM. 26 (2): 120-125.
Database_Normalization_Basics by Mike Chapple (About.com)
Database_Normalization_Intro, Part_2
An_Introduction_to_Database_Normalization by Mike Hillyer.
A_tutorial_on_the_first_3_normal_forms by Fred Coulson
Description_of_the_database_normalization_basics by Microsoft
Normalization_in_DBMS_by_Chaitanya_(beginnersbook.com)
A_Step-by-Step_Guide_to_Database_Normalization
ETNF_â_Essential_tuple_normal_form
    * v
    * t
    * e
Database normalization
    * Unnormalized_form (UNF/NF2)
    * First_normal_form (1NF)
    * Second_normal_form (2NF)
    * Third_normal_form (3NF)
    * Elementary_key_normal_form (EKNF)
    * BoyceâCodd_normal_form (3.5NF / BCNF)
    * Fourth_normal_form (4NF)
    * Fifth_normal_form (5NF / PJNF)
    * Domain-key_normal_form (DKNF)
    * Sixth_normal_form (6NF)
Denormalization
    * v
    * t
    * e
Database
                * Requirements
                * Theory
                * Models
                * Database_management_system
                * Machine
                * Server
Main            * Application
                * Connection
                      o datasource
                      o DSN
                * Administrator
                * Lock
                * Types
                * Tools
                * Data_definition
Languages       * Data_manipulation
                * Query
                      o information_retrieval
                * Activity_monitoring
Security        * Audit
                * Forensics
                * Negative_database
                * Entities_and_relationships (and Enhanced notation)
Design          * Normalization
                * Refactoring
Programming     * Abstraction_layer
                * Object-relational_mapping
                * Virtualization
                * Tuning
Management            o caching
                * Migration
                * Preservation
                * Integrity
                * Database-centric_architecture
                * Intelligent_database
                * Two-phase_locking
See also        * Locks_with_ordered_sharing
                * Load_file
                * Publishing
                * Halloween_Problem
                * Log_shipping
    * [Wikipedia book] Book
    * [Category] Category
    * [WikiProject] WikiProject
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
                   * Database normalization
                   * Database_storage
                   * Distributed_database
                   * Federated_database_system
Related topics     * Referential_integrity
                   * Relational_algebra
                   * Relational_calculus
                   * Relational_database
                   * Relational_model
                   * Object-relational_database
                   * Transaction_processing

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Database_normalization&oldid=906685735"
Categories:
    * Database_normalization
    * Database_management_systems
    * Database_constraints
    * Data_management
    * Data_modeling
    * Relational_algebra
Hidden categories:
    * Webarchive_template_wayback_links
    * CS1_Czech-language_sources_(cs)
    * Use_American_English_from_February_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * Use_mdy_dates_from_February_2019
    * Articles_needing_expert_attention_from_March_2018
    * All_articles_needing_expert_attention
    * Databases_articles_needing_expert_attention
    * Wikipedia_articles_needing_clarification_from_February_2019
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
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Hrvatski
    * Italiano
    * ×¢××¨××ª
    * LatvieÅ¡u
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 17 July 2019, at 14:27 (UTC).
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
