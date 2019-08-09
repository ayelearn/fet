The following text has been accessed from https://en.wikipedia.org/wiki/Particle_in_a_box at Fri Aug 9 03:12:00 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Particle in a box ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Physical model in quantum mechanics which is analytically solvable
Some trajectories of a particle in a box according to Newton's_laws of
classical_mechanics (A), and according to the SchrÃ¶dinger_equation of quantum
mechanics (BâF). In (BâF), the horizontal axis is position, and the
vertical axis is the real part (blue) and imaginary part (red) of the
wavefunction. The states (B,C,D) are energy_eigenstates, but (E,F) are not.
In quantum_mechanics, the particle in a box model (also known as the infinite
potential well or the infinite square well) describes a particle free to move
in a small space surrounded by impenetrable barriers. The model is mainly used
as a hypothetical example to illustrate the differences between classical and
quantum systems. In classical systems, for example, a particle trapped inside a
large box can move at any speed within the box and it is no more likely to be
found at one position than another. However, when the well becomes very narrow
(on the scale of a few nanometers), quantum effects become important. The
particle may only occupy certain positive energy_levels. Likewise, it can never
have zero energy, meaning that the particle can never "sit still".
Additionally, it is more likely to be found at certain positions than at
others, depending on its energy level. The particle may never be detected at
certain positions, known as spatial nodes.
The particle in a box model is one of the very few problems in quantum
mechanics which can be solved analytically, without approximations. Due to its
simplicity, the model allows insight into quantum effects without the need for
complicated mathematics. It serves as a simple illustration of how energy
quantizations (energy levels), which are found in more complicated quantum
systems such as atoms and molecules, come about. It is one of the first quantum
mechanics problems taught in undergraduate physics courses, and it is commonly
used as an approximation for more complicated quantum systems.
⁰
***** Contents *****
    * 1_One-dimensional_solution
          o 1.1_Position_wave_function
          o 1.2_Momentum_wave_function
          o 1.3_Position_and_momentum_probability_distributions
          o 1.4_Energy_levels
    * 2_Higher-dimensional_boxes
          o 2.1_(Hyper)rectangular_walls
          o 2.2_More_complicated_wall_shapes
    * 3_Applications
          o 3.1_Conjugated_polyenes
          o 3.2_Quantum_well_laser
                # 3.2.1_Quantum_dots
    * 4_Relativistic_Effects
    * 5_See_also
    * 6_References
    * 7_Bibliography
    * 8_External_links
***** One-dimensional solution[edit] *****
The barriers outside a one-dimensional box have infinitely large potential,
while the interior of the box has a constant, zero potential.
The simplest form of the particle in a box model considers a one-dimensional
system. Here, the particle may only move backwards and forwards along a
straight line with impenetrable barriers at either end.[1] The walls of a one-
dimensional box may be visualised as regions of space with an infinitely large
potential_energy. Conversely, the interior of the box has a constant, zero
potential energy.[2] This means that no forces act upon the particle inside the
box and it can move freely in that region. However, infinitely large forces
repel the particle if it touches the walls of the box, preventing it from
escaping. The potential energy in this model is given as
         V ( x ) =   {    0 ,    x  c   &#x2212;    L 2    < x <  x  c   +    L
      2    ,     &#x221E; ,    otherwise,        ,   {\displaystyle V(x)=
      {\begin{cases}0,&x_{c}-{\tfrac {L}{2}}<x<x_{c}+{\tfrac {L}{2}},\\\infty
      ,&{\text{otherwise,}}\end{cases}},}  [{\displaystyle V(x)={\begin
      {cases}0,&x_{c}-{\tfrac {L}{2}}<x<x_{c}+{\tfrac {L}{2}},\\\infty ,&{\text
      {otherwise,}}\end{cases}},}]
where L is the length of the box, xc is the location of the center of the box
and x is the position of the particle within the box. Simple cases include the
centered box (xc = 0) and the shifted box (xc = L/2).
**** Position wave function[edit] ****
In quantum mechanics, the wavefunction gives the most fundamental description
of the behavior of a particle; the measurable properties of the particle (such
as its position, momentum and energy) may all be derived from the wavefunction.
[3] The wavefunction     &#x03C8; ( x , t )   {\displaystyle \psi (x,t)}  [\psi
(x,t)] can be found by solving the SchrÃ¶dinger_equation for the system
         i &#x210F;   &#x2202;  &#x2202; t    &#x03C8; ( x , t ) = &#x2212;
      &#x210F;  2    2 m       &#x2202;  2    &#x2202;  x  2      &#x03C8; ( x
      , t ) + V ( x ) &#x03C8; ( x , t ) ,   {\displaystyle i\hbar {\frac
      {\partial }{\partial t}}\psi (x,t)=-{\frac {\hbar ^{2}}{2m}}{\frac
      {\partial ^{2}}{\partial x^{2}}}\psi (x,t)+V(x)\psi (x,t),}  [i\hbar
      {\frac {\partial }{\partial t}}\psi (x,t)=-{\frac {\hbar ^{2}}{2m}}{\frac
      {\partial ^{2}}{\partial x^{2}}}\psi (x,t)+V(x)\psi (x,t),]
where     &#x210F;   {\displaystyle \hbar }  [\hbar ] is the reduced_Planck
constant,     m   {\displaystyle m}  [m] is the mass of the particle,     i
{\displaystyle i}  [i] is the imaginary_unit and     t   {\displaystyle t}  [t]
is time.
Inside the box, no forces act upon the particle, which means that the part of
the wavefunction inside the box oscillates through space and time with the same
form as a free_particle:[1][4]
         &#x03C8; ( x , t ) = [ A sin &#x2061; ( k x ) + B cos
      &#x2061; ( k x ) ]   e   &#x2212; i &#x03C9; t   ,                
      {\displaystyle \psi (x,t)=[A\sin(kx)+B\cos(kx)]\mathrm {e} ^{-      (1)
      i\omega t},}  [\psi (x,t)=[A\sin(kx)+B\cos(kx)]\mathrm {e} ^{-
      i\omega t},]
where     A   {\displaystyle A}  [A] and     B   {\displaystyle B}  [B] are
arbitrary complex_numbers. The frequency of the oscillations through space and
time is given by the wavenumber     k   {\displaystyle k}  [k] and the angular
frequency     &#x03C9;   {\displaystyle \omega }  [\omega ] respectively. These
are both related to the total energy of the particle by the expression
         E = &#x210F; &#x03C9; =     &#x210F;  2    k  2     2 m    ,
      {\displaystyle E=\hbar \omega ={\frac {\hbar ^{2}k^{2}}{2m}},}  [E=\hbar
      \omega ={\frac {\hbar ^{2}k^{2}}{2m}},]
