The following text has been accessed from https://en.wikipedia.org/wiki/Dirac_delta_function at Thu Aug 8 23:21:32 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















[This_is_a_good_article._Follow_the_link_for_more_information.]
****** Dirac delta function ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
pseudo-function Î´ such that an integral of Î´(x-c)f(x) always takes the value
of f(c)
"Delta function" redirects here. For other uses, see Delta_function_
(disambiguation).
Schematic representation of the Dirac delta function by a line surmounted by an
arrow. The height of the arrow is usually meant to specify the value of any
multiplicative constant, which will give the area under the function. The other
convention is to write the area next to the arrowhead.
The Dirac delta function as the limit (in the sense of distributions) of the
sequence of zero-centered normal_distributions      &#x03B4;  a   ( x ) =   1
| a |    &#x03C0;        e   &#x2212; ( x  /  a  )  2       {\displaystyle
\delta _{a}(x)={\frac {1}{\left|a\right|{\sqrt {\pi }}}}\mathrm {e} ^{-(x/a)^
{2}}}  [{\displaystyle \delta _{a}(x)={\frac {1}{\left|a\right|{\sqrt {\pi
}}}}\mathrm {e} ^{-(x/a)^{2}}}] as     a &#x2192; 0   {\displaystyle
a\rightarrow 0}  [{\displaystyle a\rightarrow 0}].
In mathematics, the Dirac delta function (Î´ function) is a generalized
function or distribution introduced by the physicist Paul_Dirac. It is used to
model the density of an idealized point_mass or point_charge as a function
equal to zero everywhere except for zero and whose integral over the entire
real line is equal to one.[1][2][3] As there is no function that has these
properties, the computations made by the theoretical physicists appeared to
mathematicians as nonsense until the introduction of distributions by Laurent
Schwartz to formalize and validate the computations. As a distribution, the
Dirac delta function is a linear_functional that maps every function to its
value at zero.[4][5] The Kronecker_delta function, which is usually defined on
a discrete domain and takes values 0 and 1, is a discrete analog of the Dirac
delta function.
In engineering and signal_processing, the delta function, also known as the
unit impulse symbol,[6] may be regarded through its Laplace_transform, as
coming from the boundary values of a complex_analytic function of a complex
variable. The formal rules obeyed by this function are part of the operational
calculus, a standard tool kit of physics and engineering. In many applications,
the Dirac delta is regarded as a kind of limit (a weak_limit) of a sequence of
functions having a tall spike at the origin (in theory of distributions, this
is a true limit). The approximating functions of the sequence are thus
"approximate" or "nascent" delta functions.
⁰
***** Contents *****
    * 1_Motivation_and_overview
    * 2_History
    * 3_Definitions
          o 3.1_As_a_measure
          o 3.2_As_a_distribution
          o 3.3_Generalizations
    * 4_Properties
          o 4.1_Scaling_and_symmetry
          o 4.2_Algebraic_properties
          o 4.3_Translation
          o 4.4_Composition_with_a_function
          o 4.5_Properties_in_n_dimensions
    * 5_Fourier_transform
    * 6_Distributional_derivatives
          o 6.1_Higher_dimensions
    * 7_Representations_of_the_delta_function
          o 7.1_Approximations_to_the_identity
          o 7.2_Probabilistic_considerations
          o 7.3_Semigroups
          o 7.4_Oscillatory_integrals
          o 7.5_Plane_wave_decomposition
          o 7.6_Fourier_kernels
          o 7.7_Hilbert_space_theory
                # 7.7.1_Spaces_of_holomorphic_functions
                # 7.7.2_Resolutions_of_the_identity
          o 7.8_Infinitesimal_delta_functions
    * 8_Dirac_comb
    * 9_SokhotskiâPlemelj_theorem
    * 10_Relationship_to_the_Kronecker_delta
    * 11_Applications
          o 11.1_Probability_theory
          o 11.2_Quantum_mechanics
          o 11.3_Structural_mechanics
    * 12_See_also
    * 13_Notes
    * 14_References
    * 15_External_links
***** Motivation and overview[edit] *****
The graph of the delta function is usually thought of as following the whole x-
axis and the positive y-axis. The Dirac delta is used to model a tall narrow
spike function (an impulse), and other similar abstractions such as a point
charge, point_mass or electron point. For example, to calculate the dynamics of
a billiard_ball being struck, one can approximate the force of the impact by a
delta function. In doing so, one not only simplifies the equations, but one
also is able to calculate the motion of the ball by only considering the total
impulse of the collision without a detailed model of all of the elastic energy
transfer at subatomic levels (for instance).
To be specific, suppose that a billiard ball is at rest. At time     t = 0
{\displaystyle t=0}  [t=0] it is struck by another ball, imparting it with a
momentum P, in      kg m   /   s    {\displaystyle {\text{kg m}}/{\text{s}}}  [
{\displaystyle {\text{kg m}}/{\text{s}}}]. The exchange of momentum is not
actually instantaneous, being mediated by elastic processes at the molecular
and subatomic level, but for practical purposes it is convenient to consider
that energy transfer as effectively instantaneous. The force therefore is     P
&#x03B4; ( t )   {\displaystyle P\delta (t)}  [{\displaystyle P\delta (t)}].
(The units of     &#x03B4; ( t )   {\displaystyle \delta (t)}  [\delta (t)] are
s  &#x2212; 1     {\displaystyle s^{-1}}  [s^{-1}].)
To model this situation more rigorously, suppose that the force instead is
uniformly distributed over a small time interval     &#x0394; t
{\displaystyle \Delta t}  [\Delta t]. That is,
          F  &#x0394; t   ( t ) =   {    P  /  &#x0394; t   0 < t < &#x0394; t
      ,     0    otherwise  .         {\displaystyle F_{\Delta t}(t)={\begin
      {cases}P/\Delta t&0<t<\Delta t,\\0&{\text{otherwise}}.\end{cases}}}  [
      {\displaystyle F_{\Delta t}(t)={\begin{cases}P/\Delta t&0<t<\Delta t,\\0&
      {\text{otherwise}}.\end{cases}}}]
Then the momentum at any time t is found by integration:
         p ( t ) =  &#x222B;  0   t    F  &#x0394; t   ( &#x03C4; )  d &#x03C4;
      =   {    P   t > &#x0394; t     P t  /  &#x0394; t   0 < t < &#x0394; t
      0    otherwise.          {\displaystyle p(t)=\int _{0}^{t}F_{\Delta t}
      (\tau )\,d\tau ={\begin{cases}P&t>\Delta t\\Pt/\Delta t&0<t<\Delta t\\0&
      {\text{otherwise.}}\end{cases}}}  [{\displaystyle p(t)=\int _{0}^{t}F_
      {\Delta t}(\tau )\,d\tau ={\begin{cases}P&t>\Delta t\\Pt/\Delta
      t&0<t<\Delta t\\0&{\text{otherwise.}}\end{cases}}}]
Now, the model situation of an instantaneous transfer of momentum requires
taking the limit as     &#x0394; t &#x2192; 0   {\displaystyle \Delta t\to 0}
[{\displaystyle \Delta t\to 0}], giving
         p ( t ) =   {    P   t > 0     0   t &#x2264; 0.
      {\displaystyle p(t)={\begin{cases}P&t>0\\0&t\leq 0.\end{cases}}}  [
      {\displaystyle p(t)={\begin{cases}P&t>0\\0&t\leq 0.\end{cases}}}]
Here the functions      F  &#x0394; t     {\displaystyle F_{\Delta t}}  [
{\displaystyle F_{\Delta t}}] are thought of as useful approximations to the
idea of instantaneous transfer of momentum.
The delta function allows us to construct an idealized limit of these
approximations. Unfortunately, the actual limit of the functions (in the sense
of ordinary calculus)      lim  &#x0394; t &#x2192; 0    F  &#x0394; t
{\displaystyle \lim _{\Delta t\to 0}F_{\Delta t}}  [{\displaystyle \lim _
{\Delta t\to 0}F_{\Delta t}}] is zero everywhere but a single point, where it
is infinite. To make proper sense of the delta function, we should instead
insist that the property
          &#x222B;  &#x2212; &#x221E;   &#x221E;    F  &#x0394; t   ( t )  d t
      = P ,   {\displaystyle \int _{-\infty }^{\infty }F_{\Delta t}(t)\,dt=P,}
      [{\displaystyle \int _{-\infty }^{\infty }F_{\Delta t}(t)\,dt=P,}]
which holds for all     &#x0394; t > 0   {\displaystyle \Delta t>0}  [\Delta
t>0], should continue to hold in the limit. So, in the equation     F ( t ) = P
&#x03B4; ( t ) =  lim  &#x0394; t &#x2192; 0    F  &#x0394; t   ( t )
{\displaystyle F(t)=P\delta (t)=\lim _{\Delta t\to 0}F_{\Delta t}(t)}  [
{\displaystyle F(t)=P\delta (t)=\lim _{\Delta t\to 0}F_{\Delta t}(t)}], it is
understood that the limit is always taken outside the integral.
In applied mathematics, as we have done here, the delta function is often
manipulated as a kind of limit (a weak_limit) of a sequence of functions, each
member of which has a tall spike at the origin: for example, a sequence of
Gaussian_distributions centered at the origin with variance tending to zero.
Despite its name, the delta function is not truly a function, at least not a
usual one with range in real_numbers. For example, the objects f(x) = Î´(x) and
g(x) = 0 are equal everywhere except at x = 0 yet have integrals that are
different. According to Lebesgue_integration_theory, if f and g are functions
such that f = g almost_everywhere, then f is integrable if_and_only_if g is
integrable and the integrals of f and g are identical. A rigorous approach to
regarding the Dirac delta function as a mathematical_object in its own right
requires measure_theory or the theory of distributions.
***** History[edit] *****
Joseph_Fourier presented what is now called the Fourier_integral_theorem in his
treatise ThÃ©orie analytique de la chaleur in the form:[7]
         f ( x ) =   1  2 &#x03C0;     &#x222B;  &#x2212; &#x221E;   &#x221E;
      &#xA0; &#xA0; d &#x03B1;  f ( &#x03B1; ) &#xA0;  &#x222B;  &#x2212;
      &#x221E;   &#x221E;   d p &#xA0; cos &#x2061; ( p x &#x2212; p &#x03B1; )
      &#xA0; ,   {\displaystyle f(x)={\frac {1}{2\pi }}\int _{-\infty }^{\infty
      }\ \ d\alpha \,f(\alpha )\ \int _{-\infty }^{\infty }dp\ \cos(px-p\alpha
      )\ ,}  [{\displaystyle f(x)={\frac {1}{2\pi }}\int _{-\infty }^{\infty }\
      \ d\alpha \,f(\alpha )\ \int _{-\infty }^{\infty }dp\ \cos(px-p\alpha )\
      ,}]
which is tantamount to the introduction of the Î´-function in the form:[8]
         &#x03B4; ( x &#x2212; &#x03B1; ) =   1  2 &#x03C0;     &#x222B;
      &#x2212; &#x221E;   &#x221E;   d p &#xA0; cos &#x2061; ( p x &#x2212; p
      &#x03B1; ) &#xA0; .   {\displaystyle \delta (x-\alpha )={\frac {1}{2\pi
      }}\int _{-\infty }^{\infty }dp\ \cos(px-p\alpha )\ .}  [\delta (x-\alpha
      )={\frac {1}{2\pi }}\int _{-\infty }^{\infty }dp\ \cos(px-p\alpha )\ .]
Later, Augustin_Cauchy expressed the theorem using exponentials:[9][10]
         f ( x ) =   1  2 &#x03C0;     &#x222B;  &#x2212; &#x221E;   &#x221E;
      &#xA0;  e  i p x    (   &#x222B;  &#x2212; &#x221E;   &#x221E;    e
      &#x2212; i p &#x03B1;   f ( &#x03B1; ) &#xA0; d &#x03B1;  )  &#xA0; d p .
      {\displaystyle f(x)={\frac {1}{2\pi }}\int _{-\infty }^{\infty }\ e^
      {ipx}\left(\int _{-\infty }^{\infty }e^{-ip\alpha }f(\alpha )\ d\alpha
      \right)\ dp.}  [f(x)={\frac {1}{2\pi }}\int _{-\infty }^{\infty }\ e^
      {ipx}\left(\int _{-\infty }^{\infty }e^{-ip\alpha }f(\alpha )\ d\alpha
      \right)\ dp.]
Cauchy pointed out that in some circumstances the order of integration in this
result is significant (contrast Fubini's_theorem).[11][12]
As justified using the theory_of_distributions, the Cauchy equation can be
rearranged to resemble Fourier's original formulation and expose the Î´-
function as
             f ( x )    =   1  2 &#x03C0;     &#x222B;  &#x2212; &#x221E;
      &#x221E;    e  i p x    (   &#x222B;  &#x2212; &#x221E;   &#x221E;    e
      &#x2212; i p &#x03B1;   f ( &#x03B1; ) &#xA0; d &#x03B1;  )  &#xA0; d p
      =   1  2 &#x03C0;     &#x222B;  &#x2212; &#x221E;   &#x221E;
      (   &#x222B;  &#x2212; &#x221E;   &#x221E;    e  i p x    e  &#x2212; i p
      &#x03B1;   &#xA0; d p  )  f ( &#x03B1; ) &#xA0; d &#x03B1; =  &#x222B;
      &#x2212; &#x221E;   &#x221E;   &#x03B4; ( x &#x2212; &#x03B1; ) f
      ( &#x03B1; ) &#xA0; d &#x03B1; ,       {\displaystyle {\begin{aligned}f
      (x)&={\frac {1}{2\pi }}\int _{-\infty }^{\infty }e^{ipx}\left(\int _{-
      \infty }^{\infty }e^{-ip\alpha }f(\alpha )\ d\alpha \right)\ dp\\[4pt]&=
      {\frac {1}{2\pi }}\int _{-\infty }^{\infty }\left(\int _{-\infty }^
      {\infty }e^{ipx}e^{-ip\alpha }\ dp\right)f(\alpha )\ d\alpha =\int _{-
      \infty }^{\infty }\delta (x-\alpha )f(\alpha )\ d\alpha ,\end{aligned}}}
      [{\displaystyle {\begin{aligned}f(x)&={\frac {1}{2\pi }}\int _{-\infty }^
      {\infty }e^{ipx}\left(\int _{-\infty }^{\infty }e^{-ip\alpha }f(\alpha )\
      d\alpha \right)\ dp\\[4pt]&={\frac {1}{2\pi }}\int _{-\infty }^{\infty
      }\left(\int _{-\infty }^{\infty }e^{ipx}e^{-ip\alpha }\ dp\right)f(\alpha
      )\ d\alpha =\int _{-\infty }^{\infty }\delta (x-\alpha )f(\alpha )\
      d\alpha ,\end{aligned}}}]
where the Î´-function is expressed as
         &#x03B4; ( x &#x2212; &#x03B1; ) =   1  2 &#x03C0;     &#x222B;
      &#x2212; &#x221E;   &#x221E;    e  i p ( x &#x2212; &#x03B1; )   &#xA0; d
      p &#xA0; .   {\displaystyle \delta (x-\alpha )={\frac {1}{2\pi }}\int _{-
      \infty }^{\infty }e^{ip(x-\alpha )}\ dp\ .}  [\delta (x-\alpha )={\frac
      {1}{2\pi }}\int _{-\infty }^{\infty }e^{ip(x-\alpha )}\ dp\ .]
A rigorous interpretation of the exponential form and the various limitations
upon the function f necessary for its application extended over several
centuries. The problems with a classical interpretation are explained as
follows:[13]
      The greatest drawback of the classical Fourier transformation is a rather
      narrow class of functions (originals) for which it can be effectively
      computed. Namely, it is necessary that these functions decrease
      sufficiently_rapidly to zero (in the neighborhood of infinity) in order
      to ensure the existence of the Fourier integral. For example, the Fourier
      transform of such simple functions as polynomials does not exist in the
      classical sense. The extension of the classical Fourier transformation to
      distributions considerably enlarged the class of functions that could be
      transformed and this removed many obstacles.
Further developments included generalization of the Fourier integral,
"beginning with Plancherel's pathbreaking L2-theory (1910), continuing with
Wiener's and Bochner's works (around 1930) and culminating with the
amalgamation into L._Schwartz's theory of distributions (1945) ...",[14] and
leading to the formal development of the Dirac delta function.
An infinitesimal formula for an infinitely tall, unit impulse delta function
(infinitesimal version of Cauchy_distribution) explicitly appears in an 1827
text of Augustin_Louis_Cauchy.[15] SimÃ©on_Denis_Poisson considered the issue
in connection with the study of wave propagation as did Gustav_Kirchhoff
somewhat later. Kirchhoff and Hermann_von_Helmholtz also introduced the unit
impulse as a limit of Gaussians, which also corresponded to Lord_Kelvin's
notion of a point heat source. At the end of the 19th century, Oliver_Heaviside
used formal Fourier_series to manipulate the unit impulse.[16] The Dirac delta
function as such was introduced as a "convenient notation" by Paul_Dirac in his
influential 1930 book The_Principles_of_Quantum_Mechanics.[17] He called it the
"delta function" since he used it as a continuous analogue of the discrete
Kronecker_delta.
***** Definitions[edit] *****
The Dirac delta can be loosely thought of as a function on the real line which
is zero everywhere except at the origin, where it is infinite,
         &#x03B4; ( x ) =   {    + &#x221E; ,   x = 0     0 ,   x &#x2260; 0
      {\displaystyle \delta (x)={\begin{cases}+\infty ,&x=0\\0,&x\neq 0\end
      {cases}}}  [\delta (x)={\begin{cases}+\infty ,&x=0\\0,&x\neq 0\end
      {cases}}]
