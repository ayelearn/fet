The following text has been accessed from https://en.wikipedia.org/wiki/Uniform_convergence at Fri Aug 9 02:35:06 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Uniform convergence ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In the mathematical field of analysis, uniform convergence is a mode of
convergence of functions stronger than pointwise_convergence. A sequence of
functions     (  f  n   )   {\displaystyle (f_{n})}  [(f_{n})] converges
uniformly to a limiting function     f   {\displaystyle f}  [f] on a set     E
{\displaystyle E}  [E] if, given any arbitrarily small positive number
&#x03F5;   {\displaystyle \epsilon }  [\epsilon ], a number     N
{\displaystyle N}  [N] can be found such that each of the functions      f  N
,  f  N + 1   ,  f  N + 2   , &#x2026;   {\displaystyle f_{N},f_{N+1},f_
{N+2},\ldots }  [{\displaystyle f_{N},f_{N+1},f_{N+2},\ldots }] differ from
f   {\displaystyle f}  [f] by no more than     &#x03F5;   {\displaystyle
\epsilon }  [\epsilon ] at every point     x   {\displaystyle x}  [x] in     E
{\displaystyle E}  [E]. Described in an informal way, if      f  n
{\displaystyle f_{n}}  [f_{n}] converges to     f   {\displaystyle f}  [f]
uniformly, then the rate at which      f  n   ( x )   {\displaystyle f_{n}(x)}
[f_{n}(x)] approaches     f ( x )   {\displaystyle f(x)}  [f(x)] is "uniform"
throughout its domain in the following sense: in order to determine how large
n   {\displaystyle n}  [n] needs to be to guarantee that      f  n   ( x )
{\displaystyle f_{n}(x)}  [f_{n}(x)] falls within a certain distance
&#x03F5;   {\displaystyle \epsilon }  [\epsilon ] of     f ( x )
{\displaystyle f(x)}  [f(x)], we do not need to know the value of     x
&#x2208; E   {\displaystyle x\in E}  [x\in E] in question â there is a single
value of     N = N ( &#x03F5; )   {\displaystyle N=N(\epsilon )}  [
{\displaystyle N=N(\epsilon )}] independent of     x   {\displaystyle x}  [x],
such that choosing     n   {\displaystyle n}  [n] to be larger than     N
{\displaystyle N}  [N] will suffice.
The difference between uniform convergence and pointwise convergence was not
fully appreciated early in the history of calculus, leading to instances of
faulty reasoning. The concept, which was first formalized by Karl_Weierstrass,
is important because several properties of the functions      f  n
{\displaystyle f_{n}}  [f_{n}], such as continuity, Riemann_integrability, and,
with additional hypotheses, differentiability, are transferred to the limit
f   {\displaystyle f}  [f] if the convergence is uniform, but not necessarily
if the convergence is not uniform.
⁰
***** Contents *****
    * 1_History
    * 2_Definition
          o 2.1_Notes
          o 2.2_Generalizations
          o 2.3_Definition_in_a_hyperreal_setting
    * 3_Examples
          o 3.1_Exponential_function
    * 4_Properties
    * 5_Applications
          o 5.1_To_continuity
          o 5.2_To_differentiability
          o 5.3_To_integrability
          o 5.4_To_analyticity
          o 5.5_To_series
    * 6_Almost_uniform_convergence
    * 7_See_also
    * 8_Notes
    * 9_References
    * 10_External_links
***** History[edit] *****
In 1821 Augustin-Louis_Cauchy published a proof that a convergent sum of
continuous functions is always continuous, to which Niels_Henrik_Abel in 1826
found purported counterexamples in the context of Fourier_series, arguing that
Cauchy's proof had to be incorrect. Completely standard notions of convergence
did not exist at the time, and Cauchy handled convergence using infinitesimal
methods. When put into the modern language, what Cauchy proved is that a
uniformly convergent sequence of continuous functions has a continuous limit.
The failure of a merely pointwise-convergent limit of continuous functions to
converge to a continuous function illustrates the importance of distinguishing
between different types of convergence when handling sequences of functions.[1]
The term uniform convergence was probably first used by Christoph_Gudermann, in
an 1838 paper on elliptic_functions, where he employed the phrase "convergence
in a uniform way" when the "mode of convergence" of a series        &#x2211;  n
= 1   &#x221E;    f  n   ( x , &#x03D5; , &#x03C8; )     {\displaystyle
\textstyle {\sum _{n=1}^{\infty }f_{n}(x,\phi ,\psi )}}  [\textstyle {\sum _
{n=1}^{\infty }f_{n}(x,\phi ,\psi )}] is independent of the variables
&#x03D5;   {\displaystyle \phi }  [\phi ] and     &#x03C8; .   {\displaystyle
\psi .}  [\psi .] While he thought it a "remarkable fact" when a series
converged in this way, he did not give a formal definition, nor use the
property in any of his proofs.[2]
Later Gudermann's pupil Karl_Weierstrass, who attended his course on elliptic
functions in 1839â1840, coined the term gleichmÃ¤Ãig konvergent (German:
uniformly convergent) which he used in his 1841 paper Zur Theorie der
Potenzreihen, published in 1894. Independently, similar concepts were
articulated by Philipp_Ludwig_von_Seidel[3] and George_Gabriel_Stokes. G._H.
Hardy compares the three definitions in his paper "Sir George Stokes and the
concept of uniform convergence" and remarks: "Weierstrass's discovery was the
earliest, and he alone fully realized its far-reaching importance as one of the
fundamental ideas of analysis."
Under the influence of Weierstrass and Bernhard_Riemann this concept and
related questions were intensely studied at the end of the 19th century by
Hermann_Hankel, Paul_du_Bois-Reymond, Ulisse_Dini, Cesare_ArzelÃ  and others.
***** Definition[edit] *****
We first define uniform convergence for real-valued_functions, although the
concept is readily generalized to functions mapping to metric_spaces and, more
generally, uniform_spaces (see below).
Suppose     E   {\displaystyle E}  [E] is a set and     (  f  n    )  n
&#x2208;  N      {\displaystyle (f_{n})_{n\in \mathbb {N} }}  [{\displaystyle
(f_{n})_{n\in \mathbb {N} }}] is a sequence of real-valued functions on it. We
say the sequence     (  f  n    )  n &#x2208;  N      {\displaystyle (f_{n})_
{n\in \mathbb {N} }}  [{\displaystyle (f_{n})_{n\in \mathbb {N} }}] is
uniformly convergent on     E   {\displaystyle E}  [E] with limit     f : E
&#x2192;  R    {\displaystyle f:E\to \mathbb {R} }  [{\displaystyle f:E\to
\mathbb {R} }] if for every     &#x03F5; > 0 ,   {\displaystyle \epsilon >0,}
[\epsilon > 0,] there exists a natural number     N   {\displaystyle N}  [N]
such that for all     n &#x2265; N   {\displaystyle n\geq N}  [n\geq N] and
x &#x2208; E   {\displaystyle x\in E}  [x \in E]
          |   f  n   ( x ) &#x2212; f ( x )  |  < &#x03F5; .   {\displaystyle
      |f_{n}(x)-f(x)|<\epsilon .}  [{\displaystyle |f_{n}(x)-f(x)|<\epsilon .}]
