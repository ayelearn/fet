The following text has been accessed from https://en.wikipedia.org/wiki/Relational_algebra at Fri Aug 9 01:11:48 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Relational algebra ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Not to be confused with Relation_algebra.
                    This article's lead_section does not adequately summarize
                    key points of its contents. Please consider expanding the
[Wiki_letter_w.svg] lead to provide_an_accessible_overview of all important
                    aspects of the article. Please discuss this issue on the
                    article's talk_page. (April 2015)
Relational algebra, first created by Edgar_F._Codd while at IBM, is a family of
algebras with a well-founded_semantics used for modelling the data stored in
relational databases, and defining queries on it.
The main application of relational algebra is providing a theoretical
foundation for relational_databases, particularly query_languages for such
databases, chief among which is SQL.
⁰
***** Contents *****
    * 1_Introduction
          o 1.1_Set_operators
          o 1.2_Projection_(Π)
          o 1.3_Selection_(σ)
          o 1.4_Rename_(ρ)
    * 2_Joins_and_join-like_operators
          o 2.1_Natural_join_(â)
          o 2.2_Î¸-join_and_equijoin
          o 2.3_Semijoin_(â)(â)
          o 2.4_Antijoin_(â·)
          o 2.5_Division_(Ã·)
    * 3_Common_extensions
          o 3.1_Outer_joins
                # 3.1.1_Left_outer_join_(â)
                # 3.1.2_Right_outer_join_(â)
                # 3.1.3_Full_outer_join_(â)
          o 3.2_Operations_for_domain_computations
                # 3.2.1_Aggregation
          o 3.3_Transitive_closure
    * 4_Use_of_algebraic_properties_for_query_optimization
          o 4.1_Selection
                # 4.1.1_Basic_selection_properties
                # 4.1.2_Breaking_up_selections_with_complex_conditions
                # 4.1.3_Selection_and_cross_product
                # 4.1.4_Selection_and_set_operators
                # 4.1.5_Selection_and_projection
          o 4.2_Projection
                # 4.2.1_Basic_projection_properties
                # 4.2.2_Projection_and_set_operators
          o 4.3_Rename
                # 4.3.1_Basic_rename_properties
                # 4.3.2_Rename_and_set_operators
          o 4.4_Product_and_union
    * 5_Implementations
    * 6_See_also
    * 7_References
    * 8_Further_reading
    * 9_External_links
***** Introduction[edit] *****
Relational algebra received little attention outside of pure mathematics until
the publication of E.F._Codd's relational_model_of_data in 1970. Codd proposed
such an algebra as a basis for database query languages. (See section
Implementations.)
Five primitive operators of Codd's algebra are the selection, the projection,
the Cartesian_product (also called the cross product or cross join), the set
union, and the set_difference.
**** Set operators[edit] ****
The relational algebra uses set_union, set_difference, and Cartesian_product
from set_theory, but adds additional constraints to these operators.
For set union and set difference, the two relations involved must be union-
compatibleâthat is, the two relations must have the same set of attributes.
Because set_intersection is defined in terms of set union and set difference,
the two relations involved in set intersection must also be union-compatible.
For the Cartesian product to be defined, the two relations involved must have
disjoint headersâthat is, they must not have a common attribute name.
In addition, the Cartesian product is defined differently from the one in set
theory in the sense that tuples are considered to be "shallow" for the purposes
of the operation. That is, the Cartesian product of a set of n-tuples with a
set of m-tuples yields a set of "flattened" (n + m)-tuples (whereas basic set
theory would have prescribed a set of 2-tuples, each containing an n-tuple and
an m-tuple). More formally, R Ã S is defined as follows:
   R &#x00D7; S := { (  r  1   ,  r  2   , &#x2026; ,  r  n   ,  s  1   ,  s  2
, &#x2026; ,  s  m   )  |  (  r  1   ,  r  2   , &#x2026; ,  r  n   ) &#x2208;
R , (  s  1   ,  s  2   , &#x2026; ,  s  m   ) &#x2208; S }   {\displaystyle
R\times S:=\{(r_{1},r_{2},\dots ,r_{n},s_{1},s_{2},\dots ,s_{m})|(r_{1},r_
{2},\dots ,r_{n})\in R,(s_{1},s_{2},\dots ,s_{m})\in S\}}  [R\times S:=\{(r_
{1},r_{2},\dots ,r_{n},s_{1},s_{2},\dots ,s_{m})|(r_{1},r_{2},\dots ,r_{n})\in
R,(s_{1},s_{2},\dots ,s_{m})\in S\}]
The cardinality of the Cartesian product is the product of the cardinalities of
its factors, that is, |R Ã S| = |R| Ã |S|.
**** Projection (Π)[edit] ****
Main article: Projection_(relational_algebra)
A projection is a unary_operation written as      &#x03A0;   a  1   , &#x2026;
,  a  n     ( R )   {\displaystyle \Pi _{a_{1},\ldots ,a_{n}}(R)}  [\Pi_{a_1,
\ldots,a_n}( R )] where      a  1   , &#x2026; ,  a  n     {\displaystyle a_
{1},\ldots ,a_{n}}  [a_1,\ldots,a_n] is a set of attribute names. The result of
such projection is defined as the set that is obtained when all tuples in R are
restricted to the set     {  a  1   , &#x2026; ,  a  n   }   {\displaystyle \
{a_{1},\ldots ,a_{n}\}}  [\{a_{1},\ldots ,a_{n}\}].
Note: when implemented in SQL standard the "default projection" returns a
multiset instead of a set, and the Π projection is obtained by the addition of
the DISTINCT_keyword to eliminate duplicate data.
**** Selection (σ)[edit] ****
Main article: Selection_(relational_algebra)
A generalized selection is a unary_operation written as      &#x03C3;  &#x03C6;
( R )   {\displaystyle \sigma _{\varphi }(R)}  [\sigma_\varphi(R)] where Ï is
a propositional_formula that consists of atoms as allowed in the normal
selection and the logical operators     &#x2227;   {\displaystyle \wedge }
[\wedge ] (and),     &#x2228;   {\displaystyle \lor }  [\lor ] (or) and
&#x00AC;   {\displaystyle \neg }  [\neg ] (negation). This selection selects
all those tuples in R for which Ï holds.
To obtain a listing of all friends or business associates in an address book,
the selection might be written as      &#x03C3;   isFriend = true   &#x2228;
isBusinessContact = true    (  addressBook  )   {\displaystyle \sigma _{{\text
{isFriend = true}}\,\lor \,{\text{isBusinessContact = true}}}({\text
{addressBook}})}  [{\displaystyle \sigma _{{\text{isFriend = true}}\,\lor \,
{\text{isBusinessContact = true}}}({\text{addressBook}})}]. The result would be
a relation containing every attribute of every unique record where isFriend is
true or where isBusinessContact is true.
**** Rename (ρ)[edit] ****
Main article: Rename_(relational_algebra)
A rename is a unary_operation written as      &#x03C1;  a  /  b   ( R )
{\displaystyle \rho _{a/b}(R)}  [\rho_{a / b}(R)] where the result is identical
to R except that the b attribute in all tuples is renamed to an a attribute.
This is simply used to rename the attribute of a relation or the relation
itself.
To rename the 'isFriend' attribute to 'isBusinessContact' in a relation,
&#x03C1;  isBusinessContact / isFriend   (  addressBook  )   {\displaystyle
\rho _{\text{isBusinessContact / isFriend}}({\text{addressBook}})}  [\rho_
{\text{isBusinessContact / isFriend} } ( \text{addressBook} )] might be used.
***** Joins and join-like operators[edit] *****
**** Natural join (â)[edit] ****
"Natural join" redirects here. For the SQL implementation, see Natural_join_
(SQL).
Natural join (â) is a binary_operator that is written as (R â S) where R
and S are relations.[1] The result of the natural join is the set of all
combinations of tuples in R and S that are equal on their common attribute
names. For an example consider the tables Employee and Dept and their natural
join:
       Employee               Dept              Employee â Dept
