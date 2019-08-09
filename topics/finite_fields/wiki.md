The following text has been accessed from https://en.wikipedia.org/wiki/Finite_field at Fri Aug 9 02:39:36 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Finite field ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Galois field" redirects here. For Galois field extensions, see Galois
extension.
Algebraic structure
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (February 2015)(Learn_how_and
 when_to_remove_this_template_message)
In mathematics, a finite field or Galois field (so-named in honor of Ãvariste
Galois) is a field that contains a finite number of elements. As with any
field, a finite field is a set on which the operations of multiplication,
addition, subtraction and division are defined and satisfy certain basic rules.
The most common examples of finite fields are given by the integers_mod_p when
p is a prime_number.
Finite fields are fundamental in a number of areas of mathematics and computer
science, including number_theory, algebraic_geometry, Galois_theory, finite
geometry, cryptography and coding_theory.
⁰
***** Contents *****
    * 1_Properties
    * 2_Existence_and_uniqueness
    * 3_Explicit_construction
          o 3.1_Non-prime_fields
          o 3.2_Field_with_four_elements
          o 3.3_GF(p2)_for_an_odd_prime_p
          o 3.4_GF(8)_and_GF(27)
          o 3.5_GF(16)
    * 4_Multiplicative_structure
          o 4.1_Discrete_logarithm
          o 4.2_Roots_of_unity
          o 4.3_Example:_GF(64)
    * 5_Frobenius_automorphism_and_Galois_theory
    * 6_Polynomial_factorization
          o 6.1_Irreducible_polynomials_of_a_given_degree
          o 6.2_Number_of_monic_irreducible_polynomials_of_a_given_degree_over
            a_finite_field
    * 7_Applications
    * 8_Extensions
          o 8.1_Algebraic_closure
          o 8.2_Wedderburn's_little_theorem
          o 8.3_Relationship_to_other_commutative_ring_classes
    * 9_See_also
    * 10_Notes
    * 11_References
    * 12_External_links
***** Properties[edit] *****
A finite field is a finite set which is a field; this means that
multiplication, addition, subtraction and division (excluding division by zero)
are defined and satisfy the rules of arithmetic known as the field_axioms.
The number of elements of a finite field is called its order or, sometimes, its
size. A finite field of order q exists if and only if the order q is a prime
power pk (where p is a prime number and k is a positive integer). In a field of
order pk, adding p copies of any element always results in zero; that is, the
characteristic of the field is p.
If     q =  p  k   ,   {\displaystyle q=p^{k},}  [{\displaystyle q=p^{k},}] all
fields of order q are isomorphic (see Â§ Existence_and_uniqueness below).[1]
Moreover, a field cannot contain two different finite subfields with the same
order. One may therefore identify all finite fields with the same order, and
they are unambiguously denoted       F   q     {\displaystyle \mathbb {F} _{q}}
[{\mathbb  {F}}_{{q}}], Fq or GF(q), where the letters GF stand for "Galois
field".[2]
In a finite field of order q, the polynomial Xq â X has all q elements of the
finite field as roots. The non-zero elements of a finite field form a
multiplicative_group. This group is cyclic, so all non-zero elements can be
expressed as powers of a single element called a primitive_element of the
field. (In general there will be several primitive elements for a given field.)
The simplest examples of finite fields are the fields of prime order: for each
prime_number p, the prime_field of order p, denoted GF(p), Z/pZ,       F   p
{\displaystyle \mathbb {F} _{p}}  [\mathbb {F} _{p}], or Fp, may be constructed
as the integers_modulo_p.
The elements of the prime field of order p may be represented by integers in
the range 0, ..., p â 1. The sum, the difference and the product are the
remainder_of_the_division by p of the result of the corresponding integer
operation. The multiplicative inverse of an element may be computed by using
the extended Euclidean algorithm (see Extended_Euclidean_algorithm_Â§ Modular
integers).
Let F be a finite field. For any element x in F and any integer n, denote by n
â x the sum of n copies of x. The least positive n such that n â 1 = 0 is
the characteristic p of the field. This allows defining a multiplication
( k , x ) &#x21A6; k &#x22C5; x   {\displaystyle (k,x)\mapsto k\cdot x}  [
(k,x)\mapsto k\cdot x] of an element k of GF(p) by an element x of F by
choosing an integer representative for k. This multiplication makes F into a GF
(p)-vector_space. It follows that the number of elements of F is pn for some
integer n.
The identity
         ( x + y  )  p   =  x  p   +  y  p     {\displaystyle (x+y)^{p}=x^
      {p}+y^{p}}  [(x+y)^{p}=x^{p}+y^{p}]
