The following text has been accessed from https://en.wikipedia.org/wiki/Thyristor at Thu Aug 8 22:49:05 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Thyristor ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
                Thyristor
[SCR1369.jpg]
Thyristor
Type              Passive
First production  1956
Pin configuration anode, gate and cathode
Electronic_symbol
[Thyristor_circuit_symbol.svg]
A thyristor (/Î¸aÉªËrÉªstÉr/) is a solid-state semiconductor_device with four
layers of alternating P- and N-type materials. It acts exclusively as a
bistable switch, conducting when the gate receives a current trigger, and
continuing to conduct until the voltage across the device is reversed biased,
or until the voltage is removed (by some other means). A three-lead thyristor
is designed to control the larger current of the Anode to Cathode path by
controlling that current with the smaller current of its other lead, known as
its Gate. In contrast, a two-lead thyristor is designed to switch on if the
potential difference between its leads is sufficiently large (breakdown
voltage).
Some sources define silicon-controlled_rectifier (SCR) and thyristor as
synonymous.[1] Other sources define thyristors as more ornately constructed
devices that incorporate at least four layers of alternating N-type and P-type
substrate.
The first thyristor devices were released commercially in 1956. Because
thyristors can control a relatively large amount of power and voltage with a
small device, they find wide application in control of electric power, ranging
from light dimmers and electric motor speed control to high-voltage_direct-
current power transmission. Thyristors may be used in power-switching circuits,
relay-replacement circuits, inverter circuits, oscillator circuits, level-
detector circuits, chopper circuits, light-dimming circuits, low-cost timer
circuits, logic circuits, speed-control circuits, phase-control circuits, etc.
Originally, thyristors relied only on current reversal to turn them off, making
them difficult to apply for direct current; newer device types can be turned on
and off through the control gate signal. The latter is known as a gate_turn-off
thyristor, or GTO thyristor. A thyristor is not a proportional device like a
transistor. In other words, a thyristor can only be fully on or off, while a
transistor can lie in between on and off states. This makes a thyristor
unsuitable as an analog amplifier, but useful as a switch.
⁰
***** Contents *****
    * 1_Introduction
          o 1.1_Function_of_the_gate_terminal
          o 1.2_Switching_characteristics
    * 2_History
          o 2.1_Etymology
    * 3_Applications
          o 3.1_Snubber_circuits
          o 3.2_HVDC_electricity_transmission
    * 4_Comparisons_to_other_devices
    * 5_Failure_modes
    * 6_Silicon_carbide_thyristors
    * 7_Types
          o 7.1_Reverse_conducting_thyristor
          o 7.2_Photothyristors
    * 8_See_also
    * 9_References
    * 10_Sources
    * 11_External_links
***** Introduction[edit] *****
The thyristor is a four-layered, three-terminal semiconductor device, with each
layer consisting of alternately N-type or P-type material, for example P-N-P-N.
The main terminals, labelled anode and cathode, are across all four layers. The
control terminal, called the gate, is attached to p-type material near the
cathode. (A variant called an SCSâsilicon controlled switchâbrings all four
layers out to terminals.) The operation of a thyristor can be understood in
terms of a pair of tightly coupled bipolar_junction_transistors, arranged to
cause a self-latching action:
      Structure on the physical and electronic level, and the thyristor symbol.
Thyristors have three states:
   1. Reverse blocking mode â Voltage is applied in the direction that would
      be blocked by a diode
   2. Forward blocking mode â Voltage is applied in the direction that would
      cause a diode to conduct, but the thyristor has not been triggered into
      conduction
   3. Forward conducting mode â The thyristor has been triggered into
      conduction and will remain conducting until the forward current drops
      below a threshold value known as the "holding current"