which is known as the dispersion_relation for a free particle.[1] Here one must
notice that now, since the particle is not entirely free but under the
influence of a potential (the potential V described above), the energy of the
particle given above is not the same thing as        p  2    2 m
{\displaystyle {\frac {p^{2}}{2m}}}  [{\frac {p^{2}}{2m}}] where p is the
momentum of the particle, and thus the wavenumber k above actually describes
the energy states of the particle, not the momentum states (i.e. it turns out
that the momentum of the particle is not given by     p = &#x210F; k
{\displaystyle p=\hbar k}  [p=\hbar k]). In this sense, it is quite dangerous
to call the number k a wavenumber, since it is not related to momentum like
"wavenumber" usually is. The rationale for calling k the wavenumber is that it
enumerates the number of crests that the wavefunction has inside the box, and
in this sense it is a wavenumber. This discrepancy can be seen more clearly
below, when we find out that the energy spectrum of the particle is discrete
(only discrete values of energy are allowed) but the momentum spectrum is
continuous (momentum can vary continuously) and in particular, the relation
E =    p  2    2 m      {\displaystyle E={\frac {p^{2}}{2m}}}  [E={\frac {p^
{2}}{2m}}] for the energy and momentum of the particle does not hold. As said
above, the reason this relation between energy and momentum does not hold is
that the particle is not free, but there is a potential V in the system, and
the energy of the particle is     E = T + V   {\displaystyle E=T+V}  [E=T+V],
where T is the kinetic and V the potential energy.
Initial wavefunctions for the first four states in a one-dimensional particle
in a box
The size (or amplitude) of the wavefunction at a given position is related to
the probability of finding a particle there by     P ( x , t ) =  |  &#x03C8;
( x , t )   |   2     {\displaystyle P(x,t)=|\psi (x,t)|^{2}}  [P(x,t)=|\psi
(x,t)|^{2}]. The wavefunction must therefore vanish everywhere beyond the edges
of the box.[1][4] Also, the amplitude of the wavefunction may not "jump"
abruptly from one point to the next.[1] These two conditions are only satisfied
by wavefunctions with the form
          &#x03C8;  n   ( x , t ) =   {    A sin &#x2061;  (   k  n    (  x
      &#x2212;  x  c   +    L 2     )   )    e   &#x2212; i  &#x03C9;  n   t
      ,    x  c   &#x2212;    L 2    < x <  x  c   +    L 2    ,     0 ,
      otherwise,          {\displaystyle \psi _{n}(x,t)={\begin{cases}A\sin
      \left(k_{n}\left(x-x_{c}+{\tfrac {L}{2}}\right)\right)\mathrm {e} ^{-
      i\omega _{n}t},&x_{c}-{\tfrac {L}{2}}<x<x_{c}+{\tfrac {L}{2}},\\0,&{\text
      {otherwise,}}\end{cases}}}  [{\displaystyle \psi _{n}(x,t)={\begin
      {cases}A\sin \left(k_{n}\left(x-x_{c}+{\tfrac {L}
      {2}}\right)\right)\mathrm {e} ^{-i\omega _{n}t},&x_{c}-{\tfrac {L}
      {2}}<x<x_{c}+{\tfrac {L}{2}},\\0,&{\text{otherwise,}}\end{cases}}}]
where [5]
          k  n   =    n &#x03C0;  L     {\displaystyle k_{n}={\frac {n\pi }
      {L}}}  [{\displaystyle k_{n}={\frac {n\pi }{L}}}],
and
          E  n   = &#x210F;  &#x03C9;  n   =     n  2    &#x03C0;  2
      &#x210F;  2     2 m  L  2        {\displaystyle E_{n}=\hbar \omega _{n}=
      {\frac {n^{2}\pi ^{2}\hbar ^{2}}{2mL^{2}}}}  [{\displaystyle E_{n}=\hbar
      \omega _{n}={\frac {n^{2}\pi ^{2}\hbar ^{2}}{2mL^{2}}}}],
where n is a positive integer (1,2,3,4...). For a shifted box (xc = L/2), the
solution is particularly simple. The simplest solutions,      k  n   = 0
{\displaystyle k_{n}=0}  [k_{n}=0] or     A = 0   {\displaystyle A=0}  [A=0]
both yield the trivial wavefunction     &#x03C8; ( x ) = 0   {\displaystyle
\psi (x)=0}  [\psi (x)=0], which describes a particle that does not exist
anywhere in the system.[6] Negative values of     n   {\displaystyle n}  [n]
are neglected, since they give wavefunctions identical to the positive     n
{\displaystyle n}  [n] solutions except for a physically unimportant sign
change.[6] Here one sees that only a discrete set of energy values and
wavenumbers k are allowed for the particle. Usually in quantum mechanics it is
also demanded that the derivative of the wavefunction in addition to the
wavefunction itself be continuous; here this demand would lead to the only
solution being the constant zero function, which is not what we desire, so we
give up this demand (as this system with infinite potential can be regarded as
a nonphysical abstract limiting case, we can treat it as such and "bend the
rules"). Note that giving up this demand means that the wavefunction is not a
differentiable function at the boundary of the box, and thus it can be said
that the wavefunction does not solve the SchrÃ¶dinger equation at the boundary
points     x = 0   {\displaystyle x=0}  [x=0] and     x = L   {\displaystyle
x=L}  [x=L] (but does solve everywhere else).
Finally, the unknown constant     A   {\displaystyle A}  [A] may be found by
normalizing_the_wavefunction so that the total probability density of finding
the particle in the system is 1. It follows that
          | A |  =    2 L    .   {\displaystyle \left|A\right|={\sqrt {\frac
      {2}{L}}}.}  [\left|A\right|={\sqrt {\frac {2}{L}}}.]
Thus, A may be any complex number with absolute_value √2/L; these different
values of A yield the same physical state, so A = √2/L can be selected to
simplify.
It is expected that the eigenvalues, i.e., the energy      E  n
{\displaystyle E_{n}}  [E_{n}] of the box should be the same regardless of its
position in space, but      &#x03C8;  n   ( x , t )   {\displaystyle \psi _{n}
(x,t)}  [\psi _{n}(x,t)] changes. Notice that      x  c   &#x2212;    L 2     L
{\displaystyle x_{c}-{\tfrac {L}{2}}{L}}  [{\displaystyle x_{c}-{\tfrac {L}{2}}
{L}}] represents a phase shift in the wave function, This phase shift has no
effect when solving the SchrÃ¶dinger equation, and therefore does not affect
the eigenvalue.
**** Momentum wave function[edit] ****
The momentum wavefunction is proportional to the Fourier_transform of the
position wavefunction. With     k = p  /  &#x210F;   {\displaystyle k=p/\hbar }
[k=p/\hbar ] (note that the parameter k describing the momentum wavefunction
below is not exactly the special kn above, linked to the energy eigenvalues),
the momentum wavefunction is given by
          &#x03D5;  n   ( p , t ) =   1  2 &#x03C0; &#x210F;     &#x222B;
      &#x2212; &#x221E;   &#x221E;    &#x03C8;  n   ( x , t )  e  &#x2212; i k
      x    d x =    L  &#x03C0; &#x210F;      (    n &#x03C0;   n &#x03C0; + k
      L    )     sinc    (     1 2    ( n &#x03C0; &#x2212; k L )  )   e
      &#x2212; i k  x  c      e  i ( n &#x2212; 1 )    &#x03C0; 2       e
      &#x2212; i  &#x03C9;  n   t   ,   {\displaystyle \phi _{n}(p,t)={\frac
      {1}{\sqrt {2\pi \hbar }}}\int _{-\infty }^{\infty }\psi _{n}(x,t)e^{-
      ikx}\,dx={\sqrt {\frac {L}{\pi \hbar }}}\left({\frac {n\pi }{n\pi
      +kL}}\right)\,{\textrm {sinc}}\left({\tfrac {1}{2}}(n\pi -kL)\right)e^{-
      ikx_{c}}e^{i(n-1){\tfrac {\pi }{2}}}e^{-i\omega _{n}t},}  [{\displaystyle
      \phi _{n}(p,t)={\frac {1}{\sqrt {2\pi \hbar }}}\int _{-\infty }^{\infty
      }\psi _{n}(x,t)e^{-ikx}\,dx={\sqrt {\frac {L}{\pi \hbar }}}\left({\frac
      {n\pi }{n\pi +kL}}\right)\,{\textrm {sinc}}\left({\tfrac {1}{2}}(n\pi -
      kL)\right)e^{-ikx_{c}}e^{i(n-1){\tfrac {\pi }{2}}}e^{-i\omega _{n}t},}]
