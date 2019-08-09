The following text has been accessed from https://en.wikipedia.org/wiki/Electronic_band_structure at Fri Aug 9 02:07:58 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Electronic band structure ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Electronic_structure methods
Valence_bond_theory
CoulsonâFischer_theory
Generalized_valence_bond
Modern_valence_bond
Molecular_orbital_theory
HartreeâFock_method
Density_functional_theory
Semi-empirical_quantum_chemistry_methods
MÃ¸llerâPlesset_perturbation_theory
Configuration_interaction
Coupled_cluster
Multi-configurational_self-consistent_field
Quantum_chemistry_composite_methods
Quantum_Monte_Carlo
Electronic band structure
Nearly_free_electron_model
Tight_binding
Muffin-tin_approximation
kÂ·p_perturbation_theory
Empty_lattice_approximation
[Wikipedia book] Book
    * v
    * t
    * e
In solid-state_physics, the electronic band structure (or simply band
structure) of a solid describes the range of energies an electron within the
solid may have (called energy bands, allowed bands, or simply bands) and ranges
of energy that it may not have (called band_gaps or forbidden bands).
Band theory derives these bands and band gaps by examining the allowed quantum
mechanical wave_functions for an electron in a large, periodic lattice of atoms
or molecules. Band theory has been successfully used to explain many physical
properties of solids, such as electrical_resistivity and optical_absorption,
and forms the foundation of the understanding of all solid-state_devices
(transistors, solar cells, etc.).
⁰
***** Contents *****
    * 1_Why_bands_and_band_gaps_occur
    * 2_Basic_concepts
          o 2.1_Assumptions_and_limits_of_band_structure_theory
          o 2.2_Crystalline_symmetry_and_wavevectors
                # 2.2.1_Asymmetry:_Band_structures_in_non-crystalline_solids
          o 2.3_Density_of_states
          o 2.4_Filling_of_bands
                # 2.4.1_Names_of_bands_near_the_Fermi_level_(conduction_band,
                  valence_band)
    * 3_Theory_in_crystals
          o 3.1_Nearly_free_electron_approximation
          o 3.2_Tight_binding_model
          o 3.3_KKR_model
          o 3.4_Density-functional_theory
          o 3.5_Green's_function_methods_and_the_ab_initio_GW_approximation
          o 3.6_Mott_insulators
          o 3.7_Others
    * 4_Band_diagrams
    * 5_See_also
    * 6_References
    * 7_Bibliography
    * 8_Further_reading
    * 9_External_links
