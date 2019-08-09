The following text has been accessed from https://en.wikipedia.org/wiki/Smith_chart at Fri Aug 9 03:43:49 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Smith chart ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The Smith chart, invented by Phillip_H._Smith (1905â1987),[1][2] is a
graphical aid or nomogram designed for electrical_and_electronics_engineers
specializing in radio_frequency (RF) engineering to assist in solving problems
with transmission_lines and matching circuits.[3] The Smith chart can be used
to simultaneously display multiple parameters including impedances,
admittances, reflection_coefficients,      S  n n      {\displaystyle S_{nn}\,}
[S_{{nn}}\,] scattering_parameters, noise_figure circles, constant gain
contours and regions for unconditional_stability, including mechanical
vibrations analysis.[4][5] The Smith chart is most frequently used at or within
the unity radius region. However, the remainder is still mathematically
relevant, being used, for example, in oscillator design and stability analysis.
[6]
While the use of paper Smith charts for solving the complex mathematics
involved in matching problems has been largely replaced by software based
methods, the Smith charts display is still the preferred method of displaying
how RF parameters behave at one or more frequencies, an alternative to using
tabular information. Thus most RF circuit analysis software includes a Smith
chart option for the display of results and all but the simplest impedance
measuring instruments can display measured results on a Smith chart display.
An impedance Smith chart (with no data plotted)
⁰
***** Contents *****
    * 1_Overview
    * 2_Mathematical_basis
          o 2.1_Actual_and_normalised_impedance_and_admittance
          o 2.2_The_normalised_impedance_Smith_chart
                # 2.2.1_The_variation_of_complex_reflection_coefficient_with
                  position_along_the_line
                # 2.2.2_The_variation_of_normalised_impedance_with_position
                  along_the_line
                # 2.2.3_Regions_of_the_Z_Smith_chart
                # 2.2.4_Circles_of_constant_normalised_resistance_and_constant
                  normalised_reactance
          o 2.3_The_Y_Smith_chart
          o 2.4_Practical_examples
          o 2.5_Working_with_both_the_Z_Smith_chart_and_the_Y_Smith_charts
          o 2.6_Choice_of_Smith_chart_type_and_component_type
    * 3_Using_the_Smith_chart_to_solve_conjugate_matching_problems_with
      distributed_components
    * 4_Using_the_Smith_chart_to_analyze_lumped_element_circuits
    * 5_3D_Smith_chart
    * 6_References
    * 7_Further_reading
    * 8_External_links
***** Overview[edit] *****
A network_analyzer (HP 8720A) showing a Smith chart.
The Smith chart is plotted on the complex reflection_coefficient plane in two
dimensions and is scaled in normalised impedance (the most common), normalised
admittance or both, using different colours to distinguish between them. These
are often known as the Z, Y and YZ Smith charts respectively.[7] Normalised
scaling allows the Smith chart to be used for problems involving any
characteristic or system impedance which is represented by the center point of
the chart. The most commonly used normalization impedance is 50 ohms. Once an
answer is obtained through the graphical constructions described below, it is
straightforward to convert between normalised impedance (or normalised
admittance) and the corresponding unnormalized value by multiplying by the
characteristic impedance (admittance). Reflection coefficients can be read
directly from the chart as they are unitless parameters.
The Smith chart has circumferential scaling in wavelengths and degrees. The
wavelengths scale is used in distributed_component problems and represents the
distance measured along the transmission line connected between the generator
or source and the load to the point under consideration. The degrees scale
represents the angle of the voltage reflection coefficient at that point. The
Smith chart may also be used for lumped_element matching and analysis problems.
Use of the Smith chart and the interpretation of the results obtained using it
requires a good understanding of AC_circuit_theory and transmission line
theory, both of which are pre-requisites for RF engineers.
As impedances and admittances change with frequency, problems using the Smith
chart can only be solved manually using one frequency at a time, the result
being represented by a point. This is often adequate for narrow_band
applications (typically up to about 5% to 10% bandwidth) but for wider
bandwidths it is usually necessary to apply Smith chart techniques at more than
one frequency across the operating frequency band. Provided the frequencies are
sufficiently close, the resulting Smith chart points may be joined by straight
lines to create a locus.
A locus of points on a Smith chart covering a range of frequencies can be used
to visually represent:
    * how capacitive or how inductive a load is across the frequency range
    * how difficult matching is likely to be at various frequencies
    * how well matched a particular component is.
The accuracy of the Smith chart is reduced for problems involving a large locus
of impedances or admittances, although the scaling can be magnified for
individual areas to accommodate these.
***** Mathematical basis[edit] *****
Most basic use of an impedance Smith chart. A wave travels down a transmission
line of characteristic_impedance Z0, terminated at a load with impedance ZL and
normalised impedance z=ZL/Z0. There is a signal_reflection with coefficient Î.
Each point on the Smith chart simultaneously represents both a value of z
(bottom left), and the corresponding value of Î (bottom right), related by z=
(1 + Î)/(1 − Î).
**** Actual and normalised impedance and admittance[edit] ****
A transmission line with a characteristic impedance of      Z  0
{\displaystyle Z_{0}\,}  [Z_{0}\,] may be universally considered to have a
characteristic_admittance of      Y  0      {\displaystyle Y_{0}\,}  [Y_{0}\,]
where
          Y  0   =   1  Z  0        {\displaystyle Y_{0}={\frac {1}{Z_{0}}}\,}
      [Y_{0}={\frac  {1}{Z_{0}}}\,]
Any impedance,      Z  T      {\displaystyle Z_{\text{T}}\,}  [{\displaystyle
Z_{\text{T}}\,}] expressed in ohms, may be normalised by dividing it by the
characteristic impedance, so the normalised impedance using the lower case zT
is given by
          z  T   =    Z  T    Z  0        {\displaystyle z_{\text{T}}={\frac
      {Z_{\text{T}}}{Z_{0}}}\,}  [{\displaystyle z_{\text{T}}={\frac {Z_{\text
      {T}}}{Z_{0}}}\,}]
Similarly, for normalised admittance
          y  T   =    Y  T    Y  0        {\displaystyle y_{\text{T}}={\frac
      {Y_{\text{T}}}{Y_{0}}}\,}  [{\displaystyle y_{\text{T}}={\frac {Y_{\text
      {T}}}{Y_{0}}}\,}]
The SI_unit of impedance is the ohm with the symbol of the upper case Greek
letter omega (Î©) and the SI_unit for admittance is the siemens with the symbol
of an upper case letter S. Normalised impedance and normalised admittance are
dimensionless. Actual impedances and admittances must be normalised before
using them on a Smith chart. Once the result is obtained it may be de-
normalised to obtain the actual result.
**** The normalised impedance Smith chart[edit] ****
Transmission lines terminated by an open circuit (top) and a short circuit
(bottom). A pulse reflects perfectly off both these terminations, but the sign
of the reflected voltage is opposite in the two cases. Black dots represent
electrons, and arrows show the electric field.
Using transmission line theory, if a transmission line is terminated in an
impedance (     Z  T      {\displaystyle Z_{\text{T}}\,}  [{\displaystyle Z_
{\text{T}}\,}]) which differs from its characteristic impedance (     Z  0
{\displaystyle Z_{0}\,}  [Z_{0}\,]), a standing_wave will be formed on the line
comprising the resultant of both the incident or forward (     V  F
{\displaystyle V_{\text{F}}\,}  [{\displaystyle V_{\text{F}}\,}]) and the
reflected or reversed (     V  R      {\displaystyle V_{\text{R}}\,}  [
{\displaystyle V_{\text{R}}\,}]) waves. Using complex exponential notation:
          V  F   = A exp &#x2061; ( j &#x03C9; t ) exp &#x2061; ( + &#x03B3;
      &#x2113; ) &#xA0;    {\displaystyle V_{\text{F}}=A\exp(j\omega t)\exp
      (+\gamma \ell )~\,}  [{\displaystyle V_{\text{F}}=A\exp(j\omega t)\exp
      (+\gamma \ell )~\,}] and
          V  R   = B exp &#x2061; ( j &#x03C9; t ) exp &#x2061; ( &#x2212;
      &#x03B3; &#x2113; )    {\displaystyle V_{\text{R}}=B\exp(j\omega t)\exp(-
      \gamma \ell )\,}  [{\displaystyle V_{\text{R}}=B\exp(j\omega t)\exp(-
      \gamma \ell )\,}]
