The following text has been accessed from https://en.wikipedia.org/wiki/MOSFET at Thu Aug 8 22:49:13 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** MOSFET ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Transistor used for amplifying or switching electronic signals
"MOS technology" redirects here. For the company, see MOS_Technology.
MOSFET, showing gate (G), body (B), source (S) and drain (D) terminals. The
gate is separated from the body by an insulating layer (pink).
The metalâoxideâsemiconductor field-effect transistor (MOSFET, MOS-FET, or
MOS FET), also known as the metalâoxideâsilicon transistor (MOS),[1] is a
type of field-effect_transistor (FET) that is fabricated by the controlled
oxidation of silicon. It has an insulated gate, whose voltage determines the
conductivity of the device. This ability to change conductivity with the amount
of applied voltage can be used for amplifying or switching electronic signals.
The MOSFET was invented by Mohamed_Atalla and Dawon_Kahng at Bell_Labs in 1959,
[2][1][3] and is the most widely used semiconductor_device in the world.[4]
The main advantage of a MOSFET is that it requires almost no input current to
control the load current, when compared with bipolar_transistors (bipolar
junction transistors, or BJTs). In an enhancement mode MOSFET, voltage applied
to the gate terminal increases the conductivity of the device. In depletion
mode transistors, voltage applied at the gate reduces the conductivity.[5]
MOSFETs are capable of high_scalability (Moore's_law and Dennard_scaling),[6]
with increasing miniaturisation,[7] and can be easily scaled down to smaller
dimensions.[8] They also consume much less power, and allow higher density,
than bipolar transistors.[9] The MOSFET is also cheaper[10] and has relatively
simple processing steps, resulting in a high manufacturing_yield.[8] Since
MOSFETs can be made with either p-type or n-type_semiconductors (PMOS or NMOS
logic, respectively), complementary pairs of MOS transistors can be used to
make switching circuits with very low power consumption, in the form of CMOS
logic.
The name "metal-oxide-silicon" (MOS) typically refers to a metal_gate, oxide
insulation, and silicon semiconductor.[1] However, the "metal" in the name
MOSFET is sometimes a misnomer, because the gate material can also be a layer
of polysilicon (polycrystalline silicon). Similarly, "oxide" in the name can
also be a misnomer, as different dielectric materials can be used with the aim
of obtaining strong channels with smaller applied voltages.
The MOSFET is the most widely manufactured device in history,[11][12] with an
estimated total of 13 sextillion MOS transistors manufactured as of 2018.[11]
It is by far the most common transistor used in digital_circuits[13][14] and
power_electronics,[15] and is fundamental to building high-density integrated
circuits (ICs)[1] and VLSI (very large-scale integration) devices.[8] It
revolutionized the electronics_industry,[16][17] has been central to the
microelectronic and digital_revolutions,[18][19] and is the fundamental
building block of digital_electronics in the information_age.[20][21] Billions
of MOS transistors are often found within a single integrated circuit, such as
a memory_chip or microprocessor. The US_Patent_and_Trademark_Office calls the
MOSFET a "groundbreaking invention that transformed_life_and_culture around the
world".[22]
A cross-section through an nMOSFET when the gate voltage VGS is below the
threshold for making a conductive channel; there is little or no conduction
between the terminals drain and source; the switch is off. When the gate is
more positive, it attracts electrons, inducing an n-type conductive channel in
the substrate below the oxide, which allows electrons to flow between the n-
doped terminals; the switch is on.
Simulation of formation of inversion channel (electron density) and attainment
of threshold vol­tage (IV) in a nanowire MOSFET. Note: threshold_voltage for
this device lies around 0.45 V
⁰
***** Contents *****
    * 1_History
    * 2_Composition
    * 3_Operation
          o 3.1_Metalâoxideâsemiconductor_structure
          o 3.2_MOS_capacitors_and_band_diagrams
          o 3.3_Structure_and_channel_formation
          o 3.4_Modes_of_operation
          o 3.5_Body_effect
    * 4_Circuit_symbols
    * 5_Applications
          o 5.1_MOS_integrated_circuits
          o 5.2_CMOS_circuits
                # 5.2.1_Digital
                # 5.2.2_Analog
          o 5.3_Analog_switches
                # 5.3.1_Single-type
                # 5.3.2_Dual-type_(CMOS)
    * 6_Construction
          o 6.1_Gate_material
          o 6.2_Insulator
          o 6.3_Junction_design
    * 7_Scaling
    * 8_Other_MOSFET_types
          o 8.1_Depletion-mode
          o 8.2_Metal-insulator-semiconductor_field-effect_transistor_(MISFET)
          o 8.3_Multi-gate_field-effect_transistor_(MuGET)
          o 8.4_NMOS_logic
          o 8.5_Power_MOSFET
          o 8.6_Double-diffused_metalâoxideâsemiconductor_(DMOS)
          o 8.7_Radiation-hardened-by-design_(RHBD)
    * 9_See_also
    * 10_References
    * 11_External_links
***** History[edit] *****
The basic principle of the field-effect_transistor (FET) was first patented by
Julius_Edgar_Lilienfeld in 1925.[23] However, this early FET design was not
practical.[14] The FET concept was later also theorized by Oskar_Heil in the
1930s and William_Shockley in the 1940s,[2] but there was no working practical
FET built at the time.[14] Shockley's research team initially attempted to
build a working FET, by trying to modulate the conductivity of a semiconductor,
but they were unsuccessful, mainly due to problems with the surface_states, the
dangling_bond, and the germanium and copper compound materials. In the course
of trying to understand the mysterious reasons behind their failure to build a
working FET, this led them to instead invent the bipolar point-contact and
junction_transistors.[24][25] None of these early FET proposals involved
thermally_oxidized silicon, which later made the MOS transistor possible.[26]
Mohamed_Atalla (left) and Dawon_Kahng (right) invented the MOSFET in 1959.
A breakthrough in FET research came with the work of Mohamed_Atalla in the late
1950s.[25] He investigated the surface properties of silicon semiconductors at
Bell_Labs, where he adopted a new method of semiconductor_device_fabrication,
coating a silicon_wafer with an insulating layer of silicon_oxide, so that
electricity could reliably penetrate to the conducting silicon below,
overcoming the surface states that prevented electricity from reaching the
semiconducting layer. This is known as surface_passivation, a method that later
became critical to the semiconductor_industry as it made possible the mass-
production of silicon integrated_circuits (ICs).[13][14][3] The surface
passivation method, which substantially reduced the influence of the dangling
bond that had prevented Shockley's research team from building a working FET,
[25] was presented by Atalla in 1957.[27] Building on the surface passivation
method, Atalla developed the metalâoxideâsemiconductor (MOS) process,[13]
with the use of thermally oxidized silicon.[26][28] He proposed that the MOS
process could be used to build the first working silicon FET, which he began
working on building with the help of his colleague Dawon_Kahng.[13]
The MOSFET was invented by Mohamed Atalla and Dawon Kahng in 1959,[2][3] and
presented in 1960.[29][30][31] Operationally and structurally different from
the bipolar_junction_transistor,[32] the MOSFET was made by putting an
insulating layer on the surface of the semiconductor and then placing a
metallic gate electrode on that. It used crystalline silicon for the
semiconductor and a thermally_oxidized layer of silicon_dioxide for the
insulator. The silicon MOSFET did not generate localized electron traps at the
interface between the silicon and its native oxide layer, and thus was
inherently free from the trapping and scattering of carriers that had impeded
the performance of earlier attempts at building a field-effect transistor.
With its high_scalability,[6] and much lower power consumption and higher
density than bipolar junction transistors,[9] the MOSFET made it possible to
build high-density ICs,[1] allowing the integration of more than 10,000
transistors in a single small integrated circuit chip.[33]
There were originally two types of MOSFET logic, PMOS (p-type MOS) and NMOS (n-
type MOS).[2] Both types were developed by Atalla and Kahng when they
originally invented the MOSFET. They fabricated both PMOS and NMOS devices.[3]
A new type of MOSFET logic, CMOS, was developed by Chih-Tang_Sah and Frank
Wanlass at Fairchild_Semiconductor in 1963.[34]
The thin-film_transistor (TFT), a type of MOSFET distinct from the standard
bulk MOSFET,[35] was invented by Paul_K._Weimer at RCA in 1962, building on the
earlier work of Atalla and Kahng on MOSFETs.[36] TFTs are the basis for TFT_LCD
technology, used by liquid-crystal_display (LCD) displays and LCD_televisions.
[37]
The first modern memory_cells were introduced in 1965, when John Schmidt
designed the first 64-bit MOS SRAM (static RAM).[38] In 1967, Robert_H._Dennard
of IBM filed a patent for a single-transistor DRAM (dynamic RAM) memory cell,
using a MOSFET.[39] The first report of a floating-gate_MOSFET (FGMOS) was made
by Dawon Kahng and Simon_Sze in 1967.[40] The earliest practical application of
FGMOS was floating-gate memory cells, which Kahng and Sze proposed could be
used to produce reprogrammable_ROM (read-only_memory).[41] Floating-gate memory
cells later became the basis for non-volatile_memory (NVM) technologies
including EPROM (erasable programable ROM), EEPROM (electrically erasable
programmable ROM) and flash_memory.[42]
The MOSFET enabled physicists to study electron_behavior_in_a_two-dimensional
gas. In a MOSFET, conduction electrons travel in a thin surface layer, and a
"gate" voltage controls the number of charge carriers in this layer. This
allows researchers to explore quantum_effects by operating high-purity MOSFETs
at liquid_helium temperatures.[43] In 1978, the Gakushuin_University
researchers Jun-ichi Wakabayashi and Shinji Kawaji observed the Hall_effect in
experiments carried out on the inversion layer of MOSFETs.[44] In 1980, Klaus
von_Klitzing, working at the high magnetic field laboratory in Grenoble with
silicon-based MOSFET samples developed by Michael_Pepper and Gerhard Dorda,
made the unexpected discovery of the quantum_Hall_effect.[45][43] For this
finding, von Klitzing was awarded the 1985 Nobel_Prize_in_Physics.[43]
***** Composition[edit] *****
Photomicrograph of two metal-gate MOSFETs in a test pattern. Probe pads for two
gates and three source/drain nodes are labeled.
Usually the semiconductor of choice is silicon. Recently, some chip
manufacturers, most notably IBM and Intel, have started using a chemical
compound of silicon and germanium (SiGe) in MOSFET channels. Unfortunately,
many semiconductors with better electrical properties than silicon, such as
gallium_arsenide, do not form good semiconductor-to-insulator interfaces, and
thus are not suitable for MOSFETs. Research continues[when?] on creating
insulators with acceptable electrical characteristics on other semiconductor
materials.
To overcome the increase in power consumption due to gate current leakage, a
high-Îº_dielectric is used instead of silicon dioxide for the gate insulator,
while polysilicon is replaced by metal gates (e.g. Intel, 2009[46]).
The gate is separated from the channel by a thin insulating layer,
traditionally of silicon dioxide and later of silicon_oxynitride. Some
companies have started to introduce a high-Îº dielectric and metal gate
combination in the 45_nanometer node.
When a voltage is applied between the gate and body terminals, the electric
field generated penetrates through the oxide and creates an inversion layer or
channel at the semiconductor-insulator interface. The inversion layer provides
a channel through which current can pass between source and drain terminals.
Varying the voltage between the gate and body modulates the conductivity of
this layer and thereby controls the current flow between drain and source. This
is known as enhancement mode.
***** Operation[edit] *****
Metalâoxideâsemiconductor structure on p-type silicon
**** Metalâoxideâsemiconductor structure[edit] ****
The traditional metalâoxideâsemiconductor (MOS) structure is obtained by
growing a layer of silicon_dioxide (SiO
2) on top of a silicon substrate, commonly by thermal_oxidation and depositing
a layer of metal or polycrystalline_silicon (the latter is commonly used). As
the silicon dioxide is a dielectric material, its structure is equivalent to a
planar capacitor, with one of the electrodes replaced by a semiconductor.
When a voltage is applied across a MOS structure, it modifies the distribution
of charges in the semiconductor. If we consider a p-type semiconductor (with
N  A     {\displaystyle N_{\text{A}}}  [N_{{\text{A}}}] the density of
acceptors, p the density of holes; p = NA in neutral bulk), a positive voltage,
V  GB     {\displaystyle V_{\text{GB}}}  [{\displaystyle V_{\text{GB}}}], from
gate to body (see figure) creates a depletion_layer by forcing the positively
charged holes away from the gate-insulator/semiconductor interface, leaving
exposed a carrier-free region of immobile, negatively charged acceptor ions
(see doping_(semiconductor)). If      V  GB     {\displaystyle V_{\text{GB}}}
[{\displaystyle V_{\text{GB}}}] is high enough, a high concentration of
negative charge carriers forms in an inversion layer located in a thin layer
next to the interface between the semiconductor and the insulator.
Conventionally, the gate voltage at which the volume density of electrons in
the inversion layer is the same as the volume density of holes in the body is
called the threshold_voltage. When the voltage between transistor gate and
source (VGS) exceeds the threshold voltage (Vth), the difference is known as
overdrive_voltage.
This structure with p-type body is the basis of the n-type MOSFET, which
requires the addition of n-type source and drain regions.
**** MOS capacitors and band diagrams[edit] ****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (January 2019)(Learn_how_and_when_to_remove_this_template_message)
The MOS capacitor structure is the heart of the MOSFET. Consider a MOS
capacitor where the silicon base is of p-type. If a positive voltage is applied
at the gate, holes which are at the surface of the p-type substrate will be
repelled by the electric field generated by the voltage applied. At first, the
holes will simply be repelled and what will remain on the surface will be
immobile (negative) atoms of the acceptor type, which creates a depletion
region on the surface. Remember that a hole is created by an acceptor atom,
e.g. Boron, which has one less electron than Silicon. One might ask how can
holes be repelled if they are actually non-entities? The answer is that what
really happens is not that a hole is repelled, but electrons are attracted by
the positive field, and fill these holes, creating a depletion region where no
charge carriers exist because the electron is now fixed onto the atom and
immobile.
As the voltage at the gate increases, there will be a point at which the
surface above the depletion region will be converted from p-type into n-type,
as electrons from the bulk area will start to get attracted by the larger
electric field. This is known as inversion. The threshold voltage at which this
conversion happens is one of the most important parameters in a MOSFET.
In the case of a p-type bulk, inversion happens when the intrinsic energy level
at the surface becomes smaller than the Fermi_level at the surface. One can see
this from a band diagram. Remember that the Fermi level defines the type of
semiconductor in discussion. If the Fermi level is equal to the Intrinsic
level, the semiconductor is of intrinsic, or pure type. If the Fermi level lies
closer to the conduction band (valence band) then the semiconductor type will
be of n-type (p-type). Therefore, when the gate voltage is increased in a
positive sense (for the given example), this will "bend" the intrinsic energy
level band so that it will curve downwards towards the valence band. If the
Fermi level lies closer to the valence band (for p-type), there will be a point
when the Intrinsic level will start to cross the Fermi level and when the
voltage reaches the threshold voltage, the intrinsic level does cross the Fermi
level, and that is what is known as inversion. At that point, the surface of
the semiconductor is inverted from p-type into n-type. Remember that as said
above, if the Fermi level lies above the Intrinsic level, the semiconductor is
of n-type, therefore at Inversion, when the Intrinsic level reaches and crosses
the Fermi level (which lies closer to the valence band), the semiconductor type
changes at the surface as dictated by the relative positions of the Fermi and
Intrinsic energy levels.
**** Structure and channel formation[edit] ****
See also: Field_effect_(semiconductor)
Channel formation in nMOS MOSFET shown as band_diagram: Top panels: An applied
gate voltage bends bands, depleting holes from surface (left). The charge
inducing the bending is balanced by a layer of negative acceptor-ion charge
(right). Bottom panel: A larger applied voltage further depletes holes but
conduction band lowers enough in energy to populate a conducting channel
CâV profile for a bulk MOSFET with different oxide thickness. The leftmost
part of the curve corresponds to accumulation. The valley in the middle
corresponds to depletion. The curve on the right corresponds to inversion
A MOSFET is based on the modulation of charge concentration by a MOS
capacitance between a body electrode and a gate electrode located above the
body and insulated from all other device regions by a gate dielectric layer. If
dielectrics other than an oxide are employed, the device may be referred to as
a metal-insulator-semiconductor FET (MISFET). Compared to the MOS capacitor,
the MOSFET includes two additional terminals (source and drain), each connected
to individual highly doped regions that are separated by the body region. These
regions can be either p or n type, but they must both be of the same type, and
of opposite type to the body region. The source and drain (unlike the body) are
highly doped as signified by a "+" sign after the type of doping.
If the MOSFET is an n-channel or nMOS FET, then the source and drain are n+
regions and the body is a p region. If the MOSFET is a p-channel or pMOS FET,
then the source and drain are p+ regions and the body is a n region. The source
is so named because it is the source of the charge carriers (electrons for n-
channel, holes for p-channel) that flow through the channel; similarly, the
drain is where the charge carriers leave the channel.
The occupancy of the energy bands in a semiconductor is set by the position of
the Fermi_level relative to the semiconductor energy-band edges.
See also: Depletion_region
With sufficient gate voltage, the valence band edge is driven far from the
Fermi level, and holes from the body are driven away from the gate.
At larger gate bias still, near the semiconductor surface the conduction band
edge is brought close to the Fermi level, populating the surface with electrons
in an inversion layer or n-channel at the interface between the p region and
the oxide. This conducting channel extends between the source and the drain,
and current is conducted through it when a voltage is applied between the two
electrodes. Increasing the voltage on the gate leads to a higher electron
density in the inversion layer and therefore increases the current flow between
the source and drain. For gate voltages below the threshold value, the channel
is lightly populated, and only a very small subthreshold_leakage current can
flow between the source and the drain.
When a negative gate-source voltage (positive source-gate) is applied, it
creates a p-channel at the surface of the n region, analogous to the n-channel
case, but with opposite polarities of charges and voltages. When a voltage less
negative than the threshold value (a negative voltage for the p-channel) is
applied between gate and source, the channel disappears and only a very small
subthreshold current can flow between the source and the drain. The device may
comprise a silicon_on_insulator device in which a buried oxide is formed below
a thin semiconductor layer. If the channel region between the gate dielectric
and the buried oxide region is very thin, the channel is referred to as an
ultrathin channel region with the source and drain regions formed on either
side in or above the thin semiconductor layer. Other semiconductor materials
may be employed. When the source and drain regions are formed above the channel
in whole or in part, they are referred to as raised source/drain regions.
                   Comparison of n- and p-type MOSFETs[47]
Parameter                nMOSFET                    pMOSFET
Source/drain type        n-type                     p-type
Channel type             n-type                     p-type
(MOS capacitor)
Gate Polysilicon         n+                         p+
type Metal               Ïm ~ Si conduction band Ïm ~ Si valence band
Well type                p-type                     n-type
                             * Positive                 * Negative
Threshold voltage, Vth         (enhancement)              (enhancement)
                             * Negative (depletion)     * Positive (depletion)
Band-bending             Downwards                  Upwards
Inversion layer carriers Electrons                  Holes
Substrate type           p-type                     n-type
**** Modes of operation[edit] ****
Source tied to the body to ensure no body bias:
top left: Subthreshold, top right: Ohmic mode, bottom left: Active mode at
onset of pinch-off, bottom right: Active mode well into pinch-off â channel
length modulation evident
Example application of an n-channel MOSFET. When the switch is pushed, the LED
lights up.[48]
The operation of a MOSFET can be separated into three different modes,
depending on the voltages at the terminals. In the following discussion, a
simplified algebraic model is used.[49] Modern MOSFET characteristics are more
complex than the algebraic model presented here.[50]
For an enhancement-mode, n-channel MOSFET, the three operational modes are:
  Cutoff, subthreshold, and weak-inversion mode
When VGS < Vth:
where      V  GS     {\displaystyle V_{\text{GS}}}  [{\displaystyle V_{\text
{GS}}}] is gate-to-source bias and      V  th     {\displaystyle V_{\text{th}}}
[{\displaystyle V_{\text{th}}}] is the threshold_voltage of the device.
According to the basic threshold model, the transistor is turned off, and there
is no conduction between drain and source. A more accurate model considers the
effect of thermal energy on the FermiâDirac_distribution of electron energies
which allow some of the more energetic electrons at the source to enter the
channel and flow to the drain. This results in a subthreshold current that is
an exponential function of gate-source voltage. While the current between drain
and source should ideally be zero when the transistor is being used as a
turned-off switch, there is a weak-inversion current, sometimes called
subthreshold leakage.
In weak inversion where the source is tied to bulk, the current varies
exponentially with      V  GS     {\displaystyle V_{\text{GS}}}  [
{\displaystyle V_{\text{GS}}}] as given approximately by:[51][52]
          I  D   &#x2248;  I  D0    e     V  GS   &#x2212;  V  th     n  V  T
      ,   {\displaystyle I_{\text{D}}\approx I_{\text{D0}}e^{\frac {V_{\text
      {GS}}-V_{\text{th}}}{nV_{\text{T}}}},}  [{\displaystyle I_{\text
      {D}}\approx I_{\text{D0}}e^{\frac {V_{\text{GS}}-V_{\text{th}}}{nV_{\text
      {T}}}},}]
where      I  D0     {\displaystyle I_{\text{D0}}}  [{\displaystyle I_{\text
{D0}}}] = current at      V  GS   =  V  th     {\displaystyle V_{\text{GS}}=V_
{\text{th}}}  [{\displaystyle V_{\text{GS}}=V_{\text{th}}}], the thermal
voltage      V  T   = k T  /  q   {\displaystyle V_{\text{T}}=kT/q}  [
{\displaystyle V_{\text{T}}=kT/q}] and the slope factor n is given by:
         n = 1 +    C  dep    C  ox     ,    {\displaystyle n=1+{\frac {C_
      {\text{dep}}}{C_{\text{ox}}}},\,}  [{\displaystyle n=1+{\frac {C_{\text
      {dep}}}{C_{\text{ox}}}},\,}]
with      C  dep     {\displaystyle C_{\text{dep}}}  [{\displaystyle C_{\text
{dep}}}] = capacitance of the depletion layer and      C  ox     {\displaystyle
C_{\text{ox}}}  [{\displaystyle C_{\text{ox}}}] = capacitance of the oxide
layer. This equation is generally used, but is only an adequate approximation
for the source tied to the bulk. For the source not tied to the bulk, the
subthreshold equation for drain current in saturation is[53][54]
          I  D   &#x2248;  I  D0    e    &#x03BA;  (   V  G   &#x2212;  V  th
      )  &#x2212;  V  S     V  T      ,   {\displaystyle I_{\text{D}}\approx I_
      {\text{D0}}e^{\frac {\kappa \left(V_{\text{G}}-V_{\text{th}}\right)-V_
      {\text{S}}}{V_{\text{T}}}},}  [{\displaystyle I_{\text{D}}\approx I_
      {\text{D0}}e^{\frac {\kappa \left(V_{\text{G}}-V_{\text{th}}\right)-V_
      {\text{S}}}{V_{\text{T}}}},}]
