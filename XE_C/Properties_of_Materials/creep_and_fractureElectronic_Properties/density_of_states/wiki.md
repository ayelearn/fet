The following text has been accessed from https://en.wikipedia.org/wiki/Density_of_states at Thu Aug 8 22:57:16 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Density of states ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Condensed_matter_physics
[QuantumPhaseTransition.svg]
Phases · Phase_transition · QCP
States_of_matter
Solid · Liquid · Gas · BoseâEinstein_condensate · Bose_gas · Fermionic_condensate · Fermi_gas ·
Fermi_liquid · Supersolid · Superfluidity · Luttinger_liquid  · Time_crystal
Phase phenomena
Order_parameter · Phase_transition · QCP
Electronic phases
Electronic_band_structure · Plasma · Insulator · Mott_insulator · Semiconductor · Semimetal ·
Conductor · Superconductor · Thermoelectric · Piezoelectric · Ferroelectric · Topological
insulator · Spin_gapless_semiconductor
Electronic phenomena
Quantum_Hall_effect · Spin_Hall_effect · Kondo_effect
Magnetic phases
Diamagnet · Superdiamagnet
Paramagnet · Superparamagnet
Ferromagnet · Antiferromagnet
Metamagnet · Spin_glass
Quasiparticles
Phonon · Exciton · Plasmon
Polariton · Polaron · Magnon
Soft_matter
Amorphous_solid · Colloid · Granular_material · Liquid_crystal · Polymer
Scientists
Van_der_Waals · Onnes · von_Laue · Bragg · Debye · Bloch · Onsager · Mott · Peierls · Landau ·
Luttinger · Anderson · Van_Vleck · Mott · Hubbard · Shockley · Bardeen · Cooper · Schrieffer ·
Josephson · Louis_NÃ©el · Esaki · Giaever · Kohn · Kadanoff · Fisher · Wilson · von_Klitzing ·
Binnig · Rohrer · Bednorz · MÃ¼ller · Laughlin · StÃ¶rmer · Yang · Tsui · Abrikosov · Ginzburg ·
Leggett
    * v
    * t
    * e
In solid_state_physics and condensed_matter_physics, the density of states
(DOS) of a system describes the number of states that are available to be
occupied by the system at each level of energy. It is mathematically
represented as a distribution by a probability_density_function, and it is
generally an average over the space and time domains of the various states
occupied by the system. The density of states is directly related to the
dispersion_relations of the properties of the system. High DOS at a specific
energy level means that many states are available for occupation.
Generally, the density of states of matter is continuous. In isolated_systems
however, such as atoms or molecules in the gas phase, the density distribution
is discrete, like a spectral_density. Local variations, most often due to
distortions of the original system, are often called local density of states
(LDOS). If the DOS of an undisturbed system is zero, the LDOS can locally be
non-zero due to the presence of a local potential.
⁰
***** Contents *****
    * 1_Introduction
    * 2_Definition
    * 3_Symmetry
    * 4_k-space_topologies
          o 4.1_Density_of_wave_vector_states_(sphere)
          o 4.2_Density_of_energy_states
    * 5_Dispersion_relations
          o 5.1_Isotropic_dispersion_relations
          o 5.2_Parabolic_dispersion
          o 5.3_Linear_dispersion
    * 6_Distribution_functions
    * 7_Applications
          o 7.1_Quantization
          o 7.2_Photonic_crystals
    * 8_Computational_calculation
    * 9_Local_density_of_states
          o 9.1_Solid_state_devices
    * 10_See_also
    * 11_References
    * 12_Further_reading
    * 13_External_links
***** Introduction[edit] *****
In quantum mechanical systems, waves, or wave-like particles, can occupy modes
or states with wavelengths and propagation directions dictated by the system.
For example, in some systems, the interatomic spacing and the atomic charge of
a material could allow only electrons of certain wavelengths to exist. In other
systems, the crystalline structure of a material could allow waves to propagate
in one direction, while suppressing wave propagation in another direction.
Often, only specific states are permitted. Thus, it can happen that many states
are available for occupation at a specific energy level, while no states are
available at other energy levels .
For example, the density of states of electrons at the band edge between the
valence_and_conduction_bands in a semiconductor is shown in orange in Fig. 4.
For an electron in the conduction band, an increase of the electron energy
makes more states available for occupation. Alternatively, the density of state
is discontinuous for an interval of energy, which means that no states are
available for electrons to occupy within the band gap of the material. This
condition also means that an electron at the conduction band edge must lose at
least the band gap energy of the material in order to transition to another
state in the valence band.
Depending on the quantum mechanical system, the density of states can be
calculated for electrons, photons, or phonons, and can be given as a function
of either energy or the wave_vector k. To convert between the DOS as a function
of the energy and the DOS as a function of the wave vector, the system-specific
energy dispersion relation between E and k must be known.
In general, the topological properties of the system have a major impact on the
properties of the density of states. The most well-known systems, like
neutronium in neutron_stars and free_electron_gases_in_metals (examples of
degenerate_matter and a Fermi_gas), have a 3-dimensional Euclidean_topology.
Less familiar systems, like two-dimensional_electron_gases (2DEG) in graphite
layers and the quantum_Hall_effect system in MOSFET type devices, have a 2-
dimensional Euclidean topology. Even less familiar are carbon_nanotubes, the
quantum_wire and Luttinger_liquid with their 1-dimensional topologies. Systems
with 1D and 2D topologies are likely to become more common, assuming
developments in nanotechnology and materials_science proceed.
***** Definition[edit] *****
In general the density of states, related to volume V and N countable energy
levels, is defined by:
         D ( E ) =   1 V   &#x22C5;  &#x2211;  i = 1   N   &#x03B4;  (  E
      &#x2212; E  (     k &#x2192;     i   )   )  .   {\displaystyle D(E)=
      {\frac {1}{V}}\cdot \sum _{i=1}^{N}\delta \left(E-E\left({\vec {k}}_
      {i}\right)\right).}  [{\displaystyle D(E)={\frac {1}{V}}\cdot \sum _
      {i=1}^{N}\delta \left(E-E\left({\vec {k}}_{i}\right)\right).}]
