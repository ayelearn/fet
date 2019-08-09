The following text has been accessed from https://en.wikipedia.org/wiki/Improper_integral at Fri Aug 9 02:35:46 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Improper integral ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Limit of a definite integral with as one or both limits approach infinity or
values at which the integrand is undefined
An improper integral of the first kind. The integral may need to be defined on
an unbounded domain.
An improper Riemann integral of the second kind. The integral may fail to exist
because of a vertical_asymptote in the function.
Part of a series of articles about
Calculus
    * Fundamental_theorem
    * Limits_of_functions
    * Continuity
    * Mean_value_theorem
    * Rolle's_theorem
Differential
Definitions
    * Derivative (generalizations)
    * Differential
          o infinitesimal
          o of_a_function
          o total
Concepts
    * Differentiation_notation
    * Second_derivative
    * Third_derivative
    * Change_of_variables
    * Implicit_differentiation
    * Related_rates
    * Taylor's_theorem
Rules_and_identities
    * Sum
    * Product
    * Chain
    * Power
    * Quotient
    * Inverse
    * General_Leibniz
    * FaÃ _di_Bruno's_formula
Integral
    * Lists_of_integrals
Definitions
    * Antiderivative
    * Integral (improper)
    * Riemann_integral
    * Lebesgue_integration
    * Contour_integration
Integration by
    * Parts
    * Discs
    * Cylindrical_shells
    * Substitution (trigonometric)
    * Partial_fractions
    * Order
    * Reduction_formulae
Series
    * Geometric (arithmetico-geometric)
    * Harmonic
    * Alternating
    * Power
    * Binomial
    * Taylor
Convergence_tests
    * Summand_limit_(term_test)
    * Ratio
    * Root
    * Integral
    * Direct_comparison
    *
      Limit_comparison
    * Alternating_series
    * Cauchy_condensation
    * Dirichlet
    * Abel
Vector
    * Gradient
    * Divergence
    * Curl
    * Laplacian
    * Directional_derivative
    * Identities
Theorems
    * Divergence
    * Gradient
    * Green's
    * KelvinâStokes
    * Stokes
Multivariable
Formalisms
    * Matrix
    * Tensor
    * Exterior
    * Geometric
Definitions
    * Partial_derivative
    * Multiple_integral
    * Line_integral
    * Surface_integral
    * Volume_integral
    * Jacobian
    * Hessian
Specialized
    * Fractional
    * Malliavin
    * Stochastic
    * Variations
Glossary_of_calculus
    * Glossary_of_calculus
    * v
    * t
    * e
In mathematical_analysis, an improper integral is the limit of a definite
integral as an endpoint of the interval(s) of integration approaches either a
specified real_number,     &#x221E;   {\displaystyle \infty }  [\infty ],
&#x2212; &#x221E;   {\displaystyle -\infty }  [-\infty ], or in some instances
as both endpoints approach limits. Such an integral is often written
symbolically just like a standard definite integral, in some cases with
infinity as a limit of integration.
Specifically, an improper integral is a limit of the form:
          lim  b &#x2192; &#x221E;    &#x222B;  a   b   f ( x )  d x ,   lim  a
      &#x2192; &#x2212; &#x221E;    &#x222B;  a   b   f ( x )  d x ,
      {\displaystyle \lim _{b\to \infty }\int _{a}^{b}f(x)\,dx,\qquad \lim _
      {a\to -\infty }\int _{a}^{b}f(x)\,dx,}  [{\displaystyle \lim _{b\to
      \infty }\int _{a}^{b}f(x)\,dx,\qquad \lim _{a\to -\infty }\int _{a}^{b}f
      (x)\,dx,}]
or
          lim  c &#x2192;  b  &#x2212;      &#x222B;  a   c   f ( x )  d x ,
      lim  c &#x2192;  a  +      &#x222B;  c   b   f ( x )  d x ,
      {\displaystyle \lim _{c\to b^{-}}\int _{a}^{c}f(x)\,dx,\quad \lim _{c\to
      a^{+}}\int _{c}^{b}f(x)\,dx,}  [{\displaystyle \lim _{c\to b^{-}}\int _
      {a}^{c}f(x)\,dx,\quad \lim _{c\to a^{+}}\int _{c}^{b}f(x)\,dx,}]
in which one takes a limit in one or the other (or sometimes both) endpoints
(Apostol_1967, Â§10.23).
By abuse_of_notation, improper integrals are often written symbolically just
like standard definite integrals, perhaps with infinity among the limits of
integration. When the definite integral exists (in the sense of either the
Riemann_integral or the more advanced Lebesgue_integral), this ambiguity is
resolved as both the proper and improper integral will coincide in value.
Often one is able to compute values for improper integrals, even when the
function is not integrable in the conventional sense (as a Riemann_integral,
for instance) because of a singularity in the function or because one of the
bounds of integration is infinite.
⁰
***** Contents *****
    * 1_Examples
    * 2_Convergence_of_the_integral
    * 3_Types_of_integrals
    * 4_Improper_Riemann_integrals_and_Lebesgue_integrals
    * 5_Singularities
    * 6_Cauchy_principal_value
    * 7_Summability
    * 8_Multivariable_improper_integrals
          o 8.1_Improper_integrals_over_arbitrary_domains
          o 8.2_Improper_integrals_with_singularities
          o 8.3_Functions_with_both_positive_and_negative_values
    * 9_Notes
    * 10_Bibliography
    * 11_External_links
