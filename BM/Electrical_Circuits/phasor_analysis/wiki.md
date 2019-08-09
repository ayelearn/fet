The following text has been accessed from https://en.wikipedia.org/wiki/Phasor at Fri Aug 9 02:45:09 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Phasor ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other uses, see Phasor_(disambiguation).
Not to be confused with phaser.
"Complex amplitude" redirects here. For the quantum-mechanical concept, see
Complex_probability_amplitude.
An example of series RLC_circuit and respective phasor diagram for a specific ω
In physics and engineering, a phasor (a portmanteau of phase vector[1][2]), is
a complex_number representing a sinusoidal_function whose amplitude (A),
angular_frequency (Ï), and initial_phase (Î¸) are time-invariant. It is
related to a more general concept called analytic_representation,[3] which
decomposes a sinusoid into the product of a complex constant and a factor that
encapsulates the frequency and time dependence. The complex constant, which
encapsulates amplitude and phase dependence, is known as phasor, complex
amplitude,[4][5] and (in older texts) sinor[6] or even complexor.[6]
A common situation in electrical networks is the existence of multiple
sinusoids all with the same frequency, but different amplitudes and phases. The
only difference in their analytic representations is the complex amplitude
(phasor). A linear combination of such functions can be factored into the
product of a linear combination of phasors (known as phasor arithmetic) and the
time/frequency dependent factor that they all have in common.
The origin of the term phasor rightfully suggests that a (diagrammatic)
calculus somewhat similar to that possible for vectors is possible for phasors
as well.[6] An important additional feature of the phasor transform is that
differentiation and integration of sinusoidal signals (having constant
amplitude, period and phase) corresponds to simple algebraic operations on the
phasors; the phasor transform thus allows the analysis (calculation) of the AC
steady_state of RLC_circuits by solving simple algebraic_equations (albeit with
complex coefficients) in the phasor domain instead of solving differential
equations (with real coefficients) in the time domain.[7][8] The originator of
the phasor transform was Charles_Proteus_Steinmetz working at General_Electric
in the late 19th century.[9][10]
Glossing over some mathematical details, the phasor transform can also be seen
as a particular case of the Laplace_transform, which additionally can be used
to (simultaneously) derive the transient_response of an RLC circuit.[8][10]
However, the Laplace transform is mathematically more difficult to apply and
the effort may be unjustified if only steady state analysis is required.[10]
Fig 2. When function      A &#x22C5;  e  i ( &#x03C9; t + &#x03B8; )
{\displaystyle \scriptstyle A\cdot e^{i(\omega t+\theta )}}  [\scriptstyle
A\cdot e^{i(\omega t+\theta )}] is depicted in the complex plane, the vector
formed by its imaginary and real parts rotates around the origin. Its magnitude
is A, and it completes one cycle every 2Ï/Ï seconds. Î¸ is the angle it forms
with the real axis at t = nâ¢2Ï/Ï, for integer values of n.
⁰
***** Contents *****
    * 1_Definition
    * 2_Phasor_arithmetic
          o 2.1_Multiplication_by_a_constant_(scalar)
          o 2.2_Differentiation_and_integration
          o 2.3_Addition
    * 3_Applications
          o 3.1_Circuit_laws
          o 3.2_Power_engineering
          o 3.3_Telecommunications:_analog_modulations
    * 4_See_also
    * 5_Footnotes
    * 6_References
    * 7_Further_reading
    * 8_External_links
***** Definition[edit] *****
Euler's_formula indicates that sinusoids can be represented mathematically as
the sum of two complex-valued functions:
         A &#x22C5; cos &#x2061; ( &#x03C9; t + &#x03B8; ) = A &#x22C5;     e
      i ( &#x03C9; t + &#x03B8; )   +  e  &#x2212; i ( &#x03C9; t + &#x03B8; )
      2   ,   {\displaystyle A\cdot \cos(\omega t+\theta )=A\cdot {\frac {e^{i
      (\omega t+\theta )}+e^{-i(\omega t+\theta )}}{2}},}  [A\cdot \cos(\omega
      t+\theta )=A\cdot {\frac {e^{i(\omega t+\theta )}+e^{-i(\omega t+\theta
      )}}{2}},]    [a]
or as the real_part of one of the functions:
             A &#x22C5; cos &#x2061; ( &#x03C9; t + &#x03B8; ) = Re &#x2061;
      { A &#x22C5;  e  i ( &#x03C9; t + &#x03B8; )   } = Re &#x2061; { A  e  i
      &#x03B8;   &#x22C5;  e  i &#x03C9; t   } .       {\displaystyle {\begin
      {aligned}A\cdot \cos(\omega t+\theta )=\operatorname {Re} \{A\cdot e^{i
      (\omega t+\theta )}\}=\operatorname {Re} \{Ae^{i\theta }\cdot e^{i\omega
      t}\}.\end{aligned}}}  [{\begin{aligned}A\cdot \cos(\omega t+\theta
      )=\operatorname {Re} \{A\cdot e^{i(\omega t+\theta )}\}=\operatorname
      {Re} \{Ae^{i\theta }\cdot e^{i\omega t}\}.\end{aligned}}]