Using     ( &#x0394; k  )  d   =   (    2 &#x03C0;  L   )   d
{\displaystyle (\Delta k)^{d}=\left({\frac {2\pi }{L}}\right)^{d}}  [
{\displaystyle (\Delta k)^{d}=\left({\frac {2\pi }{L}}\right)^{d}}] (the
smallest allowed change of     k   {\displaystyle k}  [k] for a particle in a
box of dimension     d   {\displaystyle d}  [d] and length     L
{\displaystyle L}  [L]) under the limit     L &#x2192; &#x221E;
{\displaystyle L\to \infty }  [{\displaystyle L\to \infty }], one derives the
volume-related density of states for continuous energy levels
         D ( E ) :=  &#x222B;    R   d          d   d   k   ( 2 &#x03C0;  )  d
      &#x22C5; &#x03B4;  (  E &#x2212; E  (    k &#x2192;    )   )  .
      {\displaystyle D(E):=\int _{\mathbb {R} ^{d}}{\frac {\mathrm {d} ^{d}k}{
      (2\pi )^{d}}}\cdot \delta \left(E-E\left({\vec {k}}\right)\right).}  [
      {\displaystyle D(E):=\int _{\mathbb {R} ^{d}}{\frac {\mathrm {d} ^{d}k}{
      (2\pi )^{d}}}\cdot \delta \left(E-E\left({\vec {k}}\right)\right).}]
With     d   {\displaystyle d}  [d] of the spatial dimension of the considered
system and     k   {\displaystyle k}  [ k] the wave vector.
Equivalently, the density of states can also be understood as the derivative of
the microcanonical partition function      Z  m   ( E )   {\displaystyle Z_{m}
(E)}  [{\displaystyle Z_{m}(E)}] with respect to the energy:
         D ( E ) =   1 V   &#x22C5;     d   Z  m   ( E )    d  E
      {\displaystyle D(E)={\frac {1}{V}}\cdot {\frac {\mathrm {d} Z_{m}(E)}
      {\mathrm {d} E}}}  [{\displaystyle D(E)={\frac {1}{V}}\cdot {\frac
      {\mathrm {d} Z_{m}(E)}{\mathrm {d} E}}}]
The number of states with energy      E &#x2032;    {\displaystyle E'}  [E']
(degree of degeneracy) is given by:
         g  (  E &#x2032;  )  =  lim  &#x0394; E &#x2192; 0    &#x222B;   E
      &#x2032;     E &#x2032;  + &#x0394; E   D ( E )  d  E =  lim  &#x0394; E
      &#x2192; 0   D  (  E &#x2032;  )  &#x0394; E ,   {\displaystyle g\left
      (E'\right)=\lim _{\Delta E\to 0}\int _{E'}^{E'+\Delta E}D(E)\mathrm {d}
      E=\lim _{\Delta E\to 0}D\left(E'\right)\Delta E,}  [{\displaystyle g\left
      (E'\right)=\lim _{\Delta E\to 0}\int _{E'}^{E'+\Delta E}D(E)\mathrm {d}
      E=\lim _{\Delta E\to 0}D\left(E'\right)\Delta E,}]
where the last equality only applies when the mean value theorem for integrals
is valid.
***** Symmetry[edit] *****
First Brillouin zone of the FCC_lattice, a truncated_octahedron, showing
symmetry labels for high symmetry lines and points
There is a large variety of systems and types of states for which DOS
calculations can be done.
Some condensed matter systems possess a symmetry of its structure on its
microscopic scale which simplifies calculations of its density of states. In
spherically symmetric systems, the integrals of function are one-dimensional
because all variables in the calculation depend only on the radial parameter of
the dispersion relation. Fluids, glasses or amorphous_solids are example of a
symmetric system whose dispersion_relations has a rotational symmetry.
Octahedron.
Measurements on powders or polycrystalline samples require evaluation and
calculation functions and integrals over the whole domain, most often a
Brillouin_zone, of the dispersion relations of the system of interest.
Sometimes the symmetry of the system is high, which causes the shape of the
functions describing the dispersion relations of the system to appear many
times over the whole domain of the dispersion relation. In such cases the
effort to calculate the DOS can be reduced by a great amount when the
calculation is limited to a reduced zone or fundamental_domain.[1] The
Brillouin zone of the face-centered_cubic_lattice (FCC) in the figure on the
right has the 48-fold symmetry of the point_group Oh with full octahedral
symmetry. This configuration means that the integration over the whole domain
of the Brillouin zone can be reduced to a 48-th part of the whole Brillouin
zone. As a crystal_structure_periodic_table shows, there are many elements with
a FCC crystal structure, like diamond, silicon and platinum and their Brillouin
zones and dispersion relations have this 48-fold symmetry. Two other familiar
crystal structures are the body-centered cubic lattice (BCC) and hexagonal
closed packed structures (HCP) with cubic and hexagonal lattices, respectively.
The BCC structure has the 24-fold pyritohedral_symmetry of the point group Th.
The HCP structure has the 12-fold prismatic_dihedral symmetry of the point
group D3h. A complete list of symmetry properties of a point group can be found
in point_group_character_tables.
In general it is easier to calculate a DOS when the symmetry of the system is
higher and the number of topological dimensions of the dispersion relation is
lower. The DOS of dispersion relations with rotational symmetry can often be
calculated analytically. This result is fortunate, since many materials of
practical interest, such as steel and silicon, have high symmetry.
In anisotropic condensed matter systems such as a single_crystal of a compound,
the density of states could be different in one crystallographic direction than
in another. These causes the anisotropic density of states to be more difficult
to visualize, and might require methods such as calculating the DOS for
particular points or directions only, or calculating the projected density of
states (PDOS) to a particular crystal orientation.
***** k-space topologies[edit] *****
Figure 1: Spherical surface in k-space for electrons in three dimensions.
The density of states is dependent upon the dimensional limits of the object
itself. In a system described by three orthogonal parameters (3 Dimension), the
units of DOS is Energyâ1Volumeâ1 , in a two dimensional system, the units
of DOS is Energyâ1Areaâ1 , in a one dimensional system, the units of DOS is
Energyâ1Lengthâ1. The referenced volume is the volume of k-space; the space
enclosed by the constant_energy_surface of the system derived through a
dispersion_relation that relates E to k. An example of a 3-dimensional k-space
is given in Fig. 1. It can be seen that the dimensionality of the system
confines the momentum of particles inside the system.
**** Density of wave vector states (sphere)[edit] ****
The calculation for DOS starts by counting the N allowed states at a certain k
that are contained within [k, k + dk] inside the volume of the system. This
procedure is done by differentiating the whole k-space volume      &#x03A9;  n
, k     {\displaystyle \Omega _{n,k}}  [{\displaystyle \Omega _{n,k}}] in n-
dimensions at an arbitrary k, with respect to k. The volume, area or length in
3, 2 or 1-dimensional spherical k-spaces are expressed by
          &#x03A9;  n   ( k ) =  c  n    k  n     {\displaystyle \Omega _{n}
      (k)=c_{n}k^{n}}  [\Omega _{n}(k)=c_{n}k^{n}]
for a n-dimensional k-space with the topologically determined constants
          c  1   = 2 , &#xA0;  c  2   = &#x03C0; , &#xA0;  c  3   =    4
      &#x03C0;  3     {\displaystyle c_{1}=2,\ c_{2}=\pi ,\ c_{3}={\frac {4\pi
      }{3}}}  [{\displaystyle c_{1}=2,\ c_{2}=\pi ,\ c_{3}={\frac {4\pi }{3}}}]
for linear, disk and spherical symmetrical shaped functions in 1, 2 and 3-
dimensional Euclidean k-spaces respectively.
According to this scheme, the density of wave vector states N is, through
differentiating      &#x03A9;  n , k     {\displaystyle \Omega _{n,k}}  [\Omega
_{n,k}] with respect to k, expressed by
          N  n   ( k ) =      d    &#x03A9;  n   ( k )     d   k    = n   c  n
      k  n &#x2212; 1     {\displaystyle N_{n}(k)={\frac {{\rm {d}}\Omega _{n}
      (k)}{{\rm {d}}k}}=n\;c_{n}\;k^{n-1}}  [{\displaystyle N_{n}(k)={\frac {
      {\rm {d}}\Omega _{n}(k)}{{\rm {d}}k}}=n\;c_{n}\;k^{n-1}}]
