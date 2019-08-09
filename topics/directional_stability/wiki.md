The following text has been accessed from https://en.wikipedia.org/wiki/Directional_stability at Thu Aug 8 23:18:05 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Directional stability ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article has multiple issues. Please help improve_it or discuss these
 issues on the talk_page. (Learn_how_and_when_to_remove_these_template
 messages)
  This article may be too technical for most readers to understand. Please help
  improve_it to make_it_understandable_to_non-experts, without removing the
  technical details. (April 2011)(Learn_how_and_when_to_remove_this_template
  message)
  This article includes a list_of_references, related reading or external
  links, but its sources remain unclear because it lacks inline_citations.
  Please help to improve this article by introducing more precise citations.
  (August 2012)(Learn_how_and_when_to_remove_this_template_message)
 (Learn_how_and_when_to_remove_this_template_message)
Directional stability is stability of a moving body or vehicle about an axis
which is perpendicular to its direction of motion. Stability of a vehicle
concerns itself with the tendency of a vehicle to return to its original
direction in relation to the oncoming medium (water, air, road surface, etc.)
when disturbed (rotated) away from that original direction. If a vehicle is
directionally stable, a restoring moment is produced which is in a direction
opposite to the rotational disturbance. This "pushes" the vehicle (in rotation)
so as to return it to the original orientation, thus tending to keep the
vehicle oriented in the original direction.
Directional stability is frequently called "weather vaning" because a
directionally stable vehicle free to rotate about its center of mass is similar
to a weather_vane rotating about its (vertical) pivot.
With the exception of spacecraft, vehicles generally have a recognisable front
and rear and are designed so that the front points more or less in the
direction of motion. Without this stability, they may tumble end over end, spin
or orient themselves at a high angle_of_attack, even broadside on to the
direction of motion. At high angles of attack, drag forces may become
excessive, the vehicle may be impossible to control, or may even experience
structural failure. In general, land, sea, air and underwater vehicles are
designed to have a natural tendency to point in the direction of motion.
⁰
***** Contents *****
    * 1_Example:_road_vehicle
          o 1.1_Introduction
          o 1.2_Stability_analysis
          o 1.3_Relative_effect_of_front_and_rear_tyres
          o 1.4_Steering_forces
          o 1.5_Limitations_of_the_analysis
    * 2_References
    * 3_See_also
***** Example: road vehicle[edit] *****
Arrows, darts, rockets, and airships have tail surfaces to achieve stability. A
road vehicle does not have elements specifically designed to maintain
stability, but relies primarily on the distribution of mass.
**** Introduction[edit] ****
These points are best illustrated with an example. The first stage of studying
the stability of a road vehicle is the derivation of a reasonable approximation
to the equations of motion.
[Car0_stabilty.png]
The diagram illustrates a four-wheel vehicle, in which the front axle is
located a distance     a   {\displaystyle a}  [a] ahead of the centre_of
gravity and the rear axle is a distance     b   {\displaystyle b}  [b] aft of
the cg. The body of the car is pointing in a direction     &#x03B8;
{\displaystyle \theta }  [\theta ] (theta) whilst it is travelling in a
direction     &#x03C8;   {\displaystyle \psi }  [\psi ] (psi). In general,
these are not the same. The tyre treads at the region of contact point in the
direction of travel, but the hubs are aligned with the vehicle body, with the
steering held central. The tyres distort as they rotate to accommodate this
mis-alignment, and generate side forces as a consequence.
The net side force Y on the vehicle is the centripetal force causing the
vehicle to change the direction it is traveling:
         M V    d &#x03C8;   d t    = Y  cos &#x2061; ( &#x03B8; &#x2212;
      &#x03C8; )   {\displaystyle MV{\frac {d\psi }{dt}}=Y\,\cos(\theta -\psi
      )}  [{\displaystyle MV{\frac {d\psi }{dt}}=Y\,\cos(\theta -\psi )}]
where M is the vehicle mass and V the speed. The angles are all assumed small,
so the lateral force equation is:
         M V    d &#x03C8;   d t    = Y   {\displaystyle MV{\frac {d\psi }
      {dt}}=Y}  [MV{\frac  {d\psi }{dt}}=Y]