***** Why bands and band gaps occur[edit] *****
Showing how electronic band structure comes about by the hypothetical example
of a large number of carbon atoms being brought together to form a diamond
crystal. The graph (right) shows the energy levels as a function of the spacing
between atoms. When the atoms are far apart (right side of graph) each atom has
valence atomic orbitals p and s which have the same energy. However, when the
atoms come closer together their orbitals begin to overlap. Due to the Pauli
Exclusion Principle each atomic orbital splits into N molecular orbitals each
with a different energy, where N is the number of atoms in the crystal. Since N
is such a large number, adjacent orbitals are extremely close together in
energy so the orbitals can be considered a continuous energy band. a is the
atomic spacing in an actual crystal of diamond. At that spacing the orbitals
form two bands, called the valence and conduction bands, with a 5.5 eV band gap
between them.
[File:Metals and insulators, quantum difference from band structure.ogv]Play
media
Animation of band formation and how electrons fill them in a metal and an
insulator
The electrons of a single, isolated atom occupy atomic_orbitals each of which
has a discrete energy_level. When two or more atoms join together to form into
a molecule, their atomic orbitals overlap.[1][2] The Pauli_exclusion_principle
dictates that no two electrons can have the same quantum numbers in a molecule.
So if two identical atoms combine to form a diatomic_molecule, each atomic
orbital splits into two molecular_orbitals of different energy, allowing the
electrons in the former atomic orbitals to occupy the new orbital structure
without any having the same energy.
Similarly if a large number N of identical atoms come together to form a solid,
such as a crystal_lattice, the atoms' atomic orbitals overlap.[1] Since the
Pauli exclusion principle dictates that no two electrons in the solid have the
same quantum numbers, each atomic orbital splits into N discrete molecular
orbitals, each with a different energy. Since the number of atoms in a
macroscopic piece of solid is a very large number (N~1022) the number of
orbitals is very large and thus they are very closely spaced in energy (of the
order of 10â22 eV). The energy of adjacent levels is so close together that
they can be considered as a continuum, an energy band.
This formation of bands is mostly a feature of the outermost electrons (valence
electrons) in the atom, which are the ones involved in chemical bonding and
electrical_conductivity. The inner electron orbitals do not overlap to a
significant degree, so their bands are very narrow.
Band_gaps are essentially leftover ranges of energy not covered by any band, a
result of the finite widths of the energy bands. The bands have different
widths, with the widths depending upon the degree of overlap in the atomic
orbitals from which they arise. Two adjacent bands may simply not be wide
enough to fully cover the range of energy. For example, the bands associated
with core orbitals (such as 1s_electrons) are extremely narrow due to the small
overlap between adjacent atoms. As a result, there tend to be large band gaps
between the core bands. Higher bands involve comparatively larger orbitals with
more overlap, becoming progressively wider at higher energies so that there are
no band gaps at higher energies.
***** Basic concepts[edit] *****
**** Assumptions and limits of band structure theory[edit] ****
Band theory is only an approximation to the quantum state of a solid, which
applies to solids consisting of many identical atoms or molecules bonded
together. These are the assumptions necessary for band theory to be valid:
    * Infinite-size system: For the bands to be continuous, the piece of
      material must consist of a large number of atoms. Since a macroscopic
      piece of material contains on the order of 1022 atoms, this is not a
      serious restriction; band theory even applies to microscopic-sized
      transistors in integrated_circuits. With modifications, the concept of
      band structure can also be extended to systems which are only "large"
      along some dimensions, such as two-dimensional_electron_systems.
    * Homogeneous system: Band structure is an intrinsic property of a
      material, which assumes that the material is homogeneous. Practically,
      this means that the chemical makeup of the material must be uniform
      throughout the piece.
    * Non-interactivity: The band structure describes "single electron states".
      The existence of these states assumes that the electrons travel in a
      static potential without dynamically interacting with lattice_vibrations,
      other electrons, photons, etc.
The above assumptions are broken in a number of important practical situations,
and the use of band structure requires one to keep a close check on the
limitations of band theory:
    * Inhomogeneities and interfaces: Near surfaces, junctions, and other
      inhomogeneities, the bulk band structure is disrupted. Not only are there
      local small-scale disruptions (e.g., surface_states or dopant states
      inside the band gap), but also local charge imbalances. These charge
      imbalances have electrostatic effects that extend deeply into
      semiconductors, insulators, and the vacuum (see doping, band_bending).
    * Along the same lines, most electronic effects (capacitance, electrical
      conductance, electric-field_screening) involve the physics of electrons
      passing through surfaces and/or near interfaces. The full description of
      these effects, in a band structure picture, requires at least a
      rudimentary model of electron-electron interactions (see space_charge,
      band_bending).
    * Small systems: For systems which are small along every dimension (e.g., a
      small molecule or a quantum_dot), there is no continuous band structure.
      The crossover between small and large dimensions is the realm of
      mesoscopic_physics.
    * Strongly_correlated_materials (for example, Mott_insulators) simply
      cannot be understood in terms of single-electron states. The electronic
      band structures of these materials are poorly defined (or at least, not
      uniquely defined) and may not provide useful information about their
      physical state.
**** Crystalline symmetry and wavevectors[edit] ****
Fig 1. Brillouin_zone of a face-centered_cubic_lattice showing labels for
special symmetry points.
Fig 2. Band structure plot for Si, Ge, GaAs and InAs generated with tight
binding model. Note that Si and Ge are indirect band gap materials, while GaAs
and InAs are direct.
Main articles: Bloch_wave and Brillouin_zone
See also: Symmetry_in_physics, Crystallographic_point_group, and Space_group
Band structure calculations take advantage of the periodic nature of a crystal
lattice, exploiting its symmetry. The single-electron SchrÃ¶dinger_equation is
solved for an electron in a lattice-periodic potential, giving Bloch_waves as
solutions:
          &#x03C8;  n  k    (  r  ) =  e  i  k  &#x22C5;  r     u  n  k    (  r
      )   {\displaystyle \psi _{n\mathbf {k} }(\mathbf {r} )=e^{i\mathbf {k}
      \cdot \mathbf {r} }u_{n\mathbf {k} }(\mathbf {r} )}  [\psi _{n\mathbf {k}
      }(\mathbf {r} )=e^{i\mathbf {k} \cdot \mathbf {r} }u_{n\mathbf {k} }
      (\mathbf {r} )],
