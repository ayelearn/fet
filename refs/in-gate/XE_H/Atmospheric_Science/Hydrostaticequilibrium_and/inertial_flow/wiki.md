The following text has been accessed from https://en.wikipedia.org/wiki/Balanced_flow#Inertial_flow at Fri Aug 9 01:59:41 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Balanced flow ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article needs additional citations for verification. Please help improve_this_article by
 adding_citations_to_reliable_sources. Unsourced material may be challenged and removed.
 Find sources: "Balanced_flow" â news Â· newspapers Â· books Â· scholar Â· JSTOR (September
 2018)(Learn_how_and_when_to_remove_this_template_message)
In atmospheric_science, balanced flow is an idealisation of atmospheric motion.
The idealisation consists in considering the behaviour of one isolated parcel
of air having constant density, its motion on a horizontal plane subject to
selected forces acting on it and, finally, steady-state conditions.
Balanced flow is often an accurate approximation of the actual flow, and is
useful in improving the qualitative understanding and interpretation of
atmospheric motion. In particular, the balanced-flow speeds can be used as
estimates of the wind speed for particular arrangements of the atmospheric
pressure on Earth's surface.
⁰
***** Contents *****
    * 1_The_Momentum_Equations_in_Natural_Coordinates
          o 1.1_Trajectories
          o 1.2_Kinematics
          o 1.3_Forces
          o 1.4_Governing_equations
          o 1.5_Steady-state_assumption
    * 2_General_framework
          o 2.1_The_schematisations
          o 2.2_The_limitations
                # 2.2.1_Vertical_differences_of_air_properties
                # 2.2.2_Horizontal_differences_of_air_properties
                # 2.2.3_Unsteadiness
    * 3_Antitriptic_flow
          o 3.1_Formulation
          o 3.2_Application
    * 4_Geostrophic_flow
          o 4.1_Formulation
          o 4.2_Application
    * 5_Cyclostrophic_flow
          o 5.1_Formulation
          o 5.2_Application
    * 6_Inertial_flow
          o 6.1_Formulation
          o 6.2_Application
    * 7_Gradient_flow
          o 7.1_Formulation
                # 7.1.1_Pressure_lows_and_cyclones
                # 7.1.2_Pressure_highs_and_anticyclones
          o 7.2_Application
    * 8_Balanced-flow_speeds_compared
    * 9_See_also
    * 10_References
    * 11_Further_reading
    * 12_External_links
***** The Momentum Equations in Natural Coordinates[edit] *****
**** Trajectories[edit] ****
The momentum equations are written primarily for the generic trajectory of a
packet of flow travelling on a horizontal plane and taken at a certain elapsed
time called t. The position of the packet is defined by the distance on the
trajectory s=s(t) which it has travelled by time t. In reality, however, the
trajectory is the outcome of the balance of forces upon the particle. In this
section we assume to know it from the start for convenience of representation.
When we consider the motion determined by the forces selected next, we will
have clues of which type of trajectory fits the particular balance of forces.
The trajectory at a position s has one tangent unit vector s that invariably
points in the direction of growing sâs, as well as one unit vector n,
perpendicular to s, that points towards the local centre of curvature O. The
centre of curvature is found on the 'inner side' of the bend, and can shift
across either side of the trajectory according to the shape of it. The distance
between the parcel position and the centre of curvature is the radius of
curvature R at that position. The radius of curvature approaches an infinite
length at the points where the trajectory becomes straight and the positive
orientation of n is not determined in this particular case (discussed in
geostrophic_flows). The frame of reference (s,n) is shown by the red arrows in
the figure. This frame is termed natural or intrinsic because the axes
continuously adjust to the moving parcel, and so they are the most closely
connected to its fate.
[Trajectory.jpg]
**** Kinematics[edit] ****
The velocity vector (V) is oriented like s and has intensity (speed) V = ds/dt.
This speed is always a positive quantity, since any parcel moves along its own
trajectory and, for increasing times (dt>0), the trodden length increases as
well (ds>0).
The acceleration vector of the parcel is decomposed in the tangential
acceleration parallel to s and in the centripetal acceleration along positive
n. The tangential acceleration only changes the speed V and is equal to DV/Dt,
where big d's denote the material_derivative. The centripetal acceleration
always points towards the centre of curvature O and only changes the direction
s of the forward displacement while the parcel moves on.
**** Forces[edit] ****
In the balanced-flow idealization we consider a three-way balance of forces
that are:
    * Pressure force. This is the action on the parcel arising from the spatial
      differences of atmospheric pressure p around it. (Temporal changes are of
      no interest here.) The spatial change of pressure is visualised through
      isobars, that are contours joining the locations where the pressure has a
      same value. In the figure this is simplistically shown by equally spaced
      straight lines. The pressure force acting on the parcel is minus the
      gradient vector of p (in symbols: grad p) â drawn in the figure as a
      blue arrow. At all points, the pressure gradient points to the direction
      of maximum increase of p and is always normal to the isobar at that
      point. Since the flow packet feels a push from the higher to the lower
      pressures, the effective pressure vector force is contrary to the
      pressure gradient, whence the minus sign before the gradient vector.
    * Friction. This is a force always opposing the forward motion, whereby the
      vector invariably acts in the negative direction s with an effect to
      reduce the speed. The friction at play in the balanced-flow models is the
      one exerted by the roughness of the Earth's surface on the air moving
      higher above. For simplicity, we here assume that the frictional force
      (per unit mass) adjusts to the parcel's speed proportionally through a
      constant coefficient_of_friction K. In more realistic conditions, the
      dependence of friction on the speed is non-linear except for slow laminar
      flows.
    * Coriolis_force. This action, due to the Earth's rotation, tends to
      displace any body travelling in the northern (southern) hemisphere
      towards its right (left). Its intensity per unit mass is proportional to
      the speed V and increases in magnitude from the equator (where it is
      zero) towards the poles proportionally to the local Coriolis_frequency f
      (a positive number north of the equator and negative south). Therefore,
      the Coriolis vector invariably points sideways, that is along the n axis.
      Its sign in the balance equation may change, since the positive
      orientation of n flips between right and left of the trajectory based
      solely on its curvature, while the Coriolis vector points to either side
      based on the packet's position on the Earth. The exact expression of the
      Coriolis force is a bit more complex than the product of the Coriolis
      parameter and parcel's velocity. However, this approximation is
      consistent with having neglected the curvature of the Earth's surface.