and which is also constrained to satisfy the identity
          &#x222B;  &#x2212; &#x221E;   &#x221E;   &#x03B4; ( x )  d x = 1.
      {\displaystyle \int _{-\infty }^{\infty }\delta (x)\,dx=1.}  [\int _{-
      \infty }^{\infty }\delta (x)\,dx=1.][18]
This is merely a heuristic characterization. The Dirac delta is not a function
in the traditional sense as no function defined on the real numbers has these
properties.[17] The Dirac delta function can be rigorously defined either as a
distribution or as a measure.
**** As a measure[edit] ****
One way to rigorously capture the notion of the Dirac delta function is to
define a measure, which accepts a subset A of the real line R as an argument,
and returns Î´(A) = 1 if 0 â A, and Î´(A) = 0 otherwise.[19] If the delta
function is conceptualized as modeling an idealized point mass at 0, then Î´(A)
represents the mass contained in the set A. One may then define the integral
against Î´ as the integral of a function against this mass distribution.
Formally, the Lebesgue_integral provides the necessary analytic device. The
Lebesgue integral with respect to the measure Î´ satisfies
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x )  &#x03B4; { d x } =
      f ( 0 )   {\displaystyle \int _{-\infty }^{\infty }f(x)\,\delta \{dx\}=f
      (0)}  [\int _{-\infty }^{\infty }f(x)\,\delta \{dx\}=f(0)]
for all continuous compactly supported functions f. The measure Î´ is not
absolutely_continuous with respect to the Lebesgue_measure â in fact, it is a
singular_measure. Consequently, the delta measure has no RadonâNikodym
derivative â no true function for which the property
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x ) &#x03B4; ( x )  d x
      = f ( 0 )   {\displaystyle \int _{-\infty }^{\infty }f(x)\delta (x)\,dx=f
      (0)}  [\int _{-\infty }^{\infty }f(x)\delta (x)\,dx=f(0)]
holds.[20] As a result, the latter notation is a convenient abuse_of_notation,
and not a standard (Riemann or Lebesgue) integral.
As a probability_measure on R, the delta measure is characterized by its
cumulative_distribution_function, which is the unit_step_function[21]
         H ( x ) =   {    1    if&#xA0;  x &#x2265; 0     0    if&#xA0;  x < 0.
      {\displaystyle H(x)={\begin{cases}1&{\text{if }}x\geq 0\\0&{\text{if
      }}x<0.\end{cases}}}  [H(x)={\begin{cases}1&{\text{if }}x\geq 0\\0&{\text
      {if }}x<0.\end{cases}}]
This means that H(x) is the integral of the cumulative indicator_function 1
(ââ, x] with respect to the measure Î´; to wit,
         H ( x ) =  &#x222B;   R      1   ( &#x2212; &#x221E; , x ]   ( t )
      &#x03B4; { d t } = &#x03B4; ( &#x2212; &#x221E; , x ] .   {\displaystyle
      H(x)=\int _{\mathbf {R} }\mathbf {1} _{(-\infty ,x]}(t)\,\delta \
      {dt\}=\delta (-\infty ,x].}  [H(x)=\int _{\mathbf {R} }\mathbf {1} _{(-
      \infty ,x]}(t)\,\delta \{dt\}=\delta (-\infty ,x].]
Thus in particular the integral of the delta function against a continuous
function can be properly understood as a RiemannâStieltjes_integral:[22]
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x ) &#x03B4; { d x } =
      &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x )  d H ( x ) .
      {\displaystyle \int _{-\infty }^{\infty }f(x)\delta \{dx\}=\int _{-\infty
      }^{\infty }f(x)\,dH(x).}  [\int _{-\infty }^{\infty }f(x)\delta \
      {dx\}=\int _{-\infty }^{\infty }f(x)\,dH(x).]
All higher moments of Î´ are zero. In particular, characteristic_function and
moment_generating_function are both equal to one.
**** As a distribution[edit] ****
In the theory of distributions, a generalized function is considered not a
function in itself but only in relation to how it affects other functions when
"integrated" against them. In keeping with this philosophy, to define the delta
function properly, it is enough to say what the "integral" of the delta
function is against a sufficiently "good" test function Ï. Test functions are
also known as bump_functions. If the delta function is already understood as a
measure, then the Lebesgue integral of a test function against that measure
supplies the necessary integral.
A typical space of test functions consists of all smooth_functions on R with
compact_support that have as many derivatives as required. As a distribution,
the Dirac delta is a linear_functional on the space of test functions and is
defined by[23]
          &#x03B4; [ &#x03C6; ] = &#x03C6; ( 0 )   {\displaystyle        
      \delta [\varphi ]=\varphi (0)}  [{\displaystyle \delta [\varphi      (1)
      ]=\varphi (0)}]
for every test function    &#x03C6;   {\displaystyle \varphi }  [\varphi ].
For Î´ to be properly a distribution, it must be continuous in a suitable
topology on the space of test functions. In general, for a linear functional S
on the space of test functions to define a distribution, it is necessary and
sufficient that, for every positive integer N there is an integer MN and a
constant CN such that for every test function Ï, one has the inequality[24]
          |  S [ &#x03C6; ]  |  &#x2264;  C  N    &#x2211;  k = 0    M  N
      sup  x &#x2208; [ &#x2212; N , N ]    |   &#x03C6;  ( k )   ( x )  |  .
      {\displaystyle |S[\varphi ]|\leq C_{N}\sum _{k=0}^{M_{N}}\sup _{x\in [-
      N,N]}|\varphi ^{(k)}(x)|.}  [|S[\varphi ]|\leq C_{N}\sum _{k=0}^{M_
      {N}}\sup _{x\in [-N,N]}|\varphi ^{(k)}(x)|.]
With the Î´ distribution, one has such an inequality (with CN = 1) with MN = 0
for all N. Thus Î´ is a distribution of order zero. It is, furthermore, a
distribution with compact support (the support being {0}).
The delta distribution can also be defined in a number of equivalent ways. For
instance, it is the distributional_derivative of the Heaviside_step_function.
This means that, for every test function Ï, one has
         &#x03B4; [ &#x03C6; ] = &#x2212;  &#x222B;  &#x2212; &#x221E;
      &#x221E;    &#x03C6; &#x2032;  ( x ) H ( x )  d x .   {\displaystyle
      \delta [\varphi ]=-\int _{-\infty }^{\infty }\varphi '(x)H(x)\,dx.}
      [\delta [\varphi ]=-\int _{-\infty }^{\infty }\varphi '(x)H(x)\,dx.]
Intuitively, if integration_by_parts were permitted, then the latter integral
should simplify to
          &#x222B;  &#x2212; &#x221E;   &#x221E;   &#x03C6; ( x )  H &#x2032;
      ( x )  d x =  &#x222B;  &#x2212; &#x221E;   &#x221E;   &#x03C6; ( x )
      &#x03B4; ( x )  d x ,   {\displaystyle \int _{-\infty }^{\infty }\varphi
      (x)H'(x)\,dx=\int _{-\infty }^{\infty }\varphi (x)\delta (x)\,dx,}  [\int
      _{-\infty }^{\infty }\varphi (x)H'(x)\,dx=\int _{-\infty }^{\infty
      }\varphi (x)\delta (x)\,dx,]
and indeed, a form of integration by parts is permitted for the Stieltjes
integral, and in that case one does have
         &#x2212;  &#x222B;  &#x2212; &#x221E;   &#x221E;    &#x03C6; &#x2032;
      ( x ) H ( x )  d x =  &#x222B;  &#x2212; &#x221E;   &#x221E;   &#x03C6;
      ( x )  d H ( x ) .   {\displaystyle -\int _{-\infty }^{\infty }\varphi '
      (x)H(x)\,dx=\int _{-\infty }^{\infty }\varphi (x)\,dH(x).}  [-\int _{-
      \infty }^{\infty }\varphi '(x)H(x)\,dx=\int _{-\infty }^{\infty }\varphi
      (x)\,dH(x).]
In the context of measure theory, the Dirac measure gives rise to a
distribution by integration. Conversely, equation (1) defines a Daniell
integral on the space of all compactly supported continuous functions Ï which,
by the Riesz_representation_theorem, can be represented as the Lebesgue
integral of Ï with respect to some Radon_measure.
Generally, when the term "Dirac delta function" is used, it is in the sense of
distributions rather than measures, the Dirac_measure being among several terms
for the corresponding notion in measure theory. Some sources may also use the
term Dirac delta distribution.
**** Generalizations[edit] ****
The delta function can be defined in n-dimensional Euclidean_space Rn as the
measure such that
          &#x222B;    R   n     f (  x  ) &#x03B4; { d  x  } = f (  0  )
      {\displaystyle \int _{\mathbf {R} ^{n}}f(\mathbf {x} )\delta \{d\mathbf
      {x} \}=f(\mathbf {0} )}  [\int _{\mathbf {R} ^{n}}f(\mathbf {x} )\delta \
      {d\mathbf {x} \}=f(\mathbf {0} )]
for every compactly supported continuous function f. As a measure, the n-
dimensional delta function is the product_measure of the 1-dimensional delta
functions in each variable separately. Thus, formally, with x = (x1, x2, ...,
xn), one has[6]
         &#x03B4; (  x  ) = &#x03B4; (  x  1   ) &#x03B4; (  x  2   )
      &#x22EF; &#x03B4; (  x  n   ) .   {\displaystyle \delta            
      (\mathbf {x} )=\delta (x_{1})\delta (x_{2})\cdots \delta (x_         (2)
      {n}).}  [{\displaystyle \delta (\mathbf {x} )=\delta (x_
      {1})\delta (x_{2})\cdots \delta (x_{n}).}]
The delta function can also be defined in the sense of distributions exactly as
above in the one-dimensional case.[25] However, despite widespread use in
engineering contexts, (2) should be manipulated with care, since the product of
distributions can only be defined under quite narrow circumstances.[26]
The notion of a Dirac_measure makes sense on any set.[19] Thus if X is a set,
x0 â X is a marked point, and Î£ is any sigma_algebra of subsets of X, then
the measure defined on sets A â Î£ by
          &#x03B4;   x  0     ( A ) =   {    1    if&#xA0;   x  0   &#x2208; A
      0    if&#xA0;   x  0   &#x2209; A         {\displaystyle \delta _{x_{0}}
      (A)={\begin{cases}1&{\text{if }}x_{0}\in A\\0&{\text{if }}x_{0}\notin
      A\end{cases}}}  [\delta _{x_{0}}(A)={\begin{cases}1&{\text{if }}x_{0}\in
      A\\0&{\text{if }}x_{0}\notin A\end{cases}}]
is the delta measure or unit mass concentrated at x0.
Another common generalization of the delta function is to a differentiable
manifold where most of its properties as a distribution can also be exploited
because of the differentiable_structure. The delta function on a manifold M
centered at the point x0 â M is defined as the following distribution:
          &#x03B4;   x  0     [ &#x03C6; ] = &#x03C6; (  x  0   )       
      {\displaystyle \delta _{x_{0}}[\varphi ]=\varphi (x_{0})}           (3)
      [\delta _{x_{0}}[\varphi ]=\varphi (x_{0})]
for all compactly supported smooth real-valued functions Ï on M.[27] A common
special case of this construction is that in which M is an open_set in the
Euclidean space Rn.
On a locally_compact_Hausdorff_space X, the Dirac delta measure concentrated at
a point x is the Radon_measure associated with the Daniell integral (3) on
compactly supported continuous functions Ï.[28] At this level of generality,
calculus as such is no longer possible, however a variety of techniques from
abstract analysis are available. For instance, the mapping      x  0   &#x21A6;
&#x03B4;   x  0       {\displaystyle x_{0}\mapsto \delta _{x_{0}}}  [x_
{0}\mapsto \delta _{x_{0}}] is a continuous embedding of X into the space of
finite Radon measures on X, equipped with its vague_topology. Moreover, the
convex_hull of the image of X under this embedding is dense in the space of
probability measures on X.[29]
***** Properties[edit] *****
**** Scaling and symmetry[edit] ****
The delta function satisfies the following scaling property for a non-zero
scalar Î±:[30]
          &#x222B;  &#x2212; &#x221E;   &#x221E;   &#x03B4; ( &#x03B1; x )  d x
      =  &#x222B;  &#x2212; &#x221E;   &#x221E;   &#x03B4; ( u )     d u    |
      &#x03B1;  |     =   1   |  &#x03B1;  |       {\displaystyle \int _{-
      \infty }^{\infty }\delta (\alpha x)\,dx=\int _{-\infty }^{\infty }\delta
      (u)\,{\frac {du}{|\alpha |}}={\frac {1}{|\alpha |}}}  [\int _{-\infty }^
      {\infty }\delta (\alpha x)\,dx=\int _{-\infty }^{\infty }\delta (u)\,
      {\frac {du}{|\alpha |}}={\frac {1}{|\alpha |}}]
and so
         &#x03B4; ( &#x03B1; x ) =    &#x03B4; ( x )    |  &#x03B1;
      |     .   {\displaystyle \delta (\alpha x)={\frac {\delta (x)}    (4)
      {|\alpha |}}.}  [\delta (\alpha x)={\frac {\delta (x)}{|\alpha    
      |}}.]
In particular, the delta function is an even distribution, in the sense that
         &#x03B4; ( &#x2212; x ) = &#x03B4; ( x )   {\displaystyle \delta (-
      x)=\delta (x)}  [\delta (-x)=\delta (x)]
which is homogeneous of degree â1.
**** Algebraic properties[edit] ****
The distributional_product of Î´ with x is equal to zero:
         x &#x03B4; ( x ) = 0.   {\displaystyle x\delta (x)=0.}  [x\delta
      (x)=0.]
Conversely, if xf(x) = xg(x), where f and g are distributions, then
         f ( x ) = g ( x ) + c &#x03B4; ( x )   {\displaystyle f(x)=g
      (x)+c\delta (x)}  [f(x)=g(x)+c\delta (x)]
for some constant c.[31]
**** Translation[edit] ****
The integral of the time-delayed Dirac delta is
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( t ) &#x03B4; ( t
      &#x2212; T )  d t = f ( T ) .   {\displaystyle \int _{-\infty }^{\infty
      }f(t)\delta (t-T)\,dt=f(T).}  [\int _{-\infty }^{\infty }f(t)\delta (t-
      T)\,dt=f(T).]
This is sometimes referred to as the sifting property[32] or the sampling
property. The delta function is said to "sift out" the value at t = T.
It follows that the effect of convolving a function f(t) with the time-delayed
Dirac delta is to time-delay f(t) by the same amount:
         ( f ( t )
      &#x2217;
      &#x03B4; ( t      &#xA0;     =    d e f      &#xA0;  &#x222B;  &#x2212; &#x221E;
      &#x2212; T ) ) &#x221E;   f ( &#x03C4; ) &#x03B4; ( t &#x2212; T &#x2212; &#x03C4; )  d
      {\displaystyle &#x03C4;   {\displaystyle \ {\stackrel {\mathrm {def} }{=}}\ \int _{-
      (f(t)*\delta   \infty }^{\infty }f(\tau )\delta (t-T-\tau )\,d\tau }  [\ {\stackrel
      (t-T))}  [     {\mathrm {def} }{=}}\ \int _{-\infty }^{\infty }f(\tau )\delta (t-T-\tau
      {\displaystyle )\,d\tau ]
      (f(t)*\delta
      (t-T))}]
                        =  &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( &#x03C4; ) &#x03B4;
                     ( &#x03C4; &#x2212; ( t &#x2212; T ) )  d &#x03C4;   {\displaystyle
                     =\int \limits _{-\infty }^{\infty }f(\tau )\delta (\tau -(t-T))\,d\tau }
                     [=\int \limits _{-\infty }^{\infty }f(\tau )\delta (\tau -(t-T))\,d\tau
                     ]       (using  (4):     &#x03B4; ( &#x2212; x ) = &#x03B4; ( x )
                     {\displaystyle \delta (-x)=\delta (x)}  [\delta (-x)=\delta (x)])
                        = f ( t &#x2212; T ) .   {\displaystyle =f(t-T).}  [{\displaystyle =f
                     (t-T).}]
This holds under the precise condition that f be a tempered_distribution (see
the discussion of the Fourier transform below). As a special case, for
instance, we have the identity (understood in the distribution sense)
          &#x222B;  &#x2212; &#x221E;   &#x221E;   &#x03B4; ( &#x03BE; &#x2212;
      x ) &#x03B4; ( x &#x2212; &#x03B7; )  d x = &#x03B4; ( &#x03BE; &#x2212;
      &#x03B7; ) .   {\displaystyle \int _{-\infty }^{\infty }\delta (\xi -
      x)\delta (x-\eta )\,dx=\delta (\xi -\eta ).}  [\int _{-\infty }^{\infty
      }\delta (\xi -x)\delta (x-\eta )\,dx=\delta (\xi -\eta ).]
