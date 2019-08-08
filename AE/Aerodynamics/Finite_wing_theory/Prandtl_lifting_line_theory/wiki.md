The following text has been accessed from https://en.wikipedia.org/wiki/Lifting-line_theory at Thu Aug 8 23:16:23 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Lifting-line theory ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Mathematical model to quantify lift
The Prandtl lifting-line theory[1] is a mathematical model that predicts lift
distribution over a three-dimensional wing based on its geometry. It is also
known as the LanchesterâPrandtl wing theory.[2]
The theory was expressed independently[3] by Frederick_W._Lanchester in 1907,
[4] and by Ludwig_Prandtl in 1918â1919[5] after working with Albert_Betz and
Max_Munk.
In this model, the vortex loses strength along the whole wingspan because it is
shed as a vortex-sheet from the trailing edge, rather than just at the wing-
tips.[6][7]
⁰
***** Contents *****
    * 1_Introduction
    * 2_Principle
    * 3_Derivation
    * 4_Lift_and_drag_from_coefficients
    * 5_Symmetric_wing
    * 6_Rolling_wings
    * 7_Control_deflection
    * 8_Elliptical_wings
    * 9_Useful_approximations
    * 10_Limitations_of_the_theory
    * 11_See_also
    * 12_Notes
    * 13_References
***** Introduction[edit] *****
An unrealistic lift distribution that neglects three-dimensional effects
A lift distribution as observed over a (finite) trapezoidal wing
On a three-dimensional, finite wing, lift over each wing segment (local lift
per unit span,     l   {\displaystyle l}  [l] or        L &#x007E;
{\displaystyle {\tilde {L}}}  [{\tilde  L}]) does not correspond simply to what
two-dimensional analysis predicts. Instead, this local amount of lift is
strongly affected by the lift generated at neighboring wing sections.
It is difficult to predict analytically the overall amount of lift that a wing
of given geometry will generate. The lifting-line theory yields the lift
distribution along the span-wise direction,         L &#x007E;     ( y )
{\displaystyle {\tilde {L}}_{(y)}}  [{\tilde  L}_{{(y)}}] based only on the
wing geometry (span-wise distribution of chord, airfoil, and twist) and flow
conditions (    &#x03C1;   {\displaystyle \rho }  [\rho ],      V  &#x221E;
{\displaystyle V_{\infty }}  [V_{\infty }],      &#x03B1;  &#x221E;
{\displaystyle \alpha _{\infty }}  [\alpha _{\infty }]).
***** Principle[edit] *****
The lifting-line theory applies the concept of circulation and the
KuttaâJoukowski_theorem,
             L &#x007E;     ( y )   = &#x03C1; V  &#x0393;  ( y )
      {\displaystyle {\tilde {L}}_{(y)}=\rho V\Gamma _{(y)}}  [{\tilde  L}_{{
      (y)}}=\rho V\Gamma _{{(y)}}]
so that instead of the lift distribution function, the unknown effectively
becomes the distribution of circulation over the span,      &#x0393;  ( y )
{\displaystyle \Gamma _{(y)}}  [\Gamma _{{(y)}}].
    * The lift distribution over a wing can be modeled with the concept of
      circulation
    * A_vortex_is_shed_downstream for every span-wise change in lift
Modeling the (unknown and sought-after) local lift with the (also unknown)
local circulation allows us to account for the influence of one section over
its neighbors. In this view, any span-wise change in lift is equivalent to a
span-wise change of circulation. According to Helmholtz's_theorems, a vortex
filament cannot begin or terminate in the air. Any span-wise change in lift can
be modeled as the_shedding_of_a_vortex_filament_down_the_flow, behind the wing.
This shed vortex, whose strength is the derivative of the (unknown) local wing
circulation distribution,        d &#x2061; &#x0393;   d &#x2061; y
{\displaystyle {\operatorname {d} \Gamma \over \operatorname {d} y}}  [
{\operatorname {d}\Gamma  \over \operatorname {d}y}], influences the flow left
and right of the wing section.
    * The shed vortex can be modeled as a vertical velocity distribution
    * The upwash and downwash induced by the shed vortex can be computed at
      each neighbor segment.
