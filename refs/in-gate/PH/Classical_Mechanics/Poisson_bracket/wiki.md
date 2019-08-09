The following text has been accessed from https://en.wikipedia.org/wiki/Poisson_bracket at Fri Aug 9 03:07:11 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Poisson bracket ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics and classical_mechanics, the Poisson bracket is an important
binary_operation in Hamiltonian_mechanics, playing a central role in Hamilton's
equations of motion, which govern the time evolution of a Hamiltonian dynamical
system. The Poisson bracket also distinguishes a certain class of coordinate
transformations, called canonical_transformations, which map canonical
coordinate_systems into canonical coordinate systems. A "canonical coordinate
system" consists of canonical position and momentum variables (below symbolized
by      q  i     {\displaystyle q_{i}}  [q_{i}] and      p  i
{\displaystyle p_{i}}  [p_{i}], respectively) that satisfy canonical Poisson
bracket relations. The set of possible canonical transformations is always very
rich. For instance, it is often possible to choose the Hamiltonian itself     H
= H ( q , p ; t )   {\displaystyle H=H(q,p;t)}  [{\displaystyle H=H(q,p;t)}] as
one of the new canonical momentum coordinates.
In a more general sense, the Poisson bracket is used to define a Poisson
algebra, of which the algebra of functions on a Poisson_manifold is a special
case. There are other general examples, as well: it occurs in the theory of Lie
algebras, where the tensor_algebra of a Lie algebra forms a Poisson algebra; a
detailed construction of how this comes about is given in the universal
enveloping_algebra article. Quantum deformations of the universal enveloping
algebra lead to the notion of quantum_groups.
All of these objects are named in honour of SimÃ©on_Denis_Poisson.
⁰
***** Contents *****
    * 1_Properties
    * 2_Definition_in_canonical_coordinates
    * 3_Hamilton's_equations_of_motion
    * 4_Constants_of_motion
    * 5_The_Poisson_bracket_in_coordinate-free_language
    * 6_A_result_on_conjugate_momenta
    * 7_Quantization
    * 8_See_also
    * 9_Remarks
    * 10_Notes
    * 11_References
    * 12_External_links
***** Properties[edit] *****
Given two functions     f , &#xA0; g   {\displaystyle f,\ g}  [{\displaystyle
f,\ g}] that depend on phase_space and time, their Poisson bracket     { f , g
}   {\displaystyle \{f,g\}}  [{\displaystyle \{f,g\}}] is another function that
depends on phase space and time. The following rules hold for any three
functions     f ,  g ,  h   {\displaystyle f,\,g,\,h}  [{\displaystyle
f,\,g,\,h}] of phase space and time:
  Anticommutativity
         { f , g } = &#x2212; { g , f }   {\displaystyle \{f,g\}=-\{g,f\}}  [\
      {f,g\}=-\{g,f\}]
  Bilinearity
         { a f + b g , h } = a { f , h } + b { g , h } ,  { h , a f + b g } = a
      { h , f } + b { h , g } ,  a , b &#x2208;  R    {\displaystyle \
      {af+bg,h\}=a\{f,h\}+b\{g,h\},\quad \{h,af+bg\}=a\{h,f\}+b\{h,g\},\quad
      a,b\in \mathbb {R} }  [{\displaystyle \{af+bg,h\}=a\{f,h\}+b\{g,h\},\quad
      \{h,af+bg\}=a\{h,f\}+b\{h,g\},\quad a,b\in \mathbb {R} }]
  Leibniz's_rule
         { f g , h } = { f , h } g + f { g , h }   {\displaystyle \{fg,h\}=\
      {f,h\}g+f\{g,h\}}  [\{fg,h\}=\{f,h\}g+f\{g,h\}]
  Jacobi_identity
         { f , { g , h } } + { g , { h , f } } + { h , { f , g } } = 0
      {\displaystyle \{f,\{g,h\}\}+\{g,\{h,f\}\}+\{h,\{f,g\}\}=0}  [\{f,\
      {g,h\}\}+\{g,\{h,f\}\}+\{h,\{f,g\}\}=0]
