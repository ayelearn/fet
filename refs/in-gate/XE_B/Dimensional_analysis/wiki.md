The following text has been accessed from https://en.wikipedia.org/wiki/Dimensional_analysis at Fri Aug 9 01:22:25 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Dimensional analysis ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In engineering and science, dimensional analysis is the analysis of the
relationships between different physical_quantities by identifying their base
quantities (such as length, mass, time, and electric_charge) and units_of
measure (such as miles vs. kilometers, or pounds vs. kilograms) and tracking
these dimensions as calculations or comparisons are performed. The conversion
of_units from one dimensional unit to another is often somewhat complex.
Dimensional analysis, or more specifically the factor-label method, also known
as the unit-factor method, is a widely used technique for such conversions
using the rules of algebra.[1][2][3]
The concept of physical dimension was introduced by Joseph_Fourier in 1822.[4]
Physical quantities that are of the same kind (also called commensurable)
(e.g., length or time or mass) have the same dimension and can be directly
compared to other physical quantities of the same kind (i.e., length or time or
mass, resp.), even if they are originally expressed in differing units of
measure (such as yards and meters). If physical quantities have different
dimensions (such as length vs. mass), they cannot be expressed in terms of
similar units and cannot be compared in quantity (also called incommensurable).
For example, asking whether a kilogram is larger than an hour is meaningless.
Any physically meaningful equation (and any inequality) will have the same
dimensions on its left and right sides, a property known as dimensional
homogeneity. Checking for dimensional homogeneity is a common application of
dimensional analysis, serving as a plausibility check on derived equations and
computations. It also serves as a guide and constraint in deriving equations
that may describe a physical system in the absence of a more rigorous
derivation.
⁰
***** Contents *****
    * 1_Concrete_numbers_and_base_units
          o 1.1_Percentages_and_derivatives
    * 2_Conversion_factor
    * 3_Dimensional_homogeneity
    * 4_The_factor-label_method_for_converting_units
          o 4.1_Checking_equations_that_involve_dimensions
          o 4.2_Limitations
    * 5_Applications
          o 5.1_Mathematics
          o 5.2_Finance,_economics,_and_accounting
          o 5.3_Fluid_mechanics
    * 6_History
    * 7_Mathematical_examples
          o 7.1_Definition
          o 7.2_Mathematical_properties
          o 7.3_Mechanics
          o 7.4_Other_fields_of_physics_and_chemistry
          o 7.5_Polynomials_and_transcendental_functions
          o 7.6_Incorporating_units
          o 7.7_Position_vs_displacement
          o 7.8_Orientation_and_frame_of_reference
    * 8_Examples
          o 8.1_A_simple_example:_period_of_a_harmonic_oscillator
          o 8.2_A_more_complex_example:_energy_of_a_vibrating_wire
          o 8.3_A_third_example:_demand_versus_capacity_for_a_rotating_disc
    * 9_Extensions
          o 9.1_Huntley's_extension:_directed_dimensions
          o 9.2_Siano's_extension:_orientational_analysis
    * 10_Dimensionless_concepts
          o 10.1_Constants
          o 10.2_Formalisms
    * 11_Dimensional_equivalences
          o 11.1_SI_units
          o 11.2_Natural_units
    * 12_See_also
          o 12.1_Related_areas_of_math
    * 13_Notes
    * 14_References
    * 15_External_links
          o 15.1_Converting_units
***** Concrete numbers and base units[edit] *****
Many parameters and measurements in the physical sciences and engineering are
expressed as a concrete_number â a numerical quantity and a corresponding
dimensional unit. Often a quantity is expressed in terms of several other
quantities; for example, speed is a combination of length and time, e.g. 60
miles per hour or 1.4 kilometers per second. Compound relations with "per" are
expressed with division, e.g. 60 mi/1 h. Other relations can involve
multiplication (often shown with a centered_dot or juxtaposition), powers (like
m2 for square meters), or combinations thereof.
A set of base_units for a system_of_measurement is a conventionally chosen set
of units, none of which can be expressed as a combination of the others, and in
terms of which all the remaining units of the system can be expressed.[5] For
example, units for length and time are normally chosen as base units. Units for
volume, however, can be factored into the base units of length (m3), thus they
are considered derived or compound units.
Sometimes the names of units obscure the fact that they are derived units. For
example, a newton (N) is a unit of force, which will have units of mass (kg)
times acceleration (mâsâ2). The newton is defined as 1 N = 1
kgâmâsâ2.
**** Percentages and derivatives[edit] ****
Percentages are dimensionless quantities, since they are ratios of two
quantities with the same dimensions. In other words, the % sign can be read as
"hundredths", since 1% = 1/100.
Taking a derivative with respect to a quantity adds the dimension of the
variable one is differentiating with respect to, in the denominator. Thus:
    * position (x) has the dimension L (length);
    * derivative of position with respect to time (dx/dt, velocity) has
      dimension LTâ1 â length from position, time due to the derivative;
    * the second derivative (d2x/dt2 = d(dx/dt) / dt, acceleration) has
      dimension LTâ2.
In economics, one distinguishes between stocks_and_flows: a stock has units of
"units" (say, widgets or dollars), while a flow is a derivative of a stock, and
has units of "units/time" (say, dollars/year).
In some contexts, dimensional quantities are expressed as dimensionless
quantities or percentages by omitting some dimensions. For example, debt-to-GDP
ratios are generally expressed as percentages: total debt outstanding
(dimension of currency) divided by annual GDP (dimension of currency) â but
one may argue that in comparing a stock to a flow, annual GDP should have
dimensions of currency/time (dollars/year, for instance), and thus Debt-to-GDP
should have units of years, which indicates that Debt-to-GDP is the number of
years needed for a constant GDP to pay the debt, if all GDP is spent on the
debt and the debt is otherwise unchanged.
***** Conversion factor[edit] *****
Main article: Conversion_factor
In dimensional analysis, a ratio which converts one unit of measure into
another without changing the quantity is called a conversion_factor. For
example, kPa and bar are both units of pressure, and 100 kPa = 1 bar. The rules
of algebra allow both sides of an equation to be divided by the same
expression, so this is equivalent to 100 kPa / 1 bar = 1. Since any quantity
can be multiplied by 1 without changing it, the expression "100 kPa / 1 bar"
can be used to convert from bars to kPa by multiplying it with the quantity to
be converted, including units. For example, 5 bar Ã 100 kPa / 1 bar = 500 kPa
because 5 Ã 100 / 1 = 500, and bar/bar cancels out, so 5 bar = 500 kPa.
***** Dimensional homogeneity[edit] *****
See also: Apples_and_oranges
The most basic rule of dimensional analysis is that of dimensional homogeneity.
[6]
            1. Only commensurable quantities (physical quantities having the
            same dimension) may be compared, equated, added, or subtracted.
However, the dimensions form an abelian_group under multiplication, so:
            2. One may take ratios of incommensurable quantities (quantities
            with different dimensions), and multiply or divide them.
For example, it makes no sense to ask whether 1 hour is more, the same, or less
than 1 kilometer, as these have different dimensions, nor to add 1 hour to 1
kilometer. However, it makes perfect sense to ask whether 1 mile is more, the
same, or less than 1 kilometer being the same dimension of physical quantity
even though the units are different. On the other hand, if an object travels
100 km in 2 hours, one may divide these and conclude that the object's average
speed was 50 km/h.
The rule implies that in a physically meaningful expression only quantities of
the same dimension can be added, subtracted, or compared. For example, if mman,
mrat and Lman denote, respectively, the mass of some man, the mass of a rat and
the length of that man, the dimensionally homogeneous expression mman + mrat is
meaningful, but the heterogeneous expression mman + Lman is meaningless.
However, mman/L2man is fine. Thus, dimensional analysis may be used as a sanity
check of physical equations: the two sides of any equation must be
commensurable or have the same dimensions.
This has the implication that most mathematical functions, particularly the
transcendental_functions must have a dimensionless quantity, a pure number, as
the argument and must return a dimensionless number as a result. This is clear
because many transcendental functions can be expressed as an infinite power
series with dimensionless coefficients.
         f ( x ) =  &#x2211;  n = 0   &#x221E;    a  n    x  n   =  a  0   +  a
      1   x +  a  2    x  2   +  a  3    x  3   + &#x22EF;   {\displaystyle f
      (x)=\sum _{n=0}^{\infty }a_{n}x^{n}=a_{0}+a_{1}x+a_{2}x^{2}+a_{3}x^
      {3}+\cdots }  [{\displaystyle f(x)=\sum _{n=0}^{\infty }a_{n}x^{n}=a_
      {0}+a_{1}x+a_{2}x^{2}+a_{3}x^{3}+\cdots }]
All powers of x must have the same dimension for the terms to be commensurable.
But if x is not dimensionless, then the different powers of x will have
different, incommensurable dimensions. However, power_functions including root
functions may have a dimensional argument and will return a result having
dimension that is the same power applied to the argument dimension. This is
because power functions and root functions are, loosely, just an expression of
multiplication of quantities.
Even when two physical quantities have identical dimensions, it may
nevertheless be meaningless to compare or add them. For example, although
torque and energy share the dimension L2MTâ2, they are fundamentally
different physical quantities.
To compare, add, or subtract quantities with the same dimensions but expressed
in different units, the standard procedure is first to convert them all to the
same units. For example, to compare 32 metres with 35 yards, use 1 yard =
0.9144 m to convert 35 yards to 32.004 m.
A related principle is that any physical law that accurately describes the real
world must be independent of the units used to measure the physical variables.
[7] For example, Newton's_laws_of_motion must hold true whether distance is
measured in miles or kilometers. This principle gives rise to the form that
conversion factors must take between units that measure the same dimension:
multiplication by a simple constant. It also ensures equivalence; for example,
if two buildings are the same height in feet, then they must be the same height
in meters.
***** The factor-label method for converting units[edit] *****
The factor-label method is the sequential application of conversion factors
expressed as fractions and arranged so that any dimensional unit appearing in
both the numerator and denominator of any of the fractions can be cancelled out
until only the desired set of dimensional units is obtained. For example, 10
miles_per_hour can be converted to meters_per_second by using a sequence of
conversion factors as shown below:
            10 &#xA0;   mile     1 &#xA0;   hour      &#x00D7;    1609.344
      &#xA0;meter    1 &#xA0;   mile      &#x00D7;    1 &#xA0;   hour     3600
      &#xA0;second     = 4.4704 &#xA0;   meter second   .   {\displaystyle
      {\frac {10\ {\cancel {\text{mile}}}}{1\ {\cancel {\text{hour}}}}}\times
      {\frac {1609.344{\text{ meter}}}{1\ {\cancel {\text{mile}}}}}\times
      {\frac {1\ {\cancel {\text{hour}}}}{3600{\text{ second}}}}=4.4704\ {\frac
      {\text{meter}}{\text{second}}}.}  [{\displaystyle {\frac {10\ {\cancel
      {\text{mile}}}}{1\ {\cancel {\text{hour}}}}}\times {\frac {1609.344{\text
      { meter}}}{1\ {\cancel {\text{mile}}}}}\times {\frac {1\ {\cancel {\text
      {hour}}}}{3600{\text{ second}}}}=4.4704\ {\frac {\text{meter}}{\text
      {second}}}.}]