The 1, 2 and 3-dimensional density of wave vector states for a line, disk, or
sphere are explicitly written as
              N  1   ( k )    = 2      N  2   ( k )    = 2 &#x03C0; k      N  3
      ( k )    = 4 &#x03C0;  k  2         {\displaystyle {\begin{aligned}N_{1}
      (k)&=2\\N_{2}(k)&=2\pi k\\N_{3}(k)&=4\pi k^{2}\end{aligned}}}  [
      {\displaystyle {\begin{aligned}N_{1}(k)&=2\\N_{2}(k)&=2\pi k\\N_{3}
      (k)&=4\pi k^{2}\end{aligned}}}]
One state is large enough to contain particles having wavelength Î». The
wavelength is related to k through the relationship.
         k =    2 &#x03C0;  &#x03BB;     {\displaystyle k={\frac {2\pi }
      {\lambda }}}  [k={\frac {2\pi }{\lambda }}]
In a quantum system the length of Î» will depend on a characteristic spacing of
the system L that is confining the particles. Finally the density of states N
is multiplied by a factor    s  /   V  k     {\displaystyle s/V_{k}}  [s/V_
{k}], where s is a constant degeneracy factor that accounts for internal
degrees of freedom due to such physical phenomena as spin or polarization. If
no such phenomenon is present then     s = 1   {\displaystyle s=1}  [s=1]. Vk
is the volume in k-space whose wavevectors are smaller than the smallest
possible wavevectors decided by the characteristic spacing of the system.
**** Density of energy states[edit] ****
To finish the calculation for DOS find the number of states per unit sample
volume at an energy     E   {\displaystyle E}  [E] inside an interval     [ E ,
E + d E ]   {\displaystyle [E,E+dE]}  [[E,E+dE]]. The general form of DOS of a
system is given as
          D  n    ( E )  =      d    &#x03A9;  n   ( E )     d   E
      {\displaystyle D_{n}\left(E\right)={\frac {{\rm {d}}\Omega _{n}(E)}{{\rm
      {d}}E}}}  [{\displaystyle D_{n}\left(E\right)={\frac {{\rm {d}}\Omega _
      {n}(E)}{{\rm {d}}E}}}]