The notation for uniform convergence of      f  n     {\displaystyle f_{n}}
[f_{n}] to     f   {\displaystyle f}  [f] is not quite standardized and
different authors have used a variety of symbols, including (in roughly
decreasing order of popularity):
          f  n   &#x21C9; f ,     u n i f &#xA0; l i m   n &#x2192; &#x221E;
      f  n   = f ,   f  n     &#x27F6;  u n i f .    f .   {\displaystyle f_
      {n}\rightrightarrows f,\quad {\underset {n\to \infty }{\mathrm {unif\
      lim} }}f_{n}=f,\quad f_{n}{\overset {\mathrm {unif.} }{\longrightarrow
      }}f.}  [{\displaystyle f_{n}\rightrightarrows f,\quad {\underset {n\to
      \infty }{\mathrm {unif\ lim} }}f_{n}=f,\quad f_{n}{\overset {\mathrm
      {unif.} }{\longrightarrow }}f.}]
Frequently, no special symbol is used, and authors simply write
          f  n   &#x2192; f   u n i f o r m l y    {\displaystyle f_{n}\to
      f\quad \mathrm {uniformly} }  [{\displaystyle f_{n}\to f\quad \mathrm
      {uniformly} }]
to indicate that convergence is uniform. (In contrast, the expression      f  n
&#x2192; f   {\displaystyle f_{n}\to f}  [f_{n}\to f] on     E   {\displaystyle
E}  [E] without an adverb is taken to mean pointwise_convergence on     E
{\displaystyle E}  [E]: for all     x &#x2208; E   {\displaystyle x\in E}  [
{\displaystyle x\in E}],      f  n   ( x ) &#x2192; f ( x )   {\displaystyle f_
{n}(x)\to f(x)}  [f_n(x)\to f(x)] as     n &#x2192; &#x221E;   {\displaystyle
n\to \infty }  [n\to \infty ].)
Since      R    {\displaystyle \mathbb {R} }  [\mathbb {R} ] is a complete
metric_space, the Cauchy_criterion can be used to give an equivalent
alternative formulation for uniform convergence:     (  f  n    )  n &#x2208;
N      {\displaystyle (f_{n})_{n\in \mathbb {N} }}  [(f_n)_{n\in\N}] converges
uniformly on     E   {\displaystyle E}  [E] (in the previous sense) if and only
if for every     &#x03F5; > 0   {\displaystyle \epsilon >0}  [ \epsilon > 0 ],
there exists a natural number     N   {\displaystyle N}  [N] such that
         x &#x2208; E , m , n &#x2265; N  &#x27F9;   |   f  m   ( x ) &#x2212;
      f  n   ( x )  |  < &#x03F5;   {\displaystyle x\in E,m,n\geq N\implies |f_
      {m}(x)-f_{n}(x)|<\epsilon }  [{\displaystyle x\in E,m,n\geq N\implies |f_
      {m}(x)-f_{n}(x)|<\epsilon }].
In yet another equivalent formulation, if we define
          d  n   =  sup  x &#x2208; E    |   f  n   ( x ) &#x2212; f ( x )  |
      ,   {\displaystyle d_{n}=\sup _{x\in E}|f_{n}(x)-f(x)|,}  [{\displaystyle
      d_{n}=\sup _{x\in E}|f_{n}(x)-f(x)|,}]
then      f  n     {\displaystyle f_{n}}  [f_{n}] converges to     f
{\displaystyle f}  [f] uniformly if and only if      d  n   &#x2192; 0
{\displaystyle d_{n}\to 0}  [{\displaystyle d_{n}\to 0}] as     n &#x2192;
&#x221E;   {\displaystyle n\to \infty }  [n\to \infty ]. Thus, we can
characterize uniform convergence of     (  f  n    )  n &#x2208;  N
{\displaystyle (f_{n})_{n\in \mathbb {N} }}  [{\displaystyle (f_{n})_{n\in
\mathbb {N} }}] on     E   {\displaystyle E}  [E] as (simple) convergence of
(  f  n    )  n &#x2208;  N      {\displaystyle (f_{n})_{n\in \mathbb {N} }}  [
{\displaystyle (f_{n})_{n\in \mathbb {N} }}] in the function_space       R   E
{\displaystyle \mathbb {R} ^{E}}  [{\displaystyle \mathbb {R} ^{E}}] with
respect to the uniform_metric (also called the supremum metric), defined by
         d ( f , g ) =  sup  x &#x2208; E    |  f ( x ) &#x2212; g ( x )  |  .
      {\displaystyle d(f,g)=\sup _{x\in E}|f(x)-g(x)|.}  [{\displaystyle d
      (f,g)=\sup _{x\in E}|f(x)-g(x)|.}]