where
         exp &#x2061; ( j &#x03C9; t )    {\displaystyle \exp(j\omega t)\,}
      [\exp(j\omega t)\,] is the temporal part of the wave
         exp &#x2061; ( &#x00B1; &#x03B3; &#x2113; )    {\displaystyle \exp(\pm
      \gamma \ell )\,}  [{\displaystyle \exp(\pm \gamma \ell )\,}] is the
      spatial part of the wave and
         &#x03C9; = 2 &#x03C0; f    {\displaystyle \omega =2\pi f\,}  [\omega
      =2\pi f\,] where
         &#x03C9;    {\displaystyle \omega \,}  [\omega\,] is the angular
      frequency in radians per second (rad/s)
         f    {\displaystyle f\,}  [f\,] is the frequency in hertz (Hz)
         t    {\displaystyle t\,}  [t\,] is the time in seconds (s)
         A    {\displaystyle A\,}  [A\,] and     B    {\displaystyle B\,}
      [B\,] are constants
         &#x2113;    {\displaystyle \ell \,}  [\ell \,] is the distance
      measured along the transmission line from the load toward the generator
      in metres (m)
Also
         &#x03B3; = &#x03B1; + j &#x03B2;    {\displaystyle \gamma =\alpha
      +j\beta \,}  [{\displaystyle \gamma =\alpha +j\beta \,}] is the
      propagation_constant which has units 1/m
where
         &#x03B1;    {\displaystyle \alpha \,}  [\alpha \,] is the attenuation
      constant in nepers per metre (Np/m)
         &#x03B2;    {\displaystyle \beta \,}  [\beta \,] is the phase_constant
      in radians per metre (rad/m)
The Smith chart is used with one frequency (    &#x03C9;   {\displaystyle
\omega }  [\omega ]) at a time, and only for one moment (    t   {\displaystyle
t}  [t]) at a time, so the temporal part of the phase (    exp &#x2061; ( j
&#x03C9; t )    {\displaystyle \exp(j\omega t)\,}  [\exp(j\omega t)\,]) is
fixed. All terms are actually multiplied by this to obtain the instantaneous
phase, but it is conventional and understood to omit it. Therefore,
          V  F   = A exp &#x2061; ( + &#x03B3; &#x2113; )    {\displaystyle V_
      {\text{F}}=A\exp(+\gamma \ell )\,}  [{\displaystyle V_{\text{F}}=A\exp
      (+\gamma \ell )\,}] and
          V  R   = B exp &#x2061; ( &#x2212; &#x03B3; &#x2113; )
      {\displaystyle V_{\text{R}}=B\exp(-\gamma \ell )\,}  [{\displaystyle V_
      {\text{R}}=B\exp(-\gamma \ell )\,}]
where     A    {\displaystyle A\,}  [A\,] and     B    {\displaystyle B\,}
[B\,] are respectively the forward and reverse voltage amplitudes at the load.
*** The variation of complex reflection coefficient with position along the
line[edit] ***
Looking towards a load through a length     &#x2113;    {\displaystyle \ell \,}
[\ell \,] of lossless transmission line, the impedance changes as     &#x2113;
{\displaystyle \ell \,}  [\ell \,] increases, following the blue circle. (This
impedance is characterized by its reflection coefficient      V  reflected    /
V  incident     {\displaystyle V_{\text{reflected}}/V_{\text{incident}}}  [
{\displaystyle V_{\text{reflected}}/V_{\text{incident}}}].) The blue circle,
centered within the impedance Smith chart, is sometimes called an SWR circle
(short for constant standing_wave_ratio).
The complex voltage reflection coefficient     &#x0393;    {\displaystyle
\Gamma \,}  [\Gamma \,] is defined as the ratio of the reflected wave to the
incident (or forward) wave. Therefore,
         &#x0393; =    V  R    V  F     =    B exp &#x2061; ( &#x2212; &#x03B3;
      &#x2113; )   A exp &#x2061; ( + &#x03B3; &#x2113; )    = C exp &#x2061;
      ( &#x2212; 2 &#x03B3; &#x2113; )    {\displaystyle \Gamma ={\frac {V_
      {\text{R}}}{V_{\text{F}}}}={\frac {B\exp(-\gamma \ell )}{A\exp(+\gamma
      \ell )}}=C\exp(-2\gamma \ell )\,}  [{\displaystyle \Gamma ={\frac {V_
      {\text{R}}}{V_{\text{F}}}}={\frac {B\exp(-\gamma \ell )}{A\exp(+\gamma
      \ell )}}=C\exp(-2\gamma \ell )\,}]
where C is also a constant.
For a uniform transmission line (in which     &#x03B3;    {\displaystyle \gamma
\,}  [\gamma \,] is constant), the complex reflection coefficient of a standing
wave varies according to the position on the line. If the line is lossy
(    &#x03B1;    {\displaystyle \alpha \,}  [\alpha \,] is non-zero) this is
represented on the Smith chart by a spiral path. In most Smith chart problems
however, losses can be assumed negligible (    &#x03B1; = 0    {\displaystyle
\alpha =0\,}  [\alpha =0\,]) and the task of solving them is greatly
simplified. For the loss free case therefore, the expression for complex
reflection coefficient becomes
         &#x0393; =  &#x0393;  L   exp &#x2061; ( &#x2212; 2 j &#x03B2;
      &#x2113; )    {\displaystyle \Gamma =\Gamma _{\text{L}}\exp(-2j\beta \ell
      )\,}  [{\displaystyle \Gamma =\Gamma _{\text{L}}\exp(-2j\beta \ell )\,}]
where      &#x0393;  L      {\displaystyle \Gamma _{\text{L}}\,}  [
{\displaystyle \Gamma _{\text{L}}\,}] is the reflection coefficient at the
load, and     &#x2113;    {\displaystyle \ell \,}  [\ell \,] is the line length
from the load to the location where the reflection coefficient is measured. The
phase constant     &#x03B2;    {\displaystyle \beta \,}  [\beta \,] may also be
written as
         &#x03B2; =    2 &#x03C0;  &#x03BB;      {\displaystyle \beta ={\frac
      {2\pi }{\lambda }}\,}  [{\displaystyle \beta ={\frac {2\pi }{\lambda
      }}\,}]
where     &#x03BB;    {\displaystyle \lambda \,}  [\lambda \,] is the
wavelength within the transmission line at the test frequency.
Therefore,
         &#x0393; =  &#x0393;  L   exp &#x2061;  (     &#x2212; 4 j &#x03C0;
      &#x03BB;   &#x2113;  )     {\displaystyle \Gamma =\Gamma _{\text{L}}\exp
      \left({\frac {-4j\pi }{\lambda }}\ell \right)\,}  [{\displaystyle \Gamma
      =\Gamma _{\text{L}}\exp \left({\frac {-4j\pi }{\lambda }}\ell \right)\,}]