where k is called the wavevector. For each value of k, there are multiple
solutions to the SchrÃ¶dinger equation labelled by n, the band index, which
simply numbers the energy bands. Each of these energy levels evolves smoothly
with changes in k, forming a smooth band of states. For each band we can define
a function En(k), which is the dispersion_relation for electrons in that band.
The wavevector takes on any value inside the Brillouin_zone, which is a
polyhedron in wavevector space that is related to the crystal's lattice.
Wavevectors outside the Brillouin zone simply correspond to states that are
physically identical to those states within the Brillouin zone. Special high
symmetry points/lines in the Brillouin zone are assigned labels like Î, Î,
Î, Î£ (see Fig 1).
It is difficult to visualize the shape of a band as a function of wavevector,
as it would require a plot in four-dimensional space, E vs. kx, ky, kz. In
scientific literature it is common to see band structure plots which show the
values of En(k) for values of k along straight lines connecting symmetry
points, often labelled Î, Î, Î£, or [100],_[111],_and_[110], respectively.[3]
[4] Another method for visualizing band structure is to plot a constant-energy
isosurface in wavevector space, showing all of the states with energy equal to
a particular value. The isosurface of states with energy equal to the Fermi
level is known as the Fermi_surface.
Energy band gaps can be classified using the wavevectors of the states
surrounding the band gap:
    * Direct_band_gap: the lowest-energy state above the band gap has the same
      k as the highest-energy state beneath the band gap.
    * Indirect_band_gap: the closest states above and beneath the band gap do
      not have the same k value.
*** Asymmetry: Band structures in non-crystalline solids[edit] ***
Although electronic band structures are usually associated with crystalline
materials, quasi-crystalline and amorphous_solids may also exhibit band
structures.[citation_needed] These are somewhat more difficult to study
theoretically since they lack the simple symmetry of a crystal, and it is not
usually possible to determine a precise dispersion relation. As a result,
virtually all of the existing theoretical work on the electronic band structure
of solids has focused on crystalline materials.
**** Density of states[edit] ****
Main article: Density_of_states
The density of states function g(E) is defined as the number of electronic
states per unit volume, per unit energy, for electron energies near E.
The density of states function is important for calculations of effects based
on band theory. In Fermi's_Golden_Rule, a calculation for the rate of optical
absorption, it provides both the number of excitable electrons and the number
of final states for an electron. It appears in calculations of electrical
conductivity where it provides the number of mobile states, and in computing
electron scattering rates where it provides the number of final states after
scattering.[citation_needed]
For energies inside a band gap, g(E) = 0.
**** Filling of bands[edit] ****
Main articles: Fermi_level and FermiâDirac_statistics
Filling of the electronic states in various types of materials at equilibrium.
Here, height is energy while width is the density_of_available_states for a
certain energy in the material listed. The shade follows the FermiâDirac
distribution (black = all states filled, white = no state filled). In metals
and semimetals the Fermi_level EF lies inside at least one band. In insulators
and semiconductors the Fermi level is inside a band_gap; however, in
semiconductors the bands are near enough to the Fermi level to be thermally
populated with electrons or holes.
                                                                           edit
