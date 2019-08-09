The following text has been accessed from https://en.wikipedia.org/wiki/Rigid_rotor at Fri Aug 9 02:04:15 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Rigid rotor ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The rigid rotor is a mechanical model of rotating systems. An arbitrary rigid
rotor is a 3-dimensional rigid object, such as a top. To orient such an object
in space requires three angles, known as Euler_angles. A special rigid rotor is
the linear rotor requiring only two angles to describe, for example of a
diatomic molecule. More general_molecules are 3-dimensional, such as water
(asymmetric rotor), ammonia (symmetric rotor), or methane (spherical rotor).
⁰
***** Contents *****
    * 1_Linear_rotor
          o 1.1_Classical_linear_rigid_rotor
          o 1.2_Quantum_mechanical_linear_rigid_rotor
          o 1.3_Selection_rules
          o 1.4_Non-rigid_linear_rotor
    * 2_Arbitrarily_shaped_rigid_rotor
          o 2.1_Coordinates_of_the_rigid_rotor
          o 2.2_Classical_kinetic_energy
                # 2.2.1_Angular_velocity_form
                # 2.2.2_Lagrange_form
                # 2.2.3_Angular_momentum_form
                # 2.2.4_Hamilton_form
          o 2.3_Quantum_mechanical_rigid_rotor
    * 3_Direct_experimental_observation_of_molecular_rotations
    * 4_See_also
    * 5_References
    * 6_General_references
***** Linear rotor[edit] *****
The linear rigid rotor model consists of two point masses located at fixed
distances from their center of mass. The fixed distance between the two masses
and the values of the masses are the only characteristics of the rigid model.
However, for many actual diatomics this model is too restrictive since
distances are usually not completely fixed. Corrections on the rigid model can
be made to compensate for small variations in the distance. Even in such a case
the rigid rotor model is a useful point of departure (zeroth-order model).
**** Classical linear rigid rotor[edit] ****
The classical linear rotor consists of two point masses      m  1
{\displaystyle m_{1}}  [m_{1}] and      m  2     {\displaystyle m_{2}}  [m_{2}]
(with reduced_mass     &#x03BC; =     m  1    m  2      m  1   +  m  2
{\displaystyle \mu ={\frac {m_{1}m_{2}}{m_{1}+m_{2}}}}  [\mu ={\frac  {m_{1}m_
{2}}{m_{1}+m_{2}}}]) each at a distance     R   {\displaystyle R}  [R]. The
rotor is rigid if     R   {\displaystyle R}  [R] is independent of time. The
kinematics of a linear rigid rotor is usually described by means of spherical
polar_coordinates, which form a coordinate system of R3. In the physics
convention the coordinates are the co-latitude (zenith) angle     &#x03B8;
{\displaystyle \theta \,}  [\theta \,], the longitudinal (azimuth) angle
&#x03C6;    {\displaystyle \varphi \,}  [\varphi \,] and the distance     R
{\displaystyle R}  [R]. The angles specify the orientation of the rotor in
space. The kinetic energy     T   {\displaystyle T}  [T] of the linear rigid
rotor is given by
         2 T = &#x03BC;  R  2     [       &#x03B8; &#x02D9;     2   +
      (    &#x03C6; &#x02D9;     sin &#x2061; &#x03B8;  )  2     ]   = &#x03BC;
      R  2     (      &#x03B8; &#x02D9;         &#x03C6; &#x02D9;      )
      (    1   0     0    sin  2   &#x2061; &#x03B8;    )     (       &#x03B8;
      &#x02D9;           &#x03C6; &#x02D9;       )   = &#x03BC;
      (      &#x03B8; &#x02D9;         &#x03C6; &#x02D9;      )     (     h
      &#x03B8;   2     0     0    h  &#x03C6;   2      )     (       &#x03B8;
      &#x02D9;           &#x03C6; &#x02D9;       )   ,   {\displaystyle 2T=\mu
      R^{2}{\big [}{\dot {\theta }}^{2}+({\dot {\varphi }}\,\sin \theta )^{2}
      {\big ]}=\mu R^{2}{\big (}{\dot {\theta }}\;\;{\dot {\varphi }}{\big )}
      {\begin{pmatrix}1&0\\0&\sin ^{2}\theta \\\end{pmatrix}}{\begin{pmatrix}
      {\dot {\theta }}\\{\dot {\varphi }}\end{pmatrix}}=\mu {\Big (}{\dot
      {\theta }}\;\;{\dot {\varphi }}{\Big )}{\begin{pmatrix}h_{\theta }^
      {2}&0\\0&h_{\varphi }^{2}\\\end{pmatrix}}{\begin{pmatrix}{\dot {\theta
      }}\\{\dot {\varphi }}\end{pmatrix}},}  [{\displaystyle 2T=\mu R^{2}{\big
      [}{\dot {\theta }}^{2}+({\dot {\varphi }}\,\sin \theta )^{2}{\big ]}=\mu
      R^{2}{\big (}{\dot {\theta }}\;\;{\dot {\varphi }}{\big )}{\begin
      {pmatrix}1&0\\0&\sin ^{2}\theta \\\end{pmatrix}}{\begin{pmatrix}{\dot
      {\theta }}\\{\dot {\varphi }}\end{pmatrix}}=\mu {\Big (}{\dot {\theta
      }}\;\;{\dot {\varphi }}{\Big )}{\begin{pmatrix}h_{\theta }^{2}&0\\0&h_
      {\varphi }^{2}\\\end{pmatrix}}{\begin{pmatrix}{\dot {\theta }}\\{\dot
      {\varphi }}\end{pmatrix}},}]
where      h  &#x03B8;   = R    {\displaystyle h_{\theta }=R\,}  [h_{\theta
}=R\,] and      h  &#x03C6;   = R sin &#x2061; &#x03B8;    {\displaystyle h_
{\varphi }=R\sin \theta \,}  [h_{\varphi }=R\sin \theta \,] are scale_(or
LamÃ©)_factors.
Scale factors are of importance for quantum mechanical applications since they
enter the Laplacian expressed in curvilinear_coordinates. In the case at hand
(constant     R   {\displaystyle R}  [R])
          &#x2207;  2   =   1   h  &#x03B8;    h  &#x03C6;       [    &#x2202;
      &#x2202; &#x03B8;       h  &#x03C6;    h  &#x03B8;       &#x2202;
      &#x2202; &#x03B8;    +   &#x2202;  &#x2202; &#x03C6;       h  &#x03B8;
      h  &#x03C6;       &#x2202;  &#x2202; &#x03C6;     ]  =   1  R  2
      [    1  sin &#x2061; &#x03B8;      &#x2202;  &#x2202; &#x03B8;    sin
      &#x2061; &#x03B8;   &#x2202;  &#x2202; &#x03B8;    +   1   sin  2
      &#x2061; &#x03B8;       &#x2202;  2    &#x2202;  &#x03C6;  2       ]  .
      {\displaystyle \nabla ^{2}={\frac {1}{h_{\theta }h_{\varphi }}}\left[
      {\frac {\partial }{\partial \theta }}{\frac {h_{\varphi }}{h_{\theta }}}
      {\frac {\partial }{\partial \theta }}+{\frac {\partial }{\partial \varphi
      }}{\frac {h_{\theta }}{h_{\varphi }}}{\frac {\partial }{\partial \varphi
      }}\right]={\frac {1}{R^{2}}}\left[{\frac {1}{\sin \theta }}{\frac
      {\partial }{\partial \theta }}\sin \theta {\frac {\partial }{\partial
      \theta }}+{\frac {1}{\sin ^{2}\theta }}{\frac {\partial ^{2}}{\partial
      \varphi ^{2}}}\right].}  [\nabla ^{2}={\frac  {1}{h_{\theta }h_{\varphi
      }}}\left[{\frac  {\partial }{\partial \theta }}{\frac  {h_{\varphi }}{h_
      {\theta }}}{\frac  {\partial }{\partial \theta }}+{\frac  {\partial }
      {\partial \varphi }}{\frac  {h_{\theta }}{h_{\varphi }}}{\frac  {\partial
      }{\partial \varphi }}\right]={\frac  {1}{R^{2}}}\left[{\frac  {1}{\sin
      \theta }}{\frac  {\partial }{\partial \theta }}\sin \theta {\frac
      {\partial }{\partial \theta }}+{\frac  {1}{\sin ^{2}\theta }}{\frac
      {\partial ^{2}}{\partial \varphi ^{2}}}\right].]
The classical Hamiltonian function of the linear rigid rotor is
         H =   1  2 &#x03BC;  R  2       [   p  &#x03B8;   2   +    p  &#x03C6;
      2     sin  2   &#x2061; &#x03B8;     ]  .   {\displaystyle H={\frac {1}
      {2\mu R^{2}}}\left[p_{\theta }^{2}+{\frac {p_{\varphi }^{2}}{\sin ^
      {2}\theta }}\right].}  [H={\frac  {1}{2\mu R^{2}}}\left[p_{{\theta }}^
      {2}+{\frac  {p_{{\varphi }}^{2}}{\sin ^{2}\theta }}\right].]
