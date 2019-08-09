The following text has been accessed from https://en.wikipedia.org/wiki/Nernst_equation at Fri Aug 9 02:55:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Nernst equation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In electrochemistry, the Nernst equation is an equation that relates the
reduction_potential of an electrochemical reaction (half-cell or full_cell
reaction) to the standard_electrode_potential, temperature, and activities
(often approximated by concentrations) of the chemical species undergoing
reduction and oxidation. It was named after Walther_Nernst, a German physical
chemist who formulated the equation.[1][2]
⁰
***** Contents *****
    * 1_Expression
    * 2_Nernst_potential
    * 3_Derivation
          o 3.1_Using_Boltzmann_factors
          o 3.2_Using_thermodynamics_(chemical_potential)
    * 4_Relation_to_equilibrium
    * 5_Limitations
          o 5.1_Time_dependence_of_the_potential
    * 6_Significance_to_related_scientific_domains
    * 7_See_also
    * 8_References
    * 9_External_links
***** Expression[edit] *****
The Nernst equation is derived from the standard changes in the Gibbs_free
energy associated with an electrochemical transformation. For any
electrochemical reduction reaction of the form
      Ox + z eâ â Red
standard thermodynamics says that the actual free energy change ÎG is related
to the free energy change under standard_state ÎGo by the relationship
         &#x0394; G = &#x0394;  G  &#x2296;   + R T ln &#x2061; Q ,
      {\displaystyle \Delta G=\Delta G^{\ominus }+RT\ln Q,}  [{\displaystyle
      \Delta G=\Delta G^{\ominus }+RT\ln Q,}]
where Q is the reaction_quotient. The electrochemical potential E associated
with the electrochemical reaction is defined as the decrease in Gibbs_free
energy per coulomb of charge transferred, which leads to the relationship
         &#x0394; G = &#x2212; z F E .   {\displaystyle \Delta G=-zFE.}  [
      {\displaystyle \Delta G=-zFE.}]
The constant F (the Faraday_constant) is a unit conversion factor F = NAq,
where NA is Avogadro's_number and q is the fundamental electron charge. This
immediately leads to the Nernst equation.
The Nernst equation for an electrochemical half-cell is
          E  red   =  E  red   &#x2296;   &#x2212;    R T   z F    ln &#x2061;
      Q =  E  red   &#x2296;   &#x2212;    R T   z F    ln &#x2061;    a  Red
      a  Ox     .   {\displaystyle E_{\text{red}}=E_{\text{red}}^{\ominus }-
      {\frac {RT}{zF}}\ln Q=E_{\text{red}}^{\ominus }-{\frac {RT}{zF}}\ln
      {\frac {a_{\text{Red}}}{a_{\text{Ox}}}}.}  [{\displaystyle E_{\text
      {red}}=E_{\text{red}}^{\ominus }-{\frac {RT}{zF}}\ln Q=E_{\text{red}}^
      {\ominus }-{\frac {RT}{zF}}\ln {\frac {a_{\text{Red}}}{a_{\text{Ox}}}}.}]
For a complete electrochemical reaction (full cell), the equation can also be
written as
          E  cell   =  E  cell   &#x2296;   &#x2212;    R T   z F    ln
      &#x2061;  Q  r   ,   {\displaystyle E_{\text{cell}}=E_{\text{cell}}^
      {\ominus }-{\frac {RT}{zF}}\ln Q_{r},}  [{\displaystyle E_{\text
      {cell}}=E_{\text{cell}}^{\ominus }-{\frac {RT}{zF}}\ln Q_{r},}]    (total
      cell potential)
where
      Ered is the half-cell reduction_potential at the temperature of interest,
      Eo
      red is the standard_half-cell_reduction_potential,
      Ecell is the cell potential (electromotive_force) at the temperature of
      interest,
      Eo
      cell is the standard_cell_potential,
      R is the universal_gas_constant: R = 8.314472(15) J Kâ1 molâ1,
      T is the temperature in kelvins,
      a is the chemical activity for the relevant species, where aRed is the
      activity of the reduced form and aOx is the activity of the oxidized
      form. Similarly to equilibrium constants, activities are always measured
      with respect to the standard state (1 mol/L for solutes, 1 atm for
      gases). The activity of species x, aX , can be related to the physical
      concentrations cX via aX = Î³XcX, where Î³X is the activity_coefficient
      of species X. Because activity coefficients tend to unity at low
      concentrations, activities in the Nernst equation are frequently replaced
      by simple concentrations.
      F is the Faraday_constant, the number of coulombs per mole of electrons:
      F = 9.64853399(24)Ã104 C molâ1,
      z is the number of electrons transferred in the cell reaction or half-
      reaction,
      Qr is the reaction_quotient of the cell reaction.