**** Function of the gate terminal[edit] ****
The thyristor has three p-n_junctions (serially named J1, J2, J3 from the
anode).
Layer diagram of thyristor.
When the anode is at a positive potential VAK with respect to the cathode with
no voltage applied at the gate, junctions J1 and J3 are forward biased, while
junction J2 is reverse biased. As J2 is reverse biased, no conduction takes
place (Off state). Now if VAK is increased beyond the breakdown voltage VBO of
the thyristor, avalanche_breakdown of J2 takes place and the thyristor starts
conducting (On state).
If a positive potential VG is applied at the gate terminal with respect to the
cathode, the breakdown of the junction J2 occurs at a lower value of VAK. By
selecting an appropriate value of VG, the thyristor can be switched into the on
state quickly.
Once avalanche breakdown has occurred, the thyristor continues to conduct,
irrespective of the gate voltage, until: (a) the potential VAK is removed or
(b) the current through the device (anodeâcathode) becomes less than the
holding current specified by the manufacturer. Hence VG can be a voltage pulse,
such as the voltage output from a UJT relaxation_oscillator.
The gate pulses are characterized in terms of gate trigger voltage (VGT) and
gate trigger current (IGT). Gate trigger current varies inversely with gate
pulse width in such a way that it is evident that there is a minimum gate
charge required to trigger the thyristor.
**** Switching characteristics[edit] ****
V â I characteristics.
In a conventional thyristor, once it has been switched on by the gate terminal,
the device remains latched in the on-state (i.e. does not need a continuous
supply of gate current to remain in the on state), providing the anode current
has exceeded the latching current (IL). As long as the anode remains positively
biased, it cannot be switched off until the anode current falls below the
holding current (IH). In normal working condition the latching current is
always greater than holding current. In the above figure IL has to come above
the IH on y-axis since IL>IH.
A thyristor can be switched off if the external circuit causes the anode to
become negatively biased (a method known as natural, or line, commutation). In
some applications this is done by switching a second thyristor to discharge a
capacitor into the cathode of the first thyristor. This method is called forced
commutation.
After the current in a thyristor has extinguished, a finite time delay must
elapse before the anode can again be positively biased and retain the thyristor
in the off-state. This minimum delay is called the circuit commutated turn off
time (tQ). Attempting to positively bias the anode within this time causes the
thyristor to be self-triggered by the remaining charge carriers (holes and
electrons) that have not yet recombined.
For applications with frequencies higher than the domestic AC mains supply
(e.g. 50 Hz or 60 Hz), thyristors with lower values of tQ are required. Such
fast thyristors can be made by diffusing heavy_metal ions such as gold or
platinum which act as charge combination centers into the silicon. Today, fast
thyristors are more usually made by electron or proton irradiation of the
silicon, or by ion_implantation. Irradiation is more versatile than heavy metal
doping because it permits the dosage to be adjusted in fine steps, even at
quite a late stage in the processing of the silicon.
***** History[edit] *****
The silicon controlled rectifier (SCR) or thyristor proposed by William
Shockley in 1950 and championed by Moll and others at Bell_Labs was developed
in 1956 by power engineers at General_Electric (G.E.), led by Gordon Hall and
commercialized by G.E.'s Frank W. "Bill" Gutzwiller. The Institute_of
Electrical_and_Electronics_Engineers recognized the invention by placing a
plaque at the invention site in Clyde, NY and declaring it an IEEE Historic
Milestone.
A bank of six 2000 A thyristors (white disks arranged in a row at top, and seen
edge-on)
**** Etymology[edit] ****
An earlier gas-filled_tube device called a thyratron provided a similar
electronic switching capability, where a small control voltage could switch a
large current. It is from a combination of "thyratron" and "transistor" that
the term "thyristor" is derived.[2]
***** Applications[edit] *****
Waveforms in a rectified multiple thyristor circuit controlling an AC current.
Red trace: load (output) voltage
Blue trace: trigger voltage.
Thyristors are mainly used where high currents and voltages are involved, and
are often used to control alternating_currents, where the change of polarity of
the current causes the device to switch off automatically, referred to as "zero
cross" operation. The device can be said to operate synchronously; being that,
once the device is triggered, it conducts current in phase with the voltage
applied over its cathode to anode junction with no further gate modulation
being required, i.e., the device is biased fully on. This is not to be confused
with asymmetrical operation, as the output is unidirectional, flowing only from
cathode to anode, and so is asymmetrical in nature.
Thyristors can be used as the control elements for phase angle triggered
controllers, also known as phase_fired_controllers.
They can also be found in power supplies for digital_circuits, where they are
used as a sort of "enhanced circuit_breaker" to prevent a failure in the power
supply from damaging downstream components. A thyristor is used in conjunction
with a Zener_diode attached to its gate, and if the output voltage of the
supply rises above the Zener voltage, the thyristor will conduct and short-
circuit the power supply output to ground (in general also tripping an upstream
breaker or fuse). This kind of protection circuit is known as a crowbar, and
has the advantage over a standard circuit breaker or fuse in that it creates a
high-conductance path to ground for the damaging supply voltage and potentially
for stored energy in the system being powered.
The first large-scale application of thyristors, with associated triggering
diac, in consumer products related to stabilized power supplies within color
television receivers in the early 1970s.[clarification_needed] The stabilized
high voltage DC supply for the receiver was obtained by moving the switching
point of the thyristor device up and down the falling slope of the positive
going half of the AC supply input (if the rising slope was used the output
voltage would always rise towards the peak input voltage when the device was
triggered and thus defeat the aim of regulation). The precise switching point
was determined by the load on the DC output supply, as well as AC input
fluctuations.
Thyristors have been used for decades as light dimmers in television, motion
pictures, and theater, where they replaced inferior technologies such as
autotransformers and rheostats. They have also been used in photography as a
critical part of flashes (strobes).
**** Snubber circuits[edit] ****
Thyristors can be triggered by a high rise-rate of off-state voltage. This is
prevented by connecting a resistor-capacitor (RC) snubber circuit between the
anode and cathode in order to limit the dV/dt (i.e., rate of voltage change
over time). Snubbers are energy-absorbing circuits used to suppress the voltage
spikes caused by the circuit's inductance when a switch, electrical or
mechanical, opens. The most common snubber circuit is a capacitor and resistor
connected in series across the switch (transistor).
**** HVDC electricity transmission[edit] ****
Valve_hall containing thyristor_valve stacks used for long-distance
transmission of power from Manitoba_Hydro dams
Since modern thyristors can switch power on the scale of megawatts, thyristor
valves have become the heart of high-voltage_direct_current (HVDC) conversion
either to or from alternating current. In the realm of this and other very
high-power applications, both electrically triggered (ETT) and light-triggered
(LTT) thyristors[3][4] are still the primary choice. The valves are arranged in
stacks usually suspended from the ceiling of a transmission building called a
valve_hall. Thyristors are arranged into a diode_bridge circuit and to reduce
harmonics are connected in series to form a 12-pulse_converter. Each thyristor
is cooled with deionized_water, and the entire arrangement becomes one of
multiple identical modules forming a layer in a multilayer valve stack called a
quadruple valve. Three such stacks are typically mounted on the floor or hung
from the ceiling of the valve hall of a long-distance transmission facility.[5]
[6]
***** Comparisons to other devices[edit] *****
The functional drawback of a thyristor is that, like a diode, it only conducts
in one direction. A similar self-latching 5-layer device, called a TRIAC, is
able to work in both directions. This added capability, though, also can become
a shortfall. Because the TRIAC can conduct in both directions, reactive loads
can cause it to fail to turn off during the zero-voltage instants of the AC
power cycle. Because of this, use of TRIACs with (for example) heavily
inductive motor loads usually requires the use of a "snubber" circuit around
the TRIAC to assure that it will turn off with each half-cycle of mains power.
Inverse_parallel SCRs can also be used in place of the triac; because each SCR
in the pair has an entire half-cycle of reverse polarity applied to it, the
SCRs, unlike TRIACs, are sure to turn off. The "price" to be paid for this
arrangement, however, is the added complexity of two separate, but essentially
identical gating circuits.
Although thyristors are heavily used in megawatt-scale rectification of AC to
DC, in low- and medium-power (from few tens of watts to few tens of kilowatts)
applications they have virtually been replaced by other devices with superior
switching characteristics like Power_MOSFETs or IGBTs. One major problem
associated with SCRs is that they are not fully controllable switches. The GTO
thyristor and IGCT are two devices related to the thyristor that address this
problem. In high-frequency applications, thyristors are poor candidates due to
long switching times arising from bipolar conduction. MOSFETs, on the other
hand, have much faster switching capability because of their unipolar
conduction (only majority_carriers carry the current).
***** Failure modes[edit] *****
Thyristor manufacturers generally specify a region of safe firing defining
acceptable levels of voltage and current for a given operating_temperature. The
boundary of this region is partly determined by the requirement that the
maximum permissible gate power (PG), specified for a given trigger pulse
duration, is not exceeded.[7]
As well as the usual failure modes due to exceeding voltage, current or power
ratings, thyristors have their own particular modes of failure, including:
    * Turn on di/dt â in which the rate of rise of on-state current after
      triggering is higher than can be supported by the spreading speed of the
      active conduction area (SCRs & triacs).
    * Forced commutation â in which the transient peak reverse recovery
      current causes such a high voltage drop in the sub-cathode region that it
      exceeds the reverse breakdown voltage of the gate cathode diode junction
      (SCRs only).
    * Switch on dv/dt â the thyristor can be spuriously fired without trigger
      from the gate if the anode-to-cathode voltage rise-rate is too great.
