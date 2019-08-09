The following text has been accessed from https://en.wikipedia.org/wiki/Fourier_series at Fri Aug 9 03:27:04 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Fourier series ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Decomposition of periodic functions into sums of simpler sinusoidal forms
Fourier_transforms
Continuous_Fourier_transform
Fourier series
Discrete-time_Fourier_transform
Discrete_Fourier_transform
Discrete_Fourier_transform_over_a_ring
Fourier_analysis
Related_transforms
In mathematics, a Fourier series (/ËfÊrieÉª,_-iÉr/)[1] is a periodic
function composed of harmonically related sinusoids, combined by a weighted
summation. With appropriate weights, one cycle (or period) of the summation can
be made to approximate an arbitrary function in that interval (or the entire
function if it too is periodic). As such, the summation is a synthesis of
another function. The discrete-time_Fourier_transform is an example of Fourier
series. The process of deriving the weights that describe a given function is a
form of Fourier_analysis. For functions on unbounded intervals, the analysis
and synthesis analogies are Fourier_transform and inverse transform.
Function     s ( x )   {\displaystyle s(x)}  [s(x)] (in red) is a sum of six
sine functions of different amplitudes and harmonically related frequencies.
Their summation is called a Fourier series. The Fourier transform,     S ( f )
{\displaystyle S(f)}  [S(f)] (in blue), which depicts amplitude vs frequency,
reveals the 6 frequencies (at odd harmonics) and their amplitudes (1/odd
number).
⁰
***** Contents *****
    * 1_History
    * 2_Definition
          o 2.1_Complex-valued_functions
          o 2.2_Other_common_notations
    * 3_Convergence
    * 4_Examples
          o 4.1_Example_1:_a_simple_Fourier_series
          o 4.2_Example_2:_Fourier's_motivation
          o 4.3_Other_applications
    * 5_Beginnings
          o 5.1_Birth_of_harmonic_analysis
    * 6_Extensions
          o 6.1_Fourier_series_on_a_square
          o 6.2_Fourier_series_of_Bravais-lattice-periodic-function
          o 6.3_Hilbert_space_interpretation
    * 7_Properties
          o 7.1_Table_of_basic_properties
          o 7.2_Symmetry_properties
          o 7.3_RiemannâLebesgue_lemma
          o 7.4_Derivative_property
          o 7.5_Parseval's_theorem
          o 7.6_Plancherel's_theorem
          o 7.7_Convolution_theorems
          o 7.8_Compact_groups
          o 7.9_Riemannian_manifolds
          o 7.10_Locally_compact_Abelian_groups
    * 8_Table_of_common_Fourier_series
    * 9_Approximation_and_convergence_of_Fourier_series
          o 9.1_Least_squares_property
          o 9.2_Convergence
          o 9.3_Divergence
    * 10_See_also
    * 11_Notes
    * 12_References
          o 12.1_Further_reading
    * 13_External_links
***** History[edit] *****
See also: Fourier_analysis_Â§ History
The Fourier series is named in honour of Jean-Baptiste_Joseph_Fourier
(1768â1830), who made important contributions to the study of trigonometric
series, after preliminary investigations by Leonhard_Euler, Jean_le_Rond
d'Alembert, and Daniel_Bernoulli.[nb_1] Fourier introduced the series for the
purpose of solving the heat_equation in a metal plate, publishing his initial
results in his 1807 MÃ©moire_sur_la_propagation_de_la_chaleur_dans_les_corps
solides (Treatise on the propagation of heat in solid bodies), and publishing
his ThÃ©orie analytique de la chaleur (Analytical theory of heat) in 1822. The
MÃ©moire introduced Fourier analysis, specifically Fourier series. Through
Fourier's research the fact was established that an arbitrary (continuous)[2]
function can be represented by a trigonometric series. The first announcement
of this great discovery was made by Fourier in 1807, before the French_Academy.
[3] Early ideas of decomposing a periodic function into the sum of simple
oscillating functions date back to the 3rd century BC, when ancient astronomers
proposed an empiric model of planetary motions, based on deferents_and
epicycles.
The heat_equation is a partial_differential_equation. Prior to Fourier's work,
no solution to the heat equation was known in the general case, although
particular solutions were known if the heat source behaved in a simple way, in
particular, if the heat source was a sine or cosine wave. These simple
solutions are now sometimes called eigensolutions. Fourier's idea was to model
a complicated heat source as a superposition (or linear_combination) of simple
sine and cosine waves, and to write the solution_as_a_superposition of the
corresponding eigensolutions. This superposition or linear combination is
called the Fourier series.
From a modern point of view, Fourier's results are somewhat informal, due to
the lack of a precise notion of function and integral in the early nineteenth
century. Later, Peter_Gustav_Lejeune_Dirichlet[4] and Bernhard_Riemann[5][6][7]
expressed Fourier's results with greater precision and formality.
Although the original motivation was to solve the heat equation, it later
became obvious that the same techniques could be applied to a wide array of
mathematical and physical problems, and especially those involving linear
differential equations with constant coefficients, for which the eigensolutions
are sinusoids. The Fourier series has many such applications in electrical
engineering, vibration analysis, acoustics, optics, signal_processing, image
processing, quantum_mechanics, econometrics,[8] thin-walled_shell theory,[9]
etc.
***** Definition[edit] *****
Consider a real-valued function,     s ( x ) ,   {\displaystyle s(x),}  [
{\displaystyle s(x),}]  that is integrable on an interval of length     P ,
{\displaystyle P,}  [P,]  which will be the period of the Fourier series. 
Common examples of analysis intervals are:
         x &#x2208; [ 0 , 1 ] ,   {\displaystyle x\in [0,1],}  [{\displaystyle
      x\in [0,1],}] and     P = 1.   {\displaystyle P=1.}  [{\displaystyle
      P=1.}]
         x &#x2208; [ &#x2212; &#x03C0; , &#x03C0; ] ,   {\displaystyle x\in [-
      \pi ,\pi ],}  [{\displaystyle x\in [-\pi ,\pi ],}] and     P = 2 &#x03C0;
      .   {\displaystyle P=2\pi .}  [{\displaystyle P=2\pi .}]
The analysis process determines the weights, indexed by integer     n ,
{\displaystyle n,}  [{\displaystyle n,}] which is also the number of cycles of
the      n  th     {\displaystyle n^{\text{th}}}  [n^{{\text{th}}}] harmonic in
the analysis interval. Therefore, the length of a cycle, in the units of     x
,   {\displaystyle x,}  [x,] is     P  /  n .   {\displaystyle P/n.}  [
{\displaystyle P/n.}]  And the corresponding harmonic frequency is     n  /  P
.   {\displaystyle n/P.}  [{\displaystyle n/P.}]       sin &#x2061;  (  2
&#x03C0; x    n P     )    {\displaystyle \sin \left(2\pi x{\tfrac {n}
{P}}\right)}  [{\displaystyle \sin \left(2\pi x{\tfrac {n}{P}}\right)}] and
cos &#x2061;  (  2 &#x03C0; x    n P     )    {\displaystyle \cos \left(2\pi x
{\tfrac {n}{P}}\right)}  [{\displaystyle \cos \left(2\pi x{\tfrac {n}
{P}}\right)}] are      n  t h     {\displaystyle n^{th}}  [n^{th}] harmonics,
and their amplitudes (weights) are found by integration over the interval of
length     P   {\displaystyle P}  [P]:[10]
Fourier coefficients
        a  n      =   2 P    &#x222B;  P   s ( x ) &#x22C5; cos
&#x2061;  (  2 &#x03C0; x    n P     )  &#xA0; d x      b  n
=   2 P    &#x222B;  P   s ( x ) &#x22C5; sin &#x2061;  (  2
&#x03C0; x    n P     )  &#xA0; d x .       {\displaystyle {\begin
{aligned}a_{n}&={\frac {2}{P}}\int _{P}s(x)\cdot \cos \left(2\pi x    
{\tfrac {n}{P}}\right)\ dx\\b_{n}&={\frac {2}{P}}\int _{P}s             (Eq.1)
(x)\cdot \sin \left(2\pi x{\tfrac {n}{P}}\right)\ dx.\end
{aligned}}}  [{\displaystyle {\begin{aligned}a_{n}&={\frac {2}
{P}}\int _{P}s(x)\cdot \cos \left(2\pi x{\tfrac {n}{P}}\right)\
dx\\b_{n}&={\frac {2}{P}}\int _{P}s(x)\cdot \sin \left(2\pi x
{\tfrac {n}{P}}\right)\ dx.\end{aligned}}}]
          * If     s ( x )   {\displaystyle s(x)}  [s(x)] is     P
            {\displaystyle P}  [P]-periodic, then any interval of that length
            is sufficient.
          *     a  0     {\displaystyle a_{0}}  [a_{0}] and      b  0
            {\displaystyle b_{0}}  [b_{0}] can be reduced to just:       a  0
            =   2 P    &#x222B;  P   s ( x )  d x   {\displaystyle a_{0}={\frac
            {2}{P}}\int _{P}s(x)\;dx}  [{\displaystyle a_{0}={\frac {2}{P}}\int
            _{P}s(x)\;dx}]   and        b  0   = 0.   {\displaystyle b_{0}=0.}
            [{\displaystyle b_{0}=0.}]
          * Many texts choose     P = 2 &#x03C0;   {\displaystyle P=2\pi }  [
            {\displaystyle P=2\pi }] to simplify the argument of the sinusoid
            functions.
The synthesis process (the actual Fourier series) is:
Fourier series, sine-cosine form
        s  N   ( x ) =    a  0   2   +  &#x2211;  n = 1   N
(   a  n   cos &#x2061;  (     2 &#x03C0; n x  P    )  +  b  n
sin &#x2061;  (     2 &#x03C0; n x  P    )   )  .
{\displaystyle {\begin{aligned}s_{N}(x)={\frac {a_{0}}{2}}+\sum _     
{n=1}^{N}\left(a_{n}\cos \left({\tfrac {2\pi nx}{P}}\right)+b_          (Eq.2)
{n}\sin \left({\tfrac {2\pi nx}{P}}\right)\right).\end{aligned}}}
[{\displaystyle {\begin{aligned}s_{N}(x)={\frac {a_{0}}{2}}+\sum _
{n=1}^{N}\left(a_{n}\cos \left({\tfrac {2\pi nx}{P}}\right)+b_
{n}\sin \left({\tfrac {2\pi nx}{P}}\right)\right).\end{aligned}}}]
In general, integer     N   {\displaystyle N}  [N] is theoretically infinite.
Even so, the series might not converge or exactly equate to     s ( x )
{\displaystyle s(x)}  [s(x)] at all values of     x   {\displaystyle x}  [x]
(such as a single-point discontinuity) in the analysis interval.  For the
"well-behaved" functions typical of physical processes, equality is customarily
assumed.
If     s ( t )   {\displaystyle s(t)}  [s(t)] is a function contained in an
interval of length     P   {\displaystyle P}  [P] (and zero elsewhere), the
upper-right quadrant is an example of what its Fourier series coefficients
(     A  n     {\displaystyle A_{n}}  [A_{n}]) might look like when plotted
against their corresponding harmonic frequencies. The upper-left quadrant is
the corresponding Fourier transform of     s ( t ) .   {\displaystyle s(t).}
[s(t).] The Fourier series summation (not shown) synthesizes a periodic
summation of     s ( t ) ,   {\displaystyle s(t),}  [s(t),] whereas the inverse
Fourier transform (not shown) synthesizes only     s ( t ) .   {\displaystyle s
(t).}  [s(t).]
Using a trigonometric identity:
          A  n   &#x22C5; cos &#x2061;  (      2 &#x03C0; n x  P    &#x2212;
      &#x03C6;  n    )  &#xA0; &#x2261; &#xA0;      A  n   cos &#x2061;
      (  &#x03C6;  n   )  &#x23DF;     a  n     &#x22C5; cos &#x2061;  (     2
      &#x03C0; n x  P    )  +      A  n   sin &#x2061; (  &#x03C6;  n   )
      &#x23DF;     b  n     &#x22C5; sin &#x2061;  (     2 &#x03C0; n x  P    )
      ,   {\displaystyle A_{n}\cdot \cos \left({\tfrac {2\pi nx}{P}}-\varphi _
      {n}\right)\ \equiv \ \underbrace {A_{n}\cos(\varphi _{n})} _{a_{n}}\cdot
      \cos \left({\tfrac {2\pi nx}{P}}\right)+\underbrace {A_{n}\sin(\varphi _
      {n})} _{b_{n}}\cdot \sin \left({\tfrac {2\pi nx}{P}}\right),}  [
      {\displaystyle A_{n}\cdot \cos \left({\tfrac {2\pi nx}{P}}-\varphi _
      {n}\right)\ \equiv \ \underbrace {A_{n}\cos(\varphi _{n})} _{a_{n}}\cdot
      \cos \left({\tfrac {2\pi nx}{P}}\right)+\underbrace {A_{n}\sin(\varphi _
      {n})} _{b_{n}}\cdot \sin \left({\tfrac {2\pi nx}{P}}\right),}]
and definitions:       A  n   &#x225C;    a  n   2   +  b  n   2     ;
{\displaystyle A_{n}\triangleq {\sqrt {a_{n}^{2}+b_{n}^{2}}};}  [{\displaystyle
A_{n}\triangleq {\sqrt {a_{n}^{2}+b_{n}^{2}}};}]       &#x03C6;  n   &#x225C;
arctan2 &#x2061; (  b  n   ,  a  n   ) ,   {\displaystyle \varphi _
{n}\triangleq \operatorname {arctan2} (b_{n},a_{n}),}  [{\displaystyle \varphi
_{n}\triangleq \operatorname {arctan2} (b_{n},a_{n}),}]  the sine and cosine
pairs can be expressed as a single sinusoid with a phase offset, analogous to
the conversion between orthogonal (Cartesian) and polar coordinates:
Fourier series, amplitude-phase form
    s  N   ( x ) =    A  0   2   +  &#x2211;  n = 1   N    A  n
&#x22C5; cos &#x2061;  (      2 &#x03C0; n x  P    &#x2212;
&#x03C6;  n    )  .   {\displaystyle s_{N}(x)={\frac {A_{0}}        
{2}}+\sum _{n=1}^{N}A_{n}\cdot \cos \left({\tfrac {2\pi nx}{P}}-      (Eq.3)
\varphi _{n}\right).}  [{\displaystyle s_{N}(x)={\frac {A_{0}}
{2}}+\sum _{n=1}^{N}A_{n}\cdot \cos \left({\tfrac {2\pi nx}{P}}-
\varphi _{n}\right).}]
The customary form for generalizing to complex-valued     s ( x )
{\displaystyle s(x)}  [s(x)] (next section) is obtained using Euler's_formula
to split the cosine function into complex exponentials. Here, complex
conjugation is denoted by an asterisk:
             cos &#x2061;  (      2 &#x03C0; n x  P    &#x2212;  &#x03C6;  n
      )      &#x2261;    1 2     e  i  (      2 &#x03C0; n x  P    &#x2212;
      &#x03C6;  n    )        +    1 2     e  &#x2212; i  (      2 &#x03C0; n x
      P    &#x2212;  &#x03C6;  n    )         =  (     1 2     e  &#x2212; i
      &#x03C6;  n      )  &#x22C5;  e  i     2 &#x03C0; ( + n ) x  P          +
      (     1 2     e  &#x2212; i  &#x03C6;  n      )   &#x2217;   &#x22C5;  e
      i     2 &#x03C0; ( &#x2212; n ) x  P      .       {\displaystyle {\begin
      {array}{lll}\cos \left({\tfrac {2\pi nx}{P}}-\varphi _{n}\right)&{}\equiv
      {\tfrac {1}{2}}e^{i\left({\tfrac {2\pi nx}{P}}-\varphi _{n}\right)}&{}+
      {\tfrac {1}{2}}e^{-i\left({\tfrac {2\pi nx}{P}}-\varphi _
      {n}\right)}\\&=\left({\tfrac {1}{2}}e^{-i\varphi _{n}}\right)\cdot e^{i
      {\tfrac {2\pi (+n)x}{P}}}&{}+\left({\tfrac {1}{2}}e^{-i\varphi _
      {n}}\right)^{*}\cdot e^{i{\tfrac {2\pi (-n)x}{P}}}.\end{array}}}  [
      {\displaystyle {\begin{array}{lll}\cos \left({\tfrac {2\pi nx}{P}}-
      \varphi _{n}\right)&{}\equiv {\tfrac {1}{2}}e^{i\left({\tfrac {2\pi nx}
      {P}}-\varphi _{n}\right)}&{}+{\tfrac {1}{2}}e^{-i\left({\tfrac {2\pi nx}
      {P}}-\varphi _{n}\right)}\\&=\left({\tfrac {1}{2}}e^{-i\varphi _
      {n}}\right)\cdot e^{i{\tfrac {2\pi (+n)x}{P}}}&{}+\left({\tfrac {1}{2}}e^
      {-i\varphi _{n}}\right)^{*}\cdot e^{i{\tfrac {2\pi (-n)x}{P}}}.\end
      {array}}}]