At room temperature (25 Â°C), RT/F may be treated as a constant and replaced by
25.693 mV for cells.
The Nernst equation is frequently expressed in terms of base-10 logarithms
(i.e., common_logarithms) rather than natural_logarithms, in which case it is
written, for a cell at 25 Â°C:
         E =  E  0   +    0.059   V   z    log  10   &#x2061;    a  Ox    a
      Red     .   {\displaystyle E=E^{0}+{\frac {0.059\;{\text{V}}}{z}}\log _
      {10}{\frac {a_{\text{Ox}}}{a_{\text{Red}}}}.}  [{\displaystyle E=E^{0}+
      {\frac {0.059\;{\text{V}}}{z}}\log _{10}{\frac {a_{\text{Ox}}}{a_{\text
      {Red}}}}.}]
The Nernst equation is used in physiology for finding the electric_potential of
a cell_membrane with respect to one type of ion.
***** Nernst potential[edit] *****
Main article: Reversal_potential
The Nernst equation has a physiological application when used to calculate the
potential of an ion of charge z across a membrane. This potential is determined
using the concentration of the ion both inside and outside the cell:
         E =    R T   z F    ln &#x2061;    [  ion outside cell  ]   [  ion
      inside cell  ]    = 2.3026    R T   z F     log  10   &#x2061;    [  ion
      outside cell  ]   [  ion inside cell  ]    .   {\displaystyle E={\frac
      {RT}{zF}}\ln {\frac {[{\text{ion outside cell}}]}{[{\text{ion inside
      cell}}]}}=2.3026{\frac {RT}{zF}}\log _{10}{\frac {[{\text{ion outside
      cell}}]}{[{\text{ion inside cell}}]}}.}  [E={\frac {RT}{zF}}\ln {\frac {[
      {\text{ion outside cell}}]}{[{\text{ion inside cell}}]}}=2.3026{\frac
      {RT}{zF}}\log _{10}{\frac {[{\text{ion outside cell}}]}{[{\text{ion
      inside cell}}]}}.]
When the membrane is in thermodynamic_equilibrium (i.e., no net flux of ions),
the membrane_potential must be equal to the Nernst potential. However, in
physiology, due to active ion_pumps, the inside and outside of a cell are not
in equilibrium. In this case, the resting_potential can be determined from the
Goldman_equation, which is a solution of G-H-K_influx_equation under the
constraints that total current density driven by electrochemical force is zero:
          E   m    =    R T  F   ln &#x2061;   (     &#x2211;  i   N    P    M
      i   +       [   M   i   +   ]    o u t    +   &#x2211;  j   M    P    A
      j   &#x2212;       [   A   j   &#x2212;   ]    i n        &#x2211;  i   N
      P    M   i   +       [   M   i   +   ]    i n    +   &#x2211;  j   M    P
      A   j   &#x2212;       [   A   j   &#x2212;   ]    o u t        )   ,
      {\displaystyle E_{\mathrm {m} }={\frac {RT}{F}}\ln {\left({\frac
      {\displaystyle \sum _{i}^{N}P_{\mathrm {M} _{i}^{+}}\left[\mathrm {M} _
      {i}^{+}\right]_{\mathrm {out} }+\displaystyle \sum _{j}^{M}P_{\mathrm {A}
      _{j}^{-}}\left[\mathrm {A} _{j}^{-}\right]_{\mathrm {in} }}{\displaystyle
      \sum _{i}^{N}P_{\mathrm {M} _{i}^{+}}\left[\mathrm {M} _{i}^{+}\right]_
      {\mathrm {in} }+\displaystyle \sum _{j}^{M}P_{\mathrm {A} _{j}^{-}}\left
      [\mathrm {A} _{j}^{-}\right]_{\mathrm {out} }}}\right)},}  [
      {\displaystyle E_{\mathrm {m} }={\frac {RT}{F}}\ln {\left({\frac
      {\displaystyle \sum _{i}^{N}P_{\mathrm {M} _{i}^{+}}\left[\mathrm {M} _
      {i}^{+}\right]_{\mathrm {out} }+\displaystyle \sum _{j}^{M}P_{\mathrm {A}
      _{j}^{-}}\left[\mathrm {A} _{j}^{-}\right]_{\mathrm {in} }}{\displaystyle
      \sum _{i}^{N}P_{\mathrm {M} _{i}^{+}}\left[\mathrm {M} _{i}^{+}\right]_
      {\mathrm {in} }+\displaystyle \sum _{j}^{M}P_{\mathrm {A} _{j}^{-}}\left
      [\mathrm {A} _{j}^{-}\right]_{\mathrm {out} }}}\right)},}]