(sometimes called the freshman's_dream) is true in a field of characteristic p.
This follows from the binomial_theorem, as each binomial_coefficient of the
expansion of (x + y)p, except the first and the last, is a multiple of p.
By Fermat's_little_theorem, if p is a prime number and x is in the field GF(p)
then xp = x. This implies the equality
          X  p   &#x2212; X =  &#x220F;  a &#x2208;   G F   ( p )   ( X
      &#x2212; a )   {\displaystyle X^{p}-X=\prod _{a\in {\rm {GF}}(p)}(X-a)}
      [X^{p}-X=\prod _{a\in {\rm {GF}}(p)}(X-a)]
for polynomials over GF(p). More generally, every element in GF(pn) satisfies
the polynomial equation xpn â x = 0.
Any finite field extension of a finite field is separable and simple. That is,
if E is a finite field and F is a subfield of E, then E is obtained from F by
adjoining a single element whose minimal_polynomial is separable. To use a
jargon, finite fields are perfect.
A more general algebraic structure that satisfies all the other axioms of a
field, but whose multiplication is not required to be commutative, is called a
division_ring (or sometimes skew field). By Wedderburn's_little_theorem, any
finite division ring is commutative, and hence is a finite field.
***** Existence and uniqueness[edit] *****
Let q = pn be a prime_power, and F be the splitting_field of the polynomial
         P =  X  q   &#x2212; X   {\displaystyle P=X^{q}-X}  [P=X^{q}-X]
over the prime field GF(p). This means that F is a finite field of lowest
order, in which P has q distinct roots (the roots are distinct, as the formal
derivative of P is equal to â1). The above_identity shows that the sum and
the product of two roots of P are roots of P, as well as the multiplicative
inverse of a root of P. In other word, the roots of P form a field of order q,
which is equal to F by the minimality of the splitting field.
The uniqueness up to isomorphism of splitting fields implies thus that all
fields of order q are isomorphic. Also, if a field F has a field of order     q
=  p  k     {\displaystyle q=p^{k}}  [{\displaystyle q=p^{k}}] as a subfield,
its elements are the q roots of      X  q   &#x2212; X ,   {\displaystyle X^
{q}-X,}  [{\displaystyle X^{q}-X,}] and F cannot contain another subfield of
order q.
In summary, we have the following classification theorem first proved in 1893
by E._H._Moore:[1]
            The order of a finite field is a prime power. For every prime power
            q there are fields of order q, and they are all isomorphic. In
            these fields, every element satisfies
                      x  q   = x ,   {\displaystyle x^{q}=x,}  [x^{q}=x,]
            and the polynomial Xq â X factors as
                      X  q   &#x2212; X =  &#x220F;  a &#x2208; F   ( X
                  &#x2212; a ) .   {\displaystyle X^{q}-X=\prod _{a\in F}(X-
                  a).}  [X^{q}-X=\prod _{a\in F}(X-a).]
It follows that GF(pn) contains a subfield isomorphic to GF(pm) if and only if
m is a divisor of n; in that case, this subfield is unique. In fact, the
polynomial Xpm â X divides Xpn â X if and only if m is a divisor of n.
***** Explicit construction[edit] *****
**** Non-prime fields[edit] ****
Given a prime power q = pn with p prime and n > 1, the field GF(q) may be
explicitly constructed in the following way. One chooses first an irreducible
polynomial P in GF(p)[X] of degree n (such an irreducible polynomial always
exists). Then the quotient_ring
           G F   ( q ) =   G F   ( p ) [ X ]  /  ( P )   {\displaystyle {\rm
      {GF}}(q)={\rm {GF}}(p)[X]/(P)}  [{\rm {GF}}(q)={\rm {GF}}(p)[X]/(P)]
of the polynomial ring GF(p)[X] by the ideal generated by P is a field of order
q.
More explicitly, the elements of GF(q) are the polynomials over GF(p) whose
degree is strictly less than n. The addition and the subtraction are those of
polynomials over GF(p). The product of two elements is the remainder of the
Euclidean_division by P of the product in GF(p)[X]. The multiplicative inverse
of a non-zero element may be computed with the extended Euclidean algorithm;
see Extended_Euclidean_algorithm_Â§_Simple_algebraic_field_extensions.
Except in the construction of GF(4), there are several possible choices for P,
which produce isomorphic results. To simplify the Euclidean division, for P one
commonly chooses polynomials of the form
          X  n   + a X + b ,   {\displaystyle X^{n}+aX+b,}  [X^{n}+aX+b,]
which make the needed Euclidean divisions very efficient. However, for some
fields, typically in characteristic 2, irreducible polynomials of the form Xn +
aX + b may not exist. In characteristic 2, if the polynomial Xn + X + 1 is
reducible, it is recommended to choose Xn + Xk + 1 with the lowest possible k
that makes the polynomial irreducible. If all these trinomials are reducible,
one chooses "pentanomials" Xn + Xa + Xb + Xc + 1, as polynomials of degree
greater than 1, with an even number of terms, are never irreducible in
characteristic 2, having 1 as a root.[3]
A possible choice for such a polynomial is given by Conway_polynomials. They
ensure a certain compatibility between the representation of a field and the
representations of its subfields.
In the next sections, we will show how the general construction method outlined
above works for small finite fields.
**** Field with four elements[edit] ****
Over GF(2), there is only one irreducible_polynomial of degree 2:
          X  2   + X + 1   {\displaystyle X^{2}+X+1}  [X^{2}+X+1]
