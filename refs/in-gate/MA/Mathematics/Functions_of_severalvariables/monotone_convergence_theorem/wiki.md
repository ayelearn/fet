The following text has been accessed from https://en.wikipedia.org/wiki/Monotone_convergence_theorem at Fri Aug 9 02:34:07 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Monotone convergence theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In the mathematical field of real_analysis, the monotone convergence theorem is
any of a number of related theorems proving the convergence of monotonic
sequences (sequences that are increasing or decreasing) that are also bounded.
Informally, the theorems state that if a sequence is increasing and bounded
above by a supremum, then the sequence will converge to the supremum; in the
same way, if a sequence is decreasing and is bounded below by an infimum, it
will converge to the infimum.
⁰
***** Contents *****
    * 1_Convergence_of_a_monotone_sequence_of_real_numbers
          o 1.1_Lemma_1
          o 1.2_Proof
          o 1.3_Lemma_2
          o 1.4_Proof
          o 1.5_Theorem
          o 1.6_Proof
    * 2_Convergence_of_a_monotone_series
          o 2.1_Theorem
    * 3_Beppo_Levi's_monotone_convergence_theorem_for_Lebesgue_integral
          o 3.1_Theorem
          o 3.2_Proof
                # 3.2.1_Intermediate_results
                      # 3.2.1.1_Lebesgue_integral_as_measure
                            # 3.2.1.1.1_Proof
                      # 3.2.1.2_"Continuity_from_below"
                # 3.2.2_Proof_of_theorem
    * 4_See_also
    * 5_Notes
***** Convergence of a monotone sequence of real numbers[edit] *****
**** Lemma 1[edit] ****
If a sequence of real numbers is increasing and bounded above, then its
supremum is the limit.
**** Proof[edit] ****
Let     {  a  n   }   {\displaystyle \{a_{n}\}}  [\{ a_n \}] be such a
sequence. By assumption,     {  a  n   }   {\displaystyle \{a_{n}\}}  [\{ a_n
\}] is non-empty and bounded above. By the least-upper-bound_property of real
numbers,     c =  sup  n   {  a  n   }   {\displaystyle c=\sup _{n}\{a_{n}\}}
[c = \sup_n \{a_n\}] exists and is finite. Now, for every     &#x03B5; > 0
{\displaystyle \varepsilon >0}  [\varepsilon >0], there exists     N
{\displaystyle N}  [N] such that      a  N   > c &#x2212; &#x03B5;
{\displaystyle a_{N}>c-\varepsilon }  [a_N > c - \varepsilon ], since otherwise
c &#x2212; &#x03B5;   {\displaystyle c-\varepsilon }  [c - \varepsilon ] is an
upper bound of     {  a  n   }   {\displaystyle \{a_{n}\}}  [\{ a_n \}], which
contradicts to the definition of     c   {\displaystyle c}  [c]. Then since
{  a  n   }   {\displaystyle \{a_{n}\}}  [\{ a_n \}] is increasing, and     c
{\displaystyle c}  [c] is its upper bound, for every     n > N   {\displaystyle
n>N}  [n>N], we have      |  c &#x2212;  a  n    |  &#x2264;  |  c &#x2212;  a
N    |  < &#x03B5;   {\displaystyle |c-a_{n}|\leq |c-a_{N}|<\varepsilon }  [
{\displaystyle |c-a_{n}|\leq |c-a_{N}|<\varepsilon }]. Hence, by definition,
the limit of     {  a  n   }   {\displaystyle \{a_{n}\}}  [\{ a_n \}] is
sup  n   {  a  n   } .   {\displaystyle \sup _{n}\{a_{n}\}.}  [\sup_n \{a_n\}.]
**** Lemma 2[edit] ****
If a sequence of real numbers is decreasing and bounded below, then its infimum
is the limit.
**** Proof[edit] ****
The proof is similar to the proof for the case when the sequence is increasing
and bounded above,
**** Theorem[edit] ****
If     {  a  n   }   {\displaystyle \{a_{n}\}}  [\{ a_n \}] is a monotone
sequence of real_numbers (i.e., if an â¤ an+1 for every n â¥ 1 or an â¥ an+1
for every n â¥ 1), then this sequence has a finite limit if and only if the
sequence is bounded.[1]
**** Proof[edit] ****
    * "If"-direction: The proof follows directly from the lemmas.
    * "Only If"-direction: By definition_of_limit, every sequence     {  a  n
      }   {\displaystyle \{a_{n}\}}  [\{a_{n}\}] with a finite limit     L
      {\displaystyle L}  [L] is necessarily bounded.
***** Convergence of a monotone series[edit] *****
**** Theorem[edit] ****
If for all natural numbers j and k, aj,k is a non-negative real number and
aj,k â¤ aj+1,k, then[2]:168
          lim  j &#x2192; &#x221E;    &#x2211;  k    a  j , k   =  &#x2211;  k
      lim  j &#x2192; &#x221E;    a  j , k   .   {\displaystyle \lim _{j\to
      \infty }\sum _{k}a_{j,k}=\sum _{k}\lim _{j\to \infty }a_{j,k}.}  [\lim_
      {j\to\infty} \sum_k a_{j,k} = \sum_k \lim_{j\to\infty} a_{j,k}.]
The theorem states that if you have an infinite matrix of non-negative real
numbers such that
   1. the columns are weakly increasing and bounded, and
   2. for each row, the series whose terms are given by this row has a
      convergent sum,
then the limit of the sums of the rows is equal to the sum of the series whose
term k is given by the limit of column k (which is also its supremum). The
series has a convergent sum if and only if the (weakly increasing) sequence of
row sums is bounded and therefore convergent.
As an example, consider the infinite series of rows
                 (  1 +   1 n    )   n   =  &#x2211;  k = 0   n      (   n k
            )     /   n  k   =  &#x2211;  k = 0   n     1  k !    &#x00D7;   n
            n   &#x00D7;    n &#x2212; 1  n   &#x00D7; &#x22EF; &#x00D7;    n
            &#x2212; k + 1  n   ,   {\displaystyle \left(1+{\frac {1}
            {n}}\right)^{n}=\sum _{k=0}^{n}{\binom {n}{k}}/n^{k}=\sum _{k=0}^
            {n}{\frac {1}{k!}}\times {\frac {n}{n}}\times {\frac {n-1}
            {n}}\times \cdots \times {\frac {n-k+1}{n}},}  [{\displaystyle
            \left(1+{\frac {1}{n}}\right)^{n}=\sum _{k=0}^{n}{\binom {n}{k}}/n^
            {k}=\sum _{k=0}^{n}{\frac {1}{k!}}\times {\frac {n}{n}}\times
            {\frac {n-1}{n}}\times \cdots \times {\frac {n-k+1}{n}},}]