Also, if a function     k   {\displaystyle k}  [k] is constant over phase space
(but may depend on time), then     { f ,  k } = 0   {\displaystyle \{f,\,k\}=0}
[{\displaystyle \{f,\,k\}=0}] for any     f   {\displaystyle f}  [f].
***** Definition in canonical coordinates[edit] *****
In canonical_coordinates (also known as Darboux_coordinates)     (  q  i   ,
p  i   )   {\displaystyle (q_{i},\,p_{i})}  [{\displaystyle (q_{i},\,p_{i})}]
on the phase_space, given two functions     f (  p  i   ,   q  i   , t )
{\displaystyle f(p_{i},\,q_{i},t)}  [{\displaystyle f(p_{i},\,q_{i},t)}] and
g (  p  i   ,   q  i   , t )   {\displaystyle g(p_{i},\,q_{i},t)}  [
{\displaystyle g(p_{i},\,q_{i},t)}],[Note_1] the Poisson bracket takes the form
         { f , g } =  &#x2211;  i = 1   N    (     &#x2202; f   &#x2202;  q  i
      &#x2202; g   &#x2202;  p  i      &#x2212;    &#x2202; f   &#x2202;  p  i
      &#x2202; g   &#x2202;  q  i       )  .   {\displaystyle \{f,g\}=\sum _
      {i=1}^{N}\left({\frac {\partial f}{\partial q_{i}}}{\frac {\partial g}
      {\partial p_{i}}}-{\frac {\partial f}{\partial p_{i}}}{\frac {\partial g}
      {\partial q_{i}}}\right).}  [\{f,g\}=\sum _{i=1}^{N}\left({\frac
      {\partial f}{\partial q_{i}}}{\frac {\partial g}{\partial p_{i}}}-{\frac
      {\partial f}{\partial p_{i}}}{\frac {\partial g}{\partial q_
      {i}}}\right).]
The Poisson brackets of the canonical coordinates are
             {  q  i   ,  q  j   }    = 0     {  p  i   ,  p  j   }    = 0
      {  q  i   ,  p  j   }    =  &#x03B4;  i j         {\displaystyle {\begin
      {aligned}\{q_{i},q_{j}\}&=0\\\{p_{i},p_{j}\}&=0\\\{q_{i},p_{j}\}&=\delta
      _{ij}\end{aligned}}}  [{\begin{aligned}\{q_{i},q_{j}\}&=0\\\{p_{i},p_
      {j}\}&=0\\\{q_{i},p_{j}\}&=\delta _{ij}\end{aligned}}]
where     &#x03B4;  i j     {\displaystyle \delta _{ij}}  [\delta _{ij}] is the
Kronecker_delta.
***** Hamilton's equations of motion[edit] *****
Hamilton's_equations_of_motion have an equivalent expression in terms of the
Poisson bracket. This may be most directly demonstrated in an explicit
coordinate frame. Suppose that     f ( p , q , t )   {\displaystyle f(p,q,t)}
[{\displaystyle f(p,q,t)}] is a function on the manifold. Then from the
multivariable chain_rule,
            d    d  t    f ( p , q , t ) =    &#x2202; f   &#x2202; q        d
      q    d  t    +    &#x2202; f   &#x2202; p        d  p    d  t    +
      &#x2202; f   &#x2202; t    .   {\displaystyle {\frac {\mathrm {d} }
      {\mathrm {d} t}}f(p,q,t)={\frac {\partial f}{\partial q}}{\frac {\mathrm
      {d} q}{\mathrm {d} t}}+{\frac {\partial f}{\partial p}}{\frac {\mathrm
      {d} p}{\mathrm {d} t}}+{\frac {\partial f}{\partial t}}.}  [{\frac
      {\mathrm {d} }{\mathrm {d} t}}f(p,q,t)={\frac {\partial f}{\partial q}}
      {\frac {\mathrm {d} q}{\mathrm {d} t}}+{\frac {\partial f}{\partial p}}
      {\frac {\mathrm {d} p}{\mathrm {d} t}}+{\frac {\partial f}{\partial t}}.]
Further, one may take     p = p ( t )   {\displaystyle p=p(t)}  [{\displaystyle
p=p(t)}] and     q = q ( t )   {\displaystyle q=q(t)}  [{\displaystyle q=q(t)}]
to be solutions to Hamilton's_equations; that is,
           {       q &#x02D9;    =    &#x2202; H   &#x2202; p    = { q , H } ;
      p &#x02D9;    = &#x2212;    &#x2202; H   &#x2202; q    = { p , H } .
      {\displaystyle {\begin{cases}{\dot {q}}={\frac {\partial H}{\partial
      p}}=\{q,H\};\\{\dot {p}}=-{\frac {\partial H}{\partial q}}=\{p,H\}.\end
      {cases}}}  [{\displaystyle {\begin{cases}{\dot {q}}={\frac {\partial H}
      {\partial p}}=\{q,H\};\\{\dot {p}}=-{\frac {\partial H}{\partial q}}=\
      {p,H\}.\end{cases}}}]
Then
                d    d  t    f ( p , q , t )    =    &#x2202; f   &#x2202; q
      &#x2202; H   &#x2202; p    &#x2212;    &#x2202; f   &#x2202; p
      &#x2202; H   &#x2202; q    +    &#x2202; f   &#x2202; t          = { f ,
      H } +    &#x2202; f   &#x2202; t    &#xA0; .       {\displaystyle {\begin
      {aligned}{\frac {\mathrm {d} }{\mathrm {d} t}}f(p,q,t)&={\frac {\partial
      f}{\partial q}}{\frac {\partial H}{\partial p}}-{\frac {\partial f}
      {\partial p}}{\frac {\partial H}{\partial q}}+{\frac {\partial f}
      {\partial t}}\\&=\{f,H\}+{\frac {\partial f}{\partial t}}~.\end
      {aligned}}}  [{\begin{aligned}{\frac {\mathrm {d} }{\mathrm {d} t}}f
      (p,q,t)&={\frac {\partial f}{\partial q}}{\frac {\partial H}{\partial
      p}}-{\frac {\partial f}{\partial p}}{\frac {\partial H}{\partial q}}+
      {\frac {\partial f}{\partial t}}\\&=\{f,H\}+{\frac {\partial f}{\partial
      t}}~.\end{aligned}}]