where the     &#x03BA;   {\displaystyle \kappa }  [\kappa ] is the channel
divider that is given by:
         &#x03BA; =    C  ox     C  ox   +  C  D      ,   {\displaystyle \kappa
      ={\frac {C_{\text{ox}}}{C_{\text{ox}}+C_{\text{D}}}},}  [{\displaystyle
      \kappa ={\frac {C_{\text{ox}}}{C_{\text{ox}}+C_{\text{D}}}},}]
with      C  D     {\displaystyle C_{\text{D}}}  [{\displaystyle C_{\text{D}}}]
= capacitance of the depletion layer and      C  ox     {\displaystyle C_{\text
{ox}}}  [{\displaystyle C_{\text{ox}}}] = capacitance of the oxide layer. In a
long-channel device, there is no drain voltage dependence of the current once
V  DS   &#x226B;  V  T     {\displaystyle V_{\text{DS}}\gg V_{\text{T}}}  [
{\displaystyle V_{\text{DS}}\gg V_{\text{T}}}], but as channel length is
reduced drain-induced_barrier_lowering introduces drain voltage dependence that
depends in a complex way upon the device geometry (for example, the channel
doping, the junction doping and so on). Frequently, threshold voltage Vth for
this mode is defined as the gate voltage at which a selected value of current
ID0 occurs, for example, ID0 = 1 Î¼A, which may not be the same Vth-value used
in the equations for the following modes.
Some micropower analog circuits are designed to take advantage of subthreshold
conduction.[55][56][57] By working in the weak-inversion region, the MOSFETs in
these circuits deliver the highest possible transconductance-to-current ratio,
namely:      g  m    /   I  D   = 1  /   (  n  V  T    )    {\displaystyle g_
{m}/I_{\text{D}}=1/\left(nV_{\text{T}}\right)}  [{\displaystyle g_{m}/I_{\text
{D}}=1/\left(nV_{\text{T}}\right)}], almost that of a bipolar transistor.[58]
The subthreshold IâV_curve depends exponentially upon threshold voltage,
introducing a strong dependence on any manufacturing variation that affects
threshold voltage; for example: variations in oxide thickness, junction depth,
or body doping that change the degree of drain-induced barrier lowering. The
resulting sensitivity to fabricational variations complicates optimization for
leakage and performance.[59][60]
MOSFET drain current vs. drain-to-source voltage for several values of      V
GS   &#x2212;  V  th     {\displaystyle V_{\text{GS}}-V_{\text{th}}}  [
{\displaystyle V_{\text{GS}}-V_{\text{th}}}]; the boundary between linear
(Ohmic) and saturation (active) modes is indicated by the upward curving
parabola
Cross section of a MOSFET operating in the linear (Ohmic) region; strong
inversion region present even near drain
Cross section of a MOSFET operating in the saturation (active) region; channel
exhibits channel_pinching near drain
  Triode mode or linear region (also known as the ohmic mode[61][62])
When VGS > Vth and VDS < VGS â Vth:
The transistor is turned on, and a channel has been created which allows
current between the drain and the source. The MOSFET operates like a resistor,
controlled by the gate voltage relative to both the source and drain voltages.
The current from drain to source is modeled as:
          I  D   =  &#x03BC;  n    C  ox     W L    (   (   V  GS   &#x2212;  V
      t h     )   V  DS   &#x2212;      V  DS     2   2    )    {\displaystyle
      I_{\text{D}}=\mu _{n}C_{\text{ox}}{\frac {W}{L}}\left(\left(V_{\text
      {GS}}-V_{\rm {th}}\right)V_{\text{DS}}-{\frac {{V_{\text{DS}}}^{2}}
      {2}}\right)}  [{\displaystyle I_{\text{D}}=\mu _{n}C_{\text{ox}}{\frac
      {W}{L}}\left(\left(V_{\text{GS}}-V_{\rm {th}}\right)V_{\text{DS}}-{\frac
      {{V_{\text{DS}}}^{2}}{2}}\right)}]