where
      Em is the membrane potential (in volts, equivalent to joules per
      coulomb),
      Pion is the permeability for that ion (in meters per second),
      [ion]out is the extracellular concentration of that ion (in moles per
      cubic meter, to match the other SI units, though the units strictly don't
      matter, as the ion concentration terms become a dimensionless ratio),
      [ion]in is the intracellular concentration of that ion (in moles per
      cubic meter),
      R is the ideal_gas_constant (joules per kelvin per mole),
      T is the temperature in kelvins,
      F is Faraday's_constant (coulombs per mole).
The potential across the cell membrane that exactly opposes net diffusion of a
particular ion through the membrane is called the Nernst potential for that
ion. As seen above, the magnitude of the Nernst potential is determined by the
ratio of the concentrations of that specific ion on the two sides of the
membrane. The greater this ratio the greater the tendency for the ion to
diffuse in one direction, and therefore the greater the Nernst potential
required to prevent the diffusion.
A similar expression exists that includes r (the absolute value of the
transport ratio). This takes transporters with unequal exchanges into account.
See: sodium-potassium_pump where the transport ratio would be 2/3, so r equals
1.5 in the formula below. The reason why we insert a factor r = 1.5 here is
that current density by electrochemical force Je.c.(Na+)+Je.c.(K+) is no longer
zero, but rather Je.c.(Na+)+1.5Je.c.(K+)=0 (as for both ions flux by
electrochemical force is compensated by that by the pump, i.e. Je.c.=-Jpump),
altering the constraints for applying GHK equation. The other variables are the
same as above. The following example includes two ions: potassium (K+) and
sodium (Na+). Chloride is assumed to be in equilibrium.
          E  m   =    R T  F   ln &#x2061;   (    r  P    K   +       [   K   +
      ]    o u t    +  P    N a   +       [   N a   +   ]    o u t      r  P
      K   +       [   K   +   ]    i n    +  P    N a   +       [   N a   +   ]
      i n       )   .   {\displaystyle E_{m}={\frac {RT}{F}}\ln {\left({\frac
      {rP_{\mathrm {K} ^{+}}\left[\mathrm {K} ^{+}\right]_{\mathrm {out} }+P_
      {\mathrm {Na} ^{+}}\left[\mathrm {Na} ^{+}\right]_{\mathrm {out} }}{rP_
      {\mathrm {K} ^{+}}\left[\mathrm {K} ^{+}\right]_{\mathrm {in} }+P_
      {\mathrm {Na} ^{+}}\left[\mathrm {Na} ^{+}\right]_{\mathrm {in}
      }}}\right)}.}  [{\displaystyle E_{m}={\frac {RT}{F}}\ln {\left({\frac
      {rP_{\mathrm {K} ^{+}}\left[\mathrm {K} ^{+}\right]_{\mathrm {out} }+P_
      {\mathrm {Na} ^{+}}\left[\mathrm {Na} ^{+}\right]_{\mathrm {out} }}{rP_
      {\mathrm {K} ^{+}}\left[\mathrm {K} ^{+}\right]_{\mathrm {in} }+P_
      {\mathrm {Na} ^{+}}\left[\mathrm {Na} ^{+}\right]_{\mathrm {in}
      }}}\right)}.}]
