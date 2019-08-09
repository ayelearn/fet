The following text has been accessed from https://en.wikipedia.org/wiki/Laplace_transform at Fri Aug 9 03:11:18 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Laplace transform ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"â" redirects here. For the Lagrangian, see Lagrangian_mechanics.
In mathematics, the Laplace transform is an integral_transform named after its
inventor Pierre-Simon_Laplace (/lÉËplÉËs/). It transforms a function of a
real variable t (often time) to a function of a complex_variable s (complex
frequency). The transform has many applications in science and engineering.
The Laplace transform is similar to the Fourier_transform. While the Fourier
transform of a function is a complex_function of a real variable (frequency),
the Laplace transform of a function is a complex function of a complex
variable. Laplace transforms are usually restricted to functions of t with t
â¥ 0. A consequence of this restriction is that the Laplace transform of a
function is a holomorphic_function of the variable s. Unlike the Fourier
transform, the Laplace transform of a distribution is generally a well-behaved
function. Techniques of complex variables can also be used to directly study
Laplace transforms. As a holomorphic function, the Laplace transform has a
power series representation. This power series expresses a function as a linear
superposition of moments of the function. This perspective has applications in
probability_theory.
The Laplace transform is invertible on a large class of functions. The inverse
Laplace transform takes a function of a complex variable s (often frequency)
and yields a function of a real variable t (often time). Given a simple
mathematical or functional description of an input or output to a system, the
Laplace transform provides an alternative functional description that often
simplifies the process of analyzing the behavior of the system, or in
synthesizing a new system based on a set of specifications.[1] So, for example,
Laplace transformation from the time_domain to the frequency_domain transforms
differential equations into algebraic equations and convolution into
multiplication.
Laplace wrote extensively about the use of generating_functions in Essai
philosophique sur les probabilitÃ©s (1814) and the integral form of the Laplace
transform evolved naturally as a result [2].
⁰
***** Contents *****
    * 1_History
    * 2_Formal_definition
          o 2.1_Bilateral_Laplace_transform
          o 2.2_Inverse_Laplace_transform
          o 2.3_Probability_theory
    * 3_Region_of_convergence
    * 4_Properties_and_theorems
          o 4.1_Relation_to_power_series
          o 4.2_Relation_to_moments
          o 4.3_Proof_of_the_Laplace_transform_of_a_function's_derivative
          o 4.4_Evaluating_integrals_over_the_positive_real_axis
          o 4.5_Relationship_to_other_transforms
                # 4.5.1_LaplaceâStieltjes_transform
                # 4.5.2_Fourier_transform
                # 4.5.3_Mellin_transform
                # 4.5.4_Z-transform
                # 4.5.5_Borel_transform
                # 4.5.6_Fundamental_relationships
    * 5_Table_of_selected_Laplace_transforms
    * 6_s-domain_equivalent_circuits_and_impedances
    * 7_Examples_and_applications
          o 7.1_Evaluating_improper_integrals
          o 7.2_Nuclear_physics
          o 7.3_Complex_impedance_of_a_capacitor
          o 7.4_Partial_fraction_expansion
          o 7.5_Phase_delay
          o 7.6_Determining_structure_of_astronomical_object_from_spectrum
          o 7.7_Statistical_mechanics
    * 8_See_also
    * 9_Notes
    * 10_References
          o 10.1_Modern
          o 10.2_Historical
    * 11_Further_reading
    * 12_External_links
***** History[edit] *****
The Laplace transform is named after mathematician and astronomer Pierre-Simon
Laplace, who used a similar transform in his work on probability theory.[3]
Laplace's use of generating functions was similar to what is now known as the
z-transform and he gave little attention to the continuous variable case which
was discussed by Abel.[4] The theory was further developed in the 19th and
early 20th centuries by Lerch,[5] Heaviside,[6] and Bromwich.[7] The current
widespread use of the transform (mainly in engineering) came about during and
soon after World War II[8] replacing the earlier Heaviside operational
calculus. The advantages of the Laplace transform had been emphasized by
Doetsch[9] to whom the name Laplace Transform is apparently due.
The early history of methods having some similarity to Laplace transform is as
follows. From 1744, Leonhard_Euler investigated integrals of the form
         z = &#x222B; X ( x )  e  a x    d x   &#xA0;and&#xA0;   z = &#x222B; X
      ( x )  x  A    d x   {\displaystyle z=\int X(x)e^{ax}\,dx\quad {\text
      { and }}\quad z=\int X(x)x^{A}\,dx}  [z=\int X(x)e^{ax}\,dx\quad {\text
      { and }}\quad z=\int X(x)x^{A}\,dx]
as solutions of differential_equations but did not pursue the matter very far.
[10]
Joseph_Louis_Lagrange was an admirer of Euler and, in his work on integrating
probability_density_functions, investigated expressions of the form
         &#x222B; X ( x )  e  &#x2212; a x    a  x    d x ,   {\displaystyle
      \int X(x)e^{-ax}a^{x}\,dx,}  [\int X(x)e^{-ax}a^{x}\,dx,]
which some modern historians have interpreted within modern Laplace transform
theory.[11][12][clarification_needed]
These types of integrals seem first to have attracted Laplace's attention in
1782 where he was following in the spirit of Euler in using the integrals
themselves as solutions of equations.[13] However, in 1785, Laplace took the
critical step forward when, rather than just looking for a solution in the form
of an integral, he started to apply the transforms in the sense that was later
to become popular. He used an integral of the form
         &#x222B;  x  s   &#x03C6; ( x )  d x ,   {\displaystyle \int x^
      {s}\varphi (x)\,dx,}  [{\displaystyle \int x^{s}\varphi (x)\,dx,}]
akin to a Mellin_transform, to transform the whole of a difference_equation, in
order to look for solutions of the transformed equation. He then went on to
apply the Laplace transform in the same way and started to derive some of its
properties, beginning to appreciate its potential power.[14]
Laplace also recognised that Joseph_Fourier's method of Fourier_series for
solving the diffusion_equation could only apply to a limited region of space
because those solutions were periodic. In 1809, Laplace applied his transform
to find solutions that diffused indefinitely in space.[15]
***** Formal definition[edit] *****
The Laplace transform of a function f(t), defined for all real_numbers t â¥ 0,
is the function F(s), which is a unilateral transform defined by
   F ( s ) =  &#x222B;  0   &#x221E;   f ( t )  e  &#x2212; s t     
d t   {\displaystyle F(s)=\int _{0}^{\infty }f(t)e^{-st}\,dt}  [      (Eq.1)
{\displaystyle F(s)=\int _{0}^{\infty }f(t)e^{-st}\,dt}]
where s is a complex_number frequency parameter
         s = &#x03C3; + i &#x03C9;   {\displaystyle s=\sigma +i\omega }
      [s=\sigma +i\omega ], with real numbers Ï and Ï.
An alternate notation for the Laplace transform is       L   { f }
{\displaystyle {\mathcal {L}}\{f\}}  [{\mathcal {L}}\{f\}] instead of F.
The meaning of the integral depends on types of functions of interest. A
necessary condition for existence of the integral is that f must be locally
integrable on [0, â). For locally integrable functions that decay at infinity
or are of exponential_type, the integral can be understood to be a (proper)
Lebesgue_integral. However, for many applications it is necessary to regard it
as a conditionally_convergent improper_integral at â. Still more generally,
the integral can be understood in a weak_sense, and this is dealt with below.
One can define the Laplace transform of a finite Borel_measure Î¼ by the
Lebesgue_integral[16]
           L   { &#x03BC; } ( s ) =  &#x222B;  [ 0 , &#x221E; )    e  &#x2212;
      s t    d &#x03BC; ( t ) .   {\displaystyle {\mathcal {L}}\{\mu \}(s)=\int
      _{[0,\infty )}e^{-st}\,d\mu (t).}  [{\mathcal {L}}\{\mu \}(s)=\int _{
      [0,\infty )}e^{-st}\,d\mu (t).]
An important special case is where Î¼ is a probability_measure, for example,
the Dirac_delta_function. In operational_calculus, the Laplace transform of a
measure is often treated as though the measure came from a probability_density
function f. In that case, to avoid potential confusion, one often writes
           L   { f } ( s ) =  &#x222B;   0  &#x2212;     &#x221E;   f ( t )  e
      &#x2212; s t    d t ,   {\displaystyle {\mathcal {L}}\{f\}(s)=\int _{0^{-
      }}^{\infty }f(t)e^{-st}\,dt,}  [{\displaystyle {\mathcal {L}}\{f\}
      (s)=\int _{0^{-}}^{\infty }f(t)e^{-st}\,dt,}]
where the lower limit of 0â is shorthand notation for
          lim  &#x03B5; &#x2192;  0  +      &#x222B;  &#x2212; &#x03B5;
      &#x221E;   .   {\displaystyle \lim _{\varepsilon \rightarrow 0^{+}}\int _
      {-\varepsilon }^{\infty }.}  [{\displaystyle \lim _{\varepsilon
      \rightarrow 0^{+}}\int _{-\varepsilon }^{\infty }.}]
This limit emphasizes that any point mass located at 0 is entirely captured by
the Laplace transform. Although with the Lebesgue integral, it is not necessary
to take such a limit, it does appear more naturally in connection with the
LaplaceâStieltjes_transform.
**** Bilateral Laplace transform[edit] ****
Main article: Two-sided_Laplace_transform
When one says "the Laplace transform" without qualification, the unilateral or
one-sided transform is normally intended. The Laplace transform can be
alternatively defined as the bilateral Laplace transform or two-sided_Laplace
transform by extending the limits of integration to be the entire real axis. If
that is done the common unilateral transform simply becomes a special case of
the bilateral transform where the definition of the function being transformed
is multiplied by the Heaviside_step_function. The bilateral Laplace transform
is defined as follows: F(s), which is a unilateral transform defined by
   F ( s ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;    e
&#x2212; s t   f ( t )  d t   {\displaystyle F(s)=\int _{-\infty    (Eq.2)
}^{\infty }e^{-st}f(t)\,dt}  [{\displaystyle F(s)=\int _{-\infty    
}^{\infty }e^{-st}f(t)\,dt}]
An alternate notation for the bilateral Laplace transform is       B   { f }
{\displaystyle {\mathcal {B}}\{f\}}  [{\displaystyle {\mathcal {B}}\{f\}}]
instead of     F   {\displaystyle F}  [F].
**** Inverse Laplace transform[edit] ****
Main article: Inverse_Laplace_transform
Two integrable functions have the same Laplace transform only if they differ on
a set of Lebesgue_measure zero. This means that, on the range of the transform,
there is an inverse transform. In fact, besides integrable functions, the
Laplace transform is a one-to-one mapping from one function space into another
in many other function spaces as well, although there is usually no easy
characterization of the range. Typical function spaces in which this is true
include the spaces of bounded continuous functions, the space L∞(0,_∞), or more
generally tempered_distributions on (0, ∞). The Laplace transform is also
defined and injective for suitable spaces of tempered_distributions.
In these cases, the image of the Laplace transform lives in a space of analytic
functions in the region_of_convergence. The inverse_Laplace_transform is given
by the following complex integral, which is known by various names (the
Bromwich integral, the FourierâMellin integral, and Mellin's inverse
formula):
   f ( t ) =    L    &#x2212; 1   { F } ( t ) =   1  2 &#x03C0; i
lim  T &#x2192; &#x221E;       &#x222E;       &#x03B3; &#x2212; i
T   &#x03B3; + i T   &#x2061;  e  s t   F ( s )  d s
{\displaystyle f(t)={\mathcal {L}}^{-1}\{F\}(t)={\frac {1}{2\pi       (Eq.3)
i}}\lim _{T\to \infty }\oint _{\gamma -iT}^{\gamma +iT}e^{st}F        
(s)\,ds}  [{\displaystyle f(t)={\mathcal {L}}^{-1}\{F\}(t)={\frac
{1}{2\pi i}}\lim _{T\to \infty }\oint _{\gamma -iT}^{\gamma +iT}e^
{st}F(s)\,ds}]
where Î³ is a real number so that the contour path of integration is in the
region of convergence of F(s). An alternative formula for the inverse Laplace
transform is given by Post's_inversion_formula. The limit here is interpreted
in the weak-* topology.
In practice, it is typically more convenient to decompose a Laplace transform
into known transforms of functions obtained from a table, and construct the
inverse by inspection.
**** Probability theory[edit] ****
In pure and applied_probability, the Laplace transform is defined as an
expected_value. If X is a random_variable with probability_density_function f,
then the Laplace transform of f is given by the expectation
           L   { f } ( s ) = E   [  e  &#x2212; s X   ]   .   {\displaystyle
      {\mathcal {L}}\{f\}(s)=\operatorname {E} \!\left[e^{-sX}\right]\!.}  [
      {\displaystyle {\mathcal {L}}\{f\}(s)=\operatorname {E} \!\left[e^{-
      sX}\right]\!.}]