Name    EmpId DeptName DeptName   Manager Name    EmpId DeptName Manager
Harry   3415  Finance  Finance    George  Harry   3415  Finance  George
Sally   2241  Sales    Sales      Harriet Sally   2241  Sales    Harriet
George  3401  Finance  Production Charles George  3401  Finance  George
Harriet 2202  Sales                       Harriet 2202  Sales    Harriet
This can also be used to define composition_of_relations. For example, the
composition of Employee and Dept is their join as shown above, projected on all
but the common attribute DeptName. In category_theory, the join is precisely
the fiber_product.
The natural join is arguably one of the most important operators since it is
the relational counterpart of logical AND. Note carefully that if the same
variable appears in each of two predicates that are connected by AND, then that
variable stands for the same thing and both appearances must always be
substituted by the same value. In particular, natural join allows the
combination of relations that are associated by a foreign_key. For example, in
the above example a foreign key probably holds from Employee.DeptName to
Dept.DeptName and then the natural join of Employee and Dept combines all
employees with their departments. This works because the foreign key holds
between attributes with the same name. If this is not the case such as in the
foreign key from Dept.Manager to Employee.Name then we have to rename these
columns before we take the natural join. Such a join is sometimes also referred
to as an equijoin (see Î¸-join).
More formally the semantics of the natural join are defined as follows:
         R &#x22C8; S =  {  r &#x222A; s &#xA0; | &#xA0; r &#x2208; R
      &#xA0; &#x2227; &#xA0; s &#x2208; S &#xA0; &#x2227; &#xA0;   F
      u n   ( r &#x222A; s )  }    {\displaystyle R\bowtie S=\left\      
      {r\cup s\ \vert \ r\in R\ \land \ s\in S\ \land \ {\mathit           (1)
      {Fun}}(r\cup s)\right\}}  [R \bowtie S = \left\{ r \cup s \
      \vert \ r \in R \ \land \ s \in S \ \land \ \mathit{Fun}(r \cup
      s) \right\}]
where Fun is a predicate that is true for a relation t (in the mathematical
sense) iff t is a function. It is usually required that R and S must have at
least one common attribute, but if this constraint is omitted, and R and S have
no common attributes, then the natural join becomes exactly the Cartesian
product.
The natural join can be simulated with Codd's primitives as follows. Assume
that c1,...,cm are the attribute names common to R and S, r1,...,rn are the
attribute names unique to R and s1,...,sk are the attribute names unique to S.
Furthermore, assume that the attribute names x1,...,xm are neither in R nor in
S. In a first step we can now rename the common attribute names in S:
         T =  &#x03C1;   x  1    /   c  1   , &#x2026; ,  x  m    /
      c  m     ( S ) =  &#x03C1;   x  1    /   c  1     (  &#x03C1;
      x  2    /   c  2     ( &#x2026;  &#x03C1;   x  m    /   c  m
      ( S ) &#x2026; ) )   {\displaystyle T=\rho _{x_{1}/c_{1},\ldots    (2)
      ,x_{m}/c_{m}}(S)=\rho _{x_{1}/c_{1}}(\rho _{x_{2}/c_{2}}(\ldots    
      \rho _{x_{m}/c_{m}}(S)\ldots ))}  [T=\rho _{x_{1}/c_{1},\ldots
      ,x_{m}/c_{m}}(S)=\rho _{x_{1}/c_{1}}(\rho _{x_{2}/c_{2}}(\ldots
      \rho _{x_{m}/c_{m}}(S)\ldots ))]