When chloride (Clâ) is taken into account,
          E  m   =    R T  F   ln &#x2061;   (    r  P    K   +       [   K   +
      ]    o u t    +  P    N a   +       [   N a   +   ]    o u t    +  P    C
      l   &#x2212;       [   C l   &#x2212;   ]    i n      r  P    K   +
      [   K   +   ]    i n    +  P    N a   +       [   N a   +   ]    i n    +
      P    C l   &#x2212;       [   C l   &#x2212;   ]    o u t       )   .
      {\displaystyle E_{m}={\frac {RT}{F}}\ln {\left({\frac {rP_{\mathrm {K} ^
      {+}}\left[\mathrm {K} ^{+}\right]_{\mathrm {out} }+P_{\mathrm {Na} ^
      {+}}\left[\mathrm {Na} ^{+}\right]_{\mathrm {out} }+P_{\mathrm {Cl} ^{-
      }}\left[\mathrm {Cl} ^{-}\right]_{\mathrm {in} }}{rP_{\mathrm {K} ^
      {+}}\left[\mathrm {K} ^{+}\right]_{\mathrm {in} }+P_{\mathrm {Na} ^
      {+}}\left[\mathrm {Na} ^{+}\right]_{\mathrm {in} }+P_{\mathrm {Cl} ^{-
      }}\left[\mathrm {Cl} ^{-}\right]_{\mathrm {out} }}}\right)}.}  [
      {\displaystyle E_{m}={\frac {RT}{F}}\ln {\left({\frac {rP_{\mathrm {K} ^
      {+}}\left[\mathrm {K} ^{+}\right]_{\mathrm {out} }+P_{\mathrm {Na} ^
      {+}}\left[\mathrm {Na} ^{+}\right]_{\mathrm {out} }+P_{\mathrm {Cl} ^{-
      }}\left[\mathrm {Cl} ^{-}\right]_{\mathrm {in} }}{rP_{\mathrm {K} ^
      {+}}\left[\mathrm {K} ^{+}\right]_{\mathrm {in} }+P_{\mathrm {Na} ^
      {+}}\left[\mathrm {Na} ^{+}\right]_{\mathrm {in} }+P_{\mathrm {Cl} ^{-
      }}\left[\mathrm {Cl} ^{-}\right]_{\mathrm {out} }}}\right)}.}]
***** Derivation[edit] *****
**** Using Boltzmann factors[edit] ****
For simplicity, we will consider a solution of redox-active molecules that
undergo a one-electron reversible reaction
      Ox + eâ â Red
and that have a standard potential of zero. The chemical_potential Î¼c of this
solution is the difference between the energy barriers for taking electrons
from and for giving electrons to the working_electrode that is setting the
solution's electrochemical_potential.
The ratio of oxidized to reduced molecules, [Ox]/[Red], is equivalent to the
probability of being oxidized (giving electrons) over the probability of being
reduced (taking electrons), which we can write in terms of the Boltzmann_factor
for these processes:
                [  R e d  ]   [  O x  ]       =    exp &#x2061;  (  &#x2212;
      [   barrier for gaining an electron   ]  /  k T  )    exp &#x2061;
      (  &#x2212; [   barrier for losing an electron   ]  /  k T  )           =
      exp &#x2061;  (    &#x03BC;   c     k T    )  .       {\displaystyle
      {\begin{aligned}{\frac {[\mathrm {Red} ]}{[\mathrm {Ox} ]}}&={\frac {\exp
      \left(-[{\mbox{barrier for gaining an electron}}]/kT\right)}{\exp \left(-
      [{\mbox{barrier for losing an electron}}]/kT\right)}}\\[6px]&=\exp \left(
      {\frac {\mu _{\mathrm {c} }}{kT}}\right).\end{aligned}}}  [{\displaystyle
      {\begin{aligned}{\frac {[\mathrm {Red} ]}{[\mathrm {Ox} ]}}&={\frac {\exp
      \left(-[{\mbox{barrier for gaining an electron}}]/kT\right)}{\exp \left(-
      [{\mbox{barrier for losing an electron}}]/kT\right)}}\\[6px]&=\exp \left(
      {\frac {\mu _{\mathrm {c} }}{kT}}\right).\end{aligned}}}]
Taking the natural logarithm of both sides gives
          &#x03BC;   c    = k T ln &#x2061;    [  R e d  ]   [  O x  ]    .
      {\displaystyle \mu _{\mathrm {c} }=kT\ln {\frac {[\mathrm {Red} ]}{
      [\mathrm {Ox} ]}}.}  [{\displaystyle \mu _{\mathrm {c} }=kT\ln {\frac {
      [\mathrm {Red} ]}{[\mathrm {Ox} ]}}.}]