Therefore, for GF(4) the construction of the preceding section must involve
this polynomial, and
           G F   ( 4 ) =   G F   ( 2 ) [ X ]  /  (  X  2   + X + 1 ) .
      {\displaystyle {\rm {GF}}(4)={\rm {GF}}(2)[X]/(X^{2}+X+1).}  [{\rm {GF}}
      (4)={\rm {GF}}(2)[X]/(X^{2}+X+1).]
If one denotes a a root of this polynomial in GF(4), the tables of the
operations in GF(4) are the following. There is no table for subtraction,
because subtraction is identical to addition, as is the case for every field of
characteristic 2. In the third table, for the division of x by y, x must be
read on the left, and y on the top.
Addition                  Multiplication            Division
+   0   1     a     1 + a Ã  0 1     a     1 + a x/y   0   1     a     1 + a
0   0   1     a     1 + a 0     0 0     0     0     0     â0�    0     0
1   1   0     1 + a a     1     0 1     a     1 + a 1     â1�    1 + a a
a   a   1 + a 0     1     a     0 a     1 + a 1     a     âa�    1     1 + a
1 + 1 + a     1     0     1 + a 0 1 + a 1     a     1 + a â1 + a a     1
a   a
**** GF(p2) for an odd prime p[edit] ****
For applying the above_general_construction of finite fields in the case of GF
(p2), one has to find an irreducible polynomial of degree 2. For p = 2, this
has been done in the preceding section. If p is an odd prime, there are always
irreducible polynomials of the form X2 â r, with r in GF(p).
More precisely, the polynomial X2 â r is irreducible over GF(p) if and only
if r is a quadratic_non-residue modulo p (this is almost the definition of a
quadratic non-residue). There are        p &#x2212; 1  2     {\displaystyle
{\frac {p-1}{2}}}  [{\frac {p-1}{2}}] quadratic non-residues modulo p. For
example, 2 is a quadratic non-residue for p = 3, 5, 11, 13, ..., and 3 is a
quadratic non-residue for p = 5, 7, 17, .... If p â¡ 3 mod 4, that is p = 3,
7, 11, 19, ..., one may choose â1 â¡ p â 1 as a quadratic non-residue,
which allows us to have a very simple irreducible polynomial X2 + 1.
Having chosen a quadratic non-residue r, let Î± be a symbolic square root of r,
that is a symbol which has the property Î±2 = r, in the same way as the complex
number i is a symbolic square root of â1. Then, the elements of GF(p2) are
all the linear expressions
         a + b &#x03B1; ,   {\displaystyle a+b\alpha ,}  [a+b\alpha ,]
with a and b in GF(p). The operations on GF(p2) are defined as follows (the
operations between elements of GF(p) represented by Latin letters are the
operations in GF(p)):
             &#x2212; ( a + b &#x03B1; )    = &#x2212; a + ( &#x2212; b )
      &#x03B1;     ( a + b &#x03B1; ) + ( c + d &#x03B1; )    = ( a + c ) + ( b
      + d ) &#x03B1;     ( a + b &#x03B1; ) ( c + d &#x03B1; )    = ( a c + r b
      d ) + ( a d + b c ) &#x03B1;     ( a + b &#x03B1;  )  &#x2212; 1      = a
      (  a  2   &#x2212; r  b  2    )  &#x2212; 1   + ( &#x2212; b ) (  a  2
      &#x2212; r  b  2    )  &#x2212; 1   &#x03B1;       {\displaystyle {\begin
      {aligned}-(a+b\alpha )&=-a+(-b)\alpha \\(a+b\alpha )+(c+d\alpha )&=(a+c)+
      (b+d)\alpha \\(a+b\alpha )(c+d\alpha )&=(ac+rbd)+(ad+bc)\alpha \\
      (a+b\alpha )^{-1}&=a(a^{2}-rb^{2})^{-1}+(-b)(a^{2}-rb^{2})^{-1}\alpha
      \end{aligned}}}  [{\begin{aligned}-(a+b\alpha )&=-a+(-b)\alpha \\
      (a+b\alpha )+(c+d\alpha )&=(a+c)+(b+d)\alpha \\(a+b\alpha )(c+d\alpha )&=
      (ac+rbd)+(ad+bc)\alpha \\(a+b\alpha )^{-1}&=a(a^{2}-rb^{2})^{-1}+(-b)(a^
      {2}-rb^{2})^{-1}\alpha \end{aligned}}]
**** GF(8) and GF(27)[edit] ****
The polynomial
          X  3   &#x2212; X &#x2212; 1   {\displaystyle X^{3}-X-1}  [X^{3}-X-1]
is irreducible over GF(2) and GF(3), that is, it is irreducible modulo 2 and 3
(to show this it suffices to show that it has no root in GF(2) nor in GF(3)).
It follows that the elements of GF(8) and GF(27) may be represented by
expressions
         a + b &#x03B1; + c  &#x03B1;  2   ,   {\displaystyle a+b\alpha
      +c\alpha ^{2},}  [a+b\alpha +c\alpha ^{2},]
where a, b, c are elements of GF(2) or GF(3) (respectively), and     &#x03B1;
{\displaystyle \alpha }  [\alpha ] is a symbol such that
          &#x03B1;  3   = &#x03B1; + 1.   {\displaystyle \alpha ^{3}=\alpha
      +1.}  [\alpha ^{3}=\alpha +1.]