Then we take the Cartesian product and select the tuples that are to be joined:
         P =  &#x03C3;   c  1   =  x  1   , &#x2026; ,  c  m   =  x
      m     ( R &#x00D7; T ) =  &#x03C3;   c  1   =  x  1
      (  &#x03C3;   c  2   =  x  2     ( &#x2026;  &#x03C3;   c  m
      =  x  m     ( R &#x00D7; T ) &#x2026; ) )   {\displaystyle         
      P=\sigma _{c_{1}=x_{1},\ldots ,c_{m}=x_{m}}(R\times T)=\sigma _      (3)
      {c_{1}=x_{1}}(\sigma _{c_{2}=x_{2}}(\ldots \sigma _{c_{m}=x_
      {m}}(R\times T)\ldots ))}  [P=\sigma _{c_{1}=x_{1},\ldots ,c_
      {m}=x_{m}}(R\times T)=\sigma _{c_{1}=x_{1}}(\sigma _{c_{2}=x_
      {2}}(\ldots \sigma _{c_{m}=x_{m}}(R\times T)\ldots ))]
Finally we take a projection to get rid of the renamed attributes:
         U =  &#x03C0;   r  1   , &#x2026; ,  r  n   ,  c  1   ,
      &#x2026; ,  c  m   ,  s  1   , &#x2026; ,  s  k     ( P )        
      {\displaystyle U=\pi _{r_{1},\ldots ,r_{n},c_{1},\ldots ,c_        (4)
      {m},s_{1},\ldots ,s_{k}}(P)}  [U=\pi _{r_{1},\ldots ,r_{n},c_
      {1},\ldots ,c_{m},s_{1},\ldots ,s_{k}}(P)]
**** Î¸-join and equijoin[edit] ****
Consider tables Car and Boat which list models of cars and boats and their
respective prices. Suppose a customer wants to buy a car and a boat, but she
does not want to spend more money for the boat than for the car. The Î¸-join
(âÎ¸) on the predicate CarPrice â¥ BoatPrice produces the flattened pairs of
rows which satisfy the predicate. When using a condition where the attributes
are equal, for example Price, then the condition may be specified as
Price=Price or alternatively (Price) itself.
                                            C a r &#x22C8; B o a t   C a r
                                      P r i c e &#x2265; B o a t P r i c e
                                      {\displaystyle {Car\bowtie Boat \atop
       Car               Boat         \scriptstyle CarPrice\geq BoatPrice}}
CarModel CarPrice BoatModel BoatPrice   [{\displaystyle {Car\bowtie Boat
CarA     20,000   Boat1     10,000       \atop \scriptstyle CarPrice\geq
CarB     30,000   Boat2     40,000                BoatPrice}}]
CarC     50,000   Boat3     60,000    CarModel CarPrice BoatModel BoatPrice
                                      CarA     20,000   Boat1     10,000
                                      CarB     30,000   Boat1     10,000
                                      CarC     50,000   Boat1     10,000
                                      CarC     50,000   Boat2     40,000
If we want to combine tuples from two relations where the combination condition
is not simply the equality of shared attributes then it is convenient to have a
more general form of join operator, which is the Î¸-join (or theta-join). The
Î¸-join is a binary operator that is written as        R &#xA0; &#x22C8; &#xA0;
S   a &#xA0; &#x03B8; &#xA0; b      {\displaystyle {R\ \bowtie \ S \atop a\
\theta \ b}}  [{\displaystyle {R\ \bowtie \ S \atop a\ \theta \ b}}] or
R &#xA0; &#x22C8; &#xA0; S   a &#xA0; &#x03B8; &#xA0; v      {\displaystyle {R\
\bowtie \ S \atop a\ \theta \ v}}  [{\displaystyle {R\ \bowtie \ S \atop a\
\theta \ v}}] where a and b are attribute names, Î¸ is a binary relational
operator in the set {<, â¤, =, â , >, â¥}, v is a value constant, and R and
S are relations. The result of this operation consists of all combinations of
tuples in R and S that satisfy Î¸. The result of the Î¸-join is defined only if
the headers of S and R are disjoint, that is, do not contain a common
attribute.
The simulation of this operation in the fundamental operations is therefore as
follows:
      R âÎ¸ S = ÏÎ¸(R Ã S)
In case the operator Î¸ is the equality operator (=) then this join is also
called an equijoin.
Note, however, that a computer language that supports the natural join and
selection operators does not need Î¸-join as well, as this can be achieved by
selection from the result of a natural join (which degenerates to Cartesian
product when there are no shared attributes).
In SQL implementations, joining on a predicate is usually called an inner join,
and the on keyword allows one to specify the predicate used to filter the rows.
It is important to note: forming the flattened Cartesian product then filtering
the rows is conceptually correct, but an implementation would use more
sophisticated data structures to speed up the join query.
**** Semijoin (â)(â)[edit] ****
The left semijoin is a joining similar to the natural join and written as R â
S where R and S are relations.[2] The result is the set of all tuples in R for
which there is a tuple in S that is equal on their common attribute names. The
difference from a natural join is that other columns of S do not appear. For
example, consider the tables Employee and Dept and their semijoin:
        Employee
Name    EmpId DeptName          Dept           Employee â Dept
Harry   3415  Finance    DeptName   Manager Name    EmpId DeptName
Sally   2241  Sales      Sales      Sally   Sally   2241  Sales
George  3401  Finance    Production Harriet Harriet 2202  Production
Harriet 2202  Production
More formally the semantics of the semijoin can be defined as follows:
      R â S = { t : t ∈ R ∧ ∃s ∈ S(Fun (t ∪ s)) }
where Fun(r) is as in the definition of natural join.
The semijoin can be simulated using the natural join as follows. If a1, ..., an
are the attribute names of R, then
      R â S = πa1,..,an(R â S).
Since we can simulate the natural join with the basic operators it follows that
this also holds for the semijoin.
In Codd's 1970 paper, semijoin is called restriction.[3]
**** Antijoin (â·)[edit] ****
The antijoin, written as R â· S where R and S are relations, is similar to the
semijoin, but the result of an antijoin is only those tuples in R for which
there is no tuple in S that is equal on their common attribute names.[4]
For an example consider the tables Employee and Dept and their antijoin:
        Employee
Name    EmpId DeptName          Dept          Employee â· Dept
Harry   3415  Finance    DeptName   Manager Name   EmpId DeptName
Sally   2241  Sales      Sales      Sally   Harry  3415  Finance
George  3401  Finance    Production Harriet George 3401  Finance
Harriet 2202  Production
The antijoin is formally defined as follows:
      R â· S = { t : t ∈ R ∧ ¬∃s ∈ S(Fun (t ∪ s)) }
or
      R â· S = { t : t ∈ R, there is no tuple s of S that satisfies Fun (t ∪
      s) }
where Fun (t ∪ s) is as in the definition of natural join.
The antijoin can also be defined as the complement of the semijoin, as follows:
      R â· S = R − R   (5)
                               
Given this, the antijoin is sometimes called the anti-semijoin, and the
antijoin operator is sometimes written as semijoin symbol with a bar above it,
instead of â·.
**** Division (Ã·)[edit] ****
The division is a binary operation that is written as R Ã· S. Division is not
implemented directly in SQL. The result consists of the restrictions of tuples
in R to the attribute names unique to R, i.e., in the header of R but not in
the header of S, for which it holds that all their combinations with tuples in
S are present in R. For an example see the tables Completed, DBProject and
their division:
    Completed