where      &#x03BC;  n     {\displaystyle \mu _{n}}  [\mu _{n}] is the charge-
carrier effective mobility,     W   {\displaystyle W}  [W] is the gate width,
L   {\displaystyle L}  [L] is the gate length and      C  ox     {\displaystyle
C_{\text{ox}}}  [{\displaystyle C_{\text{ox}}}] is the gate oxide capacitance
per unit area. The transition from the exponential subthreshold region to the
triode region is not as sharp as the equations suggest.
  Saturation or active mode[63][64]
When VGS > Vth and VDS â¥ (VGS â Vth):
The switch is turned on, and a channel has been created, which allows current
between the drain and source. Since the drain voltage is higher than the source
voltage, the electrons spread out, and conduction is not through a narrow
channel but through a broader, two- or three-dimensional current distribution
extending away from the interface and deeper in the substrate. The onset of
this region is also known as pinch-off to indicate the lack of channel region
near the drain. Although the channel does not extend the full length of the
device, the electric field between the drain and the channel is very high, and
conduction continues. The drain current is now weakly dependent upon drain
voltage and controlled primarily by the gate-source voltage, and modeled
approximately as:
          I  D   =     &#x03BC;  n    C  ox    2     W L     [   V  GS
      &#x2212;  V  th    ]   2    [  1 + &#x03BB; (  V  DS   &#x2212;  V  DSsat
      )  ]  .   {\displaystyle I_{\text{D}}={\frac {\mu _{n}C_{\text{ox}}}{2}}
      {\frac {W}{L}}\left[V_{\text{GS}}-V_{\text{th}}\right]^{2}\left[1+\lambda
      (V_{\text{DS}}-V_{\text{DSsat}})\right].}  [{\displaystyle I_{\text{D}}=
      {\frac {\mu _{n}C_{\text{ox}}}{2}}{\frac {W}{L}}\left[V_{\text{GS}}-V_
      {\text{th}}\right]^{2}\left[1+\lambda (V_{\text{DS}}-V_{\text
      {DSsat}})\right].}]
The additional factor involving Î», the channel-length modulation parameter,
models current dependence on drain voltage due to the Early_effect, or channel
length_modulation. According to this equation, a key design parameter, the
MOSFET transconductance is:
          g  m   =    &#x2202;  I  D     &#x2202;  V  GS      =    2  I  D
      V  GS   &#x2212;  V  th      =    2  I  D     V  ov     ,
      {\displaystyle g_{m}={\frac {\partial I_{D}}{\partial V_{\text{GS}}}}=
      {\frac {2I_{\text{D}}}{V_{\text{GS}}-V_{\text{th}}}}={\frac {2I_{\text
      {D}}}{V_{\text{ov}}}},}  [{\displaystyle g_{m}={\frac {\partial I_{D}}
      {\partial V_{\text{GS}}}}={\frac {2I_{\text{D}}}{V_{\text{GS}}-V_{\text
      {th}}}}={\frac {2I_{\text{D}}}{V_{\text{ov}}}},}]
where the combination Vov = VGS â Vth is called the overdrive_voltage,[65]
and where VDSsat = VGS â Vth accounts for a small discontinuity in      I  D
{\displaystyle I_{\text{D}}}  [{\displaystyle I_{\text{D}}}] which would
otherwise appear at the transition between the triode and saturation regions.
Another key design parameter is the MOSFET output resistance rout given by:
          r  out   =   1  &#x03BB;  I  D        {\displaystyle r_{\text{out}}=
      {\frac {1}{\lambda I_{\text{D}}}}}  [{\displaystyle r_{\text{out}}={\frac
      {1}{\lambda I_{\text{D}}}}}].
rout is the inverse of gDS where      g  DS   =    &#x2202;  I  DS     &#x2202;
V  DS        {\displaystyle g_{\text{DS}}={\frac {\partial I_{\text{DS}}}
{\partial V_{\text{DS}}}}}  [{\displaystyle g_{\text{DS}}={\frac {\partial I_
{\text{DS}}}{\partial V_{\text{DS}}}}}]. ID is the expression in saturation
region.
If Î» is taken as zero, an infinite output resistance of the device results
that leads to unrealistic circuit predictions, particularly in analog circuits.
As the channel length becomes very short, these equations become quite
inaccurate. New physical effects arise. For example, carrier transport in the
active mode may become limited by velocity_saturation. When velocity saturation
dominates, the saturation drain current is more nearly linear than quadratic in
VGS. At even shorter lengths, carriers transport with near zero scattering,
known as quasi-ballistic_transport. In the ballistic regime, the carriers
travel at an injection velocity that may exceed the saturation velocity and
approaches the Fermi_velocity at high inversion charge density. In addition,
drain-induced barrier lowering increases off-state (cutoff) current and
requires an increase in threshold voltage to compensate, which in turn reduces
the saturation current.
**** Body effect[edit] ****
Band_diagram showing body effect. VSB splits Fermi levels Fn for electrons and
Fp for holes, requiring larger VGB to populate the conduction band in an nMOS
MOSFET
The occupancy of the energy bands in a semiconductor is set by the position of
the Fermi_level relative to the semiconductor energy-band edges. Application of
a source-to-substrate reverse bias of the source-body pn-junction introduces a
split between the Fermi levels for electrons and holes, moving the Fermi level
for the channel further from the band edge, lowering the occupancy of the
channel. The effect is to increase the gate voltage necessary to establish the
channel, as seen in the figure. This change in channel strength by application
of reverse bias is called the 'body effect'.
Simply put, using an nMOS example, the gate-to-body bias VGB positions the
conduction-band energy levels, while the source-to-body bias VSB positions the
electron Fermi level near the interface, deciding occupancy of these levels
near the interface, and hence the strength of the inversion layer or channel.
The body effect upon the channel can be described using a modification of the
threshold voltage, approximated by the following equation:
          V  TB   =  V  T 0   + &#x03B3;  (     V  SB   + 2  &#x03C6;  B
      &#x2212;   2  &#x03C6;  B      )  ,   {\displaystyle V_{\text{TB}}=V_
      {T0}+\gamma \left({\sqrt {V_{\text{SB}}+2\varphi _{B}}}-{\sqrt {2\varphi
      _{B}}}\right),}  [{\displaystyle V_{\text{TB}}=V_{T0}+\gamma \left({\sqrt
      {V_{\text{SB}}+2\varphi _{B}}}-{\sqrt {2\varphi _{B}}}\right),}]
where VTB is the threshold voltage with substrate bias present, and VT0 is the
zero-VSB value of threshold voltage,     &#x03B3;   {\displaystyle \gamma }
[\gamma ] is the body effect parameter, and 2ÏB is the approximate potential
drop between surface and bulk across the depletion layer when VSB = 0 and gate
bias is sufficient to ensure that a channel is present.[66] As this equation
shows, a reverse bias VSB > 0 causes an increase in threshold voltage VTB and
therefore demands a larger gate voltage before the channel populates.
The body can be operated as a second gate, and is sometimes referred to as the
"back gate"; the body effect is sometimes called the "back-gate effect".[67]
***** Circuit symbols[edit] *****
A variety of symbols are used for the MOSFET. The basic design is generally a
line for the channel with the source and drain leaving it at right angles and
then bending back at right angles into the same direction as the channel.
Sometimes three line segments are used for enhancement_mode and a solid line
for depletion mode (see depletion_and_enhancement_modes). Another line is drawn
parallel to the channel for the gate.
The bulk or body connection, if shown, is shown connected to the back of the
channel with an arrow indicating pMOS or nMOS. Arrows always point from P to N,
so an NMOS (N-channel in P-well or P-substrate) has the arrow pointing in (from
the bulk to the channel). If the bulk is connected to the source (as is
generally the case with discrete devices) it is sometimes angled to meet up
with the source leaving the transistor. If the bulk is not shown (as is often
the case in IC design as they are generally common bulk) an inversion symbol is
sometimes used to indicate PMOS, alternatively an arrow on the source may be
used in the same way as for bipolar transistors (out for nMOS, in for pMOS).
Comparison of enhancement-mode and depletion-mode MOSFET symbols, along with
JFET symbols. The orientation of the symbols, (most significantly the position
of source relative to drain) is such that more positive voltages appear higher
on the page than less positive voltages, implying current flowing "down" the
page:[68][69][70]
          [JFET_P-      [IGFET_P-Ch   [IGFET_P-Ch_Enh [Mosfet_P- [IGFET_P-Ch
P-channel Channel       Enh           Labelled        Ch         Dep
          Labelled.svg] Labelled.svg] simplified.svg] Sedra.svg] Labelled.svg]
          [JFET_N-      [IGFET_N-Ch   [IGFET_N-Ch_Enh [Mosfet_N- [IGFET_N-Ch
N-channel Channel       Enh           Labelled        Ch         Dep
          Labelled.svg] Labelled.svg] simplified.svg] Sedra.svg] Labelled.svg]
          JFET          MOSFET enh.   MOSFET enh. (no bulk)      MOSFET dep.
In schematics where G, S, D are not labeled, the detailed features of the
symbol indicate which terminal is source and which is drain. For enhancement-
mode and depletion-mode MOSFET symbols (in columns two and five), the source
terminal is the one connected to the triangle. Additionally, in this diagram,
the gate is shown as an "L" shape, whose input leg is closer to S than D, also
indicating which is which. However, these symbols are often drawn with a "T"
shaped gate (as elsewhere on this page), so it is the triangle which must be
relied upon to indicate the source terminal.
For the symbols in which the bulk, or body, terminal is shown, it is here shown
internally connected to the source (i.e., the black triangles in the diagrams
in columns 2 and 5). This is a typical configuration, but by no means the only
important configuration. In general, the MOSFET is a four-terminal device, and
in integrated circuits many of the MOSFETs share a body connection, not
necessarily connected to the source terminals of all the transistors.
***** Applications[edit] *****
Semiconductor
manufacturing
processes
[4-fach-NAND-C10.JPG]
    * 10 Âµm.0 â 1971
    * 06 Âµm.0 â 1974
    * 03 Âµm.0 â 1977
    * 01.5 Âµm â 1981
    * 01 Âµm.0 â 1984
    * 800 nm â 1987
    * 600 nm â 1990
    * 350 nm â 1994
    * 250 nm â 1996
    * 180 nm â 1999
    * 130 nm â 2001
    * 090 nm â 2003
    * 065 nm â 2005
    * 045 nm â 2007
    * 032 nm â 2009
    * 022 nm â 2012
    * 014 nm â 2014
    * 010 nm â 2016
    * 007 nm â 2018
    * 005 nm â 2019
    * 003 nm â ~2021
===============================================================================
    * Half-nodes
    * Scale_examples
    * Density
    * Device
    * MOSFET
    * Moore's_law
    * Multigate_device
    * Semiconductor
    * v
    * t
    * e