The addition, additive inverse and multiplication on GF(8) and GF(27) may thus
be defined as follows; in following formulas, the operations between elements
of GF(2) or GF(3), represented by Latin letters, are the operations in GF(2) or
GF(3), respectively:
             &#x2212; ( a + b &#x03B1; + c  &#x03B1;  2   )    = &#x2212; a +
      ( &#x2212; b ) &#x03B1; + ( &#x2212; c )  &#x03B1;  2     (for&#xA0;   G
      F  ( 8 ) ,  this operation is the identity)      ( a + b &#x03B1; + c
      &#x03B1;  2   ) + ( d + e &#x03B1; + f  &#x03B1;  2   )    = ( a + d ) +
      ( b + e ) &#x03B1; + ( c + f )  &#x03B1;  2       ( a + b &#x03B1; + c
      &#x03B1;  2   ) ( d + e &#x03B1; + f  &#x03B1;  2   )    = ( a d + b f +
      c e ) + ( a e + b d + b f + c e + c f ) &#x03B1; + ( a f + b e + c d + c
      f )  &#x03B1;  2         {\displaystyle {\begin{aligned}-(a+b\alpha
      +c\alpha ^{2})&=-a+(-b)\alpha +(-c)\alpha ^{2}\qquad {\text{(for
      }}\mathrm {GF} (8),{\text{this operation is the identity)}}\\(a+b\alpha
      +c\alpha ^{2})+(d+e\alpha +f\alpha ^{2})&=(a+d)+(b+e)\alpha +(c+f)\alpha
      ^{2}\\(a+b\alpha +c\alpha ^{2})(d+e\alpha +f\alpha ^{2})&=(ad+bf+ce)+
      (ae+bd+bf+ce+cf)\alpha +(af+be+cd+cf)\alpha ^{2}\end{aligned}}}  [
      {\displaystyle {\begin{aligned}-(a+b\alpha +c\alpha ^{2})&=-a+(-b)\alpha
      +(-c)\alpha ^{2}\qquad {\text{(for }}\mathrm {GF} (8),{\text{this
      operation is the identity)}}\\(a+b\alpha +c\alpha ^{2})+(d+e\alpha
      +f\alpha ^{2})&=(a+d)+(b+e)\alpha +(c+f)\alpha ^{2}\\(a+b\alpha +c\alpha
      ^{2})(d+e\alpha +f\alpha ^{2})&=(ad+bf+ce)+(ae+bd+bf+ce+cf)\alpha +
      (af+be+cd+cf)\alpha ^{2}\end{aligned}}}]
**** GF(16)[edit] ****
The polynomial
          X  4   + X + 1   {\displaystyle X^{4}+X+1}  [X^{4}+X+1]
is irreducible over GF(2), that is, it is irreducible modulo 2. It follows that
the elements of GF(16) may be represented by expressions
         a + b &#x03B1; + c  &#x03B1;  2   + d  &#x03B1;  3   ,
      {\displaystyle a+b\alpha +c\alpha ^{2}+d\alpha ^{3},}  [a+b\alpha
      +c\alpha ^{2}+d\alpha ^{3},]
where a, b, c, d are either 0 or 1 (elements of GF(2)), and Î± is a symbol such
that
          &#x03B1;  4   = &#x03B1; + 1.   {\displaystyle \alpha ^{4}=\alpha
      +1.}  [\alpha ^{4}=\alpha +1.]
As the characteristic of GF(2) is 2, each element is its additive inverse in GF
(16). The addition and multiplication on GF(16) may be defined as follows; in
following formulas, the operations between elements of GF(2), represented by
Latin letters are the operations in GF(2).
             ( a + b &#x03B1; + c  &#x03B1;  2   + d  &#x03B1;  3   ) + ( e + f
      &#x03B1; + g  &#x03B1;  2   + h  &#x03B1;  3   )    = ( a + e ) + ( b + f
      ) &#x03B1; + ( c + g )  &#x03B1;  2   + ( d + h )  &#x03B1;  3       ( a
      + b &#x03B1; + c  &#x03B1;  2   + d  &#x03B1;  3   ) ( e + f &#x03B1; + g
      &#x03B1;  2   + h  &#x03B1;  3   )    = ( a e + b h + c g + d f ) + ( a f
      + b e + b h + c g + d f + c h + d g ) &#x03B1;  +         ( a g + b f + c
      e + c h + d g + d h )  &#x03B1;  2   + ( a h + b g + c f + d e + d h )
      &#x03B1;  3         {\displaystyle {\begin{aligned}(a+b\alpha +c\alpha ^
      {2}+d\alpha ^{3})+(e+f\alpha +g\alpha ^{2}+h\alpha ^{3})&=(a+e)+
      (b+f)\alpha +(c+g)\alpha ^{2}+(d+h)\alpha ^{3}\\(a+b\alpha +c\alpha ^
      {2}+d\alpha ^{3})(e+f\alpha +g\alpha ^{2}+h\alpha ^{3})&=(ae+bh+cg+df)+
      (af+be+bh+cg+df+ch+dg)\alpha \;+\\&\quad \;(ag+bf+ce+ch+dg+dh)\alpha ^
      {2}+(ah+bg+cf+de+dh)\alpha ^{3}\end{aligned}}}  [{\begin{aligned}
      (a+b\alpha +c\alpha ^{2}+d\alpha ^{3})+(e+f\alpha +g\alpha ^{2}+h\alpha ^
      {3})&=(a+e)+(b+f)\alpha +(c+g)\alpha ^{2}+(d+h)\alpha ^{3}\\(a+b\alpha
      +c\alpha ^{2}+d\alpha ^{3})(e+f\alpha +g\alpha ^{2}+h\alpha ^{3})&=
      (ae+bh+cg+df)+(af+be+bh+cg+df+ch+dg)\alpha \;+\\&\quad \;
      (ag+bf+ce+ch+dg+dh)\alpha ^{2}+(ah+bg+cf+de+dh)\alpha ^{3}\end{aligned}}]