At thermodynamic_equilibrium, the likelihood of a state of energy E being
filled with an electron is given by the FermiâDirac_distribution, a
thermodynamic distribution that takes into account the Pauli_exclusion
principle:
         f ( E ) =   1  1 +  e   ( E &#x2212; &#x03BC; )   /    k   B    T
      {\displaystyle f(E)={\frac {1}{1+e^{{(E-\mu )}/{k_{\rm {B}}T}}}}}  [f(E)=
      {\frac {1}{1+e^{{(E-\mu )}/{k_{\rm {B}}T}}}}]
where:
    * kBT is the product of Boltzmann's_constant and temperature, and
    * Âµ is the total_chemical_potential of electrons, or Fermi level (in
      semiconductor_physics, this quantity is more often denoted EF). The Fermi
      level of a solid is directly related to the voltage on that solid, as
      measured with a voltmeter. Conventionally, in band structure plots the
      Fermi level is taken to be the zero of energy (an arbitrary choice).
The density of electrons in the material is simply the integral of the
FermiâDirac distribution times the density of states:
         N  /  V =  &#x222B;  &#x2212; &#x221E;   &#x221E;   g ( E ) f ( E )  d
      E   {\displaystyle N/V=\int _{-\infty }^{\infty }g(E)f(E)\,dE}  [N/V=\int
      _{-\infty }^{\infty }g(E)f(E)\,dE]
Although there are an infinite number of bands and thus an infinite number of
states, there are only a finite number of electrons to place in these bands.
The preferred value for the number of electrons is a consequence of
electrostatics: even though the surface of a material can be charged, the
internal bulk of a material prefers to be charge neutral. The condition of
charge neutrality means that N/V must match the density of protons in the
material. For this to occur, the material electrostatically adjusts itself,
shifting its band structure up or down in energy (thereby shifting g(E)), until
it is at the correct equilibrium with respect to the Fermi level.
*** Names of bands near the Fermi level (conduction band, valence band)[edit]
***
A solid has an infinite number of allowed bands, just as an atom has infinitely
many energy levels. However, most of the bands simply have too high energy, and
are usually disregarded under ordinary circumstances.[5] Conversely, there are
very low energy bands associated with the core orbitals (such as 1s_electrons).
These low-energy core bands are also usually disregarded since they remain
filled with electrons at all times, and are therefore inert.[6] Likewise,
materials have several band gaps throughout their band structure.
The most important bands and band gapsâthose relevant for electronics and
optoelectronicsâare those with energies near the Fermi level. The bands and
band gaps near the Fermi level are given special names, depending on the
material:
    * In a semiconductor or band_insulator, the Fermi level is surrounded by a
      band gap, referred to as the band gap (to distinguish it from the other
      band gaps in the band structure). The closest band above the band gap is
      called the conduction_band, and the closest band beneath the band gap is
      called the valence_band. The name "valence band" was coined by analogy to
      chemistry, since in semiconductors (and insulators) the valence band is
      built out of the valence_orbitals.
    * In a metal or semimetal, the Fermi level is inside of one or more allowed
      bands. In semimetals the bands are usually referred to as "conduction
      band" or "valence band" depending on whether the charge transport is more
      electron-like or hole-like, by analogy to semiconductors. In many metals,
      however, the bands are neither electron-like nor hole-like, and often
      just called "valence band" as they are made of valence orbitals.[7] The
      band gaps in a metal's band structure are not important for low energy
      physics, since they are too far from the Fermi level.
***** Theory in crystals[edit] *****
The ansatz is the special case of electron waves in a periodic crystal lattice
using Bloch_waves as treated generally in the dynamical_theory_of_diffraction.
Every crystal is a periodic structure which can be characterized by a Bravais
lattice, and for each Bravais_lattice we can determine the reciprocal_lattice,
which encapsulates the periodicity in a set of three reciprocal lattice vectors
(b1,b2,b3). Now, any periodic potential V(r) which shares the same periodicity
as the direct lattice can be expanded out as a Fourier_series whose only non-
vanishing components are those associated with the reciprocal lattice vectors.
So the expansion can be written as:
         V (  r  ) =  &#x2211;   K      V   K     e  i  K  &#x22C5;  r
      {\displaystyle V(\mathbf {r} )=\sum _{\mathbf {K} }{V_{\mathbf {K} }e^
      {i\mathbf {K} \cdot \mathbf {r} }}}  [V(\mathbf {r} )=\sum _{\mathbf {K}
      }{V_{\mathbf {K} }e^{i\mathbf {K} \cdot \mathbf {r} }}]
where K = m1b1 + m2b2 + m3b3 for any set of integers (m1,m2,m3).
From this theory, an attempt can be made to predict the band structure of a
particular material, however most ab initio methods for electronic structure
calculations fail to predict the observed band gap.
**** Nearly free electron approximation[edit] ****
Main articles: Nearly_free_electron_model, Free_electron_model, and
pseudopotential
In the nearly free electron approximation, interactions between electrons are
completely ignored. This approximation allows use of Bloch's_Theorem which
states that electrons in a periodic potential have wavefunctions and energies
which are periodic in wavevector up to a constant phase shift between
neighboring reciprocal_lattice vectors. The consequences of periodicity are
described mathematically by the Bloch wavefunction:
           &#x03A8;   n ,  k    (  r  ) =  e  i  k  &#x22C5;  r     u  n   (  r
      )   {\displaystyle {\Psi }_{n,\mathbf {k} }(\mathbf {r} )=e^{i\mathbf {k}
      \cdot \mathbf {r} }u_{n}(\mathbf {r} )}  [{\Psi }_{n,\mathbf {k} }
      (\mathbf {r} )=e^{i\mathbf {k} \cdot \mathbf {r} }u_{n}(\mathbf {r} )]
