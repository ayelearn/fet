The following text has been accessed from https://en.wikipedia.org/wiki/Z-transform at Fri Aug 9 03:38:30 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Z-transform ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For standard z-score in statistics, see Standard_score. For Fisher z-
transformation in statistics, see Fisher_transformation.
In mathematics and signal_processing, the Z-transform converts a discrete-time
signal, which is a sequence of real or complex_numbers, into a complex
frequency-domain representation.
It can be considered as a discrete-time equivalent of the Laplace_transform.
This similarity is explored in the theory of time-scale_calculus.
⁰
***** Contents *****
    * 1_History
    * 2_Definition
          o 2.1_Bilateral_Z-transform
          o 2.2_Unilateral_Z-transform
          o 2.3_Geophysical_definition
    * 3_Inverse_Z-transform
    * 4_Region_of_convergence
          o 4.1_Example_1_(no_ROC)
          o 4.2_Example_2_(causal_ROC)
          o 4.3_Example_3_(anti_causal_ROC)
          o 4.4_Examples_conclusion
    * 5_Properties
    * 6_Table_of_common_Z-transform_pairs
    * 7_Relationship_to_Fourier_series_and_Fourier_transform
    * 8_Relationship_to_Laplace_transform
          o 8.1_Bilinear_transform
          o 8.2_Starred_transform
    * 9_Linear_constant-coefficient_difference_equation
          o 9.1_Transfer_function
          o 9.2_Zeros_and_poles
          o 9.3_Output_response
    * 10_See_also
    * 11_References
    * 12_Further_reading
    * 13_External_links
***** History[edit] *****
The basic idea now known as the Z-transform was known to Laplace, and it was
re-introduced in 1947 by W._Hurewicz[1][2] and others as a way to treat
sampled-data control systems used with radar. It gives a tractable way to solve
linear, constant-coefficient difference_equations. It was later dubbed "the z-
transform" by Ragazzini and Zadeh in the sampled-data control group at Columbia
University in 1952.[3][4]
The modified or advanced_Z-transform was later developed and popularized by E.
I._Jury.[5][6]
The idea contained within the Z-transform is also known in mathematical
literature as the method of generating_functions which can be traced back as
early as 1730 when it was introduced by de_Moivre in conjunction with
probability theory.[7] From a mathematical view the Z-transform can also be
viewed as a Laurent_series where one views the sequence of numbers under
consideration as the (Laurent) expansion of an analytic function.
***** Definition[edit] *****
The Z-transform can be defined as either a one-sided or two-sided transform.[8]
**** Bilateral Z-transform[edit] ****
The bilateral or two-sided Z-transform of a discrete-time signal     x [ n ]
{\displaystyle x[n]}  [x[n]] is the formal_power_series     X ( z )
{\displaystyle X(z)}  [X(z)] defined as
         X ( z ) =   Z   { x [ n ] } =  &#x2211;  n = &#x2212;
      &#x221E;   &#x221E;   x [ n ]  z  &#x2212; n                   
      {\displaystyle X(z)={\mathcal {Z}}\{x[n]\}=\sum _{n=-\infty      (Eq.1)
      }^{\infty }x[n]z^{-n}}  [X(z)={\mathcal {Z}}\{x[n]\}=\sum _
      {n=-\infty }^{\infty }x[n]z^{-n}]
where     n   {\displaystyle n}  [n] is an integer and     z   {\displaystyle
z}  [z] is, in general, a complex_number:
         z = A  e  j &#x03D5;   = A &#x22C5; ( cos &#x2061;  &#x03D5;  + j sin
      &#x2061;  &#x03D5;  )   {\displaystyle z=Ae^{j\phi }=A\cdot (\cos {\phi
      }+j\sin {\phi })}  [{\displaystyle z=Ae^{j\phi }=A\cdot (\cos {\phi
      }+j\sin {\phi })}]
where     A   {\displaystyle A}  [A] is the magnitude of     z   {\displaystyle
z}  [z],     j   {\displaystyle j}  [j] is the imaginary_unit, and     &#x03D5;
{\displaystyle \phi }  [\phi ] is the complex_argument (also referred to as
angle or phase) in radians.
**** Unilateral Z-transform[edit] ****
Alternatively, in cases where     x [ n ]   {\displaystyle x[n]}  [x[n]] is
defined only for     n &#x2265; 0   {\displaystyle n\geq 0}  [n\geq 0], the
single-sided or unilateral Z-transform is defined as
         X ( z ) =   Z   { x [ n ] } =  &#x2211;  n = 0   &#x221E;
      x [ n ]  z  &#x2212; n   .   {\displaystyle X(z)={\mathcal      (Eq.2)
      {Z}}\{x[n]\}=\sum _{n=0}^{\infty }x[n]z^{-n}.}  [X(z)=          
      {\mathcal {Z}}\{x[n]\}=\sum _{n=0}^{\infty }x[n]z^{-n}.]
In signal_processing, this definition can be used to evaluate the Z-transform
of the unit_impulse_response of a discrete-time causal_system.
An important example of the unilateral Z-transform is the probability-
generating_function, where the component     x [ n ]   {\displaystyle x[n]}  [x
[n]] is the probability that a discrete random variable takes the value     n
{\displaystyle n}  [n], and the function     X ( z )   {\displaystyle X(z)}  [X
(z)] is usually written as     X ( s )   {\displaystyle X(s)}  [X(s)] in terms
of     s =  z  &#x2212; 1     {\displaystyle s=z^{-1}}  [{\displaystyle s=z^{-
1}}]. The properties of Z-transforms (below) have useful interpretations in the
context of probability theory.
**** Geophysical definition[edit] ****
In geophysics, the usual definition for the Z-transform is a power series in z
as opposed to zâ1. This convention is used, for example, by Robinson and
Treitel[9] and by Kanasewich.[1] The geophysical definition is:
         X ( z ) =   Z   { x [ n ] } =  &#x2211;  n   x [ n ]  z  n   .
      {\displaystyle X(z)={\mathcal {Z}}\{x[n]\}=\sum _{n}x[n]z^{n}.}  [X(z)=
      {\mathcal {Z}}\{x[n]\}=\sum _{n}x[n]z^{n}.]
The two definitions are equivalent; however, the difference results in a number
of changes. For example, the location of zeros_and_poles move from inside the
unit_circle using one definition, to outside the unit circle using the other
definition.[9][1] Thus, care is required to note which definition is being used
by a particular author.
***** Inverse Z-transform[edit] *****
The inverse Z-transform is
         x [ n ] =    Z    &#x2212; 1   { X ( z ) } =   1  2
      &#x03C0; j        &#x222E;       C   &#x2061; X ( z )  z  n
      &#x2212; 1   d z   {\displaystyle x[n]={\mathcal {Z}}^{-1}\    (Eq.3)
      {X(z)\}={\frac {1}{2\pi j}}\oint _{C}X(z)z^{n-1}dz}  [x[n]=    
      {\mathcal {Z}}^{-1}\{X(z)\}={\frac {1}{2\pi j}}\oint _{C}X
      (z)z^{n-1}dz]
where C is a counterclockwise closed path encircling the origin and entirely in
the region_of_convergence (ROC). In the case where the ROC is causal (see
Example_2), this means the path C must encircle all of the poles of     X ( z )
{\displaystyle X(z)}  [X(z)].
A special case of this contour_integral occurs when C is the unit circle. This
contour can be used when the ROC includes the unit circle, which is always
guaranteed when     X ( z )   {\displaystyle X(z)}  [X(z)] is stable, that is,
when all the poles are inside the unit circle. With this contour, the inverse
Z-transform simplifies to the inverse_discrete-time_Fourier_transform, or
Fourier_series, of the periodic values of the Z-transform around the unit
circle:
         x [ n ] =   1  2 &#x03C0;     &#x222B;  &#x2212; &#x03C0;   + &#x03C0;
      X (  e  j &#x03C9;   )  e  j &#x03C9; n   d &#x03C9; .   {\displaystyle x
      [n]={\frac {1}{2\pi }}\int _{-\pi }^{+\pi }X(e^{j\omega })e^{j\omega
      n}d\omega .}  [x[n]={\frac {1}{2\pi }}\int _{-\pi }^{+\pi }X(e^{j\omega
      })e^{j\omega n}d\omega .]
The Z-transform with a finite range of n and a finite number of uniformly
spaced z values can be computed efficiently via Bluestein's_FFT_algorithm. The
discrete-time_Fourier_transform (DTFT)ânot to be confused with the discrete
Fourier_transform (DFT)âis a special case of such a Z-transform obtained by
restricting z to lie on the unit circle.
***** Region of convergence[edit] *****
The region_of_convergence (ROC) is the set of points in the complex plane for
which the Z-transform summation converges.
          R O C  =  {  z :  |   &#x2211;  n = &#x2212; &#x221E;   &#x221E;   x
      [ n ]  z  &#x2212; n    |  < &#x221E;  }    {\displaystyle \mathrm {ROC}
      =\left\{z:\left|\sum _{n=-\infty }^{\infty }x[n]z^{-n}\right|<\infty
      \right\}}  [{\displaystyle \mathrm {ROC} =\left\{z:\left|\sum _{n=-\infty
      }^{\infty }x[n]z^{-n}\right|<\infty \right\}}]
**** Example 1 (no ROC)[edit] ****
Let x[n] = (0.5)n. Expanding x[n] on the interval (ââ, â) it becomes
         x [ n ] =  {  &#x22EF; ,  0.5  &#x2212; 3   ,  0.5  &#x2212; 2   ,
      0.5  &#x2212; 1   , 1 , 0.5 ,  0.5  2   ,  0.5  3   , &#x22EF;  }  =
      {  &#x22EF; ,  2  3   ,  2  2   , 2 , 1 , 0.5 ,  0.5  2   ,  0.5  3   ,
      &#x22EF;  }  .   {\displaystyle x[n]=\left\{\cdots ,0.5^{-3},0.5^{-
      2},0.5^{-1},1,0.5,0.5^{2},0.5^{3},\cdots \right\}=\left\{\cdots ,2^{3},2^
      {2},2,1,0.5,0.5^{2},0.5^{3},\cdots \right\}.}  [x[n]=\left\{\cdots ,0.5^
      {-3},0.5^{-2},0.5^{-1},1,0.5,0.5^{2},0.5^{3},\cdots \right\}=\left\
      {\cdots ,2^{3},2^{2},2,1,0.5,0.5^{2},0.5^{3},\cdots \right\}.]