***** Multiplicative structure[edit] *****
The set of non-zero elements in GF(q) is an abelian_group under the
multiplication, of order q â 1. By Lagrange's_theorem, there exists a divisor
k of q â 1 such that xk = 1 for every non-zero x in GF(q). As the equation Xk
= 1 has at most k solutions in any field, q â 1 is the lowest possible value
for k. The structure_theorem_of_finite_abelian_groups implies that this
multiplicative group is cyclic, that is, all non-zero elements are powers of a
single element. In summary:
      The multiplicative group of the non-zero elements in GF(q) is cyclic, and
      there exist an element a, such that the q â 1 non-zero elements of GF
      (q) are a, a2, ..., aqâ2, aqâ1 = 1.
Such an element a is called a primitive_element. Unless q = 2, 3, the primitive
element is not unique. The number of primitive elements is Ï(q â 1) where Ï
is Euler's_totient_function.
The result above implies that xq = x for every x in GF(q). The particular case
where q is prime is Fermat's_little_theorem.
**** Discrete logarithm[edit] ****
If a is a primitive element in GF(q), then for any non-zero element x in F,
there is a unique integer n with 0 â¤ n â¤ q â 2 such that
      x = an.
This integer n is called the discrete_logarithm of x to the base a.
While an can be computed very quickly, for example using exponentiation_by
squaring, there is no known efficient algorithm for computing the inverse
operation, the discrete logarithm. This has been used in various cryptographic
protocols, see Discrete_logarithm for details.
When the nonzero elements of GF(q) are represented by their discrete
logarithms, multiplication and division are easy, as they reduce to addition
and subtraction modulo q â 1. However, addition amounts to computing the
discrete logarithm of am + an. The identity
      am + an = an(amân + 1)