Symbolically,
          f  n   &#x21C9; f  &#x27FA;   lim  n &#x2192; &#x221E;   d (  f  n
      , f ) = 0   {\displaystyle f_{n}\rightrightarrows f\iff \lim _{n\to
      \infty }d(f_{n},f)=0}  [{\displaystyle f_{n}\rightrightarrows f\iff \lim
      _{n\to \infty }d(f_{n},f)=0}].
The sequence     (  f  n    )  n &#x2208;  N      {\displaystyle (f_{n})_{n\in
\mathbb {N} }}  [{\displaystyle (f_{n})_{n\in \mathbb {N} }}] is said to be
locally uniformly convergent with limit     f   {\displaystyle f}  [f] if     E
{\displaystyle E}  [E] is a metric_space and for every     x &#x2208; E
{\displaystyle x\in E}  [x\in E], there exists an     r > 0   {\displaystyle
r>0}  [r > 0] such that     (  f  n   )   {\displaystyle (f_{n})}  [(f_{n})]
converges uniformly on     B ( x , r ) &#x2229; E .   {\displaystyle B(x,r)\cap
E.}  [{\displaystyle B(x,r)\cap E.}] It is clear that uniform convergence
implies local uniform convergence, which implies pointwise convergence.
**** Notes[edit] ****
Intuitively, a sequence of functions      f  n     {\displaystyle f_{n}}  [f_
{n}] converges uniformly to     f   {\displaystyle f}  [f] if, given an
arbitrarily small     &#x03F5; > 0   {\displaystyle \epsilon >0}  [\epsilon
>0], we can find an     N &#x2208;  N    {\displaystyle N\in \mathbb {N} }
[N\in \mathbb {N} ] so that the functions      f  n     {\displaystyle f_{n}}
[f_{n}] with     n > N   {\displaystyle n>N}  [n>N] all fall within a "tube" of
width     2 &#x03F5;   {\displaystyle 2\epsilon }  [2\epsilon] centered around
f   {\displaystyle f}  [f] (i.e., between     f ( x ) &#x2212; &#x03F5;
{\displaystyle f(x)-\epsilon }  [{\displaystyle f(x)-\epsilon }] and     f ( x
) + &#x03F5;   {\displaystyle f(x)+\epsilon }  [{\displaystyle f(x)+\epsilon
}]) for the entire domain of the function.
Note that interchanging the order of quantifiers in the definition of uniform
convergence by moving "for all     x &#x2208; E   {\displaystyle x\in E}  [x\in
E]" in front of "there exists a natural number     N   {\displaystyle N}  [N]"
results in a definition of pointwise_convergence of the sequence. To make this
difference explicit, in the case of uniform convergence,     N = N ( &#x03F5; )
{\displaystyle N=N(\epsilon )}  [{\displaystyle N=N(\epsilon )}] can only
depend on     &#x03F5;   {\displaystyle \epsilon }  [\epsilon ], and the choice
of     N   {\displaystyle N}  [N] has to work for all     x &#x2208; E
{\displaystyle x\in E}  [x\in E], for a specific value of     &#x03F5;
{\displaystyle \epsilon }  [\epsilon ] that is given. In contrast, in the case
of pointwise convergence,     N = N ( &#x03F5; , x )   {\displaystyle N=N
(\epsilon ,x)}  [{\displaystyle N=N(\epsilon ,x)}] may depend on both
&#x03F5;   {\displaystyle \epsilon }  [\epsilon ] and     x   {\displaystyle x}
[x], and the choice of     N   {\displaystyle N}  [N] only has to work for the
specific values of     &#x03F5;   {\displaystyle \epsilon }  [\epsilon ] and
x   {\displaystyle x}  [x] that are given. Thus uniform convergence implies
pointwise convergence, however the converse is not true, as the example in the
section below illustrates.
**** Generalizations[edit] ****
One may straightforwardly extend the concept to functions E â M, where (M, d)
is a metric_space, by replacing      |   f  n   ( x ) &#x2212; f ( x )  |
{\displaystyle |f_{n}(x)-f(x)|}  [{\displaystyle |f_{n}(x)-f(x)|}] with     d
(  f  n   ( x ) , f ( x ) )   {\displaystyle d(f_{n}(x),f(x))}  [{\displaystyle
d(f_{n}(x),f(x))}].
The most general setting is the uniform convergence of nets of functions E â
X, where X is a uniform_space. We say that the net     (  f  &#x03B1;   )
{\displaystyle (f_{\alpha })}  [{\displaystyle (f_{\alpha })}] converges
uniformly with limit f : E â X if and only if for every entourage V in X,
there exists an      &#x03B1;  0     {\displaystyle \alpha _{0}}  [\alpha _
{0}], such that for every x in E and every     &#x03B1; &#x2265;  &#x03B1;  0
{\displaystyle \alpha \geq \alpha _{0}}  [{\displaystyle \alpha \geq \alpha _
{0}}],     (  f  &#x03B1;   ( x ) , f ( x ) )   {\displaystyle (f_{\alpha }
(x),f(x))}  [{\displaystyle (f_{\alpha }(x),f(x))}] is in V. In this situation,
uniform limit of continuous functions remains continuous.
**** Definition in a hyperreal setting[edit] ****
Uniform convergence admits a simplified definition in a hyperreal setting.
Thus, a sequence      f  n     {\displaystyle f_{n}}  [f_{n}] converges to f
uniformly if for all x in the domain of      f  &#x2217;     {\displaystyle f^
{*}}  [f^{*}] and all infinite n,      f  n   &#x2217;   ( x )   {\displaystyle
f_{n}^{*}(x)}  [f_{n}^{*}(x)] is infinitely close to      f  &#x2217;   ( x )
{\displaystyle f^{*}(x)}  [f^{*}(x)] (see microcontinuity for a similar
definition of uniform continuity).
***** Examples[edit] *****
Given a topological_space X, we can equip the space of bounded real or complex-
valued functions over X with the uniform_norm topology, with the uniform metric
defined by
         d ( f , g ) = &#x2016; f &#x2212; g  &#x2016;  &#x221E;   =  sup  x
      &#x2208; X    |  f ( x ) &#x2212; g ( x )  |  .   {\displaystyle d
      (f,g)=\|f-g\|_{\infty }=\sup _{x\in X}|f(x)-g(x)|.}  [{\displaystyle d
      (f,g)=\|f-g\|_{\infty }=\sup _{x\in X}|f(x)-g(x)|.}]
