The following text has been accessed from https://en.wikipedia.org/wiki/Poynting%27s_theorem at Fri Aug 9 03:05:47 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Poynting's theorem ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article has multiple issues. Please help improve_it or discuss these
 issues on the talk_page. (Learn_how_and_when_to_remove_these_template_messages)
  This article may be confusing_or_unclear to readers. Please help us clarify
  the_article. There is a discussion about this on Talk:Poynting's_theorem
  Â§ Inconsistencies_throughout_article. (October 2017)(Learn_how_and_when_to
  remove_this_template_message)
  This article needs attention from an expert in Physics. Please add a reason or
  a talk parameter to this template to explain the issue with the article.
  WikiProject_Physics may be able to help recruit an expert. (October 2017)
 (Learn_how_and_when_to_remove_this_template_message)
In electrodynamics, Poynting's theorem is a statement of conservation_of_energy
for the electromagnetic_field,[clarification_needed] in the form of a partial
differential_equation, due to the British physicist John_Henry_Poynting.[1]
Poynting's theorem is analogous to the work-energy_theorem in classical
mechanics, and mathematically similar to the continuity_equation, because it
relates the energy stored in the electromagnetic field to the work done on a
charge_distribution (i.e. an electrically charged object), through energy_flux.
⁰
***** Contents *****
    * 1_Statement
          o 1.1_General
          o 1.2_Electrical_Engineering
    * 2_Derivation
          o 2.1_Poynting's_theorem
          o 2.2_Poynting_vector
    * 3_Poynting_vector_in_macroscopic_media
    * 4_Alternative_forms
    * 5_Generalization
    * 6_References
    * 7_External_links
***** Statement[edit] *****
**** General[edit] ****
In words, the theorem is an energy balance:
      The rate of energy transfer (per unit volume) from a region of space
      equals the rate of work done on a charge distribution plus the energy
      flux leaving that region.
A second statement can also explain the theorem - "The decrease in the
electromagnetic energy per unit time in a certain volume is equal to the sum of
work done by the field forces and the net outward flux per unit time".
Mathematically, this is summarised in differential form as:
   &#x2212;    &#x2202; u   &#x2202; t    = &#x2207; &#x22C5;  S  +  J
&#x22C5;  E    {\displaystyle -{\frac {\partial u}{\partial t}}=\nabla \cdot
\mathbf {S} +\mathbf {J} \cdot \mathbf {E} }  [-{\frac  {\partial u}{\partial
t}}=\nabla \cdot {\mathbf  {S}}+{\mathbf  {J}}\cdot {\mathbf  {E}}]
where ââ¢S is the divergence of the Poynting_vector (energy flow) and Jâ¢E
is the rate at which the fields do work on a charged object (J is the current
density corresponding to the motion of charge, E is the electric_field, and â¢
is the dot_product). The energy_density u is given by:[2]
         u =   1 2    (   &#x03F5;  0    E  &#x22C5;  E  +   1  &#x03BC;  0
      B  &#x22C5;  B   )    {\displaystyle u={\frac {1}{2}}\left(\epsilon _
      {0}\mathbf {E} \cdot \mathbf {E} +{\frac {1}{\mu _{0}}}\mathbf {B} \cdot
      \mathbf {B} \right)}  [{\displaystyle u={\frac {1}{2}}\left(\epsilon _
      {0}\mathbf {E} \cdot \mathbf {E} +{\frac {1}{\mu _{0}}}\mathbf {B} \cdot
      \mathbf {B} \right)}]