allows one to solve this problem by constructing the table of the discrete
logarithms of an + 1, called Zech's_logarithms, for n = 0, ..., q â 2 (it is
convenient to define the discrete logarithm of zero as being ââ).
Zech's logarithms are useful for large computations, such as linear_algebra
over medium-sized fields, that is, fields that are sufficiently large for
making natural algorithms inefficient, but not too large, as one has to pre-
compute a table of the same size as the order of the field.
**** Roots of unity[edit] ****
Every nonzero element of a finite field is a root_of_unity, as xqâ1 = 1 for
every nonzero element of GF(q).
If n is a positive integer, an nth primitive root of unity is a solution of the
equation xn = 1 that is not a solution of the equation xm = 1 for any positive
integer m < n. If a is a nth primitive root of unity in a field F, then F
contains all the n roots of unity, which are 1, a, a2, ..., anâ1.
The field GF(q) contains a nth primitive root of unity if and only if n is a
divisor of q â 1; if n is a divisor of q â 1, then the number of primitive
nth roots of unity in GF(q) is Ï(n) (Euler's_totient_function). The number of
nth roots of unity in GF(q) is gcd(n, q â 1).
In a field of characteristic p, every (np)th root of unity is also a nth root
of unity. It follows that primitive (np)th roots of unity never exist in a
field of characteristic p.
On the other hand, if n is coprime to p, the roots of the nth cyclotomic
polynomial are distinct in every field of characteristic p, as this polynomial
is a divisor of Xn â 1, whose discriminant      n  n     {\displaystyle n^
{n}}  [n^n] is nonzero modulo p. It follows that the nth cyclotomic_polynomial
factors over GF(p) into distinct irreducible polynomials that have all the same
degree, say d, and that GF(pd) is the smallest field of characteristic p that
contains the nth primitive roots of unity.
**** Example: GF(64)[edit] ****
The field GF(64) has several interesting properties that smaller fields do not
share: it has two subfields such that neither is contained in the other; not
all generators (elements with minimal_polynomial of degree 6 over GF(2)) are
primitive elements; and the primitive elements are not all conjugate under the
Galois group.
The order of this field being 26, and the divisors of 6 being 1, 2, 3, 6, the
subfields of GF(64) are GF(2), GF(22) = GF(4), GF(23) = GF(8), and GF(64)
itself. As 2 and 3 are coprime, the intersection of GF(4) and GF(8) in GF(64)
is the prime field GF(2).
The union of GF(4) and GF(8) has thus 10 elements. The remaining 54 elements of
GF(64) generate GF(64) in the sense that no other subfield contains any of
them. It follows that they are roots of irreducible polynomials of degree 6
over GF(2). This implies that, over GF(2), there are exactly 9 = 54/
6 irreducible monic polynomials of degree 6. This may be verified by factoring
X64 â X over GF(2).
The elements of GF(64) are primitive nth roots of unity for some n dividing 63.
As the 3rd and the 7th roots of unity belong to GF(4) and GF(8), respectively,
the 54 generators are primitive nth roots of unity for some n in {9, 21, 63}.
Euler's_totient_function shows that there are 6 primitive 9th roots of unity,
12 primitive 21st roots of unity, and 36 primitive 63rd roots of unity. Summing
these numbers, one finds again 54 elements.
By factoring the cyclotomic_polynomials over GF(2), one finds that:
    * The six primitive 9th roots of unity are roots of
                X  6   +  X  3   + 1 ,   {\displaystyle X^{6}+X^{3}+1,}  [X^
            {6}+X^{3}+1,]
      and are all conjugate under the action of the Galois group.
    * The twelve primitive 21st roots of unity are roots of
               (  X  6   +  X  4   +  X  2   + X + 1 ) (  X  6   +  X  5   +  X
            4   +  X  2   + 1 ) .   {\displaystyle (X^{6}+X^{4}+X^{2}+X+1)(X^
            {6}+X^{5}+X^{4}+X^{2}+1).}  [(X^{6}+X^{4}+X^{2}+X+1)(X^{6}+X^{5}+X^
            {4}+X^{2}+1).]
      They form two orbits under the action of the Galois group. As the two
      factors are reciprocal to each other, a root and its (multiplicative)
      inverse do not belong to the same orbit.
    * The 36 primitive elements of GF(64) are the roots of
               (  X  6   +  X  4   +  X  3   + X + 1 ) (  X  6   + X + 1 ) (  X
            6   +  X  5   + 1 ) (  X  6   +  X  5   +  X  3   +  X  2   + 1 )
            (  X  6   +  X  5   +  X  2   + X + 1 ) (  X  6   +  X  5   +  X  4
            + X + 1 ) ,   {\displaystyle (X^{6}+X^{4}+X^{3}+X+1)(X^{6}+X+1)(X^
            {6}+X^{5}+1)(X^{6}+X^{5}+X^{3}+X^{2}+1)(X^{6}+X^{5}+X^{2}+X+1)(X^
            {6}+X^{5}+X^{4}+X+1),}  [(X^{6}+X^{4}+X^{3}+X+1)(X^{6}+X+1)(X^
            {6}+X^{5}+1)(X^{6}+X^{5}+X^{3}+X^{2}+1)(X^{6}+X^{5}+X^{2}+X+1)(X^
            {6}+X^{5}+X^{4}+X+1),]
      They split into 6 orbits of 6 elements under the action of the Galois
      group.
This shows that the best choice to construct GF(64) is to define it as GF(2)
[X]/(X6 + X + 1). In fact, this generator is a primitive element, and this
polynomial is the irreducible polynomial that produces the easiest Euclidean
division.
***** Frobenius automorphism and Galois theory[edit] *****
In this section, p is a prime number, and q = pn is a power of p.
In GF(q), the identity (x + y)p = xp + yp implies that the map
         &#x03C6; : x &#x21A6;  x  p     {\displaystyle \varphi :x\mapsto x^
      {p}}  [\varphi :x\mapsto x^{p}]
is a GF(p)-linear_endomorphism and a field_automorphism of GF(q), which fixes
every element of the subfield GF(p). It is called the Frobenius_automorphism,
after Ferdinand_Georg_Frobenius.
Denoting by Ïk the composition of Ï with itself k times, we have
          &#x03C6;  k   : x &#x21A6;  x   p  k     .   {\displaystyle \varphi ^
      {k}:x\mapsto x^{p^{k}}.}  [\varphi ^{k}:x\mapsto x^{p^{k}}.]
It has been shown in the preceding section that Ïn is the identity. For 0 < k
< n, the automorphism Ïk is not the identity, as, otherwise, the polynomial
          X   p  k     &#x2212; X   {\displaystyle X^{p^{k}}-X}  [X^{p^{k}}-X]
would have more than pk roots.
There are no other GF(p)-automorphisms of GF(q). In other words, GF(pn) has
exactly n GF(p)-automorphisms, which are
          I d  =  &#x03C6;  0   , &#x03C6; ,  &#x03C6;  2   , &#x2026; ,
      &#x03C6;  n &#x2212; 1   .   {\displaystyle \mathrm {Id} =\varphi ^
      {0},\varphi ,\varphi ^{2},\ldots ,\varphi ^{n-1}.}  [\mathrm {Id}
      =\varphi ^{0},\varphi ,\varphi ^{2},\ldots ,\varphi ^{n-1}.]