***** Examples[edit] *****
The original definition of the Riemann_integral does not apply to a function
such as     1  /    x  2      {\displaystyle 1/{x^{2}}}  [1/{x^{2}}] on the
interval [1, â), because in this case the domain of integration is unbounded.
However, the Riemann integral can often be extended by continuity, by defining
the improper integral instead as a limit
          &#x222B;  1   &#x221E;     1  x  2      d x =  lim  b &#x2192;
      &#x221E;    &#x222B;  1   b     1  x  2      d x =  lim  b &#x2192;
      &#x221E;    (  &#x2212;   1 b   +   1 1    )  = 1.   {\displaystyle \int
      _{1}^{\infty }{\frac {1}{x^{2}}}\,dx=\lim _{b\to \infty }\int _{1}^{b}
      {\frac {1}{x^{2}}}\,dx=\lim _{b\to \infty }\left(-{\frac {1}{b}}+{\frac
      {1}{1}}\right)=1.}  [{\displaystyle \int _{1}^{\infty }{\frac {1}{x^
      {2}}}\,dx=\lim _{b\to \infty }\int _{1}^{b}{\frac {1}{x^{2}}}\,dx=\lim _
      {b\to \infty }\left(-{\frac {1}{b}}+{\frac {1}{1}}\right)=1.}]
The narrow definition of the Riemann integral also does not cover the function
1  /    x     {\displaystyle 1/{\sqrt {x}}}  [1/{\sqrt {x}}] on the interval
[0, 1]. The problem here is that the integrand is unbounded in the domain of
integration (the definition requires that both the domain of integration and
the integrand be bounded). However, the improper integral does exist if
understood as the limit
          &#x222B;  0   1     1  x     d x =  lim  a &#x2192;  0  +
      &#x222B;  a   1     1  x     d x =  lim  a &#x2192;  0  +     ( 2
      &#x2212; 2   a   ) = 2.   {\displaystyle \int _{0}^{1}{\frac {1}{\sqrt
      {x}}}\,dx=\lim _{a\to 0^{+}}\int _{a}^{1}{\frac {1}{\sqrt {x}}}\,dx=\lim
      _{a\to 0^{+}}(2-2{\sqrt {a}})=2.}  [{\displaystyle \int _{0}^{1}{\frac
      {1}{\sqrt {x}}}\,dx=\lim _{a\to 0^{+}}\int _{a}^{1}{\frac {1}{\sqrt
      {x}}}\,dx=\lim _{a\to 0^{+}}(2-2{\sqrt {a}})=2.}]
The improper integral
    &#x222B;  0   &#x221E;      d x   ( x + 1 )   x      = &#x03C0;
{\displaystyle \int _{0}^{\infty }{\frac {dx}{(x+1){\sqrt {x}}}}=\pi }  [\int _
{0}^{\infty }{\frac {dx}{(x+1){\sqrt {x}}}}=\pi ]
has unbounded intervals for both domain and range.
Sometimes integrals may have two singularities where they are improper.
Consider, for example, the function 1/((x + 1)√x) integrated from 0 to â
(shown right). At the lower bound, as x goes to 0 the function goes to â, and
the upper bound is itself â, though the function goes to 0. Thus this is a
doubly improper integral. Integrated, say, from 1 to 3, an ordinary Riemann sum
suffices to produce a result of Ï/6. To integrate from 1 to â, a Riemann sum
is not possible. However, any finite upper bound, say t (with t > 1), gives a
well-defined result, 2 arctan(√t) â Ï/2. This has a finite limit as t goes
to infinity, namely Ï/2. Similarly, the integral from 1/3 to 1 allows a
Riemann sum as well, coincidentally again producing Ï/6. Replacing 1/3 by an
arbitrary positive value s (with s < 1) is equally safe, giving Ï/2 â 2
arctan(√s). This, too, has a finite limit as s goes to zero, namely Ï/2.
Combining the limits of the two fragments, the result of this improper integral
is
              &#x222B;  0   &#x221E;      d x   ( x + 1 )   x           =  lim
      s &#x2192;  0  +      &#x222B;  s   1      d x   ( x + 1 )   x      +
      lim  t &#x2192; &#x221E;    &#x222B;  1   t      d x   ( x + 1 )   x
      =  lim  s &#x2192;  0  +      (    &#x03C0; 2   &#x2212; 2 arctan
      &#x2061;   s    )  +  lim  t &#x2192; &#x221E;    (  2 arctan &#x2061;
      t   &#x2212;   &#x03C0; 2    )          =   &#x03C0; 2   +  (  &#x03C0;
      &#x2212;   &#x03C0; 2    )          = &#x03C0; .       {\displaystyle
      {\begin{aligned}\int _{0}^{\infty }{\frac {dx}{(x+1){\sqrt {x}}}}&{}=\lim
      _{s\to 0^{+}}\int _{s}^{1}{\frac {dx}{(x+1){\sqrt {x}}}}+\lim _{t\to
      \infty }\int _{1}^{t}{\frac {dx}{(x+1){\sqrt {x}}}}\\&{}=\lim _{s\to 0^
      {+}}\left({\frac {\pi }{2}}-2\arctan {\sqrt {s}}\right)+\lim _{t\to
      \infty }\left(2\arctan {\sqrt {t}}-{\frac {\pi }{2}}\right)\\&{}={\frac
      {\pi }{2}}+\left(\pi -{\frac {\pi }{2}}\right)\\&{}=\pi .\end{aligned}}}
      [{\displaystyle {\begin{aligned}\int _{0}^{\infty }{\frac {dx}{(x+1)
      {\sqrt {x}}}}&{}=\lim _{s\to 0^{+}}\int _{s}^{1}{\frac {dx}{(x+1){\sqrt
      {x}}}}+\lim _{t\to \infty }\int _{1}^{t}{\frac {dx}{(x+1){\sqrt {x}}}}\\&
      {}=\lim _{s\to 0^{+}}\left({\frac {\pi }{2}}-2\arctan {\sqrt
      {s}}\right)+\lim _{t\to \infty }\left(2\arctan {\sqrt {t}}-{\frac {\pi }
      {2}}\right)\\&{}={\frac {\pi }{2}}+\left(\pi -{\frac {\pi }{2}}\right)\\&
      {}=\pi .\end{aligned}}}]
