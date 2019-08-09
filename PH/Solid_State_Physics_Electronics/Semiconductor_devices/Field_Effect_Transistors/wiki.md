The following text has been accessed from https://en.wikipedia.org/wiki/Field-effect_transistor at Fri Aug 9 03:08:53 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Field-effect transistor ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"FET" redirects here. For other uses, see FET_(disambiguation).
Cross-sectional view of a field-effect transistor, showing source, gate and
drain terminals
The field-effect transistor (FET) is an electronic device which uses an
electric_field to control the flow of current. FETs are devices with three
terminals: source, gate, and drain. FETs control the flow of current by the
application of a voltage to the gate, which in turn alters the conductivity
between the drain and source.
FETs are also known as unipolar transistors since they involve single-carrier-
type operation. That is, FETs use electrons or holes as charge_carriers in
their operation, but not both. Many different types of field effect transistors
exist. Field effect transistors generally display very high_input_impedance at
low frequencies. The most widely used field-effect transistor is the MOSFET
(metal-oxide-semiconductor field-effect transistor).
⁰
***** Contents *****
    * 1_History
    * 2_Basic_information
    * 3_More_about_terminals
          o 3.1_Effect_of_gate_voltage_on_current
                # 3.1.1_n-channel_FET
                # 3.1.2_p-channel_FET
          o 3.2_Effect_of_drain-to-source_voltage_on_channel
    * 4_Composition
    * 5_Types
    * 6_Advantages
    * 7_Disadvantages
    * 8_Failure_modes
    * 9_Uses
    * 10_Source-gated_transistor
    * 11_See_also
    * 12_References
    * 13_External_links
***** History[edit] *****
Main articles: MOSFET_Â§ History, and History_of_the_transistor
Julius_Edgar_Lilienfeld proposed the concept of a field-effect transistor in
1925.
The concept of a field-effect transistor (FET) was first patented by Julius
Edgar_Lilienfeld in 1925 and by Oskar_Heil in 1934, but they were unable to
build a working practical semiconducting_device based on the concept. The
transistor effect was later observed and explained by the team of William
Shockley at Bell_Labs in 1947, shortly after the 17-year patent expired.
Shockley initially attempted to build a working FET, by trying to modulate the
conductivity of a semiconductor, but was unsuccessful, mainly due to problems
with the surface_states, the dangling_bond, and the germanium and copper
compound materials. In the course of trying to understand the mysterious
reasons behind their failure to build a working FET, this led them to instead
inventing the bipolar point-contact and junction_transistors.[1][2]
The first FET device to be successfully built was the junction_field-effect
transistor (JFET).[1] A JFET was first patented by Heinrich_Welker in 1945.[3]
The static_induction_transistor (SIT), a type of JFET with a short channel, was
invented by Japanese engineers Jun-ichi_Nishizawa and Y. Watanabe in 1950.
Following Shockley's theoretical treatment on JFET in 1952, a working practical
JFET was built by George F. Dacey and Ian_M._Ross in 1953.[4] However, while
the JFET was a useful device, it was not the type of FET that Shockley had
originally sought to build.[1]
Mohamed_Atalla (left) and Dawon_Kahng (right) invented the MOSFET (MOS field-
effect transistor) in 1959.
A breakthrough in FET research came with the work of Mohamed_Atalla in the late
1950s.[2] He investigated the surface properties of silicon semiconductors at
Bell_Labs, where he adopted a new method of semiconductor_device_fabrication,
coating a silicon_wafer with an insulating layer of silicon_oxide, so that
electricity could reliably penetrate to the conducting silicon below,
overcoming the surface states that prevented electricity from reaching the
semiconducting layer. This is known as surface_passivation, a method that
became critical to the semiconductor_industry as it made possible the mass-
production of silicon integrated_circuits.[5][6] Building on his surface
passivation method, he developed the metalâoxideâsemiconductor (MOS)
process,[5] which he presented in 1957.[7] He later proposed the MOS process
could be used to build the first working silicon FET, which he began working on
building with the help of Dawon_Kahng.[5]
The metalâoxideâsemiconductor_field-effect_transistor (MOSFET) was invented
by Mohamed Atalla and Dawon Kahng in 1959.[8][9] The MOSFET largely superseded
both the bipolar transistor and the JFET,[1] and had a profound effect on
digital_electronic development.[10][9] With its high_scalability,[11] and much
lower power consumption and higher density than bipolar junction transistors,
[12] the MOSFET made it possible to build high-density integrated circuits.[13]
The MOSFET is also capable of handling higher power than the JFET.[14] The
MOSFET thus became the most common type of transistor in computers,
electronics,[6] and communications_technology (such as smartphones).[15] The US
Patent_and_Trademark_Office calls the MOSFET a "groundbreaking invention that
transformed life and culture around the world".[15]
CMOS (complementary MOS) was invented by Chih-Tang_Sah and Frank_Wanlass at
Fairchild_Semiconductor in 1963.[16][17] The first report of a floating-gate
MOSFET was made by Dawon Kahng and Simon_Sze in 1967.[18] A double-gate MOSFET
was first demonstrated in 1984 by Electrotechnical_Laboratory researchers
Toshihiro Sekigawa and Yutaka Hayashi.[19][20] FinFET (fin field-effect
transistor), a type of 3D non-planar multi-gate MOSFET, originated from the
research of Digh Hisamoto and his team at Hitachi_Central_Research_Laboratory
in 1989.[21][22]
***** Basic information[edit] *****
See also: Charge_carrier_Â§ Majority_and_minority_carriers
FETs can be majority-charge-carrier devices, in which the current is carried
predominantly by majority carriers, or minority-charge-carrier devices, in
which the current is mainly due to a flow of minority carriers.[23] The device
consists of an active channel through which charge carriers, electrons or
holes, flow from the source to the drain. Source and drain terminal conductors
are connected to the semiconductor through ohmic_contacts. The conductivity of
the channel is a function of the potential applied across the gate and source
terminals.
The FET's three terminals are:[24]
   1. source (S), through which the carriers enter the channel. Conventionally,
      current entering the channel at S is designated by IS.
   2. drain (D), through which the carriers leave the channel. Conventionally,
      current entering the channel at D is designated by ID. Drain-to-source
      voltage is VDS.
   3. gate (G), the terminal that modulates the channel conductivity. By
      applying voltage to G, one can control ID.