If Î¼c â  0 at [Ox]/[Red] = 1, we need to add in this additional constant:
          &#x03BC;   c    =  &#x03BC;   c    0   + k T ln &#x2061;    [  R e d
      ]   [  O x  ]    .   {\displaystyle \mu _{\mathrm {c} }=\mu _{\mathrm {c}
      }^{0}+kT\ln {\frac {[\mathrm {Red} ]}{[\mathrm {Ox} ]}}.}  [
      {\displaystyle \mu _{\mathrm {c} }=\mu _{\mathrm {c} }^{0}+kT\ln {\frac {
      [\mathrm {Red} ]}{[\mathrm {Ox} ]}}.}]
Dividing the equation by e to convert from chemical potentials to electrode
potentials, and remembering that k/e = R/F,[3] we obtain the Nernst equation
for the one-electron process Ox + eâ â Red:
             E    =  E  0   &#x2212;    k T  e   ln &#x2061;    [  R e d  ]
      [  O x  ]          =  E  0   &#x2212;    R T  F   ln &#x2061;    [  R e d
      ]   [  O x  ]    .       {\displaystyle {\begin{aligned}E&=E^{0}-{\frac
      {kT}{e}}\ln {\frac {[\mathrm {Red} ]}{[\mathrm {Ox} ]}}\\&=E^{0}-{\frac
      {RT}{F}}\ln {\frac {[\mathrm {Red} ]}{[\mathrm {Ox} ]}}.\end{aligned}}}
      [{\displaystyle {\begin{aligned}E&=E^{0}-{\frac {kT}{e}}\ln {\frac {
      [\mathrm {Red} ]}{[\mathrm {Ox} ]}}\\&=E^{0}-{\frac {RT}{F}}\ln {\frac {
      [\mathrm {Red} ]}{[\mathrm {Ox} ]}}.\end{aligned}}}]
**** Using thermodynamics (chemical potential)[edit] ****
Quantities here are given per molecule, not per mole, and so Boltzmann_constant
k and the electron charge e are used instead of the gas constant R and
Faraday's constant F. To convert to the molar quantities given in most
chemistry textbooks, it is simply necessary to multiply by Avogadro's number: R
= kNA and F = eNA.
The entropy of a molecule is defined as
         S &#xA0;     =    d e f      &#xA0; k ln &#x2061; &#x03A9; ,
      {\displaystyle S\ {\stackrel {\mathrm {def} }{=}}\ k\ln \Omega ,}  [
      {\displaystyle S\ {\stackrel {\mathrm {def} }{=}}\ k\ln \Omega ,}]
where Î© is the number of states available to the molecule. The number of
states must vary linearly with the volume V of the system (here an idealized
system is considered for better understanding, so that activities are posited
very close to the true concentrations. Fundamental statistical proof of the
mentioned linearity goes beyond the scope of this section, but to see this is
true it is simpler to consider usual isothermal process for an ideal gas where
the change of entropy ÎS = nR ln(V2/V1) takes place. It follows from the
definition of entropy and from the condition of constant temperature and
quantity of gas n that the change in the number of states must be proportional
to the relative change in volume V2/V1. In this sense there is no difference in
statistical properties of ideal gas atoms compared with the dissolved species
of a solution with activity coefficients equaling one: particles freely "hang
around" filling the provided volume), which is inversely proportional to the
concentration c, so we can also write the entropy as
         S = k ln &#x2061; &#xA0; (  c o n s t a n t  &#x00D7; V ) = &#x2212; k
      ln &#x2061; &#xA0; (  c o n s t a n t  &#x00D7; c ) .   {\displaystyle
      S=k\ln \ (\mathrm {constant} \times V)=-k\ln \ (\mathrm {constant} \times
      c).}  [S=k\ln \ (\mathrm {constant} \times V)=-k\ln \ (\mathrm {constant}
      \times c).]
The change in entropy from some state 1 to another state 2 is therefore
         &#x0394; S =  S  2   &#x2212;  S  1   = &#x2212; k ln &#x2061;    c  2
      c  1     ,   {\displaystyle \Delta S=S_{2}-S_{1}=-k\ln {\frac {c_{2}}{c_
      {1}}},}  [\Delta S=S_{2}-S_{1}=-k\ln {\frac {c_{2}}{c_{1}}},]