Each conversion factor is chosen based on the relationship between one of the
original units and one of the desired units (or some intermediary unit), before
being re-arranged to create a factor that cancels out the original unit. For
example, as "mile" is the numerator in the original fraction and     1 &#xA0;
mile  = 1609.344 &#xA0;  meter    {\displaystyle 1\ {\text{mile}}=1609.344\
{\text{meter}}}  [{\displaystyle 1\ {\text{mile}}=1609.344\ {\text{meter}}}],
"mile" will need to be the denominator in the conversion factor. Dividing both
sides of the equation by 1 mile yields        1 &#xA0;  mile    1 &#xA0;  mile
=    1609.344 &#xA0;  meter    1 &#xA0;  mile       {\displaystyle {\frac {1\
{\text{mile}}}{1\ {\text{mile}}}}={\frac {1609.344\ {\text{meter}}}{1\ {\text
{mile}}}}}  [{\displaystyle {\frac {1\ {\text{mile}}}{1\ {\text{mile}}}}={\frac
{1609.344\ {\text{meter}}}{1\ {\text{mile}}}}}], which when simplified results
in the dimensionless     1 =    1609.344 &#xA0;  meter    1 &#xA0;  mile
{\displaystyle 1={\frac {1609.344\ {\text{meter}}}{1\ {\text{mile}}}}}  [
{\displaystyle 1={\frac {1609.344\ {\text{meter}}}{1\ {\text{mile}}}}}].
Multiplying any quantity (physical quantity or not) by the dimensionless 1 does
not change that quantity. Once this and the conversion factor for seconds per
hour have been multiplied by the original fraction to cancel out the units mile
and hour, 10 miles per hour converts to 4.4704 meters per second.
As a more complex example, the concentration of nitrogen_oxides (i.e., ______NO
x______{\displaystyle_\color_{Blue}{\ce_{NO}}_{x}}__[{\displaystyle_\color_
{Blue}{\ce_{NO}}_{x}}]) in the flue_gas from an industrial furnace can be
converted to a mass_flow_rate expressed in grams per hour (i.e., g/h) of
NO   x     {\displaystyle {\ce {NO}}_{x}}  [{\displaystyle {\ce {NO}}_{x}}] by
using the following information as shown below:
  NOx concentration 
      = 10 parts_per_million by volume = 10 ppmv = 10 volumes/106 volumes
  NOx molar mass 
      = 46 kg/kmol = 46 g/mol
  Flow rate of flue gas 
      = 20 cubic meters per minute = 20 m3/min
      The flue gas exits the furnace at 0 Â°C temperature and 101.325 kPa
      absolute pressure.
      The molar_volume of a gas at 0 Â°C temperature and 101.325 kPa is 22.414
      m3/kmol.
            1000 &#xA0;   g &#xA0; NO   x     1     kg &#xA0; NO   x
      &#x00D7;    46 &#xA0;     kg &#xA0; NO   x       1 &#xA0;     kmol &#xA0;
      NO   x        &#x00D7;    1 &#xA0;     kmol &#xA0; NO   x       22.414
      &#xA0;     m   3   &#xA0;   NO   x        &#x00D7;    10 &#xA0;     m   3
      &#xA0;   NO   x        10  6   &#xA0;     m   3   &#xA0;  gas
      &#x00D7;    20 &#xA0;     m   3   &#xA0;  gas      1 &#xA0;   minute
      &#x00D7;    60 &#xA0;   minute     1 &#xA0;  hour     = 24.63 &#xA0;
      g &#xA0; NO   x   hour     {\displaystyle {\frac {1000\ {\ce {g\ NO}}_
      {x}}{1{\cancel {{\ce {kg\ NO}}_{x}}}}}\times {\frac {46\ {\cancel {{\ce
      {kg\ NO}}_{x}}}}{1\ {\cancel {{\ce {kmol\ NO}}_{x}}}}}\times {\frac {1\
      {\cancel {{\ce {kmol\ NO}}_{x}}}}{22.414\ {\cancel {{\ce {m}}^{3}\ {\ce
      {NO}}_{x}}}}}\times {\frac {10\ {\cancel {{\ce {m}}^{3}\ {\ce {NO}}_
      {x}}}}{10^{6}\ {\cancel {{\ce {m}}^{3}\ {\ce {gas}}}}}}\times {\frac {20\
      {\cancel {{\ce {m}}^{3}\ {\ce {gas}}}}}{1\ {\cancel {\ce
      {minute}}}}}\times {\frac {60\ {\cancel {\ce {minute}}}}{1\ {\ce
      {hour}}}}=24.63\ {\frac {{\ce {g\ NO}}_{x}}{\ce {hour}}}}  [
      {\displaystyle {\frac {1000\ {\ce {g\ NO}}_{x}}{1{\cancel {{\ce {kg\
      NO}}_{x}}}}}\times {\frac {46\ {\cancel {{\ce {kg\ NO}}_{x}}}}{1\
      {\cancel {{\ce {kmol\ NO}}_{x}}}}}\times {\frac {1\ {\cancel {{\ce {kmol\
      NO}}_{x}}}}{22.414\ {\cancel {{\ce {m}}^{3}\ {\ce {NO}}_{x}}}}}\times
      {\frac {10\ {\cancel {{\ce {m}}^{3}\ {\ce {NO}}_{x}}}}{10^{6}\ {\cancel {
      {\ce {m}}^{3}\ {\ce {gas}}}}}}\times {\frac {20\ {\cancel {{\ce {m}}^{3}\
      {\ce {gas}}}}}{1\ {\cancel {\ce {minute}}}}}\times {\frac {60\ {\cancel
      {\ce {minute}}}}{1\ {\ce {hour}}}}=24.63\ {\frac {{\ce {g\ NO}}_{x}}{\ce
      {hour}}}}]
After canceling out any dimensional units that appear both in the numerators
and denominators of the fractions in the above equation, the NOx concentration
of 10 ppmv converts to mass flow rate of 24.63 grams per hour.
**** Checking equations that involve dimensions[edit] ****
The factor-label method can also be used on any mathematical equation to check
whether or not the dimensional units on the left hand side of the equation are
the same as the dimensional units on the right hand side of the equation.
Having the same units on both sides of an equation does not ensure that the
equation is correct, but having different units on the two sides (when
expressed in terms of base units) of an equation implies that the equation is
wrong.
For example, check the Universal_Gas_Law equation of PV = nRT, when:
    * the pressure P is in pascals (Pa)
    * the volume V is in cubic meters (m3)
    * the amount of substance n is in moles (mol)
    * the universal_gas_law_constant_R is 8.3145 Paâm3/(molâK)
    * the temperature T is in kelvins (K)
          Pa &#x22C5;  m  3    =     mol   1   &#x00D7;    Pa &#x22C5;  m  3
      mol    &#xA0;    K       &#x00D7;     K   1     {\displaystyle {\ce
      {Pa.m^3}}={\frac {\cancel {{\ce {mol}}}}{1}}\times {\frac {{\ce
      {Pa.m^3}}}{{\cancel {{\ce {mol}}}}\ {\cancel {{\ce {K}}}}}}\times {\frac
      {\cancel {{\ce {K}}}}{1}}}  [{\displaystyle {\ce {Pa.m^3}}={\frac
      {\cancel {{\ce {mol}}}}{1}}\times {\frac {{\ce {Pa.m^3}}}{{\cancel {{\ce
      {mol}}}}\ {\cancel {{\ce {K}}}}}}\times {\frac {\cancel {{\ce {K}}}}
      {1}}}]
As can be seen, when the dimensional units appearing in the numerator and
denominator of the equation's right hand side are cancelled out, both sides of
the equation have the same dimensional units. Dimensional analysis can be used
as a tool to construct equations that relate non-associated physico-chemical
properties. The equations may reveal hitherto unknown or overlooked properties
of matter, in the form of left-over dimensions â dimensional adjusters â
that can then be assigned physical significance. It is important to point out
that such âmathematical manipulationâ is neither without prior precedent,
nor without considerable scientific significance, indeed, the Planckâs
constant; a fundamental constant of the universe, was âdiscoveredâ as a
purely mathematical abstraction or representation that built on the Rayleigh-
Jeans Equation for preventing the ultraviolet catastrophe. It was assigned and
ascended to its quantum physical significance either in tandem or post
mathematical dimensional adjustment â not earlier.
**** Limitations[edit] ****
The factor-label method can convert only unit quantities for which the units
are in a linear relationship intersecting at 0. Most units fit this paradigm.
An example for which it cannot be used is the conversion between degrees
Celsius and kelvins (or degrees_Fahrenheit). Between degrees Celsius and
kelvins, there is a constant difference rather than a constant ratio, while
between degrees Celsius and degrees Fahrenheit there is neither a constant
difference nor a constant ratio. There is, however, an affine_transform (    x
&#x21A6; a x + b   {\displaystyle x\mapsto ax+b}  [x\mapsto ax+b], rather than
a linear_transform     x &#x21A6; a x   {\displaystyle x\mapsto ax}  [x\mapsto
ax]) between them.
For example, the freezing point of water is 0 Â°C and 32 Â°F, and a 5 Â°C
change is the same as a 9 Â°F change. Thus, to convert from units of Fahrenheit
to units of Celsius, one subtracts 32 Â°F (the offset from the point of
reference), divides by 9 Â°F and multiplies by 5 Â°C (scales by the ratio of
units), and adds 0 Â°C (the offset from the point of reference). Reversing this
yields the formula for obtaining a quantity in units of Celsius from units of
Fahrenheit; one could have started with the equivalence between 100 Â°C and
212 Â°F, though this would yield the same formula at the end.
Hence, to convert the numerical quantity value of a temperature T[F] in degrees
Fahrenheit to a numerical quantity value T[C] in degrees Celsius, this formula
may be used:
      T[C] = (T[F] â 32) Ã 5/9.
To convert T[C] in degrees Celsius to T[F] in degrees Fahrenheit, this formula
may be used:
      T[F] = (T[C] Ã 9/5) + 32.
***** Applications[edit] *****
Dimensional analysis is most often used in physics and chemistry â and in the
mathematics thereof â but finds some applications outside of those fields as
well.
**** Mathematics[edit] ****
A simple application of dimensional analysis to mathematics is in computing the
form of the volume_of_an_n-ball (the solid ball in n dimensions), or the area
of its surface, the n-sphere: being an n-dimensional figure, the volume scales
as      x  n   ,   {\displaystyle x^{n},}  [x^{n},] while the surface area,
being     ( n &#x2212; 1 )   {\displaystyle (n-1)}  [(n-1)]-dimensional, scales
as      x  n &#x2212; 1   .   {\displaystyle x^{n-1}.}  [x^{n-1}.] Thus the
volume of the n-ball in terms of the radius is      C  n    r  n   ,
{\displaystyle C_{n}r^{n},}  [C_{n}r^{n},] for some constant      C  n   .
{\displaystyle C_{n}.}  [C_{n}.] Determining the constant takes more involved
mathematics, but the form can be deduced and checked by dimensional analysis
alone.
**** Finance, economics, and accounting[edit] ****
In finance, economics, and accounting, dimensional analysis is most commonly
referred to in terms of the distinction_between_stocks_and_flows. More
generally, dimensional analysis is used in interpreting various financial
ratios, economics ratios, and accounting ratios.
    * For example, the P/E_ratio has dimensions of time (units of years), and
      can be interpreted as "years of earnings to earn the price paid".
    * In economics, debt-to-GDP_ratio also has units of years (debt has units
      of currency, GDP has units of currency/year).
    * More surprisingly, bond_duration also has units of years, which can be
      shown by dimensional analysis, but takes some financial intuition to
      understand.
    * Velocity_of_money has units of 1/years (GDP/money supply has units of
      currency/year over currency): how often a unit of currency circulates per
      year.
    * Interest rates are often expressed as a percentage, but more properly
      percent per annum, which has dimensions of 1/years.
**** Fluid mechanics[edit] ****
In fluid mechanics, dimensional analysis is performed in order to obtain
dimensionless Pi_terms or groups. According to the principles of dimensional
analysis, any prototype can be described by a series of these terms or groups
that describe the behaviour of the system. Using suitable Pi terms or groups,
it is possible to develop a similar set of Pi terms for a model that has the
same dimensional relationships.[8] In other words, Pi terms provide a shortcut
to developing a model representing a certain prototype. Common dimensionless
groups in fluid mechanics include:
    * Reynolds_number (Re), generally important in all types of fluid problems:
                R e  =    &#x03C1;  V d  &#x03BC;     {\displaystyle \mathrm
            {Re} ={\frac {\rho \,Vd}{\mu }}}  [{\displaystyle \mathrm {Re} =
            {\frac {\rho \,Vd}{\mu }}}].
    * Froude_number (Fr), modeling flow with a free surface:
                F r  =   V  g  L    .   {\displaystyle \mathrm {Fr} ={\frac {V}
            {\sqrt {g\,L}}}.}  [{\displaystyle \mathrm {Fr} ={\frac {V}{\sqrt
            {g\,L}}}.}]
    * Euler_number (Eu), used in problems in which pressure is of interest:
                E u  =    &#x0394; p   &#x03C1;  V  2      .   {\displaystyle
            \mathrm {Eu} ={\frac {\Delta p}{\rho V^{2}}}.}  [{\displaystyle
            \mathrm {Eu} ={\frac {\Delta p}{\rho V^{2}}}.}]
    * Mach_number (M), important high speed flows where the velocity approaches
      or exceeds the local speed of sound:
                M  =   V c   ,   {\displaystyle \mathrm {M} ={\frac {V}{c}},}
            [{\displaystyle \mathrm {M} ={\frac {V}{c}},}] where: c is the
            local speed of sound.