***** Silicon carbide thyristors[edit] *****
In recent years, some manufacturers[8] have developed thyristors using silicon
carbide (SiC) as the semiconductor material. These have applications in high
temperature environments, being capable of operating_at_temperatures up to
350 Â°C.
***** Types[edit] *****
    * ACS
    * ACST
    * AGT â Anode Gate Thyristor â A thyristor with gate on n-type layer
      near to the anode
    * ASCR â Asymmetrical SCR
    * BCT â Bidirectional Control Thyristor â A bidirectional switching
      device containing two thyristor structures with separate gate contacts
    * BOD â Breakover Diode â A gateless thyristor triggered by avalanche
      current
          o DIAC â Bidirectional trigger device
          o Dynistor â Unidirectional switching device
          o Shockley_diode â Unidirectional trigger and switching device
          o SIDAC â Bidirectional switching device
          o Trisil, SIDACtor â Bidirectional protection devices
    * BRT â Base Resistance Controlled Thyristor
    * ETO â Emitter Turn-Off Thyristor[9]
    * GTO â Gate Turn-Off thyristor
          o DB-GTO â Distributed buffer gate turn-off thyristor
          o MA-GTO â Modified anode gate turn-off thyristor
    * IGCT â Integrated gate-commutated thyristor
    * Ignitor â Spark generators for fire-lighter ckts
    * LASCR â Light-activated SCR, or LTT â light-triggered thyristor
    * LASS â light-activated semiconducting switch
    * MCT â MOSFET Controlled Thyristor â It contains two additional FET
      structures for on/off control.
    * CSMT or MCS â MOS composite static induction thyristor
    * PUT or PUJT â Programmable Unijunction Transistor â A thyristor with
      gate on n-type layer near to the anode used as a functional replacement
      for unijunction_transistor
    * RCT â Reverse Conducting Thyristor
    * SCS â Silicon Controlled Switch or Thyristor Tetrode â A thyristor
      with both cathode and anode gates
    * SCR â Silicon Controlled Rectifier
    * SITh â Static Induction Thyristor, or FCTh â Field Controlled
      Thyristor â containing a gate structure that can shut down anode
      current flow.
    * TRIAC â Triode for Alternating Current â A bidirectional switching
      device containing two thyristor structures with common gate contact
    * Quadrac â special type of thyristor which combines a DIAC and a TRIAC
      into a single package.