The MOSFET revolutionized the electronics_industry,[16] including power
electronics,[71] consumer_electronics, control systems, and computers.[17] It
is the most common transistor in computers, electronics,[14] and communications
technology (such as smartphones).[22] The MOSFET has been central to the
microelectronics revolution since the late 20th century.[18]
The MOS transistor has been the fundamental building block of modern digital
electronics since the late 20th century, paving the way for the digital_age and
information_age.[20][21] The MOS transistor is the basic building block of the
digital_revolution.[19] It has been described as the "workhorse of the
electronics industry" due to being the building block of every microprocessor,
memory_chip and telecommunication_circuit in use,[72] and the basis for nearly
every silicon integrated_circuit (IC),[73] thin-film_transistor (TFT)[35] and
graphics_processing_unit (GPU), among other uses.[74]
The MOSFET is the most widely manufactured device in history.[11][12] As of
2013, billions of MOS transistors are manufactured every day.[1] As of 2018, an
estimated total of 13 sextillion MOS transistors have been manufactured.[11]
Digital integrated_circuits such as microprocessors and memory_devices contain
thousands to billions of integrated MOSFET transistors on each device,
providing the basic switching functions required to implement logic_gates and
data storage. There are also memory devices which contain at least a trillion
MOS transistors, such as a 256 GB microSD memory_card, larger than the number
of stars in the Milky_Way galaxy.[72]
The US_Patent_and_Trademark_Office calls the MOSFET a "groundbreaking invention
that transformed_life_and_culture around the world"[22] and the Computer
History_Museum credits it with "irrevocably changing the human experience."[20]
The MOSFET is on the list_of_IEEE_milestones in electronics.[75]
Discrete devices are widely used in applications such as switch_mode_power
supplies, variable-frequency_drives and other power_electronics applications
where each device may be switching thousands of watts. Radio-frequency
amplifiers up to the UHF spectrum use MOSFET transistors as analog signal and
power amplifiers. Radio systems also use MOSFETs as oscillators, or mixers to
convert frequencies. MOSFET devices are also applied in audio-frequency power
amplifiers for public address systems, sound_reinforcement and home and
automobile sound systems.[citation_needed]
**** MOS integrated circuits[edit] ****
See also: Integrated_circuit and Three-dimensional_integrated_circuit
Following the development of clean_rooms to reduce contamination to levels
never before thought necessary, and of photolithography[76] and the planar
process to allow circuits to be made in very few steps, the SiâSiO2 system
possessed the technical attractions of low cost of production (on a per circuit
basis) and ease of integration. Largely because of these two factors, the
MOSFET has become the most widely used type of transistor in integrated
circuits (ICs), and it is the most critical device component in modern ICs.[77]
The earliest experimental MOS IC was a 16-transistor chip built by Fred Heiman
and Steven Hofstein at RCA in 1962.[10] General_Microelectronics later
introduced the first commercial MOS integrated circuit in 1964; it consisted of
120 p-channel transistors,[78] and was a 20-bit shift_register, developed by
Robert Norman.[10] By the early 1970s, MOS technology enabled the integration
of more than 10,000 transistors in a single LSI (large-scale integration) chip.
[33] In 1967, Bell_Labs researchers Robert Kerwin, Donald Klein and John Sarace
developed the self-aligned_gate (silicon-gate) MOS transistor, which Fairchild
Semiconductor researchers Federico_Faggin and Tom Klein used to develop the
first silicon-gate MOS IC.[79]
The MOSFET is the basis of every microprocessor.[72] The earliest
microprocessors were all MOS microprocessors, built with MOS LSI circuits. The
first multi-chip microprocessors, the Four-Phase_Systems_AL1 in 1969 and the
Garrett_AiResearch MP944 in 1970, were developed with multiple MOS LSI chips.
The first commercial single-chip microprocessor, the Intel_4004, was developed
by Federico_Faggin, using his silicon-gate MOS IC technology, with Intel
engineers Marcian_Hoff and Stan_Mazor, and Busicom engineer Masatoshi_Shima.
[80] With the arrival of CMOS microprocessors in 1975, the term "MOS
microprocessors" began to refer to chips fabricated entirely from PMOS_logic or
fabricated entirely from NMOS_logic, contrasted with "CMOS microprocessors" and
"bipolar bit-slice processors".[81]
One of the earliest influential consumer_electronic products enabled by MOS LSI
circuits was the electronic pocket_calculator.[33] In 1965, the Victor 3900
desktop_calculator was the first MOS LSI calculator, with 29 MOS LSI chips.[82]
In 1967 the Texas_Instruments Cal-Tech was the first prototype electronic
handheld_calculator, with three MOS LSI chips, and it was later released as the
Canon Pocketronic in 1970.[83] The Sharp_QT-8D desktop calculator was the first
mass-produced LSI MOS calculator in 1969,[82] and the Sharp_EL-8 which used
four MOS LSI chips was the first commercial electronic handheld calculator in
1970.[83] The first true electronic pocket calculator was the Busicom LE-120A
HANDY LE, which used a single MOS LSI calculator-on-a-chip from Mostek, and was
released in 1971.[83]
**** CMOS circuits[edit] ****
Main article: CMOS
The MOSFET is used in digital complementary_metalâoxideâsemiconductor
(CMOS) logic,[84] which uses p- and n-channel MOSFETs as building blocks.
Overheating is a major concern in integrated_circuits since ever more
transistors are packed into ever smaller chips. CMOS logic reduces power
consumption because no current flows (ideally), and thus no power is consumed,
except when the inputs to logic_gates are being switched. CMOS accomplishes
this current reduction by complementing every nMOSFET with a pMOSFET and
connecting both gates and both drains together. A high voltage on the gates
will cause the nMOSFET to conduct and the pMOSFET not to conduct and a low
voltage on the gates causes the reverse. During the switching time as the
voltage goes from one state to another, both MOSFETs will conduct briefly. This
arrangement greatly reduces power consumption and heat generation.
CMOS was developed by Chih-Tang_Sah and Frank_Wanlass at Fairchild
Semiconductor in 1963.[34] CMOS had lower power consumption, but was initially
slower than NMOS, which was more widely used for computers in the 1970s. In
1978, Hitachi introduced the twin-well CMOS process, which allowed CMOS to
match the performance of NMOS with less power consumption. The twin-well CMOS
process eventually overtook NMOS as the most common semiconductor_manufacturing
process for computers in the 1980s.[85]
*** Digital[edit] ***
The growth of digital technologies like the microprocessor has provided the
motivation to advance MOSFET technology faster than any other type of silicon-
based transistor.[86] A big advantage of MOSFETs for digital switching is that
the oxide layer between the gate and the channel prevents DC current from
flowing through the gate, further reducing power consumption and giving a very
large input impedance. The insulating oxide between the gate and channel
effectively isolates a MOSFET in one logic stage from earlier and later stages,
which allows a single MOSFET output to drive a considerable number of MOSFET
inputs. Bipolar transistor-based logic (such as TTL) does not have such a high
fanout capacity. This isolation also makes it easier for the designers to
ignore to some extent loading effects between logic stages independently. That
extent is defined by the operating frequency: as frequencies increase, the
input impedance of the MOSFETs decreases.
*** Analog[edit] ***
The MOSFET's advantages in digital circuits do not translate into supremacy in
all analog_circuits. The two types of circuit draw upon different features of
transistor behavior. Digital circuits switch, spending most of their time
either fully on or fully off. The transition from one to the other is only of
concern with regards to speed and charge required. Analog circuits depend on
operation in the transition region where small changes to Vgs can modulate the
output (drain) current. The JFET and bipolar_junction_transistor (BJT) are
preferred for accurate matching (of adjacent devices in integrated circuits),
higher transconductance and certain temperature characteristics which simplify
keeping performance predictable as circuit temperature varies.
Nevertheless, MOSFETs are widely used in many types of analog circuits because
of their own advantages (zero gate current, high and adjustable output
impedance and improved robustness vs. BJTs which can be permanently degraded by
even lightly breaking down the emitter-base).[vague] The characteristics and
performance of many analog circuits can be scaled up or down by changing the
sizes (length and width) of the MOSFETs used. By comparison, in bipolar
transistors the size of the device does not significantly affect its
performance.[citation_needed] MOSFETs' ideal characteristics regarding gate
current (zero) and drain-source offset voltage (zero) also make them nearly
ideal switch elements, and also make switched_capacitor analog circuits
practical. In their linear region, MOSFETs can be used as precision resistors,
which can have a much higher controlled resistance than BJTs. In high power
circuits, MOSFETs sometimes have the advantage of not suffering from thermal
runaway as BJTs do.[dubious  – discuss] Also, MOSFETs can be configured to
perform as capacitors and gyrator_circuits which allow op-amps made from them
to appear as inductors, thereby allowing all of the normal analog devices on a
chip (except for diodes, which can be made smaller than a MOSFET anyway) to be
built entirely out of MOSFETs. This means that complete analog circuits can be
made on a silicon chip in a much smaller space and with simpler fabrication
techniques. MOSFETS are ideally suited to switch inductive loads because of
tolerance to inductive kickback.
Some ICs combine analog and digital MOSFET circuitry on a single mixed-signal
integrated_circuit, making the needed board space even smaller. This creates a
need to isolate the analog circuits from the digital circuits on a chip level,
leading to the use of isolation rings and silicon_on_insulator (SOI). Since
MOSFETs require more space to handle a given amount of power than a BJT,
fabrication processes can incorporate BJTs and MOSFETs into a single device.
Mixed-transistor devices are called bi-FETs (bipolar FETs) if they contain just
one BJT-FET and BiCMOS (bipolar-CMOS) if they contain complementary BJT-FETs.
Such devices have the advantages of both insulated gates and higher current
density.
**** Analog switches[edit] ****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (September 2016)(Learn_how_and_when_to_remove_this_template_message)
MOSFET analog switches use the MOSFET to pass analog signals when on, and as a
high impedance when off. Signals flow in both directions across a MOSFET
switch. In this application, the drain and source of a MOSFET exchange places
depending on the relative voltages of the source/drain electrodes. The source
is the more negative side for an N-MOS or the more positive side for a P-MOS.
All of these switches are limited on what signals they can pass or stop by
their gate-source, gate-drain and sourceâdrain voltages; exceeding the
voltage, current, or power limits will potentially damage the switch.
*** Single-type[edit] ***
This analog switch uses a four-terminal simple MOSFET of either P or N type.
In the case of an n-type switch, the body is connected to the most negative
supply (usually GND) and the gate is used as the switch control. Whenever the
gate voltage exceeds the source voltage by at least a threshold voltage, the
MOSFET conducts. The higher the voltage, the more the MOSFET can conduct. An N-
MOS switch passes all voltages less than Vgate â Vtn. When the switch is
conducting, it typically operates in the linear (or ohmic) mode of operation,
since the source and drain voltages will typically be nearly equal.
In the case of a P-MOS, the body is connected to the most positive voltage, and
the gate is brought to a lower potential to turn the switch on. The P-MOS
switch passes all voltages higher than Vgate â Vtp (threshold voltage Vtp is
negative in the case of enhancement-mode P-MOS).
*** Dual-type (CMOS)[edit] ***
This "complementary" or CMOS type of switch uses one P-MOS and one N-MOS FET to
counteract the limitations of the single-type switch. The FETs have their
drains and sources connected in parallel, the body of the P-MOS is connected to
the high potential (VDD) and the body of the N-MOS is connected to the low
potential (gnd). To turn the switch on, the gate of the P-MOS is driven to the
low potential and the gate of the N-MOS is driven to the high potential. For
voltages between VDD â Vtn and gnd â Vtp, both FETs conduct the signal; for
voltages less than gnd â Vtp, the N-MOS conducts alone; and for voltages
greater than VDD â Vtn, the P-MOS conducts alone.
The voltage limits for this switch are the gate-source, gate-drain and source-
drain voltage limits for both FETs. Also, the P-MOS is typically two to three
times wider than the N-MOS, so the switch will be balanced for speed in the two
directions.
Tri-state_circuitry sometimes incorporates a CMOS MOSFET switch on its output
to provide for a low-ohmic, full-range output when on, and a high-ohmic, mid-
level signal when off.
***** Construction[edit] *****
**** Gate material[edit] ****
The primary criterion for the gate material is that it is a good conductor.
Highly doped polycrystalline_silicon is an acceptable but certainly not ideal
conductor, and also suffers from some more technical deficiencies in its role
as the standard gate material. Nevertheless, there are several reasons favoring
use of polysilicon:
   1. The threshold_voltage (and consequently the drain to source on-current)
      is modified by the work_function difference between the gate material and
      channel material. Because polysilicon is a semiconductor, its work
      function can be modulated by adjusting the type and level of doping.
      Furthermore, because polysilicon has the same bandgap as the underlying
      silicon channel, it is quite straightforward to tune the work function to
      achieve low threshold voltages for both NMOS and PMOS devices. By
      contrast, the work functions of metals are not easily modulated, so
      tuning the work_function to obtain low_threshold_voltages (LVT) becomes a
      significant challenge. Additionally, obtaining low-threshold devices on
      both PMOS and NMOS devices sometimes requires the use of different metals
      for each device type. While bimetallic integrated circuits (i.e., one
      type of metal for gate electrodes of NFETS and a second type of metal for
      gate electrodes of PFETS) are not common, they are known in patent
      literature and provide some benefit in terms of tuning electrical
      circuits' overall electrical performance.
   2. The silicon-SiO2 interface has been well studied and is known to have
      relatively few defects. By contrast many metal-insulator interfaces
      contain significant levels of defects which can lead to Fermi_level
      pinning, charging, or other phenomena that ultimately degrade device
      performance.
   3. In the MOSFET IC_fabrication process, it is preferable to deposit the
      gate material prior to certain high-temperature steps in order to make
      better-performing transistors. Such high temperature steps would melt
      some metals, limiting the types of metal that can be used in a metal-
      gate-based process.
While polysilicon gates have been the de facto standard for the last twenty
years, they do have some disadvantages which have led to their likely future
replacement by metal gates. These disadvantages include:
    * Polysilicon is not a great conductor (approximately 1000 times more
      resistive than metals) which reduces the signal propagation speed through
      the material. The resistivity can be lowered by increasing the level of
      doping, but even highly doped polysilicon is not as conductive as most
      metals. To improve conductivity further, sometimes a high-temperature
      metal such as tungsten, titanium, cobalt, and more recently nickel is
      alloyed with the top layers of the polysilicon. Such a blended material
      is called silicide. The silicide-polysilicon combination has better
      electrical properties than polysilicon alone and still does not melt in
      subsequent processing. Also the threshold voltage is not significantly
      higher than with polysilicon alone, because the silicide material is not
      near the channel. The process in which silicide is formed on both the
      gate electrode and the source and drain regions is sometimes called
      salicide, self-aligned silicide.
    * When the transistors are extremely scaled down, it is necessary to make
      the gate dielectric layer very thin, around 1 nm in state-of-the-art
      technologies. A phenomenon observed here is the so-called poly_depletion,
      where a depletion layer is formed in the gate polysilicon layer next to
      the gate dielectric when the transistor is in the inversion. To avoid
      this problem, a metal gate is desired. A variety of metal gates such as
      tantalum, tungsten, tantalum_nitride, and titanium_nitride are used,
      usually in conjunction with high-Îº_dielectrics. An alternative is to use
      fully silicided polysilicon gates, a process known as FUSI.
Present high performance CPUs use metal gate technology, together with high-Îº
dielectrics, a combination known as high-Îº, metal gate (HKMG). The
disadvantages of metal gates are overcome by a few techniques:[87]
   1. The threshold voltage is tuned by including a thin "work function metal"
      layer between the high-Îº dielectric and the main metal. This layer is
      thin enough that the total work function of the gate is influenced by
      both the main metal and thin metal work functions (either due to alloying
      during annealing, or simply due to the incomplete screening by the thin
      metal). The threshold voltage thus can be tuned by the thickness of the
      thin metal layer.
   2. High-Îº dielectrics are now well studied, and their defects are
      understood.
   3. HKMG processes exist that do not require the metals to experience high
      temperature anneals; other processes select metals that can survive the
      annealing step.
**** Insulator[edit] ****
As devices are made smaller, insulating layers are made thinner, often through
steps of thermal_oxidation or localised oxidation of silicon (LOCOS). For nano-
scaled devices, at some point tunneling of carriers through the insulator from
the channel to the gate electrode takes place. To reduce the resulting leakage
current, the insulator can be made thinner by choosing a material with a higher
dielectric constant. To see how thickness and dielectric constant are related,
note that Gauss's_law connects field to charge as:
         Q = &#x03BA;  &#x03F5;  0   E ,   {\displaystyle Q=\kappa \epsilon _
      {0}E,}  [{\displaystyle Q=\kappa \epsilon _{0}E,}]