The function     A &#x22C5;  e  i ( &#x03C9; t + &#x03B8; )     {\displaystyle
A\cdot e^{i(\omega t+\theta )}}  [A\cdot e^{i(\omega t+\theta )}] is called the
analytic_representation of     A &#x22C5; cos &#x2061; ( &#x03C9; t + &#x03B8;
)   {\displaystyle A\cdot \cos(\omega t+\theta )}  [{\displaystyle A\cdot \cos
(\omega t+\theta )}]. Figure 2 depicts it as a rotating vector in a complex
plane. It is sometimes convenient to refer to the entire function as a phasor,
[11] as we do in the next section. But the term phasor usually implies just the
static vector     A  e  i &#x03B8;     {\displaystyle Ae^{i\theta }}  [
{\displaystyle Ae^{i\theta }}]. An even more compact representation of a phasor
is the angle_notation:     A &#x2220; &#x03B8;   {\displaystyle A\angle \theta
}  [{\displaystyle A\angle \theta }]. See also vector_notation.
***** Phasor arithmetic[edit] *****
**** Multiplication by a constant (scalar)[edit] ****
Multiplication of the phasor      A  e  i &#x03B8;    e  i &#x03C9; t
{\displaystyle Ae^{i\theta }e^{i\omega t}\,}  [Ae^{i\theta }e^{i\omega t}\,] by
a complex constant,      B  e  i &#x03D5;      {\displaystyle Be^{i\phi }\,}
[Be^{i\phi }\,] , produces another phasor. That means its only effect is to
change the amplitude and phase of the underlying sinusoid:
             Re &#x2061; { ( A  e  i &#x03B8;   &#x22C5; B  e  i &#x03D5;   )
      &#x22C5;  e  i &#x03C9; t   }    = Re &#x2061; { ( A B  e  i ( &#x03B8; +
      &#x03D5; )   ) &#x22C5;  e  i &#x03C9; t   }       = A B cos &#x2061;
      ( &#x03C9; t + ( &#x03B8; + &#x03D5; ) )       {\displaystyle {\begin
      {aligned}\operatorname {Re} \{(Ae^{i\theta }\cdot Be^{i\phi })\cdot e^
      {i\omega t}\}&=\operatorname {Re} \{(ABe^{i(\theta +\phi )})\cdot e^
      {i\omega t}\}\\&=AB\cos(\omega t+(\theta +\phi ))\end{aligned}}}  [
      {\displaystyle {\begin{aligned}\operatorname {Re} \{(Ae^{i\theta }\cdot
      Be^{i\phi })\cdot e^{i\omega t}\}&=\operatorname {Re} \{(ABe^{i(\theta
      +\phi )})\cdot e^{i\omega t}\}\\&=AB\cos(\omega t+(\theta +\phi ))\end
      {aligned}}}]
In electronics,     B  e  i &#x03D5;      {\displaystyle Be^{i\phi }\,}  [Be^
{i\phi }\,]  would represent an impedance, which is independent of time. In
particular it is not the shorthand notation for another phasor. Multiplying a
phasor current by an impedance produces a phasor voltage. But the product of
two phasors (or squaring a phasor) would represent the product of two
sinusoids, which is a non-linear operation that produces new frequency
components. Phasor notation can only represent systems with one frequency, such
as a linear system stimulated by a sinusoid.
**** Differentiation and integration[edit] ****
The time derivative or integral of a phasor produces another phasor.[b] For
example:
             Re &#x2061;  {     d    d  t    ( A  e  i &#x03B8;   &#x22C5;  e
      i &#x03C9; t   )  }  = Re &#x2061; { A  e  i &#x03B8;   &#x22C5; i
      &#x03C9;  e  i &#x03C9; t   } = Re &#x2061; { A  e  i &#x03B8;   &#x22C5;
      e  i &#x03C0;  /  2   &#x03C9;  e  i &#x03C9; t   } = Re &#x2061;
      { &#x03C9; A  e  i ( &#x03B8; + &#x03C0;  /  2 )   &#x22C5;  e  i
      &#x03C9; t   } = &#x03C9; A &#x22C5; cos &#x2061; ( &#x03C9; t + &#x03B8;
      + &#x03C0;  /  2 )       {\displaystyle {\begin{aligned}\operatorname
      {Re} \left\{{\frac {\mathrm {d} }{\mathrm {d} t}}(Ae^{i\theta }\cdot e^
      {i\omega t})\right\}=\operatorname {Re} \{Ae^{i\theta }\cdot i\omega e^
      {i\omega t}\}=\operatorname {Re} \{Ae^{i\theta }\cdot e^{i\pi /2}\omega
      e^{i\omega t}\}=\operatorname {Re} \{\omega Ae^{i(\theta +\pi /2)}\cdot
      e^{i\omega t}\}=\omega A\cdot \cos(\omega t+\theta +\pi /2)\end
      {aligned}}}  [{\displaystyle {\begin{aligned}\operatorname {Re} \left\{
      {\frac {\mathrm {d} }{\mathrm {d} t}}(Ae^{i\theta }\cdot e^{i\omega
      t})\right\}=\operatorname {Re} \{Ae^{i\theta }\cdot i\omega e^{i\omega
      t}\}=\operatorname {Re} \{Ae^{i\theta }\cdot e^{i\pi /2}\omega e^{i\omega
      t}\}=\operatorname {Re} \{\omega Ae^{i(\theta +\pi /2)}\cdot e^{i\omega
      t}\}=\omega A\cdot \cos(\omega t+\theta +\pi /2)\end{aligned}}}]