**** Reverse conducting thyristor[edit] ****
A reverse conducting thyristor (RCT) has an integrated reverse diode, so is not
capable of reverse blocking. These devices are advantageous where a reverse or
freewheel diode must be used. Because the SCR and diode never conduct at the
same time they do not produce heat simultaneously and can easily be integrated
and cooled together. Reverse conducting thyristors are often used in frequency
changers and inverters.
**** Photothyristors[edit] ****
Electronic_symbol for light-activated SCR (LASCR)
Photothyristors are activated by light. The advantage of photothyristors is
their insensitivity to electrical signals, which can cause faulty operation in
electrically noisy environments. A light-triggered thyristor (LTT) has an
optically sensitive region in its gate, into which electromagnetic_radiation
(usually infrared) is coupled by an optical_fiber. Since no electronic boards
need to be provided at the potential of the thyristor in order to trigger it,
light-triggered thyristors can be an advantage in high-voltage applications
such as HVDC. Light-triggered thyristors are available with in-built over-
voltage (VBO) protection, which triggers the thyristor when the forward voltage
across it becomes too high; they have also been made with in-built forward
recovery protection, but not commercially. Despite the simplification they can
bring to the electronics of an HVDC valve, light-triggered thyristors may still
require some simple monitoring electronics and are only available from a few
manufacturers.
Two common photothyristors include the light-activated SCR (LASCR) and the
light-activated TRIAC. A LASCR acts as a switch that turns on when exposed to
light. Following light exposure, when light is absent, if the power is not
removed and the polarities of the cathode and anode have not yet reversed, the
LASCR is still in the "on" state. A light-activated TRIAC resembles a LASCR,
except that it is designed for alternating currents.
***** See also[edit] *****
    * [icon]Electronics_portal
    * Latchup
    * Quadrac
    * Thyristor_drive
    * Valve_hall
    * Thyratron
    * Insulated-gate_bipolar_transistor