in which B is the magnetic_flux_density. Using the divergence_theorem,
Poynting's theorem can be rewritten in integral form:
   &#x2212;   &#x2202;  &#x2202; t     &#x222B;  V   u d V =   {\displaystyle -
{\frac {\partial }{\partial t}}\int _{V}udV=}  [-{\frac  {\partial }{\partial
t}}\int _{V}udV=] [\oiint]     &#x2202; V    {\displaystyle \scriptstyle
\partial V}  [\scriptstyle \partial V]      S  &#x22C5; d  A  +  &#x222B;  V
J  &#x22C5;  E  d V   {\displaystyle \mathbf {S} \cdot d\mathbf {A} +\int _
{V}\mathbf {J} \cdot \mathbf {E} dV}  [{\mathbf  {S}}\cdot d{\mathbf  {A}}+\int
_{V}{\mathbf  {J}}\cdot {\mathbf  {E}}dV]
where     &#x2202; V    {\displaystyle \partial V\!}  [\partial V\!] is the
boundary of a volume V. The shape of the volume is arbitrary but fixed for the
calculation.
**** Electrical Engineering[edit] ****
In electrical_engineering context the theorem is usually written with the
energy density term u expanded in the following way, which resembles the
continuity_equation:
         &#x2207; &#x22C5;  S  +  &#x03F5;  0    E  &#x22C5;    &#x2202;  E
      &#x2202; t    +    B   &#x03BC;  0     &#x22C5;    &#x2202;  B
      &#x2202; t    +  J  &#x22C5;  E  = 0 ,   {\displaystyle \nabla \cdot
      \mathbf {S} +\epsilon _{0}\mathbf {E} \cdot {\frac {\partial \mathbf {E}
      }{\partial t}}+{\frac {\mathbf {B} }{\mu _{0}}}\cdot {\frac {\partial
      \mathbf {B} }{\partial t}}+\mathbf {J} \cdot \mathbf {E} =0,}  [\nabla
      \cdot {\mathbf  {S}}+\epsilon _{0}{\mathbf  {E}}\cdot {\frac  {\partial
      {\mathbf  {E}}}{\partial t}}+{\frac  {{\mathbf  {B}}}{\mu _{0}}}\cdot
      {\frac  {\partial {\mathbf  {B}}}{\partial t}}+{\mathbf  {J}}\cdot
      {\mathbf  {E}}=0,]
where
    * Îµ0 is the electric_constant and Î¼0 is the magnetic_constant.
    *     &#x03F5;  0    E  &#x22C5;    &#x2202;  E    &#x2202; t
      {\displaystyle \epsilon _{0}\mathbf {E} \cdot {\frac {\partial \mathbf
      {E} }{\partial t}}}  [\epsilon _{0}{\mathbf  {E}}\cdot {\frac  {\partial
      {\mathbf  {E}}}{\partial t}}] is the density of reactive_power driving
      the build-up of electric field,
    *       B   &#x03BC;  0     &#x22C5;    &#x2202;  B    &#x2202; t
      {\displaystyle {\frac {\mathbf {B} }{\mu _{0}}}\cdot {\frac {\partial
      \mathbf {B} }{\partial t}}}  [{\frac  {{\mathbf  {B}}}{\mu _{0}}}\cdot
      {\frac  {\partial {\mathbf  {B}}}{\partial t}}] is the density of
      reactive_power driving the build-up of magnetic field, and
    *     J  &#x22C5;  E    {\displaystyle \mathbf {J} \cdot \mathbf {E} }  [
      {\mathbf  {J}}\cdot {\mathbf  {E}}] is the density of electric_power
      dissipated by the Lorentz_force acting on charge carriers.