This equation shows that, for a standing wave, the complex reflection
coefficient and impedance repeats every half wavelength along the transmission
line. The complex reflection coefficient is generally simply referred to as
reflection coefficient. The outer circumferential scale of the Smith chart
represents the distance from the generator to the load scaled in wavelengths
and is therefore scaled from zero to 0.50 .
*** The variation of normalised impedance with position along the line[edit]
***
If     V    {\displaystyle V\,}  [V\,] and     I    {\displaystyle I\,}  [I\,]
are the voltage across and the current entering the termination at the end of
the transmission line respectively, then
          V  F   +  V  R   = V    {\displaystyle V_{\text{F}}+V_{\text{R}}=V\,}
      [{\displaystyle V_{\text{F}}+V_{\text{R}}=V\,}] and
          V  F   &#x2212;  V  R   =  Z  0   I    {\displaystyle V_{\text{F}}-V_
      {\text{R}}=Z_{0}I\,}  [{\displaystyle V_{\text{F}}-V_{\text{R}}=Z_
      {0}I\,}].
By dividing these equations and substituting for both the voltage reflection
coefficient
         &#x0393; =    V  R    V  F        {\displaystyle \Gamma ={\frac {V_
      {\text{R}}}{V_{\text{F}}}}\,}  [{\displaystyle \Gamma ={\frac {V_{\text
      {R}}}{V_{\text{F}}}}\,}]
and the normalised impedance of the termination represented by the lower case
z, subscript T
          z  T   =   V   Z  0   I       {\displaystyle z_{\text{T}}={\frac {V}
      {Z_{0}I}}\,}  [{\displaystyle z_{\text{T}}={\frac {V}{Z_{0}I}}\,}]
gives the result:
          z  T   =    1 + &#x0393;   1 &#x2212; &#x0393;       {\displaystyle
      z_{\text{T}}={\frac {1+\Gamma }{1-\Gamma }}\,}  [{\displaystyle z_{\text
      {T}}={\frac {1+\Gamma }{1-\Gamma }}\,}].
Alternatively, in terms of the reflection coefficient
         &#x0393; =     z  T   &#x2212; 1    z  T   + 1       {\displaystyle
      \Gamma ={\frac {z_{\text{T}}-1}{z_{\text{T}}+1}}\,}  [{\displaystyle
      \Gamma ={\frac {z_{\text{T}}-1}{z_{\text{T}}+1}}\,}]
These are the equations which are used to construct the Z Smith chart.
Mathematically speaking     &#x0393;    {\displaystyle \Gamma \,}  [\Gamma \,]
and      z  T      {\displaystyle z_{\text{T}}\,}  [{\displaystyle z_{\text
{T}}\,}] are related via a MÃ¶bius_transformation.
Both     &#x0393;    {\displaystyle \Gamma \,}  [\Gamma \,] and      z  T
{\displaystyle z_{\text{T}}\,}  [{\displaystyle z_{\text{T}}\,}] are expressed
in complex_numbers without any units. They both change with frequency so for
any particular measurement, the frequency at which it was performed must be
stated together with the characteristic impedance.
   &#x0393;    {\displaystyle \Gamma \,}  [\Gamma \,] may be expressed in
magnitude and angle on a polar_diagram. Any actual reflection coefficient must
have a magnitude of less than or equal to unity so, at the test frequency, this
may be expressed by a point inside a circle of unity radius. The Smith chart is
actually constructed on such a polar diagram. The Smith chart scaling is
designed in such a way that reflection coefficient can be converted to
normalised impedance or vice versa. Using the Smith chart, the normalised
impedance may be obtained with appreciable accuracy by plotting the point
representing the reflection coefficient treating the Smith chart as a polar
diagram and then reading its value directly using the characteristic Smith
chart scaling. This technique is a graphical alternative to substituting the
values in the equations.
By substituting the expression for how reflection coefficient changes along an
unmatched loss free transmission line
         &#x0393; =    B exp &#x2061; ( &#x2212; &#x03B3; &#x2113; )   A exp
      &#x2061; ( &#x03B3; &#x2113; )    =    B exp &#x2061; ( &#x2212; j
      &#x03B2; &#x2113; )   A exp &#x2061; ( j &#x03B2; &#x2113; )
      {\displaystyle \Gamma ={\frac {B\exp(-\gamma \ell )}{A\exp(\gamma \ell
      )}}={\frac {B\exp(-j\beta \ell )}{A\exp(j\beta \ell )}}\,}  [
      {\displaystyle \Gamma ={\frac {B\exp(-\gamma \ell )}{A\exp(\gamma \ell
      )}}={\frac {B\exp(-j\beta \ell )}{A\exp(j\beta \ell )}}\,}]
for the loss free case, into the equation for normalised impedance in terms of
reflection coefficient
          z  T   =    1 + &#x0393;   1 &#x2212; &#x0393;       {\displaystyle
      z_{\text{T}}={\frac {1+\Gamma }{1-\Gamma }}\,}  [{\displaystyle z_{\text
      {T}}={\frac {1+\Gamma }{1-\Gamma }}\,}].
and using Euler's_formula
         exp &#x2061; ( j &#x03B8; ) = cos &#x2061; &#x03B8; + j sin &#x2061;
      &#x03B8;    {\displaystyle \exp(j\theta )=\cos \theta +j\sin \theta \,}
      [\exp(j\theta )=\cos \theta +j\sin \theta \,]
yields the impedance version transmission line equation for the loss free case:
[8]
          Z  in   =  Z  0       Z  L   + j  Z  0   tan &#x2061; ( &#x03B2;
      &#x2113; )    Z  0   + j  Z  L   tan &#x2061; ( &#x03B2; &#x2113; )
      {\displaystyle Z_{\text{in}}=Z_{0}{\frac {Z_{\text{L}}+jZ_{0}\tan(\beta
      \ell )}{Z_{0}+jZ_{\text{L}}\tan(\beta \ell )}}\,}  [{\displaystyle Z_
      {\text{in}}=Z_{0}{\frac {Z_{\text{L}}+jZ_{0}\tan(\beta \ell )}{Z_{0}+jZ_
      {\text{L}}\tan(\beta \ell )}}\,}]
where      Z  in      {\displaystyle Z_{\text{in}}\,}  [{\displaystyle Z_{\text
{in}}\,}] is the impedance 'seen' at the input of a loss free transmission line
of length     &#x2113;   {\displaystyle \ell }  [\ell ], terminated with an
impedance      Z  L      {\displaystyle Z_{\text{L}}\,}  [{\displaystyle Z_
{\text{L}}\,}]
Versions of the transmission line equation may be similarly derived for the
admittance loss free case and for the impedance and admittance lossy cases.
The Smith chart graphical equivalent of using the transmission line equation is
to normalise      Z  L      {\displaystyle Z_{\text{L}}\,}  [{\displaystyle Z_
{\text{L}}\,}], to plot the resulting point on a Z Smith chart and to draw a
circle through that point centred at the Smith chart centre. The path along the
arc of the circle represents how the impedance changes whilst moving along the
transmission line. In this case the circumferential (wavelength) scaling must
be used, remembering that this is the wavelength within the transmission line
and may differ from the free space wavelength.
*** Regions of the Z Smith chart[edit] ***
If a polar diagram is mapped on to a cartesian_coordinate_system it is
conventional to measure angles relative to the positive x-axis using a
counterclockwise direction for positive angles. The magnitude of a complex
number is the length of a straight line drawn from the origin to the point
representing it. The Smith chart uses the same convention, noting that, in the
normalised impedance plane, the positive x-axis extends from the center of the
Smith chart at      z  T   = 1 &#x00B1; j 0    {\displaystyle z_{\text{T}}=1\pm
j0\,}  [{\displaystyle z_{\text{T}}=1\pm j0\,}] to the point      z  T   =
&#x221E; &#x00B1; j &#x221E;    {\displaystyle z_{\text{T}}=\infty \pm j\infty
\,}  [{\displaystyle z_{\text{T}}=\infty \pm j\infty \,}]. The region above the
x-axis represents inductive impedances (positive imaginary parts) and the
region below the x-axis represents capacitive impedances (negative imaginary
parts).
If the termination is perfectly matched, the reflection coefficient will be
zero, represented effectively by a circle of zero radius or in fact a point at
the centre of the Smith chart. If the termination was a perfect open circuit or
short_circuit the magnitude of the reflection coefficient would be unity, all
power would be reflected and the point would lie at some point on the unity
circumference circle.
*** Circles of constant normalised resistance and constant normalised reactance
[edit] ***
The normalised impedance Smith chart is composed of two families of circles:
circles of constant normalised resistance and circles of constant normalised
reactance. In the complex reflection coefficient plane the Smith chart occupies
a circle of unity radius centred at the origin. In cartesian coordinates
therefore the circle would pass through the points (+1,0) and (−1,0) on the x-
axis and the points (0,+1) and (0,−1) on the y-axis.
Since both     &#x0393;   {\displaystyle \Gamma }  [\Gamma ] and     z
{\displaystyle z\,}  [z\,] are complex numbers, in general they may be written
as:
         z = a + j b    {\displaystyle z=a+jb\,}  [{\displaystyle z=a+jb\,}]
         &#x0393; = c + j d    {\displaystyle \Gamma =c+jd\,}  [{\displaystyle
      \Gamma =c+jd\,}]