**** Composition with a function[edit] ****
More generally, the delta distribution may be composed with a smooth function g
(x) in such a way that the familiar change of variables formula holds, that
          &#x222B;   R    &#x03B4;   (   g ( x )   )   f   (   g ( x )   )    |
      g &#x2032;  ( x )  |   d x =  &#x222B;  g (  R  )   &#x03B4; ( u ) f ( u
      )  d u   {\displaystyle \int _{\mathbf {R} }\delta {\bigl (}g(x){\bigr
      )}f{\bigl (}g(x){\bigr )}|g'(x)|\,dx=\int _{g(\mathbf {R} )}\delta (u)f
      (u)\,du}  [\int _{\mathbf {R} }\delta {\bigl (}g(x){\bigr )}f{\bigl (}g
      (x){\bigr )}|g'(x)|\,dx=\int _{g(\mathbf {R} )}\delta (u)f(u)\,du]
provided that g is a continuously_differentiable function with gâ² nowhere
zero.[33] That is, there is a unique way to assign meaning to the distribution
&#x03B4; &#x2218; g   {\displaystyle \delta \circ g}  [\delta \circ g] so that
this identity holds for all compactly supported test functions f. Therefore,
the domain must be broken up to exclude the gâ² = 0 point. This distribution
satisfies Î´(g(x)) = 0 if g is nowhere zero, and otherwise if g has a real root
at x0, then
         &#x03B4; ( g ( x ) ) =    &#x03B4; ( x &#x2212;  x  0   )    |   g
      &#x2032;  (  x  0   )  |     .   {\displaystyle \delta (g(x))={\frac
      {\delta (x-x_{0})}{|g'(x_{0})|}}.}  [\delta (g(x))={\frac {\delta (x-x_
      {0})}{|g'(x_{0})|}}.]
It is natural therefore to define the composition Î´(g(x)) for continuously
differentiable functions g by
         &#x03B4; ( g ( x ) ) =  &#x2211;  i      &#x03B4; ( x &#x2212;  x  i
      )    |   g &#x2032;  (  x  i   )  |       {\displaystyle \delta (g
      (x))=\sum _{i}{\frac {\delta (x-x_{i})}{|g'(x_{i})|}}}  [\delta (g
      (x))=\sum _{i}{\frac {\delta (x-x_{i})}{|g'(x_{i})|}}]
where the sum extends over all roots of g(x), which are assumed to be simple.
[33] Thus, for example
         &#x03B4;  (   x  2   &#x2212;  &#x03B1;  2    )  =   1  2  |  &#x03B1;
      |       [   &#x03B4;  (  x + &#x03B1;  )  + &#x03B4;  (  x &#x2212;
      &#x03B1;  )    ]   .   {\displaystyle \delta \left(x^{2}-\alpha ^
      {2}\right)={\frac {1}{2|\alpha |}}{\Big [}\delta \left(x+\alpha
      \right)+\delta \left(x-\alpha \right){\Big ]}.}  [\delta \left(x^{2}-
      \alpha ^{2}\right)={\frac {1}{2|\alpha |}}{\Big [}\delta \left(x+\alpha
      \right)+\delta \left(x-\alpha \right){\Big ]}.]
In the integral form the generalized scaling property may be written as
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x )  &#x03B4; ( g ( x )
      )  d x =  &#x2211;  i      f (  x  i   )    |   g &#x2032;  (  x  i   )
      |     .   {\displaystyle \int _{-\infty }^{\infty }f(x)\,\delta (g
      (x))\,dx=\sum _{i}{\frac {f(x_{i})}{|g'(x_{i})|}}.}  [\int _{-\infty }^
      {\infty }f(x)\,\delta (g(x))\,dx=\sum _{i}{\frac {f(x_{i})}{|g'(x_
      {i})|}}.]
**** Properties in n dimensions[edit] ****
The delta distribution in an n-dimensional space satisfies the following
scaling property instead,
         &#x03B4; ( &#x03B1;  x  ) =  |  &#x03B1;   |   &#x2212; n   &#x03B4;
      (  x  ) &#xA0; ,   {\displaystyle \delta (\alpha \mathbf {x} )=|\alpha |^
      {-n}\delta (\mathbf {x} )~,}  [{\displaystyle \delta (\alpha \mathbf {x}
      )=|\alpha |^{-n}\delta (\mathbf {x} )~,}]
so that Î´ is a homogeneous distribution of degree ân.
Under any reflection or rotation Ï, the delta function is invariant,
         &#x03B4; ( &#x03C1;  x  ) = &#x03B4; (  x  ) &#xA0; .   {\displaystyle
      \delta (\rho \mathbf {x} )=\delta (\mathbf {x} )~.}  [{\displaystyle
      \delta (\rho \mathbf {x} )=\delta (\mathbf {x} )~.}]
As in the one-variable case, it is possible to define the composition of Î´
with a bi-Lipschitz_function[34] g: Rn â Rn uniquely so that the identity
          &#x222B;    R   n     &#x03B4; ( g (  x  ) )  f ( g (  x  ) )  |  det
      g &#x2032;  (  x  )  |   d  x  =  &#x222B;  g (   R   n   )   &#x03B4;
      (  u  ) f (  u  )  d  u    {\displaystyle \int _{\mathbf {R} ^{n}}\delta
      (g(\mathbf {x} ))\,f(g(\mathbf {x} ))\left|\det g'(\mathbf {x}
      )\right|\,d\mathbf {x} =\int _{g(\mathbf {R} ^{n})}\delta (\mathbf {u} )f
      (\mathbf {u} )\,d\mathbf {u} }  [{\displaystyle \int _{\mathbf {R} ^
      {n}}\delta (g(\mathbf {x} ))\,f(g(\mathbf {x} ))\left|\det g'(\mathbf {x}
      )\right|\,d\mathbf {x} =\int _{g(\mathbf {R} ^{n})}\delta (\mathbf {u} )f
      (\mathbf {u} )\,d\mathbf {u} }]
for all compactly supported functions f.
Using the coarea_formula from geometric_measure_theory, one can also define the
composition of the delta function with a submersion from one Euclidean space to
another one of different dimension; the result is a type of current. In the
special case of a continuously differentiable function g: Rn â R such that
the gradient of g is nowhere zero, the following identity holds[35]
          &#x222B;    R   n     f (  x  )  &#x03B4; ( g (  x  ) )  d  x  =
      &#x222B;   g  &#x2212; 1   ( 0 )      f (  x  )    |   &#x2207;  g  |
      d &#x03C3; (  x  )   {\displaystyle \int _{\mathbf {R} ^{n}}f(\mathbf {x}
      )\,\delta (g(\mathbf {x} ))\,d\mathbf {x} =\int _{g^{-1}(0)}{\frac {f
      (\mathbf {x} )}{|\mathbf {\nabla } g|}}\,d\sigma (\mathbf {x} )}  [\int _
      {\mathbf {R} ^{n}}f(\mathbf {x} )\,\delta (g(\mathbf {x} ))\,d\mathbf {x}
      =\int _{g^{-1}(0)}{\frac {f(\mathbf {x} )}{|\mathbf {\nabla }
      g|}}\,d\sigma (\mathbf {x} )]
where the integral on the right is over gâ1(0), the (n â 1)-dimensional
surface defined by g(x) = 0 with respect to the Minkowski_content measure. This
is known as a simple layer integral.
More generally, if S is a smooth hypersurface of Rn, then we can associate to S
the distribution that integrates any compactly supported smooth function g over
S:
          &#x03B4;  S   [ g ] =  &#x222B;  S   g (  s  )  d &#x03C3; (  s  )
      {\displaystyle \delta _{S}[g]=\int _{S}g(\mathbf {s} )\,d\sigma (\mathbf
      {s} )}  [\delta _{S}[g]=\int _{S}g(\mathbf {s} )\,d\sigma (\mathbf {s} )]
where Ï is the hypersurface measure associated to S. This generalization is
associated with the potential_theory of simple_layer_potentials on S. If D is a
domain in Rn with smooth boundary S, then Î´S is equal to the normal_derivative
of the indicator_function of D in the distribution sense,
         &#x2212;  &#x222B;    R   n     g (  x  )     &#x2202;  1  D   (  x  )
      &#x2202; n     d  x  =  &#x222B;  S    g (  s  )  d &#x03C3; (  s  ) ,
      {\displaystyle -\int _{\mathbf {R} ^{n}}g(\mathbf {x} )\,{\frac {\partial
      1_{D}(\mathbf {x} )}{\partial n}}\;d\mathbf {x} =\int _{S}\,g(\mathbf {s}
      )\;d\sigma (\mathbf {s} ),}  [-\int _{\mathbf {R} ^{n}}g(\mathbf {x} )\,
      {\frac {\partial 1_{D}(\mathbf {x} )}{\partial n}}\;d\mathbf {x} =\int _
      {S}\,g(\mathbf {s} )\;d\sigma (\mathbf {s} ),]
where n is the outward normal.[36][37] For a proof, see e.g. the article on the
surface_delta_function.
***** Fourier transform[edit] *****
The delta function is a tempered_distribution, and therefore it has a well-
defined Fourier_transform. Formally, one finds[38]
            &#x03B4; &#x005E;    ( &#x03BE; ) =  &#x222B;  &#x2212; &#x221E;
      &#x221E;    e  &#x2212; 2 &#x03C0; i x &#x03BE;   &#x03B4; ( x )  d x =
      1.   {\displaystyle {\widehat {\delta }}(\xi )=\int _{-\infty }^{\infty
      }e^{-2\pi ix\xi }\delta (x)\,dx=1.}  [{\displaystyle {\widehat {\delta }}
      (\xi )=\int _{-\infty }^{\infty }e^{-2\pi ix\xi }\delta (x)\,dx=1.}]
Properly speaking, the Fourier transform of a distribution is defined by
imposing self-adjointness of the Fourier transform under the duality pairing
&#x27E8; &#x22C5; , &#x22C5; &#x27E9;   {\displaystyle \langle \cdot ,\cdot
\rangle }  [\langle \cdot ,\cdot \rangle ] of tempered distributions with
Schwartz_functions. Thus        &#x03B4; &#x005E;      {\displaystyle {\widehat
{\delta }}}  [{\widehat {\delta }}] is defined as the unique tempered
distribution satisfying
         &#x27E8;    &#x03B4; &#x005E;    , &#x03C6; &#x27E9; = &#x27E8;
      &#x03B4; ,    &#x03C6; &#x005E;    &#x27E9;   {\displaystyle \langle
      {\widehat {\delta }},\varphi \rangle =\langle \delta ,{\widehat {\varphi
      }}\rangle }  [{\displaystyle \langle {\widehat {\delta }},\varphi \rangle
      =\langle \delta ,{\widehat {\varphi }}\rangle }]
for all Schwartz functions Ï. And indeed it follows from this that
&#x03B4; &#x005E;    = 1.   {\displaystyle {\widehat {\delta }}=1.}  [
{\displaystyle {\widehat {\delta }}=1.}]
As a result of this identity, the convolution of the delta function with any
other tempered distribution S is simply S:
         S &#x2217; &#x03B4; = S .   {\displaystyle S*\delta =S.}  [
      {\displaystyle S*\delta =S.}]
That is to say that Î´ is an identity_element for the convolution on tempered
distributions, and in fact the space of compactly supported distributions under
convolution is an associative_algebra with identity the delta function. This
property is fundamental in signal_processing, as convolution with a tempered
distribution is a linear_time-invariant_system, and applying the linear time-
invariant system measures its impulse_response. The impulse response can be
computed to any desired degree of accuracy by choosing a suitable approximation
for Î´, and once it is known, it characterizes the system completely. See LTI
system_theory_Â§ Impulse_response_and_convolution.
The inverse Fourier transform of the tempered distribution f(Î¾) = 1 is the
delta function. Formally, this is expressed
          &#x222B;  &#x2212; &#x221E;   &#x221E;   1 &#x22C5;  e  2 &#x03C0; i
      x &#x03BE;    d &#x03BE; = &#x03B4; ( x )   {\displaystyle \int _{-\infty
      }^{\infty }1\cdot e^{2\pi ix\xi }\,d\xi =\delta (x)}  [\int _{-\infty }^
      {\infty }1\cdot e^{2\pi ix\xi }\,d\xi =\delta (x)]
and more rigorously, it follows since
         &#x27E8; 1 ,  f  &#x2228;   &#x27E9; = f ( 0 ) = &#x27E8; &#x03B4; , f
      &#x27E9;   {\displaystyle \langle 1,f^{\vee }\rangle =f(0)=\langle \delta
      ,f\rangle }  [\langle 1,f^{\vee }\rangle =f(0)=\langle \delta ,f\rangle ]
for all Schwartz functions f.
In these terms, the delta function provides a suggestive statement of the
orthogonality property of the Fourier kernel on R. Formally, one has
          &#x222B;  &#x2212; &#x221E;   &#x221E;    e  i 2 &#x03C0;  &#x03BE;
      1   t     [  e  i 2 &#x03C0;  &#x03BE;  2   t   ]   &#x2217;    d t =
      &#x222B;  &#x2212; &#x221E;   &#x221E;    e  &#x2212; i 2 &#x03C0;
      (  &#x03BE;  2   &#x2212;  &#x03BE;  1   ) t    d t = &#x03B4;
      (  &#x03BE;  2   &#x2212;  &#x03BE;  1   ) .   {\displaystyle \int _{-
      \infty }^{\infty }e^{i2\pi \xi _{1}t}\left[e^{i2\pi \xi _{2}t}\right]^
      {*}\,dt=\int _{-\infty }^{\infty }e^{-i2\pi (\xi _{2}-\xi _
      {1})t}\,dt=\delta (\xi _{2}-\xi _{1}).}  [\int _{-\infty }^{\infty }e^
      {i2\pi \xi _{1}t}\left[e^{i2\pi \xi _{2}t}\right]^{*}\,dt=\int _{-\infty
      }^{\infty }e^{-i2\pi (\xi _{2}-\xi _{1})t}\,dt=\delta (\xi _{2}-\xi _
      {1}).]
This is, of course, shorthand for the assertion that the Fourier transform of
the tempered distribution
         f ( t ) =  e  i 2 &#x03C0;  &#x03BE;  1   t     {\displaystyle f(t)=e^
      {i2\pi \xi _{1}t}}  [f(t)=e^{i2\pi \xi _{1}t}]
is
            f &#x005E;    (  &#x03BE;  2   ) = &#x03B4; (  &#x03BE;  1
      &#x2212;  &#x03BE;  2   )   {\displaystyle {\widehat {f}}(\xi _
      {2})=\delta (\xi _{1}-\xi _{2})}  [{\displaystyle {\widehat {f}}(\xi _
      {2})=\delta (\xi _{1}-\xi _{2})}]
which again follows by imposing self-adjointness of the Fourier transform.
By analytic_continuation of the Fourier transform, the Laplace_transform of the
delta function is found to be[39]
          &#x222B;  0   &#x221E;   &#x03B4; ( t &#x2212; a )  e  &#x2212; s t
      d t =  e  &#x2212; s a   .   {\displaystyle \int _{0}^{\infty }\delta (t-
      a)e^{-st}\,dt=e^{-sa}.}  [\int _{0}^{\infty }\delta (t-a)e^{-st}\,dt=e^{-
      sa}.]
***** Distributional derivatives[edit] *****
The distributional derivative of the Dirac delta distribution is the
distribution Î´â² defined on compactly supported smooth test functions Ï by
[40]
          &#x03B4; &#x2032;  [ &#x03C6; ] = &#x2212; &#x03B4; [  &#x03C6;
      &#x2032;  ] = &#x2212;  &#x03C6; &#x2032;  ( 0 ) .   {\displaystyle
      \delta '[\varphi ]=-\delta [\varphi ']=-\varphi '(0).}  [\delta '[\varphi
      ]=-\delta [\varphi ']=-\varphi '(0).]
The first equality here is a kind of integration by parts, for if Î´ were a
true function then
          &#x222B;  &#x2212; &#x221E;   &#x221E;    &#x03B4; &#x2032;  ( x )
      &#x03C6; ( x )  d x = &#x2212;  &#x222B;  &#x2212; &#x221E;   &#x221E;
      &#x03B4; ( x )  &#x03C6; &#x2032;  ( x )  d x .   {\displaystyle \int _{-
      \infty }^{\infty }\delta '(x)\varphi (x)\,dx=-\int _{-\infty }^{\infty
      }\delta (x)\varphi '(x)\,dx.}  [{\displaystyle \int _{-\infty }^{\infty
      }\delta '(x)\varphi (x)\,dx=-\int _{-\infty }^{\infty }\delta (x)\varphi
      '(x)\,dx.}]
The k-th derivative of Î´ is defined similarly as the distribution given on
test functions by
          &#x03B4;  ( k )   [ &#x03C6; ] = ( &#x2212; 1  )  k    &#x03C6;  ( k
      )   ( 0 ) .   {\displaystyle \delta ^{(k)}[\varphi ]=(-1)^{k}\varphi ^{
      (k)}(0).}  [\delta ^{(k)}[\varphi ]=(-1)^{k}\varphi ^{(k)}(0).]
In particular, Î´ is an infinitely differentiable distribution.
The first derivative of the delta function is the distributional limit of the
difference quotients:[41]
          &#x03B4; &#x2032;  ( x ) =  lim  h &#x2192; 0      &#x03B4; ( x + h )
      &#x2212; &#x03B4; ( x )  h   .   {\displaystyle \delta '(x)=\lim _{h\to
      0}{\frac {\delta (x+h)-\delta (x)}{h}}.}  [\delta '(x)=\lim _{h\to 0}
      {\frac {\delta (x+h)-\delta (x)}{h}}.]