where the function      u  n   (  r  )   {\displaystyle u_{n}(\mathbf {r} )}
[u_{n}(\mathbf {r} )] is periodic over the crystal lattice, that is,
          u  n   (  r  ) =  u  n   (  r &#x2212; R  )   {\displaystyle u_{n}
      (\mathbf {r} )=u_{n}(\mathbf {r-R} )}  [u_{n}(\mathbf {r} )=u_{n}(\mathbf
      {r-R} )].
Here index n refers to the n-th energy band, wavevector k is related to the
direction of motion of the electron, r is the position in the crystal, and R is
the location of an atomic site.[8]
The NFE model works particularly well in materials like metals where distances
between neighbouring atoms are small. In such materials the overlap of atomic
orbitals and potentials on neighbouring atoms is relatively large. In that case
the wave_function of the electron can be approximated by a (modified) plane
wave. The band structure of a metal like aluminium even gets close to the empty
lattice_approximation.
**** Tight binding model[edit] ****
Main article: Tight_binding
The opposite extreme to the nearly free electron approximation assumes the
electrons in the crystal behave much like an assembly of constituent atoms.
This tight_binding_model assumes the solution to the time-independent single
electron SchrÃ¶dinger_equation     &#x03A8;   {\displaystyle \Psi }  [\Psi ] is
well approximated by a linear_combination of atomic_orbitals      &#x03C8;  n
(  r  )   {\displaystyle \psi _{n}(\mathbf {r} )}  [\psi _{n}(\mathbf {r} )].
[9]
         &#x03A8; (  r  ) =  &#x2211;  n ,  R     b  n ,  R     &#x03C8;  n
      (  r &#x2212; R  )   {\displaystyle \Psi (\mathbf {r} )=\sum _{n,\mathbf
      {R} }b_{n,\mathbf {R} }\psi _{n}(\mathbf {r-R} )}  [\Psi (\mathbf {r}
      )=\sum _{n,\mathbf {R} }b_{n,\mathbf {R} }\psi _{n}(\mathbf {r-R} )],
where the coefficients      b  n ,  R      {\displaystyle b_{n,\mathbf {R} }}
[b_{n,\mathbf {R} }] are selected to give the best approximate solution of this
form. Index n refers to an atomic energy level and R refers to an atomic site.
A more accurate approach using this idea employs Wannier_functions, defined by:
[10][11]
          a  n   (  r &#x2212; R  ) =    V  C    ( 2 &#x03C0;  )  3
      &#x222B;  BZ   d  k   e  &#x2212; i  k  &#x22C5; (  R &#x2212; r  )    u
      n  k      {\displaystyle a_{n}(\mathbf {r-R} )={\frac {V_{C}}{(2\pi )^
      {3}}}\int \limits _{\text{BZ}}d\mathbf {k} e^{-i\mathbf {k} \cdot
      (\mathbf {R-r} )}u_{n\mathbf {k} }}  [{\displaystyle a_{n}(\mathbf {r-R}
      )={\frac {V_{C}}{(2\pi )^{3}}}\int \limits _{\text{BZ}}d\mathbf {k} e^{-
      i\mathbf {k} \cdot (\mathbf {R-r} )}u_{n\mathbf {k} }}];
in which      u  n  k      {\displaystyle u_{n\mathbf {k} }}  [u_{n\mathbf {k}
}] is the periodic part of the Bloch wave and the integral is over the
Brillouin_zone. Here index n refers to the n-th energy band in the crystal. The
Wannier functions are localized near atomic sites, like atomic orbitals, but
being defined in terms of Bloch functions they are accurately related to
solutions based upon the crystal potential. Wannier functions on different
atomic sites R are orthogonal. The Wannier functions can be used to form the
SchrÃ¶dinger solution for the n-th energy band as:
          &#x03A8;  n ,  k    (  r  ) =  &#x2211;   R     e  &#x2212; i  k
      &#x22C5; (  R &#x2212; r  )    a  n   (  r &#x2212; R  )   {\displaystyle
      \Psi _{n,\mathbf {k} }(\mathbf {r} )=\sum _{\mathbf {R} }e^{-i\mathbf {k}
      \cdot (\mathbf {R-r} )}a_{n}(\mathbf {r-R} )}  [\Psi _{n,\mathbf {k} }
      (\mathbf {r} )=\sum _{\mathbf {R} }e^{-i\mathbf {k} \cdot (\mathbf {R-r}
      )}a_{n}(\mathbf {r-R} )].