This process does not guarantee success; a limit might fail to exist, or might
be infinite. For example, over the bounded interval from 0 to 1 the integral of
1/x does not converge; and over the unbounded interval from 1 to â the
integral of 1/√x does not converge.
The improper integral
    &#x222B;  &#x2212; 1   1      d x    x  2    3     = 6   {\displaystyle
\int _{-1}^{1}{\frac {dx}{\sqrt[{3}]{x^{2}}}}=6}  [\int _{-1}^{1}{\frac {dx}
{\sqrt[{3}]{x^{2}}}}=6]
converges, since both left and right limits exist, though the integrand is
unbounded near an interior point.
It might also happen that an integrand is unbounded near an interior point, in
which case the integral must be split at that point. For the integral as a
whole to converge, the limit integrals on both sides must exist and must be
bounded. For example:
              &#x222B;  &#x2212; 1   1      d x    x  2    3          =  lim  s
      &#x2192; 0    &#x222B;  &#x2212; 1   &#x2212; s      d x    x  2    3
      +  lim  t &#x2192; 0    &#x222B;  t   1      d x    x  2    3
      =  lim  s &#x2192; 0   3 ( 1 &#x2212;   s  3    ) +  lim  t &#x2192; 0
      3 ( 1 &#x2212;   t  3    )         = 3 + 3         = 6.
      {\displaystyle {\begin{aligned}\int _{-1}^{1}{\frac {dx}{\sqrt[{3}]{x^
      {2}}}}&{}=\lim _{s\to 0}\int _{-1}^{-s}{\frac {dx}{\sqrt[{3}]{x^
      {2}}}}+\lim _{t\to 0}\int _{t}^{1}{\frac {dx}{\sqrt[{3}]{x^{2}}}}\\&
      {}=\lim _{s\to 0}3(1-{\sqrt[{3}]{s}})+\lim _{t\to 0}3(1-{\sqrt[{3}]
      {t}})\\&{}=3+3\\&{}=6.\end{aligned}}}  [{\begin{aligned}\int _{-1}^{1}
      {\frac {dx}{\sqrt[{3}]{x^{2}}}}&{}=\lim _{s\to 0}\int _{-1}^{-s}{\frac
      {dx}{\sqrt[{3}]{x^{2}}}}+\lim _{t\to 0}\int _{t}^{1}{\frac {dx}{\sqrt[
      {3}]{x^{2}}}}\\&{}=\lim _{s\to 0}3(1-{\sqrt[{3}]{s}})+\lim _{t\to 0}3(1-
      {\sqrt[{3}]{t}})\\&{}=3+3\\&{}=6.\end{aligned}}]
But the similar integral
          &#x222B;  &#x2212; 1   1      d x  x     {\displaystyle \int _{-1}^
      {1}{\frac {dx}{x}}}  [{\displaystyle \int _{-1}^{1}{\frac {dx}{x}}}]
cannot be assigned a value in this way, as the integrals above and below zero
do not independently converge. (However, see Cauchy_principal_value.)
***** Convergence of the integral[edit] *****
An improper integral converges if the limit defining it exists. Thus for
example one says that the improper integral
          lim  t &#x2192; &#x221E;    &#x222B;  a   t   f ( x )  d x
      {\displaystyle \lim _{t\to \infty }\int _{a}^{t}f(x)\,dx}  [
      {\displaystyle \lim _{t\to \infty }\int _{a}^{t}f(x)\,dx}]
exists and is equal to L if the integrals under the limit exist for all
sufficiently large t, and the value of the limit is equal to L.
It is also possible for an improper integral to diverge to infinity. In that
case, one may assign the value of â (or -â) to the integral. For instance
          lim  b &#x2192; &#x221E;    &#x222B;  1   b     1 x    d x = &#x221E;
      .   {\displaystyle \lim _{b\to \infty }\int _{1}^{b}{\frac {1}
      {x}}\,dx=\infty .}  [{\displaystyle \lim _{b\to \infty }\int _{1}^{b}
      {\frac {1}{x}}\,dx=\infty .}]
However, other improper integrals may simply diverge in no particular
direction, such as
          lim  b &#x2192; &#x221E;    &#x222B;  1   b   x sin &#x2061; ( x )  d
      x ,   {\displaystyle \lim _{b\to \infty }\int _{1}^{b}x\sin(x)\,dx,}  [
      {\displaystyle \lim _{b\to \infty }\int _{1}^{b}x\sin(x)\,dx,}]
which does not exist, even as an extended_real_number. This is called
divergence by oscillation.
A limitation of the technique of improper integration is that the limit must be
taken with respect to one endpoint at a time. Thus, for instance, an improper
integral of the form
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x )  d x
      {\displaystyle \int _{-\infty }^{\infty }f(x)\,dx}  [{\displaystyle \int
      _{-\infty }^{\infty }f(x)\,dx}]