By convention, this is referred to as the Laplace transform of the random
variable X itself. Replacing s by ât gives the moment_generating_function of
X. The Laplace transform has applications throughout probability theory,
including first_passage_times of stochastic_processes such as Markov_chains,
and renewal_theory.
Of particular use is the ability to recover the cumulative_distribution
function of a continuous random variable X by means of the Laplace transform as
follows[17]
          F  X   ( x ) =    L    &#x2212; 1     {    1 s   E &#x2061;  [  e
      &#x2212; s X   ]   }   ( x ) =    L    &#x2212; 1     {    1 s     L
      { f } ( s )  }   ( x ) .   {\displaystyle F_{X}(x)={\mathcal {L}}^{-
      1}\!\left\{{\frac {1}{s}}\operatorname {E} \left[e^{-sX}\right]\right\}\!
      (x)={\mathcal {L}}^{-1}\!\left\{{\frac {1}{s}}{\mathcal {L}}\{f\}
      (s)\right\}\!(x).}  [{\displaystyle F_{X}(x)={\mathcal {L}}^{-1}\!\left\{
      {\frac {1}{s}}\operatorname {E} \left[e^{-sX}\right]\right\}\!(x)=
      {\mathcal {L}}^{-1}\!\left\{{\frac {1}{s}}{\mathcal {L}}\{f\}
      (s)\right\}\!(x).}]
***** Region of convergence[edit] *****
If f is a locally_integrable function (or more generally a Borel measure
locally of bounded variation), then the Laplace transform F(s) of f converges
provided that the limit
          lim  R &#x2192; &#x221E;    &#x222B;  0   R   f ( t )  e  &#x2212; s
      t    d t   {\displaystyle \lim _{R\to \infty }\int _{0}^{R}f(t)e^{-
      st}\,dt}  [\lim _{R\to \infty }\int _{0}^{R}f(t)e^{-st}\,dt]
exists.
The Laplace transform converges absolutely if the integral
          &#x222B;  0   &#x221E;    |  f ( t )  e  &#x2212; s t    |   d t
      {\displaystyle \int _{0}^{\infty }\left|f(t)e^{-st}\right|\,dt}  [\int _
      {0}^{\infty }\left|f(t)e^{-st}\right|\,dt]
exists (as a proper Lebesgue integral). The Laplace transform is usually
understood as conditionally convergent, meaning that it converges in the former
instead of the latter sense.
The set of values for which F(s) converges absolutely is either of the form Re
(s) > a or else Re(s) â¥ a, where a is an extended_real_constant, ââ â¤ a
â¤ â. (This follows from the dominated_convergence_theorem.) The constant a
is known as the abscissa of absolute convergence, and depends on the growth
behavior of f(t).[18] Analogously, the two-sided transform converges absolutely
in a strip of the form a < Re(s) < b, and possibly including the lines Re(s) =
a or Re(s) = b.[19] The subset of values of s for which the Laplace transform
converges absolutely is called the region of absolute convergence or the domain
of absolute convergence. In the two-sided case, it is sometimes called the
strip of absolute convergence. The Laplace transform is analytic in the region
of absolute convergence: this is a consequence of Fubini's_theorem and Morera's
theorem.
Similarly, the set of values for which F(s) converges (conditionally or
absolutely) is known as the region of conditional convergence, or simply the
region_of_convergence (ROC). If the Laplace transform converges (conditionally)
at s = s0, then it automatically converges for all s with Re(s) > Re(s0).
Therefore, the region of convergence is a half-plane of the form Re(s) > a,
possibly including some points of the boundary line Re(s) = a.
In the region of convergence Re(s) > Re(s0), the Laplace transform of f can be
expressed by integrating_by_parts as the integral
         F ( s ) = ( s &#x2212;  s  0   )  &#x222B;  0   &#x221E;    e
      &#x2212; ( s &#x2212;  s  0   ) t   &#x03B2; ( t )  d t ,  &#x03B2; ( u )
      =  &#x222B;  0   u    e  &#x2212;  s  0   t   f ( t )  d t .
      {\displaystyle F(s)=(s-s_{0})\int _{0}^{\infty }e^{-(s-s_{0})t}\beta
      (t)\,dt,\quad \beta (u)=\int _{0}^{u}e^{-s_{0}t}f(t)\,dt.}  [F(s)=(s-s_
      {0})\int _{0}^{\infty }e^{-(s-s_{0})t}\beta (t)\,dt,\quad \beta (u)=\int
      _{0}^{u}e^{-s_{0}t}f(t)\,dt.]
That is, in the region of convergence F(s) can effectively be expressed as the
absolutely convergent Laplace transform of some other function. In particular,
it is analytic.
There are several PaleyâWiener_theorems concerning the relationship between
the decay properties of f and the properties of the Laplace transform within
the region of convergence.
In engineering applications, a function corresponding to a linear_time-
invariant_(LTI)_system is stable if every bounded input produces a bounded
output. This is equivalent to the absolute convergence of the Laplace transform
of the impulse response function in the region Re(s) â¥ 0. As a result, LTI
systems are stable provided the poles of the Laplace transform of the impulse
response function have negative real part.
This ROC is used in knowing about the causality and stability of a system.
***** Properties and theorems[edit] *****
The Laplace transform has a number of properties that make it useful for
analyzing linear dynamical_systems. The most significant advantage is that
differentiation and integration become multiplication and division,
respectively, by s (similarly to logarithms changing multiplication of numbers
to addition of their logarithms).
Because of this property, the Laplace variable s is also known as operator
variable in the L domain: either derivative operator or (for sâ1) integration
operator. The transform turns integral_equations and differential_equations to
polynomial_equations, which are much easier to solve. Once solved, use of the
inverse Laplace transform reverts to the original domain.
Given the functions f(t) and g(t), and their respective Laplace transforms F(s)
and G(s),
             f ( t )    =    L    &#x2212; 1   { F ( s ) } ,     g ( t )    =
      L    &#x2212; 1   { G ( s ) } ,       {\displaystyle {\begin{aligned}f
      (t)&={\mathcal {L}}^{-1}\{F(s)\},\\g(t)&={\mathcal {L}}^{-1}\{G(s)\},\end
      {aligned}}}  [{\begin{aligned}f(t)&={\mathcal {L}}^{-1}\{F(s)\},\\g(t)&=
      {\mathcal {L}}^{-1}\{G(s)\},\end{aligned}}]
The following table is a list of properties of unilateral Laplace transform:
[20]
                                        Properties of the unilateral Laplace transform
               Time domain    s domain       Comment
                  a f ( t ) +    a F ( s ) +
               b g ( t )      b G ( s )
               &#xA0;         &#xA0;
Linearity      {\displaystyle {\displaystyle Can be proved using basic rules of integration.
               af(t)+bg(t)\ } aF(s)+bG(s)\ }
               [af(t)+bg(t)\  [aF(s)+bG(s)\
               ]              ]
                  t f ( t )      &#x2212;  F