In terms of Galois_theory, this means that GF(pn) is a Galois_extension of GF
(p), which has a cyclic Galois group.
The fact that the Frobenius map is surjective implies that every finite field
is perfect.
***** Polynomial factorization[edit] *****
Main article: Factorization_of_polynomials_over_finite_fields
If F is a finite field, a non-constant monic_polynomial with coefficients in F
is irreducible over F, if it is not the product of two non-constant monic
polynomials, with coefficients in F.
As every polynomial_ring over a field is a unique_factorization_domain, every
monic polynomial over a finite field may be factored in a unique way (up to the
order of the factors) into a product of irreducible monic polynomials.
There are efficient algorithms for testing polynomial irreducibility and
factoring polynomials over finite field. They are a key step for factoring
polynomials over the integers or the rational_numbers. At least for this
reason, every computer_algebra_system has functions for factoring polynomials
over finite fields, or, at least, over finite prime fields.
**** Irreducible polynomials of a given degree[edit] ****
The polynomial
          X  q   &#x2212; X   {\displaystyle X^{q}-X}  [X^{q}-X]
factors into linear factors over a field of order q. More precisely, this
polynomial is the product of all monic polynomials of degree one over a field
of order q.
This implies that, if q = pn then Xq â X is the product of all monic
irreducible polynomials over GF(p), whose degree divides n. In fact, if P is an
irreducible factor over GF(p) of Xq â X, its degree divides n, as its
splitting_field is contained in GF(pn). Conversely, if P is an irreducible
monic polynomial over GF(p) of degree d dividing n, it defines a field
extension of degree d, which is contained in GF(pn), and all roots of P belong
to GF(pn), and are roots of Xq â X; thus P divides Xq â X. As Xq â X does
not have any multiple factor, it is thus the product of all the irreducible
monic polynomials that divide it.
This property is used to compute the product of the irreducible factors of each
degree of polynomials over GF(p); see Distinct_degree_factorization.
**** Number of monic irreducible polynomials of a given degree over a finite
field[edit] ****
The number N(q, n) of monic irreducible polynomials of degree n over GF(q) is
given by[4]
         N ( q , n ) =   1 n    &#x2211;  d &#x2223; n   &#x03BC; ( d )  q  n
      /  d   ,   {\displaystyle N(q,n)={\frac {1}{n}}\sum _{d\mid n}\mu (d)q^
      {n/d},}  [{\displaystyle N(q,n)={\frac {1}{n}}\sum _{d\mid n}\mu (d)q^{n/
      d},}]
where Î¼ is the MÃ¶bius_function. This formula is almost a direct consequence
of above property of Xq â X.
By the above formula, the number of irreducible (not necessarily monic)
polynomials of degree n over GF(q) is (q â 1)N(q, n).
A (slightly simpler) lower bound for N(q, n) is
         N ( q , n ) &#x2265;   1 n    (   q  n   &#x2212;  &#x2211;  p
      &#x2223; n , &#xA0; p  &#xA0;prime     q  n  /  p    )  .
      {\displaystyle N(q,n)\geq {\frac {1}{n}}\left(q^{n}-\sum _{p\mid n,\ p
      {\text{ prime}}}q^{n/p}\right).}  [{\displaystyle N(q,n)\geq {\frac {1}
      {n}}\left(q^{n}-\sum _{p\mid n,\ p{\text{ prime}}}q^{n/p}\right).}]
One may easily deduce that, for every q and every n, there is at least one
irreducible polynomial of degree n over GF(q). This lower bound is sharp for q
= n = 2.
***** Applications[edit] *****
In cryptography, the difficulty of the discrete_logarithm_problem in finite
fields or in elliptic_curves is the basis of several widely used protocols,
such as the DiffieâHellman protocol. For example, in 2014 a secure internet
connection to Wikipedia involved the elliptic curve DiffieâHellman protocol
(ECDHE) over a large finite field.[5] In coding_theory, many codes are
constructed as subspaces of vector_spaces over finite fields.
Finite fields are widely used in number_theory, as many problems over the
integers may be solved by reducing them modulo one or several prime_numbers.
For example, the fastest known algorithms for polynomial_factorization and
linear_algebra over the field of rational_numbers proceed by reduction modulo
one or several primes, and then reconstruction of the solution by using Chinese
remainder_theorem, Hensel_lifting or the LLL_algorithm.
Similarly many theoretical problems in number theory can be solved by
considering their reductions modulo some or all prime numbers. See, for
example, Hasse_principle. Many recent developments of algebraic_geometry were
motivated by the need to enlarge the power of these modular methods. Wiles'
proof_of_Fermat's_Last_Theorem is an example of a deep result involving many
mathematical tools, including finite fields.
***** Extensions[edit] *****
**** Algebraic closure[edit] ****
A finite field F is not algebraically closed. To demonstrate this, consider the
polynomial
         f ( T ) = 1 +  &#x220F;  &#x03B1; &#x2208;  F    ( T &#x2212; &#x03B1;
      ) ,   {\displaystyle f(T)=1+\prod _{\alpha \in \mathbf {F} }(T-\alpha ),}
      [f(T)=1+\prod _{\alpha \in \mathbf {F} }(T-\alpha ),]
which has no roots in F, since f (Î±) = 1 for all Î± in F.
The direct_limit of the system:
      {Fp, Fp2, ..., Fpn, ...},