This sideways influence (upwash on the outboard, downwash on the inboard) is
the key to the lifting-line theory. Now, if the change in lift distribution is
known at given lift section, it is possible to predict how that section
influences the lift over its neighbors: the vertical induced velocity (upwash
or downwash,      &#x03C9;  i     {\displaystyle \omega _{i}}  [\omega _{i}])
can be quantified using the velocity distribution within a vortex, and related
to a change in effective angle of attack over neighboring sections.
In mathematical terms, the local induced change of angle of attack
&#x03B1;  i     {\displaystyle \alpha _{i}}  [\alpha _{i}] on a given section
can be quantified with the integral sum of the downwash induced by every other
wing section. In turn, the integral sum of the lift on each downwashed wing
section is equal to the (known) total desired amount of lift.
This leads to an integro-differential_equation in the form of      L  t o t a l
= &#x03C1;  V  &#x221E;    &#x222B;  t i p   t i p    &#x0393;  ( y )   d
&#x2061; y   {\displaystyle L_{total}=\rho V_{\infty }\int _{tip}^{tip}\Gamma _
{(y)}\operatorname {d} y}  [L_{{total}}=\rho V_{\infty }\int _{{tip}}^{
{tip}}\Gamma _{{(y)}}\operatorname {d}y] where      &#x0393;  ( y )
{\displaystyle \Gamma _{(y)}}  [\Gamma _{{(y)}}] is expressed solely in terms
of the wing geometry and its own span-wise variation,        d &#x2061;
&#x0393;  ( y )     d &#x2061; y      {\displaystyle {\operatorname {d} \Gamma
_{(y)} \over \operatorname {d} y}}  [{\operatorname {d}\Gamma _{{(y)}} \over
\operatorname {d}y}]. The solution to this equation is a function,
&#x0393;  ( y )     {\displaystyle \Gamma _{(y)}}  [\Gamma _{{(y)}}], that
accurately describes the circulation (and therefore lift) distribution over a
finite wing of known geometry.
***** Derivation[edit] *****
(Based on.[8])
Nomenclature:
    *    &#xA0; &#x0393;   {\displaystyle \ \Gamma }  [\ \Gamma ] is the
      circulation over the entire wing (mÂ²/s)
    *    &#xA0;  C  L     {\displaystyle \ C_{L}}  [\ C_{L}] is the 3D lift
      coefficient (for the entire wing)
    *    &#xA0; A R   {\displaystyle \ AR}  [\ AR] is the aspect_ratio
    *    &#xA0;  &#x03B1;  &#x221E;     {\displaystyle \ \alpha _{\infty }}  [\
      \alpha _{\infty }] is the freestream angle_of_attack (rad)
    *    &#xA0;  V  &#x221E;     {\displaystyle \ V_{\infty }}  [\ V_{\infty }]
      is the freestream velocity (m/s)
    *    &#xA0;  C   D  i       {\displaystyle \ C_{D_{i}}}  [\ C_{{D_{i}}}] is
      the drag coefficient for induced_drag
    *    &#xA0; e   {\displaystyle \ e}  [\ e] is the planform_efficiency
      factor
The following are all functions of the wings span-wise station     y
{\displaystyle y}  [y] (i.e. they can all vary along the wing)
    *    &#xA0;  C  l     {\displaystyle \ C_{l}}  [\ C_{l}] is the 2D lift
      coefficient (units/m)
    *    &#xA0; &#x03B3;   {\displaystyle \ \gamma }  [\ \gamma ] is the 2D
      circulation at a section (m/s)
    *    &#xA0; c   {\displaystyle \ c}  [\ c] is the chord_length of the local
      section
    *    &#xA0;  &#x03B1;  g e o     {\displaystyle \ \alpha _{geo}}  [\ \alpha
      _{{geo}}] is the local change in angle of attack due to geometric twist
      of the wing
    *    &#xA0;  &#x03B1;  0     {\displaystyle \ \alpha _{0}}  [\ \alpha _{0}]
      is zero-lift angle of attack of that section (depends on the airfoil
      geometry)
    *    &#xA0;  C   l  &#x03B1;       {\displaystyle \ C_{l_{\alpha }}}  [\ C_
      {{l_{\alpha }}}] is the 2D lift coefficient slope (units/mârad, and
      depends on airfoil geometry, see Thin_airfoil_theory)
    *    &#xA0;  &#x03B1;  i     {\displaystyle \ \alpha _{i}}  [\ \alpha _{i}]
      is change in angle of attack due to downwash
    *    &#xA0;  w  i     {\displaystyle \ w_{i}}  [\ w_{i}] is the local
      downwash velocity