can be defined by taking two separate limits; to wit
          &#x222B;  &#x2212; &#x221E;   &#x221E;   f ( x )  d x =  lim  a
      &#x2192; &#x2212; &#x221E;    lim  b &#x2192; &#x221E;    &#x222B;  a   b
      f ( x )  d x   {\displaystyle \int _{-\infty }^{\infty }f(x)\,dx=\lim _
      {a\to -\infty }\lim _{b\to \infty }\int _{a}^{b}f(x)\,dx}  [
      {\displaystyle \int _{-\infty }^{\infty }f(x)\,dx=\lim _{a\to -\infty
      }\lim _{b\to \infty }\int _{a}^{b}f(x)\,dx}]
provided the double limit is finite. It can also be defined as a pair of
distinct improper integrals of the first kind:
          lim  a &#x2192; &#x2212; &#x221E;    &#x222B;  a   c   f ( x )  d x +
      lim  b &#x2192; &#x221E;    &#x222B;  c   b   f ( x )  d x
      {\displaystyle \lim _{a\to -\infty }\int _{a}^{c}f(x)\,dx+\lim _{b\to
      \infty }\int _{c}^{b}f(x)\,dx}  [{\displaystyle \lim _{a\to -\infty }\int
      _{a}^{c}f(x)\,dx+\lim _{b\to \infty }\int _{c}^{b}f(x)\,dx}]
where c is any convenient point at which to start the integration. This
definition also applies when one of these integrals is infinite, or both if
they have the same sign.
An example of an improper integrals where both endpoints are infinite is the
Gaussian_integral      &#x222B;  &#x2212; &#x221E;   &#x221E;    e  &#x2212;  x
2      d x =   &#x03C0;     {\displaystyle \int _{-\infty }^{\infty }e^{-x^
{2}}\,dx={\sqrt {\pi }}}  [{\displaystyle \int _{-\infty }^{\infty }e^{-x^
{2}}\,dx={\sqrt {\pi }}}]. An example which evaluates to infinity is
&#x222B;  &#x2212; &#x221E;   &#x221E;    e  x    d x   {\displaystyle \int _{-
\infty }^{\infty }e^{x}\,dx}  [{\displaystyle \int _{-\infty }^{\infty }e^
{x}\,dx}]. But one cannot even define other integrals of this kind
unambiguously, such as      &#x222B;  &#x2212; &#x221E;   &#x221E;   x  d x
{\displaystyle \int _{-\infty }^{\infty }x\,dx}  [{\displaystyle \int _{-\infty
}^{\infty }x\,dx}], since the double limit is infinite and the two-integral
method
          lim  a &#x2192; &#x2212; &#x221E;    &#x222B;  a   c   x  d x +  lim
      b &#x2192; &#x221E;    &#x222B;  c   b   x  d x   {\displaystyle \lim _
      {a\to -\infty }\int _{a}^{c}x\,dx+\lim _{b\to \infty }\int _{c}^{b}x\,dx}
      [{\displaystyle \lim _{a\to -\infty }\int _{a}^{c}x\,dx+\lim _{b\to
      \infty }\int _{c}^{b}x\,dx}]
yields     &#x221E; &#x2212; &#x221E;   {\displaystyle \infty -\infty }
[\infty -\infty ]. In this case, one can however define an improper integral in
the sense of Cauchy_principal_value:
          p . v .  &#x2061;  &#x222B;  &#x2212; &#x221E;   &#x221E;   x  d x =
      lim  b &#x2192; &#x221E;    &#x222B;  &#x2212; b   b   x  d x = 0.
      {\displaystyle \operatorname {p.v.} \int _{-\infty }^{\infty }x\,dx=\lim
      _{b\to \infty }\int _{-b}^{b}x\,dx=0.}  [{\displaystyle \operatorname
      {p.v.} \int _{-\infty }^{\infty }x\,dx=\lim _{b\to \infty }\int _{-b}^
      {b}x\,dx=0.}]
The questions one must address in determining an improper integral are:
    * Does the limit exist?
    * Can the limit be computed?
The first question is an issue of mathematical_analysis. The second one can be
addressed by calculus techniques, but also in some cases by contour
integration, Fourier_transforms and other more advanced methods.
***** Types of integrals[edit] *****
There is more than one theory of integration. From the point of view of
calculus, the Riemann_integral theory is usually assumed as the default theory.
In using improper integrals, it can matter which integration theory is in play.
    * For the Riemann integral (or the Darboux_integral, which is equivalent to
      it), improper integration is necessary both for unbounded intervals
      (since one cannot divide the interval into finitely many subintervals of
      finite length) and for unbounded functions with finite integral (since,
      supposing it is unbounded above, then the upper integral will be
      infinite, but the lower integral will be finite).
    * The Lebesgue_integral deals differently with unbounded domains and
      unbounded functions, so that often an integral which only exists as an
      improper Riemann integral will exist as a (proper) Lebesgue integral,
      such as      &#x222B;  1   &#x221E;     1  x  2      d x   {\displaystyle
      \int _{1}^{\infty }{\frac {1}{x^{2}}}\,dx}  [{\displaystyle \int _{1}^
      {\infty }{\frac {1}{x^{2}}}\,dx}]. On the other hand, there are also
      integrals that have an improper Riemann integral but do not have a
      (proper) Lebesgue integral, such as      &#x222B;  0   &#x221E;      sin
      &#x2061; x  x    d x   {\displaystyle \int _{0}^{\infty }{\frac {\sin x}
      {x}}\,dx}  [\int _{0}^{\infty }{\frac  {\sin x}{x}}\,dx]. The Lebesgue
      theory does not see this as a deficiency: from the point of view of
      measure_theory,      &#x222B;  0   &#x221E;      sin &#x2061; x  x    d x
      = &#x221E; &#x2212; &#x221E;   {\displaystyle \int _{0}^{\infty }{\frac
      {\sin x}{x}}\,dx=\infty -\infty }  [{\displaystyle \int _{0}^{\infty }
      {\frac {\sin x}{x}}\,dx=\infty -\infty }] and cannot be defined
      satisfactorily. In some situations, however, it may be convenient to
      employ improper Lebesgue integrals as is the case, for instance, when
      defining the Cauchy_principal_value. The Lebesgue integral is more or
      less essential in the theoretical treatment of the Fourier_transform,
      with pervasive use of integrals over the whole real line.
    * For the HenstockâKurzweil_integral, improper integration is not
      necessary, and this is seen as a strength of the theory: it encompasses
      all Lebesgue integrable and improper Riemann integrable functions.
