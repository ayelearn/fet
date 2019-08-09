The following text has been accessed from https://en.wikipedia.org/wiki/Bipolar_junction_transistor at Fri Aug 9 03:08:56 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Bipolar junction transistor ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
"Junction transistor" redirects here. For other uses, see Junction_transistor_
(disambiguation).
"BJT" redirects here. For the Japanese language proficiency test, see Business
Japanese_Proficiency_Test. For Beijing Time, see China_Standard_Time.
[BJT_NPN_symbol_(case).svg] NPN
[BJT_PNP_symbol_(case).svg] PNP
BJT schematic symbols
Typical individual BJT packages. From top to bottom: TO-3, TO-126, TO-92, SOT-
23
A bipolar junction transistor (bipolar transistor or BJT) is a type of
transistor that uses both electrons and holes as charge carriers.
Unipolar transistors, such as field-effect_transistors, only use one kind of
charge carrier. BJTs use two junctions between two semiconductor types, n-type
and p-type.
BJTs are manufactured in two types: NPN and PNP, and are available as
individual components, or fabricated in integrated_circuits, often in large
numbers.
⁰
***** Contents *****
    * 1_Usage
    * 2_Current_direction_conventions
    * 3_Function
          o 3.1_Voltage,_current,_and_charge_control
          o 3.2_Turn-on,_turn-off,_and_storage_delay
          o 3.3_Transistor_characteristics:_alpha_(Î±)_and_beta_(Î²)
    * 4_Structure
          o 4.1_NPN
          o 4.2_PNP
          o 4.3_Heterojunction_bipolar_transistor
    * 5_Regions_of_operation
          o 5.1_Active-mode_transistors_in_circuits
    * 6_History
          o 6.1_Germanium_transistors
          o 6.2_Early_manufacturing_techniques
                # 6.2.1_Bipolar_transistors
    * 7_Theory_and_modeling
          o 7.1_Large-signal_models
                # 7.1.1_EbersâMoll_model
                      # 7.1.1.1_Base-width_modulation
                      # 7.1.1.2_Punchthrough
                # 7.1.2_GummelâPoon_charge-control_model
          o 7.2_Small-signal_models
                # 7.2.1_Hybrid-pi_model
                # 7.2.2_h-parameter_model
                      # 7.2.2.1_Etymology_of_hFE
          o 7.3_Industry_models
    * 8_Applications
          o 8.1_High-speed_digital_logic
          o 8.2_Amplifiers
          o 8.3_Temperature_sensors
          o 8.4_Logarithmic_converters
    * 9_Vulnerabilities
    * 10_See_also
    * 11_Notes
    * 12_References
    * 13_External_links
***** Usage[edit] *****
BJTs can be used as amplifiers or switches. This ability gives them many
applications in electronic equipment such as computers, televisions, mobile
phones, audio amplifiers, industrial control, and radio transmitters.
***** Current direction conventions[edit] *****
By convention, the direction of current on diagrams is shown as the direction
that a positive charge would move. This is called conventional current.
However, current in many metal conductors is due to the flow of electrons.
Because electrons carry a negative charge, they move in the direction opposite
to conventional current.[a] On the other hand, inside a bipolar transistor,
currents can be composed of both positively charged holes and negatively
charged electrons. In this article, current arrows are shown in the
conventional direction, but labels for the movement of holes and electrons show
their actual direction inside the transistor. The arrow on the symbol for
bipolar transistors indicates the PN junction between base and emitter and
points in the direction in which conventional current travels.
***** Function[edit] *****
 This section may be too technical for most readers to understand. Please help
 improve_it to make_it_understandable_to_non-experts, without removing the
 technical details. (July 2012)(Learn_how_and_when_to_remove_this_template
 message)