Student Task                Completed
Fred    Database1 DBProject   Ã·
Fred    Database2 Task      DBProject
Fred    Compiler1 Database1 Student
Eugene  Database1 Database2 Fred
Eugene  Compiler1           Sarah
Sarah   Database1
Sarah   Database2
If DBProject contains all the tasks of the Database project, then the result of
the division above contains exactly the students who have completed both of the
tasks in the Database project. More formally the semantics of the division is
defined as follows:
      R Ã· S = { t[a1,...,an] : t â R â§ âs â S ( (t[a1,...,an] âª    (6) R) }
                                                                                                
where {a1,...,an} is the set of attribute names unique to R and t[a1,...,an] is
the restriction of t to this set. It is usually required that the attribute
names in the header of S are a subset of those of R because otherwise the
result of the operation will always be empty.
The simulation of the division with the basic operations is as follows. We
assume that a1,...,an are the attribute names unique to R and b1,...,bm are the
attribute names of S. In the first step we project R on its unique attribute
names and construct all combinations with tuples in S:
      T := Ïa1,...,an(R) Ã S
In the prior example, T would represent a table such that every Student
(because Student is the unique key / attribute of the Completed table) is
combined with every given Task. So Eugene, for instance, would have two rows,
Eugene → Database1 and Eugene → Database2 in T.
            EG: First, let's pretend that "Completed" has a third attribute
            called "grade". It's unwanted baggage here, so we must project it
            off always. In fact in this step we can drop 'Task' from R as well;
            the multiply puts it back on.
            T := ÏStudent(R) Ã S // This gives us every possible desired
            combination, including those that don't actually exist in R, and
            excluding others (eg Fred | compiler1, which is not a desired
            combination)
        T
Student Task
Fred    Database1
Fred    Database2
Eugene  Database1
Eugene  Database2
Sarah   Database1
Sarah   Database2
In the next step we subtract R from T
relation:
      U := T − R
In U we have the possible combinations that "could have" been in R, but
weren't.
            EG: Again with projections â T and R need to have identical
            attribute names/headers.
            U := T − ÏStudent,Task(R) // This gives us a "what's missing"
            list.
                      R a.k.a.
        T             Completed
Student Task      Student Task
Fred    Database1 Fred    Database1         U
Fred    Database2 Fred    Database2 Student Task
Eugene  Database1 Fred    Compiler1 Eugene  Database2
Eugene  Database2 Eugene  Database1
Sarah   Database1 Eugene  Compiler1
Sarah   Database2 Sarah   Database1
                  Sarah   Database2
So if we now take the projection on the attribute names unique to R
then we have the restrictions of the tuples in R for which not all combinations
with tuples in S were present in R:
      V := Ïa1,...,an(U)
            EG: Project U down to just the attribute(s) in question (Student)
            V := ÏStudent(U)
   V
Student
Eugene
So what remains to be done is take the projection of R on its unique attribute
names and subtract those in V:
      W := Ïa1,...,an(R) − V
            EG: W := ÏStudent(R) − V.
ÏStudent
  (R)          V       W
Student     Student Student
Fred        Eugene  Fred
Eugene              Sarah
Sarah
***** Common extensions[edit] *****
In practice the classical relational algebra described above is extended with
various operations such as outer joins, aggregate functions and even transitive
closure.[5]
**** Outer joins[edit] ****
Main article: Outer_join
Whereas the result of a join (or inner join) consists of tuples formed by
combining matching tuples in the two operands, an outer join contains those
tuples and additionally some tuples formed by extending an unmatched tuple in
one of the operands by "fill" values for each of the attributes of the other
operand. Outer joins are not considered part of the classical relational
algebra discussed so far.[6]
The operators defined in this section assume the existence of a null value, Ï,
which we do not define, to be used for the fill values; in practice this
corresponds to the NULL in SQL. In order to make subsequent selection
operations on the resulting table meaningful, a semantic meaning needs to be
assigned to nulls; in Codd's approach the propositional logic used by the
selection is extended_to_a_three-valued_logic, although we elide those details
in this article.
Three outer join operators are defined: left outer join, right outer join, and
full outer join. (The word "outer" is sometimes omitted.)
*** Left outer join (â)[edit] ***
The left outer join is written as R â S where R and S are relations.[7] The
result of the left outer join is the set of all combinations of tuples in R and
S that are equal on their common attribute names, in addition (loosely
speaking) to tuples in R that have no matching tuples in S.
For an example consider the tables Employee and Dept and their left outer join:
       Employee                                   Employee â Dept
Name    EmpId DeptName         Dept        Name    EmpId DeptName  Manager
Harry   3415  Finance   DeptName   Manager Harry   3415  Finance   Ï
Sally   2241  Sales     Sales      Harriet Sally   2241  Sales     Harriet
George  3401  Finance   Production Charles George  3401  Finance   Ï
Harriet 2202  Sales                        Harriet 2202  Sales     Harriet
Tim     1123  Executive                    Tim     1123  Executive Ï
In the resulting relation, tuples in S which have no common values in common
attribute names with tuples in R take a null value, Ï.
Since there are no tuples in Dept with a DeptName of Finance or Executive, Ïs
occur in the resulting relation where tuples in Employee have a DeptName of
Finance or Executive.
Let r1, r2, ..., rn be the attributes of the relation R and let {(Ï, ..., Ï)}
be the singleton relation on the attributes that are unique to the relation S
(those that are not attributes of R). Then the left outer join can be described
in terms of the natural join (and hence using basic operators) as follows:
         ( R &#x22C8; S ) &#x222A; ( ( R &#x2212;  &#x03C0;   r  1   ,  r  2
      , &#x2026; ,  r  n     ( R &#x22C8; S ) ) &#x00D7; { ( &#x03C9; ,
      &#x2026; &#x03C9; ) } )   {\displaystyle (R\bowtie S)\cup ((R-\pi _{r_
      {1},r_{2},\dots ,r_{n}}(R\bowtie S))\times \{(\omega ,\dots \omega )\})}
      [(R \bowtie S) \cup ((R - \pi_{r_1, r_2, \dots, r_n}(R \bowtie S)) \times
      \{(\omega, \dots \omega)\})]
*** Right outer join (â)[edit] ***
The right outer join behaves almost identically to the left outer join, but the
roles of the tables are switched.
The right outer join of relations R and S is written as R â S.[8] The result
of the right outer join is the set of all combinations of tuples in R and S
that are equal on their common attribute names, in addition to tuples in S that
have no matching tuples in R.
For example, consider the tables Employee and Dept and their right outer join:
       Employee
Name    EmpId DeptName         Dept               Employee â Dept
Harry   3415  Finance   DeptName   Manager Name    EmpId DeptName   Manager
Sally   2241  Sales     Sales      Harriet Sally   2241  Sales      Harriet
George  3401  Finance   Production Charles Harriet 2202  Sales      Harriet
Harriet 2202  Sales                        Ï    Ï  Production Charles
Tim     1123  Executive
In the resulting relation, tuples in R which have no common values in common
attribute names with tuples in S take a null value, Ï.
Since there are no tuples in Employee with a DeptName of Production, Ïs occur
in the Name and EmpId attributes of the resulting relation where tuples in Dept
had DeptName of Production.
Let s1, s2, ..., sn be the attributes of the relation S and let {(Ï, ..., Ï)}
be the singleton relation on the attributes that are unique to the relation R
(those that are not attributes of S). Then, as with the left outer join, the
right outer join can be simulated using the natural join as follows:
         ( R &#x22C8; S ) &#x222A; ( { ( &#x03C9; , &#x2026; , &#x03C9; ) }
      &#x00D7; ( S &#x2212;  &#x03C0;   s  1   ,  s  2   , &#x2026; ,  s  n
      ( R &#x22C8; S ) ) )   {\displaystyle (R\bowtie S)\cup (\{(\omega ,\dots
      ,\omega )\}\times (S-\pi _{s_{1},s_{2},\dots ,s_{n}}(R\bowtie S)))}  [(R
      \bowtie S) \cup (\{(\omega, \dots, \omega)\} \times (S - \pi_{s_1, s_2,
      \dots, s_n}(R \bowtie S)))]