To derive the model we start with the assumption that the circulation of the
wing varies as a function of the spanwise locations. The function assumed is a
Fourier function. Firstly, the coordinate for the spanwise location     y
{\displaystyle y}  [y] is transformed by     y = s c o s  &#x03B8;
{\displaystyle y=scos{\theta }}  [y=scos{\theta }], where y is spanwise
location, and s is the semi-span of the wing.
[Prandtl-lifting-line-coordinate-change.PNG]
and so the circulation is assumed to be:
   &#x0393; ( y ) = &#x0393; ( &#x03B8; ) = &#x03B3; = 4 s  V  &#x221E;
&#x2211;  n     A  n   sin &#x2061; ( n &#x03B8;  )  ( 1 )   {\displaystyle
\Gamma (y)=\Gamma (\theta )=\gamma =4sV_{\infty }\sum _{n}{A_{n}\sin(n\theta
})\qquad (1)}  [\Gamma (y)=\Gamma (\theta )=\gamma =4sV_{\infty }\sum _{n}{A_
{n}\sin(n\theta })\qquad (1)]
Since the circulation of a section is related to the      C  l
{\displaystyle C_{l}}  [C_{l}] by the equation:
    C  l   =    2 &#x03B3;    V  &#x221E;   c     ( 2 )   {\displaystyle C_{l}=
{\frac {2\gamma }{V_{\infty }c}}\qquad (2)}  [C_{l}={\frac  {2\gamma }{V_
{\infty }c}}\qquad (2)]
but since the coefficient of lift is a function of angle of attack:
    C  l   =  C   l  &#x03B1;     (  &#x03B1;  &#x221E;   +  &#x03B1;  g e o
&#x2212;  &#x03B1;  0   &#x2212;  &#x03B1;  i   )  ( 3 )   {\displaystyle C_
{l}=C_{l_{\alpha }}(\alpha _{\infty }+\alpha _{geo}-\alpha _{0}-\alpha _
{i})\qquad (3)}  [C_{l}=C_{{l_{\alpha }}}(\alpha _{\infty }+\alpha _{{geo}}-
\alpha _{0}-\alpha _{i})\qquad (3)]
hence the vortex strength at any particular spanwise station can be given by
the equations:
   &#x03B3; =   1 2    V  &#x221E;   c  C   l  &#x03B1;     (  &#x03B1;
&#x221E;   +  &#x03B1;  g e o   &#x2212;  &#x03B1;  0   &#x2212;  &#x03B1;  i
)  ( 4 )   {\displaystyle \gamma ={\frac {1}{2}}V_{\infty }cC_{l_{\alpha }}
(\alpha _{\infty }+\alpha _{geo}-\alpha _{0}-\alpha _{i})\qquad (4)}  [\gamma =
{\frac  {1}{2}}V_{\infty }cC_{{l_{\alpha }}}(\alpha _{\infty }+\alpha _{{geo}}-
\alpha _{0}-\alpha _{i})\qquad (4)]
This one equation has two unknowns: the value for     &#x03B3;   {\displaystyle
\gamma }  [\gamma ] and the value for      &#x03B1;  i     {\displaystyle
\alpha _{i}}  [\alpha _{i}]. However, the downwash is purely a function of the
circulation only. So we can determine the value      &#x03B1;  i
{\displaystyle \alpha _{i}}  [\alpha _{i}] in terms of     &#x0393; ( y )
{\displaystyle \Gamma (y)}  [\Gamma (y)], bring this term across to the left
hand side of the equation and solve. The downwash at any given station is a
function of the entire shed vortex system. This is determined by integrating
the influence of each differential shed vortex over the span of the wing.
Differential element of circulation:
   d &#x0393; = 4 s  V  &#x221E;    &#x2211;  n = 1   &#x221E;   n  A  n   cos