***** Derivation[edit] *****
While conservation_of_energy and the Lorentz_force law can give the general
form of the theorem, Maxwell's_equations are additionally required to derive
the expression for the Poynting vector and hence complete the statement.
**** Poynting's theorem[edit] ****
Considering the statement in words above - there are three elements to the
theorem, which involve writing energy transfer (per unit time) as volume
integrals:[3]
   1. Since u is the energy density, integrating over the volume of the region
      gives the total energy U stored in the region, then taking the (partial)
      time derivative gives the rate of change of energy:
               U =  &#x222B;  V   u d V &#xA0; &#x2192; &#xA0;    &#x2202; U
            &#x2202; t    =   &#x2202;  &#x2202; t     &#x222B;  V   u d V =
            &#x222B;  V      &#x2202; u   &#x2202; t    d V .   {\displaystyle
            U=\int _{V}udV\ \rightarrow \ {\frac {\partial U}{\partial t}}=
            {\frac {\partial }{\partial t}}\int _{V}udV=\int _{V}{\frac
            {\partial u}{\partial t}}dV.}  [U=\int _{V}udV\ \rightarrow \
            {\frac  {\partial U}{\partial t}}={\frac  {\partial }{\partial
            t}}\int _{V}udV=\int _{V}{\frac  {\partial u}{\partial t}}dV.]
   2. The energy flux leaving the region is the surface_integral of the
      Poynting vector, and using the divergence_theorem this can be written as
      a volume integral:
            [\oiint]     &#x2202; V    {\displaystyle \scriptstyle \partial V}
            [\scriptstyle \partial V]      S  &#x22C5; d  A  =  &#x222B;  V
            &#x2207; &#x22C5;  S  d V .   {\displaystyle \mathbf {S} \cdot
            d\mathbf {A} =\int _{V}\nabla \cdot \mathbf {S} dV.}  [{\mathbf
            {S}}\cdot d{\mathbf  {A}}=\int _{V}\nabla \cdot {\mathbf  {S}}dV.]
   3. The Lorentz_force density f on a charge distribution, integrated over the
      volume to get the total force F, is
                f  = &#x03C1;  E  +  J  &#x00D7;  B  &#xA0; &#x2192; &#xA0;
            &#x222B;  V    f  d V =  F  =  &#x222B;  V   ( &#x03C1;  E  +  J
            &#x00D7;  B  ) d V ,   {\displaystyle \mathbf {f} =\rho \mathbf {E}
            +\mathbf {J} \times \mathbf {B} \ \rightarrow \ \int _{V}\mathbf
            {f} dV=\mathbf {F} =\int _{V}(\rho \mathbf {E} +\mathbf {J} \times
            \mathbf {B} )dV,}  [{\mathbf  {f}}=\rho {\mathbf  {E}}+{\mathbf
            {J}}\times {\mathbf  {B}}\ \rightarrow \ \int _{V}{\mathbf  {f}}dV=
            {\mathbf  {F}}=\int _{V}(\rho {\mathbf  {E}}+{\mathbf  {J}}\times
            {\mathbf  {B}})dV,]
      where Ï is the charge_density of the distribution and v its velocity.
      Since      J  = &#x03C1;  v    {\displaystyle \mathbf {J} =\rho \mathbf
      {v} }  [{\mathbf  {J}}=\rho {\mathbf  {v}}], the rate of work done by the
      force is
                F  &#x22C5;    d  r    d t    =  F  &#x22C5;  v  =  &#x222B;  V
            ( &#x03C1;  E  &#x22C5;  v  + &#x03C1;  v  &#x00D7;  B  &#x22C5;  v
            ) d V &#xA0; &#x2192; &#xA0;  F  &#x22C5;  v  =  &#x222B;  V    E
            &#x22C5;  J  d V .   {\displaystyle \mathbf {F} \cdot {\frac
            {d\mathbf {r} }{dt}}=\mathbf {F} \cdot \mathbf {v} =\int _{V}(\rho
            \mathbf {E} \cdot \mathbf {v} +\rho \mathbf {v} \times \mathbf {B}
            \cdot \mathbf {v} )dV\ \rightarrow \ \mathbf {F} \cdot \mathbf {v}
            =\int _{V}\mathbf {E} \cdot \mathbf {J} dV.}  [{\mathbf  {F}}\cdot
            {\frac  {d{\mathbf  {r}}}{dt}}={\mathbf  {F}}\cdot {\mathbf
            {v}}=\int _{V}(\rho {\mathbf  {E}}\cdot {\mathbf  {v}}+\rho
            {\mathbf  {v}}\times {\mathbf  {B}}\cdot {\mathbf  {v}})dV\
            \rightarrow \ {\mathbf  {F}}\cdot {\mathbf  {v}}=\int _{V}{\mathbf
            {E}}\cdot {\mathbf  {J}}dV.]
So by conservation of energy, the balance equation for the energy flow per unit
time is the integral form of the theorem:
         &#x2212;  &#x222B;  V      &#x2202; u   &#x2202; t    d V =  &#x222B;
      V   &#x2207; &#x22C5;  S  d V +  &#x222B;  V    J  &#x22C5;  E  d V ,
      {\displaystyle -\int _{V}{\frac {\partial u}{\partial t}}dV=\int _
      {V}\nabla \cdot \mathbf {S} dV+\int _{V}\mathbf {J} \cdot \mathbf {E}
      dV,}  [-\int _{V}{\frac  {\partial u}{\partial t}}dV=\int _{V}\nabla
      \cdot {\mathbf  {S}}dV+\int _{V}{\mathbf  {J}}\cdot {\mathbf  {E}}dV,]