The scheme sketched so far only applies to monotonically rising and spherically
symmetric dispersion relations. In general the dispersion relation     E ( k )
{\displaystyle E(k)}  [E(k)] is not spherically symmetric and in many cases it
isn't continuously rising either. To express D as a function of E the inverse
of_the_dispersion_relation     E ( k )   {\displaystyle E(k)}  [E(k)] has to be
substituted into the expression of      &#x03A9;  n   ( k )   {\displaystyle
\Omega _{n}(k)}  [\Omega _{n}(k)] as a function of k to get the expression of
&#x03A9;  n   ( E )   {\displaystyle \Omega _{n}(E)}  [\Omega _{n}(E)] as a
function of the energy. If the dispersion relation is not spherically symmetric
or continuously rising and can't be inverted easily then in most cases the DOS
has to be calculated numerically. More detailed derivations are available.[2]
[3]
***** Dispersion relations[edit] *****
The dispersion relation for electrons in a solid is given by the electronic
band_structure.
The kinetic_energy of a particle depends on the magnitude and direction of the
wave_vector k, the properties of the particle and the environment in which the
particle is moving. For example, the kinetic energy of an electron in a Fermi
gas is given by
         E =  E  0   +     (  &#x210F; k  )   2    2 m    &#xA0; ,
      {\displaystyle E=E_{0}+{\frac {\left(\hbar k\right)^{2}}{2m}}\ ,}  [
      {\displaystyle E=E_{0}+{\frac {\left(\hbar k\right)^{2}}{2m}}\ ,}]
where m is the electron_mass. The dispersion relation is a spherically
symmetric parabola and it is continuously rising so the DOS can be calculated
easily.
Figure 2: Monatomic chain phonon dispersion relation
For longitudinal phonons in a string of atoms the dispersion relation of the
kinetic energy in a 1-dimensional k-space, as shown in Figure 2, is given by
         E = 2 &#x210F;  &#x03C9;  0    |  sin &#x2061;  (    k a  2   )   |
      {\displaystyle E=2\hbar \omega _{0}\left|\sin \left({\frac {ka}
      {2}}\right)\right|}  [{\displaystyle E=2\hbar \omega _{0}\left|\sin \left
      ({\frac {ka}{2}}\right)\right|}]
where      &#x03C9;  0   =    k   F     /  m     {\displaystyle \omega _{0}=
{\sqrt {k_{\rm {F}}/m}}}  [{\displaystyle \omega _{0}={\sqrt {k_{\rm {F}}/m}}}]
is the oscillator frequency,     m   {\displaystyle m}  [m] the mass of the
atoms,      k   F      {\displaystyle k_{\rm {F}}}  [{\displaystyle k_{\rm
{F}}}] the inter-atomic force constant and     a   {\displaystyle a}  [a]
inter-atomic spacing. For small values of     k &#x226A; &#x03C0;  /  a
{\displaystyle k\ll \pi /a}  [k\ll \pi /a] the dispersion relation is rather
linear:
         E = &#x210F;  &#x03C9;  0   k a   {\displaystyle E=\hbar \omega _
      {0}ka}  [E=\hbar \omega _{0}ka]