The rotation of the body subjected to a yawing moment N is governed by:
         I     d  2   &#x03B8;   d  t  2      = N   {\displaystyle I{\frac {d^
      {2}\theta }{dt^{2}}}=N}  [I{\frac  {d^{2}\theta }{dt^{2}}}=N]
where I is the moment_of_inertia in yaw. The forces and moments of interest
arise from the distortion of the tyres. The angle between the direction the
tread is rolling and the hub is called the slip_angle. This is a bit of a
misnomer, because the tyre as a whole does not actually slip, part of the
region in contact with the road adheres, and part of the region slips. We
assume that the tyre force is directly proportional to the slip angle
(    &#x03D5;   {\displaystyle \phi }  [\phi ]). This is made up of the slip of
the vehicle as a whole modified by the angular velocity of the body. For the
front axle:
         &#x03D5; ( f r o n t ) = &#x03B8; &#x2212; &#x03C8; &#x2212;   a V
      d &#x03B8;   d t      {\displaystyle \phi (front)=\theta -\psi -{\frac
      {a}{V}}{\frac {d\theta }{dt}}}  [\phi (front)=\theta -\psi -{\frac  {a}
      {V}}{\frac  {d\theta }{dt}}]
whilst for the rear axle:
         &#x03D5; ( r e a r ) = &#x03B8; &#x2212; &#x03C8; +   b V      d
      &#x03B8;   d t      {\displaystyle \phi (rear)=\theta -\psi +{\frac {b}
      {V}}{\frac {d\theta }{dt}}}  [\phi (rear)=\theta -\psi +{\frac  {b}{V}}
      {\frac  {d\theta }{dt}}]
Let the constant of proportionality be k. The sideforce is, therefore:
         Y = 2 k ( &#x03D5; ( f r o n t ) + &#x03D5; ( r e a r ) ) = 4 k
      ( &#x03B8; &#x2212; &#x03C8; ) + 2 k    ( b &#x2212; a )  V      d
      &#x03B8;   d t      {\displaystyle Y=2k(\phi (front)+\phi (rear))=4k
      (\theta -\psi )+2k{\frac {(b-a)}{V}}{\frac {d\theta }{dt}}}  [Y=2k(\phi
      (front)+\phi (rear))=4k(\theta -\psi )+2k{\frac  {(b-a)}{V}}{\frac
      {d\theta }{dt}}]
The moment is:
         N = 2 k ( a &#x03D5; ( f r o n t ) &#x2212; b &#x03D5; ( r e a r ) ) =
      2 k ( a &#x2212; b ) ( &#x03B8; &#x2212; &#x03C8; ) &#x2212; 2 k    (  a
      2   +  b  2   )  V      d &#x03B8;   d t      {\displaystyle N=2k(a\phi
      (front)-b\phi (rear))=2k(a-b)(\theta -\psi )-2k{\frac {(a^{2}+b^{2})}{V}}
      {\frac {d\theta }{dt}}}  [N=2k(a\phi (front)-b\phi (rear))=2k(a-b)(\theta
      -\psi )-2k{\frac  {(a^{2}+b^{2})}{V}}{\frac  {d\theta }{dt}}]
Denoting the angular velocity     &#x03C9;   {\displaystyle \omega }  [\omega
], the equations of motion are:
            d &#x03C9;   d t    = 2 k    ( a &#x2212; b )  I   ( &#x03B8;
      &#x2212; &#x03C8; ) &#x2212; 2 k    (  a  2   +  b  2   )   V I
      &#x03C9;   {\displaystyle {\frac {d\omega }{dt}}=2k{\frac {(a-b)}{I}}
      (\theta -\psi )-2k{\frac {(a^{2}+b^{2})}{VI}}\omega }  [{\frac  {d\omega
      }{dt}}=2k{\frac  {(a-b)}{I}}(\theta -\psi )-2k{\frac  {(a^{2}+b^{2})}
      {VI}}\omega ]
            d &#x03B8;   d t    = &#x03C9;   {\displaystyle {\frac {d\theta }
      {dt}}=\omega }  [{\frac  {d\theta }{dt}}=\omega ]
            d &#x03C8;   d t    =    4 k   M V    ( &#x03B8; &#x2212; &#x03C8;
      ) + 2 k    ( b &#x2212; a )   M  V  2      &#x03C9;   {\displaystyle
      {\frac {d\psi }{dt}}={\frac {4k}{MV}}(\theta -\psi )+2k{\frac {(b-a)}{MV^
      {2}}}\omega }  [{\frac  {d\psi }{dt}}={\frac  {4k}{MV}}(\theta -\psi )+2k
      {\frac  {(b-a)}{MV^{2}}}\omega ]