Therefore, with definitions:
          c  n   &#x225C;  {      A  0    /  2   =  a  0    /  2 ,    n = 0
      A  n   2     e  &#x2212; i  &#x03C6;  n       =    1 2    (  a  n
      &#x2212; i  b  n   ) ,    n > 0      c   |  n  |    &#x2217;   ,     n <
      0     }   =    1 P    &#x222B;  P   s ( x ) &#x22C5;  e  &#x2212; i     2
      &#x03C0; n x  P      &#xA0; d x ,   {\displaystyle c_{n}\triangleq \left\
      {{\begin{array}{lll}A_{0}/2&=a_{0}/2,\quad &n=0\\{\tfrac {A_{n}}{2}}e^{-
      i\varphi _{n}}&={\tfrac {1}{2}}(a_{n}-ib_{n}),\quad &n>0\\c_{|n|}^
      {*},\quad &&n<0\end{array}}\right\}\quad =\quad {\frac {1}{P}}\int _{P}s
      (x)\cdot e^{-i{\tfrac {2\pi nx}{P}}}\ dx,}  [{\displaystyle c_
      {n}\triangleq \left\{{\begin{array}{lll}A_{0}/2&=a_{0}/2,\quad &n=0\\
      {\tfrac {A_{n}}{2}}e^{-i\varphi _{n}}&={\tfrac {1}{2}}(a_{n}-ib_
      {n}),\quad &n>0\\c_{|n|}^{*},\quad &&n<0\end{array}}\right\}\quad =\quad
      {\frac {1}{P}}\int _{P}s(x)\cdot e^{-i{\tfrac {2\pi nx}{P}}}\ dx,}]
the final result is:
Fourier series, exponential form
    s  N   ( x ) =  &#x2211;  n = &#x2212; N   N    c  n
&#x22C5;  e  i     2 &#x03C0; n x  P      .   {\displaystyle s_{N}    
(x)=\sum _{n=-N}^{N}c_{n}\cdot e^{i{\tfrac {2\pi nx}{P}}}.}  [          (Eq.4)
{\displaystyle s_{N}(x)=\sum _{n=-N}^{N}c_{n}\cdot e^{i{\tfrac
{2\pi nx}{P}}}.}]
**** Complex-valued functions[edit] ****
If     s ( x )   {\displaystyle s(x)}  [s(x)] is a complex-valued function of a
real variable     x ,   {\displaystyle x,}  [x,] both components (real and
imaginary part) are real-valued functions that can be represented by a Fourier
series. The two sets of coefficients and the partial sum are given by:
          c     R n     =   1 P    &#x222B;  P   Re &#x2061; { s ( x ) }
      &#x22C5;  e  &#x2212; i     2 &#x03C0; n x  P      &#xA0; d x
      {\displaystyle c_{_{Rn}}={\frac {1}{P}}\int _{P}\operatorname {Re} \{s
      (x)\}\cdot e^{-i{\tfrac {2\pi nx}{P}}}\ dx}  [{\displaystyle c_{_{Rn}}=
      {\frac {1}{P}}\int _{P}\operatorname {Re} \{s(x)\}\cdot e^{-i{\tfrac
      {2\pi nx}{P}}}\ dx}]     and          c     I n     =   1 P    &#x222B;
      P   Im &#x2061; { s ( x ) } &#x22C5;  e  &#x2212; i     2 &#x03C0; n x  P
      &#xA0; d x   {\displaystyle c_{_{In}}={\frac {1}{P}}\int _
      {P}\operatorname {Im} \{s(x)\}\cdot e^{-i{\tfrac {2\pi nx}{P}}}\ dx}  [
      {\displaystyle c_{_{In}}={\frac {1}{P}}\int _{P}\operatorname {Im} \{s
      (x)\}\cdot e^{-i{\tfrac {2\pi nx}{P}}}\ dx}]
          s  N   ( x ) =  &#x2211;  n = &#x2212; N   N    c     R n
      &#x22C5;  e  i     2 &#x03C0; n x  P      + i &#x22C5;  &#x2211;  n =
      &#x2212; N   N    c     I n     &#x22C5;  e  i     2 &#x03C0; n x  P
      =  &#x2211;  n = &#x2212; N   N    (   c     R n     + i &#x22C5;  c
      I n      )  &#x22C5;  e  i     2 &#x03C0; n x  P      .   {\displaystyle
      s_{N}(x)=\sum _{n=-N}^{N}c_{_{Rn}}\cdot e^{i{\tfrac {2\pi nx}{P}}}+i\cdot
      \sum _{n=-N}^{N}c_{_{In}}\cdot e^{i{\tfrac {2\pi nx}{P}}}=\sum _{n=-N}^
      {N}\left(c_{_{Rn}}+i\cdot c_{_{In}}\right)\cdot e^{i{\tfrac {2\pi nx}
      {P}}}.}  [{\displaystyle s_{N}(x)=\sum _{n=-N}^{N}c_{_{Rn}}\cdot e^{i
      {\tfrac {2\pi nx}{P}}}+i\cdot \sum _{n=-N}^{N}c_{_{In}}\cdot e^{i{\tfrac
      {2\pi nx}{P}}}=\sum _{n=-N}^{N}\left(c_{_{Rn}}+i\cdot c_{_
      {In}}\right)\cdot e^{i{\tfrac {2\pi nx}{P}}}.}]
Defining      c  n   &#x225C;  c     R n     + i &#x22C5;  c     I n
{\displaystyle c_{n}\triangleq c_{_{Rn}}+i\cdot c_{_{In}}}  [{\displaystyle c_
{n}\triangleq c_{_{Rn}}+i\cdot c_{_{In}}}] yields:
    s  N   ( x ) =  &#x2211;  n = &#x2212; N   N    c  n
&#x22C5;  e  i     2 &#x03C0; n x  P      .   {\displaystyle s_{N}    
(x)=\sum _{n=-N}^{N}c_{n}\cdot e^{i{\tfrac {2\pi nx}{P}}}.}  [          (Eq.5)
{\displaystyle s_{N}(x)=\sum _{n=-N}^{N}c_{n}\cdot e^{i{\tfrac
{2\pi nx}{P}}}.}]
This is identical to Eq.4 except      c  n     {\displaystyle c_{n}}  [c_{n}]
and      c  &#x2212; n     {\displaystyle c_{-n}}  [{\displaystyle c_{-n}}] are
no longer complex conjugates. The formula for      c  n     {\displaystyle c_
{n}}  [c_{n}] is also unchanged:
              c  n      =   1 P    &#x222B;  P   Re &#x2061; { s ( x ) }
      &#x22C5;  e  &#x2212; i     2 &#x03C0; n x  P      &#xA0; d x + i
      &#x22C5;   1 P    &#x222B;  P   Im &#x2061; { s ( x ) } &#x22C5;  e
      &#x2212; i     2 &#x03C0; n x  P      &#xA0; d x       =   1 P
      &#x222B;  P    (  Re &#x2061; { s ( x ) } + i &#x22C5; Im &#x2061; { s
      ( x ) }  )  &#x22C5;  e  &#x2212; i     2 &#x03C0; n x  P      &#xA0; d x
      &#xA0; = &#xA0;   1 P    &#x222B;  P   s ( x ) &#x22C5;  e  &#x2212; i
      2 &#x03C0; n x  P      &#xA0; d x .       {\displaystyle {\begin
      {aligned}c_{n}&={\frac {1}{P}}\int _{P}\operatorname {Re} \{s(x)\}\cdot
      e^{-i{\tfrac {2\pi nx}{P}}}\ dx+i\cdot {\frac {1}{P}}\int _
      {P}\operatorname {Im} \{s(x)\}\cdot e^{-i{\tfrac {2\pi nx}{P}}}\ dx\\
      [4pt]&={\frac {1}{P}}\int _{P}\left(\operatorname {Re} \{s(x)\}+i\cdot
      \operatorname {Im} \{s(x)\}\right)\cdot e^{-i{\tfrac {2\pi nx}{P}}}\ dx\
      =\ {\frac {1}{P}}\int _{P}s(x)\cdot e^{-i{\tfrac {2\pi nx}{P}}}\ dx.\end
      {aligned}}}  [{\displaystyle {\begin{aligned}c_{n}&={\frac {1}{P}}\int _
      {P}\operatorname {Re} \{s(x)\}\cdot e^{-i{\tfrac {2\pi nx}{P}}}\
      dx+i\cdot {\frac {1}{P}}\int _{P}\operatorname {Im} \{s(x)\}\cdot e^{-i
      {\tfrac {2\pi nx}{P}}}\ dx\\[4pt]&={\frac {1}{P}}\int _{P}\left
      (\operatorname {Re} \{s(x)\}+i\cdot \operatorname {Im} \{s
      (x)\}\right)\cdot e^{-i{\tfrac {2\pi nx}{P}}}\ dx\ =\ {\frac {1}{P}}\int
      _{P}s(x)\cdot e^{-i{\tfrac {2\pi nx}{P}}}\ dx.\end{aligned}}}]
**** Other common notations[edit] ****
The notation      c  n     {\displaystyle c_{n}}  [c_{n}] is inadequate for
discussing the Fourier coefficients of several different functions. Therefore,
it is customarily replaced by a modified form of the function (    s
{\displaystyle s}  [s], in this case), such as        s &#x005E;    ( n )
{\displaystyle {\hat {s}}(n)}  [{\displaystyle {\hat {s}}(n)}] or     S [ n ]
{\displaystyle S[n]}  [{\displaystyle S[n]}], and functional notation often
replaces subscripting:
              s  &#x221E;   ( x )    =  &#x2211;  n = &#x2212; &#x221E;
      &#x221E;      s &#x005E;    ( n ) &#x22C5;  e  i  2 &#x03C0; n x  /  P
      =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;   S [ n ] &#x22C5;  e  j  2
      &#x03C0; n x  /  P         c o m m o n &#xA0; e n g i n e e r i n g
      &#xA0; n o t a t i o n          {\displaystyle {\begin{aligned}s_{\infty
      }(x)&=\sum _{n=-\infty }^{\infty }{\hat {s}}(n)\cdot e^{i\,2\pi nx/P}\\
      [6pt]&=\sum _{n=-\infty }^{\infty }S[n]\cdot e^{j\,2\pi nx/
      P}&&\scriptstyle {\mathsf {common\ engineering\ notation}}\end{aligned}}}
      [{\displaystyle {\begin{aligned}s_{\infty }(x)&=\sum _{n=-\infty }^
      {\infty }{\hat {s}}(n)\cdot e^{i\,2\pi nx/P}\\[6pt]&=\sum _{n=-\infty }^
      {\infty }S[n]\cdot e^{j\,2\pi nx/P}&&\scriptstyle {\mathsf {common\
      engineering\ notation}}\end{aligned}}}]
In engineering, particularly when the variable     x   {\displaystyle x}  [x]
represents time, the coefficient sequence is called a frequency_domain
representation. Square brackets are often used to emphasize that the domain of
this function is a discrete set of frequencies.
Another commonly used frequency domain representation uses the Fourier series
coefficients to modulate a Dirac_comb:
         S ( f ) &#xA0; &#x225C; &#xA0;  &#x2211;  n = &#x2212; &#x221E;
      &#x221E;   S [ n ] &#x22C5; &#x03B4;  (  f &#x2212;   n P    )  ,
      {\displaystyle S(f)\ \triangleq \ \sum _{n=-\infty }^{\infty }S[n]\cdot
      \delta \left(f-{\frac {n}{P}}\right),}  [{\displaystyle S(f)\ \triangleq
      \ \sum _{n=-\infty }^{\infty }S[n]\cdot \delta \left(f-{\frac {n}
      {P}}\right),}]
where     f   {\displaystyle f}  [f] represents a continuous frequency domain.
When variable     x   {\displaystyle x}  [x] has units of seconds,     f
{\displaystyle f}  [f] has units of hertz. The "teeth" of the comb are spaced
at multiples (i.e. harmonics) of     1  /  P   {\displaystyle 1/P}  [1/P],
which is called the fundamental_frequency.       s  &#x221E;   ( x )
{\displaystyle s_{\infty }(x)}  [{\displaystyle s_{\infty }(x)}]  can be
recovered from this representation by an inverse_Fourier_transform:
                F    &#x2212; 1   { S ( f ) }    =  &#x222B;  &#x2212; &#x221E;
      &#x221E;    (   &#x2211;  n = &#x2212; &#x221E;   &#x221E;   S [ n ]
      &#x22C5; &#x03B4;  (  f &#x2212;   n P    )   )   e  i 2 &#x03C0; f x
      d f ,       =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;   S [ n ]
      &#x22C5;  &#x222B;  &#x2212; &#x221E;   &#x221E;   &#x03B4;  (  f
      &#x2212;   n P    )   e  i 2 &#x03C0; f x    d f ,       =  &#x2211;  n =
      &#x2212; &#x221E;   &#x221E;   S [ n ] &#x22C5;  e  i  2 &#x03C0; n x  /
      P   &#xA0; &#xA0; &#x225C; &#xA0;  s  &#x221E;   ( x ) .
      {\displaystyle {\begin{aligned}{\mathcal {F}}^{-1}\{S(f)\}&=\int _{-
      \infty }^{\infty }\left(\sum _{n=-\infty }^{\infty }S[n]\cdot \delta
      \left(f-{\frac {n}{P}}\right)\right)e^{i2\pi fx}\,df,\\[6pt]&=\sum _{n=-
      \infty }^{\infty }S[n]\cdot \int _{-\infty }^{\infty }\delta \left(f-
      {\frac {n}{P}}\right)e^{i2\pi fx}\,df,\\[6pt]&=\sum _{n=-\infty }^{\infty
      }S[n]\cdot e^{i\,2\pi nx/P}\ \ \triangleq \ s_{\infty }(x).\end
      {aligned}}}  [{\displaystyle {\begin{aligned}{\mathcal {F}}^{-1}\{S
      (f)\}&=\int _{-\infty }^{\infty }\left(\sum _{n=-\infty }^{\infty }S
      [n]\cdot \delta \left(f-{\frac {n}{P}}\right)\right)e^{i2\pi fx}\,df,\\
      [6pt]&=\sum _{n=-\infty }^{\infty }S[n]\cdot \int _{-\infty }^{\infty
      }\delta \left(f-{\frac {n}{P}}\right)e^{i2\pi fx}\,df,\\[6pt]&=\sum _{n=-
      \infty }^{\infty }S[n]\cdot e^{i\,2\pi nx/P}\ \ \triangleq \ s_{\infty }
      (x).\end{aligned}}}]
The constructed function     S ( f )   {\displaystyle S(f)}  [S(f)] is
therefore commonly referred to as a Fourier transform, even though the Fourier
integral of a periodic function is not convergent at the harmonic frequencies.
[nb_2]
    * The first four partial sums of the Fourier series for a square_wave
    * [SquareWaveFourierArrows,rotated.gif]
***** Convergence[edit] *****
Main article: Convergence_of_Fourier_series
In engineering applications, the Fourier series is generally presumed to
converge everywhere except at discontinuities, since the functions encountered
in engineering are more well behaved than the ones that mathematicians can
provide as counter-examples to this presumption. In particular, if     s
{\displaystyle s}  [s] is continuous and the derivative of     s ( x )
{\displaystyle s(x)}  [s(x)] (which may not exist everywhere) is square
integrable, then the Fourier series of     s   {\displaystyle s}  [s] converges
absolutely and uniformly to     s ( x )   {\displaystyle s(x)}  [s(x)].[11]  If
a function is square-integrable on the interval     [  x  0   ,  x  0   + P ]
{\displaystyle [x_{0},x_{0}+P]}  [{\displaystyle [x_{0},x_{0}+P]}], then the
Fourier series converges_to_the_function_at_almost_every_point. Convergence of
Fourier series also depends on the finite number of maxima and minima in a
function which is popularly known as one of the Dirichlet's_condition_for
Fourier_series. See Convergence_of_Fourier_series. It is possible to define
Fourier coefficients for more general functions or distributions, in such cases
convergence in norm or weak_convergence is usually of interest.
    * Another visualisation of an approximation of a square wave by taking the
      first 1, 2, 3 and 4 terms of its Fourier series. (An interactive
      animation can be seen here)
    * A visualisation of an approximation of a sawtooth wave of the same
      amplitude and frequency for comparison
    * Example of convergence to a somewhat arbitrary function. Note the
      development of the "ringing" (Gibbs phenomenon) at the transitions to/
      from the vertical sections.