When     k &#x2248; &#x03C0;  /  a   {\displaystyle k\approx \pi /a}  [k\approx
\pi /a] the energy is
         E = 2 &#x210F;  &#x03C9;  0    |  cos &#x2061;  (    &#x03C0; &#x2212;
      k a  2   )   |    {\displaystyle E=2\hbar \omega _{0}\left|\cos \left(
      {\frac {\pi -ka}{2}}\right)\right|}  [{\displaystyle E=2\hbar \omega _
      {0}\left|\cos \left({\frac {\pi -ka}{2}}\right)\right|}]
With the transformation     q = k &#x2212; &#x03C0;  /  a   {\displaystyle q=k-
\pi /a}  [q=k-\pi /a] and small     q   {\displaystyle q}  [q] this relation
can be transformed to
         E = 2 &#x210F;  &#x03C9;  0    [  1 &#x2212;   (    q a  2   )   2
      ]    {\displaystyle E=2\hbar \omega _{0}\left[1-\left({\frac {qa}
      {2}}\right)^{2}\right]}  [{\displaystyle E=2\hbar \omega _{0}\left[1-
      \left({\frac {qa}{2}}\right)^{2}\right]}]
**** Isotropic dispersion relations[edit] ****
The two examples mentioned here can be expressed like
         E =  E  0   +  c  k    k  p     {\displaystyle E=E_{0}+c_{k}k^{p}}  [
      {\displaystyle E=E_{0}+c_{k}k^{p}}]
This expression is a kind of dispersion_relation because it interrelates two
wave properties and it is isotropic because only the length and not the
direction of the wave vector appears in the expression. The magnitude of the
wave vector is related to the energy as:
         k =   (    E &#x2212;  E  0     c  k     )    1 p    &#xA0; ,
      {\displaystyle k=\left({\frac {E-E_{0}}{c_{k}}}\right)^{\frac {1}{p}}\ ,}
      [{\displaystyle k=\left({\frac {E-E_{0}}{c_{k}}}\right)^{\frac {1}{p}}\
      ,}]
Accordingly, the volume of n-dimensional k-space containing wave vectors
smaller than k is:
          &#x03A9;  n   ( k ) =  c  n    k  n     {\displaystyle \Omega _{n}
      (k)=c_{n}k^{n}}  [\Omega _{n}(k)=c_{n}k^{n}]
Substitution of the isotropic energy relation gives the volume of occupied
states
          &#x03A9;  n   ( E ) =    c  n      c  k      n p        (  E &#x2212;
      E  0    )    n p    &#xA0; ,   {\displaystyle \Omega _{n}(E)={\frac {c_
      {n}}{{c_{k}}^{\frac {n}{p}}}}\left(E-E_{0}\right)^{\frac {n}{p}}\ ,}  [
      {\displaystyle \Omega _{n}(E)={\frac {c_{n}}{{c_{k}}^{\frac {n}
      {p}}}}\left(E-E_{0}\right)^{\frac {n}{p}}\ ,}]
Differentiating this volume with respect to the energy gives an expression for
the DOS of the isotropic dispersion relation
          D  n    ( E )  =   d  d E     &#x03A9;  n   ( E ) =    n  c  n     p
      c  k      n p         (  E &#x2212;  E  0    )     n p   &#x2212; 1
      {\displaystyle D_{n}\left(E\right)={\frac {d}{dE}}\Omega _{n}(E)={\frac
      {nc_{n}}{p{c_{k}}^{\frac {n}{p}}}}\left(E-E_{0}\right)^{{\frac {n}{p}}-
      1}}  [{\displaystyle D_{n}\left(E\right)={\frac {d}{dE}}\Omega _{n}(E)=
      {\frac {nc_{n}}{p{c_{k}}^{\frac {n}{p}}}}\left(E-E_{0}\right)^{{\frac {n}
      {p}}-1}}]
**** Parabolic dispersion[edit] ****
Figure 3: Free-electron DOS in 3-dimensional k-space
In the case of a parabolic dispersion relation (p = 2), such as applies to free
electrons in a Fermi gas, the resulting density of states,      D  n    ( E )
{\displaystyle D_{n}\left(E\right)}  [D_{n}\left(E\right)], for electrons in a
n-dimensional systems is
              D  1    ( E )     =   1   c  k    (  E &#x2212;  E  0    )
      D  2    ( E )     =   &#x03C0;  c  k          D  3    ( E )     = 2
      &#x03C0;     E &#x2212;  E  0     c  k   3      &#xA0; .
      {\displaystyle {\begin{aligned}D_{1}\left(E\right)&={\frac {1}{\sqrt {c_
      {k}\left(E-E_{0}\right)}}}\\D_{2}\left(E\right)&={\frac {\pi }{c_
      {k}}}\\D_{3}\left(E\right)&=2\pi {\sqrt {\frac {E-E_{0}}{c_{k}^{3}}}}\
      .\end{aligned}}}  [{\displaystyle {\begin{aligned}D_{1}\left(E\right)&=
      {\frac {1}{\sqrt {c_{k}\left(E-E_{0}\right)}}}\\D_{2}\left(E\right)&=
      {\frac {\pi }{c_{k}}}\\D_{3}\left(E\right)&=2\pi {\sqrt {\frac {E-E_{0}}
      {c_{k}^{3}}}}\ .\end{aligned}}}]
for     E >  E  0     {\displaystyle E>E_{0}}  [E>E_{0}], with     D ( E ) = 0
{\displaystyle D(E)=0}  [D(E)=0] for     E <  E  0     {\displaystyle E<E_{0}}
[E<E_{0}].
In 1-dimensional systems the DOS diverges at the bottom of the band as     E
{\displaystyle E}  [E] drops to      E  0     {\displaystyle E_{0}}  [E_{0}].
[citation_needed] In 2-dimensional systems the DOS turns out to be independent
of     E   {\displaystyle E}  [E].[citation_needed] Finally for 3-dimensional
systems the DOS rises as the square root of the energy.[4]
Including the prefactor    s  /   V  k     {\displaystyle s/V_{k}}  [s/V_{k}],
the expression for the 3D DOS is
         N ( E ) =   V  2  &#x03C0;  2        (    2 m   &#x210F;  2     )    3
      2      E &#x2212;  E  0       {\displaystyle N(E)={\frac {V}{2\pi ^
      {2}}}\left({\frac {2m}{\hbar ^{2}}}\right)^{\frac {3}{2}}{\sqrt {E-E_
      {0}}}}  [{\displaystyle N(E)={\frac {V}{2\pi ^{2}}}\left({\frac {2m}
      {\hbar ^{2}}}\right)^{\frac {3}{2}}{\sqrt {E-E_{0}}}}],