where n approaches infinity (the limit of this series is e). Here the matrix
entry in row n and column k is
            (   n k   )     /   n  k   =   1  k !    &#x00D7;   n n   &#x00D7;
      n &#x2212; 1  n   &#x00D7; &#x22EF; &#x00D7;    n &#x2212; k + 1  n   ;
      {\displaystyle {\binom {n}{k}}/n^{k}={\frac {1}{k!}}\times {\frac {n}
      {n}}\times {\frac {n-1}{n}}\times \cdots \times {\frac {n-k+1}{n}};}
      [\binom nk/n^k=\frac1{k!}\times\frac nn\times\frac{n-
      1}n\times\cdots\times\frac{n-k+1}n;]
the columns (fixed k) are indeed weakly increasing with n and bounded (by 1/
k!), while the rows only have finitely many nonzero terms, so condition 2 is
satisfied; the theorem now says that you can compute the limit of the row sums
( 1 + 1  /  n  )  n     {\displaystyle (1+1/n)^{n}}  [(1+1/n)^n] by taking the
sum of the column limits, namely       1  k !      {\displaystyle {\frac {1}
{k!}}}  [\frac1{k!}].
***** Beppo Levi's monotone convergence theorem for Lebesgue integral[edit]
*****
The following result is due to Beppo_Levi and Henri_Lebesgue. In what follows,
B      R   &#x2265; 0       {\displaystyle \operatorname {\mathcal {B}} _
{\mathbb {R} _{\geq 0}}}  [{\displaystyle \operatorname {\mathcal {B}} _
{\mathbb {R} _{\geq 0}}}] denotes the     &#x03C3;   {\displaystyle \sigma }
[\sigma ]-algebra of Borel sets on     [ 0 , + &#x221E; ]   {\displaystyle
[0,+\infty ]}  [{\displaystyle [0,+\infty ]}]. By definition,        B      R
&#x2265; 0       {\displaystyle \operatorname {\mathcal {B}} _{\mathbb {R} _
{\geq 0}}}  [{\displaystyle \operatorname {\mathcal {B}} _{\mathbb {R} _{\geq
0}}}] contains the set     { + &#x221E; }   {\displaystyle \{+\infty \}}  [
{\displaystyle \{+\infty \}}] and all Borel subsets of       R   &#x2265; 0   .
{\displaystyle \mathbb {R} _{\geq 0}.}  [{\displaystyle \mathbb {R} _{\geq
0}.}]
**** Theorem[edit] ****
Let     ( &#x03A9; , &#x03A3; , &#x03BC; )   {\displaystyle (\Omega ,\Sigma
,\mu )}  [(\Omega ,\Sigma ,\mu )] be a measure_space, and     X &#x2208;
&#x03A3;   {\displaystyle X\in \Sigma }  [{\displaystyle X\in \Sigma }].
Consider a pointwise non-decreasing sequence     {  f  k    }  k = 1   &#x221E;
{\displaystyle \{f_{k}\}_{k=1}^{\infty }}  [{\displaystyle \{f_{k}\}_{k=1}^
{\infty }}] of     ( &#x03A3; ,    B      R   &#x2265; 0     )   {\displaystyle
(\Sigma ,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq 0}})}  [
{\displaystyle (\Sigma ,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq
0}})}]-measurable non-negative functions      f  k   : X &#x2192; [ 0 , +
&#x221E; ]   {\displaystyle f_{k}:X\to [0,+\infty ]}  [{\displaystyle f_{k}:
X\to [0,+\infty ]}], i.e., for every      k &#x2265; 1    {\displaystyle {k\geq
1}}  [{\displaystyle {k\geq 1}}] and every      x &#x2208; X    {\displaystyle
{x\in X}}  [{\displaystyle {x\in X}}],
         0 &#x2264;  f  k   ( x ) &#x2264;  f  k + 1   ( x ) &#x2264; &#x221E;
      .   {\displaystyle 0\leq f_{k}(x)\leq f_{k+1}(x)\leq \infty .}  [
      {\displaystyle 0\leq f_{k}(x)\leq f_{k+1}(x)\leq \infty .}]
Set the pointwise limit of the sequence     {  f  n   }   {\displaystyle \{f_
{n}\}}  [\{f_{{n}}\}] to be     f   {\displaystyle f}  [f]. That is, for every
x &#x2208; X   {\displaystyle x\in X}  [x\in X],
         f ( x ) :=  lim  k &#x2192; &#x221E;    f  k   ( x ) .
      {\displaystyle f(x):=\lim _{k\to \infty }f_{k}(x).}  [{\displaystyle f
      (x):=\lim _{k\to \infty }f_{k}(x).}]
Then     f   {\displaystyle f}  [f] is     ( &#x03A3; ,    B      R   &#x2265;
0     )   {\displaystyle (\Sigma ,\operatorname {\mathcal {B}} _{\mathbb {R} _
{\geq 0}})}  [{\displaystyle (\Sigma ,\operatorname {\mathcal {B}} _{\mathbb
{R} _{\geq 0}})}]-measurable and
          lim  k &#x2192; &#x221E;    &#x222B;  X    f  k    d &#x03BC; =
      &#x222B;  X   f  d &#x03BC; .   {\displaystyle \lim _{k\to \infty }\int _
      {X}f_{k}\,d\mu =\int _{X}f\,d\mu .}  [{\displaystyle \lim _{k\to \infty
      }\int _{X}f_{k}\,d\mu =\int _{X}f\,d\mu .}]
Remark 1. The integrals may be finite or infinite.
Remark 2. The theorem remains true if its assumptions hold     &#x03BC;
{\displaystyle \mu }  [\mu ]-almost everywhere. In other words, it is enough
that there is a null_set     N   {\displaystyle N}  [N] such that the sequence
{  f  n   ( x ) }   {\displaystyle \{f_{n}(x)\}}  [\{f_{n}(x)\}] non-decreases
for every      x &#x2208; X &#x2216; N  .   {\displaystyle {x\in X\setminus
N}.}  [{\displaystyle {x\in X\setminus N}.}] To see why this is true, we start
with an observation that allowing the sequence     {  f  n   }   {\displaystyle
\{f_{n}\}}  [\{ f_n \}] to pointwise non-decrease almost everywhere causes its
pointwise limit     f   {\displaystyle f}  [f] to be undefined on some null set
N   {\displaystyle N}  [N]. On that null set,     f   {\displaystyle f}  [f]
may then be defined arbitrarily, e.g. as zero, or in any other way that
preserves measurability. To see why this will not affect the outcome of the
theorem, note that since      &#x03BC; ( N ) = 0  ,   {\displaystyle {\mu
(N)=0},}  [{\displaystyle {\mu (N)=0},}] we have, for every     k ,
{\displaystyle k,}  [k,]
          &#x222B;  X    f  k    d &#x03BC; =  &#x222B;  X &#x2216; N    f  k
      d &#x03BC;   {\displaystyle \int _{X}f_{k}\,d\mu =\int _{X\setminus N}f_
      {k}\,d\mu }  [{\displaystyle \int _{X}f_{k}\,d\mu =\int _{X\setminus N}f_
      {k}\,d\mu }] and      &#x222B;  X   f  d &#x03BC; =  &#x222B;  X &#x2216;
      N   f  d &#x03BC; ,   {\displaystyle \int _{X}f\,d\mu =\int _{X\setminus
      N}f\,d\mu ,}  [{\displaystyle \int _{X}f\,d\mu =\int _{X\setminus
      N}f\,d\mu ,}]