***** Examples[edit] *****
**** Example 1: a simple Fourier series[edit] ****
Plot of the sawtooth_wave, a periodic continuation of the linear function     s
( x ) = x  /  &#x03C0;   {\displaystyle s(x)=x/\pi }  [s(x)=x/\pi ] on the
interval     ( &#x2212; &#x03C0; , &#x03C0; ]   {\displaystyle (-\pi ,\pi ]}  [
(-\pi ,\pi ]]
Animated plot of the first five successive partial Fourier series
We now use the formula above to give a Fourier series expansion of a very
simple function. Consider a sawtooth wave
         s ( x ) =   x &#x03C0;   ,   f o r  &#x2212; &#x03C0; < x < &#x03C0; ,
      {\displaystyle s(x)={\frac {x}{\pi }},\quad \mathrm {for} -\pi <x<\pi ,}
      [s(x) = \frac{x}{\pi}, \quad \mathrm{for } -\pi < x < \pi,]
         s ( x + 2 &#x03C0; k ) = s ( x ) ,   f o r  &#x2212; &#x03C0; < x <
      &#x03C0;  &#xA0;and&#xA0;  k &#x2208;  Z  .   {\displaystyle s(x+2\pi
      k)=s(x),\quad \mathrm {for} -\pi <x<\pi {\text{ and }}k\in \mathbb {Z} .}
      [{\displaystyle s(x+2\pi k)=s(x),\quad \mathrm {for} -\pi <x<\pi {\text
      { and }}k\in \mathbb {Z} .}]
In this case, the Fourier coefficients are given by
              a  n      =   1 &#x03C0;    &#x222B;  &#x2212; &#x03C0;
      &#x03C0;   s ( x ) cos &#x2061; ( n x )  d x = 0 ,  n &#x2265; 0.      b
      n      =   1 &#x03C0;    &#x222B;  &#x2212; &#x03C0;   &#x03C0;   s ( x )
      sin &#x2061; ( n x )  d x       = &#x2212;   2  &#x03C0; n    cos
      &#x2061; ( n &#x03C0; ) +   2   &#x03C0;  2    n  2      sin &#x2061; ( n
      &#x03C0; )       =    2  ( &#x2212; 1  )  n + 1     &#x03C0; n    ,  n
      &#x2265; 1.       {\displaystyle {\begin{aligned}a_{n}&={\frac {1}{\pi
      }}\int _{-\pi }^{\pi }s(x)\cos(nx)\,dx=0,\quad n\geq 0.\\[4pt]b_{n}&=
      {\frac {1}{\pi }}\int _{-\pi }^{\pi }s(x)\sin(nx)\,dx\\[4pt]&=-{\frac {2}
      {\pi n}}\cos(n\pi )+{\frac {2}{\pi ^{2}n^{2}}}\sin(n\pi )\\[4pt]&={\frac
      {2\,(-1)^{n+1}}{\pi n}},\quad n\geq 1.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}a_{n}&={\frac {1}{\pi }}\int _{-\pi }^{\pi }s(x)\cos
      (nx)\,dx=0,\quad n\geq 0.\\[4pt]b_{n}&={\frac {1}{\pi }}\int _{-\pi }^
      {\pi }s(x)\sin(nx)\,dx\\[4pt]&=-{\frac {2}{\pi n}}\cos(n\pi )+{\frac {2}
      {\pi ^{2}n^{2}}}\sin(n\pi )\\[4pt]&={\frac {2\,(-1)^{n+1}}{\pi n}},\quad
      n\geq 1.\end{aligned}}}]
It can be proven that Fourier series converges to     s ( x )   {\displaystyle
s(x)}  [s(x)] at every point     x   {\displaystyle x}  [x] where     s
{\displaystyle s}  [s] is differentiable, and therefore:
             s ( x )    =    a  0   2   +  &#x2211;  n = 1
      &#x221E;    [   a  n   cos &#x2061;  (  n x  )  +  b  n
      sin &#x2061;  (  n x  )   ]        =   2 &#x03C0;
      &#x2211;  n = 1   &#x221E;      ( &#x2212; 1  )  n + 1    n
      sin &#x2061; ( n x ) ,   f o r   x &#x2212; &#x03C0;
      &#x2209; 2 &#x03C0;  Z  .       {\displaystyle {\begin
      {aligned}s(x)&={\frac {a_{0}}{2}}+\sum _{n=1}^{\infty }\left
      [a_{n}\cos \left(nx\right)+b_{n}\sin \left                      (Eq.7)
      (nx\right)\right]\\[4pt]&={\frac {2}{\pi }}\sum _{n=1}^         
      {\infty }{\frac {(-1)^{n+1}}{n}}\sin(nx),\quad \mathrm {for}
      \quad x-\pi \notin 2\pi \mathbb {Z} .\end{aligned}}}  [
      {\displaystyle {\begin{aligned}s(x)&={\frac {a_{0}}{2}}+\sum
      _{n=1}^{\infty }\left[a_{n}\cos \left(nx\right)+b_{n}\sin
      \left(nx\right)\right]\\[4pt]&={\frac {2}{\pi }}\sum _{n=1}^
      {\infty }{\frac {(-1)^{n+1}}{n}}\sin(nx),\quad \mathrm {for}
      \quad x-\pi \notin 2\pi \mathbb {Z} .\end{aligned}}}]
When     x = &#x03C0;   {\displaystyle x=\pi }  [x=\pi], the Fourier series
converges to 0, which is the half-sum of the left- and right-limit of s at
x = &#x03C0;   {\displaystyle x=\pi }  [x=\pi]. This is a particular instance
of the Dirichlet_theorem for Fourier series.
Heat distribution in a metal plate, using Fourier's method
This example leads us to a solution to the Basel_problem.
**** Example 2: Fourier's motivation[edit] ****
The Fourier series expansion of our function in Example 1 looks more
complicated than the simple formula     s ( x ) = x  /  &#x03C0;
{\displaystyle s(x)=x/\pi }  [{\displaystyle s(x)=x/\pi }], so it is not
immediately apparent why one would need the Fourier series. While there are
many applications, Fourier's motivation was in solving the heat_equation. For
example, consider a metal plate in the shape of a square whose side measures
&#x03C0;   {\displaystyle \pi }  [\pi ] meters, with coordinates     ( x , y )
&#x2208; [ 0 , &#x03C0; ] &#x00D7; [ 0 , &#x03C0; ]   {\displaystyle (x,y)\in
[0,\pi ]\times [0,\pi ]}  [{\displaystyle (x,y)\in [0,\pi ]\times [0,\pi ]}].
If there is no heat source within the plate, and if three of the four sides are
held at 0 degrees Celsius, while the fourth side, given by     y = &#x03C0;
{\displaystyle y=\pi }  [{\displaystyle y=\pi }], is maintained at the
temperature gradient     T ( x , &#x03C0; ) = x   {\displaystyle T(x,\pi )=x}
[{\displaystyle T(x,\pi )=x}] degrees Celsius, for     x   {\displaystyle x}
[x] in     ( 0 , &#x03C0; )   {\displaystyle (0,\pi )}  [{\displaystyle (0,\pi
)}], then one can show that the stationary heat distribution (or the heat
distribution after a long period of time has elapsed) is given by
         T ( x , y ) = 2  &#x2211;  n = 1   &#x221E;      ( &#x2212; 1  )  n +
      1    n   sin &#x2061; ( n x )    sinh &#x2061; ( n y )   sinh &#x2061;
      ( n &#x03C0; )    .   {\displaystyle T(x,y)=2\sum _{n=1}^{\infty }{\frac
      {(-1)^{n+1}}{n}}\sin(nx){\sinh(ny) \over \sinh(n\pi )}.}  [T(x,y) =
      2\sum_{n=1}^\infty \frac{(-1)^{n+1}}{n} \sin(nx) {\sinh(ny) \over \sinh
      (n\pi)}.]
Here, sinh is the hyperbolic_sine function. This solution of the heat equation
is obtained by multiplying each term of  Eq.7 by     sinh &#x2061; ( n y )  /
sinh &#x2061; ( n &#x03C0; )   {\displaystyle \sinh(ny)/\sinh(n\pi )}  [
{\displaystyle \sinh(ny)/\sinh(n\pi )}]. While our example function     s ( x )
{\displaystyle s(x)}  [s(x)] seems to have a needlessly complicated Fourier
series, the heat distribution     T ( x , y )   {\displaystyle T(x,y)}  [
{\displaystyle T(x,y)}] is nontrivial. The function     T   {\displaystyle T}
[T] cannot be written as a closed-form_expression. This method of solving the
heat problem was made possible by Fourier's work.
**** Other applications[edit] ****
Another application of this Fourier series is to solve the Basel_problem by
using Parseval's_theorem. The example generalizes and one may compute Î¶(2n),
for any positive integer n.
***** Beginnings[edit] *****
       &#x03C6; ( y ) =  a  0   cos &#x2061;    &#x03C0; y  2   +  a  1
    cos &#x2061; 3    &#x03C0; y  2   +  a  2   cos &#x2061; 5    &#x03C0;
    y  2   + &#x22EF; .   {\displaystyle \varphi (y)=a_{0}\cos {\frac {\pi
    y}{2}}+a_{1}\cos 3{\frac {\pi y}{2}}+a_{2}\cos 5{\frac {\pi y}
    {2}}+\cdots .}  [\varphi(y)=a_0\cos\frac{\pi y}{2}+a_1\cos 3\frac{\pi
    y}{2}+a_2\cos5\frac{\pi y}{2}+\cdots.]
âMultiplying both sides by     cos &#x2061; ( 2 k + 1 )    &#x03C0; y  2 â
    {\displaystyle \cos(2k+1){\frac {\pi y}{2}}}  [\cos(2k+1)\frac{\pi y}
    {2}], and then integrating from     y = &#x2212; 1   {\displaystyle y=-
    1}  [y=-1] to     y = + 1   {\displaystyle y=+1}  [y=+1] yields:
              a  k   =  &#x222B;  &#x2212; 1   1   &#x03C6; ( y ) cos
          &#x2061; ( 2 k + 1 )    &#x03C0; y  2    d y .   {\displaystyle
          a_{k}=\int _{-1}^{1}\varphi (y)\cos(2k+1){\frac {\pi y}{2}}\,dy.}
          [a_k=\int_{-1}^1\varphi(y)\cos(2k+1)\frac{\pi y}{2}\,dy.]
â Joseph Fourier, MÃ©moire_sur_la_propagation_de_la_chaleur_dans_les_corps
solides. (1807)[12][nb_3]
This immediately gives any coefficient ak of the trigonometrical_series for Ï
(y) for any function which has such an expansion. It works because if Ï has
such an expansion, then (under suitable convergence assumptions) the integral
              a  k      =  &#x222B;  &#x2212; 1   1   &#x03C6; ( y ) cos
      &#x2061; ( 2 k + 1 )    &#x03C0; y  2    d y       =  &#x222B;  &#x2212;
      1   1    (  a cos &#x2061;    &#x03C0; y  2   cos &#x2061; ( 2 k + 1 )
      &#x03C0; y  2   +  a &#x2032;  cos &#x2061; 3    &#x03C0; y  2   cos
      &#x2061; ( 2 k + 1 )    &#x03C0; y  2   + &#x22EF;  )   d y
      {\displaystyle {\begin{aligned}a_{k}&=\int _{-1}^{1}\varphi (y)\cos(2k+1)
      {\frac {\pi y}{2}}\,dy\\&=\int _{-1}^{1}\left(a\cos {\frac {\pi y}
      {2}}\cos(2k+1){\frac {\pi y}{2}}+a'\cos 3{\frac {\pi y}{2}}\cos(2k+1)
      {\frac {\pi y}{2}}+\cdots \right)\,dy\end{aligned}}}  [\begin{align}
      a_k&=\int_{-1}^1\varphi(y)\cos(2k+1)\frac{\pi y}{2}\,dy \\
      &= \int_{-1}^1\left(a\cos\frac{\pi y}{2}\cos(2k+1)\frac{\pi y}{2}+a'\cos
      3\frac{\pi y}{2}\cos(2k+1)\frac{\pi y}{2}+\cdots\right)\,dy
      \end{align}]
can be carried out term-by-term. But all terms involving     cos &#x2061; ( 2 j
+ 1 )    &#x03C0; y  2   cos &#x2061; ( 2 k + 1 )    &#x03C0; y  2
{\displaystyle \cos(2j+1){\frac {\pi y}{2}}\cos(2k+1){\frac {\pi y}{2}}}  [\cos
(2j+1)\frac{\pi y}{2} \cos(2k+1)\frac{\pi y}{2}] for j ≠ k vanish when
integrated from â1 to 1, leaving only the kth term.
In these few lines, which are close to the modern formalism used in Fourier
series, Fourier revolutionized both mathematics and physics. Although similar
trigonometric series were previously used by Euler, d'Alembert, Daniel
Bernoulli and Gauss, Fourier believed that such trigonometric series could
represent any arbitrary function. In what sense that is actually true is a
somewhat subtle issue and the attempts over many years to clarify this idea
have led to important discoveries in the theories of convergence, function
spaces, and harmonic_analysis.
When Fourier submitted a later competition essay in 1811, the committee (which
included Lagrange, Laplace, Malus and Legendre, among others) concluded: ...the
manner in which the author arrives at these equations is not exempt of
difficulties and...his analysis to integrate them still leaves something to be
desired on the score of generality and even rigour.[citation_needed]
**** Birth of harmonic analysis[edit] ****
Since Fourier's time, many different approaches to defining and understanding
the concept of Fourier series have been discovered, all of which are consistent
with one another, but each of which emphasizes different aspects of the topic.
Some of the more powerful and elegant approaches are based on mathematical
ideas and tools that were not available at the time Fourier completed his
original work. Fourier originally defined the Fourier series for real-valued
functions of real arguments, and using the sine and cosine functions as the
basis_set for the decomposition.
Many other Fourier-related_transforms have since been defined, extending the
initial idea to other applications. This general area of inquiry is now
sometimes called harmonic_analysis. A Fourier series, however, can be used only
for periodic functions, or for functions on a bounded (compact) interval.
***** Extensions[edit] *****
**** Fourier series on a square[edit] ****
We can also define the Fourier series for functions of two variables     x
{\displaystyle x}  [x] and     y   {\displaystyle y}  [y] in the square
[ &#x2212; &#x03C0; , &#x03C0; ] &#x00D7; [ &#x2212; &#x03C0; , &#x03C0; ]
{\displaystyle [-\pi ,\pi ]\times [-\pi ,\pi ]}  [{\displaystyle [-\pi ,\pi
]\times [-\pi ,\pi ]}]:
             f ( x , y )    =  &#x2211;  j , k  &#x2208;   Z   &#xA0;(integers)
      c  j , k    e  i j x    e  i k y   ,      c  j , k      =   1  4
      &#x03C0;  2       &#x222B;  &#x2212; &#x03C0;   &#x03C0;    &#x222B;
      &#x2212; &#x03C0;   &#x03C0;   f ( x , y )  e  &#x2212; i j x    e
      &#x2212; i k y    d x  d y .       {\displaystyle {\begin{aligned}f
      (x,y)&=\sum _{j,k\,\in \,\mathbb {Z} {\text{ (integers)}}}c_{j,k}e^
      {ijx}e^{iky},\\[5pt]c_{j,k}&={1 \over 4\pi ^{2}}\int _{-\pi }^{\pi }\int
      _{-\pi }^{\pi }f(x,y)e^{-ijx}e^{-iky}\,dx\,dy.\end{aligned}}}  [
      {\displaystyle {\begin{aligned}f(x,y)&=\sum _{j,k\,\in \,\mathbb {Z}
      {\text{ (integers)}}}c_{j,k}e^{ijx}e^{iky},\\[5pt]c_{j,k}&={1 \over 4\pi
      ^{2}}\int _{-\pi }^{\pi }\int _{-\pi }^{\pi }f(x,y)e^{-ijx}e^{-
      iky}\,dx\,dy.\end{aligned}}}]
Aside from being useful for solving partial differential equations such as the
heat equation, one notable application of Fourier series on the square is in
image_compression. In particular, the jpeg image compression standard uses the
two-dimensional discrete_cosine_transform, which is a Fourier transform using
the cosine basis functions.
**** Fourier series of Bravais-lattice-periodic-function[edit] ****
The three-dimensional Bravais_lattice is defined as the set of vectors of the
form:
          R  =  n  1     a   1   +  n  2     a   2   +  n  3     a   3
      {\displaystyle \mathbf {R} =n_{1}\mathbf {a} _{1}+n_{2}\mathbf {a} _
      {2}+n_{3}\mathbf {a} _{3}}  [{\displaystyle \mathbf {R} =n_{1}\mathbf {a}
      _{1}+n_{2}\mathbf {a} _{2}+n_{3}\mathbf {a} _{3}}]