BJTs are available in two types, or polarities, known as PNP and NPN based on
the doping types of the three main terminal regions. An NPN transistor
comprises two semiconductor_junctions that share a thin p-doped region, and a
PNP transistor comprises two semiconductor junctions that share a thin n-doped
region.
NPN BJT with forward-biased EâB junction and reverse-biased BâC junction
Charge flow in a BJT is due to diffusion of charge_carriers across a junction
between two regions of different charge concentrations. The regions of a BJT
are called emitter, base, and collector.[b] A discrete transistor has three
leads for connection to these regions. Typically, the emitter region is heavily
doped compared to the other two layers, and the collector is doped much lighter
than the base (collector doping is typically ten times lighter than base doping
[2]). By design, most of the BJT collector current is due to the flow of charge
carriers (electrons or holes) injected from a heavily doped emitter into the
base where they are minority_carriers that diffuse toward the collector, and so
BJTs are classified as minority-carrier devices.
In typical operation, the baseâemitter junction is forward-biased, which
means that the p-doped side of the junction is at a more positive potential
than the n-doped side, and the baseâcollector junction is reverse-biased.
When forward bias is applied to the baseâemitter junction, the equilibrium
between the thermally generated carriers and the repelling electric field of
the n-doped emitter depletion_region is disturbed. This allows thermally
excited electrons to inject from the emitter into the base region. These
electrons diffuse through the base from the region of high concentration near
the emitter toward the region of low concentration near the collector. The
electrons in the base are called minority_carriers because the base is doped p-
type, which makes holes the majority_carrier in the base.
To minimize the fraction of carriers that recombine before reaching the
collectorâbase junction, the transistor's base region must be thin enough
that carriers can diffuse across it in much less time than the semiconductor's
minority-carrier lifetime. Having a lightly doped base ensures recombination
rates are low. In particular, the thickness of the base must be much less than
the diffusion_length of the electrons. The collectorâbase junction is
reverse-biased, and so negligible electron injection occurs from the collector
to the base, but carriers that are injected into the base and diffuse to reach
the collector-base depletion region are swept into the collector by the
electric field in the depletion region. The thin shared base and asymmetric
collectorâemitter doping are what differentiates a bipolar transistor from
two separate and oppositely biased diodes connected in series.
**** Voltage, current, and charge control[edit] ****
The collectorâemitter current can be viewed as being controlled by the
baseâemitter current (current control), or by the baseâemitter voltage
(voltage control). These views are related by the currentâvoltage relation of
the baseâemitter junction, which is the usual exponential currentâvoltage
curve of a pân_junction (diode).[3]
The explanation for collector current is the concentration gradient of minority
carriers in the base region.[3][4][5] Due to low-level_injection (in which
there are much fewer excess carriers than normal majority carriers) the
ambipolar_transport rates (in which the excess majority and minority carriers
flow at the same rate) is in effect determined by the excess minority carriers.
Detailed transistor_models of transistor action, such as the GummelâPoon
model, account for the distribution of this charge explicitly to explain
transistor behaviour more exactly.[6] The charge-control view easily handles
phototransistors, where minority carriers in the base region are created by the
absorption of photons, and handles the dynamics of turn-off, or recovery time,
which depends on charge in the base region recombining. However, because base
charge is not a signal that is visible at the terminals, the current- and
voltage-control views are generally used in circuit design and analysis.
In analog_circuit design, the current-control view is sometimes used because it
is approximately linear. That is, the collector current is approximately
&#x03B2;  F     {\displaystyle \beta _{\text{F}}}  [{\displaystyle \beta _
{\text{F}}}] times the base current. Some basic circuits can be designed by
assuming that the base-emitter voltage is approximately constant and that
collector current is Î² times the base current. However, to accurately and
reliably design production BJT circuits, the voltage-control (for example,
EbersâMoll) model is required[3]. The voltage-control model requires an
exponential function to be taken into account, but when it is linearized such
that the transistor can be modeled as a transconductance, as in the
EbersâMoll_model, design for circuits such as differential amplifiers again
becomes a mostly linear problem, so the voltage-control view is often
preferred. For translinear_circuits, in which the exponential IâV curve is
key to the operation, the transistors are usually modeled as voltage-controlled
current sources whose transconductance is proportional to their collector
current. In general, transistor-level circuit analysis is performed using SPICE
or a comparable analog-circuit simulator, so mathematical model complexity is
usually not of much concern to the designer, but a simplified view of the
characteristics allows designs to be created following a logical process.
**** Turn-on, turn-off, and storage delay[edit] ****
Main article: Baker_clamp
Bipolar transistors, and particularly power transistors, have long base-storage
times when they are driven into saturation; the base storage limits turn-off
time in switching applications. A Baker_clamp can prevent the transistor from
heavily saturating, which reduces the amount of charge stored in the base and
thus improves switching time.
**** Transistor characteristics: alpha (Î±) and beta (Î²) [edit] ****
The proportion of carriers able to cross the base and reach the collector is a
measure of the BJT efficiency. The heavy doping of the emitter region and light
doping of the base region causes many more electrons to be injected from the
emitter into the base than holes to be injected from the base into the emitter.
A thin and lightly-doped base region means that most of the minority carriers
that are injected into the base will diffuse to the collector and not
recombine.
The common-emitter current gain is represented by Î²F or the h-parameter hFE;
it is approximately the ratio of the DC collector current to the DC base
current in forward-active region. It is typically greater than 50 for small-
signal transistors, but can be smaller in transistors designed for high-power
applications. Both injection efficiency and recombination in the base reduce
the BJT gain.
Another useful characteristic is the common-base current gain, Î±F. The common-
base current gain is approximately the gain of current from emitter to
collector in the forward-active region. This ratio usually has a value close to
unity; between 0.980 and 0.998. It is less than unity due to recombination_of
charge_carriers as they cross the base region.
Alpha and beta are related by the following identities:
              &#x03B1;  F      =    I  C    I  E     ,    &#x03B2;  F      =
      I  C    I  B     ,      &#x03B1;  F      =    &#x03B2;  F    1 +
      &#x03B2;  F         &#x27FA;   &#x03B2;  F      =    &#x03B1;  F    1
      &#x2212;  &#x03B1;  F      .       {\displaystyle {\begin{aligned}\alpha
      _{\text{F}}&={\frac {I_{\text{C}}}{I_{\text{E}}}},&\beta _{\text{F}}&=
      {\frac {I_{\text{C}}}{I_{\text{B}}}},\\\alpha _{\text{F}}&={\frac {\beta
      _{\text{F}}}{1+\beta _{\text{F}}}}&\iff \beta _{\text{F}}&={\frac {\alpha
      _{\text{F}}}{1-\alpha _{\text{F}}}}.\end{aligned}}}  [{\displaystyle
      {\begin{aligned}\alpha _{\text{F}}&={\frac {I_{\text{C}}}{I_{\text
      {E}}}},&\beta _{\text{F}}&={\frac {I_{\text{C}}}{I_{\text{B}}}},\\\alpha
      _{\text{F}}&={\frac {\beta _{\text{F}}}{1+\beta _{\text{F}}}}&\iff \beta
      _{\text{F}}&={\frac {\alpha _{\text{F}}}{1-\alpha _{\text{F}}}}.\end
      {aligned}}}]