with Q = charge density, Îº = dielectric constant, Îµ0 = permittivity of empty
space and E = electric field. From this law it appears the same charge can be
maintained in the channel at a lower field provided Îº is increased. The
voltage on the gate is given by:
          V  G   =  V  ch   + E   t  ins   =  V  ch   +    Q  t  ins
      &#x03BA;  &#x03F5;  0      ,   {\displaystyle V_{\text{G}}=V_{\text
      {ch}}+E\,t_{\text{ins}}=V_{\text{ch}}+{\frac {Qt_{\text{ins}}}{\kappa
      \epsilon _{0}}},}  [{\displaystyle V_{\text{G}}=V_{\text{ch}}+E\,t_{\text
      {ins}}=V_{\text{ch}}+{\frac {Qt_{\text{ins}}}{\kappa \epsilon _{0}}},}]
with VG = gate voltage, Vch = voltage at channel side of insulator, and tins =
insulator thickness. This equation shows the gate voltage will not increase
when the insulator thickness increases, provided Îº increases to keep tins / Îº
= constant (see the article on high-Îº dielectrics for more detail, and the
section in this article on gate-oxide_leakage).
The insulator in a MOSFET is a dielectric which can in any event be silicon
oxide, formed by LOCOS but many other dielectric materials are employed. The
generic term for the dielectric is gate dielectric since the dielectric lies
directly below the gate electrode and above the channel of the MOSFET.
**** Junction design[edit] ****
The source-to-body and drain-to-body junctions are the object of much attention
because of three major factors: their design affects the current-voltage_(I-V)
characteristics of the device, lowering output resistance, and also the speed
of the device through the loading effect of the junction capacitances, and
finally, the component of stand-by power dissipation due to junction leakage.
MOSFET showing shallow junction extensions, raised source and drain and halo
implant. Raised source and drain separated from gate by oxide spacers
The drain induced barrier lowering of the threshold voltage and channel_length
modulation effects upon I-V curves are reduced by using shallow junction
extensions. In addition, halo doping can be used, that is, the addition of very
thin heavily doped regions of the same doping type as the body tight against
the junction walls to limit the extent of depletion_regions.[88]
The capacitive effects are limited by using raised source and drain geometries
that make most of the contact area border thick dielectric instead of silicon.
[89]
These various features of junction design are shown (with artistic_license) in
the figure.
***** Scaling[edit] *****
 This section is written like a personal_reflection,_personal_essay,_or
 argumentative_essay that states a Wikipedia editor's personal feelings or
 presents an original argument about a topic. Please help_improve_it by
 rewriting it in an encyclopedic_style. (September 2016)(Learn_how_and_when_to
 remove_this_template_message)
Further information: Dennard_scaling
Trend of Intel CPU transistor gate length
MOSFET version of gain-boosted current_mirror; M1 and M2 are in active mode,
while M3 and M4 are in Ohmic mode, and act like resistors. The operational
amplifier provides feedback that maintains a high output resistance.
Over the past decades, the MOSFET (as used for digital logic) has continually
been scaled down in size; typical MOSFET channel lengths were once several
micrometres, but modern integrated circuits are incorporating MOSFETs with
channel lengths of tens of nanometers. Robert_Dennard's work on scaling_theory
was pivotal in recognising that this ongoing reduction was possible. Intel
began production of a process featuring a 32 nm feature size (with the channel
being even shorter) in late 2009. The semiconductor industry maintains a
"roadmap", the ITRS,[90] which sets the pace for MOSFET development.
Historically, the difficulties with decreasing the size of the MOSFET have been
associated with the semiconductor device fabrication process, the need to use
very low voltages, and with poorer electrical performance necessitating circuit
redesign and innovation (small MOSFETs exhibit higher leakage currents and
lower output resistance).
Smaller MOSFETs are desirable for several reasons. The main reason to make
transistors smaller is to pack more and more devices in a given chip area. This
results in a chip with the same functionality in a smaller area, or chips with
more functionality in the same area. Since fabrication costs for a
semiconductor_wafer are relatively fixed, the cost per integrated circuits is
mainly related to the number of chips that can be produced per wafer. Hence,
smaller ICs allow more chips per wafer, reducing the price per chip. In fact,
over the past 30 years the number of transistors per chip has been doubled
every 2â3 years once a new technology node is introduced. For example, the
number of MOSFETs in a microprocessor fabricated in a 45_nm technology can well
be twice as many as in a 65_nm chip. This doubling of transistor density was
first observed by Gordon_Moore in 1965 and is commonly referred to as Moore's
law.[91] It is also expected that smaller transistors switch faster. For
example, one approach to size reduction is a scaling of the MOSFET that
requires all device dimensions to reduce proportionally. The main device
dimensions are the channel length, channel width, and oxide thickness. When
they are scaled down by equal factors, the transistor channel resistance does
not change, while gate capacitance is cut by that factor. Hence, the RC_delay
of the transistor scales with a similar factor. While this has been
traditionally the case for the older technologies, for the state-of-the-art
MOSFETs reduction of the transistor dimensions does not necessarily translate
to higher chip speed because the delay due to interconnections is more
significant.
Producing MOSFETs with channel lengths much smaller than a micrometre is a
challenge, and the difficulties of semiconductor device fabrication are always
a limiting factor in advancing integrated circuit technology. Though processes
such as ALD have improved fabrication for small components, the small size of
the MOSFET (less than a few tens of nanometers) has created operational
problems:
  Higher subthreshold conduction
      As MOSFET geometries shrink, the voltage that can be applied to the gate
      must be reduced to maintain reliability. To maintain performance, the
      threshold voltage of the MOSFET has to be reduced as well. As threshold
      voltage is reduced, the transistor cannot be switched from complete turn-
      off to complete turn-on with the limited voltage swing available; the
      circuit design is a compromise between strong current in the on case and
      low current in the off case, and the application determines whether to
      favor one over the other. Subthreshold leakage (including subthreshold
      conduction, gate-oxide leakage and reverse-biased junction leakage),
      which was ignored in the past, now can consume upwards of half of the
      total power consumption of modern high-performance VLSI chips.[92][93]
  Increased gate-oxide leakage
      The gate oxide, which serves as insulator between the gate and channel,
      should be made as thin as possible to increase the channel conductivity
      and performance when the transistor is on and to reduce subthreshold
      leakage when the transistor is off. However, with current gate oxides
      with a thickness of around 1.2 nm (which in silicon is ~5 atoms thick)
      the quantum_mechanical phenomenon of electron_tunneling occurs between
      the gate and channel, leading to increased power consumption. Silicon
      dioxide has traditionally been used as the gate insulator. Silicon
      dioxide however has a modest dielectric constant. Increasing the
      dielectric constant of the gate dielectric allows a thicker layer while
      maintaining a high capacitance (capacitance is proportional to dielectric
      constant and inversely proportional to dielectric thickness). All else
      equal, a higher dielectric thickness reduces the quantum_tunneling
      current through the dielectric between the gate and the channel.
      Insulators that have a larger dielectric_constant than silicon dioxide
      (referred to as high-Îº_dielectrics), such as group IVb metal silicates
      e.g. hafnium and zirconium silicates and oxides are being used to reduce
      the gate leakage from the 45 nanometer technology node onwards. On the
      other hand, the barrier height of the new gate insulator is an important
      consideration; the difference in conduction_band energy between the
      semiconductor and the dielectric (and the corresponding difference in
      valence_band energy) also affects leakage current level. For the
      traditional gate oxide, silicon dioxide, the former barrier is
      approximately 8 eV. For many alternative dielectrics the value is
      significantly lower, tending to increase the tunneling current, somewhat
      negating the advantage of higher dielectric constant. The maximum gate-
      source voltage is determined by the strength of the electric field able
      to be sustained by the gate dielectric before significant leakage occurs.
      As the insulating dielectric is made thinner, the electric field strength
      within it goes up for a fixed voltage. This necessitates using lower
      voltages with the thinner dielectric.
  Increased junction leakage
      To make devices smaller, junction design has become more complex, leading
      to higher doping levels, shallower junctions, "halo" doping and so forth,
      [94][95] all to decrease drain-induced barrier lowering (see the section
      on junction_design). To keep these complex junctions in place, the
      annealing steps formerly used to remove damage and electrically active
      defects must be curtailed[96] increasing junction leakage. Heavier doping
      is also associated with thinner depletion layers and more recombination
      centers that result in increased leakage current, even without lattice
      damage.
  Drain-induced_barrier_lowering (DIBL) and VT roll off
      Because of the short-channel_effect, channel formation is not entirely
      done by the gate, but now the drain and source also affect the channel
      formation. As the channel length decreases, the depletion regions of the
      source and drain come closer together and make the threshold voltage (VT)
      a function of the length of the channel. This is called VT roll-off. VT
      also becomes function of drain to source voltage VDS. As we increase the
      VDS, the depletion regions increase in size, and a considerable amount of
      charge is depleted by the VDS. The gate voltage required to form the
      channel is then lowered, and thus, the VT decreases with an increase in
      VDS. This effect is called drain induced barrier lowering (DIBL).
  Lower output resistance
      For analog operation, good gain requires a high MOSFET output impedance,
      which is to say, the MOSFET current should vary only slightly with the
      applied drain-to-source voltage. As devices are made smaller, the
      influence of the drain competes more successfully with that of the gate
      due to the growing proximity of these two electrodes, increasing the
      sensitivity of the MOSFET current to the drain voltage. To counteract the
      resulting decrease in output resistance, circuits are made more complex,
      either by requiring more devices, for example the cascode and cascade
      amplifiers, or by feedback circuitry using operational_amplifiers, for
      example a circuit like that in the adjacent figure.
  Lower transconductance
      The transconductance of the MOSFET decides its gain and is proportional
      to hole or electron_mobility (depending on device type), at least for low
      drain voltages. As MOSFET size is reduced, the fields in the channel
      increase and the dopant impurity levels increase. Both changes reduce the
      carrier mobility, and hence the transconductance. As channel lengths are
      reduced without proportional reduction in drain voltage, raising the
      electric field in the channel, the result is velocity saturation of the
      carriers, limiting the current and the transconductance.
  Interconnect capacitance
      Traditionally, switching time was roughly proportional to the gate
      capacitance of gates. However, with transistors becoming smaller and more
      transistors being placed on the chip, interconnect_capacitance (the
      capacitance of the metal-layer connections between different parts of the
      chip) is becoming a large percentage of capacitance.[97][98] Signals have
      to travel through the interconnect, which leads to increased delay and
      lower performance.
  Heat production
      The ever-increasing density of MOSFETs on an integrated circuit creates
      problems of substantial localized heat generation that can impair circuit
      operation. Circuits operate more slowly at high temperatures, and have
      reduced reliability and shorter lifetimes. Heat sinks and other cooling
      devices and methods are now required for many integrated circuits
      including microprocessors. Power_MOSFETs are at risk of thermal_runaway.
      As their on-state resistance rises with temperature, if the load is
      approximately a constant-current load then the power loss rises
      correspondingly, generating further heat. When the heatsink is not able
      to keep the temperature low enough, the junction temperature may rise
      quickly and uncontrollably, resulting in destruction of the device.
  Process variations
      With MOSFETs becoming smaller, the number of atoms in the silicon that
      produce many of the transistor's properties is becoming fewer, with the
      result that control of dopant numbers and placement is more erratic.
      During chip manufacturing, random process variations affect all
      transistor dimensions: length, width, junction depths, oxide thickness
      etc., and become a greater percentage of overall transistor size as the
      transistor shrinks. The transistor characteristics become less certain,
      more statistical. The random nature of manufacture means we do not know
      which particular example MOSFETs actually will end up in a particular
      instance of the circuit. This uncertainty forces a less optimal design
      because the design must work for a great variety of possible component
      MOSFETs. See process_variation, design_for_manufacturability, reliability
      engineering, and statistical_process_control.[99]
  Modeling challenges
      Modern ICs are computer-simulated with the goal of obtaining working
      circuits from the very first manufactured lot. As devices are
      miniaturized, the complexity of the processing makes it difficult to
      predict exactly what the final devices look like, and modeling of
      physical processes becomes more challenging as well. In addition,
      microscopic variations in structure due simply to the probabilistic
      nature of atomic processes require statistical (not just deterministic)
      predictions. These factors combine to make adequate simulation and "right
      the first time" manufacture difficult.
***** Other MOSFET types[edit] *****
**** Depletion-mode[edit] ****
Further information: Depletion_and_enhancement_modes and Depletion-load_NMOS
logic
There are depletion-mode MOSFET devices, which are less commonly used than the
standard enhancement-mode devices already described. These are MOSFET devices
that are doped so that a channel exists even with zero voltage from gate to
source. To control the channel, a negative voltage is applied to the gate (for
an n-channel device), depleting the channel, which reduces the current flow
through the device. In essence, the depletion-mode device is equivalent to a
normally_closed (on) switch, while the enhancement-mode device is equivalent to
a normally_open (off) switch.[100]
Due to their low noise_figure in the RF region, and better gain, these devices
are often preferred to bipolars in RF_front-ends such as in TV sets.
Depletion-mode MOSFET families include BF960 by Siemens and Telefunken, and the
BF980 in the 1980s by Philips (later to become NXP_Semiconductors), whose
derivatives are still used in AGC and RF mixer front-ends.
**** Metal-insulator-semiconductor field-effect transistor (MISFET)[edit] ****
Metal-insulator-semiconductor field-effect-transistor,[101][102][103] or
MISFET, is a more general term than MOSFET and a synonym to insulated-gate
field-effect transistor (IGFET). All MOSFETs are MISFETs, but not all MISFETs
are MOSFETs.
The gate dielectric insulator in a MISFET is silicon_dioxide in a MOSFET, but
other materials can also be employed. The gate_dielectric lies directly below
the gate_electrode and above the channel of the MISFET. The term metal is
historically used for the gate material, even though now it is usually highly
doped polysilicon or some other non-metal.
Insulator types may be:
    * Silicon dioxide, in MOSFETs
    * Organic insulators (e.g., undoped trans-polyacetylene; cyanoethyl
      pullulan, CEP[104]), for organic-based FETs.[103]