The TB model works well in materials with limited overlap between atomic
orbitals and potentials on neighbouring atoms. Band structures of materials
like Si, GaAs, SiO2 and diamond for instance are well described by TB-
Hamiltonians on the basis of atomic sp3 orbitals. In transition_metals a mixed
TB-NFE model is used to describe the broad NFE conduction_band and the narrow
embedded TB d-bands. The radial functions of the atomic orbital part of the
Wannier functions are most easily calculated by the use of pseudopotential
methods. NFE, TB or combined NFE-TB band structure calculations,[12] sometimes
extended with wave function approximations based on pseudopotential methods,
are often used as an economic starting point for further calculations.
**** KKR model[edit] ****
Main article: Muffin-tin_approximation
The simplest form of this approximation centers non-overlapping spheres
(referred to as muffin tins) on the atomic positions. Within these regions, the
potential experienced by an electron is approximated to be spherically
symmetric about the given nucleus. In the remaining interstitial region, the
screened_potential is approximated as a constant. Continuity of the potential
between the atom-centered spheres and interstitial region is enforced.
A variational implementation was suggested by Korringa and by Kohn and
Rostocker, and is often referred to as the KKR_model.[13][14]
**** Density-functional theory[edit] ****
Main article: Density_functional_theory
See also: KohnâSham_equations
In recent physics literature, a large majority of the electronic structures and
band plots are calculated using density-functional_theory (DFT), which is not a
model but rather a theory, i.e., a microscopic first-principles theory of
condensed_matter_physics that tries to cope with the electron-electron many-
body problem via the introduction of an exchange-correlation term in the
functional of the electronic_density. DFT-calculated bands are in many cases
found to be in agreement with experimentally measured bands, for example by
angle-resolved_photoemission_spectroscopy (ARPES). In particular, the band
shape is typically well reproduced by DFT. But there are also systematic errors
in DFT bands when compared to experiment results. In particular, DFT seems to
systematically underestimate by about 30-40% the band gap in insulators and
semiconductors.[15]
It is commonly believed that DFT is a theory to predict ground_state properties
of a system only (e.g. the total_energy, the atomic_structure, etc.), and that
excited_state properties cannot be determined by DFT. This is a misconception.
In principle, DFT can determine any property (ground state or excited state) of
a system given a functional that maps the ground state density to that
property. This is the essence of the HohenbergâKohn theorem.[16] In practice,
however, no known functional exists that maps the ground state density to
excitation energies of electrons within a material. Thus, what in the
literature is quoted as a DFT band plot is a representation of the DFT
KohnâSham_energies, i.e., the energies of a fictive non-interacting system,
the KohnâSham system, which has no physical interpretation at all. The
KohnâSham electronic structure must not be confused with the real,
quasiparticle electronic structure of a system, and there is no Koopman's
theorem holding for KohnâSham energies, as there is for HartreeâFock
energies, which can be truly considered as an approximation for quasiparticle
energies. Hence, in principle, KohnâSham based DFT is not a band theory,
i.e., not a theory suitable for calculating bands and band-plots. In principle
time-dependent_DFT can be used to calculate the true band structure although in
practice this is often difficult. A popular approach is the use of hybrid
functionals, which incorporate a portion of HartreeâFock exact exchange; this
produces a substantial improvement in predicted bandgaps of semiconductors, but
is less reliable for metals and wide-bandgap materials.[17]
**** Green's function methods and the ab initio GW approximation[edit] ****
Main articles: Green's_function_(many-body_theory) and GreenâKubo_relations
To calculate the bands including electron-electron interaction many-body
effects, one can resort to so-called Green's_function methods. Indeed,
knowledge of the Green's function of a system provides both ground (the total
energy) and also excited state observables of the system. The poles of the
Green's function are the quasiparticle energies, the bands of a solid. The
Green's function can be calculated by solving the Dyson_equation once the self-
energy of the system is known. For real systems like solids, the self-energy is
a very complex quantity and usually approximations are needed to solve the
problem. One such approximation is the GW_approximation, so called from the
mathematical form the self-energy takes as the product Î£ = GW of the Green's
function G and the dynamically screened interaction W. This approach is more
pertinent when addressing the calculation of band plots (and also quantities
beyond, such as the spectral function) and can also be formulated in a
completely ab initio way. The GW approximation seems to provide band gaps of
insulators and semiconductors in agreement with experiment, and hence to
correct the systematic DFT underestimation.
**** Mott insulators[edit] ****
Main article: Mott_insulator
Although the nearly free electron approximation is able to describe many
properties of electron band structures, one consequence of this theory is that
it predicts the same number of electrons in each unit cell. If the number of
electrons is odd, we would then expect that there is an unpaired electron in
each unit cell, and thus that the valence band is not fully occupied, making
the material a conductor. However, materials such as CoO that have an odd
number of electrons per unit cell are insulators, in direct conflict with this
result. This kind of material is known as a Mott_insulator, and requires
inclusion of detailed electron-electron interactions (treated only as an
averaged effect on the crystal potential in band theory) to explain the
discrepancy. The Hubbard_model is an approximate theory that can include these
interactions. It can be treated non-perturbatively within the so-called
dynamical_mean_field_theory, which attempts to bridge the gap between the
nearly free electron approximation and the atomic limit. Formally, however, the
states are not non-interacting in this case and the concept of a band structure
is not adequate to describe these cases.
**** Others[edit] ****
Calculating band structures is an important topic in theoretical solid_state
physics. In addition to the models mentioned above, other models include the
following:
    * Empty_lattice_approximation: the "band structure" of a region of free
      space that has been divided into a lattice.
    * kÂ·p_perturbation_theory is a technique that allows a band structure to
      be approximately described in terms of just a few parameters. The
      technique is commonly used for semiconductors, and the parameters in the
      model are often determined by experiment.
    * The Kronig-Penney_Model, a one-dimensional rectangular well model useful
      for illustration of band formation. While simple, it predicts many
      important phenomena, but is not quantitative.
    * Hubbard_model