and since the volume V is arbitrary, this is true for all volumes, implying
         &#x2212;    &#x2202; u   &#x2202; t    = &#x2207; &#x22C5;  S  +  J
      &#x22C5;  E  ,   {\displaystyle -{\frac {\partial u}{\partial t}}=\nabla
      \cdot \mathbf {S} +\mathbf {J} \cdot \mathbf {E} ,}  [-{\frac  {\partial
      u}{\partial t}}=\nabla \cdot {\mathbf  {S}}+{\mathbf  {J}}\cdot {\mathbf
      {E}},]
which is Poynting's theorem in differential form.
**** Poynting vector[edit] ****
Main article: Poynting_vector
From the theorem, the actual form of the Poynting vector S can be found. The
time derivative of the energy density (using the product_rule for vector dot
products) is
            &#x2202; u   &#x2202; t    =   1 2    (   E  &#x22C5;    &#x2202;
      D    &#x2202; t    +  D  &#x22C5;    &#x2202;  E    &#x2202; t    +  H
      &#x22C5;    &#x2202;  B    &#x2202; t    +  B  &#x22C5;    &#x2202;  H
      &#x2202; t     )  =  E  &#x22C5;    &#x2202;  D    &#x2202; t    +  H
      &#x22C5;    &#x2202;  B    &#x2202; t    ,   {\displaystyle {\frac
      {\partial u}{\partial t}}={\frac {1}{2}}\left(\mathbf {E} \cdot {\frac
      {\partial \mathbf {D} }{\partial t}}+\mathbf {D} \cdot {\frac {\partial
      \mathbf {E} }{\partial t}}+\mathbf {H} \cdot {\frac {\partial \mathbf {B}
      }{\partial t}}+\mathbf {B} \cdot {\frac {\partial \mathbf {H} }{\partial
      t}}\right)=\mathbf {E} \cdot {\frac {\partial \mathbf {D} }{\partial
      t}}+\mathbf {H} \cdot {\frac {\partial \mathbf {B} }{\partial t}},}  [
      {\frac  {\partial u}{\partial t}}={\frac  {1}{2}}\left({\mathbf
      {E}}\cdot {\frac  {\partial {\mathbf  {D}}}{\partial t}}+{\mathbf
      {D}}\cdot {\frac  {\partial {\mathbf  {E}}}{\partial t}}+{\mathbf
      {H}}\cdot {\frac  {\partial {\mathbf  {B}}}{\partial t}}+{\mathbf
      {B}}\cdot {\frac  {\partial {\mathbf  {H}}}{\partial t}}\right)={\mathbf
      {E}}\cdot {\frac  {\partial {\mathbf  {D}}}{\partial t}}+{\mathbf
      {H}}\cdot {\frac  {\partial {\mathbf  {B}}}{\partial t}},]
using the constitutive_relations[clarification_needed]
          D  =  &#x03F5;  0    E  ,   H  =    B   &#x03BC;  0
      {\displaystyle \mathbf {D} =\epsilon _{0}\mathbf {E} ,\quad \mathbf {H} =
      {\frac {\mathbf {B} }{\mu _{0}}}}  [{\displaystyle \mathbf {D} =\epsilon
      _{0}\mathbf {E} ,\quad \mathbf {H} ={\frac {\mathbf {B} }{\mu _{0}}}}]
