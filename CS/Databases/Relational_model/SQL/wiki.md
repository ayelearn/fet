The following text has been accessed from https://en.wikipedia.org/wiki/SQL at Fri Aug 9 01:11:36 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** SQL ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the database language. For the IATA code, see San_Carlos
Airport_(California).
"SEQUEL" redirects here. For the topic of the word, see sequel. For other uses,
see sequel_(disambiguation).
Language for management and use of relational databases
                             SQL
Paradigm            Multi-paradigm: declarative
Family              Programming_language
Designed by        Donald_D._Chamberlin
                    Raymond_F._Boyce
Developer           ISO/IEC
First appeared     1974; 45 years ago (1974)
Typing_discipline   Static, strong
OS                  Cross-platform
File_formats        File format details
Filename_extension  .sql
Internet_media typeapplication/sql[1][2]
Developed by       ISO/IEC
Initial release     1986 (1986)
Latest_release      SQL:2016
                    (December 2016; 2 years ago (2016-12))
Type of format      Database
Standard            ISO/IEC 9075
Open_format?        Yes
Major implementations
Many
Dialects
    * SQL-86
    * SQL-89
    * SQL-92
    * SQL:1999
    * SQL:2003
    * SQL:2006
    * SQL:2008
    * SQL:2011
    * SQL:2016
Influenced by
Datalog
Influenced
CQL, LINQ, SPARQL, SOQL, PowerShell,[3] JPQL, jOOQ, N1QL
    *  Structured_Query_Language at Wikibooks
SQL (/ËÉsËkjuËËÉl/ ([About_this_sound]listen) S-Q-L,[4] /ËsiËkwÉl/
"sequel"; Structured Query Language)[5][6][7][8] is a domain-specific_language
used in programming and designed for managing data held in a relational
database_management_system (RDBMS), or for stream processing in a relational
data_stream_management_system (RDSMS). It is particularly useful in handling
structured_data where there are relations between different entities/variables
of the data. SQL offers two main advantages over older read/write APIs like
ISAM or VSAM. First, it introduced the concept of accessing many records with
one single command; and second, it eliminates the need to specify how to reach
a record, e.g. with or without an index.
Originally based upon relational_algebra and tuple_relational_calculus, SQL
consists of many types of statements,[9] which may be informally classed as
sublanguages, commonly: a data_query_language (DQL),[a] a data_definition
language (DDL),[b] a data_control_language (DCL), and a data_manipulation
language (DML).[c][10] The scope of SQL includes data query, data manipulation
(insert, update and delete), data definition (schema creation and
modification), and data access control. Although SQL is often described as, and
to a great extent is, a declarative_language (4GL), it also includes procedural
elements.
SQL was one of the first commercial languages for Edgar_F._Codd's relational
model. The model was described in his influential 1970 paper, "A Relational
Model of Data for Large Shared Data Banks".[11] Despite not entirely adhering
to the_relational_model_as_described_by_Codd, it became the most widely used
database language.[12][13]
SQL became a standard of the American_National_Standards_Institute (ANSI) in
1986, and of the International_Organization_for_Standardization (ISO) in 1987.
[14] Since then, the standard has been revised to include a larger set of
features. Despite the existence of such standards, most SQL code is not
completely portable among different database systems without adjustments.
⁰
***** Contents *****
    * 1_History
    * 2_Design
    * 3_Syntax
    * 4_Procedural_extensions
    * 5_Interoperability_and_standardization
    * 6_Alternatives
    * 7_Distributed_SQL_processing
    * 8_Criticisms
          o 8.1_Orthogonality_and_completeness
          o 8.2_NULLs
          o 8.3_Duplicates
          o 8.4_Impedance_mismatch
    * 9_See_also
    * 10_Notes
    * 11_References
    * 12_Sources
          o 12.1_SQL_standards_documents
                # 12.1.1_ITTF_publicly_available_standards_and_technical
                  reports
                # 12.1.2_Draft_documents
    * 13_External_links
***** History[edit] *****
SQL was initially developed at IBM by Donald_D._Chamberlin and Raymond_F._Boyce
after learning about the relational model from Ted_Codd[15] in the early 1970s.
[16] This version, initially called SEQUEL (Structured English Query Language),
was designed to manipulate and retrieve data stored in IBM's original quasi-
relational database management system, System_R, which a group at IBM_San_Jose
Research_Laboratory had developed during the 1970s.[16]
Chamberlin and Boyce's first attempt of a relational database language was
Square, but it was difficult to use due to subscript notation. After moving to
the San Jose Research Laboratory in 1973, they began work on SEQUEL.[15] The
acronym SEQUEL was later changed to SQL because "SEQUEL" was a trademark of the
UK-based Hawker_Siddeley Dynamics Engineering Limited company.[17]
After testing SQL at customer test sites to determine the usefulness and
practicality of the system, IBM began developing commercial products based on
their System R prototype including System/38, SQL/DS, and DB2, which were
commercially available in 1979, 1981, and 1983, respectively.[18]
In the late 1970s, Relational Software, Inc. (now Oracle_Corporation) saw the
potential of the concepts described by Codd, Chamberlin, and Boyce, and
developed their own SQL-based RDBMS with aspirations of selling it to the U.S.
Navy, Central_Intelligence_Agency, and other U.S._government agencies. In June
1979, Relational Software, Inc. introduced the first commercially available
implementation of SQL, Oracle V2 (Version2) for VAX computers.
By 1986, ANSI and ISO standard groups officially adopted the standard "Database
Language SQL" language definition. New versions of the standard were published
in 1989, 1992, 1996, 1999, 2003, 2006, 2008, 2011,[15] and most recently, 2016.
***** Design[edit] *****
SQL deviates in several ways from its theoretical foundation, the relational
model and its tuple_calculus. In that model, a table is a set of tuples, while
in SQL, tables and query results are lists of rows: the same row may occur
multiple times, and the order of rows can be employed in queries (e.g. in the
LIMIT clause).
Critics argue that SQL should be replaced with a language that strictly returns
to the original foundation: for example, see The_Third_Manifesto. However, no
known proof exists that such uniqueness cannot be added to SQL itself[citation
needed], or at least a variation of SQL. In other words, it's quite possible
that SQL can be "fixed" or at least improved in this regard such that the
industry may not have to switch to a completely different query language to
obtain uniqueness. Debate on this remains open.
***** Syntax[edit] *****
Main article: SQL_syntax
            U P D A T E &#xA0; c l a u s e      {   U P D A T E &#xA0; c o u n