In the fictitious situation drawn in the figure, the pressure force pushes the
parcel forward along the trajectory and inward with respect to the bend; the
Coriolis force pushes inwards (outwards) of the bend in the northern (southern)
hemisphere; and friction pulls (necessarily) rearwards.
**** Governing equations[edit] ****
For the dynamical_equilibrium_of_the_parcel, either component of acceleration
times the parcel's mass is equal to the components of the external forces
acting in the same direction. As the equations of equilibrium for the parcel
are written in natural coordinates, the component equations for the horizontal
momentum per unit mass are expressed as follows:
      D V   D t    = &#x2212;   1 &#x03C1;      &#x2202; p   &#x2202; s
&#x2212; K V   {\displaystyle {\frac {DV}{Dt}}=-{\frac {1}{\rho }}{\frac
{\partial p}{\partial s}}-KV}  [{\frac  {DV}{Dt}}=-{\frac  {1}{\rho }}{\frac
{\partial p}{\partial s}}-KV]
      V  2   R   = &#x2212;   1 &#x03C1;      &#x2202; p   &#x2202; n
&#x00B1; f V   {\displaystyle {\frac {V^{2}}{R}}=-{\frac {1}{\rho }}{\frac
{\partial p}{\partial n}}\pm fV}  [{\frac  {V^{2}}{R}}=-{\frac  {1}{\rho }}
{\frac  {\partial p}{\partial n}}\pm fV],
Ã¯n the forward and sideway directions respectively, where Ï is the density_of
air.
The terms can be broken down as follows:
    *     D V   /   D t    {\displaystyle {DV}/{Dt}}  [{DV}/{Dt}] is the
      temporal rate of speed change to the parcel (tangential acceleration);
    *    &#x2212;  &#x2202; p   /   &#x2202; s    {\displaystyle -{\partial p}/
      {\partial s}}  [-{\partial p}/{\partial s}] is the component of the
      pressure force per unit volume along the trajectory;
    *    &#x2212; K V   {\displaystyle -KV}  [-KV] is the deceleration due to
      friction;
    *      V  2     /   R    {\displaystyle {V^{2}}/{R}}  [{V^{2}}/{R}] is the
      centripetal acceleration;
    *    &#x2212;  &#x2202; p   /   &#x2202; n    {\displaystyle -{\partial p}/
      {\partial n}}  [-{\partial p}/{\partial n}] is the component of the
      pressure force per unit volume perpendicular to the trajectory;
    *    &#x00B1; f V   {\displaystyle \pm fV}  [\pm fV] is the Coriolis force
      per unit mass (the sign ambiguity depends on the mutual orientation of
      the force vector and n).
**** Steady-state assumption[edit] ****
In the following discussions, we consider steady-state flow. The speed cannot
thus change with time, and the component forces producing tangential
acceleration need to sum up to zero. In other words, active and resistive
forces must balance out in the forward direction in order that     D V  /  D t
= 0   {\displaystyle DV/Dt=0}  [DV/Dt=0]. Importantly, no assumption is made
yet on whether the right-hand side forces are of either significant or
negligible magnitude there. Moreover, trajectories and streamlines coincide in
steady-state conditions, and the pairs of adjectives tangential/normal and
streamwise/cross-stream become interchangeable. An atmospheric flow in which
the tangential acceleration is not negligible is called allisobaric.
The velocity direction can still change in space along the trajectory that,
excluding inertial_flows, is set by the pressure pattern.
***** General framework[edit] *****
**** The schematisations[edit] ****
Omitting specific terms in the tangential and normal balance equations, we
obtain one of the five following idealized flows: antitriptic, geostrophic,
cyclostrophic, inertial, and gradient flows. By reasoning on the balance of the
remaining terms, we can understand
    * what arrangement of the pressure field supports such flows;
    * along which trajectory the parcel of air travels; and
    * with which speed it does so.
The following yes/no table shows which contributions are considered in each
idealisation. The Ekman_layer's schematisation is also mentioned for
completeness, and is treated separately since it involves the internal friction
of air rather than that between air and ground.
 ____________________________________________________________________________