**** Quantum mechanical linear rigid rotor[edit] ****
The linear rigid rotor model can be used in quantum_mechanics to predict the
rotational energy of a diatomic molecule. The rotational energy depends on the
moment_of_inertia for the system,     I   {\displaystyle I}  [I]. In the center
of_mass reference frame, the moment of inertia is equal to:
         I = &#x03BC;  R  2     {\displaystyle I=\mu R^{2}}  [I=\mu R^{2}]
where     &#x03BC;   {\displaystyle \mu }  [\mu ] is the reduced_mass of the
molecule and     R   {\displaystyle R}  [R] is the distance between the two
atoms.
According to quantum_mechanics, the energy levels of a system can be determined
by solving the SchrÃ¶dinger_equation:
            H &#x005E;    &#x03A8; = E &#x03A8;   {\displaystyle {\hat {H}}\Psi
      =E\Psi }  [{\hat  H}\Psi =E\Psi ]
where     &#x03A8;   {\displaystyle \Psi }  [\Psi ] is the wave_function and
H &#x005E;      {\displaystyle {\hat {H}}}  [\hat H] is the energy
(Hamiltonian) operator. For the rigid rotor in a field-free space, the energy
operator corresponds to the kinetic_energy[1] of the system:
            H &#x005E;    = &#x2212;    &#x210F;  2    2 &#x03BC;     &#x2207;
      2     {\displaystyle {\hat {H}}=-{\frac {\hbar ^{2}}{2\mu }}\nabla ^{2}}
      [{\hat  H}=-{\frac  {\hbar ^{2}}{2\mu }}\nabla ^{2}]
where     &#x210F;   {\displaystyle \hbar }  [\hbar ] is reduced_Planck
constant and      &#x2207;  2     {\displaystyle \nabla ^{2}}  [\nabla ^{2}] is
the Laplacian. The Laplacian is given above in terms of spherical polar
coordinates. The energy operator written in terms of these coordinates is:
            H &#x005E;    = &#x2212;    &#x210F;  2    2 I     [    1  sin
      &#x2061; &#x03B8;      &#x2202;  &#x2202; &#x03B8;     (  sin &#x2061;
      &#x03B8;   &#x2202;  &#x2202; &#x03B8;     )  +   1   sin  2   &#x2061;
      &#x03B8;       &#x2202;  2    &#x2202;  &#x03C6;  2       ]
      {\displaystyle {\hat {H}}=-{\frac {\hbar ^{2}}{2I}}\left[{1 \over \sin
      \theta }{\partial \over \partial \theta }\left(\sin \theta {\partial
      \over \partial \theta }\right)+{1 \over {\sin ^{2}\theta }}{\partial ^{2}
      \over \partial \varphi ^{2}}\right]}  [{\hat  H}=-{\frac  {\hbar ^{2}}
      {2I}}\left[{1 \over \sin \theta }{\partial  \over \partial \theta }\left
      (\sin \theta {\partial  \over \partial \theta }\right)+{1 \over {\sin ^
      {2}\theta }}{\partial ^{2} \over \partial \varphi ^{2}}\right]]
This operator appears also in the SchrÃ¶dinger equation of the hydrogen atom
after the radial part is separated off. The eigenvalue equation becomes
            H &#x005E;     Y  &#x2113;   m   ( &#x03B8; , &#x03C6; ) =
      &#x210F;  2    2 I    &#x2113; ( &#x2113; + 1 )  Y  &#x2113;   m
      ( &#x03B8; , &#x03C6; ) .   {\displaystyle {\hat {H}}Y_{\ell }^{m}(\theta
      ,\varphi )={\frac {\hbar ^{2}}{2I}}\ell (\ell +1)Y_{\ell }^{m}(\theta
      ,\varphi ).}  [{\hat  H}Y_{\ell }^{m}(\theta ,\varphi )={\frac  {\hbar ^
      {2}}{2I}}\ell (\ell +1)Y_{\ell }^{m}(\theta ,\varphi ).]
The symbol      Y  &#x2113;   m   ( &#x03B8; , &#x03C6; )   {\displaystyle Y_
{\ell }^{m}(\theta ,\varphi )}  [Y_{\ell }^{m}(\theta ,\varphi )] represents a
set of functions known as the spherical_harmonics. Note that the energy does
not depend on     m    {\displaystyle m\,}  [m\,]. The energy
          E  &#x2113;   =    &#x210F;  2    2 I    &#x2113;  (  &#x2113; + 1  )
      {\displaystyle E_{\ell }={\hbar ^{2} \over 2I}\ell \left(\ell +1\right)}
      [E_{\ell }={\hbar ^{2} \over 2I}\ell \left(\ell +1\right)]
is     2 &#x2113; + 1   {\displaystyle 2\ell +1}  [2\ell +1]-fold degenerate:
the functions with fixed     &#x2113;    {\displaystyle \ell \,}  [\ell \,] and
m = &#x2212; &#x2113; , &#x2212; &#x2113; + 1 , &#x2026; , &#x2113;
{\displaystyle m=-\ell ,-\ell +1,\dots ,\ell }  [m=-\ell ,-\ell +1,\dots ,\ell
] have the same energy.
Introducing the rotational constant B, we write,
          E  &#x2113;   = B  &#x2113;  (  &#x2113; + 1  )     with    B
      &#x2261;    &#x210F;  2    2 I    .   {\displaystyle E_{\ell }=B\;\ell
      \left(\ell +1\right)\quad {\textrm {with}}\quad B\equiv {\frac {\hbar ^
      {2}}{2I}}.}  [E_{\ell }=B\;\ell \left(\ell +1\right)\quad {\textrm
      {with}}\quad B\equiv {\frac  {\hbar ^{2}}{2I}}.]
In the units of reciprocal_length the rotational constant is,
            B &#x00AF;    &#x2261;   B  h c    =   h  8  &#x03C0;  2   c I    =
      &#x210F;  4 &#x03C0; c &#x03BC;  R  e   2      ,   {\displaystyle {\bar
      {B}}\equiv {\frac {B}{hc}}={\frac {h}{8\pi ^{2}cI}}={\frac {\hbar }{4\pi
      c\mu R_{e}^{2}}},}  [{\displaystyle {\bar {B}}\equiv {\frac {B}{hc}}=
      {\frac {h}{8\pi ^{2}cI}}={\frac {\hbar }{4\pi c\mu R_{e}^{2}}},}]