Let     &#x03B8; &#x2212; &#x03C8; = &#x03B2;   {\displaystyle \theta -\psi
=\beta }  [\theta -\psi =\beta ] (beta), the slip angle for the vehicle as a
whole:
            d &#x03C9;   d t    = 2 k    ( a &#x2212; b )  I   &#x03B2;
      &#x2212; 2 k    (  a  2   +  b  2   )   V I    &#x03C9;   {\displaystyle
      {\frac {d\omega }{dt}}=2k{\frac {(a-b)}{I}}\beta -2k{\frac {(a^{2}+b^
      {2})}{VI}}\omega }  [{\frac {d\omega }{dt}}=2k{\frac {(a-b)}{I}}\beta -2k
      {\frac {(a^{2}+b^{2})}{VI}}\omega ]
            d &#x03B2;   d t    = &#x2212;    4 k   M V    &#x03B2; + ( 1
      &#x2212; 2 k )    ( b &#x2212; a )   M  V  2      &#x03C9;
      {\displaystyle {\frac {d\beta }{dt}}=-{\frac {4k}{MV}}\beta +(1-2k){\frac
      {(b-a)}{MV^{2}}}\omega }  [{\frac {d\beta }{dt}}=-{\frac {4k}{MV}}\beta +
      (1-2k){\frac {(b-a)}{MV^{2}}}\omega ]
Eliminating     &#x03C9;   {\displaystyle \omega }  [\omega ] yields the
following equation in     &#x03B2;   {\displaystyle \beta }  [\beta ]:
             d  2   &#x03B2;   d  t  2      + (    4 k   M V    +    2 k (  a
      2   +  b  2   )   V I    )    d &#x03B2;   d t    + (    4  k  2   ( a +
      b  )  2     M  V  2   I    +    2 k ( b &#x2212; a )  I   ) &#x03B2; = 0
      {\displaystyle {\frac {d^{2}\beta }{dt^{2}}}+({\frac {4k}{MV}}+{\frac {2k
      (a^{2}+b^{2})}{VI}}){\frac {d\beta }{dt}}+({\frac {4k^{2}(a+b)^{2}}{MV^
      {2}I}}+{\frac {2k(b-a)}{I}})\beta =0}  [{\frac  {d^{2}\beta }{dt^{2}}}+(
      {\frac  {4k}{MV}}+{\frac  {2k(a^{2}+b^{2})}{VI}}){\frac  {d\beta }{dt}}+(
      {\frac  {4k^{2}(a+b)^{2}}{MV^{2}I}}+{\frac  {2k(b-a)}{I}})\beta =0]
This is called a second order linear homogeneous equation, and its properties
form the basis of much of control_theory.
**** Stability analysis[edit] ****
We do not need to solve the equation of motion explicitly to decide whether the
solution diverges indefinitely or converges to zero following an initial
perturbation. The form of the solution depends on the signs of the
coefficients.
The coefficient of        d &#x03B2;   d t      {\displaystyle {\frac {d\beta }
{dt}}}  [{\frac {d\beta }{dt}}] will be called the 'damping' by analogy with a
mass-spring-damper which has a similar equation of motion.
By the same analogy, the coefficient of     &#x03B2;   {\displaystyle \beta }
[\beta ] will be called the 'stiffness', as its function is to return the
system to zero deflection, in the same manner as a spring.
The form of the solution depends only on the signs of the damping and stiffness
terms. The four possible solution types are presented in the figure.
[Second_Order_Solutions.png]
The only satisfactory solution requires both stiffness and damping to be
positive.
The damping term is:
               (    4 k   M V    +    2 k (  a  2   +  b  2   )   V I    )
            {\displaystyle ({\frac {4k}{MV}}+{\frac {2k(a^{2}+b^{2})}{VI}})}  [
            ({\frac  {4k}{MV}}+{\frac  {2k(a^{2}+b^{2})}{VI}})]