Frequency-     &#xA0;         &#x2032;  ( s
domain         {\displaystyle ) &#xA0;       Fâ² is the first derivative of F with respect to s.
derivative     tf(t)\ }  [tf  {\displaystyle
               (t)\ ]         -F'(s)\ }  [-
                              F'(s)\ ]
                                 ( &#x2212;
                              1  )  n    F
                   t  n   f   ( n )   ( s )
Frequency-     ( t ) &#xA0;   &#xA0;
domain general {\displaystyle {\displaystyle More general form, nth derivative of F(s).
derivative     t^{n}f(t)\ }   (-1)^{n}F^{
               [t^{n}f(t)\ ]  (n)}(s)\ }  [
                              (-1)^{n}F^{
                              (n)}(s)\ ]
                                 s F ( s )
                              &#x2212; f
                   f &#x2032; (  0  &#x2212;
               ( t ) &#xA0;   ) &#xA0;
Derivative     {\displaystyle {\displaystyle f is assumed to be a differentiable_function, and its derivative is assumed to be
               f'(t)\ }  [f'  sF(s)-f(0^{-   of exponential_type. This can then be obtained by integration_by_parts
               (t)\ ]         })\ }  [
                              {\displaystyle
                              sF(s)-f(0^{-
                              })\ }]
                                  s  2   F
                              ( s ) &#x2212;
                              s f (  0
                              &#x2212;   )
                              &#x2212;  f
                   f &#x2033; &#x2032;  (  0
               ( t ) &#xA0;   &#x2212;   )
Second         {\displaystyle &#xA0;         f is assumed twice differentiable and the second derivative to be of exponential
derivative     f''(t)\ }      {\displaystyle type. Follows by applying the Differentiation property to fâ²(t).
               [f''(t)\ ]     s^{2}F(s)-sf
                              (0^{-})-f'(0^
                              {-})\ }  [
                              {\displaystyle
                              s^{2}F(s)-sf
                              (0^{-})-f'(0^
                              {-})\ }]
                                  s  n   F
                              ( s ) &#x2212;
                              &#x2211;  k =
                              1   n    s  n
                              &#x2212; k
                              f  ( k
                              &#x2212; 1 )
                   f  ( n )   (  0  &#x2212;
General        ( t ) &#xA0;   ) &#xA0;       f is assumed to be n-times differentiable, with nth derivative of exponential
derivative     {\displaystyle {\displaystyle type. Follows by mathematical_induction.
               f^{(n)}(t)\ }  s^{n}F(s)-\sum
               [f^{(n)}(t)\ ] _{k=1}^{n}s^
                              {n-k}f^{(k-1)}
                              (0^{-})\ }  [
                              {\displaystyle
                              s^{n}F(s)-\sum
                              _{k=1}^{n}s^
                              {n-k}f^{(k-1)}
                              (0^{-})\ }]
                                  &#x222B;
                              s   &#x221E;
                              F ( &#x03C3; )
                    1 t   f   d &#x03C3;
               ( t ) &#xA0;   &#xA0;
Frequency-     {\displaystyle {\displaystyle
domain         {\frac {1}     \int _{s}^     This is deduced using the nature of frequency differentiation and conditional
integration    {t}}f(t)\ }  [ {\infty }F     convergence.
               {\frac {1}     (\sigma
               {t}}f(t)\ ]    )\,d\sigma \ }
                              [\int _{s}^
                              {\infty }F
                              (\sigma
                              )\,d\sigma \ ]
                   &#x222B;
               0   t   f
               ( &#x03C4; )
               d &#x03C4; =
               ( u &#x2217; f      1 s   F
               ) ( t )        ( s )
Time-domain    {\displaystyle {\displaystyle u(t) is the Heaviside_step_function and (u â f)(t) is the convolution of u(t)
integration    \int _{0}^{t}f {1 \over s}F   and f(t).
               (\tau )\,d\tau (s)}  [{1
               =(u*f)(t)}     \over s}F(s)]
               [\int _{0}^
               {t}f(\tau
               )\,d\tau =
               (u*f)(t)]
                   e  a t   f    F ( s
               ( t ) &#xA0;   &#x2212; a )
Frequency      {\displaystyle &#xA0;
shifting       e^{at}f(t)\ }  {\displaystyle
               [e^{at}f(t)\ ] F(s-a)\ }  [F
                              (s-a)\ ]
                  f ( t           e
               &#x2212; a ) u &#x2212; a s
               ( t &#x2212; a F ( s ) &#xA0;
Time shifting  ) &#xA0;       {\displaystyle u(t) is the Heaviside_step_function
               {\displaystyle e^{-as}F(s)\ }
               f(t-a)u(t-a)\  [e^{-as}F(s)\
               }  [f(t-a)u(t- ]
               a)\ ]
                                   1 a   F
                              (   s a   )
                              {\displaystyle
                  f ( a t )   {\frac {1}
               {\displaystyle {a}}F\left({s
Time scaling   f(at)}  [f     \over             a > 0 &#xA0;   {\displaystyle a>0\ }  [a>0\ ]
               (at)]          a}\right)}  [
                              {\frac {1}
                              {a}}F\left({s
                              \over
                              a}\right)]
                                   1  2
                              &#x03C0; i
                              lim  T
                              &#x2192;
                              &#x221E;
                              &#x222B;  c
                              &#x2212; i T
                              c + i T   F
                              ( &#x03C3; ) G
                              ( s &#x2212;
                              &#x03C3; )  d
                  f ( t ) g   &#x03C3;
               ( t )          &#xA0;
Multiplication {\displaystyle {\displaystyle The integration is done along the vertical line Re(Ï) = c that lies entirely
               f(t)g(t)}  [f  {\frac {1}     within the region of convergence of F.[21]
               (t)g(t)]       {2\pi i}}\lim
                              _{T\to \infty
                              }\int _{c-iT}^
                              {c+iT}F(\sigma
                              )G(s-\sigma
                              )\,d\sigma \ }
                              [{\frac {1}
                              {2\pi i}}\lim
                              _{T\to \infty
                              }\int _{c-iT}^
                              {c+iT}F(\sigma
                              )G(s-\sigma
                              )\,d\sigma \ ]
                  ( f
               &#x2217; g )
               ( t ) =
               &#x222B;  0
               t   f
               ( &#x03C4; ) g    F ( s )
               ( t &#x2212;   &#x22C5; G ( s
               &#x03C4; )  d  ) &#xA0;
Convolution    &#x03C4;       {\displaystyle
               {\displaystyle F(s)\cdot G
               (f*g)(t)=\int  (s)\ }  [F
               _{0}^{t}f(\tau (s)\cdot G(s)\
               )g(t-\tau      ]
               )\,d\tau }  [
               (f*g)(t)=\int
               _{0}^{t}f(\tau
               )g(t-\tau
               )\,d\tau ]
                   f              F
               &#x2217;   ( t &#x2217;
Complex        )              (  s  &#x2217;
conjugation    {\displaystyle )
               f^{*}(t)}  [f^ {\displaystyle
               {*}(t)]        F^{*}(s^{*})}
                              [F^{*}(s^{*})]
                                  F
                              &#x2217;
                  f ( t )     ( &#x2212;  s
               &#x22C6; g ( t &#x2217;   )
               )              &#x22C5; G ( s
Cross-         {\displaystyle )
correlation    f(t)\star g    {\displaystyle
               (t)}  [f       F^{*}(-s^
               (t)\star g(t)] {*})\cdot G
                              (s)}  [F^{*}(-
                              s^{*})\cdot G
                              (s)]
                                   1  1
                              &#x2212;  e
                              &#x2212; T s
                              &#x222B;  0
                              T    e
                              &#x2212; s t
                  f ( t )     f ( t )  d t
Periodic       {\displaystyle {\displaystyle f(t) is a periodic function of period T so that f(t) = f(t + T), for all t â¥ 0.
function       f(t)}  [f(t)]  {1 \over 1-e^  This is the result of the time shifting property and the geometric_series.
                              {-Ts}}\int _
                              {0}^{T}e^{-
                              st}f(t)\,dt}
                              [{1 \over 1-e^
                              {-Ts}}\int _
                              {0}^{T}e^{-
                              st}f(t)\,dt]
    * Initial_value_theorem:
         f (  0  +   ) =  lim  s &#x2192; &#x221E;    s F ( s )  .
      {\displaystyle f(0^{+})=\lim _{s\to \infty }{sF(s)}.}  [f(0^{+})=\lim _
      {s\to \infty }{sF(s)}.]
    * Final_value_theorem:
         f ( &#x221E; ) =  lim  s &#x2192; 0    s F ( s )    {\displaystyle f
      (\infty )=\lim _{s\to 0}{sF(s)}}  [f(\infty )=\lim _{s\to 0}{sF(s)}], if
      all poles of sF(s) are in the left half-plane.
      The final value theorem is useful because it gives the long-term
      behaviour without having to perform partial_fraction decompositions or
      other difficult algebra. If F(s) has a pole in the right-hand plane or
      poles on the imaginary axis (e.g., if     f ( t ) =  e  t
      {\displaystyle f(t)=e^{t}}  [f(t)=e^{t}] or     f ( t ) = sin &#x2061;
      ( t )   {\displaystyle f(t)=\sin(t)}  [f(t)=\sin(t)]), the behaviour of
      this formula is undefined.
**** Relation to power series[edit] ****
The Laplace transform can be viewed as a continuous analogue of a power_series.
[22] If a(n) is a discrete function of a positive integer n, then the power
series associated to a(n) is the series
          &#x2211;  n = 0   &#x221E;   a ( n )  x  n     {\displaystyle \sum _
      {n=0}^{\infty }a(n)x^{n}}  [\sum _{n=0}^{\infty }a(n)x^{n}]
where x is a real variable (see Z_transform). Replacing summation over n with
integration over t, a continuous version of the power series becomes
          &#x222B;  0   &#x221E;   f ( t )  x  t    d t   {\displaystyle \int _
      {0}^{\infty }f(t)x^{t}\,dt}  [\int _{0}^{\infty }f(t)x^{t}\,dt]
where the discrete function a(n) is replaced by the continuous one f(t).
Changing the base of the power from x to e gives
          &#x222B;  0   &#x221E;   f ( t )   (  e  ln &#x2061;  x    )   t    d
      t   {\displaystyle \int _{0}^{\infty }f(t)\left(e^{\ln {x}}\right)^
      {t}\,dt}  [{\displaystyle \int _{0}^{\infty }f(t)\left(e^{\ln
      {x}}\right)^{t}\,dt}]
For this to converge for, say, all bounded functions f, it is necessary to
require that ln x < 0. Making the substitution −s = ln x gives just the Laplace
transform:
          &#x222B;  0   &#x221E;   f ( t )  e  &#x2212; s t    d t
      {\displaystyle \int _{0}^{\infty }f(t)e^{-st}\,dt}  [\int _{0}^{\infty }f
      (t)e^{-st}\,dt]
In other words, the Laplace transform is a continuous analog of a power series
in which the discrete parameter n is replaced by the continuous parameter t,
and x is replaced by e−s.
**** Relation to moments[edit] ****
Main article: Moment_generating_function
The quantities
          &#x03BC;  n   =  &#x222B;  0   &#x221E;    t  n   f ( t )  d t
      {\displaystyle \mu _{n}=\int _{0}^{\infty }t^{n}f(t)\,dt}  [\mu _{n}=\int
      _{0}^{\infty }t^{n}f(t)\,dt]
are the moments of the function f. If the first n moments of f converge
absolutely, then by repeated differentiation_under_the_integral,
         ( &#x2212; 1  )  n   (   L   f  )  ( n )   ( 0 ) =  &#x03BC;  n   .
      {\displaystyle (-1)^{n}({\mathcal {L}}f)^{(n)}(0)=\mu _{n}.}  [
      {\displaystyle (-1)^{n}({\mathcal {L}}f)^{(n)}(0)=\mu _{n}.}]
This is of special significance in probability theory, where the moments of a
random variable X are given by the expectation values      &#x03BC;  n   = E
&#x2061; [  X  n   ]   {\displaystyle \mu _{n}=\operatorname {E} [X^{n}]}  [
{\displaystyle \mu _{n}=\operatorname {E} [X^{n}]}]. Then, the relation holds
          &#x03BC;  n   = ( &#x2212; 1  )  n      d  n    d  s  n      E
      &#x2061;  [  e  &#x2212; s X   ]  ( 0 ) .   {\displaystyle \mu _{n}=(-1)^
      {n}{\frac {d^{n}}{ds^{n}}}\operatorname {E} \left[e^{-sX}\right](0).}  [
      {\displaystyle \mu _{n}=(-1)^{n}{\frac {d^{n}}{ds^{n}}}\operatorname {E}
      \left[e^{-sX}\right](0).}]
**** Proof of the Laplace transform of a function's derivative[edit] ****
It is often convenient to use the differentiation property of the Laplace
transform to find the transform of a function's derivative. This can be derived
from the basic expression for a Laplace transform as follows:
               L    {  f ( t )  }     =  &#x222B;   0  &#x2212;     &#x221E;
      e  &#x2212; s t   f ( t )  d t       =   [    f ( t )  e  &#x2212; s t
      &#x2212; s    ]    0  &#x2212;     &#x221E;   &#x2212;  &#x222B;   0
      &#x2212;     &#x221E;      e  &#x2212; s t    &#x2212; s     f &#x2032;
      ( t )  d t   (by parts)        =  [  &#x2212;    f (  0  &#x2212;   )
      &#x2212; s     ]  +   1 s     L    {   f &#x2032;  ( t )  }  ,
      {\displaystyle {\begin{aligned}{\mathcal {L}}\left\{f(t)\right\}&=\int _
      {0^{-}}^{\infty }e^{-st}f(t)\,dt\\[6pt]&=\left[{\frac {f(t)e^{-st}}{-
      s}}\right]_{0^{-}}^{\infty }-\int _{0^{-}}^{\infty }{\frac {e^{-st}}{-
      s}}f'(t)\,dt\quad {\text{(by parts)}}\\[6pt]&=\left[-{\frac {f(0^{-})}{-
      s}}\right]+{\frac {1}{s}}{\mathcal {L}}\left\{f'(t)\right\},\end
      {aligned}}}  [{\displaystyle {\begin{aligned}{\mathcal {L}}\left\{f
      (t)\right\}&=\int _{0^{-}}^{\infty }e^{-st}f(t)\,dt\\[6pt]&=\left[{\frac
      {f(t)e^{-st}}{-s}}\right]_{0^{-}}^{\infty }-\int _{0^{-}}^{\infty }{\frac
      {e^{-st}}{-s}}f'(t)\,dt\quad {\text{(by parts)}}\\[6pt]&=\left[-{\frac {f
      (0^{-})}{-s}}\right]+{\frac {1}{s}}{\mathcal {L}}\left\{f'
      (t)\right\},\end{aligned}}}]
yielding
           L   {  f &#x2032;  ( t ) } = s &#x22C5;   L   { f ( t ) } &#x2212; f
      (  0  &#x2212;   ) ,   {\displaystyle {\mathcal {L}}\{f'(t)\}=s\cdot
      {\mathcal {L}}\{f(t)\}-f(0^{-}),}  [{\displaystyle {\mathcal {L}}\{f'
      (t)\}=s\cdot {\mathcal {L}}\{f(t)\}-f(0^{-}),}]
and in the bilateral case,
           L   {  f &#x2032;  ( t ) } = s  &#x222B;  &#x2212; &#x221E;
      &#x221E;    e  &#x2212; s t   f ( t )  d t = s &#x22C5;   L   { f ( t ) }
      .   {\displaystyle {\mathcal {L}}\{f'(t)\}=s\int _{-\infty }^{\infty }e^
      {-st}f(t)\,dt=s\cdot {\mathcal {L}}\{f(t)\}.}  [{\displaystyle {\mathcal
      {L}}\{f'(t)\}=s\int _{-\infty }^{\infty }e^{-st}f(t)\,dt=s\cdot {\mathcal
      {L}}\{f(t)\}.}]
The general result
           L    {   f  ( n )   ( t )  }  =  s  n   &#x22C5;   L   { f ( t ) }
      &#x2212;  s  n &#x2212; 1   f (  0  &#x2212;   ) &#x2212; &#x22EF;
      &#x2212;  f  ( n &#x2212; 1 )   (  0  &#x2212;   ) ,   {\displaystyle
      {\mathcal {L}}\left\{f^{(n)}(t)\right\}=s^{n}\cdot {\mathcal {L}}\{f
      (t)\}-s^{n-1}f(0^{-})-\cdots -f^{(n-1)}(0^{-}),}  [{\displaystyle
      {\mathcal {L}}\left\{f^{(n)}(t)\right\}=s^{n}\cdot {\mathcal {L}}\{f
      (t)\}-s^{n-1}f(0^{-})-\cdots -f^{(n-1)}(0^{-}),}]
where      f  ( n )     {\displaystyle f^{(n)}}  [f^{(n)}] denotes the nth
derivative of f, can then be established with an inductive argument.
**** Evaluating integrals over the positive real axis[edit] ****
A useful property of the Laplace transform is the following:
          &#x222B;  0   &#x221E;   f ( x ) g ( x )  d x =  &#x222B;  0
      &#x221E;   (   L   f ) ( s ) &#x22C5; (    L    &#x2212; 1   g ) ( s )  d
      s   {\displaystyle \int _{0}^{\infty }f(x)g(x)\,dx=\int _{0}^{\infty }(
      {\mathcal {L}}f)(s)\cdot ({\mathcal {L}}^{-1}g)(s)\,ds}  [{\displaystyle
      \int _{0}^{\infty }f(x)g(x)\,dx=\int _{0}^{\infty }({\mathcal {L}}f)
      (s)\cdot ({\mathcal {L}}^{-1}g)(s)\,ds}]
under suitable assumptions on the behaviour of     f , g   {\displaystyle f,g}
[f,g] in a right neighbourhood of     0   {\displaystyle 0}  [{\displaystyle
0}] and on the decay rate of     f , g   {\displaystyle f,g}  [f,g] in a left
neighbourhood of     &#x221E;   {\displaystyle \infty }  [\infty ]. The above
formula is a variation of integration_by_parts, with the operators       d  d x
{\displaystyle {\frac {d}{dx}}}  [{\frac {d}{dx}}] and     &#x222B;  d x
{\displaystyle \int \,dx}  [{\displaystyle \int \,dx}] being replaced by
L     {\displaystyle {\mathcal {L}}}  [{\mathcal {L}}] and        L    &#x2212;
1     {\displaystyle {\mathcal {L}}^{-1}}  [{\displaystyle {\mathcal {L}}^{-
1}}]. Let us prove the equivalent formulation:
          &#x222B;  0   &#x221E;   (   L   f ) ( x ) g ( x )  d x =  &#x222B;
      0   &#x221E;   f ( s ) (   L   g ) ( s )  d s .   {\displaystyle \int _
      {0}^{\infty }({\mathcal {L}}f)(x)g(x)\,dx=\int _{0}^{\infty }f(s)(
      {\mathcal {L}}g)(s)\,ds.}  [{\displaystyle \int _{0}^{\infty }({\mathcal
      {L}}f)(x)g(x)\,dx=\int _{0}^{\infty }f(s)({\mathcal {L}}g)(s)\,ds.}]
By plugging in     (   L   f ) ( x ) =  &#x222B;  0   &#x221E;   f ( s )  e
&#x2212; s x    d s   {\displaystyle ({\mathcal {L}}f)(x)=\int _{0}^{\infty }f
(s)e^{-sx}\,ds}  [{\displaystyle ({\mathcal {L}}f)(x)=\int _{0}^{\infty }f(s)e^
{-sx}\,ds}] the left-hand side turns into:
          &#x222B;  0   &#x221E;    &#x222B;  0   &#x221E;   f ( s ) g ( x )  e
      &#x2212; s x    d s  d x ,   {\displaystyle \int _{0}^{\infty }\int _{0}^
      {\infty }f(s)g(x)e^{-sx}\,ds\,dx,}  [{\displaystyle \int _{0}^{\infty
      }\int _{0}^{\infty }f(s)g(x)e^{-sx}\,ds\,dx,}]