so that the entropy of state 2 is
          S  2   =  S  1   &#x2212; k ln &#x2061;    c  2    c  1     .
      {\displaystyle S_{2}=S_{1}-k\ln {\frac {c_{2}}{c_{1}}}.}  [S_{2}=S_{1}-
      k\ln {\frac {c_{2}}{c_{1}}}.]
If state 1 is at standard conditions, in which c1 is unity (e.g., 1 atm or
1 M), it will merely cancel the units of c2. We can, therefore, write the
entropy of an arbitrary molecule A as
         S (  A  ) =  S  0   (  A  ) &#x2212; k ln &#x2061; [  A  ] ,
      {\displaystyle S(\mathrm {A} )=S^{0}(\mathrm {A} )-k\ln[\mathrm {A} ],}
      [{\displaystyle S(\mathrm {A} )=S^{0}(\mathrm {A} )-k\ln[\mathrm {A} ],}]
where S0 is the entropy at standard conditions and [A] denotes the
concentration of A.
The change in entropy for a reaction
      a A + b B â y Y + z Z
is then given by
         &#x0394;  S   r x n    =   (   y S (  Y  ) + z S (  Z  )   )
      &#x2212;   (   a S (  A  ) + b S (  B  )   )   = &#x0394;  S   r x n    0
      &#x2212; k ln &#x2061;    [  Y   ]  y   [  Z   ]  z     [  A   ]  a
      [  B   ]  b      .   {\displaystyle \Delta S_{\mathrm {rxn} }={\big (}yS
      (\mathrm {Y} )+zS(\mathrm {Z} ){\big )}-{\big (}aS(\mathrm {A} )+bS
      (\mathrm {B} ){\big )}=\Delta S_{\mathrm {rxn} }^{0}-k\ln {\frac {
      [\mathrm {Y} ]^{y}[\mathrm {Z} ]^{z}}{[\mathrm {A} ]^{a}[\mathrm {B} ]^
      {b}}}.}  [{\displaystyle \Delta S_{\mathrm {rxn} }={\big (}yS(\mathrm {Y}
      )+zS(\mathrm {Z} ){\big )}-{\big (}aS(\mathrm {A} )+bS(\mathrm {B} ){\big
      )}=\Delta S_{\mathrm {rxn} }^{0}-k\ln {\frac {[\mathrm {Y} ]^{y}[\mathrm
      {Z} ]^{z}}{[\mathrm {A} ]^{a}[\mathrm {B} ]^{b}}}.}]
We define the ratio in the last term as the reaction_quotient:
          Q  r   =     &#x220F;  j    a  j    &#x03BD;  j        &#x220F;  i
      a  i    &#x03BD;  i        &#x2248;    [  Z   ]  z   [  Y   ]  y     [  A
      ]  a   [  B   ]  b      ,   {\displaystyle Q_{r}={\frac {\displaystyle
      \prod _{j}a_{j}^{\nu _{j}}}{\displaystyle \prod _{i}a_{i}^{\nu _
      {i}}}}\approx {\frac {[\mathrm {Z} ]^{z}[\mathrm {Y} ]^{y}}{[\mathrm {A}
      ]^{a}[\mathrm {B} ]^{b}}},}  [{\displaystyle Q_{r}={\frac {\displaystyle
      \prod _{j}a_{j}^{\nu _{j}}}{\displaystyle \prod _{i}a_{i}^{\nu _
      {i}}}}\approx {\frac {[\mathrm {Z} ]^{z}[\mathrm {Y} ]^{y}}{[\mathrm {A}
      ]^{a}[\mathrm {B} ]^{b}}},}]
where the numerator is a product of reaction product activities, aj, each
raised to the power of a stoichiometric_coefficient, Î½j, and the denominator
is a similar product of reactant activities. All activities refer to a time t.
Under certain circumstances (see chemical_equilibrium) each activity term such
as aÎ½j
j may be replaced by a concentration term, [A].
In an electrochemical cell, the cell potential E is the chemical potential
available from redox reactions (E = Î¼c/e). E is related to the Gibbs_energy
change ÎG only by a constant: ÎG = ânFE, where n is the number of electrons
transferred and F is the Faraday constant. There is a negative sign because a
spontaneous reaction has a negative free energy ÎG and a positive potential E.
The Gibbs energy is related to the entropy by G = H â TS, where H is the
enthalpy and T is the temperature of the system. Using these relations, we can
now write the change in Gibbs energy,
         &#x0394; G = &#x0394; H &#x2212; T &#x0394; S = &#x0394;  G  0   + k T
      ln &#x2061;  Q  r   ,   {\displaystyle \Delta G=\Delta H-T\Delta S=\Delta
      G^{0}+kT\ln Q_{r},}  [{\displaystyle \Delta G=\Delta H-T\Delta S=\Delta
      G^{0}+kT\ln Q_{r},}]