*** Full outer join (â)[edit] ***
âThe outer join or full outer join in effect combines the results of the left
and right outer joins.
The full outer join is written as R â S where R and S are relations.[9] The
result of the full outer join is the set of all combinations of tuples in R and
S that are equal on their common attribute names, in addition to tuples in S
that have no matching tuples in R and tuples in R that have no matching tuples
in S in their common attribute names.
For an example consider the tables Employee and Dept and their full outer join:
       Employee                                   Employee â Dept
Name    EmpId DeptName                     Name    EmpId DeptName   Manager
Harry   3415  Finance          Dept        Harry   3415  Finance    Ï
Sally   2241  Sales     DeptName   Manager Sally   2241  Sales      Harriet
George  3401  Finance   Sales      Harriet George  3401  Finance    Ï
Harriet 2202  Sales     Production Charles Harriet 2202  Sales      Harriet
Tim     1123  Executive                    Tim     1123  Executive  Ï
                                           Ï    Ï  Production Charles
In the resulting relation, tuples in R which have no common values in common
attribute names with tuples in S take a null value, Ï. Tuples in S which have
no common values in common attribute names with tuples in R also take a null
value, Ï.
The full outer join can be simulated using the left and right outer joins (and
hence the natural join and set union) as follows:
      R â S = (R â S) ∪ (R â S)
**** Operations for domain computations[edit] ****
There is nothing in relational algebra introduced so far that would allow
computations on the data domains (other than evaluation of propositional
expressions involving equality). For example, it is not possible using only the
algebra introduced so far to write an expression that would multiply the
numbers from two columns, e.g. a unit price with a quantity to obtain a total
price. Practical query languages have such facilities, e.g. the SQL SELECT
allows arithmetic operations to define new columns in the result SELECT
unit_price * quantity AS total_price FROM t, and a similar facility is provided
more explicitly by Tutorial_D's EXTEND keyword.[10] In database theory, this is
called extended projection.[11]:213
*** Aggregation[edit] ***
Furthermore, computing various functions on a column, like the summing up of
its elements, is also not possible using the relational algebra introduced so
far. There are five aggregate_functions that are included with most relational
database systems. These operations are Sum, Count, Average, Maximum and
Minimum. In relational algebra the aggregation operation over a schema (A1, A2,
... An) is written as follows:
          G  1   ,  G  2   , &#x2026; ,  G  m   &#xA0;  g   f  1   (    A  1
      &#x2032;  ) ,  f  2   (    A  2    &#x2032;  ) , &#x2026; ,  f  k
      (    A  k    &#x2032;  )   &#xA0; ( r )   {\displaystyle G_{1},G_
      {2},\ldots ,G_{m}\ g_{f_{1}({A_{1}}'),f_{2}({A_{2}}'),\ldots ,f_{k}({A_
      {k}}')}\ (r)}  [G_1, G_2, \ldots, G_m\ g_{f_1({A_1}'), f_2({A_2}'),
      \ldots, f_k({A_k}')}\ (r)]
where each Aj', 1 â¤ j â¤ k, is one of the original attributes Ai, 1 â¤ i
â¤ n.
The attributes preceding the g are grouping attributes, which function like a
"group by" clause in SQL. Then there are an arbitrary number of aggregation
functions applied to individual attributes. The operation is applied to an
arbitrary relation r. The grouping attributes are optional, and if they are not
supplied, the aggregation functions are applied across the entire relation to
which the operation is applied.
Let's assume that we have a table named
Account with three columns, namely
Account_Number, Branch_Name and
Balance. We wish to find the maximum balance of each branch. This is
accomplished by
Branch_Name
GMax(
Balance)
(
Account). To find the highest balance of all accounts regardless of branch, we
could simply write GMax(
Balance)
(
Account).
**** Transitive closure[edit] ****
Although relational algebra seems powerful enough for most practical purposes,
there are some simple and natural operators on relations that cannot be
expressed by relational algebra. One of them is the transitive_closure of a
binary relation. Given a domain D, let binary relation R be a subset of D×D.
The transitive closure R+ of R is the smallest subset of D×D that contains R
and satisfies the following condition:
         &#x2200; x &#x2200; y &#x2200; z  (  ( x , y ) &#x2208;  R  +
      &#x2227; ( y , z ) &#x2208;  R  +   &#x21D2; ( x , z ) &#x2208;  R  +
      )    {\displaystyle \forall x\forall y\forall z\left((x,y)\in R^{+}\wedge
      (y,z)\in R^{+}\Rightarrow (x,z)\in R^{+}\right)}  [\forall x \forall y
      \forall z \left( (x,y) \in R^+ \wedge (y,z) \in R^+ \Rightarrow (x,z) \in
      R^+ \right)]
There is no relational algebra expression E(R) taking R as a variable argument
that produces R+. This can be proved using the fact that, given a relational
expression E for which it is claimed that E(R) = R+, where R is a variable, we
can always find an instance r of R (and a corresponding domain d) such that E
(r) â  r+.[12]
SQL however officially supports such fixpoint_queries since 1999, and it had
vendor-specific extensions in this direction well before that.
***** Use of algebraic properties for query optimization[edit] *****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (June 2013)(Learn_how_and_when_to_remove_this_template_message)
Queries can be represented as a tree, where
    * the internal nodes are operators,
    * leaves are relations,
    * subtrees are subexpressions.
Our primary goal is to transform expression trees into equivalent expression
trees, where the average size of the relations yielded by subexpressions in the
tree is smaller than it was before the optimization. Our secondary goal is to
try to form common subexpressions within a single query, or if there is more
than one query being evaluated at the same time, in all of those queries. The
rationale behind the second goal is that it is enough to compute common
subexpressions once, and the results can be used in all queries that contain
that subexpression.
Here we present a set of rules that can be used in such transformations.
**** Selection[edit] ****
Rules about selection operators play the most important role in query
optimization. Selection is an operator that very effectively decreases the
number of rows in its operand, so if we manage to move the selections in an
expression tree towards the leaves, the internal relations (yielded by
subexpressions) will likely shrink.
*** Basic selection properties[edit] ***
Selection is idempotent (multiple applications of the same selection have no
additional effect beyond the first one), and commutative (the order selections
are applied in has no effect on the eventual result).
   1.     &#x03C3;  A   ( R ) =  &#x03C3;  A    &#x03C3;  A   ( R )
      {\displaystyle \sigma _{A}(R)=\sigma _{A}\sigma _{A}(R)\,\!}  [\sigma_{A}
      (R)=\sigma_{A}\sigma_{A}(R)\,\!]
   2.     &#x03C3;  A    &#x03C3;  B   ( R ) =  &#x03C3;  B    &#x03C3;  A
      ( R )     {\displaystyle \sigma _{A}\sigma _{B}(R)=\sigma _{B}\sigma _{A}
      (R)\,\!}  [\sigma_{A}\sigma_{B}(R)=\sigma_{B}\sigma_{A}(R)\,\!]
*** Breaking up selections with complex conditions[edit] ***
A selection whose condition is a conjunction of simpler conditions is
equivalent to a sequence of selections with those same individual conditions,
and selection whose condition is a disjunction is equivalent to a union of
selections. These identities can be used to merge selections so that fewer
selections need to be evaluated, or to split them so that the component
selections may be moved or optimized separately.
   1.     &#x03C3;  A &#x2227; B   ( R ) =  &#x03C3;  A   (  &#x03C3;  B   ( R
      ) ) =  &#x03C3;  B   (  &#x03C3;  A   ( R ) )   {\displaystyle \sigma _
      {A\land B}(R)=\sigma _{A}(\sigma _{B}(R))=\sigma _{B}(\sigma _{A}(R))}
      [\sigma_{A \land B}(R)=\sigma_{A}(\sigma_{B}(R))=\sigma_{B}(\sigma_{A}
      (R))]
   2.     &#x03C3;  A &#x2228; B   ( R ) =  &#x03C3;  A   ( R ) &#x222A;
      &#x03C3;  B   ( R )   {\displaystyle \sigma _{A\lor B}(R)=\sigma _{A}
      (R)\cup \sigma _{B}(R)}  [\sigma_{A \lor B}(R)=\sigma_{A}(R)\cup\sigma_
      {B}(R)]