***** History[edit] *****
The origins of dimensional analysis have been disputed by historians.[9][10]
The 19th-century French mathematician Joseph_Fourier is generally credited with
having made important contributions[11] based on the idea that physical laws
like F_=_ma should be independent of the units employed to measure the physical
variables. This led to the conclusion that meaningful laws must be homogeneous
equations in their various units of measurement, a result which was eventually
formalized in the Buckingham_Ï_theorem. However, the first application of
dimensional analysis has been credited to the Italian scholar FranÃ§ois_Daviet
de_Foncenex (1734â1799). It was published in 1761, 61 years before the
publication of Fourier's work.[10]
James_Clerk_Maxwell played a major role in establishing modern use of
dimensional analysis by distinguishing mass, length, and time as fundamental
units, while referring to other units as derived.[12] Although Maxwell defined
length, time and mass to be "the three fundamental units", he also noted that
gravitational mass can be derived from length and time by assuming a form of
Newton's_law_of_universal_gravitation in which the gravitational_constant G is
taken as unity, thereby defining M = L3Tâ2.[13] By assuming a form of
Coulomb's_law in which Coulomb's_constant ke is taken as unity, Maxwell then
determined that the dimensions of an electrostatic unit of charge were Q = L3/
2M1/2Tâ1,[14] which, after substituting his M = L3Tâ2 equation for mass,
results in charge having the same dimensions as mass, viz. Q = L3Tâ2.
Dimensional analysis is also used to derive relationships between the physical
quantities that are involved in a particular phenomenon that one wishes to
understand and characterize. It was used for the first time (Pesic_2005) in
this way in 1872 by Lord_Rayleigh, who was trying to understand why the sky is
blue. Rayleigh first published the technique in his 1877 book The Theory of
Sound.[15]
The original meaning of the word dimension, in Fourier's Theorie de la Chaleur,
was the numerical value of the exponents of the base units. For example,
acceleration was considered to have the dimension 1 with respect to the unit of
length, and the dimension â2 with respect to the unit of time.[16] This was
slightly changed by Maxwell, who said the dimensions of acceleration are
LTâ2, instead of just the exponents.[17]
***** Mathematical examples[edit] *****
The Buckingham_Ï_theorem describes how every physically meaningful equation
involving n variables can be equivalently rewritten as an equation of n â m
dimensionless parameters, where m is the rank of the dimensional matrix.
Furthermore, and most importantly, it provides a method for computing these
dimensionless parameters from the given variables.
A dimensional equation can have the dimensions reduced or eliminated through
nondimensionalization, which begins with dimensional analysis, and involves
scaling quantities by characteristic_units of a system or natural_units of
nature. This gives insight into the fundamental properties of the system, as
illustrated in the examples below.
**** Definition[edit] ****
The dimension of a physical_quantity can be expressed as a product of the basic
physical dimensions such as length, mass and time, each raised to a rational
power. The dimension of a physical quantity is more fundamental than some scale
unit used to express the amount of that physical quantity. For example, mass is
a dimension, while the kilogram is a particular scale unit chosen to express a
quantity of mass. Except for natural_units, the choice of scale is cultural and
arbitrary.
There are many possible choices of basic physical dimensions. The SI_standard
recommends the usage of the following dimensions and corresponding symbols:
length (L), mass (M), time (T), electric_current (I), absolute_temperature
(Î), amount_of_substance (N) and luminous_intensity (J). The symbols are by
convention usually written in roman sans_serif typeface.[18] Mathematically,
the dimension of the quantity Q is given by
          dim  &#xA0;  Q  =    L    a      M    b      T    c      I    d
      &#x0398;    e      N    f      J    g     {\displaystyle {\text{dim}}~
      {Q}={\mathsf {L}}^{a}{\mathsf {M}}^{b}{\mathsf {T}}^{c}{\mathsf {I}}^{d}
      {\mathsf {\Theta }}^{e}{\mathsf {N}}^{f}{\mathsf {J}}^{g}}  [
      {\displaystyle {\text{dim}}~{Q}={\mathsf {L}}^{a}{\mathsf {M}}^{b}
      {\mathsf {T}}^{c}{\mathsf {I}}^{d}{\mathsf {\Theta }}^{e}{\mathsf {N}}^
      {f}{\mathsf {J}}^{g}}]
where a, b, c, d, e, f, g are the dimensional exponents. Other physical
quantities could be defined as the base quantities, as long as they form a
linearly_independent basis. For instance, one could replace the dimension of
electrical_current (I) of the SI basis with a dimension of electric_charge (Q),
since Q = IT.
As examples, the dimension of the physical quantity speed v is
          dim  &#xA0; v =   length time   =    L   T    =    L T    &#x2212; 1
      {\displaystyle {\text{dim}}~v={\frac {\text{length}}{\text{time}}}={\frac
      {\mathsf {L}}{\mathsf {T}}}={\mathsf {LT}}^{-1}}  [{\displaystyle {\text
      {dim}}~v={\frac {\text{length}}{\text{time}}}={\frac {\mathsf {L}}
      {\mathsf {T}}}={\mathsf {LT}}^{-1}}]
and the dimension of the physical quantity force F is
          dim  &#xA0; F =  mass  &#x00D7;  acceleration  =  mass  &#x00D7;
      length   time   2     =    M L     T    2     =    M L T    &#x2212; 2
      {\displaystyle {\text{dim}}~F={\text{mass}}\times {\text{acceleration}}=
      {\text{mass}}\times {\frac {\text{length}}{{\text{time}}^{2}}}={\frac
      {\mathsf {ML}}{{\mathsf {T}}^{2}}}={\mathsf {MLT}}^{-2}}  [{\displaystyle
      {\text{dim}}~F={\text{mass}}\times {\text{acceleration}}={\text
      {mass}}\times {\frac {\text{length}}{{\text{time}}^{2}}}={\frac {\mathsf
      {ML}}{{\mathsf {T}}^{2}}}={\mathsf {MLT}}^{-2}}]
The unit chosen to express a physical quantity and its dimension are related,
but not identical concepts. The units of a physical quantity are defined by
convention and related to some standard; e.g., length may have units of metres,
feet, inches, miles or micrometres; but any length always has a dimension of L,
no matter what units of length are chosen to express it. Two different units of
the same physical quantity have conversion_factors that relate them. For
example, 1 in = 2.54 cm; in this case (2.54 cm/in) is the conversion factor,
which is itself dimensionless. Therefore, multiplying by that conversion factor
does not change the dimensions of a physical quantity.
There are also physicists that have cast doubt on the very existence of
incompatible fundamental dimensions of physical quantity,[19] although this
does not invalidate the usefulness of dimensional analysis.
**** Mathematical properties[edit] ****
Main article: Buckingham_Ï_theorem
The dimensions that can be formed from a given collection of basic physical
dimensions, such as M, L, and T, form an abelian_group: The identity is written
as 1; L0 = 1, and the inverse to L is 1/L or Lâ1. L raised to any rational
power p is a member of the group, having an inverse of Lâp or 1/Lp. The
operation of the group is multiplication, having the usual rules for handling
exponents (Ln Ã Lm = Ln+m).
This group can be described as a vector_space over the rational numbers, with
for example dimensional symbol MiLjTk corresponding to the vector (i, j, k).
When physical measured quantities (be they like-dimensioned or unlike-
dimensioned) are multiplied or divided by one other, their dimensional units
are likewise multiplied or divided; this corresponds to addition or subtraction
in the vector space. When measurable quantities are raised to a rational power,
the same is done to the dimensional symbols attached to those quantities; this
corresponds to scalar_multiplication in the vector space.
A basis for such a vector space of dimensional symbols is called a set of base
quantities, and all other vectors are called derived units. As in any vector
space, one may choose different bases, which yields different systems of units
(e.g., choosing whether the unit for charge is derived from the unit for
current, or vice versa).
The group identity 1, the dimension of dimensionless quantities, corresponds to
the origin in this vector space.
The set of units of the physical quantities involved in a problem correspond to
a set of vectors (or a matrix). The nullity describes some number (e.g., m) of
ways in which these vectors can be combined to produce a zero vector. These
correspond to producing (from the measurements) a number of dimensionless
quantities, {Ï1, ..., Ïm}. (In fact these ways completely span the null
subspace of another different space, of powers of the measurements.) Every
possible way of multiplying (and exponentiating) together the measured
quantities to produce something with the same units as some derived quantity X
can be expressed in the general form
         X =  &#x220F;  i = 1   m   (  &#x03C0;  i    )   k  i      .
      {\displaystyle X=\prod _{i=1}^{m}(\pi _{i})^{k_{i}}\,.}  [X=\prod _{i=1}^
      {m}(\pi _{i})^{k_{i}}\,.]