&#x2061; ( n &#x03B8; )  ( 5 )   {\displaystyle d\Gamma =4sV_{\infty }\sum _
{n=1}^{\infty }nA_{n}\cos(n\theta )\qquad (5)}  [d\Gamma =4sV_{\infty }\sum _{
{n=1}}^{{\infty }}nA_{n}\cos(n\theta )\qquad (5)]
Differential downwash due to the differential element of circulation (acts like
half an infinite vortex line):
   d  w  i   =    d &#x0393;   4 &#x03C0; r     ( 6 )   {\displaystyle dw_{i}=
{\frac {d\Gamma }{4\pi r}}\qquad (6)}  [dw_{i}={\frac  {d\Gamma }{4\pi
r}}\qquad (6)]
The integral equation over the span of the wing to determine the downwash at a
particular location is:
    w  i   =  &#x222B;  &#x2212; s   s     1  y &#x2212;  y  0      d &#x0393;
( 7 )   {\displaystyle w_{i}=\int _{-s}^{s}{\frac {1}{y-y_{0}}}d\Gamma \qquad
(7)}  [w_{i}=\int _{{-s}}^{s}{\frac  {1}{y-y_{0}}}d\Gamma \qquad (7)]
After appropriate substitutions and integrations we get:
    w  i   =  V  &#x221E;    &#x2211;  n = 1   &#x221E;      n  A  n   sin
&#x2061; ( n &#x03B8; )   sin &#x2061; ( &#x03B8; )     ( 8 )   {\displaystyle
w_{i}=V_{\infty }\sum _{n=1}^{\infty }{\frac {nA_{n}\sin(n\theta )}{\sin(\theta
)}}\qquad (8)}  [w_{i}=V_{\infty }\sum _{{n=1}}^{{\infty }}{\frac  {nA_{n}\sin
(n\theta )}{\sin(\theta )}}\qquad (8)]
And so the change in angle attack is determined by (assuming_small_angles):
    &#x03B1;  i   =    w  i    V  &#x221E;      ( 9 )   {\displaystyle \alpha _
{i}={\frac {w_{i}}{V_{\infty }}}\qquad (9)}  [\alpha _{i}={\frac  {w_{i}}{V_
{\infty }}}\qquad (9)]
By substituting equations 8 and 9 into RHS of equation 4 and equation 1 into
the LHS of equation 4, we then get:
   4 s  V  &#x221E;    &#x2211;  n = 1   &#x221E;    A  n   sin &#x2061; ( n
&#x03B8; ) =   1 2    V  &#x221E;   c  C   l  &#x03B1;      [   &#x03B1;
&#x221E;   +  &#x03B1;  g e o   &#x2212;  &#x03B1;  0   &#x2212;  &#x2211;  n =
1   &#x221E;      n  A  n   sin &#x2061; ( n &#x03B8; )   sin &#x2061;
( &#x03B8; )     ]   ( 10 )   {\displaystyle 4sV_{\infty }\sum _{n=1}^{\infty
}A_{n}\sin(n\theta )={\frac {1}{2}}V_{\infty }cC_{l_{\alpha }}\left[\alpha _
{\infty }+\alpha _{geo}-\alpha _{0}-\sum _{n=1}^{\infty }{\frac {nA_{n}\sin
(n\theta )}{\sin(\theta )}}\right]\qquad (10)}  [4sV_{\infty }\sum _{{n=1}}^
{\infty }A_{n}\sin(n\theta )={\frac  {1}{2}}V_{\infty }cC_{{l_{\alpha }}}\left
[\alpha _{\infty }+\alpha _{{geo}}-\alpha _{0}-\sum _{{n=1}}^{{\infty }}{\frac
{nA_{n}\sin(n\theta )}{\sin(\theta )}}\right]\qquad (10)]
After rearranging, we get the series of simultaneous equations:
    &#x2211;  n = 1   &#x221E;    A  n   sin &#x2061; ( n &#x03B8; )   (   sin