The band structure has been generalised to wavevectors that are complex
numbers, resulting in what is called a complex band structure, which is of
interest at surfaces and interfaces.
Each model describes some types of solids very well, and others poorly. The
nearly free electron model works well for metals, but poorly for non-metals.
The tight binding model is extremely accurate for ionic insulators, such as
metal_halide salts (e.g. NaCl).
***** Band diagrams[edit] *****
To understand how band structure changes relative to the Fermi level in real
space, a band structure plot is often first simplified in the form of a band
diagram. In a band diagram the vertical axis is energy while the horizontal
axis represents real space. Horizontal lines represent energy levels, while
blocks represent energy bands. When the horizontal lines in these diagram are
slanted then the energy of the level or band changes with distance.
Diagrammatically, this depicts the presence of an electric field within the
crystal system. Band diagrams are useful in relating the general band structure
properties of different materials to one another when placed in contact with
each other.
***** See also[edit] *****
 Wikimedia Commons has media related to Dispersion_relations_of_electrons.
    * Felix_Bloch â pioneer in the theory of band structure
    * Alan_Herries_Wilson â pioneer in the theory of band structure
    * Band-gap_engineering - the process of altering a material's band
      structure
***** References[edit] *****
   1. ^ a bHolgate, Sharon Ann (2009). Understanding_Solid_State_Physics. CRC
      Press. pp. 177â178. ISBN 978-1-4200-1232-3.
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
   3. ^Van Zeghbroeck, B. , 2011 (2011). "Section_2.3:_Energy_Bands".
      Principles of Semiconductor Devices. Electrical, Computer, Energy
      Engineering Dept., Univ. of Colorado at Boulder. Retrieved March 13,
      2017.
   4. ^ Band_structure_and_carrier_concentration
   5. ^"Electronic_Band_Structure" (PDF). www.springer.com. Springer. p. 24.
      Retrieved 10 November 2016.
   6. ^ High-energy bands are important for electron_diffraction physics, where
      the electrons can be injected into a material at high energies, seeStern,
      R.; Perry, J.; Boudreaux, D. (1969). "Low-Energy Electron-Diffraction
      Dispersion Surfaces and Band Structure in Three-Dimensional Mixed Laue
      and Bragg Reflections". Reviews of Modern Physics. 41 (2): 275. Bibcode:
      1969RvMP...41..275S. doi:10.1103/RevModPhys.41.275.
   7. .
   8. ^ Low-energy bands are however important in the Auger_effect.
   9. ^ In copper, for example, the effective mass is a tensor and also changes
      sign depending on the wave vector, as can be seen in the de_Haasâvan
      Alphen_effect; see http://www.phys.ufl.edu/fermisurface/
  10. ^ Kittel, p. 179
  11. ^ Kittel, pp. 245-248
  12. ^ Kittel, Eq. 42 p. 267
  13. ^Daniel Charles Mattis (1994). The_Many-Body_Problem:_Encyclopaedia_of
      Exactly_Solved_Models_in_One_Dimension. World Scientific. p. 340.
      ISBN 978-981-02-1476-0.
  14. ^Walter Ashley Harrison (1989). Electronic_Structure_and_the_Properties
      of_Solids. Dover Publications. ISBN 978-0-486-66021-9.
  15. ^Joginder Singh Galsin (2001). Impurity_Scattering_in_Metal_Alloys.
      Springer. Appendix C. ISBN 978-0-306-46574-1.
  16. ^Kuon Inoue, Kazuo Ohtaka (2004). Photonic_Crystals. Springer. p. 66.
      ISBN 978-3-540-20559-3.
  17. ^ Theoretical_study_on_copperâs_energetics_and_magnetism_in_TiO2
      polymorphs Journal of Applied Physics, 2013,113(23), 233913
  18. ^Hohenberg, P; Kohn, W. (Nov 1964). "Inhomogeneous Electron Gas". Phys.
      Rev. 136 (3B): B864âB871. Bibcode:1964PhRv..136..864H. doi:10.1103/
      PhysRev.136.B864.
  19. ^Paier, J.; Marsman, M.; Hummer, K.; Kresse, G.; Gerber, IC.; AngyÃ¡n,
      JG. (Apr 2006). "Screened hybrid density functionals applied to solids".
      J Chem Phys. 124 (15): 154709. Bibcode:2006JChPh.124o4709P. doi:10.1063/
      1.2187006. PMID 16674253.