where     V   {\displaystyle V}  [V] is the total volume, and     N ( E
&#x2212;  E  0   )   {\displaystyle N(E-E_{0})}  [N(E-E_{0})] includes the 2-
fold spin degeneracy.
**** Linear dispersion[edit] ****
In the case of a linear relation (p = 1), such as applies to photons, acoustic
phonons, or to some special kinds of electronic bands in a solid, the DOS in 1,
2 and 3 dimensional systems is related to the energy as:
              D  1    ( E )     =   1  c  k          D  2    ( E )     =    2
      &#x03C0;   c  k   2      (  E &#x2212;  E  0    )       D  3    ( E )
      =    4 &#x03C0;   c  k   3       (  E &#x2212;  E  0    )   2
      {\displaystyle {\begin{aligned}D_{1}\left(E\right)&={\frac {1}{c_
      {k}}}\\D_{2}\left(E\right)&={\frac {2\pi }{c_{k}^{2}}}\left(E-E_
      {0}\right)\\D_{3}\left(E\right)&={\frac {4\pi }{c_{k}^{3}}}\left(E-E_
      {0}\right)^{2}\end{aligned}}}  [{\displaystyle {\begin{aligned}D_{1}\left
      (E\right)&={\frac {1}{c_{k}}}\\D_{2}\left(E\right)&={\frac {2\pi }{c_{k}^
      {2}}}\left(E-E_{0}\right)\\D_{3}\left(E\right)&={\frac {4\pi }{c_{k}^
      {3}}}\left(E-E_{0}\right)^{2}\end{aligned}}}]
***** Distribution functions[edit] *****
Main article: Kinetic_theory_of_solids
The density of states plays an important role in the kinetic_theory_of_solids.
The product of the density of states and the probability_distribution_function
is the number of occupied states per unit volume at a given energy for a system
in thermal equilibrium. This value is widely used to investigate various
physical properties of matter. The following are examples, using two common
distribution functions, of how applying a distribution function to the density
of states can give rise to physical properties.
Figure 4: The      Fermi-Dirac probability distribution,      density of
states, and      their product for a semiconductor. The lower green lobe
depicts hole energy, and thus uses     f ( &#x2212; x )   {\displaystyle f(-x)}
[f(-x)] as the distribution function.
FermiâDirac_statistics: The FermiâDirac probability distribution function,
Fig. 4, is used to find the probability that a fermion occupies a specific
quantum state in a system at thermal equilibrium. Fermions are particles which
obey the Pauli_exclusion_principle (e.g. electrons, protons, neutrons). The
distribution function can be written as
          f   F D    ( E ) =   1  exp &#x2061;  (    E &#x2212; &#x03BC;    k
      B    T    )  + 1      {\displaystyle f_{\mathrm {FD} }(E)={\frac {1}{\exp
      \left({\frac {E-\mu }{k_{\mathrm {B} }T}}\right)+1}}}  [{\displaystyle f_
      {\mathrm {FD} }(E)={\frac {1}{\exp \left({\frac {E-\mu }{k_{\mathrm {B}
      }T}}\right)+1}}}]
   &#x03BC;   {\displaystyle \mu }  [\mu ] is the chemical_potential (also
denoted as EF and called the Fermi_level when T=0),      k   B
{\displaystyle k_{\mathrm {B} }}  [k_{\mathrm {B} }] is the Boltzmann constant,
and     T   {\displaystyle T}  [T] is temperature. Fig. 4 illustrates how the
product of the Fermi-Dirac distribution function and the three-dimensional
density of states for a semiconductor can give insight to physical properties
such as carrier concentration and Energy band gaps.
BoseâEinstein_statistics: The BoseâEinstein probability distribution
function is used to find the probability that a boson occupies a specific
quantum state in a system at thermal equilibrium. Bosons are particles which do
not obey the Pauli exclusion principle (e.g. phonons and photons). The
distribution function can be written as
          f   B E    ( E ) =   1  exp &#x2061;  (    E &#x2212; &#x03BC;    k
      B    T    )  &#x2212; 1      {\displaystyle f_{\mathrm {BE} }(E)={\frac
      {1}{\exp \left({\frac {E-\mu }{k_{\rm {B}}T}}\right)-1}}}  [
      {\displaystyle f_{\mathrm {BE} }(E)={\frac {1}{\exp \left({\frac {E-\mu }
      {k_{\rm {B}}T}}\right)-1}}}]