The partial time derivatives suggest using two of Maxwell's_Equations. Taking
the dot_product of the MaxwellâFaraday_equation with H:
            &#x2202;  B    &#x2202; t    = &#x2212; &#x2207; &#x00D7;  E
      &#xA0; &#x2192; &#xA0;  H  &#x22C5;    &#x2202;  B    &#x2202; t    =
      &#x2212;  H  &#x22C5; &#x2207; &#x00D7;  E  ,   {\displaystyle {\frac
      {\partial \mathbf {B} }{\partial t}}=-\nabla \times \mathbf {E} \
      \rightarrow \ \mathbf {H} \cdot {\frac {\partial \mathbf {B} }{\partial
      t}}=-\mathbf {H} \cdot \nabla \times \mathbf {E} ,}  [{\frac  {\partial
      {\mathbf  {B}}}{\partial t}}=-\nabla \times {\mathbf  {E}}\ \rightarrow \
      {\mathbf  {H}}\cdot {\frac  {\partial {\mathbf  {B}}}{\partial t}}=-
      {\mathbf  {H}}\cdot \nabla \times {\mathbf  {E}},]
next taking the dot product of the MaxwellâAmpÃ¨re_equation with E:
            &#x2202;  D    &#x2202; t    +  J  = &#x2207; &#x00D7;  H  &#xA0;
      &#x2192; &#xA0;  E  &#x22C5;    &#x2202;  D    &#x2202; t    +  E
      &#x22C5;  J  =  E  &#x22C5; &#x2207; &#x00D7;  H  .   {\displaystyle
      {\frac {\partial \mathbf {D} }{\partial t}}+\mathbf {J} =\nabla \times
      \mathbf {H} \ \rightarrow \ \mathbf {E} \cdot {\frac {\partial \mathbf
      {D} }{\partial t}}+\mathbf {E} \cdot \mathbf {J} =\mathbf {E} \cdot
      \nabla \times \mathbf {H} .}  [{\frac  {\partial {\mathbf  {D}}}{\partial
      t}}+{\mathbf  {J}}=\nabla \times {\mathbf  {H}}\ \rightarrow \ {\mathbf
      {E}}\cdot {\frac  {\partial {\mathbf  {D}}}{\partial t}}+{\mathbf
      {E}}\cdot {\mathbf  {J}}={\mathbf  {E}}\cdot \nabla \times {\mathbf
      {H}}.]
Collecting the results so far gives:
             &#x2212; &#x2207; &#x22C5;  S     =    &#x2202; u   &#x2202; t
      +  J  &#x22C5;  E        =  (   H  &#x22C5;    &#x2202;  B    &#x2202; t
      +  E  &#x22C5;    &#x2202;  D    &#x2202; t     )  +  J  &#x22C5;  E
      =  E  &#x22C5; &#x2207; &#x00D7;  H  &#x2212;  H  &#x22C5; &#x2207;
      &#x00D7;  E  ,       {\displaystyle {\begin{aligned}-\nabla \cdot \mathbf
      {S} &={\frac {\partial u}{\partial t}}+\mathbf {J} \cdot \mathbf {E}
      \\&=\left(\mathbf {H} \cdot {\frac {\partial \mathbf {B} }{\partial
      t}}+\mathbf {E} \cdot {\frac {\partial \mathbf {D} }{\partial
      t}}\right)+\mathbf {J} \cdot \mathbf {E} \\&=\mathbf {E} \cdot \nabla
      \times \mathbf {H} -\mathbf {H} \cdot \nabla \times \mathbf {E} ,\\\end
      {aligned}}}  [{\begin{aligned}-\nabla \cdot {\mathbf  {S}}&={\frac
      {\partial u}{\partial t}}+{\mathbf  {J}}\cdot {\mathbf  {E}}\\&=\left(
      {\mathbf  {H}}\cdot {\frac  {\partial {\mathbf  {B}}}{\partial t}}+
      {\mathbf  {E}}\cdot {\frac  {\partial {\mathbf  {D}}}{\partial
      t}}\right)+{\mathbf  {J}}\cdot {\mathbf  {E}}\\&={\mathbf  {E}}\cdot
      \nabla \times {\mathbf  {H}}-{\mathbf  {H}}\cdot \nabla \times {\mathbf
      {E}},\\\end{aligned}}]