Thus, the time evolution of a function     f   {\displaystyle f}  [f] on a
symplectic_manifold can be given as a one-parameter_family of
symplectomorphisms (i.e., canonical_transformations, area-preserving
diffeomorphisms), with the time     t   {\displaystyle t}  [t] being the
parameter: Hamiltonian motion is a canonical transformation generated by the
Hamiltonian. That is, Poisson brackets are preserved in it, so that any time
t   {\displaystyle t}  [t] in the solution to Hamilton's equations,
         q ( t ) = exp &#x2061; ( &#x2212; t { H , &#x22C5; } ) q ( 0 ) ,  p
      ( t ) = exp &#x2061; ( &#x2212; t { H , &#x22C5; } ) p ( 0 ) ,
      {\displaystyle q(t)=\exp(-t\{H,\cdot \})q(0),\quad p(t)=\exp(-t\{H,\cdot
      \})p(0),}  [{\displaystyle q(t)=\exp(-t\{H,\cdot \})q(0),\quad p(t)=\exp
      (-t\{H,\cdot \})p(0),}]
can serve as the bracket coordinates. Poisson brackets are canonical
invariants.
Dropping the coordinates,
           d   d  t    f =  (    &#x2202;  &#x2202; t    &#x2212; { H ,
      &#x22C5; }  )  f .   {\displaystyle {\frac {\text{d}}{{\text
      {d}}t}}f=\left({\frac {\partial }{\partial t}}-\{H,\cdot \}\right)f.}  [
      {\displaystyle {\frac {\text{d}}{{\text{d}}t}}f=\left({\frac {\partial }
      {\partial t}}-\{H,\cdot \}\right)f.}]
The operator in the convective part of the derivative,     i    L &#x005E;    =
&#x2212; { H , &#x22C5; }   {\displaystyle i{\hat {L}}=-\{H,\cdot \}}  [
{\displaystyle i{\hat {L}}=-\{H,\cdot \}}], is sometimes referred to as the
Liouvillian (see Liouville's_theorem_(Hamiltonian)).
***** Constants of motion[edit] *****
An integrable_dynamical_system will have constants_of_motion in addition to the
energy. Such constants of motion will commute with the Hamiltonian under the
Poisson bracket. Suppose some function     f ( p , q )   {\displaystyle f(p,q)}
[{\displaystyle f(p,q)}] is a constant of motion. This implies that if     p
( t ) , q ( t )   {\displaystyle p(t),q(t)}  [{\displaystyle p(t),q(t)}] is a
trajectory or solution to the Hamilton's_equations_of_motion, then
         0 =     d  f    d  t      {\displaystyle 0={\frac {{\text{d}}f}{{\text
      {d}}t}}}  [0={\frac {{\text{d}}f}{{\text{d}}t}}]
along that trajectory. Then
         0 =   d   d  t    f ( p , q ) = { f , H } +    &#x2202; f   &#x2202; t
      = { f , H }   {\displaystyle 0={\frac {\text{d}}{{\text{d}}t}}f(p,q)=\
      {f,H\}+{\frac {\partial f}{\partial t}}=\{f,H\}}  [{\displaystyle 0=
      {\frac {\text{d}}{{\text{d}}t}}f(p,q)=\{f,H\}+{\frac {\partial f}
      {\partial t}}=\{f,H\}}]
where, as above, the intermediate step follows by applying the equations of
motion and we supposed that     f   {\displaystyle f}  [f] does not explicitly
depend on time. This equation is known as the Liouville_equation. The content
of Liouville's_theorem is that the time evolution of a measure (or
"distribution_function" on the phase space) is given by the above.
If the Poisson bracket of     f   {\displaystyle f}  [f] and     g
{\displaystyle g}  [g] vanishes (    { f , g } = 0   {\displaystyle \{f,g\}=0}
[{\displaystyle \{f,g\}=0}]), then     f   {\displaystyle f}  [f] and     g
{\displaystyle g}  [g] are said to be in involution. In order for a Hamiltonian
system to be completely_integrable,     n   {\displaystyle n}  [n] independent
constants of motion must be in mutual_involution, where     n   {\displaystyle
n}  [n] is the number of degrees of freedom.
Furthermore, according to the Poisson's Theorem, if two quantities     A
{\displaystyle A}  [A] and     B   {\displaystyle B}  [B] are explicitly time
independent (    A ( p , q ) , B ( p , q )   {\displaystyle A(p,q),B(p,q)}  [
{\displaystyle A(p,q),B(p,q)}]) constants of motion, so is their Poisson
bracket     { A ,  B }   {\displaystyle \{A,\,B\}}  [{\displaystyle \
{A,\,B\}}]. This does not always supply a useful result, however, since the
number of possible constants of motion is limited (    2 n &#x2212; 1
{\displaystyle 2n-1}  [2n-1] for a system with     n   {\displaystyle n}  [n]
degrees of freedom), and so the result may be trivial (a constant, or a
function of     A   {\displaystyle A}  [A] and     B   {\displaystyle B}  [B].)
***** The Poisson bracket in coordinate-free language[edit] *****
Let     M   {\displaystyle M}  [M] be symplectic_manifold, that is, a manifold
equipped with a symplectic_form: a 2-form     &#x03C9;   {\displaystyle \omega
}  [\omega ] which is both closed (i.e., its exterior_derivative      d
&#x03C9;   {\displaystyle {\text{d}}\omega }  [{\displaystyle {\text{d}}\omega
}] vanishes) and non-degenerate. For example, in the treatment above, take
M   {\displaystyle M}  [M] to be       R   2 n     {\displaystyle \mathbb {R} ^
{2n}}  [{\mathbb  {R}}^{{2n}}] and take
         &#x03C9; =  &#x2211;  i = 1   n    d   q  i   &#x2227;  d   p  i   .
      {\displaystyle \omega =\sum _{i=1}^{n}{\text{d}}q_{i}\wedge {\text{d}}p_
      {i}.}  [{\displaystyle \omega =\sum _{i=1}^{n}{\text{d}}q_{i}\wedge
      {\text{d}}p_{i}.}]