From these two distributions it is possible to calculate properties such as the
internal_energy     U   {\displaystyle U}  [U], the number of particles     N
{\displaystyle N}  [N], specific_heat_capacity     C   {\displaystyle C}  [C],
and thermal_conductivity     k   {\displaystyle k}  [k]. The relationships
between these properties and the product of the density of states and the
probability distribution, denoting the density of states by     g ( E )
{\displaystyle g(E)}  [g(E)] instead of     D ( E )   {\displaystyle D(E)}  [D
(E)], are given by
             U    = &#x222B; E  f ( E )  g ( E )    d   E     N    = &#x222B; f
      ( E )  g ( E )    d   E     C    =   &#x2202;  &#x2202; T    &#x222B; E
      f ( E )  g ( E )    d   E     k    =   1 d     &#x2202;  &#x2202; T
      &#x222B; E f ( E )  g ( E )  &#x03BD; ( E )  &#x039B; ( E )    d   E
      {\displaystyle {\begin{aligned}U&=\int E\,f(E)\,g(E)\,{\rm {d}}E\\N&=\int
      f(E)\,g(E)\,{\rm {d}}E\\C&={\frac {\partial }{\partial T}}\int E\,f(E)\,g
      (E)\,{\rm {d}}E\\k&={\frac {1}{d}}{\frac {\partial }{\partial T}}\int Ef
      (E)\,g(E)\,\nu (E)\,\Lambda (E)\,{\rm {d}}E\end{aligned}}}  [
      {\displaystyle {\begin{aligned}U&=\int E\,f(E)\,g(E)\,{\rm {d}}E\\N&=\int
      f(E)\,g(E)\,{\rm {d}}E\\C&={\frac {\partial }{\partial T}}\int E\,f(E)\,g
      (E)\,{\rm {d}}E\\k&={\frac {1}{d}}{\frac {\partial }{\partial T}}\int Ef
      (E)\,g(E)\,\nu (E)\,\Lambda (E)\,{\rm {d}}E\end{aligned}}}]
   d   {\displaystyle d}  [d] is dimensionality,     &#x03BD;   {\displaystyle
\nu }  [\nu ] is sound velocity and     &#x039B;   {\displaystyle \Lambda }
[\Lambda ] is mean_free_path.
***** Applications[edit] *****
The density of states appears in many areas of physics, and helps to explain a
number of quantum mechanical phenomena.
**** Quantization[edit] ****
Calculating the density of states for small structures shows that the
distribution of electrons changes as dimensionality is reduced. For quantum
wires, the DOS for certain energies actually becomes higher than the DOS for
bulk semiconductors, and for quantum_dots the electrons become quantized to
certain energies.
**** Photonic crystals[edit] ****
The photon density of states can be manipulated by using periodic structures
with length scales on the order of the wavelength of light. Some structures can
completely inhibit the propagation of light of certain colors (energies),
creating a photonic band gap: the DOS is zero for those photon energies. Other
structures can inhibit the propagation of light only in certain directions to
create mirrors, waveguides, and cavities. Such periodic structures are known as
photonic_crystals. In nanostructured media the concept of local_density_of
states (LDOS) is often more relevant than that of DOS, as the DOS varies
considerably from point to point.
***** Computational calculation[edit] *****
Interesting systems are in general complex, for instance compounds,
biomolecules, polymers, etc. Because of the complexity of these systems the
analytical calculation of the density of states is in most of the cases
impossible. Computer simulations offer a set of algorithms to evaluate the
density of states with a high accuracy. One of these algorithms is called the
Wang_and_Landau_algorithm.[5]
Within the Wang and Landau scheme any previous knowledge of the density of
states is required. One proceeds as follows: the cost function (for example the
energy) of the system is discretized. Each time the bin i is reached one
updates a histogram for the density of states,     g ( i )   {\displaystyle g
(i)}  [g(i)], by
         g ( i ) &#x2192; g ( i ) + f   {\displaystyle g(i)\rightarrow g(i)+f}
      [{\displaystyle g(i)\rightarrow g(i)+f}]