Beta is a convenient figure of merit to describe the performance of a bipolar
transistor, but is not a fundamental physical property of the device. Bipolar
transistors can be considered voltage-controlled devices (fundamentally the
collector current is controlled by the base-emitter voltage; the base current
could be considered a defect and is controlled by the characteristics of the
base-emitter junction and recombination in the base). In many designs beta is
assumed high enough so that base current has a negligible effect on the
circuit. In some circuits (generally switching circuits), sufficient base
current is supplied so that even the lowest beta value a particular device may
have will still allow the required collector current to flow.
***** Structure[edit] *****
Simplified cross section of a planar NPN bipolar junction transistor
A BJT consists of three differently doped semiconductor regions: the emitter
region, the base region and the collector region. These regions are,
respectively, p type, n type and p type in a PNP transistor, and n type, p type
and n type in an NPN transistor. Each semiconductor region is connected to a
terminal, appropriately labeled: emitter (E), base (B) and collector (C).
The base is physically located between the emitter and the collector and is
made from lightly doped, high-resistivity material. The collector surrounds the
emitter region, making it almost impossible for the electrons injected into the
base region to escape without being collected, thus making the resulting value
of Î± very close to unity, and so, giving the transistor a large Î². A cross-
section view of a BJT indicates that the collectorâbase junction has a much
larger area than the emitterâbase junction.
The bipolar junction transistor, unlike other transistors, is usually not a
symmetrical device. This means that interchanging the collector and the emitter
makes the transistor leave the forward active mode and start to operate in
reverse mode. Because the transistor's internal structure is usually optimized
for forward-mode operation, interchanging the collector and the emitter makes
the values of Î± and Î² in reverse operation much smaller than those in forward
operation; often the Î± of the reverse mode is lower than 0.5. The lack of
symmetry is primarily due to the doping ratios of the emitter and the
collector. The emitter is heavily doped, while the collector is lightly doped,
allowing a large reverse bias voltage to be applied before the collectorâbase
junction breaks down. The collectorâbase junction is reverse biased in normal
operation. The reason the emitter is heavily doped is to increase the emitter
injection efficiency: the ratio of carriers injected by the emitter to those
injected by the base. For high current gain, most of the carriers injected into
the emitterâbase junction must come from the emitter.
Die of a KSY34 high-frequency NPN transistor. Bond wires connect to the base
and emitter
The low-performance "lateral" bipolar transistors sometimes used in CMOS
processes are sometimes designed symmetrically, that is, with no difference
between forward and backward operation.
Small changes in the voltage applied across the baseâemitter terminals cause
the current between the emitter and the collector to change significantly. This
effect can be used to amplify the input voltage or current. BJTs can be thought
of as voltage-controlled current_sources, but are more simply characterized as
current-controlled current sources, or current amplifiers, due to the low
impedance at the base.
Early transistors were made from germanium but most modern BJTs are made from
silicon. A significant minority are also now made from gallium_arsenide,
especially for very high speed applications (see HBT, below).
**** NPN[edit] ****
The symbol of an NPN BJT. A mnemonic for the symbol is "not pointing in".
NPN is one of the two types of bipolar transistors, consisting of a layer of P-
doped semiconductor (the "base") between two N-doped layers. A small current
entering the base is amplified to produce a large collector and emitter
current. That is, when there is a positive potential difference measured from
the base of an NPN transistor to its emitter (that is, when the base is high
relative to the emitter), as well as a positive potential difference measured
from the collector to the emitter, the transistor becomes active. In this "on"
state, current flows from the collector to the emitter of the transistor. Most
of the current is carried by electrons moving from emitter to collector as
minority_carriers in the P-type base region. To allow for greater current and
faster operation, most bipolar transistors used today are NPN because electron
mobility is higher than hole_mobility.
**** PNP[edit] ****
The symbol of a PNP BJT. A mnemonic for the symbol is "points in proudly".
The other type of BJT is the PNP, consisting of a layer of N-doped
semiconductor between two layers of P-doped material. A small current leaving
the base is amplified in the collector output. That is, a PNP transistor is
"on" when its base is pulled low relative to the emitter. In a PNP transistor,
the emitterâbase region is forward biased, so holes are injected into the
base as minority carriers. The base is very thin, and most of the holes cross
the reverse-biased baseâcollector junction to the collector.
The arrows in the NPN and PNP transistor symbols indicate the PN junction
between the base and emitter. When the device is in forward active or forward
saturated mode, the arrow, placed on the emitter leg, points in the direction
of the conventional_current.
**** Heterojunction bipolar transistor[edit] ****
Bands in graded heterojunction NPN bipolar transistor. Barriers indicated for
electrons to move from emitter to base and for holes to be injected backward
from base to emitter; also, grading of bandgap in base assists electron
transport in base region. Light colors indicate depleted_regions.
The heterojunction_bipolar_transistor (HBT) is an improvement of the BJT that
can handle signals of very high frequencies up to several hundred GHz. It is
common in modern ultrafast circuits, mostly RF systems.[7][8]
Symbol for NPN bipolar transistor with current flow direction
Heterojunction transistors have different semiconductors for the elements of
the transistor. Usually the emitter is composed of a larger bandgap material
than the base. The figure shows that this difference in bandgap allows the
barrier for holes to inject backward from the base into the emitter, denoted in
the figure as ÎÏp, to be made large, while the barrier for electrons to
inject into the base ÎÏn is made low. This barrier arrangement helps reduce
minority carrier injection from the base when the emitter-base junction is
under forward bias, and thus reduces base current and increases emitter
injection efficiency.
The improved injection of carriers into the base allows the base to have a
higher doping level, resulting in lower resistance to access the base
electrode. In the more traditional BJT, also referred to as homojunction BJT,
the efficiency of carrier injection from the emitter to the base is primarily
determined by the doping ratio between the emitter and base, which means the
base must be lightly doped to obtain high injection efficiency, making its
resistance relatively high. In addition, higher doping in the base can improve
figures of merit like the Early_voltage by lessening base narrowing.
The grading of composition in the base, for example, by progressively
increasing the amount of germanium in a SiGe transistor, causes a gradient in
bandgap in the neutral base, denoted in the figure by ÎÏG, providing a
"built-in" field that assists electron transport across the base. That drift
component of transport aids the normal diffusive transport, increasing the
frequency response of the transistor by shortening the transit time across the
base.
Two commonly used HBTs are siliconâgermanium and aluminum gallium arsenide,
though a wide variety of semiconductors may be used for the HBT structure. HBT
structures are usually grown by epitaxy techniques like MOCVD and MBE.
***** Regions of operation[edit] *****
Junction  Applied   Junction bias   Mode
type      voltages  B-E     B-C
          E < B < C Forward Reverse Forward-active
NPN       E < B > C Forward Forward Saturation
          E > B < C Reverse Reverse Cut-off
          E > B > C Reverse Forward Reverse-active
          E < B < C Reverse Forward Reverse-active
PNP       E < B > C Reverse Reverse Cut-off
          E > B < C Forward Forward Saturation
          E > B > C Forward Reverse Forward-active
Bipolar transistors have four distinct regions of operation, defined by BJT
junction biases.
  Forward-active (or simply active)
      The baseâemitter junction is forward biased and the baseâcollector
      junction is reverse biased. Most bipolar transistors are designed to
      afford the greatest common-emitter current gain, Î²F, in forward-active
      mode. If this is the case, the collectorâemitter current is
      approximately proportional to the base current, but many times larger,
      for small base current variations.
  Reverse-active (or inverse-active or inverted)
      By reversing the biasing conditions of the forward-active region, a
      bipolar transistor goes into reverse-active mode. In this mode, the
      emitter and collector regions switch roles. Because most BJTs are
      designed to maximize current gain in forward-active mode, the Î²F in
      inverted mode is several times smaller (2â3 times for the ordinary
      germanium transistor). This transistor mode is seldom used, usually being
      considered only for failsafe conditions and some types of bipolar_logic.
      The reverse bias breakdown voltage to the base may be an order of
      magnitude lower in this region.
  Saturation
      With both junctions forward-biased, a BJT is in saturation mode and
      facilitates high current conduction from the emitter to the collector (or
      the other direction in the case of NPN, with negatively charged carriers
      flowing from emitter to collector). This mode corresponds to a logical
      "on", or a closed switch.
  Cut-off
      In cut-off, biasing conditions opposite of saturation (both junctions
      reverse biased) are present. There is very little current, which
      corresponds to a logical "off", or an open switch.
  Avalanche_breakdown region
Input characteristics
output characteristics
Input and output characteristics for a common-base silicon transistor
amplifier.
The modes of operation can be described in terms of the applied voltages (this
description applies to NPN transistors; polarities are reversed for PNP
transistors):
  Forward-active
      Base higher than emitter, collector higher than base (in this mode the
      collector current is proportional to base current by      &#x03B2;  F
      {\displaystyle \beta _{\text{F}}}  [{\displaystyle \beta _{\text{F}}}]).
  Saturation
      Base higher than emitter, but collector is not higher than base.
  Cut-off
      Base lower than emitter, but collector is higher than base. It means the
      transistor is not letting conventional current go through from collector
      to emitter.
  Reverse-active
      Base lower than emitter, collector lower than base: reverse conventional
      current goes through transistor.