*** Selection and cross product[edit] ***
Cross product is the costliest operator to evaluate. If the input relations
have N and M rows, the result will contain     N M   {\displaystyle NM}  [NM]
rows. Therefore, it is very important to do our best to decrease the size of
both operands before applying the cross product operator.
This can be effectively done if the cross product is followed by a selection
operator, e.g.      &#x03C3;  A   ( R &#x00D7; P )   {\displaystyle \sigma _{A}
(R\times P)}  [{\displaystyle \sigma _{A}(R\times P)}]. Considering the
definition of join, this is the most likely case. If the cross product is not
followed by a selection operator, we can try to push down a selection from
higher levels of the expression tree using the other selection rules.
In the above case we break up condition A into conditions B, C and D using the
split rules about complex selection conditions, so that     A = B &#x2227; C
&#x2227; D   {\displaystyle A=B\wedge C\wedge D}  [{\displaystyle A=B\wedge
C\wedge D}] and B contains attributes only from R, C contains attributes only
from P, and D contains the part of A that contains attributes from both R and
P. Note, that B, C or D are possibly empty. Then the following holds:
          &#x03C3;  A   ( R &#x00D7; P ) =  &#x03C3;  B &#x2227; C &#x2227; D
      ( R &#x00D7; P ) =  &#x03C3;  D   (  &#x03C3;  B   ( R ) &#x00D7;
      &#x03C3;  C   ( P ) )   {\displaystyle \sigma _{A}(R\times P)=\sigma _
      {B\wedge C\wedge D}(R\times P)=\sigma _{D}(\sigma _{B}(R)\times \sigma _
      {C}(P))}  [\sigma_{A}(R \times P) = \sigma_{B \wedge C \wedge D}(R \times
      P) = \sigma_{D}(\sigma_{B}(R) \times \sigma_{C}(P))]
*** Selection and set operators[edit] ***
Selection is distributive over the set difference, intersection, and union
operators. The following three rules are used to push selection below set
operations in the expression tree. For the set difference and the intersection
operators, it is possible to apply the selection operator to just one of the
operands following the transformation. This can be beneficial where one of the
operands is small, and the overhead of evaluating the selection operator
outweighs the benefits of using a smaller relation as an operand.
   1.     &#x03C3;  A   ( R &#x2216; P ) =  &#x03C3;  A   ( R ) &#x2216;
      &#x03C3;  A   ( P ) =  &#x03C3;  A   ( R ) &#x2216; P   {\displaystyle
      \sigma _{A}(R\setminus P)=\sigma _{A}(R)\setminus \sigma _{A}(P)=\sigma _
      {A}(R)\setminus P}  [\sigma_{A}(R\setminus P)=\sigma_{A}(R)\setminus
      \sigma_{A}(P) =\sigma_{A}(R)\setminus P]
   2.     &#x03C3;  A   ( R &#x222A; P ) =  &#x03C3;  A   ( R ) &#x222A;
      &#x03C3;  A   ( P )   {\displaystyle \sigma _{A}(R\cup P)=\sigma _{A}
      (R)\cup \sigma _{A}(P)}  [\sigma_{A}(R\cup P)=\sigma_{A}(R)\cup\sigma_{A}
      (P)]
   3.     &#x03C3;  A   ( R &#x2229; P ) =  &#x03C3;  A   ( R ) &#x2229;
      &#x03C3;  A   ( P ) =  &#x03C3;  A   ( R ) &#x2229; P = R &#x2229;
      &#x03C3;  A   ( P )   {\displaystyle \sigma _{A}(R\cap P)=\sigma _{A}
      (R)\cap \sigma _{A}(P)=\sigma _{A}(R)\cap P=R\cap \sigma _{A}(P)}
      [\sigma_{A}(R\cap P)=\sigma_{A}(R)\cap\sigma_{A}(P)=\sigma_{A}(R)\cap
      P=R\cap \sigma_{A}(P)]
*** Selection and projection[edit] ***
Selection commutes with projection if and only if the fields referenced in the
selection condition are a subset of the fields in the projection. Performing
selection before projection may be useful if the operand is a cross product or
join. In other cases, if the selection condition is relatively expensive to
compute, moving selection outside the projection may reduce the number of
tuples which must be tested (since projection may produce fewer tuples due to
the elimination of duplicates resulting from omitted fields).
          &#x03C0;   a  1   , &#x2026; ,  a  n     (  &#x03C3;  A   ( R ) ) =
      &#x03C3;  A   (  &#x03C0;   a  1   , &#x2026; ,  a  n     ( R ) )
      &#xA0;where fields in&#xA0;  A &#x2286; {  a  1   , &#x2026; ,  a  n   }
      {\displaystyle \pi _{a_{1},\ldots ,a_{n}}(\sigma _{A}(R))=\sigma _{A}(\pi
      _{a_{1},\ldots ,a_{n}}(R)){\text{ where fields in }}A\subseteq \{a_
      {1},\ldots ,a_{n}\}}  [\pi_{a_1, \ldots ,a_n}(\sigma_A( R )) = \sigma_A
      (\pi_{a_1, \ldots,a_n}( R ))\text{ where fields in }A \subseteq \
      {a_1,\ldots,a_n\}]