**** Multi-gate field-effect transistor (MuGET)[edit] ****
A FinFET
Main article: Multigate_device
Further information: FinFET
The dual-gate MOSFET has a tetrode configuration, where both gates control the
current in the device. It is commonly used for small-signal devices in radio
frequency applications where biasing the drain-side gate at constant potential
reduces the gain loss caused by Miller_effect, replacing two separate
transistors in cascode configuration. Other common uses in RF circuits include
gain control and mixing (frequency conversion). The tetrode description, though
accurate, does not replicate the vacuum-tube tetrode. Vacuum-tube tetrodes,
using a screen grid, exhibit much lower grid-plate capacitance and much higher
output impedance and voltage gains than triode vacuum tubes. These improvements
are commonly an order of magnitude (10 times) or considerably more. Tetrode
transistors (whether bipolar junction or field-effect) do not exhibit
improvements of such a great degree.
The FinFET is a double-gate silicon-on-insulator device, one of a number of
geometries being introduced to mitigate the effects of short channels and
reduce drain-induced barrier lowering. The fin refers to the narrow channel
between source and drain. A thin insulating oxide layer on either side of the
fin separates it from the gate. SOI FinFETs with a thick oxide on top of the
fin are called double-gate and those with a thin oxide on top as well as on the
sides are called triple-gate FinFETs.[105][106]
A double-gate MOSFET transistor was first demonstrated in 1984 by
Electrotechnical_Laboratory researchers Toshihiro Sekigawa and Yutaka Hayashi.
[107][108] A GAAFET (gate-all-around MOSFET), a type of multi-gate non-planar
3D_transistor, was first demonstrated in 1988, by a Toshiba research team
including Fujio_Masuoka, H. Takato and K. Sunouchi.[109][110] The FinFET (fin
field-effect transistor), a type of 3D non-planar double-gate MOSFET,
originated from the research of Digh Hisamoto and his team at Hitachi_Central
Research_Laboratory in 1989.[111][112]
**** NMOS logic[edit] ****
Main article: NMOS_logic
See also: Depletion-load_NMOS_logic
For devices of equal current driving capability, n-channel MOSFETs can be made
smaller than p-channel MOSFETs, due to p-channel charge carriers (holes) having
lower mobility than do n-channel charge carriers (electrons), and producing
only one type of MOSFET on a silicon substrate is cheaper and technically
simpler. These were the driving principles in the design of NMOS_logic which
uses n-channel MOSFETs exclusively. However, neglecting leakage_current, unlike
CMOS logic, NMOS logic consumes power even when no switching is taking place.
Mohamed_Atalla and Dawon_Kahng, after they invented the MOSFET, fabricated both
pMOS and nMOS devices with a 20 Âµm_process in 1960. However, the nMOS devices
were impractical, and only the pMOS type were practical working devices.[3] A
more practical NMOS process was developed several years later. NMOS was
initially faster than CMOS, thus NMOS was more widely used for computers in the
1970s.[85] With advances in technology, CMOS logic displaced NMOS logic in the
mid-1980s to become the preferred process for digital chips.
**** Power MOSFET[edit] ****
Two power_MOSFETs in D2PAK surface-mount packages. Operating as switches, each
of these components can sustain a blocking voltage of 120 V in the off state,
and can conduct a con­ti­nuous current of 30 A in the on state, dissipating up
to about 100 W and controlling a load of over 2000 W. A matchstick is pictured
for scale.
Cross section of a power_MOSFET, with square cells. A typical transistor is
constituted of several thousand cells
Main article: Power_MOSFET
Power_MOSFETs have a different structure.[113] As with most power devices, the
structure is vertical and not planar. Using a vertical structure, it is
possible for the transistor to sustain both high blocking voltage and high
current. The voltage rating of the transistor is a function of the doping and
thickness of the N-epitaxial layer (see cross section), while the current
rating is a function of the channel width (the wider the channel, the higher
the current). In a planar structure, the current and breakdown voltage ratings
are both a function of the channel dimensions (respectively width and length of
the channel), resulting in inefficient use of the "silicon estate". With the
vertical structure, the component area is roughly proportional to the current
it can sustain, and the component thickness (actually the N-epitaxial layer
thickness) is proportional to the breakdown voltage.[114]
Power MOSFETs with lateral structure are mainly used in high-end audio
amplifiers and high-power PA systems. Their advantage is a better behaviour in
the saturated region (corresponding to the linear region of a bipolar
transistor) than the vertical MOSFETs. Vertical MOSFETs are designed for
switching applications.[115]
The power MOSFET, which is commonly used in power_electronics, was developed in
the early 1970s.[116] The power MOSFET is the most common power_device in the
world, due to its low gate drive power, fast switching speed, and advanced
paralleling capability.[15] It has a wide range of power_electronic
applications, such as portable information_appliances, power_integrated
circuits, cell_phones, notebook_computers, and the communications
infrastructure that enables the internet.[117]
**** Double-diffused metalâoxideâsemiconductor (DMOS)[edit] ****
Main articles: LDMOS and VDMOS
There are LDMOS (lateral double-diffused metal oxide semiconductor) and VDMOS
(vertical double-diffused metal oxide semiconductor). Most power MOSFETs are
made using this technology.
**** Radiation-hardened-by-design (RHBD)[edit] ****
Semiconductor sub-micrometer and nanometer electronic circuits are the primary
concern for operating within the normal tolerance in harsh radiation
environments like outer_space. One of the design approaches for making a
radiation-hardened-by-design (RHBD) device is enclosed-layout-transistor (ELT).
Normally, the gate of the MOSFET surrounds the drain, which is placed in the
center of the ELT. The source of the MOSFET surrounds the gate. Another RHBD
MOSFET is called H-Gate. Both of these transistors have very low leakage
current with respect to radiation. However, they are large in size and take
more space on silicon than a standard MOSFET. In older STI (shallow trench
isolation) designs, radiation strikes near the silicon oxide region cause the
channel inversion at the corners of the standard MOSFET due to accumulation of
radiation induced trapped charges. If the charges are large enough, the
accumulated charges affect STI surface edges along the channel near the channel
interface (gate) of the standard MOSFET. Thus the device channel inversion
occurs along the channel edges and the device creates off-state leakage path,
causing device to turn on. So the reliability of circuits degrades severely.
The ELT offers many advantages. These advantages include improvement of
reliability by reducing unwanted surface inversion at the gate edges that
occurs in the standard MOSFET. Since the gate edges are enclosed in ELT, there
is no gate oxide edge (STI at gate interface), and thus the transistor off-
state leakage is reduced very much. Low-power microelectronic circuits
including computers, communication devices and monitoring systems in space
shuttle and satellites are very different from what is used on earth. They are
radiation (high-speed atomic particles like proton and neutron, solar_flare
magnetic energy dissipation in Earth's space, energetic cosmic_rays like X-ray,
gamma_ray etc.) tolerant circuits. These special electronics are designed by
applying different techniques using RHBD MOSFETs to ensure safe space journeys
and safe space-walks of astronauts.
***** See also[edit] *****
    * Floating-gate_MOSFET
    * BSIM
    * ggNMOS
    * High_electron_mobility_transistor
    * Polysilicon_depletion_effect
    * Power_MOSFET
    * Quantum_Hall_effect
    * Transistor_model
    * Intrinsic_diode