then, using the vector_calculus_identity:
         &#x2207; &#x22C5; (  E  &#x00D7;  H  ) =  H  &#x22C5; ( &#x2207;
      &#x00D7;  E  ) &#x2212;  E  &#x22C5; ( &#x2207; &#x00D7;  H  ) ,
      {\displaystyle \nabla \cdot (\mathbf {E} \times \mathbf {H} )=\mathbf {H}
      \cdot (\nabla \times \mathbf {E} )-\mathbf {E} \cdot (\nabla \times
      \mathbf {H} ),}  [{\displaystyle \nabla \cdot (\mathbf {E} \times \mathbf
      {H} )=\mathbf {H} \cdot (\nabla \times \mathbf {E} )-\mathbf {E} \cdot
      (\nabla \times \mathbf {H} ),}]
gives an expression for the Poynting vector:
          S  =  E  &#x00D7;  H  ,   {\displaystyle \mathbf {S} =\mathbf {E}
      \times \mathbf {H} ,}  [{\mathbf  {S}}={\mathbf  {E}}\times {\mathbf
      {H}},]
which physically means the energy transfer due to time-varying electric and
magnetic fields is perpendicular to the fields.
***** Poynting vector in macroscopic media[edit] *****
In a macroscopic medium, electromagnetic effects are described by spatially
averaged (macroscopic) fields. The Poynting vector in a macroscopic medium can
be defined self-consistently with microscopic theory, in such a way that the
spatially averaged microscopic Poynting vector is exactly predicted by a
macroscopic formalism. This result is strictly valid in the limit of low-loss
and allows for the unambiguous identification of the Poynting vector form in
macroscopic electrodynamics.[4][5]
***** Alternative forms[edit] *****
It is possible to derive alternative versions of Poynting's theorem.[6] Instead
of the flux vector E Ã B as above, it is possible to follow the same style of
derivation, but instead choose the Abraham form E Ã H, the Minkowski form D Ã
B, or perhaps D Ã H. Each choice represents the response of the propagation
medium in its own way: the E Ã B form above has the property that the response
happens only due to electric currents, while the D Ã H form uses only
(fictitious) magnetic_monopole currents. The other two forms (Abraham and
Minkowski) use complementary combinations of electric and magnetic currents to
represent the polarization and magnetization responses of the medium.
***** Generalization[edit] *****
The mechanical energy counterpart of the above theorem for the electromagnetic
energy continuity equation is
           &#x2202;  &#x2202; t     u  m   (  r  , t ) + &#x2207; &#x22C5;   S
      m   (  r  , t ) =  J  (  r  , t ) &#x22C5;  E  (  r  , t ) ,
      {\displaystyle {\frac {\partial }{\partial t}}u_{m}(\mathbf {r}
      ,t)+\nabla \cdot \mathbf {S} _{m}(\mathbf {r} ,t)=\mathbf {J} (\mathbf
      {r} ,t)\cdot \mathbf {E} (\mathbf {r} ,t),}  [{\frac  {\partial }
      {\partial t}}u_{m}({\mathbf  {r}},t)+\nabla \cdot {\mathbf  {S}}_{m}(
      {\mathbf  {r}},t)={\mathbf  {J}}({\mathbf  {r}},t)\cdot {\mathbf  {E}}(
      {\mathbf  {r}},t),]
where um is the (mechanical) kinetic_energy density in the system. It can be
described as the sum of kinetic energies of particles Î± (e.g., electrons in a
wire), whose trajectory is given by rÎ±(t):
          u  m   (  r  , t ) =  &#x2211;  &#x03B1;      m  &#x03B1;   2       r
      &#x02D9;     &#x03B1;   2   &#x03B4; (  r  &#x2212;   r   &#x03B1;   ( t
      ) ) ,   {\displaystyle u_{m}(\mathbf {r} ,t)=\sum _{\alpha }{\frac {m_
      {\alpha }}{2}}{\dot {r}}_{\alpha }^{2}\delta (\mathbf {r} -\mathbf {r} _
      {\alpha }(t)),}  [u_{m}({\mathbf  {r}},t)=\sum _{{\alpha }}{\frac  {m_{
      {\alpha }}}{2}}{\dot  {r}}_{{\alpha }}^{2}\delta ({\mathbf  {r}}-{\mathbf
      {r}}_{{\alpha }}(t)),]