***** Improper Riemann integrals and Lebesgue integrals[edit] *****
Figure 1
Figure 2
In some cases, the integral
          &#x222B;  a   c   f ( x )  d x   {\displaystyle \int _{a}^{c}f
      (x)\,dx}  [{\displaystyle \int _{a}^{c}f(x)\,dx}]
can be defined as an integral (a Lebesgue_integral, for instance) without
reference to the limit
          lim  b &#x2192;  c  &#x2212;      &#x222B;  a   b   f ( x )  d x
      {\displaystyle \lim _{b\to c^{-}}\int _{a}^{b}f(x)\,dx}  [{\displaystyle
      \lim _{b\to c^{-}}\int _{a}^{b}f(x)\,dx}]
but cannot otherwise be conveniently computed. This often happens when the
function f being integrated from a to c has a vertical_asymptote at c, or if
c = â (see Figures 1 and 2). In such cases, the improper Riemann integral
allows one to calculate the Lebesgue integral of the function. Specifically,
the following theorem holds (Apostol_1974, Theorem 10.33):
    * If a function f is Riemann integrable on [a,b] for every b â¥ a, and the
      partial integrals
                &#x222B;  a   b    |  f ( x )  |   d x   {\displaystyle \int _
            {a}^{b}|f(x)|\,dx}  [{\displaystyle \int _{a}^{b}|f(x)|\,dx}]
      are bounded as b → â, then the improper Riemann integrals
                &#x222B;  a   &#x221E;   f ( x )  d x ,    and&#xA0;
            &#x222B;  a   &#x221E;    |  f ( x )  |   d x   {\displaystyle \int
            _{a}^{\infty }f(x)\,dx,\quad {\mbox{and }}\int _{a}^{\infty }|f
            (x)|\,dx}  [{\displaystyle \int _{a}^{\infty }f(x)\,dx,\quad {\mbox
            {and }}\int _{a}^{\infty }|f(x)|\,dx}]
      both exist. Furthermore, f is Lebesgue integrable on [a, â), and its
      Lebesgue integral is equal to its improper Riemann integral.
For example, the integral
          &#x222B;  0   &#x221E;      d x   1 +  x  2        {\displaystyle
      \int _{0}^{\infty }{\frac {dx}{1+x^{2}}}}  [\int _{0}^{\infty }{\frac
      {dx}{1+x^{2}}}]
can be interpreted alternatively as the improper integral
          lim  b &#x2192; &#x221E;    &#x222B;  0   b      d x   1 +  x  2
      =  lim  b &#x2192; &#x221E;   arctan &#x2061;  b  =   &#x03C0; 2   ,
      {\displaystyle \lim _{b\to \infty }\int _{0}^{b}{\frac {dx}{1+x^
      {2}}}=\lim _{b\to \infty }\arctan {b}={\frac {\pi }{2}},}  [\lim _{{b\to
      \infty }}\int _{0}^{b}{\frac  {dx}{1+x^{2}}}=\lim _{{b\to \infty
      }}\arctan {b}={\frac  {\pi }{2}},]
or it may be interpreted instead as a Lebesgue_integral over the set (0, â).
Since both of these kinds of integral agree, one is free to choose the first
method to calculate the value of the integral, even if one ultimately wishes to
regard it as a Lebesgue integral. Thus improper integrals are clearly useful
tools for obtaining the actual values of integrals.
In other cases, however, a Lebesgue integral between finite endpoints may not
even be defined, because the integrals of the positive and negative parts of f
are both infinite, but the improper Riemann integral may still exist. Such
cases are "properly improper" integrals, i.e. their values cannot be defined
except as such limits. For example,
          &#x222B;  0   &#x221E;      sin &#x2061; ( x )  x    d x
      {\displaystyle \int _{0}^{\infty }{\frac {\sin(x)}{x}}\,dx}  [
      {\displaystyle \int _{0}^{\infty }{\frac {\sin(x)}{x}}\,dx}]
cannot be interpreted as a Lebesgue integral, since
          &#x222B;  0   &#x221E;    |    sin &#x2061; ( x )  x   |   d x =
      &#x221E; .   {\displaystyle \int _{0}^{\infty }\left|{\frac {\sin(x)}
      {x}}\right|\,dx=\infty .}  [{\displaystyle \int _{0}^{\infty }\left|
      {\frac {\sin(x)}{x}}\right|\,dx=\infty .}]