Therefore, in phasor representation, the time derivative of a sinusoid becomes
just multiplication by the constant     i &#x03C9; = (  e  i &#x03C0;  /  2
&#x22C5; &#x03C9; )    {\displaystyle i\omega =(e^{i\pi /2}\cdot \omega )\,}  [
{\displaystyle i\omega =(e^{i\pi /2}\cdot \omega )\,}].
Similarly, integrating a phasor corresponds to multiplication by       1  i
&#x03C9;    =    e  &#x2212; i &#x03C0;  /  2   &#x03C9;      {\displaystyle
{\frac {1}{i\omega }}={\frac {e^{-i\pi /2}}{\omega }}\,}  [{\displaystyle
{\frac {1}{i\omega }}={\frac {e^{-i\pi /2}}{\omega }}\,}]. The time-dependent
factor,      e  i &#x03C9; t      {\displaystyle e^{i\omega t}\,}  [e^{{i\omega
t}}\,], is unaffected.
When we solve a linear_differential_equation with phasor arithmetic, we are
merely factoring      e  i &#x03C9; t      {\displaystyle e^{i\omega t}\,}  [e^
{{i\omega t}}\,] out of all terms of the equation, and reinserting it into the
answer. For example, consider the following differential equation for the
voltage across the capacitor in an RC_circuit:
             d  &#xA0;  v  C   ( t )    d  t    +   1  R C     v  C   ( t ) =
      1  R C     v  S   ( t )   {\displaystyle {\frac {\mathrm {d} \ v_{C}(t)}
      {\mathrm {d} t}}+{\frac {1}{RC}}v_{C}(t)={\frac {1}{RC}}v_{S}(t)}  [
      {\displaystyle {\frac {\mathrm {d} \ v_{C}(t)}{\mathrm {d} t}}+{\frac {1}
      {RC}}v_{C}(t)={\frac {1}{RC}}v_{S}(t)}]
When the voltage source in this circuit is sinusoidal:
          v  S   ( t ) =  V  P   &#x22C5; cos &#x2061; ( &#x03C9; t + &#x03B8;
      ) ,    {\displaystyle v_{S}(t)=V_{P}\cdot \cos(\omega t+\theta ),\,}  [v_
      {S}(t)=V_{P}\cdot \cos(\omega t+\theta ),\,]
we may substitute          v  S   ( t )    = Re &#x2061; {  V  s   &#x22C5;  e
i &#x03C9; t   }       {\displaystyle {\begin{aligned}v_{S}(t)&=\operatorname
{Re} \{V_{s}\cdot e^{i\omega t}\}\\\end{aligned}}}  [{\begin{aligned}v_{S}
(t)&=\operatorname {Re} \{V_{s}\cdot e^{i\omega t}\}\\\end{aligned}}]
          v  C   ( t ) = Re &#x2061; {  V  c   &#x22C5;  e  i &#x03C9; t   } ,
      {\displaystyle v_{C}(t)=\operatorname {Re} \{V_{c}\cdot e^{i\omega t}\},}
      [v_{C}(t)=\operatorname {Re} \{V_{c}\cdot e^{i\omega t}\},]
where phasor      V  s   =  V  P    e  i &#x03B8;      {\displaystyle V_{s}=V_
{P}e^{i\theta }\,}  [{\displaystyle V_{s}=V_{P}e^{i\theta }\,}], and phasor
V  c      {\displaystyle V_{c}\,}  [V_{c}\,] is the unknown quantity to be
determined.
In the phasor shorthand notation, the differential equation reduces to
         i &#x03C9;  V  c   +   1  R C     V  c   =   1  R C     V  s
      {\displaystyle i\omega V_{c}+{\frac {1}{RC}}V_{c}={\frac {1}{RC}}V_{s}}
      [i\omega V_{c}+{\frac {1}{RC}}V_{c}={\frac {1}{RC}}V_{s}] [c]
Solving for the phasor capacitor voltage gives
          V  c   =   1  1 + i &#x03C9; R C    &#x22C5; (  V  s   ) =    1
      &#x2212; i &#x03C9; R C   1 + ( &#x03C9; R C  )  2      &#x22C5; (  V  P
      e  i &#x03B8;   )    {\displaystyle V_{c}={\frac {1}{1+i\omega RC}}\cdot
      (V_{s})={\frac {1-i\omega RC}{1+(\omega RC)^{2}}}\cdot (V_{P}e^{i\theta
      })\,}  [V_{c}={\frac {1}{1+i\omega RC}}\cdot (V_{s})={\frac {1-i\omega
      RC}{1+(\omega RC)^{2}}}\cdot (V_{P}e^{i\theta })\,]
As we have seen, the factor multiplying      V  s      {\displaystyle V_{s}\,}
[V_{s}\,] represents differences of the amplitude and phase of      v  C   ( t
)    {\displaystyle v_{C}(t)\,}  [v_{C}(t)\,]  relative to      V  P
{\displaystyle V_{P}\,}  [V_{P}\,]  and     &#x03B8;    {\displaystyle \theta
\,}  [\theta \,].
In polar coordinate form, it is
           1  1 + ( &#x03C9; R C  )  2      &#x22C5;  e  &#x2212; i &#x03D5;
      ( &#x03C9; )   ,  &#xA0;where&#xA0;  &#x03D5; ( &#x03C9; ) = arctan
      &#x2061; ( &#x03C9; R C ) .    {\displaystyle {\frac {1}{\sqrt {1+(\omega
      RC)^{2}}}}\cdot e^{-i\phi (\omega )},{\text{ where }}\phi (\omega
      )=\arctan(\omega RC).\,}  [{\frac {1}{\sqrt {1+(\omega RC)^{2}}}}\cdot e^
      {-i\phi (\omega )},{\text{ where }}\phi (\omega )=\arctan(\omega RC).\,]