with c the speed of light. If cgs_units are used for h, c, and I,        B
&#x00AF;      {\displaystyle {\bar {B}}}  [{\bar  B}] is expressed in wave
numbers, cmâ1, a unit that is often used for rotational-vibrational
spectroscopy. The rotational constant        B &#x00AF;    ( R )
{\displaystyle {\bar {B}}(R)}  [{\bar  B}(R)] depends on the distance     R
{\displaystyle R}  [R]. Often one writes      B  e   =    B &#x00AF;    (  R  e
)   {\displaystyle B_{e}={\bar {B}}(R_{e})}  [B_{e}={\bar  B}(R_{e})] where
R  e     {\displaystyle R_{e}}  [R_e] is the equilibrium value of     R
{\displaystyle R}  [R] (the value for which the interaction energy of the atoms
in the rotor has a minimum).
A typical rotational spectrum consists of a series of peaks that correspond to
transitions between levels with different values of the angular momentum
quantum_number (    &#x2113;   {\displaystyle \ell }  [\ell ]). Consequently,
rotational_peaks appear at energies corresponding to an integer multiple of
2    B &#x00AF;      {\displaystyle 2{\bar {B}}}  [2{\bar  B}].
**** Selection rules[edit] ****
Rotational transitions of a molecule occur when the molecule absorbs a photon
[a particle of a quantized electromagnetic (em) field]. Depending on the energy
of the photon (i.e., the wavelength of the em field) this transition may be
seen as a sideband of a vibrational and/or electronic transition. Pure
rotational transitions, in which the vibronic (= vibrational plus electronic)
wave function does not change, occur in the microwave region of the
electromagnetic spectrum.
Typically, rotational transitions can only be observed when the angular
momentum quantum_number changes by 1 (    &#x0394; l = &#x00B1; 1
{\displaystyle \Delta l=\pm 1}  [\Delta l=\pm 1]). This selection rule arises
from a first-order perturbation theory approximation of the time-dependent
SchrÃ¶dinger_equation. According to this treatment, rotational transitions can
only be observed when one or more components of the dipole_operator have a non-
vanishing transition moment. If z is the direction of the electric field
component of the incoming electromagnetic wave, the transition moment is,
         &#x27E8;  &#x03C8;  2    |   &#x03BC;  z    |   &#x03C8;  1   &#x27E9;
      =   (  &#x03BC;  z   )   21   = &#x222B;  &#x03C8;  2   &#x2217;
      &#x03BC;  z    &#x03C8;  1     d  &#x03C4; .   {\displaystyle \langle
      \psi _{2}|\mu _{z}|\psi _{1}\rangle =\left(\mu _{z}\right)_{21}=\int \psi
      _{2}^{*}\mu _{z}\psi _{1}\,\mathrm {d} \tau .}  [\langle \psi _{2}|\mu _
      {z}|\psi _{1}\rangle =\left(\mu _{z}\right)_{{21}}=\int \psi _{2}^{*}\mu
      _{z}\psi _{1}\,{\mathrm  {d}}\tau .]
A transition occurs if this integral is non-zero. By separating the rotational
part of the molecular wavefunction from the vibronic part, one can show that
this means that the molecule must have a permanent dipole_moment. After
integration over the vibronic coordinates the following rotational part of the
transition moment remains,
           (  &#x03BC;  z   )   l , m ;  l &#x2032;  ,  m &#x2032;    =
      &#x03BC;  &#x222B;  0   2 &#x03C0;    d  &#x03D5;  &#x222B;  0   &#x03C0;
      Y   l &#x2032;     m &#x2032;      (  &#x03B8; , &#x03D5;  )   &#x2217;
      cos &#x2061; &#x03B8;   Y  l   m     (  &#x03B8; , &#x03D5;  )    d  cos
      &#x2061; &#x03B8; .   {\displaystyle \left(\mu _{z}\right)_
      {l,m;l',m'}=\mu \int _{0}^{2\pi }\mathrm {d} \phi \int _{0}^{\pi }Y_{l'}^
      {m'}\left(\theta ,\phi \right)^{*}\cos \theta \,Y_{l}^{m}\,\left(\theta
      ,\phi \right)\;\mathrm {d} \cos \theta .}  [\left(\mu _{z}\right)_{
      {l,m;l',m'}}=\mu \int _{0}^{{2\pi }}{\mathrm  {d}}\phi \int _{0}^{\pi }Y_
      {{l'}}^{{m'}}\left(\theta ,\phi \right)^{*}\cos \theta \,Y_{l}^{m}\,\left
      (\theta ,\phi \right)\;{\mathrm  {d}}\cos \theta .]
Here     &#x03BC; cos &#x2061; &#x03B8;    {\displaystyle \mu \cos \theta \,}
[\mu \cos \theta \,] is the z component of the permanent dipole moment. The
moment     &#x03BC;   {\displaystyle \mu }  [\mu ] is the vibronically averaged
component of the dipole_operator. Only the component of the permanent dipole
along the axis of a heteronuclear molecule is non-vanishing. By the use of the
orthogonality of the spherical_harmonics      Y  l   m     (  &#x03B8; ,
&#x03D5;  )    {\displaystyle Y_{l}^{m}\,\left(\theta ,\phi \right)}  [Y_{l}^
{m}\,\left(\theta ,\phi \right)] it is possible to determine which values of
l   {\displaystyle l}  [l],     m   {\displaystyle m}  [m],      l &#x2032;
{\displaystyle l'}  [l'], and      m &#x2032;    {\displaystyle m'}  [m'] will
result in nonzero values for the dipole transition moment integral. This
constraint results in the observed selection rules for the rigid rotor:
         &#x0394; m = 0    and    &#x0394; l = &#x00B1; 1   {\displaystyle
      \Delta m=0\quad {\hbox{and}}\quad \Delta l=\pm 1}  [\Delta m=0\quad
      {\hbox{and}}\quad \Delta l=\pm 1]
**** Non-rigid linear rotor[edit] ****
The rigid rotor is commonly used to describe the rotational energy of diatomic
molecules but it is not a completely accurate description of such molecules.
This is because molecular bonds (and therefore the interatomic distance     R
{\displaystyle R}  [R]) are not completely fixed; the bond between the atoms
stretches out as the molecule rotates faster (higher values of the rotational
quantum_number     l   {\displaystyle l}  [l]). This effect can be accounted
for by introducing a correction factor known as the centrifugal distortion
constant        D &#x00AF;      {\displaystyle {\bar {D}}}  [\bar{D}] (bars on
top of various quantities indicate that these quantities are expressed in
cmâ1):
             E &#x00AF;     l   =    E  l    h c    =    B &#x00AF;    l  (  l
      + 1  )  &#x2212;    D &#x00AF;     l  2     (  l + 1  )   2
      {\displaystyle {\bar {E}}_{l}={E_{l} \over hc}={\bar {B}}l\left
      (l+1\right)-{\bar {D}}l^{2}\left(l+1\right)^{2}}  [{\bar  E}_{l}={E_{l}
      \over hc}={\bar  {B}}l\left(l+1\right)-{\bar  {D}}l^{2}\left(l+1\right)^
      {2}]
where
            D &#x00AF;    =    4     B &#x00AF;     3        &#x03C9; &#x00AF;
      2       {\displaystyle {\bar {D}}={4{\bar {B}}^{3} \over {\bar
      {\boldsymbol {\omega }}}^{2}}}  [{\bar  D}={4{\bar  {B}}^{3} \over {\bar
      {{\boldsymbol  \omega }}}^{2}}]
            &#x03C9; &#x00AF;      {\displaystyle {\bar {\boldsymbol {\omega
      }}}}  [{\bar  {{\boldsymbol  \omega }}}] is the fundamental vibrational
      frequency of the bond (in cmâ1). This frequency is related to the
      reduced mass and the force_constant (bond strength) of the molecule
      according to
            &#x03C9; &#x00AF;    =   1  2 &#x03C0; c       k &#x03BC;
      {\displaystyle {\bar {\boldsymbol {\omega }}}={1 \over 2\pi c}{\sqrt {k
      \over \mu }}}  [{\bar  {{\boldsymbol  \omega }}}={1 \over 2\pi c}{\sqrt
      {k \over \mu }}]
The non-rigid rotor is an acceptably accurate model for diatomic molecules but
is still somewhat imperfect. This is because, although the model does account
for bond stretching due to rotation, it ignores any bond stretching due to
vibrational energy in the bond (anharmonicity in the potential).
***** Arbitrarily shaped rigid rotor[edit] *****
An arbitrarily shaped rigid rotor is a rigid_body of arbitrary shape with its
center_of_mass fixed (or in uniform rectilinear motion) in field-free space R3,
so that its energy consists only of rotational kinetic energy (and possibly
constant translational energy that can be ignored). A rigid body can be
(partially) characterized by the three eigenvalues of its moment_of_inertia
tensor, which are real nonnegative values known as principal moments of
inertia. In microwave_spectroscopy—the spectroscopy based on rotational
transitions—one usually classifies molecules (seen as rigid rotors) as follows:
    * spherical rotors
    * symmetric rotors
          o oblate symmetric rotors
          o prolate symmetric rotors
    * asymmetric rotors
This classification depends on the relative_magnitudes of the principal moments
of inertia.
**** Coordinates of the rigid rotor[edit] ****
Different branches of physics and engineering use different coordinates for the
description of the kinematics of a rigid rotor. In molecular physics Euler
angles are used almost exclusively. In quantum mechanical applications it is
advantageous to use Euler angles in a convention that is a simple extension of
the physical convention of spherical_polar_coordinates.
The first step is the attachment of a right-handed orthonormal frame (3-
dimensional system of orthogonal axes) to the rotor (a body-fixed frame) . This
frame can be attached arbitrarily to the body, but often one uses the principal
axes frame—the normalized eigenvectors of the inertia tensor, which always can
be chosen orthonormal, since the tensor is symmetric. When the rotor possesses
a symmetry-axis, it usually coincides with one of the principal axes. It is
convenient to choose as body-fixed z-axis the highest-order symmetry axis.
One starts by aligning the body-fixed frame with a space-fixed frame
(laboratory axes), so that the body-fixed x, y, and z axes coincide with the
space-fixed X, Y, and Z axis. Secondly, the body and its frame are rotated
actively over a positive angle     &#x03B1;    {\displaystyle \alpha \,}
[\alpha \,] around the z-axis (by the right-hand_rule), which moves the     y
{\displaystyle y}  [y]- to the      y &#x2032;    {\displaystyle y'}  [y']-
axis. Thirdly, one rotates the body and its frame over a positive angle
&#x03B2;    {\displaystyle \beta \,}  [\beta \,] around the      y &#x2032;
{\displaystyle y'}  [y']-axis. The z-axis of the body-fixed frame has after
these two rotations the longitudinal angle     &#x03B1;    {\displaystyle
\alpha \,}  [\alpha \,] (commonly designated by     &#x03C6;    {\displaystyle
\varphi \,}  [\varphi \,]) and the colatitude angle     &#x03B2;
{\displaystyle \beta \,}  [\beta \,] (commonly designated by     &#x03B8;
{\displaystyle \theta \,}  [\theta \,] ), both with respect to the space-fixed
frame. If the rotor were cylindrical symmetric around its z-axis, like the
linear rigid rotor, its orientation in space would be unambiguously specified
at this point.
If the body lacks cylinder (axial) symmetry, a last rotation around its z-axis
(which has polar coordinates     &#x03B2;    {\displaystyle \beta \,}  [\beta
\,] and     &#x03B1;    {\displaystyle \alpha \,}  [\alpha \,] ) is necessary
to specify its orientation completely. Traditionally the last rotation angle is
called     &#x03B3;    {\displaystyle \gamma \,}  [\gamma \,].
The convention_for_Euler_angles described here is known as the      z &#x2033;
&#x2212;  y &#x2032;  &#x2212; z   {\displaystyle z''-y'-z}  [z''-y'-z]
convention; it can be shown (in the same manner as in this_article) that it is
equivalent to the     z &#x2212; y &#x2212; z   {\displaystyle z-y-z}  [z-y-z]
convention in which the order of rotations is reversed.
The total matrix of the three consecutive rotations is the product
          R  ( &#x03B1; , &#x03B2; , &#x03B3; ) =   (    cos &#x2061; &#x03B1;
      &#x2212; sin &#x2061; &#x03B1;   0     sin &#x2061; &#x03B1;   cos
      &#x2061; &#x03B1;   0     0   0   1    )     (    cos &#x2061; &#x03B2;
      0   sin &#x2061; &#x03B2;     0   1   0     &#x2212; sin &#x2061;
      &#x03B2;   0   cos &#x2061; &#x03B2;    )     (    cos &#x2061; &#x03B3;
      &#x2212; sin &#x2061; &#x03B3;   0     sin &#x2061; &#x03B3;   cos
      &#x2061; &#x03B3;   0     0   0   1    )     {\displaystyle \mathbf {R}
      (\alpha ,\beta ,\gamma )={\begin{pmatrix}\cos \alpha &-\sin \alpha
      &0\\\sin \alpha &\cos \alpha &0\\0&0&1\end{pmatrix}}{\begin{pmatrix}\cos
      \beta &0&\sin \beta \\0&1&0\\-\sin \beta &0&\cos \beta \\\end{pmatrix}}
      {\begin{pmatrix}\cos \gamma &-\sin \gamma &0\\\sin \gamma &\cos \gamma
      &0\\0&0&1\end{pmatrix}}}  [{\mathbf  {R}}(\alpha ,\beta ,\gamma )={\begin
      {pmatrix}\cos \alpha &-\sin \alpha &0\\\sin \alpha &\cos \alpha
      &0\\0&0&1\end{pmatrix}}{\begin{pmatrix}\cos \beta &0&\sin \beta
      \\0&1&0\\-\sin \beta &0&\cos \beta \\\end{pmatrix}}{\begin{pmatrix}\cos
      \gamma &-\sin \gamma &0\\\sin \gamma &\cos \gamma &0\\0&0&1\end
      {pmatrix}}]