If      &#x03B9;  v   &#x03C9;   {\displaystyle \iota _{v}\omega }  [
{\displaystyle \iota _{v}\omega }] is the interior_product or contraction
operation defined by     (  &#x03B9;  v   &#x03C9; ) ( w ) = &#x03C9; ( v ,  w
)   {\displaystyle (\iota _{v}\omega )(w)=\omega (v,\,w)}  [{\displaystyle
(\iota _{v}\omega )(w)=\omega (v,\,w)}], then non-degeneracy is equivalent to
saying that for every one-form     &#x03B1;   {\displaystyle \alpha }  [\alpha
] there is a unique vector field      &#x03A9;  &#x03B1;     {\displaystyle
\Omega _{\alpha }}  [{\displaystyle \Omega _{\alpha }}] such that      &#x03B9;
&#x03A9;  &#x03B1;     &#x03C9; = &#x03B1;   {\displaystyle \iota _{\Omega _
{\alpha }}\omega =\alpha }  [{\displaystyle \iota _{\Omega _{\alpha }}\omega
=\alpha }]. Alternatively,      &#x03A9;   d  H   =  &#x03C9;  &#x2212; 1
(  d  H )   {\displaystyle \Omega _{{\text{d}}H}=\omega ^{-1}({\text{d}}H)}  [
{\displaystyle \Omega _{{\text{d}}H}=\omega ^{-1}({\text{d}}H)}]. Then if     H
{\displaystyle H}  [H] is a smooth function on     M   {\displaystyle M}  [M],
the Hamiltonian_vector_field      X  H     {\displaystyle X_{H}}  [X_{H}] can
be defined to be      &#x03A9;   d  H     {\displaystyle \Omega _{{\text{d}}H}}
[{\displaystyle \Omega _{{\text{d}}H}}]. It is easy to see that
              X   p  i        =   &#x2202;  &#x2202;  q  i           X   q  i
      = &#x2212;   &#x2202;  &#x2202;  p  i      .       {\displaystyle {\begin
      {aligned}X_{p_{i}}&={\frac {\partial }{\partial q_{i}}}\\X_{q_{i}}&=-
      {\frac {\partial }{\partial p_{i}}}.\end{aligned}}}  [{\begin{aligned}X_
      {p_{i}}&={\frac {\partial }{\partial q_{i}}}\\X_{q_{i}}&=-{\frac
      {\partial }{\partial p_{i}}}.\end{aligned}}]
The Poisson bracket     &#xA0; { &#x22C5; ,  &#x22C5; }   {\displaystyle \ \
{\cdot ,\,\cdot \}}  [{\displaystyle \ \{\cdot ,\,\cdot \}}] on (M, Ï) is a
bilinear_operation on differentiable functions, defined by     { f ,  g }  =
&#x03C9; (  X  f   ,   X  g   )   {\displaystyle \{f,\,g\}\;=\;\omega (X_
{f},\,X_{g})}  [{\displaystyle \{f,\,g\}\;=\;\omega (X_{f},\,X_{g})}]; the
Poisson bracket of two functions on M is itself a function on M. The Poisson
bracket is antisymmetric because:
         { f , g } = &#x03C9; (  X  f   ,  X  g   ) = &#x2212; &#x03C9; (  X  g
      ,  X  f   ) = &#x2212; { g , f }   {\displaystyle \{f,g\}=\omega (X_
      {f},X_{g})=-\omega (X_{g},X_{f})=-\{g,f\}}  [\{f,g\}=\omega (X_{f},X_
      {g})=-\omega (X_{g},X_{f})=-\{g,f\}].