with a, b, c and d real numbers.
Substituting these into the equation relating normalised impedance and complex
reflection coefficient:
         &#x0393; =    z &#x2212; 1   z + 1       {\displaystyle \Gamma ={\frac
      {z-1}{z+1}}\,}  [{\displaystyle \Gamma ={\frac {z-1}{z+1}}\,}]
gives the following result:
         &#x0393; = c + j d =  [     a  2   +  b  2   &#x2212; 1   ( a + 1  )
      2   +  b  2      ]  + j  [    2 b   ( a + 1  )  2   +  b  2      ]
      {\displaystyle \Gamma =c+jd=\left[{\frac {a^{2}+b^{2}-1}{(a+1)^{2}+b^
      {2}}}\right]+j\left[{\frac {2b}{(a+1)^{2}+b^{2}}}\right]\,}  [
      {\displaystyle \Gamma =c+jd=\left[{\frac {a^{2}+b^{2}-1}{(a+1)^{2}+b^
      {2}}}\right]+j\left[{\frac {2b}{(a+1)^{2}+b^{2}}}\right]\,}].
This is the equation which describes how the complex reflection coefficient
changes with the normalised impedance and may be used to construct both
families of circles.[9]
**** The Y Smith chart[edit] ****
The Y Smith chart is constructed in a similar way to the Z Smith chart case but
by expressing values of voltage reflection coefficient in terms of normalised
admittance instead of normalised impedance. The normalised admittance yT is the
reciprocal of the normalised impedance zT, so
          y  T   =   1  z  T        {\displaystyle y_{\text{T}}={\frac {1}{z_
      {\text{T}}}}\,}  [{\displaystyle y_{\text{T}}={\frac {1}{z_{\text
      {T}}}}\,}]
Therefore:
          y  T   =    1 &#x2212; &#x0393;   1 + &#x0393;       {\displaystyle
      y_{\text{T}}={\frac {1-\Gamma }{1+\Gamma }}\,}  [{\displaystyle y_{\text
      {T}}={\frac {1-\Gamma }{1+\Gamma }}\,}]
and
         &#x0393; =    1 &#x2212;  y  T     1 +  y  T         {\displaystyle
      \Gamma ={\frac {1-y_{\text{T}}}{1+y_{\text{T}}}}\,}  [{\displaystyle
      \Gamma ={\frac {1-y_{\text{T}}}{1+y_{\text{T}}}}\,}]
The Y Smith chart appears like the normalised impedance type but with the
graphic scaling rotated through 180Â°, the numeric scaling remaining unchanged.
The region above the x-axis represents capacitive admittances and the region
below the x-axis represents inductive admittances. Capacitive admittances have
positive imaginary parts and inductive admittances have negative imaginary
parts.
Again, if the termination is perfectly matched the reflection coefficient will
be zero, represented by a 'circle' of zero radius or in fact a point at the
centre of the Smith chart. If the termination was a perfect open or short
circuit the magnitude of the voltage reflection coefficient would be unity, all
power would be reflected and the point would lie at some point on the unity
circumference circle of the Smith chart.
**** Practical examples[edit] ****
Example points plotted on the normalised impedance Smith chart
A point with a reflection coefficient magnitude 0.63 and angle 60Â° represented
in polar form as     0.63 &#x2220;  60  &#x2218;      {\displaystyle 0.63\angle
60^{\circ }\,}  [0.63\angle 60^{\circ }\,], is shown as point P1 on the Smith
chart. To plot this, one may use the circumferential (reflection coefficient)
angle scale to find the     &#x2220;  60  &#x2218;      {\displaystyle \angle
60^{\circ }\,}  [\angle 60^{\circ }\,] graduation and a ruler to draw a line
passing through this and the centre of the Smith chart. The length of the line
would then be scaled to P1 assuming the Smith chart radius to be unity. For
example, if the actual radius measured from the paper was 100 mm, the length
OP1 would be 63 mm.
The following table gives some similar examples of points which are plotted on
the Z Smith chart. For each, the reflection coefficient is given in polar form
together with the corresponding normalised impedance in rectangular form. The
conversion may be read directly from the Smith chart or by substitution into
the equation.
 ___Some_examples_of_points_plotted_on_the_normalised_impedance_Smith_chart___
|Point Identity |Reflection Coefficient (Polar |Normalised Impedance          |
|_______________|Form)_________________________|(Rectangular_Form)____________|
|               |   0.63 &#x2220;  60  &#x2218;|   0.80 + j 1.40              |
|P1 (Inductive) |{\displaystyle 0.63\angle 60^ |{\displaystyle 0.80+j1.40\,}  |
|               |{\circ }\,}  [0.63\angle 60^  |[0.80+j1.40\,]                |
|_______________|{\circ_}\,]___________________|______________________________|
|               |   0.73 &#x2220;  125         |   0.20 + j 0.50              |
|P2 (Inductive) |&#x2218;      {\displaystyle  |{\displaystyle 0.20+j0.50\,}  |
|               |0.73\angle 125^{\circ }\,}    |[0.20+j0.50\,]                |
|_______________|[0.73\angle_125^{\circ_}\,]___|______________________________|
|               |   0.44 &#x2220; &#x2212;  116|   0.50 &#x2212; j 0.50       |
|P3 (Capacitive)|&#x2218;      {\displaystyle  |{\displaystyle 0.50-j0.50\,}  |
|               |0.44\angle -116^{\circ }\,}   |[0.50-j0.50\,]                |
|_______________|[0.44\angle_-116^{\circ_}\,]__|______________________________|
**** Working with both the Z Smith chart and the Y Smith charts[edit] ****
In RF circuit and matching problems sometimes it is more convenient to work
with admittances (representing conductances and susceptances) and sometimes it
is more convenient to work with impedances (representing resistances and
reactances). Solving a typical matching problem will often require several
changes between both types of Smith chart, using normalised impedance for
series elements and normalised admittances for parallel elements. For these a
dual (normalised) impedance and admittance Smith chart may be used.
Alternatively, one type may be used and the scaling converted to the other when
required. In order to change from normalised impedance to normalised admittance
or vice versa, the point representing the value of reflection coefficient under
consideration is moved through exactly 180 degrees at the same radius. For
example, the point P1 in the example representing a reflection coefficient of
0.63 &#x2220;  60  &#x2218;      {\displaystyle 0.63\angle 60^{\circ }\,}
[0.63\angle 60^{\circ }\,] has a normalised impedance of      z  P   = 0.80 + j
1.40    {\displaystyle z_{P}=0.80+j1.40\,}  [z_{P}=0.80+j1.40\,]. To
graphically change this to the equivalent normalised admittance point, say Q1,
a line is drawn with a ruler from P1 through the Smith chart centre to Q1, an
equal radius in the opposite direction. This is equivalent to moving the point
through a circular path of exactly 180 degrees. Reading the value from the
Smith chart for Q1, remembering that the scaling is now in normalised
admittance, gives      y  P   = 0.30 &#x2212; j 0.54    {\displaystyle y_
{P}=0.30-j0.54\,}  [{\displaystyle y_{P}=0.30-j0.54\,}]. Performing the
calculation
          y  T   =   1  z  T        {\displaystyle y_{\text{T}}={\frac {1}{z_
      {\text{T}}}}\,}  [{\displaystyle y_{\text{T}}={\frac {1}{z_{\text
      {T}}}}\,}]