More properly, one has
          &#x03B4; &#x2032;  =  lim  h &#x2192; 0     1 h   (  &#x03C4;  h
      &#x03B4; &#x2212; &#x03B4; )   {\displaystyle \delta '=\lim _{h\to 0}
      {\frac {1}{h}}(\tau _{h}\delta -\delta )}  [\delta '=\lim _{h\to 0}{\frac
      {1}{h}}(\tau _{h}\delta -\delta )]
where Ïh is the translation operator, defined on functions by ÏhÏ(x) = Ï(x
+ h), and on a distribution S by
         (  &#x03C4;  h   S ) [ &#x03C6; ] = S [  &#x03C4;  &#x2212; h
      &#x03C6; ] .   {\displaystyle (\tau _{h}S)[\varphi ]=S[\tau _{-h}\varphi
      ].}  [(\tau _{h}S)[\varphi ]=S[\tau _{-h}\varphi ].]
In the theory of electromagnetism, the first derivative of the delta function
represents a point magnetic dipole situated at the origin. Accordingly, it is
referred to as a dipole or the doublet_function.[42]
The derivative of the delta function satisfies a number of basic properties,
including:
                d  d x    &#x03B4; ( &#x2212; x ) =   d  d x    &#x03B4; ( x )
      &#x03B4; &#x2032;  ( &#x2212; x ) = &#x2212;  &#x03B4; &#x2032;  ( x )
      x  &#x03B4; &#x2032;  ( x ) = &#x2212; &#x03B4; ( x ) .
      {\displaystyle {\begin{aligned}&{\frac {d}{dx}}\delta (-x)={\frac {d}
      {dx}}\delta (x)\\[8pt]&\delta '(-x)=-\delta '(x)\\[8pt]&x\delta '(x)=-
      \delta (x).\end{aligned}}}  [{\displaystyle {\begin{aligned}&{\frac {d}
      {dx}}\delta (-x)={\frac {d}{dx}}\delta (x)\\[8pt]&\delta '(-x)=-\delta '
      (x)\\[8pt]&x\delta '(x)=-\delta (x).\end{aligned}}}][43]
Furthermore, the convolution of Î´â² with a compactly supported smooth
function f is
          &#x03B4; &#x2032;  &#x2217; f = &#x03B4; &#x2217;  f &#x2032;  =  f
      &#x2032;  ,   {\displaystyle \delta '*f=\delta *f'=f',}  [\delta
      '*f=\delta *f'=f',]
which follows from the properties of the distributional derivative of a
convolution.
**** Higher dimensions[edit] ****
More generally, on an open_set U in the n-dimensional Euclidean_space Rn, the
Dirac delta distribution centered at a point a â U is defined by[44]
          &#x03B4;  a   [ &#x03C6; ] = &#x03C6; ( a )   {\displaystyle \delta _
      {a}[\varphi ]=\varphi (a)}  [\delta _{a}[\varphi ]=\varphi (a)]
for all Ï â S(U), the space of all smooth compactly supported functions on
U. If Î± = (Î±1, ..., Î±n) is any multi-index and âÎ± denotes the associated
mixed partial_derivative operator, then the Î±th derivative âÎ±Î´a of Î´a is
given by[44]
          &#x27E8;   &#x2202;  &#x03B1;    &#x03B4;  a   , &#x03C6;  &#x27E9;
      = ( &#x2212; 1  )   |  &#x03B1;  |     &#x27E8;   &#x03B4;  a   ,
      &#x2202;  &#x03B1;   &#x03C6;  &#x27E9;  = ( &#x2212; 1  )   |  &#x03B1;
      |     &#x2202;  &#x03B1;   &#x03C6; ( x )    |    x = a    &#xA0;for
      all&#xA0;  &#x03C6; &#x2208; S ( U ) .   {\displaystyle \left\langle
      \partial ^{\alpha }\delta _{a},\varphi \right\rangle =(-1)^{|\alpha
      |}\left\langle \delta _{a},\partial ^{\alpha }\varphi \right\rangle =(-
      1)^{|\alpha |}\partial ^{\alpha }\varphi (x){\Big |}_{x=a}{\text{ for all
      }}\varphi \in S(U).}  [{\displaystyle \left\langle \partial ^{\alpha
      }\delta _{a},\varphi \right\rangle =(-1)^{|\alpha |}\left\langle \delta _
      {a},\partial ^{\alpha }\varphi \right\rangle =(-1)^{|\alpha |}\partial ^
      {\alpha }\varphi (x){\Big |}_{x=a}{\text{ for all }}\varphi \in S(U).}]
That is, the Î±th derivative of Î´a is the distribution whose value on any test
function Ï is the Î±th derivative of Ï at a (with the appropriate positive or
negative sign).
The first partial derivatives of the delta function are thought of as double
layers along the coordinate planes. More generally, the normal_derivative of a
simple layer supported on a surface is a double layer supported on that
surface, and represents a laminar magnetic monopole. Higher derivatives of the
delta function are known in physics as multipoles.
Higher derivatives enter into mathematics naturally as the building blocks for
the complete structure of distributions with point support. If S is any
distribution on U supported on the set {a} consisting of a single point, then
there is an integer m and coefficients cÎ± such that[45]
         S =  &#x2211;   |  &#x03B1;  |  &#x2264; m    c  &#x03B1;    &#x2202;
      &#x03B1;    &#x03B4;  a   .   {\displaystyle S=\sum _{|\alpha |\leq m}c_
      {\alpha }\partial ^{\alpha }\delta _{a}.}  [S=\sum _{|\alpha |\leq m}c_
      {\alpha }\partial ^{\alpha }\delta _{a}.]
***** Representations of the delta function[edit] *****
The delta function can be viewed as the limit of a sequence of functions
         &#x03B4; ( x ) =  lim  &#x03B5; &#x2192;  0  +      &#x03B7;  &#x03B5;
      ( x ) ,   {\displaystyle \delta (x)=\lim _{\varepsilon \to 0^{+}}\eta _
      {\varepsilon }(x),}  [{\displaystyle \delta (x)=\lim _{\varepsilon \to 0^
      {+}}\eta _{\varepsilon }(x),}]
where Î·Îµ(x) is sometimes called a nascent delta function. This limit is meant
in a weak sense: either that
          lim  &#x03B5; &#x2192;  0  +      &#x222B;  &#x2212;
      &#x221E;   &#x221E;    &#x03B7;  &#x03B5;   ( x ) f ( x )  d x
      = f ( 0 )   {\displaystyle \lim _{\varepsilon \to 0^{+}}\int _    (5)
      {-\infty }^{\infty }\eta _{\varepsilon }(x)f(x)\,dx=f(0)}  [      
      {\displaystyle \lim _{\varepsilon \to 0^{+}}\int _{-\infty }^
      {\infty }\eta _{\varepsilon }(x)f(x)\,dx=f(0)}]
for all continuous functions f having compact_support, or that this limit holds
for all smooth functions f with compact support. The difference between these
two slightly different modes of weak convergence is often subtle: the former is
convergence in the vague_topology of measures, and the latter is convergence in
the sense of distributions.
**** Approximations to the identity[edit] ****
Typically a nascent delta function Î·Îµ can be constructed in the following
manner. Let Î· be an absolutely integrable function on R of total integral 1,
and define
          &#x03B7;  &#x03B5;   ( x ) =  &#x03B5;  &#x2212; 1   &#x03B7;  (   x
      &#x03B5;   )  .   {\displaystyle \eta _{\varepsilon }(x)=\varepsilon ^{-
      1}\eta \left({\frac {x}{\varepsilon }}\right).}  [\eta _{\varepsilon }
      (x)=\varepsilon ^{-1}\eta \left({\frac {x}{\varepsilon }}\right).]
In n dimensions, one uses instead the scaling
          &#x03B7;  &#x03B5;   ( x ) =  &#x03B5;  &#x2212; n   &#x03B7;  (   x
      &#x03B5;   )  .   {\displaystyle \eta _{\varepsilon }(x)=\varepsilon ^{-
      n}\eta \left({\frac {x}{\varepsilon }}\right).}  [\eta _{\varepsilon }
      (x)=\varepsilon ^{-n}\eta \left({\frac {x}{\varepsilon }}\right).]
Then a simple change of variables shows that Î·Îµ also has integral 1. One may
show that (5) holds for all continuous compactly supported functions f,[46] and
so Î·Îµ converges weakly to Î´ in the sense of measures.
The Î·Îµ constructed in this way are known as an approximation to the identity.
[47] This terminology is because the space L1(R) of absolutely integrable
functions is closed under the operation of convolution of functions: f â g
â L1(R) whenever f and g are in L1(R). However, there is no identity in L1(R)
for the convolution product: no element h such that f â h = f for all f.
Nevertheless, the sequence Î·Îµ does approximate such an identity in the sense
that
         f &#x2217;  &#x03B7;  &#x03B5;   &#x2192; f   as&#xA0;  &#x03B5;
      &#x2192; 0.   {\displaystyle f*\eta _{\varepsilon }\to f\quad {\text{as
      }}\varepsilon \to 0.}  [{\displaystyle f*\eta _{\varepsilon }\to f\quad
      {\text{as }}\varepsilon \to 0.}]
This limit holds in the sense of mean_convergence (convergence in L1). Further
conditions on the Î·Îµ, for instance that it be a mollifier associated to a
compactly supported function,[48] are needed to ensure pointwise convergence
almost_everywhere.
If the initial Î· = Î·1 is itself smooth and compactly supported then the
sequence is called a mollifier. The standard mollifier is obtained by choosing
Î· to be a suitably normalized bump_function, for instance
         &#x03B7; ( x ) =   {     e  &#x2212;   1  1 &#x2212;  |  x   |   2
      if&#xA0;   |  x  |  < 1     0    if&#xA0;   |  x  |  &#x2265; 1.
      {\displaystyle \eta (x)={\begin{cases}e^{-{\frac {1}{1-|x|^{2}}}}&{\text
      {if }}|x|<1\\0&{\text{if }}|x|\geq 1.\end{cases}}}  [{\displaystyle \eta
      (x)={\begin{cases}e^{-{\frac {1}{1-|x|^{2}}}}&{\text{if }}|x|<1\\0&{\text
      {if }}|x|\geq 1.\end{cases}}}]
In some situations such as numerical_analysis, a piecewise_linear approximation
to the identity is desirable. This can be obtained by taking Î·1 to be a hat
function. With this choice of Î·1, one has
          &#x03B7;  &#x03B5;   ( x ) =  &#x03B5;  &#x2212; 1   max  (  1
      &#x2212;  |   x &#x03B5;   |  , 0  )    {\displaystyle \eta _{\varepsilon
      }(x)=\varepsilon ^{-1}\max \left(1-\left|{\frac {x}{\varepsilon
      }}\right|,0\right)}  [\eta _{\varepsilon }(x)=\varepsilon ^{-1}\max \left
      (1-\left|{\frac {x}{\varepsilon }}\right|,0\right)]
which are all continuous and compactly supported, although not smooth and so
not a mollifier.
**** Probabilistic considerations[edit] ****
In the context of probability_theory, it is natural to impose the additional
condition that the initial Î·1 in an approximation to the identity should be
positive, as such a function then represents a probability_distribution.
Convolution with a probability distribution is sometimes favorable because it
does not result in overshoot or undershoot, as the output is a convex
combination of the input values, and thus falls between the maximum and minimum
of the input function. Taking Î·1 to be any probability distribution at all,
and letting Î·Îµ(x) = Î·1(x/Îµ)/Îµ as above will give rise to an approximation
to the identity. In general this converges more rapidly to a delta function if,
in addition, Î· has mean 0 and has small higher moments. For instance, if Î·1
is the uniform_distribution on [â1/2, 1/2], also known as the rectangular
function, then:[49]
          &#x03B7;  &#x03B5;   ( x ) =   1 &#x03B5;   rect &#x2061;  (   x
      &#x03B5;   )  =   {      1 &#x03B5;   ,   &#x2212;   &#x03B5; 2   < x <
      &#x03B5; 2       0 ,    otherwise  .         {\displaystyle \eta _
      {\varepsilon }(x)={\frac {1}{\varepsilon }}\operatorname {rect} \left(
      {\frac {x}{\varepsilon }}\right)={\begin{cases}{\frac {1}{\varepsilon
      }},&-{\frac {\varepsilon }{2}}<x<{\frac {\varepsilon }{2}}\\0,&{\text
      {otherwise}}.\end{cases}}}  [{\displaystyle \eta _{\varepsilon }(x)=
      {\frac {1}{\varepsilon }}\operatorname {rect} \left({\frac {x}
      {\varepsilon }}\right)={\begin{cases}{\frac {1}{\varepsilon }},&-{\frac
      {\varepsilon }{2}}<x<{\frac {\varepsilon }{2}}\\0,&{\text
      {otherwise}}.\end{cases}}}]
Another example is with the Wigner_semicircle_distribution
          &#x03B7;  &#x03B5;   ( x ) =   {      2  &#x03C0;  &#x03B5;  2
      &#x03B5;  2   &#x2212;  x  2     ,   &#x2212; &#x03B5; < x < &#x03B5;
      0 ,    otherwise          {\displaystyle \eta _{\varepsilon }(x)={\begin
      {cases}{\frac {2}{\pi \varepsilon ^{2}}}{\sqrt {\varepsilon ^{2}-x^
      {2}}},&-\varepsilon <x<\varepsilon \\0,&{\text{otherwise}}\end{cases}}}
      [\eta _{\varepsilon }(x)={\begin{cases}{\frac {2}{\pi \varepsilon ^{2}}}
      {\sqrt {\varepsilon ^{2}-x^{2}}},&-\varepsilon <x<\varepsilon \\0,&{\text
      {otherwise}}\end{cases}}]
This is continuous and compactly supported, but not a mollifier because it is
not smooth.
**** Semigroups[edit] ****
Nascent delta functions often arise as convolution semigroups. This amounts to
the further constraint that the convolution of Î·Îµ with Î·Î´ must satisfy
          &#x03B7;  &#x03B5;   &#x2217;  &#x03B7;  &#x03B4;   =  &#x03B7;
      &#x03B5; + &#x03B4;     {\displaystyle \eta _{\varepsilon }*\eta _{\delta
      }=\eta _{\varepsilon +\delta }}  [\eta _{\varepsilon }*\eta _{\delta
      }=\eta _{\varepsilon +\delta }]
for all Îµ, Î´ > 0. Convolution semigroups in L1 that form a nascent delta
function are always an approximation to the identity in the above sense,
however the semigroup condition is quite a strong restriction.
In practice, semigroups approximating the delta function arise as fundamental
solutions or Green's_functions to physically motivated elliptic or parabolic
partial_differential_equations. In the context of applied_mathematics,
semigroups arise as the output of a linear_time-invariant_system. Abstractly,
if A is a linear operator acting on functions of x, then a convolution
semigroup arises by solving the initial_value_problem
           {       &#x2202;  &#x2202; t     &#x03B7; ( t , x ) = A &#x03B7; ( t
      , x ) ,  t > 0       lim  t &#x2192;  0  +     &#x03B7; ( t , x ) =
      &#x03B4; ( x )          {\displaystyle {\begin{cases}{\dfrac {\partial }
      {\partial t}}\eta (t,x)=A\eta (t,x),\quad t>0\\[5pt]\displaystyle \lim _
      {t\to 0^{+}}\eta (t,x)=\delta (x)\end{cases}}}  [{\displaystyle {\begin
      {cases}{\dfrac {\partial }{\partial t}}\eta (t,x)=A\eta (t,x),\quad t>0\\
      [5pt]\displaystyle \lim _{t\to 0^{+}}\eta (t,x)=\delta (x)\end{cases}}}]
in which the limit is as usual understood in the weak sense. Setting Î·Îµ(x) =
Î·(Îµ, x) gives the associated nascent delta function.
Some examples of physically important convolution semigroups arising from such
a fundamental solution include the following.
  The heat kernel
The heat_kernel, defined by
          &#x03B7;  &#x03B5;   ( x ) =   1  2 &#x03C0; &#x03B5;      e
      &#x2212;    x  2    2 &#x03B5;        {\displaystyle \eta _{\varepsilon }
      (x)={\frac {1}{\sqrt {2\pi \varepsilon }}}\mathrm {e} ^{-{\frac {x^{2}}
      {2\varepsilon }}}}  [\eta _{\varepsilon }(x)={\frac {1}{\sqrt {2\pi
      \varepsilon }}}\mathrm {e} ^{-{\frac {x^{2}}{2\varepsilon }}}]
represents the temperature in an infinite wire at time t > 0, if a unit of heat
energy is stored at the origin of the wire at time t = 0. This semigroup
evolves according to the one-dimensional heat_equation:
            &#x2202; u   &#x2202; t    =   1 2       &#x2202;  2   u   &#x2202;
      x  2      .   {\displaystyle {\frac {\partial u}{\partial t}}={\frac {1}
      {2}}{\frac {\partial ^{2}u}{\partial x^{2}}}.}  [{\frac {\partial u}
      {\partial t}}={\frac {1}{2}}{\frac {\partial ^{2}u}{\partial x^{2}}}.]