Let      r  ( 0 )   {\displaystyle \mathbf {r} (0)}  [{\mathbf  {r}}(0)] be the
coordinate vector of an arbitrary point       P     {\displaystyle {\mathcal
{P}}}  [{\mathcal {P}}] in the body with respect to the body-fixed frame. The
elements of      r  ( 0 )   {\displaystyle \mathbf {r} (0)}  [{\mathbf  {r}}
(0)] are the 'body-fixed coordinates' of       P     {\displaystyle {\mathcal
{P}}}  [{\mathcal {P}}]. Initially      r  ( 0 )   {\displaystyle \mathbf {r}
(0)}  [{\mathbf  {r}}(0)] is also the space-fixed coordinate vector of       P
{\displaystyle {\mathcal {P}}}  [{\mathcal {P}}]. Upon rotation of the body,
the body-fixed coordinates of       P     {\displaystyle {\mathcal {P}}}  [
{\mathcal {P}}] do not change, but the space-fixed coordinate vector of       P
{\displaystyle {\mathcal {P}}}  [{\mathcal {P}}] becomes,
          r  ( &#x03B1; , &#x03B2; , &#x03B3; ) =  R  ( &#x03B1; , &#x03B2; ,
      &#x03B3; )  r  ( 0 ) .   {\displaystyle \mathbf {r} (\alpha ,\beta
      ,\gamma )=\mathbf {R} (\alpha ,\beta ,\gamma )\mathbf {r} (0).}  [
      {\mathbf  {r}}(\alpha ,\beta ,\gamma )={\mathbf  {R}}(\alpha ,\beta
      ,\gamma ){\mathbf  {r}}(0).]