***** Bibliography[edit] *****
    * Charles Kittel (1996). Introduction to Solid State Physics (Seventh ed.).
      New York: Wiley. ISBN 978-0-471-11181-8.
***** Further reading[edit] *****
   1. Microelectronics, by Jacob Millman and Arvin Gabriel,
   2. ISBN 0-07-463736-3, Tata McGraw-Hill Edition.
   3. Solid State Physics, by Neil Ashcroft and N. David Mermin,
   4. ISBN 0-03-083993-9
   5. Elementary Solid State Physics: Principles and Applications, by M. Ali
      Omar,
   6. ISBN 0-201-60733-6
   7. Electronic and Optoelectronic Properties of Semiconductor Structures â
      Chapter 2 and 3 by Jasprit Singh,
   8. ISBN 0-521-82379-X
   9. Electronic Structure: Basic Theory and Practical Methods by Richard
      Martin,
  10. ISBN 0-521-78285-6
  11. Condensed Matter Physics by Michael P. Marder,
  12. ISBN 0-471-17779-2
  13. Computational Methods in Solid State Physics by V V Nemoshkalenko and
      N.V. Antonov,
  14. ISBN 90-5699-094-2
  15. Elementary Electronic Structure by Walter A. Harrison,
  16. ISBN 981-238-708-0
  17. Pseudopotentials in the theory of metals by Walter A. Harrison, W.A.
      Benjamin (New York) 1966
  18. Tutorial_on_Bandstructure_Methods_by_Dr._Vasileska_(2008)
***** External links[edit] *****
    *  Media related to Electronic_band_structures at Wikimedia Commons
    * Animation,_applications_and_research_about_quantum_physics_and_band
      theory (UniversitÃ© Paris Sud)

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Electronic_band_structure&oldid=903052899"
Categories:
    * Electronic_band_structures
    * Solid_state_engineering
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_June_2013
    * Articles_with_unsourced_statements_from_October_2015
    * Commons_category_link_is_on_Wikidata
    * Commons_category_link_is_locally_defined
    * Articles_containing_video_clips
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ä¸­æ
Edit_links
    * This page was last edited on 23 June 2019, at 06:12 (UTC).
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