but assuming Fubini's theorem holds, by reversing the order of integration we
get the wanted right-hand side.
**** Relationship to other transforms[edit] ****
*** LaplaceâStieltjes transform[edit] ***
The (unilateral) LaplaceâStieltjes_transform of a function g : R â R is
defined by the LebesgueâStieltjes_integral
         {    L    &#x2217;   g } ( s ) =  &#x222B;  0   &#x221E;    e
      &#x2212; s t    d g ( t ) .   {\displaystyle \{{\mathcal {L}}^{*}g\}
      (s)=\int _{0}^{\infty }e^{-st}\,dg(t).}  [{\displaystyle \{{\mathcal
      {L}}^{*}g\}(s)=\int _{0}^{\infty }e^{-st}\,dg(t).}]
The function g is assumed to be of bounded_variation. If g is the
antiderivative of f:
         g ( x ) =  &#x222B;  0   x   f ( t )  d t   {\displaystyle g(x)=\int _
      {0}^{x}f(t)\,dt}  [g(x)=\int _{0}^{x}f(t)\,dt]
then the LaplaceâStieltjes transform of g and the Laplace transform of f
coincide. In general, the LaplaceâStieltjes transform is the Laplace
transform of the Stieltjes_measure associated to g. So in practice, the only
distinction between the two transforms is that the Laplace transform is thought
of as operating on the density function of the measure, whereas the
LaplaceâStieltjes transform is thought of as operating on its cumulative
distribution_function.[23]
*** Fourier transform[edit] ***
The continuous_Fourier_transform is equivalent to evaluating the bilateral
Laplace transform with imaginary argument s = iÏ or s = 2Ïfi[24] when the
condition explained below is fulfilled,
                f &#x005E;    ( &#x03C9; )    =   F   { f ( t ) }       =   L
      { f ( t ) }   |   s = i &#x03C9;   = F ( s )   |   s = i &#x03C9;
      =  &#x222B;  &#x2212; &#x221E;   &#x221E;    e  &#x2212; i &#x03C9; t   f
      ( t )  d t &#xA0; .       {\displaystyle {\begin{aligned}{\widehat {f}}
      (\omega )&={\mathcal {F}}\{f(t)\}\\[4pt]&={\mathcal {L}}\{f(t)\}|_
      {s=i\omega }=F(s)|_{s=i\omega }\\[4pt]&=\int _{-\infty }^{\infty }e^{-
      i\omega t}f(t)\,dt~.\end{aligned}}}  [{\displaystyle {\begin{aligned}
      {\widehat {f}}(\omega )&={\mathcal {F}}\{f(t)\}\\[4pt]&={\mathcal {L}}\{f
      (t)\}|_{s=i\omega }=F(s)|_{s=i\omega }\\[4pt]&=\int _{-\infty }^{\infty
      }e^{-i\omega t}f(t)\,dt~.\end{aligned}}}]
This definition of the Fourier transform requires a prefactor of 1/2 Ï on the
reverse Fourier transform. This relationship between the Laplace and Fourier
transforms is often used to determine the frequency_spectrum of a signal or
dynamical_system.
The above relation is valid as stated if and only if the region of convergence
(ROC) of F(s) contains the imaginary axis, Ï = 0.
For example, the function f(t) = cos(Ï0t) has a Laplace transform F(s) = s/(s2
+ Ï02) whose ROC is Re(s) > 0. As s = iÏ is a pole of F(s), substituting s =
iÏ in F(s) does not yield the Fourier transform of f(t)u(t), which is
proportional to the Dirac_delta-function Î´(Ï â Ï0).
However, a relation of the form
          lim  &#x03C3; &#x2192;  0  +     F ( &#x03C3; + i &#x03C9; ) =    f
      &#x005E;    ( &#x03C9; )   {\displaystyle \lim _{\sigma \to 0^{+}}F
      (\sigma +i\omega )={\widehat {f}}(\omega )}  [{\displaystyle \lim _
      {\sigma \to 0^{+}}F(\sigma +i\omega )={\widehat {f}}(\omega )}]
holds under much weaker conditions. For instance, this holds for the above
example provided that the limit is understood as a weak_limit of measures (see
vague_topology). General conditions relating the limit of the Laplace transform
of a function on the boundary to the Fourier transform take the form of
PaleyâWiener_theorems.
*** Mellin transform[edit] ***
The Mellin_transform and its inverse are related to the two-sided Laplace
transform by a simple change of variables.
If in the Mellin transform
         G ( s ) =   M   { g ( &#x03B8; ) } =  &#x222B;  0   &#x221E;
      &#x03B8;  s   g ( &#x03B8; )     d &#x03B8;  &#x03B8;     {\displaystyle
      G(s)={\mathcal {M}}\{g(\theta )\}=\int _{0}^{\infty }\theta ^{s}g(\theta
      )\,{\frac {d\theta }{\theta }}}  [{\displaystyle G(s)={\mathcal {M}}\{g
      (\theta )\}=\int _{0}^{\infty }\theta ^{s}g(\theta )\,{\frac {d\theta }
      {\theta }}}]
we set Î¸ = eât we get a two-sided Laplace transform.
*** Z-transform[edit] ***
The unilateral or one-sided Z-transform is simply the Laplace transform of an
ideally sampled signal with the substitution of
         z       =      d e f       e  s T   ,   {\displaystyle z{\stackrel
      {\mathrm {def} }{{}={}}}e^{sT},}  [{\displaystyle z{\stackrel {\mathrm
      {def} }{{}={}}}e^{sT},}]
where T = 1/fs is the sampling period (in units of time e.g., seconds) and fs
is the sampling_rate (in samples_per_second or hertz).
Let
          &#x0394;  T   ( t ) &#xA0;     =    d e f      &#xA0;  &#x2211;  n =
      0   &#x221E;   &#x03B4; ( t &#x2212; n T )   {\displaystyle \Delta _{T}
      (t)\ {\stackrel {\mathrm {def} }{=}}\ \sum _{n=0}^{\infty }\delta (t-nT)}
      [\Delta _{T}(t)\ {\stackrel {\mathrm {def} }{=}}\ \sum _{n=0}^{\infty
      }\delta (t-nT)]
be a sampling impulse train (also called a Dirac_comb) and
              x  q   ( t ) &#xA0;        =    d e f      &#xA0; x ( t )
      &#x0394;  T   ( t ) = x ( t )  &#x2211;  n = 0   &#x221E;   &#x03B4; ( t
      &#x2212; n T )       =  &#x2211;  n = 0   &#x221E;   x ( n T ) &#x03B4;
      ( t &#x2212; n T ) =  &#x2211;  n = 0   &#x221E;   x [ n ] &#x03B4; ( t
      &#x2212; n T )       {\displaystyle {\begin{aligned}x_{q}(t)\ &{\stackrel
      {\mathrm {def} }{=}}\ x(t)\Delta _{T}(t)=x(t)\sum _{n=0}^{\infty }\delta
      (t-nT)\\&=\sum _{n=0}^{\infty }x(nT)\delta (t-nT)=\sum _{n=0}^{\infty }x
      [n]\delta (t-nT)\end{aligned}}}  [{\begin{aligned}x_{q}(t)\ &{\stackrel
      {\mathrm {def} }{=}}\ x(t)\Delta _{T}(t)=x(t)\sum _{n=0}^{\infty }\delta
      (t-nT)\\&=\sum _{n=0}^{\infty }x(nT)\delta (t-nT)=\sum _{n=0}^{\infty }x
      [n]\delta (t-nT)\end{aligned}}]
be the sampled representation of the continuous-time x(t)
         x [ n ]       =      d e f      x ( n T ) &#xA0; .   {\displaystyle x
      [n]{\stackrel {\mathrm {def} }{{}={}}}x(nT)~.}  [{\displaystyle x[n]
      {\stackrel {\mathrm {def} }{{}={}}}x(nT)~.}]
The Laplace transform of the sampled signal xq(t) is
              X  q   ( s )    =  &#x222B;   0  &#x2212;     &#x221E;    x  q
      ( t )  e  &#x2212; s t    d t       =  &#x222B;   0  &#x2212;
      &#x221E;    &#x2211;  n = 0   &#x221E;   x [ n ] &#x03B4; ( t &#x2212; n
      T )  e  &#x2212; s t    d t       =  &#x2211;  n = 0   &#x221E;   x [ n ]
      &#x222B;   0  &#x2212;     &#x221E;   &#x03B4; ( t &#x2212; n T )  e
      &#x2212; s t    d t       =  &#x2211;  n = 0   &#x221E;   x [ n ]  e
      &#x2212; n s T   &#xA0; .       {\displaystyle {\begin{aligned}X_{q}
      (s)&=\int _{0^{-}}^{\infty }x_{q}(t)e^{-st}\,dt\\&=\int _{0^{-}}^{\infty
      }\sum _{n=0}^{\infty }x[n]\delta (t-nT)e^{-st}\,dt\\&=\sum _{n=0}^{\infty
      }x[n]\int _{0^{-}}^{\infty }\delta (t-nT)e^{-st}\,dt\\&=\sum _{n=0}^
      {\infty }x[n]e^{-nsT}~.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}X_{q}(s)&=\int _{0^{-}}^{\infty }x_{q}(t)e^{-st}\,dt\\&=\int _
      {0^{-}}^{\infty }\sum _{n=0}^{\infty }x[n]\delta (t-nT)e^{-
      st}\,dt\\&=\sum _{n=0}^{\infty }x[n]\int _{0^{-}}^{\infty }\delta (t-
      nT)e^{-st}\,dt\\&=\sum _{n=0}^{\infty }x[n]e^{-nsT}~.\end{aligned}}}]
This is the precise definition of the unilateral Z-transform of the discrete
function x[n]
         X ( z ) =  &#x2211;  n = 0   &#x221E;   x [ n ]  z  &#x2212; n
      {\displaystyle X(z)=\sum _{n=0}^{\infty }x[n]z^{-n}}  [X(z)=\sum _{n=0}^
      {\infty }x[n]z^{-n}]
with the substitution of z â esT.
Comparing the last two equations, we find the relationship between the
unilateral Z-transform and the Laplace transform of the sampled signal,
          X  q   ( s ) = X ( z )    |    z =  e  s T     .   {\displaystyle X_
      {q}(s)=X(z){\Big |}_{z=e^{sT}}.}  [X_{q}(s)=X(z){\Big |}_{z=e^{sT}}.]
The similarity between the Z and Laplace transforms is expanded upon in the
theory of time_scale_calculus.
*** Borel transform[edit] ***
The integral form of the Borel_transform
         F ( s ) =  &#x222B;  0   &#x221E;   f ( z )  e  &#x2212; s z    d z
      {\displaystyle F(s)=\int _{0}^{\infty }f(z)e^{-sz}\,dz}  [F(s)=\int _{0}^
      {\infty }f(z)e^{-sz}\,dz]
is a special case of the Laplace transform for f an entire_function of
exponential_type, meaning that
          |  f ( z )  |  &#x2264; A  e  B  |  z  |      {\displaystyle |f
      (z)|\leq Ae^{B|z|}}  [|f(z)|\leq Ae^{B|z|}]