In terms of junction biasing: (reverse biased baseâcollector junction means
Vbc < 0 for NPN, opposite for PNP)
Although these regions are well defined for sufficiently large applied voltage,
they overlap somewhat for small (less than a few hundred millivolts) biases.
For example, in the typical grounded-emitter configuration of an NPN BJT used
as a pulldown switch in digital logic, the "off" state never involves a
reverse-biased junction because the base voltage never goes below ground;
nevertheless the forward bias is close enough to zero that essentially no
current flows, so this end of the forward active region can be regarded as the
cutoff region.
**** Active-mode transistors in circuits[edit] ****
Structure and use of NPN transistor. Arrow according to schematic.
The diagram shows a schematic representation of an NPN transistor connected to
two voltage sources. (The same description applies to a PNP transistor with
reversed directions of current flow and applied voltage.) This applied voltage
causes the lower P-N junction to become forward biased, allowing a flow of
electrons from the emitter into the base. In active mode, the electric field
existing between base and collector (caused by VCE) will cause the majority of
these electrons to cross the upper P-N junction into the collector to form the
collector current IC. The remainder of the electrons recombine with holes, the
majority carriers in the base, making a current through the base connection to
form the base current, IB. As shown in the diagram, the emitter current, IE, is
the total transistor current, which is the sum of the other terminal currents,
(i.e., IE = IB + IC).
In the diagram, the arrows representing current point in the direction of
conventional_current â the flow of electrons is in the opposite direction of
the arrows because electrons carry negative electric_charge. In active mode,
the ratio of the collector current to the base current is called the DC current
gain. This gain is usually 100 or more, but robust circuit designs do not
depend on the exact value (for example see op-amp). The value of this gain for
DC signals is referred to as      h  FE     {\displaystyle h_{\text{FE}}}  [h_
{\text{FE}}], and the value of this gain for small signals is referred to as
h  fe     {\displaystyle h_{\text{fe}}}  [h_{\text{fe}}]. That is, when a small
change in the currents occurs, and sufficient time has passed for the new
condition to reach a steady state      h  fe     {\displaystyle h_{\text{fe}}}
[h_{\text{fe}}] is the ratio of the change in collector current to the change
in base current. The symbol     &#x03B2;   {\displaystyle \beta }  [\beta ] is
used for both      h  FE     {\displaystyle h_{\text{FE}}}  [h_{\text{FE}}] and
h  fe     {\displaystyle h_{\text{fe}}}  [h_{\text{fe}}].[9]
The emitter current is related to      V  BE     {\displaystyle V_{\text{BE}}}
[V_{\text{BE}}] exponentially. At room_temperature, an increase in      V  BE
{\displaystyle V_{\text{BE}}}  [V_{\text{BE}}] by approximately 60 mV increases
the emitter current by a factor of 10. Because the base current is
approximately proportional to the collector and emitter currents, they vary in
the same way.
***** History[edit] *****
The bipolar point-contact_transistor was invented in December 1947[10] at the
Bell_Telephone_Laboratories by John_Bardeen and Walter_Brattain under the
direction of William_Shockley. The junction version known as the bipolar
junction transistor (BJT), invented by Shockley in 1948,[11] was for three
decades the device of choice in the design of discrete and integrated_circuits.
Nowadays, the use of the BJT has declined in favor of CMOS technology in the
design of digital integrated circuits. The incidental low performance BJTs
inherent in CMOS ICs, however, are often utilized as bandgap_voltage_reference,
silicon_bandgap_temperature_sensor and to handle electrostatic_discharge.
**** Germanium transistors[edit] ****
The germanium transistor was more common in the 1950s and 1960s but has a
greater tendency to exhibit thermal_runaway.
**** Early manufacturing techniques[edit] ****
Various methods of manufacturing bipolar transistors were developed.[12]
*** Bipolar transistors[edit] ***
    * Point-contact_transistor â first transistor ever constructed (December
      1947), a bipolar transistor, limited commercial use due to high cost and
      noise.
          o Tetrode_point-contact_transistor â Point-contact transistor
            having two emitters. It became obsolete in the middle 1950s.
    * Junction transistors
          o Grown-junction_transistor – first bipolar junction transistor made.
            [13] Invented by William_Shockley at Bell_Labs on June 23, 1948.
            [14] Patent filed on June 26, 1948.
          o Alloy-junction_transistor – emitter and collector alloy beads fused
            to base. Developed at General_Electric and RCA[15] in 1951.
                # Micro-alloy_transistor (MAT) – high speed type of alloy
                  junction transistor. Developed at Philco.[16]
                # Micro-alloy_diffused_transistor (MADT) – high speed type of
                  alloy junction transistor, speedier than MAT, a diffused-base
                  transistor. Developed at Philco.
                # Post-alloy_diffused_transistor (PADT) – high speed type of
                  alloy junction transistor, speedier than MAT, a diffused-base
                  transistor. Developed at Philips.
          o Tetrode_transistor – high speed variant of grown-junction
            transistor[17] or alloy junction transistor[18] with two
            connections to base.
          o Surface-barrier_transistor – high-speed metal barrier junction
            transistor. Developed at Philco[19] in 1953.[20]
          o Drift-field_transistor – high speed bipolar junction transistor.
            Invented by Herbert_Kroemer[21][22] at the Central Bureau of
            Telecommunications Technology of the German Postal Service, in
            1953.
          o Spacistor – circa 1957.
          o Diffusion_transistor – modern type bipolar junction transistor.
            Prototypes[23] developed at Bell Labs in 1954.
                # Diffused-base_transistor – first implementation of diffusion
                  transistor.
                # Mesa_transistor – Developed at Texas_Instruments in 1957.
                # Planar_transistor – the bipolar junction transistor that made
                  mass-produced monolithic integrated_circuits possible.
                  Developed by Jean_Hoerni[24] at Fairchild in 1959.
          o Epitaxial transistor[25] – a bipolar junction transistor made using
            vapor phase deposition. See epitaxy. Allows very precise control of
            doping levels and gradients.
***** Theory and modeling[edit] *****
Band_diagram for NPN transistor at equilibrium
Band_diagram for NPN transistor in active mode, showing injection of electrons
from emitter to base, and their overshoot into the collector
Transistors can be thought of as two diodes (PâN_junctions) sharing a common
region that minority carriers can move through. A PNP BJT will function like
two diodes that share an N-type cathode region, and the NPN like two diodes
sharing a P-type anode region. Connecting two diodes with wires will not make a
transistor, since minority carriers will not be able to get from one PâN
junction to the other through the wire.
Both types of BJT function by letting a small current input to the base control
an amplified output from the collector. The result is that the transistor makes
a good switch that is controlled by its base input. The BJT also makes a good
amplifier, since it can multiply a weak input signal to about 100 times its
original strength. Networks of transistors are used to make powerful amplifiers
with many different applications. In the discussion below, focus is on the NPN
bipolar transistor. In the NPN transistor in what is called active mode, the
baseâemitter voltage      V  BE     {\displaystyle V_{\text{BE}}}  [V_{\text
{BE}}] and collectorâbase voltage      V  CB     {\displaystyle V_{\text
{CB}}}  [V_{\text{CB}}] are positive, forward biasing the emitterâbase
junction and reverse-biasing the collectorâbase junction. In the active mode
of operation, electrons are injected from the forward biased n-type emitter
region into the p-type base where they diffuse as minority carriers to the
reverse-biased n-type collector and are swept away by the electric field in the
reverse-biased collectorâbase junction. For a figure describing forward and
reverse bias, see semiconductor_diodes.
**** Large-signal models[edit] ****
In 1954, Jewell_James_Ebers and John_L._Moll introduced their mathematical
model of transistor currents:[26]
*** EbersâMoll model[edit] ***
Ebers–Moll model for an NPN transistor.[27] IB, IC and IE are the base,
collector and emitter currents; ICD and IED are the collector and emitter diode
currents; Î±F and Î±R are the forward and reverse common-base current gains.
Ebers–Moll model for a PNP transistor
Approximated Ebers–Moll model for an NPN transistor in the forward active mode.
The collector diode is reverse-biased so ICD is virtually zero. Most of the
emitter diode current (Î±F is nearly 1) is drawn from the collector, providing
the amplification of the base current.
The DC emitter and collector currents in active mode are well modeled by an
approximation to the EbersâMoll model:
              I  E      =  I  ES    (   e    V  BE    V  T      &#x2212; 1  )
      I  C      =  &#x03B1;  F    I  E        I  B      =  (  1 &#x2212;
      &#x03B1;  F    )   I  E         {\displaystyle {\begin{aligned}I_{\text
      {E}}&=I_{\text{ES}}\left(e^{\frac {V_{\text{BE}}}{V_{\text{T}}}}-
      1\right)\\I_{\text{C}}&=\alpha _{\text{F}}I_{\text{E}}\\I_{\text
      {B}}&=\left(1-\alpha _{\text{F}}\right)I_{\text{E}}\end{aligned}}}  [
      {\displaystyle {\begin{aligned}I_{\text{E}}&=I_{\text{ES}}\left(e^{\frac
      {V_{\text{BE}}}{V_{\text{T}}}}-1\right)\\I_{\text{C}}&=\alpha _{\text
      {F}}I_{\text{E}}\\I_{\text{B}}&=\left(1-\alpha _{\text{F}}\right)I_{\text
      {E}}\end{aligned}}}]