where sinc is the cardinal sine sinc_function, sinc(x)=sin(x)/x. For the
centered box (xc= 0), the solution is real and particularly simple, since the
phase factor on the right reduces to unity. (With care, it can be written as an
even function of p.)
It can be seen that the momentum spectrum in this wave packet is continuous,
and one may conclude that for the energy state described by the wavenumber kn,
the momentum can, when measured, also attain other values beyond     p =
&#x00B1; &#x210F;  k  n     {\displaystyle p=\pm \hbar k_{n}}  [p=\pm \hbar k_
{n}].
Hence, it also appears that, since the energy is      E  n   =     &#x210F;  2
k  n   2     2 m      {\displaystyle E_{n}={\frac {\hbar ^{2}k_{n}^{2}}{2m}}}
[E_{n}={\frac {\hbar ^{2}k_{n}^{2}}{2m}}] for the nth eigenstate, the relation
E =    p  2    2 m      {\displaystyle E={\frac {p^{2}}{2m}}}  [E={\frac {p^
{2}}{2m}}] does not strictly hold for the measured momentum p; the energy
eigenstate      &#x03C8;  n     {\displaystyle \psi _{n}}  [\psi _{n}] is not a
momentum eigenstate, and, in fact, not even a superposition of two momentum
eigenstates, as one might be tempted to imagine from equation (1) above:
peculiarly, it has no well-defined momentum before measurement!
**** Position and momentum probability distributions[edit] ****
In classical physics, the particle can be detected anywhere in the box with
equal probability. In quantum mechanics, however, the probability density for
finding a particle at a given position is derived from the wavefunction as
P ( x ) =  |  &#x03C8; ( x )   |   2   .   {\displaystyle P(x)=|\psi (x)|^{2}.}
[P(x)=|\psi (x)|^{2}.] For the particle in a box, the probability density for
finding the particle at a given position depends upon its state, and is given
by
          P  n   ( x , t ) =   {      2 L    sin  2   &#x2061; (  k  n   ( x
      &#x2212;  x  c   +    L 2    ) ) ,    x  c   &#x2212; L  /  2 < x <  x  c
      + L  /  2 ,     0 ,    otherwise,          {\displaystyle P_{n}(x,t)=
      {\begin{cases}{\frac {2}{L}}\sin ^{2}(k_{n}(x-x_{c}+{\tfrac {L}{2}})),&x_
      {c}-L/2<x<x_{c}+L/2,\\0,&{\text{otherwise,}}\end{cases}}}  [
      {\displaystyle P_{n}(x,t)={\begin{cases}{\frac {2}{L}}\sin ^{2}(k_{n}(x-
      x_{c}+{\tfrac {L}{2}})),&x_{c}-L/2<x<x_{c}+L/2,\\0,&{\text
      {otherwise,}}\end{cases}}}]
Thus, for any value of n greater than one, there are regions within the box for
which     P ( x ) = 0   {\displaystyle P(x)=0}  [P(x)=0], indicating that
spatial nodes exist at which the particle cannot be found.
In quantum mechanics, the average, or expectation_value of the position of a
particle is given by
         &#x27E8; x &#x27E9; =  &#x222B;  &#x2212; &#x221E;   &#x221E;   x  P
      n   ( x )   d  x .   {\displaystyle \langle x\rangle =\int _{-\infty }^
      {\infty }xP_{n}(x)\,\mathrm {d} x.}  [\langle x\rangle =\int _{-\infty }^
      {\infty }xP_{n}(x)\,\mathrm {d} x.]
For the steady state particle in a box, it can be shown that the average
position is always     &#x27E8; x &#x27E9; =  x  c     {\displaystyle \langle
x\rangle =x_{c}}  [{\displaystyle \langle x\rangle =x_{c}}], regardless of the
state of the particle. For a superposition of states, the expectation value of
the position will change based on the cross term which is proportional to
cos &#x2061; ( &#x03C9; t )   {\displaystyle \cos(\omega t)}  [\cos(\omega t)].
The variance in the position is a measure of the uncertainty in position of the
particle:
          V a r  ( x ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;   ( x &#x2212;
      &#x27E8; x &#x27E9;  )  2    P  n   ( x )  d x =    L  2   12    (  1
      &#x2212;   6   n  2    &#x03C0;  2       )    {\displaystyle \mathrm
      {Var} (x)=\int _{-\infty }^{\infty }(x-\langle x\rangle )^{2}P_{n}
      (x)\,dx={\frac {L^{2}}{12}}\left(1-{\frac {6}{n^{2}\pi ^{2}}}\right)}
      [\mathrm {Var} (x)=\int _{-\infty }^{\infty }(x-\langle x\rangle )^{2}P_
      {n}(x)\,dx={\frac {L^{2}}{12}}\left(1-{\frac {6}{n^{2}\pi ^{2}}}\right)]
The probability density for finding a particle with a given momentum is derived
from the wavefunction as     P ( x ) =  |  &#x03D5; ( x )   |   2
{\displaystyle P(x)=|\phi (x)|^{2}}  [{\displaystyle P(x)=|\phi (x)|^{2}}]. As
with position, the probability density for finding the particle at a given
momentum depends upon its state, and is given by
          P  n   ( p ) =   L  &#x03C0; &#x210F;      (    n &#x03C0;   n
      &#x03C0; + k L    )   2       sinc    2    (     1 2    ( n &#x03C0;
      &#x2212; k L )  )    {\displaystyle P_{n}(p)={\frac {L}{\pi \hbar }}\left
      ({\frac {n\pi }{n\pi +kL}}\right)^{2}\,{\textrm {sinc}}^{2}\left({\tfrac
      {1}{2}}(n\pi -kL)\right)}  [{\displaystyle P_{n}(p)={\frac {L}{\pi \hbar
      }}\left({\frac {n\pi }{n\pi +kL}}\right)^{2}\,{\textrm {sinc}}^{2}\left(
      {\tfrac {1}{2}}(n\pi -kL)\right)}]