provided that     f   {\displaystyle f}  [f] is     ( &#x03A3; ,    B      R
&#x2265; 0     )   {\displaystyle (\Sigma ,\operatorname {\mathcal {B}} _
{\mathbb {R} _{\geq 0}})}  [{\displaystyle (\Sigma ,\operatorname {\mathcal
{B}} _{\mathbb {R} _{\geq 0}})}]-measurable.[3](section 21.38) (These
equalities follow directly from the definition of Lebesgue integral for a non-
negative function).
Remark 3. Under assumptions of the theorem,
   1.     f ( x ) =  lim&#x2006;inf  k    f  k   ( x ) =  lim&#x2006;sup  k
      f  k   ( x ) =  sup  k    f  k   ( x )    {\displaystyle \textstyle f
      (x)=\liminf _{k}f_{k}(x)=\limsup _{k}f_{k}(x)=\sup _{k}f_{k}(x)}  [
      {\displaystyle \textstyle f(x)=\liminf _{k}f_{k}(x)=\limsup _{k}f_{k}
      (x)=\sup _{k}f_{k}(x)}]
   2.      lim&#x2006;inf  k    &#x222B;  X    f  k    d &#x03BC; =
      lim&#x2006;sup  k    &#x222B;  X    f  k    d &#x03BC; =  lim  k
      &#x222B;  X    f  k    d &#x03BC; =  sup  k    &#x222B;  X    f  k    d
      &#x03BC;     {\displaystyle \textstyle \liminf _{k}\int _{X}f_{k}\,d\mu
      =\textstyle \limsup _{k}\int _{X}f_{k}\,d\mu =\lim _{k}\int _{X}f_
      {k}\,d\mu =\sup _{k}\int _{X}f_{k}\,d\mu }  [{\displaystyle \textstyle
      \liminf _{k}\int _{X}f_{k}\,d\mu =\textstyle \limsup _{k}\int _{X}f_
      {k}\,d\mu =\lim _{k}\int _{X}f_{k}\,d\mu =\sup _{k}\int _{X}f_{k}\,d\mu
      }]
(Note that the second chain of equalities follows from Remark 5).
Remark 4. The proof below does not use any properties of Lebesgue integral
except those established here. The theorem, thus, can be used to prove other
basic properties, such as linearity, pertaining to Lebesgue integration.
Remark 5 (monotonicity of Lebesgue integral). In the proof below, we apply the
monotonic property of Lebesgue integral to non-negative functions only.
Specifically (see Remark 4), let the functions     f , g : X &#x2192; [ 0 , +
&#x221E; ]   {\displaystyle f,g:X\to [0,+\infty ]}  [{\displaystyle f,g:X\to
[0,+\infty ]}] be     ( &#x03A3; ,    B      R   &#x2265; 0     )
{\displaystyle (\Sigma ,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq 0}})}
[{\displaystyle (\Sigma ,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq
0}})}]-measurable.
    * If     f &#x2264; g   {\displaystyle f\leq g}  [{\displaystyle f\leq g}]
      everywhere on     X ,   {\displaystyle X,}  [X,] then
          &#x222B;  X   f  d &#x03BC; &#x2264;  &#x222B;  X   g  d &#x03BC; .
      {\displaystyle \int _{X}f\,d\mu \leq \int _{X}g\,d\mu .}  [{\displaystyle
      \int _{X}f\,d\mu \leq \int _{X}g\,d\mu .}]
    * If      X  1   ,  X  2   &#x2208; &#x03A3;   {\displaystyle X_{1},X_
      {2}\in \Sigma }  [{\displaystyle X_{1},X_{2}\in \Sigma }] and      X  1
      &#x2286;  X  2   ,   {\displaystyle X_{1}\subseteq X_{2},}  [
      {\displaystyle X_{1}\subseteq X_{2},}] then
          &#x222B;   X  1     f  d &#x03BC; &#x2264;  &#x222B;   X  2     f  d
      &#x03BC; .   {\displaystyle \int _{X_{1}}f\,d\mu \leq \int _{X_
      {2}}f\,d\mu .}  [{\displaystyle \int _{X_{1}}f\,d\mu \leq \int _{X_
      {2}}f\,d\mu .}]
Proof. Denote     SF &#x2061; ( h )   {\displaystyle \operatorname {SF} (h)}  [
{\displaystyle \operatorname {SF} (h)}] the set of simple     ( &#x03A3; ,    B
R   &#x2265; 0     )   {\displaystyle (\Sigma ,\operatorname {\mathcal {B}} _
{\mathbb {R} _{\geq 0}})}  [{\displaystyle (\Sigma ,\operatorname {\mathcal
{B}} _{\mathbb {R} _{\geq 0}})}]-measurable functions     s : X &#x2192; [ 0 ,
&#x221E; )   {\displaystyle s:X\to [0,\infty )}  [{\displaystyle s:X\to
[0,\infty )}] such that     0 &#x2264; s &#x2264; h   {\displaystyle 0\leq
s\leq h}  [{\displaystyle 0\leq s\leq h}] everywhere on     X .
{\displaystyle X.}  [X.]
1. Since     f &#x2264; g ,   {\displaystyle f\leq g,}  [{\displaystyle f\leq
g,}] we have
         SF &#x2061; ( f ) &#x2286; SF &#x2061; ( g ) .   {\displaystyle
      \operatorname {SF} (f)\subseteq \operatorname {SF} (g).}  [{\displaystyle
      \operatorname {SF} (f)\subseteq \operatorname {SF} (g).}]
By definition of Lebesgue integral and the properties of supremum,
          &#x222B;  X   f  d &#x03BC; =  sup  s &#x2208;   S F   ( f )
      &#x222B;  X   s  d &#x03BC; &#x2264;  sup  s &#x2208;   S F   ( g )
      &#x222B;  X   s  d &#x03BC; =  &#x222B;  X   g  d &#x03BC; .
      {\displaystyle \int _{X}f\,d\mu =\sup _{s\in {\rm {SF}}(f)}\int _
      {X}s\,d\mu \leq \sup _{s\in {\rm {SF}}(g)}\int _{X}s\,d\mu =\int _
      {X}g\,d\mu .}  [{\displaystyle \int _{X}f\,d\mu =\sup _{s\in {\rm {SF}}
      (f)}\int _{X}s\,d\mu \leq \sup _{s\in {\rm {SF}}(g)}\int _{X}s\,d\mu
      =\int _{X}g\,d\mu .}]