***** More about terminals[edit] *****
Cross section of an n-type MOSFET
All FETs have source, drain, and gate terminals that correspond roughly to the
emitter, collector, and base of BJTs. Most FETs have a fourth terminal called
the body, base, bulk, or substrate. This fourth terminal serves to bias the
transistor into operation; it is rare to make non-trivial use of the body
terminal in circuit designs, but its presence is important when setting up the
physical_layout of an integrated_circuit. The size of the gate, length L in the
diagram, is the distance between source and drain. The width is the extension
of the transistor, in the direction perpendicular to the cross section in the
diagram (i.e., into/out of the screen). Typically the width is much larger than
the length of the gate. A gate length of 1 Âµm limits the upper frequency to
about 5 GHz, 0.2 Âµm to about 30 GHz.
The names of the terminals refer to their functions. The gate terminal may be
thought of as controlling the opening and closing of a physical gate. This gate
permits electrons to flow through or blocks their passage by creating or
eliminating a channel between the source and drain. Electron-flow from the
source terminal towards the drain terminal is influenced by an applied voltage.
The body simply refers to the bulk of the semiconductor in which the gate,
source and drain lie. Usually the body terminal is connected to the highest or
lowest voltage within the circuit, depending on the type of the FET. The body
terminal and the source terminal are sometimes connected together since the
source is often connected to the highest or lowest voltage within the circuit,
although there are several uses of FETs which do not have such a configuration,
such as transmission_gates and cascode circuits.
**** Effect of gate voltage on current[edit] ****
IâV characteristics and output plot of a JFET n-channel transistor.
Simulation result for right side: formation of inversion_channel (electron
density) and left side: current-gate voltage curve(transfer characteristics) in
an n-channel nanowire MOSFET. Note that the threshold_voltage for this device
lies around 0.45 V.
FET conventional symbol types
The FET controls the flow of electrons (or electron_holes) from the source to
drain by affecting the size and shape of a "conductive channel" created and
influenced by voltage (or lack of voltage) applied across the gate and source
terminals. (For simplicity, this discussion assumes that the body and source
are connected.) This conductive channel is the "stream" through which electrons
flow from source to drain.
*** n-channel FET[edit] ***
In an n-channel "depletion-mode" device, a negative gate-to-source voltage
causes a depletion_region to expand in width and encroach on the channel from
the sides, narrowing the channel. If the active region expands to completely
close the channel, the resistance of the channel from source to drain becomes
large, and the FET is effectively turned off like a switch (see right figure,
when there is very small current). This is called "pinch-off", and the voltage
at which it occurs is called the "pinch-off voltage". Conversely, a positive
gate-to-source voltage increases the channel size and allows electrons to flow
easily (see right figure, when there is a conduction channel and current is
large).
In an n-channel "enhancement-mode" device, a conductive channel does not exist
naturally within the transistor, and a positive gate-to-source voltage is
necessary to create one. The positive voltage attracts free-floating electrons
within the body towards the gate, forming a conductive channel. But first,
enough electrons must be attracted near the gate to counter the dopant ions
added to the body of the FET; this forms a region with no mobile carriers
called a depletion_region, and the voltage at which this occurs is referred to
as the threshold_voltage of the FET. Further gate-to-source voltage increase
will attract even more electrons towards the gate which are able to create a
conductive channel from source to drain; this process is called inversion.
*** p-channel FET[edit] ***
In a p-channel "depletion-mode" device, a positive voltage from gate to body
widens the depletion layer by forcing electrons to the gate-insulator/
semiconductor interface, leaving exposed a carrier-free region of immobile,
positively charged acceptor ions.
Conversely, in a p-channel "enhancement-mode" device, a conductive region does
not exist and negative voltage must be used to generate a conduction channel.
**** Effect of drain-to-source voltage on channel[edit] ****
For either enhancement- or depletion-mode devices, at drain-to-source voltages
much less than gate-to-source voltages, changing the gate voltage will alter
the channel resistance, and drain current will be proportional to drain voltage
(referenced to source voltage). In this mode the FET operates like a variable
resistor and the FET is said to be operating in a linear mode or ohmic mode.
[25][26]
If drain-to-source voltage is increased, this creates a significant
asymmetrical change in the shape of the channel due to a gradient of voltage
potential from source to drain. The shape of the inversion region becomes
"pinched-off" near the drain end of the channel. If drain-to-source voltage is
increased further, the pinch-off point of the channel begins to move away from
the drain towards the source. The FET is said to be in saturation mode;[27]
although some authors refer to it as active mode, for a better analogy with
bipolar transistor operating regions.[28][29] The saturation mode, or the
region between ohmic and saturation, is used when amplification is needed. The
in-between region is sometimes considered to be part of the ohmic or linear
region, even where drain current is not approximately linear with drain
voltage.
Even though the conductive channel formed by gate-to-source voltage no longer
connects source to drain during saturation mode, carriers are not blocked from
flowing. Considering again an n-channel enhancement-mode device, a depletion
region exists in the p-type body, surrounding the conductive channel and drain
and source regions. The electrons which comprise the channel are free to move
out of the channel through the depletion region if attracted to the drain by
drain-to-source voltage. The depletion region is free of carriers and has a
resistance similar to silicon. Any increase of the drain-to-source voltage will
increase the distance from drain to the pinch-off point, increasing the
resistance of the depletion region in proportion to the drain-to-source voltage
applied. This proportional change causes the drain-to-source current to remain
relatively fixed, independent of changes to the drain-to-source voltage, quite
unlike its ohmic behavior in the linear mode of operation. Thus, in saturation
mode, the FET behaves as a constant-current_source rather than as a resistor,
and can effectively be used as a voltage amplifier. In this case, the gate-to-
source voltage determines the level of constant current through the channel.
***** Composition[edit] *****
FETs can be constructed from various semiconductors -- silicon is by far the
most common. Most FETs are made by using conventional bulk semiconductor
processing_techniques, using a single_crystal_semiconductor wafer as the active
region, or channel.
Among the more unusual body materials are amorphous_silicon, polycrystalline
silicon or other amorphous semiconductors in thin-film_transistors or organic
field-effect_transistors (OFETs) that are based on organic_semiconductors;
often, OFET gate insulators and electrodes are made of organic materials, as
well. Such FETs are manufactured using a variety of materials such as silicon
carbide (SiC), gallium arsenide (GaAs), gallium nitride (GaN), and indium
gallium arsenide (InGaAs).
In June 2011, IBM announced that it had successfully used graphene-based FETs
in an integrated_circuit.[30][31] These transistors are capable of about
2.23 GHz cutoff frequency, much higher than standard silicon FETs.[32]
***** Types[edit] *****
Depletion-type FETs under typical voltages: JFET, poly-silicon MOSFET, double-
gate MOSFET, metal-gate MOSFET, MESFET.
  Depletion
  Electrons
  Holes
  Metal
  Insulator