***** References[edit] *****
   1. ^ Christiansen, Donald; Alexander, Charles K. (2005); Standard Handbook
      of Electrical Engineering (5th edition.). McGraw-Hill,
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
   3. ISBN 0-07-138421-9
   4. ^ [1] Archived September 5, 2012, at the Wayback_Machine
   5. ^"Chapter 5.1". High_Voltage_Direct_Current_Transmission_â_Proven
      Technology_for_Power_Exchange (PDF). Siemens. Retrieved 2013-08-04.
   6. ^"ETT_vs._LTT_for_HVDC" (PDF). ABB_Asea_Brown_Boveri. Retrieved 2014-01-
      24.
   7. ^"HVDC_Thyristor_Valves". ABB_Asea_Brown_Boveri. Archived from the
      original on January 22, 2009. Retrieved 2008-12-20.
   8. ^"High_Power". IET. Archived from the_original on September 10, 2009.
      Retrieved 2009-07-12.
   9. ^ "Safe_Firing_of_Thyristors" on powerguru.org
  10. ^ Example: Silicon_Carbide_Inverter_Demonstrates_Higher_Power_Output in
      Power Electronics Technology (2006-02-01)
  11. ^ Rashid, Muhammad H.(2011); Power Electronics (3rd ed.). Pearson,
  12. ISBN 978-81-317-0246-8
***** Sources[edit] *****
    * Wintrich, Arendt; Nicolai, Ulrich; Tursky, Werner; Reimann, Tobias
      (2011). Application_Manual_Power_Semiconductors_2011 (PDF) (2nd ed.).
      Nuremberg: Semikron. ISBN 978-3-938843-66-6. Archived from the_original
      (PDF) on 2013-09-16.
Thyristor Theory and Design Considerations; ON Semiconductor; 240 pages; 2006;
HBD855/D. (Free_PDF_download)
Ulrich Nicolai, Tobias Reimann, JÃ¼rgen Petzoldt, Josef Lutz: Application
Manual IGBT and MOSFET Power Modules, 1. Edition, ISLE Verlag, 1998,
ISBN 3-932633-24-5. (Free_PDF_download)
SCR Manual; 6th edition; General Electric Corporation; Prentice-Hall; 1979.
***** External links[edit] *****
 Wikimedia Commons has media related to Thyristors.
 Look up thyristor in Wiktionary, the free dictionary.
    * The_Early_History_of_the_Silicon_Controlled_Rectifier â by Frank
      William Gutzwiller (of G.E.)
    * THYRISTORS â from All About Circuits
    * Universal_thyristor_driving_circuit
    * Thyristor_Resources_(simpler_explanation)
    * Thyristors_of_STMicroelectronics
    * Thyristor_basics
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
Authority_control [Edit_this_at_Wikidata]     * GND: 4060020-8

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Thyristor&oldid=907460764"
Categories:
    * Electric_power_systems_components
    * High-voltage_direct_current
    * Power_electronics
    * Solid_state_switches
Hidden categories:
    * Webarchive_template_wayback_links
    * Wikipedia_articles_needing_clarification_from_April_2015
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
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * Hrvatski
    * Italiano
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * OÊ»zbekcha/ÑÐ·Ð±ÐµÐºÑÐ°
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Shqip
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ä¸­æ
Edit_links
    * This page was last edited on 23 July 2019, at 02:09 (UTC).
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