manually will confirm this.
Once a transformation from impedance to admittance has been performed, the
scaling changes to normalised admittance until a later transformation back to
normalised impedance is performed.
The table below shows examples of normalised impedances and their equivalent
normalised admittances obtained by rotation of the point through 180Â°. Again,
these may be obtained either by calculation or using a Smith chart as shown,
converting between the normalised impedance and normalised admittances planes.
     Values of reflection coefficient as normalised impedances and the
 ____________________equivalent_normalised_admittances____________________
|Normalised_Impedance_Plane______|Normalised_Admittance_Plane_____________|
|P1 (    z = 0.80 + j 1.40       |Q1 (    y = 0.30 &#x2212; j 0.54        |
|{\displaystyle z=0.80+j1.40\,}  |{\displaystyle y=0.30-j0.54\,}  [y=0.30-|
|[z=0.80+j1.40\,])_______________|j0.54\,])_______________________________|
|P10 (    z = 0.10 + j 0.22      |Q10 (    y = 1.80 &#x2212; j 3.90       |
|{\displaystyle z=0.10+j0.22\,}  |{\displaystyle y=1.80-j3.90\,}  [y=1.80-|
|[z=0.10+j0.22\,])_______________|j3.90\,])_______________________________|
Values of complex reflection coefficient plotted on the normalised impedance
Smith chart and their equivalents on the normalised admittance Smith chart
**** Choice of Smith chart type and component type[edit] ****
The choice of whether to use the Z Smith chart or the Y Smith chart for any
particular calculation depends on which is more convenient. Impedances in
series and admittances in parallel add while impedances in parallel and
admittances in series are related by a reciprocal equation. If      Z  TS
{\displaystyle Z_{\text{TS}}}  [{\displaystyle Z_{\text{TS}}}] is the
equivalent impedance of series impedances and      Z  TP     {\displaystyle Z_
{\text{TP}}}  [{\displaystyle Z_{\text{TP}}}] is the equivalent impedance of
parallel impedances, then
          Z  TS   =  Z  1   +  Z  2   +  Z  3   + . . .    {\displaystyle Z_
      {\text{TS}}=Z_{1}+Z_{2}+Z_{3}+...\,}  [{\displaystyle Z_{\text{TS}}=Z_
      {1}+Z_{2}+Z_{3}+...\,}]
           1  Z  TP     =   1  Z  1     +   1  Z  2     +   1  Z  3     + . . .
      {\displaystyle {\frac {1}{Z_{\text{TP}}}}={\frac {1}{Z_{1}}}+{\frac {1}
      {Z_{2}}}+{\frac {1}{Z_{3}}}+...\,}  [{\displaystyle {\frac {1}{Z_{\text
      {TP}}}}={\frac {1}{Z_{1}}}+{\frac {1}{Z_{2}}}+{\frac {1}{Z_{3}}}+...\,}]
For admittances the reverse is true, that is
          Y  TP   =  Y  1   +  Y  2   +  Y  3   + . . .    {\displaystyle Y_
      {\text{TP}}=Y_{1}+Y_{2}+Y_{3}+...\,}  [{\displaystyle Y_{\text{TP}}=Y_
      {1}+Y_{2}+Y_{3}+...\,}]
           1  Y  TS     =   1  Y  1     +   1  Y  2     +   1  Y  3     + . . .
      {\displaystyle {\frac {1}{Y_{\text{TS}}}}={\frac {1}{Y_{1}}}+{\frac {1}
      {Y_{2}}}+{\frac {1}{Y_{3}}}+...\,}  [{\displaystyle {\frac {1}{Y_{\text
      {TS}}}}={\frac {1}{Y_{1}}}+{\frac {1}{Y_{2}}}+{\frac {1}{Y_{3}}}+...\,}]
Dealing with the reciprocals, especially in complex numbers, is more time
consuming and error-prone than using linear addition. In general therefore,
most RF engineers work in the plane where the circuit_topography supports
linear addition. The following table gives the complex expressions for
impedance (real and normalised) and admittance (real and normalised) for each
of the three basic passive_circuit_elements: resistance, inductance and
capacitance. Using just the characteristic impedance (or characteristic
admittance) and test frequency an equivalent_circuit can be found and vice
versa.
                   Expressions for Impedance and Admittance
 _________________Normalised_by_Impedance_Z0_or_Admittance_Y0_________________