Looking at the sum
          &#x2211;  n = &#x2212; &#x221E;   &#x221E;   x [ n ]  z  &#x2212; n
      &#x2192; &#x221E; .   {\displaystyle \sum _{n=-\infty }^{\infty }x[n]z^{-
      n}\to \infty .}  [\sum _{n=-\infty }^{\infty }x[n]z^{-n}\to \infty .]
Therefore, there are no values of z that satisfy this condition.
**** Example 2 (causal ROC)[edit] ****
ROC shown in blue, the unit circle as a dotted grey circle and the circle
|z| = 0.5 is shown as a dashed black circle
Let     x [ n ] =  0.5  n   u [ n ] &#xA0;   {\displaystyle x[n]=0.5^{n}u[n]\ }
[x[n]=0.5^{n}u[n]\ ] (where u is the Heaviside_step_function). Expanding x[n]
on the interval (ââ, â) it becomes
         x [ n ] =  {  &#x22EF; , 0 , 0 , 0 , 1 , 0.5 ,  0.5  2   ,  0.5  3   ,
      &#x22EF;  }  .   {\displaystyle x[n]=\left\{\cdots ,0,0,0,1,0.5,0.5^
      {2},0.5^{3},\cdots \right\}.}  [x[n]=\left\{\cdots ,0,0,0,1,0.5,0.5^
      {2},0.5^{3},\cdots \right\}.]
Looking at the sum
          &#x2211;  n = &#x2212; &#x221E;   &#x221E;   x [ n ]  z  &#x2212; n
      =  &#x2211;  n = 0   &#x221E;    0.5  n    z  &#x2212; n   =  &#x2211;  n
      = 0   &#x221E;     (   0.5 z   )   n   =   1  1 &#x2212; 0.5  z  &#x2212;
      1      .   {\displaystyle \sum _{n=-\infty }^{\infty }x[n]z^{-n}=\sum _
      {n=0}^{\infty }0.5^{n}z^{-n}=\sum _{n=0}^{\infty }\left({\frac {0.5}
      {z}}\right)^{n}={\frac {1}{1-0.5z^{-1}}}.}  [\sum _{n=-\infty }^{\infty
      }x[n]z^{-n}=\sum _{n=0}^{\infty }0.5^{n}z^{-n}=\sum _{n=0}^{\infty }\left
      ({\frac {0.5}{z}}\right)^{n}={\frac {1}{1-0.5z^{-1}}}.]
The last equality arises from the infinite geometric_series and the equality
only holds if |0.5zâ1| < 1 which can be rewritten in terms of z as |z| > 0.5.
Thus, the ROC is |z| > 0.5. In this case the ROC is the complex plane with a
disc of radius 0.5 at the origin "punched out".
**** Example 3 (anti causal ROC)[edit] ****
ROC shown in blue, the unit circle as a dotted grey circle and the circle
|z| = 0.5 is shown as a dashed black circle
Let     x [ n ] = &#x2212; ( 0.5  )  n   u [ &#x2212; n &#x2212; 1 ] &#xA0;
{\displaystyle x[n]=-(0.5)^{n}u[-n-1]\ }  [x[n]=-(0.5)^{n}u[-n-1]\ ] (where u
is the Heaviside_step_function). Expanding x[n] on the interval (ââ, â)
it becomes
         x [ n ] =  {  &#x22EF; , &#x2212; ( 0.5  )  &#x2212; 3   , &#x2212;
      ( 0.5  )  &#x2212; 2   , &#x2212; ( 0.5  )  &#x2212; 1   , 0 , 0 , 0 , 0
      , &#x22EF;  }  .   {\displaystyle x[n]=\left\{\cdots ,-(0.5)^{-3},-(0.5)^
      {-2},-(0.5)^{-1},0,0,0,0,\cdots \right\}.}  [x[n]=\left\{\cdots ,-(0.5)^
      {-3},-(0.5)^{-2},-(0.5)^{-1},0,0,0,0,\cdots \right\}.]
Looking at the sum
          &#x2211;  n = &#x2212; &#x221E;   &#x221E;   x [ n ]  z  &#x2212; n
      = &#x2212;  &#x2211;  n = &#x2212; &#x221E;   &#x2212; 1    0.5  n    z
      &#x2212; n   = &#x2212;  &#x2211;  m = 1   &#x221E;     (   z 0.5   )   m
      = &#x2212;     0.5  &#x2212; 1   z   1 &#x2212;  0.5  &#x2212; 1   z    =
      &#x2212;   1  0.5  z  &#x2212; 1   &#x2212; 1    =   1  1 &#x2212; 0.5  z
      &#x2212; 1      .   {\displaystyle \sum _{n=-\infty }^{\infty }x[n]z^{-
      n}=-\sum _{n=-\infty }^{-1}0.5^{n}z^{-n}=-\sum _{m=1}^{\infty }\left(
      {\frac {z}{0.5}}\right)^{m}=-{\frac {0.5^{-1}z}{1-0.5^{-1}z}}=-{\frac {1}
      {0.5z^{-1}-1}}={\frac {1}{1-0.5z^{-1}}}.}  [{\displaystyle \sum _{n=-
      \infty }^{\infty }x[n]z^{-n}=-\sum _{n=-\infty }^{-1}0.5^{n}z^{-n}=-\sum
      _{m=1}^{\infty }\left({\frac {z}{0.5}}\right)^{m}=-{\frac {0.5^{-1}z}{1-
      0.5^{-1}z}}=-{\frac {1}{0.5z^{-1}-1}}={\frac {1}{1-0.5z^{-1}}}.}]
Using the infinite geometric_series, again, the equality only holds if
|0.5â1z| < 1 which can be rewritten in terms of z as |z| < 0.5. Thus, the ROC
is |z| < 0.5. In this case the ROC is a disc centered at the origin and of
radius 0.5.
What differentiates this example from the previous example is only the ROC.
This is intentional to demonstrate that the transform result alone is
insufficient.
**** Examples conclusion[edit] ****
Examples 2 & 3 clearly show that the Z-transform X(z) of x[n] is unique when
and only when specifying the ROC. Creating the poleâzero_plot for the causal
and anticausal case show that the ROC for either case does not include the pole
that is at 0.5. This extends to cases with multiple poles: the ROC will never
contain poles.
In example 2, the causal system yields an ROC that includes |z| = â while the
anticausal system in example 3 yields an ROC that includes |z| = 0.
ROC shown as a blue ring 0.5 < |z| < 0.75
In systems with multiple poles it is possible to have a ROC that includes
neither |z| = â nor |z| = 0. The ROC creates a circular band. For example,
         x [ n ] =  0.5  n   u [ n ] &#x2212;  0.75  n   u [ &#x2212; n
      &#x2212; 1 ]   {\displaystyle x[n]=0.5^{n}u[n]-0.75^{n}u[-n-1]}  [x
      [n]=0.5^{n}u[n]-0.75^{n}u[-n-1]]
has poles at 0.5 and 0.75. The ROC will be 0.5 < |z| < 0.75, which includes
neither the origin nor infinity. Such a system is called a mixed-causality
system as it contains a causal term (0.5)nu[n] and an anticausal term −(0.75)nu
[−n−1].
The stability of a system can also be determined by knowing the ROC alone. If
the ROC contains the unit circle (i.e., |z| = 1) then the system is stable. In
the above systems the causal system (Example 2) is stable because |z| > 0.5
contains the unit circle.
If you are provided a Z-transform of a system without a ROC (i.e., an ambiguous
x[n]) you can determine a unique x[n] provided you desire the following:
    * Stability
    * Causality