Then uniform convergence simply means convergence in the uniform_norm topology:
          lim  n &#x2192; &#x221E;   &#x2016;  f  n   &#x2212; f  &#x2016;
      &#x221E;   = 0   {\displaystyle \lim _{n\to \infty }\|f_{n}-f\|_{\infty
      }=0}  [{\displaystyle \lim _{n\to \infty }\|f_{n}-f\|_{\infty }=0}].
The sequence of functions     (  f  n   )   {\displaystyle (f_{n})}  [(f_{n})]
           {     f  n   : [ 0 , 1 ] &#x2192; [ 0 , 1 ]      f  n   ( x ) =  x
      n           {\displaystyle {\begin{cases}f_{n}:[0,1]\to [0,1]\\f_{n}
      (x)=x^{n}\end{cases}}}  [{\displaystyle {\begin{cases}f_{n}:[0,1]\to
      [0,1]\\f_{n}(x)=x^{n}\end{cases}}}]
is a classic example of a sequence of functions that converges to a function
f   {\displaystyle f}  [f] pointwise but not uniformly. To show this, we first
observe that the pointwise limit of     (  f  n   )   {\displaystyle (f_{n})}
[(f_{n})] as     n &#x2192; &#x221E;   {\displaystyle n\to \infty }  [n\to
\infty ] is the function     f   {\displaystyle f}  [f], given by
         f ( x ) =  lim  n &#x2192; &#x221E;    f  n   ( x ) =   {    0 ,   x
      &#x2208; [ 0 , 1 ) ;     1 ,   x = 1.         {\displaystyle f(x)=\lim _
      {n\to \infty }f_{n}(x)={\begin{cases}0,&x\in [0,1);\\1,&x=1.\end{cases}}}
      [{\displaystyle f(x)=\lim _{n\to \infty }f_{n}(x)={\begin{cases}0,&x\in
      [0,1);\\1,&x=1.\end{cases}}}]
Pointwise convergence: Convergence is trivial for     x = 0   {\displaystyle
x=0}  [x=0] and     x = 1   {\displaystyle x=1}  [x=1], since      f  n   ( 0 )
= f ( 0 ) = 0   {\displaystyle f_{n}(0)=f(0)=0}  [{\displaystyle f_{n}(0)=f
(0)=0}] and      f  n   ( 1 ) = f ( 1 ) = 1   {\displaystyle f_{n}(1)=f(1)=1}
[{\displaystyle f_{n}(1)=f(1)=1}], for all     n   {\displaystyle n}  [n]. For
x &#x2208; ( 0 , 1 )   {\displaystyle x\in (0,1)}  [x\in (0,1)] and given
&#x03F5; > 0   {\displaystyle \epsilon >0}  [\epsilon >0], we can ensure that
|   f  n   ( x ) &#x2212; f ( x )  |  < &#x03F5;   {\displaystyle |f_{n}(x)-f
(x)|<\epsilon }  [{\displaystyle |f_{n}(x)-f(x)|<\epsilon }] whenever     n
&#x2265; N   {\displaystyle n\geq N}  [n\geq N] by choosing     N = &#x2308;
log &#x2061; &#x03F5;  /  log &#x2061; x &#x2309;   {\displaystyle N=\lceil
\log \epsilon /\log x\rceil }  [{\displaystyle N=\lceil \log \epsilon /\log
x\rceil }] (here the upper square brackets indicate rounding up, see ceiling
function). Hence,      f  n   &#x2192; f   {\displaystyle f_{n}\to f}  [f_
{n}\to f] pointwise for all     x &#x2208; [ 0 , 1 ]   {\displaystyle x\in
[0,1]}  [{\displaystyle x\in [0,1]}]. Note that the choice of     N
{\displaystyle N}  [N] depends on the value of     &#x03F5;   {\displaystyle
\epsilon }  [\epsilon ] and     x   {\displaystyle x}  [x]. Moreover, for a
fixed choice of     &#x03F5;   {\displaystyle \epsilon }  [\epsilon ],     N
{\displaystyle N}  [N] (which cannot be defined to be smaller) grows without
bound as     x   {\displaystyle x}  [x] approaches 1. These observations
preclude the possibility of uniform convergence.
Non-uniformity of convergence: The convergence is not uniform, because we can
find an     &#x03F5; > 0   {\displaystyle \epsilon >0}  [\epsilon >0] so that
no matter how large we choose     N ,   {\displaystyle N,}  [N,] there will be
values of     x &#x2208; [ 0 , 1 ]   {\displaystyle x\in [0,1]}  [x \in [0,1]]
and     n &#x2265; N   {\displaystyle n\geq N}  [n\geq N] such that      |   f
n   ( x ) &#x2212; f ( x )  |  &#x2265; &#x03F5; .   {\displaystyle |f_{n}(x)-f
(x)|\geq \epsilon .}  [{\displaystyle |f_{n}(x)-f(x)|\geq \epsilon .}] To see
this, first observe that regardless of how large     n   {\displaystyle n}  [n]
becomes, there is always an      x  0   &#x2208; [ 0 , 1 )   {\displaystyle x_
{0}\in [0,1)}  [x_{0}\in [0,1)] such that      f  n   (  x  0   ) = 1  /  2.
{\displaystyle f_{n}(x_{0})=1/2.}  [{\displaystyle f_{n}(x_{0})=1/2.}] Thus, if
we choose     &#x03F5; = 1  /  4 ,   {\displaystyle \epsilon =1/4,}  [
{\displaystyle \epsilon =1/4,}] we can never find an     N   {\displaystyle N}
[N] such that      |   f  n   ( x ) &#x2212; f ( x )  |  < &#x03F5;
{\displaystyle |f_{n}(x)-f(x)|<\epsilon }  [{\displaystyle |f_{n}(x)-f
(x)|<\epsilon }] for all     x &#x2208; [ 0 , 1 ]   {\displaystyle x\in [0,1]}
[{\displaystyle x\in [0,1]}] and     n &#x2265; N   {\displaystyle n\geq N}
[n\geq N]. Explicitly, whatever candidate we choose for     N   {\displaystyle
N}  [N], consider the value of      f  N     {\displaystyle f_{N}}  [f_{N}] at
x  0   = ( 1  /  2  )  1  /  N     {\displaystyle x_{0}=(1/2)^{1/N}}  [
{\displaystyle x_{0}=(1/2)^{1/N}}]. Since
          |   f  N   (  x  0   ) &#x2212; f (  x  0   )  |  =  |    [  ( 1  /
      2  )   1 N     ]   N   &#x2212; 0  |  =   1 2   >   1 4   = &#x03F5; ,
      {\displaystyle \left|f_{N}(x_{0})-f(x_{0})\right|=\left|\left[(1/2)^
      {\frac {1}{N}}\right]^{N}-0\right|={\frac {1}{2}}>{\frac {1}{4}}=\epsilon
      ,}  [{\displaystyle \left|f_{N}(x_{0})-f(x_{0})\right|=\left|\left[(1/2)^
      {\frac {1}{N}}\right]^{N}-0\right|={\frac {1}{2}}>{\frac {1}{4}}=\epsilon
      ,}]