The tyre slip coefficient k is positive, as are the mass, moment of inertia and
speed, so the damping is positive, and the directional motion should be
dynamically stable.
The stiffness term is:
               (    4  k  2   ( a + b  )  2     M I  V  2      +    2 k ( b
            &#x2212; a )  I   )   {\displaystyle ({\frac {4k^{2}(a+b)^{2}}{MIV^
            {2}}}+{\frac {2k(b-a)}{I}})}  [({\frac  {4k^{2}(a+b)^{2}}{MIV^
            {2}}}+{\frac  {2k(b-a)}{I}})]
If the centre of gravity is ahead of the centre of the wheelbase (    ( b > a )
{\displaystyle (b>a)}  [(b>a)], this will always be positive, and the vehicle
will be stable at all speeds. However, if it lies further aft, the term has the
potential of becoming negative above a speed given by:
                V  2   =    2 k ( a + b  )  2     M ( a &#x2212; b )
            {\displaystyle V^{2}={\frac {2k(a+b)^{2}}{M(a-b)}}}  [V^{2}={\frac
            {2k(a+b)^{2}}{M(a-b)}}]
Above this speed, the vehicle will be directionally unstable.
**** Relative effect of front and rear tyres[edit] ****
If for some reason (incorrect inflation pressure, worn tread) the tyres on one
axle are incapable of generating significant lateral force, the stability will
obviously be affected.
Assume to begin with that the rear tyres are faulty, what is the effect on
stability? If the rear tyres produce no significant forces, the side force and
yawing moment become:
         Y = 2 k ( &#x03D5; ( f r o n t ) ) = 2 k ( &#x03B8; &#x2212; &#x03C8;
      ) &#x2212; 2 k   a V      d &#x03B8;   d t      {\displaystyle Y=2k(\phi
      (front))=2k(\theta -\psi )-2k{\frac {a}{V}}{\frac {d\theta }{dt}}}  [Y=2k
      (\phi (front))=2k(\theta -\psi )-2k{\frac  {a}{V}}{\frac  {d\theta }
      {dt}}]
         N = 2 k ( a &#x03D5; ( f r o n t ) ) = 2 k a ( &#x03B8; &#x2212;
      &#x03C8; ) &#x2212; 2 k    a  2   V      d &#x03B8;   d t
      {\displaystyle N=2k(a\phi (front))=2ka(\theta -\psi )-2k{\frac {a^{2}}
      {V}}{\frac {d\theta }{dt}}}  [N=2k(a\phi (front))=2ka(\theta -\psi )-2k
      {\frac  {a^{2}}{V}}{\frac  {d\theta }{dt}}]
The equation of motion becomes:
             d  2   &#x03B2;   d  t  2      + (    2 k   M V    +    2 k  a  2
      V I    )    d &#x03B2;   d t    &#x2212; (    2 k a  I   ) &#x03B2; = 0
      {\displaystyle {\frac {d^{2}\beta }{dt^{2}}}+({\frac {2k}{MV}}+{\frac
      {2ka^{2}}{VI}}){\frac {d\beta }{dt}}-({\frac {2ka}{I}})\beta =0}  [{\frac
      {d^{2}\beta }{dt^{2}}}+({\frac  {2k}{MV}}+{\frac  {2ka^{2}}{VI}}){\frac
      {d\beta }{dt}}-({\frac  {2ka}{I}})\beta =0]