2. Let        1     X  1       {\displaystyle {\mathbf {1} }_{X_{1}}}  [
{\displaystyle {\mathbf {1} }_{X_{1}}}] be the indicator function of the set
X  1   .   {\displaystyle X_{1}.}  [{\displaystyle X_{1}.}] It can be deduced
from the definition of Lebesgue integral that
          &#x222B;   X  2     f &#x22C5;    1     X  1      d &#x03BC; =
      &#x222B;   X  1     f  d &#x03BC;   {\displaystyle \int _{X_{2}}f\cdot
      {\mathbf {1} }_{X_{1}}\,d\mu =\int _{X_{1}}f\,d\mu }  [{\displaystyle
      \int _{X_{2}}f\cdot {\mathbf {1} }_{X_{1}}\,d\mu =\int _{X_{1}}f\,d\mu }]
if we notice that, for every     s &#x2208;   S F   ( f &#x22C5;    1     X  1
) ,   {\displaystyle s\in {\rm {SF}}(f\cdot {\mathbf {1} }_{X_{1}}),}  [
{\displaystyle s\in {\rm {SF}}(f\cdot {\mathbf {1} }_{X_{1}}),}]     s = 0
{\displaystyle s=0}  [s=0] outside of      X  1   .   {\displaystyle X_{1}.}  [
{\displaystyle X_{1}.}] Combined with the previous property, the inequality
f &#x22C5;    1     X  1     &#x2264; f   {\displaystyle f\cdot {\mathbf {1} }_
{X_{1}}\leq f}  [{\displaystyle f\cdot {\mathbf {1} }_{X_{1}}\leq f}] implies
          &#x222B;   X  1     f  d &#x03BC; =  &#x222B;   X  2     f &#x22C5;
      1     X  1      d &#x03BC; &#x2264;  &#x222B;   X  2     f  d &#x03BC; .
      {\displaystyle \int _{X_{1}}f\,d\mu =\int _{X_{2}}f\cdot {\mathbf {1} }_
      {X_{1}}\,d\mu \leq \int _{X_{2}}f\,d\mu .}  [{\displaystyle \int _{X_
      {1}}f\,d\mu =\int _{X_{2}}f\cdot {\mathbf {1} }_{X_{1}}\,d\mu \leq \int _
      {X_{2}}f\,d\mu .}]
**** Proof[edit] ****
This proof does not rely on Fatou's_lemma. However, we do explain how that
lemma might be used.
For those not interested in independent proof, the intermediate results below
may be skipped.
*** Intermediate results[edit] ***
** Lebesgue integral as measure[edit] **
Lemma 1. Let     ( &#x03A9; , &#x03A3; , &#x03BC; )   {\displaystyle (\Omega
,\Sigma ,\mu )}  [(\Omega ,\Sigma ,\mu )] be a measurable space. Consider a
simple     ( &#x03A3; ,    B      R   &#x2265; 0     )   {\displaystyle (\Sigma
,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq 0}})}  [{\displaystyle
(\Sigma ,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq 0}})}]-measurable
non-negative function     s : &#x03A9; &#x2192;    R   &#x2265; 0
{\displaystyle s:\Omega \to {\mathbb {R} _{\geq 0}}}  [{\displaystyle s:\Omega
\to {\mathbb {R} _{\geq 0}}}]. For a subset     S &#x2286; &#x03A9;
{\displaystyle S\subseteq \Omega }  [{\displaystyle S\subseteq \Omega }],
define
         &#x03BD; ( S ) =  &#x222B;  S   s  d &#x03BC;   {\displaystyle \nu
      (S)=\int _{S}s\,d\mu }  [{\displaystyle \nu (S)=\int _{S}s\,d\mu }].
Then     &#x03BD;   {\displaystyle \nu }  [\nu ] is a measure on     &#x03A9;
{\displaystyle \Omega }  [\Omega ].
* Proof[edit] *
Monotonicity follows from Remark 5. Here, we will only prove countable
additivity, leaving the rest up to the reader. Let     S =  &#x222A;  i = 1
&#x221E;    S  i     {\displaystyle S=\cup _{i=1}^{\infty }S_{i}}  [
{\displaystyle S=\cup _{i=1}^{\infty }S_{i}}], where all the sets      S  i
{\displaystyle S_{i}}  [S_{i}] are pairwise disjoint. Due to simplicity,
         s =  &#x2211;  i = 1   n    c  i   &#x22C5;    1     A  i
      {\displaystyle s=\sum _{i=1}^{n}c_{i}\cdot {\mathbf {1} }_{A_{i}}}  [
      {\displaystyle s=\sum _{i=1}^{n}c_{i}\cdot {\mathbf {1} }_{A_{i}}}],
for some finite non-negative constants      c  i   &#x2208;    R    &#x2265; 0
{\displaystyle c_{i}\in {\mathbb {R} }_{\geq 0}}  [{\displaystyle c_{i}\in
{\mathbb {R} }_{\geq 0}}] and pairwise disjoint sets      A  i   &#x2208;
&#x03A3;   {\displaystyle A_{i}\in \Sigma }  [{\displaystyle A_{i}\in \Sigma }]
such that      &#x222A;  i = 1   n    A  i   = &#x03A9;   {\displaystyle \cup _
{i=1}^{n}A_{i}=\Omega }  [{\displaystyle \cup _{i=1}^{n}A_{i}=\Omega }]. By
definition of Lebesgue integral,
             &#x03BD; ( S )    =  &#x2211;  i = 1   n    c  i   &#x22C5;
      &#x03BC; ( S &#x2229;  A  i   )       =  &#x2211;  i = 1   n    c  i
      &#x22C5; &#x03BC;   (   (  &#x222A;  j = 1   &#x221E;    S  j   )
      &#x2229;  A  i     )         =  &#x2211;  i = 1   n    c  i   &#x22C5;
      &#x03BC;   (    &#x222A;  j = 1   &#x221E;   (  S  j   &#x2229;  A  i   )
      )         {\displaystyle {\begin{aligned}\nu (S)&=\sum _{i=1}^{n}c_
      {i}\cdot \mu (S\cap A_{i})\\&=\sum _{i=1}^{n}c_{i}\cdot \mu {\bigl (}
      (\cup _{j=1}^{\infty }S_{j})\cap A_{i}{\bigr )}\\&=\sum _{i=1}^{n}c_
      {i}\cdot \mu {\bigl (}\cup _{j=1}^{\infty }(S_{j}\cap A_{i}){\bigr )}\end
      {aligned}}}  [{\displaystyle {\begin{aligned}\nu (S)&=\sum _{i=1}^{n}c_
      {i}\cdot \mu (S\cap A_{i})\\&=\sum _{i=1}^{n}c_{i}\cdot \mu {\bigl (}
      (\cup _{j=1}^{\infty }S_{j})\cap A_{i}{\bigr )}\\&=\sum _{i=1}^{n}c_
      {i}\cdot \mu {\bigl (}\cup _{j=1}^{\infty }(S_{j}\cap A_{i}){\bigr )}\end
      {aligned}}}]