Furthermore,
             { f , g }    = &#x03C9; (  X  f   ,  X  g   ) = &#x03C9;
      (  &#x03A9;  d f   ,  X  g   )       = (  &#x03B9;   &#x03A9;
      d f     &#x03C9; ) (  X  g   ) = d f (  X  g   )       =  X  g
      f =    L     X  g     f       {\displaystyle {\begin{aligned}\
      {f,g\}&=\omega (X_{f},X_{g})=\omega (\Omega _{df},X_{g})\\&=       (1)
      (\iota _{\Omega _{df}}\omega )(X_{g})=df(X_{g})\\&=X_{g}f=         
      {\mathcal {L}}_{X_{g}}f\end{aligned}}}  [{\begin{aligned}\
      {f,g\}&=\omega (X_{f},X_{g})=\omega (\Omega _{df},X_{g})\\&=
      (\iota _{\Omega _{df}}\omega )(X_{g})=df(X_{g})\\&=X_{g}f=
      {\mathcal {L}}_{X_{g}}f\end{aligned}}].
Here Xgf denotes the vector field Xg applied to the function f as a directional
derivative, and        L     X  g     f   {\displaystyle {\mathcal {L}}_{X_
{g}}f}  [{\mathcal {L}}_{X_{g}}f] denotes the (entirely equivalent) Lie
derivative of the function f.
If Î± is an arbitrary one-form on M, the vector field Î©Î± generates (at least
locally) a flow      &#x03D5;  x   ( t )   {\displaystyle \phi _{x}(t)}  [
{\displaystyle \phi _{x}(t)}] satisfying the boundary condition      &#x03D5;
x   ( 0 ) = x   {\displaystyle \phi _{x}(0)=x}  [{\displaystyle \phi _{x}
(0)=x}] and the first-order differential equation
            d  &#x03D5;  x     d t    =     &#x03A9;  &#x03B1;   |    &#x03D5;
      x   ( t )   .   {\displaystyle {\frac {d\phi _{x}}{dt}}=\left.\Omega _
      {\alpha }\right|_{\phi _{x}(t)}.}  [{\frac {d\phi _{x}}{dt}}=\left.\Omega
      _{\alpha }\right|_{\phi _{x}(t)}.]
The      &#x03D5;  x   ( t )   {\displaystyle \phi _{x}(t)}  [{\displaystyle
\phi _{x}(t)}] will be symplectomorphisms (canonical_transformations) for every
t as a function of x if and only if        L     &#x03A9;  &#x03B1;
&#x03C9;  =  0   {\displaystyle {\mathcal {L}}_{\Omega _{\alpha }}\omega
\;=\;0}  [{\displaystyle {\mathcal {L}}_{\Omega _{\alpha }}\omega \;=\;0}];
when this is true, Î©Î± is called a symplectic_vector_field. Recalling Cartan's
identity        L    X   &#x03C9;  =  d (  &#x03B9;  X   &#x03C9; )  +
&#x03B9;  X   d &#x03C9;   {\displaystyle {\mathcal {L}}_{X}\omega \;=\;d(\iota
_{X}\omega )\,+\,\iota _{X}d\omega }  [{\displaystyle {\mathcal {L}}_{X}\omega
\;=\;d(\iota _{X}\omega )\,+\,\iota _{X}d\omega }] and dÏ = 0, it follows that
L     &#x03A9;  &#x03B1;     &#x03C9;  =  d  (   &#x03B9;   &#x03A9;  &#x03B1;
&#x03C9;  )   =  d &#x03B1;   {\displaystyle {\mathcal {L}}_{\Omega _{\alpha
}}\omega \;=\;d\left(\iota _{\Omega _{\alpha }}\omega \right)\;=\;d\alpha }  [
{\displaystyle {\mathcal {L}}_{\Omega _{\alpha }}\omega \;=\;d\left(\iota _
{\Omega _{\alpha }}\omega \right)\;=\;d\alpha }]. Therefore, Î©Î± is a
symplectic vector field if and only if Î± is a closed_form. Since     d ( d f )
=   d  2   f  =  0   {\displaystyle d(df)\;=\;d^{2}f\;=\;0}  [{\displaystyle d
(df)\;=\;d^{2}f\;=\;0}], it follows that every Hamiltonian vector field Xf is a
symplectic vector field, and that the Hamiltonian flow consists of canonical
transformations. From (1) above, under the Hamiltonian flow XH,
           d  d t    f (  &#x03D5;  x   ( t ) ) =  X  H   f = { f , H } .
      {\displaystyle {\frac {d}{dt}}f(\phi _{x}(t))=X_{H}f=\{f,H\}.}  [{\frac
      {d}{dt}}f(\phi _{x}(t))=X_{H}f=\{f,H\}.]
This is a fundamental result in Hamiltonian mechanics, governing the time
evolution of functions defined on phase space. As noted above, when {f,H} = 0,
f is a constant of motion of the system. In addition, in canonical coordinates
(with     {  p  i   ,   p  j   }  =  {  q  i   ,  q  j   }  =  0
{\displaystyle \{p_{i},\,p_{j}\}\;=\;\{q_{i},q_{j}\}\;=\;0}  [{\displaystyle \
{p_{i},\,p_{j}\}\;=\;\{q_{i},q_{j}\}\;=\;0}] and     {  q  i   ,   p  j   }  =
&#x03B4;  i j     {\displaystyle \{q_{i},\,p_{j}\}\;=\;\delta _{ij}}  [
{\displaystyle \{q_{i},\,p_{j}\}\;=\;\delta _{ij}}]), Hamilton's equations for
the time evolution of the system follow immediately from this formula.
It also follows from (1) that the Poisson bracket is a derivation; that is, it
satisfies a non-commutative version of Leibniz's product_rule:
         { f g , h } = f { g , h } + g { f , h }   {\displaystyle \
      {fg,h\}=f\{g,h\}+g\{f,h\}}  [\{fg,h\}=f\{g,h\}+g\{f,h\}], and    (2)
      { f , g h } = g { f , h } + h { f , g }   {\displaystyle \       
      {f,gh\}=g\{f,h\}+h\{f,g\}}  [\{f,gh\}=g\{f,h\}+h\{f,g\}]