|              |Impedance (Z or z) or         |Admittance (Y or y) or         |
|              |Reactance_(X_or_x)____________|Susceptance_(B_or_b)___________|
|              |Real          |               |               |               |
|Element Type  |(    &#x03A9; |Normalised (No |               |Normalised (No |
|              |{\displaystyle|Unit)          |Real (S)       |Unit)          |
|              |\Omega \,}    |               |               |               |
|______________|[\Omega_\,])__|_______________|_______________|_______________|
|              |              |               |               |   y = g =   1 |
|              |              |               |               |R  Y  0      = |
|              |              |   z =   R  Z  |               |Z  0   R       |
|              |              |0     = R  Y  0|   Y = G =   1 |{\displaystyle |
|              |   Z = R      |{\displaystyle |R              |y=g={\frac {1} |
|              |{\displaystyle|z={\frac {R}{Z_|{\displaystyle |{RY_{0}}}=     |
|Resistance (R)|Z=R\,}  [     |{0}}}=RY_{0}\,}|Y=G={\frac {1} |{\frac {Z_{0}} |
|              |{\displaystyle|[{\displaystyle|{R}}\,}  [Y=G= |{R}}\,}  [     |
|              |Z=R\,}]       |z={\frac {R}{Z_|{\frac  {1}    |{\displaystyle |
|              |              |{0}}}=RY_      |{R}}\,]        |y=g={\frac {1} |
|              |              |{0}\,}]        |               |{RY_{0}}}=     |
|              |              |               |               |{\frac {Z_{0}} |
|______________|______________|_______________|_______________|{R}}\,}]_______|
|              |              |               |               |   y = &#x2212;|
|              |              |               |               |j  b  L   =    |
|              |              |   z = j  x  L |               |&#x2212; j     |
|              |              |= j    &#x03C9;|               |&#x03C9; L  Y  |
|              |              |L   Z  0     = |               |0      =       |
|              |              |j &#x03C9; L  Y|   Y = &#x2212;|&#x2212; j  Z  |
|              |   Z = j  X  L|0              |j  B  L   =    |0     &#x03C9; |
|              |= j &#x03C9; L|{\displaystyle |&#x2212; j     |L              |
|              |{\displaystyle|z=jx_{\text    |&#x03C9; L     |{\displaystyle |
|              |Z=jX_{\text   |{L}}=j{\frac   |{\displaystyle |y=-jb_{\text   |
|Inductance (L)|{L}}=j\omega  |{\omega L}{Z_  |Y=-jB_{\text   |{L}}={\frac {- |
|              |L\,}  [       |{0}}}=j\omega  |{L}}={\frac {- |j}{\omega LY_  |
|              |{\displaystyle|LY_{0}\,}  [   |j}{\omega L}}} |{0}}}={\frac {-|
|              |Z=jX_{\text   |{\displaystyle |[{\displaystyle|jZ_{0}}{\omega |
|              |{L}}=j\omega  |z=jx_{\text    |Y=-jB_{\text   |L}}\,}  [      |
|              |L\,}]         |{L}}=j{\frac   |{L}}={\frac {- |{\displaystyle |
|              |              |{\omega L}{Z_  |j}{\omega L}}}]|y=-jb_{\text   |
|              |              |{0}}}=j\omega  |               |{L}}={\frac {- |
|              |              |LY_{0}\,}]     |               |j}{\omega LY_  |
|              |              |               |               |{0}}}={\frac {-|
|              |              |               |               |jZ_{0}}{\omega |
|______________|______________|_______________|_______________|L}}\,}]________|
|              |              |   z = &#x2212;|               |               |
|              |              |j  x  C   =    |               |               |
|              |              |&#x2212; j     |               |   y = j  b  C |
|              |   Z =        |&#x03C9; C  Z  |               |= j    &#x03C9;|
|              |&#x2212; j  X |0      =       |               |C   Y  0     = |
|              |C   =         |&#x2212; j  Y  |               |j &#x03C9; C  Z|
|              |&#x2212; j    |0     &#x03C9; |   Y = j  B  C |0              |
|              |&#x03C9; C    |C              |= j &#x03C9; C |{\displaystyle |
|              |{\displaystyle|{\displaystyle |{\displaystyle |y=jb_{\text    |
|              |Z=-jX_{\text  |z=-jx_{\text   |Y=jB_{\text    |{C}}=j{\frac   |
|Capacitance   |{C}}={\frac {-|{C}}={\frac {- |{C}}=j\omega   |{\omega C}{Y_  |
|(C)           |j}{\omega     |j}{\omega CZ_  |C\,}  [        |{0}}}=j\omega  |
|              |C}}\,}  [     |{0}}}={\frac {-|{\displaystyle |CZ_{0}\,}  [   |
|              |{\displaystyle|jY_{0}}{\omega |Y=jB_{\text    |{\displaystyle |
|              |Z=-jX_{\text  |C}}\,}  [      |{C}}=j\omega   |y=jb_{\text    |
|              |{C}}={\frac {-|{\displaystyle |C\,}]          |{C}}=j{\frac   |
|              |j}{\omega     |z=-jx_{\text   |               |{\omega C}{Y_  |
|              |C}}\,}]       |{C}}={\frac {- |               |{0}}}=j\omega  |
|              |              |j}{\omega CZ_  |               |CZ_{0}\,}]     |
|              |              |{0}}}={\frac {-|               |               |
|              |              |jY_{0}}{\omega |               |               |
|______________|______________|C}}\,}]________|_______________|_______________|
***** Using the Smith chart to solve conjugate matching problems with
distributed components[edit] *****
Distributed matching becomes feasible and is sometimes required when the
physical size of the matching components is more than about 5% of a wavelength
at the operating frequency. Here the electrical behaviour of many lumped
components becomes rather unpredictable. This occurs in microwave circuits and
when high power requires large components in shortwave, FM and TV Broadcasting,
For distributed components the effects on reflection coefficient and impedance
of moving along the transmission line must be allowed for using the outer
circumferential scale of the Smith chart which is calibrated in wavelengths.
The following example shows how a transmission line, terminated with an
arbitrary load, may be matched at one frequency either with a series or
parallel reactive component in each case connected at precise positions.
Smith chart construction for some distributed transmission line matching
Supposing a loss-free air-spaced transmission line of characteristic impedance
Z  0   = 50 &#xA0; &#x03A9;   {\displaystyle Z_{0}=50\ \Omega }  [Z_{0}=50\
\Omega ], operating at a frequency of 800 MHz, is terminated with a circuit
comprising a 17.5     &#x03A9;   {\displaystyle \Omega }  [\Omega ] resistor in
series with a 6.5 nanohenry (6.5 nH) inductor. How may the line be matched?
From the table above, the reactance of the inductor forming part of the
termination at 800 MHz is
          Z  L   = j &#x03C9; L = j 2 &#x03C0; f L = j 32.7 &#xA0; &#x03A9;
      {\displaystyle Z_{L}=j\omega L=j2\pi fL=j32.7\ \Omega \,}  [Z_{L}=j\omega
      L=j2\pi fL=j32.7\ \Omega \,]
so the impedance of the combination (     Z  T     {\displaystyle Z_{T}}  [Z_
{T}]) is given by
          Z  T   = 17.5 + j 32.7 &#xA0; &#x03A9;    {\displaystyle Z_
      {T}=17.5+j32.7\ \Omega \,}  [Z_{T}=17.5+j32.7\ \Omega \,]
and the normalised impedance (     z  T     {\displaystyle z_{T}}  [z_{T}]) is
          z  T   =    Z  T    Z  0     = 0.35 + j 0.65    {\displaystyle z_{T}=
      {\frac {Z_{T}}{Z_{0}}}=0.35+j0.65\,}  [z_{T}={\frac  {Z_{T}}{Z_
      {0}}}=0.35+j0.65\,]
This is plotted on the Z Smith chart at point P20. The line OP20 is extended
through to the wavelength scale where it intersects at the point      L  1   =
0.098 &#x03BB;    {\displaystyle L_{1}=0.098\lambda \,}  [L_{1}=0.098\lambda
\,]. As the transmission line is loss free, a circle centred at the centre of
the Smith chart is drawn through the point P20 to represent the path of the
constant magnitude reflection coefficient due to the termination. At point P21
the circle intersects with the unity circle of constant normalised resistance
at
          z  P 21   = 1.00 + j 1.52    {\displaystyle z_{P21}=1.00+j1.52\,}
      [z_{{P21}}=1.00+j1.52\,].
The extension of the line OP21 intersects the wavelength scale at      L  2   =
0.177 &#x03BB;    {\displaystyle L_{2}=0.177\lambda \,}  [L_{2}=0.177\lambda
\,], therefore the distance from the termination to this point on the line is
given by
          L  2   &#x2212;  L  1   = 0.177 &#x03BB; &#x2212; 0.098 &#x03BB; =
      0.079 &#x03BB;    {\displaystyle L_{2}-L_{1}=0.177\lambda -0.098\lambda
      =0.079\lambda \,}  [L_{2}-L_{1}=0.177\lambda -0.098\lambda =0.079\lambda
      \,]
Since the transmission line is air-spaced, the wavelength at 800 MHz in the
line is the same as that in free space and is given by
         &#x03BB; =   c f      {\displaystyle \lambda ={\frac {c}{f}}\,}
      [\lambda ={\frac  {c}{f}}\,]
where     c    {\displaystyle c\,}  [c\,] is the velocity of electromagnetic
radiation_in_free_space and     f    {\displaystyle f\,}  [f\,] is the
frequency in hertz. The result gives     &#x03BB; = 375 &#xA0;  m m
{\displaystyle \lambda =375\ \mathrm {mm} \,}  [\lambda =375\ {\mathrm
{mm}}\,], making the position of the matching component 29.6 mm from the load.
The conjugate match for the impedance at P21 (     z  m a t c h
{\displaystyle z_{match}\,}  [z_{{match}}\,]) is
          z  m a t c h   = &#x2212; j ( 1.52 ) ,    {\displaystyle z_{match}=-j
      (1.52),\!}  [z_{{match}}=-j(1.52),\!]