where, again,     k = p  /  &#x210F;   {\displaystyle k=p/\hbar }  [k=p/\hbar
]. The expectation value for the momentum is then calculated to be zero, and
the variance in the momentum is calculated to be:
          V a r  ( p ) =   (    &#x210F; n &#x03C0;  L   )   2
      {\displaystyle \mathrm {Var} (p)=\left({\frac {\hbar n\pi }{L}}\right)^
      {2}}  [\mathrm {Var} (p)=\left({\frac {\hbar n\pi }{L}}\right)^{2}]
The uncertainties in position and momentum (    &#x0394; x   {\displaystyle
\Delta x}  [\Delta x] and     &#x0394; p   {\displaystyle \Delta p}  [\Delta
p]) are defined as being equal to the square root of their respective
variances, so that:
         &#x0394; x &#x0394; p =   &#x210F; 2         n  2    &#x03C0;  2    3
      &#x2212; 2     {\displaystyle \Delta x\Delta p={\frac {\hbar }{2}}{\sqrt
      {{\frac {n^{2}\pi ^{2}}{3}}-2}}}  [\Delta x\Delta p={\frac {\hbar }{2}}
      {\sqrt {{\frac {n^{2}\pi ^{2}}{3}}-2}}]
This product increases with increasing n, having a minimum value for n=1. The
value of this product for n=1 is about equal to 0.568     &#x210F;
{\displaystyle \hbar }  [\hbar ] which obeys the Heisenberg_uncertainty
principle, which states that the product will be greater than or equal to
&#x210F;  /  2   {\displaystyle \hbar /2}  [\hbar /2]
Another measure of uncertainty in position is the information_entropy of the
probability distribution Hx:[7]
          H  x   =  &#x222B;  &#x2212; &#x221E;   &#x221E;    P  n   ( x ) log
      &#x2061; (  P  n   ( x )  x  0   )  d x = log &#x2061;  (    2 L   e   x
      0      )    {\displaystyle H_{x}=\int _{-\infty }^{\infty }P_{n}(x)\log
      (P_{n}(x)x_{0})\,dx=\log \left({\frac {2L}{e\,x_{0}}}\right)}  [
      {\displaystyle H_{x}=\int _{-\infty }^{\infty }P_{n}(x)\log(P_{n}(x)x_
      {0})\,dx=\log \left({\frac {2L}{e\,x_{0}}}\right)}]
where x0 is an arbitrary reference length.
Another measure of uncertainty in momentum is the information_entropy of the
probability distribution Hp:
          H  p   ( n ) =  &#x222B;  &#x2212; &#x221E;   &#x221E;    P  n   ( p
      ) log &#x2061; (  P  n   ( p )  p  0   )  d p   {\displaystyle H_{p}
      (n)=\int _{-\infty }^{\infty }P_{n}(p)\log(P_{n}(p)p_{0})\,dp}  [
      {\displaystyle H_{p}(n)=\int _{-\infty }^{\infty }P_{n}(p)\log(P_{n}(p)p_
      {0})\,dp}]
          lim  n &#x2192; &#x221E;    H  p   ( n ) = log &#x2061;  (    4
      &#x03C0; &#x210F;   e  2 ( 1 &#x2212; &#x03B3; )     L   p  0      )
      {\displaystyle \lim _{n\to \infty }H_{p}(n)=\log \left({\frac {4\pi \hbar
      \,e^{2(1-\gamma )}}{L\,p_{0}}}\right)}  [{\displaystyle \lim _{n\to
      \infty }H_{p}(n)=\log \left({\frac {4\pi \hbar \,e^{2(1-\gamma )}}{L\,p_
      {0}}}\right)}]
where γ is Euler's_constant. The quantum mechanical entropic_uncertainty
principle states that for      x  0     p  0   = &#x210F;   {\displaystyle x_
{0}\,p_{0}=\hbar }  [{\displaystyle x_{0}\,p_{0}=\hbar }]
          H  x   +  H  p   ( n ) &#x2265; log &#x2061; ( e  &#x03C0; ) &#x2248;
      2.14473...   {\displaystyle H_{x}+H_{p}(n)\geq \log(e\,\pi )\approx
      2.14473...}  [{\displaystyle H_{x}+H_{p}(n)\geq \log(e\,\pi )\approx
      2.14473...}] (nats)
For      x  0     p  0   = &#x210F;   {\displaystyle x_{0}\,p_{0}=\hbar }  [
{\displaystyle x_{0}\,p_{0}=\hbar }], the sum of the position and momentum
entropies yields:
          H  x   +  H  p   ( &#x221E; ) = log &#x2061; ( 8 &#x03C0;   e  1
      &#x2212; 2 &#x03B3;   ) &#x2248; 3.06974...   {\displaystyle H_{x}+H_{p}
      (\infty )=\log(8\pi \,e^{1-2\gamma })\approx 3.06974...}  [{\displaystyle
      H_{x}+H_{p}(\infty )=\log(8\pi \,e^{1-2\gamma })\approx 3.06974...}]
      (nats)