|         |Antitriptic|Geostrophic|Cyclostrophic|Inertial|Gradient|Ekman_flow|
|_________|flow_______|flow_______|flow_________|flow____|flow____|__________|
|curvature|N__________|N__________|Y____________|Y_______|Y_______|N_________|
|friction_|Y__________|N__________|N____________|N_______|N_______|Y_________|
|pressure_|Y__________|Y__________|Y____________|N_______|Y_______|Y_________|
|Coriolis_|N__________|Y__________|N____________|Y_______|Y_______|Y_________|
**** The limitations[edit] ****
*** Vertical differences of air properties[edit] ***
Main article: Buoyancy
The equations were said to apply to parcels of air moving on horizontal planes.
Indeed, when one considers a column of atmosphere, it is seldom the case that
the air density is the same all the height up, since temperature and moisture
content, hence density, do change with height. Every parcel within such a
column moves according to the air properties at its own height.
Homogeneous sheets of air may slide one over the other, so long as stable
stratification of lighter air on top of heavier air leads to well-separated
layers. If some air happens to be heavier/lighter than that in the
surroundings, though, vertical motions do occur and modify the horizontal
motion in turn. In nature downdrafts and updrafts can sometimes be more rapid
and intense than the motion parallel to the ground. The balanced-flow equations
do not contain either a force representing the sinking/buoyancy action or the
vertical component of velocity.
Consider also that the pressure is normally known through instruments
(barometers) near the ground/sea level. The isobars of the ordinary weather
charts summarise these pressure measurements, adjusted to the mean sea level
for uniformity of presentation, at one particular time. Such values represent
the weight of the air column overhead without indicating the details of the
changes of the air's specific_weight overhead. Also, by Bernoulli's_theorem,
the measured pressure is not exactly the weight of the air column, should
significant vertical motion of air occur. Thus, the pressure force acting on
individual parcels of air at different heights is not really known through the
measured values. When using information from a surface-pressure chart in
balanced-flow formulations, the forces are best viewed as applied to the entire
air column.
One difference of air speed in every air column invariably occurs, however,
near the ground/sea, also if the air density is the same anywhere and no
vertical motion occurs. There, the roughness of the contact surface slows down
the air motion above, and this retarding effect peters out with height. See,
for example, planetary_boundary_layer. Frictional antitriptic flow applies near
the ground, while the other schematisations apply far enough from the ground
not to feel its `braking' effect (free-air flow). This is a reason to keep the
two groups conceptually separated. The transition from low-quote to high-quote
schematisations is bridged by Ekman-like_schematisations where air-to-air
friction, Coriolis and pressure forces are in balance.
In summary, the balanced-flow speeds apply well to air columns that can be
regarded as homogeneous (constant density, no vertical motion) or, at most,
stably stratified (non-constant density, yet no vertical motion). An
uncertainty in the estimate arises if we are not able to verify these
conditions to occur. They also cannot describe the motion of the entire column
from the contact surface with the Earth up to the outer atmosphere, because of
the on-off handling of the friction forces.
*** Horizontal differences of air properties[edit] ***
Main article: Baroclinicity
Even if air columns are homogeneous with height, the density of each column can
change from location to location, firstly since air masses have different
temperatures and moisture content depending on their origin; and then since air
masses modify their properties as they flow over Earth's surface. For example,
in extra-tropical_cyclones the air circulating around a pressure low typically
comes with a sector of warmer temperature wedged within colder air. The
gradient-flow model of cyclonic circulation does not allow for these features.
Balanced-flow schematisations can be used to estimate the wind speed in air
flows covering several degrees of latitude of Earth's surface. However, in this
case assuming a constant Coriolis parameter is unrealistic, and the balanced-
flow speed can be applied locally. See Rossby_waves as an example of when
changes of latitude are dynamically effective.
*** Unsteadiness[edit] ***
The balanced-flow approach identifies typical trajectories and steady-state
wind speeds derived from balance-giving pressure patterns. In reality, pressure
patterns and the motion of air masses are tied together, since accumulation (or
density increase) of air mass somewhere increases the pressure on the ground
and vice versa. Any new pressure gradient will cause a new displacement of air,
and thus a continuous rearrangement. As weather itself demonstrates, steady-
state conditions are exceptional.
Since friction, pressure gradient and Coriolis forces do not necessarily
balance out, air masses actually accelerate and decelerate, so the actual speed
depends on its past values too. As seen next, the neat arrangement of pressure
fields and flow trajectories, either parallel or at a right angle, in balanced-
flow follows from the assumption of steady flow.
The steady-state balanced-flow equations do not explain how the flow was set in
motion in the first place. Also, if pressure patterns change quickly enough,
balanced-flow speeds cannot help track the air parcels over long distances,
simply because the forces that the parcel feels have changed while it is
displaced. The particle will end up somewhere else compared to the case that it
had followed the original pressure pattern.
In summary, the balanced-flow equations give out consistent steady-state wind
speeds that can estimate the situation at a certain moment and a certain place.
These speeds cannot be confidently used to understand where the air is moving
to in the long run, because the forcing naturally changes or the trajectories
are skewed with respect to the pressure pattern.
***** Antitriptic flow[edit] *****
Antitriptic flow describes a steady-state flow in a spatially varying pressure
field when
    * the entire pressure gradient exactly balances friction alone; and:
    * all actions promoting curvature are neglected.
The name comes from the Greek words 'anti' (against, counter-) and 'triptein'
(to rub) â meaning that this kind of flow proceeds by countering friction.
**** Formulation[edit] ****
In the streamwise momentum equation, friction balances the pressure gradient
component without being negligible (so that Kâ 0). The pressure gradient
vector is only made by the component along the trajectory tangent s. The
balance in the streamwise direction determines the antitriptic speed as:
   V = &#x2212;   1  K &#x03C1;       &#x2202; p   &#x2202; s
{\displaystyle V=-{\frac {1}{K\rho }}{\frac {\partial p}{\partial s}}}  [V=-
{\frac  {1}{K\rho }}{\frac  {\partial p}{\partial s}}]
A positive speed is guaranteed by the fact that antitriptic flows move along
the downward slope of the pressure field, so that mathematically      &#x2202;
p   /   &#x2202; s  < 0   {\displaystyle {\partial p}/{\partial s}<0}  [
{\partial p}/{\partial s}<0]. Provided the product KV is constant and Ï stays
the same, p turns out to vary linearly with s and the trajectory is such that
the parcel feels equal pressure drops while it covers equal distances. (This
changes, of course, when using a non-linear model of friction or a coefficient
of friction that varies in space to allow for different surface roughness.)
In the cross-stream momentum equation, the Coriolis force and normal pressure
gradient are both negligible, leading to no net bending action. As the
centrifugal term       V  2     /   R    {\displaystyle {V^{2}}/{R}}  [{V^{2}}/
{R}] vanishes while the speed is non-zero, the radius of curvature goes to
infinity, and the trajectory must be a straight line. In addition, the
trajectory is perpendicular to the isobars since     &#x2202; p  /  &#x2202; n
= 0   {\displaystyle \partial p/\partial n=0}  [\partial p/\partial n=0]. Since
this condition occurs when the n direction is that of an isobar, s is
perpendicular to the isobars. Thus, antitriptic isobars need to be equispaced
circles or straight lines.
**** Application[edit] ****
Antitriptic flow is probably the least used of the five balanced-flow
idealizations, because the conditions are quite strict. However, it is the only
one for which the friction underneath is regarded as a primary contribution.
Therefore, the antitriptic schematisation applies to flows that take place near
the Earth's surface, in a region known as constant-stress_layer.
In reality, the flow in the constant-stress layer has a component parallel to
the isobars too, since it is often driven by the faster flow overhead. This
occurs owing to the so-called free-air flow at high quotes, which tends to be
parallel to the isobars, and to the Ekman flow at intermediate quotes, which
causes a reduction of the free-air speed and a turning of direction while
approaching the surface.
Because the Coriolis effects are neglected, antitriptic flow occurs either near
the equator (irrespective of the motion's lengthscale) or elsewhere whenever
the Ekman_number of the flow is large (normally for small-scale processes), as
opposed to geostrophic flows.
Antitriptic flow can be used to describe some boundary-layer phenomena such as
sea breezes, Ekman pumping, and the low level jet of the Great Plains.[1]
***** Geostrophic flow[edit] *****
Main article: Geostrophic_wind
See also: Geostrophic_current
Nearly parallel isobars supporting quasi-geostrophic conditions
[Geostrophic_flow_(westerly)]
A westerly stream flow of global scale spans, approximately along parallels,
from Labrador (Canada) across the North Atlantic Ocean as fas as inner Russia
[Geostrophic_flow_(easterly)]
An easterly westerly stream flow of global scale spans, approximately along
parallels, from Russia over Europe as fas as the mid latitude Atlantic Ocean
[Geostrophic_flow_(northerly)]
An northerly air stream flows from Arctic to mid latitudes south of the 40th
parallel
[Geostrophic_flow_(north-westerly)]
A northwesterly stream sets in between two large-scale counter-rotating curved
flows (cyclone and anticyclone ). Close isobars indicate high speeds
© British Crown Copyright 2008, 2009 and 2010, The Met Office
Geostrophic flow describes a steady-state flow in a spatially varying pressure
field when
    * frictional effects are neglected; and:
    * the entire pressure gradient exactly balances the Coriolis force alone
      (resulting in no curvature).
The name 'geostrophic' stems from the Greek words 'ge' (Earth) and 'strephein'
(to turn). This etymology does not suggest turning of trajectories, rather a
rotation around the Earth.
**** Formulation[edit] ****
In the streamwise momentum equation, negligible friction is expressed by K=0
and, for steady-state balance, negligible streamwise pressure force follows.
The speed cannot be determined by this balance. However,     &#x2202; p  /
&#x2202; s = 0   {\displaystyle \partial p/\partial s=0}  [\partial p/\partial
s=0] entails that the trajectory must run along isobars, else the moving parcel
would experience changes of pressure like in antitriptic flows. No bending is
thus only possible if the isobars are straight lines in the first instance. So,
geostrophic flows take the appearance of a stream channelled along such
isobars.
In the cross-stream momentum equation, non-negligible Coriolis force is
balanced by the pressure force, in a way that the parcel does not experience
any bending action. Since the trajectory does not bend, the positive
orientation of n cannot be determined for lack of a centre of curvature. The
signs of the normal vector components become uncertain in this case. However,
the pressure force must exactly counterbalance the Coriolis force anyway, so
the parcel of air needs to travel with the Coriolis force contrary to the
decreasing sideways slope of pressure. Therefore, irrespective of the
uncertainty in formally setting the unit vector n, the parcel always travels
with the lower pressure at its left (right) in the northern (southern)
hemisphere.
The geostrophic speed is
   V =   1 &#x03C1;    |    1 f      &#x2202; p   &#x2202; n     |
{\displaystyle V={\frac {1}{\rho }}\left|{\frac {1}{f}}{\frac {\partial p}
{\partial n}}\right|}  [V={\frac  {1}{\rho }}\left|{\frac  {1}{f}}{\frac
{\partial p}{\partial n}}\right|].
The expression of geostrophic speed resembles that of antitriptic speed: here
the speed is determined by the magnitude of the pressure gradient across
(instead of along) the trajectory that develops along (instead of across) an
isobar.
**** Application[edit] ****
Modelers, theoreticians, and operational forecasters frequently make use of
geostrophic/quasi-geostrophic_approximation. Because friction is unimportant,
the geostrophic balance fits flows high enough above the Earth's surface.
Because the Coriolis force is relevant, it normally fits processes with small
Rossby_number, typically having large lengthscales. Geostrophic conditions are
also realised for flows having small Ekman_number, as opposed to antitriptic
conditions.
It is frequent that the geostrophic conditions develop between a well-defined
pair of pressure high and low; or that a major geostrophic stream is flanked by
several higher- and lower-pressure regions at either side of it (see images).
Although the balanced-flow equations do not allow for internal (air-to-air)
friction, the flow directions in geostrophic streams and nearby rotating
systems are also consistent with shear contact between those.
The speed of a geostrophic stream is larger (smaller) than that in the curved
flow around a pressure low (high) with the same pressure gradient: this feature
is explained by the more general gradient-flow schematisation. This helps use
the geostrophic speed as a back-of-the-envelope estimate of more complex
arrangementsâsee also the balanced-flow_speeds_compared below.
The etymology and the pressure charts shown suggest that geostrophic flows may
describe atmospheric motion at rather large scales, although not necessarily
so.
***** Cyclostrophic flow[edit] *****
Cyclostrophic flow describes a steady-state flow in a spatially varying
pressure field when
    * the frictional and Coriolis actions are neglected; and:
    * the centripetal acceleration is entirely sustained by the pressure
      gradient.
Trajectories do bend. The name 'cyclostrophic' stems from the Greek words
'kyklos' (circle) and 'strephein' (to turn).
**** Formulation[edit] ****
Like in geostrophic balance, the flow is frictionless and, for steady-state
motion, the trajectories follow the isobars.
In the cross-stream momentum equation, only the Coriolis force is discarded, so
that the centripetal acceleration is just the cross-stream pressure force per
unit mass
      V  2   R   = &#x2212;   1 &#x03C1;      &#x2202; p   &#x2202; n
{\displaystyle {\frac {V^{2}}{R}}=-{\frac {1}{\rho }}{\frac {\partial p}
{\partial n}}}  [{\frac  {V^{2}}{R}}=-{\frac  {1}{\rho }}{\frac  {\partial p}
{\partial n}}].
This implies that the trajectory is subject to a bending action, and that the
cyclostrophic speed is
   V =   &#x2212;   R &#x03C1;      &#x2202; p   &#x2202; n
{\displaystyle V={\sqrt {-{\frac {R}{\rho }}{\frac {\partial p}{\partial n}}}}}
[V={\sqrt  {-{\frac  {R}{\rho }}{\frac  {\partial p}{\partial n}}}}].
So, the cyclostrophic speed is determined by the magnitude of the pressure
gradient across the trajectory and by the radius of curvature of the isobar.
The flow is faster, the farther away from its centre of curvature, albeit less
than linearly.
Another implication of the cross-stream momentum equation is that a
cyclostrophic flow can only develop next to a low-pressure area. This is
implied in the requirement that the quantity under the square root is positive.
Recall that the cyclostrophic trajectory was found to be an isobar. Only if the
pressure increases from the centre of curvature outwards, the pressure
derivative is negative and the square root is well defined â the pressure in
the centre of curvature must thus be a low. The above mathematics gives no clue
whether the cyclostrophic rotation ends up to be clockwise or anticlockwise,
meaning that the eventual arrangement is a consequence of effects not allowed
for in the relationship, namely the rotation of the parent cell.
**** Application[edit] ****
The cyclostrophic schematisation is realistic when Coriolis and frictional
forces are both negligible, that is for flows having large Rossby_number and
small Ekman_number. Coriolis effects are ordinarily negligible in lower
latitudes or on smaller scales. Cyclostrophic balance can be achieved in
systems such as tornadoes, dust_devils and waterspouts. Cyclostrophic speed can
also be seen as one of the contribution of the gradient balance-speed, as shown
next.
Among the studies using the cyclostrophic schematisation, RennÃ³ and Bluestein
[2] use the cyclostrophic speed equation to construct a theory for waterspouts;
and Winn, Hunyady, and Aulich [3] use the cyclostrophic approximation to
compute the maximum tangential winds of a large tornado which passed near
Allison, Texas on 8 June 1995.
***** Inertial flow[edit] *****
Unlike all other flows, inertial balance implies a uniform pressure field. In
this idealisation:
    * the flow is frictionless;
    * no pressure gradient (and force) is present at all.
The only remaining action is the Coriolis force, which imparts curvature to the
trajectory.
**** Formulation[edit] ****
As before, frictionless flow in steady-state conditions implies that
&#x2202; p  /  &#x2202; s = 0   {\displaystyle \partial p/\partial s=0}
[\partial p/\partial s=0]. However, in this case isobars are not defined in the
first place. We cannot draw any anticipation about the trajectory from the
arrangement of the pressure field.
In the cross-stream momentum equation, after omitting the pressure force, the
centripetal acceleration is the Coriolis force per unit mass. The sign
ambiguity disappears, because the bending is solely determined by the Coriolis
force that sets unchallenged the side of curvature â so this force has always
a positive sign. The inertial rotation will be clockwise (anticlockwise) in the
northern (southern) hemisphere. The momentum equation
      V  2   R   =  | f |  V   {\displaystyle {\frac {V^{2}}
{R}}=\left|f\right|V}  [{\frac  {V^{2}}{R}}=\left|f\right|V],
gives us the inertial speed
   V =  | f |  R   {\displaystyle V=\left|f\right|R}  [V=\left|f\right|R].
The inertial speed's equation only helps determine either the speed or the
radius of curvature once the other is given. The trajectory resulting from this
motion is also known as inertial_circle. The balance-flow model gives no clue
on the initial speed of an inertial circle, which needs to be triggered by some
external perturbation.
**** Application[edit] ****
Since atmospheric motion is due largely to pressure differences, inertial flow
is not very applicable in atmospheric dynamics. However, the inertial speed
appears as a contribution to the solution of the gradient speed (see next).
Moreover, inertial flows are observed in the ocean streams, where flows are
less driven by pressure differences than in air because of higher
densityâinertial balance can occur at depths such that the friction
transmitted by the surface winds downwards vanishes.
[Nearly_inertial_flow_over_Central_Europe_and_Russia]
A nearly uniform pressure field covers Central Europe and Russia with pressure
differences smaller than 8 mbar over several tens of degrees of latitude and
longitude. (For the conditions over the Atlantic Ocean see geostrophic and
gradient flow) British Crown Copyright 2009, The Met Office
***** Gradient flow[edit] *****
Gradient flow is an extension of geostrophic flow as it accounts for curvature
too, making this a more accurate approximation for the flow in the upper
atmosphere. However, mathematically gradient flow is slightly more complex, and
geostrophic flow may be fairly accurate, so the gradient approximation is not
as frequently mentioned.
Gradient flow is also an extension of the cyclostrophic balance, as it allows
for the effect of the Coriolis force, making it suitable for flows with any
Rossby number.
Finally, it is an extension of inertial balance, as it allows for a pressure
force to drive the flow.
**** Formulation[edit] ****
Like in all but the antitriptic balance, frictional and pressure forces are
neglected in the streamwise momentum equation, so that it follows from
&#x2202; p  /  &#x2202; s = 0   {\displaystyle \partial p/\partial s=0}
[\partial p/\partial s=0] that the flow is parallel to the isobars.
Solving the full cross-stream momentum equation as a quadratic_equation for V
yields
   V = &#x00B1;    f R  2   &#x00B1;       f  2    R  2    4   &#x2212;   R
&#x03C1;      &#x2202; p   &#x2202; n        {\displaystyle V=\pm {\frac {fR}
{2}}\pm {\sqrt {{\frac {f^{2}R^{2}}{4}}-{\frac {R}{\rho }}{\frac {\partial p}
{\partial n}}}}}  [V=\pm {\frac  {fR}{2}}\pm {\sqrt  {{\frac  {f^{2}R^{2}}{4}}-
{\frac  {R}{\rho }}{\frac  {\partial p}{\partial n}}}}].
Not all solutions of the gradient wind speed yield physically plausible
results: the right-hand side as a whole needs be positive because of the
definition of speed; and the quantity under square root needs to be non-
negative. The first sign ambiguity follows from the mutual orientation of the
Coriolis force and unit vector n, whereas the second follows from the square
root.
The important cases of cyclonic and anticyclonic circulations are discussed
next.
*** Pressure lows and cyclones[edit] ***
Main article: Extratropical_cyclone
For regular cyclones (air circulation around pressure lows), the pressure force
is inward (positive term) and the Coriolis force outward (negative term)
irrespective of the hemisphere. The cross-trajectory momentum equation is
      V  2   R   =   1 &#x03C1;    |    &#x2202; p   &#x2202; n    |  &#x2212;
| f |  V   {\displaystyle {\frac {V^{2}}{R}}={\frac {1}{\rho }}\left|{\frac
{\partial p}{\partial n}}\right|-\left|f\right|V}  [{\frac  {V^{2}}{R}}={\frac
{1}{\rho }}\left|{\frac  {\partial p}{\partial n}}\right|-\left|f\right|V].
Dividing both sides by |f|V, one recognizes that
      V  g e o s t r o p h i c    V  c y c l o n e     = 1 +    V  c y c l o n
e    V  i n e r t i a l     > 1   {\displaystyle {\frac {V_{geostrophic}}{V_
{cyclone}}}=1+{\frac {V_{cyclone}}{V_{inertial}}}>1}  [{\frac  {V_{
{geostrophic}}}{V_{{cyclone}}}}=1+{\frac  {V_{{cyclone}}}{V_{{inertial}}}}>1],
whereby the cyclonic gradient speed V is smaller than the corresponding
geostrophic, less accurate estimate, and naturally approaches it as the radius
of curvature grows (as the inertial velocity goes to infinity). In cyclones,
therefore, curvature slows down the flow compared to the no-curvature value of
geostrophic speed. See also the balanced-flow_speeds_compared below.
The positive root of the cyclone equation is
    V  c y c l o n e   = &#x2212;    V  i n e r t i a l   2   +      V  i n e r
t i a l   2   4   +  V  c y c l o s t r o p h i c   2       {\displaystyle V_
{cyclone}=-{\frac {V_{inertial}}{2}}+{\sqrt {{\frac {V_{inertial}^{2}}{4}}+V_
{cyclostrophic}^{2}}}}  [V_{{cyclone}}=-{\frac  {V_{{inertial}}}{2}}+{\sqrt  {
{\frac  {V_{{inertial}}^{2}}{4}}+V_{{cyclostrophic}}^{2}}}].
This speed is always well defined as the quantity under the square root is
always positive.
*** Pressure highs and anticyclones[edit] ***
Main article: Anticyclone
In anticyclones (air circulation around pressure highs), the Coriolis force is
always inward (and positive), and the pressure force outward (and negative)
irrespective of the hemisphere. The cross-trajectory momentum equation is
      V  2   R   = &#x2212;   1 &#x03C1;    |    &#x2202; p   &#x2202; n    |
+  | f |  V   {\displaystyle {\frac {V^{2}}{R}}=-{\frac {1}{\rho }}\left|{\frac
{\partial p}{\partial n}}\right|+\left|f\right|V}  [{\frac  {V^{2}}{R}}=-{\frac
{1}{\rho }}\left|{\frac  {\partial p}{\partial n}}\right|+\left|f\right|V].
Dividing both sides by |f|V, we obtain
      V  g e o s t r o p h i c    V  a n t i c y c l o n e     = 1 &#x2212;
V  a n t i c y c l o n e    V  i n e r t i a l     < 1   {\displaystyle {\frac
{V_{geostrophic}}{V_{anticyclone}}}=1-{\frac {V_{anticyclone}}{V_
{inertial}}}<1}  [{\frac  {V_{{geostrophic}}}{V_{{anticyclone}}}}=1-{\frac  {V_
{{anticyclone}}}{V_{{inertial}}}}<1],
whereby the anticyclonic gradient speed V is larger than the geostrophic value
and approaches it as the radius of curvature becomes larger. In anticyclones,
therefore, the curvature of isobars speeds up the airflow compared to the
(geostrophic) no-curvature value. See also the balanced-flow_speeds_compared
below.
There are two positive roots for V, but the only one consistent with the limit
to geostrophic conditions is
    V  a n t i c y c l o n e   =    V  i n e r t i a l   2   &#x2212;      V  i
n e r t i a l   2   4   &#x2212;  V  c y c l o s t r o p h i c   2
{\displaystyle V_{anticyclone}={\frac {V_{inertial}}{2}}-{\sqrt {{\frac {V_
{inertial}^{2}}{4}}-V_{cyclostrophic}^{2}}}}  [V_{{anticyclone}}={\frac  {V_{
{inertial}}}{2}}-{\sqrt  {{\frac  {V_{{inertial}}^{2}}{4}}-V_{{cyclostrophic}}^
{2}}}]
that requires that      V  i n e r t i a l   &#x2265; 2  V  c y c l o s t r o p
h i c     {\displaystyle V_{inertial}\geq 2V_{cyclostrophic}}  [V_{
{inertial}}\geq 2V_{{cyclostrophic}}] to be meaningful. This condition can be
translated in the requirement that, given a high-pressure zone with a constant
pressure slope at a certain latitude, there must be a circular region around
the high without wind. On its circumference the air blows at half the
corresponding inertial speed (at the cyclostrophic speed), and the radius is
    R  &#x2217;   =   4  &#x03C1;  f  2       |    &#x2202; p   &#x2202; n    |
{\displaystyle R^{*}={\frac {4}{\rho f^{2}}}\left|{\frac {\partial p}{\partial
n}}\right|}  [R^{*}={\frac  {4}{\rho f^{2}}}\left|{\frac  {\partial p}{\partial
n}}\right|],
obtained by solving the above inequality for R. Outside this circle the speed
decreases to the geostrophic value as the radius of curvature increases. The
width of this radius grows with the intensity of the pressure gradient.
**** Application[edit] ****
Gradient Flow is useful in studying atmospheric flow rotating around high and
low pressures centers with small Rossby numbers. This is the case where the
radius of curvature of the flow about the pressure centers is small, and
geostrophic flow no longer applies with a useful degree of accuracy.
Surface pressure charts supporting gradient-wind conditions
[Cyclone]
Low pressure W of Ireland and cyclonic conditions.
[Anticyclone]
High pressure over the British Isles and anticyclonic conditions.
© British Crown Copyright 2009, The Met Office
***** Balanced-flow speeds compared[edit] *****
Each balanced-flow idealisation gives a different estimate for the wind speed
in the same conditions. Here we focus on the schematisations valid in the upper
atmosphere.
Firstly, imagine that a sample parcel of air flows 500 meters above the sea
surface, so that frictional effects are already negligible. The density of
(dry) air at 500 meter above the mean sea level is 1.167 kg/m3 according to its
equation of state.
Secondly, let the pressure force driving the flow be measured by a rate of
change taken as 1hPa/100 km (an average value). Recall that it is not the value
of the pressure to be important, but the slope with which it changes across the
trajectory. This slope applies equally well to the spacing of straight isobars
(geostrophic flow) or of curved isobars (cyclostrophic and gradient flows).
Thirdly, let the parcel travel at a latitude of 45 degrees, either in the
southern or northern hemisphereâso the Coriolis force is at play with a
Coriolis parameter of 0.000115 Hz.
The balance-flow speeds also changes with the radius of curvature R of the
trajectory/isobar. In case of circular isobars, like in schematic cyclones and
anticyclones, the radius of curvature is also the distance from the pressure
low and high respectively.
Taking two of such distances R as 100 km and 300 km, the speeds are (in m/s)
 _____________________________________________________________________
|        |Geostrophic|Cyclostrophic|Inertial|Gradient (H-|Gradient (L-|
|________|___________|_____________|________|pressure)___|pressure)___|
|R=100 k|7.45_______|9.25_________|11.50___|N/A_________|5.15________|
|R=300 k|7.45_______|16.00________|34.50___|10.90_______|6.30________|
The chart shows how the different speeds change in the conditions chosen above
and with increasing radius of curvature.
[Balanced-flow-speeds.PNG]
The geostrophic_speed (pink line) does not depend on curvature at all, and it
appears as a horizontal line. However, the cyclonic and anticyclonic gradient
speeds approach it as the radius of curvature becomes indefinitely
largeâgeostrophic balance is indeed the limiting case of gradient flow for
vanishing centripetal acceleration (that is, for pressure and Coriolis force
exactly balancing out).
The cyclostrophic_speed (black line) increases from zero and its rate of growth
with R is less than linear. In reality an unbounded speed growth is impossible
because the conditions supporting the flow change at some distance. Also recall
that the cyclostrophic conditions apply to small-scale processes, so
extrapolation to higher radii is physically meaningless.
The inertial_speed (green line), which is independent of the pressure gradient
that we chose, increases linearly from zero and it soon becomes much larger
than any other.
The gradient_speed comes with two curves valid for the speeds around a pressure
low (blue) and a pressure high (red). The wind speed in cyclonic circulation
grows from zero as the radius increases and is always less than the goestrophic
estimate.
In the anticyclonic-circulation example, there is no wind within the distance
of 260 km (point R*) â this is the area of no/low winds around a pressure
high. At that distance the first anticyclonic wind has the same speed as the
cyclostrophic winds (point Q), and half of that of the inertial wind (point P).
Farther away from point R*, the anticyclonic wind slows down and approaches the
geostrophic value with decreasingly larger speeds.
There is also another noteworthy point in the curve, labelled as S, where
inertial, cyclostrophic and geostrophic speeds are equal. The radius at S is
always a fourth of R*, that is 65 km here.
Some limitations of the schematisations become also apparent. For example, as
the radius of curvature increases along a meridian, the corresponding change of
latitude implies different values of the Coriolis parameter and, in turn,
force. Conversely, the Coriolis force stays the same if the radius is along a
parallel. So, in the case of circular flow, it is unlikely that the speed of
the parcel does not change in time around the full circle, because the air
parcel will feel the different intensity of the Coriolis force as it travels
across different latitudes. Additionally, the pressure fields quite rarely take
the shape of neat circular isobars that keep the same spacing all around the
circle. Also, important differences of density occur in the horizontal plan as
well, for example when warmer air joins the cyclonic circulation, thus creating
a warm sector between a cold and a warm front.
***** See also[edit] *****
    * Secondary_flow
***** References[edit] *****
   1. ^ Schaefer Etling, J.; C. Doswell (1980). "The Theory and Practical
      Application of Antitriptic Balance". Monthly Weather Review. 108 (6):
      746â756. Bibcode:1980MWRv..108..746S. doi:10.1175/1520-0493
      (1980)108<0746:TTAPAO>2.0.CO;2. ISSN 1520-0493.
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
   3. ^RennÃ³, N.O.D.; H.B. Bluestein (2001). "A Simple Theory for
      Waterspouts". Journal of the Atmospheric Sciences. 58 (8): 927â932.
      Bibcode:2001JAtS...58..927R. doi:10.1175/1520-0469(2001)058<0927:
      ASTFW>2.0.CO;2. ISSN 1520-0469.
   4. ^ Winn, W.P.; S.J. Hunyady G.D. Aulich (1999). "Pressure at the ground in
      a large tornado". Journal of Geophysical Research. 104 (D18): 22,
      067â22, 082. Bibcode:1999JGR...10422067W. doi:10.1029/1999JD900387.
***** Further reading[edit] *****
    * Holton, James R.: An Introduction to Dynamic Meteorology, 2004.
ISBN 0-12-354015-1
***** External links[edit] *****
    * American Meteorological Society Glossary_of_Terms
    * Met Office UK Pressure_Charts_in_NE_Atlantic_and_Europe
    * Plymouth State Weather Center Balanced_Flows_Tutorial

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Balanced_flow&oldid=901483652"
Categories:
    * Atmospheric_dynamics
Hidden categories:
    * Articles_needing_additional_references_from_September_2018
    * All_articles_needing_additional_references
    * Use_dmy_dates_from_June_2019
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
    * FranÃ§ais
    * Norsk
    * Norsk_nynorsk
Edit_links
    * This page was last edited on 12 June 2019, at 05:34 (UTC).
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