But     f ( x ) =    sin &#x2061; ( x )  x     {\displaystyle f(x)={\frac {\sin
(x)}{x}}}  [{\displaystyle f(x)={\frac {\sin(x)}{x}}}] is nevertheless
integrable between any two finite endpoints, and its integral between 0 and â
is usually understood as the limit of the integral:
          &#x222B;  0   &#x221E;      sin &#x2061; ( x )  x    d x =  lim  b
      &#x2192; &#x221E;    &#x222B;  0   b      sin &#x2061; ( x )  x    d x =
      &#x03C0; 2   .   {\displaystyle \int _{0}^{\infty }{\frac {\sin(x)}
      {x}}\,dx=\lim _{b\to \infty }\int _{0}^{b}{\frac {\sin(x)}{x}}\,dx={\frac
      {\pi }{2}}.}  [{\displaystyle \int _{0}^{\infty }{\frac {\sin(x)}
      {x}}\,dx=\lim _{b\to \infty }\int _{0}^{b}{\frac {\sin(x)}{x}}\,dx={\frac
      {\pi }{2}}.}]
***** Singularities[edit] *****
One can speak of the singularities of an improper integral, meaning those
points of the extended_real_number_line at which limits are used.
***** Cauchy principal value[edit] *****
Main article: Cauchy_principal_value
Consider the difference in values of two limits:
          lim  a &#x2192;  0  +      (   &#x222B;  &#x2212; 1   &#x2212; a
      d x  x   +  &#x222B;  a   1      d x  x    )  = 0 ,   {\displaystyle \lim
      _{a\to 0^{+}}\left(\int _{-1}^{-a}{\frac {dx}{x}}+\int _{a}^{1}{\frac
      {dx}{x}}\right)=0,}  [{\displaystyle \lim _{a\to 0^{+}}\left(\int _{-1}^
      {-a}{\frac {dx}{x}}+\int _{a}^{1}{\frac {dx}{x}}\right)=0,}]
          lim  a &#x2192;  0  +      (   &#x222B;  &#x2212; 1   &#x2212; a
      d x  x   +  &#x222B;  2 a   1      d x  x    )  = &#x2212; ln &#x2061; 2.
      {\displaystyle \lim _{a\to 0^{+}}\left(\int _{-1}^{-a}{\frac {dx}
      {x}}+\int _{2a}^{1}{\frac {dx}{x}}\right)=-\ln 2.}  [{\displaystyle \lim
      _{a\to 0^{+}}\left(\int _{-1}^{-a}{\frac {dx}{x}}+\int _{2a}^{1}{\frac
      {dx}{x}}\right)=-\ln 2.}]
The former is the Cauchy principal value of the otherwise ill-defined
expression
          &#x222B;  &#x2212; 1   1      d x  x    &#xA0;   (    which   &#xA0;
      gives   &#xA0; &#x2212; &#x221E; + &#x221E;  )  .   {\displaystyle \int _
      {-1}^{1}{\frac {dx}{x}}{\ }\left({\mbox{which}}\ {\mbox{gives}}\ -\infty
      +\infty \right).}  [{\displaystyle \int _{-1}^{1}{\frac {dx}{x}}{\ }\left
      ({\mbox{which}}\ {\mbox{gives}}\ -\infty +\infty \right).}]
Similarly, we have
          lim  a &#x2192; &#x221E;    &#x222B;  &#x2212; a   a      2 x  d x
      x  2   + 1    = 0 ,   {\displaystyle \lim _{a\to \infty }\int _{-a}^{a}
      {\frac {2x\,dx}{x^{2}+1}}=0,}  [{\displaystyle \lim _{a\to \infty }\int _
      {-a}^{a}{\frac {2x\,dx}{x^{2}+1}}=0,}]
but
          lim  a &#x2192; &#x221E;    &#x222B;  &#x2212; 2 a   a      2 x  d x
      x  2   + 1    = &#x2212; ln &#x2061; 4.   {\displaystyle \lim _{a\to
      \infty }\int _{-2a}^{a}{\frac {2x\,dx}{x^{2}+1}}=-\ln 4.}  [
      {\displaystyle \lim _{a\to \infty }\int _{-2a}^{a}{\frac {2x\,dx}{x^
      {2}+1}}=-\ln 4.}]
The former is the principal value of the otherwise ill-defined expression
          &#x222B;  &#x2212; &#x221E;   &#x221E;      2 x  d x    x  2   + 1
      &#xA0;   (    which   &#xA0;   gives   &#xA0; &#x2212; &#x221E; +
      &#x221E;  )  .   {\displaystyle \int _{-\infty }^{\infty }{\frac {2x\,dx}
      {x^{2}+1}}{\ }\left({\mbox{which}}\ {\mbox{gives}}\ -\infty +\infty
      \right).}  [{\displaystyle \int _{-\infty }^{\infty }{\frac {2x\,dx}{x^
      {2}+1}}{\ }\left({\mbox{which}}\ {\mbox{gives}}\ -\infty +\infty
      \right).}]
All of the above limits are cases of the indeterminate_form â − â.
These pathologies do not affect "Lebesgue-integrable" functions, that is,
functions the integrals of whose absolute_values are finite.
***** Summability[edit] *****
An improper integral may diverge in the sense that the limit defining it may
not exist. In this case, there are more sophisticated definitions of the limit
which can produce a convergent value for the improper integral. These are
called summability methods.
One summability method, popular in Fourier_analysis, is that of CesÃ ro
summation. The integral
          &#x222B;  0   &#x221E;   f ( x )  d x   {\displaystyle \int _{0}^
      {\infty }f(x)\,dx}  [{\displaystyle \int _{0}^{\infty }f(x)\,dx}]