where      n  i     {\displaystyle n_{i}}  [n_{i}] are integers and       a   i
{\displaystyle \mathbf {a} _{i}}  [\mathbf{a}_i] are three linearly independent
vectors. Assuming we have some function,     f (  r  )   {\displaystyle f
(\mathbf {r} )}  [f(\mathbf{r})], such that it obeys the following condition
for any Bravais lattice vector      R  : f (  r  ) = f (  R  +  r  )
{\displaystyle \mathbf {R} :f(\mathbf {r} )=f(\mathbf {R} +\mathbf {r} )}  [
{\displaystyle \mathbf {R} :f(\mathbf {r} )=f(\mathbf {R} +\mathbf {r} )}], we
could make a Fourier series of it. This kind of function can be, for example,
the effective potential that one electron "feels" inside a periodic crystal. It
is useful to make a Fourier series of the potential then when applying Bloch's
theorem. First, we may write any arbitrary vector      r    {\displaystyle
\mathbf {r} }  [\mathbf {r} ] in the coordinate-system of the lattice:
          r  =  x  1       a   1    a  1     +  x  2       a   2    a  2     +
      x  3       a   3    a  3     ,   {\displaystyle \mathbf {r} =x_{1}{\frac
      {\mathbf {a} _{1}}{a_{1}}}+x_{2}{\frac {\mathbf {a} _{2}}{a_{2}}}+x_{3}
      {\frac {\mathbf {a} _{3}}{a_{3}}},}  [\mathbf{r} = x_1\frac{\mathbf{a}_
      {1}}{a_1}+ x_2\frac{\mathbf{a}_{2}}{a_2}+ x_3\frac{\mathbf{a}_{3}}{a_3},]
where      a  i   :=  |    a   i    |  .   {\displaystyle a_{i}:=|\mathbf {a} _
{i}|.}  [{\displaystyle a_{i}:=|\mathbf {a} _{i}|.}]
Thus we can define a new function,
         g (  x  1   ,  x  2   ,  x  3   ) := f (  r  ) = f  (   x  1       a
      1    a  1     +  x  2       a   2    a  2     +  x  3       a   3    a  3
      )  .   {\displaystyle g(x_{1},x_{2},x_{3}):=f(\mathbf {r} )=f\left(x_{1}
      {\frac {\mathbf {a} _{1}}{a_{1}}}+x_{2}{\frac {\mathbf {a} _{2}}{a_
      {2}}}+x_{3}{\frac {\mathbf {a} _{3}}{a_{3}}}\right).}  [g(x_1,x_2,x_3) :
      = f(\mathbf{r}) = f \left (x_1\frac{\mathbf{a}_{1}}{a_1}+x_2\frac{\mathbf
      {a}_{2}}{a_2}+x_3\frac{\mathbf{a}_{3}}{a_3} \right ).]
This new function,     g (  x  1   ,  x  2   ,  x  3   )   {\displaystyle g(x_
{1},x_{2},x_{3})}  [g(x_1,x_2,x_3)], is now a function of three-variables, each
of which has periodicity a1, a2, a3 respectively:
         g (  x  1   ,  x  2   ,  x  3   ) = g (  x  1   +  a  1   ,  x  2   ,
      x  3   ) = g (  x  1   ,  x  2   +  a  2   ,  x  3   ) = g (  x  1   ,  x
      2   ,  x  3   +  a  3   ) .   {\displaystyle g(x_{1},x_{2},x_{3})=g(x_
      {1}+a_{1},x_{2},x_{3})=g(x_{1},x_{2}+a_{2},x_{3})=g(x_{1},x_{2},x_{3}+a_
      {3}).}  [{\displaystyle g(x_{1},x_{2},x_{3})=g(x_{1}+a_{1},x_{2},x_{3})=g
      (x_{1},x_{2}+a_{2},x_{3})=g(x_{1},x_{2},x_{3}+a_{3}).}]
If we write a series for g on the interval [0, a1] for x1, we can define the
following:
          h   o n e    (  m  1   ,  x  2   ,  x  3   ) :=   1  a  1
      &#x222B;  0    a  1     g (  x  1   ,  x  2   ,  x  3   ) &#x22C5;  e
      &#x2212; i 2 &#x03C0;    m  1    a  1      x  1      d  x  1
      {\displaystyle h^{\mathrm {one} }(m_{1},x_{2},x_{3}):={\frac {1}{a_
      {1}}}\int _{0}^{a_{1}}g(x_{1},x_{2},x_{3})\cdot e^{-i2\pi {\frac {m_{1}}
      {a_{1}}}x_{1}}\,dx_{1}}  [h^\mathrm{one}(m_1, x_2, x_3) := \frac{1}
      {a_1}\int_0^{a_1} g(x_1, x_2, x_3)\cdot e^{-i 2\pi \frac{m_1}{a_1} x_1}\,
      dx_1]
And then we can write:
         g (  x  1   ,  x  2   ,  x  3   ) =  &#x2211;   m  1   = &#x2212;
      &#x221E;   &#x221E;    h   o n e    (  m  1   ,  x  2   ,  x  3   )
      &#x22C5;  e  i 2 &#x03C0;    m  1    a  1      x  1       {\displaystyle
      g(x_{1},x_{2},x_{3})=\sum _{m_{1}=-\infty }^{\infty }h^{\mathrm {one} }
      (m_{1},x_{2},x_{3})\cdot e^{i2\pi {\frac {m_{1}}{a_{1}}}x_{1}}}  [g(x_1,
      x_2, x_3)=\sum_{m_1=-\infty}^\infty h^\mathrm{one}(m_1, x_2, x_3) \cdot
      e^{i 2\pi \frac{m_1}{a_1} x_1}]
Further defining:
              h   t w o    (  m  1   ,  m  2   ,  x  3   )    :=   1  a  2
      &#x222B;  0    a  2      h   o n e    (  m  1   ,  x  2   ,  x  3   )
      &#x22C5;  e  &#x2212; i 2 &#x03C0;    m  2    a  2      x  2      d  x  2
      =   1  a  2      &#x222B;  0    a  2     d  x  2     1  a  1
      &#x222B;  0    a  1     d  x  1   g (  x  1   ,  x  2   ,  x  3   )
      &#x22C5;  e  &#x2212; i 2 &#x03C0;  (     m  1    a  1      x  1   +    m
      2    a  2      x  2    )          {\displaystyle {\begin{aligned}h^
      {\mathrm {two} }(m_{1},m_{2},x_{3})&:={\frac {1}{a_{2}}}\int _{0}^{a_
      {2}}h^{\mathrm {one} }(m_{1},x_{2},x_{3})\cdot e^{-i2\pi {\frac {m_{2}}
      {a_{2}}}x_{2}}\,dx_{2}\\[12pt]&={\frac {1}{a_{2}}}\int _{0}^{a_{2}}dx_{2}
      {\frac {1}{a_{1}}}\int _{0}^{a_{1}}dx_{1}g(x_{1},x_{2},x_{3})\cdot e^{-
      i2\pi \left({\frac {m_{1}}{a_{1}}}x_{1}+{\frac {m_{2}}{a_{2}}}x_
      {2}\right)}\end{aligned}}}  [
      \begin{align}
      h^\mathrm{two}(m_1, m_2, x_3) & := \frac{1}{a_2}\int_0^{a_2} h^\mathrm
      {one}(m_1, x_2, x_3)\cdot e^{-i 2\pi \frac{m_2}{a_2} x_2}\, dx_2 \\[12pt]
      & = \frac{1}{a_2}\int_0^{a_2} dx_2 \frac{1}{a_1}\int_0^{a_1} dx_1 g(x_1,
      x_2, x_3)\cdot e^{-i 2\pi \left(\frac{m_1}{a_1} x_1+\frac{m_2}{a_2}
      x_2\right)}
      \end{align}
      ]
We can write     g   {\displaystyle g}  [g] once again as:
         g (  x  1   ,  x  2   ,  x  3   ) =  &#x2211;   m  1   = &#x2212;
      &#x221E;   &#x221E;    &#x2211;   m  2   = &#x2212; &#x221E;   &#x221E;
      h   t w o    (  m  1   ,  m  2   ,  x  3   ) &#x22C5;  e  i 2 &#x03C0;
      m  1    a  1      x  1     &#x22C5;  e  i 2 &#x03C0;    m  2    a  2
      x  2       {\displaystyle g(x_{1},x_{2},x_{3})=\sum _{m_{1}=-\infty }^
      {\infty }\sum _{m_{2}=-\infty }^{\infty }h^{\mathrm {two} }(m_{1},m_
      {2},x_{3})\cdot e^{i2\pi {\frac {m_{1}}{a_{1}}}x_{1}}\cdot e^{i2\pi
      {\frac {m_{2}}{a_{2}}}x_{2}}}  [g(x_1, x_2, x_3)=\sum_{m_1=-
      \infty}^\infty \sum_{m_2=-\infty}^\infty h^\mathrm{two}(m_1, m_2, x_3)
      \cdot e^{i 2\pi \frac{m_1}{a_1} x_1} \cdot e^{i 2\pi \frac{m_2}
      {a_2} x_2}]
Finally applying the same for the third coordinate, we define:
              h   t h r e e    (  m  1   ,  m  2   ,  m  3   )    :=   1  a  3
      &#x222B;  0    a  3      h   t w o    (  m  1   ,  m  2   ,  x  3   )
      &#x22C5;  e  &#x2212; i 2 &#x03C0;    m  3    a  3      x  3      d  x  3
      =   1  a  3      &#x222B;  0    a  3     d  x  3     1  a  2
      &#x222B;  0    a  2     d  x  2     1  a  1      &#x222B;  0    a  1
      d  x  1   g (  x  1   ,  x  2   ,  x  3   ) &#x22C5;  e  &#x2212; i 2
      &#x03C0;  (     m  1    a  1      x  1   +    m  2    a  2      x  2   +
      m  3    a  3      x  3    )          {\displaystyle {\begin{aligned}h^
      {\mathrm {three} }(m_{1},m_{2},m_{3})&:={\frac {1}{a_{3}}}\int _{0}^{a_
      {3}}h^{\mathrm {two} }(m_{1},m_{2},x_{3})\cdot e^{-i2\pi {\frac {m_{3}}
      {a_{3}}}x_{3}}\,dx_{3}\\[12pt]&={\frac {1}{a_{3}}}\int _{0}^{a_{3}}dx_{3}
      {\frac {1}{a_{2}}}\int _{0}^{a_{2}}dx_{2}{\frac {1}{a_{1}}}\int _{0}^{a_
      {1}}dx_{1}g(x_{1},x_{2},x_{3})\cdot e^{-i2\pi \left({\frac {m_{1}}{a_
      {1}}}x_{1}+{\frac {m_{2}}{a_{2}}}x_{2}+{\frac {m_{3}}{a_{3}}}x_
      {3}\right)}\end{aligned}}}  [
      \begin{align}
      h^\mathrm{three}(m_1, m_2, m_3) & := \frac{1}{a_3}\int_0^{a_3} h^\mathrm
      {two}(m_1, m_2, x_3)\cdot e^{-i 2\pi \frac{m_3}{a_3} x_3}\, dx_3 \\[12pt]
      & = \frac{1}{a_3}\int_0^{a_3} dx_3 \frac{1}{a_2}\int_0^{a_2} dx_2 \frac
      {1}{a_1}\int_0^{a_1} dx_1 g(x_1, x_2, x_3)\cdot e^{-i 2\pi \left(\frac
      {m_1}{a_1} x_1+\frac{m_2}{a_2} x_2 + \frac{m_3}{a_3} x_3\right)}
      \end{align}
      ]
We write     g   {\displaystyle g}  [g] as:
         g (  x  1   ,  x  2   ,  x  3   ) =  &#x2211;   m  1   = &#x2212;
      &#x221E;   &#x221E;    &#x2211;   m  2   = &#x2212; &#x221E;   &#x221E;
      &#x2211;   m  3   = &#x2212; &#x221E;   &#x221E;    h   t h r e e    (  m
      1   ,  m  2   ,  m  3   ) &#x22C5;  e  i 2 &#x03C0;    m  1    a  1
      x  1     &#x22C5;  e  i 2 &#x03C0;    m  2    a  2      x  2     &#x22C5;
      e  i 2 &#x03C0;    m  3    a  3      x  3       {\displaystyle g(x_{1},x_
      {2},x_{3})=\sum _{m_{1}=-\infty }^{\infty }\sum _{m_{2}=-\infty }^{\infty
      }\sum _{m_{3}=-\infty }^{\infty }h^{\mathrm {three} }(m_{1},m_{2},m_
      {3})\cdot e^{i2\pi {\frac {m_{1}}{a_{1}}}x_{1}}\cdot e^{i2\pi {\frac {m_
      {2}}{a_{2}}}x_{2}}\cdot e^{i2\pi {\frac {m_{3}}{a_{3}}}x_{3}}}  [g(x_1,
      x_2, x_3)=\sum_{m_1=-\infty}^\infty \sum_{m_2=-\infty}^\infty \sum_{m_3=-
      \infty}^\infty h^\mathrm{three}(m_1, m_2, m_3) \cdot e^{i 2\pi \frac{m_1}
      {a_1} x_1} \cdot e^{i 2\pi \frac{m_2}{a_2} x_2}\cdot e^{i 2\pi \frac{m_3}
      {a_3} x_3}]
Re-arranging:
         g (  x  1   ,  x  2   ,  x  3   ) =  &#x2211;   m  1   ,  m  2   ,  m
      3   &#x2208;  Z     h   t h r e e    (  m  1   ,  m  2   ,  m  3   )
      &#x22C5;  e  i 2 &#x03C0;  (     m  1    a  1      x  1   +    m  2    a
      2      x  2   +    m  3    a  3      x  3    )    .   {\displaystyle g(x_
      {1},x_{2},x_{3})=\sum _{m_{1},m_{2},m_{3}\in \mathbb {Z} }h^{\mathrm
      {three} }(m_{1},m_{2},m_{3})\cdot e^{i2\pi \left({\frac {m_{1}}{a_{1}}}x_
      {1}+{\frac {m_{2}}{a_{2}}}x_{2}+{\frac {m_{3}}{a_{3}}}x_{3}\right)}.}  [g
      (x_1, x_2, x_3)=\sum_{m_1, m_2, m_3 \in \Z } h^\mathrm{three}(m_1, m_2,
      m_3) \cdot e^{i 2\pi \left( \frac{m_1}{a_1} x_1+ \frac{m_2}{a_2} x_2 +
      \frac{m_3}{a_3} x_3\right)}. ]
Now, every reciprocal lattice vector can be written as      K  =  &#x2113;  1
g   1   +  &#x2113;  2     g   2   +  &#x2113;  3     g   3     {\displaystyle
\mathbf {K} =\ell _{1}\mathbf {g} _{1}+\ell _{2}\mathbf {g} _{2}+\ell _
{3}\mathbf {g} _{3}}  [{\displaystyle \mathbf {K} =\ell _{1}\mathbf {g} _
{1}+\ell _{2}\mathbf {g} _{2}+\ell _{3}\mathbf {g} _{3}}], where      l  i
{\displaystyle l_{i}}  [l_{i}] are integers and       g   i     {\displaystyle
\mathbf {g} _{i}}  [\mathbf{g}_i] are the reciprocal lattice vectors, we can
use the fact that       g  i    &#x22C5;   a  j    = 2 &#x03C0;  &#x03B4;  i j
{\displaystyle \mathbf {g_{i}} \cdot \mathbf {a_{j}} =2\pi \delta _{ij}}
[\mathbf{g_i} \cdot \mathbf{a_j}=2\pi\delta_{ij}] to calculate that for any
arbitrary reciprocal lattice vector      K    {\displaystyle \mathbf {K} }
[\mathbf {K} ] and arbitrary vector in space      r    {\displaystyle \mathbf
{r} }  [\mathbf {r} ], their scalar product is:
          K  &#x22C5;  r  =  (   &#x2113;  1     g   1   +  &#x2113;  2     g
      2   +  &#x2113;  3     g   3    )  &#x22C5;  (   x  1       a   1    a  1
      +  x  2       a   2    a  2     +  x  3       a   3    a  3      )  = 2
      &#x03C0;  (   x  1      &#x2113;  1    a  1     +  x  2      &#x2113;  2
      a  2     +  x  3      &#x2113;  3    a  3      )  .   {\displaystyle
      \mathbf {K} \cdot \mathbf {r} =\left(\ell _{1}\mathbf {g} _{1}+\ell _
      {2}\mathbf {g} _{2}+\ell _{3}\mathbf {g} _{3}\right)\cdot \left(x_{1}
      {\frac {\mathbf {a} _{1}}{a_{1}}}+x_{2}{\frac {\mathbf {a} _{2}}{a_
      {2}}}+x_{3}{\frac {\mathbf {a} _{3}}{a_{3}}}\right)=2\pi \left(x_{1}
      {\frac {\ell _{1}}{a_{1}}}+x_{2}{\frac {\ell _{2}}{a_{2}}}+x_{3}{\frac
      {\ell _{3}}{a_{3}}}\right).}  [{\displaystyle \mathbf {K} \cdot \mathbf
      {r} =\left(\ell _{1}\mathbf {g} _{1}+\ell _{2}\mathbf {g} _{2}+\ell _
      {3}\mathbf {g} _{3}\right)\cdot \left(x_{1}{\frac {\mathbf {a} _{1}}{a_
      {1}}}+x_{2}{\frac {\mathbf {a} _{2}}{a_{2}}}+x_{3}{\frac {\mathbf {a} _
      {3}}{a_{3}}}\right)=2\pi \left(x_{1}{\frac {\ell _{1}}{a_{1}}}+x_{2}
      {\frac {\ell _{2}}{a_{2}}}+x_{3}{\frac {\ell _{3}}{a_{3}}}\right).}]