Therefore
          v  C   ( t ) =   1  1 + ( &#x03C9; R C  )  2      &#x22C5;  V  P
      cos &#x2061; ( &#x03C9; t + &#x03B8; &#x2212; &#x03D5; ( &#x03C9; ) )
      {\displaystyle v_{C}(t)={\frac {1}{\sqrt {1+(\omega RC)^{2}}}}\cdot V_
      {P}\cos(\omega t+\theta -\phi (\omega ))}  [v_{C}(t)={\frac {1}{\sqrt {1+
      (\omega RC)^{2}}}}\cdot V_{P}\cos(\omega t+\theta -\phi (\omega ))]
**** Addition[edit] ****
The sum of phasors as addition of rotating vectors
The sum of multiple phasors produces another phasor. That is because the sum of
sinusoids with the same frequency is also a sinusoid with that frequency:
              A  1   cos &#x2061; ( &#x03C9; t +  &#x03B8;  1   ) +  A  2   cos
      &#x2061; ( &#x03C9; t +  &#x03B8;  2   )    = Re &#x2061; {  A  1    e  i
      &#x03B8;  1      e  i &#x03C9; t   } + Re &#x2061; {  A  2    e  i
      &#x03B8;  2      e  i &#x03C9; t   }       = Re &#x2061; {  A  1    e  i
      &#x03B8;  1      e  i &#x03C9; t   +  A  2    e  i  &#x03B8;  2      e  i
      &#x03C9; t   }       = Re &#x2061; { (  A  1    e  i  &#x03B8;  1     +
      A  2    e  i  &#x03B8;  2     )  e  i &#x03C9; t   }       = Re &#x2061;
      { (  A  3    e  i  &#x03B8;  3     )  e  i &#x03C9; t   }       =  A  3
      cos &#x2061; ( &#x03C9; t +  &#x03B8;  3   ) ,       {\displaystyle
      {\begin{aligned}A_{1}\cos(\omega t+\theta _{1})+A_{2}\cos(\omega t+\theta
      _{2})&=\operatorname {Re} \{A_{1}e^{i\theta _{1}}e^{i\omega
      t}\}+\operatorname {Re} \{A_{2}e^{i\theta _{2}}e^{i\omega t}\}\\
      [8pt]&=\operatorname {Re} \{A_{1}e^{i\theta _{1}}e^{i\omega t}+A_{2}e^
      {i\theta _{2}}e^{i\omega t}\}\\[8pt]&=\operatorname {Re} \{(A_{1}e^
      {i\theta _{1}}+A_{2}e^{i\theta _{2}})e^{i\omega t}\}\\
      [8pt]&=\operatorname {Re} \{(A_{3}e^{i\theta _{3}})e^{i\omega t}\}\\
      [8pt]&=A_{3}\cos(\omega t+\theta _{3}),\end{aligned}}}  [{\begin
      {aligned}A_{1}\cos(\omega t+\theta _{1})+A_{2}\cos(\omega t+\theta _
      {2})&=\operatorname {Re} \{A_{1}e^{i\theta _{1}}e^{i\omega
      t}\}+\operatorname {Re} \{A_{2}e^{i\theta _{2}}e^{i\omega t}\}\\
      [8pt]&=\operatorname {Re} \{A_{1}e^{i\theta _{1}}e^{i\omega t}+A_{2}e^
      {i\theta _{2}}e^{i\omega t}\}\\[8pt]&=\operatorname {Re} \{(A_{1}e^
      {i\theta _{1}}+A_{2}e^{i\theta _{2}})e^{i\omega t}\}\\
      [8pt]&=\operatorname {Re} \{(A_{3}e^{i\theta _{3}})e^{i\omega t}\}\\
      [8pt]&=A_{3}\cos(\omega t+\theta _{3}),\end{aligned}}]
where
          A  3   2   = (  A  1   cos &#x2061;  &#x03B8;  1   +  A  2   cos
      &#x2061;  &#x03B8;  2    )  2   + (  A  1   sin &#x2061;  &#x03B8;  1   +
      A  2   sin &#x2061;  &#x03B8;  2    )  2   ,   {\displaystyle A_{3}^{2}=
      (A_{1}\cos \theta _{1}+A_{2}\cos \theta _{2})^{2}+(A_{1}\sin \theta _
      {1}+A_{2}\sin \theta _{2})^{2},}  [A_{3}^{2}=(A_{1}\cos \theta _{1}+A_
      {2}\cos \theta _{2})^{2}+(A_{1}\sin \theta _{1}+A_{2}\sin \theta _{2})^
      {2},]
      and, if we take      &#x03B8;  3   &#x2208; [ &#x2212;    &#x03C0; 2    ;
      3 &#x03C0;  2    [   {\displaystyle \theta _{3}\in [-{\tfrac {\pi }{2}};
      {\tfrac {3\pi }{2}}[}  [{\displaystyle \theta _{3}\in [-{\tfrac {\pi }
      {2}};{\tfrac {3\pi }{2}}[}], then :
          * if      A  1   cos &#x2061;  &#x03B8;  1   +  A  2   cos &#x2061;
            &#x03B8;  2   = 0   {\displaystyle A_{1}\cos \theta _{1}+A_{2}\cos
            \theta _{2}=0}  [{\displaystyle A_{1}\cos \theta _{1}+A_{2}\cos
            \theta _{2}=0}], then      &#x03B8;  3   = sgn &#x2061; (  A  1
            sin &#x2061; (  &#x03B8;  1   ) +  A  2   sin &#x2061; (  &#x03B8;
            2   ) ) &#x2217;   &#x03C0; 2     {\displaystyle \theta _
            {3}=\operatorname {sgn}(A_{1}\sin(\theta _{1})+A_{2}\sin(\theta _
            {2}))*{\frac {\pi }{2}}}  [{\displaystyle \theta _{3}=\operatorname
            {sgn}(A_{1}\sin(\theta _{1})+A_{2}\sin(\theta _{2}))*{\frac {\pi }
            {2}}}], with     sgn   {\displaystyle \operatorname {sgn} }
            [\operatorname {sgn} ] the sign_function;
          * if      A  1   cos &#x2061;  &#x03B8;  1   +  A  2   cos &#x2061;
            &#x03B8;  2   > 0   {\displaystyle A_{1}\cos \theta _{1}+A_{2}\cos
            \theta _{2}>0}  [{\displaystyle A_{1}\cos \theta _{1}+A_{2}\cos
            \theta _{2}>0}], then      &#x03B8;  3   = arctan &#x2061;  (     A
            1   sin &#x2061;  &#x03B8;  1   +  A  2   sin &#x2061;  &#x03B8;  2
            A  1   cos &#x2061;  &#x03B8;  1   +  A  2   cos &#x2061;  &#x03B8;
            2      )    {\displaystyle \theta _{3}=\arctan \left({\frac {A_
            {1}\sin \theta _{1}+A_{2}\sin \theta _{2}}{A_{1}\cos \theta _{1}+A_
            {2}\cos \theta _{2}}}\right)}  [\theta _{3}=\arctan \left({\frac
            {A_{1}\sin \theta _{1}+A_{2}\sin \theta _{2}}{A_{1}\cos \theta _
            {1}+A_{2}\cos \theta _{2}}}\right)];
          * if      A  1   cos &#x2061;  &#x03B8;  1   +  A  2   cos &#x2061;
            &#x03B8;  2   < 0   {\displaystyle A_{1}\cos \theta _{1}+A_{2}\cos
            \theta _{2}<0}  [{\displaystyle A_{1}\cos \theta _{1}+A_{2}\cos
            \theta _{2}<0}], then      &#x03B8;  3   = &#x03C0; + arctan
            &#x2061;  (     A  1   sin &#x2061;  &#x03B8;  1   +  A  2   sin
            &#x2061;  &#x03B8;  2      A  1   cos &#x2061;  &#x03B8;  1   +  A
            2   cos &#x2061;  &#x03B8;  2      )    {\displaystyle \theta _
            {3}=\pi +\arctan \left({\frac {A_{1}\sin \theta _{1}+A_{2}\sin
            \theta _{2}}{A_{1}\cos \theta _{1}+A_{2}\cos \theta _{2}}}\right)}
            [{\displaystyle \theta _{3}=\pi +\arctan \left({\frac {A_{1}\sin
            \theta _{1}+A_{2}\sin \theta _{2}}{A_{1}\cos \theta _{1}+A_{2}\cos
            \theta _{2}}}\right)}].