with inclusion, is an infinite field. It is the algebraic_closure of all the
fields in the system, and is denoted by:         F   p   &#x00AF;
{\displaystyle {\overline {\mathbf {F} _{p}}}}  [{\overline {\mathbf {F} _
{p}}}].
The inclusions commute with the Frobenius map, as it is defined the same way on
each field (x â¦ x p ), so the Frobenius map defines an automorphism of
F   p   &#x00AF;     {\displaystyle {\overline {\mathbf {F} _{p}}}}  [
{\overline {\mathbf {F} _{p}}}], which carries all subfields back to
themselves. In fact Fpn can be recovered as the fixed points of the nth iterate
of the Frobenius map.
However unlike the case of finite fields, the Frobenius automorphism on
F   p   &#x00AF;     {\displaystyle {\overline {\mathbf {F} _{p}}}}  [
{\overline {\mathbf {F} _{p}}}] has infinite order, and it does not generate
the full group of automorphisms of this field. That is, there are automorphisms
of         F   p   &#x00AF;     {\displaystyle {\overline {\mathbf {F} _{p}}}}
[{\overline {\mathbf {F} _{p}}}] which are not a power of the Frobenius map.
However, the group generated by the Frobenius map is a dense subgroup of the
automorphism group in the Krull_topology. Algebraically, this corresponds to
the additive group Z being dense in the profinite_integers (direct product of
the p-adic integers over all primes p, with the product_topology).
If we actually construct our finite fields in such a fashion that Fpn is
contained in Fpm whenever n divides m, then this direct limit can be
constructed as the union of all these fields. Even if we do not construct our
fields this way, we can still speak of the algebraic closure, but some more
delicacy is required in its construction.
**** Wedderburn's little theorem[edit] ****
A division_ring is a generalization of field. Division rings are not assumed to
be commutative. There are no non-commutative finite division rings:
Wedderburn's_little_theorem states that all finite division_rings are
commutative, hence finite fields. The result holds even if we relax
associativity and consider alternative_rings, by the ArtinâZorn_theorem.[6]
**** Relationship to other commutative ring classes[edit] ****
Finite fields appear in the following chain of inclusions:
      commutative_rings â integral_domains â integrally_closed_domains â
      GCD_domains â unique_factorization_domains â principal_ideal_domains
      â Euclidean_domains â fields â finite fields
***** See also[edit] *****
    * Quasi-finite_field
    * Field_with_one_element
    * Finite_field_arithmetic
    * Finite_ring
    * Finite_group
    * Elementary_abelian_group
    * Hamming_space
***** Notes[edit] *****
   1. ^ a bMoore,_E._H. (1896), "A doubly-infinite system of simple groups", in
      E. H. Moore; et al. (eds.), Mathematical Papers Read at the International
      Mathematics Congress Held in Connection with the World's Columbian
      Exposition, Macmillan & Co., pp. 208â242
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
   3. ^ This latter notation was introduced by E._H._Moore in an address given
      in 1893 at the International Mathematical Congress held in Chicago Mullen
      &_Panario_2013, p. 10.
   4. ^Recommended_Elliptic_Curves_for_Government_Use (PDF), National_Institute
      of_Standards_and_Technology, July 1999, p. 3
   5. ^ Jacobson_2009, Â§4.13
   6. ^ This can be verified by looking at the information on the page provided
      by the browser.
   7. ^Shult, Ernest E. (2011). Points and lines. Characterizing the classical
      geometries. Universitext. Berlin: Springer-Verlag. p. 123. ISBN 978-3-
      642-15626-7. Zbl 1213.51001.
***** References[edit] *****
    * W. H. Bussey (1905) "Galois field tables for pn â¤ 169", Bulletin_of_the
      American_Mathematical_Society 12(1): 22â38, doi:10.1090/S0002-9904-
      1905-01284-2
    * W. H. Bussey (1910) "Tables of Galois fields of order < 1000", Bulletin
      of the American Mathematical Society 16(4): 188â206, doi:10.1090/S0002-
      9904-1910-01888-7
    * Jacobson,_Nathan (2009) [1985], Basic algebra I (Second ed.), Dover
      Publications, ISBN 978-0-486-47189-1
Mullen, Gary L.; Mummert, Carl (2007), Finite Fields and Applications I,
Student Mathematical Library (AMS), ISBN 978-0-8218-4418-2
Mullen, Gary L.; Panario, Daniel (2013), Handbook of Finite Fields, CRC Press,
ISBN 978-1-4398-7378-6
Lidl, Rudolf; Niederreiter,_Harald (1997), Finite Fields (2nd ed.), Cambridge
University_Press, ISBN 0-521-39231-4
Skopin, A. I. (2001) [1994], "Galois_field", in Hazewinkel,_Michiel (ed.),
Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. / Kluwer
Academic Publishers, ISBN 978-1-55608-010-4
***** External links[edit] *****
    * Finite_Fields at Wolfram research.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Finite_field&oldid=907887229"
Categories:
    * Finite_fields
Hidden categories:
    * Articles_with_short_description
    * Articles_lacking_in-text_citations_from_February_2015
    * All_articles_lacking_in-text_citations
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
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 25 July 2019, at 23:19 (UTC).
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