In particular, if       P     {\displaystyle {\mathcal {P}}}  [{\mathcal {P}}]
is initially on the space-fixed Z-axis, it has the space-fixed coordinates
          R  ( &#x03B1; , &#x03B2; , &#x03B3; )   (    0     0     r    )   =
      (    r cos &#x2061; &#x03B1; sin &#x2061; &#x03B2;     r sin &#x2061;
      &#x03B1; sin &#x2061; &#x03B2;     r cos &#x2061; &#x03B2;    )   ,
      {\displaystyle \mathbf {R} (\alpha ,\beta ,\gamma ){\begin
      {pmatrix}0\\0\\r\\\end{pmatrix}}={\begin{pmatrix}r\cos \alpha \sin \beta
      \\r\sin \alpha \sin \beta \\r\cos \beta \\\end{pmatrix}},}  [{\mathbf
      {R}}(\alpha ,\beta ,\gamma ){\begin{pmatrix}0\\0\\r\\\end{pmatrix}}=
      {\begin{pmatrix}r\cos \alpha \sin \beta \\r\sin \alpha \sin \beta \\r\cos
      \beta \\\end{pmatrix}},]
which shows the correspondence with the spherical_polar_coordinates (in the
physical convention).
Knowledge of the Euler angles as function of time t and the initial coordinates
r  ( 0 )   {\displaystyle \mathbf {r} (0)}  [{\mathbf  {r}}(0)] determine the
kinematics of the rigid rotor.
**** Classical kinetic energy[edit] ****
The following text forms a generalization of the well-known special case of the
rotational_energy of an object that rotates around one axis.
It will be assumed from here on that the body-fixed frame is a principal axes
frame; it diagonalizes the instantaneous inertia_tensor      I  ( t )
{\displaystyle \mathbf {I} (t)}  [{\mathbf  {I}}(t)] (expressed with respect to
the space-fixed frame), i.e.,
          R  ( &#x03B1; , &#x03B2; , &#x03B3;  )  &#x2212; 1     I  ( t )   R
      ( &#x03B1; , &#x03B2; , &#x03B3; ) =  I  ( 0 )    with     I  ( 0 ) =
      (     I  1     0   0     0    I  2     0     0   0    I  3      )   ,
      {\displaystyle \mathbf {R} (\alpha ,\beta ,\gamma )^{-1}\;\mathbf {I}
      (t)\;\mathbf {R} (\alpha ,\beta ,\gamma )=\mathbf {I} (0)\quad {\hbox
      {with}}\quad \mathbf {I} (0)={\begin{pmatrix}I_{1}&0&0\\0&I_{2}&0\\0&0&I_
      {3}\\\end{pmatrix}},}  [{\mathbf  {R}}(\alpha ,\beta ,\gamma )^{{-1}}\;
      {\mathbf  {I}}(t)\;{\mathbf  {R}}(\alpha ,\beta ,\gamma )={\mathbf  {I}}
      (0)\quad {\hbox{with}}\quad {\mathbf  {I}}(0)={\begin{pmatrix}I_
      {1}&0&0\\0&I_{2}&0\\0&0&I_{3}\\\end{pmatrix}},]
where the Euler angles are time-dependent and in fact determine the time
dependence of      I  ( t )   {\displaystyle \mathbf {I} (t)}  [{\mathbf  {I}}
(t)] by the inverse of this equation. This notation implies that at     t = 0
{\displaystyle t=0}  [t=0] the Euler angles are zero, so that at     t = 0
{\displaystyle t=0}  [t=0] the body-fixed frame coincides with the space-fixed
frame.
The classical kinetic energy T of the rigid rotor can be expressed in different
ways:
    * as a function of angular velocity
    * in Lagrangian form
    * as a function of angular momentum
    * in Hamiltonian form.
Since each of these forms has its use and can be found in textbooks we will
present all of them.
*** Angular velocity form[edit] ***
As a function of angular velocity T reads,
         T =   1 2    [   I  1    &#x03C9;  x   2   +  I  2    &#x03C9;  y   2
      +  I  3    &#x03C9;  z   2    ]    {\displaystyle T={\frac {1}{2}}\left
      [I_{1}\omega _{x}^{2}+I_{2}\omega _{y}^{2}+I_{3}\omega _{z}^{2}\right]}
      [T={\frac  {1}{2}}\left[I_{1}\omega _{x}^{2}+I_{2}\omega _{y}^{2}+I_
      {3}\omega _{z}^{2}\right]]
with
           (     &#x03C9;  x        &#x03C9;  y        &#x03C9;  z      )   =
      (    &#x2212; sin &#x2061; &#x03B2; cos &#x2061; &#x03B3;   sin &#x2061;
      &#x03B3;   0     sin &#x2061; &#x03B2; sin &#x2061; &#x03B3;   cos
      &#x2061; &#x03B3;   0     cos &#x2061; &#x03B2;   0   1    )
      (       &#x03B1; &#x02D9;           &#x03B2; &#x02D9;           &#x03B3;
      &#x02D9;       )   .   {\displaystyle {\begin{pmatrix}\omega _{x}\\\omega
      _{y}\\\omega _{z}\\\end{pmatrix}}={\begin{pmatrix}-\sin \beta \cos \gamma
      &\sin \gamma &0\\\sin \beta \sin \gamma &\cos \gamma &0\\\cos \beta
      &0&1\\\end{pmatrix}}{\begin{pmatrix}{\dot {\alpha }}\\{\dot {\beta }}\\
      {\dot {\gamma }}\\\end{pmatrix}}.}  [{\begin{pmatrix}\omega _{x}\\\omega
      _{y}\\\omega _{z}\\\end{pmatrix}}={\begin{pmatrix}-\sin \beta \cos \gamma
      &\sin \gamma &0\\\sin \beta \sin \gamma &\cos \gamma &0\\\cos \beta
      &0&1\\\end{pmatrix}}{\begin{pmatrix}{\dot  {\alpha }}\\{\dot  {\beta }}\\
      {\dot  {\gamma }}\\\end{pmatrix}}.]
The vector      &#x03C9;  = (  &#x03C9;  x   ,  &#x03C9;  y   ,  &#x03C9;  z
)   {\displaystyle {\boldsymbol {\omega }}=(\omega _{x},\omega _{y},\omega _
{z})}  [{\boldsymbol  {\omega }}=(\omega _{x},\omega _{y},\omega _{z})]
contains the components of the angular_velocity of the rotor expressed with
respect to the body-fixed frame. It can be shown that      &#x03C9;
{\displaystyle {\boldsymbol {\omega }}}  [{\boldsymbol {\omega }}] is not the
time derivative of any vector, in contrast to the usual definition_of_velocity.
[2] The dots over the time-dependent Euler angles indicate time_derivatives.
The angular velocity satisfies equations of motion known as Euler's_equations
(with zero applied torque, since by assumption the rotor is in field-free
space).
*** Lagrange form[edit] ***
Backsubstitution of the expression of      &#x03C9;    {\displaystyle
{\boldsymbol {\omega }}}  [{\boldsymbol {\omega }}] into T gives the kinetic
energy in Lagrange_form (as a function of the time derivatives of the Euler
angles). In matrix-vector notation,
         2 T =   (       &#x03B1; &#x02D9;         &#x03B2; &#x02D9;
      &#x03B3; &#x02D9;       )     g     (       &#x03B1; &#x02D9;
      &#x03B2; &#x02D9;           &#x03B3; &#x02D9;       )   ,
      {\displaystyle 2T={\begin{pmatrix}{\dot {\alpha }}&{\dot {\beta }}&{\dot
      {\gamma }}\end{pmatrix}}\;\mathbf {g} \;{\begin{pmatrix}{\dot {\alpha
      }}\\{\dot {\beta }}\\{\dot {\gamma }}\\\end{pmatrix}},}  [2T={\begin
      {pmatrix}{\dot  {\alpha }}&{\dot  {\beta }}&{\dot  {\gamma }}\end
      {pmatrix}}\;{\mathbf  {g}}\;{\begin{pmatrix}{\dot  {\alpha }}\\{\dot
      {\beta }}\\{\dot  {\gamma }}\\\end{pmatrix}},]
where      g    {\displaystyle \mathbf {g} }  [\mathbf {g} ] is the metric
tensor expressed in Euler angles—a non-orthogonal system of curvilinear
coordinates—
          g  =   (     I  1    sin  2   &#x2061; &#x03B2;  cos  2   &#x2061;
      &#x03B3; +  I  2    sin  2   &#x2061; &#x03B2;  sin  2   &#x2061;
      &#x03B3; +  I  3    cos  2   &#x2061; &#x03B2;   (  I  2   &#x2212;  I  1
      ) sin &#x2061; &#x03B2; sin &#x2061; &#x03B3; cos &#x2061; &#x03B3;    I
      3   cos &#x2061; &#x03B2;     (  I  2   &#x2212;  I  1   ) sin &#x2061;
      &#x03B2; sin &#x2061; &#x03B3; cos &#x2061; &#x03B3;    I  1    sin  2
      &#x2061; &#x03B3; +  I  2    cos  2   &#x2061; &#x03B3;   0      I  3
      cos &#x2061; &#x03B2;   0    I  3      )   .   {\displaystyle \mathbf {g}
      ={\begin{pmatrix}I_{1}\sin ^{2}\beta \cos ^{2}\gamma +I_{2}\sin ^{2}\beta
      \sin ^{2}\gamma +I_{3}\cos ^{2}\beta &(I_{2}-I_{1})\sin \beta \sin \gamma
      \cos \gamma &I_{3}\cos \beta \\(I_{2}-I_{1})\sin \beta \sin \gamma \cos
      \gamma &I_{1}\sin ^{2}\gamma +I_{2}\cos ^{2}\gamma &0\\I_{3}\cos \beta
      &0&I_{3}\\\end{pmatrix}}.}  [{\mathbf  {g}}={\begin{pmatrix}I_{1}\sin ^
      {2}\beta \cos ^{2}\gamma +I_{2}\sin ^{2}\beta \sin ^{2}\gamma +I_{3}\cos
      ^{2}\beta &(I_{2}-I_{1})\sin \beta \sin \gamma \cos \gamma &I_{3}\cos
      \beta \\(I_{2}-I_{1})\sin \beta \sin \gamma \cos \gamma &I_{1}\sin ^
      {2}\gamma +I_{2}\cos ^{2}\gamma &0\\I_{3}\cos \beta &0&I_{3}\\\end
      {pmatrix}}.]
*** Angular momentum form[edit] ***
Often the kinetic energy is written as a function of the angular_momentum
L    {\displaystyle \mathbf {L} }  [\mathbf {L} ] of the rigid rotor. With
respect to the body-fixed frame it has the components       L  i
{\displaystyle \quad L_{i}}  [\quad L_{i}], and can be shown to be related to
the angular velocity,
          L  =  I  ( 0 )   &#x03C9;     or     L  i   =    &#x2202; T
      &#x2202;  &#x03C9;  i      ,   i = x ,  y ,  z .   {\displaystyle \mathbf
      {L} =\mathbf {I} (0)\;{\boldsymbol {\omega }}\quad {\hbox{or}}\quad L_
      {i}={\frac {\partial T}{\partial \omega _{i}}},\;\;i=x,\,y,\,z.}  [
      {\mathbf  {L}}={\mathbf  {I}}(0)\;{\boldsymbol  {\omega }}\quad {\hbox
      {or}}\quad L_{i}={\frac  {\partial T}{\partial \omega _
      {i}}},\;\;i=x,\,y,\,z.]
This angular momentum is a conserved (time-independent) quantity if viewed from
a stationary space-fixed frame. Since the body-fixed frame moves (depends on
time) the components       L  i     {\displaystyle \quad L_{i}}  [\quad L_{i}]
are not time independent. If we were to represent      L    {\displaystyle
\mathbf {L} }  [\mathbf {L} ] with respect to the stationary space-fixed frame,
we would find time independent expressions for its components.
The kinetic energy is expressed in terms of the angular momentum by
         T =   1 2    [     L  x   2    I  1     +    L  y   2    I  2     +
      L  z   2    I  3      ]  .   {\displaystyle T={\frac {1}{2}}\left[{\frac
      {L_{x}^{2}}{I_{1}}}+{\frac {L_{y}^{2}}{I_{2}}}+{\frac {L_{z}^{2}}{I_
      {3}}}\right].}  [T={\frac  {1}{2}}\left[{\frac  {L_{x}^{2}}{I_{1}}}+
      {\frac  {L_{y}^{2}}{I_{2}}}+{\frac  {L_{z}^{2}}{I_{3}}}\right].]
*** Hamilton form[edit] ***
The Hamilton_form of the kinetic energy is written in terms of generalized
momenta
           (     p  &#x03B1;        p  &#x03B2;        p  &#x03B3;      )
      &#xA0;     =    d e f      &#xA0;   (    &#x2202; T  /   &#x2202;
      &#x03B1; &#x02D9;         &#x2202; T  /   &#x2202;    &#x03B2; &#x02D9;
      &#x2202; T  /   &#x2202;    &#x03B3; &#x02D9;        )   =  g
      (         &#x03B1; &#x02D9;           &#x03B2; &#x02D9;
      &#x03B3; &#x02D9;       )   ,   {\displaystyle {\begin{pmatrix}p_{\alpha
      }\\p_{\beta }\\p_{\gamma }\\\end{pmatrix}}\ {\stackrel {\mathrm {def} }
      {=}}\ {\begin{pmatrix}\partial T/{\partial {\dot {\alpha }}}\\\partial T/
      {\partial {\dot {\beta }}}\\\partial T/{\partial {\dot {\gamma }}}\\\end
      {pmatrix}}=\mathbf {g} {\begin{pmatrix}\;\,{\dot {\alpha }}\\{\dot {\beta
      }}\\{\dot {\gamma }}\\\end{pmatrix}},}  [{\begin{pmatrix}p_{\alpha }\\p_
      {\beta }\\p_{\gamma }\\\end{pmatrix}}\ {\stackrel  {{\mathrm  {def}}}
      {=}}\ {\begin{pmatrix}\partial T/{\partial {\dot  {\alpha }}}\\\partial
      T/{\partial {\dot  {\beta }}}\\\partial T/{\partial {\dot  {\gamma
      }}}\\\end{pmatrix}}={\mathbf  {g}}{\begin{pmatrix}\;\,{\dot  {\alpha }}\\
      {\dot  {\beta }}\\{\dot  {\gamma }}\\\end{pmatrix}},]
where it is used that the      g    {\displaystyle \mathbf {g} }  [\mathbf {g}
] is symmetric. In Hamilton form the kinetic energy is,
         2 T =   (     p  &#x03B1;      p  &#x03B2;      p  &#x03B3;      )
      g   &#x2212; 1      (     p  &#x03B1;        p  &#x03B2;        p
      &#x03B3;      )   ,   {\displaystyle 2T={\begin{pmatrix}p_{\alpha }&p_
      {\beta }&p_{\gamma }\end{pmatrix}}\;\mathbf {g} ^{-1}\;{\begin{pmatrix}p_
      {\alpha }\\p_{\beta }\\p_{\gamma }\\\end{pmatrix}},}  [2T={\begin
      {pmatrix}p_{{\alpha }}&p_{{\beta }}&p_{{\gamma }}\end{pmatrix}}\;{\mathbf
      {g}}^{{-1}}\;{\begin{pmatrix}p_{{\alpha }}\\p_{{\beta }}\\p_{{\gamma
      }}\\\end{pmatrix}},]