The Poisson bracket is intimately connected to the Lie_bracket of the
Hamiltonian vector fields. Because the Lie derivative is a derivation,
            L    v    &#x03B9;  w   &#x03C9; =  &#x03B9;     L    v   w
      &#x03C9; +  &#x03B9;  w      L    v   &#x03C9; =  &#x03B9;  [ v , w ]
      &#x03C9; +  &#x03B9;  w      L    v   &#x03C9;   {\displaystyle {\mathcal
      {L}}_{v}\iota _{w}\omega =\iota _{{\mathcal {L}}_{v}w}\omega +\iota _{w}
      {\mathcal {L}}_{v}\omega =\iota _{[v,w]}\omega +\iota _{w}{\mathcal {L}}_
      {v}\omega }  [{\mathcal {L}}_{v}\iota _{w}\omega =\iota _{{\mathcal {L}}_
      {v}w}\omega +\iota _{w}{\mathcal {L}}_{v}\omega =\iota _{[v,w]}\omega
      +\iota _{w}{\mathcal {L}}_{v}\omega ].
Thus if v and w are symplectic, using        L    v   &#x03C9;  =  0
{\displaystyle {\mathcal {L}}_{v}\omega \;=\;0}  [{\displaystyle {\mathcal
{L}}_{v}\omega \;=\;0}], Cartan's identity, and the fact that      &#x03B9;  w
&#x03C9;   {\displaystyle \iota _{w}\omega }  [\iota _{w}\omega ] is a closed
form,
          &#x03B9;  [ v , w ]   &#x03C9; =    L    v    &#x03B9;  w   &#x03C9;
      = d (  &#x03B9;  v    &#x03B9;  w   &#x03C9; ) +  &#x03B9;  v   d
      (  &#x03B9;  w   &#x03C9; ) = d (  &#x03B9;  v    &#x03B9;  w   &#x03C9;
      ) = d ( &#x03C9; ( w , v ) ) .   {\displaystyle \iota _{[v,w]}\omega =
      {\mathcal {L}}_{v}\iota _{w}\omega =d(\iota _{v}\iota _{w}\omega )+\iota
      _{v}d(\iota _{w}\omega )=d(\iota _{v}\iota _{w}\omega )=d(\omega (w,v)).}
      [\iota _{[v,w]}\omega ={\mathcal {L}}_{v}\iota _{w}\omega =d(\iota _
      {v}\iota _{w}\omega )+\iota _{v}d(\iota _{w}\omega )=d(\iota _{v}\iota _
      {w}\omega )=d(\omega (w,v)).]
It follows that     [ v , w ] =  X  &#x03C9; ( w , v )     {\displaystyle
[v,w]=X_{\omega (w,v)}}  [[v,w]=X_{\omega (w,v)}], so that
         [  X  f   ,  X  g   ] =  X  &#x03C9; (  X  g   ,  X  f   )
      = &#x2212;  X  &#x03C9; (  X  f   ,  X  g   )   = &#x2212;  X
      { f , g }     {\displaystyle [X_{f},X_{g}]=X_{\omega (X_{g},X_     (3)
      {f})}=-X_{\omega (X_{f},X_{g})}=-X_{\{f,g\}}}  [[X_{f},X_          
      {g}]=X_{\omega (X_{g},X_{f})}=-X_{\omega (X_{f},X_{g})}=-X_{\
      {f,g\}}].