Since all the sets      S  j   &#x2229;  A  i     {\displaystyle S_{j}\cap A_
{i}}  [{\displaystyle S_{j}\cap A_{i}}] are pairwise disjoint, the countable
additivity of     &#x03BC;   {\displaystyle \mu }  [\mu ] gives us
          &#x2211;  i = 1   n    c  i   &#x22C5; &#x03BC;   (    &#x222A;  j =
      1   &#x221E;   (  S  j   &#x2229;  A  i   )   )   =  &#x2211;  i = 1   n
      c  i   &#x22C5;  &#x2211;  j = 1   &#x221E;   &#x03BC; (  S  j   &#x2229;
      A  i   ) .   {\displaystyle \sum _{i=1}^{n}c_{i}\cdot \mu {\bigl (}\cup _
      {j=1}^{\infty }(S_{j}\cap A_{i}){\bigr )}=\sum _{i=1}^{n}c_{i}\cdot \sum
      _{j=1}^{\infty }\mu (S_{j}\cap A_{i}).}  [{\displaystyle \sum _{i=1}^
      {n}c_{i}\cdot \mu {\bigl (}\cup _{j=1}^{\infty }(S_{j}\cap A_{i}){\bigr
      )}=\sum _{i=1}^{n}c_{i}\cdot \sum _{j=1}^{\infty }\mu (S_{j}\cap A_
      {i}).}]
Since all the summands are non-negative, the sum of the series, whether this
sum is finite or infinite, cannot change if summation order does. For that
reason,
              &#x2211;  i = 1   n    c  i   &#x22C5;  &#x2211;  j = 1
      &#x221E;   &#x03BC; (  S  j   &#x2229;  A  i   )    =  &#x2211;  j = 1
      &#x221E;    &#x2211;  i = 1   n    c  i   &#x22C5; &#x03BC; (  S  j
      &#x2229;  A  i   )       =  &#x2211;  j = 1   &#x221E;    &#x222B;   S  j
      s  d &#x03BC;       =  &#x2211;  j = 1   &#x221E;   &#x03BD; (  S  j   )
      ,       {\displaystyle {\begin{aligned}\sum _{i=1}^{n}c_{i}\cdot \sum _
      {j=1}^{\infty }\mu (S_{j}\cap A_{i})&=\sum _{j=1}^{\infty }\sum _{i=1}^
      {n}c_{i}\cdot \mu (S_{j}\cap A_{i})\\&=\sum _{j=1}^{\infty }\int _{S_
      {j}}s\,d\mu \\&=\sum _{j=1}^{\infty }\nu (S_{j}),\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\sum _{i=1}^{n}c_{i}\cdot \sum _{j=1}^
      {\infty }\mu (S_{j}\cap A_{i})&=\sum _{j=1}^{\infty }\sum _{i=1}^{n}c_
      {i}\cdot \mu (S_{j}\cap A_{i})\\&=\sum _{j=1}^{\infty }\int _{S_
      {j}}s\,d\mu \\&=\sum _{j=1}^{\infty }\nu (S_{j}),\end{aligned}}}]
as required.
** "Continuity from below"[edit] **
The following property is a direct consequence of the definition of measure.
Lemma 2. Let     &#x03BC;   {\displaystyle \mu }  [\mu ] be a measure, and
S =  &#x222A;  i = 1   &#x221E;    S  i     {\displaystyle S=\cup _{i=1}^
{\infty }S_{i}}  [{\displaystyle S=\cup _{i=1}^{\infty }S_{i}}], where
          S  1   &#x2286; &#x2026; &#x2286;  S  i   &#x2286;  S  i + 1
      &#x2286; &#x2026; &#x2286; S   {\displaystyle S_{1}\subseteq \ldots
      \subseteq S_{i}\subseteq S_{i+1}\subseteq \ldots \subseteq S}  [
      {\displaystyle S_{1}\subseteq \ldots \subseteq S_{i}\subseteq S_
      {i+1}\subseteq \ldots \subseteq S}]
is a non-decreasing chain with all its sets     &#x03BC;   {\displaystyle \mu }
[\mu ]-measurable. Then
         &#x03BC; ( S ) =  lim  i   &#x03BC; (  S  i   )   {\displaystyle \mu
      (S)=\lim _{i}\mu (S_{i})}  [{\displaystyle \mu (S)=\lim _{i}\mu (S_
      {i})}].
*** Proof of theorem[edit] ***
Step 1. We begin by showing that     f   {\displaystyle f}  [f] is
( &#x03A3; ,    B      R   &#x2265; 0     )   {\displaystyle (\Sigma
,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq 0}})}  [{\displaystyle
(\Sigma ,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq 0}})}]âmeasurable.
[3](section 21.3)
Note. If we were using Fatou's lemma, the measurability would follow easily
from Remark 3(a).
To do this without using Fatou's lemma, it is sufficient to show that the
inverse image of an interval     [ 0 , t ]   {\displaystyle [0,t]}  [[0,t]]
under     f   {\displaystyle f}  [f] is an element of the sigma-algebra
&#x03A3;   {\displaystyle \Sigma }  [\Sigma ] on     X   {\displaystyle X}
[X], because (closed) intervals generate the Borel_sigma_algebra on the reals.
Since     [ 0 , t ]   {\displaystyle [0,t]}  [[0,t]] is a closed interval, and,
for every     k   {\displaystyle k}  [k],     0 &#x2264;  f  k   ( x ) &#x2264;
f ( x )   {\displaystyle 0\leq f_{k}(x)\leq f(x)}  [{\displaystyle 0\leq f_{k}
(x)\leq f(x)}],
         0 &#x2264; f ( x ) &#x2264; t  &#x21D4;    [   &#x2200; k  0 &#x2264;
      f  k   ( x ) &#x2264; t   ]   .   {\displaystyle 0\leq f(x)\leq t\quad
      \Leftrightarrow \quad {\Bigl [}\forall k\quad 0\leq f_{k}(x)\leq t{\Bigr
      ]}.}  [{\displaystyle 0\leq f(x)\leq t\quad \Leftrightarrow \quad {\Bigl
      [}\forall k\quad 0\leq f_{k}(x)\leq t{\Bigr ]}.}]