with the inverse metric tensor given by
            sin  2   &#x2061; &#x03B2;       g   &#x2212; 1   =
      {\displaystyle {\scriptstyle \sin ^{2}\beta }\;\;\mathbf {g} ^{-1}=}  [
      {\scriptstyle \sin ^{2}\beta }\;\;{\mathbf  {g}}^{{-1}}=]
           (        cos  2   &#x2061; &#x03B3;   I  1     +     sin  2
      &#x2061; &#x03B3;   I  2        (    1  I  2     &#x2212;   1  I  1
      )    sin &#x2061; &#x03B2; sin &#x2061; &#x03B3; cos &#x2061; &#x03B3;
      &#x2212;    cos &#x2061; &#x03B2;  cos  2   &#x2061; &#x03B3;   I  1
      &#x2212;    cos &#x2061; &#x03B2;  sin  2   &#x2061; &#x03B3;   I  2
      (    1  I  2     &#x2212;   1  I  1      )    sin &#x2061; &#x03B2; sin
      &#x2061; &#x03B3; cos &#x2061; &#x03B3;         sin  2   &#x2061;
      &#x03B2;  sin  2   &#x2061; &#x03B3;   I  1     +     sin  2   &#x2061;
      &#x03B2;  cos  2   &#x2061; &#x03B3;   I  2        (    1  I  1
      &#x2212;   1  I  2      )    sin &#x2061; &#x03B2; cos &#x2061; &#x03B2;
      sin &#x2061; &#x03B3; cos &#x2061; &#x03B3;       &#x2212;    cos
      &#x2061; &#x03B2;  cos  2   &#x2061; &#x03B3;   I  1     &#x2212;    cos
      &#x2061; &#x03B2;  sin  2   &#x2061; &#x03B3;   I  2        (    1  I  1
      &#x2212;   1  I  2      )    sin &#x2061; &#x03B2; cos &#x2061; &#x03B2;
      sin &#x2061; &#x03B3; cos &#x2061; &#x03B3;         cos  2   &#x2061;
      &#x03B2;  cos  2   &#x2061; &#x03B3;   I  1     +     cos  2   &#x2061;
      &#x03B2;  sin  2   &#x2061; &#x03B3;   I  2     +     sin  2   &#x2061;
      &#x03B2;   I  3        )   .   {\displaystyle {\begin{pmatrix}{\frac
      {\cos ^{2}\gamma }{I_{1}}}+{\frac {\sin ^{2}\gamma }{I_{2}}}&\left({\frac
      {1}{I_{2}}}-{\frac {1}{I_{1}}}\right){\scriptstyle \sin \beta \sin \gamma
      \cos \gamma }&-{\frac {\cos \beta \cos ^{2}\gamma }{I_{1}}}-{\frac {\cos
      \beta \sin ^{2}\gamma }{I_{2}}}\\\left({\frac {1}{I_{2}}}-{\frac {1}{I_
      {1}}}\right){\scriptstyle \sin \beta \sin \gamma \cos \gamma }&{\frac
      {\sin ^{2}\beta \sin ^{2}\gamma }{I_{1}}}+{\frac {\sin ^{2}\beta \cos ^
      {2}\gamma }{I_{2}}}&\left({\frac {1}{I_{1}}}-{\frac {1}{I_{2}}}\right)
      {\scriptstyle \sin \beta \cos \beta \sin \gamma \cos \gamma }\\-{\frac
      {\cos \beta \cos ^{2}\gamma }{I_{1}}}-{\frac {\cos \beta \sin ^{2}\gamma
      }{I_{2}}}&\left({\frac {1}{I_{1}}}-{\frac {1}{I_{2}}}\right){\scriptstyle
      \sin \beta \cos \beta \sin \gamma \cos \gamma }&{\frac {\cos ^{2}\beta
      \cos ^{2}\gamma }{I_{1}}}+{\frac {\cos ^{2}\beta \sin ^{2}\gamma }{I_
      {2}}}+{\frac {\sin ^{2}\beta }{I_{3}}}\\\end{pmatrix}}.}  [{\begin
      {pmatrix}{\frac  {\cos ^{2}\gamma }{I_{1}}}+{\frac  {\sin ^{2}\gamma }{I_
      {2}}}&\left({\frac  {1}{I_{2}}}-{\frac  {1}{I_{1}}}\right){\scriptstyle
      \sin \beta \sin \gamma \cos \gamma }&-{\frac  {\cos \beta \cos ^{2}\gamma
      }{I_{1}}}-{\frac  {\cos \beta \sin ^{2}\gamma }{I_{2}}}\\\left({\frac
      {1}{I_{2}}}-{\frac  {1}{I_{1}}}\right){\scriptstyle \sin \beta \sin
      \gamma \cos \gamma }&{\frac  {\sin ^{2}\beta \sin ^{2}\gamma }{I_{1}}}+
      {\frac  {\sin ^{2}\beta \cos ^{2}\gamma }{I_{2}}}&\left({\frac  {1}{I_
      {1}}}-{\frac  {1}{I_{2}}}\right){\scriptstyle \sin \beta \cos \beta \sin
      \gamma \cos \gamma }\\-{\frac  {\cos \beta \cos ^{2}\gamma }{I_{1}}}-
      {\frac  {\cos \beta \sin ^{2}\gamma }{I_{2}}}&\left({\frac  {1}{I_{1}}}-
      {\frac  {1}{I_{2}}}\right){\scriptstyle \sin \beta \cos \beta \sin \gamma
      \cos \gamma }&{\frac  {\cos ^{2}\beta \cos ^{2}\gamma }{I_{1}}}+{\frac
      {\cos ^{2}\beta \sin ^{2}\gamma }{I_{2}}}+{\frac  {\sin ^{2}\beta }{I_
      {3}}}\\\end{pmatrix}}.]
This inverse tensor is needed to obtain the Laplace-Beltrami_operator, which
(multiplied by     &#x2212;  &#x210F;  2     {\displaystyle -\hbar ^{2}}  [-
\hbar ^{2}]) gives the quantum mechanical energy operator of the rigid rotor.
The classical Hamiltonian given above can be rewritten to the following
expression, which is needed in the phase integral arising in the classical
statistical mechanics of rigid rotors,
             T   =     1  2  I  1    sin  2   &#x2061; &#x03B2;      (  (  p
      &#x03B1;   &#x2212;  p  &#x03B3;   cos &#x2061; &#x03B2; ) cos &#x2061;
      &#x03B3; &#x2212;  p  &#x03B2;   sin &#x2061; &#x03B2; sin &#x2061;
      &#x03B3;  )   2         +   1  2  I  2    sin  2   &#x2061; &#x03B2;
      (  (  p  &#x03B1;   &#x2212;  p  &#x03B3;   cos &#x2061; &#x03B2; ) sin
      &#x2061; &#x03B3; +  p  &#x03B2;   sin &#x2061; &#x03B2; cos &#x2061;
      &#x03B3;  )   2   +    p  &#x03B3;   2    2  I  3      .
      {\displaystyle {\begin{array}{lcl}T&=&{\frac {1}{2I_{1}\sin ^{2}\beta
      }}\left((p_{\alpha }-p_{\gamma }\cos \beta )\cos \gamma -p_{\beta }\sin
      \beta \sin \gamma \right)^{2}\\&&+{\frac {1}{2I_{2}\sin ^{2}\beta }}\left
      ((p_{\alpha }-p_{\gamma }\cos \beta )\sin \gamma +p_{\beta }\sin \beta
      \cos \gamma \right)^{2}+{\frac {p_{\gamma }^{2}}{2I_{3}}}.\\\end{array}}}
      [{\begin{array}{lcl}T&=&{\frac  {1}{2I_{1}\sin ^{2}\beta }}\left((p_
      {\alpha }-p_{\gamma }\cos \beta )\cos \gamma -p_{\beta }\sin \beta \sin
      \gamma \right)^{2}\\&&+{\frac  {1}{2I_{2}\sin ^{2}\beta }}\left((p_
      {\alpha }-p_{\gamma }\cos \beta )\sin \gamma +p_{\beta }\sin \beta \cos
      \gamma \right)^{2}+{\frac  {p_{\gamma }^{2}}{2I_{3}}}.\\\end{array}}]
**** Quantum mechanical rigid rotor[edit] ****
See also: Rotational_spectroscopy
As usual quantization is performed by the replacement of the generalized
momenta by operators that give first derivatives with respect to its
canonically_conjugate variables (positions). Thus,
          p  &#x03B1;   &#x27F6; &#x2212; i &#x210F;   &#x2202;  &#x2202;
      &#x03B1;      {\displaystyle p_{\alpha }\longrightarrow -i\hbar {\frac
      {\partial }{\partial \alpha }}}  [p_{\alpha }\longrightarrow -i\hbar
      {\frac  {\partial }{\partial \alpha }}]