&#x2061; ( &#x03B8; ) +    n  C  l &#x03B1;   c   8 s      )   =     C  l
&#x03B1;   c   8 s    sin &#x2061; ( &#x03B8; ) (  &#x03B1;  &#x221E;   +
&#x03B1;  g e o   &#x2212;  &#x03B1;  0   )  ( 11 )   {\displaystyle \sum _
{n=1}^{\infty }A_{n}\sin(n\theta ){\bigg (}\sin(\theta )+{\frac {nC_{l\alpha
}c}{8s}}{\bigg )}={\frac {C_{l\alpha }c}{8s}}\sin(\theta )(\alpha _{\infty
}+\alpha _{geo}-\alpha _{0})\qquad (11)}  [\sum _{{n=1}}^{\infty }A_{n}\sin
(n\theta ){\bigg (}\sin(\theta )+{\frac  {nC_{{l\alpha }}c}{8s}}{\bigg )}=
{\frac  {C_{{l\alpha }}c}{8s}}\sin(\theta )(\alpha _{\infty }+\alpha _{{geo}}-
\alpha _{0})\qquad (11)]
By taking a finite number of terms, equation 11 can be expressed in matrix form
and solved for coefficients A. Note the left-hand side of the equation
represents each element in the matrix, and the terms on the RHS of equation 11
represent the RHS of the matrix form. Each row in the matrix form represents a
different span-wise station, and each column represents a different value for
n.
Appropriate choices for     &#x03B8;   {\displaystyle \theta }  [\theta ] are
as a linear variation between     ( 0 , &#x03C0; )   {\displaystyle (0,\pi )}
[{\displaystyle (0,\pi )}]. Note that this range does not include the values
for 0 and     &#x03C0;   {\displaystyle \pi }  [\pi ], as this leads to a
singular matrix, which can't be solved.
***** Lift and drag from coefficients[edit] *****
The lift can be determined by integrating the circulation terms:
    Lift  = &#x03C1;  V  &#x221E;    &#x222B;  &#x2212; s   s   &#x0393; ( y )
cos &#x2061;  (  &#x03B1;  i   ( y ) )  d y &#x2248; &#x03C1;  V  &#x221E;
&#x222B;  &#x2212; s   s   &#x0393; ( y ) d y   {\displaystyle {\text
{Lift}}=\rho V_{\infty }\int _{-s}^{s}\Gamma (y)\cos {(\alpha _{i}
(y))}dy\approx \rho V_{\infty }\int _{-s}^{s}\Gamma (y)dy}  [{\displaystyle
{\text{Lift}}=\rho V_{\infty }\int _{-s}^{s}\Gamma (y)\cos {(\alpha _{i}
(y))}dy\approx \rho V_{\infty }\int _{-s}^{s}\Gamma (y)dy}]
which can be reduced to:
    C  L   = &#x03C0; A  R  A  1     {\displaystyle C_{L}=\pi A\!RA_{1}}  [C_
{L}=\pi A\!RA_{1}]
where      A  1     {\displaystyle A_{1}}  [A_{1}] is the first term of the
solution of the simultaneous equations shown above.
The induced drag can be determined from
     Drag   induced   = &#x03C1;  V  &#x221E;    &#x222B;  &#x2212; s   s
&#x0393; ( y ) sin &#x2061;  (  &#x03B1;  i   ( y ) )  d y &#x2248; &#x03C1;  V
&#x221E;    &#x222B;  &#x2212; s   s   &#x0393; ( y )  &#x03B1;  i   ( y ) d y
{\displaystyle {\text{Drag}}_{\text{induced}}=\rho V_{\infty }\int _{-s}^
{s}\Gamma (y)\sin {(\alpha _{i}(y))}dy\approx \rho V_{\infty }\int _{-s}^
{s}\Gamma (y)\alpha _{i}(y)dy}  [{\displaystyle {\text{Drag}}_{\text
{induced}}=\rho V_{\infty }\int _{-s}^{s}\Gamma (y)\sin {(\alpha _{i}
(y))}dy\approx \rho V_{\infty }\int _{-s}^{s}\Gamma (y)\alpha _{i}(y)dy}]
which can also be reduced to:
    C   D  induced     = &#x03C0; A  R  &#x2211;  n = 1   &#x221E;   n  A  n