If you need stability then the ROC must contain the unit circle. If you need a
causal system then the ROC must contain infinity and the system function will
be a right-sided sequence. If you need an anticausal system then the ROC must
contain the origin and the system function will be a left-sided sequence. If
you need both stability and causality, all the poles of the system function
must be inside the unit circle.
The unique x[n] can then be found.
***** Properties[edit] *****
                                                Properties of the z-transform
                Time domain           Z-domain       Proof              ROC
                                         X ( z ) =
                   x [ n ] =    Z     Z   { x [ n ]
                &#x2212; 1   { X ( z  }
                ) }   {\displaystyle  {\displaystyle                        r  2   <  |  z  |  <  r  1     {\displaystyle r_
Notation        x[n]={\mathcal {Z}}^  X(z)={\mathcal                    {2}<|z|<r_{1}}  [r_{2}<|z|<r_{1}]
                {-1}\{X(z)\}}  [x[n]= {Z}}\{x[n]\}}
                {\mathcal {Z}}^{-1}\  [X(z)=
                {X(z)\}]              {\mathcal
                                      {Z}}\{x[n]\}]
                                                            X ( z )
                                                     =  &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   (  a  1
                                                     x  1   ( n ) +  a
                                                     2    x  2   ( n )
                                                     )  z  &#x2212; n
                                                     =  a  1
                                                     &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;    x  1
                                                     ( n )  z  &#x2212;
                                                     n   +  a  2
                                                     &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;    x  2
                                                     ( n )  z  &#x2212;
                                                     n         =  a  1
                                                     X  1   ( z ) +  a
                                                     2    X  2   ( z )
                                          a  1    X  {\displaystyle
                                      1   ( z ) +  a {\begin{aligned}X
                    a  1    x  1      2    X  2      (z)&=\sum _{n=-
                [ n ] +  a  2    x  2 ( z )          \infty }^{\infty }
                [ n ]                 {\displaystyle (a_{1}x_{1}(n)+a_
Linearity       {\displaystyle a_     a_{1}X_{1}     {2}x_{2}(n))z^{-   Contains ROC1 â© ROC2
                {1}x_{1}[n]+a_{2}x_   (z)+a_{2}X_{2} n}\\&=a_{1}\sum _
                {2}[n]}  [a_{1}x_{1}  (z)}  [a_{1}X_ {n=-\infty }^
                [n]+a_{2}x_{2}[n]]    {1}(z)+a_{2}X_ {\infty }x_{1}
                                      {2}(z)]        (n)z^{-n}+a_
                                                     {2}\sum _{n=-
                                                     \infty }^{\infty
                                                     }x_{2}(n)z^{-
                                                     n}\\&=a_{1}X_{1}
                                                     (z)+a_{2}X_{2}
                                                     (z)\end{aligned}}}
                                                     [{\begin{aligned}X
                                                     (z)&=\sum _{n=-
                                                     \infty }^{\infty }
                                                     (a_{1}x_{1}(n)+a_
                                                     {2}x_{2}(n))z^{-
                                                     n}\\&=a_{1}\sum _
                                                     {n=-\infty }^
                                                     {\infty }x_{1}
                                                     (n)z^{-n}+a_
                                                     {2}\sum _{n=-
                                                     \infty }^{\infty
                                                     }x_{2}(n)z^{-
                                                     n}\\&=a_{1}X_{1}
                                                     (z)+a_{2}X_{2}
                                                     (z)\end{aligned}}]
                                                             X  K   ( z
                                                     )    =  &#x2211;
                                                     n = &#x2212;
                                                     &#x221E;
                                                     &#x221E;    x  K
                                                     ( n )  z  &#x2212;
                                                     n         =
                                                     &#x2211;  r =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   x ( r )
                    x  K   [ n ] =                   z  &#x2212; r K
                {    x [ r ] ,   n =                 =  &#x2211;  r =
                K r     0 ,   n                      &#x2212; &#x221E;
                &#x2209; K  Z                        &#x221E;   x ( r )
                {\displaystyle x_{K}                 (  z  K    )
                [n]={\begin{cases}x                  &#x2212; r
                [r],&n=Kr\\0,&n\notin                = X (  z  K   )
                K\mathbb {Z} \end                    {\displaystyle
                {cases}}}  [             X (  z  K   {\begin{aligned}X_
                {\displaystyle x_{K}  )              {K}(z)&=\sum _{n=-
Time_expansion  [n]={\begin{cases}x   {\displaystyle \infty }^{\infty       R   1 K      {\displaystyle R^{\frac {1}{K}}}
                [r],&n=Kr\\0,&n\notin X(z^{K})}  [X  }x_{K}(n)z^{-      [R^{\frac {1}{K}}]
                K\mathbb {Z} \end     (z^{K})]       n}\\&=\sum _{r=-
                {cases}}}]                           \infty }^{\infty
                with     K  Z  := { K                }x(r)z^{-
                r : r &#x2208;  Z  }                 rK}\\&=\sum _{r=-
                {\displaystyle                       \infty }^{\infty
                K\mathbb {Z} :=\{Kr:                 }x(r)(z^{K})^{-
                r\in \mathbb {Z} \}}                 r}\\&=X(z^{K})\end
                [{\displaystyle                      {aligned}}}  [
                K\mathbb {Z} :=\{Kr:                 {\begin{aligned}X_
                r\in \mathbb {Z} \}}]                {K}(z)&=\sum _{n=-
                                                     \infty }^{\infty
                                                     }x_{K}(n)z^{-
                                                     n}\\&=\sum _{r=-
                                                     \infty }^{\infty
                                                     }x(r)z^{-
                                                     rK}\\&=\sum _{r=-
                                                     \infty }^{\infty
                                                     }x(r)(z^{K})^{-
                                                     r}\\&=X(z^{K})\end
                                                     {aligned}}]
                                           1 K
                                      &#x2211;  p =
                                      0   K &#x2212;
                                      1   X  (   z
                                      1 K
                                      &#x22C5;  e
                                      &#x2212; i
                                      2 &#x03C0;  K
                                      p    )
                                      {\displaystyle
                                      {\frac {1}
                                      {K}}\sum _
                   x [ K n ]          {p=0}^{K-
Decimation      {\displaystyle x[Kn]} 1}X\left(z^    ohio-state.edu  or
                [{\displaystyle x     {\tfrac {1}     ee.ic.ac.uk
                [Kn]}]                {K}}\cdot e^{-
                                      i{\tfrac {2\pi
                                      }
                                      {K}}p}\right)}
                                      [{\frac {1}
                                      {K}}\sum _
                                      {p=0}^{K-
                                      1}X\left(z^
                                      {\tfrac {1}
                                      {K}}\cdot e^{-
                                      i{\tfrac {2\pi
                                      }
                                      {K}}p}\right)]
                                                            Z { x [ n
                                                     &#x2212; k ] }
                                                     =  &#x2211;  n = 0
                                                     &#x221E;   x [ n
                                                     &#x2212; k ]  z
                                                     &#x2212; n
                                                     =  &#x2211;  j =
                                                     &#x2212; k
                                                     &#x221E;   x [ j ]
                                                     z  &#x2212; ( j +
                                                     k )      j = n
                                                     &#x2212; k       =
                                                     &#x2211;  j =
                                                     &#x2212; k
                                                     &#x221E;   x [ j ]
                                                     z  &#x2212; j    z
                                                     &#x2212; k
                                                     =  z  &#x2212; k
                                                     &#x2211;  j =
                                                     &#x2212; k
                                                     &#x221E;   x [ j ]
                                                     z  &#x2212; j
                                                     =  z  &#x2212; k
                                                     &#x2211;  j = 0
                                                     &#x221E;   x [ j ]
                                                     z  &#x2212; j
                                                     x [ &#x03B2; ] = 0
                   x [ n &#x2212; k ]                , &#x03B2; < 0
                {\displaystyle x[n-                  =  z  &#x2212; k
                k]}  [x[n-k]]                        X ( z )
                with     k > 0            z          {\displaystyle
                {\displaystyle k>0}   &#x2212; k   X {\begin{aligned}Z\
                [k>0] and     x : x   ( z )          {x[n-k]\}&=\sum _
Time delay      [ n ] = 0 &#xA0;      {\displaystyle {n=0}^{\infty }x   ROC, except z = 0 if k > 0 and z = â if k < 0
                &#x2200; n < 0        z^{-k}X(z)}    [n-k]z^{-
                {\displaystyle x:x    [z^{-k}X(z)]   n}\\&=\sum _{j=-
                [n]=0\ \forall n<0}                  k}^{\infty }x[j]z^
                [{\displaystyle x:x                  {-(j+k)}&&j=n-
                [n]=0\ \forall n<0}]                 k\\&=\sum _{j=-k}^
                                                     {\infty }x[j]z^{-
                                                     j}z^{-k}\\&=z^{-
                                                     k}\sum _{j=-k}^
                                                     {\infty }x[j]z^{-
                                                     j}\\&=z^{-k}\sum _
                                                     {j=0}^{\infty }x
                                                     [j]z^{-j}&&x[\beta
                                                     ]=0,\beta <0\\&=z^
                                                     {-k}X(z)\end
                                                     {aligned}}}  [
                                                     {\begin{aligned}Z\
                                                     {x[n-k]\}&=\sum _
                                                     {n=0}^{\infty }x
                                                     [n-k]z^{-
                                                     n}\\&=\sum _{j=-
                                                     k}^{\infty }x[j]z^
                                                     {-(j+k)}&&j=n-
                                                     k\\&=\sum _{j=-k}^
                                                     {\infty }x[j]z^{-
                                                     j}z^{-k}\\&=z^{-
                                                     k}\sum _{j=-k}^
                                                     {\infty }x[j]z^{-
                                                     j}\\&=z^{-k}\sum _
                                                     {j=0}^{\infty }x
                                                     [j]z^{-j}&&x[\beta
                                                     ]=0,\beta <0\\&=z^
                                                     {-k}X(z)\end
                                                     {aligned}}]
                                      Bilateral Z-
                                      transform:
                                          z  k   X
                                      ( z )
                                      {\displaystyle
                                      z^{k}X(z)}
                                      [
                                      {\displaystyle
                                      z^{k}X(z)}]
                                      Unilateral Z-
                   x [ n + k ]        transform:[10]
                {\displaystyle x          z  k   X
                [n+k]}  [             ( z ) &#x2212;
                {\displaystyle x      z  k
Time advance    [n+k]}]               &#x2211;  n =
                with     k > 0        0   k &#x2212;
                {\displaystyle k>0}   1   x [ n ]  z
                [k>0]                 &#x2212; n
                                      {\displaystyle
                                      z^{k}X(z)-z^
                                      {k}\sum _
                                      {n=0}^{k-1}x
                                      [n]z^{-n}}
                                      [
                                      {\displaystyle
                                      z^{k}X(z)-z^
                                      {k}\sum _
                                      {n=0}^{k-1}x
                                      [n]z^{-n}}]
                                         ( 1
                   x [ n ] &#x2212; x &#x2212;  z
First           [ n &#x2212; 1 ]      &#x2212; 1   )
difference      {\displaystyle x[n]-x X ( z )                           Contains the intersection of ROC of X1(z) and z â  0
backward        [n-1]}  [x[n]-x[n-1]] {\displaystyle
                with x[n]=0 for n<0   (1-z^{-1})X
                                      (z)}  [(1-z^{-
                                      1})X(z)]
                                         ( z
                                      &#x2212; 1 ) X
                   x [ n + 1 ]        ( z ) &#x2212;
First           &#x2212; x [ n ]      z x [ 0 ]
difference      {\displaystyle x      {\displaystyle
forward         [n+1]-x[n]}  [        (z-1)X(z)-zx
                {\displaystyle x      [0]}  [
                [n+1]-x[n]}]          {\displaystyle
                                      (z-1)X(z)-zx
                                      [0]}]
                                                              Z   { x
                                                     ( &#x2212; n ) }
                                                     =  &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   x
                                                     ( &#x2212; n )  z
                                                     &#x2212; n
                                                     =  &#x2211;  m =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   x ( m )
                                                     z  m         =
                                                     &#x2211;  m =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   x ( m )
                                                     (  z  &#x2212; 1
                                                     )   &#x2212; m
                                                     = X (  z  &#x2212;
                                                     1   )
                                                     {\displaystyle
                                                     {\begin{aligned}
                                         X (  z      {\mathcal {Z}}\{x
                   x [ &#x2212; n ]   &#x2212; 1   ) (-n)\}&=\sum _{n=-       1  r  1      <  |  z  |  <    1  r  2
Time reversal   {\displaystyle x[-n]} {\displaystyle \infty }^{\infty   {\displaystyle {\tfrac {1}{r_{1}}}<|z|<{\tfrac {1}{r_
                [x[-n]]               X(z^{-1})}  [X }x(-n)z^{-         {2}}}}  [{\tfrac {1}{r_{1}}}<|z|<{\tfrac {1}{r_{2}}}]
                                      (z^{-1})]      n}\\&=\sum _{m=-
                                                     \infty }^{\infty
                                                     }x(m)z^{m}\\&=\sum
                                                     _{m=-\infty }^
                                                     {\infty }x(m){(z^
                                                     {-1})}^{-m}\\&=X
                                                     (z^{-1})\\\end
                                                     {aligned}}}  [
                                                     {\begin{aligned}
                                                     {\mathcal {Z}}\{x
                                                     (-n)\}&=\sum _{n=-
                                                     \infty }^{\infty
                                                     }x(-n)z^{-
                                                     n}\\&=\sum _{m=-
                                                     \infty }^{\infty
                                                     }x(m)z^{m}\\&=\sum
                                                     _{m=-\infty }^
                                                     {\infty }x(m){(z^
                                                     {-1})}^{-m}\\&=X
                                                     (z^{-1})\\\end
                                                     {aligned}}]
                                                              Z
                                                     {   a  n   x [ n ]
                                                     }     =  &#x2211;
                                                     n = &#x2212;
                                                     &#x221E;
                                                     &#x221E;    a  n
                                                     x ( n )  z
                                                     &#x2212; n
                                                     =  &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   x ( n )
                                                     (  a  &#x2212; 1
                                                     z  )  &#x2212; n
                                                     = X (  a  &#x2212;
                                                     1   z )
                                                     {\displaystyle
                                                     {\begin{aligned}
                                         X (  a      {\mathcal
                    a  n   x [ n ]    &#x2212; 1   z {Z}}\left\{a^{n}x      |  a  |   r  2   <  |  z  |  <  |  a  |   r  1
Scaling in the  {\displaystyle a^{n}x )              [n]\right\}&=\sum  {\displaystyle |a|r_{2}<|z|<|a|r_{1}}  [|a|r_
z-domain        [n]}  [a^{n}x[n]]     {\displaystyle _{n=-\infty }^     {2}<|z|<|a|r_{1}]
                                      X(a^{-1}z)}    {\infty }a^{n}x
                                      [X(a^{-1}z)]   (n)z^{-n}\\&=\sum
                                                     _{n=-\infty }^
                                                     {\infty }x(n)(a^{-
                                                     1}z)^{-n}\\&=X(a^
                                                     {-1}z)\end
                                                     {aligned}}}  [
                                                     {\begin{aligned}
                                                     {\mathcal
                                                     {Z}}\left\{a^{n}x
                                                     [n]\right\}&=\sum
                                                     _{n=-\infty }^
                                                     {\infty }a^{n}x
                                                     (n)z^{-n}\\&=\sum
                                                     _{n=-\infty }^
                                                     {\infty }x(n)(a^{-
                                                     1}z)^{-n}\\&=X(a^
                                                     {-1}z)\end
                                                     {aligned}}]
                                                              Z   {  x
                                                     &#x2217;   ( n ) }
                                                     =  &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;    x
                                                     &#x2217;   ( n )
                                                     z  &#x2212; n
                                                     =  &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;     [  x
                                                     ( n ) (  z
                                                     &#x2217;    )
                                                     &#x2212; n    ]
                                                     &#x2217;         =
                                                     [   &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   x ( n )
                                                     (  z  &#x2217;
                                                     )  &#x2212; n    ]
                                                     &#x2217;         =
                                                     X  &#x2217;   (  z
                                                     &#x2217;   )
                                                     {\displaystyle
                                                     {\begin{aligned}
                                                     {\mathcal {Z}}\{x^
                                          X          {*}(n)\}&=\sum _
                                      &#x2217;       {n=-\infty }^
Complex             x  &#x2217;   [ n (  z  &#x2217; {\infty }x^{*}
conjugation     ]   {\displaystyle x^ )              (n)z^{-n}\\&=\sum
                {*}[n]}  [x^{*}[n]]   {\displaystyle _{n=-\infty }^
                                      X^{*}(z^{*})}  {\infty }\left[x
                                      [X^{*}(z^{*})] (n)(z^{*})^{-
                                                     n}\right]^
                                                     {*}\\&=\left[\sum
                                                     _{n=-\infty }^
                                                     {\infty }x(n)(z^
                                                     {*})^{-n}\right]^
                                                     {*}\\&=X^{*}(z^
                                                     {*})\end
                                                     {aligned}}}  [
                                                     {\begin{aligned}
                                                     {\mathcal {Z}}\{x^
                                                     {*}(n)\}&=\sum _
                                                     {n=-\infty }^
                                                     {\infty }x^{*}
                                                     (n)z^{-n}\\&=\sum
                                                     _{n=-\infty }^
                                                     {\infty }\left[x
                                                     (n)(z^{*})^{-
                                                     n}\right]^
                                                     {*}\\&=\left[\sum
                                                     _{n=-\infty }^
                                                     {\infty }x(n)(z^
                                                     {*})^{-n}\right]^
                                                     {*}\\&=X^{*}(z^
                                                     {*})\end
                                                     {aligned}}]
                                            1 2
                                      [  X ( z ) +
                                      X  &#x2217;
                   Re &#x2061; { x    (  z  &#x2217;
                [ n ] }               )  ]
                {\displaystyle        {\displaystyle
Real_part       \operatorname {Re} \  {\tfrac {1}
                {x[n]\}}              {2}}\left[X
                [\operatorname {Re} \ (z)+X^{*}(z^
                {x[n]\}]              {*})\right]}
                                      [{\tfrac {1}
                                      {2}}\left[X
                                      (z)+X^{*}(z^
                                      {*})\right]]
                                            1  2 j
                                      [  X ( z )
                                      &#x2212;  X
                                      &#x2217;
                   Im &#x2061; { x    (  z  &#x2217;
                [ n ] }               )  ]
                {\displaystyle        {\displaystyle
Imaginary_part  \operatorname {Im} \  {\tfrac {1}
                {x[n]\}}              {2j}}\left[X
                [\operatorname {Im} \ (z)-X^{*}(z^
                {x[n]\}]              {*})\right]}
                                      [{\tfrac {1}
                                      {2j}}\left[X
                                      (z)-X^{*}(z^
                                      {*})\right]]
                                                              Z   { n x
                                                     ( n ) }    =
                                                     &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   n x ( n
                                                     )  z  &#x2212; n
                                                     = z  &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   n x ( n
                                                     )  z  &#x2212; n
                                                     &#x2212; 1
                                                     = &#x2212; z
                                                     &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   x ( n )
                                                     ( &#x2212; n  z
                                                     &#x2212; n
                                                     &#x2212; 1   )
                                                     = &#x2212; z
                                                     &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   x ( n )
                                                     d  d z    (  z
                                                     &#x2212; n   )
                                                     = &#x2212; z    d
                                                     X ( z )   d z
                                                     {\displaystyle
                                         &#x2212; z  {\begin{aligned}
                                      d X ( z )   d  {\mathcal {Z}}\{nx
                                      z              (n)\}&=\sum _{n=-  ROC, if     X ( z )   {\displaystyle X(z)}  [X(z)] is
                   n x [ n ]          {\displaystyle \infty }^{\infty   rational;
Differentiation {\displaystyle nx[n]} -z{\frac {dX   }nx(n)z^{-         ROC possibly excluding the boundary, if     X ( z )
                [nx[n]]               (z)}{dz}}}  [- n}\\&=z\sum _{n=-  {\displaystyle X(z)}  [X(z)] is irrational[11]
                                      z{\frac {dX    \infty }^{\infty
                                      (z)}{dz}}]     }nx(n)z^{-n-
                                                     1}\\&=-z\sum _{n=-
                                                     \infty }^{\infty
                                                     }x(n)(-nz^{-n-
                                                     1})\\&=-z\sum _
                                                     {n=-\infty }^
                                                     {\infty }x(n)
                                                     {\frac {d}{dz}}(z^
                                                     {-n})\\&=-z{\frac
                                                     {dX(z)}{dz}}\end
                                                     {aligned}}}  [
                                                     {\begin{aligned}
                                                     {\mathcal {Z}}\{nx
                                                     (n)\}&=\sum _{n=-
                                                     \infty }^{\infty
                                                     }nx(n)z^{-
                                                     n}\\&=z\sum _{n=-
                                                     \infty }^{\infty
                                                     }nx(n)z^{-n-
                                                     1}\\&=-z\sum _{n=-
                                                     \infty }^{\infty
                                                     }x(n)(-nz^{-n-
                                                     1})\\&=-z\sum _
                                                     {n=-\infty }^
                                                     {\infty }x(n)
                                                     {\frac {d}{dz}}(z^
                                                     {-n})\\&=-z{\frac
                                                     {dX(z)}{dz}}\end
                                                     {aligned}}]
                                                              Z   {  x
                                                     1   ( n ) &#x2217;
                                                     x  2   ( n ) }
                                                     =   Z
                                                     {   &#x2211;  l =
                                                     &#x2212; &#x221E;
                                                     &#x221E;    x  1
                                                     ( l )  x  2   ( n
                                                     &#x2212; l )  }
                                                     =  &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;
                                                     [   &#x2211;  l =
                                                     &#x2212; &#x221E;
                                                     &#x221E;    x  1
                                                     ( l )  x  2   ( n
                                                     &#x2212; l )  ]
                                                     z  &#x2212; n
                                                     =  &#x2211;  l =
                                                     &#x2212; &#x221E;
                                                     &#x221E;    x  1
                                                     ( l )
                                                     [   &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;    x  2
                                                     ( n &#x2212; l )
                                                     z  &#x2212; n    ]
                                                     =  [   &#x2211;  l
                                                     = &#x2212;
                                                     &#x221E;
                                                     &#x221E;    x  1
                                                     ( l )  z  &#x2212;
                                                     l    ]
                                                     [   &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;    x  2
                                                     ( n )  z  &#x2212;
                                                     n    ]        =  X
                                                     1   ( z )  X  2
                                                     ( z )
                                                     {\displaystyle
                                                     {\begin{aligned}
                                                     {\mathcal {Z}}\{x_
                                                     {1}(n)*x_{2}
                                                     (n)\}&={\mathcal
                                                     {Z}}\left\{\sum _
                                                     {l=-\infty }^
                                                     {\infty }x_{1}
                                                     (l)x_{2}(n-
                                          X  1   ( z l)\right\}\\&=\sum
                    x  1   [ n ]      )  X  2   ( z  _{n=-\infty }^
                &#x2217;  x  2   [ n  )              {\infty }\left
Convolution     ]   {\displaystyle x_ {\displaystyle [\sum _{l=-\infty  Contains ROC1 â© ROC2
                {1}[n]*x_{2}[n]}  [x_ X_{1}(z)X_{2}  }^{\infty }x_{1}
                {1}[n]*x_{2}[n]]      (z)}  [X_{1}   (l)x_{2}(n-
                                      (z)X_{2}(z)]   l)\right]z^{-
                                                     n}\\&=\sum _{l=-
                                                     \infty }^{\infty
                                                     }x_{1}(l)\left
                                                     [\sum _{n=-\infty
                                                     }^{\infty }x_{2}
                                                     (n-l)z^{-
                                                     n}\right]\\&=\left
                                                     [\sum _{l=-\infty
                                                     }^{\infty }x_{1}
                                                     (l)z^{-
                                                     l}\right]\!\!\left
                                                     [\sum _{n=-\infty
                                                     }^{\infty }x_{2}
                                                     (n)z^{-
                                                     n}\right]\\&=X_{1}
                                                     (z)X_{2}(z)\end
                                                     {aligned}}}  [
                                                     {\begin{aligned}
                                                     {\mathcal {Z}}\{x_
                                                     {1}(n)*x_{2}
                                                     (n)\}&={\mathcal
                                                     {Z}}\left\{\sum _
                                                     {l=-\infty }^
                                                     {\infty }x_{1}
                                                     (l)x_{2}(n-
                                                     l)\right\}\\&=\sum
                                                     _{n=-\infty }^
                                                     {\infty }\left
                                                     [\sum _{l=-\infty
                                                     }^{\infty }x_{1}
                                                     (l)x_{2}(n-
                                                     l)\right]z^{-
                                                     n}\\&=\sum _{l=-
                                                     \infty }^{\infty
                                                     }x_{1}(l)\left
                                                     [\sum _{n=-\infty
                                                     }^{\infty }x_{2}
                                                     (n-l)z^{-
                                                     n}\right]\\&=\left
                                                     [\sum _{l=-\infty
                                                     }^{\infty }x_{1}
                                                     (l)z^{-
                                                     l}\right]\!\!\left
                                                     [\sum _{n=-\infty
                                                     }^{\infty }x_{2}
                                                     (n)z^{-
                                                     n}\right]\\&=X_{1}
                                                     (z)X_{2}(z)\end
                                                     {aligned}}]
                                          R   x  1
                                      ,  x  2
                                      ( z ) =  X  1
                                      &#x2217;
                    r   x  1   ,  x   (    1  z
                2     =  x  1         &#x2217;
                &#x2217;   [ &#x2212; )  X  2   ( z
                n ] &#x2217;  x  2    )                                 Contains the intersection of ROC of      X  1
Cross-          [ n ]                 {\displaystyle                    (    1  z  &#x2217;      )   {\displaystyle X_{1}(
correlation     {\displaystyle r_{x_  R_{x_{1},x_                       {\tfrac {1}{z^{*}}})}  [X_{1}({\tfrac {1}{z^{*}}})]
                {1},x_{2}}=x_{1}^{*}  {2}}(z)=X_{1}^                    and      X  2   ( z )   {\displaystyle X_{2}(z)}  [X_
                [-n]*x_{2}[n]}  [r_   {*}({\tfrac                       {2}(z)]
                {x_{1},x_{2}}=x_{1}^  {1}{z^{*}}})X_
                {*}[-n]*x_{2}[n]]     {2}(z)}  [R_
                                      {x_{1},x_{2}}
                                      (z)=X_{1}^{*}(
                                      {\tfrac {1}{z^
                                      {*}}})X_{2}
                                      (z)]
                                                             &#x2211;
                                                     n = &#x2212;
                                                     &#x221E;
                                                     &#x221E;
                                                     &#x2211;  k =
                                                     &#x2212; &#x221E;
                                                     n   x [ k ]  z
                                                     &#x2212; n      =
                                                     &#x2211;  n =
                                                     &#x2212; &#x221E;
                                                     &#x221E;   ( x [ n
                                                     ] + &#x22EF; + x
                                                     [ &#x2212;
                                                     &#x221E; ] )  z
                                                     &#x2212; n
                                                     = X [ z ]  (  1 +
                                                     z  &#x2212; 1   +
                                                     z  &#x2212; 2   +
                                                     &#x22EF;  )
                                                     = X [ z ]
                                                     &#x2211;  j = 0
                                                     &#x221E;    z
                                                     &#x2212; j
                                                     = X [ z ]   1  1
                                                     &#x2212;  z
                                                     &#x2212; 1
                                                     {\displaystyle
                                                     {\begin
                                           1  1      {aligned}\sum _
                    &#x2211;  k =     &#x2212;  z    {n=-\infty }^
                &#x2212; &#x221E;   n &#x2212; 1     {\infty }\sum _
                x [ k ]               X ( z )        {k=-\infty }^{n}x
Accumulation    {\displaystyle \sum _ {\displaystyle [k]z^{-n}&=\sum _
                {k=-\infty }^{n}x[k]} {\frac {1}{1-  {n=-\infty }^
                [\sum _{k=-\infty }^  z^{-1}}}X(z)}  {\infty }(x
                {n}x[k]]              [{\frac {1}{1- [n]+\cdots +x[-
                                      z^{-1}}}X(z)]  \infty ])z^{-
                                                     n}\\&=X[z]\left
                                                     (1+z^{-1}+z^{-
                                                     2}+\cdots
                                                     \right)\\&=X
                                                     [z]\sum _{j=0}^
                                                     {\infty }z^{-
                                                     j}\\&=X[z]{\frac
                                                     {1}{1-z^{-1}}}\end
                                                     {aligned}}}  [
                                                     {\begin
                                                     {aligned}\sum _
                                                     {n=-\infty }^
                                                     {\infty }\sum _
                                                     {k=-\infty }^{n}x
                                                     [k]z^{-n}&=\sum _
                                                     {n=-\infty }^
                                                     {\infty }(x
                                                     [n]+\cdots +x[-
                                                     \infty ])z^{-
                                                     n}\\&=X[z]\left
                                                     (1+z^{-1}+z^{-
                                                     2}+\cdots
                                                     \right)\\&=X
                                                     [z]\sum _{j=0}^
                                                     {\infty }z^{-
                                                     j}\\&=X[z]{\frac
                                                     {1}{1-z^{-1}}}\end
                                                     {aligned}}]
                                           1  j 2
                                      &#x03C0;
                                      &#x222E;
                                      C   &#x2061;
                                      X  1   ( v )
                                      X  2   (    z
                                      v    )  v
                                      &#x2212; 1
                                      d  v
                    x  1   [ n ]  x   {\displaystyle
                2   [ n ]             {\frac {1}
Multiplication  {\displaystyle x_{1}  {j2\pi }}\oint                    -
                [n]x_{2}[n]}  [x_{1}  _{C}X_{1}(v)X_
                [n]x_{2}[n]]          {2}({\tfrac
                                      {z}{v}})v^{-
                                      1}\mathrm {d}
                                      v}  [{\frac
                                      {1}{j2\pi
                                      }}\oint _{C}X_
                                      {1}(v)X_{2}(
                                      {\tfrac {z}
                                      {v}})v^{-
                                      1}\mathrm {d}
                                      v]
Parseval's_theorem
          &#x2211;  n = &#x2212; &#x221E;   &#x221E;    x  1   [ n ]  x  2
      &#x2217;   [ n ]  =    1  j 2 &#x03C0;        &#x222E;       C   &#x2061;
      X  1   ( v )  X  2   &#x2217;   (    1  v  &#x2217;      )  v  &#x2212; 1
      d  v   {\displaystyle \sum _{n=-\infty }^{\infty }x_{1}[n]x_{2}^{*}
      [n]\quad =\quad {\frac {1}{j2\pi }}\oint _{C}X_{1}(v)X_{2}^{*}({\tfrac
      {1}{v^{*}}})v^{-1}\mathrm {d} v}  [\sum _{n=-\infty }^{\infty }x_{1}[n]x_
      {2}^{*}[n]\quad =\quad {\frac {1}{j2\pi }}\oint _{C}X_{1}(v)X_{2}^{*}(
      {\tfrac {1}{v^{*}}})v^{-1}\mathrm {d} v]
Initial_value_theorem: If x[n] is causal, then
         x [ 0 ] =  lim  z &#x2192; &#x221E;   X ( z ) .   {\displaystyle x
      [0]=\lim _{z\to \infty }X(z).}  [x[0]=\lim _{z\to \infty }X(z).]
Final_value_theorem: If the poles of (zâ1)X(z) are inside the unit circle,
then
         x [ &#x221E; ] =  lim  z &#x2192; 1   ( z &#x2212; 1 ) X ( z ) .
      {\displaystyle x[\infty ]=\lim _{z\to 1}(z-1)X(z).}  [x[\infty ]=\lim _
      {z\to 1}(z-1)X(z).]
***** Table of common Z-transform pairs[edit] *****
Here:
         u : n &#x21A6; u [ n ] =   {    1 ,   n &#x2265; 0     0 ,   n < 0
      {\displaystyle u:n\mapsto u[n]={\begin{cases}1,&n\geq 0\\0,&n<0\end
      {cases}}}  [u:n\mapsto u[n]={\begin{cases}1,&n\geq 0\\0,&n<0\end{cases}}]
is the unit_(or_Heaviside)_step_function and
         &#x03B4; : n &#x21A6; &#x03B4; [ n ] =   {    1 ,   n = 0     0 ,   n
      &#x2260; 0         {\displaystyle \delta :n\mapsto \delta [n]={\begin
      {cases}1,&n=0\\0,&n\neq 0\end{cases}}}  [\delta :n\mapsto \delta [n]=
      {\begin{cases}1,&n=0\\0,&n\neq 0\end{cases}}]
is the discrete-time_unit_impulse_function (cf Dirac_delta_function which is a
continuous-time version). The two functions are chosen together so that the
unit step function is the accumulation (running total) of the unit impulse
function.
   Signal,     x [ n ]      Z-transform,     X ( z )
   {\displaystyle x[n]}  [x {\displaystyle X(z)}  [X  ROC
   [n]]                     (z)]
      &#x03B4; [ n ]
1  {\displaystyle \delta    1                         all z
   [n]}  [\delta [n]]
      &#x03B4; [ n &#x2212;
   n  0   ]                     z  &#x2212;  n  0        z &#x2260; 0
2  {\displaystyle \delta    {\displaystyle z^{-n_     {\displaystyle z\neq 0}
   [n-n_{0}]}  [\delta [n-  {0}}}  [z^{-n_{0}}]       [z\neq 0]
   n_{0}]]
                                 1  1 &#x2212;  z
      u [ n ]               &#x2212; 1                    |  z  |  > 1
3  {\displaystyle u[n]\,}   {\displaystyle {\frac {1} {\displaystyle |z|>1}
   [u[n]\,]                 {1-z^{-1}}}}  [{\frac {1} [|z|>1]
                            {1-z^{-1}}}]
      &#x2212; u [ &#x2212;      1  1 &#x2212;  z
   n &#x2212; 1 ]           &#x2212; 1                    |  z  |  < 1
4  {\displaystyle -u[-n-1]} {\displaystyle {\frac {1} {\displaystyle |z|<1}
   [  -u[-n-1]]             {1-z^{-1}}}}  [ \frac{1}  [|z|<1]
                            {1 - z^{-1}}]
                                  z  &#x2212; 1
                            ( 1 &#x2212;  z  &#x2212;
      n u [ n ]             1    )  2                     |  z  |  > 1
5  {\displaystyle nu[n]}    {\displaystyle {\frac {z^ {\displaystyle |z|>1}
   [nu[n]]                  {-1}}{(1-z^{-1})^{2}}}}   [|z|>1]
                            [{\frac {z^{-1}}{(1-z^{-
                            1})^{2}}}]
                                  z  &#x2212; 1
      &#x2212; n u          ( 1 &#x2212;  z  &#x2212;
   [ &#x2212; n &#x2212; 1  1    )  2                     |  z  |  < 1
6  ]    {\displaystyle -nu  {\displaystyle {\frac {z^ {\displaystyle |z|<1}
   [-n-1]\,}  [-nu[-n-1]\,] {-1}}{(1-z^{-1})^{2}}}}   [|z|<1]
                            [{\frac {z^{-1}}{(1-z^{-
                            1})^{2}}}]
                                   z  &#x2212; 1
                            ( 1 +  z  &#x2212; 1   )
                            ( 1 &#x2212;  z  &#x2212;
       n  2   u [ n ]       1    )  3                     |  z  |  > 1
7  {\displaystyle n^{2}u    {\displaystyle {\frac {z^ {\displaystyle |z|>1\,}
   [n]}  [n^{2}u[n]]        {-1}(1+z^{-1})}{(1-z^{-   [|z|>1\,]
                            1})^{3}}}}  [{\frac {z^{-
                            1}(1+z^{-1})}{(1-z^{-1})^
                            {3}}}]
                                   z  &#x2212; 1
                            ( 1 +  z  &#x2212; 1   )
      &#x2212;  n  2   u    ( 1 &#x2212;  z  &#x2212;
   [ &#x2212; n &#x2212; 1  1    )  3                     |  z  |  < 1
8  ]    {\displaystyle -n^  {\displaystyle {\frac {z^ {\displaystyle |z|<1\,}
   {2}u[-n-1]\,}  [-n^{2}u  {-1}(1+z^{-1})}{(1-z^{-   [|z|<1\,]
   [-n-1]\,]                1})^{3}}}}  [{\frac {z^{-
                            1}(1+z^{-1})}{(1-z^{-1})^
                            {3}}}]
                                   z  &#x2212; 1
                            ( 1 + 4  z  &#x2212; 1
                            +  z  &#x2212; 2   )
                            ( 1 &#x2212;  z  &#x2212;
       n  3   u [ n ]       1    )  4                     |  z  |  > 1
9  {\displaystyle n^{3}u    {\displaystyle {\frac {z^ {\displaystyle |z|>1\,}
   [n]}  [n^{3}u[n]]        {-1}(1+4z^{-1}+z^{-2})}{  [|z|>1\,]
                            (1-z^{-1})^{4}}}}  [
                            {\frac {z^{-1}(1+4z^{-
                            1}+z^{-2})}{(1-z^{-1})^
                            {4}}}]
                                   z  &#x2212; 1
                            ( 1 + 4  z  &#x2212; 1
                            +  z  &#x2212; 2   )
      &#x2212;  n  3   u    ( 1 &#x2212;  z  &#x2212;
   [ &#x2212; n &#x2212; 1  1    )  4                     |  z  |  < 1
10 ]   {\displaystyle -n^   {\displaystyle {\frac {z^ {\displaystyle |z|<1\,}
   {3}u[-n-1]}  [-n^{3}u[-  {-1}(1+4z^{-1}+z^{-2})}{  [|z|<1\,]
   n-1]]                    (1-z^{-1})^{4}}}}  [
                            {\frac {z^{-1}(1+4z^{-
                            1}+z^{-2})}{(1-z^{-1})^
                            {4}}}]
                                 1  1 &#x2212; a  z
       a  n   u [ n ]       &#x2212; 1                    |  z  |  >  |  a  |
11 {\displaystyle a^{n}u    {\displaystyle {\frac {1} {\displaystyle |z|>|a|}
   [n]}  [a^{n}u[n]]        {1-az^{-1}}}}  [{\frac    [|z|>|a|]
                            {1}{1-az^{-1}}}]
      &#x2212;  a  n   u         1  1 &#x2212; a  z
   [ &#x2212; n &#x2212; 1  &#x2212; 1                    |  z  |  <  |  a  |
12 ]   {\displaystyle -a^   {\displaystyle {\frac {1} {\displaystyle |z|<|a|}
   {n}u[-n-1]}  [-a^{n}u[-  {1-az^{-1}}}}  [{\frac    [|z|<|a|]
   n-1]]                    {1}{1-az^{-1}}}]
                                  a  z  &#x2212; 1
                            ( 1 &#x2212; a  z
      n  a  n   u [ n ]     &#x2212; 1    )  2            |  z  |  >  |  a  |
13 {\displaystyle na^{n}u   {\displaystyle {\frac     {\displaystyle |z|>|a|}
   [n]}  [na^{n}u[n]]       {az^{-1}}{(1-az^{-1})^    [|z|>|a|]
                            {2}}}}  [{\frac {az^{-1}}
                            {(1-az^{-1})^{2}}}]
                                  a  z  &#x2212; 1
      &#x2212; n  a  n   u  ( 1 &#x2212; a  z
   [ &#x2212; n &#x2212; 1  &#x2212; 1    )  2            |  z  |  <  |  a  |
14 ]   {\displaystyle -na^  {\displaystyle {\frac     {\displaystyle |z|<|a|}
   {n}u[-n-1]}  [-na^{n}u[- {az^{-1}}{(1-az^{-1})^    [|z|<|a|]
   n-1]]                    {2}}}}  [{\frac {az^{-1}}
                            {(1-az^{-1})^{2}}}]
                                  a  z  &#x2212; 1
                            ( 1 + a  z  &#x2212; 1
       n  2    a  n   u [ n )   ( 1 &#x2212; a  z
   ]   {\displaystyle n^    &#x2212; 1    )  3            |  z  |  >  |  a  |
15 {2}a^{n}u[n]}  [n^{2}a^  {\displaystyle {\frac     {\displaystyle |z|>|a|}
   {n}u[n]]                 {az^{-1}(1+az^{-1})}{(1-  [|z|>|a|]
                            az^{-1})^{3}}}}  [{\frac
                            {az^{-1}(1+az^{-1})}{(1-
                            az^{-1})^{3}}}]
                                  a  z  &#x2212; 1
      &#x2212;  n  2    a   ( 1 + a  z  &#x2212; 1
   n   u [ &#x2212; n       )   ( 1 &#x2212; a  z
   &#x2212; 1 ]             &#x2212; 1    )  3            |  z  |  <  |  a  |
16 {\displaystyle -n^{2}a^  {\displaystyle {\frac     {\displaystyle |z|<|a|}
   {n}u[-n-1]}  [-n^{2}a^   {az^{-1}(1+az^{-1})}{(1-  [|z|<|a|]
   {n}u[-n-1]]              az^{-1})^{3}}}}  [{\frac
                            {az^{-1}(1+az^{-1})}{(1-
                            az^{-1})^{3}}}]
       (     n + m &#x2212;
   1     m &#x2212; 1     )      1  ( 1 &#x2212; a  z
   a  n   u [ n ]           &#x2212; 1    )  m
   {\displaystyle \left(    {\displaystyle {\frac {1}
   {\begin{array}{c}n+m-    {(1-az^{-1})^{m}}}}  [        |  z  |  >  |  a  |
17 1\\m-1\end               {\displaystyle {\frac {1} {\displaystyle |z|>|a|}
   {array}}\right)a^{n}u    {(1-az^{-1})^{m}}}}], for [|z|>|a|]
   [n]}  [{\displaystyle    positive integer     m
   \left({\begin{array}     {\displaystyle m}  [m]
   {c}n+m-1\\m-1\end        [11]
   {array}}\right)a^{n}u
   [n]}]
      ( &#x2212; 1  )  m
   (     &#x2212; n
   &#x2212; 1     m              1  ( 1 &#x2212; a  z
   &#x2212; 1     )   a  n  &#x2212; 1    )  m
   u [ &#x2212; n &#x2212;  {\displaystyle {\frac {1}
   m ]   {\displaystyle (-  {(1-az^{-1})^{m}}}}  [        |  z  |  <  |  a  |
18 1)^{m}\left({\begin      {\displaystyle {\frac {1} {\displaystyle |z|<|a|}
   {array}{c}-n-1\\m-1\end  {(1-az^{-1})^{m}}}}], for [|z|<|a|]
   {array}}\right)a^{n}u[-  positive integer     m
   n-m]}  [{\displaystyle   {\displaystyle m}  [m]
   (-1)^{m}\left({\begin    [11]
   {array}{c}-n-1\\m-1\end
   {array}}\right)a^{n}u[-
   n-m]}]
                                  1 &#x2212;  z
                            &#x2212; 1   cos &#x2061;
                            (  &#x03C9;  0   )   1
                            &#x2212; 2  z  &#x2212; 1
      cos &#x2061;          cos &#x2061; (  &#x03C9;
   (  &#x03C9;  0   n ) u   0   ) +  z  &#x2212; 2        |  z  |  > 1
19 [ n ]   {\displaystyle   {\displaystyle {\frac {1- {\displaystyle |z|>1}
   \cos(\omega _{0}n)u[n]}  z^{-1}\cos(\omega _{0})}  [|z|>1]
   [\cos(\omega _{0}n)u[n]] {1-2z^{-1}\cos(\omega _
                            {0})+z^{-2}}}}  [{\frac
                            {1-z^{-1}\cos(\omega _
                            {0})}{1-2z^{-1}\cos
                            (\omega _{0})+z^{-2}}}]
                                   z  &#x2212; 1
                            sin &#x2061; (  &#x03C9;
                            0   )   1 &#x2212; 2  z
                            &#x2212; 1   cos &#x2061;
      sin &#x2061;          (  &#x03C9;  0   ) +  z
   (  &#x03C9;  0   n ) u   &#x2212; 2                    |  z  |  > 1
20 [ n ]   {\displaystyle   {\displaystyle {\frac {z^ {\displaystyle |z|>1}
   \sin(\omega _{0}n)u[n]}  {-1}\sin(\omega _{0})}{1- [|z|>1]
   [\sin(\omega _{0}n)u[n]] 2z^{-1}\cos(\omega _
                            {0})+z^{-2}}}}  [{\frac
                            {z^{-1}\sin(\omega _{0})}
                            {1-2z^{-1}\cos(\omega _
                            {0})+z^{-2}}}]
                                  1 &#x2212; a  z
                            &#x2212; 1   cos &#x2061;
                            (  &#x03C9;  0   )   1
                            &#x2212; 2 a  z  &#x2212;
       a  n   cos &#x2061;  1   cos &#x2061;
   (  &#x03C9;  0   n ) u   (  &#x03C9;  0   ) +  a
   [ n ]   {\displaystyle   2    z  &#x2212; 2            |  z  |  >  |  a  |
21 a^{n}\cos(\omega _{0}n)u {\displaystyle {\frac {1- {\displaystyle |z|>|a|}
   [n]}  [a^{n}\cos(\omega  az^{-1}\cos(\omega _{0})} [|z|>|a|]
   _{0}n)u[n]]              {1-2az^{-1}\cos(\omega _
                            {0})+a^{2}z^{-2}}}}  [
                            {\frac {1-az^{-1}\cos
                            (\omega _{0})}{1-2az^{-
                            1}\cos(\omega _{0})+a^
                            {2}z^{-2}}}]
                                  a  z  &#x2212; 1
                            sin &#x2061; (  &#x03C9;
                            0   )   1 &#x2212; 2 a  z
                            &#x2212; 1   cos &#x2061;
       a  n   sin &#x2061;  (  &#x03C9;  0   ) +  a
   (  &#x03C9;  0   n ) u   2    z  &#x2212; 2            |  z  |  >  |  a  |
22 [ n ]   {\displaystyle   {\displaystyle {\frac     {\displaystyle |z|>|a|}
   a^{n}\sin(\omega _{0}n)u {az^{-1}\sin(\omega _     [|z|>|a|]
   [n]}  [a^{n}\sin(\omega  {0})}{1-2az^{-1}\cos
   _{0}n)u[n]]              (\omega _{0})+a^{2}z^{-
                            2}}}}  [{\frac {az^{-
                            1}\sin(\omega _{0})}{1-
                            2az^{-1}\cos(\omega _
                            {0})+a^{2}z^{-2}}}]
***** Relationship to Fourier series and Fourier transform[edit] *****
For values of     z   {\displaystyle z}  [z] in the region      |  z  |  = 1
{\displaystyle |z|=1}  [|z|=1], known as the unit_circle, we can express the
transform as a function of a single, real variable, ω, by defining     z =  e
j &#x03C9;     {\displaystyle z=e^{j\omega }}  [{\displaystyle z=e^{j\omega
}}]. And the bi-lateral transform reduces to a Fourier_series:
          &#x2211;  n = &#x2212; &#x221E;   &#x221E;   x [ n ]
      &#xA0;  z  &#x2212; n   =  &#x2211;  n = &#x2212; &#x221E;
      &#x221E;   x [ n ] &#xA0;  e  &#x2212; j &#x03C9; n   ,         
      {\displaystyle \sum _{n=-\infty }^{\infty }x[n]\ z^{-n}=\sum      (Eq.4)
      _{n=-\infty }^{\infty }x[n]\ e^{-j\omega n},}  [\sum _{n=-
      \infty }^{\infty }x[n]\ z^{-n}=\sum _{n=-\infty }^{\infty }x
      [n]\ e^{-j\omega n},]
which is also known as the discrete-time_Fourier_transform (DTFT) of the     x
[ n ]   {\displaystyle x[n]}  [x[n]] sequence. This 2Ï-periodic function is
the periodic_summation of a Fourier_transform, which makes it a widely used
analysis tool. To understand this, let     X ( f )   {\displaystyle X(f)}  [X
(f)] be the Fourier transform of any function,     x ( t )   {\displaystyle x
(t)}  [x(t)], whose samples at some interval, T, equal the x[n] sequence. Then
the DTFT of the x[n] sequence can be written as follows.
              &#x2211;  n = &#x2212; &#x221E;   &#x221E;       x
      ( n T )  &#x23DE;    x [ n ]   &#xA0;  e  &#x2212; j 2
      &#x03C0; f n T    &#x23DF;    DTFT   =   1 T    &#x2211;  k
      = &#x2212; &#x221E;   &#x221E;   X ( f &#x2212; k  /  T ) .
      {\displaystyle \underbrace {\sum _{n=-\infty }^{\infty          (Eq.5)
      }\overbrace {x(nT)} ^{x[n]}\ e^{-j2\pi fnT}} _{\text{DTFT}}=    
      {\frac {1}{T}}\sum _{k=-\infty }^{\infty }X(f-k/T).}
      [\underbrace {\sum _{n=-\infty }^{\infty }\overbrace {x(nT)}
      ^{x[n]}\ e^{-j2\pi fnT}} _{\text{DTFT}}={\frac {1}{T}}\sum _
      {k=-\infty }^{\infty }X(f-k/T).]
When T has units of seconds,      f    {\displaystyle \scriptstyle f}
[\scriptstyle f] has units of hertz. Comparison of the two series reveals that
      &#x03C9; = 2 &#x03C0; f T    {\displaystyle \scriptstyle \omega =2\pi fT}
[\scriptstyle \omega =2\pi fT]  is a normalized_frequency with units of radians
per sample. The value Ï=2Ï corresponds to      f =   1 T      {\displaystyle
\scriptstyle f={\frac {1}{T}}}  [\scriptstyle f={\frac {1}{T}}] Hz.  And now,
with the substitution       f =   &#x03C9;  2 &#x03C0; T    ,    {\displaystyle
\scriptstyle f={\frac {\omega }{2\pi T}},}  [\scriptstyle f={\frac {\omega }
{2\pi T}},]  Eq.4 can be expressed in terms of the Fourier transform, X(â¢):
          &#x2211;  n = &#x2212; &#x221E;   &#x221E;   x [ n ]
      &#xA0;  e  &#x2212; j &#x03C9; n   =   1 T    &#x2211;  k =
      &#x2212; &#x221E;   &#x221E;       X  (     &#x03C9;  2
      &#x03C0; T     &#x2212;    k T     )   &#x23DF;    X
      (    &#x03C9; &#x2212; 2 &#x03C0; k   2 &#x03C0; T    )    .
      {\displaystyle \sum _{n=-\infty }^{\infty }x[n]\ e^{-j\omega    
      n}={\frac {1}{T}}\sum _{k=-\infty }^{\infty }\underbrace          (Eq.6)
      {X\left({\tfrac {\omega }{2\pi T}}-{\tfrac {k}{T}}\right)} _
      {X\left({\frac {\omega -2\pi k}{2\pi T}}\right)}.}  [\sum _
      {n=-\infty }^{\infty }x[n]\ e^{-j\omega n}={\frac {1}
      {T}}\sum _{k=-\infty }^{\infty }\underbrace {X\left({\tfrac
      {\omega }{2\pi T}}-{\tfrac {k}{T}}\right)} _{X\left({\frac
      {\omega -2\pi k}{2\pi T}}\right)}.]
As parameter T changes, the individual terms of Eq.5 move farther apart or
closer together along the f-axis. In Eq.6 however, the centers remain 2Ï
apart, while their widths expand or contract. When sequence x(nT) represents
the impulse_response of an LTI_system, these functions are also known as its
frequency_response. When the     x ( n T )   {\displaystyle x(nT)}  [
{\displaystyle x(nT)}] sequence is periodic, its DTFT is divergent at one or
more harmonic frequencies, and zero at all other frequencies. This is often
represented by the use of amplitude-variant Dirac_delta functions at the
harmonic frequencies. Due to periodicity, there are only a finite number of
unique amplitudes, which are readily computed by the much simpler discrete
Fourier_transform (DFT).  (See DTFT;_periodic_data.)
***** Relationship to Laplace transform[edit] *****
**** Bilinear transform[edit] ****
Main article: Bilinear_transform
The bilinear transform can be used to convert continuous-time filters
(represented in the Laplace domain) into discrete-time filters (represented in
the Z-domain), and vice versa. The following substitution is used:
         s =   2 T      ( z &#x2212; 1 )   ( z + 1 )      {\displaystyle s=
      {\frac {2}{T}}{\frac {(z-1)}{(z+1)}}}  [s={\frac {2}{T}}{\frac {(z-1)}{
      (z+1)}}]
to convert some function     H ( s )   {\displaystyle H(s)}  [H(s)] in the
Laplace domain to a function     H ( z )   {\displaystyle H(z)}  [H(z)] in the
Z-domain (Tustin_transformation), or
         z =    2 + s T   2 &#x2212; s T      {\displaystyle z={\frac {2+sT}{2-
      sT}}}  [z={\frac {2+sT}{2-sT}}]
from the Z-domain to the Laplace domain. Through the bilinear transformation,
the complex s-plane (of the Laplace transform) is mapped to the complex z-plane
(of the z-transform). While this mapping is (necessarily) nonlinear, it is
useful in that it maps the entire     j &#x03C9;   {\displaystyle j\omega }
[j\omega ] axis of the s-plane onto the unit_circle in the z-plane. As such,
the Fourier transform (which is the Laplace transform evaluated on the     j
&#x03C9;   {\displaystyle j\omega }  [j\omega ] axis) becomes the discrete-time
Fourier transform. This assumes that the Fourier transform exists; i.e., that
the     j &#x03C9;   {\displaystyle j\omega }  [j\omega ] axis is in the region
of convergence of the Laplace transform.
**** Starred transform[edit] ****
Main article: Starred_transform
Given a one-sided Z-transform, X(z), of a time-sampled function, the
corresponding starred transform produces a Laplace transform and restores the
dependence on sampling parameter, T:
               X  &#x2217;   ( s ) = X ( z )    |     z =  e  s T
      {\displaystyle {\bigg .}X^{*}(s)=X(z){\bigg |}_{\displaystyle z=e^{sT}}}
      [{\bigg .}X^{*}(s)=X(z){\bigg |}_{\displaystyle z=e^{sT}}]
The inverse Laplace transform is a mathematical abstraction known as an
impulse-sampled function.
***** Linear constant-coefficient difference equation[edit] *****
The linear constant-coefficient difference (LCCD) equation is a representation
for a linear system based on the autoregressive_moving-average equation.
          &#x2211;  p = 0   N   y [ n &#x2212; p ]  &#x03B1;  p   =  &#x2211;
      q = 0   M   x [ n &#x2212; q ]  &#x03B2;  q     {\displaystyle \sum _
      {p=0}^{N}y[n-p]\alpha _{p}=\sum _{q=0}^{M}x[n-q]\beta _{q}}  [\sum _
      {p=0}^{N}y[n-p]\alpha _{p}=\sum _{q=0}^{M}x[n-q]\beta _{q}]
Both sides of the above equation can be divided by Î±0, if it is not zero,
normalizing Î±0 = 1 and the LCCD equation can be written
         y [ n ] =  &#x2211;  q = 0   M   x [ n &#x2212; q ]  &#x03B2;  q
      &#x2212;  &#x2211;  p = 1   N   y [ n &#x2212; p ]  &#x03B1;  p   .
      {\displaystyle y[n]=\sum _{q=0}^{M}x[n-q]\beta _{q}-\sum _{p=1}^{N}y[n-
      p]\alpha _{p}.}  [y[n]=\sum _{q=0}^{M}x[n-q]\beta _{q}-\sum _{p=1}^{N}y
      [n-p]\alpha _{p}.]
This form of the LCCD equation is favorable to make it more explicit that the
"current" output y[n] is a function of past outputs y[nâp], current input x
[n], and previous inputs x[nâq].
**** Transfer function[edit] ****
Taking the Z-transform of the above equation (using linearity and time-shifting
laws) yields
         Y ( z )  &#x2211;  p = 0   N    z  &#x2212; p    &#x03B1;  p   = X ( z
      )  &#x2211;  q = 0   M    z  &#x2212; q    &#x03B2;  q     {\displaystyle
      Y(z)\sum _{p=0}^{N}z^{-p}\alpha _{p}=X(z)\sum _{q=0}^{M}z^{-q}\beta _{q}}
      [Y(z)\sum _{p=0}^{N}z^{-p}\alpha _{p}=X(z)\sum _{q=0}^{M}z^{-q}\beta _
      {q}]
and rearranging results in
         H ( z ) =    Y ( z )   X ( z )    =     &#x2211;  q = 0   M    z
      &#x2212; q    &#x03B2;  q      &#x2211;  p = 0   N    z  &#x2212; p
      &#x03B1;  p      =     &#x03B2;  0   +  z  &#x2212; 1    &#x03B2;  1   +
      z  &#x2212; 2    &#x03B2;  2   + &#x22EF; +  z  &#x2212; M    &#x03B2;  M
      &#x03B1;  0   +  z  &#x2212; 1    &#x03B1;  1   +  z  &#x2212; 2
      &#x03B1;  2   + &#x22EF; +  z  &#x2212; N    &#x03B1;  N      .
      {\displaystyle H(z)={\frac {Y(z)}{X(z)}}={\frac {\sum _{q=0}^{M}z^{-
      q}\beta _{q}}{\sum _{p=0}^{N}z^{-p}\alpha _{p}}}={\frac {\beta _{0}+z^{-
      1}\beta _{1}+z^{-2}\beta _{2}+\cdots +z^{-M}\beta _{M}}{\alpha _{0}+z^{-
      1}\alpha _{1}+z^{-2}\alpha _{2}+\cdots +z^{-N}\alpha _{N}}}.}  [H(z)=
      {\frac {Y(z)}{X(z)}}={\frac {\sum _{q=0}^{M}z^{-q}\beta _{q}}{\sum _
      {p=0}^{N}z^{-p}\alpha _{p}}}={\frac {\beta _{0}+z^{-1}\beta _{1}+z^{-
      2}\beta _{2}+\cdots +z^{-M}\beta _{M}}{\alpha _{0}+z^{-1}\alpha _{1}+z^{-
      2}\alpha _{2}+\cdots +z^{-N}\alpha _{N}}}.]
**** Zeros and poles[edit] ****
From the fundamental_theorem_of_algebra the numerator has M roots
(corresponding to zeros of H) and the denominator has N roots (corresponding to
poles). Rewriting the transfer_function in terms of zeros_and_poles
         H ( z ) =    ( 1 &#x2212;  q  1    z  &#x2212; 1   ) ( 1 &#x2212;  q
      2    z  &#x2212; 1   ) &#x22EF; ( 1 &#x2212;  q  M    z  &#x2212; 1   )
      ( 1 &#x2212;  p  1    z  &#x2212; 1   ) ( 1 &#x2212;  p  2    z  &#x2212;
      1   ) &#x22EF; ( 1 &#x2212;  p  N    z  &#x2212; 1   )
      {\displaystyle H(z)={\frac {(1-q_{1}z^{-1})(1-q_{2}z^{-1})\cdots (1-q_
      {M}z^{-1})}{(1-p_{1}z^{-1})(1-p_{2}z^{-1})\cdots (1-p_{N}z^{-1})}}}  [H
      (z)={\frac {(1-q_{1}z^{-1})(1-q_{2}z^{-1})\cdots (1-q_{M}z^{-1})}{(1-p_
      {1}z^{-1})(1-p_{2}z^{-1})\cdots (1-p_{N}z^{-1})}}]
where qk is the k-th zero and pk is the k-th pole. The zeros and poles are
commonly complex and when plotted on the complex plane (z-plane) it is called
the poleâzero_plot.
In addition, there may also exist zeros and poles at z = 0 and z = â. If we
take these poles and zeros as well as multiple-order zeros and poles into
consideration, the number of zeros and poles are always equal.
By factoring the denominator, partial_fraction decomposition can be used, which
can then be transformed back to the time domain. Doing so would result in the
impulse_response and the linear constant coefficient difference equation of the
system.
**** Output response[edit] ****
If such a system H(z) is driven by a signal X(z) then the output is Y(z) = H
(z)X(z). By performing partial_fraction decomposition on Y(z) and then taking
the inverse Z-transform the output y[n] can be found. In practice, it is often
useful to fractionally decompose         Y ( z )  z      {\displaystyle
\textstyle {\frac {Y(z)}{z}}}  [{\displaystyle \textstyle {\frac {Y(z)}{z}}}]
before multiplying that quantity by z to generate a form of Y(z) which has
terms with easily computable inverse Z-transforms.
***** See also[edit] *****
    * Advanced_Z-transform
    * Bilinear_transform
    * Difference_equation (recurrence relation)
    * Discrete_convolution
    * Discrete-time_Fourier_transform
    * Finite_impulse_response
    * Formal_power_series
    * Generating_function
    * Generating_function_transformation
    * Laplace_transform
    * Laurent_series
    * Probability-generating_function
    * Star_transform
    * Zak_transform
    * Zeta_function_regularization
***** References[edit] *****
   1. ^ a b c E. R. Kanasewich (1981). Time_Sequence_Analysis_in_Geophysics.
      University of Alberta. pp. 186, 249. ISBN 978-0-88864-074-1.
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
   3. ^E. R. Kanasewich (1981). Time_sequence_analysis_in_geophysics (3rd ed.).
      University of Alberta. pp. 185â186. ISBN 978-0-88864-074-1.
   4. ^J. R. Ragazzini and L. A. Zadeh (1952). "The analysis of sampled-data
      systems". Trans. Am. Inst. Elec. Eng. 71 (II): 225â234.
   5. ^Cornelius T. Leondes (1996). Digital_control_systems_implementation_and
      computational_techniques. Academic Press. p. 123. ISBN 978-0-12-012779-5.
   6. ^ Eliahu Ibrahim Jury (1958). Sampled-Data Control Systems. John Wiley &
      Sons.
   7. ^ Eliahu Ibrahim Jury (1973). Theory and Application of the Z-Transform
      Method. Krieger Pub Co. ISBN 0-88275-122-0.
   8. ^ Eliahu Ibrahim Jury (1964). Theory and Application of the Z-Transform
      Method. John Wiley & Sons. p. 1.
   9. ^ Just like we have the one-sided_Laplace_transform and the two-sided
      Laplace_transform.
  10. ^ a b Enders A. Robinson, Sven Treitel (2008). Digital_Imaging_and
      Deconvolution:_The_ABCs_of_Seismic_Exploration_and_Processing_Digital
      Imaging_and_Deconvolution:_The_ABCs_of_Seismic_Exploration_and
      Processing. SEG Books. pp. 163, 375â376. ISBN 9781560801481.
  11. ^Bolzern, Paolo; Scattolini, Riccardo; Schiavoni, Nicola. Fondamenti di
      Controlli Automatici (in Italian). MC Graw Hill Education. ISBN 978-88-
      386-6882-1.
  12. ^ a b cA. R. Forouzan (2016). "Region of convergence of derivative of Z
      transform". Elec. Lett. IET. 52 (8): 617â619. doi:10.1049/el.2016.0189.
***** Further reading[edit] *****
    * Refaat El Attar, Lecture notes on Z-Transform, Lulu Press, Morrisville
      NC, 2005.
ISBN 1-4116-1979-X.
Ogata, Katsuhiko, Discrete Time Control Systems 2nd Ed, Prentice-Hall Inc,
1995, 1987.
ISBN 0-13-034281-5.
Alan V. Oppenheim and Ronald W. Schafer (1999). Discrete-Time Signal
Processing, 2nd Edition, Prentice Hall Signal Processing Series.
ISBN 0-13-754920-2.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Z-transform", Encyclopedia_of
      Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Numerical_inversion_of_the_Z-transform
Z-Transform_table_of_some_common_Laplace_transforms
Mathworld's_entry_on_the_Z-transform
Z-Transform_threads_in_Comp.DSP
A_graphic_of_the_relationship_between_Laplace_transform_s-plane_to_Z-plane_of
the_Z_transform
An_video_based_explanation_of_the_Z-Transform_for_engineers
    * v
    * t
    * e
Digital_signal_processing
               * Detection_theory
Theory         * Discrete_signal
               * Estimation_theory
               * NyquistâShannon_sampling_theorem
               * Audio_signal_processing
Sub-fields     * Digital_image_processing
               * Speech_processing
               * Statistical_signal_processing
               * Advanced_Z-transform
               * Bilinear_transform
               * Constant-Q_transform
               * Discrete_Fourier_transform (DFT)
               * Discrete-time_Fourier_transform (DTFT)
               * Impulse_invariance
Techniques     * Integral_transform
               * Laplace_transform
               * Matched_Z-transform_method
               * Post's_inversion_formula
               * Starred_transform
               * Z-transform
               * Zak_transform
               * Aliasing
               * Anti-aliasing_filter
               * Downsampling
               * Nyquist_rate / frequency
Sampling       * Oversampling
               * Quantization
               * Sampling_rate
               * Undersampling
               * Upsampling

Retrieved from "https://en.wikipedia.org/w/index.php?title=Z-
transform&oldid=903878218"
Categories:
    * Transforms
    * Laplace_transforms
Hidden categories:
    * CS1_Italian-language_sources_(it)
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
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * à´®à´²à´¯à´¾à´³à´
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 28 June 2019, at 14:15 (UTC).
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