for some constants A and B. The generalized Borel transform allows a different
weighting function to be used, rather than the exponential function, to
transform functions not of exponential type. Nachbin's_theorem gives necessary
and sufficient conditions for the Borel transform to be well defined.
*** Fundamental relationships[edit] ***
Since an ordinary Laplace transform can be written as a special case of a two-
sided transform, and since the two-sided transform can be written as the sum of
two one-sided transforms, the theory of the Laplace-, Fourier-, Mellin-, and Z-
transforms are at bottom the same subject. However, a different point of view
and different characteristic problems are associated with each of these four
major integral transforms.
***** Table of selected Laplace transforms[edit] *****
Main article: List_of_Laplace_transforms
The following table provides Laplace transforms for many common functions of a
single variable.[25][26] For definitions and explanations, see the Explanatory
Notes at the end of the table.
Because the Laplace transform is a linear operator,
    * The Laplace transform of a sum is the sum of Laplace transforms of each
      term.
                 L   { f ( t ) + g ( t ) } =   L   { f ( t ) } +   L   { g ( t
            ) }   {\displaystyle {\mathcal {L}}\{f(t)+g(t)\}={\mathcal {L}}\{f
            (t)\}+{\mathcal {L}}\{g(t)\}}  [{\mathcal {L}}\{f(t)+g(t)\}=
            {\mathcal {L}}\{f(t)\}+{\mathcal {L}}\{g(t)\}]
    * The Laplace transform of a multiple of a function is that multiple times
      the Laplace transformation of that function.
                 L   { a f ( t ) } = a   L   { f ( t ) }   {\displaystyle
            {\mathcal {L}}\{af(t)\}=a{\mathcal {L}}\{f(t)\}}  [{\mathcal {L}}\
            {af(t)\}=a{\mathcal {L}}\{f(t)\}]
Using this linearity, and various trigonometric, hyperbolic, and complex_number
(etc.) properties and/or identities, some Laplace transforms can be obtained
from others more quickly than by using the definition directly.
The unilateral Laplace transform takes as input a function whose time domain is
the non-negative reals, which is why all of the time domain functions in the
table below are multiples of the Heaviside_step_function, u(t).
The entries of the table that involve a time delay Ï are required to be causal
(meaning that Ï > 0). A causal system is a system where the impulse_response h
(t) is zero for all time t prior to t = 0. In general, the region of
convergence for causal systems is not the same as that of anticausal_systems.
              Time domain
                  f ( t ) =  Laplace s-
              L    &#x2212;  domain
              1   { F ( s )      F ( s ) =
              }              L   { f ( t ) }
Function      {\displaystyle {\displaystyle  Region of          Reference
              f(t)={\mathcal F(s)={\mathcal  convergence
              {L}}^{-1}\{F   {L}}\{f(t)\}}
              (s)\}}  [f(t)= [F(s)={\mathcal
              {\mathcal      {L}}\{f(t)\}]
              {L}}^{-1}\{F
              (s)\}]
                 &#x03B4;
              ( t ) &#xA0;      1
unit_impulse  {\displaystyle {\displaystyle  all s              inspection
              \delta (t)\ }  1}  [1]
              [\delta (t)\ ]
                 &#x03B4;
              ( t &#x2212;       e  &#x2212;
              &#x03C4; )     &#x03C4; s
delayed       &#xA0;         &#xA0;                             time shift of
impulse       {\displaystyle {\displaystyle                     unit impulse
              \delta (t-\tau e^{-\tau s}\ }
              )\ }  [\delta  [e^{-\tau s}\ ]
              (t-\tau )\ ]
                 u ( t )          1 s
              &#xA0;         {\displaystyle
unit_step     {\displaystyle {1 \over s}}  [ Re(s) > 0          integrate unit impulse
              u(t)\ }  [u    {1 \over s}]
              (t)\ ]
                                  1 s    e
                             &#x2212;
                 u ( t       &#x03C4; s
              &#x2212;       {\displaystyle
delayed unit  &#x03C4; )     {\frac {1}                         time shift of
step          &#xA0;         {s}}e^{-\tau    Re(s) > 0          unit step
              {\displaystyle s}}  [
              u(t-\tau )\ }  {\displaystyle
              [u(t-\tau )\ ] {\frac {1}
                             {s}}e^{-\tau
                             s}}]
                 t &#x22C5;       1  s  2
              u ( t ) &#xA0; {\displaystyle
              {\displaystyle {\frac {1}{s^                      integrate unit
ramp          t\cdot u(t)\ } {2}}}}  [       Re(s) > 0          impulse twice
              [t\cdot u(t)\  {\displaystyle
              ]              {\frac {1}{s^
                             {2}}}}]
                  t  n             n !   s
              &#x22C5; u ( t n + 1
nth power     )              {\displaystyle  Re(s) > 0          Integrate unit
(for integer  {\displaystyle {n! \over s^    (n > â1)      step n times
n)            t^{n}\cdot u   {n+1}}}  [{n!
              (t)}  [t^      \over s^{n+1}}]
              {n}\cdot u(t)]
                  t  q             &#x0393;
              &#x22C5; u ( t ( q + 1 )   s
qth power     )              q + 1
(for complex  {\displaystyle {\displaystyle  Re(s) > 0          [27][28]
q)            t^{q}\cdot u   {\Gamma (q+1)   Re(q) > â1
              (t)}  [t^      \over s^{q+1}}}
              {q}\cdot u(t)] [{\Gamma (q+1)
                             \over s^{q+1}}]
                                  1  s    1
                             n   + 1
                             &#x0393;
                             (    1 n   + 1
                             )
                   t  n      {\displaystyle
              &#x22C5; u ( t {1 \over s^{
              )              {\frac {1}
              {\displaystyle {n}}+1}}\Gamma
nth root      {\sqrt[{n}]    \left({\frac    Re(s) > 0          Set q = 1/n above.
              {t}}\cdot u    {1}
              (t)}  [{\sqrt[ {n}}+1\right)}
              {n}]{t}}\cdot  [{\displaystyle
              u(t)]          {1 \over s^{
                             {\frac {1}
                             {n}}+1}}\Gamma
                             \left({\frac
                             {1}
                             {n}}+1\right)}]
                  t  n    e        n !   ( s
              &#x2212;       + &#x03B1;  )
              &#x03B1; t     n + 1
nth power     &#x22C5; u ( t {\displaystyle
with          )              {\frac {n!}{                       Integrate unit step,
frequency     {\displaystyle (s+\alpha )^    Re(s) > âÎ± apply frequency shift
shift         t^{n}e^{-      {n+1}}}}  [
              \alpha t}\cdot {\frac {n!}{
              u(t)}  [t^     (s+\alpha )^
              {n}e^{-\alpha  {n+1}}}]
              t}\cdot u(t)]
                 ( t
              &#x2212;
              &#x03C4;  )  n       n !
              e  &#x2212;    &#x22C5;  e
              &#x03B1; ( t   &#x2212;
              &#x2212;       &#x03C4; s
              &#x03C4; )     ( s + &#x03B1;
delayed nth   &#x22C5; u ( t )  n + 1
power         &#x2212;       {\displaystyle                     Integrate unit step,
with          &#x03C4; )     {\frac {n!\cdot Re(s) > âÎ± apply frequency shift,
frequency     {\displaystyle e^{-\tau s}}{                      apply time shift
shift         (t-\tau )^     (s+\alpha )^
              {n}e^{-\alpha  {n+1}}}}  [
              (t-\tau        {\frac {n!\cdot
              )}\cdot u(t-   e^{-\tau s}}{
              \tau )}  [(t-  (s+\alpha )^
              \tau )^{n}e^{- {n+1}}}]
              \alpha (t-\tau
              )}\cdot u(t-
              \tau )]
                  e
              &#x2212;            1  s +
              &#x03B1; t     &#x03B1;
              &#x22C5; u ( t {\displaystyle
exponential   )              {1 \over        Re(s) > âÎ± Frequency shift of
decay         {\displaystyle s+\alpha }}  [                     unit step
              e^{-\alpha     {1 \over
              t}\cdot u(t)}  s+\alpha }]
              [e^{-\alpha
              t}\cdot u(t)]
                                   2
                  e          &#x03B1;
two-sided     &#x2212;       &#x03B1;  2
exponential   &#x03B1;  |  t &#x2212;  s  2
decay         |    &#xA0;    {\displaystyle                     Frequency shift of
(only for     {\displaystyle {2\alpha \over  âÎ± < Re(s) unit step
bilateral     e^{-\alpha     \alpha ^{2}-s^
transform)    |t|}\ }  [e^{- {2}}}  [
              \alpha |t|}\ ] {2\alpha  \over
                             \alpha ^{2}-s^
                             {2}}]
                 ( 1
              &#x2212;  e
              &#x2212;            &#x03B1;
              &#x03B1; t   ) s ( s +
              &#x22C5; u ( t &#x03B1; )
exponential   ) &#xA0;       {\displaystyle                     Unit step minus
approach      {\displaystyle {\frac {\alpha  Re(s) > 0          exponential decay
              (1-e^{-\alpha  }{s(s+\alpha
              t})\cdot u(t)\ )}}}  [{\frac
              }  [(1-e^{-    {\alpha }{s
              \alpha         (s+\alpha )}}]
              t})\cdot u(t)\
              ]
                 sin
              &#x2061;            &#x03C9;
              ( &#x03C9; t ) s  2   +
              &#x22C5; u ( t &#x03C9;  2
              ) &#xA0;       {\displaystyle
sine          {\displaystyle {\omega \over   Re(s) > 0          Bracewell_1978, p. 227
              \sin(\omega    s^{2}+\omega ^
              t)\cdot u(t)\  {2}}}  [{\omega
              }  [\sin       \over s^
              (\omega        {2}+\omega ^
              t)\cdot u(t)\  {2}}]
              ]
                 cos
              &#x2061;            s   s  2
              ( &#x03C9; t ) +  &#x03C9;  2
              &#x22C5; u ( t {\displaystyle
              ) &#xA0;       {s \over s^
cosine        {\displaystyle {2}+\omega ^    Re(s) > 0          Bracewell_1978, p. 227
              \cos(\omega    {2}}}  [{s
              t)\cdot u(t)\  \over s^
              }  [\cos       {2}+\omega ^
              (\omega        {2}}]
              t)\cdot u(t)\
              ]
                 sinh
              &#x2061;            &#x03B1;
              ( &#x03B1; t ) s  2   &#x2212;
              &#x22C5; u ( t &#x03B1;  2
              ) &#xA0;       {\displaystyle
hyperbolic    {\displaystyle {\alpha \over   Re(s) > |Î±|     Williams_1973, p. 88
sine          \sinh(\alpha   s^{2}-\alpha ^
              t)\cdot u(t)\  {2}}}  [{\alpha
              }  [\sinh      \over s^{2}-
              (\alpha        \alpha ^{2}}]
              t)\cdot u(t)\
              ]
                 cosh
              &#x2061;            s   s  2
              ( &#x03B1; t ) &#x2212;
              &#x22C5; u ( t &#x03B1;  2
              ) &#xA0;       {\displaystyle
hyperbolic    {\displaystyle {s \over s^{2}- Re(s) > |Î±|     Williams_1973, p. 88
cosine        \cosh(\alpha   \alpha ^{2}}}
              t)\cdot u(t)\  [{s \over s^
              }  [\cosh      {2}-\alpha ^
              (\alpha        {2}}]
              t)\cdot u(t)\
              ]
                  e
              &#x2212;            &#x03C9;
              &#x03B1; t     ( s + &#x03B1;
              sin &#x2061;   )  2   +
              ( &#x03C9; t ) &#x03C9;  2
              &#x22C5; u ( t {\displaystyle
exponentially ) &#xA0;       {\omega \over
decaying      {\displaystyle (s+\alpha )^    Re(s) > âÎ± Bracewell_1978, p. 227
sine wave     e^{-\alpha     {2}+\omega ^
              t}\sin(\omega  {2}}}  [{\omega
              t)\cdot u(t)\  \over (s+\alpha
              }  [e^{-\alpha )^{2}+\omega ^
              t}\sin(\omega  {2}}]
              t)\cdot u(t)\
              ]
                  e                s +
              &#x2212;       &#x03B1;   ( s
              &#x03B1; t     + &#x03B1;  )
              cos &#x2061;   2   +  &#x03C9;
              ( &#x03C9; t ) 2
              &#x22C5; u ( t {\displaystyle
exponentially ) &#xA0;       {s+\alpha \over
decaying      {\displaystyle (s+\alpha )^    Re(s) > âÎ± Bracewell_1978, p. 227
cosine wave   e^{-\alpha     {2}+\omega ^
              t}\cos(\omega  {2}}}  [
              t)\cdot u(t)\  {s+\alpha
              }  [e^{-\alpha \over (s+\alpha
              t}\cos(\omega  )^{2}+\omega ^
              t)\cdot u(t)\  {2}}]
              ]
                                &#x2212;   1
                             s     [  ln
                 ln &#x2061; &#x2061; ( s )
              ( t ) &#x22C5; + &#x03B3;  ]
              u ( t )        {\displaystyle
natural       {\displaystyle -{1 \over       Re(s) > 0          Williams_1973, p. 88
logarithm     \ln(t)\cdot u  s}\,\left[\ln
              (t)}  [\ln     (s)+\gamma
              (t)\cdot u(t)] \right]}  [-{1
                             \over s}\,\left
                             [\ln(s)+\gamma
                             \right]]
                                    (     s
                             2   +  &#x03C9;
                             2     &#x2212;
                             s  )   n
                             &#x03C9;  n
                             s  2   +
                             &#x03C9;  2
                             {\displaystyle
                  J  n       {\frac {\left(
              ( &#x03C9; t ) {\sqrt {s^
Bessel        &#x22C5; u ( t {2}+\omega ^
function      )              {2}}}-s\right)^ Re(s) > 0
of the first  {\displaystyle {n}}{\omega ^   (n > â1)      Williams_1973, p. 89
kind,         J_{n}(\omega   {n}{\sqrt {s^
of order n    t)\cdot u(t)}  {2}+\omega ^
              [J_{n}(\omega  {2}}}}}}  [
              t)\cdot u(t)]  {\displaystyle
                             {\frac {\left(
                             {\sqrt {s^
                             {2}+\omega ^
                             {2}}}-s\right)^
                             {n}}{\omega ^
                             {n}{\sqrt {s^
                             {2}+\omega ^
                             {2}}}}}}]
                                  1 s    e
                             ( 1  /  4 )  s
                             2      (  1
                             &#x2212; erf
                 erf         &#x2061;   s 2
              &#x2061; ( t ) )
              &#x22C5; u ( t {\displaystyle
              )              {\frac {1}
              {\displaystyle {s}}e^{(1/4)s^
Error         \operatorname  {2}}\left(1-
function      {erf} (t)\cdot \operatorname   Re(s) > 0          Williams_1973, p. 89
              u(t)}  [       {erf} {\frac
              {\displaystyle {s}{2}}\right)}
              \operatorname  [{\displaystyle
              {erf} (t)\cdot {\frac {1}
              u(t)}]         {s}}e^{(1/4)s^
                             {2}}\left(1-
                             \operatorname
                             {erf} {\frac
                             {s}
                             {2}}\right)}]