***** References[edit] *****
   1. ^ a b c d e f"Who_Invented_the_Transistor?". Computer_History_Museum. 4
      December 2013. Retrieved 20 July 2019.
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
   3. ^ a b c d"1960_-_Metal_Oxide_Semiconductor_(MOS)_Transistor
      Demonstrated". The Silicon Engine. Computer_History_Museum.
   4. ^ a b c d eLojek, Bo (2007). History of Semiconductor Engineering.
      Springer_Science_&_Business_Media. pp. 321â3. ISBN 9783540342588.
   5. ^Golio, Mike; Golio, Janet (2018). RF_and_Microwave_Passive_and_Active
      Technologies. CRC_Press. p. 18â2. ISBN 9781420006728.
   6. ^Bakshi, U. A.; Godse, A. P. (2007). "Â§8.2_The_depletion_mode_MOSFET".
      Electronic Circuits. Technical Publications. pp. 8â2. ISBN 978-81-8431-
      284-3.
   7. ^ a bMotoyoshi, M. (2009). "Through-Silicon_Via_(TSV)" (PDF). Proceedings
      of the IEEE. 97 (1): 43â48. doi:10.1109/JPROC.2008.2007462. ISSN 0018-
      9219.
   8. ^LÃ©cuyer, Christophe (2006). Making_Silicon_Valley:_Innovation_and_the
      Growth_of_High_Tech,_1930-1970. Chemical_Heritage_Foundation. p. 273.
      ISBN 9780262122818.
   9. ^ a b cSze,_Simon_Min. "Metal-oxide-semiconductor_field-effect
      transistors". Encyclopedia_Britannica. Retrieved 21 July 2019.
  10. ^ a b"Transistors_Keep_Moore's_Law_Alive". EETimes. 12 December 2018.
      Retrieved 18 July 2019.
  11. ^ a b c"Tortoise_of_Transistors_Wins_the_Race_-_CHM_Revolution". Computer
      History_Museum. Retrieved 22 July 2019.
  12. ^ a b c d"13_Sextillion_&_Counting:_The_Long_&_Winding_Road_to_the_Most
      Frequently_Manufactured_Human_Artifact_in_History". Computer_History
      Museum. April 2, 2018. Retrieved 28 July 2019.
  13. ^ a bBaker, R. Jacob (2011). CMOS:_Circuit_Design,_Layout,_and
      Simulation. John_Wiley_&_Sons. p. 7. ISBN 978-1118038239.
  14. ^ a b c d"Martin_Atalla_in_Inventors_Hall_of_Fame,_2009". Retrieved 21
      June 2013.
  15. ^ a b c d e"Dawon_Kahng". National_Inventors_Hall_of_Fame. Retrieved 27
      June 2019.
  16. ^ a b"Power_MOSFET_Basics" (PDF). Alpha & Omega Semiconductor. Retrieved
      29 July 2019.
  17. ^ a bChan, Yi-Jen (1992). Studies_of_InAIAs/InGaAs_and_GaInP/GaAs
      heterostructure_FET's_for_high_speed_applications. University_of
      Michigan. p. 1. The Si MOSFET has revolutionized the electronics industry
      and as a result impacts our daily lives in almost every conceivable way.
  18. ^ a bGrant, Duncan Andrew; Gowar, John (1989). Power_MOSFETS:_theory_and
      applications. Wiley. p. 1. ISBN 9780471828679. The metal-oxide-
      semiconductor field-effect transistor (MOSFET) is the most commonly used
      active device in the very large-scale integration of digital integrated
      circuits (VLSI). During the 1970s these components revolutionized
      electronic signal processing, control systems and computers.
  19. ^ a bZimbovskaya, Natalya A. (2013). Transport_Properties_of_Molecular
      Junctions. Springer. p. 231. ISBN 9781461480112.
  20. ^ a bWong, Kit Po (2009). Electrical_Engineering_-_Volume_II. EOLSS
      Publications. p. 7. ISBN 9781905839780.
  21. ^ a b c"Triumph_of_the_MOS_Transistor". YouTube. Computer_History_Museum.
      6 August 2010. Retrieved 21 July 2019.
  22. ^ a bRaymer, Michael G. (2009). The_Silicon_Web:_Physics_for_the_Internet
      Age. CRC_Press. p. 365. ISBN 9781439803127.
  23. ^ a b c"Remarks_by_Director_Iancu_at_the_2019_International_Intellectual
      Property_Conference". United_States_Patent_and_Trademark_Office. June 10,
      2019. Retrieved 20 July 2019.
  24. ^ Lilienfeld, Julius Edgar (1926-10-08) "Method and apparatus for
      controlling electric currents" U.S._Patent_1,745,175A
  25. ^Lee, Thomas H. (2003). The_Design_of_CMOS_Radio-Frequency_Integrated
      Circuits (PDF). Cambridge_University_Press. ISBN 9781139643771.
  26. ^ a b cPuers, Robert; Baldi, Livio; Voorde, Marcel Van de; Nooten,
      Sebastiaan E. van (2017). Nanoelectronics:_Materials,_Devices,
      Applications,_2_Volumes. John_Wiley_&_Sons. p. 14. ISBN 9783527340538.
  27. ^ a bDeal, Bruce E. (1998). "Highlights_Of_Silicon_Thermal_Oxidation
      Technology". Silicon materials science and technology. The
      Electrochemical_Society. p. 183. ISBN 9781566771931.
  28. ^Lojek, Bo (2007). History of Semiconductor Engineering. Springer_Science
      &_Business_Media. p. 120. ISBN 9783540342588.
  29. ^ U.S._Patent_2,953,486
  30. ^Atalla,_M.; Kahng,_D. (1960). "Silicon-silicon dioxide field induced
      surface devices". IRE-AIEE Solid State Device Research Conference.
  31. ^ U.S._Patent_3,206,670 (1960)
  32. ^ U.S._Patent_3,102,230 (1960)
  33. ^ "The_Silicon_Engine_|_1948 â_Conception_of_the_Junction_Transistor".
      Computer History Museum. 2007.
  34. ^ a b cHittinger, William C. (1973). "METAL-OXIDE-SEMICONDUCTOR
      TECHNOLOGY". Scientific American. 229 (2): 48â59. Bibcode:
      1973SciAm.229b..48H. doi:10.1038/scientificamerican0873-48. ISSN 0036-
      8733. JSTOR 24923169.
  35. ^ a b"1963:_Complementary_MOS_Circuit_Configuration_is_Invented".
      Computer_History_Museum. Retrieved 6 July 2019.
  36. ^ a bKimizuka, Noboru; Yamazaki, Shunpei (2016). Physics_and_Technology
      of_Crystalline_Oxide_Semiconductor_CAAC-IGZO:_Fundamentals. John Wiley &
      Sons. p. 217. ISBN 9781119247401.
  37. ^Weimer,_Paul_K. (1962). "The TFT A New Thin-Film Transistor".
      Proceedings_of_the_IRE. 50 (6): 1462â1469. doi:10.1109/
      JRPROC.1962.288190. ISSN 0096-8390.
  38. ^Kuo, Yue (1 January 2013). "Thin_Film_Transistor_TechnologyâPast,
      Present,_and_Future" (PDF). The Electrochemical Society Interface. 22
      (1): 55â61. doi:10.1149/2.F06131if. ISSN 1064-8208.
  39. ^Solid_State_Design_-_Vol._6. Horizon House. 1965.
  40. ^"Robert_Dennard". Encyclopedia_Britannica. Retrieved 8 July 2019.
  41. ^ D. Kahng and S. M. Sze, "A floating-gate and its application to memory
      devices", The Bell System Technical Journal, vol. 46, no. 4, 1967, pp.
      1288â1295
  42. ^"1971:_Reusable_semiconductor_ROM_introduced". Computer_History_Museum.
      Retrieved 19 June 2019.
  43. ^Bez, R.; Pirovano, A. (2019). Advances_in_Non-Volatile_Memory_and
      Storage_Technology. Woodhead_Publishing. ISBN 9780081025857.
  44. ^ a b cLindley, David (15 May 2015). "Focus:_LandmarksâAccidental
      Discovery_Leads_to_Calibration_Standard". Physics. 8.
  45. ^Jun-ichi Wakabayashi; Shinji Kawaji (1978). "Hall effect in silicon MOS
      inversion layers under strong magnetic fields". J. Phys. Soc. Jpn. 44
      (6): 1839. Bibcode:1978JPSJ...44.1839W. doi:10.1143/JPSJ.44.1839.
  46. ^K. v. Klitzing; G. Dorda; M. Pepper (1980). "New method for high-
      accuracy determination of the fine-structure constant based on quantized
      Hall resistance". Phys. Rev. Lett. 45 (6): 494â497. Bibcode:
      1980PhRvL..45..494K. doi:10.1103/PhysRevLett.45.494.
  47. ^"Intel_45nm_Hi-k_Silicon_Technology". Archived from the_original on
      October 6, 2009.
  48. ^"memory_components_data_book" (PDF). memory components data book. Intel.
      pp. 2â1. Archived from the_original (PDF) on 4 March 2016. Retrieved 30
      August 2015.
  49. ^"Using_a_MOSFET_as_a_Switch".
  50.  090507 brunningsoftware.co.uk
  51. ^Shichman, H. & Hodges, D. A. (1968). "Modeling and simulation of
      insulated-gate field-effect transistor switching circuits". IEEE Journal
      of Solid-State Circuits. SC-3 (3): 285â289. Bibcode:
      1968IJSSC...3..285S. doi:10.1109/JSSC.1968.1049902.
  52. ^ For example, seeCheng, Yuhua; Hu, Chenming (1999). MOSFET_modeling_&
      BSIM3_user's_guide. Springer. ISBN 978-0-7923-8575-2.
  53. . The most recent version of the BSIM model is described inV.,
      Sriramkumar; Paydavosi, Navid; Lu, Darsen; Lin, Chung-Hsun; Dunga, Mohan;
      Yao, Shijing; Morshed, Tanvir; Niknejad, Ali & Hu, Chenming (2012).
      "BSIM-CMG_106.1.0beta_Multi-Gate_MOSFET_Compact_Model" (PDF). Department
      of EE and CS, UC Berkeley. Archived from the_original (PDF) on 2014-07-
      27. Retrieved 2012-04-01.
  54. ^ Gray, P. R.; Hurst, P. J.; Lewis, S. H. & Meyer, R. G. (2001). Analysis
      and_Design_of_Analog_Integrated_Circuits (Fourth ed.). New York: Wiley.
      pp. 66â67. ISBN 978-0-471-32168-2.
  55. ^ van der Meer, P. R.; van Staveren, A.; van Roermund, A. H. M. (2004).
      Low-Power_Deep_Sub-Micron_CMOS_Logic:_Subthreshold_Current_Reduction.
      Dordrecht: Springer. p. 78. ISBN 978-1-4020-2848-9.
  56. ^Degnan, Brian. "Wikipedia_fails_subvt".
  57. ^Mead, Carver (1989). Analog VLSI and Neural Systems. Reading, MA:
      Addison-Wesley. p. 370. ISBN 9780201059922.
  58. ^Smith, Leslie S.; Hamilton, Alister (1998). Neuromorphic_Systems:
      Engineering_Silicon_from_Neurobiology. World Scientific. pp. 52â56.
      ISBN 978-981-02-3377-8.
  59. ^Kumar, Satish (2004). Neural_Networks:_A_Classroom_Approach. Tata
      McGraw-Hill. p. 688. ISBN 978-0-07-048292-0.
  60. ^Glesner, Manfred; Zipf, Peter; Renovell, Michel (2002). Field-
      programmable_Logic_and_Applications:_12th_International_Conference.
      Dordrecht: Springer. p. 425. ISBN 978-3-540-44108-3.
  61. ^Vittoz, Eric A. (1996). "The_Fundamentals_of_Analog_Micropower_Design".
      In Toumazou, Chris; Battersby, Nicholas C.; Porta, Sonia (eds.). Circuits
      and systems tutorials. John Wiley and Sons. pp. 365â372. ISBN 978-0-
      7803-1170-1.
  62. ^Shukla, Sandeep K.; Bahar, R. Iris (2004). Nano,_Quantum_and_Molecular
      Computing. Springer. p. 10 and Fig. 1.4, p. 11. ISBN 978-1-4020-8067-8.
  63. ^Srivastava, Ashish; Sylvester, Dennis; Blaauw, David (2005). Statistical
      Analysis_and_Optimization_For_VLSI:_Timing_and_Power. Springer. p. 135.
      ISBN 978-0-387-25738-9.
  64. ^Galup-Montoro, C. & M.C., Schneider (2007). MOSFET_modeling_for_circuit
      analysis_and_design. London/Singapore: World Scientific. p. 83. ISBN 978-
      981-256-810-6.
  65. ^Malik, Norbert R. (1995). Electronic_circuits:_analysis,_simulation,_and
      design. Englewood Cliffs, NJ: Prentice Hall. pp. 315â316. ISBN 978-0-
      02-374910-0.
  66. ^Gray, P. R.; Hurst, P. J.; Lewis, S. H.; Meyer, R. G. (2001). Â§1.5.2_p.
      45. ISBN 978-0-471-32168-2.
  67. ^Sedra, A. S. & Smith, K. C. (2004). Microelectronic_circuits (Fifth
      ed.). New York: Oxford. p. 552. ISBN 978-0-19-514251-8.
  68. ^Sedra, A. S. & Smith, K.C. (2004). p._250,_Eq._4.14. ISBN 978-0-19-
      514251-8.
  69. ^  For a uniformly doped p-type substrate with bulk acceptor doping of NA
      per unit volume,
                &#x03C6;  B   =     k  B   T  q   ln &#x2061;  (    N  A    n
            i     )  &#xA0; ,   {\displaystyle \varphi _{B}={\frac {k_{B}T}
            {q}}\ln \left({\frac {N_{A}}{n_{i}}}\right)\ ,}  [{\displaystyle
            \varphi _{B}={\frac {k_{B}T}{q}}\ln \left({\frac {N_{A}}{n_
            {i}}}\right)\ ,}]
      with ni the intrinsic mobile carrier density per unit volume in the bulk.
      See, for example,Arora, Narain (2007). "Equation_5.12". Mosfet modeling
      for VLSI simulation: theory and practice. World Scientific. p. 173.
      ISBN 978-981-256-862-5.
  70. ^"Body_effect". Equars.com. Archived from the_original on 2014-11-10.
      Retrieved 2012-06-02.
  71. ^"Electronic_Circuit_Symbols". circuitstoday.com. 9 November 2011.
      Archived from the_original on 13 October 2014.
  72. ^IEEE Std 315-1975 â Graphic Symbols for Electrical and Electronics
      Diagrams (Including Reference Designation Letters)
  73. ^Jaeger, Richard C.; Blalock, Travis N. "Figure_4.15_IEEE_Standard_MOS
      transistor_circuit_symbols" (PDF). Microelectronic Circuit Design.
  74. ^"Rethink_Power_Density_with_GaN". Electronic_Design. 21 April 2017.
      Retrieved 23 July 2019.
  75. ^ a b cColinge, Jean-Pierre; Greer, James C. (2016). Nanowire
      Transistors:_Physics_of_Devices_and_Materials_in_One_Dimension. Cambridge
      University_Press. p. 2. ISBN 9781107052406.
  76. ^Memories:_A_Personal_History_of_Bell_Telephone_Laboratories (PDF).
      Institute_of_Electrical_and_Electronics_Engineers. 2011. p. 59.
      ISBN 1463677979.
  77. ^"MOSFET:_Toward_the_Scaling_Limit". Semiconductor Technology Online.
      Retrieved 29 July 2019.
  78. ^"Milestones:List_of_IEEE_Milestones". Institute_of_Electrical_and
      Electronics_Engineers. Retrieved 25 July 2019.
  79. ^"Computer_History_Museum â_The_Silicon_Engine_|_1955 â
      Photolithography_Techniques_Are_Used_to_Make_Silicon_Devices".
      Computerhistory.org. Retrieved 2012-06-02.
  80. ^Kuo, Yue (1 January 2013). "Thin_Film_Transistor_TechnologyâPast,
      Present,_and_Future" (PDF). The Electrochemical Society Interface. 22
      (1): 55â61. doi:10.1149/2.F06131if. ISSN 1064-8208.
  81. ^"1964_â_First_Commercial_MOS_IC_Introduced". Computer_History_Museum.
  82. ^"1968:_Silicon_Gate_Technology_Developed_for_ICs". Computer_History
      Museum. Retrieved 22 July 2019.
  83. ^"1971:_Microprocessor_Integrates_CPU_Function_onto_a_Single_Chip_|_The
      Silicon_Engine". Computer_History_Museum. Retrieved 22 July 2019.
  84. ^Cushman, Robert H. (20 September 1975). "2-1/2-generation_Î¼P's-$10
      parts_that_perform_like_low-end_mini's" (PDF). EDN.
  85. ^ a bNigel Tout. "Sharp_QT-8D_"micro_Compet"". Vintage Calculators Web
      Museum. Retrieved September 29, 2010.
  86. ^ a b c"Hand-held_Calculators". Vintage Calculators Web Museum. Retrieved
      22 July 2019.
  87. ^"Computer_History_Museum â_The_Silicon_Engine_|_1963 â_Complementary
      MOS_Circuit_Configuration_is_Invented". Computerhistory.org. Retrieved
      2012-06-02.
  88. ^ a b"1978:_Double-well_fast_CMOS_SRAM_(Hitachi)" (PDF). Semiconductor
      History Museum of Japan. Retrieved 5 July 2019.
  89. ^"Computer_History_Museum â_Exhibits â_Microprocessors".
      Computerhistory.org. Retrieved 2012-06-02.
  90. ^"ReVera's_FinFET_Control". revera.com. Archived from the_original on 19
      September 2010.
  91. ^Colinge, Jean-Pierre; Colinge, Cynthia A. (2002). Physics_of
      Semiconductor_Devices. Dordrecht: Springer. p. 233, Figure 7.46.
      ISBN 978-1-4020-7018-1.
  92. ^Weber, Eicke R.; Dabrowski, Jarek, eds. (2004). Predictive_Simulation_of
      Semiconductor_Processing:_Status_and_Challenges. Dordrecht: Springer.
      p. 5, Figure 1.2. ISBN 978-3-540-20481-7.
  93. ^"International_Technology_Roadmap_for_Semiconductors". Archived from the
      original on 2015-12-28.
  94. ^"1965 â_"Moore's_Law"_Predicts_the_Future_of_Integrated_Circuits".
      Computer History Museum.
  95. ^Roy, Kaushik; Yeo, Kiat Seng (2004). Low_Voltage,_Low_Power_VLSI
      Subsystems. McGraw-Hill Professional. Fig. 2.1, p. 44, Fig. 1.1, p. 4.
      ISBN 978-0-07-143786-8.
  96. ^Vasileska, Dragica; Goodnick, Stephen (2006). Computational_Electronics.
      Morgan & Claypool. p. 103. ISBN 978-1-59829-056-1.
  97. ^"Frontier_Semiconductor_Paper" (PDF). Archived from the_original (PDF)
      on February 27, 2012. Retrieved 2012-06-02.
  98. ^Chen, Wai-Kai (2006). The_VLSI_Handbook. CRC Press. Fig. 2.28, p.
      2â22. ISBN 978-0-8493-4199-1.
  99. ^Lindsay, R.; Pawlak; Kittl; Henson; Torregiani; Giangrandi; Surdeanu;
      Vandervorst; Mayur; Ross; McCoy; Gelpey; Elliott; Pages; Satta; Lauwers;
      Stolk; Maex (2011). "A Comparison of Spike, Flash, SPER and Laser
      Annealing for 45nm CMOS". MRS Proceedings. 765. doi:10.1557/PROC-765-
      D7.4.
 100. ^"VLSI_wiring_capacitance" (PDF). IBM Journal of Research and
      Development.
 101. [dead_link]
 102. ^Soudris, D.; Pirsch, P.; Barke, E., eds. (2000). Integrated_Circuit
      Design:_Power_and_Timing_Modeling,_Optimization,_and_Simulation_(10th
      Int._Workshop). Springer. p. 38. ISBN 978-3-540-41068-3.
 103. ^Orshansky, Michael; Nassif, Sani; Boning, Duane (2007). Design_for
      Manufacturability_And_Statistical_Design:_A_Constructive_Approach. New
      York 309284: Springer. ISBN 9780387309286.
 104. ^ "Depletion_Mode". Techweb. Techweb. 29 January 2010. Retrieved 27
      November 2010.
 105. ^ "MIS". Semiconductor Glossary.
 106. ^ Hadziioannou, Georges; Malliaras, George G. (2007). Semiconducting
      polymers:_chemistry,_physics_and_engineering. Wiley-VCH. ISBN 978-3-527-
      31271-9.
 107. ^ a b Jones, William (1997). Organic_Molecular_Solids:_Properties_and
      Applications. CRC Press. ISBN 978-0-8493-9428-7.
 108. ^ Xu, Wentao; Guo, Chang; Rhee, Shi-Woo (2013). "High_performance_organic
      field-effect_transistors_using_cyanoethyl_pullulan_(CEP)_high-k_polymer
      cross-linked_with_trimethylolpropane_triglycidyl_ether_(TTE)_at_low
      temperatures". Journal of Materials Chemistry C. 1 (25): 3955. doi:
      10.1039/C3TC30134F.
 109. ^Zeitzoff, P. M.; Hutchby, J. A.; Huff, H. R. (2002). "Figure_12:
      Simplified_cross_section_of_FinFET_double-gate_MOSFET.". In Park, Yoon-
      Soo; Shur, Michael; Tang, William (eds.). Frontiers in electronics:
      future chips : proceedings of the 2002 Workshop on Frontiers in
      Electronics (WOFE-02), St Croix, Virgin Islands, USA, 6â11 January
      2002. World Scientific. p. 82. ISBN 978-981-238-222-1.
 110. ^Lee, J.-H.; Lee, J.-W.; Jung, H.-A.-R.; Choi, B.-K. (2009). "Comparison
      of_SOI_FinFETs_and_bulk_FinFETs:_Figure_2". Silicon-on-Insulator
      Technology and Devices. The Electrochemical Society. p. 102. ISBN 978-1-
      56677-712-4.
 111. ^Colinge, J.P. (2008). FinFETs_and_Other_Multi-Gate_Transistors. Springer
      Science & Business Media. p. 11. ISBN 9780387717517.
 112. ^Sekigawa, Toshihiro; Hayashi, Yutaka (1 August 1984). "Calculated
      threshold-voltage characteristics of an XMOS transistor having an
      additional bottom gate". Solid-State Electronics. 27 (8): 827â828.
      Bibcode:1984SSEle..27..827S. doi:10.1016/0038-1101(84)90036-4. ISSN 0038-
      1101.
 113. ^Masuoka,_Fujio; Takato, H.; Sunouchi, K.; Okabe, N.; Nitayama, A.;
      Hieda, K.; Horiguchi, F. (December 1988). "High performance CMOS
      surrounding-gate transistor (SGT) for ultra high density LSIs". Technical
      Digest., International Electron Devices Meeting: 222â225. doi:10.1109/
      IEDM.1988.32796.
 114. ^Brozek, Tomasz (2017). Micro-_and_Nanoelectronics:_Emerging_Device
      Challenges_and_Solutions. CRC_Press. p. 117. ISBN 9781351831345.
 115. ^"IEEE_Andrew_S._Grove_Award_Recipients". IEEE_Andrew_S._Grove_Award.
      Institute_of_Electrical_and_Electronics_Engineers. Retrieved 4 July 2019.
 116. ^"The_Breakthrough_Advantage_for_FPGAs_with_Tri-Gate_Technology" (PDF).
      Intel. 2014. Retrieved 4 July 2019.
 117. ^Baliga, B. Jayant (1996). Power Semiconductor Devices. Boston: PWS
      publishing Company. ISBN 978-0-534-94098-0.
 118. ^"Power_MOSFET_Basics:_Understanding_MOSFET_Characteristics_Associated
      With_The_Figure_of_Merit". element14. Archived from the_original on 5
      April 2015. Retrieved 27 November 2010.
 119. ^"Power_MOSFET_Basics:_Understanding_Gate_Charge_and_Using_It_To_Assess
      Switching_Performance". element14. Archived from the_original on 30 June
      2014. Retrieved 27 November 2010.
 120. ^Irwin, J. David (1997). The_Industrial_Electronics_Handbook. CRC_Press.
      p. 218. ISBN 9780849383434.
 121. ^Whiteley, Carol; McLaughlin, John Robert (2002). Technology,
      Entrepreneurs,_and_Silicon_Valley. Institute for the History of
      Technology. ISBN 9780964921719. These active electronic components, or
      power semiconductor products, from Siliconix are used to switch and
      convert power in a wide range of systems, from portable information
      appliances to the communications infrastructure that enables the
      Internet. The company's power MOSFETs â tiny solid-state switches, or
      metal oxide semiconductor field-effect transistors â and power
      integrated circuits are widely used in cell phones and notebook computers
      to manage battery power efficiently