And so it is clear that in our expansion, the sum is actually over reciprocal
lattice vectors:
         f (  r  ) =  &#x2211;   K    h (  K  ) &#x22C5;  e  i  K  &#x22C5;  r
      ,   {\displaystyle f(\mathbf {r} )=\sum _{\mathbf {K} }h(\mathbf {K}
      )\cdot e^{i\mathbf {K} \cdot \mathbf {r} },}  [f(\mathbf{r})=\sum_
      {\mathbf{K}} h(\mathbf{K}) \cdot e^{i \mathbf{K} \cdot \mathbf{r}}, ]
where
         h (  K  ) =   1  a  3      &#x222B;  0    a  3     d  x  3      1  a
      2      &#x222B;  0    a  2     d  x  2      1  a  1      &#x222B;  0    a
      1     d  x  1    f  (   x  1       a   1    a  1     +  x  2       a   2
      a  2     +  x  3       a   3    a  3      )  &#x22C5;  e  &#x2212; i  K
      &#x22C5;  r    .   {\displaystyle h(\mathbf {K} )={\frac {1}{a_{3}}}\int
      _{0}^{a_{3}}dx_{3}\,{\frac {1}{a_{2}}}\int _{0}^{a_{2}}dx_{2}\,{\frac {1}
      {a_{1}}}\int _{0}^{a_{1}}dx_{1}\,f\left(x_{1}{\frac {\mathbf {a} _{1}}{a_
      {1}}}+x_{2}{\frac {\mathbf {a} _{2}}{a_{2}}}+x_{3}{\frac {\mathbf {a} _
      {3}}{a_{3}}}\right)\cdot e^{-i\mathbf {K} \cdot \mathbf {r} }.}  [
      {\displaystyle h(\mathbf {K} )={\frac {1}{a_{3}}}\int _{0}^{a_{3}}dx_
      {3}\,{\frac {1}{a_{2}}}\int _{0}^{a_{2}}dx_{2}\,{\frac {1}{a_{1}}}\int _
      {0}^{a_{1}}dx_{1}\,f\left(x_{1}{\frac {\mathbf {a} _{1}}{a_{1}}}+x_{2}
      {\frac {\mathbf {a} _{2}}{a_{2}}}+x_{3}{\frac {\mathbf {a} _{3}}{a_
      {3}}}\right)\cdot e^{-i\mathbf {K} \cdot \mathbf {r} }.}]
Assuming
          r  = ( x , y , z ) =  x  1       a   1    a  1     +  x  2       a
      2    a  2     +  x  3       a   3    a  3     ,   {\displaystyle \mathbf
      {r} =(x,y,z)=x_{1}{\frac {\mathbf {a} _{1}}{a_{1}}}+x_{2}{\frac {\mathbf
      {a} _{2}}{a_{2}}}+x_{3}{\frac {\mathbf {a} _{3}}{a_{3}}},}  [
      {\displaystyle \mathbf {r} =(x,y,z)=x_{1}{\frac {\mathbf {a} _{1}}{a_
      {1}}}+x_{2}{\frac {\mathbf {a} _{2}}{a_{2}}}+x_{3}{\frac {\mathbf {a} _
      {3}}{a_{3}}},}]
we can solve this system of three linear equations for     x   {\displaystyle
x}  [x],     y   {\displaystyle y}  [y], and     z   {\displaystyle z}  [z] in
terms of      x  1     {\displaystyle x_{1}}  [x_{1}],      x  2
{\displaystyle x_{2}}  [x_{2}] and      x  3     {\displaystyle x_{3}}  [x_{3}]
in order to calculate the volume element in the original cartesian coordinate
system. Once we have     x   {\displaystyle x}  [x],     y   {\displaystyle y}
[y], and     z   {\displaystyle z}  [z] in terms of      x  1
{\displaystyle x_{1}}  [x_{1}],      x  2     {\displaystyle x_{2}}  [x_{2}]
and      x  3     {\displaystyle x_{3}}  [x_{3}], we can calculate the Jacobian
determinant:
           |        &#x2202;  x  1     &#x2202; x           &#x2202;  x  1
      &#x2202; y           &#x2202;  x  1     &#x2202; z             &#x2202;
      x  2     &#x2202; x           &#x2202;  x  2     &#x2202; y
      &#x2202;  x  2     &#x2202; z             &#x2202;  x  3     &#x2202; x
      &#x2202;  x  3     &#x2202; y           &#x2202;  x  3     &#x2202; z
      |     {\displaystyle {\begin{vmatrix}{\dfrac {\partial x_{1}}{\partial
      x}}&{\dfrac {\partial x_{1}}{\partial y}}&{\dfrac {\partial x_{1}}
      {\partial z}}\\[12pt]{\dfrac {\partial x_{2}}{\partial x}}&{\dfrac
      {\partial x_{2}}{\partial y}}&{\dfrac {\partial x_{2}}{\partial z}}\\
      [12pt]{\dfrac {\partial x_{3}}{\partial x}}&{\dfrac {\partial x_{3}}
      {\partial y}}&{\dfrac {\partial x_{3}}{\partial z}}\end{vmatrix}}}  [
      {\displaystyle {\begin{vmatrix}{\dfrac {\partial x_{1}}{\partial x}}&
      {\dfrac {\partial x_{1}}{\partial y}}&{\dfrac {\partial x_{1}}{\partial
      z}}\\[12pt]{\dfrac {\partial x_{2}}{\partial x}}&{\dfrac {\partial x_{2}}
      {\partial y}}&{\dfrac {\partial x_{2}}{\partial z}}\\[12pt]{\dfrac
      {\partial x_{3}}{\partial x}}&{\dfrac {\partial x_{3}}{\partial y}}&
      {\dfrac {\partial x_{3}}{\partial z}}\end{vmatrix}}}]
which after some calculation and applying some non-trivial cross-product
identities can be shown to be equal to:
             a  1    a  2    a  3       a  1    &#x22C5; (   a  2    &#x00D7;
      a  3    )      {\displaystyle {\frac {a_{1}a_{2}a_{3}}{\mathbf {a_{1}}
      \cdot (\mathbf {a_{2}} \times \mathbf {a_{3}} )}}}  [\frac{a_1 a_2 a_3}
      {\mathbf{a_1}\cdot(\mathbf{a_2} \times \mathbf{a_3})}]
(it may be advantageous for the sake of simplifying calculations, to work in
such a cartesian coordinate system, in which it just so happens that       a  1
{\displaystyle \mathbf {a_{1}} }  [{\displaystyle \mathbf {a_{1}} }] is
parallel to the x axis,       a  2      {\displaystyle \mathbf {a_{2}} }  [
{\displaystyle \mathbf {a_{2}} }] lies in the x-y plane, and       a  3
{\displaystyle \mathbf {a_{3}} }  [{\displaystyle \mathbf {a_{3}} }] has
components of all three axes). The denominator is exactly the volume of the
primitive unit cell which is enclosed by the three primitive-vectors       a  1
{\displaystyle \mathbf {a_{1}} }  [{\displaystyle \mathbf {a_{1}} }],       a
2      {\displaystyle \mathbf {a_{2}} }  [{\displaystyle \mathbf {a_{2}} }] and
a  3      {\displaystyle \mathbf {a_{3}} }  [{\displaystyle \mathbf {a_{3}} }].
In particular, we now know that
         d  x  1    d  x  2    d  x  3   =     a  1    a  2    a  3       a  1
      &#x22C5; (   a  2    &#x00D7;   a  3    )    &#x22C5; d x  d y  d z .
      {\displaystyle dx_{1}\,dx_{2}\,dx_{3}={\frac {a_{1}a_{2}a_{3}}{\mathbf
      {a_{1}} \cdot (\mathbf {a_{2}} \times \mathbf {a_{3}} )}}\cdot
      dx\,dy\,dz.}  [dx_1 \, dx_2 \, dx_3 = \frac{a_1 a_2 a_3}{\mathbf
      {a_1}\cdot(\mathbf{a_2} \times \mathbf{a_3})} \cdot dx \, dy \, dz. ]
We can write now     h (  K  )   {\displaystyle h(\mathbf {K} )}  [
{\displaystyle h(\mathbf {K} )}] as an integral with the traditional coordinate
system over the volume of the primitive cell, instead of with the      x  1
{\displaystyle x_{1}}  [x_{1}],      x  2     {\displaystyle x_{2}}  [x_{2}]
and      x  3     {\displaystyle x_{3}}  [x_{3}] variables:
         h (  K  ) =   1    a  1    &#x22C5; (   a  2    &#x00D7;   a  3    )
      &#x222B;  C   d  r  f (  r  ) &#x22C5;  e  &#x2212; i  K  &#x22C5;  r
      {\displaystyle h(\mathbf {K} )={\frac {1}{\mathbf {a_{1}} \cdot (\mathbf
      {a_{2}} \times \mathbf {a_{3}} )}}\int _{C}d\mathbf {r} f(\mathbf {r}
      )\cdot e^{-i\mathbf {K} \cdot \mathbf {r} }}  [h(\mathbf{K}) = \frac{1}
      {\mathbf{a_1}\cdot(\mathbf{a_2} \times \mathbf{a_3})}\int_{C} d\mathbf{r}
      f(\mathbf{r})\cdot e^{-i \mathbf{K} \cdot \mathbf{r}} ]
And     C   {\displaystyle C}  [C] is the primitive unit cell, thus,       a  1
&#x22C5; (   a  2    &#x00D7;   a  3    )   {\displaystyle \mathbf {a_{1}}
\cdot (\mathbf {a_{2}} \times \mathbf {a_{3}} )}  [\mathbf{a_1}\cdot(\mathbf
{a_2} \times \mathbf{a_3})] is the volume of the primitive unit cell.
**** Hilbert space interpretation[edit] ****
Main article: Hilbert_space
In the language of Hilbert_spaces, the set of functions     {  e  n   =  e  i n
x   : n &#x2208;  Z  }   {\displaystyle \{e_{n}=e^{inx}:n\in \mathbb {Z} \}}  [
{\displaystyle \{e_{n}=e^{inx}:n\in \mathbb {Z} \}}] is an orthonormal_basis
for the space      L  2   ( [ &#x2212; &#x03C0; , &#x03C0; ] )   {\displaystyle
L^{2}([-\pi ,\pi ])}  [{\displaystyle L^{2}([-\pi ,\pi ])}] of square-
integrable functions on     [ &#x2212; &#x03C0; , &#x03C0; ]   {\displaystyle
[-\pi ,\pi ]}  [[-\pi ,\pi ]]. This space is actually a Hilbert space with an
inner_product given for any two elements     f   {\displaystyle f}  [f] and
g   {\displaystyle g}  [g] by
         &#x27E8; f ,  g &#x27E9;  &#x225C;    1  2 &#x03C0;     &#x222B;
      &#x2212; &#x03C0;   &#x03C0;   f ( x )    g ( x )  &#x00AF;    d x .
      {\displaystyle \langle f,\,g\rangle \;\triangleq \;{\frac {1}{2\pi }}\int
      _{-\pi }^{\pi }f(x){\overline {g(x)}}\,dx.}  [{\displaystyle \langle
      f,\,g\rangle \;\triangleq \;{\frac {1}{2\pi }}\int _{-\pi }^{\pi }f(x)
      {\overline {g(x)}}\,dx.}]
The basic Fourier series result for Hilbert spaces can be written as
         f =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;   &#x27E8; f ,  e  n
      &#x27E9;   e  n   .   {\displaystyle f=\sum _{n=-\infty }^{\infty
      }\langle f,e_{n}\rangle \,e_{n}.}  [f=\sum_{n=-\infty}^\infty \langle
      f,e_n \rangle \, e_n.]
Sines and cosines form an orthonormal set, as illustrated above. The integral
of sine, cosine and their product is zero (green and red areas are equal, and
cancel out) when     m   {\displaystyle m}  [m],     n   {\displaystyle n}  [n]
or the functions are different, and pi only if     m   {\displaystyle m}  [m]
and     n   {\displaystyle n}  [n] are equal, and the function used is the
same.
This corresponds exactly to the complex exponential formulation given above.
The version with sines and cosines is also justified with the Hilbert space
interpretation. Indeed, the sines and cosines form an orthogonal_set:
          &#x222B;  &#x2212; &#x03C0;   &#x03C0;   cos &#x2061; ( m x )  cos
      &#x2061; ( n x )  d x =   1 2    &#x222B;  &#x2212; &#x03C0;   &#x03C0;
      cos &#x2061; ( ( n &#x2212; m ) x ) + cos &#x2061; ( ( n + m ) x )  d x =
      &#x03C0;  &#x03B4;  m n   ,  m , n &#x2265; 1 ,    {\displaystyle \int _
      {-\pi }^{\pi }\cos(mx)\,\cos(nx)\,dx={\frac {1}{2}}\int _{-\pi }^{\pi
      }\cos((n-m)x)+\cos((n+m)x)\,dx=\pi \delta _{mn},\quad m,n\geq 1,\,}  [
      {\displaystyle \int _{-\pi }^{\pi }\cos(mx)\,\cos(nx)\,dx={\frac {1}
      {2}}\int _{-\pi }^{\pi }\cos((n-m)x)+\cos((n+m)x)\,dx=\pi \delta _
      {mn},\quad m,n\geq 1,\,}]
          &#x222B;  &#x2212; &#x03C0;   &#x03C0;   sin &#x2061; ( m x )  sin
      &#x2061; ( n x )  d x =   1 2    &#x222B;  &#x2212; &#x03C0;   &#x03C0;
      cos &#x2061; ( ( n &#x2212; m ) x ) &#x2212; cos &#x2061; ( ( n + m ) x )
      d x = &#x03C0;  &#x03B4;  m n   ,  m , n &#x2265; 1   {\displaystyle \int
      _{-\pi }^{\pi }\sin(mx)\,\sin(nx)\,dx={\frac {1}{2}}\int _{-\pi }^{\pi
      }\cos((n-m)x)-\cos((n+m)x)\,dx=\pi \delta _{mn},\quad m,n\geq 1}  [
      {\displaystyle \int _{-\pi }^{\pi }\sin(mx)\,\sin(nx)\,dx={\frac {1}
      {2}}\int _{-\pi }^{\pi }\cos((n-m)x)-\cos((n+m)x)\,dx=\pi \delta _
      {mn},\quad m,n\geq 1}]
(where Î´mn is the Kronecker_delta), and
          &#x222B;  &#x2212; &#x03C0;   &#x03C0;   cos &#x2061; ( m x )  sin
      &#x2061; ( n x )  d x =   1 2    &#x222B;  &#x2212; &#x03C0;   &#x03C0;
      sin &#x2061; ( ( n + m ) x ) + sin &#x2061; ( ( n &#x2212; m ) x )  d x =
      0 ;    {\displaystyle \int _{-\pi }^{\pi }\cos(mx)\,\sin(nx)\,dx={\frac
      {1}{2}}\int _{-\pi }^{\pi }\sin((n+m)x)+\sin((n-m)x)\,dx=0;\,}  [
      {\displaystyle \int _{-\pi }^{\pi }\cos(mx)\,\sin(nx)\,dx={\frac {1}
      {2}}\int _{-\pi }^{\pi }\sin((n+m)x)+\sin((n-m)x)\,dx=0;\,}]
furthermore, the sines and cosines are orthogonal to the constant function
1   {\displaystyle 1}  [1]. An orthonormal basis for      L  2   ( [ &#x2212;
&#x03C0; , &#x03C0; ] )   {\displaystyle L^{2}([-\pi ,\pi ])}  [{\displaystyle
L^{2}([-\pi ,\pi ])}] consisting of real functions is formed by the functions
1   {\displaystyle 1}  [1] and       2   cos &#x2061; ( n x )   {\displaystyle
{\sqrt {2}}\cos(nx)}  [{\displaystyle {\sqrt {2}}\cos(nx)}],       2   sin
&#x2061; ( n x )   {\displaystyle {\sqrt {2}}\sin(nx)}  [{\displaystyle {\sqrt
{2}}\sin(nx)}] with n = 1, 2,...  The density of their span is a consequence of
the StoneâWeierstrass_theorem, but follows also from the properties of
classical kernels like the FejÃ©r_kernel.
***** Properties[edit] *****
**** Table of basic properties[edit] ****
This table shows some mathematical operations in the time domain and the
corresponding effect in the Fourier series coefficients. Notation:
    *     z  &#x2217;     {\displaystyle z^{*}}  [z^{*}] is the complex
      conjugate of     z   {\displaystyle z}  [z].
    *    f ( x ) , g ( x )   {\displaystyle f(x),g(x)}  [{\displaystyle f(x),g
      (x)}] designate     P   {\displaystyle P}  [P]-periodic functions defined
      on     0 < x &#x2264; P   {\displaystyle 0<x\leq P}  [{\displaystyle
      0<x\leq P}].
    *    F [ n ] , G [ n ]   {\displaystyle F[n],G[n]}  [{\displaystyle F[n],G
      [n]}] designate the Fourier series coefficients (exponential form) of
      f   {\displaystyle f}  [f] and     g   {\displaystyle g}  [g] as defined
      in equation Eq.5.
                                  Frequency domain