Consequently, every possible commensurate equation for the physics of the
system can be rewritten in the form
         f (  &#x03C0;  1   ,  &#x03C0;  2   , . . . ,  &#x03C0;  m   ) = 0  .
      {\displaystyle f(\pi _{1},\pi _{2},...,\pi _{m})=0\,.}  [f(\pi _{1},\pi _
      {2},...,\pi _{m})=0\,.]
Knowing this restriction can be a powerful tool for obtaining new insight into
the system.
**** Mechanics[edit] ****
The dimension of physical quantities of interest in mechanics can be expressed
in terms of base dimensions M, L, and T â these form a 3-dimensional vector
space. This is not the only valid choice of base dimensions, but it is the one
most commonly used. For example, one might choose force, length and mass as the
base dimensions (as some have done), with associated dimensions F, L, M; this
corresponds to a different basis, and one may convert between these
representations by a change_of_basis. The choice of the base set of dimensions
is thus a convention, with the benefit of increased utility and familiarity.
The choice of base dimensions is not arbitrary, because the dimensions must
form a basis: they must span the space, and be linearly_independent.
For example, F, L, M form a set of fundamental dimensions because they form a
basis that is equivalent to M, L, T: the former can be expressed as [F = ML/
T2], L, M, while the latter can be expressed as M, L, [T = (ML/F)1/2].
On the other hand, length, velocity and time (L, V, T) do not form a set of as
base dimensions, for two reasons:
    * There is no way to obtain mass â or anything derived from it, such as
      force â without introducing another base dimension (thus, they do not
      span the space).
    * Velocity, being expressible in terms of length and time (V = L/T), is
      redundant (the set is not linearly independent).
**** Other fields of physics and chemistry[edit] ****
Depending on the field of physics, it may be advantageous to choose one or
another extended set of dimensional symbols. In electromagnetism, for example,
it may be useful to use dimensions of M, L, T, and Q, where Q represents the
dimension of electric_charge. In thermodynamics, the base set of dimensions is
often extended to include a dimension for temperature, Î. In chemistry, the
amount_of_substance (the number of molecules divided by the Avogadro_constant,
â 6.02Ã1023 molâ1) is defined as a base dimension, N, as well. In the
interaction of relativistic_plasma with strong laser pulses, a dimensionless
relativistic_similarity_parameter, connected with the symmetry properties of
the collisionless Vlasov_equation, is constructed from the plasma-, electron-
and critical-densities in addition to the electromagnetic vector potential. The
choice of the dimensions or even the number of dimensions to be used in
different fields of physics is to some extent arbitrary, but consistency in use
and ease of communications are common and necessary features.
**** Polynomials and transcendental functions[edit] ****
Scalar arguments to transcendental_functions such as exponential, trigonometric
and logarithmic functions, or to inhomogeneous_polynomials, must be
dimensionless_quantities. (Note: this requirement is somewhat relaxed in
Siano's orientational analysis described below, in which the square of certain
dimensioned quantities are dimensionless.)
While most mathematical identities about dimensionless numbers translate in a
straightforward manner to dimensional quantities, care must be taken with
logarithms of ratios: the identity log(a/b) = log a â log b, where the
logarithm is taken in any base, holds for dimensionless numbers a and b, but it
does not hold if a and b are dimensional, because in this case the left-hand
side is well-defined but the right-hand side is not.
Similarly, while one can evaluate monomials (xn) of dimensional quantities, one
cannot evaluate polynomials of mixed degree with dimensionless coefficients on
dimensional quantities: for x2, the expression (3 m)2 = 9 m2 makes sense (as an
area), while for x2 + x, the expression (3 m)2 + 3 m = 9 m2 + 3 m does not make
sense.
However, polynomials of mixed degree can make sense if the coefficients are
suitably chosen physical quantities that are not dimensionless. For example,
           1 2   &#x22C5;  (  &#x2212; 32 &#xA0;   foot   second   2      )
      &#x22C5;  t  2   +  (  500 &#xA0;   foot second    )  &#x22C5; t .
      {\displaystyle {\frac {1}{2}}\cdot \left(-32\ {\frac {\text{foot}}{{\text
      {second}}^{2}}}\right)\cdot t^{2}+\left(500\ {\frac {\text{foot}}{\text
      {second}}}\right)\cdot t.}  [{\displaystyle {\frac {1}{2}}\cdot \left(-
      32\ {\frac {\text{foot}}{{\text{second}}^{2}}}\right)\cdot t^{2}+\left
      (500\ {\frac {\text{foot}}{\text{second}}}\right)\cdot t.}]
This is the height to which an object rises in time t if the acceleration of
gravity is 32 feet per second per second and the initial upward speed is
500 feet per second. It is not even necessary for t to be in seconds. For
example, suppose t = 0.01 minutes. Then the first term would be
                1 2   &#x22C5;  (  &#x2212; 32 &#xA0;   foot   second   2
      )  &#x22C5; ( 0.01  &#xA0;minute   )  2       =       1 2   &#x22C5;
      &#x2212; 32 &#x22C5;  (  0.01  2   )    (   minute second   )   2
      &#x22C5;  foot      =       1 2   &#x22C5; &#x2212; 32 &#x22C5;  (  0.01
      2   )  &#x22C5;  60  2   &#x22C5;  foot  .       {\displaystyle {\begin
      {aligned}&{\frac {1}{2}}\cdot \left(-32\ {\frac {\text{foot}}{{\text
      {second}}^{2}}}\right)\cdot (0.01{\text{ minute}})^{2}\\[10pt]={}&{\frac
      {1}{2}}\cdot -32\cdot \left(0.01^{2}\right)\left({\frac {\text{minute}}
      {\text{second}}}\right)^{2}\cdot {\text{foot}}\\[10pt]={}&{\frac {1}
      {2}}\cdot -32\cdot \left(0.01^{2}\right)\cdot 60^{2}\cdot {\text
      {foot}}.\end{aligned}}}  [{\displaystyle {\begin{aligned}&{\frac {1}
      {2}}\cdot \left(-32\ {\frac {\text{foot}}{{\text{second}}^
      {2}}}\right)\cdot (0.01{\text{ minute}})^{2}\\[10pt]={}&{\frac {1}
      {2}}\cdot -32\cdot \left(0.01^{2}\right)\left({\frac {\text{minute}}
      {\text{second}}}\right)^{2}\cdot {\text{foot}}\\[10pt]={}&{\frac {1}
      {2}}\cdot -32\cdot \left(0.01^{2}\right)\cdot 60^{2}\cdot {\text
      {foot}}.\end{aligned}}}]
**** Incorporating units[edit] ****
The value of a dimensional physical quantity Z is written as the product of a
unit [Z] within the dimension and a dimensionless numerical factor, n.[20]
         Z = n &#x00D7; [ Z ] = n [ Z ]   {\displaystyle Z=n\times [Z]=n[Z]}
      [Z=n\times [Z]=n[Z]]
When like-dimensioned quantities are added or subtracted or compared, it is
convenient to express them in consistent units so that the numerical values of
these quantities may be directly added or subtracted. But, in concept, there is
no problem adding quantities of the same dimension expressed in different
units. For example, 1 meter added to 1 foot is a length, but one cannot derive
that length by simply adding 1 and 1. A conversion_factor, which is a ratio of
like-dimensioned quantities and is equal to the dimensionless unity, is needed:
         1 &#xA0;   ft   = 0.3048 &#xA0;   m   &#xA0;   {\displaystyle 1\
      {\mbox{ft}}=0.3048\ {\mbox{m}}\ }  [1\ {\mbox{ft}}=0.3048\ {\mbox{m}}\ ]
      is identical to     1 =    0.3048 &#xA0;   m     1 &#xA0;   ft      .
      &#xA0;   {\displaystyle 1={\frac {0.3048\ {\mbox{m}}}{1\ {\mbox{ft}}}}.\
      }  [1={\frac {0.3048\ {\mbox{m}}}{1\ {\mbox{ft}}}}.\ ]
The factor     0.3048 &#xA0;    m   ft      {\displaystyle 0.3048\ {\frac
{\mbox{m}}{\mbox{ft}}}}  [0.3048\ {\frac {\mbox{m}}{\mbox{ft}}}] is identical
to the dimensionless 1, so multiplying by this conversion factor changes
nothing. Then when adding two quantities of like dimension, but expressed in
different units, the appropriate conversion factor, which is essentially the
dimensionless 1, is used to convert the quantities to identical units so that
their numerical values can be added or subtracted.
Only in this manner is it meaningful to speak of adding like-dimensioned
quantities of differing units.
**** Position vs displacement[edit] ****
Main article: Affine_space
Some discussions of dimensional analysis implicitly describe all quantities as
mathematical vectors. (In mathematics scalars are considered a special case of
vectors[citation_needed]; vectors can be added to or subtracted from other
vectors, and, inter alia, multiplied or divided by scalars. If a vector is used
to define a position, this assumes an implicit point of reference: an origin.
While this is useful and often perfectly adequate, allowing many important
errors to be caught, it can fail to model certain aspects of physics. A more
rigorous approach requires distinguishing between position and displacement (or
moment in time versus duration, or absolute temperature versus temperature
change).
Consider points on a line, each with a position with respect to a given origin,
and distances among them. Positions and displacements all have units of length,
but their meaning is not interchangeable:
    * adding two displacements should yield a new displacement (walking ten
      paces then twenty paces gets you thirty paces forward),
    * adding a displacement to a position should yield a new position (walking
      one block down the street from an intersection gets you to the next
      intersection),
    * subtracting two positions should yield a displacement,
    * but one may not add two positions.
This illustrates the subtle distinction between affine quantities (ones modeled
by an affine_space, such as position) and vector quantities (ones modeled by a
vector_space, such as displacement).
    * Vector quantities may be added to each other, yielding a new vector
      quantity, and a vector quantity may be added to a suitable affine
      quantity (a vector space acts_on an affine space), yielding a new affine
      quantity.
    * Affine quantities cannot be added, but may be subtracted, yielding
      relative quantities which are vectors, and these relative differences may
      then be added to each other or to an affine quantity.
Properly then, positions have dimension of affine length, while displacements
have dimension of vector length. To assign a number to an affine unit, one must
not only choose a unit of measurement, but also a point_of_reference, while to
assign a number to a vector unit only requires a unit of measurement.
Thus some physical quantities are better modeled by vectorial quantities while
others tend to require affine representation, and the distinction is reflected
in their dimensional analysis.
This distinction is particularly important in the case of temperature, for
which the numeric value of absolute_zero is not the origin 0 in some scales.
For absolute zero,
      0 K = â273.15 Â°C = â459.67 Â°F = 0 Â°R,
but for temperature differences,
      1 K = 1 Â°C â  1 Â°F = 1 Â°R.
(Here Â°R refers to the Rankine_scale, not the RÃ©aumur_scale). Unit conversion
for temperature differences is simply a matter of multiplying by, e.g., 1 Â°F /
1 K (although the ratio is not a constant value). But because some of these
scales have origins that do not correspond to absolute zero, conversion from
one temperature scale to another requires accounting for that. As a result,
simple dimensional analysis can lead to errors if it is ambiguous whether 1 K
means the absolute temperature equal to â272.15 Â°C, or the temperature
difference equal to 1 Â°C.
**** Orientation and frame of reference[edit] ****
Similar to the issue of a point of reference is the issue of orientation: a
displacement in 2 or 3 dimensions is not just a length, but is a length
together with a direction. (This issue does not arise in 1 dimension, or rather
is equivalent to the distinction between positive and negative.) Thus, to
compare or combine two dimensional quantities in a multi-dimensional space, one
also needs an orientation: they need to be compared to a frame_of_reference.
This leads to the extensions discussed below, namely Huntley's directed
dimensions and Siano's orientational analysis.
***** Examples[edit] *****
**** A simple example: period of a harmonic oscillator[edit] ****
What is the period of oscillation T of a mass m attached to an ideal linear
spring with spring constant k suspended in gravity of strength g? That period
is the solution for T of some dimensionless equation in the variables T, m, k,
and g. The four quantities have the following dimensions: T [T]; m [M]; k [M/
T2]; and g [L/T2]. From these we can form only one dimensionless product of
powers of our chosen variables,      G  1     {\displaystyle G_{1}}  [G_{1}] =
T  2   k  /  m   {\displaystyle T^{2}k/m}  [T^{2}k/m] [T2 Â· M/T2 / M = 1], and
putting      G  1   = C   {\displaystyle G_{1}=C}  [G_{1}=C] for some
dimensionless constant C gives the dimensionless equation sought. The
dimensionless product of powers of variables is sometimes referred to as a
dimensionless group of variables; here the term "group" means "collection"
rather than mathematical group. They are often called dimensionless_numbers as
well.
Note that the variable g does not occur in the group. It is easy to see that it
is impossible to form a dimensionless product of powers that combines g with k,
m, and T, because g is the only quantity that involves the dimension L. This
implies that in this problem the g is irrelevant. Dimensional analysis can
sometimes yield strong statements about the irrelevance of some quantities in a
problem, or the need for additional parameters. If we have chosen enough
variables to properly describe the problem, then from this argument we can
conclude that the period of the mass on the spring is independent of g: it is
the same on the earth or the moon. The equation demonstrating the existence of
a product of powers for our problem can be written in an entirely equivalent
way:     T = &#x03BA;     m k       {\displaystyle T=\kappa {\sqrt {\tfrac {m}
{k}}}}  [{\displaystyle T=\kappa {\sqrt {\tfrac {m}{k}}}}], for some
dimensionless constant Îº (equal to       C     {\displaystyle {\sqrt {C}}}  [
{\sqrt {C}}] from the original dimensionless equation).
When faced with a case where dimensional analysis rejects a variable (g, here)
that one intuitively expects to belong in a physical description of the
situation, another possibility is that the rejected variable is in fact
relevant, but that some other relevant variable has been omitted, which might
combine with the rejected variable to form a dimensionless quantity. That is,
however, not the case here.
When dimensional analysis yields only one dimensionless group, as here, there
are no unknown functions, and the solution is said to be "complete" â
although it still may involve unknown dimensionless constants, such as Îº.
**** A more complex example: energy of a vibrating wire[edit] ****
Consider the case of a vibrating wire of length â (L) vibrating with an
amplitude A (L). The wire has a linear_density Ï (M/L) and is under tension s
(ML/T2), and we want to know the energy E (ML2/T2) in the wire. Let Ï1 and Ï2
be two dimensionless products of powers of the variables chosen, given by
              &#x03C0;  1      =   E  A s         &#x03C0;  2      =   &#x2113;
      A   .       {\displaystyle {\begin{aligned}\pi _{1}&={\frac {E}{As}}\\\pi
      _{2}&={\frac {\ell }{A}}.\end{aligned}}}  [{\displaystyle {\begin
      {aligned}\pi _{1}&={\frac {E}{As}}\\\pi _{2}&={\frac {\ell }{A}}.\end
      {aligned}}}]