Thus,
         { x &#x2208; X &#x2223; 0 &#x2264; f ( x ) &#x2264; t } =  &#x22C2;  k
      { x &#x2208; X &#x2223; 0 &#x2264;  f  k   ( x ) &#x2264; t } .
      {\displaystyle \{x\in X\mid 0\leq f(x)\leq t\}=\bigcap _{k}\{x\in X\mid
      0\leq f_{k}(x)\leq t\}.}  [{\displaystyle \{x\in X\mid 0\leq f(x)\leq
      t\}=\bigcap _{k}\{x\in X\mid 0\leq f_{k}(x)\leq t\}.}]
Being the inverse image of a Borel_set under a     ( &#x03A3; ,    B      R
&#x2265; 0     )   {\displaystyle (\Sigma ,\operatorname {\mathcal {B}} _
{\mathbb {R} _{\geq 0}})}  [{\displaystyle (\Sigma ,\operatorname {\mathcal
{B}} _{\mathbb {R} _{\geq 0}})}]-measurable function      f  k
{\displaystyle f_{k}}  [f_{k}], each set in the countable intersection is an
element of     &#x03A3;   {\displaystyle \Sigma }  [\Sigma ]. Since
&#x03C3;   {\displaystyle \sigma }  [\sigma ]-algebras are, by definition,
closed under countable intersections, this shows that     f   {\displaystyle f}
[f] is     ( &#x03A3; ,    B      R   &#x2265; 0     )   {\displaystyle (\Sigma
,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq 0}})}  [{\displaystyle
(\Sigma ,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq 0}})}]-measurable,
and the integral       &#x222B;  X   f  d &#x03BC;    {\displaystyle \textstyle
\int _{X}f\,d\mu }  [{\displaystyle \textstyle \int _{X}f\,d\mu }] is well
defined (and possibly infinite).
Step 2. We will first show that       &#x222B;  X   f  d &#x03BC; &#x2265;  lim
k    &#x222B;  X    f  k    d &#x03BC; .    {\displaystyle \textstyle \int _
{X}f\,d\mu \geq \lim _{k}\int _{X}f_{k}\,d\mu .}  [{\displaystyle \textstyle
\int _{X}f\,d\mu \geq \lim _{k}\int _{X}f_{k}\,d\mu .}]
The definition of     f   {\displaystyle f}  [f] and monotonicity of     {  f
k   }   {\displaystyle \{f_{k}\}}  [\{f_{k}\}] imply that     f ( x ) &#x2265;
f  k   ( x )   {\displaystyle f(x)\geq f_{k}(x)}  [{\displaystyle f(x)\geq f_
{k}(x)}], for every     k   {\displaystyle k}  [k] and every     x &#x2208; X
{\displaystyle x\in X}  [x\in X]. By monotonicity (or, more precisely, its
narrower version established in Remark 5; see also Remark 4) of Lebesgue
integral,
          &#x222B;  X   f  d &#x03BC; &#x2265;  &#x222B;  X    f  k    d
      &#x03BC; ,   {\displaystyle \int _{X}f\,d\mu \geq \int _{X}f_{k}\,d\mu ,}
      [{\displaystyle \int _{X}f\,d\mu \geq \int _{X}f_{k}\,d\mu ,}]
and
          &#x222B;  X   f  d &#x03BC; &#x2265;  lim  k    &#x222B;  X    f  k
      d &#x03BC; .   {\displaystyle \int _{X}f\,d\mu \geq \lim _{k}\int _{X}f_
      {k}\,d\mu .}  [{\displaystyle \int _{X}f\,d\mu \geq \lim _{k}\int _{X}f_
      {k}\,d\mu .}]
Note that the limit on the right exists (finite or infinite) because, due to
monotonicity (see Remark 5 and Remark 4), the sequence is non-decreasing.
End of Step 2.
We now prove the reverse inequality. We seek to show that
          &#x222B;  X   f  d &#x03BC; &#x2264;  lim  k    &#x222B;  X    f  k
      d &#x03BC;   {\displaystyle \int _{X}f\,d\mu \leq \lim _{k}\int _{X}f_
      {k}\,d\mu }  [{\displaystyle \int _{X}f\,d\mu \leq \lim _{k}\int _{X}f_
      {k}\,d\mu }].
Proof using Fatou's lemma. Per Remark 3, the inequality we want to prove is
equivalent to
          &#x222B;  X    lim&#x2006;inf  k    f  k   ( x )  d &#x03BC; &#x2264;
      lim&#x2006;inf  k    &#x222B;  X    f  k    d &#x03BC;   {\displaystyle
      \int _{X}\liminf _{k}f_{k}(x)\,d\mu \leq \liminf _{k}\int _{X}f_{k}\,d\mu
      }  [{\displaystyle \int _{X}\liminf _{k}f_{k}(x)\,d\mu \leq \liminf _
      {k}\int _{X}f_{k}\,d\mu }].
But the latter follows immediately from Fatou's lemma, and the proof is
complete.
Independent proof. To prove the inequality without using Fatou's lemma, we need
some extra machinery. Denote     SF &#x2061; ( f )   {\displaystyle
\operatorname {SF} (f)}  [{\displaystyle \operatorname {SF} (f)}] the set of
simple     ( &#x03A3; ,    B      R   &#x2265; 0     )   {\displaystyle (\Sigma
,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq 0}})}  [{\displaystyle
(\Sigma ,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq 0}})}]-measurable
functions     s : X &#x2192; [ 0 , &#x221E; )   {\displaystyle s:X\to [0,\infty
)}  [{\displaystyle s:X\to [0,\infty )}] such that     0 &#x2264; s &#x2264; f
{\displaystyle 0\leq s\leq f}  [{\displaystyle 0\leq s\leq f}] on     X
{\displaystyle X}  [X].
Step 3. Given a simple function     s &#x2208; SF &#x2061; ( f )
{\displaystyle s\in \operatorname {SF} (f)}  [{\displaystyle s\in \operatorname
{SF} (f)}] and a real number     t &#x2208; ( 0 , 1 )   {\displaystyle t\in
(0,1)}  [{\displaystyle t\in (0,1)}], define
          B  k   s , t   = { x &#x2208; X &#x2223; t &#x22C5; s ( x ) &#x2264;
      f  k   ( x ) } &#x2286; X .   {\displaystyle B_{k}^{s,t}=\{x\in X\mid
      t\cdot s(x)\leq f_{k}(x)\}\subseteq X.}  [{\displaystyle B_{k}^{s,t}=\
      {x\in X\mid t\cdot s(x)\leq f_{k}(x)\}\subseteq X.}]