Top: source, bottom: drain, left: gate, right: bulk. Voltages that lead to
channel formation are not shown.
The channel of a FET is doped to produce either an n-type semiconductor or a p-
type semiconductor. The drain and source may be doped of opposite type to the
channel, in the case of enhancement mode FETs, or doped of similar type to the
channel as in depletion mode FETs. Field-effect transistors are also
distinguished by the method of insulation between channel and gate. Types of
FETs include:
    * The JFET (junction field-effect transistor) uses a reverse biased pân
      junction to separate the gate from the body.
    * The MOSFET (metalâoxideâsemiconductor field-effect transistor)
      utilizes an insulator (typically SiO2) between the gate and the body.
    * The MNOS metalânitrideâoxideâsemiconductor_transistor utilizes an
      nitride-oxide layer insulator between the gate and the body.
    * The DGMOSFET (dual-gate_MOSFET), a FET with two insulated gates.
    * The DEPFET is a FET formed in a fully depleted substrate and acts as a
      sensor, amplifier and memory node at the same time. It can be used as an
      image (photon) sensor.
    * The FREDFET (fast-reverse or fast-recovery epitaxial diode FET) is a
      specialized FET designed to provide a very fast recovery (turn-off) of
      the body diode.
    * The HIGFET (heterostructure insulated-gate field-effect transistor) is
      now used mainly in research.[33]
    * The MODFET (modulation-doped field-effect transistor) is a high-electron-
      mobility_transistor using a quantum_well structure formed by graded
      doping of the active region.
    * The TFET (tunnel_field-effect_transistor) is based on band-to-band
      tunneling.[34]
    * The IGBT (insulated-gate_bipolar_transistor) is a device for power
      control. It has a structure akin to a MOSFET coupled with a bipolar-like
      main conduction channel. These are commonly used for the 200â3000 V
      drain-to-source voltage range of operation. Power_MOSFETs are still the
      device of choice for drain-to-source voltages of 1 to 200 V.
    * The HEMT (high-electron-mobility_transistor), also called a HFET
      (heterostructure FET), can be made using bandgap_engineering in a ternary
      semiconductor such as AlGaAs. The fully depleted wide-band-gap material
      forms the isolation between gate and body.
    * The ISFET (ion-sensitive field-effect transistor) can be used to measure
      ion concentrations in a solution; when the ion concentration (such as H+,
      see pH_electrode) changes, the current through the transistor will change
      accordingly.
    * The BioFET (Biologically sensitive field-effect transistor) is a class of
      sensors/biosensors based on ISFET technology which are utilized to detect
      charged molecules; when a charged molecule is present, changes in the
      electrostatic field at the BioFET surface result in a measurable change
      in current through the transistor. These include EnFETs, ImmunoFETs,
      GenFETs, DNAFETs, CPFETs, BeetleFETs, and FETs based on ion-channels/
      protein binding.[35]
    * The MESFET (metalâsemiconductor field-effect transistor) substitutes
      the pân_junction of the JFET with a Schottky_barrier; and is used in
      GaAs and other III-V_semiconductor materials.
    * The NOMFET is a nanoparticle organic memory field-effect transistor.[36]
    * The GNRFET (graphene nanoribbon field-effect transistor) uses a graphene
      nanoribbon for its channel.[37]
    * The VeSFET (vertical-slit field-effect transistor) is a square-shaped
      junctionless FET with a narrow slit connecting the source and drain at
      opposite corners. Two gates occupy the other corners, and control the
      current through the slit.[38]
    * The CNTFET (carbon_nanotube_field-effect_transistor).
    * The OFET (organic_field-effect_transistor) uses an organic semiconductor
      in its channel.
    * The DNAFET (DNA_field-effect_transistor) is a specialized FET that acts
      as a biosensor, by using a gate made of single-strand DNA molecules to
      detect matching DNA strands.
    * The QFET (quantum_field_effect_transistor) takes advantage of quantum
      tunneling to greatly increase the speed of transistor operation by
      eliminating the traditional transistor's area of electron conduction.
    * The SB-FET (Schottky-barrier field-effect transistor) is a field-effect
      transistor with metallic source and drain contact electrodes, which
      create Schottky_barriers at both the source-channel and drain-channel
      interfaces.[39][40]
    * The GFET is a highly sensitive graphene-based field effect transistor
      used as biosensors and chemical_sensors. Due to the 2 dimensional
      structure of graphene, along with its physical properties, GFETs offer
      increased sensitivity, and reduced instances of 'false positives' in
      sensing applications[41]
    * The Fe_FET uses a ferroelectric between the gate, allowing the transistor
      to retain its state in the absence of bias - such devices may have
      application as non-volatile_memory.
