The following text has been accessed from https://en.wikipedia.org/wiki/Characteristic_impedance at Fri Aug 9 03:43:37 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Characteristic impedance ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about impedance in electrical circuits. For impedance of
electromagnetic waves, see Wave_impedance. For characteristic acoustic
impedance, see Acoustic_impedance.
A transmission_line drawn as two black wires. At a distance x into the line,
there is current phasor I(x) traveling through each wire, and there is a
voltage_difference phasor V(x) between the wires (bottom voltage minus top
voltage). If      Z  0     {\displaystyle Z_{0}}  [Z_{0}] is the characteristic
impedance of the line, then     V ( x )  /  I ( x ) =  Z  0     {\displaystyle
V(x)/I(x)=Z_{0}}  [V(x)/I(x)=Z_{0}] for a wave moving rightward, or     V ( x )
/  I ( x ) = &#x2212;  Z  0     {\displaystyle V(x)/I(x)=-Z_{0}}  [V(x)/I(x)=-
Z_{0}] for a wave moving leftward.
Schematic representation of a circuit where a source is coupled to a load with
a transmission_line having characteristic impedance      Z  0
{\displaystyle Z_{0}}  [Z_{0}].
The characteristic impedance or surge impedance (usually written Z0) of a
uniform transmission_line is the ratio of the amplitudes of voltage and current
of a single wave propagating along the line; that is, a wave travelling in one
direction in the absence of reflections in the other direction. Alternatively
and equivalently it can be defined as the input_impedance of a transmission
line when its length is infinite. Characteristic impedance is determined by the
geometry and materials of the transmission line and, for a uniform line, is not
dependent on its length. The SI unit of characteristic impedance is the ohm.
The characteristic impedance of a lossless transmission line is purely real,
with no reactive component. Energy supplied by a source at one end of such a
line is transmitted through the line without being dissipated in the line
itself. A transmission line of finite length (lossless or lossy) that is
terminated at one end with an impedance equal to the characteristic impedance
appears to the source like an infinitely long transmission line and produces no
reflections.
⁰
***** Contents *****
    * 1_Transmission_line_model
    * 2_Derivation
          o 2.1_Using_telegrapher's_equation
          o 2.2_Alternative_approach
    * 3_Lossless_line
    * 4_Surge_impedance_loading
    * 5_Practical_examples
          o 5.1_Coaxial_cable
    * 6_See_also
    * 7_References
    * 8_External_links
***** Transmission line model[edit] *****
Schematic representation of an elemental length of a transmission line.
The characteristic impedance     Z ( &#x03C9; )   {\displaystyle Z(\omega )}  [
{\displaystyle Z(\omega )}] of an infinite transmission line at a given angular
frequency     &#x03C9;   {\displaystyle \omega }  [\omega ] is the ratio of the
voltage and current of a pure sinusoidal wave of the same frequency travelling
along the line. This definition extends to DC by letting     &#x03C9;
{\displaystyle \omega }  [\omega ] tend to 0, and subsists for finite
transmission lines until the wave reaches the end of the line. In this case,
there will be in general a reflected wave which travels back along the line in
the opposite direction. When this wave reaches the source, it adds to the
transmitted wave and the ratio of the voltage and current at the input to the
line will no longer be the characteristic impedance. This new ratio is called
the input_impedance. The input impedance of an infinite line is equal to the
characteristic impedance since the transmitted wave is never reflected back
from the end. It can be shown that an equivalent definition is: the
characteristic impedance of a line is that impedance which, when terminating an
arbitrary length of line at its output, produces an input impedance of equal
value. This is so because there is no reflection on a line terminated in its
own characteristic impedance.
Applying the transmission line model based on the telegrapher's_equations as
derived below,[1][2] the general expression for the characteristic impedance of
a transmission line is:
          Z  0   =     R + j &#x03C9; L   G + j &#x03C9; C       {\displaystyle
      Z_{0}={\sqrt {\frac {R+j\omega L}{G+j\omega C}}}}  [Z_{0}={\sqrt {\frac
      {R+j\omega L}{G+j\omega C}}}]