The base internal current is mainly by diffusion (see Fick's_law) and
          J  n  (  base  )   =   1 W   q  D  n    n  b o    e    V  EB    V  T
      {\displaystyle J_{n\,({\text{base}})}={\frac {1}{W}}qD_{n}n_{bo}e^{\frac
      {V_{\text{EB}}}{V_{\text{T}}}}}  [{\displaystyle J_{n\,({\text{base}})}=
      {\frac {1}{W}}qD_{n}n_{bo}e^{\frac {V_{\text{EB}}}{V_{\text{T}}}}}]
where
    *     V  T     {\displaystyle V_{\text{T}}}  [V_{\text{T}}] is the thermal
      voltage     k T  /  q   {\displaystyle kT/q}  [kT/q] (approximately 26 mV
      at 300 K â room temperature).
    *     I  E     {\displaystyle I_{\text{E}}}  [I_{\text{E}}] is the emitter
      current
    *     I  C     {\displaystyle I_{\text{C}}}  [I_{\text{C}}] is the
      collector current
    *     &#x03B1;  F     {\displaystyle \alpha _{\text{F}}}  [{\displaystyle
      \alpha _{\text{F}}}] is the common base forward short-circuit current
      gain (0.98 to 0.998)
    *     I  ES     {\displaystyle I_{\text{ES}}}  [I_{\text{ES}}] is the
      reverse saturation current of the baseâemitter diode (on the order of
      10â15 to 10â12 amperes)
    *     V  BE     {\displaystyle V_{\text{BE}}}  [V_{\text{BE}}] is the
      baseâemitter voltage
    *     D  n     {\displaystyle D_{n}}  [D_{n}] is the diffusion constant for
      electrons in the p-type base
    * W is the base width
The     &#x03B1;   {\displaystyle \alpha }  [\alpha ] and forward     &#x03B2;
{\displaystyle \beta }  [\beta ] parameters are as described previously. A
reverse     &#x03B2;   {\displaystyle \beta }  [\beta ] is sometimes included
in the model.
The unapproximated Ebers–Moll equations used to describe the three currents in
any operating region are given below. These equations are based on the
transport model for a bipolar junction transistor.[28]
              i  C      =  I  S    [   (   e    V  BE    V  T      &#x2212;  e
      V  BC    V  T       )  &#x2212;   1  &#x03B2;  R      (   e    V  BC    V
      T      &#x2212; 1  )   ]       i  B      =  I  S    [    1  &#x03B2;  F
      (   e    V  BE    V  T      &#x2212; 1  )  +   1  &#x03B2;  R      (   e
      V  BC    V  T      &#x2212; 1  )   ]       i  E      =  I  S    [   (   e
      V  BE    V  T      &#x2212;  e    V  BC    V  T       )  +   1  &#x03B2;
      F      (   e    V  BE    V  T      &#x2212; 1  )   ]
      {\displaystyle {\begin{aligned}i_{\text{C}}&=I_{\text{S}}\left[\left(e^
      {\frac {V_{\text{BE}}}{V_{\text{T}}}}-e^{\frac {V_{\text{BC}}}{V_{\text
      {T}}}}\right)-{\frac {1}{\beta _{\text{R}}}}\left(e^{\frac {V_{\text
      {BC}}}{V_{\text{T}}}}-1\right)\right]\\i_{\text{B}}&=I_{\text{S}}\left[
      {\frac {1}{\beta _{\text{F}}}}\left(e^{\frac {V_{\text{BE}}}{V_{\text
      {T}}}}-1\right)+{\frac {1}{\beta _{\text{R}}}}\left(e^{\frac {V_{\text
      {BC}}}{V_{\text{T}}}}-1\right)\right]\\i_{\text{E}}&=I_{\text{S}}\left
      [\left(e^{\frac {V_{\text{BE}}}{V_{\text{T}}}}-e^{\frac {V_{\text{BC}}}
      {V_{\text{T}}}}\right)+{\frac {1}{\beta _{\text{F}}}}\left(e^{\frac {V_
      {\text{BE}}}{V_{\text{T}}}}-1\right)\right]\end{aligned}}}  [
      {\displaystyle {\begin{aligned}i_{\text{C}}&=I_{\text{S}}\left[\left(e^
      {\frac {V_{\text{BE}}}{V_{\text{T}}}}-e^{\frac {V_{\text{BC}}}{V_{\text
      {T}}}}\right)-{\frac {1}{\beta _{\text{R}}}}\left(e^{\frac {V_{\text
      {BC}}}{V_{\text{T}}}}-1\right)\right]\\i_{\text{B}}&=I_{\text{S}}\left[
      {\frac {1}{\beta _{\text{F}}}}\left(e^{\frac {V_{\text{BE}}}{V_{\text
      {T}}}}-1\right)+{\frac {1}{\beta _{\text{R}}}}\left(e^{\frac {V_{\text
      {BC}}}{V_{\text{T}}}}-1\right)\right]\\i_{\text{E}}&=I_{\text{S}}\left
      [\left(e^{\frac {V_{\text{BE}}}{V_{\text{T}}}}-e^{\frac {V_{\text{BC}}}
      {V_{\text{T}}}}\right)+{\frac {1}{\beta _{\text{F}}}}\left(e^{\frac {V_
      {\text{BE}}}{V_{\text{T}}}}-1\right)\right]\end{aligned}}}]
where
    *     i  C     {\displaystyle i_{\text{C}}}  [{\displaystyle i_{\text{C}}}]
      is the collector current
    *     i  B     {\displaystyle i_{\text{B}}}  [{\displaystyle i_{\text{B}}}]
      is the base current
    *     i  E     {\displaystyle i_{\text{E}}}  [{\displaystyle i_{\text{E}}}]
      is the emitter current
    *     &#x03B2;  F     {\displaystyle \beta _{\text{F}}}  [{\displaystyle
      \beta _{\text{F}}}] is the forward common emitter current gain (20 to
      500)
    *     &#x03B2;  R     {\displaystyle \beta _{\text{R}}}  [{\displaystyle
      \beta _{\text{R}}}] is the reverse common emitter current gain (0 to 20)
    *     I  S     {\displaystyle I_{\text{S}}}  [{\displaystyle I_{\text{S}}}]
      is the reverse saturation current (on the order of 10â15 to 10â12
      amperes)
    *     V  T     {\displaystyle V_{\text{T}}}  [{\displaystyle V_{\text{T}}}]
      is the thermal_voltage (approximately 26 mV at 300 K â room
      temperature).
    *     V  BE     {\displaystyle V_{\text{BE}}}  [{\displaystyle V_{\text
      {BE}}}] is the baseâemitter voltage
    *     V  BC     {\displaystyle V_{\text{BC}}}  [{\displaystyle V_{\text
      {BC}}}] is the baseâcollector voltage