***** Advantages[edit] *****
The FET has high gate-to-main current resistance, on the order of 100 MÎ© or
more, providing a high degree of isolation between control and flow. Because
base current noise will increase with shaping time,[42] a FET typically
produces less noise than a bipolar_junction_transistor (BJT), and is found in
noise-sensitive electronics such as tuners and low-noise_amplifiers for VHF and
satellite receivers. It is relatively immune to radiation. It exhibits no
offset voltage at zero drain current and makes an excellent signal chopper. It
typically has better thermal stability than a BJT.[24] Because they are
controlled by gate charge, once the gate is closed or open, there is no
additional power draw, as there would be with a bipolar_junction_transistor or
with non-latching relays in some states. This allows extremely low-power
switching, which in turn allows greater miniaturization of circuits because
heat dissipation needs are reduced compared to other types of switches.
***** Disadvantages[edit] *****
A field-effect transistor has a relatively low gainâbandwidth_product
compared to a BJT. The MOSFET is very susceptible to overload voltages, thus
requiring special handling during installation.[43] The fragile insulating
layer of the MOSFET between the gate and channel makes it vulnerable to
electrostatic_discharge or changes to threshold voltage during handling. This
is not usually a problem after the device has been installed in a properly
designed circuit.
FETs often have a very low "on" resistance and have a high "off" resistance.
However, the intermediate resistances are significant, and so FETs can
dissipate large amounts of power while switching. Thus efficiency can put a
premium on switching quickly, but this can cause transients that can excite
stray inductances and generate significant voltages that can couple to the gate
and cause unintentional switching. FET circuits can therefore require very
careful layout and can involve trades between switching speed and power
dissipation. There is also a trade-off between voltage rating and "on"
resistance, so high-voltage FETs have a relatively high "on" resistance and
hence conduction losses.[citation_needed]
***** Failure modes[edit] *****
FETs are relatively robust, especially when operated within the temperature and
electrical limitations defined by the manufacturer (proper derating). However,
modern FET devices can often incorporate a body diode. If the characteristics
of the body diode are not taken into consideration, the FET can experience slow
body diode behavior, where a parasitic transistor will turn on and allow high
current to be drawn from drain to source when the FET is off.[44]
***** Uses[edit] *****
 This section does not cite any sources. Please help improve_this_section by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and
 removed. (September 2018)(Learn_how_and_when_to_remove_this_template_message)