Thus, the Poisson bracket on functions corresponds to the Lie bracket of the
associated Hamiltonian vector fields. We have also shown that the Lie bracket
of two symplectic vector fields is a Hamiltonian vector field and hence is also
symplectic. In the language of abstract_algebra, the symplectic vector fields
form a subalgebra of the Lie_algebra of smooth vector fields on M, and the
Hamiltonian vector fields form an ideal of this subalgebra. The symplectic
vector fields are the Lie algebra of the (infinite-dimensional) Lie_group of
symplectomorphisms of M.
It is widely asserted that the Jacobi_identity for the Poisson bracket,
         &#xA0; { f , { g , h } } + { g , { h , f } } + { h , { f , g } } = 0
      {\displaystyle \ \{f,\{g,h\}\}+\{g,\{h,f\}\}+\{h,\{f,g\}\}=0}  [\ \{f,\
      {g,h\}\}+\{g,\{h,f\}\}+\{h,\{f,g\}\}=0]
follows from the corresponding identity for the Lie bracket of vector fields,
but this is true only up to a locally constant function. However, to prove the
Jacobi identity for the Poisson bracket, it is sufficient to show that:
          ad  { f , g }   = [  ad  f   ,  ad  g   ]   {\displaystyle
      \operatorname {ad} _{\{f,g\}}=[\operatorname {ad} _{f},\operatorname {ad}
      _{g}]}  [\operatorname {ad} _{\{f,g\}}=[\operatorname {ad} _
      {f},\operatorname {ad} _{g}]]
where the operator      ad  g     {\displaystyle \operatorname {ad} _{g}}
[\operatorname {ad} _{g}] on smooth functions on M is defined by      ad  g
&#x2061; ( &#x22C5; )  =  { &#x22C5; ,  g }   {\displaystyle \operatorname {ad}
_{g}(\cdot )\;=\;\{\cdot ,\,g\}}  [{\displaystyle \operatorname {ad} _{g}(\cdot
)\;=\;\{\cdot ,\,g\}}] and the bracket on the right-hand side is the commutator
of operators,     [ A ,  B ]  =  A &#x2061; B &#x2212; B &#x2061; A
{\displaystyle [\operatorname {A} ,\,\operatorname {B} ]\;=\;\operatorname {A}
\operatorname {B} -\operatorname {B} \operatorname {A} }  [{\displaystyle
[\operatorname {A} ,\,\operatorname {B} ]\;=\;\operatorname {A} \operatorname
{B} -\operatorname {B} \operatorname {A} }]. By (1), the operator      ad  g
{\displaystyle \operatorname {ad} _{g}}  [\operatorname {ad} _{g}] is equal to
the operator Xg. The proof of the Jacobi identity follows from (3) because the
Lie bracket of vector fields is just their commutator as differential
operators.
The algebra of smooth functions on M, together with the Poisson bracket forms a
Poisson_algebra, because it is a Lie_algebra under the Poisson bracket, which
additionally satisfies Leibniz's rule (2). We have shown that every symplectic
manifold is a Poisson_manifold, that is a manifold with a "curly-bracket"
operator on smooth functions such that the smooth functions form a Poisson
algebra. However, not every Poisson manifold arises in this way, because
Poisson manifolds allow for degeneracy which cannot arise in the symplectic
case.
***** A result on conjugate momenta[edit] *****
Given a smooth vector_field     X   {\displaystyle X}  [X] on the configuration
space, let      P  X     {\displaystyle P_{X}}  [P_X] be its conjugate
momentum. The conjugate momentum mapping is a Lie_algebra anti-homomorphism
from the Poisson bracket to the Lie_bracket:
         {  P  X   ,  P  Y   } = &#x2212;  P  [ X , Y ]   .    {\displaystyle \
      {P_{X},P_{Y}\}=-P_{[X,Y]}.\,}  [\{P_{X},P_{Y}\}=-P_{[X,Y]}.\,]
This important result is worth a short proof. Write a vector field     X
{\displaystyle X}  [X] at point     q   {\displaystyle q}  [q] in the
configuration_space as
          X  q   =  &#x2211;  i    X  i   ( q )   &#x2202;  &#x2202;  q  i
      {\displaystyle X_{q}=\sum _{i}X^{i}(q){\frac {\partial }{\partial q^
      {i}}}}  [X_{q}=\sum _{i}X^{i}(q){\frac {\partial }{\partial q^{i}}}]
where the        &#x2202;  &#x2202;  q  i         {\displaystyle \scriptstyle
{\frac {\partial }{\partial q^{i}}}}  [\scriptstyle {\frac {\partial }{\partial
q^{i}}}] is the local coordinate frame. The conjugate momentum to     X
{\displaystyle X}  [X] has the expression
          P  X   ( q , p ) =  &#x2211;  i    X  i   ( q )   p  i
      {\displaystyle P_{X}(q,p)=\sum _{i}X^{i}(q)\;p_{i}}  [P_{X}(q,p)=\sum _
      {i}X^{i}(q)\;p_{i}]