2     {\displaystyle C_{D_{\text{induced}}}=\pi A\!R\sum _{n=1}^{\infty }nA_
{n}^{2}}  [{\displaystyle C_{D_{\text{induced}}}=\pi A\!R\sum _{n=1}^{\infty
}nA_{n}^{2}}]
where      A  n     {\displaystyle A_{n}}  [{\displaystyle A_{n}}] are all the
terms of the solution of the simultaneous equations shown above.
Moreover, this expression may be arranged as a function of      C  L
{\displaystyle C_{L}}  [{\displaystyle C_{L}}] in the following way :
    C   D  induced     = &#x03C0; A  R  A  1   2   + &#x03C0; A  R  &#x2211;  n
= 2   &#x221E;   n  A  n   2     {\displaystyle C_{D_{\text{induced}}}=\pi
A\!RA_{1}^{2}+\pi A\!R\sum _{n=2}^{\infty }nA_{n}^{2}}  [{\displaystyle C_{D_
{\text{induced}}}=\pi A\!RA_{1}^{2}+\pi A\!R\sum _{n=2}^{\infty }nA_{n}^{2}}]
    C   D  induced     = &#x03C0; A  R  A  1   2   &#x2217;    &#x03C0; A  R
&#x03C0; A  R    + &#x03C0; A  R  &#x2211;  n = 2   &#x221E;   n  A  n   2
&#x2217;    &#x03C0; A  R  A  1   2     &#x03C0; A  R  A  1   2
{\displaystyle C_{D_{\text{induced}}}=\pi A\!RA_{1}^{2}*{\frac {\pi A\!R}{\pi
A\!R}}+\pi A\!R\sum _{n=2}^{\infty }nA_{n}^{2}*{\frac {\pi A\!RA_{1}^{2}}{\pi
A\!RA_{1}^{2}}}}  [{\displaystyle C_{D_{\text{induced}}}=\pi A\!RA_{1}^{2}*
{\frac {\pi A\!R}{\pi A\!R}}+\pi A\!R\sum _{n=2}^{\infty }nA_{n}^{2}*{\frac
{\pi A\!RA_{1}^{2}}{\pi A\!RA_{1}^{2}}}}]
    C   D  induced     =     &#x03C0;  2   A   R  2    A  1   2     &#x03C0; A
R    +     &#x03C0;  2   A   R  2    A  1   2     &#x03C0; A  R    &#x2217;
&#x2211;  n = 2   &#x221E;   n  A  n   2     A  1   2       {\displaystyle C_
{D_{\text{induced}}}={\frac {\pi ^{2}A\!R^{2}A_{1}^{2}}{\pi A\!R}}+{\frac {\pi
^{2}A\!R^{2}A_{1}^{2}}{\pi A\!R}}*{\frac {\sum _{n=2}^{\infty }nA_{n}^{2}}{A_
{1}^{2}}}}  [{\displaystyle C_{D_{\text{induced}}}={\frac {\pi ^{2}A\!R^{2}A_
{1}^{2}}{\pi A\!R}}+{\frac {\pi ^{2}A\!R^{2}A_{1}^{2}}{\pi A\!R}}*{\frac {\sum
_{n=2}^{\infty }nA_{n}^{2}}{A_{1}^{2}}}}]
    C   D  induced     =    C  L   2    &#x03C0; A  R    ( 1 +     &#x2211;  n
= 2   &#x221E;   n  A  n   2     A  1   2     ) =    C  L   2    &#x03C0; A  R
e      {\displaystyle C_{D_{\text{induced}}}={\frac {C_{L}^{2}}{\pi A\!R}}(1+
{\frac {\sum _{n=2}^{\infty }nA_{n}^{2}}{A_{1}^{2}}})={\frac {C_{L}^{2}}{\pi
A\!Re}}}  [{\displaystyle C_{D_{\text{induced}}}={\frac {C_{L}^{2}}{\pi A\!R}}
(1+{\frac {\sum _{n=2}^{\infty }nA_{n}^{2}}{A_{1}^{2}}})={\frac {C_{L}^{2}}{\pi
A\!Re}}}]
where
   &#x03B4; =     &#x2211;  n = 2   &#x221E;   n  A  n   2     A  1   2
{\displaystyle \delta ={\frac {\sum _{n=2}^{\infty }nA_{n}^{2}}{A_{1}^{2}}}}  [
{\displaystyle \delta ={\frac {\sum _{n=2}^{\infty }nA_{n}^{2}}{A_{1}^{2}}}}]
   e =   1  1 + &#x03B4;      {\displaystyle e={\frac {1}{1+\delta }}}  [
{\displaystyle e={\frac {1}{1+\delta }}}] is the span_efficiency_factor
***** Symmetric wing[edit] *****
For a symmetric wing, the even terms of the series coefficients are identically
equal to 0, and so can be dropped.
***** Rolling wings[edit] *****
When the aircraft is rolling, an additional term can be added that adds the
wing station distance multiplied by the rate of roll to give additional angle
of attack change. Equation 3 then becomes:
    C  l   =  C   l  &#x03B1;      (   &#x03B1;  &#x221E;   +  &#x03B1;  g e o