which satisfies the quantum entropic uncertainty principle.
**** Energy levels[edit] ****
The energy of a particle in a box (black circles) and a free particle (grey
line) both depend upon wavenumber in the same way. However, the particle in a
box may only have certain, discrete energy levels.
The energies which correspond with each of the permitted wavenumbers may be
written as[5]
          E  n   =     n  2    &#x210F;  2    &#x03C0;  2     2 m  L  2      =
      n  2    h  2     8 m  L  2        {\displaystyle E_{n}={\frac {n^{2}\hbar
      ^{2}\pi ^{2}}{2mL^{2}}}={\frac {n^{2}h^{2}}{8mL^{2}}}}  [E_{n}={\frac {n^
      {2}\hbar ^{2}\pi ^{2}}{2mL^{2}}}={\frac {n^{2}h^{2}}{8mL^{2}}}].
The energy levels increase with      n  2     {\displaystyle n^{2}}  [n^{2}],
meaning that high energy levels are separated from each other by a greater
amount than low energy levels are. The lowest possible energy for the particle
(its zero-point_energy) is found in state 1, which is given by[8]
          E  1   =     &#x210F;  2    &#x03C0;  2     2 m  L  2      .
      {\displaystyle E_{1}={\frac {\hbar ^{2}\pi ^{2}}{2mL^{2}}}.}  [E_{1}=
      {\frac {\hbar ^{2}\pi ^{2}}{2mL^{2}}}.]
The particle, therefore, always has a positive energy. This contrasts with
classical systems, where the particle can have zero energy by resting
motionlessly. This can be explained in terms of the uncertainty_principle,
which states that the product of the uncertainties in the position and momentum
of a particle is limited by
         &#x0394; x &#x0394; p &#x2265;   &#x210F; 2     {\displaystyle \Delta
      x\Delta p\geq {\frac {\hbar }{2}}}  [\Delta x\Delta p\geq {\frac {\hbar }
      {2}}]
It can be shown that the uncertainty in the position of the particle is
proportional to the width of the box.[9] Thus, the uncertainty in momentum is
roughly inversely proportional to the width of the box.[8] The kinetic energy
of a particle is given by     E =  p  2    /  ( 2 m )   {\displaystyle E=p^{2}/
(2m)}  [E=p^{2}/(2m)], and hence the minimum kinetic energy of the particle in
a box is inversely proportional to the mass and the square of the well width,
in qualitative agreement with the calculation above.[8]
***** Higher-dimensional boxes[edit] *****
**** (Hyper)rectangular walls[edit] ****
The wavefunction of a 2D well with nx=4 and ny=4
If a particle is trapped in a two-dimensional box, it may freely move in the
x   {\displaystyle x}  [x] and     y   {\displaystyle y}  [y]-directions,
between barriers separated by lengths      L  x     {\displaystyle L_{x}}  [L_
{x}] and      L  y     {\displaystyle L_{y}}  [L_{y}] respectively. For a
centered box, the position wave function may be written including the length of
the box as      &#x03C8;  n   ( x , t , L )   {\displaystyle \psi _{n}(x,t,L)}
[{\displaystyle \psi _{n}(x,t,L)}]. Using a similar approach to that of the
one-dimensional box, it can be shown that the wavefunctions and energies for a
centered box are given respectively by
          &#x03C8;   n  x   ,  n  y     =  &#x03C8;   n  x     ( x , t ,  L  x
      )  &#x03C8;   n  y     ( y , t ,  L  y   )   {\displaystyle \psi _{n_
      {x},n_{y}}=\psi _{n_{x}}(x,t,L_{x})\psi _{n_{y}}(y,t,L_{y})}  [
      {\displaystyle \psi _{n_{x},n_{y}}=\psi _{n_{x}}(x,t,L_{x})\psi _{n_{y}}
      (y,t,L_{y})}],
          E   n  x   ,  n  y     =     &#x210F;  2    k   n  x   ,  n  y     2
      2 m      {\displaystyle E_{n_{x},n_{y}}={\frac {\hbar ^{2}k_{n_{x},n_
      {y}}^{2}}{2m}}}  [E_{n_{x},n_{y}}={\frac {\hbar ^{2}k_{n_{x},n_{y}}^{2}}
      {2m}}],
where the two-dimensional wavevector is given by
           k   n  x   ,  n  y      =  k   n  x        x &#x005E;    +  k   n  y
      y &#x005E;    =     n  x   &#x03C0;   L  x        x &#x005E;    +     n
      y   &#x03C0;   L  y        y &#x005E;      {\displaystyle \mathbf {k_{n_
      {x},n_{y}}} =k_{n_{x}}\mathbf {\hat {x}} +k_{n_{y}}\mathbf {\hat {y}} =
      {\frac {n_{x}\pi }{L_{x}}}\mathbf {\hat {x}} +{\frac {n_{y}\pi }{L_
      {y}}}\mathbf {\hat {y}} }  [\mathbf {k_{n_{x},n_{y}}} =k_{n_{x}}\mathbf
      {\hat {x}} +k_{n_{y}}\mathbf {\hat {y}} ={\frac {n_{x}\pi }{L_
      {x}}}\mathbf {\hat {x}} +{\frac {n_{y}\pi }{L_{y}}}\mathbf {\hat {y}} ].
For a three dimensional box, the solutions are
          &#x03C8;   n  x   ,  n  y   ,  n  z     =  &#x03C8;   n  x     ( x ,
      t ,  L  x   )  &#x03C8;   n  y     ( y , t ,  L  y   )  &#x03C8;   n  z
      ( z , t ,  L  z   )   {\displaystyle \psi _{n_{x},n_{y},n_{z}}=\psi _{n_
      {x}}(x,t,L_{x})\psi _{n_{y}}(y,t,L_{y})\psi _{n_{z}}(z,t,L_{z})}  [
      {\displaystyle \psi _{n_{x},n_{y},n_{z}}=\psi _{n_{x}}(x,t,L_{x})\psi _
      {n_{y}}(y,t,L_{y})\psi _{n_{z}}(z,t,L_{z})}],
          E   n  x   ,  n  y   ,  n  z     =     &#x210F;  2    k   n  x   ,  n
      y   ,  n  z     2     2 m      {\displaystyle E_{n_{x},n_{y},n_{z}}=
      {\frac {\hbar ^{2}k_{n_{x},n_{y},n_{z}}^{2}}{2m}}}  [E_{n_{x},n_{y},n_
      {z}}={\frac {\hbar ^{2}k_{n_{x},n_{y},n_{z}}^{2}}{2m}}],