** Base-width modulation[edit] **
Top: NPN base width for low collectorâbase reverse bias; Bottom: narrower NPN
base width for large collectorâbase reverse bias. Hashed regions are depleted
regions.
Main article: Early_effect
As the collectorâbase voltage (     V  CB   =  V  CE   &#x2212;  V  BE
{\displaystyle V_{\text{CB}}=V_{\text{CE}}-V_{\text{BE}}}  [{\displaystyle V_
{\text{CB}}=V_{\text{CE}}-V_{\text{BE}}}]) varies, the collectorâbase
depletion region varies in size. An increase in the collectorâbase voltage,
for example, causes a greater reverse bias across the collectorâbase
junction, increasing the collectorâbase depletion region width, and
decreasing the width of the base. This variation in base width often is called
the Early_effect after its discoverer James_M._Early.
Narrowing of the base width has two consequences:
    * There is a lesser chance for recombination within the "smaller" base
      region.
    * The charge gradient is increased across the base, and consequently, the
      current of minority carriers injected across the emitter junction
      increases.
Both factors increase the collector or "output" current of the transistor in
response to an increase in the collectorâbase voltage.
In the forward-active_region, the Early effect modifies the collector current
(     i  C     {\displaystyle i_{\text{C}}}  [{\displaystyle i_{\text{C}}}])
and the forward common emitter current gain (     &#x03B2;  F
{\displaystyle \beta _{\text{F}}}  [{\displaystyle \beta _{\text{F}}}]) as
given by:[citation_needed]
              i  C      =  I  S     e    v  BE    V  T       (  1 +    V  CE
      V  A      )       &#x03B2;  F      =  &#x03B2;   F  0    (  1 +    V  CB
      V  A      )       r  o      =    V  A    I  C           {\displaystyle
      {\begin{aligned}i_{\text{C}}&=I_{\text{S}}\,e^{\frac {v_{\text{BE}}}{V_
      {\text{T}}}}\left(1+{\frac {V_{\text{CE}}}{V_{\text{A}}}}\right)\\\beta _
      {\text{F}}&=\beta _{{\text{F}}0}\left(1+{\frac {V_{\text{CB}}}{V_{\text
      {A}}}}\right)\\r_{\text{o}}&={\frac {V_{\text{A}}}{I_{\text{C}}}}\end
      {aligned}}}  [{\displaystyle {\begin{aligned}i_{\text{C}}&=I_{\text
      {S}}\,e^{\frac {v_{\text{BE}}}{V_{\text{T}}}}\left(1+{\frac {V_{\text
      {CE}}}{V_{\text{A}}}}\right)\\\beta _{\text{F}}&=\beta _{{\text
      {F}}0}\left(1+{\frac {V_{\text{CB}}}{V_{\text{A}}}}\right)\\r_{\text
      {o}}&={\frac {V_{\text{A}}}{I_{\text{C}}}}\end{aligned}}}]
where:
    *     V  CE     {\displaystyle V_{\text{CE}}}  [{\displaystyle V_{\text
      {CE}}}] is the collectorâemitter voltage
    *     V  A     {\displaystyle V_{\text{A}}}  [{\displaystyle V_{\text{A}}}]
      is the Early voltage (15 V to 150 V)
    *     &#x03B2;   F  0     {\displaystyle \beta _{{\text{F}}0}}  [
      {\displaystyle \beta _{{\text{F}}0}}] is forward common-emitter current
      gain when      V  CB     {\displaystyle V_{\text{CB}}}  [{\displaystyle
      V_{\text{CB}}}] = 0 V
    *     r  o     {\displaystyle r_{\text{o}}}  [{\displaystyle r_{\text{o}}}]
      is the output impedance
    *     I  C     {\displaystyle I_{\text{C}}}  [{\displaystyle I_{\text{C}}}]
      is the collector current
** Punchthrough[edit] **
When the baseâcollector voltage reaches a certain (device-specific) value,
the baseâcollector depletion region boundary meets the baseâemitter
depletion region boundary. When in this state the transistor effectively has no
base. The device thus loses all gain when in this state.
*** GummelâPoon charge-control model[edit] ***
The GummelâPoon_model[29] is a detailed charge-controlled model of BJT
dynamics, which has been adopted and elaborated by others to explain transistor
dynamics in greater detail than the terminal-based models typically do.[30]
This model also includes the dependence of transistor     &#x03B2;
{\displaystyle \beta }  [\beta ]-values upon the direct current levels in the
transistor, which are assumed current-independent in the EbersâMoll model.
[31]
**** Small-signal models[edit] ****
*** Hybrid-pi model[edit] ***
Hybrid-pi model
Main article: hybrid-pi_model
The hybrid-pi model is a popular circuit model used for analyzing the small
signal and AC behavior of bipolar junction and field effect transistors.
Sometimes it is also called Giacoletto model because it was introduced by L.J.
Giacoletto in 1969. The model can be quite accurate for low-frequency circuits
and can easily be adapted for higher-frequency circuits with the addition of
appropriate inter-electrode capacitances and other parasitic elements.
*** h-parameter model[edit] ***
Generalized h-parameter model of an NPN BJT.
Replace x with e, b or c for CE, CB and CC topologies respectively.
Another model commonly used to analyze BJT circuits is the h-parameter model,
closely related to the hybrid-pi_model and the y-parameter two-port, but using
input current and output voltage as independent variables, rather than input
and output voltages. This two-port network is particularly suited to BJTs as it
lends itself easily to the analysis of circuit behaviour, and may be used to
develop further accurate models. As shown, the term, x, in the model represents
a different BJT lead depending on the topology used. For common-emitter mode
the various symbols take on the specific values as:
    * Terminal 1, base
    * Terminal 2, collector
    * Terminal 3 (common), emitter; giving x to be e
    * ii, base current (ib)
    * io, collector current (ic)
    * Vin, base-to-emitter voltage (VBE)
    * Vo, collector-to-emitter voltage (VCE)