In probability_theory, Î·Îµ(x) is a normal_distribution of variance Îµ and mean
0. It represents the probability_density at time t = Îµ of the position of a
particle starting at the origin following a standard Brownian_motion. In this
context, the semigroup condition is then an expression of the Markov_property
of Brownian motion.
In higher-dimensional Euclidean space Rn, the heat kernel is
          &#x03B7;  &#x03B5;   =   1  ( 2 &#x03C0; &#x03B5;  )  n  /  2
      e   &#x2212;    x &#x22C5; x   2 &#x03B5;      ,   {\displaystyle \eta _
      {\varepsilon }={\frac {1}{(2\pi \varepsilon )^{n/2}}}\mathrm {e} ^{-
      {\frac {x\cdot x}{2\varepsilon }}},}  [\eta _{\varepsilon }={\frac {1}{
      (2\pi \varepsilon )^{n/2}}}\mathrm {e} ^{-{\frac {x\cdot x}{2\varepsilon
      }}},]
and has the same physical interpretation, mutatis_mutandis. It also represents
a nascent delta function in the sense that Î·Îµ â Î´ in the distribution
sense as Îµ â 0.
  The Poisson kernel
The Poisson_kernel
          &#x03B7;  &#x03B5;   ( x ) =   1 &#x03C0;     &#x03B5;   &#x03B5;  2
      +  x  2      =  &#x222B;  &#x2212; &#x221E;   &#x221E;     e   2 &#x03C0;
      i  &#x03BE; x &#x2212;  |  &#x03B5; &#x03BE;  |     d &#x03BE;
      {\displaystyle \eta _{\varepsilon }(x)={\frac {1}{\pi }}{\frac
      {\varepsilon }{\varepsilon ^{2}+x^{2}}}=\int _{-\infty }^{\infty }\mathrm
      {e} ^{2\pi \mathrm {i} \xi x-|\varepsilon \xi |}\;d\xi }  [\eta _
      {\varepsilon }(x)={\frac {1}{\pi }}{\frac {\varepsilon }{\varepsilon ^
      {2}+x^{2}}}=\int _{-\infty }^{\infty }\mathrm {e} ^{2\pi \mathrm {i} \xi
      x-|\varepsilon \xi |}\;d\xi ]
is the fundamental solution of the Laplace_equation in the upper half-plane.
[50] It represents the electrostatic_potential in a semi-infinite plate whose
potential along the edge is held at fixed at the delta function. The Poisson
kernel is also closely related to the Cauchy_distribution. This semigroup
evolves according to the equation
            &#x2202; u   &#x2202; t    = &#x2212;   (  &#x2212;    &#x2202;  2
      &#x2202;  x  2       )    1 2    u ( t , x )   {\displaystyle {\frac
      {\partial u}{\partial t}}=-\left(-{\frac {\partial ^{2}}{\partial x^
      {2}}}\right)^{\frac {1}{2}}u(t,x)}  [{\frac {\partial u}{\partial t}}=-
      \left(-{\frac {\partial ^{2}}{\partial x^{2}}}\right)^{\frac {1}{2}}u
      (t,x)]
where the operator is rigorously defined as the Fourier_multiplier
           F    [    (  &#x2212;    &#x2202;  2    &#x2202;  x  2       )    1
      2    f  ]  ( &#x03BE; ) =  |  2 &#x03C0; &#x03BE;  |    F   f ( &#x03BE;
      ) .   {\displaystyle {\mathcal {F}}\left[\left(-{\frac {\partial ^{2}}
      {\partial x^{2}}}\right)^{\frac {1}{2}}f\right](\xi )=|2\pi \xi |
      {\mathcal {F}}f(\xi ).}  [{\mathcal {F}}\left[\left(-{\frac {\partial ^
      {2}}{\partial x^{2}}}\right)^{\frac {1}{2}}f\right](\xi )=|2\pi \xi |
      {\mathcal {F}}f(\xi ).]
**** Oscillatory integrals[edit] ****
In areas of physics such as wave_propagation and wave_mechanics, the equations
involved are hyperbolic and so may have more singular solutions. As a result,
the nascent delta functions that arise as fundamental solutions of the
associated Cauchy_problems are generally oscillatory_integrals. An example,
which comes from a solution of the EulerâTricomi_equation of transonic gas
dynamics,[51] is the rescaled Airy_function
          &#x03B5;  &#x2212; 1  /  3   Ai &#x2061;  (  x  &#x03B5;  &#x2212; 1
      /  3    )  .   {\displaystyle \varepsilon ^{-1/3}\operatorname {Ai} \left
      (x\varepsilon ^{-1/3}\right).}  [{\displaystyle \varepsilon ^{-1/
      3}\operatorname {Ai} \left(x\varepsilon ^{-1/3}\right).}]
Although using the Fourier transform, it is easy to see that this generates a
semigroup in some senseâit is not absolutely integrable and so cannot define
a semigroup in the above strong sense. Many nascent delta functions constructed
as oscillatory integrals only converge in the sense of distributions (an
example is the Dirichlet_kernel below), rather than in the sense of measures.
Another example is the Cauchy problem for the wave_equation in R1+1:[52]
              c  &#x2212; 2       &#x2202;  2   u   &#x2202;  t  2
      &#x2212; &#x0394; u    = 0     u = 0 ,     &#x2202; u   &#x2202; t    =
      &#x03B4;     for&#xA0;  t = 0.       {\displaystyle {\begin{aligned}c^{-
      2}{\frac {\partial ^{2}u}{\partial t^{2}}}-\Delta u&=0\\u=0,\quad {\frac
      {\partial u}{\partial t}}=\delta &\qquad {\text{for }}t=0.\end{aligned}}}
      [{\begin{aligned}c^{-2}{\frac {\partial ^{2}u}{\partial t^{2}}}-\Delta
      u&=0\\u=0,\quad {\frac {\partial u}{\partial t}}=\delta &\qquad {\text
      {for }}t=0.\end{aligned}}]
The solution u represents the displacement from equilibrium of an infinite
elastic string, with an initial disturbance at the origin.
Other approximations to the identity of this kind include the sinc_function
(used widely in electronics and telecommunications)
          &#x03B7;  &#x03B5;   ( x ) =   1  &#x03C0; x    sin &#x2061;  (   x
      &#x03B5;   )  =   1  2 &#x03C0;     &#x222B;  &#x2212;   1 &#x03B5;
      1 &#x03B5;    cos &#x2061; ( k x )  d k   {\displaystyle \eta _
      {\varepsilon }(x)={\frac {1}{\pi x}}\sin \left({\frac {x}{\varepsilon
      }}\right)={\frac {1}{2\pi }}\int _{-{\frac {1}{\varepsilon }}}^{\frac {1}
      {\varepsilon }}\cos(kx)\;dk}  [\eta _{\varepsilon }(x)={\frac {1}{\pi
      x}}\sin \left({\frac {x}{\varepsilon }}\right)={\frac {1}{2\pi }}\int _{-
      {\frac {1}{\varepsilon }}}^{\frac {1}{\varepsilon }}\cos(kx)\;dk]
and the Bessel_function
          &#x03B7;  &#x03B5;   ( x ) =   1 &#x03B5;    J   1 &#x03B5;
      (    x + 1  &#x03B5;   )  .   {\displaystyle \eta _{\varepsilon }(x)=
      {\frac {1}{\varepsilon }}J_{\frac {1}{\varepsilon }}\left({\frac {x+1}
      {\varepsilon }}\right).}  [\eta _{\varepsilon }(x)={\frac {1}{\varepsilon
      }}J_{\frac {1}{\varepsilon }}\left({\frac {x+1}{\varepsilon }}\right).]
**** Plane wave decomposition[edit] ****
One approach to the study of a linear partial differential equation
         L [ u ] = f ,   {\displaystyle L[u]=f,}  [{\displaystyle L[u]=f,}]
where L is a differential_operator on Rn, is to seek first a fundamental
solution, which is a solution of the equation
         L [ u ] = &#x03B4; .   {\displaystyle L[u]=\delta .}  [{\displaystyle
      L[u]=\delta .}]
When L is particularly simple, this problem can often be resolved using the
Fourier transform directly (as in the case of the Poisson kernel and heat
kernel already mentioned). For more complicated operators, it is sometimes
easier first to consider an equation of the form
         L [ u ] = h   {\displaystyle L[u]=h}  [{\displaystyle L[u]=h}]
where h is a plane_wave function, meaning that it has the form
         h = h ( x &#x22C5; &#x03BE; )   {\displaystyle h=h(x\cdot \xi )}  [h=h
      (x\cdot \xi )]
for some vector Î¾. Such an equation can be resolved (if the coefficients of L
are analytic_functions) by the CauchyâKovalevskaya_theorem or (if the
coefficients of L are constant) by quadrature. So, if the delta function can be
decomposed into plane waves, then one can in principle solve linear partial
differential equations.
Such a decomposition of the delta function into plane waves was part of a
general technique first introduced essentially by Johann_Radon, and then
developed in this form by Fritz_John (1955).[53] Choose k so that n + k is an
even integer, and for a real number s, put
         g ( s ) = Re &#x2061;  [    &#x2212;  s  k   log &#x2061; ( &#x2212; i
      s )   k ! ( 2 &#x03C0; i  )  n      ]  =   {        |  s   |   k     4 k
      ! ( 2 &#x03C0; i  )  n &#x2212; 1        n  &#xA0;odd      &#x2212;     |
      s   |   k   log &#x2061;  |  s  |    k ! ( 2 &#x03C0; i  )  n        n
      &#xA0;even.          {\displaystyle g(s)=\operatorname {Re} \left[{\frac
      {-s^{k}\log(-is)}{k!(2\pi i)^{n}}}\right]={\begin{cases}{\frac {|s|^{k}}
      {4k!(2\pi i)^{n-1}}}&n{\text{ odd}}\\[5pt]-{\frac {|s|^{k}\log |s|}{k!
      (2\pi i)^{n}}}&n{\text{ even.}}\end{cases}}}  [{\displaystyle g
      (s)=\operatorname {Re} \left[{\frac {-s^{k}\log(-is)}{k!(2\pi i)^
      {n}}}\right]={\begin{cases}{\frac {|s|^{k}}{4k!(2\pi i)^{n-1}}}&n{\text
      { odd}}\\[5pt]-{\frac {|s|^{k}\log |s|}{k!(2\pi i)^{n}}}&n{\text
      { even.}}\end{cases}}}]
Then Î´ is obtained by applying a power of the Laplacian to the integral with
respect to the unit sphere_measure dÏ of g(x Â· Î¾) for Î¾ in the unit_sphere
Snâ1:
         &#x03B4; ( x ) =  &#x0394;  x   ( n + k )  /  2    &#x222B;   S  n
      &#x2212; 1     g ( x &#x22C5; &#x03BE; )  d  &#x03C9;  &#x03BE;   .
      {\displaystyle \delta (x)=\Delta _{x}^{(n+k)/2}\int _{S^{n-1}}g(x\cdot
      \xi )\,d\omega _{\xi }.}  [{\displaystyle \delta (x)=\Delta _{x}^{(n+k)/
      2}\int _{S^{n-1}}g(x\cdot \xi )\,d\omega _{\xi }.}]
The Laplacian here is interpreted as a weak derivative, so that this equation
is taken to mean that, for any test function Ï,
         &#x03C6; ( x ) =  &#x222B;    R   n     &#x03C6; ( y )  d y   &#x0394;
      x     n + k  2     &#x222B;   S  n &#x2212; 1     g ( ( x &#x2212; y )
      &#x22C5; &#x03BE; )  d  &#x03C9;  &#x03BE;   .   {\displaystyle \varphi
      (x)=\int _{\mathbf {R} ^{n}}\varphi (y)\,dy\,\Delta _{x}^{\frac {n+k}
      {2}}\int _{S^{n-1}}g((x-y)\cdot \xi )\,d\omega _{\xi }.}  [\varphi
      (x)=\int _{\mathbf {R} ^{n}}\varphi (y)\,dy\,\Delta _{x}^{\frac {n+k}
      {2}}\int _{S^{n-1}}g((x-y)\cdot \xi )\,d\omega _{\xi }.]
The result follows from the formula for the Newtonian_potential (the
fundamental solution of Poisson's equation). This is essentially a form of the
inversion formula for the Radon_transform, because it recovers the value of Ï
(x) from its integrals over hyperplanes. For instance, if n is odd and k = 1,
then the integral on the right hand side is
               c  n    &#x0394;  x     n + 1  2    &#x222B;  &#x222B;   S  n
      &#x2212; 1     &#x03C6; ( y )  |  ( y &#x2212; x ) &#x22C5; &#x03BE;  |
      d  &#x03C9;  &#x03BE;    d y     =      c  n    &#x0394;  x   ( n + 1 )
      /  2    &#x222B;   S  n &#x2212; 1      d  &#x03C9;  &#x03BE;    &#x222B;
      &#x2212; &#x221E;   &#x221E;    |  p  |  R &#x03C6; ( &#x03BE; , p + x
      &#x22C5; &#x03BE; )  d p       {\displaystyle {\begin{aligned}&c_
      {n}\Delta _{x}^{\frac {n+1}{2}}\int \int _{S^{n-1}}\varphi (y)|(y-x)\cdot
      \xi |\,d\omega _{\xi }\,dy\\[5pt]={}&c_{n}\Delta _{x}^{(n+1)/2}\int _{S^
      {n-1}}\,d\omega _{\xi }\int _{-\infty }^{\infty }|p|R\varphi (\xi
      ,p+x\cdot \xi )\,dp\end{aligned}}}  [{\displaystyle {\begin{aligned}&c_
      {n}\Delta _{x}^{\frac {n+1}{2}}\int \int _{S^{n-1}}\varphi (y)|(y-x)\cdot
      \xi |\,d\omega _{\xi }\,dy\\[5pt]={}&c_{n}\Delta _{x}^{(n+1)/2}\int _{S^
      {n-1}}\,d\omega _{\xi }\int _{-\infty }^{\infty }|p|R\varphi (\xi
      ,p+x\cdot \xi )\,dp\end{aligned}}}]
where RÏ(Î¾, p) is the Radon transform of Ï:
         R &#x03C6; ( &#x03BE; , p ) =  &#x222B;  x &#x22C5; &#x03BE; = p   f
      ( x )   d  n &#x2212; 1   x .   {\displaystyle R\varphi (\xi ,p)=\int _
      {x\cdot \xi =p}f(x)\,d^{n-1}x.}  [R\varphi (\xi ,p)=\int _{x\cdot \xi
      =p}f(x)\,d^{n-1}x.]
An alternative equivalent expression of the plane wave decomposition, from
Gel'fand_&_Shilov_(1966â1968, I, Â§3.10), is
         &#x03B4; ( x ) =    ( n &#x2212; 1 ) !   ( 2 &#x03C0; i  )  n
      &#x222B;   S  n &#x2212; 1     ( x &#x22C5; &#x03BE;  )  &#x2212; n    d
      &#x03C9;  &#x03BE;     {\displaystyle \delta (x)={\frac {(n-1)!}{(2\pi
      i)^{n}}}\int _{S^{n-1}}(x\cdot \xi )^{-n}\,d\omega _{\xi }}  [
      {\displaystyle \delta (x)={\frac {(n-1)!}{(2\pi i)^{n}}}\int _{S^{n-1}}
      (x\cdot \xi )^{-n}\,d\omega _{\xi }}]
for n even, and
         &#x03B4; ( x ) =   1  2 ( 2 &#x03C0; i  )  n &#x2212; 1       &#x222B;
      S  n &#x2212; 1      &#x03B4;  ( n &#x2212; 1 )   ( x &#x22C5; &#x03BE; )
      d  &#x03C9;  &#x03BE;     {\displaystyle \delta (x)={\frac {1}{2(2\pi i)^
      {n-1}}}\int _{S^{n-1}}\delta ^{(n-1)}(x\cdot \xi )\,d\omega _{\xi }}
      [\delta (x)={\frac {1}{2(2\pi i)^{n-1}}}\int _{S^{n-1}}\delta ^{(n-1)}
      (x\cdot \xi )\,d\omega _{\xi }]
for n odd.
**** Fourier kernels[edit] ****
See also: Convergence_of_Fourier_series
In the study of Fourier_series, a major question consists of determining
whether and in what sense the Fourier series associated with a periodic
function converges to the function. The nth partial sum of the Fourier series
of a function f of period 2Ï is defined by convolution (on the interval
[âÏ,Ï]) with the Dirichlet_kernel:
          D  N   ( x ) =  &#x2211;  n = &#x2212; N   N    e  i n x   =    sin
      &#x2061;  (  ( N +    1 2    ) x  )    sin &#x2061; ( x  /  2 )    .
      {\displaystyle D_{N}(x)=\sum _{n=-N}^{N}e^{inx}={\frac {\sin \left((N+
      {\tfrac {1}{2}})x\right)}{\sin(x/2)}}.}  [D_{N}(x)=\sum _{n=-N}^{N}e^
      {inx}={\frac {\sin \left((N+{\tfrac {1}{2}})x\right)}{\sin(x/2)}}.]
Thus,
          s  N   ( f ) ( x ) =  D  N   &#x2217; f ( x ) =  &#x2211;  n =
      &#x2212; N   N    a  n    e  i n x     {\displaystyle s_{N}(f)(x)=D_{N}*f
      (x)=\sum _{n=-N}^{N}a_{n}e^{inx}}  [s_{N}(f)(x)=D_{N}*f(x)=\sum _{n=-N}^
      {N}a_{n}e^{inx}]