Explanatory notes:
                                                    * t, a real number, typically represents time,
    * u(t) represents the Heaviside_step
      function.                                       although it can represent any independent
    * Î´ represents the Dirac_delta_function.       dimension.
    * Î(z) represents the Gamma_function.        * s is the complex frequency domain parameter,
    * Î³ is the Euler–Mascheroni_constant.        and Re(s) is its real_part.
                                                    * Î±, Î², Ï, and Ï are real_numbers.
                                                    * n is an integer.
***** s-domain equivalent circuits and impedances[edit] *****
The Laplace transform is often used in circuit analysis, and simple conversions
to the s-domain of circuit elements can be made. Circuit elements can be
transformed into impedances, very similar to phasor impedances.
Here is a summary of equivalents:
      [s-domain_equivalent_circuits]
Note that the resistor is exactly the same in the time domain and the s-domain.
The sources are put in if there are initial conditions on the circuit elements.
For example, if a capacitor has an initial voltage across it, or if the
inductor has an initial current through it, the sources inserted in the s-
domain account for that.
The equivalents for current and voltage sources are simply derived from the
transformations in the table above.
***** Examples and applications[edit] *****
The Laplace transform is used frequently in engineering and physics; the output
of a linear_time-invariant system can be calculated by convolving its unit
impulse_response with the input signal. Performing this calculation in Laplace
space turns the convolution into a multiplication; the latter being easier to
solve because of its algebraic form. For more information, see control_theory.
The Laplace transform can also be used to solve_differential_equations and is
used extensively in mechanical_engineering and electrical_engineering. The
Laplace transform reduces a linear differential_equation to an algebraic
equation, which can then be solved by the formal rules of algebra. The original
differential equation can then be solved by applying the inverse Laplace
transform. The English electrical engineer Oliver_Heaviside first proposed a
similar scheme, although without using the Laplace transform; and the resulting
operational_calculus is credited as the Heaviside calculus.
**** Evaluating improper integrals[edit] ****
Let       L    {  f ( t )  }  = F ( s )   {\displaystyle {\mathcal {L}}\left\{f
(t)\right\}=F(s)}  [{\mathcal {L}}\left\{f(t)\right\}=F(s)], then (see the
table above)
           L    {    f ( t )  t   }  =  &#x222B;  s   &#x221E;   F ( p )  d p ,
      {\displaystyle {\mathcal {L}}\left\{{\frac {f(t)}{t}}\right\}=\int _{s}^
      {\infty }F(p)\,dp,}  [{\displaystyle {\mathcal {L}}\left\{{\frac {f(t)}
      {t}}\right\}=\int _{s}^{\infty }F(p)\,dp,}]
or
          &#x222B;  0   &#x221E;      f ( t )  t    e  &#x2212; s t    d t =
      &#x222B;  s   &#x221E;   F ( p )  d p .   {\displaystyle \int _{0}^
      {\infty }{\frac {f(t)}{t}}e^{-st}\,dt=\int _{s}^{\infty }F(p)\,dp.}
      [\int _{0}^{\infty }{\frac {f(t)}{t}}e^{-st}\,dt=\int _{s}^{\infty }F
      (p)\,dp.]
Letting s â 0, gives one the identity
          &#x222B;  0   &#x221E;      f ( t )  t    d t =  &#x222B;  0
      &#x221E;   F ( p )  d p .   {\displaystyle \int _{0}^{\infty }{\frac {f
      (t)}{t}}\,dt=\int _{0}^{\infty }F(p)\,dp.}  [{\displaystyle \int _{0}^
      {\infty }{\frac {f(t)}{t}}\,dt=\int _{0}^{\infty }F(p)\,dp.}]
provided that the interchange of limits can be justified. Even when the
interchange cannot be justified the calculation can be suggestive. For example,
with a â  0 â  b, proceeding formally one has
                &#x222B;  0   &#x221E;     1 t   ( cos &#x2061; ( a t )
      &#x2212; cos &#x2061; ( b t ) )  d t =  &#x222B;  0   &#x221E;    (    p
      p  2   +  a  2      &#x2212;   p   p  2   +  b  2       )   d p     =
      1 2       ln &#x2061;     p  2   +  a  2      p  2   +  b  2       |   p
      :=  0   &#x221E;   = ln &#x2061;  |  b  |  &#x2212; ln &#x2061;  |  a  |
      .       {\displaystyle {\begin{aligned}&\int _{0}^{\infty }{\frac {1}{t}}
      (\cos(at)-\cos(bt))\,dt=\int _{0}^{\infty }\left({\frac {p}{p^{2}+a^
      {2}}}-{\frac {p}{p^{2}+b^{2}}}\right)\,dp\\[6pt]={}&{\frac {1}
      {2}}\left.\ln {\frac {p^{2}+a^{2}}{p^{2}+b^{2}}}\right|_{p\,:=\,0}^
      {\infty }=\ln |b|-\ln |a|.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}&\int _{0}^{\infty }{\frac {1}{t}}(\cos(at)-\cos(bt))\,dt=\int _
      {0}^{\infty }\left({\frac {p}{p^{2}+a^{2}}}-{\frac {p}{p^{2}+b^
      {2}}}\right)\,dp\\[6pt]={}&{\frac {1}{2}}\left.\ln {\frac {p^{2}+a^{2}}
      {p^{2}+b^{2}}}\right|_{p\,:=\,0}^{\infty }=\ln |b|-\ln |a|.\end
      {aligned}}}]
The validity of this identity can be proved by other means. It is an example of
a Frullani_integral.
Another example is Dirichlet_integral.
**** Nuclear physics[edit] ****
In nuclear_physics, the following fundamental relationship governs radioactive
decay: the number of radioactive atoms N in a sample of a radioactive isotope
decays at a rate proportional to N. This leads to the first order linear
differential equation
            d N   d t    = &#x2212; &#x03BB; N ,   {\displaystyle {\frac {dN}
      {dt}}=-\lambda N,}  [{\frac {dN}{dt}}=-\lambda N,]
where Î» is the decay_constant. The Laplace transform can be used to solve this
equation.
Rearranging the equation to one side, we have
            d N   d t    + &#x03BB; N = 0.   {\displaystyle {\frac {dN}
      {dt}}+\lambda N=0.}  [{\frac {dN}{dt}}+\lambda N=0.]
Next, we take the Laplace transform of both sides of the equation:
          (  s    N &#x007E;    ( s ) &#x2212;  N  0    )  + &#x03BB;    N
      &#x007E;    ( s ) = 0 ,   {\displaystyle \left(s{\widetilde {N}}(s)-N_
      {0}\right)+\lambda {\widetilde {N}}(s)=0,}  [{\displaystyle \left(s
      {\widetilde {N}}(s)-N_{0}\right)+\lambda {\widetilde {N}}(s)=0,}]
where
            N &#x007E;    ( s ) =   L   { N ( t ) }   {\displaystyle
      {\widetilde {N}}(s)={\mathcal {L}}\{N(t)\}}  [{\displaystyle {\widetilde
      {N}}(s)={\mathcal {L}}\{N(t)\}}]
and
          N  0   = N ( 0 ) .   {\displaystyle N_{0}=N(0).}  [{\displaystyle N_
      {0}=N(0).}]
Solving, we find
            N &#x007E;    ( s ) =    N  0    s + &#x03BB;    .   {\displaystyle
      {\widetilde {N}}(s)={\frac {N_{0}}{s+\lambda }}.}  [{\displaystyle
      {\widetilde {N}}(s)={\frac {N_{0}}{s+\lambda }}.}]
Finally, we take the inverse Laplace transform to find the general solution
             N ( t )    =    L    &#x2212; 1   {    N &#x007E;    ( s ) } =
      L    &#x2212; 1     {    N  0    s + &#x03BB;    }        = &#xA0;  N  0
      e  &#x2212; &#x03BB; t   ,       {\displaystyle {\begin{aligned}N(t)&=
      {\mathcal {L}}^{-1}\{{\widetilde {N}}(s)\}={\mathcal {L}}^{-1}\!\left\{
      {\frac {N_{0}}{s+\lambda }}\right\}\\&=\ N_{0}e^{-\lambda t},\end
      {aligned}}}  [{\displaystyle {\begin{aligned}N(t)&={\mathcal {L}}^{-1}\{
      {\widetilde {N}}(s)\}={\mathcal {L}}^{-1}\!\left\{{\frac {N_{0}}
      {s+\lambda }}\right\}\\&=\ N_{0}e^{-\lambda t},\end{aligned}}}]
which is indeed the correct form for radioactive decay.
**** Complex impedance of a capacitor[edit] ****
In the theory of electrical_circuits, the current flow in a capacitor is
proportional to the capacitance and rate of change in the electrical potential
(in SI units). Symbolically, this is expressed by the differential equation
         i = C    d v   d t    ,   {\displaystyle i=C{dv \over dt},}  [
      {\displaystyle i=C{dv \over dt},}]
where C is the capacitance (in farads) of the capacitor, i = i(t) is the
electric_current (in amperes) through the capacitor as a function of time, and
v = v(t) is the voltage (in volts) across the terminals of the capacitor, also
as a function of time.
Taking the Laplace transform of this equation, we obtain
         I ( s ) = C ( s V ( s ) &#x2212;  V  0   ) ,   {\displaystyle I(s)=C
      (sV(s)-V_{0}),}  [{\displaystyle I(s)=C(sV(s)-V_{0}),}]
where
             I ( s )    =   L   { i ( t ) } ,     V ( s )    =   L   { v ( t )
      } ,       {\displaystyle {\begin{aligned}I(s)&={\mathcal {L}}\{i(t)\},\\V
      (s)&={\mathcal {L}}\{v(t)\},\end{aligned}}}  [{\begin{aligned}I(s)&=
      {\mathcal {L}}\{i(t)\},\\V(s)&={\mathcal {L}}\{v(t)\},\end{aligned}}]
and
          V  0   = v ( t )    |    t = 0   .    {\displaystyle V_{0}=v(t){\Big
      |}_{t=0}.\,}  [{\displaystyle V_{0}=v(t){\Big |}_{t=0}.\,}]
Solving for V(s) we have
         V ( s ) =    I ( s )   s C    +    V  0   s   .   {\displaystyle V(s)=
      {I(s) \over sC}+{V_{0} \over s}.}  [{\displaystyle V(s)={I(s) \over sC}+
      {V_{0} \over s}.}]
The definition of the complex impedance Z (in ohms) is the ratio of the complex
voltage V divided by the complex current I while holding the initial state V0
at zero:
         Z ( s ) =       V ( s )   I ( s )    |    V  0   = 0   .
      {\displaystyle Z(s)=\left.{V(s) \over I(s)}\right|_{V_{0}=0}.}  [
      {\displaystyle Z(s)=\left.{V(s) \over I(s)}\right|_{V_{0}=0}.}]
Using this definition and the previous equation, we find:
         Z ( s ) =   1  s C    ,   {\displaystyle Z(s)={\frac {1}{sC}},}  [Z
      (s)={\frac {1}{sC}},]