where
         R   {\displaystyle R}  [R] is the resistance per unit length,
      considering the two conductors to be in_series,
         L   {\displaystyle L}  [L] is the inductance per unit length,
         G   {\displaystyle G}  [G] is the conductance of the dielectric per
      unit length,
         C   {\displaystyle C}  [C] is the capacitance per unit length,
         j   {\displaystyle j}  [j] is the imaginary_unit, and
         &#x03C9;   {\displaystyle \omega }  [\omega ] is the angular
      frequency.
Although an infinite line is assumed, since all quantities are per unit length,
the characteristic impedance is independent of the length of the transmission
line.
The voltage and current phasors on the line are related by the characteristic
impedance as:
            V  +    I  +     =  Z  0   = &#x2212;    V  &#x2212;    I  &#x2212;
      {\displaystyle {\frac {V^{+}}{I^{+}}}=Z_{0}=-{\frac {V^{-}}{I^{-}}}}  [
      {\frac {V^{+}}{I^{+}}}=Z_{0}=-{\frac {V^{-}}{I^{-}}}]
where the superscripts     +   {\displaystyle +}  [+] and     &#x2212;
{\displaystyle -}  [-] represent forward- and backward-traveling waves,
respectively. A surge of energy on a finite transmission line will see an
impedance of Z0 prior to any reflections arriving, hence surge impedance is an
alternative name for characteristic impedance.
***** Derivation[edit] *****
**** Using telegrapher's equation[edit] ****
Consider one section of the transmission line for the derivation of the
characteristic impedance. The voltage on the left would be V and on the right
side would be V+dV. This figure is to be used for both the derivation methods.
The differential equations describing the dependence of the voltage and current
on time and space are linear, so that a linear combination of solutions is
again a solution. This means that we can consider solutions with a time
dependence ejÏt, and the time dependence will factor out, leaving an ordinary
differential equation for the coefficients, which will be phasors depending on
space only. Moreover, the parameters can be generalized to be frequency-
dependent.[1]
Let
   V ( x , t ) = V ( x )  e  j &#x03C9; t     {\displaystyle V(x,t)=V(x)e^
{j\omega t}}  [{\displaystyle V(x,t)=V(x)e^{j\omega t}}] and
   I ( x , t ) = I ( x )  e  j &#x03C9; t     {\displaystyle I(x,t)=I(x)e^
{j\omega t}}  [{\displaystyle I(x,t)=I(x)e^{j\omega t}}]
The positive directions of V and I are in a loop of clockwise direction.
We find that
   d V = &#x2212; ( R + j &#x03C9; L ) I d x = &#x2212; Z I d x
{\displaystyle dV=-(R+j\omega L)Idx=-ZIdx}  [{\displaystyle dV=-(R+j\omega
L)Idx=-ZIdx}]
and
   d I = &#x2212; ( G + j &#x03C9; C ) V d x = &#x2212; Y V d x
{\displaystyle dI=-(G+j\omega C)Vdx=-YVdx}  [{\displaystyle dI=-(G+j\omega
C)Vdx=-YVdx}]
or
      d V   d x    = &#x2212; Z I   {\displaystyle {\frac {dV}{dx}}=-ZI}  [
{\displaystyle {\frac {dV}{dx}}=-ZI}]
and
      d I   d x    = &#x2212; Y V   {\displaystyle {\frac {dI}{dx}}=-YV}  [
{\displaystyle {\frac {dI}{dx}}=-YV}]
These first-order_equations are easily uncoupled by a second differentiation,
with the results:
       d  2   V   d  z  2      &#x2212; Z Y V = 0   {\displaystyle {\frac {d^
{2}V}{dz^{2}}}-ZYV=0}  [{\displaystyle {\frac {d^{2}V}{dz^{2}}}-ZYV=0}] and
d  2   I   d  z  2      &#x2212; Z Y I = 0   {\displaystyle {\frac {d^{2}I}{dz^
{2}}}-ZYI=0}  [{\displaystyle {\frac {d^{2}I}{dz^{2}}}-ZYI=0}]
Both V and I satisfy the same equation. Since ZY is independent of z and t, it
can be represented by a constant -k2. The minus sign is included so that k will
appear as Â±jkz in the exponential solutions of the equation. In fact,
   V =  V  +    e  &#x2212; &#x03B3; k z   +  V  &#x2212;    e  &#x03B3; k z
{\displaystyle V=V^{+}e^{-\gamma kz}+V^{-}e^{\gamma kz}}  [{\displaystyle V=V^
{+}e^{-\gamma kz}+V^{-}e^{\gamma kz}}]
where V+ and V- are the constant_of_integration, The above equation will be the
wave solution for V, and
   I = ( j k  /  Z ) (  V  &#x2212;    e  &#x2212; &#x03B3; k z   &#x2212;  V
+    e  &#x03B3; k z   )   {\displaystyle I=(jk/Z)(V^{-}e^{-\gamma kz}-V^{+}e^
{\gamma kz})}  [{\displaystyle I=(jk/Z)(V^{-}e^{-\gamma kz}-V^{+}e^{\gamma
kz})}]
from the first-order_equation.[1]
If lumped circuit analysis has to be valid at all frequencies, the length of
the sub section must tend to Zero.[2]
    lim  &#x0394; x &#x2192; 0      &#x0394; V   &#x0394; x    =    d V   d x