where
          a  n   =   1  2 &#x03C0;     &#x222B;  &#x2212; &#x03C0;   &#x03C0;
      f ( y )  e  &#x2212; i n y    d y .   {\displaystyle a_{n}={\frac {1}
      {2\pi }}\int _{-\pi }^{\pi }f(y)e^{-iny}\,dy.}  [a_{n}={\frac {1}{2\pi
      }}\int _{-\pi }^{\pi }f(y)e^{-iny}\,dy.]
A fundamental result of elementary Fourier series states that the Dirichlet
kernel tends to the a multiple of the delta function as N â â. This is
interpreted in the distribution sense, that
          s  N   ( f ) ( 0 ) =  &#x222B;   R     D  N   ( x ) f ( x )  d x
      &#x2192; 2 &#x03C0; f ( 0 )   {\displaystyle s_{N}(f)(0)=\int _{\mathbf
      {R} }D_{N}(x)f(x)\,dx\to 2\pi f(0)}  [s_{N}(f)(0)=\int _{\mathbf {R} }D_
      {N}(x)f(x)\,dx\to 2\pi f(0)]
for every compactly supported smooth function f. Thus, formally one has
         &#x03B4; ( x ) =   1  2 &#x03C0;     &#x2211;  n = &#x2212; &#x221E;
      &#x221E;    e  i n x     {\displaystyle \delta (x)={\frac {1}{2\pi }}\sum
      _{n=-\infty }^{\infty }e^{inx}}  [\delta (x)={\frac {1}{2\pi }}\sum _{n=-
      \infty }^{\infty }e^{inx}]
on the interval [âÏ,Ï].
In spite of this, the result does not hold for all compactly supported
continuous functions: that is DN does not converge weakly in the sense of
measures. The lack of convergence of the Fourier series has led to the
introduction of a variety of summability_methods in order to produce
convergence. The method of CesÃ ro_summation leads to the FejÃ©r_kernel[54]
          F  N   ( x ) =   1 N    &#x2211;  n = 0   N &#x2212; 1    D  n   ( x
      ) =   1 N     (    sin &#x2061;    N x  2     sin &#x2061;   x 2      )
      2   .   {\displaystyle F_{N}(x)={\frac {1}{N}}\sum _{n=0}^{N-1}D_{n}(x)=
      {\frac {1}{N}}\left({\frac {\sin {\frac {Nx}{2}}}{\sin {\frac {x}
      {2}}}}\right)^{2}.}  [F_{N}(x)={\frac {1}{N}}\sum _{n=0}^{N-1}D_{n}(x)=
      {\frac {1}{N}}\left({\frac {\sin {\frac {Nx}{2}}}{\sin {\frac {x}
      {2}}}}\right)^{2}.]
The FejÃ©r_kernels tend to the delta function in a stronger sense that[55]
          &#x222B;   R     F  N   ( x ) f ( x )  d x &#x2192; 2 &#x03C0; f ( 0
      )   {\displaystyle \int _{\mathbf {R} }F_{N}(x)f(x)\,dx\to 2\pi f(0)}
      [\int _{\mathbf {R} }F_{N}(x)f(x)\,dx\to 2\pi f(0)]
for every compactly supported continuous function f. The implication is that
the Fourier series of any continuous function is CesÃ ro summable to the value
of the function at every point.
**** Hilbert space theory[edit] ****
The Dirac delta distribution is a densely_defined unbounded linear_functional
on the Hilbert_space L2 of square-integrable_functions. Indeed, smooth
compactly support functions are dense in L2, and the action of the delta
distribution on such functions is well-defined. In many applications, it is
possible to identify subspaces of L2 and to give a stronger topology on which
the delta function defines a bounded_linear_functional.
  Sobolev spaces
The Sobolev_embedding_theorem for Sobolev_spaces on the real line R implies
that any square-integrable function f such that
         &#x2016; f  &#x2016;   H  1     2   =  &#x222B;  &#x2212; &#x221E;
      &#x221E;    |     f &#x005E;    ( &#x03BE; )   |   2   ( 1 +  |  &#x03BE;
      |   2   )  d &#x03BE; < &#x221E;   {\displaystyle \|f\|_{H^{1}}^{2}=\int
      _{-\infty }^{\infty }|{\widehat {f}}(\xi )|^{2}(1+|\xi |^{2})\,d\xi
      <\infty }  [{\displaystyle \|f\|_{H^{1}}^{2}=\int _{-\infty }^{\infty }|
      {\widehat {f}}(\xi )|^{2}(1+|\xi |^{2})\,d\xi <\infty }]
is automatically continuous, and satisfies in particular
         &#x03B4; [ f ] =  |  f ( 0 )  |  < C &#x2016; f  &#x2016;   H  1     .
      {\displaystyle \delta [f]=|f(0)|<C\|f\|_{H^{1}}.}  [\delta [f]=|f
      (0)|<C\|f\|_{H^{1}}.]
Thus Î´ is a bounded linear functional on the Sobolev space H1. Equivalently Î´
is an element of the continuous_dual_space Hâ1 of H1. More generally, in n
dimensions, one has Î´ â Hâs(Rn) provided s > nâ/â2.
*** Spaces of holomorphic functions[edit] ***
In complex_analysis, the delta function enters via Cauchy's_integral_formula,
which asserts that if D is a domain in the complex_plane with smooth boundary,
then
         f ( z ) =   1  2 &#x03C0; i        &#x222E;       &#x2202; D
      &#x2061;    f ( &#x03B6; )  d &#x03B6;   &#x03B6; &#x2212; z    ,  z
      &#x2208; D   {\displaystyle f(z)={\frac {1}{2\pi i}}\oint _{\partial D}
      {\frac {f(\zeta )\,d\zeta }{\zeta -z}},\quad z\in D}  [f(z)={\frac {1}
      {2\pi i}}\oint _{\partial D}{\frac {f(\zeta )\,d\zeta }{\zeta -z}},\quad
      z\in D]
for all holomorphic_functions f in D that are continuous on the closure of D.
As a result, the delta function Î´z is represented in this class of holomorphic
functions by the Cauchy integral:
          &#x03B4;  z   [ f ] = f ( z ) =   1  2 &#x03C0; i        &#x222E;
      &#x2202; D   &#x2061;    f ( &#x03B6; )  d &#x03B6;   &#x03B6; &#x2212; z
      .   {\displaystyle \delta _{z}[f]=f(z)={\frac {1}{2\pi i}}\oint _
      {\partial D}{\frac {f(\zeta )\,d\zeta }{\zeta -z}}.}  [\delta _{z}[f]=f
      (z)={\frac {1}{2\pi i}}\oint _{\partial D}{\frac {f(\zeta )\,d\zeta }
      {\zeta -z}}.]
Moreover, let H2(âD) be the Hardy_space consisting of the closure in L2(âD)
of all holomorphic functions in D continuous up to the boundary of D. Then
functions in H2(âD) uniquely extend to holomorphic functions in D, and the
Cauchy integral formula continues to hold. In particular for z â D, the delta
function Î´z is a continuous linear functional on H2(âD). This is a special
case of the situation in several_complex_variables in which, for smooth domains
D, the SzegÅ_kernel plays the role of the Cauchy integral.
*** Resolutions of the identity[edit] ***
Given a complete orthonormal_basis set of functions {Ïn} in a separable
Hilbert space, for example, the normalized eigenvectors of a compact_self-
adjoint_operator, any vector f can be expressed as
         f =  &#x2211;  n = 1   &#x221E;    &#x03B1;  n    &#x03C6;  n   .
      {\displaystyle f=\sum _{n=1}^{\infty }\alpha _{n}\varphi _{n}.}  [f=\sum
      _{n=1}^{\infty }\alpha _{n}\varphi _{n}.]
The coefficients {Î±n} are found as
          &#x03B1;  n   = &#x27E8;  &#x03C6;  n   , f &#x27E9; ,
      {\displaystyle \alpha _{n}=\langle \varphi _{n},f\rangle ,}  [\alpha _
      {n}=\langle \varphi _{n},f\rangle ,]
which may be represented by the notation:
          &#x03B1;  n   =  &#x03C6;  n   &#x2020;   f ,   {\displaystyle \alpha
      _{n}=\varphi _{n}^{\dagger }f,}  [\alpha _{n}=\varphi _{n}^{\dagger }f,]
a form of the braâket_notation of Dirac.[56] Adopting this notation, the
expansion of f takes the dyadic form:[57]
         f =  &#x2211;  n = 1   &#x221E;    &#x03C6;  n    (   &#x03C6;  n
      &#x2020;   f  )  .   {\displaystyle f=\sum _{n=1}^{\infty }\varphi _
      {n}\left(\varphi _{n}^{\dagger }f\right).}  [f=\sum _{n=1}^{\infty
      }\varphi _{n}\left(\varphi _{n}^{\dagger }f\right).]
Letting I denote the identity_operator on the Hilbert space, the expression
         I =  &#x2211;  n = 1   &#x221E;    &#x03C6;  n    &#x03C6;  n
      &#x2020;   ,   {\displaystyle I=\sum _{n=1}^{\infty }\varphi _{n}\varphi
      _{n}^{\dagger },}  [I=\sum _{n=1}^{\infty }\varphi _{n}\varphi _{n}^
      {\dagger },]
is called a resolution_of_the_identity. When the Hilbert space is the space L2
(D) of square-integrable functions on a domain D, the quantity:
          &#x03C6;  n    &#x03C6;  n   &#x2020;   ,   {\displaystyle \varphi _
      {n}\varphi _{n}^{\dagger },}  [\varphi _{n}\varphi _{n}^{\dagger },]
is an integral operator, and the expression for f can be rewritten
         f ( x ) =  &#x2211;  n = 1   &#x221E;    &#x222B;  D     (   &#x03C6;
      n   ( x )  &#x03C6;  n   &#x2217;   ( &#x03BE; )  )  f ( &#x03BE; )  d
      &#x03BE; .   {\displaystyle f(x)=\sum _{n=1}^{\infty }\int _{D}\,\left
      (\varphi _{n}(x)\varphi _{n}^{*}(\xi )\right)f(\xi )\,d\xi .}  [f(x)=\sum
      _{n=1}^{\infty }\int _{D}\,\left(\varphi _{n}(x)\varphi _{n}^{*}(\xi
      )\right)f(\xi )\,d\xi .]
The right-hand side converges to f in the L2 sense. It need not hold in a
pointwise sense, even when f is a continuous function. Nevertheless, it is
common to abuse notation and write
         f ( x ) = &#x222B;  &#x03B4; ( x &#x2212; &#x03BE; ) f ( &#x03BE; )  d
      &#x03BE; ,   {\displaystyle f(x)=\int \,\delta (x-\xi )f(\xi )\,d\xi ,}
      [f(x)=\int \,\delta (x-\xi )f(\xi )\,d\xi ,]
resulting in the representation of the delta function:[58]
         &#x03B4; ( x &#x2212; &#x03BE; ) =  &#x2211;  n = 1   &#x221E;
      &#x03C6;  n   ( x )  &#x03C6;  n   &#x2217;   ( &#x03BE; ) .
      {\displaystyle \delta (x-\xi )=\sum _{n=1}^{\infty }\varphi _{n}
      (x)\varphi _{n}^{*}(\xi ).}  [\delta (x-\xi )=\sum _{n=1}^{\infty
      }\varphi _{n}(x)\varphi _{n}^{*}(\xi ).]
With a suitable rigged_Hilbert_space (Î¦, L2(D), Î¦*) where Î¦ â L2(D)
contains all compactly supported smooth functions, this summation may converge
in Î¦*, depending on the properties of the basis Ïn. In most cases of
practical interest, the orthonormal basis comes from an integral or
differential operator, in which case the series converges in the distribution
sense.[59]
**** Infinitesimal delta functions[edit] ****
Cauchy used an infinitesimal Î± to write down a unit impulse, infinitely tall
and narrow Dirac-type delta function Î´Î± satisfying     &#x222B; F ( x )
&#x03B4;  &#x03B1;   ( x ) = F ( 0 )   {\displaystyle \int F(x)\delta _{\alpha
}(x)=F(0)}  [\int F(x)\delta _{\alpha }(x)=F(0)] in a number of articles in
1827.[60] Cauchy defined an infinitesimal in Cours d'Analyse (1827) in terms of
a sequence tending to zero. Namely, such a null sequence becomes an
infinitesimal in Cauchy's and Lazare_Carnot's terminology.
Non-standard_analysis allows one to rigorously treat infinitesimals. The
article by Yamashita_(2007) contains a bibliography on modern Dirac delta
functions in the context of an infinitesimal-enriched continuum provided by the
hyperreals. Here the Dirac delta can be given by an actual function, having the
property that for every real function F one has     &#x222B; F ( x )  &#x03B4;
&#x03B1;   ( x ) = F ( 0 )   {\displaystyle \int F(x)\delta _{\alpha }(x)=F(0)}
[\int F(x)\delta _{\alpha }(x)=F(0)] as anticipated by Fourier and Cauchy.
***** Dirac comb[edit] *****
Main article: Dirac_comb
A Dirac comb is an infinite series of Dirac delta functions spaced at intervals
of T
A so-called uniform "pulse train" of Dirac delta measures, which is known as a
Dirac_comb, or as the Shah distribution, creates a sampling function, often
used in digital_signal_processing (DSP) and discrete time signal analysis. The
Dirac comb is given as the infinite_sum, whose limit is understood in the
distribution sense,
         III &#x2061; ( x ) =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;
      &#x03B4; ( x &#x2212; n ) ,   {\displaystyle \operatorname {III} (x)=\sum
      _{n=-\infty }^{\infty }\delta (x-n),}  [{\displaystyle \operatorname
      {III} (x)=\sum _{n=-\infty }^{\infty }\delta (x-n),}]
which is a sequence of point masses at each of the integers.
Up to an overall normalizing constant, the Dirac comb is equal to its own
Fourier transform. This is significant because if f is any Schwartz_function,
then the periodization of f is given by the convolution
         ( f &#x2217; III ) ( x ) =  &#x2211;  n = &#x2212; &#x221E;   &#x221E;
      f ( x &#x2212; n ) .   {\displaystyle (f*\operatorname {III} )(x)=\sum _
      {n=-\infty }^{\infty }f(x-n).}  [{\displaystyle (f*\operatorname {III} )
      (x)=\sum _{n=-\infty }^{\infty }f(x-n).}]
In particular,
         ( f &#x2217; III  )  &#x2227;   =    f &#x005E;       III &#x005E;
      =    f &#x005E;    III   {\displaystyle (f*\operatorname {III} )^{\wedge
      }={\widehat {f}}{\widehat {\operatorname {III} }}={\widehat
      {f}}\operatorname {III} }  [{\displaystyle (f*\operatorname {III} )^
      {\wedge }={\widehat {f}}{\widehat {\operatorname {III} }}={\widehat
      {f}}\operatorname {III} }]
is precisely the Poisson_summation_formula.[61]
***** SokhotskiâPlemelj theorem[edit] *****
The SokhotskiâPlemelj_theorem, important in quantum mechanics, relates the
delta function to the distribution p.v. 1/x, the Cauchy_principal_value of the
function 1/x, defined by
          &#x27E8;   p . v .  &#x2061;   1 x   , &#x03C6;  &#x27E9;  =  lim
      &#x03B5; &#x2192;  0  +      &#x222B;   |  x  |  > &#x03B5;      &#x03C6;
      ( x )  x    d x .   {\displaystyle \left\langle \operatorname {p.v.}
      {\frac {1}{x}},\varphi \right\rangle =\lim _{\varepsilon \to 0^{+}}\int _
      {|x|>\varepsilon }{\frac {\varphi (x)}{x}}\,dx.}  [\left\langle
      \operatorname {p.v.} {\frac {1}{x}},\varphi \right\rangle =\lim _
      {\varepsilon \to 0^{+}}\int _{|x|>\varepsilon }{\frac {\varphi (x)}
      {x}}\,dx.]
Sokhotsky's formula states that[62]
          lim  &#x03B5; &#x2192;  0  +       1  x &#x00B1; i &#x03B5;    =  p .
      v .  &#x2061;   1 x   &#x2213; i &#x03C0; &#x03B4; ( x ) ,
      {\displaystyle \lim _{\varepsilon \to 0^{+}}{\frac {1}{x\pm i\varepsilon
      }}=\operatorname {p.v.} {\frac {1}{x}}\mp i\pi \delta (x),}  [\lim _
      {\varepsilon \to 0^{+}}{\frac {1}{x\pm i\varepsilon }}=\operatorname
      {p.v.} {\frac {1}{x}}\mp i\pi \delta (x),]
Here the limit is understood in the distribution sense, that for all compactly
supported smooth functions f,
          lim  &#x03B5; &#x2192;  0  +      &#x222B;  &#x2212; &#x221E;
      &#x221E;      f ( x )   x &#x00B1; i &#x03B5;     d x = &#x2213; i
      &#x03C0; f ( 0 ) +  lim  &#x03B5; &#x2192;  0  +      &#x222B;   |  x  |
      > &#x03B5;      f ( x )  x    d x .   {\displaystyle \lim _{\varepsilon
      \to 0^{+}}\int _{-\infty }^{\infty }{\frac {f(x)}{x\pm i\varepsilon
      }}\,dx=\mp i\pi f(0)+\lim _{\varepsilon \to 0^{+}}\int _{|x|>\varepsilon
      }{\frac {f(x)}{x}}\,dx.}  [\lim _{\varepsilon \to 0^{+}}\int _{-\infty }^
      {\infty }{\frac {f(x)}{x\pm i\varepsilon }}\,dx=\mp i\pi f(0)+\lim _
      {\varepsilon \to 0^{+}}\int _{|x|>\varepsilon }{\frac {f(x)}{x}}\,dx.]