and similarly for      p  &#x03B2;     {\displaystyle p_{\beta }}  [p_{\beta }]
and      p  &#x03B3;     {\displaystyle p_{\gamma }}  [p_{\gamma }]. It is
remarkable that this rule replaces the fairly complicated function      p
&#x03B1;     {\displaystyle p_{\alpha }}  [p_{\alpha }] of all three Euler
angles, time derivatives of Euler angles, and inertia moments (characterizing
the rigid rotor) by a simple differential operator that does not depend on time
or inertia moments and differentiates to one Euler angle only.
The quantization rule is sufficient to obtain the operators that correspond
with the classical angular momenta. There are two kinds: space-fixed and body-
fixed angular momentum operators. Both are vector operators, i.e., both have
three components that transform as vector components among themselves upon
rotation of the space-fixed and the body-fixed frame, respectively. The
explicit form of the rigid rotor angular momentum operators is given here (but
beware, they must be multiplied with     &#x210F;   {\displaystyle \hbar }
[\hbar ]). The body-fixed angular momentum operators are written as          P
&#x005E;     i     {\displaystyle {\hat {\mathcal {P}}}_{i}}  [{\hat  {
{\mathcal  {P}}}}_{i}]. They satisfy anomalous_commutation_relations.
The quantization rule is not sufficient to obtain the kinetic energy operator
from the classical Hamiltonian. Since classically      p  &#x03B2;
{\displaystyle p_{\beta }}  [p_{\beta }] commutes with     cos &#x2061;
&#x03B2;   {\displaystyle \cos \beta }  [\cos \beta ] and     sin &#x2061;
&#x03B2;   {\displaystyle \sin \beta }  [\sin \beta ] and the inverses of these
functions, the position of these trigonometric functions in the classical
Hamiltonian is arbitrary. After quantization the commutation does no longer
hold and the order of operators and functions in the Hamiltonian (energy
operator) becomes a point of concern. Podolsky[1] proposed in 1928 that the
Laplace-Beltrami_operator (times     &#x2212;    1 2     &#x210F;  2
{\displaystyle -{\tfrac {1}{2}}\hbar ^{2}}  [-{\tfrac  {1}{2}}\hbar ^{2}]) has
the appropriate form for the quantum mechanical kinetic energy operator. This
operator has the general form (summation convention: sum over repeated
indices—in this case over the three Euler angles      q  1   ,   q  2   ,   q
3   &#x2261; &#x03B1; ,  &#x03B2; ,  &#x03B3;   {\displaystyle q^{1},\,q^
{2},\,q^{3}\equiv \alpha ,\,\beta ,\,\gamma }  [q^{1},\,q^{2},\,q^{3}\equiv
\alpha ,\,\beta ,\,\gamma ]):
            H &#x005E;    = &#x2212;     &#x210F;  2   2      |  g   |
      &#x2212; 1  /  2     &#x2202;  &#x2202;  q  i       |  g   |   1  /  2
      g  i j     &#x2202;  &#x2202;  q  j      ,   {\displaystyle {\hat {H}}=-
      {\tfrac {\hbar ^{2}}{2}}\;|g|^{-1/2}{\frac {\partial }{\partial q^
      {i}}}|g|^{1/2}g^{ij}{\frac {\partial }{\partial q^{j}}},}  [{\hat  {H}}=-
      {\tfrac  {\hbar ^{2}}{2}}\;|g|^{{-1/2}}{\frac  {\partial }{\partial q^
      {i}}}|g|^{{1/2}}g^{{ij}}{\frac  {\partial }{\partial q^{j}}},]
where      |  g  |    {\displaystyle |g|}  [|g|] is the determinant of the g-
tensor:
          |  g  |  =  I  1     I  2     I  3     sin  2   &#x2061; &#x03B2;
      and     g  i j   = (   g   &#x2212; 1    )  i j   .   {\displaystyle
      |g|=I_{1}\,I_{2}\,I_{3}\,\sin ^{2}\beta \quad {\hbox{and}}\quad g^{ij}=
      (\mathbf {g} ^{-1})_{ij}.}  [|g|=I_{1}\,I_{2}\,I_{3}\,\sin ^{2}\beta
      \quad {\hbox{and}}\quad g^{{ij}}=({\mathbf  {g}}^{{-1}})_{{ij}}.]
Given the inverse of the metric tensor above, the explicit form of the kinetic
energy operator in terms of Euler angles follows by simple substitution. (Note:
The corresponding eigenvalue equation gives the SchrÃ¶dinger_equation for the
rigid rotor in the form that it was solved for the first time by Kronig and
Rabi[3] (for the special case of the symmetric rotor). This is one of the few
cases where the SchrÃ¶dinger equation can be solved analytically. All these
cases were solved within a year of the formulation of the SchrÃ¶dinger
equation.)
Nowadays it is common to proceed as follows. It can be shown that        H
&#x005E;      {\displaystyle {\hat {H}}}  [{\hat {H}}] can be expressed in
body-fixed angular momentum operators (in this proof one must carefully commute
differential operators with trigonometric functions). The result has the same
appearance as the classical formula expressed in body-fixed coordinates,
            H &#x005E;    =    1 2     [       P    x   2    I  1     +      P
      y   2    I  2     +      P    z   2    I  3      ]  .   {\displaystyle
      {\hat {H}}={\tfrac {1}{2}}\left[{\frac {{\mathcal {P}}_{x}^{2}}{I_{1}}}+
      {\frac {{\mathcal {P}}_{y}^{2}}{I_{2}}}+{\frac {{\mathcal {P}}_{z}^{2}}
      {I_{3}}}\right].}  [{\hat  {H}}={\tfrac  {1}{2}}\left[{\frac  {{\mathcal
      {P}}_{x}^{2}}{I_{1}}}+{\frac  {{\mathcal  {P}}_{y}^{2}}{I_{2}}}+{\frac  {
      {\mathcal  {P}}_{z}^{2}}{I_{3}}}\right].]