**** Projection[edit] ****
*** Basic projection properties[edit] ***
Projection is idempotent, so that a series of (valid) projections is equivalent
to the outermost projection.
          &#x03C0;   a  1   , &#x2026; ,  a  n     (  &#x03C0;   b  1   ,
      &#x2026; ,  b  m     ( R ) ) =  &#x03C0;   a  1   , &#x2026; ,  a  n
      ( R )  &#xA0;where&#xA0;  {  a  1   , &#x2026; ,  a  n   } &#x2286; {  b
      1   , &#x2026; ,  b  m   }   {\displaystyle \pi _{a_{1},\ldots ,a_{n}}
      (\pi _{b_{1},\ldots ,b_{m}}(R))=\pi _{a_{1},\ldots ,a_{n}}(R){\text
      { where }}\{a_{1},\ldots ,a_{n}\}\subseteq \{b_{1},\ldots ,b_{m}\}}
      [\pi_{a_1, \ldots , a_n}(\pi_{b_1,\ldots , b_m}(R)) = \pi_{a_1, \ldots ,
      a_n}(R)\text{ where }\{a_1, \ldots , a_n\} \subseteq \{b_1, \ldots ,
      b_m\}]
*** Projection and set operators[edit] ***
Projection is distributive over set union.
          &#x03C0;   a  1   , &#x2026; ,  a  n     ( R &#x222A; P ) =  &#x03C0;
      a  1   , &#x2026; ,  a  n     ( R ) &#x222A;  &#x03C0;   a  1   ,
      &#x2026; ,  a  n     ( P ) .    {\displaystyle \pi _{a_{1},\ldots ,a_{n}}
      (R\cup P)=\pi _{a_{1},\ldots ,a_{n}}(R)\cup \pi _{a_{1},\ldots ,a_{n}}
      (P).\,}  [\pi_{a_1, \ldots, a_n}(R \cup P) = \pi_{a_1, \ldots, a_n}(R)
      \cup \pi_{a_1, \ldots, a_n}(P). \, ]