= &#x2212; ( R + j &#x03C9; L ) I   {\displaystyle \lim _{\Delta x\to 0}{\frac
{\Delta V}{\Delta x}}={\frac {dV}{dx}}=-(R+j\omega L)I}  [{\displaystyle \lim _
{\Delta x\to 0}{\frac {\Delta V}{\Delta x}}={\frac {dV}{dx}}=-(R+j\omega L)I}]
    lim  &#x0394; x &#x2192; 0      &#x0394; I   &#x0394; x    =    d I   d x
= &#x2212; ( G + j &#x03C9; C ) V   {\displaystyle \lim _{\Delta x\to 0}{\frac
{\Delta I}{\Delta x}}={\frac {dI}{dx}}=-(G+j\omega C)V}  [{\displaystyle \lim _
{\Delta x\to 0}{\frac {\Delta I}{\Delta x}}={\frac {dI}{dx}}=-(G+j\omega C)V}]
Substituting the value of V in the above equation, we get.
     d  d x      V  +    e  &#x2212; &#x03B3; x   +  V  &#x2212;    e  +
&#x03B3; x    = &#x2212; ( R + j &#x03C9; L )   I  +    e  &#x2212; &#x03B3; x
+  I  &#x2212;    e  + &#x03B3; x      {\displaystyle {\frac {d}{dx}}{V^{+}e^{-
\gamma x}+V^{-}e^{+\gamma x}}=-(R+j\omega L){I^{+}e^{-\gamma x}+I^{-}e^{+\gamma
x}}}  [{\displaystyle {\frac {d}{dx}}{V^{+}e^{-\gamma x}+V^{-}e^{+\gamma x}}=-
(R+j\omega L){I^{+}e^{-\gamma x}+I^{-}e^{+\gamma x}}}]
   &#x2212; &#x03B3;  V  +    e  &#x2212; &#x03B3; x   + &#x03B3;  V  &#x2212;
e  + &#x03B3; x   = &#x2212; ( R + j &#x03C9; L )   I  +    e  &#x2212;
&#x03B3; x   +  I  &#x2212;    e  + &#x03B3; x      {\displaystyle -\gamma V^
{+}e^{-\gamma x}+\gamma V^{-}e^{+\gamma x}=-(R+j\omega L){I^{+}e^{-\gamma x}+I^
{-}e^{+\gamma x}}}  [{\displaystyle -\gamma V^{+}e^{-\gamma x}+\gamma V^{-}e^
{+\gamma x}=-(R+j\omega L){I^{+}e^{-\gamma x}+I^{-}e^{+\gamma x}}}]
Co-efficient of      e  &#x2212; &#x03B3; x     {\displaystyle e^{-\gamma x}}
[{\displaystyle e^{-\gamma x}}] :     &#x2212; &#x03B3;  V  +   = &#x2212; ( R
+ j &#x03C9; L )  I  +     {\displaystyle -\gamma V^{+}=-(R+j\omega L)I^{+}}  [
{\displaystyle -\gamma V^{+}=-(R+j\omega L)I^{+}}]
Co-efficient of      e  &#x03B3; x     {\displaystyle e^{\gamma x}}  [
{\displaystyle e^{\gamma x}}] :     &#x03B3;  V  &#x2212;   = &#x2212; ( R + j
&#x03C9; L )  I  &#x2212;     {\displaystyle \gamma V^{-}=-(R+j\omega L)I^{-}}
[{\displaystyle \gamma V^{-}=-(R+j\omega L)I^{-}}]
Since     &#x03B3; =   ( R + j &#x03C9; L ) ( G + j &#x03C9; C )
{\displaystyle \gamma ={\sqrt {(R+j\omega L)(G+j\omega C)}}}  [{\displaystyle
\gamma ={\sqrt {(R+j\omega L)(G+j\omega C)}}}]
      V  +    I  +     =    R + j &#x03C9; L  &#x03B3;   =     R + j &#x03C9; L