or, via the law_of_cosines on the complex_plane (or the trigonometric_identity
for_angle_differences):
          A  3   2   =  A  1   2   +  A  2   2   &#x2212; 2  A  1    A  2   cos
      &#x2061; (  180  &#x2218;   &#x2212; &#x0394; &#x03B8; ) =  A  1   2   +
      A  2   2   + 2  A  1    A  2   cos &#x2061; ( &#x0394; &#x03B8; ) ,
      {\displaystyle A_{3}^{2}=A_{1}^{2}+A_{2}^{2}-2A_{1}A_{2}\cos(180^{\circ
      }-\Delta \theta )=A_{1}^{2}+A_{2}^{2}+2A_{1}A_{2}\cos(\Delta \theta ),}
      [{\displaystyle A_{3}^{2}=A_{1}^{2}+A_{2}^{2}-2A_{1}A_{2}\cos(180^{\circ
      }-\Delta \theta )=A_{1}^{2}+A_{2}^{2}+2A_{1}A_{2}\cos(\Delta \theta ),}]
where     &#x0394; &#x03B8; =  &#x03B8;  1   &#x2212;  &#x03B8;  2
{\displaystyle \Delta \theta =\theta _{1}-\theta _{2}}  [\Delta \theta =\theta
_{1}-\theta _{2}].
A key point is that A3 and Î¸3 do not depend on Ï or t, which is what makes
phasor notation possible. The time and frequency dependence can be suppressed
and re-inserted into the outcome as long as the only operations used in between
are ones that produce another phasor. In angle_notation, the operation shown
above is written
          A  1   &#x2220;  &#x03B8;  1   +  A  2   &#x2220;  &#x03B8;  2   =  A
      3   &#x2220;  &#x03B8;  3   .    {\displaystyle A_{1}\angle \theta _
      {1}+A_{2}\angle \theta _{2}=A_{3}\angle \theta _{3}.\,}  [A_{1}\angle
      \theta _{1}+A_{2}\angle \theta _{2}=A_{3}\angle \theta _{3}.\,]
Another way to view addition is that two vectors with coordinates [ A1 cos(Ït
+ Î¸1), A1 sin(Ït + Î¸1) ] and [ A2 cos(Ït + Î¸2), A2 sin(Ït + Î¸2) ] are
added_vectorially to produce a resultant vector with coordinates [ A3 cos(Ït +
Î¸3), A3 sin(Ït + Î¸3) ]. (see animation)
Phasor diagram of three waves in perfect destructive interference
In physics, this sort of addition occurs when sinusoids interfere with each
other, constructively or destructively. The static vector concept provides
useful insight into questions like this: "What phase difference would be
required between three identical sinusoids for perfect cancellation?" In this
case, simply imagine taking three vectors of equal length and placing them head
to tail such that the last head matches up with the first tail. Clearly, the
shape which satisfies these conditions is an equilateral triangle, so the angle
between each phasor to the next is 120Â° (&#x200b;3Ï⁄2 radians), or one third
of a wavelength &#x200b;Î»⁄3. So the phase difference between each wave must
also be 120Â°, as is the case in three-phase_power
In other words, what this shows is that
         cos &#x2061; ( &#x03C9; t ) + cos &#x2061; ( &#x03C9; t + 2 &#x03C0;
      /  3 ) + cos &#x2061; ( &#x03C9; t &#x2212; 2 &#x03C0;  /  3 ) = 0.
      {\displaystyle \cos(\omega t)+\cos(\omega t+2\pi /3)+\cos(\omega t-2\pi /
      3)=0.\,}  [\cos(\omega t)+\cos(\omega t+2\pi /3)+\cos(\omega t-2\pi /
      3)=0.\,]