the candidate fails because we have found an example of an     x &#x2208; [ 0 ,
1 ]   {\displaystyle x\in [0,1]}  [{\displaystyle x\in [0,1]}] that "escaped"
our attempt to "confine" each      f  n   &#xA0; ( n &#x2265; N )
{\displaystyle f_{n}\ (n\geq N)}  [{\displaystyle f_{n}\ (n\geq N)}] to within
&#x03F5;   {\displaystyle \epsilon }  [\epsilon ] of     f   {\displaystyle f}
[f] for all     x &#x2208; [ 0 , 1 ]   {\displaystyle x\in [0,1]}  [
{\displaystyle x\in [0,1]}]. In fact, it is easy to see that
          lim  n &#x2192; &#x221E;   &#x2016;  f  n   &#x2212; f  &#x2016;
      &#x221E;   = 1 ,   {\displaystyle \lim _{n\to \infty }\|f_{n}-f\|_{\infty
      }=1,}  [{\displaystyle \lim _{n\to \infty }\|f_{n}-f\|_{\infty }=1,}]
contrary to the requirement that     &#x2016;  f  n   &#x2212; f  &#x2016;
&#x221E;   &#x2192; 0   {\displaystyle \|f_{n}-f\|_{\infty }\to 0}  [
{\displaystyle \|f_{n}-f\|_{\infty }\to 0}] if      f  n   &#x21C9; f
{\displaystyle f_{n}\rightrightarrows f}  [{\displaystyle f_
{n}\rightrightarrows f}].
In this example one can easily see that pointwise convergence does not preserve
differentiability or continuity. While each function of the sequence is smooth,
that is to say that for all n,      f  n   &#x2208;  C  &#x221E;   ( [ 0 , 1 ]
)   {\displaystyle f_{n}\in C^{\infty }([0,1])}  [f_{n}\in C^{\infty }([0,1])],
the limit      lim  n &#x2192; &#x221E;    f  n     {\displaystyle \lim _{n\to
\infty }f_{n}}  [{\displaystyle \lim _{n\to \infty }f_{n}}] is not even
continuous.
**** Exponential function[edit] ****
The series expansion of the exponential_function can be shown to be uniformly
convergent on any bounded subset     S &#x2282;  C    {\displaystyle S\subset
\mathbb {C} }  [{\displaystyle S\subset \mathbb {C} }] using the Weierstrass_M-
test.
Theorem (Weierstrass M-test). Let     (  f  n   )   {\displaystyle (f_{n})}  [
(f_{n})] be a sequence of functions      f  n   : E &#x2192;  C
{\displaystyle f_{n}:E\to \mathbb {C} }  [{\displaystyle f_{n}:E\to \mathbb {C}
}] and let      M  n     {\displaystyle M_{n}}  [{\displaystyle M_{n}}] be a
sequence of positive real numbers such that      |   f  n   ( x )  |  <  M  n
{\displaystyle |f_{n}(x)|<M_{n}}  [{\displaystyle |f_{n}(x)|<M_{n}}] for all
x &#x2208; E   {\displaystyle x\in E}  [x\in E] and     n = 1 , 2 , 3 ,
&#x2026;   {\displaystyle n=1,2,3,\ldots }  [{\displaystyle n=1,2,3,\ldots }]
If      &#x2211;  n    M  n     {\textstyle \sum _{n}M_{n}}  [{\textstyle \sum
_{n}M_{n}}] converges, then      &#x2211;  n    f  n     {\textstyle \sum _
{n}f_{n}}  [{\textstyle \sum _{n}f_{n}}] converges uniformly on     E
{\displaystyle E}  [E].
The complex exponential function can be expressed as the series:
          &#x2211;  n = 0   &#x221E;      z  n    n !    .   {\displaystyle
      \sum _{n=0}^{\infty }{\frac {z^{n}}{n!}}.}  [\sum _{n=0}^{\infty }{\frac
      {z^{n}}{n!}}.]
Any bounded subset is a subset of some disc      D  R     {\displaystyle D_{R}}
[D_{R}] of radius     R ,   {\displaystyle R,}  [R,] centered on the origin in
the complex_plane. The Weierstrass M-test requires us to find an upper bound
M  n     {\displaystyle M_{n}}  [M_{n}] on the terms of the series, with      M
n     {\displaystyle M_{n}}  [M_{n}] independent of the position in the disc:
          |    z  n    n !    |  &#x2264;  M  n   , &#x2200; z &#x2208;  D  R
      .   {\displaystyle \left|{\frac {z^{n}}{n!}}\right|\leq M_{n},\forall
      z\in D_{R}.}  [{\displaystyle \left|{\frac {z^{n}}{n!}}\right|\leq M_
      {n},\forall z\in D_{R}.}]