Property         Time domain      (exponential     Remarks         Reference
                                  form)
                    a &#x22C5; f     a &#x22C5; F
                 ( x ) + b        [ n ] + b
                 &#x22C5; g ( x ) &#x22C5; G [ n ]
                 {\displaystyle   {\displaystyle   complex numbers
Linearity        a\cdot f         a\cdot F         a , b
                 (x)+b\cdot g(x)} [n]+b\cdot G[n]} {\displaystyle
                 [{\displaystyle  [{\displaystyle  a,b}  [a,b]
                 a\cdot f         a\cdot F
                 (x)+b\cdot g     [n]+b\cdot G
                 (x)}]            [n]}]
                                     F [ &#x2212;
Time reversal /     f ( &#x2212;  n ]
Frequency        x )              {\displaystyle F                 [13]:p. 610
reversal         {\displaystyle f [-n]}  [
                 (-x)}  [f(-x)]   {\displaystyle F
                                  [-n]}]
                    f ( x  )         F [ &#x2212;
                 &#x2217;         n  ]  &#x2217;
Time conjugation {\displaystyle f {\displaystyle F                 [13]:p. 610
                 (x)^{*}}  [      [-n]^{*}}  [
                 {\displaystyle f {\displaystyle F
                 (x)^{*}}]        [-n]^{*}}]
                    f ( &#x2212;     F [ n  ]
                 x  )  &#x2217;   &#x2217;
Time reversal &  {\displaystyle f {\displaystyle F
conjugation      (-x)^{*}}  [     [n]^{*}}  [
                 {\displaystyle f {\displaystyle F
                 (-x)^{*}}]       [n]^{*}}]
                                       1 2   ( F
                    Re &#x2061;   [ n ] + F
                 ( f ( x ) )      [ &#x2212; n  ]
                 {\displaystyle   &#x2217;   )
Real part in     \operatorname    {\displaystyle
time             {Re} {(f(x))}}   {\frac {1}{2}}(F
                 [{\displaystyle  [n]+F[-n]^{*})}
                 \operatorname    [{\displaystyle
                 {Re} {(f(x))}}]  {\frac {1}{2}}(F
                                  [n]+F[-n]^{*})}]
                                       1  2 i
                                  ( F [ n ]
                    Im &#x2061;   &#x2212; F
                 ( f ( x ) )      [ &#x2212; n  ]
                 {\displaystyle   &#x2217;   )
Imaginary part   \operatorname    {\displaystyle
in time          {Im} {(f(x))}}   {\frac {1}{2i}}
                 [{\displaystyle  (F[n]-F[-n]^
                 \operatorname    {*})}  [
                 {Im} {(f(x))}}]  {\displaystyle
                                  {\frac {1}{2i}}
                                  (F[n]-F[-n]^
                                  {*})}]
                      1 2   ( f
                 ( x ) + f           Re &#x2061;
                 ( &#x2212; x  )  ( F [ n ] )
                 &#x2217;   )     {\displaystyle
Real part in     {\displaystyle   \operatorname
frequency        {\frac {1}{2}}(f {Re} {(F[n])}}
                 (x)+f(-x)^{*})}  [{\displaystyle
                 [{\displaystyle  \operatorname
                 {\frac {1}{2}}(f {Re} {(F[n])}}]
                 (x)+f(-x)^{*})}]
                      1  2 i
                 ( f ( x )
                 &#x2212; f          Im &#x2061;
                 ( &#x2212; x  )  ( F [ n ] )
                 &#x2217;   )     {\displaystyle
Imaginary part   {\displaystyle   \operatorname
in frequency     {\frac {1}{2i}}  {Im} {(F[n])}}
                 (f(x)-f(-x)^     [{\displaystyle
                 {*})}  [         \operatorname
                 {\displaystyle   {Im} {(F[n])}}]
                 {\frac {1}{2i}}
                 (f(x)-f(-x)^
                 {*})}]
                                     F [ n ]
                                  &#x22C5;  e
                                  &#x2212; i    2
                    f ( x         &#x03C0;  x  0
                 &#x2212;  x  0   T   n            real number
Shift in time /  )                {\displaystyle F x  0
Modulation in    {\displaystyle f [n]\cdot e^{-i   {\displaystyle  [13]:p. 610
frequency        (x-x_{0})}  [    {\frac {2\pi x_  x_{0}}  [x_{0}]
                 {\displaystyle f {0}}{T}}n}}  [
                 (x-x_{0})}]      {\displaystyle F
                                  [n]\cdot e^{-i
                                  {\frac {2\pi x_
                                  {0}}{T}}n}}]
                    f ( x )
                 &#x22C5;  e  i
                 2 &#x03C0;  n  0    F [ n
                 T   x            &#x2212;  n  0
Shift in         {\displaystyle f ]                integer      n
frequency /      (x)\cdot e^{i    {\displaystyle F 0               [13]:p. 610
Modulation in    {\frac {2\pi n_  [n-n_{0}]\!}  [  {\displaystyle
time             {0}}{T}}x}}  [   {\displaystyle F n_{0}}  [n_{0}]
                 {\displaystyle f [n-n_{0}]\!}]
                 (x)\cdot e^{i
                 {\frac {2\pi n_
                 {0}}{T}}x}}]
**** Symmetry properties[edit] ****
When the real and imaginary parts of a complex function are decomposed into
their even_and_odd_parts, there are four components, denoted below by the
subscripts RE, RO, IE, and IO. And there is a one-to-one mapping between the
four components of a complex time function and the four components of its
complex frequency transform:[14]
              Time domain    f   =    f     RE       +    f     RO       +   i
      f     IE       +      i &#xA0;  f     IO      &#x23DF;          &#x21D5;
      F        &#x21D5;     F      &#xA0; &#xA0;   &#x21D5;     F      &#xA0;
      &#xA0;   &#x21D5;     F      &#xA0; &#xA0;   &#x21D5;     F
      Frequency domain    F   =    F  R E     +      i &#xA0;  F  I O
      &#x23DE;     +   i &#xA0;  F  I E     +    F  R O         {\displaystyle
      {\begin{array}{rccccccccc}{\text{Time domain}}&f&=&f_{_{\text{RE}}}&+&f_
      {_{\text{RO}}}&+&if_{_{\text{IE}}}&+&\underbrace {i\ f_{_{\text{IO}}}}
      \\&{\Bigg \Updownarrow }{\mathcal {F}}&&{\Bigg \Updownarrow }{\mathcal
      {F}}&&\ \ {\Bigg \Updownarrow }{\mathcal {F}}&&\ \ {\Bigg \Updownarrow }
      {\mathcal {F}}&&\ \ {\Bigg \Updownarrow }{\mathcal {F}}\\{\text{Frequency
      domain}}&F&=&F_{RE}&+&\overbrace {i\ F_{IO}} &+&i\ F_{IE}&+&F_{RO}\end
      {array}}}  [{\displaystyle {\begin{array}{rccccccccc}{\text{Time
      domain}}&f&=&f_{_{\text{RE}}}&+&f_{_{\text{RO}}}&+&if_{_{\text
      {IE}}}&+&\underbrace {i\ f_{_{\text{IO}}}} \\&{\Bigg \Updownarrow }
      {\mathcal {F}}&&{\Bigg \Updownarrow }{\mathcal {F}}&&\ \ {\Bigg
      \Updownarrow }{\mathcal {F}}&&\ \ {\Bigg \Updownarrow }{\mathcal {F}}&&\
      \ {\Bigg \Updownarrow }{\mathcal {F}}\\{\text{Frequency domain}}&F&=&F_
      {RE}&+&\overbrace {i\ F_{IO}} &+&i\ F_{IE}&+&F_{RO}\end{array}}}]
From this, various relationships are apparent, for example:
    * The transform of a real-valued function (fRE+ fRO) is the even_symmetric
      function FRE+ i FIO. Conversely, an even-symmetric transform implies a
      real-valued time-domain.
    * The transform of an imaginary-valued function (i fIE+ i fIO) is the odd
      symmetric function FRO+ i FIE, and the converse is true.
    * The transform of an even-symmetric function (fRE+ i fIO) is the real-
      valued function FRE+ FRO, and the converse is true.
    * The transform of an odd-symmetric function (fRO+ i fIE) is the imaginary-
      valued function i FIE+ i FIO, and the converse is true.
**** RiemannâLebesgue lemma[edit] ****
If     f   {\displaystyle f}  [f] is integrable,      lim   |  n  |  &#x2192;
&#x221E;      f &#x005E;    ( n ) = 0   {\displaystyle \lim _{|n|\rightarrow
\infty }{\hat {f}}(n)=0}  [\lim_{|n|\rightarrow \infty}\hat{f}(n)=0],      lim
n &#x2192; + &#x221E;    a  n   = 0   {\displaystyle \lim _{n\rightarrow
+\infty }a_{n}=0}  [\lim_{n\rightarrow +\infty}a_n=0] and      lim  n &#x2192;
+ &#x221E;    b  n   = 0.   {\displaystyle \lim _{n\rightarrow +\infty }b_
{n}=0.}  [\lim_{n\rightarrow +\infty}b_n=0.] This result is known as the
RiemannâLebesgue_lemma.
**** Derivative property[edit] ****
We say that     f   {\displaystyle f}  [f] belongs to      C  k   (  T  )
{\displaystyle C^{k}(\mathbb {T} )}  [C^k(\mathbb{T})] if     f
{\displaystyle f}  [f] is a 2Ï-periodic function on      R    {\displaystyle
\mathbb {R} }  [\mathbb {R} ] which is     k   {\displaystyle k}  [k] times
differentiable, and its kth derivative is continuous.
    * If     f &#x2208;  C  1   (  T  )   {\displaystyle f\in C^{1}(\mathbb {T}
      )}  [f \in C^1(\mathbb{T})], then the Fourier coefficients         f
      &#x2032;  &#x005E;    ( n )   {\displaystyle {\widehat {f'}}(n)}
      [\widehat{f'}(n)] of the derivative      f &#x2032;    {\displaystyle f'}
      [f'] can be expressed in terms of the Fourier coefficients        f
      &#x005E;    ( n )   {\displaystyle {\widehat {f}}(n)}  [\widehat{f}(n)]
      of the function     f   {\displaystyle f}  [f], via the formula         f
      &#x2032;  &#x005E;    ( n ) = i n    f &#x005E;    ( n )   {\displaystyle
      {\widehat {f'}}(n)=in{\widehat {f}}(n)}  [{\displaystyle {\widehat {f'}}
      (n)=in{\widehat {f}}(n)}].
    * If     f &#x2208;  C  k   (  T  )   {\displaystyle f\in C^{k}(\mathbb {T}
      )}  [f \in C^k(\mathbb{T})], then         f  ( k )   &#x005E;    ( n ) =
      ( i n  )  k      f &#x005E;    ( n )   {\displaystyle {\widehat {f^{
      (k)}}}(n)=(in)^{k}{\widehat {f}}(n)}  [{\displaystyle {\widehat {f^{
      (k)}}}(n)=(in)^{k}{\widehat {f}}(n)}]. In particular, since         f
      ( k )   &#x005E;    ( n )   {\displaystyle {\widehat {f^{(k)}}}(n)}
      [\widehat{f^{(k)}}(n)] tends to zero, we have that      |  n   |   k
      f &#x005E;    ( n )   {\displaystyle |n|^{k}{\widehat {f}}(n)}  [
      {\displaystyle |n|^{k}{\widehat {f}}(n)}] tends to zero, which means that
      the Fourier coefficients converge to zero faster than the kth power of n.