which is the correct expression for the complex impedance of a capacitor. In
addition, the Laplace transform has large applications in control theory.
**** Partial fraction expansion[edit] ****
Consider a linear time-invariant system with transfer_function
         H ( s ) =   1  ( s + &#x03B1; ) ( s + &#x03B2; )    .   {\displaystyle
      H(s)={\frac {1}{(s+\alpha )(s+\beta )}}.}  [H(s)={\frac {1}{(s+\alpha )
      (s+\beta )}}.]
The impulse_response is simply the inverse Laplace transform of this transfer
function:
         h ( t ) =    L    &#x2212; 1   { H ( s ) } .   {\displaystyle h(t)=
      {\mathcal {L}}^{-1}\{H(s)\}.}  [h(t)={\mathcal {L}}^{-1}\{H(s)\}.]
To evaluate this inverse transform, we begin by expanding H(s) using the method
of partial_fraction expansion,
           1  ( s + &#x03B1; ) ( s + &#x03B2; )    =   P  s + &#x03B1;    +   R
      s + &#x03B2;    .   {\displaystyle {\frac {1}{(s+\alpha )(s+\beta )}}={P
      \over s+\alpha }+{R \over s+\beta }.}  [{\frac {1}{(s+\alpha )(s+\beta
      )}}={P \over s+\alpha }+{R \over s+\beta }.]
The unknown constants P and R are the residues located at the corresponding
poles of the transfer function. Each residue represents the relative
contribution of that singularity to the transfer function's overall shape.
By the residue_theorem, the inverse Laplace transform depends only upon the
poles and their residues. To find the residue P, we multiply both sides of the
equation by s + Î± to get
           1  s + &#x03B2;    = P +    R ( s + &#x03B1; )   s + &#x03B2;    .
      {\displaystyle {\frac {1}{s+\beta }}=P+{R(s+\alpha ) \over s+\beta }.}  [
      {\frac {1}{s+\beta }}=P+{R(s+\alpha ) \over s+\beta }.]
Then by letting s = âÎ±, the contribution from R vanishes and all that is
left is
         P =      1  s + &#x03B2;    |   s = &#x2212; &#x03B1;   =   1
      &#x03B2; &#x2212; &#x03B1;    .   {\displaystyle P=\left.{1 \over s+\beta
      }\right|_{s=-\alpha }={1 \over \beta -\alpha }.}  [P=\left.{1 \over
      s+\beta }\right|_{s=-\alpha }={1 \over \beta -\alpha }.]
Similarly, the residue R is given by
         R =      1  s + &#x03B1;    |   s = &#x2212; &#x03B2;   =   1
      &#x03B1; &#x2212; &#x03B2;    .   {\displaystyle R=\left.{1 \over
      s+\alpha }\right|_{s=-\beta }={1 \over \alpha -\beta }.}  [R=\left.{1
      \over s+\alpha }\right|_{s=-\beta }={1 \over \alpha -\beta }.]
Note that
         R =    &#x2212; 1   &#x03B2; &#x2212; &#x03B1;    = &#x2212; P
      {\displaystyle R={-1 \over \beta -\alpha }=-P}  [R={-1 \over \beta -
      \alpha }=-P]
and so the substitution of R and P into the expanded expression for H(s) gives
         H ( s ) =  (   1  &#x03B2; &#x2212; &#x03B1;    )  &#x22C5;  (    1  s
      + &#x03B1;    &#x2212;   1  s + &#x03B2;     )  .   {\displaystyle H
      (s)=\left({\frac {1}{\beta -\alpha }}\right)\cdot \left({1 \over s+\alpha
      }-{1 \over s+\beta }\right).}  [H(s)=\left({\frac {1}{\beta -\alpha
      }}\right)\cdot \left({1 \over s+\alpha }-{1 \over s+\beta }\right).]
Finally, using the linearity property and the known transform for exponential
decay (see Item #3 in the Table of Laplace Transforms, above), we can take the
inverse Laplace transform of H(s) to obtain
         h ( t ) =    L    &#x2212; 1   { H ( s ) } =   1  &#x03B2; &#x2212;
      &#x03B1;     (   e  &#x2212; &#x03B1; t   &#x2212;  e  &#x2212; &#x03B2;
      t    )  ,   {\displaystyle h(t)={\mathcal {L}}^{-1}\{H(s)\}={\frac {1}
      {\beta -\alpha }}\left(e^{-\alpha t}-e^{-\beta t}\right),}  [h(t)=
      {\mathcal {L}}^{-1}\{H(s)\}={\frac {1}{\beta -\alpha }}\left(e^{-\alpha
      t}-e^{-\beta t}\right),]
which is the impulse response of the system.
  Convolution
The same result can be achieved using the convolution_property as if the system
is a series of filters with transfer functions of 1/(s + a) and 1/(s + b). That
is, the inverse of
         H ( s ) =   1  ( s + a ) ( s + b )    =   1  s + a    &#x22C5;   1  s
      + b      {\displaystyle H(s)={\frac {1}{(s+a)(s+b)}}={\frac {1}
      {s+a}}\cdot {\frac {1}{s+b}}}  [H(s)={\frac {1}{(s+a)(s+b)}}={\frac {1}
      {s+a}}\cdot {\frac {1}{s+b}}]
is
            L    &#x2212; 1     {   1  s + a    }  &#x2217;    L    &#x2212; 1
      {   1  s + b    }  =  e  &#x2212; a t   &#x2217;  e  &#x2212; b t   =
      &#x222B;  0   t    e  &#x2212; a x    e  &#x2212; b ( t &#x2212; x )    d
      x =     e  &#x2212; a t   &#x2212;  e  &#x2212; b t     b &#x2212; a    .
      {\displaystyle {\mathcal {L}}^{-1}\!\left\{{\frac {1}{s+a}}\right\}*
      {\mathcal {L}}^{-1}\!\left\{{\frac {1}{s+b}}\right\}=e^{-at}*e^{-bt}=\int
      _{0}^{t}e^{-ax}e^{-b(t-x)}\,dx={\frac {e^{-at}-e^{-bt}}{b-a}}.}  [
      {\mathcal {L}}^{-1}\!\left\{{\frac {1}{s+a}}\right\}*{\mathcal {L}}^{-
      1}\!\left\{{\frac {1}{s+b}}\right\}=e^{-at}*e^{-bt}=\int _{0}^{t}e^{-
      ax}e^{-b(t-x)}\,dx={\frac {e^{-at}-e^{-bt}}{b-a}}.]
**** Phase delay[edit] ****
Time function                          Laplace transform
                                             s sin &#x2061; ( &#x03C6; ) +
                                       &#x03C9; cos &#x2061; ( &#x03C6; )    s
   sin &#x2061;  ( &#x03C9; t +        2   +  &#x03C9;  2        {\displaystyle
&#x03C6; )    {\displaystyle \sin {    {\frac {s\sin(\varphi )+\omega \cos
(\omega t+\varphi )}}  [{\displaystyle (\varphi )}{s^{2}+\omega ^{2}}}}  [
\sin {(\omega t+\varphi )}}]           {\displaystyle {\frac {s\sin(\varphi
                                       )+\omega \cos(\varphi )}{s^{2}+\omega ^
                                       {2}}}}]
                                             s cos &#x2061; ( &#x03C6; )
                                       &#x2212; &#x03C9; sin &#x2061;
   cos &#x2061;  ( &#x03C9; t +        ( &#x03C6; )    s  2   +  &#x03C9;  2
&#x03C6; )    {\displaystyle \cos {    .   {\displaystyle {\frac {s\cos(\varphi
(\omega t+\varphi )}}  [{\displaystyle )-\omega \sin(\varphi )}{s^{2}+\omega ^
\cos {(\omega t+\varphi )}}]           {2}}}.}  [{\displaystyle {\frac {s\cos
                                       (\varphi )-\omega \sin(\varphi )}{s^
                                       {2}+\omega ^{2}}}.}]
Starting with the Laplace transform,
         X ( s ) =    s sin &#x2061; ( &#x03C6; ) + &#x03C9; cos &#x2061;
      ( &#x03C6; )    s  2   +  &#x03C9;  2        {\displaystyle X(s)={\frac
      {s\sin(\varphi )+\omega \cos(\varphi )}{s^{2}+\omega ^{2}}}}  [
      {\displaystyle X(s)={\frac {s\sin(\varphi )+\omega \cos(\varphi )}{s^
      {2}+\omega ^{2}}}}]
we find the inverse by first rearranging terms in the fraction:
             X ( s )    =    s sin &#x2061; ( &#x03C6; )    s  2   +  &#x03C9;
      2      +    &#x03C9; cos &#x2061; ( &#x03C6; )    s  2   +  &#x03C9;  2
      = sin &#x2061; ( &#x03C6; )  (   s   s  2   +  &#x03C9;  2      )  + cos
      &#x2061; ( &#x03C6; )  (   &#x03C9;   s  2   +  &#x03C9;  2      )  .
      {\displaystyle {\begin{aligned}X(s)&={\frac {s\sin(\varphi )}{s^
      {2}+\omega ^{2}}}+{\frac {\omega \cos(\varphi )}{s^{2}+\omega ^
      {2}}}\\&=\sin(\varphi )\left({\frac {s}{s^{2}+\omega ^{2}}}\right)+\cos
      (\varphi )\left({\frac {\omega }{s^{2}+\omega ^{2}}}\right).\end
      {aligned}}}  [{\displaystyle {\begin{aligned}X(s)&={\frac {s\sin(\varphi
      )}{s^{2}+\omega ^{2}}}+{\frac {\omega \cos(\varphi )}{s^{2}+\omega ^
      {2}}}\\&=\sin(\varphi )\left({\frac {s}{s^{2}+\omega ^{2}}}\right)+\cos
      (\varphi )\left({\frac {\omega }{s^{2}+\omega ^{2}}}\right).\end
      {aligned}}}]
We are now able to take the inverse Laplace transform of our terms:
             x ( t )    = sin &#x2061; ( &#x03C6; )    L    &#x2212; 1    {   s
      s  2   +  &#x03C9;  2      }  + cos &#x2061; ( &#x03C6; )    L
      &#x2212; 1    {   &#x03C9;   s  2   +  &#x03C9;  2      }        = sin
      &#x2061; ( &#x03C6; ) cos &#x2061; ( &#x03C9; t ) + sin &#x2061;
      ( &#x03C9; t ) cos &#x2061; ( &#x03C6; ) .       {\displaystyle {\begin
      {aligned}x(t)&=\sin(\varphi ){\mathcal {L}}^{-1}\left\{{\frac {s}{s^
      {2}+\omega ^{2}}}\right\}+\cos(\varphi ){\mathcal {L}}^{-1}\left\{{\frac
      {\omega }{s^{2}+\omega ^{2}}}\right\}\\&=\sin(\varphi )\cos(\omega
      t)+\sin(\omega t)\cos(\varphi ).\end{aligned}}}  [{\displaystyle {\begin
      {aligned}x(t)&=\sin(\varphi ){\mathcal {L}}^{-1}\left\{{\frac {s}{s^
      {2}+\omega ^{2}}}\right\}+\cos(\varphi ){\mathcal {L}}^{-1}\left\{{\frac
      {\omega }{s^{2}+\omega ^{2}}}\right\}\\&=\sin(\varphi )\cos(\omega
      t)+\sin(\omega t)\cos(\varphi ).\end{aligned}}}]
This is just the sine_of_the_sum of the arguments, yielding:
         x ( t ) = sin &#x2061; ( &#x03C9; t + &#x03C6; ) .   {\displaystyle x
      (t)=\sin(\omega t+\varphi ).}  [{\displaystyle x(t)=\sin(\omega t+\varphi
      ).}]
We can apply similar logic to find that
            L    &#x2212; 1    {    s cos &#x2061; &#x03C6; &#x2212; &#x03C9;
      sin &#x2061; &#x03C6;    s  2   +  &#x03C9;  2      }  = cos &#x2061;
      ( &#x03C9; t + &#x03C6; )  .   {\displaystyle {\mathcal {L}}^{-1}\left\{
      {\frac {s\cos \varphi -\omega \sin \varphi }{s^{2}+\omega ^
      {2}}}\right\}=\cos {(\omega t+\varphi )}.}  [{\displaystyle {\mathcal
      {L}}^{-1}\left\{{\frac {s\cos \varphi -\omega \sin \varphi }{s^{2}+\omega
      ^{2}}}\right\}=\cos {(\omega t+\varphi )}.}]