is CesÃ ro summable (C, Î±) if
          lim  &#x03BB; &#x2192; &#x221E;    &#x222B;  0   &#x03BB;     (  1
      &#x2212;   x &#x03BB;    )   &#x03B1;   f ( x )  d x   {\displaystyle
      \lim _{\lambda \to \infty }\int _{0}^{\lambda }\left(1-{\frac {x}{\lambda
      }}\right)^{\alpha }f(x)\,dx}  [{\displaystyle \lim _{\lambda \to \infty
      }\int _{0}^{\lambda }\left(1-{\frac {x}{\lambda }}\right)^{\alpha }f
      (x)\,dx}]
exists and is finite (Titchmarsh_1948, Â§1.15). The value of this limit, should
it exist, is the (C, Î±) sum of the integral.
An integral is (C, 0) summable precisely when it exists as an improper
integral. However, there are integrals which are (C, Î±) summable for Î± > 0
which fail to converge as improper integrals (in the sense of Riemann or
Lebesgue). One example is the integral
          &#x222B;  0   &#x221E;   sin &#x2061; x  d x   {\displaystyle \int _
      {0}^{\infty }\sin x\,dx}  [{\displaystyle \int _{0}^{\infty }\sin x\,dx}]
which fails to exist as an improper integral, but is (C,Î±) summable for every
Î± > 0. This is an integral version of Grandi's_series.
***** Multivariable improper integrals[edit] *****
The improper integral can also be defined for functions of several variables.
The definition is slightly different, depending on whether one requires
integrating over an unbounded domain, such as       R   2     {\displaystyle
\mathbb {R} ^{2}}  [\R^2], or is integrating a function with singularities,
like     f ( x , y ) = log &#x2061; (  x  2   +  y  2   )   {\displaystyle f
(x,y)=\log(x^{2}+y^{2})}  [f(x,y)=\log(x^{2}+y^{2})].
**** Improper integrals over arbitrary domains[edit] ****
If     f :   R   n   &#x2192;  R    {\displaystyle f:\mathbb {R} ^{n}\to
\mathbb {R} }  [{\displaystyle f:\mathbb {R} ^{n}\to \mathbb {R} }] is a non-
negative function that is Riemann integrable over every compact cube of the
form     [ &#x2212; a , a  ]  n     {\displaystyle [-a,a]^{n}}  [[-a,a]^{n}],
for     a > 0   {\displaystyle a>0}  [a>0], then the improper integral of f
over       R   n     {\displaystyle \mathbb {R} ^{n}}  [\mathbb {R} ^{n}] is
defined to be the limit
          lim  a &#x2192; &#x221E;    &#x222B;  [ &#x2212; a , a  ]  n     f ,
      {\displaystyle \lim _{a\to \infty }\int _{[-a,a]^{n}}f,}  [\lim _{a\to
      \infty }\int _{[-a,a]^{n}}f,]
provided it exists.
A function on an arbitrary domain A in       R   n     {\displaystyle \mathbb
{R} ^{n}}  [\mathbb {R} ^{n}] is extended to a function        f &#x007E;
{\displaystyle {\tilde {f}}}  [{\tilde {f}}] on       R   n     {\displaystyle
\mathbb {R} ^{n}}  [\mathbb {R} ^{n}] by zero outside of A:
            f &#x007E;    ( x ) =   {    f ( x )   x &#x2208; A     0   x
      &#x2209; A         {\displaystyle {\tilde {f}}(x)={\begin{cases}f(x)&x\in
      A\\0&x\not \in A\end{cases}}}  [{\tilde {f}}(x)={\begin{cases}f(x)&x\in
      A\\0&x\not \in A\end{cases}}]
The Riemann integral of a function over a bounded domain A is then defined as
the integral of the extended function        f &#x007E;      {\displaystyle
{\tilde {f}}}  [{\tilde {f}}] over a cube     [ &#x2212; a , a  ]  n
{\displaystyle [-a,a]^{n}}  [[-a,a]^{n}] containing A:
          &#x222B;  A   f =  &#x222B;  [ &#x2212; a , a  ]  n        f &#x007E;
      .   {\displaystyle \int _{A}f=\int _{[-a,a]^{n}}{\tilde {f}}.}  [\int _
      {A}f=\int _{[-a,a]^{n}}{\tilde {f}}.]
More generally, if A is unbounded, then the improper Riemann integral over an
arbitrary domain in       R   n     {\displaystyle \mathbb {R} ^{n}}  [\mathbb
{R} ^{n}] is defined as the limit:
          &#x222B;  A   f =  lim  a &#x2192; &#x221E;    &#x222B;  A &#x2229;
      [ &#x2212; a , a  ]  n     f =  lim  a &#x2192; &#x221E;    &#x222B;
      [ &#x2212; a , a  ]  n        f &#x007E;    .   {\displaystyle \int _
      {A}f=\lim _{a\to \infty }\int _{A\cap [-a,a]^{n}}f=\lim _{a\to \infty
      }\int _{[-a,a]^{n}}{\tilde {f}}.}  [\int _{A}f=\lim _{a\to \infty }\int _
      {A\cap [-a,a]^{n}}f=\lim _{a\to \infty }\int _{[-a,a]^{n}}{\tilde {f}}.]
**** Improper integrals with singularities[edit] ****
If f is a non-negative function which is unbounded in a domain A, then the
improper integral of f is defined by truncating f at some cutoff M, integrating
the resulting function, and then taking the limit as M tends to infinity. That
is for     M > 0   {\displaystyle M>0}  [M>0], set      f  M   = min { f , M }
{\displaystyle f_{M}=\min\{f,M\}}  [f_{M}=\min\{f,M\}]. Then define
          &#x222B;  A   f =  lim  M &#x2192; &#x221E;    &#x222B;  A    f  M
      {\displaystyle \int _{A}f=\lim _{M\to \infty }\int _{A}f_{M}}  [\int _
      {A}f=\lim _{M\to \infty }\int _{A}f_{M}]
provided this limit exists.
**** Functions with both positive and negative values[edit] ****
These definitions apply for functions that are non-negative. A more general
function f can be decomposed as a difference of its positive part      f  +   =
max { f , 0 }   {\displaystyle f_{+}=\max\{f,0\}}  [f_{+}=\max\{f,0\}] and
negative part      f  &#x2212;   = max { &#x2212; f , 0 }   {\displaystyle f_{-
}=\max\{-f,0\}}  [f_{-}=\max\{-f,0\}], so
         f =  f  +   &#x2212;  f  &#x2212;     {\displaystyle f=f_{+}-f_{-}}
      [f=f_{+}-f_{-}]