G + j &#x03C9; C       {\displaystyle {\frac {V^{+}}{I^{+}}}={\frac {R+j\omega
L}{\gamma }}={\sqrt {\frac {R+j\omega L}{G+j\omega C}}}}  [{\displaystyle
{\frac {V^{+}}{I^{+}}}={\frac {R+j\omega L}{\gamma }}={\sqrt {\frac {R+j\omega
L}{G+j\omega C}}}}]
      V  &#x2212;    I  &#x2212;     = &#x2212;    R + j &#x03C9; L  &#x03B3;
=     R + j &#x03C9; L   G + j &#x03C9; C       {\displaystyle {\frac {V^{-}}
{I^{-}}}=-{\frac {R+j\omega L}{\gamma }}={\sqrt {\frac {R+j\omega L}{G+j\omega
C}}}}  [{\displaystyle {\frac {V^{-}}{I^{-}}}=-{\frac {R+j\omega L}{\gamma }}=
{\sqrt {\frac {R+j\omega L}{G+j\omega C}}}}]
It can be seen that, the above equations has the dimensions of Impedance (Ratio
of Voltage to Current) and is a function of primary constants of the line and
operating frequency. It is therefore called the âCharacteristic Impedanceâ
of the transmission line , often denoted by      Z  o     {\displaystyle Z_{o}}
[Z_{o}].[2]
    Z  o   =     R + j &#x03C9; L   G + j &#x03C9; C       {\displaystyle Z_
{o}={\sqrt {\frac {R+j\omega L}{G+j\omega C}}}}  [{\displaystyle Z_{o}={\sqrt
{\frac {R+j\omega L}{G+j\omega C}}}}]
**** Alternative approach[edit] ****
We follow an approach posted by Tim Healy.[3] The line is modeled by a series
of differential segments with differential series     ( R d x , L d x )
{\displaystyle (Rdx,Ldx)}  [{\displaystyle (Rdx,Ldx)}] and shunt     ( C d x ,
G d x )   {\displaystyle (Cdx,Gdx)}  [{\displaystyle (Cdx,Gdx)}] elements (as
shown in the figure above). The characteristic impedance is defined as the
ratio of the input voltage to the input current of a semi-infinite length of
line. We call this impedance      Z  o     {\displaystyle Z_{o}}  [Z_{o}]. That
is, the impedance looking into the line on the left is      Z  o
{\displaystyle Z_{o}}  [Z_{o}]. But, of course, if we go down the line one
differential length dx, the impedance into the line is still      Z  o
{\displaystyle Z_{o}}  [Z_{o}]. Hence we can say that the impedance looking
into the line on the far left is equal to      Z  o     {\displaystyle Z_{o}}
[Z_{o}] in parallel with     C d x   {\displaystyle Cdx}  [{\displaystyle Cdx}]
and     G d x   {\displaystyle Gdx}  [{\displaystyle Gdx}], all of which is in
series with     R d x   {\displaystyle Rdx}  [{\displaystyle Rdx}] and     L d
x   {\displaystyle Ldx}  [{\displaystyle Ldx}]. Hence:
    Z  o   = ( R + j &#x03C9; L ) d x +   1  ( G + j &#x03C9; C ) d x +   1  Z
o          {\displaystyle Z_{o}=(R+j\omega L)dx+{\frac {1}{(G+j\omega C)dx+
{\frac {1}{Z_{o}}}}}}  [{\displaystyle Z_{o}=(R+j\omega L)dx+{\frac {1}{
(G+j\omega C)dx+{\frac {1}{Z_{o}}}}}}]
    Z  o   = ( R + j &#x03C9; L ) d x +    Z  o     Z  o   ( G + j &#x03C9; C )
d x + 1      {\displaystyle Z_{o}=(R+j\omega L)dx+{\frac {Z_{o}}{Z_{o}
(G+j\omega C)dx+1}}}  [{\displaystyle Z_{o}=(R+j\omega L)dx+{\frac {Z_{o}}{Z_
{o}(G+j\omega C)dx+1}}}]
    Z  o   +  Z  o   2   ( G + j &#x03C9; C ) d x = ( R + j &#x03C9; L ) d x +
Z  o   ( G + j &#x03C9; C ) d x ( R + j &#x03C9; L ) d x +  Z  o
{\displaystyle Z_{o}+Z_{o}^{2}(G+j\omega C)dx=(R+j\omega L)dx+Z_{o}(G+j\omega
C)dx(R+j\omega L)dx+Z_{o}}  [{\displaystyle Z_{o}+Z_{o}^{2}(G+j\omega C)dx=
(R+j\omega L)dx+Z_{o}(G+j\omega C)dx(R+j\omega L)dx+Z_{o}}]
The term above containing two factors of     d x   {\displaystyle dx}  [dx] may
be discarded, since it is infinitesimal in comparison to the other terms,
leading to:
    Z  o   +  Z  o   2   ( G + j &#x03C9; C ) d x = ( R + j &#x03C9; L ) d x +
Z  o     {\displaystyle Z_{o}+Z_{o}^{2}(G+j\omega C)dx=(R+j\omega L)dx+Z_{o}}
[{\displaystyle Z_{o}+Z_{o}^{2}(G+j\omega C)dx=(R+j\omega L)dx+Z_{o}}]
and hence to
    Z  o   = &#x00B1;     R + j &#x03C9; L   G + j &#x03C9; C
{\displaystyle Z_{o}=\pm {\sqrt {\frac {R+j\omega L}{G+j\omega C}}}}  [
{\displaystyle Z_{o}=\pm {\sqrt {\frac {R+j\omega L}{G+j\omega C}}}}]
Reversing the sign of the square root may be regarded as changing the direction
of the current.
***** Lossless line[edit] *****
The analysis of lossless lines provides an accurate approximation for real
transmission lines that simplifies the mathematics considered in modeling
transmission lines. A lossless line is defined as a transmission line that has
no line resistance and no dielectric_loss. This would imply that the conductors
act like perfect conductors and the dielectric acts like a perfect dielectric.
For a lossless line, R and G are both zero, so the equation for characteristic
impedance derived above reduces to:
          Z  0   =    L C    .   {\displaystyle Z_{0}={\sqrt {\frac {L}{C}}}.}
      [{\displaystyle Z_{0}={\sqrt {\frac {L}{C}}}.}]
In particular,      Z  0     {\displaystyle Z_{0}}  [Z_{0}] does not depend any
more upon the frequency. The above expression is wholly real, since the
imaginary term j has canceled out, implying that Z0 is purely resistive. For a
lossless line terminated in Z0, there is no loss of current across the line,
and so the voltage remains the same along the line. The lossless line model is
a useful approximation for many practical cases, such as low-loss transmission
lines and transmission lines with high frequency. For both of these cases, R
and G are much smaller than ÏL and ÏC, respectively, and can thus be ignored.
The solutions to the long line transmission equations include incident and
reflected portions of the voltage and current:
   V =     V  r   +  I  r    Z  c    2    &#x03B5;  &#x03B3; x   +     V  r
&#x2212;  I  r    Z  c    2    &#x03B5;  &#x2212; &#x03B3; x     {\displaystyle
V={\frac {V_{r}+I_{r}Z_{c}}{2}}\varepsilon ^{\gamma x}+{\frac {V_{r}-I_{r}Z_
{c}}{2}}\varepsilon ^{-\gamma x}}
[{\displaystyle V={\frac {V_{r}+I_{r}Z_{c}}{2}}\varepsilon ^{\gamma x}+{\frac
{V_{r}-I_{r}Z_{c}}{2}}\varepsilon ^{-\gamma x}}]
   I =     V  r    /   Z  c   +  I  r    2    &#x03B5;  &#x03B3; x   &#x2212;
V  r    /   Z  c   &#x2212;  I  r    2    &#x03B5;  &#x2212; &#x03B3; x
{\displaystyle I={\frac {V_{r}/Z_{c}+I_{r}}{2}}\varepsilon ^{\gamma x}-{\frac
{V_{r}/Z_{c}-I_{r}}{2}}\varepsilon ^{-\gamma x}}
[{\displaystyle I={\frac {V_{r}/Z_{c}+I_{r}}{2}}\varepsilon ^{\gamma x}-{\frac
{V_{r}/Z_{c}-I_{r}}{2}}\varepsilon ^{-\gamma x}}]
When the line is terminated with its characteristic impedance, the reflected
portions of these equations are reduced to 0 and the solutions to the voltage
and current along the transmission line are wholly incident. Without a
reflection of the wave, the load that is being supplied by the line effectively
blends into the line making it appear to be an infinite line. In a lossless
line this implies that the voltage and current remain the same everywhere along
the transmission line. Their magnitudes remain constant along the length of the
line and are only rotated by a phase angle.
***** Surge impedance loading[edit] *****
In electric_power_transmission, the characteristic impedance of a transmission
line is expressed in terms of the surge impedance loading (SIL), or natural
loading, being the power loading at which reactive_power is neither produced
nor absorbed:
           S I L   =      V   L L      2    Z  0       {\displaystyle {\mathit
      {SIL}}={\frac {{V_{\mathrm {LL} }}^{2}}{Z_{0}}}}  [{\mathit {SIL}}={\frac
      {{V_{\mathrm {LL} }}^{2}}{Z_{0}}}]
in which      V   L L      {\displaystyle V_{\mathrm {LL} }}  [V_{\mathrm {LL}
}] is the line-to-line voltage in volts.
Loaded below its SIL, a line supplies reactive power to the system, tending to
raise system voltages. Above it, the line absorbs reactive power, tending to
depress the voltage. The Ferranti_effect describes the voltage gain towards the
remote end of a very lightly loaded (or open ended) transmission line.
Underground_cables normally have a very low characteristic impedance, resulting
in an SIL that is typically in excess of the thermal limit of the cable. Hence
a cable is almost always a source of reactive power.
***** Practical examples[edit] *****
Standard       Impedance (Î©Tolerance
Ethernet Cat.5 100            Â±5 Î©[4]
USB            90             Â±15%[5]
HDMI           95             Â±15%[6]
IEEE_1394      108            +3
                              â2%[7]
VGA            75             Â±5%[8]
DisplayPort    100            Â±20%[6]
DVI            95             Â±15%[6]
PCIe           85             Â±15%[6]
**** Coaxial cable[edit] ****
See also: Nominal_impedance_Â§ 50_Î©_and_75_Î©
The characteristic impedance of coaxial_cables (coax) is commonly chosen to be
50 Î© for RF and microwave applications. Coax for video applications is usually
75 Î© for its lower loss.
***** See also[edit] *****
    * AmpÃ¨re's_circuital_law
    * Characteristic_acoustic_impedance
    * Electrical_impedance
    * Maxwell's_equations
    * Transmission_line
    * Wave_impedance
    * Space_cloth
***** References[edit] *****
   1. ^ a b c"The_Telegrapher's_Equation". mysite.du.edu. Retrieved 2018-09-09.
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
   3. ^ a b c"Derivation_of_Characteristic_Impedance_of_Transmission_line".
      GATE ECE 2018. 2016-04-16. Retrieved 2018-09-09.
   4. ^"Characteristic_Impedance". www.ee.scu.edu. Retrieved 2018-09-09.
   5. ^"SuperCat_OUTDOOR_CAT_5e_U/UTP" (PDF). Archived from the_original (PDF)
      on 2012-03-16.
   6. ^"USB_in_a_NutShellâChapter_2âHardware". Beyond Logic.org. Retrieved
      2007-08-25.
   7. ^ a b c d https://www.nxp.com/documents/application_note/AN10798.pdf
      (PDF) modified 2011-07-04
   8. ^ http://materias.fi.uba.ar/6644/info/reflectometria/avanzado/ieee1394-
      evalwith-tdr.pdf (PDF), modified 2005-06-11
   9. ^ http://www.promusic.cz/soubory/File/Downloads/Data%20sheet/Klotz/
      Kabely%20pro%20video/VMM5FL__e.pdf (PDF) modified 2009-12-07
    * Guile, A. E. (1977). Electrical Power Systems. ISBN 0-08-021729-X.
Pozar, D. M. (February 2004). Microwave Engineering (3rd ed.). ISBN 0-471-
44878-8.
Ulaby, F. T. (2004). Fundamentals Of Applied Electromagnetics (media ed.).
Prentice Hall. ISBN 0-13-185089-X.
***** External links[edit] *****
 This article incorporates public_domain_material from the General_Services
Administration document "Federal_Standard_1037C".
    * IEEE:_Differential_Impedance..._finally_made_simple (2000)
    * v
    * t
    * e
Telecommunications
                     * Beacon
                     * Broadcasting
                     * Cable_protection_system
                     * Cable_TV
                     * Communications_satellite
                     * Computer_network
                     * Drums
                     * Electrical_telegraph
                     * Fax
                     * Heliographs
                     * Hydraulic_telegraph
                     * Internet
                     * Mass_media
                     * Mobile_phone
                     * Optical_telecommunication
                     * Optical_telegraphy
                     * Pager
                     * Photophone
History              * Prepaid_mobile_phone
                     * Radio
                     * Radiotelephone
                     * Satellite_communications
                     * Semaphore
                     * Smartphone
                     * Smoke_signals
                     * Telecommunications_history
                     * Telautograph
                     * Telegraphy
                     * Teleprinter (teletype)
                     * Telephone
                     * The_Telephone_Cases
                     * Television
                     * Undersea_telegraph_line
                     * Videoconferencing
                     * Videophone
                     * Videotelephony
                     * Whistled_language
                     * Edwin_Howard_Armstrong
                     * John_Logie_Baird
                     * Paul_Baran
                     * Alexander_Graham_Bell
                     * Tim_Berners-Lee
                     * Jagadish_Chandra_Bose
                     * Vint_Cerf
                     * Claude_Chappe
                     * Donald_Davies
                     * Lee_de_Forest
                     * Philo_Farnsworth
                     * Reginald_Fessenden
                     * Elisha_Gray
Pioneers             * Erna_Schneider_Hoover
                     * Charles_K._Kao
                     * Hedy_Lamarr                      [Telecom-icon.svg]
                     * Innocenzo_Manzetti
                     * Guglielmo_Marconi
                     * Antonio_Meucci
                     * Radia_Perlman
                     * Alexander_Stepanovich_Popov
                     * Johann_Philipp_Reis
                     * Henry_Sutton
                     * Nikola_Tesla
                     * Camille_Tissot
                     * Alfred_Vail
                     * Charles_Wheatstone
                     * Vladimir_K._Zworykin
                     * Coaxial_cable
                     * Fiber-optic_communication
Transmission               o Optical_fiber
media                * Free-space_optical_communication
                     * Molecular_communication
                     * Radio_waves
                     * Transmission_line
                     * Links
                     * Nodes
Network_topology     * Terminal_node
and switching        * Network_switching (circuit
                     * packet)
                     * Telephone_exchange
                     * Space-division
                     * Frequency-division
Multiplexing         * Time-division
                     * Polarization-division
                     * Orbital_angular-momentum
                     * Code-division
                     * ARPANET
                     * BITNET
                     * Cellular_network
                     * Computer
                     * CYCLADES
                     * Ethernet
                     * FidoNet
                     * Internet
                     * ISDN
                     * LAN
Networks             * Mobile
                     * NGN
                     * NPL_network
                     * Public_Switched_Telephone
                     * Radio
                     * Telecommunications_equipment
                     * Television
                     * Telex
                     * WAN
                     * Wireless_network
                     * World_Wide_Web
    * [Category] Category
    * [List-Class article] Outline
    * [Portal] Portal
    * [Commons page] Commons

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Characteristic_impedance&oldid=892600763"
Categories:
    * Electricity
    * Physical_quantities
    * Distributed_element_circuits
    * Transmission_lines
Hidden categories:
    * Wikipedia_articles_incorporating_text_from_the_Federal_Standard_1037C
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * PortuguÃªs
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 15 April 2019, at 16:57 (UTC).
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