The linear density of the wire is not involved. The two groups found can be
combined into an equivalent form as an equation
         F  (    E  A s    ,   &#x2113; A    )  = 0 ,   {\displaystyle F\left(
      {\frac {E}{As}},{\frac {\ell }{A}}\right)=0,}  [{\displaystyle F\left(
      {\frac {E}{As}},{\frac {\ell }{A}}\right)=0,}]
where F is some unknown function, or, equivalently as
         E = A s f  (   &#x2113; A   )  ,   {\displaystyle E=Asf\left({\frac
      {\ell }{A}}\right),}  [{\displaystyle E=Asf\left({\frac {\ell }
      {A}}\right),}]
where f is some other unknown function. Here the unknown function implies that
our solution is now incomplete, but dimensional analysis has given us something
that may not have been obvious: the energy is proportional to the first power
of the tension. Barring further analytical analysis, we might proceed to
experiments to discover the form for the unknown function f. But our
experiments are simpler than in the absence of dimensional analysis. We'd
perform none to verify that the energy is proportional to the tension. Or
perhaps we might guess that the energy is proportional to â, and so infer
that E = âs. The power of dimensional analysis as an aid to experiment and
forming hypotheses becomes evident.
The power of dimensional analysis really becomes apparent when it is applied to
situations, unlike those given above, that are more complicated, the set of
variables involved are not apparent, and the underlying equations hopelessly
complex. Consider, for example, a small pebble sitting on the bed of a river.
If the river flows fast enough, it will actually raise the pebble and cause it
to flow along with the water. At what critical velocity will this occur?
Sorting out the guessed variables is not so easy as before. But dimensional
analysis can be a powerful aid in understanding problems like this, and is
usually the very first tool to be applied to complex problems where the
underlying equations and constraints are poorly understood. In such cases, the
answer may depend on a dimensionless_number such as the Reynolds_number, which
may be interpreted by dimensional analysis.
**** A third example: demand versus capacity for a rotating disc[edit] ****
Consider the case of a thin, solid, parallel-sided rotating disc of axial
thickness t (L) and radius R (L). The disc has a density Ï (M/L3), rotates at
an angular velocity Ï (Tâ1) and this leads to a stress S (MLâ1Tâ2) in
the material. There is a theoretical linear elastic solution, given by Lame, to
this problem when the disc is thin relative to its radius, the faces of the
disc are free to move axially, and the plane stress constitutive relations can
be assumed to be valid. As the disc becomes thicker relative to the radius then
the plane stress solution breaks down. If the disc is restrained axially on its
free faces then a state of plane strain will occur. However, if this is not the
case then the state of stress may only be determined though consideration of
three-dimensional elasticity and there is no known theoretical solution for
this case. An engineer might, therefore, be interested in establishing a
relationship between the five variables. Dimensional analysis for this case
leads to the following (5 â 3 = 2) non-dimensional groups:
      demand/capacity = ÏR2Ï2/S
      thickness/radius or aspect ratio = t/R
Dimensional analysis and numerical experiments for a rotating disc
Through the use of numerical experiments using, for example, the finite element
method, the nature of the relationship between the two non-dimensional groups
can be obtained as shown in the figure. As this problem only involves two non-
dimensional groups, the complete picture is provided in a single plot and this
can be used as a design/assessment chart for rotating discs[21]
***** Extensions[edit] *****
**** Huntley's extension: directed dimensions[edit] ****
Huntley (Huntley_1967) has pointed out that it is sometimes productive to
refine our concept of dimension. Two possible refinements are:
    * The magnitude of the components of a vector are to be considered
      dimensionally distinct. For example, rather than an undifferentiated
      length dimension L, we may have Lx represent dimension in the x-
      direction, and so forth. This requirement stems ultimately from the
      requirement that each component of a physically meaningful equation
      (scalar, vector, or tensor) must be dimensionally consistent.
    * Mass as a measure of quantity is to be considered dimensionally distinct
      from mass as a measure of inertia.
As an example of the usefulness of the first refinement, suppose we wish to
calculate the distance_a_cannonball_travels when fired with a vertical velocity
component      V   y      {\displaystyle V_{\mathrm {y} }}  [{\displaystyle V_
{\mathrm {y} }}] and a horizontal velocity component      V   x
{\displaystyle V_{\mathrm {x} }}  [{\displaystyle V_{\mathrm {x} }}], assuming
it is fired on a flat surface. Assuming no use of directed lengths, the
quantities of interest are then      V   x      {\displaystyle V_{\mathrm {x}
}}  [{\displaystyle V_{\mathrm {x} }}],      V   y      {\displaystyle V_
{\mathrm {y} }}  [{\displaystyle V_{\mathrm {y} }}], both dimensioned as
LTâ1, R, the distance travelled, having dimension L, and g the downward
acceleration of gravity, with dimension LTâ2.
With these four quantities, we may conclude that the equation for the range R
may be written:
         R &#x221D;  V  x   a     V  y   b     g  c   .    {\displaystyle
      R\propto V_{\text{x}}^{a}\,V_{\text{y}}^{b}\,g^{c}.\,}  [R\propto V_
      {\text{x}}^{a}\,V_{\text{y}}^{b}\,g^{c}.\,]
Or dimensionally
           L   =   (    L   T    )   a + b     (    L     T    2     )   c
      {\displaystyle {\mathsf {L}}=\left({\frac {\mathsf {L}}{\mathsf
      {T}}}\right)^{a+b}\left({\frac {\mathsf {L}}{{\mathsf {T}}^{2}}}\right)^
      {c}\,}  [{\displaystyle {\mathsf {L}}=\left({\frac {\mathsf {L}}{\mathsf
      {T}}}\right)^{a+b}\left({\frac {\mathsf {L}}{{\mathsf {T}}^{2}}}\right)^
      {c}\,}]
from which we may deduce that     a + b + c = 1   {\displaystyle a+b+c=1}  [
{\displaystyle a+b+c=1}] and     a + b + 2 c = 0   {\displaystyle a+b+2c=0}  [
{\displaystyle a+b+2c=0}], which leaves one exponent undetermined. This is to
be expected since we have two fundamental dimensions L and T, and four
parameters, with one equation.
If, however, we use directed length dimensions, then      V   x
{\displaystyle V_{\mathrm {x} }}  [{\displaystyle V_{\mathrm {x} }}] will be
dimensioned as LxTâ1,      V   y      {\displaystyle V_{\mathrm {y} }}  [
{\displaystyle V_{\mathrm {y} }}] as LyTâ1, R as Lx and g as LyTâ2. The
dimensional equation becomes:
            L     x    =   (      L     x     T    )   a     (      L     y
      T    )   b     (      L     y       T    2     )   c     {\displaystyle
      {\mathsf {L}}_{\mathrm {x} }=\left({\frac {{\mathsf {L}}_{\mathrm {x} }}
      {\mathsf {T}}}\right)^{a}\left({\frac {{\mathsf {L}}_{\mathrm {y} }}
      {\mathsf {T}}}\right)^{b}\left({\frac {{\mathsf {L}}_{\mathrm {y} }}{
      {\mathsf {T}}^{2}}}\right)^{c}}  [{\displaystyle {\mathsf {L}}_{\mathrm
      {x} }=\left({\frac {{\mathsf {L}}_{\mathrm {x} }}{\mathsf {T}}}\right)^
      {a}\left({\frac {{\mathsf {L}}_{\mathrm {y} }}{\mathsf {T}}}\right)^
      {b}\left({\frac {{\mathsf {L}}_{\mathrm {y} }}{{\mathsf {T}}^
      {2}}}\right)^{c}}]
and we may solve completely as     a = 1   {\displaystyle a=1}  [a=1],     b =
1   {\displaystyle b=1}  [b=1] and     c = &#x2212; 1   {\displaystyle c=-1}  [
{\displaystyle c=-1}]. The increase in deductive power gained by the use of
directed length dimensions is apparent.
In a similar manner, it is sometimes found useful (e.g., in fluid mechanics and
thermodynamics) to distinguish between mass as a measure of inertia (inertial
mass), and mass as a measure of quantity (substantial mass). For example,
consider the derivation of Poiseuille's_Law. We wish to find the rate of mass
flow of a viscous fluid through a circular pipe. Without drawing distinctions
between inertial and substantial mass we may choose as the relevant variables
    *       m &#x02D9;      {\displaystyle {\dot {m}}}  [{\dot {m}}] the mass
      flow rate with dimension MTâ1
    *     p  x     {\displaystyle p_{\text{x}}}  [p_{\text{x}}] the pressure
      gradient along the pipe with dimension MLâ2Tâ2
    * ρ the density with dimension MLâ3
    * η the dynamic fluid viscosity with dimension MLâ1Tâ1
    * r the radius of the pipe with dimension L