and the cell potential,
         E =  E  0   &#x2212;    k T   n e    ln &#x2061;  Q  r   .
      {\displaystyle E=E^{0}-{\frac {kT}{ne}}\ln Q_{r}.}  [{\displaystyle E=E^
      {0}-{\frac {kT}{ne}}\ln Q_{r}.}]
This is the more general form of the Nernst equation. For the redox reaction Ox
+ n eâ â Red,
          Q  r   =    [  R e d  ]   [  O x  ]    ,   {\displaystyle Q_{r}=
      {\frac {[\mathrm {Red} ]}{[\mathrm {Ox} ]}},}  [{\displaystyle Q_{r}=
      {\frac {[\mathrm {Red} ]}{[\mathrm {Ox} ]}},}]
and we have:
             E    =  E  0   &#x2212;    k T   n e    ln &#x2061;    [  R e d  ]
      [  O x  ]          =  E  0   &#x2212;    R T   n F    ln &#x2061;    [  R
      e d  ]   [  O x  ]          =  E  0   &#x2212;    R T   n F    ln
      &#x2061;  Q  r   .       {\displaystyle {\begin{aligned}E&=E^{0}-{\frac
      {kT}{ne}}\ln {\frac {[\mathrm {Red} ]}{[\mathrm {Ox} ]}}\\&=E^{0}-{\frac
      {RT}{nF}}\ln {\frac {[\mathrm {Red} ]}{[\mathrm {Ox} ]}}\\&=E^{0}-{\frac
      {RT}{nF}}\ln Q_{r}.\end{aligned}}}  [{\displaystyle {\begin{aligned}E&=E^
      {0}-{\frac {kT}{ne}}\ln {\frac {[\mathrm {Red} ]}{[\mathrm {Ox} ]}}\\&=E^
      {0}-{\frac {RT}{nF}}\ln {\frac {[\mathrm {Red} ]}{[\mathrm {Ox} ]}}\\&=E^
      {0}-{\frac {RT}{nF}}\ln Q_{r}.\end{aligned}}}]
The cell potential at standard conditions E0 is often replaced by the formal
potential E0â², which includes some small corrections to the logarithm and is
the potential that is actually measured in an electrochemical cell.
***** Relation to equilibrium[edit] *****
At equilibrium, the electrochemical potential E = 0 and therefore the reaction
quotient attains the special value known as the equilibrium constant: Q = K.
Therefore,
             0    =  E  0   &#x2212;    R T   n F    ln &#x2061; K     ln
      &#x2061; K    =    n F  E  0     R T    .       {\displaystyle {\begin
      {aligned}0&=E^{0}-{\frac {RT}{nF}}\ln K\\\ln K&={\frac {nFE^{0}}
      {RT}}.\end{aligned}}}  [{\displaystyle {\begin{aligned}0&=E^{0}-{\frac
      {RT}{nF}}\ln K\\\ln K&={\frac {nFE^{0}}{RT}}.\end{aligned}}}]
Or at standard_temperature,
          log  10   &#x2061; K =    n  E  0     0.05916  &#xA0;V       at&#xA0;
      T = 298.15 &#xA0;  K  .   {\displaystyle \log _{10}K={\frac {nE^{0}}
      {0.05916{\text{ V}}}}\quad {\text{at }}T=298.15~{\text{K}}.}  [
      {\displaystyle \log _{10}K={\frac {nE^{0}}{0.05916{\text{ V}}}}\quad
      {\text{at }}T=298.15~{\text{K}}.}]