and the h-parameters are given by:
    * hix = hie, the input impedance of the transistor (corresponding to the
      base resistance rpi).
    * hrx = hre, represents the dependence of the transistor's IB–VBE curve on
      the value of VCE. It is usually very small and is often neglected
      (assumed to be zero).
    * hfx = hfe, the current-gain of the transistor. This parameter is often
      specified as hFE or the DC current-gain (Î²DC) in datasheets.
    * hox = 1/hoe, the output impedance of transistor. The parameter hoe
      usually corresponds to the output admittance of the bipolar transistor
      and has to be inverted to convert it to an impedance.
As shown, the h-parameters have lower-case subscripts and hence signify AC
conditions or analyses. For DC conditions they are specified in upper-case. For
the CE topology, an approximate h-parameter model is commonly used which
further simplifies the circuit analysis. For this the hoe and hre parameters
are neglected (that is, they are set to infinity and zero, respectively). The
h-parameter model as shown is suited to low-frequency, small-signal analysis.
For high-frequency analyses the inter-electrode capacitances that are important
at high frequencies must be added.
** Etymology of hFE[edit] **
The h refers to its being an h-parameter, a set of parameters named for their
origin in a hybrid equivalent circuit model. F is from forward current
amplification also called the current gain. E refers to the transistor
operating in a common emitter (CE) configuration. Capital letters used in the
subscript indicate that hFE refers to a direct current circuit.
**** Industry models[edit] ****
[[icon]] This section needs expansion. You can help by adding_to_it. (January
         2015)
The GummelâPoon SPICE model is often used, but it suffers from several
limitations. These have been addressed in various more advanced models:
Mextram, VBIC, HICUM, Modella.[32][33][34][35]
***** Applications[edit] *****
The BJT remains a device that excels in some applications, such as discrete
circuit design, due to the very wide selection of BJT types available, and
because of its high transconductance and output resistance compared to MOSFETs.
The BJT is also the choice for demanding analog circuits, especially for very-
high-frequency applications, such as radio-frequency circuits for wireless
systems.
**** High-speed digital logic[edit] ****
Emitter-coupled_logic (ECL) use BJTs.
Bipolar transistors can be combined with MOSFETs in an integrated circuit by
using a BiCMOS process of wafer fabrication to create circuits that take
advantage of the application strengths of both types of transistor.
**** Amplifiers[edit] ****
Main article: Electronic_amplifier
The transistor_parameters Î± and Î² characterizes the current_gain of the BJT.
It is this gain that allows BJTs to be used as the building blocks of
electronic amplifiers. The three main BJT amplifier topologies are:
    * Common_emitter
    * Common_base
    * Common_collector
**** Temperature sensors[edit] ****
Main article: Silicon_bandgap_temperature_sensor
Because of the known temperature and current dependence of the forward-biased
baseâemitter junction voltage, the BJT can be used to measure temperature by
subtracting two voltages at two different bias currents in a known ratio.[36]
**** Logarithmic converters[edit] ****
Because baseâemitter voltage varies as the logarithm of the baseâemitter
and collectorâemitter currents, a BJT can also be used to compute logarithms
and anti-logarithms. A diode can also perform these nonlinear functions but the
transistor provides more circuit flexibility.
***** Vulnerabilities[edit] *****
Exposure of the transistor to ionizing_radiation causes radiation_damage.
Radiation causes a buildup of 'defects' in the base region that act as
recombination_centers. The resulting reduction in minority carrier lifetime
causes gradual loss of gain of the transistor.
Transistors have "maximum ratings", including power_ratings (essentially
limited by self-heating), maximum collector and base currents (both continuous/
DC ratings and peak), and breakdown_voltage ratings, beyond which the device
may fail or at least perform badly.
In addition to normal breakdown ratings of the device, power BJTs are subject
to a failure mode called secondary_breakdown, in which excessive current and
normal imperfections in the silicon die cause portions of the silicon inside
the device to become disproportionately hotter than the others. The electrical
resistivity of doped silicon, like other semiconductors, has a negative
temperature_coefficient, meaning that it conducts more current at higher
temperatures. Thus, the hottest part of the die conducts the most current,
causing its conductivity to increase, which then causes it to become
progressively hotter again, until the device fails internally. The thermal
runaway process associated with secondary breakdown, once triggered, occurs
almost instantly and may catastrophically damage the transistor package.
If the emitter-base junction is reverse biased into avalanche or Zener mode and
charge flows for a short period of time, the current gain of the BJT will be
permanently degraded.
***** See also[edit] *****
    * [icon]Electronics_portal
    * MOSFET
    * Bipolar_transistor_biasing
    * Gummel_plot
    * Technology_CAD (TCAD)
***** Notes[edit] *****
   1. ^ Some metals, such as aluminium have significant hole bands.[1]
   2. ^ See point-contact_transistor for the historical origin of these names.