The most commonly used FET is the MOSFET. The CMOS (complementary metal oxide
semiconductor) process technology is the basis for modern digital integrated
circuits. This process_technology uses an arrangement where the (usually
"enhancement-mode") p-channel MOSFET and n-channel MOSFET are connected in
series such that when one is on, the other is off.
In FETs, electrons can flow in either direction through the channel when
operated in the linear mode. The naming convention of drain terminal and source
terminal is somewhat arbitrary, as the devices are typically (but not always)
built symmetrical from source to drain. This makes FETs suitable for switching
analog signals between paths (multiplexing). With this concept, one can
construct a solid-state mixing_board, for example. FET is commonly used as an
amplifier. For example, due to its large input resistance and low output
resistance, it is effective as a buffer in common-drain (source follower)
configuration.
IGBTs are used in switching internal combustion engine ignition coils, where
fast switching and voltage blocking capabilities are important.
***** Source-gated transistor[edit] *****
Source-gated transistors are more robust to manufacturing and environmental
issues in large-area electronics such as display screens, but are slower in
operation than FETs.[45]
***** See also[edit] *****
    * Chemical_field-effect_transistor
    * CMOS
    * FET_amplifier
    * FinFET
    * FlowFET
    * MOSFET
    * Multigate_device
***** References[edit] *****
   1. ^ a b c dLee, Thomas H. (2003). The_Design_of_CMOS_Radio-Frequency
      Integrated_Circuits (PDF). Cambridge_University_Press.
      ISBN 9781139643771.
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
   3. ^ a bPuers, Robert; Baldi, Livio; Voorde, Marcel Van de; Nooten,
      Sebastiaan E. van (2017). Nanoelectronics:_Materials,_Devices,
      Applications,_2_Volumes. John_Wiley_&_Sons. p. 14. ISBN 9783527340538.
   4. ^Grundmann, Marius (2010). The Physics of Semiconductors. Springer-
      Verlag. ISBN 978-3-642-13884-3.
   5. ^Jun-Ichi Nishizawa (1982). Junction Field-Effect Devices. Semiconductor
      Devices for Power Conditioning. Springer. pp. 241â272. doi:10.1007/978-
      1-4684-7263-9_11. ISBN 978-1-4684-7265-3.
   6. ^ a b c"Martin_Atalla_in_Inventors_Hall_of_Fame,_2009". Retrieved 21 June
      2013.
   7. ^ a b"Dawon_Kahng". National_Inventors_Hall_of_Fame. Retrieved 27 June
      2019.
   8. ^Lojek, Bo (2007). History of Semiconductor Engineering. Springer_Science
      &_Business_Media. p. 120. ISBN 9783540342588.
   9. ^"1960_-_Metal_Oxide_Semiconductor_(MOS)_Transistor_Demonstrated". The
      Silicon Engine. Computer_History_Museum.
  10. ^ a bLojek, Bo (2007). History of Semiconductor Engineering. Springer
      Science_&_Business_Media. pp. 321â3. ISBN 9783540342588.
  11. ^"960_-_Metal_Oxide_Semiconductor_(MOS)_Transistor_Demonstrated". The
      Silicon Engine. Computer_History_Museum.
  12. ^Motoyoshi, M. (2009). "Through-Silicon_Via_(TSV)" (PDF). Proceedings of
      the IEEE. 97 (1): 43â48. doi:10.1109/JPROC.2008.2007462. ISSN 0018-
      9219.
  13. ^"Transistors_Keep_Moore's_Law_Alive". EETimes. 12 December 2018.
      Retrieved 18 July 2019.
  14. ^"Who_Invented_the_Transistor?". Computer_History_Museum. 4 December
      2013. Retrieved 20 July 2019.
  15. ^Duncan, Ben (1996). High_Performance_Audio_Power_Amplifiers. Elsevier.
      p. 177. ISBN 9780080508047.
  16. ^ a b"Remarks_by_Director_Iancu_at_the_2019_International_Intellectual
      Property_Conference". United_States_Patent_and_Trademark_Office. June 10,
      2019. Retrieved 20 July 2019.
  17. ^"1963:_Complementary_MOS_Circuit_Configuration_is_Invented". Computer
      History_Museum. Retrieved 6 July 2019.
  18. ^ U.S._Patent_3,102,230, filed in 1960, issued in 1963
  19. ^ D. Kahng and S. M. Sze, "A floating gate and its application to memory
      devices", The Bell System Technical Journal, vol. 46, no. 4, 1967, pp.
      1288â1295
  20. ^Colinge, J.P. (2008). FinFETs_and_Other_Multi-Gate_Transistors. Springer
      Science & Business Media. p. 11. ISBN 9780387717517.
  21. ^Sekigawa, Toshihiro; Hayashi, Yutaka (1 August 1984). "Calculated
      threshold-voltage characteristics of an XMOS transistor having an
      additional bottom gate". Solid-State Electronics. 27 (8): 827â828. doi:
      10.1016/0038-1101(84)90036-4. ISSN 0038-1101.
  22. ^"IEEE_Andrew_S._Grove_Award_Recipients". IEEE_Andrew_S._Grove_Award.
      Institute_of_Electrical_and_Electronics_Engineers. Retrieved 4 July 2019.
  23. ^"The_Breakthrough_Advantage_for_FPGAs_with_Tri-Gate_Technology" (PDF).
      Intel. 2014. Retrieved 4 July 2019.
  24. ^Jacob_Millman (1985). Electronic devices and circuits. Singapore:
      McGraw-Hill_International. p. 397. ISBN 978-0-07-085505-2.
  25. ^ a bJacob Millman (1985). Electronic devices and circuits. Singapore:
      McGraw-Hill. pp. 384â385. ISBN 978-0-07-085505-2.
  26. ^ Galup-Montoro, C.; Schneider, M.C. (2007). MOSFET modeling for circuit
      analysis and design. London/Singapore: World_Scientific. p. 83. ISBN 978-
      981-256-810-6.
  27. ^Norbert R Malik (1995). Electronic circuits: analysis, simulation, and
      design. Englewood Cliffs, NJ: Prentice Hall. pp. 315â316. ISBN 978-0-
      02-374910-0.
  28. ^ Spencer, R.R.; Ghausi, M.S. (2001). Microelectronic circuits. Upper
      Saddle River NJ: Pearson Education/Prentice-Hall. p. 102. ISBN 978-0-201-
      36183-4.
  29. ^ Sedra, A. S.; Smith, K.C. (2004). Microelectronic circuits (Fifth ed.).
      New York: Oxford University Press. p. 552. ISBN 978-0-19-514251-8.
  30. ^ PR Gray; PJ Hurst; SH Lewis; RG Meyer (2001). Analysis and design of
      analog integrated circuits (Fourth ed.). New York: Wiley. pp. Â§1.5.2 p.
      45. ISBN 978-0-471-32168-2.
  31. ^Bob Yirka (10 January 2011). "IBM_creates_first_graphene_based
      integrated_circuit". Phys.org. Retrieved 14 January 2019.
  32. ^Lin, Y.-M.; Valdes-Garcia, A.; Han, S.-J.; Farmer, D. B.; Sun, Y.; Wu,
      Y.; Dimitrakopoulos, C.; Grill, A; Avouris, P; Jenkins, K. A. (2011).
      "Wafer-Scale Graphene Integrated Circuit". Science. 332 (6035):
      1294â1297. doi:10.1126/science.1204428. PMID 21659599.
  33. ^Belle DumÃ© (10 December 2012). "Flexible_graphene_transistor_sets_new
      records". Physics World. Retrieved 14 January 2019.
  34. ^ freepatentsonline.com, HIGFET and method - Motorola]
  35. ^Ionescu, A. M.; Riel,_H. (2011). "Tunnel field-effect transistors as
      energy-efficient electronic switches". Nature. 479 (7373): 329â337.
      doi:10.1038/nature10679. PMID 22094693.
  36. ^SchÃ¶ning, Michael J.; Poghossian, Arshak (2002). "Recent_advances_in
      biologically_sensitive_field-effect_transistors_(BioFETs)" (PDF).
      Analyst. 127 (9): 1137â1151. doi:10.1039/B204444G.
  37. ^"Organic_transistor_paves_way_for_new_generations_of_neuro-inspired
      computers". ScienceDaily. January 29, 2010. Retrieved January 14, 2019.
  38. ^Sarvari H.; Ghayour, R.; Dastjerdy, E. (2011). "Frequency analysis of
      graphene nanoribbon FET by Non-Equilibrium Green's Function in mode
      space". Physica E: Low-dimensional Systems and Nanostructures. 43 (8):
      1509â1513. doi:10.1016/j.physe.2011.04.018.
  39. ^Jerzy Ruzyllo (2016). Semiconductor_Glossary:_A_Resource_for
      Semiconductor_Community. World Scientific. p. 244. ISBN 978-981-4749-56-
      5.
  40. ^Appenzeller, J, et al. (November 2008). "Toward Nanowire Electronics".
      IEEE Transactions on Electron Devices. 55 (11): 2827â2845. doi:10.1109/
      ted.2008.2008011. ISSN 0018-9383. OCLC 755663637.
  41. ^Prakash, Abhijith; Ilatikhameneh, Hesameddin; Wu, Peng; Appenzeller,
      Joerg (2017). "Understanding_contact_gating_in_Schottky_barrier
      transistors_from_2D_channels". Scientific Reports. 7 (1): 12596. doi:
      10.1038/s41598-017-12816-3. ISSN 2045-2322. OCLC 1010581463. PMC 5626721.
      PMID 28974712.
  42. ^Miklos, Bolza. "What_Are_Graphene_Field_Effect_Transistors_(GFETs)?".
      Graphenea. Retrieved 14 January 2019.
  43. ^ VIII.5._Noise_in_Transistors
  44. ^Allen Mottershead (2004). Electronic devices and circuits. New Delhi:
      Prentice-Hall of India. ISBN 978-81-203-0124-5.
  45. ^ Slow_Body_Diode_Failures_of_Field_Effect_Transistors_(FETs):_A_Case
      Study.
  46. ^Sporea, R.A.; Trainor, M.J.; Young, N.D.; Silva, S.R.P. (2014). "Source-
      gated_transistors_for_order-of-magnitude_performance_improvements_in
      thin-film_digital_circuits". Scientific Reports. 4: 4295. doi:10.1038/
      srep04295. PMC 3944386. PMID 24599023.