In the example of three waves, the phase difference between the first and the
last wave was 240 degrees, while for two waves destructive interference happens
at 180 degrees. In the limit of many waves, the phasors must form a circle for
destructive interference, so that the first phasor is nearly parallel with the
last. This means that for many sources, destructive interference happens when
the first and last wave differ by 360 degrees, a full wavelength     &#x03BB;
{\displaystyle \lambda }  [\lambda ]. This is why in single slit diffraction,
the minima occur when light from the far edge travels a full wavelength further
than the light from the near edge.
As the single vector rotates in an anti-clockwise direction, its tip at point A
will rotate one complete revolution of 360Â° or 2Ï radians representing one
complete cycle. If the length of its moving tip is transferred at different
angular intervals in time to a graph as shown above, a sinusoidal waveform
would be drawn starting at the left with zero time. Each position along the
horizontal axis indicates the time that has elapsed since zero time, t = 0.
When the vector is horizontal the tip of the vector represents the angles at
0Â°, 180Â°, and at 360Â°.
Likewise, when the tip of the vector is vertical it represents the positive
peak value, ( +Amax ) at 90Â° or &#x200b;Ï⁄2 and the negative peak value,
( −Amax ) at 270Â° or &#x200b;3Ï⁄2. Then the time axis of the waveform
represents the angle either in degrees or radians through which the phasor has
moved. So we can say that a phasor represent a scaled voltage or current value
of a rotating vector which is âfrozenâ at some point in time, ( t ) and in
our example above, this is at an angle of 30Â°.
Sometimes when we are analysing alternating waveforms we may need to know the
position of the phasor, representing the alternating quantity at some
particular instant in time especially when we want to compare two different
waveforms on the same axis. For example, voltage and current. We have assumed
in the waveform above that the waveform starts at time t = 0 with a
corresponding phase angle in either degrees or radians.
But if a second waveform starts to the left or to the right of this zero point,
or if we want to represent in phasor notation the relationship between the two
waveforms, then we will need to take into account this phase difference, Î¦ of
the waveform. Consider the diagram below from the previous Phase Difference
tutorial.
***** Applications[edit] *****
**** Circuit laws[edit] ****
With phasors, the techniques for solving DC circuits can be applied to solve AC
circuits. A list of the basic laws is given below.
    * Ohm's law for resistors: a resistor has no time delays and therefore
      doesn't change the phase of a signal therefore V=IR remains valid.
    * Ohm's law for resistors, inductors, and capacitors: V = IZ where Z is the
      complex impedance.
    * In an AC circuit we have real power (P) which is a representation of the
      average power into the circuit and reactive power (Q) which indicates
      power flowing back and forth. We can also define the complex_power
      S = P + jQ and the apparent power which is the magnitude of S. The power
      law for an AC circuit expressed in phasors is then S = VI* (where I* is
      the complex_conjugate of I, and the magnitudes of the voltage and current
      phasors V and I are the RMS values of the voltage and current,
      respectively).
    * Kirchhoff's_circuit_laws work with phasors in complex form
Given this we can apply the techniques of analysis_of_resistive_circuits with
phasors to analyze single frequency AC circuits containing resistors,
capacitors, and inductors. Multiple frequency linear AC circuits and AC
circuits with different waveforms can be analyzed to find voltages and currents
by transforming all waveforms to sine wave components with magnitude and phase
then analyzing each frequency separately, as allowed by the superposition
theorem.
**** Power engineering[edit] ****
In analysis of three_phase AC power systems, usually a set of phasors is
defined as the three complex cube roots of unity, graphically represented as
unit magnitudes at angles of 0, 120 and 240 degrees. By treating polyphase AC
circuit quantities as phasors, balanced circuits can be simplified and
unbalanced circuits can be treated as an algebraic combination of symmetrical
components. This approach greatly simplifies the work required in electrical
calculations of voltage drop, power flow, and short-circuit currents. In the
context of power systems analysis, the phase angle is often given in degrees,
and the magnitude in rms value rather than the peak amplitude of the sinusoid.
The technique of synchrophasors uses digital instruments to measure the phasors
representing transmission system voltages at widespread points in a
transmission network. Differences among the phasors indicate power flow and
system stability.
**** Telecommunications: analog modulations[edit] ****
The rotating frame picture using phasor can be a powerful tool to understand
analog modulations such as amplitude_modulation (and its variants [12] ) and
frequency_modulation.
   x ( t ) = &#x211C; e  {  A  e  j &#x03B8;   .  e  j 2 &#x03C0;  f  0   t
}    {\displaystyle x(t)=\Re e\left\{Ae^{j\theta }.e^{j2\pi f_{0}t}\right\}}  [
{\displaystyle x(t)=\Re e\left\{Ae^{j\theta }.e^{j2\pi f_{0}t}\right\}}], where
the term in brackets is viewed as a rotating vector in the complex plane.
The phasor has length     A   {\displaystyle A}  [A], rotates anti-clockwise at
a rate of      f  0     {\displaystyle f_{0}}  [f_{0}] revolutions per second,
and at time     t = 0   {\displaystyle t=0}  [t=0] makes an angle of
&#x03B8;   {\displaystyle \theta }  [\theta ] with respect to the positive real
axis.
The waveform     x ( t )   {\displaystyle x(t)}  [x(t)] can then be viewed as a
projection of this vector onto the real axis.
    * AM modulation: phasor diagram of a single tone of frequency      f  m
      {\displaystyle f_{m}}  [f_{m}]
    * FM modulation: phasor diagram of a single tone of frequency      f  m
      {\displaystyle f_{m}}  [f_{m}]
***** See also[edit] *****
    * In-phase_and_quadrature_components
    * Analytic_signal
          o Complex_envelope
    * Phase_factor, a phasor of unit magnitude