The coefficient of     &#x03B2;   {\displaystyle \beta }  [\beta ] is negative,
so the vehicle will be unstable.
Now consider the effect of faulty tyres at the front. The Side force and yawing
moment become:
         Y = 2 k ( &#x03D5; ( r e a r ) ) = 2 k ( &#x03B8; &#x2212; &#x03C8; )
      + 2 k   b V      d &#x03B8;   d t      {\displaystyle Y=2k(\phi
      (rear))=2k(\theta -\psi )+2k{\frac {b}{V}}{\frac {d\theta }{dt}}}  [Y=2k
      (\phi (rear))=2k(\theta -\psi )+2k{\frac  {b}{V}}{\frac  {d\theta }{dt}}]
         N = &#x2212; 2 k ( b &#x03D5; ( r e a r ) ) = &#x2212; 2 k b
      ( &#x03B8; &#x2212; &#x03C8; ) &#x2212; 2 k    b  2   V      d &#x03B8;
      d t      {\displaystyle N=-2k(b\phi (rear))=-2kb(\theta -\psi )-2k{\frac
      {b^{2}}{V}}{\frac {d\theta }{dt}}}  [N=-2k(b\phi (rear))=-2kb(\theta -
      \psi )-2k{\frac  {b^{2}}{V}}{\frac  {d\theta }{dt}}]
The equation of motion becomes:
             d  2   &#x03B2;   d  t  2      + (    2 k   M V    +    2 k  b  2
      V I    )    d &#x03B2;   d t    + (    2 k b  I   ) &#x03B2; = 0
      {\displaystyle {\frac {d^{2}\beta }{dt^{2}}}+({\frac {2k}{MV}}+{\frac
      {2kb^{2}}{VI}}){\frac {d\beta }{dt}}+({\frac {2kb}{I}})\beta =0}  [{\frac
      {d^{2}\beta }{dt^{2}}}+({\frac  {2k}{MV}}+{\frac  {2kb^{2}}{VI}}){\frac
      {d\beta }{dt}}+({\frac  {2kb}{I}})\beta =0]
The coefficient of     &#x03B2;   {\displaystyle \beta }  [\beta ] is positive,
so the vehicle will be stable but unsteerable.
It follows that the condition of the rear tyres is more critical to directional
stability than the state of the front tyres. Also, locking the rear wheels by
applying the handbrake, renders the vehicle directionally unstable, causing it
to spin. Since the vehicle is not under control during the spin, the 'handbrake
turn' is usually illegal on public roads.
**** Steering forces[edit] ****
Deflecting the steering changes the slip angle of the front tyres, generating a
sideforce. With conventional steering, the tyres are deflected by different
amounts, but for the purposes of this analysis, the additional slip will be
considered equal for both front tyres.
The side force becomes:
         Y = 2 k ( &#x03D5; ( f r o n t ) + &#x03D5; ( r e a r ) ) = 4 k
      ( &#x03B8; &#x2212; &#x03C8; ) + 2 k    ( b &#x2212; a )  V      d
      &#x03B8;   d t    + 2 k &#x03B7;   {\displaystyle Y=2k(\phi (front)+\phi
      (rear))=4k(\theta -\psi )+2k{\frac {(b-a)}{V}}{\frac {d\theta }
      {dt}}+2k\eta }  [Y=2k(\phi (front)+\phi (rear))=4k(\theta -\psi )+2k
      {\frac  {(b-a)}{V}}{\frac  {d\theta }{dt}}+2k\eta ]