***** External links[edit] *****
 Wikimedia Commons has media related to Field-effect_Transistors.
    * PBS_The_Field_Effect_Transistor
    * How_Semiconductors_and_Transistors_Work_(MOSFETs) WeCanFigureThisOut.org
    * Junction_Field_Effect_Transistor
    * CMOS_gate_circuitry
    * Winning_the_Battle_Against_Latchup_in_CMOS_Analog_Switches
    * Field_Effect_Transistors_in_Theory_and_Practice
    * The_Field_Effect_Transistor_as_a_Voltage_Controlled_Resistor
    * "The_FET_(field_effect_transistor)". rolinychupetin (L.R.Linares). March
      30, 2013 – via YouTube.
    * v
    * t
    * e
Transistor amplifiers
            Bipolar_junction          * Common_emitter
            transistor:               * Common_collector
                                      * Common_base
            Field-effect              * Common_source
            transistor:               * Common_drain
[JFET_N-dep                           * Common_gate      [BJT_NPN_symbol_
symbol.svg]                           * Darlington       (case).svg]
                                        transistor
            Multiple transistors:     * Complementary
                                        feedback_pair
                                      * Cascode
                                      * Long-tailed_pair
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
                   MOS_transistors       * MOS_field-effect_transistor (MOSFET)
                                         * Multi-gate_field-effect_transistor
                                           (MuGFET)
                                         * NMOS
                                         * PMOS
                                         * Power_MOSFET
                                         * Thin-film_transistor (TFT)
                                         * VMOS
                                         * Bipolar_junction_transistor (BJT)
                                         * Darlington_transistor
                                         * Diffusion_transistor
                                         * Field-effect transistor (FET)
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
                                              * GND: 4131472-4
Authority_control [Edit_this_at_Wikidata]     * LCCN: sh85048099
                                              * NDL: 01150221

Retrieved from "https://en.wikipedia.org/w/index.php?title=Field-
effect_transistor&oldid=908697963"
Categories:
    * Transistor_types
    * FETs
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2018
    * Articles_needing_additional_references_from_September_2018
    * All_articles_needing_additional_references
    * Commons_category_link_is_on_Wikidata
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
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * EstremeÃ±u
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Bahasa_Indonesia
    * Italiano
    * Jawa
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * LietuviÅ³
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Seeltersk
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ä¸­æ
Edit_links
    * This page was last edited on 31 July 2019, at 11:28 (UTC).
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