**** Determining structure of astronomical object from spectrum[edit] ****
The wide and general applicability of the Laplace transform and its inverse is
illustrated by an application in astronomy which provides some information on
the spatial distribution of matter of an astronomical source of radio-frequency
thermal_radiation too distant to resolve as more than a point, given its flux
density spectrum, rather than relating the time domain with the spectrum
(frequency domain).
Assuming certain properties of the object, e.g. spherical shape and constant
temperature, calculations based on carrying out an inverse Laplace
transformation on the spectrum of the object can produce the only possible
model of the distribution of matter in it (density as a function of distance
from the center) consistent with the spectrum.[29] When independent information
on the structure of an object is available, the inverse Laplace transform
method has been found to be in good agreement.
**** Statistical mechanics[edit] ****
In statistical_mechanics, the Laplace transform of the density of states     g
( E ) d E   {\displaystyle g(E)dE}  [{\displaystyle g(E)dE}] defines the
partition_function.[30] That is, the partition function     Z ( &#x03B2; )
{\displaystyle Z(\beta )}  [{\displaystyle Z(\beta )}] is given by
         Z ( &#x03B2; ) =  &#x222B;  0   &#x221E;    e  &#x2212; &#x03B2; E   g
      ( E ) d E   {\displaystyle Z(\beta )=\int _{0}^{\infty }e^{-\beta E}g
      (E)dE}  [{\displaystyle Z(\beta )=\int _{0}^{\infty }e^{-\beta E}g(E)dE}]
and the inverse is given by
         g ( E ) =   1  2 &#x03C0; i     &#x222B;   &#x03B2;  0   &#x2212; i
      &#x221E;    &#x03B2;  0   + i &#x221E;    e  &#x03B2; E   Z ( &#x03B2; )
      d &#x03B2;   {\displaystyle g(E)={\frac {1}{2\pi i}}\int _{\beta _{0}-
      i\infty }^{\beta _{0}+i\infty }e^{\beta E}Z(\beta )d\beta }  [
      {\displaystyle g(E)={\frac {1}{2\pi i}}\int _{\beta _{0}-i\infty }^{\beta
      _{0}+i\infty }e^{\beta E}Z(\beta )d\beta }]
***** See also[edit] *****
    * Analog_signal_processing
    * Bernstein's_theorem_on_monotone_functions
    * Continuous-repayment_mortgage
    * Fourier_transform
    * Hamburger_moment_problem
    * HardyâLittlewood_tauberian_theorem
    * LaplaceâCarson_transform
    * Moment-generating_function
    * Pierre-Simon_Laplace
    * Post's_inversion_formula
    * Signal-flow_graph
    * Symbolic_integration
    * Transfer_function
    * Z-transform (discrete equivalent of the Laplace transform)
***** Notes[edit] *****
   1. ^ Korn_&_Korn_1967, Â§8.1
   2. ^Jaynes, E. T. (Edwin T.) (2003). Probability theory : the logic of
      science. Bretthorst, G. Larry. Cambridge, UK: Cambridge University Press.
      ISBN 0511065892. OCLC 57254076.
   3. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   4. ^"Des Fonctions gÃ©nÃ©ratrices" [On generating functions], ThÃ©orie
      analytique_des_ProbabilitÃ©s [Analytical Probability Theory] (in French)
      (2nd ed.), Paris, 1814, chap.I sect.2-20
   5. ^Abel, N. H. (1820), "Sur les fonctions gÃ©nÃ©ratrices et leurs
      dÃ©terminantes", Åuvres ComplÃ¨tes (in French), II (published 1839),
      pp. 77â88
   6.  1881_edition
   7. ^Lerch,_M. (1903), "Sur un point de la thÃ©orie des fonctions
      gÃ©nÃ©ratrices d'Abel" [Proof of the inversion formula], Acta Math. (in
      French), 27: 339â351, doi:10.1007/BF02421315
   8. ^Heaviside,_O. (January 2008), "The_solution_of_definite_integrals_by
      differential_transformation", Electromagnetic Theory, III, London,
      section 526, ISBN 9781605206189
   9. ^Bromwich,_T._J. (1916), "Normal_coordinates_in_dynamical_systems", Proc.
      London Math. Soc., 15: 401â448, doi:10.1112/plms/s2-15.1.401
  10. ^ An influential book was:Gardner, M. F.; Barnes, J. L. (1942),
      Transients in Linear Systems studied by the Laplace Transform, New York:
      Wiley
  11. ^Doetsch, G. (1937), Theorie und Anwendung der Laplacesche Transformation
      [Theory and Application of the Laplace Transform] (in German), Berlin:
      Springer
  12.  translation 1943
  13. ^ Euler_1744, Euler_1753, Euler_1769
  14. ^ Lagrange_1773
  15. ^ Grattan-Guinness_1997, p. 260
  16. ^ Grattan-Guinness_1997, p. 261
  17. ^ Grattan-Guinness_1997, pp. 261–262
  18. ^ Grattan-Guinness_1997, pp. 262–266
  19. ^ Feller_1971, Â§XIII.1
  20. ^ The cumulative distribution function is the integral of the probability
      density function.
  21. ^ Widder_1941, Chapter II, Â§1
  22. ^ Widder_1941, Chapter VI, Â§2
  23. ^ Korn_&_Korn_1967, pp. 226–227
  24. ^ Bracewell_2000, Table 14.1, p. 385
  25. ^Mattuck (Prof at MIT), Arthur. "Where_the_Laplace_Transform_comes_from".
  26. ^ Feller_1971, p. 432
  27. ^ Takacs_1953, p. 93
  28. ^Riley, K. F.; Hobson, M. P.; Bence, S. J. (2010), Mathematical methods
      for physics and engineering (3rd ed.), Cambridge University Press,
      p. 455, ISBN 978-0-521-86153-3
  29. ^Distefano, J. J.; Stubberud, A. R.; Williams, I. J. (1995), Feedback
      systems and control, Schaum's outlines (2nd ed.), McGraw-Hill, p. 78,
      ISBN 978-0-07-017052-0
  30. ^Lipschutz, S.; Spiegel, M. R.; Liu, J. (2009), Mathematical Handbook of
      Formulas and Tables, Schaum's Outline Series (3rd ed.), McGraw-Hill,
      p. 183, ISBN 978-0-07-154855-7
  31.  â provides the case for real q.
  32. ^ http://mathworld.wolfram.com/LaplaceTransform.html â Wolfram Mathword
      provides case for complex q
  33. ^Salem, M.; Seaton, M. J. (1974), "I. Continuum spectra and brightness
      contours", Monthly_Notices_of_the_Royal_Astronomical_Society, 167 (3):
      493â510, Bibcode:1974MNRAS.167..493S, doi:10.1093/mnras/167.3.493
  34. , and
      Salem, M. (1974), "II. Three-dimensional models", Monthly Notices of the
      Royal Astronomical Society, 167 (3): 511â516, Bibcode:
      1974MNRAS.167..511S, doi:10.1093/mnras/167.3.511
  35. ^RK Pathria; Paul Beal (1996). Statistical mechanics (2nd ed.).
      Butterworth-Heinemann. p. 56.
***** References[edit] *****
**** Modern[edit] ****
    * Bracewell, Ronald N. (1978), The Fourier Transform and its Applications
      (2nd ed.), McGraw-Hill Kogakusha, ISBN 978-0-07-007013-4
Bracewell, R. N. (2000), The Fourier Transform and Its Applications (3rd ed.),
Boston: McGraw-Hill, ISBN 978-0-07-116043-8
Feller,_William (1971), An introduction to probability theory and its
applications. Vol. II., Second edition, New York: John_Wiley_&_Sons, MR 0270403
Korn, G. A.; Korn, T. M. (1967), Mathematical Handbook for Scientists and
Engineers (2nd ed.), McGraw-Hill Companies, ISBN 978-0-07-035370-1
Widder, David Vernon (1941), The Laplace Transform, Princeton Mathematical
Series, v. 6, Princeton_University_Press, MR 0005923
Williams, J. (1973), Laplace Transforms, Problem Solvers, George Allen & Unwin,
ISBN 978-0-04-512021-5
Takacs, J. (1953), "Fourier amplitudok meghatarozasa operatorszamitassal",
Magyar Hiradastechnika (in Hungarian), IV (7â8): 93â96
**** Historical[edit] ****
    * Euler,_L. (1744), "De constructione aequationum" [The Construction of
      Equations], Opera Omnia, 1st series (in Latin), 22: 150â161
Euler,_L. (1753), "Methodus aequationes differentiales" [A Method for Solving
Differential Equations], Opera Omnia, 1st series (in Latin), 22: 181â213
Euler,_L. (1992) [1769], "Institutiones calculi integralis, Volume 2"
[Institutions of Integral Calculus], Opera Omnia, 1st series (in Latin), Basel:
BirkhÃ¤user, 12, ISBN 978-3764314743
, Chapters 3â5
Euler,_Leonhard (1769), Institutiones_calculi_integralis [Institutions of
Integral Calculus] (in Latin), II, Paris: Petropoli, ch. 3â5, pp. 57â153
Grattan-Guinness,_I (1997), "Laplace's integral solutions to partial
differential equations", in Gillispie, C. C. (ed.), Pierre Simon Laplace
1749â1827: A Life in Exact Science, Princeton: Princeton University Press,
ISBN 978-0-691-01185-1
Lagrange,_J._L. (1773), MÃ©moire sur l'utilitÃ© de la mÃ©thode, Åuvres de
Lagrange, 2, pp. 171â234
***** Further reading[edit] *****
    * Arendt, Wolfgang; Batty, Charles J.K.; Hieber, Matthias; Neubrander,
      Frank (2002), Vector-Valued Laplace Transforms and Cauchy Problems,
      BirkhÃ¤user Basel, ISBN 978-3-7643-6549-3
.
Davies, Brian (2002), Integral transforms and their applications (Third ed.),
New York: Springer, ISBN 978-0-387-95314-4
Deakin, M. A. B. (1981), "The development of the Laplace transform", Archive
for History of Exact Sciences, 25 (4): 343â390, doi:10.1007/BF01395660
Deakin, M. A. B. (1982), "The development of the Laplace transform", Archive
for History of Exact Sciences, 26 (4): 351â381, doi:10.1007/BF00418754
Doetsch,_Gustav (1974), Introduction to the Theory and Application of the
Laplace Transformation, Springer, ISBN 978-0-387-06407-9
Mathews, Jon; Walker, Robert L. (1970), Mathematical methods of physics (2nd
ed.), New York: W. A. Benjamin,
ISBN 0-8053-7002-1
Polyanin, A. D.; Manzhirov, A. V. (1998), Handbook of Integral Equations, Boca
Raton: CRC Press, ISBN 978-0-8493-2876-3
Schwartz,_Laurent (1952), "Transformation de Laplace des distributions", Comm.
SÃ©m. Math. Univ. Lund [Medd. Lunds Univ. Mat. Sem.] (in French), 1952:
196â206, MR 0052555
Schwartz,_Laurent (2008) [1966], Mathematics_for_the_Physical_Sciences, Dover
Books on Mathematics, New York: Dover Publications, pp. 215â241, ISBN 978-0-
486-46662-0
 - See Chapter VI. The Laplace transform.
Siebert, William McC. (1986), Circuits, Signals, and Systems, Cambridge,
Massachusetts: MIT Press, ISBN 978-0-262-19229-3
Widder, David Vernon (1945), "What is the Laplace transform?", The_American
Mathematical_Monthly, 52 (8): 419â425, doi:10.2307/2305640, ISSN 0002-9890,
JSTOR 2305640, MR 0013447
***** External links[edit] *****
 Wikiquote has quotations related to: Laplace_transform
 Wikimedia Commons has media related to Laplace_transformation.
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Laplace_transform", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Online_Computation of the transform or inverse transform, wims.unice.fr
Tables_of_Integral_Transforms at EqWorld: The World of Mathematical Equations.
Weisstein,_Eric_W. "Laplace_Transform". MathWorld.
Good_explanations_of_the_initial_and_final_value_theorems
Laplace_Transforms at MathPages
Computational_Knowledge_Engine allows to easily calculate Laplace Transforms
and its inverse Transform.
Laplace_Calculator to calculate Laplace Transforms online easily.
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85074666
                                              * NDL: 00567362

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Laplace_transform&oldid=907620734"
Categories:
    * Laplace_transforms
    * Differential_equations
    * Fourier_analysis
    * Mathematical_physics
Hidden categories:
    * CS1_French-language_sources_(fr)
    * CS1_German-language_sources_(de)
    * Wikipedia_articles_needing_clarification_from_May_2010
    * CS1_Hungarian-language_sources_(hu)
    * CS1_Latin-language_sources_(la)
    * Commons_category_link_is_on_Wikidata
    * Wikipedia_articles_with_LCCN_identifiers
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
    * Wikiquote
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * á áá­á
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * à¦¬à¦¾à¦à¦²à¦¾
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
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
    * Galego
    * å®¢å®¶èª/Hak-kÃ¢-ngÃ®
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Interlingua
    * Italiano
    * ×¢××¨××ª
    * Jawa
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LietuviÅ³
    * Magyar
    * à´®à´²à´¯à´¾à´³à´
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * áá¶áá¶ááááá
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Simple_English
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Basa_Sunda
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 24 July 2019, at 04:52 (UTC).
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