We have thus related the standard_electrode_potential and the equilibrium
constant of a redox reaction.
***** Limitations[edit] *****
In dilute solutions, the Nernst equation can be expressed directly in the terms
of concentrations (since activity coefficients are close to unity). But at
higher concentrations, the true activities of the ions must be used. This
complicates the use of the Nernst equation, since estimation of non-ideal
activities of ions generally requires experimental measurements.
The Nernst equation also only applies when there is no net current flow through
the electrode. The activity of ions at the electrode surface changes when_there
is_current_flow, and there are additional overpotential and resistive loss
terms which contribute to the measured potential.
At very low concentrations of the potential-determining ions, the potential
predicted by Nernst equation approaches toward Â±â. This is physically
meaningless because, under such conditions, the exchange_current_density
becomes very low, and there is no thermodynamic equilibrium necessary for
Nernst equation to hold. The electrode is called unpoised in such case. Other
effects tend to take control of the electrochemical behavior of the system.
**** Time dependence of the potential[edit] ****
The expression of time dependence has been established by Karaoglanoff.[4][5]
[6][7]
***** Significance to related scientific domains[edit] *****
The equation has been involved in the scientific controversy involving cold
fusion. The discoverers of cold fusion, Fleischmann and Pons, calculated that a
palladium cathode immersed in a heavy water electrolysis cell could achieve up
to 1027 atmospheres of pressure on the surface of the cathode, enough pressure
to cause spontaneous nuclear fusion. In reality, only 10,000â20,000
atmospheres were achieved. John_R._Huizenga claimed their original calculation
was affected by a misinterpretation of Nernst equation.[8] He cited a paper
about PdâZr alloys.[9] The equation permits the extent of reaction between
two redox systems to be calculated and can be used, for example, to decide
whether a particular reaction will go to completion or not.
At equilibrium the emfs of the two half cells are equal. This enables Kc to be
calculated hence the extent of the reaction.
***** See also[edit] *****
    * Concentration_cell
    * Electrode_potential
    * Galvanic_cell
    * Goldman_equation
    * Membrane_potential
    * NernstâPlanck_equation
    * Solvated_electron
***** References[edit] *****
   1. ^Orna, Mary Virginia; Stock, John (1989). Electrochemistry, past and
      present. Columbus, OH: American Chemical Society. ISBN 978-0-8412-1572-6.
      OCLC 19124885.
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
   3. ^Wahl (2005). "A Short History of Electrochemistry". Galvanotechtnik. 96
      (8): 1820â1828.
   4. ^ R = NAk; see gas_constant
      F = eNA; see Faraday_constant
   5. ^Karaoglanoff,_Z. (January 1906), "Ãber_Oxydations-_und
      ReduktionsvorgÃ¤nge_bei_der_Elektrolyse_von_EisensaltzlÃ¶sungen" [On
      Oxidation and Reduction Processes in the Electrolysis of Iron Salt
      Solutions], Zeitschrift fÃ¼r Elektrochemie (in German), 12 (1): 5â16,
      doi:10.1002/bbpc.19060120105
   6. ^Bard, Allen J.; Inzelt, GyÃ¶rgy; Scholz, Fritz, eds. (2012-10-02),
      "Karaoglanoff equation", Electrochemical_Dictionary, Springer,
      pp. 527â528, ISBN 9783642295515
   7. ^Zutshi, Kamala (2008), Introduction_to_Polarography_and_Allied
      Techniques, pp. 127â128, ISBN 9788122417913
   8. ^ The Journal of Physical Chemistry, Volume 10, p 316. https://
      books.google.com/books?id=zCMSAAAAIAAJ&pg=PA316&lpg=PA316&hl=en&f=false
   9. ^Huizenga,_John_R. (1993). Cold Fusion: The Scientific Fiasco of the
      Century (2 ed.). Oxford and New York: Oxford University Press. pp. 33,
      47. ISBN 978-0-19-855817-0.
  10. ^Huot, J. Y. (1989). "Electrolytic Hydrogenation and Amorphization of Pd-
      Zr Alloys". Journal of the Electrochemical Society. 136 (3): 630. doi:
      10.1149/1.2096700. ISSN 0013-4651.
***** External links[edit] *****
    * Nernst/Goldman_Equation_Simulator
    * Nernst_Equation_Calculator
    * Interactive_Nernst/Goldman_Java_Applet
    * DoITPoMS_Teaching_and_Learning_Package-_"The_Nernst_Equation_and_Pourbaix
      Diagrams"

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Nernst_equation&oldid=903472376"
Categories:
    * Walther_Nernst
    * Electrochemical_equations
Hidden categories:
    * CS1_German-language_sources_(de)
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
    * Dansk
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * LatvieÅ¡u
    * LietuviÅ³
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Suomi
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 25 June 2019, at 22:15 (UTC).
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