Then      B  k   s , t   &#x2208; &#x03A3;   {\displaystyle B_{k}^{s,t}\in
\Sigma }  [{\displaystyle B_{k}^{s,t}\in \Sigma }],      B  k   s , t
&#x2286;  B  k + 1   s , t     {\displaystyle B_{k}^{s,t}\subseteq B_{k+1}^
{s,t}}  [{\displaystyle B_{k}^{s,t}\subseteq B_{k+1}^{s,t}}], and      X =
&#x22C3;  k    B  k   s , t      {\displaystyle \textstyle X=\bigcup _{k}B_{k}^
{s,t}}  [{\displaystyle \textstyle X=\bigcup _{k}B_{k}^{s,t}}].
Step 3a. To prove the first claim, let      s =  &#x2211;  i = 1   m    c  i
&#x22C5;    1     A  i        {\displaystyle \textstyle s=\sum _{i=1}^{m}c_
{i}\cdot {\mathbf {1} }_{A_{i}}}  [{\displaystyle \textstyle s=\sum _{i=1}^
{m}c_{i}\cdot {\mathbf {1} }_{A_{i}}}], for some finite collection of pairwise
disjoint measurable sets      A  i   &#x2208; &#x03A3;   {\displaystyle A_
{i}\in \Sigma }  [{\displaystyle A_{i}\in \Sigma }] such that      X =
&#x222A;  i = 1   m    A  i      {\displaystyle \textstyle X=\cup _{i=1}^{m}A_
{i}}  [{\displaystyle \textstyle X=\cup _{i=1}^{m}A_{i}}], some (finite) non-
negative constants      c  i   &#x2208;    R    &#x2265; 0     {\displaystyle
c_{i}\in {\mathbb {R} }_{\geq 0}}  [{\displaystyle c_{i}\in {\mathbb {R} }_
{\geq 0}}], and        1     A  i       {\displaystyle {\mathbf {1} }_{A_{i}}}
[{\displaystyle {\mathbf {1} }_{A_{i}}}] denoting the indicator function of the
set      A  i     {\displaystyle A_{i}}  [A_{i}].
For every     x &#x2208;  A  i   ,   {\displaystyle x\in A_{i},}  [
{\displaystyle x\in A_{i},}]     t &#x22C5; s ( x ) &#x2264;  f  k   ( x )
{\displaystyle t\cdot s(x)\leq f_{k}(x)}  [{\displaystyle t\cdot s(x)\leq f_{k}
(x)}] holds if and only if      f  k   ( x ) &#x2208; [ t &#x22C5;  c  i   , +
&#x221E; ] .   {\displaystyle f_{k}(x)\in [t\cdot c_{i},+\infty ].}  [
{\displaystyle f_{k}(x)\in [t\cdot c_{i},+\infty ].}] Given that the sets
A  i     {\displaystyle A_{i}}  [A_{i}] are pairwise disjoint,
          B  k   s , t   =  &#x22C3;  i = 1   m     (    f  k   &#x2212; 1
      (   [ t &#x22C5;  c  i   , + &#x221E; ]   )   &#x2229;  A  i     )
      {\displaystyle B_{k}^{s,t}=\bigcup _{i=1}^{m}{\Bigl (}f_{k}^{-1}{\Bigl (}
      [t\cdot c_{i},+\infty ]{\Bigr )}\cap A_{i}{\Bigr )}}  [{\displaystyle B_
      {k}^{s,t}=\bigcup _{i=1}^{m}{\Bigl (}f_{k}^{-1}{\Bigl (}[t\cdot c_
      {i},+\infty ]{\Bigr )}\cap A_{i}{\Bigr )}}].
Since the pre-image      f  k   &#x2212; 1     (   [ t &#x22C5;  c  i   , +
&#x221E; ]   )     {\displaystyle f_{k}^{-1}{\Bigl (}[t\cdot c_{i},+\infty ]
{\Bigr )}}  [{\displaystyle f_{k}^{-1}{\Bigl (}[t\cdot c_{i},+\infty ]{\Bigr
)}}] of the Borel set     [ t &#x22C5;  c  i   , + &#x221E; ]   {\displaystyle
[t\cdot c_{i},+\infty ]}  [{\displaystyle [t\cdot c_{i},+\infty ]}] under the
measurable function      f  k     {\displaystyle f_{k}}  [f_{k}] is measurable,
and     &#x03C3;   {\displaystyle \sigma }  [\sigma ]-algebras, by definition,
are closed under finite intersection and unions, the first claim follows.
Step 3b. To prove the second claim, note that, for each     k   {\displaystyle
k}  [k] and every     x &#x2208; X   {\displaystyle x\in X}  [x\in X],      f
k   ( x ) &#x2264;  f  k + 1   ( x ) .   {\displaystyle f_{k}(x)\leq f_{k+1}
(x).}  [{\displaystyle f_{k}(x)\leq f_{k+1}(x).}]
Step 3c. To prove the third claim, we show that      X &#x2286;  &#x22C3;  k
B  k   s , t      {\displaystyle \textstyle X\subseteq \bigcup _{k}B_{k}^{s,t}}
[{\displaystyle \textstyle X\subseteq \bigcup _{k}B_{k}^{s,t}}].
Indeed, if, to the contrary,      X &#x2288;  &#x22C3;  k    B  k   s , t
{\displaystyle \textstyle X\not \subseteq \bigcup _{k}B_{k}^{s,t}}  [
{\displaystyle \textstyle X\not \subseteq \bigcup _{k}B_{k}^{s,t}}], then an
element
           x  0   &#x2208; X &#x2216;  &#x22C3;  k    B  k   s , t   =
      &#x22C2;  k   ( X &#x2216;  B  k   s , t   )    {\displaystyle \textstyle
      x_{0}\in X\setminus \bigcup _{k}B_{k}^{s,t}=\bigcap _{k}(X\setminus B_
      {k}^{s,t})}  [{\displaystyle \textstyle x_{0}\in X\setminus \bigcup _
      {k}B_{k}^{s,t}=\bigcap _{k}(X\setminus B_{k}^{s,t})}]
exists such that      f  k   (  x  0   ) < t &#x22C5; s (  x  0   )
{\displaystyle f_{k}(x_{0})<t\cdot s(x_{0})}  [{\displaystyle f_{k}(x_
{0})<t\cdot s(x_{0})}], for every     k   {\displaystyle k}  [k]. Taking the
limit as     k &#x2192; &#x221E;   {\displaystyle k\to \infty }  [k\to \infty
], we get
         f (  x  0   ) &#x2264; t &#x22C5; s (  x  0   ) < s (  x  0   )
      {\displaystyle f(x_{0})\leq t\cdot s(x_{0})<s(x_{0})}  [{\displaystyle f
      (x_{0})\leq t\cdot s(x_{0})<s(x_{0})}].
But by initial assumption,     s &#x2264; f   {\displaystyle s\leq f}  [
{\displaystyle s\leq f}]. This is a contradiction.
Step 4. For every simple     ( &#x03A3; ,    B      R   &#x2265; 0     )
{\displaystyle (\Sigma ,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq 0}})}
[{\displaystyle (\Sigma ,\operatorname {\mathcal {B}} _{\mathbb {R} _{\geq
0}})}]-measurable non-negative function      s  2     {\displaystyle s_{2}}
[s_{2}],
          lim  n    &#x222B;   B  n   s , t      s  2    d &#x03BC; =  &#x222B;
      X    s  2    d &#x03BC;   {\displaystyle \lim _{n}\int _{B_{n}^{s,t}}s_
      {2}\,d\mu =\int _{X}s_{2}\,d\mu }  [{\displaystyle \lim _{n}\int _{B_{n}^
      {s,t}}s_{2}\,d\mu =\int _{X}s_{2}\,d\mu }].