There are three fundamental variables so the above five equations will yield
two dimensionless variables which we may take to be      &#x03C0;  1   =    m
&#x02D9;     /  &#x03B7; r   {\displaystyle \pi _{1}={\dot {m}}/\eta r}  [
{\displaystyle \pi _{1}={\dot {m}}/\eta r}] and      &#x03C0;  2   =  p   x
&#x03C1;  r  5    /      m &#x02D9;     2     {\displaystyle \pi _{2}=p_
{\mathrm {x} }\rho r^{5}/{\dot {m}}^{2}}  [{\displaystyle \pi _{2}=p_{\mathrm
{x} }\rho r^{5}/{\dot {m}}^{2}}] and we may express the dimensional equation as
         C =  &#x03C0;  1    &#x03C0;  2   a   =  (     m &#x02D9;    &#x03B7;
      r    )    (     p   x    &#x03C1;  r  5        m &#x02D9;     2     )   a
      {\displaystyle C=\pi _{1}\pi _{2}^{a}=\left({\frac {\dot {m}}{\eta
      r}}\right)\left({\frac {p_{\mathrm {x} }\rho r^{5}}{{\dot {m}}^
      {2}}}\right)^{a}}  [{\displaystyle C=\pi _{1}\pi _{2}^{a}=\left({\frac
      {\dot {m}}{\eta r}}\right)\left({\frac {p_{\mathrm {x} }\rho r^{5}}{{\dot
      {m}}^{2}}}\right)^{a}}]
where C and a are undetermined constants. If we draw a distinction between
inertial mass with dimension      M  i     {\displaystyle M_{\text{i}}}  [M_
{\text{i}}] and substantial mass with dimension      M  s     {\displaystyle M_
{\text{s}}}  [M_{\text{s}}], then mass flow rate and density will use
substantial mass as the mass parameter, while the pressure gradient and
coefficient of viscosity will use inertial mass. We now have four fundamental
parameters, and one dimensionless constant, so that the dimensional equation
may be written:
         C =     p   x    &#x03C1;  r  4     &#x03B7;    m &#x02D9;
      {\displaystyle C={\frac {p_{\mathrm {x} }\rho r^{4}}{\eta {\dot {m}}}}}
      [{\displaystyle C={\frac {p_{\mathrm {x} }\rho r^{4}}{\eta {\dot {m}}}}}]
where now only C is an undetermined constant (found to be equal to     &#x03C0;
/  8   {\displaystyle \pi /8}  [\pi /8] by methods outside of dimensional
analysis). This equation may be solved for the mass flow rate to yield
Poiseuille's_law.
Huntley's extension has some serious drawbacks:
    * It does not deal well with vector equations involving the cross_product,
    * nor does it handle well the use of angles as physical variables.
It also is often quite difficult to assign the L, Lx, Ly, Lz, symbols to the
physical variables involved in the problem of interest. He invokes a procedure
that involves the "symmetry" of the physical problem. This is often very
difficult to apply reliably: It is unclear as to what parts of the problem that
the notion of "symmetry" is being invoked. Is it the symmetry of the physical
body that forces are acting upon, or to the points, lines or areas at which
forces are being applied? What if more than one body is involved with different
symmetries?
Consider the spherical bubble attached to a cylindrical tube, where one wants
the flow rate of air as a function of the pressure difference in the two parts.
What are the Huntley extended dimensions of the viscosity of the air contained
in the connected parts? What are the extended dimensions of the pressure of the
two parts? Are they the same or different? These difficulties are responsible
for the limited application of Huntley's addition to real problems.
**** Siano's extension: orientational analysis[edit] ****
Angles are, by convention, considered to be dimensionless variables. As an
example, consider again the projectile problem in which a point mass is
launched from the origin (x,y)=(0,0) at a speed v and angle θ above the x-axis,
with the force of gravity directed along the negative y-axis. It is desired to
find the range R, at which point the mass returns to the x-axis. Conventional
analysis will yield the dimensionless variable π=R g/v^2, but offers no insight
into the relationship between R and θ
Siano (1985-I, 1985-II) has suggested that the directed dimensions of Huntley
be replaced by using orientational symbols 1x 1y 1z to denote vector
directions, and an orientationless symbol 10. Thus, Huntley's Lx becomes L 1x
with L specifying the dimension of length, and 1x specifying the orientation.
Siano further shows that the orientational symbols have an algebra of their
own. Along with the requirement that 1iâ1 = 1i, the following multiplication
table for the orientation symbols results:
                1  0        1  x        1  y        1  z          1  0       1
      0      1  x      1  y      1  z         1  x       1  x      1  0      1
      z      1  y         1  y       1  y      1  z      1  0      1  x
      1  z       1  z      1  y      1  x      1  0         {\displaystyle
      {\begin{array}{c|cccc}&\mathbf {1_{0}} &\mathbf {1_{\text{x}}} &\mathbf
      {1_{\text{y}}} &\mathbf {1_{\text{z}}} \\\hline \mathbf {1_{0}} &1_{0}&1_
      {\text{x}}&1_{\text{y}}&1_{\text{z}}\\\mathbf {1_{\text{x}}} &1_{\text
      {x}}&1_{0}&1_{\text{z}}&1_{\text{y}}\\\mathbf {1_{\text{y}}} &1_{\text
      {y}}&1_{\text{z}}&1_{0}&1_{\text{x}}\\\mathbf {1_{\text{z}}} &1_{\text
      {z}}&1_{\text{y}}&1_{\text{x}}&1_{0}\end{array}}}  [{\displaystyle
      {\begin{array}{c|cccc}&\mathbf {1_{0}} &\mathbf {1_{\text{x}}} &\mathbf
      {1_{\text{y}}} &\mathbf {1_{\text{z}}} \\\hline \mathbf {1_{0}} &1_{0}&1_
      {\text{x}}&1_{\text{y}}&1_{\text{z}}\\\mathbf {1_{\text{x}}} &1_{\text
      {x}}&1_{0}&1_{\text{z}}&1_{\text{y}}\\\mathbf {1_{\text{y}}} &1_{\text
      {y}}&1_{\text{z}}&1_{0}&1_{\text{x}}\\\mathbf {1_{\text{z}}} &1_{\text
      {z}}&1_{\text{y}}&1_{\text{x}}&1_{0}\end{array}}}]
Note that the orientational symbols form a group (the Klein_four-group or
"Viergruppe"). In this system, scalars always have the same orientation as the
identity element, independent of the "symmetry of the problem". Physical
quantities that are vectors have the orientation expected: a force or a
velocity in the z-direction has the orientation of 1z. For angles, consider an
angle Î¸ that lies in the z-plane. Form a right triangle in the z-plane with Î¸
being one of the acute angles. The side of the right triangle adjacent to the
angle then has an orientation 1x and the side opposite has an orientation 1y.
Then, since tan(Î¸) = 1y/1x = Î¸ + ... we conclude that an angle in the xy-
plane must have an orientation 1y/1x = 1z, which is not unreasonable. Analogous
reasoning forces the conclusion that sin(Î¸) has orientation 1z while cos(Î¸)
has orientation 10. These are different, so one concludes (correctly), for
example, that there are no solutions of physical equations that are of the form
a cos(Î¸) + b sin(Î¸), where a and b are real scalars. Note that an expression
such as     sin &#x2061; ( &#x03B8; + &#x03C0;  /  2 ) = cos &#x2061;
( &#x03B8; )   {\displaystyle \sin(\theta +\pi /2)=\cos(\theta )}  [\sin(\theta
+\pi /2)=\cos(\theta )] is not dimensionally inconsistent since it is a special
case of the sum of angles formula and should properly be written:
         sin &#x2061;  (  a   1  z   + b   1  z    )  = sin &#x2061;  (  a   1
      z   ) cos &#x2061; ( b   1  z    )  + sin &#x2061;  (  b   1  z   ) cos
      &#x2061; ( a   1  z    )  ,   {\displaystyle \sin \left(a\,1_{\text
      {z}}+b\,1_{\text{z}}\right)=\sin \left(a\,1_{\text{z}})\cos(b\,1_{\text
      {z}}\right)+\sin \left(b\,1_{\text{z}})\cos(a\,1_{\text{z}}\right),}  [
      {\displaystyle \sin \left(a\,1_{\text{z}}+b\,1_{\text{z}}\right)=\sin
      \left(a\,1_{\text{z}})\cos(b\,1_{\text{z}}\right)+\sin \left(b\,1_{\text
      {z}})\cos(a\,1_{\text{z}}\right),}]
which for     a = &#x03B8;   {\displaystyle a=\theta }  [{\displaystyle
a=\theta }] and     b = &#x03C0;  /  2   {\displaystyle b=\pi /2}  [
{\displaystyle b=\pi /2}] yields     sin &#x2061; ( &#x03B8;   1  z   +
[ &#x03C0;  /  2 ]   1  z   ) =  1  z   cos &#x2061; ( &#x03B8;   1  z   )
{\displaystyle \sin(\theta \,1_{\text{z}}+[\pi /2]\,1_{\text{z}})=1_{\text
{z}}\cos(\theta \,1_{\text{z}})}  [{\displaystyle \sin(\theta \,1_{\text{z}}+
[\pi /2]\,1_{\text{z}})=1_{\text{z}}\cos(\theta \,1_{\text{z}})}]. Physical
quantities may be expressed as complex numbers (e.g.      e  i &#x03B8;
{\displaystyle e^{i\theta }}  [e^{i\theta }]) which imply that the complex
quantity i has an orientation equal to that of the angle it is associated with
(1z in the above example).
The assignment of orientational symbols to physical quantities and the
requirement that physical equations be orientationally homogeneous can actually
be used in a way that is similar to dimensional analysis to derive a little
more information about acceptable solutions of physical problems. In this
approach one sets up the dimensional equation and solves it as far as one can.
If the lowest power of a physical variable is fractional, both sides of the
solution is raised to a power such that all powers are integral. This puts it
into "normal form". The orientational equation is then solved to give a more
restrictive condition on the unknown powers of the orientational symbols,
arriving at a solution that is more complete than the one that dimensional
analysis alone gives. Often the added information is that one of the powers of
a certain variable is even or odd.
As an example, for the projectile problem, using orientational symbols, Î¸,
being in the xy-plane will thus have dimension 1z and the range of the
projectile R will be of the form:
         R =  g  a     v  b     &#x03B8;  c    &#xA0;which means&#xA0;    L
      1   x    &#x223C;   (      L     1  y       T    2     )   a     (    L
      T    )   b     1   z    c   .    {\displaystyle R=g^{a}\,v^{b}\,\theta ^
      {c}{\text{ which means }}{\mathsf {L}}\,1_{\mathrm {x} }\sim \left({\frac
      {{\mathsf {L}}\,1_{\text{y}}}{{\mathsf {T}}^{2}}}\right)^{a}\left({\frac
      {\mathsf {L}}{\mathsf {T}}}\right)^{b}\,1_{\mathsf {z}}^{c}.\,}  [
      {\displaystyle R=g^{a}\,v^{b}\,\theta ^{c}{\text{ which means }}{\mathsf
      {L}}\,1_{\mathrm {x} }\sim \left({\frac {{\mathsf {L}}\,1_{\text{y}}}{
      {\mathsf {T}}^{2}}}\right)^{a}\left({\frac {\mathsf {L}}{\mathsf
      {T}}}\right)^{b}\,1_{\mathsf {z}}^{c}.\,}]
Dimensional homogeneity will now correctly yield a = â1 and b = 2, and
orientational homogeneity requires that      1  x    /  (  1  y   a    1  z   c
) =  1  z   c + 1   = 1   {\displaystyle 1_{x}/(1_{y}^{a}1_{z}^{c})=1_{z}^
{c+1}=1}  [{\displaystyle 1_{x}/(1_{y}^{a}1_{z}^{c})=1_{z}^{c+1}=1}]. In other
words that c must be an odd integer. In fact the required function of theta
will be sin(Î¸)cos(Î¸) which is a series of odd powers of Î¸.
It is seen that the Taylor series of sin(Î¸) and cos(Î¸) are orientationally
homogeneous using the above multiplication table, while expressions like cos
(Î¸) + sin(Î¸) and exp(Î¸) are not, and are (correctly) deemed unphysical.
In orientational analysis, the unit of angle is considered to be a base unit,
rather than dimensionless, which will require more careful specification of the
units of physical variables. For example, the question of whether torque and
energy have the same units is answered in the negative. Torque will have
dimensions ML2θ/T while energy will have units ML2/T where θ is a unit of
angular measure (radians, degrees, etc.). Since torque τ is τ=r x p which is
proportional to sin(θ), it can be seen that the units of the cross product of
two physical vectors (i.e. pseudovectors) will be the product of the dimensions
of the two physical vectors times an angular unit.
***** Dimensionless concepts[edit] *****
**** Constants[edit] ****
Main article: Dimensionless_quantity
The dimensionless constants that arise in the results obtained, such as the C
in the Poiseuille's Law problem and the     &#x03BA;   {\displaystyle \kappa }
[\kappa ] in the spring problems discussed above, come from a more detailed
analysis of the underlying physics and often arise from integrating some
differential equation. Dimensional analysis itself has little to say about
these constants, but it is useful to know that they very often have a magnitude
of order unity. This observation can allow one to sometimes make "back_of_the
envelope" calculations about the phenomenon of interest, and therefore be able
to more efficiently design experiments to measure it, or to judge whether it is
important, etc.
**** Formalisms[edit] ****
Paradoxically, dimensional analysis can be a useful tool even if all the
parameters in the underlying theory are dimensionless, e.g., lattice models
such as the Ising_model can be used to study phase transitions and critical
phenomena. Such models can be formulated in a purely dimensionless way. As we
approach the critical point closer and closer, the distance over which the
variables in the lattice model are correlated (the so-called correlation
length,     &#x03BE;   {\displaystyle \xi }  [\xi ] ) becomes larger and
larger. Now, the correlation length is the relevant length scale related to
critical phenomena, so one can, e.g., surmise on "dimensional grounds" that the
non-analytical part of the free energy per lattice site should be     &#x223C;
1  /   &#x03BE;  d     {\displaystyle \sim 1/\xi ^{d}}  [\sim 1/\xi ^{d}] where
d   {\displaystyle d}  [d] is the dimension of the lattice.
It has been argued by some physicists, e.g., M._J._Duff,[19][22] that the laws
of physics are inherently dimensionless. The fact that we have assigned
incompatible dimensions to Length, Time and Mass is, according to this point of
view, just a matter of convention, borne out of the fact that before the advent
of modern physics, there was no way to relate mass, length, and time to each
other. The three independent dimensionful constants: c, Ä§, and G, in the
fundamental equations of physics must then be seen as mere conversion factors
to convert Mass, Time and Length into each other.
Just as in the case of critical properties of lattice models, one can recover
the results of dimensional analysis in the appropriate scaling limit; e.g.,
dimensional analysis in mechanics can be derived by reinserting the constants
Ä§, c, and G (but we can now consider them to be dimensionless) and demanding
that a nonsingular relation between quantities exists in the limit     c
&#x2192; &#x221E;   {\displaystyle c\rightarrow \infty }  [c\rightarrow \infty
],     &#x210F; &#x2192; 0   {\displaystyle \hbar \rightarrow 0}  [\hbar
\rightarrow 0] and     G &#x2192; 0   {\displaystyle G\rightarrow 0}
[G\rightarrow 0]. In problems involving a gravitational field the latter limit
should be taken such that the field stays finite.
***** Dimensional equivalences[edit] *****
Following are tables of commonly occurring expressions in physics, related to
the dimensions of energy, momentum, and force.[23][24][25]
**** SI units[edit] ****
Main article: SI_units
Energy, E       Expression     Nomenclature
ML2Tâ2
                   F d
                {\displaystyle F = force, d = distance
                Fd}  [Fd]
                   S  /  t
                &#x2261; P t
                {\displaystyle S = action, t = time, P = power
                S/t\equiv Pt}
                [S/t\equiv Pt]
                   m  v  2
                &#x2261; p v
                &#x2261;  p  2
                /  m
                {\displaystyle
                mv^{2}\equiv   m = mass, v = velocity, p = momentum
                pv\equiv p^
                {2}/m}  [mv^
Mechanical      {2}\equiv
                pv\equiv p^
                {2}/m]
                   I  &#x03C9;
                2   &#x2261; L
                &#x03C9;
                &#x2261;  L  2
                /  I
                {\displaystyle
                I\omega ^      L = angular_momentum, I = moment_of_inertia, Ï = angular_velocity
                {2}\equiv
                L\omega \equiv
                L^{2}/I}
                [I\omega ^
                {2}\equiv
                L\omega \equiv
                L^{2}/I]
                   p V
                &#x2261; n R T
                &#x2261;  k  B
                T &#x2261; T S
                {\displaystyle p = pressure, T = temperature, S = entropy, kB = boltzmann
Thermal         pV\equiv       constant, R = gas_constant
                nRT\equiv k_
                {B}T\equiv TS}
                [pV\equiv
                nRT\equiv k_
                {B}T\equiv TS]
                   I A t
                &#x2261; S A t