***** Relationship to the Kronecker delta[edit] *****
The Kronecker_delta Î´ij is the quantity defined by
          &#x03B4;  i j   =   {    1   i = j     0   i &#x2260; j
      {\displaystyle \delta _{ij}={\begin{cases}1&i=j\\0&i\not =j\end{cases}}}
      [\delta _{ij}={\begin{cases}1&i=j\\0&i\not =j\end{cases}}]
for all integers i, j. This function then satisfies the following analog of the
sifting property: if     (  a  i    )  i &#x2208;  Z      {\displaystyle (a_
{i})_{i\in \mathbf {Z} }}  [(a_{i})_{i\in \mathbf {Z} }] is any doubly_infinite
sequence, then
          &#x2211;  i = &#x2212; &#x221E;   &#x221E;    a  i    &#x03B4;  i k
      =  a  k   .   {\displaystyle \sum _{i=-\infty }^{\infty }a_{i}\delta _
      {ik}=a_{k}.}  [\sum _{i=-\infty }^{\infty }a_{i}\delta _{ik}=a_{k}.]
Similarly, for any real or complex valued continuous function f on R, the Dirac
delta satisfies the sifting property
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x ) &#x03B4; ( x
      &#x2212;  x  0   )  d x = f (  x  0   ) .   {\displaystyle \int _{-\infty
      }^{\infty }f(x)\delta (x-x_{0})\,dx=f(x_{0}).}  [\int _{-\infty }^{\infty
      }f(x)\delta (x-x_{0})\,dx=f(x_{0}).]
This exhibits the Kronecker delta function as a discrete analog of the Dirac
delta function.[63]
***** Applications[edit] *****
**** Probability theory[edit] ****
In probability_theory and statistics, the Dirac delta function is often used to
represent a discrete_distribution, or a partially discrete, partially
continuous distribution, using a probability_density_function (which is
normally used to represent fully continuous distributions). For example, the
probability density function f(x) of a discrete distribution consisting of
points x = {x1, ..., xn}, with corresponding probabilities p1, ..., pn, can be
written as
         f ( x ) =  &#x2211;  i = 1   n    p  i   &#x03B4; ( x &#x2212;  x  i
      ) .   {\displaystyle f(x)=\sum _{i=1}^{n}p_{i}\delta (x-x_{i}).}  [f
      (x)=\sum _{i=1}^{n}p_{i}\delta (x-x_{i}).]
As another example, consider a distribution which 6/10 of the time returns a
standard normal_distribution, and 4/10 of the time returns exactly the value
3.5 (i.e. a partly continuous, partly discrete mixture_distribution). The
density function of this distribution can be written as
         f ( x ) = 0.6    1  2 &#x03C0;     e  &#x2212;    x  2   2     + 0.4
      &#x03B4; ( x &#x2212; 3.5 ) .   {\displaystyle f(x)=0.6\,{\frac {1}{\sqrt
      {2\pi }}}e^{-{\frac {x^{2}}{2}}}+0.4\,\delta (x-3.5).}  [f(x)=0.6\,{\frac
      {1}{\sqrt {2\pi }}}e^{-{\frac {x^{2}}{2}}}+0.4\,\delta (x-3.5).]
The delta function is also used in a completely different way to represent the
local_time of a diffusion_process (like Brownian_motion). The local time of a
stochastic process B(t) is given by
         &#x2113; ( x , t ) =  &#x222B;  0   t   &#x03B4; ( x &#x2212; B ( s )
      )  d s   {\displaystyle \ell (x,t)=\int _{0}^{t}\delta (x-B(s))\,ds}
      [\ell (x,t)=\int _{0}^{t}\delta (x-B(s))\,ds]
and represents the amount of time that the process spends at the point x in the
range of the process. More precisely, in one dimension this integral can be
written
         &#x2113; ( x , t ) =  lim  &#x03B5; &#x2192;  0  +       1  2 &#x03B5;
      &#x222B;  0   t     1   [ x &#x2212; &#x03B5; , x + &#x03B5; ]   ( B ( s
      ) )  d s   {\displaystyle \ell (x,t)=\lim _{\varepsilon \to 0^{+}}{\frac
      {1}{2\varepsilon }}\int _{0}^{t}\mathbf {1} _{[x-\varepsilon
      ,x+\varepsilon ]}(B(s))\,ds}  [\ell (x,t)=\lim _{\varepsilon \to 0^{+}}
      {\frac {1}{2\varepsilon }}\int _{0}^{t}\mathbf {1} _{[x-\varepsilon
      ,x+\varepsilon ]}(B(s))\,ds]
where 1[xâÎµ, x+Îµ] is the indicator_function of the interval [xâÎµ, x+Îµ].
**** Quantum mechanics[edit] ****
The delta function is expedient in quantum_mechanics. The wave_function of a
particle gives the probability amplitude of finding a particle within a given
region of space. Wave functions are assumed to be elements of the Hilbert space
L2 of square-integrable_functions, and the total probability of finding a
particle within a given interval is the integral of the magnitude of the wave
function squared over the interval. A set {Ïn} of wave functions is
orthonormal if they are normalized by
         &#x27E8;  &#x03C6;  n   &#x2223;  &#x03C6;  m   &#x27E9; =  &#x03B4;
      n m     {\displaystyle \langle \varphi _{n}\mid \varphi _{m}\rangle
      =\delta _{nm}}  [{\displaystyle \langle \varphi _{n}\mid \varphi _
      {m}\rangle =\delta _{nm}}]
where Î´ here refers to the Kronecker delta. A set of orthonormal wave
functions is complete in the space of square-integrable functions if any wave
function Ï can be expressed as a combination of the Ïn:
         &#x03C8; = &#x2211;  c  n    &#x03C6;  n   ,   {\displaystyle \psi
      =\sum c_{n}\varphi _{n},}  [\psi =\sum c_{n}\varphi _{n},]
with      c  n   = &#x27E8;  &#x03C6;  n    |  &#x03C8; &#x27E9;
{\displaystyle c_{n}=\langle \varphi _{n}|\psi \rangle }  [c_{n}=\langle
\varphi _{n}|\psi \rangle ]. Complete orthonormal systems of wave functions
appear naturally as the eigenfunctions of the Hamiltonian (of a bound_system)
in quantum mechanics that measures the energy levels, which are called the
eigenvalues. The set of eigenvalues, in this case, is known as the spectrum of
the Hamiltonian. In braâket_notation, as above, this equality implies the
resolution of the identity:
         I = &#x2211;  |   &#x03C6;  n   &#x27E9; &#x27E8;  &#x03C6;  n    |  .
      {\displaystyle I=\sum |\varphi _{n}\rangle \langle \varphi _{n}|.}
      [I=\sum |\varphi _{n}\rangle \langle \varphi _{n}|.]
Here the eigenvalues are assumed to be discrete, but the set of eigenvalues of
an observable may be continuous rather than discrete. An example is the
position_observable, QÏ(x) = xÏ(x). The spectrum of the position (in one
dimension) is the entire real line, and is called a continuous_spectrum.
However, unlike the Hamiltonian, the position operator lacks proper
eigenfunctions. The conventional way to overcome this shortcoming is to widen
the class of available functions by allowing distributions as well: that is, to
replace the Hilbert space of quantum mechanics by an appropriate rigged_Hilbert
space.[64] In this context, the position operator has a complete set of eigen-
distributions, labeled by the points y of the real line, given by
          &#x03C6;  y   ( x ) = &#x03B4; ( x &#x2212; y ) .   {\displaystyle
      \varphi _{y}(x)=\delta (x-y).}  [{\displaystyle \varphi _{y}(x)=\delta
      (x-y).}]
The eigenfunctions of position are denoted by      &#x03C6;  y   =  |  y
&#x27E9;   {\displaystyle \varphi _{y}=|y\rangle }  [\varphi _{y}=|y\rangle ]
in Dirac notation, and are known as position eigenstates.
Similar considerations apply to the eigenstates of the momentum_operator, or
indeed any other self-adjoint unbounded_operator P on the Hilbert space,
provided the spectrum of P is continuous and there are no degenerate
eigenvalues. In that case, there is a set Î© of real numbers (the spectrum),
and a collection Ïy of distributions indexed by the elements of Î©, such that
         P  &#x03C6;  y   = y  &#x03C6;  y   .   {\displaystyle P\varphi _
      {y}=y\varphi _{y}.}  [{\displaystyle P\varphi _{y}=y\varphi _{y}.}]
That is, Ïy are the eigenvectors of P. If the eigenvectors are normalized so
that
         &#x27E8;  &#x03C6;  y   ,  &#x03C6;   y &#x2032;    &#x27E9; =
      &#x03B4; ( y &#x2212;  y &#x2032;  )   {\displaystyle \langle \varphi _
      {y},\varphi _{y'}\rangle =\delta (y-y')}  [\langle \varphi _{y},\varphi _
      {y'}\rangle =\delta (y-y')]
in the distribution sense, then for any test function Ï,
         &#x03C8; ( x ) =  &#x222B;  &#x03A9;   c ( y )  &#x03C6;  y   ( x )  d
      y   {\displaystyle \psi (x)=\int _{\Omega }c(y)\varphi _{y}(x)\,dy}
      [\psi (x)=\int _{\Omega }c(y)\varphi _{y}(x)\,dy]
where
         c ( y ) = &#x27E8; &#x03C8; ,  &#x03C6;  y   &#x27E9; .
      {\displaystyle c(y)=\langle \psi ,\varphi _{y}\rangle .}  [c(y)=\langle
      \psi ,\varphi _{y}\rangle .]
That is, as in the discrete case, there is a resolution of the identity
         I =  &#x222B;  &#x03A9;    |   &#x03C6;  y   &#x27E9;  &#x27E8;
      &#x03C6;  y    |   d y   {\displaystyle I=\int _{\Omega }|\varphi _
      {y}\rangle \,\langle \varphi _{y}|\,dy}  [I=\int _{\Omega }|\varphi _
      {y}\rangle \,\langle \varphi _{y}|\,dy]
where the operator-valued integral is again understood in the weak sense. If
the spectrum of P has both continuous and discrete parts, then the resolution
of the identity involves a summation over the discrete spectrum and an integral
over the continuous spectrum.
The delta function also has many more specialized applications in quantum
mechanics, such as the delta_potential models for a single and double potential
well.
**** Structural mechanics[edit] ****
The delta function can be used in structural_mechanics to describe transient
loads or point loads acting on structures. The governing equation of a simple
massâspring_system excited by a sudden force impulse I at time t = 0 can be
written
         m      d   2   &#x03BE;    d   t  2      + k &#x03BE; = I &#x03B4; ( t
      ) ,   {\displaystyle m{\frac {\mathrm {d} ^{2}\xi }{\mathrm {d} t^
      {2}}}+k\xi =I\delta (t),}  [m{\frac {\mathrm {d} ^{2}\xi }{\mathrm {d} t^
      {2}}}+k\xi =I\delta (t),]
where m is the mass, Î¾ the deflection and k the spring_constant.
As another example, the equation governing the static deflection of a slender
beam is, according to EulerâBernoulli_theory,
         E I      d   4   w    d   x  4      = q ( x ) ,   {\displaystyle EI
      {\frac {\mathrm {d} ^{4}w}{\mathrm {d} x^{4}}}=q(x),}  [{\displaystyle EI
      {\frac {\mathrm {d} ^{4}w}{\mathrm {d} x^{4}}}=q(x),}]
where EI is the bending_stiffness of the beam, w the deflection, x the spatial
coordinate and q(x) the load distribution. If a beam is loaded by a point force
F at x = x0, the load distribution is written
         q ( x ) = F &#x03B4; ( x &#x2212;  x  0   ) .   {\displaystyle q
      (x)=F\delta (x-x_{0}).}  [{\displaystyle q(x)=F\delta (x-x_{0}).}]
As integration of the delta function results in the Heaviside_step_function, it
follows that the static deflection of a slender beam subject to multiple point
loads is described by a set of piecewise polynomials.
Also a point moment acting on a beam can be described by delta functions.
Consider two opposing point forces F at a distance d apart. They then produce a
moment M = Fd acting on the beam. Now, let the distance d approach the limit
zero, while M is kept constant. The load distribution, assuming a clockwise
moment acting at x = 0, is written
             q ( x )    =  lim  d &#x2192; 0     (   F &#x03B4; ( x ) &#x2212;
      F &#x03B4; ( x &#x2212; d )   )         =  lim  d &#x2192; 0    (    M d
      &#x03B4; ( x ) &#x2212;   M d   &#x03B4; ( x &#x2212; d )  )        = M
      lim  d &#x2192; 0      &#x03B4; ( x ) &#x2212; &#x03B4; ( x &#x2212; d )
      d         = M  &#x03B4; &#x2032;  ( x ) .       {\displaystyle {\begin
      {aligned}q(x)&=\lim _{d\to 0}{\Big (}F\delta (x)-F\delta (x-d){\Big )}\\
      [4pt]&=\lim _{d\to 0}\left({\frac {M}{d}}\delta (x)-{\frac {M}{d}}\delta
      (x-d)\right)\\[4pt]&=M\lim _{d\to 0}{\frac {\delta (x)-\delta (x-d)}
      {d}}\\[4pt]&=M\delta '(x).\end{aligned}}}  [{\displaystyle {\begin
      {aligned}q(x)&=\lim _{d\to 0}{\Big (}F\delta (x)-F\delta (x-d){\Big )}\\
      [4pt]&=\lim _{d\to 0}\left({\frac {M}{d}}\delta (x)-{\frac {M}{d}}\delta
      (x-d)\right)\\[4pt]&=M\lim _{d\to 0}{\frac {\delta (x)-\delta (x-d)}
      {d}}\\[4pt]&=M\delta '(x).\end{aligned}}}]
Point moments can thus be represented by the derivative of the delta function.
Integration of the beam equation again results in piecewise polynomial
deflection.
***** See also[edit] *****
    * Atom_(measure_theory)
    * Delta_potential
    * Dirac_measure
    * Fundamental_solution
    * Green's_function
    * Laplacian_of_the_indicator