where the three-dimensional wavevector is given by:
           k   n  x   ,  n  y   ,  n  z      =  k   n  x        x &#x005E;    +
      k   n  y        y &#x005E;    +  k   n  z        z &#x005E;    =     n  x
      &#x03C0;   L  x        x &#x005E;    +     n  y   &#x03C0;   L  y
      y &#x005E;    +     n  z   &#x03C0;   L  z        z &#x005E;
      {\displaystyle \mathbf {k_{n_{x},n_{y},n_{z}}} =k_{n_{x}}\mathbf {\hat
      {x}} +k_{n_{y}}\mathbf {\hat {y}} +k_{n_{z}}\mathbf {\hat {z}} ={\frac
      {n_{x}\pi }{L_{x}}}\mathbf {\hat {x}} +{\frac {n_{y}\pi }{L_{y}}}\mathbf
      {\hat {y}} +{\frac {n_{z}\pi }{L_{z}}}\mathbf {\hat {z}} }  [\mathbf {k_
      {n_{x},n_{y},n_{z}}} =k_{n_{x}}\mathbf {\hat {x}} +k_{n_{y}}\mathbf {\hat
      {y}} +k_{n_{z}}\mathbf {\hat {z}} ={\frac {n_{x}\pi }{L_{x}}}\mathbf
      {\hat {x}} +{\frac {n_{y}\pi }{L_{y}}}\mathbf {\hat {y}} +{\frac {n_
      {z}\pi }{L_{z}}}\mathbf {\hat {z}} ].
In general for an n-dimensional box, the solutions are
         &#x03C8; =  &#x220F;  i    &#x03C8;   n  i     (  x  i   , t ,  L  i
      )   {\displaystyle \psi =\prod _{i}\psi _{n_{i}}(x_{i},t,L_{i})}  [
      {\displaystyle \psi =\prod _{i}\psi _{n_{i}}(x_{i},t,L_{i})}]
The n-dimensional momentum wave functions may likewise be represented by
&#x03D5;  n   ( x , t ,  L  x   )   {\displaystyle \phi _{n}(x,t,L_{x})}  [
{\displaystyle \phi _{n}(x,t,L_{x})}] and the momentum wave function for an n-
dimensional centered box is then:
         &#x03D5; =  &#x220F;  i    &#x03D5;   n  i     (  k  i   , t ,  L  i
      )   {\displaystyle \phi =\prod _{i}\phi _{n_{i}}(k_{i},t,L_{i})}  [
      {\displaystyle \phi =\prod _{i}\phi _{n_{i}}(k_{i},t,L_{i})}]