with      f  +     {\displaystyle f_{+}}  [f_{+}] and      f  &#x2212;
{\displaystyle f_{-}}  [f_{-}] both non-negative functions. The function f has
an improper Riemann integral if each of      f  +     {\displaystyle f_{+}}
[f_{+}] and      f  &#x2212;     {\displaystyle f_{-}}  [f_{-}] has one, in
which case the value of that improper integral is defined by
          &#x222B;  A   f =  &#x222B;  A    f  +   &#x2212;  &#x222B;  A    f
      &#x2212;   .   {\displaystyle \int _{A}f=\int _{A}f_{+}-\int _{A}f_{-}.}
      [\int _{A}f=\int _{A}f_{+}-\int _{A}f_{-}.]
In order to exist in this sense, the improper integral necessarily converges
absolutely, since
          &#x222B;  A    |  f  |  =  &#x222B;  A    f  +   +  &#x222B;  A    f
      &#x2212;   .   {\displaystyle \int _{A}|f|=\int _{A}f_{+}+\int _{A}f_{-
      }.}  [\int _{A}|f|=\int _{A}f_{+}+\int _{A}f_{-}.][1][2]
***** Notes[edit] *****
   1. ^ Cooper_2005, p. 538: "We need to make this stronger definition of
      convergence in terms of |f(x)| because cancellation in the integrals can
      occur in so many different ways in higher dimensions."
   2. ^ Ghorpade_&_Limaye_2010, p. 448: "The relevant notion here is that of
      unconditional convergence." ... "In fact, for improper integrals of such
      functions, unconditional convergence turns out to be equivalent to
      absolute convergence."
***** Bibliography[edit] *****
    * Apostol,_T (1974), Mathematical analysis, Addison-Wesley, ISBN 978-0-201-
      00288-1
.
Apostol,_T (1967), Calculus, Vol. 1 (2nd ed.), Jon Wiley & Sons
.
Autar Kaw, Egwu Kalu (2008), Numerical_Methods_with_Applications (1st ed.),
autarkaw.com
Titchmarsh,_E (1948), Introduction to the theory of Fourier integrals (2nd
ed.), New York, N.Y.: Chelsea Pub. Co. (published 1986), ISBN 978-0-8284-0324-5
.
Cooper, Jeffery (2005), Working analysis, Gulf Professional
Ghorpade, Sudhir; Limaye, Balmohan (2010), A course in multivariable calculus
and analysis, Springer
***** External links[edit] *****
    * Numerical_Methods_to_Solve_Improper_Integrals at Holistic Numerical
      Methods Institute
    * Improper_integrals â chapter from an online textbook
    * v
    * t
    * e
Integrals
                          * Riemann_integral
                          * Lebesgue_integral
                          * Burkill_integral
                          * Bochner_integral
                          * Daniell_integral
                          * Darboux_integral
                          * HenstockâKurzweil_integral
Numerical_integration     * Haar_integral
                          * Hellinger_integral
                          * Khinchin_integral
                          * Kolmogorov_integral
                          * LebesgueâStieltjes_integral
                          * Pettis_integral
                          * Pfeffer_integral
                          * RiemannâStieltjes_integral
                          * Regulated_integral
                          * Integration_by_parts
                          * Integration_by_substitution
                          * Inverse_function_integration
                          * Order_of_integration_(calculus)
                          * trigonometric_substitution
Methods                   * Integration_by_partial_fractions
                          * Integration_by_reduction_formulae
                          * Integration_using_parametric_derivatives
                          * Integration_using_Euler's_formula
                          * Differentiation_under_the_integral_sign
                          * Contour_integration
Improper Integrals        * Improper integral
                          * Gaussian_integral
                          * ItÃ´_integral
Stochastic integrals      * RussoâVallois_integral
                          * Stratonovich_integral
                          * Skorokhod_integral

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Improper_integral&oldid=886418366"
Categories:
    * Integral_calculus
Hidden categories:
    * Articles_with_short_description
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 6 March 2019, at 04:20 (UTC).
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