t r y          S E T &#xA0; c l a u s e      {   S E T &#xA0; p o p u l a t i o
n = &#xA0;       p o p u l a t i o n + 1  &#x23DE;     e x p r e s s i o n
W H E R E &#xA0; c l a u s e      {   W H E R E &#xA0;      n a m e =
&#x2032;  U S  A &#x2032;   &#x23DE;    e x p r e s s i o n    &#x23DF;    p r
e d i c a t e   ;       }      statement       {\displaystyle \left.{\begin
{array}{rl}\textstyle {\mathtt {UPDATE~clause}}&\{{\mathtt {UPDATE\
country}}\\\textstyle {\mathtt {SET~clause}}&\{{\mathtt {SET\
population=~}}\overbrace {\mathtt {population+1}} ^{\mathtt
{expression}}\\\textstyle {\mathtt {WHERE~clause}}&\{{\mathtt {WHERE\
\underbrace {{name=}\overbrace {'USA'} ^{expression}} _{predicate};}}\end
{array}}\right\}{\textstyle {\texttt {statement}}}}  [{\displaystyle \left.
{\begin{array}{rl}\textstyle {\mathtt {UPDATE~clause}}&\{{\mathtt {UPDATE\
country}}\\\textstyle {\mathtt {SET~clause}}&\{{\mathtt {SET\
population=~}}\overbrace {\mathtt {population+1}} ^{\mathtt
{expression}}\\\textstyle {\mathtt {WHERE~clause}}&\{{\mathtt {WHERE\
\underbrace {{name=}\overbrace {'USA'} ^{expression}} _{predicate};}}\end
{array}}\right\}{\textstyle {\texttt {statement}}}}]
A chart showing several of the SQL language elements that compose a single
statement
The SQL language is subdivided into several language elements, including:
    * Clauses, which are constituent components of statements and queries. (In
      some cases, these are optional.)[19]
    * Expressions, which can produce either scalar values, or tables consisting
      of columns and rows of data
    * Predicates, which specify conditions that can be evaluated to SQL three-
      valued_logic_(3VL) (true/false/unknown) or Boolean truth_values and are
      used to limit the effects of statements and queries, or to change program
      flow.
    * Queries, which retrieve the data based on specific criteria. This is an
      important element of SQL.
    * Statements, which may have a persistent effect on schemata and data, or
      may control transactions, program flow, connections, sessions, or
      diagnostics.
          o SQL statements also include the semicolon (";") statement
            terminator. Though not required on every platform, it is defined as
            a standard part of the SQL grammar.
    * Insignificant_whitespace is generally ignored in SQL statements and
      queries, making it easier to format SQL code for readability.
***** Procedural extensions[edit] *****
SQL is designed for a specific purpose: to query data contained in a relational
database. SQL is a set-based, declarative_programming_language, not an
imperative_programming_language like C or BASIC. However, extensions to
Standard SQL add procedural_programming_language functionality, such as
control-of-flow constructs. These include:
Source               Common name     Full name
ANSI/ISO Standard    SQL/PSM         SQL/Persistent Stored Modules
Interbase / Firebird PSQL            Procedural SQL
IBM_DB2              SQL_PL          SQL Procedural Language (implements SQL/
                                     PSM)
IBM_Informix         SPL             Stored Procedural Language
IBM Netezza          NZPLSQL[20]     (based on Postgres PL/pgSQL)
Invantive            PSQL[21]        Invantive Procedural SQL (implements SQL/
                                     PSM and PL/SQL)
                                     SQL/Persistent Stored Module (implements
MariaDB              SQL/PSM, PL/SQL SQL/PSM), Procedural Language/SQL (based
                                     on Ada)[22]
Microsoft / Sybase   T-SQL           Transact-SQL
Mimer_SQL            SQL/PSM         SQL/Persistent Stored Module (implements
                                     SQL/PSM)
MySQL                SQL/PSM         SQL/Persistent Stored Module (implements
                                     SQL/PSM)
MonetDB              SQL/PSM         SQL/Persistent Stored Module (implements
                                     SQL/PSM)
NuoDB                SSP             Starkey Stored Procedures
Oracle               PL/SQL          Procedural Language/SQL (based on Ada)
PostgreSQL           PL/pgSQL        Procedural Language/PostgreSQL Structured
                                     Query Language (implements SQL/PSM)
SAP_R/3              ABAP            Advanced Business Application Programming
SAP_HANA             SQLScript       SQLScript
Sybase               Watcom-SQL      SQL Anywhere Watcom-SQL Dialect
Teradata             SPL             Stored Procedural Language
In addition to the standard SQL/PSM extensions and proprietary SQL extensions,
procedural and object-oriented programmability is available on many SQL
platforms via DBMS integration with other languages. The SQL standard defines
SQL/JRT extensions (SQL Routines and Types for the Java Programming Language)
to support Java code in SQL databases. SQL_Server_2005 uses the SQLCLR (SQL
Server Common Language Runtime) to host managed .NET assemblies in the
database, while prior versions of SQL Server were restricted to unmanaged
extended stored procedures primarily written in C. PostgreSQL lets users write
functions in a wide variety of languagesâincluding Perl, Python, Tcl,
JavaScript (PL/V8) and C.[23]
***** Interoperability and standardization[edit] *****
SQL implementations are incompatible between vendors and do not necessarily
completely follow standards. In particular date and time syntax, string
concatenation, NULLs, and comparison case_sensitivity vary from vendor to
vendor. Particular exceptions are PostgreSQL[24] and Mimer_SQL[25] which strive
for standards compliance, though PostgreSQL does not adhere to the standard in
how folding of unquoted names is done. The folding of unquoted names to lower
case in PostgreSQL is incompatible with the SQL standard,[26] which says that
unquoted names should be folded to upper case.[27] Thus, Foo should be
equivalent to FOO not foo according to the standard.
Popular implementations of SQL commonly omit support for basic features of
Standard SQL, such as the DATE or TIME data types. The most obvious such
examples, and incidentally the most popular commercial and proprietary SQL
DBMSs, are Oracle (whose DATE behaves as DATETIME,[28][29] and lacks a TIME
type)[30] and MS SQL Server (before the 2008 version). As a result, SQL code
can rarely be ported between database systems without modifications.
There are several reasons for this lack of portability between database
systems:
    * The complexity and size of the SQL standard means that most implementors
      do not support the entire standard.
    * The standard does not specify database behavior in several important
      areas (e.g. indexes, file storage...), leaving implementations to decide
      how to behave.
    * The SQL standard precisely specifies the syntax that a conforming
      database system must implement. However, the standard's specification of
      the semantics of language constructs is less well-defined, leading to
      ambiguity.
    * Many database vendors have large existing customer bases; where the newer
      version of the SQL standard conflicts with the prior behavior of the
      vendor's database, the vendor may be unwilling to break backward
      compatibility.
    * There is little commercial incentive for vendors to make it easier for
      users to change database suppliers (see vendor_lock-in).
    * Users evaluating database software tend to place other factors such as
      performance higher in their priorities than standards conformance.
SQL was adopted as a standard by the American_National_Standards_Institute
(ANSI) in 1986 as SQL-86[31] and the International_Organization_for
Standardization (ISO) in 1987.[14] It is maintained by ISO/IEC_JTC_1,
Information_technology,_Subcommittee_SC_32,_Data_management_and_interchange.
The standard is commonly denoted by the pattern: ISO/IEC 9075-n:yyyy Part n:
title, or, as a shortcut, ISO/IEC 9075.
ISO/IEC 9075 is complemented by ISO/IEC 13249: SQL Multimedia and Application
Packages (SQL/MM), which defines SQL based interfaces and packages to widely
spread applications like video, audio and spatial_data.
Until 1996, the National_Institute_of_Standards_and_Technology (NIST) data
management standards program certified SQL DBMS compliance with the SQL
standard. Vendors now self-certify the compliance of their products.[32]
The original standard declared that the official pronunciation for "SQL" was an
initialism: /ËÉsËkjuËËÉl/ ("ess cue el").[12] Regardless, many English-
speaking database professionals (including Donald_Chamberlin himself[33]) use
the acronym-like pronunciation of /ËsiËkwÉl/ ("sequel"),[34] mirroring the
language's pre-release development name of "SEQUEL".[16][17][33][16] The SQL
standard has gone through a number of revisions:
Year Name     Alias            Comments
1986 SQL-86   SQL-87           First formalized by ANSI.
1989 SQL-89   FIPS 127-1       Minor revision that added integrity constraints,
                               adopted as FIPS 127-1.
1992 SQL-92   SQL2, FIPS 127-2 Major revision (ISO 9075), Entry Level SQL-92
                               adopted as FIPS 127-2.
                               Added regular expression matching, recursive
                               queries (e.g. transitive_closure), triggers,
                               support for procedural and control-of-flow
1999 SQL:1999 SQL3             statements, non-scalar types (arrays), and some
                               object-oriented features (e.g. structured
                               types). Support for embedding SQL in Java (SQL/
                               OLB) and vice versa (SQL/JRT).
                               Introduced XML-related features (SQL/XML),
2003 SQL:2003                  window functions, standardized sequences, and
                               columns with auto-generated values (including
                               identity-columns).
                               ISO/IEC 9075-14:2006 defines ways that SQL can
                               be used with XML. It defines ways of importing
                               and storing XML data in an SQL database,
                               manipulating it within the database, and
2006 SQL:2006                  publishing both XML and conventional SQL-data in
                               XML form. In addition, it lets applications
                               integrate queries into their SQL code with
                               XQuery, the XML Query Language published by the
                               World Wide Web Consortium (W3C), to concurrently
                               access ordinary SQL-data and XML documents.[35]
                               Legalizes ORDER BY outside cursor definitions.
2008 SQL:2008                  Adds INSTEAD OF triggers, TRUNCATE statement,
                               [36] FETCH clause.
                               Adds temporal data (PERIOD FOR)[37] (more
2011 SQL:2011                  information at: Temporal_database#History).
                               Enhancements for window functions and FETCH
                               clause.[38]
2016 SQL:2016                  Adds row pattern matching, polymorphic table
                               functions, JSON.
2019 SQL:2019                  Adds Part 15, multidimensional arrays (MDarray
                               type and operators).
Interested parties may purchase SQL standards documents from ISO,[39] IEC or
ANSI. A draft of SQL:2008 is freely available as a zip archive.[40]
The SQL standard is divided into ten parts.
    * ISO/IEC 9075-1:2016 Part 1: Framework (SQL/Framework). It provides
      logical concepts.[41]
    * ISO/IEC 9075-2:2016 Part 2: Foundation (SQL/Foundation). It contains the
      most central elements of the language and consists of both mandatory and
      optional features.
    * ISO/IEC 9075-3:2016 Part 3: Call-Level Interface (SQL/CLI). It defines
      interfacing components (structures, procedures, variable bindings) that
      can be used to execute SQL statements from applications written in Ada, C
      respectively C++, COBOL, Fortran, MUMPS, Pascal or PL/I. (For Java see
      part 10.) SQL/CLI is defined in such a way that SQL statements and SQL/
      CLI procedure calls are treated as separate from the calling
      application's source code. Open_Database_Connectivity is a well-known
      superset of SQL/CLI. This part of the standard consists solely of
      mandatory features.
    * ISO/IEC 9075-4:2016 Part 4: Persistent stored modules (SQL/PSM). It
      standardizes procedural extensions for SQL, including flow of control,
      condition handling, statement condition signals and resignals, cursors
      and local variables, and assignment of expressions to variables and
      parameters. In addition, SQL/PSM formalizes declaration and maintenance
      of persistent database language routines (e.g., "stored procedures").
      This part of the standard consists solely of optional features.
    * ISO/IEC 9075-9:2016 Part 9: Management of External Data (SQL/MED). It
      provides extensions to SQL that define foreign-data wrappers and datalink
      types to allow SQL to manage external data. External data is data that is
      accessible to, but not managed by, an SQL-based DBMS. This part of the
      standard consists solely of optional features.
    * ISO/IEC 9075-10:2016 Part 10: Object language bindings (SQL/OLB). It
      defines the syntax and semantics of SQLJ, which is SQL embedded in Java
      (see also part 3). The standard also describes mechanisms to ensure
      binary portability of SQLJ applications, and specifies various Java
      packages and their contained classes. This part of the standard consists
      solely of optional features. Unlike SQL/OLB JDBC defines an API and is
      not part of the SQL standard.[citation_needed]
    * ISO/IEC 9075-11:2016 Part 11: Information and definition schemas (SQL/
      Schemata). It defines the Information Schema and Definition Schema,
      providing a common set of tools to make SQL databases and objects self-
      describing. These tools include the SQL object identifier, structure and
      integrity constraints, security and authorization specifications,
      features and packages of ISO/IEC 9075, support of features provided by
      SQL-based DBMS implementations, SQL-based DBMS implementation information
      and sizing items, and the values supported by the DBMS implementations.
      [42] This part of the standard contains both mandatory and optional
      features.
    * ISO/IEC 9075-13:2016 Part 13: SQL Routines and types using the Java TM
      programming language (SQL/JRT). It specifies the ability to invoke static
      Java methods as routines from within SQL applications ('Java-in-the-
      database'). It also calls for the ability to use Java classes as SQL
      structured user-defined types. This part of the standard consists solely
      of optional features.
    * ISO/IEC 9075-14:2016 Part 14: XML-Related Specifications (SQL/XML). It
      specifies SQL-based extensions for using XML in conjunction with SQL. The
      XML data type is introduced, as well as several routines, functions, and
      XML-to-SQL data type mappings to support manipulation and storage of XML
      in an SQL database.[35] This part of the standard consists solely of
      optional features.[citation_needed]
    * ISO/IEC 9075-15:2019 Part 15: Multi-dimensional arrays (SQL/MDA). It
      specifies a multidimensional array type (MDarray) for SQL, along with
      operations on MDarrays, MDarray slices, MDarray cells, and related
      features. This part of the standard consists solely of optional features.
ISO/IEC 9075 is complemented by ISO/IEC 13249 SQL Multimedia and Application
Packages. This closely related but separate standard is developed by the same
committee. It defines interfaces and packages based on SQL. The aim is a
unified access to typical database applications like text, pictures, data
mining or spatial_data.
    * ISO/IEC 13249-1:2016 Part 1: Framework
    * ISO/IEC 13249-2:2003 Part 2: Full-Text
    * ISO/IEC 13249-3:2016 Part 3: Spatial
    * ISO/IEC 13249-5:2003 Part 5: Still image
    * ISO/IEC 13249-6:2006 Part 6: Data mining
    * ISO/IEC 13249-7:2013 Part 7: History
    * ISO/IEC 13249-8:xxxx Part 8: Metadata Registry Access MRA (work in
      progress)
ISO/IEC 9075 is also accompanied by a series of Technical Reports, published as
ISO/IEC TR 19075 in 8 parts. These Technical Reports explain the justification
for and usage of some features of SQL, giving examples where appropriate. The
Technical Reports are non-normative; if there is any discrepancy from 9075, the
text in 9075 holds. Currently available 19075 Technical Reports are:
    * ISO/IEC TR 19075-1:2011 Part 1: XQuery Regular Expression Support in SQL
    * ISO/IEC TR 19075-2:2015 Part 2: SQL Support for Time-Related Information
    * ISO/IEC TR 19075-3:2015 Part 3: SQL Embedded in Programs using the JavaTM
      programming language
    * ISO/IEC TR 19075-4:2015 Part 4: SQL with Routines and types using the
      JavaTM programming language
    * ISO/IEC TR 19075-5:2016 Part 5: Row Pattern Recognition in SQL
    * ISO/IEC TR 19075-6:2017 Part 6: SQL support for Javascript Object
      Notation (JSON)
    * ISO/IEC TR 19075-7:2017 Part 7: Polymorphic table functions in SQL
    * ISO/IEC TR 19075-8:2019 Part 8: Multi-Dimensional Arrays (SQL/MDA)
***** Alternatives[edit] *****
A distinction should be made between alternatives to SQL as a language, and
alternatives to the relational model itself. Below are proposed relational
alternatives to the SQL language. See navigational_database and NoSQL for
alternatives to the relational model.
    * .QL: object-oriented Datalog
    * 4D_Query_Language (4D QL)
    * Datalog: critics suggest that Datalog has two advantages over SQL: it has
      cleaner semantics, which facilitates program understanding and
      maintenance, and it is more expressive, in particular for recursive
      queries.[43]
    * HTSQL: URL based query method
    * IBM_Business_System_12 (IBM BS12): one of the first fully relational
      database management systems, introduced in 1982
    * ISBL
    * jOOQ: SQL implemented in Java as an internal_domain-specific_language
    * Java_Persistence_Query_Language (JPQL): The query language used by the
      Java Persistence API and Hibernate persistence library
    * JavaScript: MongoDB implements its query language in a JavaScript API.
    * LINQ: Runs SQL statements written like language constructs to query
      collections directly from inside .Net code.
    * Object_Query_Language
    * QBE (Query_By_Example) created by MoshÃ¨ Zloof, IBM 1977
    * Quel introduced in 1974 by the U.C. Berkeley Ingres project.
    * Tutorial_D
    * XQuery
***** Distributed SQL processing[edit] *****
Distributed_Relational_Database_Architecture (DRDA) was designed by a work
group within IBM in the period 1988 to 1994. DRDA enables network connected
relational databases to cooperate to fulfill SQL requests.[44][45]
An interactive user or program can issue SQL statements to a local RDB and
receive tables of data and status indicators in reply from remote RDBs. SQL
statements can also be compiled and stored in remote RDBs as packages and then
invoked by package name. This is important for the efficient operation of
application programs that issue complex, high-frequency queries. It is
especially important when the tables to be accessed are located in remote
systems.
The messages, protocols, and structural components of DRDA are defined by the
Distributed_Data_Management_Architecture.
***** Criticisms[edit] *****
Chamberlin's 2012 paper[15] discusses four historical criticisms of SQL:
**** Orthogonality and completeness[edit] ****
Early specifications did not support major features, such as primary keys.
Result sets could not be named, and sub-queries had not been defined. These
were added in 1992.[15]
**** NULLs[edit] ****
SQL's controversial "NULL" and three-value logic. Predicates evaluated over
nulls return the logical value of "unknown" rather than true or false. Features
such as outer-join depend on nulls. Null is not equivalent to space. NULL
represents no data in the row.
**** Duplicates[edit] ****
Another popular criticism is that it allows duplicate rows, making integration
with languages such as Python, whose data types might make it difficult to
accurately represent the data,[15] difficult in terms of parsing and by the
absence of modularity.[46]
This can be avoided declaring a unique constraint with one or more fields that
identifies uniquely a row in the table. That constraint could became also the
primary key of the table.
**** Impedance mismatch[edit] ****
In a similar sense to Object-relational_impedance_mismatch, there is a mismatch
between the declarative SQL language and the procedural languages that SQL is
typically embedded in.
***** See also[edit] *****
[icon]     * Book:_SQL
    * Comparison_of_object-relational_database_management_systems
    * Comparison_of_relational_database_management_systems
    * D_(data_language_specification)
    * D4_(programming_language)
    * Hierarchical_model
    * List_of_relational_database_management_systems
    * MUMPS
    * NoSQL
    * Query_by_Example
    * Transact-SQL
    * Online_analytical_processing (OLAP)
    * Online_transaction_processing (OLTP)
    * Data_warehouse
    * Relational_data_stream_management_system
    * Star_schema
    * Snowflake_schema
***** Notes[edit] *****
   1. ^ Formally, "SQL-data" statements excluding "SQL-data change" statements;
      this is primarily the Select statement.
   2. ^ Formally, "SQL-schema" statements.
   3. ^ Formally, "SQL-data change" statements
***** References[edit] *****
   1. ^"Media_Type_registration_for_application/sql". Internet_Assigned_Numbers
      Authority. 10 April 2013. Retrieved 10 April 2013.
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
   3. ^"The_application/sql_Media_Type,_RFC_6922". Internet_Engineering_Task
      Force. April 2013. p. 3. Retrieved 10 April 2013.
   4. ^Paul, Ryan. "A_guided_tour_of_the_Microsoft_Command_Shell". Ars
      Technica. Retrieved 10 April 2011.
   5. ^Beaulieu, Alan (April 2009). Mary E Treseler (ed.). Learning SQL (2nd
      ed.). Sebastapol, CA, USA: O'Reilly. ISBN 978-0-596-52083-0.
   6. ^"SQL". Britannica.com. Retrieved 2013-04-02.
   7. ^"SQL". Oxforddictionaries.com. Retrieved 2017-01-16.
   8. ^"SQL_Guide". Publib.boulder.ibm.com. Retrieved 2017-01-16.
   9. ^"Structured_Query_Language_(SQL)". Msdn.microsoft.com. Retrieved 2017-
      01-16.
  10. ^ SQL-92, 4.22 SQL-statements, 4.22.1 Classes of SQL-statements "There
      are at least five ways of classifying SQL-statements:", 4.22.2, SQL
      statements classified by function "The following are the main classes of
      SQL-statements:"; SQL:2003 4.11 SQL-statements, and later revisions.
  11. ^Chatham, Mark (2012). Structured Query Language By Example - Volume I:
      Data Query Language. p. 8. ISBN 978-1-29119951-2.
  12. ^Codd, Edgar F. (June 1970). "A Relational Model of Data for Large Shared
      Data Banks". Communications of the ACM. 13 (6): 377â87.
      CiteSeerX 10.1.1.88.646. doi:10.1145/362384.362685.
  13. ^ a bChapple, Mike. "SQL_Fundamentals". Databases. About.com. Retrieved
      2009-01-28.
  14. ^"Structured_Query_Language_(SQL)". International Business Machines.
      October 27, 2006. Retrieved 2007-06-10.
  15. ^ a b"ISO_9075:1987:_Information_technology â_Database_languages â
      SQL â_Part_1:_Framework_(SQL/Framework)". 1987-06-01.
  16. ^ a b c d e fChamberlin, Donald (2012). "Early_History_of_SQL". IEEE
      Annals of the History of Computing. 34 (4): 78â82. doi:10.1109/
      MAHC.2012.61. Retrieved 3 February 2018.
  17. ^ a b c dChamberlin, Donald D; Boyce, Raymond F (1974). "SEQUEL:_A
      Structured_English_Query_Language" (PDF). Proceedings of the 1974 ACM
      SIGFIDET Workshop on Data Description, Access and Control. Association
      for Computing Machinery: 249â64. Retrieved 2007-06-09.
  18. ^ a bOppel, Andy (February 27, 2004). Databases_Demystified. San
      Francisco,_CA: McGraw-Hill Osborne Media. pp. 90â1. ISBN 978-0-07-
      146960-9.
  19. ^"History_of_IBM,_1978". IBM Archives. IBM. Retrieved 2007-06-09.
  20. ^ ANSI/ISO/IEC International Standard (IS). Database Language SQLâPart
      2: Foundation (SQL/Foundation). 1999.
  21. ^"IBM_PureData_System_for_Analytics,_Version_7.0.3".
  22. ^"Invantive_Procedural_SQL".
  23. ^"CREATE_PROCEDURE". MariaDB KnowledgeBase. Retrieved 2019-04-23.
  24. ^PostgreSQL contributors (2011). "PostgreSQL_server_programming".
      PostgreSQL 9.1 official documentation. postgresql.org. Retrieved 2012-03-
      09.
  25. ^PostgreSQL contributors (2012). "About_PostgreSQL". PostgreSQL 9.1
      official website. PostgreSQL Global Development Group. Retrieved March 9,
      2012. PostgreSQL prides itself in standards compliance. Its SQL
      implementation strongly conforms to the ANSI-SQL:2008 standard
  26. ^"Mimer_SQL,_Built_on_Standards". Mimer SQL official website. Mimer
      Information Technology. 2009.
  27. ^"4.1._Lexical_Structure". PostgreSQL documentation. 2018.
  28. ^"(Second_Informal_Review_Draft)_ISO/IEC_9075:1992,_Database_Language
      SQL,_Section_5.2,_syntax_rule_11". 30 July 1992.
  29. ^Lorentz, Diana; Roeser, Mary Beth; Abraham, Sundeep; Amor, Angela;
      Arora, Geeta; Arora, Vikas; Ashdown, Lance; Baer, Hermann; Bellamkonda,
      Shrikanth (October 2010) [1996]. "Basic_Elements_of_Oracle_SQL:_Data
      Types". Oracle Database SQL Language Reference 11g Release 2 (11.2).
      Oracle Database Documentation Library. Redwood City, CA: Oracle USA, Inc.
      Retrieved December 29, 2010. For each DATE value, Oracle stores the
      following information: century, year, month, date, hour, minute, and
      second
  30. ^Lorentz, Diana; Roeser, Mary Beth; Abraham, Sundeep; Amor, Angela;
      Arora, Geeta; Arora, Vikas; Ashdown, Lance; Baer, Hermann; Bellamkonda,
      Shrikanth (October 2010) [1996]. "Basic_Elements_of_Oracle_SQL:_Data
      Types". Oracle Database SQL Language Reference 11g Release 2 (11.2).
      Oracle Database Documentation Library. Redwood City, CA: Oracle USA, Inc.
      Retrieved December 29, 2010. The datetime data types are DATE...
  31. ^Lorentz, Diana; Roeser, Mary Beth; Abraham, Sundeep; Amor, Angela;
      Arora, Geeta; Arora, Vikas; Ashdown, Lance; Baer, Hermann; Bellamkonda,
      Shrikanth (October 2010) [1996]. "Basic_Elements_of_Oracle_SQL:_Data
      Types". Oracle Database SQL Language Reference 11g Release 2 (11.2).
      Oracle Database Documentation Library. Redwood City, CA: Oracle USA, Inc.
      Retrieved December 29, 2010. Do not define columns with the following
      SQL/DS and DB2 data types, because they have no corresponding Oracle data
      type:... TIME
  32. ^"Finding_Aid". X3H2 Records, 1978â95. American National Standards
      Institute.
  33. ^Doll, Shelley (June 19, 2002). "Is_SQL_a_Standard_Anymore?".
      TechRepublic's Builder.com. TechRepublic. Archived from the_original on
      2012-07-05. Retrieved 2016-04-12.
  34. ^ a bGillespie, Patrick. "Pronouncing_SQL:_S-Q-L_or_Sequel?". Retrieved
      12 February 2012.
  35. ^Melton, Jim; Alan R Simon (1993). "1.2. What is SQL?". Understanding the
      New SQL: A Complete Guide. Morgan Kaufmann. p. 536. ISBN 978-1-55860-245-
      8. SQL (correctly pronounced "ess cue ell," instead of the somewhat
      common "sequel")...
  36. ^ a bWagner, Michael (2010). SQL/XML:2006 - Evaluierung der
      StandardkonformitÃ¤t ausgewÃ¤hlter Datenbanksysteme. Diplomica Verlag.
      p. 100. ISBN 978-3-8366-9609-8.
  37. ^"SQL:2008_now_an_approved_ISO_international_standard". Sybase. July
      2008. Archived from the_original on 2011-06-28.
  38. ^Krishna Kulkarni, Jan-Eike Michels (2012). "Temporal_features_in_SQL:
      2011" (PDF).
  39. ^Fred Zemke (2012). "What's_new_in_SQL:2011" (PDF).
  40. ^"ISO/IEC_9075-2:2016:_Information_technology_--_Database_languages_-
      -_SQL_--_Part_2:_Foundation_(SQL/Foundation)". December 2016.
  41. ^"SQL:2008_draft" (Zip). Whitemarsh Information Systems Corporation.
  42. ^"ISO/IEC_9075-1:2016:_Information_technology â_Database_languages â
      SQL â_Part_1:_Framework_(SQL/Framework)".
  43. ^"ISO/IEC 9075-11:2008: Information and Definition Schemas (SQL/
      Schemata)". 2008: 1.
  44. ^Fernando Saenz-Perez. "Outer_Joins_in_a_Deductive_Database_System"
      (PDF). Lbd.udc.es. Retrieved 2017-01-16.
  45. ^Reinsch, R. (1988). "Distributed database for SAA". IBM Systems Journal.
      27 (3): 362â389. doi:10.1147/sj.273.0362.
  46. ^Distributed Relational Database Architecture Reference. IBM Corp. SC26-
      4651-0. 1990.
  47. ^Schauder, Jen. "Why_SQL_Sucks". Schauderhaft. Retrieved 3 February 2018.
***** Sources[edit] *****
    * Codd, Edgar F (June 1970). "A_Relational_Model_of_Data_for_Large_Shared
      Data_Banks". Communications of the ACM. 13 (6): 377â87. doi:10.1145/
      362384.362685. Archived from the_original on 2007-06-12.
Discussion_on_alleged_SQL_flaws (C2 wiki)
C._J._Date with Hugh_Darwen: A Guide to the SQL standard : a users guide to the
standard database language SQL, 4th ed., Addison Wesley, USA 1997,
ISBN 978-0-201-96426-4
**** SQL standards documents[edit] ****
*** ITTF publicly available standards and technical reports[edit] ***
The ISO/IEC Information_Technology_Task_Force publishes publicly_available
standards including SQL. Technical Corrigenda (corrections) and Technical
Reports (discussion documents) are published there.
SQL_--_Part_1:_Framework_(SQL/Framework)
*** Draft documents[edit] ***
Formal SQL standards are available from ISO and ANSI for a fee. For informative
use, as opposed to strict standards compliance, late drafts often suffice.
    * SQL:2011_draft
    * SQL-92_draft
***** External links[edit] *****
SQLat Wikipedia's sister_projects
    * Definitions from Wiktionary
    * Media from Wikimedia Commons
    * Textbooks from Wikibooks
    * Resources from Wikiversity
    * 1995_SQL_Reunion:_People,_Projects,_and_Politics,_by_Paul_McJones_(ed.):
      transcript of a reunion meeting devoted to the personal history of
      relational databases and SQL.
    * American_National_Standards_Institute._X3H2_Records,_1978â1995 Charles
      Babbage_Institute Collection documents the H2 committee's development of
      the NDL and SQL standards.
    * Oral_history_interview_with_Donald_D._Chamberlin Charles_Babbage
      Institute In this oral history Chamberlin recounts his early life, his
      education at Harvey_Mudd_College and Stanford_University, and his work on
      relational database technology. Chamberlin was a member of the System R
      research team and, with Raymond_F._Boyce, developed the SQL database
      language. Chamberlin also briefly discusses his more recent research on
      XML query languages.
    * Comparison_of_Different_SQL_Implementations This comparison of various
      SQL implementations is intended to serve as a guide to those interested
      in porting SQL code between various RDBMS products, and includes
      comparisons between SQL:2008, PostgreSQL, DB2, MS SQL Server, MySQL,
      Oracle, and Informix.
    * Event_stream_processing_with_SQL - An introduction to real-time
      processing of streaming data with continuous SQL queries
    * BNF_Grammar_for_ISO/IEC_9075:2003,_part_2_SQL/Framework
    * v
    * t
    * e
SQL
                      * SQL-86
                      * SQL-89
                      * SQL-92
                      * SQL:1999
Versions              * SQL:2003
                      * SQL:2006
                      * SQL:2008
                      * SQL:2011
                      * SQL:2016
                  As
                  Case
                  Create
                  Delete
                  From
                  Having
                  Insert
                  Join
Keywords          Merge
                  Null
                  Order_by
                  Prepare
                  Select
                  Truncate
                  Union
                  Update
                  Where
                  With
Related               * Edgar_Codd
                      * Relational_database
                      * Framework
                      * Foundation
                      * Call-Level_Interface
                      * Persistent_Stored_Modules
ISO/IEC SQL parts     * Management_of_External_Data
                      * Object_Language_Bindings
                      * Information_and_Definition_Schemas
                      * SQL_Routines_and_Types_for_the_Java_Programming
                        Language
                      * XML-Related_Specifications
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
                   * Relational_model
                   * Object-relational_database
                   * Transaction_processing
    * v
    * t
    * e
Query_languages
                   * .QL
                   * ALPHA
                   * CQL
                   * Cypher
                   * D
                   * DMX
                   * Datalog
                   * GraphQL
                   * Gremlin
                   * ISBL
                   * LDAP
In current use     * LINQ
                   * MQL
                   * MDX
                   * OQL
                   * OCL
                   * QUEL
                   * SMARTS
                   * SPARQL
                   * SQL
                   * XQuery
                   * XPath
                   * YQL
Proprietary        * YQL
                   * LINQ
Superseded         * CODASYL
    * v
    * t
    * e
IBM
                * History_of_IBM
History         * Mergers_and_acquisitions
                * Think (motto)
                * Operating_Systems
                * IBM_Cloud
                * IBM_Cognos_Analytics
                * Watson
                * Cell_microprocessor
                * Power_Systems
                * Personal_Computer
                * Mainframe
                * Information_Management_Software
                * Lotus_Software
                * Rational_Software
                * SPSS
Products        * ILOG
                * Tivoli_Software: Service_Automation_Manager
                * WebSphere
                * alphaWorks
                * Criminal_Reduction_Utilising_Statistical
                  History
                * Mashup_Center
                * PureQuery
                * Redbooks
                * FlashSystem
                * Fortran
                * Connections
                * Q_System_One
                * IBM_Aspera
                * Center_for_The_Business_of_Government
                * Global_Services
                * IBM_Hybrid_Cloud
Business        * International_subsidiaries
entities        * jStart
                * Kenexa
                * Research
                * The_Weather_Company (Weather_Underground)
                * Watson_Health
                * Towers
                      o 1250_RenÃ©-LÃ©vesque,_Montreal,_QC
                      o One_Atlantic_Center,_Atlanta,_GA
                * Software Labs
                      o Rome_Software_Lab
                      o Toronto_Software_Lab
                * IBM Buildings
                      o 330_North_Wabash,_Chicago,_IL
                      o Johannesburg
                      o Seattle
                * Research Labs
                      o Africa
                      o Almaden
                      o Austin_Laboratory
                      o Australia
Facilities            o Brazil
                      o China_Laboratory
                      o Haifa_Laboratory
                      o India_Laboratory
                      o Ireland
                      o Thomas_J._Watson_Center,_New_York
                      o Tokyo
                      o Zurich_Laboratory
                * Facilities
                      o Hakozaki_Facility
                      o Yamato_Facility
                * Cambridge_Scientific_Center
                * IBM_Hursley
                * Canada_Head_Office_Building                  [IBM_logo.svg]
                * IBM_Rochester
                * Somers_Office_Complex
                * Academy_of_Technology
                * Centers_for_Advanced_Studies: CASCON
                * Deep_Thunder
                * IBM_Fellow
                * Pulse_conference
Initiatives     * The_Great_Mind_Challenge
                * DeveloperWorks: Develothon
                * Linux_Technology_Center
                * IBM_Virtual_Universe_Community
                * Smarter_Planet
                * World_Community_Grid
                * Automated_teller_machine
                * Electronic_keypunch
                * Hard_disk_drive
                * Floppy_disk
                * DRAM
Inventions      * Relational_model
                * Selectric_typewriter
                * Financial_swaps
                * Universal_Product_Code
                * Magnetic_stripe_card
                * Sabre_airline_reservation_system
                * Scanning_tunneling_microscope
                * Globally_Integrated_Enterprise
Terminology     * Commercial_Processing_Workload
                * Consumability
                * e-business
                * Thomas_J._Watson (1914â1956)
                * Thomas_Watson_Jr. (1956â1971)
                * T._Vincent_Learson (1971â1973)
                * Frank_T._Cary (1973â1981)
CEOs            * John_R._Opel (1981â1985)
                * John_Fellows_Akers (1985â1993)
                * Louis_V._Gerstner_Jr. (1993â2002)
                * Samuel_J._Palmisano (2002â2011)
                * Ginni_Rometty (2012âpresent)
                * Alain_Belda
                * William_R._Brody
                * Kenneth_Chenault
                * Michael_L._Eskew
                * David_Farr
                * Shirley_Ann_Jackson
Board of        * Andrew_N._Liveris
directors       * James_McNerney
                * James_W._Owens
                * Samuel_J._Palmisano
                * Virginia_M._Rometty
                * Joan_E._Spero
                * Sidney_Taurel
                * Lorenzo_Zambrano
                * A_Boy_and_His_Atom
                * Common_Public_License/IBM_Public_License
                * Customer_engineer
                * Deep_Blue
                * Deep_Thought
                * Dynamic_infrastructure
                * GUIDE_International
Other           * IBM_and_the_Holocaust
                * IBM_international_chess_tournament
                * Lucifer_cipher
                * Mathematica
                * IBM_Plex
                * SHARE_computing
                * ScicomP
                * Quantum_Experience
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
                                              * BNE: XX531785
Authority_control [Edit_this_at_Wikidata]     * BNF: cb12101816f (data)
                                              * LCCN: sh86006628

Retrieved from "https://en.wikipedia.org/w/index.php?title=SQL&oldid=909676772"
Categories:
    * Database_management_systems
    * SQL
    * Data_modeling_languages
    * Declarative_programming_languages
    * Programming_languages_with_an_ISO_standard
    * Query_languages
    * Relational_database_management_systems
Hidden categories:
    * Articles_with_short_description
    * Articles_with_hAudio_microformats
    * Pages_including_recorded_pronunciations_(English)
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_April_2019
    * Articles_with_unsourced_statements_from_February_2013
    * Articles_with_unsourced_statements_from_July_2012
    * Wikipedia_articles_with_BNE_identifiers
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Articles_with_example_SQL_code
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
    * Wikibooks
    * Wikiversity
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Alemannisch
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Boarisch
    * Bosanski
    * Brezhoneg
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * Galego
    * å®¢å®¶èª/Hak-kÃ¢-ngÃ®
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Interlingua
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * KurdÃ®
    * ÐÑÑÐ³ÑÐ·ÑÐ°
    * Latina
    * LatvieÅ¡u
    * LietuviÅ³
    * Lumbaart
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * Bahasa_Melayu
    * MÃ¬ng-dÄÌ¤ng-ngá¹³Ì
    * áá¼ááºáá¬áá¬áá¬
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * ÐÐ»ÑÐº_Ð¼Ð°ÑÐ¸Ð¹
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * Tetun
    * à¹à¸à¸¢
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * YorÃ¹bÃ¡
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 6 August 2019, at 22:05 (UTC).
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