**** Parseval's_theorem[edit] ****
If     f   {\displaystyle f}  [f] belongs to      L  2   ( [ &#x2212; &#x03C0;
, &#x03C0; ] )   {\displaystyle L^{2}([-\pi ,\pi ])}  [{\displaystyle L^{2}([-
\pi ,\pi ])}], then      &#x2211;  n = &#x2212; &#x221E;   &#x221E;    |     f
&#x005E;    ( n )   |   2   =   1  2 &#x03C0;     &#x222B;  &#x2212; &#x03C0;
&#x03C0;    |  f ( x )   |   2    d x   {\displaystyle \sum _{n=-\infty }^
{\infty }|{\hat {f}}(n)|^{2}={\frac {1}{2\pi }}\int _{-\pi }^{\pi }|f(x)|^
{2}\,dx}  [\sum_{n=-\infty}^\infty |\hat{f}(n)|^2 = \frac{1}{2\pi}\int_{-\pi}^
{\pi} |f(x)|^2 \, dx].
**** Plancherel's_theorem[edit] ****
If      c  0   ,   c  &#x00B1; 1   ,   c  &#x00B1; 2   , &#x2026;
{\displaystyle c_{0},\,c_{\pm 1},\,c_{\pm 2},\ldots }  [c_0,\, c_{\pm 1},\, c_
{\pm 2},\ldots] are coefficients and      &#x2211;  n = &#x2212; &#x221E;
&#x221E;    |   c  n     |   2   < &#x221E;   {\displaystyle \sum _{n=-\infty
}^{\infty }|c_{n}|^{2}<\infty }  [\sum_{n=-\infty}^\infty |c_n|^2 < \infty]
then there is a unique function     f &#x2208;  L  2   ( [ &#x2212; &#x03C0; ,
&#x03C0; ] )   {\displaystyle f\in L^{2}([-\pi ,\pi ])}  [f\in L^2([-\pi,\pi])]
such that        f &#x005E;    ( n ) =  c  n     {\displaystyle {\hat {f}}
(n)=c_{n}}  [\hat{f}(n) = c_n] for every     n   {\displaystyle n}  [n].
**** Convolution theorems[edit] ****
    * The first convolution theorem states that if     f   {\displaystyle f}
      [f] and     g   {\displaystyle g}  [g] are in      L  1   ( [ &#x2212;
      &#x03C0; , &#x03C0; ] )   {\displaystyle L^{1}([-\pi ,\pi ])}  [
      {\displaystyle L^{1}([-\pi ,\pi ])}], the Fourier series coefficients of
      the 2Ï-periodic convolution of     f   {\displaystyle f}  [f] and     g
      {\displaystyle g}  [g] are given by:
               [     f  &#x2217;  2 &#x03C0;   g  &#x005E;    ] ( n ) = 2
            &#x03C0; &#x22C5;    f &#x005E;    ( n ) &#x22C5;    g &#x005E;
            ( n ) ,   {\displaystyle [{\widehat {f*_{2\pi }g}}](n)=2\pi \cdot
            {\hat {f}}(n)\cdot {\hat {g}}(n),}  [[\widehat{f*_{2\pi}g}](n) =
            2\pi\cdot \hat{f}(n)\cdot\hat{g}(n),][nb_4]
      where:
                    [  f  &#x2217;  2 &#x03C0;   g  ]  ( x ) &#xA0;    &#x225C;
            &#x222B;  &#x2212; &#x03C0;   &#x03C0;   f ( u ) &#x22C5; g [ pv
            &#x2061; ( x &#x2212; u ) ]  d u ,       (    and&#xA0;      pv
            &#x2061; ( x ) &#xA0; &#x225C; Arg &#x2061; (  e  i x   )  &#x23DF;
            principal value      )         =  &#x222B;  &#x2212; &#x03C0;
            &#x03C0;   f ( u ) &#x22C5; g ( x &#x2212; u )  d u ,
            when&#xA0;  g ( x )  &#xA0;is&#xA0;  2 &#x03C0;  -periodic.
            =  &#x222B;  2 &#x03C0;   f ( u ) &#x22C5; g ( x &#x2212; u )  d u
            ,     when both functions are&#xA0;  2 &#x03C0;  -periodic, and the
            integral is over any&#xA0;  2 &#x03C0;  &#xA0;interval.
            {\displaystyle {\begin{aligned}\left[f*_{2\pi }g\right](x)\
            &\triangleq \int _{-\pi }^{\pi }f(u)\cdot g[\operatorname {pv} (x-
            u)]\,du,&&{\big (}{\text{and }}\underbrace {\operatorname {pv} (x)\
            \triangleq \operatorname {Arg} (e^{ix})} _{\text{principal
            value}}\,{\big )}\\&=\int _{-\pi }^{\pi }f(u)\cdot g(x-u)\,du,&&
            {\text{when }}g(x){\text{ is }}2\pi {\text{-periodic.}}\\&=\int _
            {2\pi }f(u)\cdot g(x-u)\,du,&&{\text{when both functions are }}2\pi
            {\text{-periodic, and the integral is over any }}2\pi {\text
            { interval.}}\end{aligned}}}  [{\displaystyle {\begin{aligned}\left
            [f*_{2\pi }g\right](x)\ &\triangleq \int _{-\pi }^{\pi }f(u)\cdot g
            [\operatorname {pv} (x-u)]\,du,&&{\big (}{\text{and }}\underbrace
            {\operatorname {pv} (x)\ \triangleq \operatorname {Arg} (e^{ix})} _
            {\text{principal value}}\,{\big )}\\&=\int _{-\pi }^{\pi }f(u)\cdot
            g(x-u)\,du,&&{\text{when }}g(x){\text{ is }}2\pi {\text{-
            periodic.}}\\&=\int _{2\pi }f(u)\cdot g(x-u)\,du,&&{\text{when both
            functions are }}2\pi {\text{-periodic, and the integral is over any
            }}2\pi {\text{ interval.}}\end{aligned}}}]
    * The second convolution theorem states that the Fourier series
      coefficients of the product of     f   {\displaystyle f}  [f] and     g
      {\displaystyle g}  [g] are given by the discrete_convolution of the
      f &#x005E;      {\displaystyle {\hat {f}}}  [{\hat {f}}] and        g
      &#x005E;      {\displaystyle {\hat {g}}}  [\hat g] sequences:
               [     f &#x22C5; g  &#x005E;    ] ( n ) = [    f &#x005E;
            &#x2217;    g &#x005E;    ] ( n ) .   {\displaystyle [{\widehat
            {f\cdot g}}](n)=[{\hat {f}}*{\hat {g}}](n).}  [[\widehat{f\cdot g}]
            (n) = [\hat{f}*\hat{g}](n).]
    * A doubly_infinite sequence       {  c  n   }   n &#x2208; Z
      {\displaystyle \left\{c_{n}\right\}_{n\in Z}}  [{\displaystyle \left\{c_
      {n}\right\}_{n\in Z}}] in      c  0   (  Z  )   {\displaystyle c_{0}
      (\mathbb {Z} )}  [{\displaystyle c_{0}(\mathbb {Z} )}] is the sequence of
      Fourier coefficients of a function in      L  1   ( [ 0 , 2 &#x03C0; ] )
      {\displaystyle L^{1}([0,2\pi ])}  [{\displaystyle L^{1}([0,2\pi ])}] if
      and only if it is a convolution of two sequences in      &#x2113;  2
      (  Z  )   {\displaystyle \ell ^{2}(\mathbb {Z} )}  [\ell ^{2}({\mathbb
      {Z}})]. See [15]
**** Compact groups[edit] ****
Main articles: Compact_group, Lie_group, and PeterâWeyl_theorem
One of the interesting properties of the Fourier transform which we have
mentioned, is that it carries convolutions to pointwise products. If that is
the property which we seek to preserve, one can produce Fourier series on any
compact_group. Typical examples include those classical_groups that are
compact. This generalizes the Fourier transform to all spaces of the form L2
(G), where G is a compact group, in such a way that the Fourier transform
carries convolutions to pointwise products. The Fourier series exists and
converges in similar ways to the [âÏ,Ï] case.
An alternative extension to compact groups is the PeterâWeyl_theorem, which
proves results about representations of compact groups analogous to those about
finite groups.
**** Riemannian manifolds[edit] ****
The atomic_orbitals of chemistry are partially described by spherical
harmonics, which can be used to produce Fourier series on the sphere.
Main articles: Laplace_operator and Riemannian_manifold
If the domain is not a group, then there is no intrinsically defined
convolution. However, if     X   {\displaystyle X}  [X] is a compact Riemannian
manifold, it has a LaplaceâBeltrami_operator. The LaplaceâBeltrami operator
is the differential operator that corresponds to Laplace_operator for the
Riemannian manifold     X   {\displaystyle X}  [X]. Then, by analogy, one can
consider heat equations on     X   {\displaystyle X}  [X]. Since Fourier
arrived at his basis by attempting to solve the heat equation, the natural
generalization is to use the eigensolutions of the LaplaceâBeltrami operator
as a basis. This generalizes Fourier series to spaces of the type      L  2
( X )   {\displaystyle L^{2}(X)}  [{\displaystyle L^{2}(X)}], where     X
{\displaystyle X}  [X] is a Riemannian manifold. The Fourier series converges
in ways similar to the     [ &#x2212; &#x03C0; , &#x03C0; ]   {\displaystyle [-
\pi ,\pi ]}  [[-\pi ,\pi ]] case. A typical example is to take     X
{\displaystyle X}  [X] to be the sphere with the usual metric, in which case
the Fourier basis consists of spherical_harmonics.
**** Locally compact Abelian groups[edit] ****
Main article: Pontryagin_duality
The generalization to compact groups discussed above does not generalize to
noncompact, nonabelian_groups. However, there is a straightforward
generalization to Locally Compact Abelian (LCA) groups.
This generalizes the Fourier transform to      L  1   ( G )   {\displaystyle L^
{1}(G)}  [{\displaystyle L^{1}(G)}] or      L  2   ( G )   {\displaystyle L^{2}
(G)}  [{\displaystyle L^{2}(G)}], where     G   {\displaystyle G}  [G] is an
LCA group. If     G   {\displaystyle G}  [G] is compact, one also obtains a
Fourier series, which converges similarly to the     [ &#x2212; &#x03C0; ,
&#x03C0; ]   {\displaystyle [-\pi ,\pi ]}  [[-\pi ,\pi ]] case, but if     G
{\displaystyle G}  [G] is noncompact, one obtains instead a Fourier_integral.
This generalization yields the usual Fourier_transform when the underlying
locally compact Abelian group is      R    {\displaystyle \mathbb {R} }
[\mathbb {R} ].
***** Table of common Fourier series[edit] *****
Some common pairs of periodic functions and their Fourier Series coefficients
are shown in the table below. The following notation applies:
    *    f ( x )   {\displaystyle f(x)}  [f(x)] designates a periodic function
      defined on     0 < x &#x2264; T   {\displaystyle 0<x\leq T}  [
      {\displaystyle 0<x\leq T}].
    *     a  0   ,  a  n   ,  b  n     {\displaystyle a_{0},a_{n},b_{n}}  [
      {\displaystyle a_{0},a_{n},b_{n}}] designate the Fourier Series
      coefficients (sine-cosine form) of the periodic function     f
      {\displaystyle f}  [f] as defined in Eq.4.
                                                           Frequency domain
                                                           (sine-cosine
                                                           form)
                                                                     a  0
                                                           a  n
                                                           for&#xA0;  n
                                                           &#x2265; 1
                                                           b  n
                                                           for&#xA0;  n
                                                           &#x2265; 1
                                                           {\displaystyle
                                                           {\begin
Time domain                                                {aligned}&a_
    f ( x )              Plot                              {0}\\&a_{n}\quad  Remarks        Reference
{\displaystyle f(x)}  [f                                   {\text{for
(x)]                                                       }}n\geq 1\\&b_
                                                           {n}\quad {\text
                                                           {for }}n\geq
                                                           1\end{aligned}}}
                                                           [{\displaystyle
                                                           {\begin
                                                           {aligned}&a_
                                                           {0}\\&a_{n}\quad
                                                           {\text{for
                                                           }}n\geq 1\\&b_
                                                           {n}\quad {\text
                                                           {for }}n\geq
                                                           1\end{aligned}}}]
                                                                   a  0   =
                                                           4 A  &#x03C0;
                                                           a  n   =
                                                           {       &#x2212;
                                                           4 A  &#x03C0;
                                                           1  1 &#x2212;  n
                                                           2         n
                                                           &#xA0;even      0
                                                           n  &#xA0;odd
                                                           b  n   =   0
                                                           {\displaystyle
                                                           {\begin
                                                           {aligned}a_{0}=&
                                                           {\frac {4A}{\pi
   f ( x ) = A  |  sin                                     }}\\a_{n}=&
&#x2061;  (     2                                          {\begin{cases}
&#x03C0;  T   x  )   |                                     {\frac {-4A}{\pi
for&#xA0;  0 &#x2264; x                                    }}{\frac {1}{1-n^
< T   {\displaystyle f                                     {2}}}&\quad n
(x)=A\left|\sin \left(                                     {\text
{\frac {2\pi }           [PlotRectifiedSineSignal.svg]     { even}}\\0&\quad Full-wave      [16]:p.
{T}}x\right)\right|\quad                                   n{\text           rectified sine 193
{\text{for }}0\leq x<T}                                    { odd}}\end
[{\displaystyle f                                          {cases}}\\b_
(x)=A\left|\sin \left(                                     {n}=&0\\\end
{\frac {2\pi }                                             {aligned}}}  [
{T}}x\right)\right|\quad                                   {\displaystyle
{\text{for }}0\leq x<T}]                                   {\begin
                                                           {aligned}a_{0}=&
                                                           {\frac {4A}{\pi
                                                           }}\\a_{n}=&
                                                           {\begin{cases}
                                                           {\frac {-4A}{\pi
                                                           }}{\frac {1}{1-n^
                                                           {2}}}&\quad n
                                                           {\text
                                                           { even}}\\0&\quad
                                                           n{\text
                                                           { odd}}\end
                                                           {cases}}\\b_
                                                           {n}=&0\\\end
                                                           {aligned}}}]
                                                                   a  0   =
                                                           2 A  &#x03C0;
                                                           a  n   =
                                                           {       &#x2212;
                                                           2 A  &#x03C0;
                                                           1  1 &#x2212;  n
                                                           2         n
                                                           &#xA0;even      0
                                                           n  &#xA0;odd
                                                           b  n   =
                                                           {      A 2      n
                                                           = 1     0    n >
                                                           1
                                                           {\displaystyle
                                                           {\begin
                                                           {aligned}a_{0}=&
   f ( x ) =   {    A                                      {\frac {2A}{\pi
sin &#x2061;  (     2                                      }}\\a_{n}=&
&#x03C0;  T   x  )                                         {\begin{cases}
for&#xA0;  0 &#x2264; x                                    {\frac {-2A}{\pi
< T  /  2     0                                            }}{\frac {1}{1-n^
for&#xA0;  T  /  2                                         {2}}}&\quad n
&#x2264; x < T                                             {\text
{\displaystyle f(x)=                                       { even}}\\0&\quad
{\begin{cases}A\sin                                        n{\text
\left({\frac {2\pi }                                       { odd}}\end
{T}}x\right)&\quad                                         {cases}}\\b_{n}=& Half-wave      [16]:p.
{\text{for }}0\leq x<T/  [PlotHalfRectifiedSineSignal.svg] {\begin{cases}    rectified sine 193
2\\0&\quad {\text{for                                      {\frac {A}
}}T/2\leq x<T\\\end                                        {2}}&\quad
{cases}}}  [                                               n=1\\0&\quad
{\displaystyle f(x)=                                       n>1\end
{\begin{cases}A\sin                                        {cases}}\\\end
\left({\frac {2\pi }                                       {aligned}}}  [
{T}}x\right)&\quad                                         {\displaystyle
{\text{for }}0\leq x<T/                                    {\begin
2\\0&\quad {\text{for                                      {aligned}a_{0}=&
}}T/2\leq x<T\\\end                                        {\frac {2A}{\pi
{cases}}}]                                                 }}\\a_{n}=&
                                                           {\begin{cases}
                                                           {\frac {-2A}{\pi
                                                           }}{\frac {1}{1-n^
                                                           {2}}}&\quad n
                                                           {\text
                                                           { even}}\\0&\quad
                                                           n{\text
                                                           { odd}}\end
                                                           {cases}}\\b_{n}=&
                                                           {\begin{cases}
                                                           {\frac {A}
                                                           {2}}&\quad
                                                           n=1\\0&\quad
                                                           n>1\end
                                                           {cases}}\\\end
                                                           {aligned}}}]
                                                                   a  0   =
                                                           2 A D      a  n
                                                           =     A  n
                                                           &#x03C0;    sin
                                                           &#x2061;  (  2
                                                           &#x03C0; n D  )
                                                           b  n   =      2 A
                                                           n &#x03C0;
                                                           (  sin &#x2061;
   f ( x ) =   {    A                                      (  &#x03C0; n D
for&#xA0;  0 &#x2264; x                                    )   )   2
< D &#x22C5; T     0                                       {\displaystyle
for&#xA0;  D &#x22C5; T                                    {\begin
&#x2264; x < T                                             {aligned}a_
{\displaystyle f(x)=                                       {0}=&2AD\\a_{n}=&    0 &#x2264;
{\begin{cases}A&\quad                                      {\frac {A}{n\pi   D &#x2264; 1
{\text{for }}0\leq                                         }}\sin \left(2\pi {\displaystyle
x<D\cdot T\\0&\quad                                        nD\right)\\b_     0\leq D\leq 1}
{\text{for }}D\cdot      [PlotRectangleSignal.svg]         {n}=&{\frac {2A}  [
T\leq x<T\\\end{cases}}}                                   {n\pi }}\left     {\displaystyle
[{\displaystyle f(x)=                                      (\sin \left(\pi   0\leq D\leq
{\begin{cases}A&\quad                                      nD\right)\right)^ 1}]
{\text{for }}0\leq                                         {2}\\\end
x<D\cdot T\\0&\quad                                        {aligned}}}  [
{\text{for }}D\cdot                                        {\displaystyle
T\leq x<T\\\end                                            {\begin
{cases}}}]                                                 {aligned}a_
                                                           {0}=&2AD\\a_{n}=&
                                                           {\frac {A}{n\pi
                                                           }}\sin \left(2\pi
                                                           nD\right)\\b_
                                                           {n}=&{\frac {2A}
                                                           {n\pi }}\left
                                                           (\sin \left(\pi
                                                           nD\right)\right)^
                                                           {2}\\\end
                                                           {aligned}}}]
                                                                   a  0   =
                                                           A      a  n   =
                                                           0      b  n   =
                                                           &#x2212; A   n
                                                           &#x03C0;
                                                           {\displaystyle
   f ( x ) =    A x  T                                     {\begin
for&#xA0;  0 &#x2264; x                                    {aligned}a_
< T   {\displaystyle f                                     {0}=&A\\a_
(x)={\frac {Ax}{T}}\quad                                   {n}=&0\\b_{n}=&                  [16]:p.
{\text{for }}0\leq x<T}  [PlotSawtooth1Signal.svg]         {\frac {-A}{n\pi                 192
[{\displaystyle f(x)=                                      }}\\\end
{\frac {Ax}{T}}\quad                                       {aligned}}}  [
{\text{for }}0\leq x<T}]                                   {\displaystyle
                                                           {\begin
                                                           {aligned}a_
                                                           {0}=&A\\a_
                                                           {n}=&0\\b_{n}=&
                                                           {\frac {-A}{n\pi
                                                           }}\\\end
                                                           {aligned}}}]
                                                                   a  0   =
                                                           A      a  n   =
                                                           0      b  n   =
                                                           A  n &#x03C0;
                                                           {\displaystyle
   f ( x ) = A &#x2212;                                    {\begin
A x  T     for&#xA0;  0                                    {aligned}a_
&#x2264; x < T                                             {0}=&A\\a_
{\displaystyle f(x)=A-                                     {n}=&0\\b_{n}=&
{\frac {Ax}{T}}\quad     [PlotSawtooth2Signal.svg]         {\frac {A}{n\pi                  [16]:p.
{\text{for }}0\leq x<T}                                    }}\\\end                         192
[{\displaystyle f(x)=A-                                    {aligned}}}  [
{\frac {Ax}{T}}\quad                                       {\displaystyle
{\text{for }}0\leq x<T}]                                   {\begin
                                                           {aligned}a_
                                                           {0}=&A\\a_
                                                           {n}=&0\\b_{n}=&
                                                           {\frac {A}{n\pi
                                                           }}\\\end
                                                           {aligned}}}]
                                                                   a  0   =
                                                           2 A  3        a
                                                           n   =      4 A
                                                           &#x03C0;  2    n
                                                           2           b  n
   f ( x ) =    4 A   T                                    =   0
2       (  x &#x2212;                                      {\displaystyle
T 2    )   2                                               {\begin
for&#xA0;  0 &#x2264; x                                    {aligned}a_{0}=&
< T   {\displaystyle f                                     {\frac {2A}
(x)={\frac {4A}{T^                                         {3}}\\a_{n}=&
{2}}}\left(x-{\frac {T}  [PlotParabolaSignal.svg]          {\frac {4A}{\pi ^                [16]:p.
{2}}\right)^{2}\quad                                       {2}n^{2}}}\\b_                   193
{\text{for }}0\leq x<T}                                    {n}=&0\\\end
[{\displaystyle f(x)=                                      {aligned}}}  [
{\frac {4A}{T^{2}}}\left                                   {\displaystyle
(x-{\frac {T}                                              {\begin
{2}}\right)^{2}\quad                                       {aligned}a_{0}=&
{\text{for }}0\leq x<T}]                                   {\frac {2A}
                                                           {3}}\\a_{n}=&
                                                           {\frac {4A}{\pi ^
                                                           {2}n^{2}}}\\b_
                                                           {n}=&0\\\end
                                                           {aligned}}}]
***** Approximation and convergence of Fourier series[edit] *****
Main article: Convergence_of_Fourier_series
An important question for the theory as well as applications is that of
convergence. In particular, it is often necessary in applications to replace
the infinite series      &#x2211;  &#x2212; &#x221E;   &#x221E;
{\displaystyle \sum _{-\infty }^{\infty }}  [\sum_{-\infty}^\infty]  by a
finite one,
          f  N   ( x ) =  &#x2211;  n = &#x2212; N   N      f &#x005E;    ( n )
      e  i n x   .   {\displaystyle f_{N}(x)=\sum _{n=-N}^{N}{\hat {f}}(n)e^
      {inx}.}  [f_N(x) = \sum_{n=-N}^N \hat{f}(n) e^{inx}.]
This is called a partial sum. We would like to know, in which sense does      f
N   ( x )   {\displaystyle f_{N}(x)}  [{\displaystyle f_{N}(x)}] converge to
f ( x )   {\displaystyle f(x)}  [f(x)] as     N &#x2192; &#x221E;
{\displaystyle N\rightarrow \infty }  [N\rightarrow \infty ].
**** Least squares property[edit] ****
We say that     p   {\displaystyle p}  [p] is a trigonometric_polynomial of
degree     N   {\displaystyle N}  [N] when it is of the form
         p ( x ) =  &#x2211;  n = &#x2212; N   N    p  n    e  i n x   .
      {\displaystyle p(x)=\sum _{n=-N}^{N}p_{n}e^{inx}.}  [p(x)=\sum_{n=-N}^N
      p_n e^{inx}.]
Note that      f  N     {\displaystyle f_{N}}  [f_{N}] is a trigonometric
polynomial of degree     N   {\displaystyle N}  [N]. Parseval's_theorem implies
that
     Theorem. The trigonometric polynomial      f  N     {\displaystyle f_
     {N}}  [f_{N}] is the unique best trigonometric polynomial of degree
     N   {\displaystyle N}  [N] approximating     f ( x )   {\displaystyle
     f(x)}  [f(x)], in the sense that, for any trigonometric polynomial
     p &#x2260;  f  N     {\displaystyle p\neq f_{N}}  [{\displaystyle
     p\neq f_{N}}] of degree     N   {\displaystyle N}  [N], we have
              &#x2016;  f  N   &#x2212; f  &#x2016;  2   < &#x2016; p
           &#x2212; f  &#x2016;  2   ,   {\displaystyle \|f_{N}-f\|_
           {2}<\|p-f\|_{2},}  [\|f_N - f\|_2 < \|p - f\|_2,]
     where the Hilbert space norm is defined as:
              &#x2016; g  &#x2016;  2   =     1  2 &#x03C0;     &#x222B;
           &#x2212; &#x03C0;   &#x03C0;    |  g ( x )   |   2    d x   .
           {\displaystyle \|g\|_{2}={\sqrt {{1 \over 2\pi }\int _{-\pi }^
           {\pi }|g(x)|^{2}\,dx}}.}  [\| g \|_2 = \sqrt{{1 \over 2\pi}
           \int_{-\pi}^\pi |g(x)|^2 \, dx}.]