To prove this, define      &#x03BD; ( S ) =  &#x222B;  S    s  2    d &#x03BC;
{\displaystyle \textstyle \nu (S)=\int _{S}s_{2}\,d\mu }  [{\displaystyle
\textstyle \nu (S)=\int _{S}s_{2}\,d\mu }]. By Lemma 1,     &#x03BD; ( S )
{\displaystyle \nu (S)}  [{\displaystyle \nu (S)}] is a measure on     &#x03A9;
{\displaystyle \Omega }  [\Omega ]. By "continuity from below" (Lemma 2),
          lim  n    &#x222B;   B  n   s , t      s  2    d &#x03BC; =  lim  n
      &#x03BD; (  B  n   s , t   ) = &#x03BD; ( X ) =  &#x222B;  X    s  2    d
      &#x03BC;   {\displaystyle \lim _{n}\int _{B_{n}^{s,t}}s_{2}\,d\mu =\lim _
      {n}\nu (B_{n}^{s,t})=\nu (X)=\int _{X}s_{2}\,d\mu }  [{\displaystyle \lim
      _{n}\int _{B_{n}^{s,t}}s_{2}\,d\mu =\lim _{n}\nu (B_{n}^{s,t})=\nu
      (X)=\int _{X}s_{2}\,d\mu }],
as required.
Step 5. We now prove that, for every     s &#x2208; SF &#x2061; ( f )
{\displaystyle s\in \operatorname {SF} (f)}  [{\displaystyle s\in \operatorname
{SF} (f)}],
          &#x222B;  X   s  d &#x03BC; &#x2264;  lim  k    &#x222B;  X    f  k
      d &#x03BC;   {\displaystyle \int _{X}s\,d\mu \leq \lim _{k}\int _{X}f_
      {k}\,d\mu }  [{\displaystyle \int _{X}s\,d\mu \leq \lim _{k}\int _{X}f_
      {k}\,d\mu }].
Indeed, using the definition of      B  k   s , t     {\displaystyle B_{k}^
{s,t}}  [{\displaystyle B_{k}^{s,t}}], the non-negativity of      f  k
{\displaystyle f_{k}}  [f_{k}], and the monotonicity of Lebesgue integral (see
Remark 5 and Remark 4), we have
          &#x222B;   B  k   s , t     t &#x22C5; s  d &#x03BC; &#x2264;
      &#x222B;   B  k   s , t      f  k    d &#x03BC; &#x2264;  &#x222B;  X
      f  k    d &#x03BC;   {\displaystyle \int _{B_{k}^{s,t}}t\cdot s\,d\mu
      \leq \int _{B_{k}^{s,t}}f_{k}\,d\mu \leq \int _{X}f_{k}\,d\mu }  [
      {\displaystyle \int _{B_{k}^{s,t}}t\cdot s\,d\mu \leq \int _{B_{k}^
      {s,t}}f_{k}\,d\mu \leq \int _{X}f_{k}\,d\mu }],
for every     k &#x2265; 1   {\displaystyle k\geq 1}  [k\geq 1]. In accordance
with Step 4, as     k &#x2192; &#x221E;   {\displaystyle k\to \infty }  [k\to
\infty ], the inequality becomes
         t  &#x222B;  X   s  d &#x03BC; &#x2264;  lim  k    &#x222B;  X    f  k
      d &#x03BC; .   {\displaystyle t\int _{X}s\,d\mu \leq \lim _{k}\int _{X}f_
      {k}\,d\mu .}  [{\displaystyle t\int _{X}s\,d\mu \leq \lim _{k}\int _{X}f_
      {k}\,d\mu .}]
Taking the limit as     t &#x2191; 1   {\displaystyle t\uparrow 1}  [
{\displaystyle t\uparrow 1}] yields
          &#x222B;  X   s  d &#x03BC; &#x2264;  lim  k    &#x222B;  X    f  k
      d &#x03BC;   {\displaystyle \int _{X}s\,d\mu \leq \lim _{k}\int _{X}f_
      {k}\,d\mu }  [{\displaystyle \int _{X}s\,d\mu \leq \lim _{k}\int _{X}f_
      {k}\,d\mu }],
as required.
Step 6. We are now able to prove the reverse inequality, i.e.
          &#x222B;  X   f  d &#x03BC; &#x2264;  lim  k    &#x222B;  X    f  k
      d &#x03BC;   {\displaystyle \int _{X}f\,d\mu \leq \lim _{k}\int _{X}f_
      {k}\,d\mu }  [{\displaystyle \int _{X}f\,d\mu \leq \lim _{k}\int _{X}f_
      {k}\,d\mu }].
Indeed, by non-negativity,      f  +   = f   {\displaystyle f_{+}=f}  [
{\displaystyle f_{+}=f}] and      f  &#x2212;   = 0.   {\displaystyle f_{-}=0.}
[{\displaystyle f_{-}=0.}] For the calculation below, the non-negativity of
f   {\displaystyle f}  [f] is essential. Applying the definition of Lebesgue
integral and the inequality established in Step 5, we have
          &#x222B;  X   f  d &#x03BC; =  sup  s &#x2208; SF &#x2061; ( f )
      &#x222B;  X   s  d &#x03BC; &#x2264;  lim  k    &#x222B;  X    f  k    d
      &#x03BC; .   {\displaystyle \int _{X}f\,d\mu =\sup _{s\in \operatorname
      {SF} (f)}\int _{X}s\,d\mu \leq \lim _{k}\int _{X}f_{k}\,d\mu .}  [
      {\displaystyle \int _{X}f\,d\mu =\sup _{s\in \operatorname {SF} (f)}\int
      _{X}s\,d\mu \leq \lim _{k}\int _{X}f_{k}\,d\mu .}]
The proof is complete.
***** See also[edit] *****
    * Infinite_series
    * Dominated_convergence_theorem
***** Notes[edit] *****
   1. ^ A generalisation of this theorem was given byBibby, John (1974).
      "Axiomatisations of the average and a further generalisation of monotonic
      sequences". Glasgow_Mathematical_Journal. 15 (1): 63â65. doi:10.1017/
      S0017089500002135.
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
   3. ^ See for instanceYeh, J. (2006). Real Analysis: Theory of Measure and
      Integration. Hackensack, NJ: World Scientific. ISBN 981-256-653-8.
   4. ^ a b See for instanceSchechter, Erik (1997). Handbook of Analysis and
      Its Foundations. San Diego: Academic Press. ISBN 0-12-622760-8.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Monotone_convergence_theorem&oldid=898596773"
Categories:
    * Theorems_in_calculus
    * Sequences_and_series
    * Theorems_in_real_analysis
    * Theorems_in_measure_theory
Hidden categories:
    * Articles_containing_proofs
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
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 24 May 2019, at 17:00 (UTC).
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