As the Smith chart is still in the normalised impedance plane, from the table
above a series capacitor      C  m      {\displaystyle C_{m}\,}  [C_{m}\,] is
required where
          z  m a t c h   = &#x2212; j 1.52 =    &#x2212; j   &#x03C9;  C  m
      Z  0      =    &#x2212; j   2 &#x03C0; f  C  m    Z  0
      {\displaystyle z_{match}=-j1.52={\frac {-j}{\omega C_{m}Z_{0}}}={\frac {-
      j}{2\pi fC_{m}Z_{0}}}\,}  [z_{{match}}=-j1.52={\frac  {-j}{\omega C_{m}Z_
      {0}}}={\frac  {-j}{2\pi fC_{m}Z_{0}}}\,]
Rearranging, we obtain
          C  m   =   1  ( 1.52 ) &#x03C9;  Z  0      =   1  ( 1.52 ) ( 2
      &#x03C0; f )  Z  0        {\displaystyle C_{m}={\frac {1}{(1.52)\omega Z_
      {0}}}={\frac {1}{(1.52)(2\pi f)Z_{0}}}}  [C_{m}={\frac  {1}{(1.52)\omega
      Z_{0}}}={\frac  {1}{(1.52)(2\pi f)Z_{0}}}].
Substitution of known values gives
          C  m   = 2.6 &#xA0;  p F     {\displaystyle C_{m}=2.6\ \mathrm {pF}
      \,}  [C_{m}=2.6\ {\mathrm  {pF}}\,]
To match the termination at 800 MHz, a series capacitor of 2.6 pF must be
placed in series with the transmission line at a distance of 29.6 mm from the
termination.
An alternative shunt match could be calculated after performing a Smith chart
transformation from normalised impedance to normalised admittance. Point Q20 is
the equivalent of P20 but expressed as a normalised admittance. Reading from
the Smith chart scaling, remembering that this is now a normalised admittance
gives
          y  Q 20   = 0.65 &#x2212; j 1.20    {\displaystyle y_{Q20}=0.65-
      j1.20\,}  [y_{{Q20}}=0.65-j1.20\,]
(In fact this value is not actually used). However, the extension of the line
OQ20 through to the wavelength scale gives      L  3   = 0.152 &#x03BB;
{\displaystyle L_{3}=0.152\lambda \,}  [L_{3}=0.152\lambda \,]. The earliest
point at which a shunt conjugate match could be introduced, moving towards the
generator, would be at Q21, the same position as the previous P21, but this
time representing a normalised admittance given by
          y  Q 21   = 1.00 + j 1.52    {\displaystyle y_{Q21}=1.00+j1.52\,}
      [y_{{Q21}}=1.00+j1.52\,].
The distance along the transmission line is in this case
          L  2   +  L  3   = 0.177 &#x03BB; + 0.152 &#x03BB; = 0.329 &#x03BB;
      {\displaystyle L_{2}+L_{3}=0.177\lambda +0.152\lambda =0.329\lambda \,}
      [L_{2}+L_{3}=0.177\lambda +0.152\lambda =0.329\lambda \,]
which converts to 123 mm.
The conjugate matching component is required to have a normalised admittance
(     y  m a t c h     {\displaystyle y_{match}}  [y_{{match}}]) of
          y  m a t c h   = &#x2212; j 1.52    {\displaystyle y_{match}=-
      j1.52\,}  [y_{{match}}=-j1.52\,].
From the table it can be seen that a negative admittance would require an
inductor, connected in parallel with the transmission line. If its value is
L  m      {\displaystyle L_{m}\,}  [L_{m}\,], then
         &#x2212; j 1.52 =    &#x2212; j   &#x03C9;  L  m    Y  0      =
      &#x2212; j  Z  0     2 &#x03C0; f  L  m         {\displaystyle -j1.52=
      {\frac {-j}{\omega L_{m}Y_{0}}}={\frac {-jZ_{0}}{2\pi fL_{m}}}\,}  [-
      j1.52={\frac  {-j}{\omega L_{m}Y_{0}}}={\frac  {-jZ_{0}}{2\pi fL_{m}}}\,]
This gives the result
          L  m   = 6.5 &#xA0;  n H     {\displaystyle L_{m}=6.5\ \mathrm {nH}
      \,}  [L_{m}=6.5\ {\mathrm  {nH}}\,]
A suitable inductive shunt matching would therefore be a 6.5 nH inductor in
parallel with the line positioned at 123 mm from the load.
***** Using the Smith chart to analyze lumped element circuits[edit] *****
The analysis of lumped element components assumes that the wavelength at the
frequency of operation is much greater than the dimensions of the components
themselves. The Smith chart may be used to analyze such circuits in which case
the movements around the chart are generated by the (normalized) impedances and
admittances of the components at the frequency of operation. In this case the
wavelength scaling on the Smith chart circumference is not used. The following
circuit will be analyzed using a Smith chart at an operating frequency of
100 MHz. At this frequency the free space wavelength is 3 m. The component
dimensions themselves will be in the order of millimetres so the assumption of
lumped components will be valid. Despite there being no transmission line as
such, a system impedance must still be defined to enable normalization and de-
normalization calculations and      Z  0   = 50 &#xA0; &#x03A9;
{\displaystyle Z_{0}=50\ \Omega \,}  [Z_{0}=50\ \Omega \,] is a good choice
here as      R  1   = 50 &#xA0; &#x03A9;    {\displaystyle R_{1}=50\ \Omega \,}
[R_{1}=50\ \Omega \,]. If there were very different values of resistance
present a value closer to these might be a better choice.
A lumped element circuit which may be analysed using a Smith chart
Smith chart with graphical construction for analysis of a lumped circuit
The analysis starts with a Z Smith chart looking into R1 only with no other
components present. As      R  1   = 50 &#xA0; &#x03A9;    {\displaystyle R_
{1}=50\ \Omega \,}  [R_{1}=50\ \Omega \,] is the same as the system impedance,
this is represented by a point at the centre of the Smith chart. The first
transformation is OP1 along the line of constant normalized resistance in this
case the addition of a normalized reactance of -j0.80, corresponding to a
series capacitor of 40 pF. Points with suffix P are in the Z plane and points
with suffix Q are in the Y plane. Therefore, transformations P1 to Q1 and P3 to
Q3 are from the Z Smith chart to the Y Smith chart and transformation Q2 to P2
is from the Y Smith chart to the Z Smith chart. The following table shows the
steps taken to work through the remaining components and transformations,
returning eventually back to the centre of the Smith chart and a perfect 50 ohm
match.
 _______________Smith_chart_steps_for_analysing_a_lumped_element_circuit________________