**** Convergence[edit] ****
See also: Gibbs_phenomenon
Because of the least squares property, and because of the completeness of the
Fourier basis, we obtain an elementary convergence result.
Theorem. If     f   {\displaystyle f}  [f] belongs to      L  2   (
[  &#x2212; &#x03C0; , &#x03C0;  ]  )   {\displaystyle L^{2}(\left[-\pi ,\pi
\right])}  [{\displaystyle L^{2}(\left[-\pi ,\pi \right])}], then      f
&#x221E;     {\displaystyle f_{\infty }}  [{\displaystyle f_{\infty }}]
converges to     f   {\displaystyle f}  [f] in      L  2   (  [  &#x2212;
&#x03C0; , &#x03C0;  ]  )   {\displaystyle L^{2}(\left[-\pi ,\pi \right])}  [
{\displaystyle L^{2}(\left[-\pi ,\pi \right])}], that is,      &#x2016;  f  N
&#x2212; f  &#x2016;  2     {\displaystyle \|f_{N}-f\|_{2}}  [\|f_N - f\|_2]
converges to 0 as     N &#x2192; &#x221E;   {\displaystyle N\rightarrow \infty
}  [N\rightarrow \infty ].
We have already mentioned that if     f   {\displaystyle f}  [f] is
continuously differentiable, then      ( i &#x22C5; n )    f &#x005E;    ( n )
{\displaystyle (i\cdot n){\hat {f}}(n)}  [(i\cdot n) \hat{f}(n)]  is the nth
Fourier coefficient of the derivative      f &#x2032;    {\displaystyle f'}
[f']. It follows, essentially from the CauchyâSchwarz_inequality, that      f
&#x221E;     {\displaystyle f_{\infty }}  [{\displaystyle f_{\infty }}] is
absolutely summable. The sum of this series is a continuous function, equal to
f   {\displaystyle f}  [f], since the Fourier series converges in the mean to
f   {\displaystyle f}  [f]:
Theorem. If     f &#x2208;  C  1   (  T  )   {\displaystyle f\in C^{1}(\mathbb
{T} )}  [f \in C^1(\mathbb{T})], then      f  &#x221E;     {\displaystyle f_
{\infty }}  [{\displaystyle f_{\infty }}] converges to     f   {\displaystyle
f}  [f] uniformly (and hence also pointwise.)
This result can be proven easily if     f   {\displaystyle f}  [f] is further
assumed to be      C  2     {\displaystyle C^{2}}  [C^{2}], since in that case
n  2      f &#x005E;    ( n )   {\displaystyle n^{2}{\hat {f}}(n)}  [n^2\hat{f}
(n)] tends to zero as     n &#x2192; &#x221E;   {\displaystyle n\rightarrow
\infty }  [n\rightarrow \infty ]. More generally, the Fourier series is
absolutely summable, thus converges uniformly to     f   {\displaystyle f}
[f], provided that     f   {\displaystyle f}  [f] satisfies a HÃ¶lder_condition
of order     &#x03B1; > 1  /  2   {\displaystyle \alpha >1/2}  [{\displaystyle
\alpha >1/2}]. In the absolutely summable case, the inequality      sup  x    |
f ( x ) &#x2212;  f  N   ( x )  |  &#x2264;  &#x2211;   |  n  |  > N    |     f
&#x005E;    ( n )  |    {\displaystyle \sup _{x}|f(x)-f_{N}(x)|\leq \sum _
{|n|>N}|{\hat {f}}(n)|}  [\sup_x |f(x) - f_N(x)| \le \sum_{|n| > N} |\hat{f}
(n)|]  proves uniform convergence.
Many other results concerning the convergence_of_Fourier_series are known,
ranging from the moderately simple result that the series converges at     x
{\displaystyle x}  [x] if     f   {\displaystyle f}  [f] is differentiable at
x   {\displaystyle x}  [x], to Lennart_Carleson's much more sophisticated
result that the Fourier series of an      L  2     {\displaystyle L^{2}}  [L^
{2}] function actually converges almost_everywhere.
These theorems, and informal variations of them that don't specify the
convergence conditions, are sometimes referred to generically as "Fourier's
theorem" or "the Fourier theorem".[17][18][19][20]
**** Divergence[edit] ****
Since Fourier series have such good convergence properties, many are often
surprised by some of the negative results. For example, the Fourier series of a
continuous T-periodic function need not converge pointwise. The uniform
boundedness_principle yields a simple non-constructive proof of this fact.
In 1922, Andrey_Kolmogorov published an article titled Une sÃ©rie de Fourier-
Lebesgue divergente presque partout in which he gave an example of a Lebesgue-
integrable function whose Fourier series diverges almost everywhere. He later
constructed an example of an integrable function whose Fourier series diverges
everywhere (Katznelson_1976).
***** See also[edit] *****
    * ATS_theorem
    * Dirichlet_kernel
    * Discrete_Fourier_transform
    * Fast_Fourier_transform
    * FejÃ©r's_theorem
    * Fourier_analysis
    * Fourier_sine_and_cosine_series
    * Fourier_transform
    * Gibbs_phenomenon
    * Laurent_series â the substitution q = eix transforms a Fourier series
      into a Laurent series, or conversely. This is used in the q-series
      expansion of the j-invariant.
    * Multidimensional_transform
    * Spectral_theory
    * SturmâLiouville_theory
***** Notes[edit] *****
   1. ^ These three did some important_early_work_on_the_wave_equation,
      especially D'Alembert. Euler's work in this area was mostly
      comtemporaneous/_in_collaboration_with_Bernoulli, although the latter
      made some independent contributions to the theory of waves and
      vibrations. (See Fetter_&_Walecka_2003, pp. 209-210).
   2. ^ Since the integral defining the Fourier transform of a periodic
      function is not convergent, it is necessary to view the periodic function
      and its transform as distributions. In this sense       F    {  e  i    2
      &#x03C0; n x  P     }    {\displaystyle {\mathcal {F}}\left\{e^{i{\frac
      {2\pi nx}{P}}}\right\}}  [\mathcal{F} \left\{ e^{i \frac{2\pi nx}{P} }
      \right\}] is a Dirac_delta_function, which is an example of a
      distribution.
   3. ^ These words are not strictly Fourier's. Whilst the cited article does
      list the author as Fourier, a footnote indicates that the article was
      actually written by Poisson (that it was not written by Fourier is also
      clear from the consistent use of the third person to refer to him) and
      that it is, "for reasons of historical interest", presented as though it
      were Fourier's original memoire.
   4. ^ The scale factor is always equal to the period, 2Ï in this case.
***** References[edit] *****
   1. ^"Fourier". Dictionary.com Unabridged. Random_House.
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
   3. ^Stillwell,_John (2013). "Logic and the philosophy of mathematics in the
      nineteenth century". In Ten, C. L. (ed.). Routledge_History_of
      Philosophy. Volume VII: The Nineteenth Century. Routledge. p. 204.
      ISBN 978-1-134-92880-4.
   4. ^Cajori,_Florian (1893). A_History_of_Mathematics. Macmillan. p. 283.
   5. ^Lejeune-Dirichlet,_Peter_Gustav (1829). "Sur_la_convergence_des_sÃ©ries
      trigonomÃ©triques_qui_servent_Ã _reprÃ©senter_une_fonction_arbitraire
      entre_des_limites_donnÃ©es" [On the convergence of trigonometric series
      which serve to represent an arbitrary function between two given limits].
      Journal_fÃ¼r_die_reine_und_angewandte_Mathematik (in French). 4:
      157â169. arXiv:0806.1294.
   6. ^"Ueber_die_Darstellbarkeit_einer_Function_durch_eine_trigonometrische
      Reihe" [About the representability of a function by a trigonometric
      series]. Habilitationsschrift, GÃ¶ttingen; 1854. Abhandlungen der
      KÃ¶niglichen_Gesellschaft_der_Wissenschaften_zu_GÃ¶ttingen, vol. 13,
      1867. Published posthumously for Riemann by Richard_Dedekind(in German).
      Archived from the original on 20 May 2008. Retrieved 19 May 2008.
   7. ^Mascre, D.; Riemann, Bernhard (1867), "Posthumous Thesis on the
      Representation of Functions by Trigonometric Series", in Grattan-
      Guinness, Ivor (ed.), Landmark_Writings_in_Western_Mathematics
      1640â1940, Elsevier (published 2005), p. 49
   8. ^Remmert, Reinhold (1991). Theory_of_Complex_Functions:_Readings_in
      Mathematics. Springer. p. 29.
   9. ^Nerlove, Marc; Grether, David M.; Carvalho, Jose L. (1995). Analysis of
      Economic Time Series. Economic Theory, Econometrics, and Mathematical
      Economics. Elsevier. ISBN 0-12-515751-7.
  10. ^Flugge, Wilhelm (1957). Statik_und_Dynamik_der_Schalen [Statics and
      dynamics of Shells] (in German). Berlin: Springer-Verlag.
  11. ^Dorf, Richard C.; Tallarida, Ronald J. (1993-07-15). Pocket Book of
      Electrical Engineering Formulas (1 ed.). Boca Raton,FL: CRC Press.
      pp. 171â174. ISBN 0849344735.
  12. ^Georgi P. Tolstov (1976). Fourier_Series. Courier-Dover. ISBN 0-486-
      63317-9.
  13. ^"Gallica_â_Fourier,_Jean-Baptiste-Joseph_(1768â1830)._Oeuvres_de
      Fourier._1888,_pp._218â219" (in French). Gallica.bnf.fr. 2007-10-15.
      Retrieved 2014-08-08.
  14. ^ a b c dShmaliy, Y.S. (2007). Continuous-Time Signals. Springer.
      ISBN 1402062710.
  15. ^Proakis, John G.; Manolakis, Dimitris G. (1996). Digital_Signal
      Processing:_Principles,_Algorithms,_and_Applications (3rd ed.). Prentice
      Hall. p. 291. ISBN 978-0-13-373762-2.
  16. ^"Characterizations_of_a_linear_subspace_associated_with_Fourier_series".
      MathOverflow. 2010-11-19. Retrieved 2014-08-08.
  17. ^ a b c d ePapula, Lothar (2009). Mathematische Formelsammlung: fÃ¼r
      Ingenieure und Naturwissenschaftler [Mathematical Functions for Engineers
      and Physicists] (in German). Vieweg+Teubner Verlag. ISBN 3834807575.
  18. ^Siebert, William McC. (1985). Circuits,_signals,_and_systems. MIT Press.
      p. 402. ISBN 978-0-262-19229-3.
  19. ^Marton, L.; Marton, Claire (1990). Advances_in_Electronics_and_Electron
      Physics. Academic Press. p. 369. ISBN 978-0-12-014650-5.
  20. ^Kuzmany, Hans (1998). Solid-state_spectroscopy. Springer. p. 14.
      ISBN 978-3-540-63913-8.
  21. ^Pribram, Karl H.; Yasue, Kunio; Jibu, Mari (1991). Brain_and_perception.
      Lawrence Erlbaum Associates. p. 26. ISBN 978-0-89859-995-4.
**** Further reading[edit] ****
    * William E. Boyce; Richard C. DiPrima (2005). Elementary Differential
      Equations and Boundary Value Problems (8th ed.). New Jersey: John Wiley &
      Sons, Inc. ISBN 0-471-43338-1.
Joseph Fourier, translated by Alexander Freeman (2003). The Analytical Theory
of Heat. Dover Publications. ISBN 0-486-49531-0.
 2003 unabridged republication of the 1878 English translation by Alexander
Freeman of Fourier's work ThÃ©orie Analytique de la Chaleur, originally
published in 1822.
Enrique A. Gonzalez-Velasco (1992). "Connections in Mathematical Analysis: The
Case of Fourier Series". American Mathematical Monthly. 99 (5): 427â441. doi:
10.2307/2325087. JSTOR 2325087.
Fetter, Alexander L.; Walecka, John Dirk (2003). Theoretical_Mechanics_of
Particles_and_Continua. Courier. ISBN 978-0-486-43261-8.
Katznelson, Yitzhak (1976). "An introduction to harmonic analysis" (Second
corrected ed.). New York: Dover Publications, Inc. ISBN 0-486-63331-4.
Felix_Klein, Development of mathematics in the 19th century. Mathsci Press
Brookline, Mass, 1979. Translated by M. Ackerman from Vorlesungen Ã¼ber die
Entwicklung der Mathematik im 19 Jahrhundert, Springer, Berlin, 1928.
Walter_Rudin (1976). Principles of mathematical analysis (3rd ed.). New York:
McGraw-Hill, Inc. ISBN 0-07-054235-X.
A._Zygmund (2002). Trigonometric series (third ed.). Cambridge: Cambridge
University Press. ISBN 0-521-89053-5.
 The first edition was published in 1935.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Fourier_series", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Weisstein,_Eric_W. "Fourier_Series". MathWorld.
Joseph_Fourier_â_A_site_on_Fourier's_life_which_was_used_for_the_historical
section_of_this_article at the Wayback_Machine (archived December 5, 2001)
This article incorporates material from example_of_Fourier_series on
PlanetMath, which is licensed under the Creative_Commons_Attribution/Share-
Alike_License.
Authority_control [Edit_this_at_Wikidata]     * NDL: 00562088

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Fourier_series&oldid=907731548"
Categories:
    * Fourier_series
    * Joseph_Fourier
Hidden categories:
    * CS1:_long_volume_value
    * CS1_French-language_sources_(fr)
    * CS1_German-language_sources_(de)
    * Articles_with_short_description
    * Articles_with_attributed_pull_quotes
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_November_2012
    * Webarchive_template_wayback_links
    * Wikipedia_articles_incorporating_text_from_PlanetMath
    * Wikipedia_articles_with_NDL_identifiers
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
    * Wikiversity
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * ÐÐ°ÑÒ¡Ð¾ÑÑÑÐ°
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * Ð§ÓÐ²Ð°ÑÐ»Ð°
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Latina
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Malti
    * Bahasa_Melayu
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * à·à·à¶à·à¶½
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Basa_Sunda
    * Suomi
    * Svenska
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 24 July 2019, at 22:04 (UTC).
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