where     &#x03B7;   {\displaystyle \eta }  [\eta ] (eta) is the steering
deflection. Similarly, the yawing moment becomes:
         N = 2 k ( a &#x03D5; ( f r o n t ) &#x2212; b &#x03D5; ( r e a r ) ) =
      2 k ( a &#x2212; b ) ( &#x03B8; &#x2212; &#x03C8; ) &#x2212; 2 k    (  a
      2   +  b  2   )  V      d &#x03B8;   d t    + 2 k a &#x03B7;
      {\displaystyle N=2k(a\phi (front)-b\phi (rear))=2k(a-b)(\theta -\psi )-2k
      {\frac {(a^{2}+b^{2})}{V}}{\frac {d\theta }{dt}}+2ka\eta }  [N=2k(a\phi
      (front)-b\phi (rear))=2k(a-b)(\theta -\psi )-2k{\frac  {(a^{2}+b^{2})}
      {V}}{\frac  {d\theta }{dt}}+2ka\eta ]
Including the steering term introduces a forced response:
             d  2   &#x03B2;   d  t  2      + (    4 k   M V    +    2 k (  a
      2   +  b  2   )   V I    )    d &#x03B2;   d t    + (    4  k  2   ( a +
      b  )  2     M  V  2   I    +    2 k ( b &#x2212; a )  I   ) &#x03B2; =
      &#x2212;    2 k   M V       d &#x03B7;   d t    + (    2 k a  I
      &#x2212;    4  k  2   b ( a + b )   I M  V  2      ) &#x03B7;
      {\displaystyle {\frac {d^{2}\beta }{dt^{2}}}+({\frac {4k}{MV}}+{\frac {2k
      (a^{2}+b^{2})}{VI}}){\frac {d\beta }{dt}}+({\frac {4k^{2}(a+b)^{2}}{MV^
      {2}I}}+{\frac {2k(b-a)}{I}})\beta =-{\frac {2k}{MV}}{\frac {d\eta }{dt}}+
      ({\frac {2ka}{I}}-{\frac {4k^{2}b(a+b)}{IMV^{2}}})\eta }  [{\frac  {d^
      {2}\beta }{dt^{2}}}+({\frac  {4k}{MV}}+{\frac  {2k(a^{2}+b^{2})}{VI}})
      {\frac  {d\beta }{dt}}+({\frac  {4k^{2}(a+b)^{2}}{MV^{2}I}}+{\frac  {2k
      (b-a)}{I}})\beta =-{\frac  {2k}{MV}}{\frac  {d\eta }{dt}}+({\frac  {2ka}
      {I}}-{\frac  {4k^{2}b(a+b)}{IMV^{2}}})\eta ]
The steady state response is with all time derivatives set to zero. Stability
requires that the coefficient of     &#x03B2;   {\displaystyle \beta }  [\beta
] must be positive, so the sign of the response is determined by the
coefficient of     &#x03B7;   {\displaystyle \eta }  [\eta ]:
               (    2 k a  I   &#x2212;    4  k  2   b ( a + b )   I M  V  2
            )   {\displaystyle ({\frac {2ka}{I}}-{\frac {4k^{2}b(a+b)}{IMV^
            {2}}})}  [({\frac  {2ka}{I}}-{\frac  {4k^{2}b(a+b)}{IMV^{2}}})]
This is a function of speed. When the speed is low, the slip is negative and
the body points out of the corner (it understeers). At a speed given by:
                V  2   =    2 k b ( a + b )   M a      {\displaystyle V^{2}=
            {\frac {2kb(a+b)}{Ma}}}  [V^{2}={\frac  {2kb(a+b)}{Ma}}]
The body points in the direction of motion. Above this speed, the body points
into the corner (oversteers).
As an example:
            with k=10kN/radian, M=1000kg, b=1.0m, a=1.0m, the vehicle
            understeers below 11.3mph.
Evidently moving the centre of gravity forwards increases this speed, giving
the vehicle a tendency to understeer.
Note: Installing a heavy, powerful engine in a light weight production vehicle
designed around a small engine increases both its directional stability, and
its tendency to understeer. The result is an overpowered vehicle with poor
cornering performance.
Even worse is the installation of an oversized power unit into a rear engined
production vehicle without corresponding modification of suspension or mass
distribution, as the result will be directionally unstable at high speed.
**** Limitations of the analysis[edit] ****
The forces arising from slip depend on the loading on the tyre as well as the
slip angle, this effect has been ignored, but could be taken into account by
assuming different values of k for the front and rear axles. Roll motion due to
cornering will redistribute the tyre loads between the nearside and offside of
the vehicle, again modifying the tyre forces. Engine torque likewise re-
distributes the load between front and rear tyres.
A full analysis should also take account of the suspension response.
The complete analysis is essential for the design of high performance road
vehicles, but is beyond the scope of this article.
***** References[edit] *****
    * Barwell F T : Automation and Control in Transport, Pergamon Press, 1972.
    * Synge J L and B A Griffiths : Principles of Mechanics, Section 6.3,
      McGraw-Hill Kogakusha Ltd,3rd Edition, 1970.
***** See also[edit] *****
    * Relaxed_stability
    * Car_handling
    * Flight_dynamics
    * Longitudinal_static_stability
    * Hunting_oscillation

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Directional_stability&oldid=881509180"
Categories:
    * Mechanics
Hidden categories:
    * Wikipedia_articles_that_are_too_technical_from_April_2011
    * All_articles_that_are_too_technical
    * Articles_needing_expert_attention_from_April_2011
    * All_articles_needing_expert_attention
    * Articles_lacking_in-text_citations_from_August_2012
    * All_articles_lacking_in-text_citations
    * Articles_with_multiple_maintenance_issues
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
Add_links
    * This page was last edited on 3 February 2019, at 01:37 (UTC).
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