&#x2212;  &#x03B1;  0   &#x2212;  &#x03B1;  i   +    p y  s    )   ( 3 )
{\displaystyle C_{l}=C_{l_{\alpha }}\left(\alpha _{\infty }+\alpha _{geo}-
\alpha _{0}-\alpha _{i}+{\frac {py}{s}}\right)\qquad (3)}  [C_{l}=C_{{l_{
{\alpha }}}}\left(\alpha _{{\infty }}+\alpha _{{geo}}-\alpha _{0}-\alpha _{i}+
{\frac  {py}{s}}\right)\qquad (3)]
where
    *    &#xA0; p   {\displaystyle \ p}  [\ p] is the rate of roll in rad/sec,
Note that y can be negative, which introduces non-zero even coefficients in the
equation that must be accounted for.
***** Control deflection[edit] *****
The effect of ailerons can be accounted by simply changing      &#x03B1;  0
{\displaystyle \alpha _{0}}  [\alpha _{0}] term in Equation 3. For non-
symmetric controls such as ailerons the      &#x03B1;  0     {\displaystyle
\alpha _{0}}  [\alpha _{0}] term changes on each side of the wing.
***** Elliptical wings[edit] *****
For an elliptical wing with no twist, with:
   y ( &#x03B8; ) = s cos &#x2061; ( &#x03B8; )   {\displaystyle y(\theta
)=s\cos(\theta )}  [{\displaystyle y(\theta )=s\cos(\theta )}]
The chord length is given as a function of span location as:
   c ( &#x03B8; ) =  c  r o o t   sin &#x2061; ( &#x03B8; )   {\displaystyle c
(\theta )=c_{root}\sin(\theta )}  [{\displaystyle c(\theta )=c_{root}\sin
(\theta )}]
Also,
   e = 1   {\displaystyle e=1}  [{\displaystyle e=1}]
This yields the famous equation for the elliptic induced drag coefficient:
    C   D  i n d u c e d     =    C  L   2    &#x03C0; A  R      {\displaystyle
C_{D_{induced}}={\frac {C_{L}^{2}}{\pi A\!R}}}  [{\displaystyle C_{D_
{induced}}={\frac {C_{L}^{2}}{\pi A\!R}}}]
where
    *    s   {\displaystyle s}  [s] is the value of the wing span,
    *    y ( &#x03B8; )   {\displaystyle y(\theta )}  [{\displaystyle y(\theta
      )}] is the position on the wing span, and
    *    c ( &#x03B8; )   {\displaystyle c(\theta )}  [{\displaystyle c(\theta
      )}] is the chord.
***** Useful approximations[edit] *****
A useful approximation[citation_needed] is that
         &#xA0;  C  L   =  C   l  &#x03B1;      (   AR   AR  + 2    )  &#x03B1;
      {\displaystyle \ C_{L}=C_{l_{\alpha }}\left({\frac {\text{AR}}{{\text
      {AR}}+2}}\right)\alpha }  [{\displaystyle \ C_{L}=C_{l_{\alpha }}\left(
      {\frac {\text{AR}}{{\text{AR}}+2}}\right)\alpha }]
where
    *    &#xA0;  C  L     {\displaystyle \ C_{\text{L}}}  [{\displaystyle \ C_
      {\text{L}}}] is the 3D lift_coefficient for elliptical circulation
      distribution,
    *    &#xA0;  C   l  &#x03B1;       {\displaystyle \ C_{l_{\alpha }}}  [\ C_
      {{l_{\alpha }}}] is the 2D lift coefficient slope (see Thin_Airfoil
      Theory),
    *    &#xA0;  AR    {\displaystyle \ {\text{AR}}}  [\ {\text{AR}}] is the
      aspect_ratio, and
    *    &#xA0; &#x03B1;   {\displaystyle \ \alpha }  [\ \alpha ] is the angle
      of_attack in radians.