|              |              |x or y        |Capacitance/|Formula to    |              |
|Transformation|Plane         |Normalized    |Inductance  |Solve         |Result        |
|______________|______________|Value_________|____________|______________|______________|
|              |              |              |            |   &#x2212; j |              |
|              |              |              |            |0.80 =        |    C  1   =  |
|   O &#x2192; |              |              |            |&#x2212; j    |40 &#xA0;  p F|
|P  1          |              |   &#x2212; j |            |&#x03C9;  C  1|{\displaystyle|
|{\displaystyle|   Z          |0.80          |            |Z  0          |C_{1}=40\     |
|O\rightarrow  |{\displaystyle|{\displaystyle|Capacitance |{\displaystyle|\mathrm {pF}  |
|P_{1}\,}      |Z\,}  [Z\,]   |-j0.80\,}  [- |(Series)    |-j0.80={\frac |\,}  [C_      |
|[O\rightarrow |              |j0.80\,]      |            |{-j}{\omega C_|{1}=40\       |
|P_{1}\,]      |              |              |            |{1}Z_{0}}}\,} |{\mathrm      |
|              |              |              |            |[-j0.80={\frac|{pF}}\,]      |
|              |              |              |            |{-j}{\omega C_|              |
|______________|______________|______________|____________|{1}Z_{0}}}\,]_|______________|
|              |              |              |            |   &#x2212; j |              |
|              |              |              |            |1.49 =        |    L  1   =  |
|    Q  1      |              |              |            |&#x2212; j    |53 &#xA0;  n H|
|&#x2192;  Q  2|              |   &#x2212; j |            |&#x03C9;  L  1|{\displaystyle|
|{\displaystyle|   Y          |1.49          |            |Y  0          |L_{1}=53\     |
|Q_            |{\displaystyle|{\displaystyle|Inductance  |{\displaystyle|\mathrm {nH}  |
|{1}\rightarrow|Y\,}  [Y\,]   |-j1.49\,}  [- |(Shunt)     |-j1.49={\frac |\,}  [L_      |
|Q_{2}\,}  [Q_ |              |j1.49\,]      |            |{-j}{\omega L_|{1}=53\       |
|{1}\rightarrow|              |              |            |{1}Y_{0}}}\,} |{\mathrm      |
|Q_{2}\,]      |              |              |            |[-j1.49={\frac|{nH}}\,]      |
|              |              |              |            |{-j}{\omega L_|              |
|______________|______________|______________|____________|{1}Y_{0}}}\,]_|______________|
|              |              |              |            |   &#x2212; j |              |
|              |              |              |            |0.23 =        |    C  2   =  |
|    P  2      |              |              |            |&#x2212; j    |138 &#xA0;  p |
|&#x2192;  P  3|              |   &#x2212; j |            |&#x03C9;  C  2|F             |
|{\displaystyle|              |0.23          |            |Z  0          |{\displaystyle|
|P_            |Z             |{\displaystyle|Capacitance |{\displaystyle|C_{2}=138\    |
|{2}\rightarrow|              |-j0.23\,}  [- |(Series)    |-j0.23={\frac |\mathrm {pF}  |
|P_{3}\,}  [P_ |              |j0.23\,]      |            |{-j}{\omega C_|\,}  [C_      |
|{2}\rightarrow|              |              |            |{2}Z_{0}}}\,} |{2}=138\      |
|P_{3}\,]      |              |              |            |[-j0.23={\frac|{\mathrm      |
|              |              |              |            |{-j}{\omega C_|{pF}}\,]      |
|______________|______________|______________|____________|{2}Z_{0}}}\,]_|______________|
|              |              |              |            |   + j 1.14 = |              |
|              |              |              |            |j &#x03C9;  C |    C  3   =  |
|    Q  3      |              |              |            |3     Y  0    |36 &#xA0;  p F|
|&#x2192; O    |              |              |            |{\displaystyle|{\displaystyle|
|{\displaystyle|              |   + j 1.14   |            |+j1.14={\frac |C_{3}=36\     |
|Q_            |Y             |{\displaystyle|Capacitance |{j\omega C_   |\mathrm {pF}  |
|{3}\rightarrow|              |+j1.14\,}     |(Shunt)     |{3}}{Y_       |\,}  [C_      |
|O\,}  [Q_     |              |[+j1.14\,]    |            |{0}}}\,}      |{3}=36\       |
|{3}\rightarrow|              |              |            |[+j1.14={\frac|{\mathrm      |
|O\,]          |              |              |            |{j\omega C_   |{pF}}\,]      |
|              |              |              |            |{3}}{Y_       |              |
|______________|______________|______________|____________|{0}}}\,]______|______________|
***** 3D Smith chart[edit] *****
[3D_Smith_chart_representation.]
3D Smith chart representation
A generalized 3D Smith chart based on the extended complex plane (Riemann
sphere) and inversive_geometry was proposed in 2011. The chart unifies the
passive and active circuit design on little and big circles on the surface of a
unit sphere using the stereographic conformal_map of the reflection
coefficient's generalized plane. Considering the point at infinity, the space
of the new chart includes all possible loads. The north pole is the perfect
matching point, while the south pole is the perfect mismatch point.[10]
***** References[edit] *****
   1. ^ Smith, P. H.; Transmission Line Calculator; Electronics, Vol. 12, No.
      1, pp 29-31, January 1939
   2. ^ Smith, P. H.; An Improved Transmission Line Calculator; Electronics,
      Vol. 17, No. 1, p 130, January 1944
   3. ^ Ramo, Whinnery and Van Duzer (1965); "Fields and Waves in
      Communications Electronics"; John Wiley & Sons; pp 35-39. ISBN
   4. ^ Pozar, David M. (2005); Microwave Engineering, Third Edition (Intl.
      Ed.); John Wiley & Sons, Inc.; pp 64-71.
   5. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   6. ISBN 0-471-44878-8.
   7. ^ Gonzalez, Guillermo (1997); Microwave Transistor Amplifiers Analysis
      and Design, Second Edition; Prentice Hall NJ; pp 93-103.
   8. ISBN 0-13-254335-4.
   9. ^ Gonzalez, Guillermo (1997) (op. cit);pp 98-101
  10. ^ Gonzalez, Guillermo (1997) (op. cit);p 97
  11. ^ Hayt, William H Jr.; "Engineering Electromagnetics" Fourth Ed; McGraw-
      Hill International Book Company; pp 428â433.
  12. ISBN 0-07-027395-2.
  13. ^ Davidson, C. W.;"Transmission Lines for Communications with CAD
      Programs";Macmillan; pp 80-85.
  14. ISBN 0-333-47398-1
  15. ^ Andrei Muller, Pablo Soto, D. Dascalu, D. Neculoiu, V.E. Boria A_3D
      Smith_chart_based_on_the_Riemann_sphere_for_Active_and_Passive_Microwave
      Circuits, Microwave and Wireless Components Letters doi:10.1109/
      LMWC.2011.2132697
    * Mizuhashi, T., Theory of four-terminal impedance transformation circuit
      and matching circuit, The Journal of the Institute of Electrical
      Communication Engineers of Japan, pp. 1053â1058, December 1937.
    * P.H.Smith 1969 Electronic Applications of the Smith Chart. Kay Electric
      Company
***** Further reading[edit] *****
    * For an early representation of this graphical depiction before they were
      called 'Smith Charts', see G._A._Campbell, "Cisoidal Oscillations", Proc.
      AIEE, 30, 1-6, pp. 789â824 (1911). In particular, Fig. 13 on p. 810.
***** External links[edit] *****
 Wikimedia Commons has media related to Smith_charts.
    * Mathematical_Construction_and_Properties_of_the_Smith_Chart
    * Smith_Chart_and_Impedance_Matching_Tutorial_with_Examples
    * The_Mizuhashi-Smith_Chart
    * Excel_Smith_Chart. Non-commercial, interactive Smith Chart that looks
      best in Excel 2007+
    * 3D_Smith_chart_tool (java required). Non-commercial generalized tool for
      active and passive circuits
    * SimSmith. Non-commercial, available for Windows, Mac, and Linux. Many
      Smith chart tutorial videos. No circuit size restrictions. Not limited to
      ladder circuits.
    * Smith_v3.xx. Commercial and free Smith chart for Windows
    * QuickSmith. Free web based Smith Chart Educational tool available on
      Github.
Authority_control [Edit_this_at_Wikidata]     * GND: 7715904-4

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Smith_chart&oldid=892969895"
Categories:
    * Electrical_engineering
    * Charts
Hidden categories:
    * Use_British_English_from_August_2017
    * Commons_category_link_is_on_Wikidata
    * Wikipedia_articles_with_GND_identifiers
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
    * CatalÃ 
    * Dansk
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
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
    * ä¸­æ
Edit_links
    * This page was last edited on 18 April 2019, at 02:26 (UTC).
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