An interesting feature of the above solutions is that when two or more of the
lengths are the same (e.g.      L  x   =  L  y     {\displaystyle L_{x}=L_{y}}
[L_{x}=L_{y}]), there are multiple wavefunctions corresponding to the same
total energy. For example, the wavefunction with      n  x   = 2 ,  n  y   = 1
{\displaystyle n_{x}=2,n_{y}=1}  [n_{x}=2,n_{y}=1] has the same energy as the
wavefunction with      n  x   = 1 ,  n  y   = 2   {\displaystyle n_{x}=1,n_
{y}=2}  [n_{x}=1,n_{y}=2]. This situation is called degeneracy and for the case
where exactly two degenerate wavefunctions have the same energy that energy
level is said to be doubly degenerate. Degeneracy results from symmetry in the
system. For the above case two of the lengths are equal so the system is
symmetric with respect to a 90Â° rotation.
**** More complicated wall shapes[edit] ****
The wavefunction for a quantum-mechanical particle in a box whose walls have
arbitrary shape is given by the Helmholtz_equation subject to the boundary
condition that the wavefunction vanishes at the walls. These systems are
studied in the field of quantum_chaos for wall shapes whose corresponding
dynamical_billiard_tables are non-integrable.
***** Applications[edit] *****
Because of its mathematical simplicity, the particle in a box model is used to
find approximate solutions for more complex physical systems in which a
particle is trapped in a narrow region of low electric_potential between two
high potential barriers. These quantum_well systems are particularly important
in optoelectronics, and are used in devices such as the quantum_well_laser, the
quantum_well_infrared_photodetector and the quantum-confined_Stark_effect
modulator. It is also used to model a lattice in the Kronig-Penny model and for
a finite metal with the free electron approximation.
**** Conjugated polyenes[edit] ****
Î²-carotene is a conjugated polyene
Conjugated polyene systems can be modeled using particle in a box.[10] The
conjugated system of electrons can be modeled as a one dimensional box with
length equal to the total bond distance from one terminus of the polyene to the
other. In this case each pair of electrons in each Ï bond corresponds to one
energy level. The energy difference between two energy levels, nf and ni is:
   &#x0394; E =    (  n  f   2   &#x2212;  n  i   2   )  h  2     8 m  L  2
{\displaystyle \Delta E={\frac {(n_{f}^{2}-n_{i}^{2})h^{2}}{8mL^{2}}}}  [
{\displaystyle \Delta E={\frac {(n_{f}^{2}-n_{i}^{2})h^{2}}{8mL^{2}}}}]
The difference between the ground state energy, n, and the first excited state,
n+1, corresponds to the energy required to excite the system. This energy has a
specific wavelength, and therefore color of light, related by:
   &#x03BB; =    h c   &#x0394; E      {\displaystyle \lambda ={\frac {hc}
{\Delta E}}}  [{\displaystyle \lambda ={\frac {hc}{\Delta E}}}]
A common example of this phenomenon is in Î²-carotene.[10] Î²-carotene (C40H56)
[11] is a conjugated polyene with an orange color and a molecular length of
approximately 3.8 nm (though its chain length is only approximately 2.4 nm).
[12] Due to Î²-carotene's high level of conjugation, electrons are dispersed
throughout the length of the molecule, allowing one to model it as a one-
dimensional particle in a box. Î²-carotene has 11 carbon-carbon double_bonds in
conjugation;[11] each of those double bonds contains two Ï-electrons,
therefore Î²-carotene has 22 Ï-electrons. With two electrons per energy level,
Î²-carotene can be treated as a particle in a box at energy level n=11.[12]
Therefore, the minimum energy needed to excite an electron to the next energy
level can be calculated, n=12, as follows[12] (recalling that the mass of an
electron is 9.109 Ã 10â31 kg[13]):
   &#x0394; E =    (  n  f   2   &#x2212;  n  i   2   )  h  2     8 m  L  2
{\displaystyle \Delta E={\frac {(n_{f}^{2}-n_{i}^{2})h^{2}}{8mL^{2}}}}  [
{\displaystyle \Delta E={\frac {(n_{f}^{2}-n_{i}^{2})h^{2}}{8mL^{2}}}}]
   =    (  12  2   &#x2212;  11  2   )  h  2     8 m  L  2
{\displaystyle ={\frac {(12^{2}-11^{2})h^{2}}{8mL^{2}}}}  [{\displaystyle =
{\frac {(12^{2}-11^{2})h^{2}}{8mL^{2}}}}]
   = 2.3658 &#x00D7;  10  &#x2212; 19    &#xA0;J    {\displaystyle
=2.3658\times 10^{-19}{\text{ J}}}  [{\displaystyle =2.3658\times 10^{-19}
{\text{ J}}}]
Using the previous relation of wavelength to energy, recalling both Planck's
constant h and the speed_of_light c:
   &#x03BB; =     h c   &#x0394; E       {\displaystyle \lambda ={\tfrac {hc}
{\Delta E}}}  [{\displaystyle \lambda ={\tfrac {hc}{\Delta E}}}]
   = 0.00000084  &#xA0;m  = 840  &#xA0;nm    {\displaystyle =0.00000084{\text
{ m}}=840{\text{ nm}}}  [{\displaystyle =0.00000084{\text{ m}}=840{\text
{ nm}}}]
This indicates that Î²-carotene primarily absorbs light in the infrared
spectrum, therefore it would appear white to a human eye. However the observed
wavelength is 450 nm,[14] indicating that the particle in a box is not a
perfect model for this system.
**** Quantum well laser[edit] ****
The particle in a box model can be applied to quantum_well_lasers, which are
laser diodes consisting of one semiconductor âwellâ material sandwiched
between two other semiconductor layers of different material . Because the
layers of this sandwich are very thin (the middle layer is typically about 100
Ã thick), quantum_confinement effects can be observed.[15] The idea that
quantum effects could be harnessed to create better laser diodes originated in
the 1970s. The quantum well laser was patented in 1976 by R. Dingle and C. H.
Henry[16]
Specifically, the quantum wellâs behavior can be represented by the particle
in a finite well model. Two boundary conditions must be selected. The first is
that the wave function must be continuous. Often, the second boundary condition
is chosen to be the derivative of the wave function must be continuous across
the boundary, but in the case of the quantum well the masses are different on
either side of the boundary. Instead, the second boundary condition is chosen
to conserve particle flux as    ( 1  /  m ) d &#x03D5;  /  d z   {\displaystyle
(1/m)d\phi /dz}  [{\displaystyle (1/m)d\phi /dz}], which is consistent with
experiment. The solution to the finite well particle in a box must be solved
numerically, resulting in wave functions that are sine functions inside the
quantum well and exponentially decaying functions in the barriers.[17] This
quantization of the energy levels of the electrons allows a quantum well laser
to emit light more efficiently than conventional semiconductor lasers.
Due to their small size, quantum dots do not showcase the bulk properties of
the specified semi-conductor but rather show quantised energy states.[18] This
effect is known as the quantum confinement and has led to numerous applications
of quantum dots such as the quantum well laser.[18]
Researchers at Princeton University have recently built a quantum well laser
which is no bigger than a grain of rice.[19] The laser is powered by a single
electron which passes through two quantum dots; a double quantum dot. The
electron moves from a state of higher energy, to a state of lower energy whilst
emitting photons in the microwave region. These photons bounce off mirrors to
create a beam of light; the laser.[19]
The quantum well laser is heavily based on the interaction between light and
electrons. This relationship is a key component in quantum mechanical theories
which include the De Broglie Wavelength and Particle in a box. The double
quantum dot allows scientists to gain full control over the movement of an
electron which consequently results in the production of a laser beam.[19]
*** Quantum dots[edit] ***
Quantum dots are extremely small semiconductors (on the scale of nanometers).
[20] They display quantum_confinement in that the electrons cannot escape the
âdotâ, thus allowing particle-in-a-box approximations to be applied.[21]
Their behavior can be described by three-dimensional particle-in-a-box energy
quantization equations.[21]
The energy_gap of a quantum dot is the energy gap between its valence_and
conduction_bands. This energy gap     &#x0394; E ( r )   {\displaystyle \Delta
E(r)}  [{\displaystyle \Delta E(r)}] is equal to the band gap of the bulk
material      E  gap     {\displaystyle E_{\text{gap}}}  [{\displaystyle E_
{\text{gap}}}] plus the energy equation derived from particle-in-a-box, which
gives the energy for electrons and holes.[21] This can be seen in the following
equation, where      m  e   &#x2217;     {\displaystyle m_{e}^{*}}  [
{\displaystyle m_{e}^{*}}] and      m  h   &#x2217;     {\displaystyle m_{h}^
{*}}  [{\displaystyle m_{h}^{*}}] are the effective masses of the electron and
hole,     r   {\displaystyle r}  [r] is radius of the dot, and     h
{\displaystyle h}  [h] is Planck's constant:[21]
   &#x0394; E ( r ) =  E  gap   +  (    h  2    8  r  2      )   (    1  m  e
&#x2217;     +   1  m  h   &#x2217;      )    {\displaystyle \Delta E(r)=E_
{\text{gap}}+\left({\frac {h^{2}}{8r^{2}}}\right)\left({\frac {1}{m_{e}^{*}}}+
{\frac {1}{m_{h}^{*}}}\right)}  [{\displaystyle \Delta E(r)=E_{\text
{gap}}+\left({\frac {h^{2}}{8r^{2}}}\right)\left({\frac {1}{m_{e}^{*}}}+{\frac
{1}{m_{h}^{*}}}\right)}]
Hence, the energy gap of the quantum dot is inversely proportional to the
square of the âlength of the box,â i.e. the radius of the quantum dot.[21]
Manipulation of the band gap allows for the absorption and emission of specific
wavelengths of light, as energy is inversely proportional to wavelength.[20]
The smaller the quantum dot, the larger the band gap and thus the shorter the
wavelength absorbed.[20][22]
Different semiconducting materials are used to synthesize quantum dots of
different sizes and therefore emit different wavelengths of light.[22]
Materials that normally emit light in the visible region are often used and
their sizes are fine-tuned so that certain colors are emitted.[20] Typical
substances used to synthesize quantum dots are cadmium (Cd) and selenium (Se).
[20][22] For example, when the electrons of two nanometer CdSe quantum dots
relax_after_excitation, blue light is emitted. Similarly, red light is emitted
in four nanometer CdSe quantum dots.[23][20]
Quantum dots have a variety of functions including but not limited to
fluorescent dyes, transistors, LEDs, solar_cells, and medical imaging via
optical probes.[20][21]
One function of quantum dots is their use in lymph node mapping, which is
feasible due to their unique ability to emit light in the near infrared (NIR)
region. Lymph node mapping allows surgeons to track if and where cancerous
cells exist.[24]
Quantum dots are useful for these functions due to their emission of brighter
light, excitation by a wide variety of wavelengths, and higher resistance to
light than other substances.[24][20]
***** Relativistic Effects[edit] *****
[[icon]] This section needs expansion. You can help by adding_to_it. (August
         2013)