where the      p  i     {\displaystyle p_{i}}  [p_{i}] are the momentum
functions conjugate to the coordinates. One then has, for a point     ( q , p )
{\displaystyle (q,p)}  [(q,p)] in the phase_space,
             {  P  X   ,  P  Y   } ( q , p )    =  &#x2211;  i    &#x2211;  j
      {   X  i   ( q )   p  i   ,  Y  j   ( q )   p  j    }        =  &#x2211;
      i j    p  i    Y  j   ( q )    &#x2202;  X  i     &#x2202;  q  j
      &#x2212;  p  j    X  i   ( q )    &#x2202;  Y  j     &#x2202;  q  i
      = &#x2212;  &#x2211;  i    p  i    [ X , Y  ]  i   ( q )       = &#x2212;
      P  [ X , Y ]   ( q , p ) .       {\displaystyle {\begin{aligned}\{P_
      {X},P_{Y}\}(q,p)&=\sum _{i}\sum _{j}\left\{X^{i}(q)\;p_{i},Y^{j}(q)\;p_
      {j}\right\}\\&=\sum _{ij}p_{i}Y^{j}(q){\frac {\partial X^{i}}{\partial q^
      {j}}}-p_{j}X^{i}(q){\frac {\partial Y^{j}}{\partial q^{i}}}\\&=-\sum _
      {i}p_{i}\;[X,Y]^{i}(q)\\&=-P_{[X,Y]}(q,p).\end{aligned}}}  [{\begin
      {aligned}\{P_{X},P_{Y}\}(q,p)&=\sum _{i}\sum _{j}\left\{X^{i}(q)\;p_
      {i},Y^{j}(q)\;p_{j}\right\}\\&=\sum _{ij}p_{i}Y^{j}(q){\frac {\partial X^
      {i}}{\partial q^{j}}}-p_{j}X^{i}(q){\frac {\partial Y^{j}}{\partial q^
      {i}}}\\&=-\sum _{i}p_{i}\;[X,Y]^{i}(q)\\&=-P_{[X,Y]}(q,p).\end{aligned}}]
The above holds for all     ( q , p )   {\displaystyle (q,p)}  [{\displaystyle
(q,p)}], giving the desired result.
***** Quantization[edit] *****
Poisson brackets deform to Moyal_brackets upon quantization, that is, they
generalize to a different Lie algebra, the Moyal_algebra, or, equivalently in
Hilbert_space, quantum commutators. The Wigner-Ä°nÃ¶nÃ¼ group_contraction of
these (the classical limit, Ä§ â 0) yields the above Lie algebra.
To state this more explicitly and precisely, the universal_enveloping_algebra
of the Heisenberg_algebra is the Weyl_algebra (modulo the relation that the
center be the unit). The Moyal product is then a special case of the star
product on the algebra of symbols. An explicit definition of the algebra of
symbols, and the star product is given in the article on the universal
enveloping_algebra.
***** See also[edit] *****
    * Commutator
    * Dirac_bracket
    * Lagrange_bracket
    * Moyal_bracket
    * Peierls_bracket
    * Phase_space
    * Poisson_algebra
    * Poisson_ring
    * Poisson_superalgebra
    * Poisson_superbracket
***** Remarks[edit] *****
   1. ^     f (  p  i   ,   q  i   ,  t )   {\displaystyle f(p_{i},\,q_
      {i},\,t)}  [{\displaystyle f(p_{i},\,q_{i},\,t)}] means     f
      {\displaystyle f}  [f] is a function of the     2 N + 1   {\displaystyle
      2N+1}  [{\displaystyle 2N+1}] independent variables: momentum,     p
      {\displaystyle p}  [p]1â¦N; position,     q   {\displaystyle q}
      [q]1â¦N; and time,     t   {\displaystyle t}  [t]
***** Notes[edit] *****

***** References[edit] *****
    * Arnold,_Vladimir_I. (1989). Mathematical Methods of Classical Mechanics
      (2nd ed.). New York: Springer. ISBN 978-0-387-96890-2.
Landau,_Lev_D.; Lifshitz,_Evegeny_M. (1982). Mechanics. Course_of_Theoretical
Physics. Vol. 1 (3rd ed.). Butterworth-Heinemann. ISBN 978-0-7506-2896-9.
KarasÃ«v, Mikhail V.; Maslov,_Victor_P. (1993). Nonlinear Poisson brackets,
Geometry and Quantization. Translations of Mathematical Monographs. 119.
Translated by Sossinsky, Alexey; Shishkova, M.A. Providence, RI: American
Mathematical Society. ISBN 978-0821887967. MR 1214142.
***** External links[edit] *****
    * Hazewinkel,_Michiel, ed. (2001) [1994], "Poisson_brackets", Encyclopedia
      of_Mathematics, Springer Science+Business Media B.V. / Kluwer Academic
      Publishers, ISBN 978-1-55608-010-4
Eric_W._Weisstein. "Poisson_bracket". MathWorld.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Poisson_bracket&oldid=886595344"
Categories:
    * Symplectic_geometry
    * Hamiltonian_mechanics
    * Bilinear_operators
    * Binary_operations
    * Concepts_in_physics
Hidden categories:
    * CS1:_long_volume_value
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 7 March 2019, at 07:16 (UTC).
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