Waves           {\displaystyle I = wave intensity, S = Poynting_vector
                IAt\equiv SAt}
                [IAt\equiv
                SAt]
                   q &#x03D5;
                {\displaystyle q = electric_charge, Ï = electric_potential (for changes this is
                q\phi }        voltage)
                [q\phi ]
                   &#x03B5;  E
                2   V &#x2261;
                B  2   V  /
                &#x03BC;
                {\displaystyle E = electric_field, B = magnetic_field,
                \varepsilon E^ Îµ = permittivity, Î¼ = permeability,
                {2}V\equiv B^  V = 3d volume
                {2}V/\mu }
Electromagnetic [\varepsilon
                E^{2}V\equiv
                B^{2}V/\mu ]
                   p E
                &#x2261; m B
                &#x2261; I A B
                {\displaystyle
                pE\equiv       p = electric_dipole_moment, m = magnetic moment,
                mB\equiv IAB}  A = area (bounded by a current loop), I = electric_current in loop
                [
                {\displaystyle
                pE\equiv
                mB\equiv IAB}]
Momentum, p     Expression                Nomenclature
MLTâ1
                   m v &#x2261; F t       m = mass, v = velocity, F = force, t
                {\displaystyle mv\equiv   = time
                Ft}  [mv\equiv Ft]
Mechanical         S  /  r &#x2261; L  /
                r   {\displaystyle S/     S = action, L = angular momentum, r =
                r\equiv L/r}  [S/r\equiv  displacement
                L/r]
                   m    &#x27E8;  v  2          &#x27E8;  v  2   &#x27E9;
                &#x27E9;                  {\displaystyle {\sqrt {\left\langle
                {\displaystyle m{\sqrt    v^{2}\right\rangle }}}  [
Thermal         {\left\langle v^          {\displaystyle {\sqrt {\left\langle
                {2}\right\rangle }}}  [   v^{2}\right\rangle }}}] = root_mean
                {\displaystyle m{\sqrt    square velocity, m = mass (of a
                {\left\langle v^          molecule)
                {2}\right\rangle }}}]
                   &#x03C1; V v           Ï = density, V = volume, v = phase
Waves           {\displaystyle \rho Vv}   velocity
                [\rho Vv]
Electromagnetic    q A   {\displaystyle   A = magnetic_vector_potential
                qA}  [qA]
Force, F        Expression                      Nomenclature
MLTâ2
                   m a &#x2261; p  /  t
Mechanical      {\displaystyle ma\equiv p/t}    m = mass, a = acceleration
                [ma\equiv p/t]
                   T &#x03B4; S  /  &#x03B4; r  S = entropy, T = temperature, r
Thermal         {\displaystyle T\delta S/\delta = displacement (see entropic
                r}  [T\delta S/\delta r]        force)
                   E q &#x2261; B q v           E = electric field, B =
Electromagnetic {\displaystyle Eq\equiv Bqv}    magnetic field, v = velocity, q
                [Eq\equiv Bqv]                  = charge
**** Natural units[edit] ****
Main article: Natural_units
If c = Ä§ = 1, where c is the speed_of_light and Ä§ is the reduced_Planck
constant, and a suitable fixed unit of energy is chosen, then all quantities of
length L, mass M and time T can be expressed (dimensionally) as a power of
energy E, because length, mass and time can be expressed using speed v, action
S, and energy E:[25]
         M =   E  v  2     ,  L =    S v  E   ,  t =   S E     {\displaystyle
      M={\frac {E}{v^{2}}},\quad L={\frac {Sv}{E}},\quad t={\frac {S}{E}}}  [
      {\displaystyle M={\frac {E}{v^{2}}},\quad L={\frac {Sv}{E}},\quad t=
      {\frac {S}{E}}}]
though speed and action are dimensionless (v = c = 1 and S = Ä§ = 1) â so the
only remaining quantity with dimension is energy. In terms of powers of
dimensions:
            E    n   =    M    p      L    q      T    r   =    E    p &#x2212;
      q &#x2212; r     {\displaystyle {\mathsf {E}}^{n}={\mathsf {M}}^{p}
      {\mathsf {L}}^{q}{\mathsf {T}}^{r}={\mathsf {E}}^{p-q-r}}  [{\mathsf
      {E}}^{n}={\mathsf {M}}^{p}{\mathsf {L}}^{q}{\mathsf {T}}^{r}={\mathsf
      {E}}^{p-q-r}]
This is particularly useful in particle physics and high energy physics, in
which case the energy unit is the electron volt (eV). Dimensional checks and
estimates become very simple in this system.
However, if electric charges and currents are involved, another unit to be
fixed is for electric charge, normally the electron_charge e though other
choices are possible.
Quantity    p, q, r powers of energy n power of energy
            p q r                    n
Action, S   1 2 â1              0
Speed, v    0 1 â1              0
Mass, M     1 0 0                    1
Length, L   0 1 0                    â1
Time, t     0 0 1                    â1
Momentum, p 1 1 â1              1
Energy, E   1 2 â2              1
***** See also[edit] *****
    * Dimensionless_numbers_in_fluid_mechanics
    * Fermi_problem â used to teach dimensional analysis
    * Rayleigh's_method_of_dimensional_analysis
    * Similitude_(model) â an application of dimensional analysis
    * System_of_measurement
    * Buckingham_Ï_theorem
**** Related areas of math[edit] ****
    * Covariance_and_contravariance_of_vectors
    * Exterior_algebra
    * Geometric_algebra
    * Quantity_calculus
***** Notes[edit] *****
   1. ^Goldberg, David (2006). Fundamentals of Chemistry (5th ed.). McGraw-
      Hill. ISBN 978-0-07-322104-5.
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
   3. ^Ogden, James (1999). The Handbook of Chemical Engineering. Research &
      Education Association. ISBN 978-0-87891-982-6.
   4. ^"Dimensional_Analysis_or_the_Factor_Label_Method". Mr Kent's Chemistry
      Page.
   5. ^Fourier, Joseph (1822), Theorie_analytique_de_la_chaleur (in French),
      Paris: Firmin Didot
   6. ^JCGM 200 (2012). International_vocabulary_of_metrology_â_Basic_and
      general_concepts_and_associated_terms_(VIM) (PDF) (3rd ed.). Archived
      from the_original (PDF) on 2015-09-23. Retrieved 2015-06-02.
   7. ^ John Cimbala and Yunus Cengel (2006), Essential of Fluid Mechanics:
      Fundamentals and Applications, McGraw-Hill. Chapter 7: "Dimensional
      Analysis and Modeling", Section 7-2: "Dimensional homogeneity" [1]
   8. ^de Jong, Frits J.; Quade, Wilhelm (1967). Dimensional_analysis_for
      economists. North Holland. p. 28.
   9. ^Waite, Lee; Fine, Jerry (2007). Applied Biofluid Mechanics. New York:
      McGraw-Hill. p. 260. ISBN 978-0-07-147217-3.
  10. ^Macagno, Enzo O. (1971). "Historico-critical review of dimensional
      analysis". Journal of the Franklin Institute. 292 (6): 391â40. doi:
      10.1016/0016-0032(71)90160-8.
  11. ^ a bMartins, Roberto De A. (1981). "The origin of dimensional analysis".
      Journal of the Franklin Institute. 311 (5): 331â7. doi:10.1016/0016-
      0032(81)90475-0.
  12. ^Mason, Stephen Finney (1962), A history of the sciences, New York:
      Collier Books, p. 169, ISBN 978-0-02-093400-4
  13. ^Roche, John J (1998), The Mathematics of Measurement: A Critical
      History, Springer, p. 203, ISBN 978-0-387-91581-4, Beginning_apparently
      with_Maxwell,_mass,_length_and_time_began_to_be_interpreted_as_having_a
      privileged_fundamental_character_and_all_other_quantities_as_derivative,
      not_merely_with_respect_to_measurement,_but_with_respect_to_their
      physical_status_as_well.
  14. ^Maxwell, James Clerk (1873), A Treatise on Electricity and Magnetism,
      p. 4
  15. ^Maxwell, James Clerk (1873), A Treatise on Electricity and Magnetism,
      p. 45
  16. ^Rayleigh, Baron John William Strutt (1877), The_Theory_of_Sound,
      Macmillan
  17. ^ Fourier_(1822), p. 156.
  18. ^Maxwell, James Clerk (1873), A_Treatise_on_Electricity_and_Magnetism,
      volume_1, p. 5
  19. ^"SI_Brochure_(8th_edition)._Section_1.3:_Dimensions_of_quantities".
      BIPM. Retrieved 2013-08-08.
  20. ^ a bDuff, M.J.; Okun, L.B.; Veneziano, G. (September 2002), "Trialogue
      on the number of fundamental constants", Journal of High Energy Physics,
      03 (3): 023, arXiv:physics/0110060, Bibcode:2002JHEP...03..023D, doi:
      10.1088/1126-6708/2002/03/023
  21. ^ For a review of the different conventions in use see:Pisanty, E (2013-
      09-17). "Square_bracket_notation_for_dimensions_and_units:_usage_and
      conventions". Physics Stack Exchange. Retrieved 2014-07-15.
  22. ^Ramsay, Angus. "Dimensional_Analysis_and_Numerical_Experiments_for_a
      Rotating_Disc". Ramsay Maunder Associates. Retrieved 15 April 2017.
  23. ^Duff, M.J. (July 2004). "Comment on time-variation of fundamental
      constants". arXiv:hep-th/0208093v3.
  24. ^Woan, G. (2010), The Cambridge Handbook of Physics Formulas, Cambridge
      University Press, ISBN 978-0-521-57507-2
  25. ^Mosca, Gene; Tipler, Paul Allen (2007), Physics for Scientists and
      Engineers â with Modern Physics (6th ed.), San Francisco: W. H.
      Freeman, ISBN 978-0-7167-8964-2
  26. ^ a bMartin, B.R.; Shaw, G.; Manchester Physics (2008), Particle Physics
      (2nd ed.), Wiley, ISBN 978-0-470-03294-7