where Sm is the flux of their energies, or a "mechanical Poynting vector":
           S   m   (  r  , t ) =  &#x2211;  &#x03B1;      m  &#x03B1;   2
      r &#x02D9;     &#x03B1;   2        r  &#x02D9;     &#x03B1;   &#x03B4;
      (  r  &#x2212;   r   &#x03B1;   ( t ) ) .   {\displaystyle \mathbf {S} _
      {m}(\mathbf {r} ,t)=\sum _{\alpha }{\frac {m_{\alpha }}{2}}{\dot {r}}_
      {\alpha }^{2}{\dot {\mathbf {r} }}_{\alpha }\delta (\mathbf {r} -\mathbf
      {r} _{\alpha }(t)).}  [{\mathbf  {S}}_{m}({\mathbf  {r}},t)=\sum _{
      {\alpha }}{\frac  {m_{{\alpha }}}{2}}{\dot  {r}}_{{\alpha }}^{2}{\dot  {
      {\mathbf  {r}}}}_{{\alpha }}\delta ({\mathbf  {r}}-{\mathbf  {r}}_{
      {\alpha }}(t)).]
Both can be combined via the Lorentz_force, which the electromagnetic fields
exert on the moving charged particles (see above), to the following energy
continuity_equation or energy conservation_law:[7]
           &#x2202;  &#x2202; t     (   u  e   +  u  m    )  + &#x2207;
      &#x22C5;  (    S   e   +   S   m    )  = 0 ,   {\displaystyle {\frac
      {\partial }{\partial t}}\left(u_{e}+u_{m}\right)+\nabla \cdot \left
      (\mathbf {S} _{e}+\mathbf {S} _{m}\right)=0,}  [{\frac  {\partial }
      {\partial t}}\left(u_{e}+u_{m}\right)+\nabla \cdot \left({\mathbf  {S}}_
      {e}+{\mathbf  {S}}_{m}\right)=0,]
covering both types of energy and the conversion of one into the other.
***** References[edit] *****
   1. ^Poynting, J. H. "On_the_Transfer_of_Energy_in_the_Electromagnetic
      Field" . 175: 343â361. doi:10.1098/rstl.1884.0016.
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
   3. ^ Griffiths, David J. Introduction to electrodynamics. Prentice Hall,
      1962.
   4. ^ Introduction to Electrodynamics (3rd Edition), D.J. Griffiths, Pearson
      Education, Dorling Kindersley, 2007, p.364,
   5. ISBN 81-7758-293-3
   6. ^Silveirinha, M. G. (2010). "Poynting vector, heating rate, and stored
      energy in structured materials: a first principles derivation". Phys.
      Rev. B. 82: 037104.
   7. ^Costa, J. T. , M. G. Silveirinha, A. AlÃ¹ (2011). "Poynting Vector in
      Negative-Index Metamaterials". Phys. Rev. B. 83: 165120.
   8. ^ Kinsler, P.; Favaro, A.; McCall M.W. (2009). "Four_Poynting_theorems"
      (PDF). European Journal of Physics. 30 (5): 983. arXiv:0908.1721.
      Bibcode:2009EJPh...30..983K. doi:10.1088/0143-0807/30/5/007.
   9. ^ Richter, E.; Florian, M.; Henneberger, K. (2008). "Poynting's theorem
      and energy conservation in the propagation of light in bounded media".
      Europhysics Letters. 81 (6): 67005. arXiv:0710.0515. Bibcode:
      2008EL.....8167005R. doi:10.1209/0295-5075/81/67005.
***** External links[edit] *****
    * Eric_W._Weisstein_"Poynting_Theorem"_From_ScienceWorld_â_A_Wolfram_Web
      Resource.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Poynting%27s_theorem&oldid=898551429"
Categories:
    * Electrodynamics
    * Physics_theorems
    * Circuit_theorems
Hidden categories:
    * Wikipedia_articles_needing_clarification_from_October_2017
    * All_Wikipedia_articles_needing_clarification
    * Articles_needing_expert_attention_with_no_reason_or_talk_parameter
    * Articles_needing_expert_attention_from_October_2017
    * All_articles_needing_expert_attention
    * Physics_articles_needing_expert_attention
    * Articles_with_multiple_maintenance_issues
    * Wikipedia_articles_needing_clarification_from_May_2015
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * Deutsch
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 24 May 2019, at 09:56 (UTC).
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