***** References[edit] *****
   1. ^Ashcroft and Mermin (1976). Solid State Physics (1st ed.). Holt,
      Reinhart, and Winston. pp. 299â302. ISBN 978-0030839931.
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
   3. ^Chenming Calvin Hu (2010). Modern_Semiconductor_Devices_for_Integrated
      Circuits.
   4. ^ a b cPaul_Horowitz and Winfield_Hill (1989). The_Art_of_Electronics
      (2nd ed.). Cambridge University Press. ISBN 978-0-521-37095-0.
   5. ^Juin Jei Liou and Jiann S. Yuan (1998). Semiconductor_Device_Physics_and
      Simulation. Springer. ISBN 978-0-306-45724-1.
   6. ^General Electric (1962). Transistor Manual (6th ed.). p. 12.
   7.  "If the principle of space charge neutrality is used in the analysis of
      the transistor, it is evident that the collector current is controlled by
      means of the positive charge (hole concentration) in the base region. ...
      When a transistor is used at higher frequencies, the fundamental
      limitation is the time it takes the carriers to diffuse across the base
      region..." (same in 4th and 5th editions).
   8. ^Paolo Antognetti and Giuseppe Massobrio (1993). Semiconductor_Device
      Modeling_with_Spice. McGraw–Hill Professional. ISBN 978-0-07-134955-0.
   9. ^ D.V. Morgan, Robin H. Williams (Editors) (1991). Physics_and_Technology
      of_Heterojunction_Devices. London: Institution of Electrical Engineers
      (Peter Peregrinus Ltd.). ISBN 978-0-86341-204-2.CS1 maint: Extra text:
      authors list (link)
  10. ^Peter Ashburn (2003). SiGe_Heterojunction_Bipolar_Transistors. New York:
      Wiley. Chapter 10. ISBN 978-0-470-84838-8.
  11. ^ Paul_Horowitz and Winfield_Hill (1989). The_Art_of_Electronics (2nd
      ed.). Cambridge University Press. pp. 62â66. ISBN 978-0-521-37095-0.
  12. ^"1947:_Invention_of_the_Point-Contact_Transistor_-_The_Silicon_Engine_-
      Computer_History_Museum". Retrieved August 10, 2016.
  13. ^"1948:_Conception_of_the_Junction_Transistor_-_The_Silicon_Engine_-
      Computer_History_Museum". Retrieved August 10, 2016.
  14. ^ Third_case_study_â_the_solid_state_advent Archived September 27,
      2007, at the Wayback_Machine (PDF)
  15. ^
      Transistor_Museum,_Historic_Transistor_Photo_Gallery,_Bell_Labs_Type
      M1752
  16. ^Morris, Peter Robin (1990). "4.2". A History of the World Semiconductor
      Industry. IEE History of Technology Series 12. London: Peter Peregrinus
      Ltd. p. 29. ISBN 978-0-86341-227-1.
  17. ^"Transistor_Museum_Photo_Gallery_RCA_TA153". Retrieved August 10, 2016.
  18. ^High Speed Switching Transistor Handbook (2nd ed.). Motorola. 1963.
      p. 17.
  19. [1]
  20. ^
      Transistor_Museum,_Historic_Transistor_Photo_Gallery,_Western_Electric
      3N22
  21. ^ The_Tetrode_Power_Transistor PDF
  22. ^"Transistor_Museum_Photo_Gallery_Philco_A01_Germanium_Surface_Barrier
      Transistor". Retrieved August 10, 2016.
  23. ^"Transistor_Museum_Photo_Gallery_Germanium_Surface_Barrier_Transistor".
      Retrieved August 10, 2016.
  24. ^ Herbâs_Bipolar_Transistors_IEEE_Transactions_on_Electron_Devices,
      vol._48,_no._11,_November_2001 PDF
  25. ^ Influence_of_Mobility_and_Lifetime_Variations_on_Drift-Field_Effects_in
      Silicon-Junction_Devices PDF
  26. ^"Transistor_Museum_Photo_Gallery_Bell_Labs_Prototype_Diffused_Base
      Germanium_Silicon_Transistor". Retrieved August 10, 2016.
  27. ^"Transistor_Museum_Photo_Gallery_Fairchild_2N1613_Early_Silicon_Planar
      Transistor". Retrieved August 10, 2016.
  28. ^"1960:_Epitaxial_Deposition_Process_Enhances_Transistor_Performance_-
      The_Silicon_Engine_-_Computer_History_Museum". Retrieved August 10, 2016.
  29. ^ J.J. Ebers and J.L Moll (1954) "Large-signal behavior of junction
      transistors", Proceedings of the Institute of Radio Engineers, 42 (12) :
      1761â1772.
  30. ^ Adel S. Sedra and Kenneth C. Smith (1987). Microelectronic Circuits,
      second ed. p. 903. ISBN 978-0-03-007328-1.
  31. ^ A.S. Sedra and K.C. Smith (2004). Microelectronic Circuits (5th ed.).
      New York: Oxford. Eqs.&nbsp, 4.103â4.110, p.&nbsp, 305. ISBN 978-0-19-
      514251-8.
  32. ^ H. K. Gummel and R. C. Poon, "An integral charge control model of
      bipolar transistors", Bell Syst. Tech. J., vol. 49, pp. 827â852,
      MayâJune 1970
  33. ^"Bipolar_Junction_Transistors". Retrieved August 10, 2016.
  34. ^ A.S. Sedra and K.C. Smith (2004). Microelectronic Circuits (5th ed.).
      New York: Oxford. p. 509. ISBN 978-0-19-514251-8.
  35. ^ http://www.silvaco.com/content/kbase/smartspice_device_models.pdf
  36. ^Gennady Gildenblat, ed. (2010). Compact Modeling: Principles, Techniques
      and Applications. Springer Science & Business Media. Part II: Compact
      Models of Bipolar Junction Transistors, pp. 167-267 cover Mextram and
      HiCuM in-depth. ISBN 978-90-481-8614-3.
  37. ^Michael SchrÃ¶ter (2010). Compact Hierarchical Bipolar Transistor
      Modeling with Hicum. World Scientific. ISBN 978-981-4273-21-3.
  38. ^ http://joerg-berkner.de/Fachartikel/pdf/
      2002_ICCAP_UM_Berkner_Compact_Models_4_BJTs.pdf
  39. ^"IC_Temperature_Sensors_Find_the_Hot_Spots_-_Application_Note_-_Maxim".
      maxim-ic.com. February 21, 2002. Retrieved August 10, 2016.
***** External links[edit] *****
 Wikimedia Commons has media related to Bipolar_junction_transistors.
 This section's use of external_links may not follow Wikipedia's policies or
 guidelines. Please improve_this_article by removing excessive or inappropriate
 external links, and converting useful links where appropriate into footnote
 references. (July 2012)(Learn_how_and_when_to_remove_this_template_message)
    * Lessons_In_Electric_Circuits –_Bipolar_Junction_Transistors (Note: this
      site shows current as a flow of electrons, rather than the convention_of
      showing_it_as_a_flow_of_holes)
    * EncycloBEAMia –_Bipolar_Junction_Transistor
    * Characteristic_curves
    * ENGI_242/ELEC_222:_BJT_Small_Signal_Models
    * Transistor_Museum,_Historic_Transistor_Timeline
    * ECE_327:_Transistor_Basics â Summarizes simple Ebers–Moll model of a
      bipolar transistor and gives several common BJT circuits.
    * ECE_327:_Procedures_for_Output_Filtering_Lab â Section 4 ("Power
      Amplifier") discusses design of a BJT-Sziklai-pair-based class-AB current
      driver in detail.
    * BJT_Operation_description for undergraduate and first year graduate
      students to describe the basic principles of operation of Bipolar
      Junction Transistor.
    * v
    * t
    * e
Transistor amplifiers
            Bipolar junction          * Common_emitter
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
                                         * Bipolar junction transistor (BJT)
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
Authority_control [Edit_this_at_Wikidata]     * GND: 4145669-5

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Bipolar_junction_transistor&oldid=908416565"
Categories:
    * Transistor_modeling
    * Transistor_types
    * Bipolar_transistors
Hidden categories:
    * CS1_maint:_Extra_text:_authors_list
    * Webarchive_template_wayback_links
    * Wikipedia_articles_that_are_too_technical_from_July_2012
    * All_articles_that_are_too_technical
    * Articles_needing_expert_attention_from_July_2012
    * All_articles_needing_expert_attention
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_November_2007
    * Articles_to_be_expanded_from_January_2015
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
    * Commons_category_link_is_on_Wikidata
    * Wikipedia_external_links_cleanup_from_July_2012
    * Wikipedia_spam_cleanup_from_July_2012
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
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
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * Jawa
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Latina
    * LatvieÅ¡u
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * Simple_English
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ä¸­æ
Edit_links
    * This page was last edited on 29 July 2019, at 15:46 (UTC).
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