***** Footnotes[edit] *****
   1. ^
          o i is the Imaginary_unit (     i  2   = &#x2212; 1   {\displaystyle
            i^{2}=-1}  [i^{2}=-1]).
          o In electrical engineering texts, the imaginary unit is often
            symbolized by j.
          o The frequency of the wave, in Hz, is given by     &#x03C9;  /  2
            &#x03C0;   {\displaystyle \omega /2\pi }  [\omega /2\pi ].
   2. ^  This results from        d    d  t    (  e  i &#x03C9; t   ) = i
      &#x03C9;  e  i &#x03C9; t     {\displaystyle {\frac {\mathrm {d} }
      {\mathrm {d} t}}(e^{i\omega t})=i\omega e^{i\omega t}}  [{\displaystyle
      {\frac {\mathrm {d} }{\mathrm {d} t}}(e^{i\omega t})=i\omega e^{i\omega
      t}}], which means that the complex_exponential is the eigenfunction of
      the derivative operation.
   3. ^
        Proof
                   d  &#xA0; Re &#x2061; {  V  c   &#x22C5;  e  i
            &#x03C9; t   }    d  t    +   1  R C    Re &#x2061;
            {  V  c   &#x22C5;  e  i &#x03C9; t   } =   1  R C
            Re &#x2061; {  V  s   &#x22C5;  e  i &#x03C9; t   }
            {\displaystyle {\frac {\mathrm {d} \ \operatorname
            {Re} \{V_{c}\cdot e^{i\omega t}\}}{\mathrm {d} t}}+
            {\frac {1}{RC}}\operatorname {Re} \{V_{c}\cdot e^         (Eq.1)
            {i\omega t}\}={\frac {1}{RC}}\operatorname {Re} \{V_      
            {s}\cdot e^{i\omega t}\}}  [{\displaystyle {\frac
            {\mathrm {d} \ \operatorname {Re} \{V_{c}\cdot e^
            {i\omega t}\}}{\mathrm {d} t}}+{\frac {1}
            {RC}}\operatorname {Re} \{V_{c}\cdot e^{i\omega t}\}=
            {\frac {1}{RC}}\operatorname {Re} \{V_{s}\cdot e^
            {i\omega t}\}}]
      Since this must hold for all     t    {\displaystyle t\,}  [t\,],
      specifically:     t &#x2212;   &#x03C0;  2 &#x03C9;       {\displaystyle
      t-{\frac {\pi }{2\omega }}\,}  [{\displaystyle t-{\frac {\pi }{2\omega
      }}\,}], it follows that
                   d  &#xA0; Im &#x2061; {  V  c   &#x22C5;  e  i
            &#x03C9; t   }    d  t    +   1  R C    Im &#x2061;
            {  V  c   &#x22C5;  e  i &#x03C9; t   } =   1  R C
            Im &#x2061; {  V  s   &#x22C5;  e  i &#x03C9; t   }
            {\displaystyle {\frac {\mathrm {d} \ \operatorname
            {Im} \{V_{c}\cdot e^{i\omega t}\}}{\mathrm {d} t}}+
            {\frac {1}{RC}}\operatorname {Im} \{V_{c}\cdot e^         (Eq.2)
            {i\omega t}\}={\frac {1}{RC}}\operatorname {Im} \{V_      
            {s}\cdot e^{i\omega t}\}}  [{\displaystyle {\frac
            {\mathrm {d} \ \operatorname {Im} \{V_{c}\cdot e^
            {i\omega t}\}}{\mathrm {d} t}}+{\frac {1}
            {RC}}\operatorname {Im} \{V_{c}\cdot e^{i\omega t}\}=
            {\frac {1}{RC}}\operatorname {Im} \{V_{s}\cdot e^
            {i\omega t}\}}]
      It is also readily seen that
                   d  &#xA0; Re &#x2061; {  V  c   &#x22C5;  e  i &#x03C9; t
            }    d  t    = Re &#x2061;  {     d   (   V  c   &#x22C5;  e  i
            &#x03C9; t    )     d  t    }  = Re &#x2061;  {  i &#x03C9;  V  c
            &#x22C5;  e  i &#x03C9; t    }    {\displaystyle {\frac {\mathrm
            {d} \ \operatorname {Re} \{V_{c}\cdot e^{i\omega t}\}}{\mathrm {d}
            t}}=\operatorname {Re} \left\{{\frac {\mathrm {d} \left(V_{c}\cdot
            e^{i\omega t}\right)}{\mathrm {d} t}}\right\}=\operatorname {Re}
            \left\{i\omega V_{c}\cdot e^{i\omega t}\right\}}  [{\displaystyle
            {\frac {\mathrm {d} \ \operatorname {Re} \{V_{c}\cdot e^{i\omega
            t}\}}{\mathrm {d} t}}=\operatorname {Re} \left\{{\frac {\mathrm {d}
            \left(V_{c}\cdot e^{i\omega t}\right)}{\mathrm {d}
            t}}\right\}=\operatorname {Re} \left\{i\omega V_{c}\cdot e^{i\omega
            t}\right\}}]
                   d  &#xA0; Im &#x2061; {  V  c   &#x22C5;  e  i &#x03C9; t
            }    d  t    = Im &#x2061;  {     d   (   V  c   &#x22C5;  e  i
            &#x03C9; t    )     d  t    }  = Im &#x2061;  {  i &#x03C9;  V  c
            &#x22C5;  e  i &#x03C9; t    }    {\displaystyle {\frac {\mathrm
            {d} \ \operatorname {Im} \{V_{c}\cdot e^{i\omega t}\}}{\mathrm {d}
            t}}=\operatorname {Im} \left\{{\frac {\mathrm {d} \left(V_{c}\cdot
            e^{i\omega t}\right)}{\mathrm {d} t}}\right\}=\operatorname {Im}
            \left\{i\omega V_{c}\cdot e^{i\omega t}\right\}}  [{\displaystyle
            {\frac {\mathrm {d} \ \operatorname {Im} \{V_{c}\cdot e^{i\omega
            t}\}}{\mathrm {d} t}}=\operatorname {Im} \left\{{\frac {\mathrm {d}
            \left(V_{c}\cdot e^{i\omega t}\right)}{\mathrm {d}
            t}}\right\}=\operatorname {Im} \left\{i\omega V_{c}\cdot e^{i\omega
            t}\right\}}]

      Substituting these into  Eq.1 and  Eq.2, multiplying  Eq.2 by     i ,
      {\displaystyle i,\,}  [i,\,]  and adding both equations gives
               i &#x03C9;  V  c   &#x22C5;  e  i &#x03C9; t   +   1  R C     V
            c   &#x22C5;  e  i &#x03C9; t   =   1  R C     V  s   &#x22C5;  e
            i &#x03C9; t     {\displaystyle i\omega V_{c}\cdot e^{i\omega t}+
            {\frac {1}{RC}}V_{c}\cdot e^{i\omega t}={\frac {1}{RC}}V_{s}\cdot
            e^{i\omega t}}  [i\omega V_{c}\cdot e^{i\omega t}+{\frac {1}{RC}}V_
            {c}\cdot e^{i\omega t}={\frac {1}{RC}}V_{s}\cdot e^{i\omega t}]
                (  i &#x03C9;  V  c   +   1  R C     V  c    )  &#x22C5;  e  i
            &#x03C9; t   =  (    1  R C     V  s    )  &#x22C5;  e  i &#x03C9;
            t     {\displaystyle \left(i\omega V_{c}+{\frac {1}{RC}}V_
            {c}\right)\cdot e^{i\omega t}=\left({\frac {1}{RC}}V_
            {s}\right)\cdot e^{i\omega t}}  [\left(i\omega V_{c}+{\frac {1}
            {RC}}V_{c}\right)\cdot e^{i\omega t}=\left({\frac {1}{RC}}V_
            {s}\right)\cdot e^{i\omega t}]
               i &#x03C9;  V  c   +   1  R C     V  c   =   1  R C     V  s
            (  Q E D  )   {\displaystyle i\omega V_{c}+{\frac {1}{RC}}V_{c}=
            {\frac {1}{RC}}V_{s}\quad \quad (\mathrm {QED} )}  [i\omega V_{c}+
            {\frac {1}{RC}}V_{c}={\frac {1}{RC}}V_{s}\quad \quad (\mathrm {QED}
            )]
***** References[edit] *****
   1. ^Huw Fox; William Bolton (2002). Mathematics for Engineers and
      Technologists. Butterworth-Heinemann. p. 30. ISBN 978-0-08-051119-1.
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
   3. ^Clay Rawlins (2000). Basic AC Circuits (2nd ed.). Newnes. p. 124.
      ISBN 978-0-08-049398-5.
   4. ^ Bracewell, Ron. The Fourier Transform and Its Applications. McGraw-
      Hill, 1965. p269
   5. ^K. S. Suresh Kumar (2008). Electric Circuits and Networks. Pearson
      Education India. p. 272. ISBN 978-81-317-1390-7.
   6. ^Kequian Zhang; Dejie Li (2007). Electromagnetic Theory for Microwaves
      and Optoelectronics (2nd ed.). Springer Science & Business Media. p. 13.
      ISBN 978-3-540-74296-8.
   7. ^ a b cJ. Hindmarsh (1984). Electrical Machines & their Applications (4th
      ed.). Elsevier. p. 58. ISBN 978-1-4832-9492-6.
   8. ^William J. Eccles (2011). Pragmatic Electrical Engineering:
      Fundamentals. Morgan & Claypool Publishers. p. 51. ISBN 978-1-60845-668-
      0.
   9. ^ a bRichard C. Dorf; James A. Svoboda (2010). Introduction to Electric
      Circuits (8th ed.). John Wiley & Sons. p. 661. ISBN 978-0-470-52157-1.
  10. ^Allan H. Robbins; Wilhelm Miller (2012). Circuit Analysis: Theory and
      Practice (5th ed.). Cengage Learning. p. 536. ISBN 1-285-40192-1.
  11. ^ a b cWon Y. Yang; Seung C. Lee (2008). Circuit Systems with MATLAB and
      PSpice. John Wiley & Sons. pp. 256â261. ISBN 978-0-470-82240-1.
  12. ^Singh, Ravish R (2009). "Section 4.5: Phasor Representation of
      Alternating Quantities". Electrical Networks. Mcgraw Hill Higher
      Education. p. 4.13. ISBN 0070260966.
  13. ^ de Oliveira, H.M. and Nunes, F.D. About the Phasor Pathways in
      Analogical Amplitude Modulations. International Journal of Research in
      Engineering and Science (IJRES) Vol.2, N.1, Jan., pp.11-18, 2014. ISSN
      2320-9364
***** Further reading[edit] *****
    * Douglas C. Giancoli (1989). Physics for Scientists and Engineers.
      Prentice Hall. ISBN 0-13-666322-2.
Dorf, Richard C.; Tallarida, Ronald J. (1993-07-15). Pocket Book of Electrical
Engineering Formulas (1 ed.). Boca Raton,FL: CRC Press. pp. 152â155.
ISBN 0849344735.
***** External links[edit] *****
 Wikimedia Commons has media related to Phasors.
    * Phasor_Phactory
    * Visual_Representation_of_Phasors
    * Polar_and_Rectangular_Notation

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Phasor&oldid=880283825"
Categories:
    * Electrical_circuits
    * AC_power
    * Interference
    * Trigonometry
Hidden categories:
    * Commons_category_link_is_on_Wikidata
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * Simple_English
    * SlovenÄina
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * ä¸­æ
Edit_links
    * This page was last edited on 26 January 2019, at 15:17 (UTC).
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