where f is called the modification factor. As soon as each bin in the histogram
is visited a certain number of times (10-15), the modification factor is
reduced by some criterion, for instance,
          f  n + 1   &#x2192;   1 2    f  n     {\displaystyle f_
      {n+1}\rightarrow {\frac {1}{2}}f_{n}}  [{\displaystyle f_{n+1}\rightarrow
      {\frac {1}{2}}f_{n}}]
where n denotes the n-th update step. The simulation finishes when the
modification factor is less than a certain threshold, for instance      f  n
<  10  &#x2212; 8     {\displaystyle f_{n}<10^{-8}}  [{\displaystyle f_{n}<10^
{-8}}].
The Wang and Landau algorithm has some advantages over other common algorithms
such as multicanonical_simulations and parallel_tempering. For example, the
density of states is obtained as the main product of the simulation.
Additionally, Wang and Landau simulations are completely independent of the
temperature. This feature allows to compute the density of states of systems
with very rough energy landscape such as proteins.[6]
Mathematically the density of states is formulated in terms of a tower of
covering maps.[7]
***** Local density of states[edit] *****
Local density of states (LDOS) describes a space-resolved density of states. In
materials science, for example, this term is useful when interpreting the data
from a scanning_tunneling_microscope (STM), since this method is capable of
imaging electron densities of states with atomic resolution. According to
crystal structure, this quantity can be predicted by computational methods, as
for example with density_functional_theory.
Space resolved local density of states. A sequence of images with varying gate
bias in a nanowire MOSFET at drain bias Vd=0.6V. Notice the confined energy
levels as they move with increasing gate bias.
**** Solid state devices[edit] ****
Local density of states can be used to gain insights into a solid-state device.
For example, the figure on the right illustrates LDOS of a transistor as it
turns on and off in a ballistic simulation. The LDOS has clear boundary in the
source and drain, that corresponds to the location of band edge. In the
channel, the DOS is increasing as gate voltage increase and potential barrier
goes down.
In optics and photonics the concept of local density of states refers to the
states that can be occupied by a photon. For light it is usually measured by
fluorescence methods, near-field scanning methods or by cathodoluminescence
techniques.
***** See also[edit] *****
    * Effective_mass_(solid-state_physics)
    * Band_structure
    * kÂ·p_perturbation_theory
    * Semiconductor
    * Electrical_conduction
    * Valence_band
    * KronigâPenney_model
    * Tight-binding_model
    * Muffin-tin_approximation
    * Britney_Spears'_Guide_to_Semiconductor_Physics
***** References[edit] *****
   1. ^ Walter Ashley Harrison (1989). Electronic_Structure_and_the_Properties
      of_Solids. Dover Publications. ISBN 978-0-486-66021-9.
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
   3. ^ Sample_density_of_states_calculation
   4. ^ Another_density_of_states_calculation
   5. ^Charles Kittel (1996). Introduction to Solid State Physics (7th ed.).
      Wiley. Equation (37), p. 216. ISBN 978-0-471-11181-8.
   6. ^ Wang, Fugao; Landau, D. P. (2001). "Efficient, Multiple-Range Random
      Walk Algorithm to Calculate the Density of States". Phys. Rev. Lett. 86
      (10): 2050â2053. arXiv:cond-mat/0011174. Bibcode:2001PhRvL..86.2050W.
      doi:10.1103/PhysRevLett.86.2050. PMID 11289852.
   7. ^Ojeda, P.; Garcia, M. (2010). "Electric_Field-Driven_Disruption_of_a
      Native_beta-Sheet_Protein_Conformation_and_Generation_of_a_Helix-
      Structure". Biophysical Journal. 99 (2): 595â599. Bibcode:
      2010BpJ....99..595O. doi:10.1016/j.bpj.2010.04.040. PMC 2905109.
      PMID 20643079.
   8. ^ Adachi T. and Sunada._T (1993). "Density of states in spectral geometry
      of states in spectral geometry". Comment. Math. Helvetici. 68: 480â493.
***** Further reading[edit] *****
    * Chen, Gang. Nanoscale Energy Transport and Conversion. New York: Oxford,
      2005
    * Streetman, Ben G. and Sanjay Banerjee. Solid State Electronic Devices.
      Upper Saddle River, NJ: Prentice Hall, 2000.
    * Muller, Richard S. and Theodore I. Kamins. Device Electronics for
      Integrated Circuits. New York: John Wiley and Sons, 2003.
    * Kittel, Charles and Herbert Kroemer. Thermal Physics. New York: W.H.
      Freeman and Company, 1980
    * Sze, Simon M. Physics of Semiconductor Devices. New York: John Wiley and
      Sons, 1981
***** External links[edit] *****
    * Online_lecture:ECE_606_Lecture_8:_Density_of_States by M. Alam
    * Scientists_shed_light_on_glowing_materials How to measure the Photonic
      LDOS

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Density_of_states&oldid=901865047"
Categories:
    * Statistical_mechanics
    * Concepts_in_physics
    * Electronic_band_structures
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_May_2017
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
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 14 June 2019, at 20:11 (UTC).
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