The action of the          P  &#x005E;     i     {\displaystyle {\hat {\mathcal
{P}}}_{i}}  [{\hat  {{\mathcal  {P}}}}_{i}] on the Wigner_D-matrix is simple.
In particular
            P    2     D   m &#x2032;  m   j   ( &#x03B1; , &#x03B2; , &#x03B3;
      )  &#x2217;   =  &#x210F;  2   j ( j + 1 )  D   m &#x2032;  m   j
      ( &#x03B1; , &#x03B2; , &#x03B3;  )  &#x2217;      with       P    2   =
      P    x   2   +    P    y   2   +    P    z   2   ,   {\displaystyle
      {\mathcal {P}}^{2}\,D_{m'm}^{j}(\alpha ,\beta ,\gamma )^{*}=\hbar ^{2}j
      (j+1)D_{m'm}^{j}(\alpha ,\beta ,\gamma )^{*}\quad {\hbox{with}}\quad
      {\mathcal {P}}^{2}={\mathcal {P}}_{x}^{2}+{\mathcal {P}}_{y}^{2}+
      {\mathcal {P}}_{z}^{2},}  [{\mathcal  {P}}^{2}\,D_{{m'm}}^{j}(\alpha
      ,\beta ,\gamma )^{*}=\hbar ^{2}j(j+1)D_{{m'm}}^{j}(\alpha ,\beta ,\gamma
      )^{*}\quad {\hbox{with}}\quad {\mathcal  {P}}^{2}={\mathcal  {P}}_{x}^
      {2}+{\mathcal  {P}}_{y}^{2}+{\mathcal  {P}}_{z}^{2},]
so that the SchrÃ¶dinger equation for the spherical rotor (    I =  I  1   =  I
2   =  I  3     {\displaystyle I=I_{1}=I_{2}=I_{3}}  [I=I_{1}=I_{2}=I_{3}]) is
solved with the     ( 2 j + 1  )  2     {\displaystyle (2j+1)^{2}}  [(2j+1)^
{2}] degenerate energy equal to          &#x210F;  2   j ( j + 1 )   2 I
{\displaystyle {\tfrac {\hbar ^{2}j(j+1)}{2I}}}  [{\tfrac  {\hbar ^{2}j(j+1)}
{2I}}].
The symmetric top (= symmetric rotor) is characterized by      I  1   =  I  2
{\displaystyle I_{1}=I_{2}}  [I_{1}=I_{2}]. It is a prolate (cigar shaped) top
if      I  3   <  I  1   =  I  2     {\displaystyle I_{3}<I_{1}=I_{2}}  [I_
{3}<I_{1}=I_{2}]. In the latter case we write the Hamiltonian as
            H &#x005E;    =    1 2     [       P    2    I  1     +    P    z
      2     (     1  I  3     &#x2212;   1  I  1       )    ]  ,
      {\displaystyle {\hat {H}}={\tfrac {1}{2}}\left[{\frac {{\mathcal {P}}^
      {2}}{I_{1}}}+{\mathcal {P}}_{z}^{2}{\Big (}{\frac {1}{I_{3}}}-{\frac {1}
      {I_{1}}}{\Big )}\right],}  [{\hat  {H}}={\tfrac  {1}{2}}\left[{\frac  {
      {\mathcal  {P}}^{2}}{I_{1}}}+{\mathcal  {P}}_{z}^{2}{\Big (}{\frac  {1}
      {I_{3}}}-{\frac  {1}{I_{1}}}{\Big )}\right],]
and use that
            P    z   2     D  m k   j   ( &#x03B1; , &#x03B2; , &#x03B3;  )
      &#x2217;   =  &#x210F;  2    k  2     D  m k   j   ( &#x03B1; , &#x03B2;
      , &#x03B3;  )  &#x2217;   .   {\displaystyle {\mathcal {P}}_{z}^{2}\,D_
      {mk}^{j}(\alpha ,\beta ,\gamma )^{*}=\hbar ^{2}k^{2}\,D_{mk}^{j}(\alpha
      ,\beta ,\gamma )^{*}.}  [{\mathcal  {P}}_{z}^{2}\,D_{{mk}}^{j}(\alpha
      ,\beta ,\gamma )^{*}=\hbar ^{2}k^{2}\,D_{{mk}}^{j}(\alpha ,\beta ,\gamma
      )^{*}.]
Hence
            H &#x005E;      D  m k   j   ( &#x03B1; , &#x03B2; , &#x03B3;  )
      &#x2217;   =  E  j k    D  m k   j   ( &#x03B1; , &#x03B2; , &#x03B3;  )
      &#x2217;      with     E  j k    /   &#x210F;  2   =    j ( j + 1 )   2
      I  1      +  k  2    (    1  2  I  3      &#x2212;   1  2  I  1       )
      .   {\displaystyle {\hat {H}}\,D_{mk}^{j}(\alpha ,\beta ,\gamma )^{*}=E_
      {jk}D_{mk}^{j}(\alpha ,\beta ,\gamma )^{*}\quad {\hbox{with}}\quad E_
      {jk}/\hbar ^{2}={\frac {j(j+1)}{2I_{1}}}+k^{2}\left({\frac {1}{2I_{3}}}-
      {\frac {1}{2I_{1}}}\right).}  [{\hat  {H}}\,D_{{mk}}^{j}(\alpha ,\beta
      ,\gamma )^{*}=E_{{jk}}D_{{mk}}^{j}(\alpha ,\beta ,\gamma )^{*}\quad
      {\hbox{with}}\quad E_{{jk}}/\hbar ^{2}={\frac  {j(j+1)}{2I_{1}}}+k^
      {2}\left({\frac  {1}{2I_{3}}}-{\frac  {1}{2I_{1}}}\right).]
The eigenvalue      E  j 0     {\displaystyle E_{j0}}  [E_{{j0}}] is     2 j +
1   {\displaystyle 2j+1}  [2j+1]-fold degenerate, for all eigenfunctions with
m = &#x2212; j , &#x2212; j + 1 , &#x2026; , j   {\displaystyle m=-j,-j+1,\dots
,j}  [m=-j,-j+1,\dots ,j] have the same eigenvalue. The energies with |k| > 0
are     2 ( 2 j + 1 )   {\displaystyle 2(2j+1)}  [2(2j+1)]-fold degenerate.
This exact solution of the SchrÃ¶dinger equation of the symmetric top was first
found in 1927.[3]
The asymmetric top problem (     I  1   &#x2260;  I  2   &#x2260;  I  3
{\displaystyle I_{1}\neq I_{2}\neq I_{3}}  [I_{1}\neq I_{2}\neq I_{3}]) is not
exactly soluble.
***** Direct experimental observation of molecular rotations[edit] *****
For a long time, molecular rotations could not be directly observed
experimentally. Only measurement techniques with atomic resolution made it
possible to detect the rotation of a single molecule.[4][5] At low
temperatures, the rotations of molecules (or part thereof) can be frozen. This
could be directly visualized by Scanning_tunneling_microscopy i.e., the
stabilization could be explained at higher temperatures by the rotational
entropy.[5] The direct observation of rotational excitation at single molecule
level was achieved recently using inelastic electron tunneling spectroscopy
with the scanning tunneling microscope. The rotational excitation of molecular
hydrogen and its isotopes were detected.[6][7]
***** See also[edit] *****
    * Balancing_machine
    * Gyroscope
    * Infrared_spectroscopy
    * Rigid_body
    * Rotational_spectroscopy
    * Spectroscopy
    * Vibrational_spectroscopy
    * Quantum_rotor_model
***** References[edit] *****
   1. ^ a bPodolsky, B. (1928). "Quantum-Mechanically Correct Form of
      Hamiltonian Function for Conservative Systems". Phys. Rev. 32 (5): 812.
      Bibcode:1928PhRv...32..812P. doi:10.1103/PhysRev.32.812.
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
   3. ^ Chapter 4.9 of Goldstein, H.; Poole, C. P.; Safko, J. L. (2001).
      Classical Mechanics (Third ed.). San Francisco: Addison Wesley Publishing
      Company.
   4. ISBN 0-201-65702-3.
   5. ^ a bR. de L. Kronig and I. I. Rabi (1927). "The Symmetrical Top in the
      Undulatory Mechanics". Phys. Rev. 29 (2): 262â269. Bibcode:
      1927PhRv...29..262K. doi:10.1103/PhysRev.29.262.
   6. ^J. K. Gimzewski; C. Joachim; R. R. Schlittler; V. Langlais; H. Tang; I.
      Johannsen (1998), "Rotation_of_a_Single_Molecule_Within_a_Supramolecular
      Bearing", Science (in German), 281 (5376), pp. 531â533, doi:10.1126/
      science.281.5376.531
   7. ^ a bThomas Waldmann; Jens Klein; Harry E. Hoster; R. JÃ¼rgen Behm
      (2012), "Stabilization of Large Adsorbates by Rotational Entropy: A Time-
      Resolved Variable-Temperature STM Study", ChemPhysChem (in German), 14,
      pp. 162â169, doi:10.1002/cphc.201200531
   8. ^ S. Li, A. Yu, A, F. Toledo, Z. Han, H. Wang, H. Y. He, R. Wu, and W.
      Ho, Phys. Rev. Lett. 111, 146102 (2013).http://journals.aps.org/prl/
      abstract/10.1103/PhysRevLett.111.146102
   9. ^ F. D. Natterer, F. Patthey, and H. Brune, Phys. Rev. Lett. 111, 175303
      (2013).http://journals.aps.org/prl/abstract/10.1103/
      PhysRevLett.111.175303
***** General references[edit] *****
    * D. M. Dennison (1931). "The Infrared Spectra of Polyatomic Molecules Part
      I". Rev. Mod. Phys. 3 (2): 280â345. Bibcode:1931RvMP....3..280D. doi:
      10.1103/RevModPhys.3.280.
 (Especially Section 2: The Rotation of Polyatomic Molecules).
Van Vleck, J. H. (1951). "The Coupling of Angular Momentum Vectors in
Molecules". Rev. Mod. Phys. 23 (3): 213â227. Bibcode:1951RvMP...23..213V.
doi:10.1103/RevModPhys.23.213.
McQuarrie, Donald A (1983). Quantum Chemistry. Mill Valley, Calif.: University
Science Books. ISBN 0-935702-13-X.
Goldstein, H.; Poole, C. P.; Safko, J. L. (2001). Classical Mechanics (Third
ed.). San Francisco: Addison Wesley Publishing Company. ISBN 0-201-65702-3.
 (Chapters 4 and 5)
Arnold, V. I. (1989). Mathematical Methods of Classical Mechanics. Springer-
Verlag. ISBN 0-387-96890-3.
 (Chapter 6).
Kroto, H. W. (1992). Molecular Rotation Spectra. New York: Dover.
Gordy, W.; Cook, R. L. (1984). Microwave Molecular Spectra (Third ed.). New
York: Wiley. ISBN 0-471-08681-9.
PapouÅ¡ek, D.; Aliev, M. T. (1982). Molecular Vibrational-Rotational Spectra.
Amsterdam: Elsevier. ISBN 0-444-99737-7.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Rigid_rotor&oldid=906509885"
Categories:
    * Molecular_physics
    * Rigid_bodies
    * Rigid_bodies_mechanics
    * Rotation
    * Quantum_models
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
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * ×¢××¨××ª
    * PortuguÃªs
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
Edit_links
    * This page was last edited on 16 July 2019, at 09:39 (UTC).
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