To do this, we notice
          |    z  n    n !    |  &#x2264;     |  z   |   n     n !    &#x2264;
      R  n    n !      {\displaystyle \left|{\frac {z^{n}}{n!}}\right|\leq
      {\frac {|z|^{n}}{n!}}\leq {\frac {R^{n}}{n!}}}  [{\displaystyle \left|
      {\frac {z^{n}}{n!}}\right|\leq {\frac {|z|^{n}}{n!}}\leq {\frac {R^{n}}
      {n!}}}]
and take      M  n   =     R  n    n !     .   {\displaystyle M_{n}={\tfrac {R^
{n}}{n!}}.}  [{\displaystyle M_{n}={\tfrac {R^{n}}{n!}}.}]
If      &#x2211;  n = 0   &#x221E;    M  n     {\displaystyle \sum _{n=0}^
{\infty }M_{n}}  [\sum _{n=0}^{\infty }M_{n}] is convergent, then the M-test
asserts that the original series is uniformly convergent.
The ratio_test can be used here:
          lim  n &#x2192; &#x221E;      M  n + 1    M  n     =  lim  n &#x2192;
      &#x221E;      R  n + 1    R  n        n !   ( n + 1 ) !    =  lim  n
      &#x2192; &#x221E;     R  n + 1    = 0   {\displaystyle \lim _{n\to \infty
      }{\frac {M_{n+1}}{M_{n}}}=\lim _{n\to \infty }{\frac {R^{n+1}}{R^{n}}}
      {\frac {n!}{(n+1)!}}=\lim _{n\to \infty }{\frac {R}{n+1}}=0}  [\lim _
      {n\to \infty }{\frac {M_{n+1}}{M_{n}}}=\lim _{n\to \infty }{\frac {R^
      {n+1}}{R^{n}}}{\frac {n!}{(n+1)!}}=\lim _{n\to \infty }{\frac {R}
      {n+1}}=0]
which means the series over      M  n     {\displaystyle M_{n}}  [M_{n}] is
convergent. Thus the original series converges uniformly for all     z &#x2208;
D  R   ,   {\displaystyle z\in D_{R},}  [{\displaystyle z\in D_{R},}] and since
S &#x2282;  D  R     {\displaystyle S\subset D_{R}}  [S\subset D_{R}], the
series is also uniformly convergent on     S .   {\displaystyle S.}  [S.]
***** Properties[edit] *****
    * Every uniformly convergent sequence is locally uniformly convergent.
    * Every locally uniformly convergent sequence is compactly_convergent.
    * For locally_compact_spaces local uniform convergence and compact
      convergence coincide.
    * A sequence of continuous functions on metric spaces, with the image
      metric space being complete, is uniformly convergent if and only if it is
      uniformly_Cauchy.
    * If     S   {\displaystyle S}  [S] is a compact interval (or in general a
      compact topological space), and     (  f  n   )   {\displaystyle (f_{n})}
      [(f_{n})] is a monotone_increasing sequence (meaning      f  n   ( x )
      &#x2264;  f  n + 1   ( x )   {\displaystyle f_{n}(x)\leq f_{n+1}(x)}  [f_
      {n}(x)\leq f_{n+1}(x)] for all n and x) of continuous functions with a
      pointwise limit     f   {\displaystyle f}  [f] which is also continuous,
      then the convergence is necessarily uniform (Dini's_theorem). Uniform
      convergence is also guaranteed if     S   {\displaystyle S}  [S] is a
      compact interval and     (  f  n   )   {\displaystyle (f_{n})}  [(f_{n})]
      is an equicontinuous sequence that converges pointwise.
***** Applications[edit] *****
**** To continuity[edit] ****
Main article: Uniform_limit_theorem
Counterexample to a strengthening of the uniform convergence theorem, in which
pointwise convergence, rather than uniform convergence, is assumed. The
continuous green functions      sin  n   &#x2061; ( x )   {\displaystyle \sin ^
{n}(x)}  [\sin ^{n}(x)] converge to the non-continuous red function. This can
happen only if convergence is not uniform.
If     E   {\displaystyle E}  [E] and     M   {\displaystyle M}  [M] are
topological_spaces, then it makes sense to talk about the continuity of the
functions      f  n   , f : E &#x2192; M   {\displaystyle f_{n},f:E\to M}  [
{\displaystyle f_{n},f:E\to M}]. If we further assume that     M
{\displaystyle M}  [M] is a metric_space, then (uniform) convergence of the
f  n     {\displaystyle f_{n}}  [f_{n}] to     f   {\displaystyle f}  [f] is
also well defined. The following result states that continuity is preserved by
uniform convergence:
      Uniform limit theorem. Suppose     E   {\displaystyle E}  [E] is a
      topological space,     M   {\displaystyle M}  [M] is a metric space, and
      (  f  n   )   {\displaystyle (f_{n})}  [(f_{n})] is a sequence of
      continuous functions      f  n   : E &#x2192; M   {\displaystyle f_{n}:
      E\to M}  [{\displaystyle f_{n}:E\to M}]. If      f  n   &#x21C9; f
      {\displaystyle f_{n}\rightrightarrows f}  [{\displaystyle f_
      {n}\rightrightarrows f}] on     E   {\displaystyle E}  [E], then     f
      {\displaystyle f}  [f] is also continuous.