Projection does not distribute over intersection and set difference.
Counterexamples are given by:
          &#x03C0;  A   ( { &#x27E8; A = a , B = b &#x27E9; } &#x2229;
      { &#x27E8; A = a , B =  b &#x2032;  &#x27E9; } ) = &#x2205;
      {\displaystyle \pi _{A}(\{\langle A=a,B=b\rangle \}\cap \{\langle
      A=a,B=b'\rangle \})=\emptyset }  [\pi_A(\{ \langle A=a, B=b \rangle \}
      \cap \{ \langle A=a, B=b' \rangle \}) = \emptyset]
          &#x03C0;  A   ( { &#x27E8; A = a , B = b &#x27E9; } ) &#x2229;
      &#x03C0;  A   ( { &#x27E8; A = a , B =  b &#x2032;  &#x27E9; } ) =
      { &#x27E8; A = a &#x27E9; }   {\displaystyle \pi _{A}(\{\langle
      A=a,B=b\rangle \})\cap \pi _{A}(\{\langle A=a,B=b'\rangle \})=\{\langle
      A=a\rangle \}}  [\pi_A(\{ \langle A=a, B=b \rangle \}) \cap \pi_A(\
      { \langle A=a, B=b' \rangle \}) = \{ \langle A=a \rangle \}]
and
          &#x03C0;  A   ( { &#x27E8; A = a , B = b &#x27E9; } &#x2216;
      { &#x27E8; A = a , B =  b &#x2032;  &#x27E9; } ) = { &#x27E8; A = a
      &#x27E9; }   {\displaystyle \pi _{A}(\{\langle A=a,B=b\rangle \}\setminus
      \{\langle A=a,B=b'\rangle \})=\{\langle A=a\rangle \}}  [{\displaystyle
      \pi _{A}(\{\langle A=a,B=b\rangle \}\setminus \{\langle A=a,B=b'\rangle
      \})=\{\langle A=a\rangle \}}]
          &#x03C0;  A   ( { &#x27E8; A = a , B = b &#x27E9; } ) &#x2216;
      &#x03C0;  A   ( { &#x27E8; A = a , B =  b &#x2032;  &#x27E9; } ) =
      &#x2205;  ,   {\displaystyle \pi _{A}(\{\langle A=a,B=b\rangle
      \})\setminus \pi _{A}(\{\langle A=a,B=b'\rangle \})=\emptyset \,,}
      [\pi_A(\{ \langle A=a, B=b \rangle \}) \setminus \pi_A(\{ \langle A=a,
      B=b' \rangle \}) = \emptyset\,,]
where b is assumed to be distinct from b'.
**** Rename[edit] ****
*** Basic rename properties[edit] ***
Successive renames of a variable can be collapsed into a single rename. Rename
operations which have no variables in common can be arbitrarily reordered with
respect to one another, which can be exploited to make successive renames
adjacent so that they can be collapsed.
   1.     &#x03C1;  a  /  b   (  &#x03C1;  b  /  c   ( R ) ) =  &#x03C1;  a  /
      c   ( R )     {\displaystyle \rho _{a/b}(\rho _{b/c}(R))=\rho _{a/c}
      (R)\,\!}  [\rho_{a / b}(\rho_{b / c}(R)) = \rho_{a / c}(R)\,\!]
   2.     &#x03C1;  a  /  b   (  &#x03C1;  c  /  d   ( R ) ) =  &#x03C1;  c  /
      d   (  &#x03C1;  a  /  b   ( R ) )     {\displaystyle \rho _{a/b}(\rho _
      {c/d}(R))=\rho _{c/d}(\rho _{a/b}(R))\,\!}  [\rho_{a / b}(\rho_{c / d}
      (R)) = \rho_{c / d}(\rho_{a / b}(R))\,\!]
*** Rename and set operators[edit] ***
Rename is distributive over set difference, union, and intersection.
   1.     &#x03C1;  a  /  b   ( R &#x2216; P ) =  &#x03C1;  a  /  b   ( R )
      &#x2216;  &#x03C1;  a  /  b   ( P )   {\displaystyle \rho _{a/b}
      (R\setminus P)=\rho _{a/b}(R)\setminus \rho _{a/b}(P)}  [\rho_{a / b}(R
      \setminus P) = \rho_{a / b}(R) \setminus \rho_{a / b}(P)]
   2.     &#x03C1;  a  /  b   ( R &#x222A; P ) =  &#x03C1;  a  /  b   ( R )
      &#x222A;  &#x03C1;  a  /  b   ( P )   {\displaystyle \rho _{a/b}(R\cup
      P)=\rho _{a/b}(R)\cup \rho _{a/b}(P)}  [\rho_{a / b}(R \cup P) = \rho_{a
      / b}(R) \cup \rho_{a / b}(P)]
   3.     &#x03C1;  a  /  b   ( R &#x2229; P ) =  &#x03C1;  a  /  b   ( R )
      &#x2229;  &#x03C1;  a  /  b   ( P )   {\displaystyle \rho _{a/b}(R\cap
      P)=\rho _{a/b}(R)\cap \rho _{a/b}(P)}  [\rho_{a / b}(R \cap P) = \rho_{a
      / b}(R) \cap \rho_{a / b}(P)]
**** Product and union[edit] ****
Cartesian product is distributive over union.
   1.    ( A &#x00D7; B ) &#x222A; ( A &#x00D7; C ) = A &#x00D7; ( B &#x222A; C
      )   {\displaystyle (A\times B)\cup (A\times C)=A\times (B\cup C)}  [
      {\displaystyle (A\times B)\cup (A\times C)=A\times (B\cup C)}]
***** Implementations[edit] *****
The first query language to be based on Codd's algebra was Alpha, developed by
Dr. Codd himself. Subsequently, ISBL was created, and this pioneering work has
been acclaimed by many authorities [1] as having shown the way to make Codd's
idea into a useful language. Business_System_12 was a short-lived industry-
strength relational DBMS that followed the ISBL example.
In 1998 Chris_Date and Hugh_Darwen proposed a language called Tutorial_D
intended for use in teaching relational database theory, and its query language
also draws on ISBL's ideas. Rel is an implementation of Tutorial D.
Even the query language of SQL is loosely based on a relational algebra, though
the operands in SQL (tables) are not exactly relations and several useful
theorems about the relational algebra do not hold in the SQL counterpart
(arguably to the detriment of optimisers and/or users). The SQL table model is
a bag (multiset), rather than a set. For example, the expression     ( R
&#x222A; S ) &#x2216; T = ( R &#x2216; T ) &#x222A; ( S &#x2216; T )
{\displaystyle (R\cup S)\setminus T=(R\setminus T)\cup (S\setminus T)}  [
{\displaystyle (R\cup S)\setminus T=(R\setminus T)\cup (S\setminus T)}] is a
theorem for relational algebra on sets, but not for relational algebra on bags;
for a treatment of relational algebra on bags see chapter 5 of the "Complete"
textbook by Garcia-Molina, Ullman and Widom.[11]
***** See also[edit] *****
    * Cartesian_product
    * D_(data_language_specification)
    * D4_(programming_language) (an implementation of D)
    * Database
    * Logic_of_relatives
    * Object-role_modeling
    * Projection_(mathematics)
    * Projection_(relational_algebra)
    * Projection_(set_theory)
    * Relation
    * Relation_(database)
    * Relation_algebra
    * Relation_composition
    * Relation_construction
    * Relational_calculus
    * Relational_database
    * Relational_model
    * Theory_of_relations
    * Triadic_relation
    * Tutorial_D
    * Tuple_relational_calculus
***** References[edit] *****
   1. ^ In Unicode, the bowtie symbol is â (U+22C8).
   2. ^ In Unicode, the ltimes symbol is â (U+22C9). The rtimes symbol is â
      (U+22CA)
   3. ^Codd,_E.F. (June 1970). "A Relational Model of Data for Large Shared
      Data Banks". Communications_of_the_ACM. 13 (6): 377â387. doi:10.1145/
      362384.362685.
   4. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   5. ^ In Unicode, the Antijoin symbol is â· (U+25B7).
   6. ^M. Tamer Ãzsu; Patrick Valduriez (2011). Principles_of_Distributed
      Database_Systems (3rd ed.). Springer. p. 46. ISBN 978-1-4419-8833-1.
   7. ^Patrick O'Neil; Elizabeth O'Neil (2001). Database:_Principles,
      Programming,_and_Performance,_Second_Edition. Morgan Kaufmann. p. 120.
      ISBN 978-1-55860-438-4.
   8. ^ In Unicode, the Left outer join symbol is â (U+27D5).
   9. ^ In Unicode, the Right outer join symbol is â (U+27D6).
  10. ^ In Unicode, the Full Outer join symbol is â (U+27D7).
  11. ^C. J. Date (2011). SQL_and_Relational_Theory:_How_to_Write_Accurate_SQL
      Code. O'Reilly Media, Inc. pp. 133â135. ISBN 978-1-4493-1974-8.
  12. ^ a bHector Garcia-Molina; Jeffrey D. Ullman; Jennifer Widom (2009).
      Database systems: the complete book (2nd ed.). Pearson Prentice Hall.
      ISBN 978-0-13-187325-4.
  13. ^Aho, Alfred V.; Jeffrey D. Ullman (1979). "Universality of data
      retrieval languages". Proceedings of the 6th ACM SIGACT-SIGPLAN Symposium
      on Principles of Programming Languages: 110â119. doi:10.1145/
      567752.567763.
***** Further reading[edit] *****
Practically any academic textbook on databases has a detailed treatment of the
classic relational algebra.
    * ImieliÅski,_T.; Lipski, W. (1984). "The relational model of data and
      cylindric algebras". Journal_of_Computer_and_System_Sciences. 28:
      80â102. doi:10.1016/0022-0000(84)90077-1.
 (For relationship with cylindric_algebras).
***** External links[edit] *****
 This article's use of external_links may not follow Wikipedia's policies or
 guidelines. Please improve_this_article by removing excessive or inappropriate
 external links, and converting useful links where appropriate into footnote
 references. (January 2017)(Learn_how_and_when_to_remove_this_template_message)
    * RAT._Software_Relational_Algebra_Translator_to_SQL
    * Lecture_Notes:_Relational_Algebra â A quick tutorial to adapt SQL
      queries into relational algebra
    * Relational_â_A_graphic_implementation_of_the_relational_algebra
    * Query_Optimization This paper is an introduction into the use of the
      relational algebra in optimizing queries, and includes numerous citations
      for more in-depth study.
    * bandilab.org_â_neat_graphical_illustrations_of_the_relational_operators
    * Relational_Algebra_System_for_Oracle_and_Microsoft_SQL_Server
    * Pireal_â_An_experimental_educational_tool_for_working_with_Relational
      Algebra
    * DES_â_An_educational_tool_for_working_with_Relational_Algebra_and_other
      formal_languages
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
                   * Relational algebra
                   * Relational_calculus
                   * Relational_database
                   * Relational_model
                   * Object-relational_database
                   * Transaction_processing

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Relational_algebra&oldid=909910870"
Categories:
    * Database_management_systems
    * Relational_model
Hidden categories:
    * Wikipedia_introduction_cleanup_from_April_2015
    * All_pages_needing_cleanup
    * Articles_covered_by_WikiProject_Wikify_from_April_2015
    * All_articles_covered_by_WikiProject_Wikify
    * Articles_needing_additional_references_from_June_2013
    * All_articles_needing_additional_references
    * Wikipedia_external_links_cleanup_from_January_2017
    * Wikipedia_spam_cleanup_from_January_2017
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
    * AzÉrbaycanca
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * Lumbaart
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à·à·à¶à·à¶½
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 8 August 2019, at 12:24 (UTC).
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