***** Notes[edit] *****
   1. ^ Arfken_&_Weber_2000, p. 84
   2. ^ Dirac_1958, Â§15 The Î´ function, p. 58
   3. ^ Gel'fand_&_Shilov_1968, Volume I, Â§1.1
   4. ^ Gel'fand_&_Shilov_1968, Volume I, Â§1.3
   5. ^ Schwartz_1950, p. 3
   6. ^ a b Bracewell_1986, Chapter 5
   7. ^JB Fourier (1822). The_Analytical_Theory_of_Heat (English translation by
      Alexander Freeman, 1878 ed.). The University Press. p. 408.
   8. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   9. , cf p 449 and pp 546â551. The original French text can be found here.
  10. ^Hikosaburo Komatsu (2002). "Fourier's_hyperfunctions_and_Heaviside's
      pseudodifferential_operators". In Takahiro Kawai; Keiko Fujita (eds.).
      Microlocal Analysis and Complex Fourier Analysis. World Scientific.
      p. 200. ISBN 978-981-238-161-3.
  11. ^Tyn Myint-U.; Lokenath Debnath (2007). Linear_Partial_Differential
      Equations_for_Scientists_And_Engineers (4th ed.). Springer. p. 4.
      ISBN 978-0-8176-4393-5.
  12. ^Lokenath Debnath; Dambaru Bhatta (2007). Integral_Transforms_And_Their
      Applications (2nd ed.). CRC Press. p. 2. ISBN 978-1-58488-575-7.
  13. ^Ivor Grattan-Guinness (2009). Convolutions_in_French_Mathematics,
      1800â1840:_From_the_Calculus_and_Mechanics_to_Mathematical_Analysis_and
      Mathematical_Physics,_Volume_2. BirkhÃ¤user. p. 653. ISBN 978-3-7643-
      2238-0.
  14. ^  See, for example, Des_intÃ©grales_doubles_qui_se_prÃ©sentent_sous_une
      forme_indÃ©terminÃ¨e
  15. ^DragiÅ¡a MitroviÄ; Darko Å½ubriniÄ (1998). Fundamentals_of_Applied
      Functional_Analysis:_Distributions,_Sobolev_Spaces. CRC Press. p. 62.
      ISBN 978-0-582-24694-2.
  16. ^Manfred Kracht; Erwin Kreyszig (1989). "On_singular_integral_operators
      and_generalizations". In Themistocles M. Rassias (ed.). Topics in
      Mathematical Analysis: A Volume Dedicated to the Memory of A.L. Cauchy.
      World Scientific. p. 553. ISBN 978-9971-5-0666-7.
  17. ^ Laugwitz_1989, p. 230
  18. ^ A more complete historical account can be found in van_der_Pol_&
      Bremmer_1987, Â§V.4.
  19. ^ a b Dirac_1958, Â§15
  20. ^ Gel'fand_&_Shilov_1968, Volume I, Â§1.1, p. 1
  21. ^ a b Rudin_1966, Â§1.20
  22. ^ Hewitt_&_Stromberg_1963, Â§19.61
  23. ^ Driggers_2003, p. 2321. See also Bracewell_1986, Chapter 5 for a
      different interpretation. Other conventions for the assigning the value
      of the Heaviside function at zero exist, and some of these are not
      consistent with what follows.
  24. ^ Hewitt_&_Stromberg_1965, Â§9.19
  25. ^ Strichartz_1994, Â§2.2
  26. ^ HÃ¶rmander_1983, Theorem 2.1.5
  27. ^ HÃ¶rmander_1983, Â§3.1
  28. ^ Strichartz_1994, Â§2.3; HÃ¶rmander_1983, Â§8.2
  29. ^ DieudonnÃ©_1972, Â§17.3.3
  30. ^ Krantz,_S._G., & Parks,_H._R., Geometric Integration Theory (Boston:
      BirkhÃ¤user, 2008), pp._67â69.
  31. ^ Federer_1969, Â§2.5.19
  32. ^ Strichartz_1994, Problem 2.6.2
  33. ^ Vladimirov_1971, Chapter 2, Example 3(d)
  34. ^Weisstein,_Eric_W. "Sifting_Property". MathWorld.
  35. ^ a b Gel'fand_&_Shilov_1966â1968, Vol. 1, Â§II.2.5
  36. ^ Further refinement is possible, namely to submersions, although these
      require a more involved change of variables formula.
  37. ^ HÃ¶rmander_1983, Â§6.1
  38. ^ Lange_2012, pp.29â30
  39. ^ Gelfand_&_Shilov, p. 212
  40. ^ In some conventions for the Fourier transform.
  41. ^ Bracewell_1986
  42. ^ Gel'fand_&_Shilov_1966, p. 26
  43. ^ Gel'fand_&_Shilov_1966, Â§2.1
  44. ^Weisstein,_Eric_W. "Doublet_Function". MathWorld.
  45. ^ The property follows by applying a test function and integration by
      parts.
  46. ^ a b HÃ¶rmander_1983, p. 56
  47. ^ HÃ¶rmander_1983, p. 56; Rudin_1991, Theorem 6.25
  48. ^ Stein_&_Weiss, Theorem 1.18
  49. ^ Rudin_1991, Â§II.6.31
  50. ^ More generally, one only needs Î· = Î·1 to have an integrable radially
      symmetric decreasing rearrangement.
  51. ^ Saichev_&_WoyczyÅski_1997, Â§1.1 The "delta function" as viewed by a
      physicist and an engineer, p. 3
  52. ^ Stein_&_Weiss_1971, Â§I.1
  53. ^ VallÃ©e_&_Soares_2004, Â§7.2
  54. ^ HÃ¶rmander_1983, Â§7.8
  55. ^ See also Courant_&_Hilbert_1962, Â§14.
  56. ^ Lang_1997, p. 312
  57. ^ In the terminology of Lang_(1997), the FejÃ©r kernel is a Dirac
      sequence, whereas the Dirichlet kernel is not.
  58. ^  The development of this section in braâket notation is found in
      (Levin_2002, Coordinate-space wave functions and completeness, pp.=109ff)
  59. ^ Davis_&_Thomson_2000, Perfect operators, p.344
  60. ^ Davis_&_Thomson_2000, Equation 8.9.11, p. 344
  61. ^ de_la_Madrid,_Bohm_&_Gadella_2002
  62. ^ See Laugwitz_(1989).
  63. ^ CÃ³rdoba_1988; HÃ¶rmander_1983, Â§7.2
  64. ^ Vladimirov_1971, Â§5.7
  65. ^ Hartmann_1997, pp. 154â155
  66. ^ Isham_1995, Â§6.2
***** References[edit] *****
    * Aratyn, Henrik; Rasinariu, Constantin (2006), A_short_course_in
      mathematical_methods_with_Maple, World Scientific, ISBN 978-981-256-461-0
.
Arfken,_G._B.; Weber, H. J. (2000), Mathematical Methods for Physicists (5th
ed.), Boston, Massachusetts: Academic_Press, ISBN 978-0-12-059825-0
.
Bracewell, R. (1986), The Fourier Transform and Its Applications (2nd ed.),
McGraw-Hill
.
CÃ³rdoba, A., "La formule sommatoire de Poisson", Comptes Rendus de l'AcadÃ©mie
des Sciences, SÃ©rie I, 306: 373â376
.
Courant,_Richard; Hilbert,_David (1962), Methods of Mathematical Physics,
Volume II, Wiley-Interscience
.
Davis, Howard Ted; Thomson, Kendall T (2000), Linear_algebra_and_linear
operators_in_engineering_with_applications_in_Mathematica, Academic Press,
ISBN 978-0-12-206349-7
DieudonnÃ©,_Jean (1976), Treatise on analysis. Vol. II, New York: Academic
Press [Harcourt Brace Jovanovich Publishers], ISBN 978-0-12-215502-4,
MR 0530406
.
DieudonnÃ©,_Jean (1972), Treatise on analysis. Vol. III, Boston, Massachusetts:
Academic Press, MR 0350769
Dirac,_Paul (1958), The_Principles_of_Quantum_Mechanics (4th ed.), Oxford at
the Clarendon Press, ISBN 978-0-19-852011-5
.
Driggers, Ronald G. (2003), Encyclopedia of Optical Engineering, CRC Press,
ISBN 978-0-8247-0940-2
.
Duistermaat,_Hans; Kolk (2010), Distributions: Theory and applications,
Springer
.
Federer,_Herbert (1969), Geometric measure theory, Die Grundlehren der
mathematischen Wissenschaften, 153, New York: Springer-Verlag, pp. xiv+676,
ISBN 978-3-540-60656-7, MR 0257325
.
Gannon, Terry (2008), "Vertex operator algebras", Princeton Companion to
Mathematics, Princeton University Press
.
Gel'fand,_I._M.; Shilov, G. E. (1966â1968), Generalized functions, 1â5,
Academic Press
.
Hartman, William M. (1997), Signals,_sound,_and_sensation, Springer, ISBN 978-
1-56396-283-7
.
Hewitt,_E; Stromberg, K (1963), Real and abstract analysis, Springer-Verlag
.
HÃ¶rmander,_L. (1983), The analysis of linear partial differential operators I,
Grundl. Math. Wissenschaft., 256, Springer, doi:10.1007/978-3-642-96750-4,
ISBN 978-3-540-12104-6, MR 0717035
.
Isham, C. J. (1995), Lectures on quantum theory: mathematical and structural
foundations, Imperial College Press, ISBN 978-81-7764-190-5
.
John, Fritz (1955), Plane waves and spherical means applied to partial
differential equations, Interscience Publishers, New York-London, MR 0075429
.
Lang,_Serge (1997), Undergraduate analysis, Undergraduate_Texts_in_Mathematics
(2nd ed.), Berlin, New York: Springer-Verlag, doi:10.1007/978-1-4757-2698-5,
ISBN 978-0-387-94841-6, MR 1476913
.
Lange, Rutger-Jan (2012), "Potential theory, path integrals and the Laplacian
of the indicator", Journal of High Energy Physics, 2012 (11): 29â30, arXiv:
1302.0864, Bibcode:2012JHEP...11..032L, doi:10.1007/JHEP11(2012)032
.
Laugwitz,_D. (1989), "Definite values of infinite sums: aspects of the
foundations of infinitesimal analysis around 1820", Arch. Hist. Exact Sci., 39
(3): 195â245, doi:10.1007/BF00329867
.
Levin, Frank S. (2002), "Coordinate-space_wave_functions_and_completeness", An
introduction to quantum theory, Cambridge University Press, pp. 109ff,
ISBN 978-0-521-59841-5
Li, Y. T.; Wong, R. (2008), "Integral and series representations of the Dirac
delta function", Commun. Pure Appl. Anal., 7 (2): 229â247, arXiv:1303.1943,
doi:10.3934/cpaa.2008.7.229, MR 2373214
.
de la Madrid, R.; Bohm, A.; Gadella, M. (2002), "Rigged Hilbert Space Treatment
of Continuous Spectrum", Fortschr. Phys., 50 (2): 185â216, arXiv:quant-ph/
0109154, Bibcode:2002ForPh..50..185D, doi:10.1002/1521-3978(200203)50:2<185::
AID-PROP185>3.0.CO;2-S
.
McMahon, D. (2005-11-22), "An_Introduction_to_State_Space", Quantum Mechanics
Demystified, A Self-Teaching Guide, Demystified Series, New York: McGraw-Hill,
p. 108, doi:10.1036/0071455469, ISBN 978-0-07-145546-6, retrieved 2008-03-17
.
van der Pol, Balth.; Bremmer, H. (1987), Operational calculus (3rd ed.), New
York: Chelsea Publishing Co., ISBN 978-0-8284-0327-6, MR 0904873
.
Rudin,_W. (1991), Functional Analysis (2nd ed.), McGraw-Hill, ISBN 978-0-07-
054236-5
.
Soares, Manuel; VallÃ©e, Olivier (2004), Airy functions and applications to
physics, London: Imperial College Press
.
Saichev, A I; WoyczyÅski, Wojbor Andrzej (1997), "Chapter1:_Basic_definitions
and_operations", Distributions in the Physical and Engineering Sciences:
Distributional and fractal calculus, integral transforms, and wavelets,
BirkhÃ¤user, ISBN 978-0-8176-3924-2
Schwartz,_L. (1950), ThÃ©orie des distributions, 1, Hermann
.
Schwartz,_L. (1951), ThÃ©orie des distributions, 2, Hermann
.
Stein,_Elias; Weiss, Guido (1971), Introduction to Fourier Analysis on
Euclidean Spaces, Princeton University Press, ISBN 978-0-691-08078-9
.
Strichartz, R. (1994), A Guide to Distribution Theory and Fourier Transforms,
CRC Press, ISBN 978-0-8493-8273-4
.
Vladimirov, V. S. (1971), Equations of mathematical physics, Marcel Dekker,
ISBN 978-0-8247-1713-1
.
Weisstein,_Eric_W. "Delta_Function". MathWorld.
Yamashita, H. (2006), "Pointwise analysis of scalar fields: A nonstandard
approach", Journal_of_Mathematical_Physics, 47 (9): 092301, Bibcode:
2006JMP....47i2301Y, doi:10.1063/1.2339017
Yamashita, H. (2007), "Comment on "Pointwise analysis of scalar fields: A
nonstandard approach" [J. Math. Phys. 47, 092301 (2006)]", Journal_of
Mathematical_Physics, 48 (8): 084101, Bibcode:2007JMP....48h4101Y, doi:10.1063/
1.2771422
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Delta-function", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
KhanAcademy.org_video_lesson
The_Dirac_Delta_function, a tutorial on the Dirac delta function.
Video_Lectures_â_Lecture_23, a lecture by Arthur_Mattuck.
The_Dirac_delta_measure_is_a_hyperfunction
We_show_the_existence_of_a_unique_solution_and_analyze_a_finite_element
approximation_when_the_source_term_is_a_Dirac_delta_measure
Non-Lebesgue_measures_on_R._Lebesgue-Stieltjes_measure,_Dirac_delta_measure.
    * v
    * t
    * e
Probability_distributions
List
                                          * Benford
                                          * Bernoulli
                                          * beta-binomial
                                          * binomial
                                          * categorical
Discrete univariate                       * hypergeometric
with finite support                       * Poisson_binomial
                                          * Rademacher
                                          * soliton
                                          * discrete_uniform
                                          * Zipf
                                          * ZipfâMandelbrot
                                          * beta_negative_binomial
                                          * Borel
                                          * ConwayâMaxwellâPoisson
                                          * discrete_phase-type
                                          * Delaporte
                                          * extended_negative_binomial
Discrete univariate                       * GaussâKuzmin
with infinite support                     * geometric
                                          * logarithmic
                                          * negative_binomial
                                          * parabolic_fractal
                                          * Poisson
                                          * Skellam
                                          * YuleâSimon
                                          * zeta
                                          * arcsine
                                          * ARGUS
                                          * BaldingâNichols
                                          * Bates
                                          * beta
                                          * beta_rectangular
                                          * IrwinâHall
Continuous univariate                     * Kumaraswamy
supported on a bounded interval           * logit-normal
                                          * noncentral_beta
                                          * raised_cosine
                                          * reciprocal
                                          * triangular
                                          * U-quadratic
                                          * uniform
                                          * Wigner_semicircle
                                          * Benini
                                          * Benktander_1st_kind
                                          * Benktander_2nd_kind
                                          * beta_prime
                                          * Burr
                                          * chi-squared
                                          * chi
                                          * Dagum
                                          * Davis
                                          * exponential-logarithmic
                                          * Erlang
                                          * exponential
                                          * F
                                          * folded_normal
                                          * FloryâSchulz
                                          * FrÃ©chet
                                          * gamma
                                          * gamma/Gompertz
                                          * generalized_inverse_Gaussian
                                          * Gompertz
                                          * half-logistic
                                          * half-normal
                                          * Hotelling's_T-squared
                                          * hyper-Erlang
                                          * hyperexponential
                                          * hypoexponential
Continuous univariate                     * inverse_chi-squared
supported on a semi-infinite interval           o scaled_inverse_chi-squared
                                          * inverse_Gaussian
                                          * inverse_gamma
                                          * Kolmogorov
                                          * LÃ©vy
                                          * log-Cauchy
                                          * log-Laplace
                                          * log-logistic
                                          * log-normal
                                          * Lomax
                                          * matrix-exponential
                                          * MaxwellâBoltzmann
                                          * MaxwellâJÃ¼ttner
                                          * Mittag-Leffler
                                          * Nakagami
                                          * noncentral_chi-squared
                                          * Pareto
                                          * phase-type
                                          * poly-Weibull
                                          * Rayleigh
                                          * relativistic_BreitâWigner
                                          * Rice
                                          * shifted_Gompertz
                                          * truncated_normal
                                          * type-2_Gumbel
                                          * Weibull
                                                o Discrete_Weibull
                                          * Wilks's_lambda
                                          * Cauchy
                                          * exponential_power
                                          * Fisher's_z
                                          * Gaussian_q
                                          * generalized_normal
                                          * generalized_hyperbolic
                                          * geometric_stable
                                          * Gumbel
                                          * Holtsmark
                                          * hyperbolic_secant
                                          * Johnson's_SU
                                          * Landau
Continuous univariate                     * Laplace
supported on the whole real line          * asymmetric_Laplace
                                          * logistic
                                          * noncentral_t
                                          * normal_(Gaussian)
                                          * normal-inverse_Gaussian
                                          * skew_normal
                                          * slash
                                          * stable
                                          * Student's_t
                                          * type-1_Gumbel
                                          * TracyâWidom
                                          * variance-gamma
                                          * Voigt
                                          * generalized_extreme_value
                                          * generalized_Pareto
                                          * MarchenkoâPastur
Continuous univariate                     * q-exponential
with support whose type varies            * q-Gaussian
                                          * q-Weibull
                                          * shifted_log-logistic
                                          * Tukey_lambda
Mixed continuous-discrete univariate      * rectified_Gaussian
                                            inverse_matrix_gamma
                                            inverse-Wishart
                                            matrix_normal
Multivariate_(joint)                        matrix_t
                                            matrix_gamma
                                            normal-inverse-Wishart
                                            normal-Wishart
                                            Wishart
Directional                                 von_MisesâFisher
                                            Bingham
Degenerate and singular                     Cantor
                                          * Circular
                                          * compound_Poisson
                                          * elliptical
                                          * exponential
                                          * natural_exponential
Families                                  * locationâscale
                                          * maximum_entropy
                                          * mixture
                                          * Pearson
                                          * Tweedie
                                          * wrapped
    * v
    * t
    * e
Infinitesimals
                        * Adequality
                        * Leibniz's_notation
                        * Integral_symbol
                        * Criticism_of_non-standard
History                   analysis
                        * The_Analyst
                        * The_Method_of_Mechanical
                          Theorems
                        * Cavalieri's_principle
                        * Method_of_indivisibles
                        * Non-standard_analysis
                        * Non-standard_calculus
                        * Internal_set_theory
                        * Synthetic_differential_geometry
Related branches        * Smooth_infinitesimal_analysis
                        * Constructive_non-standard
                          analysis
                        * Infinitesimal_strain_theory_
                          (physics)
                        * Differentials
Formalizations          * Hyperreal_numbers
                        * Dual_numbers                    [German_integral.gif]
                        * Surreal_numbers
                        * Standard_part_function
                        * Transfer_principle
                        * Hyperinteger
                        * Increment_theorem
                        * Monad
                        * Internal_set
Individual concepts     * Levi-Civita_field
                        * Hyperfinite_set
                        * Law_of_Continuity
                        * Overspill
                        * Microcontinuity
                        * Transcendental_law_of
                          homogeneity
                        * Gottfried_Wilhelm_Leibniz
                        * Abraham_Robinson
Mathematicians          * Pierre_de_Fermat
                        * Augustin-Louis_Cauchy
                        * Leonhard_Euler
                        * Analyse_des_Infiniment_Petits
Textbooks               * Elementary_Calculus
                        * Cours_d'Analyse

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Dirac_delta_function&oldid=902698794"
Categories:
    * Fourier_analysis
    * Generalized_functions
    * Measure_theory
    * Digital_signal_processing
    * Paul_Dirac
Hidden categories:
    * Use_American_English_from_January_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * Good_articles
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * LatvieÅ¡u
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à·à·à¶à·à¶½
    * Simple_English
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Ð¢Ð°ÑÐ°ÑÑÐ°/tatarÃ§a
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ä¸­æ
Edit_links
    * This page was last edited on 20 June 2019, at 16:32 (UTC).
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