The probability density does not go to zero at the nodes if relativistic
effects are taken into account via Dirac equation.[25]
***** See also[edit] *****
    * History_of_Quantum_Mechanics
    * Finite_potential_well
    * Delta_function_potential
    * Gas_in_a_box
    * Particle_in_a_ring
    * Particle_in_a_spherically_symmetric_potential
    * Quantum_harmonic_oscillator
    * Semicircle_potential_well
    * Configuration_integral (statistical mechanics)
    * Configuration_integral_(statistical_mechanics), 2008. this wiki site is
      down; see this_article_in_the_web_archive_on_2012_April_28.
***** References[edit] *****
   1. ^ a b c d e Davies, p.4
   2. ^ Actually, any constant, finite potential      V  0     {\displaystyle
      V_{0}}  [V_{0}] can be specified within the box. This merely shifts the
      energies of the states by      V  0     {\displaystyle V_{0}}  [V_{0}].
   3. ^ Davies, p. 1
   4. ^ a b Bransden and Joachain, p. 157
   5. ^ a b Davies p. 5
   6. ^ a b Bransden and Joachain, p.158
   7. ^Majernik, Vladimir; Richterek, Lukas (1997-12-01). "Entropic_uncertainty
      relations_for_the_infinite_well". J. Phys. A. 30 (4): L49. Bibcode:
      1997JPhA...30L..49M. doi:10.1088/0305-4470/30/4/002. Retrieved 11
      February 2016.
   8. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
   9. ^ a b c Bransden and Joachain, p. 159
  10. ^ Davies, p. 15
  11. ^ a b Todd Wimpfheimer, A Particle in a Box Laboratory Experiment Using
      Everyday Compounds, Journal of Laboratory Chemical Education, Vol. 3 No.
      2, 2015, pp. 19-21. doi:10.5923/j.jlce.20150302.01.
  12. ^ a bPubchem. "beta-carotene_|_C40H56_-_PubChem".
      pubchem.ncbi.nlm.nih.gov. Retrieved 2016-11-10.
  13. ^ a b cSathish, R. K.; Sidharthan, P. V.; Udayanandan, K. M. "Particle in
      a Box- A Treasure Island for Undergraduates".
  14. ^ P.J. Mohr, B.N. Taylor, and D.B. Newell, "The 2014 CODATA Recommended
      Values of the Fundamental Physical Constants". This database was
      developed by J. Baker, M. Douma, and S. Kotochigova. Available: [1].
      National Institute of Standards and Technology, Gaithersburg, MD 20899.
  15. ^ Î²-Carotene http://www.sigmaaldrich.com/catalog/product/aldrich/
      855553?lang=enÂ®ion=us (accessed Nov 8, 2016).
  16. ^Zory, Peter (1993). Quantum Well Lasers. San Diego: Academic Press
      Unlimited.
  17. ^ U.S. Patent #3,982,207, issued September 21, 1976, Inventors R. Dingle
      and C. H. Henry ,"Quantum Effects in Heterostructure Lasers", filed March
      7, 1975.
  18. ^Miller, David (1995). Burstein, Elias; Weisbuch, Claude (eds.). Confined
      Electrons and Photons: New Physics and Applications. New York: Plenum
      Press. pp. 675â702.
  19. ^ a bMiessler, G. L. (2013). Inorganic chemistry (5 ed.). Boston:
      Pearson. pp. 235â236. ISBN 978-0321811059.
  20. ^ a b cZandonella, Catherine. "Rice-sized_laser,_powered_one_electron_at
      a_time,_bodes_well_for_quantum_computing". Princeton University.
      Princeton University. Retrieved 8 November 2016.
  21. ^ a b c d e f g hRice, C.V.; Griffin, G.A. (2008). "Simple_Syntheses_of
      CdSe_Quantum_Dots". Journal of Chemical Education. 85 (6): 842. Bibcode:
      2008JChEd..85..842R. doi:10.1021/ed085p842. Retrieved 5 November 2016.
  22. ^ a b c d e f"Quantum_Dots :_a_True_"Particle_in_a_Box"_System".
      PhysicsOpenLab. 20 November 2015. Retrieved 5 November 2016.
  23. ^ a b cOverney, RenÃ© M. "Quantum_Confinement" (PDF). University of
      Washington. Retrieved 5 November 2016.
  24. ^Zahn, Dietrich R.T. "Surface_and_Interface_Properties_of_Semiconductor
      Quantum_Dots_by_Raman_Spectroscopy" (PDF). Technische UniversitÃ¤t
      Chemnitz. Retrieved 5 November 2016.
  25. ^ a bBentolila, Laurent A.; Ebenstein, Yuval (2009). "Quantum_Dots_for_In
      Vivo_Small-Animal_Imaging". Journal of Nuclear Medicine. 50 (4):
      493â496. doi:10.2967/jnumed.108.053561. PMC 3081879. PMID 19289434.
  26. ^Alberto, P; Fiolhais, C; Gil, V M S (1996). "Relativistic_particle_in_a
      box" (PDF). European Journal of Physics. 17 (1): 19â24. Bibcode:
      1996EJPh...17...19A. doi:10.1088/0143-0807/17/1/004. hdl:10316/12349.
***** Bibliography[edit] *****
    * Bransden, B. H.; Joachain, C. J. (2000). Quantum mechanics (2nd ed.).
      Essex: Pearson Education. ISBN 978-0-582-35691-7.
Davies, John H. (2006). The Physics of Low-Dimensional Semiconductors: An
Introduction (6th reprint ed.). Cambridge University Press. ISBN 978-0-521-
48491-6.
Griffiths, David J. (2004). Introduction to Quantum Mechanics (2nd ed.).
Prentice Hall. ISBN 978-0-13-111892-8.
***** External links[edit] *****
 Wikimedia Commons has media related to 1D_infinite_square_wells.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Particle_in_a_box&oldid=908824824"
Categories:
    * Quantum_models
Hidden categories:
    * Use_American_English_from_January_2019
    * All_Wikipedia_articles_written_in_American_English
    * Articles_with_short_description
    * Articles_to_be_expanded_from_August_2013
    * All_articles_to_be_expanded
    * Articles_using_small_message_boxes
    * Commons_category_link_is_on_Wikidata
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
    * CatalÃ 
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Bahasa_Melayu
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Suomi
    * Svenska
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * ä¸­æ
Edit_links
    * This page was last edited on 1 August 2019, at 07:18 (UTC).
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