***** References[edit] *****
    * Barenblatt,_G._I. (1996), Scaling, Self-Similarity, and Intermediate
      Asymptotics, Cambridge, UK: Cambridge University Press, ISBN 978-0-521-
      43522-2
Bhaskar, R.; Nigam, Anil (1990), "Qualitative Physics Using Dimensional
Analysis", Artificial Intelligence, 45 (1â2): 73â111, doi:10.1016/0004-3702
(90)90038-2
Bhaskar, R.; Nigam, Anil (1991), "Qualitative Explanations of Red Giant
Formation", The Astrophysical Journal, 372: 592â6, Bibcode:
1991ApJ...372..592B, doi:10.1086/170003
Boucher; Alves (1960), "Dimensionless Numbers", Chemical Engineering Progress,
55: 55â64
Bridgman,_P._W. (1922), Dimensional Analysis, Yale University Press, ISBN 978-
0-548-91029-0
Buckingham,_Edgar (1914), "On Physically Similar Systems: Illustrations of the
Use of Dimensional Analysis", Physical Review, 4 (4): 345â376, Bibcode:
1914PhRv....4..345B, doi:10.1103/PhysRev.4.345
Drobot, S. (1953â1954), "On_the_foundations_of_dimensional_analysis" (PDF),
Studia Mathematica, 14: 84â99, doi:10.4064/sm-14-1-84-99
Gibbings, J.C. (2011), Dimensional Analysis, Springer, ISBN 978-1-84996-316-9
Hart,_George_W. (1994), "The_theory_of_dimensioned_matrices", in Lewis, John G.
(ed.), Proceedings of the Fifth SIAM Conference on Applied Linear Algebra,
SIAM, pp. 186â190, ISBN 978-0-89871-336-7
 As postscript
Hart, George W. (1995), Multidimensional_Analysis:_Algebras_and_Systems_for
Science_and_Engineering, Springer-Verlag, ISBN 978-0-387-94417-3
Huntley, H. E. (1967), Dimensional Analysis, Dover, LOC 67-17978
Klinkenberg, A. (1955), "Dimensional systems and systems of units in physics
with special reference to chemical engineering: Part I. The principles
according to which dimensional systems and systems of units are constructed",
Chemical Engineering Science, 4 (3): 130â140, 167â177, doi:10.1016/0009-
2509(55)80004-8
Langhaar, H. L. (1951), Dimensional Analysis and Theory of Models, Wiley,
ISBN 978-0-88275-682-0
Mendez, P.F.; OrdÃ³Ã±ez, F. (September 2005), "Scaling Laws From Statistical
Data and Dimensional Analysis", Journal of Applied Mechanics, 72 (5):
648â657, Bibcode:2005JAM....72..648M, CiteSeerX 10.1.1.422.610, doi:10.1115/
1.1943434
Moody, L. F. (1944), "Friction Factors for Pipe Flow", Transactions of the
American Society of Mechanical Engineers, 66 (671)
Murphy, N. F. (1949), "Dimensional Analysis", Bulletin of the Virginia
Polytechnic Institute, 42 (6)
Perry, J. H.; et al. (1944), "Standard System of Nomenclature for Chemical
Engineering Unit Operations", Transactions of the American Institute of
Chemical Engineers, 40 (251)
Pesic, Peter (2005), Sky in a Bottle, MIT Press, pp. 227â8, ISBN 978-0-262-
16234-0
Petty, G. W. (2001), "Automated computation and consistency checking of
physical dimensions and units in scientific programs", Software â Practice
and Experience, 31 (11): 1067â76, doi:10.1002/spe.401
Porter, Alfred W. (1933), The_Method_of_Dimensions (3rd ed.), Methuen
Lord_Rayleigh (1915), "The Principle of Similitude", Nature, 95 (2368): 66â8,
Bibcode:1915Natur..95...66R, doi:10.1038/095066c0
Siano, Donald (1985), "Orientational Analysis â A Supplement to Dimensional
Analysis â I", Journal of the Franklin Institute, 320 (6): 267â283, doi:
10.1016/0016-0032(85)90031-6
Siano, Donald (1985), "Orientational Analysis, Tensor Analysis and The Group
Properties of the SI Supplementary Units â II", Journal of the Franklin
Institute, 320 (6): 285â302, doi:10.1016/0016-0032(85)90032-8
Silberberg, I. H.; McKetta, J. J. Jr. (1953), "Learning How to Use Dimensional
Analysis", Petroleum Refiner, 32 (4): 5
, (5): 147, (6): 101, (7): 129
Taylor, M.; Diaz, A.I.; Jodar-Sanchez, L.A.; Villanueva-Mico, R.F. (2008), "A
matrix_generalisation_of_dimensional_analysis_using_new_similarity_transforms
to_address_the_problem_of_uniqueness" (PDF), Advanced Studies in Theoretical
Physics, 2 (20): 979â995
Van Driest, E. R. (March 1946), "On Dimensional Analysis and the Presentation
of Data in Fluid Flow Problems", Journal of Applied Mechanics, 68 (Aâ34)
Whitney, H. (1968), "The Mathematics of Physical Quantities, Parts I and II",
American Mathematical Monthly, 75 (2): 115â138, 227â256, doi:10.2307/
2315883, JSTOR 2315883
Vignaux, GA (1992), Erickson, Gary J.; Neudorfer, Paul O. (eds.), Dimensional
Analysis in Data Modelling, Kluwer Academic, ISBN 978-0-7923-2031-9
Kasprzak, WacÅaw; Lysik, Bertold; Rybaczuk, Marek (1990), Dimensional Analysis
in the Identification of Mathematical Models, World Scientific, ISBN 978-981-
02-0304-7
***** External links[edit] *****
 The Wikibook Fluid_Mechanics has a page on the topic of: Dimensional_analysis
    * List_of_dimensions_for_variety_of_physical_quantities
    * Unicalc_Live_web_calculator_doing_units_conversion_by_dimensional
      analysis
    * A_C++_implementation_of_compile-time_dimensional_analysis_in_the_Boost
      open-source_libraries
    * Buckinghamâs_pi-theorem
    * Quantity_System_calculator_for_units_conversion_based_on_dimensional
      approach
    * Units,_quantities,_and_fundamental_constants_project_dimensional_analysis
      maps
    * Bowley, Roger (2009). "[_]_Dimensional_Analysis". Sixty Symbols. Brady
      Haran for the University_of_Nottingham.
Dureisseix, David (2019). "An_introduction_to_dimensional_analysis". INSA Lyon.
**** Converting units[edit] ****
    * Unicalc_Live_web_calculator_doing_units_conversion_by_dimensional
      analysis
    * Math_Skills_Review
    * U.S._EPA_tutorial
    * A_Discussion_of_Units
    * Short_Guide_to_Unit_Conversions
    * Canceling_Units_Lesson
    * Chapter_11:_Behavior_of_Gases Chemistry: Concepts and Applications,
      Denton Independent School District
    * Air_Dispersion_Modeling_Conversions_and_Formulas
    * www.gnu.org/software/units free program, very practical
    * v
    * t
    * e
Systems_of_measurement
                           * International_System_of_Units_(SI)
                           * UK_imperial_system
              General      * US_customary_units
                           * Myanmar
                           * Indian
                           * Apothecaries'
                           * Avoirdupois
              Specific     * Troy
                           * Astronomical
Current                    * Electrical
                           * Temperature
                           * Atomic
                                 o Hartree
                                 o Rydberg
                           * Geometrised
              Natural      * Gaussian
                           * LorentzâHeaviside
                           * Planck
                           * Quantum_chromodynamical
                           * Stoney
                         * Overview
                         * Introduction
              Metric     * Outline
Background               * History
                         * Metrication
                         * Overview
              UK/US      * Comparison
                         * Footâpoundâsecond (FPS)
                                * metreâkilogramâsecond (MKS)
              Metric            * metreâtonneâsecond (MTS)
                                * centimetreâgramâsecond (CGS)
                                * gravitational
                                * Byzantine
                                * Cornish
                                * Cypriot
                                * Czech
                                * Danish
                                * Dutch
                                * English
                                * Estonian
                                * Finnish
                                * French
                                      o Trad.
                                      o Mesures_usuelles
                                * German
                                * Greek
                                * Hungary
                                * Icelandic
                                * Irish
              Europe            * Scottish
                                * Italian
                                * Latvian
                                * Luxembourgian
                                * Maltese
                                * Norwegian
                                * Ottoman
                                * Polish
                                * Portuguese
                                * Romanian
                                * Russian
                                * Serbian
                                * Slovak
                                * Spanish
                                * Swedish
                                * Switzerland
                                * Welsh
                                * Winchester_measure
                                * Afghan
                                * Cambodian
                                * Chinese
                                * Hindu
Historic                        * Hong_Kong
                                * India
                                * Indonesian
                                * Japanese
                                * Korean
              Asia              * Mongolian
                                * Omani
                                * Philippine
                                * Pegu
                                * Singaporean
                                * Sri_Lankan
                                * Syrian
                                * Taiwanese
                                * Tatar
                                * Thai
                                * Vietnamese
                                * Algerian
                                * Ethiopian
                                * Egyptian
                                * Eritrean
                                * Guinean
                                * Libyan
              Africa            * Malagasy
                                * Mauritian
                                * Moroccan
                                * Seychellois
                                * Somali
                                * South_African
                                * Tunisian
                                * Tanzanian
                                * Costa_Rican
                                * Cuban
                                * Haitian
              North America     * Honduran
                                * Mexico
                                * Nicaraguan
                                * Puerto_Rican
                                * Argentine
                                * Brazilian
                                * Chilean
              South America     * Colombian
                                * Paraguayan
                                * Peruvian
                                * Uruguayan
                                * Venezuelan
                  * Arabic
                  * Biblical_and_Talmudic
                  * Egyptian
                  * Greek
Ancient           * Hindu
                  * Indian
                  * Mesopotamian
                  * Persian
                  * Roman
                  * Humorous
List articles     * Obsolete
                  * Unusual
Other             * N-body
                  * Modulor
    * v
    * t
    * e
SI_base_quantities
                Quantity                                     SI_unit
                Name                Symbol        Dimension  Unit     Unit
                                                  symbol     name     symbol
                time,_duration      t             T          second   s
                length              l, x, r, etc. L          metre    m
Base quantities mass                m             M          kilogram kg
                electric_current     I , i     I     ampere   A
                thermodynamic       T             Θ         kelvin   K
                temperature
                amount_of_substance n             N          mole     mol
                luminous_intensity  Iv            J          candela  cd
                    * History_of_the_metric_system
See also            * International_System_of_Quantities
                    * 2019_redefinition
                    * Systems_of_measurement
    * [Wikipedia book] Book
    * [Category] Category
    * Outline
Authority_control [Edit_this_at_Wikidata]     * GND: 4133116-3
                                              * LCCN: sh85038036

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Dimensional_analysis&oldid=907861871"
Categories:
    * Dimensional_analysis
    * Measurement
    * Conversion_of_units_of_measurement
    * Chemical_engineering
    * Mechanical_engineering
    * Environmental_engineering
Hidden categories:
    * CS1_French-language_sources_(fr)
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2013
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Pages_that_use_a_deprecated_format_of_the_chem_tags
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * KreyÃ²l_ayisyen
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÅ¡Äina
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 25 July 2019, at 19:32 (UTC).
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