This theorem is proved by the "ε/3 trick", and is the archetypal example of
this trick: to prove a given inequality (ε), one uses the definitions of
continuity and uniform convergence to produce 3 inequalities (ε/3), and then
combines them via the triangle_inequality to produce the desired inequality.
This theorem is an important one in the history of real and Fourier analysis,
since many 18th century mathematicians had the intuitive understanding that a
sequence of continuous functions always converges to a continuous function. The
image above shows a counterexample, and many discontinuous functions could, in
fact, be written as a Fourier_series of continuous functions. The erroneous
claim that the pointwise limit of a sequence of continuous functions is
continuous (originally stated in terms of convergent series of continuous
functions) is infamously known as "Cauchy's wrong theorem". The uniform limit
theorem shows that a stronger form of convergence, uniform convergence, is
needed to ensure the preservation of continuity in the limit function.
More precisely, this theorem states that the uniform limit of uniformly
continuous functions is uniformly continuous; for a locally_compact space,
continuity is equivalent to local uniform continuity, and thus the uniform
limit of continuous functions is continuous.
**** To differentiability[edit] ****
If     S   {\displaystyle S}  [S] is an interval and all the functions      f
n     {\displaystyle f_{n}}  [f_{n}] are differentiable and converge to a limit
f   {\displaystyle f}  [f], it is often desirable to determine the derivative
function      f &#x2032;    {\displaystyle f'}  [f'] by taking the limit of the
sequence      f  n  &#x2032;    {\displaystyle f'_{n}}  [{\displaystyle f'_
{n}}]. This is however in general not possible: even if the convergence is
uniform, the limit function need not be differentiable (not even if the
sequence consists of everywhere-analytic functions, see Weierstrass_function),
and even if it is differentiable, the derivative of the limit function need not
be equal to the limit of the derivatives. Consider for instance      f  n   ( x
) =  n  &#x2212; 1  /  2    sin &#x2061; ( n x )    {\displaystyle f_{n}(x)=n^
{-1/2}{\sin(nx)}}  [{\displaystyle f_{n}(x)=n^{-1/2}{\sin(nx)}}] with uniform
limit      f  n   &#x21C9; f &#x2261; 0   {\displaystyle f_{n}\rightrightarrows
f\equiv 0}  [{\displaystyle f_{n}\rightrightarrows f\equiv 0}]. Clearly,      f
&#x2032;    {\displaystyle f'}  [f'] is also identically zero. However, the
derivatives of the sequence of functions are given by      f  n  &#x2032;  ( x
) =  n  1  /  2   cos &#x2061; n x ,   {\displaystyle f'_{n}(x)=n^{1/2}\cos
nx,}  [{\displaystyle f'_{n}(x)=n^{1/2}\cos nx,}] and the sequence      f  n
&#x2032;    {\displaystyle f'_{n}}  [{\displaystyle f'_{n}}] does not converge
to      f &#x2032;  ,   {\displaystyle f',}  [f',] or even to any function at
all. In order to ensure a connection between the limit of a sequence of
differentiable functions and the limit of the sequence of derivatives, the
uniform convergence of the sequence of derivatives plus the convergence of the
sequence of functions at at least one point is required. The precise statement
covering this situation is as follows:[4]
      If     (  f  n   )   {\displaystyle (f_{n})}  [(f_{n})] is a sequence of
      differentiable functions on     [ a , b ]   {\displaystyle [a,b]}  [
      [a,b]] such that      lim  n &#x2192; &#x221E;    f  n   (  x  0   )
      {\displaystyle \lim _{n\to \infty }f_{n}(x_{0})}  [{\displaystyle \lim _
      {n\to \infty }f_{n}(x_{0})}] exists (and is finite) for some      x  0
      &#x2208; [ a , b ]   {\displaystyle x_{0}\in [a,b]}  [{\displaystyle x_
      {0}\in [a,b]}] and the sequence     (  f  n  &#x2032;  )   {\displaystyle
      (f'_{n})}  [{\displaystyle (f'_{n})}] converges uniformly on     [ a , b
      ]   {\displaystyle [a,b]}  [[a,b]], then      f  n     {\displaystyle f_
      {n}}  [f_{n}] converges uniformly to a function     f   {\displaystyle f}
      [f] on     [ a , b ]   {\displaystyle [a,b]}  [[a,b]], and      f
      &#x2032;  ( x ) =  lim  n &#x2192; &#x221E;    f  n  &#x2032;  ( x )
      {\displaystyle f'(x)=\lim _{n\to \infty }f'_{n}(x)}  [{\displaystyle f'
      (x)=\lim _{n\to \infty }f'_{n}(x)}] for     x &#x2208; [ a , b ]
      {\displaystyle x\in [a,b]}  [{\displaystyle x\in [a,b]}].
**** To integrability[edit] ****
Similarly, one often wants to exchange integrals and limit processes. For the
Riemann_integral, this can be done if uniform convergence is assumed:
      If     (  f  n    )  n = 1   &#x221E;     {\displaystyle (f_{n})_{n=1}^
      {\infty }}  [(f_{n})_{n=1}^{\infty }] is a sequence of Riemann integrable
      functions defined on a compact interval     I   {\displaystyle I}  [I]
      which uniformly converge with limit     f   {\displaystyle f}  [f], then
      f   {\displaystyle f}  [f] is Riemann integrable and its integral can be
      computed as the limit of the integrals of the      f  n
      {\displaystyle f_{n}}  [f_{n}]:
                &#x222B;  I   f =  lim  n &#x2192; &#x221E;    &#x222B;  I    f
            n   .   {\displaystyle \int _{I}f=\lim _{n\to \infty }\int _{I}f_
            {n}.}  [\int _{I}f=\lim _{n\to \infty }\int _{I}f_{n}.]
In fact, for a uniformly convergent family of bounded functions on an interval,
the upper and lower Riemann integrals converge to the upper and lower Riemann
integrals of the limit function. This follows because, for n sufficiently
large, the graph of      f  n     {\displaystyle f_{n}}  [f_{n}] is within ε of
the graph of f, and so the upper sum and lower sum of      f  n
{\displaystyle f_{n}}  [f_{n}] are each within     &#x03B5;  |  I  |
{\displaystyle \varepsilon |I|}  [\varepsilon |I|] of the value of the upper
and lower sums of     f   {\displaystyle f}  [f], respectively.
Much stronger theorems in this respect, which require not much more than
pointwise convergence, can be obtained if one abandons the Riemann integral and
uses the Lebesgue_integral instead.
**** To analyticity[edit] ****
If a sequence of analytic functions converges uniformly in a region S of the
complex plane, then the limit is analytic in S. This example demonstrates that
complex functions are more well-behaved than real functions, since the uniform
limit of analytic functions on a real interval need not even be differentiable
(see Weierstrass_function).
**** To series[edit] ****
We say that       &#x2211;  n = 1   &#x221E;    f  n      {\displaystyle
\textstyle \sum _{n=1}^{\infty }f_{n}}  [\textstyle \sum _{n=1}^{\infty }f_{n}]
converges:
i) pointwise on E if and only if the sequence of partial sums      s  n   ( x )
=  &#x2211;  j = 1   n    f  j   ( x )   {\displaystyle s_{n}(x)=\sum _{j=1}^
{n}f_{j}(x)}  [{\displaystyle s_{n}(x)=\sum _{j=1}^{n}f_{j}(x)}] converges for
every     x &#x2208; E   {\displaystyle x\in E}  [x\in E].
ii) uniformly on E if and only if sn converges uniformly as     n &#x2192;
&#x221E;   {\displaystyle n\to \infty }  [n\to \infty ].
iii) absolutely on E if and only if       &#x2211;  n = 1   &#x221E;    |   f
n    |     {\displaystyle \textstyle \sum _{n=1}^{\infty }|f_{n}|}  [\textstyle
\sum _{n=1}^{\infty }|f_{n}|] converges for every     x &#x2208; E
{\displaystyle x\in E}  [x\in E].
With this definition comes the following result:
     Let x0 be contained in the set E and each fn be continuous at x0. If
     f =  &#x2211;  n = 1   &#x221E;    f  n      {\displaystyle
     \textstyle f=\sum _{n=1}^{\infty }f_{n}}  [{\displaystyle \textstyle
     f=\sum _{n=1}^{\infty }f_{n}}] converges uniformly on E then f is
     continuous at x0 in E. Suppose that     E = [ a , b ]
     {\displaystyle E=[a,b]}  [{\displaystyle E=[a,b]}] and each fn is
     integrable on E. If       &#x2211;  n = 1   &#x221E;    f  n
     {\displaystyle \textstyle \sum _{n=1}^{\infty }f_{n}}  [\textstyle
     \sum _{n=1}^{\infty }f_{n}] converges uniformly on E then f is
     integrable on E and the series of integrals of fn is equal to
     integral of the series of fn.