***** External links[edit] *****
 This article's use of external_links may not follow Wikipedia's policies or
 guidelines. Please improve_this_article by removing excessive or inappropriate
 external links, and converting useful links where appropriate into footnote
 references. (September 2016)(Learn_how_and_when_to_remove_this_template
 message)
 Wikimedia Commons has media related to MOSFET.
    * How_Semiconductors_and_Transistors_Work_(MOSFETs) WeCanFigureThisOut.org
    * "Understanding_power_MOSFET_data_sheet_parameters_â_Nexperia_PDF
      Application_Note_AN11158" (PDF).
"An_introduction_to_depletion-mode_MOSFETs". Archived from the_original on 28
September 2008.
"Power_MOSFETs".
"Criteria_for_Successful_Selection_of_IGBT_and_MOSFET_Modules". Archived from
the_original on 2012-11-12. Retrieved 2018-12-16.
"MOSFET_Process_Step_by_Step". Archived from the_original on 2009-08-22.
Retrieved 2016-02-06.
 A Flash slide showing the fabricating process of a MOSFET in detail
"MOSFET_Calculator". Archived from the_original on 2008-05-27. Retrieved 2008-
06-03.
"Advanced_MOSFET_issues". ecee.colorado.edu. 27 November 2010.
"MOSFET_applet".
Nicolai, Ulrich; Reimann, Tobias; Petzoldt, JÃ¼rgen; Lutz, Josef (1998).
Application_Manual_IGBT_and_MOSFET_Power_Modules (1st ed.). ISLE Verlag.
ISBN 978-3-932633-24-9. Archived from the_original on 2 March 2012.
Wintrich, Arendt; Nicolai, Ulrich; Tursky, Werner; Reimann, Tobias (2011). PDF-
Version (PDF) (2nd ed.). Nuremberg: Semikron. ISBN 978-3-938843-66-6. Archived
from the_original (PDF) on 3 September 2013.
"MIT_Open_Courseware_6.002 â_Spring_2007".
"MIT_Open_Courseware_6.012 â_Fall_2009".
"Georgia_Tech_BJT_and_FET_Slides".
"CircuitDesign:_MOS_Diffusion_Parasitics".
Mark Lundstrom, Mark Lundstrom (2008). "Course_on_Physics_of_Nanoscale
Transistors".
Dr. Lundstrom (2005). "Notes_on_Ballistic_MOSFETs".
    * v
    * t
    * e
Electronic_components
                                         * Complementary_MOS (CMOS)
                                         * Depletion-load_NMOS
                                         * Fin_field-effect_transistor (FinFET)
                                         * Floating-gate_MOSFET (FGMOS)
                                         * Insulated-gate_bipolar_transistor
                                           (IGBT)
                                         * LDMOS
                   MOS transistors       * MOS field-effect transistor (MOSFET)
                                         * Multi-gate_field-effect_transistor
                                           (MuGET)
                                         * NMOS
                                         * PMOS
                                         * Power_MOSFET
                                         * Thin-film_transistor (TFT)
                                         * VMOS
                                         * Bipolar_junction_transistor (BJT)
                                         * Darlington_transistor
                                         * Diffusion_transistor
                                         * Field-effect_transistor (FET)
                                         * JFET
                                         * Light-emitting_transistor (LET)
                                         * Organic_field-effect_transistor
                                           (OFET)
                   Other_transistors     * Organic_light-emitting_transistor
                                           (OLET)
                                         * Pentode_transistor
                                         * Point-contact_transistor
                                         * Programmable_unijunction_transistor
Semiconductor                              (PUT)
devices                                  * Static_induction_transistor (SIT)
                                         * Tetrode_transistor
                                         * Unijunction_transistor (UJT)
                                         * Avalanche_diode
                                         * Constant-current_diode (CLD, CRD)
                                         * Laser_diode (LD)
                                         * Light-emitting_diode (LED)
                   Diodes                * Photodiode
                                         * PIN_diode
                                         * Schottky_diode
                                         * Step_recovery_diode
                                         * Zener_diode
                                         * DIAC
                                         * Heterostructure_barrier_varactor
                                         * Integrated_circuit (IC)
                                         * Memistor
                                         * Memory_cell
                                         * Memristor
                                         * Organic_semiconductor
                                         * Photodetector
                   Other devices         * Solaristor
                                         * Quantum_circuit
                                         * Silicon_controlled_rectifier (SCR)
                                         * Static_induction_thyristor (SITh)
                                         * Three-dimensional_integrated_circuit
                                           (3D IC)
                                         * Thyristor
                                         * TRIAC
                                         * Varicap
                       * Linear_regulator
                       * Low-dropout_regulator
                       * Switching_regulator
                       * Buck
                       * Boost
Voltage_regulators     * Buckâboost
                       * Split-pi
                       * Äuk
                       * SEPIC
                       * Charge_pump
                       * Switched_capacitor
                       * Acorn_tube
                       * Audion
                       * Beam_tetrode
                       * Barretter
                       * Compactron
                       * Diode
                       * Fleming_valve
Vacuum_tubes           * Nonode
                       * Nuvistor
                       * Pentagrid (Hexode, Heptode, Octode)
                       * Pentode
                       * Photomultiplier
                       * Phototube
                       * Tetrode
                       * Triode
                       * Backward-wave_oscillator (BWO)
                       * Cavity_magnetron
                       * Crossed-field_amplifier (CFA)
                       * Gyrotron
Vacuum_tubes (RF)      * Inductive_output_tube (IOT)
                       * Klystron
                       * Maser
                       * Sutton_tube
                       * Traveling-wave_tube (TWT)
                       * Beam_deflection_tube
                       * Charactron
                       * Iconoscope
                       * Magic_eye_tube
Cathode_ray_tubes      * Monoscope
                       * Selectron_tube
                       * Storage_tube
                       * Trochotron
                       * Video_camera_tube
                       * Williams_tube
                       * Cold_cathode
                       * Crossatron
                       * Dekatron
                       * Ignitron
                       * Krytron
Gas-filled_tubes       * Mercury-arc_valve
                       * Neon_lamp
                       * Nixie_tube
                       * Thyratron
                       * Trigatron
                       * Voltage-regulator_tube
                       * Potentiometer
Adjustable                   o digital
                       * Variable_capacitor
                       * Varicap
                       * Connector
                             o audio_and_video
                             o electrical_power
                             o RF
                       * Electrolytic_detector
                       * Ferrite
                       * Fuse
Passive                      o resettable
                       * Resistor
                       * Switch
                       * Thermistor
                       * Transformer
                       * Varistor
                       * Wire
                             o Wollaston_wire
                       * Capacitor
                             o types
                       * Ceramic_resonator
                       * Crystal_oscillator
Reactive               * Inductor
                       * Parametron
                       * Relay
                             o reed_relay
                             o mercury_switch
                                              * BNF: cb12423223g (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4207266-9
                                              * LCCN: sh85084065
                                              * NDL: 01142304

Retrieved from "https://en.wikipedia.org/w/
index.php?title=MOSFET&oldid=909456467"
Categories:
    * Transistor_types
    * MOSFETs
Hidden categories:
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_June_2015
    * Articles_with_short_description
    * All_articles_with_vague_or_ambiguous_time
    * Vague_or_ambiguous_time_from_April_2019
    * Articles_needing_additional_references_from_January_2019
    * All_articles_needing_additional_references
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_December_2015
    * All_Wikipedia_articles_needing_clarification
    * Wikipedia_articles_needing_clarification_from_January_2016
    * Articles_with_unsourced_statements_from_January_2016
    * All_accuracy_disputes
    * Articles_with_disputed_statements_from_January_2016
    * Articles_needing_additional_references_from_September_2016
    * Wikipedia_articles_with_style_issues_from_September_2016
    * All_articles_with_style_issues
    * Wikipedia_external_links_cleanup_from_September_2016
    * Wikipedia_spam_cleanup_from_September_2016
    * Commons_category_link_is_on_Wikidata
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
    * Wikipedia_articles_with_NDL_identifiers
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
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * LietuviÅ³
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÄina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 5 August 2019, at 15:15 (UTC).
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