The theoretical value for     &#xA0;  C   l  &#x03B1;       {\displaystyle \ C_
{l_{\alpha }}}  [\ C_{{l_{\alpha }}}] is 2    &#x03C0;   {\displaystyle \pi }
[\pi ]. Note that this equation becomes the thin_airfoil equation if AR goes to
infinity.[9]
As seen above, the lifting-line theory also states an equation for induced
drag:.[10][11]
         &#xA0;  C   D  i     =      C  L     2    &#x03C0;  AR  e
      {\displaystyle \ C_{D_{i}}={\frac {{C_{L}}^{2}}{\pi {\text{AR}}e}}}  [\
      C_{{D_{i}}}={\frac  {{C_{L}}^{2}}{\pi {\text{AR}}e}}]
where
    *    &#xA0;  C   D  i       {\displaystyle \ C_{D_{i}}}  [\ C_{{D_{i}}}] is
      the drag coefficient for induced drag,
    *    &#xA0;  C  L     {\displaystyle \ C_{L}}  [\ C_{L}] is the 3D lift
      coefficient, and
    *    &#xA0;  AR    {\displaystyle \ {\text{AR}}}  [\ {\text{AR}}] is the
      aspect_ratio.
    *    &#xA0; e   {\displaystyle \ e}  [\ e] is the planform efficiency
      factor (equals 1 for elliptical circulation distribution, and usually
      tabulated for other distributions).
***** Limitations of the theory[edit] *****
The lifting line theory does not take into account the following:
    * Compressible_flow
    * Viscous_flow
    * Swept_wings
    * Low_aspect_ratio wings
    * Unsteady_flows
***** See also[edit] *****
    * Horseshoe_vortex
    * Thin_Airfoil_Theory
    * Vortex_lattice_method
***** Notes[edit] *****
   1. ^ Anderson, John D. (2001), Fundamental of aerodynamics, McGraw-Hill,
      Boston.
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
   3. ISBN 0-07-237335-0. p360
   4. ^Houghton, E. L.; Carpenter, P.W. (2003). Butterworth Heinmann (ed.).
      Aerodynamics for Engineering Students (5th ed.). ISBN 0-7506-5111-3.
   5. ^KÃ¡rmÃ¡n,_Theodore_von (1954). Cornell University Press (reproduced by
      Dover in 2004) (ed.). Aerodynamics: Selected Topics in the Light of their
      Historical Development. ISBN 0-486-43485-0.
   6. ^Lanchester,_Frederick_W. (1907). Constable (ed.). Aerodynamics.
   7. ^Prandtl,_Ludwig (1918). KÃ¶nigliche Gesellschaft der Wissenschaften zu
      GÃ¶ttingen (ed.). TragflÃ¼geltheorie.
   8. ^ Abbott,_Ira_H., and Von Doenhoff, Albert E., Theory of Wing Sections,
      Section 1.4
   9. ^ Clancy, L.J., Aerodynamics, Section 8.11
  10. ^ Sydney_University's_Aerodynamics_for_Students_(pdf)
  11. ^ Aerospace_Web's_explanation_of_lift_coefficient
  12. ^ Abbott, Ira H., and Von Doenhoff, Albert E., Theory of Wing Sections,
      Section 1.3
  13. ^ Clancy, L.J., Aerodynamics, Equation 5.7
***** References[edit] *****
    * Clancy, L.J. (1975), Aerodynamics, Pitman Publishing Limited, London.
ISBN 0-273-01120-0
Abbott, Ira H., and Von Doenhoff, Albert E. (1959), Theory of Wing Sections,
Dover Publications Inc., New York. Standard Book Number 486-60586-8

Retrieved from "https://en.wikipedia.org/w/index.php?title=Lifting-
line_theory&oldid=909251961"
Categories:
    * Aerodynamics
Hidden categories:
    * Articles_with_short_description
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_August_2019
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
    * FranÃ§ais
Edit_links
    * This page was last edited on 4 August 2019, at 05:31 (UTC).
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