***** Almost uniform convergence[edit] *****
If the domain of the functions is a measure_space E then the related notion of
almost uniform convergence can be defined. We say a sequence of functions
(  f  n   )   {\displaystyle (f_{n})}  [(f_{n})] converges almost uniformly on
E if for every     &#x03B4; > 0   {\displaystyle \delta >0}  [\delta >0] there
exists a measurable set      E  &#x03B4;     {\displaystyle E_{\delta }}  [E_
{\delta }] with measure less than     &#x03B4;   {\displaystyle \delta }
[\delta ] such that the sequence of functions     (  f  n   )   {\displaystyle
(f_{n})}  [(f_{n})] converges uniformly on     E &#x2216;  E  &#x03B4;
{\displaystyle E\setminus E_{\delta }}  [E\setminus E_{\delta }]. In other
words, almost uniform convergence means there are sets of arbitrarily small
measure for which the sequence of functions converges uniformly on their
complement.
Note that almost uniform convergence of a sequence does not mean that the
sequence converges uniformly almost_everywhere as might be inferred from the
name. However, Egorov's_theorem does guarantee that on a finite measure space,
a sequence of functions that converges almost_everywhere also converges almost
uniformly on the same set.
Almost uniform convergence implies almost_everywhere_convergence and
convergence_in_measure.
***** See also[edit] *****
    * Uniform_convergence_in_probability
    * Modes_of_convergence_(annotated_index)
    * Dini's_theorem
    * ArzelÃ âAscoli_theorem
***** Notes[edit] *****
   1. ^SÃ¸rensen, Henrik Kragh (2005). "Exceptions and counterexamples:
      Understanding Abel's comment on Cauchy's Theorem". Historia Mathematica.
      32 (4): 453â480. doi:10.1016/j.hm.2004.11.010.
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
   3. ^Jahnke, Hans Niels (2003). "6.7 The Foundation of Analysis in the 19th
      Century: Weierstrass". A history of analysis. AMS Bookstore. ISBN 978-0-
      8218-2623-2, p._184.
   4. ^Lakatos,_Imre (1976). Proofs_and_Refutations. Cambridge University
      Press. p. 141. ISBN 978-0-521-21078-2.
   5. ^ Rudin, Walter (1976). Principles_of_Mathematical_Analysis 3rd edition,
      Theorem 7.17. McGraw-Hill: New York.
***** References[edit] *****
    * Konrad_Knopp,Theory and Application of Infinite Series; Blackie and Son,
      London, 1954, reprinted by Dover Publications,
ISBN 0-486-66165-2.
G._H._Hardy,Sir George Stokes and the concept of uniform convergence;
Proceedings_of_the_Cambridge_Philosophical_Society, 19, pp. 148â156 (1918)
Bourbaki;Elements of Mathematics: General Topology. Chapters 5â10
(Paperback);
ISBN 0-387-19374-X
Walter_Rudin,Principles of Mathematical Analysis, 3rd ed., McGrawâHill, 1976.
Gerald_Folland, Real Analysis: Modern Techniques and Their Applications, Second
Edition, John Wiley & Sons, Inc., 1999,
ISBN 0-471-31716-0.
William Wade,An Introduction to Analysis, 3rd ed., Pearson, 2005
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Uniform_convergence",
      Encyclopedia_of_Mathematics, Springer Science+Business Media B.V. /
      Kluwer Academic Publishers, ISBN 978-1-55608-010-4
"Uniform_convergence". PlanetMath.
"Limit_point_of_function". PlanetMath.
"Converges_uniformly". PlanetMath.
"Convergent_series". PlanetMath.
Graphic_examples_of_uniform_convergence_of_Fourier_series from the University
of Colorado

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Uniform_convergence&oldid=906880067"
Categories:
    * Calculus
    * Mathematical_series
    * Topology_of_function_spaces
    * Convergence_(mathematics)
Hidden categories:
    * Articles_containing_German-language_text
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * FranÃ§ais
    * íêµ­ì´
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 18 July 2019, at 22:13 (UTC).
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
