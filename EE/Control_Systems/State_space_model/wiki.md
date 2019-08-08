The following text has been accessed from https://en.wikipedia.org/wiki/State-space_representation at Thu Aug 8 22:54:29 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** State-space representation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (May 2009)(Learn_how_and_when
 to_remove_this_template_message)
In control_engineering, a state-space representation is a mathematical model of
a physical system as a set of input, output and state variables related by
first-order differential_equations or difference_equations. State variables are
variables whose values evolve through time in a way that depends on the values
they have at any given time and also depends on the externally imposed values
of input variables. Output variablesâ values depend on the values of the
state variables.
The "state_space" is the Euclidean_space in which the variables on the axes are
the state variables. The state of the system can be represented as a vector
within that space.
To abstract from the number of inputs, outputs and states, these variables are
expressed as vectors. Additionally, if the dynamical_system is linear, time-
invariant, and finite-dimensional, then the differential and algebraic
equations may be written in matrix form.[1][2] The state-space method is
characterized by significant algebraization of general system_theory, which
makes it possible to use Kronecker vector-matrix structures. The capacity of
these structures can be efficiently applied to research systems with modulation
or without it.[3] The state-space representation (also known as the "time-
domain approach") provides a convenient and compact way to model and analyze
systems with multiple inputs and outputs. With     p   {\displaystyle p}  [p]
inputs and     q   {\displaystyle q}  [q] outputs, we would otherwise have to
write down     q &#x00D7; p   {\displaystyle q\times p}  [q\times p] Laplace
transforms to encode all the information about a system. Unlike the frequency
domain approach, the use of the state-space representation is not limited to
systems with linear components and zero initial conditions. The state-space
model is used in many different areas. In econometrics, the state-space model
can be used for forecasting stock_prices[4] and numerous other variables.
⁰
***** Contents *****
    * 1_State_variables
    * 2_Linear_systems
          o 2.1_Example:_continuous-time_LTI_case
          o 2.2_Controllability
          o 2.3_Observability
          o 2.4_Transfer_function
          o 2.5_Canonical_realizations
          o 2.6_Proper_transfer_functions
          o 2.7_Feedback
                # 2.7.1_Example
          o 2.8_Feedback_with_setpoint_(reference)_input
          o 2.9_Moving_object_example
    * 3_Nonlinear_systems
          o 3.1_Pendulum_example
    * 4_See_also
    * 5_References
    * 6_Further_reading
    * 7_External_links
***** State variables[edit] *****
The internal state_variables are the smallest possible subset of system
variables that can represent the entire state of the system at any given time.
[5] The minimum number of state variables required to represent a given system,
n   {\displaystyle n}  [n], is usually equal to the order of the system's
defining differential equation, but not necessarily. If the system is
represented in transfer function form, the minimum number of state variables is
equal to the order of the transfer function's denominator after it has been
reduced to a proper fraction. It is important to understand that converting a
state-space realization to a transfer function form may lose some internal
information about the system, and may provide a description of a system which
is stable, when the state-space realization is unstable at certain points. In
electric circuits, the number of state variables is often, though not always,
the same as the number of energy storage elements in the circuit such as
capacitors and inductors. The state variables defined must be linearly
independent, i.e., no state variable can be written as a linear combination of
the other state variables or the system will not be able to be solved.
***** Linear systems[edit] *****
Block diagram representation of the linear state-space equations
The most general state-space representation of a linear system with     p
{\displaystyle p}  [p] inputs,     q   {\displaystyle q}  [q] outputs and     n
{\displaystyle n}  [n] state variables is written in the following form:[6]
             x  &#x02D9;    ( t ) = A ( t )  x  ( t ) + B ( t )  u  ( t )
      {\displaystyle {\dot {\mathbf {x} }}(t)=A(t)\mathbf {x} (t)+B(t)\mathbf
      {u} (t)}  [{\dot {\mathbf {x} }}(t)=A(t)\mathbf {x} (t)+B(t)\mathbf {u}
      (t)]
          y  ( t ) = C ( t )  x  ( t ) + D ( t )  u  ( t )   {\displaystyle
      \mathbf {y} (t)=C(t)\mathbf {x} (t)+D(t)\mathbf {u} (t)}  [\mathbf {y}
      (t)=C(t)\mathbf {x} (t)+D(t)\mathbf {u} (t)]
where:
          x  ( &#x22C5; )   {\displaystyle \mathbf {x} (\cdot )}  [\mathbf {x}
      (\cdot )] is called the "state vector",       x  ( t ) &#x2208;   R   n
      {\displaystyle \mathbf {x} (t)\in \mathbb {R} ^{n}}  [\mathbf {x} (t)\in
      \mathbb {R} ^{n}];
          y  ( &#x22C5; )   {\displaystyle \mathbf {y} (\cdot )}  [\mathbf {y}
      (\cdot )] is called the "output vector",       y  ( t ) &#x2208;   R   q
      {\displaystyle \mathbf {y} (t)\in \mathbb {R} ^{q}}  [\mathbf {y} (t)\in
      \mathbb {R} ^{q}];
          u  ( &#x22C5; )   {\displaystyle \mathbf {u} (\cdot )}  [\mathbf {u}
      (\cdot )] is called the "input (or control) vector",       u  ( t )
      &#x2208;   R   p     {\displaystyle \mathbf {u} (t)\in \mathbb {R} ^{p}}
      [\mathbf {u} (t)\in \mathbb {R} ^{p}];
         A ( &#x22C5; )   {\displaystyle A(\cdot )}  [A(\cdot )] is the "state
      (or system) matrix",      dim &#x2061; [ A ( &#x22C5; ) ] = n &#x00D7; n
      {\displaystyle \operatorname {dim} [A(\cdot )]=n\times n}  [\operatorname
      {dim} [A(\cdot )]=n\times n],
         B ( &#x22C5; )   {\displaystyle B(\cdot )}  [B(\cdot )] is the "input
      matrix",      dim &#x2061; [ B ( &#x22C5; ) ] = n &#x00D7; p
      {\displaystyle \operatorname {dim} [B(\cdot )]=n\times p}  [\operatorname
      {dim} [B(\cdot )]=n\times p],
         C ( &#x22C5; )   {\displaystyle C(\cdot )}  [C(\cdot )] is the "output
      matrix",      dim &#x2061; [ C ( &#x22C5; ) ] = q &#x00D7; n
      {\displaystyle \operatorname {dim} [C(\cdot )]=q\times n}  [\operatorname
      {dim} [C(\cdot )]=q\times n],
         D ( &#x22C5; )   {\displaystyle D(\cdot )}  [D(\cdot )] is the
      "feedthrough (or feedforward) matrix" (in cases where the system model
      does not have a direct feedthrough,     D ( &#x22C5; )   {\displaystyle D
      (\cdot )}  [D(\cdot )] is the zero matrix),      dim &#x2061; [ D
      ( &#x22C5; ) ] = q &#x00D7; p   {\displaystyle \operatorname {dim} [D
      (\cdot )]=q\times p}  [\operatorname {dim} [D(\cdot )]=q\times p],
             x  &#x02D9;    ( t ) :=   d  d &#x2061; t     x  ( t )
      {\displaystyle {\dot {\mathbf {x} }}(t):={\frac {\operatorname {d} }
      {\operatorname {d} t}}\mathbf {x} (t)}  [{\dot {\mathbf {x} }}(t):={\frac
      {\operatorname {d} }{\operatorname {d} t}}\mathbf {x} (t)].
In this general formulation, all matrices are allowed to be time-variant (i.e.
their elements can depend on time); however, in the common LTI case, matrices
will be time invariant. The time variable     t   {\displaystyle t}  [t] can be
continuous (e.g.     t &#x2208;  R    {\displaystyle t\in \mathbb {R} }  [t\in
\mathbb {R} ]) or discrete (e.g.     t &#x2208;  Z    {\displaystyle t\in
\mathbb {Z} }  [t\in \mathbb {Z} ]). In the latter case, the time variable
k   {\displaystyle k}  [k] is usually used instead of     t   {\displaystyle t}
[t]. Hybrid_systems allow for time domains that have both continuous and
discrete parts. Depending on the assumptions taken, the state-space model
representation can assume the following forms:
System type                      State-space model
Continuous time-invariant               x  &#x02D9;    ( t ) = A  x  ( t ) + B
                                 u  ( t )   {\displaystyle {\dot {\mathbf {x}
                                 }}(t)=A\mathbf {x} (t)+B\mathbf {u} (t)}  [
                                 {\dot {\mathbf {x} }}(t)=A\mathbf {x}
                                 (t)+B\mathbf {u} (t)]
                                     y  ( t ) = C  x  ( t ) + D  u  ( t )
                                 {\displaystyle \mathbf {y} (t)=C\mathbf {x}
                                 (t)+D\mathbf {u} (t)}  [\mathbf {y}
                                 (t)=C\mathbf {x} (t)+D\mathbf {u} (t)]
Continuous time-variant                 x  &#x02D9;    ( t ) =  A  ( t )  x
                                 ( t ) +  B  ( t )  u  ( t )   {\displaystyle
                                 {\dot {\mathbf {x} }}(t)=\mathbf {A}
                                 (t)\mathbf {x} (t)+\mathbf {B} (t)\mathbf {u}
                                 (t)}  [{\dot {\mathbf {x} }}(t)=\mathbf {A}
                                 (t)\mathbf {x} (t)+\mathbf {B} (t)\mathbf {u}
                                 (t)]
                                     y  ( t ) =  C  ( t )  x  ( t ) +  D  ( t )
                                 u  ( t )   {\displaystyle \mathbf {y}
                                 (t)=\mathbf {C} (t)\mathbf {x} (t)+\mathbf {D}
                                 (t)\mathbf {u} (t)}  [\mathbf {y} (t)=\mathbf
                                 {C} (t)\mathbf {x} (t)+\mathbf {D} (t)\mathbf
                                 {u} (t)]
Explicit discrete time-invariant     x  ( k + 1 ) = A  x  ( k ) + B  u  ( k )
                                 {\displaystyle \mathbf {x} (k+1)=A\mathbf {x}
                                 (k)+B\mathbf {u} (k)}  [\mathbf {x}
                                 (k+1)=A\mathbf {x} (k)+B\mathbf {u} (k)]
                                     y  ( k ) = C  x  ( k ) + D  u  ( k )
                                 {\displaystyle \mathbf {y} (k)=C\mathbf {x}
                                 (k)+D\mathbf {u} (k)}  [\mathbf {y}
                                 (k)=C\mathbf {x} (k)+D\mathbf {u} (k)]
Explicit discrete time-variant       x  ( k + 1 ) =  A  ( k )  x  ( k ) +  B
                                 ( k )  u  ( k )   {\displaystyle \mathbf {x}
                                 (k+1)=\mathbf {A} (k)\mathbf {x} (k)+\mathbf
                                 {B} (k)\mathbf {u} (k)}  [\mathbf {x}
                                 (k+1)=\mathbf {A} (k)\mathbf {x} (k)+\mathbf
                                 {B} (k)\mathbf {u} (k)]
                                     y  ( k ) =  C  ( k )  x  ( k ) +  D  ( k )
                                 u  ( k )   {\displaystyle \mathbf {y}
                                 (k)=\mathbf {C} (k)\mathbf {x} (k)+\mathbf {D}
                                 (k)\mathbf {u} (k)}  [\mathbf {y} (k)=\mathbf
                                 {C} (k)\mathbf {x} (k)+\mathbf {D} (k)\mathbf
                                 {u} (k)]
Laplace_domain of                   s  X  ( s ) = A  X  ( s ) + B  U  ( s )
continuous time-invariant        {\displaystyle s\mathbf {X} (s)=A\mathbf {X}
                                 (s)+B\mathbf {U} (s)}  [s\mathbf {X}
                                 (s)=A\mathbf {X} (s)+B\mathbf {U} (s)]
                                     Y  ( s ) = C  X  ( s ) + D  U  ( s )
                                 {\displaystyle \mathbf {Y} (s)=C\mathbf {X}
                                 (s)+D\mathbf {U} (s)}  [\mathbf {Y}
                                 (s)=C\mathbf {X} (s)+D\mathbf {U} (s)]
Z-domain of                         z  X  ( z ) = A  X  ( z ) + B  U  ( z )
discrete time-invariant          {\displaystyle z\mathbf {X} (z)=A\mathbf {X}
                                 (z)+B\mathbf {U} (z)}  [z\mathbf {X}
                                 (z)=A\mathbf {X} (z)+B\mathbf {U} (z)]
                                     Y  ( z ) = C  X  ( z ) + D  U  ( z )
                                 {\displaystyle \mathbf {Y} (z)=C\mathbf {X}
                                 (z)+D\mathbf {U} (z)}  [\mathbf {Y}
                                 (z)=C\mathbf {X} (z)+D\mathbf {U} (z)]
**** Example: continuous-time LTI case[edit] ****
Stability and natural response characteristics of a continuous-time LTI_system
(i.e., linear with matrices that are constant with respect to time) can be
studied from the eigenvalues of the matrix A. The stability of a time-invariant
state-space model can be determined by looking at the system's transfer
function in factored form. It will then look something like this:
           G   ( s ) = k    ( s &#x2212;  z  1   ) ( s &#x2212;  z  2   ) ( s
      &#x2212;  z  3   )   ( s &#x2212;  p  1   ) ( s &#x2212;  p  2   ) ( s
      &#x2212;  p  3   ) ( s &#x2212;  p  4   )    .   {\displaystyle {\textbf
      {G}}(s)=k{\frac {(s-z_{1})(s-z_{2})(s-z_{3})}{(s-p_{1})(s-p_{2})(s-p_{3})
      (s-p_{4})}}.}  [{\displaystyle {\textbf {G}}(s)=k{\frac {(s-z_{1})(s-z_
      {2})(s-z_{3})}{(s-p_{1})(s-p_{2})(s-p_{3})(s-p_{4})}}.}]
The denominator of the transfer function is equal to the characteristic
polynomial found by taking the determinant of     s I &#x2212; A
{\displaystyle sI-A}  [sI-A],
          &#x03BB;  ( s ) =  |  s I &#x2212; A  |  .   {\displaystyle \mathbf
      {\lambda } (s)=|sI-A|.}  [{\displaystyle \mathbf {\lambda } (s)=|sI-A|.}]
The roots of this polynomial (the eigenvalues) are the system transfer
function's poles (i.e., the singularities where the transfer function's
magnitude is unbounded). These poles can be used to analyze whether the system
is asymptotically_stable or marginally_stable. An alternative approach to
determining stability, which does not involve calculating eigenvalues, is to
analyze the system's Lyapunov_stability.
The zeros found in the numerator of       G   ( s )   {\displaystyle {\textbf
{G}}(s)}  [{\textbf {G}}(s)] can similarly be used to determine whether the
system is minimum_phase.
The system may still be input–output stable (see BIBO_stable) even though it is
not internally stable. This may be the case if unstable poles are canceled out
by zeros (i.e., if those singularities in the transfer function are removable).
**** Controllability[edit] ****
Main article: Controllability
The state controllability condition implies that it is possible – by admissible
inputs – to steer the states from any initial value to any final value within
some finite time window. A continuous time-invariant linear state-space model
is controllable if_and_only_if
         rank &#x2061;   [    B   A B    A  2   B   &#x2026;    A  n &#x2212; 1
      B    ]   = n ,   {\displaystyle \operatorname {rank} {\begin
      {bmatrix}B&AB&A^{2}B&\dots &A^{n-1}B\end{bmatrix}}=n,}  [{\displaystyle
      \operatorname {rank} {\begin{bmatrix}B&AB&A^{2}B&\dots &A^{n-1}B\end
      {bmatrix}}=n,}]
where rank is the number of linearly independent rows in a matrix, and where n
is the number of state variables.
**** Observability[edit] ****
Main article: Observability
Observability is a measure for how well internal states of a system can be
inferred by knowledge of its external outputs. The observability and
controllability of a system are mathematical duals (i.e., as controllability
provides that an input is available that brings any initial state to any
desired final state, observability provides that knowing an output trajectory
provides enough information to predict the initial state of the system).
A continuous time-invariant linear state-space model is observable if and only
if
         rank &#x2061;   [    C     C A     &#x22EE;     C  A  n &#x2212; 1
      ]   = n .   {\displaystyle \operatorname {rank} {\begin
      {bmatrix}C\\CA\\\vdots \\CA^{n-1}\end{bmatrix}}=n.}  [{\displaystyle
      \operatorname {rank} {\begin{bmatrix}C\\CA\\\vdots \\CA^{n-1}\end
      {bmatrix}}=n.}]
**** Transfer function[edit] ****
The "transfer_function" of a continuous time-invariant linear state-space model
can be derived in the following way:
First, taking the Laplace_transform of
             x  &#x02D9;    ( t ) = A  x  ( t ) + B  u  ( t )   {\displaystyle
      {\dot {\mathbf {x} }}(t)=A\mathbf {x} (t)+B\mathbf {u} (t)}  [{\dot
      {\mathbf {x} }}(t)=A\mathbf {x} (t)+B\mathbf {u} (t)]
yields
         s  X  ( s ) &#x2212;  x  ( 0 ) = A  X  ( s ) + B  U  ( s ) .
      {\displaystyle s\mathbf {X} (s)-\mathbf {x} (0)=A\mathbf {X} (s)+B\mathbf
      {U} (s).}  [{\displaystyle s\mathbf {X} (s)-\mathbf {x} (0)=A\mathbf {X}
      (s)+B\mathbf {U} (s).}]
Next, we simplify for      X  ( s )   {\displaystyle \mathbf {X} (s)}  [\mathbf
{X} (s)], giving
         ( s  I  &#x2212; A )  X  ( s ) =  x  ( 0 ) + B  U  ( s ) ,
      {\displaystyle (s\mathbf {I} -A)\mathbf {X} (s)=\mathbf {x} (0)+B\mathbf
      {U} (s),}  [{\displaystyle (s\mathbf {I} -A)\mathbf {X} (s)=\mathbf {x}
      (0)+B\mathbf {U} (s),}]
and thus
          X  ( s ) = ( s  I  &#x2212; A  )  &#x2212; 1    x  ( 0 ) + ( s  I
      &#x2212; A  )  &#x2212; 1   B  U  ( s ) .   {\displaystyle \mathbf {X}
      (s)=(s\mathbf {I} -A)^{-1}\mathbf {x} (0)+(s\mathbf {I} -A)^{-1}B\mathbf
      {U} (s).}  [{\displaystyle \mathbf {X} (s)=(s\mathbf {I} -A)^{-1}\mathbf
      {x} (0)+(s\mathbf {I} -A)^{-1}B\mathbf {U} (s).}]
Substituting for      X  ( s )   {\displaystyle \mathbf {X} (s)}  [\mathbf {X}
(s)] in the output equation
          Y  ( s ) = C  X  ( s ) + D  U  ( s ) ,   {\displaystyle \mathbf {Y}
      (s)=C\mathbf {X} (s)+D\mathbf {U} (s),}  [\mathbf {Y} (s)=C\mathbf {X}
      (s)+D\mathbf {U} (s),] giving
          Y  ( s ) = C ( ( s  I  &#x2212; A  )  &#x2212; 1    x  ( 0 ) + ( s  I
      &#x2212; A  )  &#x2212; 1   B  U  ( s ) ) + D  U  ( s ) .
      {\displaystyle \mathbf {Y} (s)=C((s\mathbf {I} -A)^{-1}\mathbf {x} (0)+
      (s\mathbf {I} -A)^{-1}B\mathbf {U} (s))+D\mathbf {U} (s).}  [
      {\displaystyle \mathbf {Y} (s)=C((s\mathbf {I} -A)^{-1}\mathbf {x} (0)+
      (s\mathbf {I} -A)^{-1}B\mathbf {U} (s))+D\mathbf {U} (s).}]
The transfer_function      G  ( s )   {\displaystyle \mathbf {G} (s)}  [\mathbf
{G} (s)] is defined as the ratio of the output to the input of a system
considering its initial conditions to be zero (     x  ( 0 ) =  0
{\displaystyle \mathbf {x} (0)=\mathbf {0} }  [{\displaystyle \mathbf {x}
(0)=\mathbf {0} }]). However, the ratio of a vector to a vector does not exist,
so we consider the following condition satisfied by the transfer function
          G  ( s ) &#x00D7;  U  ( s ) =  Y  ( s )   {\displaystyle \mathbf {G}
      (s)\times \mathbf {U} (s)=\mathbf {Y} (s)}  [{\displaystyle \mathbf {G}
      (s)\times \mathbf {U} (s)=\mathbf {Y} (s)}]
comparison with the equation for      Y  ( s )   {\displaystyle \mathbf {Y}
(s)}  [{\displaystyle \mathbf {Y} (s)}] above gives
          G  ( s ) = C ( s  I  &#x2212; A  )  &#x2212; 1   B + D .
      {\displaystyle \mathbf {G} (s)=C(s\mathbf {I} -A)^{-1}B+D.}  [
      {\displaystyle \mathbf {G} (s)=C(s\mathbf {I} -A)^{-1}B+D.}]
Clearly      G  ( s )   {\displaystyle \mathbf {G} (s)}  [\mathbf {G} (s)] must
have     q   {\displaystyle q}  [q] by     p   {\displaystyle p}  [p]
dimensionality, and thus has a total of     q p   {\displaystyle qp}  [qp]
elements. So for every input there are     q   {\displaystyle q}  [q] transfer
functions with one for each output. This is why the state-space representation
can easily be the preferred choice for multiple-input, multiple-output (MIMO)
systems. The Rosenbrock_system_matrix provides a bridge between the state-space
representation and its transfer_function.
**** Canonical realizations[edit] ****
Main article: Realization_(systems)
Any given transfer function which is strictly_proper can easily be transferred
into state-space by the following approach (this example is for a 4-
dimensional, single-input, single-output system):
Given a transfer function, expand it to reveal all coefficients in both the
numerator and denominator. This should result in the following form:
           G   ( s ) =     n  1    s  3   +  n  2    s  2   +  n  3   s +  n  4
      s  4   +  d  1    s  3   +  d  2    s  2   +  d  3   s +  d  4      .
      {\displaystyle {\textbf {G}}(s)={\frac {n_{1}s^{3}+n_{2}s^{2}+n_{3}s+n_
      {4}}{s^{4}+d_{1}s^{3}+d_{2}s^{2}+d_{3}s+d_{4}}}.}  [{\displaystyle
      {\textbf {G}}(s)={\frac {n_{1}s^{3}+n_{2}s^{2}+n_{3}s+n_{4}}{s^{4}+d_
      {1}s^{3}+d_{2}s^{2}+d_{3}s+d_{4}}}.}]
The coefficients can now be inserted directly into the state-space model by the
following approach:
             x  &#x02D9;    ( t ) =   [    0   1   0   0     0   0   1   0
      0   0   0   1     &#x2212;  d  4     &#x2212;  d  3     &#x2212;  d  2
      &#x2212;  d  1      ]     x   ( t ) +   [    0     0     0     1    ]
      u   ( t )   {\displaystyle {\dot {\textbf {x}}}(t)={\begin
      {bmatrix}0&1&0&0\\0&0&1&0\\0&0&0&1\\-d_{4}&-d_{3}&-d_{2}&-d_{1}\end
      {bmatrix}}{\textbf {x}}(t)+{\begin{bmatrix}0\\0\\0\\1\\\end{bmatrix}}
      {\textbf {u}}(t)}  [{\displaystyle {\dot {\textbf {x}}}(t)={\begin
      {bmatrix}0&1&0&0\\0&0&1&0\\0&0&0&1\\-d_{4}&-d_{3}&-d_{2}&-d_{1}\end
      {bmatrix}}{\textbf {x}}(t)+{\begin{bmatrix}0\\0\\0\\1\\\end{bmatrix}}
      {\textbf {u}}(t)}]
           y   ( t ) =   [     n  4      n  3      n  2      n  1      ]     x
      ( t ) .   {\displaystyle {\textbf {y}}(t)={\begin{bmatrix}n_{4}&n_{3}&n_
      {2}&n_{1}\end{bmatrix}}{\textbf {x}}(t).}  [{\displaystyle {\textbf {y}}
      (t)={\begin{bmatrix}n_{4}&n_{3}&n_{2}&n_{1}\end{bmatrix}}{\textbf {x}}
      (t).}]
This state-space realization is called controllable canonical form because the
resulting model is guaranteed to be controllable (i.e., because the control
enters a chain of integrators, it has the ability to move every state).

The transfer function coefficients can also be used to construct another type
of canonical form
             x  &#x02D9;    ( t ) =   [    0   0   0   &#x2212;  d  4       1
      0   0   &#x2212;  d  3       0   1   0   &#x2212;  d  2       0   0   1
      &#x2212;  d  1      ]     x   ( t ) +   [     n  4        n  3        n
      2        n  1      ]     u   ( t )   {\displaystyle {\dot {\textbf {x}}}
      (t)={\begin{bmatrix}0&0&0&-d_{4}\\1&0&0&-d_{3}\\0&1&0&-d_{2}\\0&0&1&-d_
      {1}\end{bmatrix}}{\textbf {x}}(t)+{\begin{bmatrix}n_{4}\\n_{3}\\n_{2}\\n_
      {1}\end{bmatrix}}{\textbf {u}}(t)}  [{\displaystyle {\dot {\textbf {x}}}
      (t)={\begin{bmatrix}0&0&0&-d_{4}\\1&0&0&-d_{3}\\0&1&0&-d_{2}\\0&0&1&-d_
      {1}\end{bmatrix}}{\textbf {x}}(t)+{\begin{bmatrix}n_{4}\\n_{3}\\n_{2}\\n_
      {1}\end{bmatrix}}{\textbf {u}}(t)}]

           y   ( t ) =   [    0   0   0   1    ]     x   ( t ) .
      {\displaystyle {\textbf {y}}(t)={\begin{bmatrix}0&0&0&1\end{bmatrix}}
      {\textbf {x}}(t).}  [{\displaystyle {\textbf {y}}(t)={\begin
      {bmatrix}0&0&0&1\end{bmatrix}}{\textbf {x}}(t).}]
This state-space realization is called observable canonical form because the
resulting model is guaranteed to be observable (i.e., because the output exits
from a chain of integrators, every state has an effect on the output).
**** Proper transfer functions[edit] ****
Transfer functions which are only proper (and not strictly_proper) can also be
realised quite easily. The trick here is to separate the transfer function into
two parts: a strictly proper part and a constant.
           G   ( s ) =    G     S P    ( s ) +   G   ( &#x221E; ) .
      {\displaystyle {\textbf {G}}(s)={\textbf {G}}_{\mathrm {SP} }(s)+{\textbf
      {G}}(\infty ).}  [{\displaystyle {\textbf {G}}(s)={\textbf {G}}_{\mathrm
      {SP} }(s)+{\textbf {G}}(\infty ).}]
The strictly proper transfer function can then be transformed into a canonical
state-space realization using techniques shown above. The state-space
realization of the constant is trivially       y   ( t ) =   G   ( &#x221E; )
u   ( t )   {\displaystyle {\textbf {y}}(t)={\textbf {G}}(\infty ){\textbf {u}}
(t)}  [{\textbf {y}}(t)={\textbf {G}}(\infty ){\textbf {u}}(t)]. Together we
then get a state-space realization with matrices A, B and C determined by the
strictly proper part, and matrix D determined by the constant.
Here is an example to clear things up a bit:
           G   ( s ) =     s  2   + 3 s + 3    s  2   + 2 s + 1    =    s + 2
      s  2   + 2 s + 1    + 1   {\displaystyle {\textbf {G}}(s)={\frac {s^
      {2}+3s+3}{s^{2}+2s+1}}={\frac {s+2}{s^{2}+2s+1}}+1}  [{\textbf {G}}(s)=
      {\frac {s^{2}+3s+3}{s^{2}+2s+1}}={\frac {s+2}{s^{2}+2s+1}}+1]
which yields the following controllable realization
             x  &#x02D9;    ( t ) =   [    &#x2212; 2   &#x2212; 1     1   0
      ]     x   ( t ) +   [    1     0    ]     u   ( t )   {\displaystyle
      {\dot {\textbf {x}}}(t)={\begin{bmatrix}-2&-1\\1&0\\\end{bmatrix}}
      {\textbf {x}}(t)+{\begin{bmatrix}1\\0\end{bmatrix}}{\textbf {u}}(t)}  [
      {\dot {\textbf {x}}}(t)={\begin{bmatrix}-2&-1\\1&0\\\end{bmatrix}}
      {\textbf {x}}(t)+{\begin{bmatrix}1\\0\end{bmatrix}}{\textbf {u}}(t)]
           y   ( t ) =   [    1   2    ]     x   ( t ) +   [    1    ]     u
      ( t )   {\displaystyle {\textbf {y}}(t)={\begin{bmatrix}1&2\end{bmatrix}}
      {\textbf {x}}(t)+{\begin{bmatrix}1\end{bmatrix}}{\textbf {u}}(t)}  [
      {\textbf {y}}(t)={\begin{bmatrix}1&2\end{bmatrix}}{\textbf {x}}(t)+
      {\begin{bmatrix}1\end{bmatrix}}{\textbf {u}}(t)]
Notice how the output also depends directly on the input. This is due to the
G   ( &#x221E; )   {\displaystyle {\textbf {G}}(\infty )}  [{\textbf {G}}
(\infty )] constant in the transfer function.
**** Feedback[edit] ****
Typical state-space model with feedback
A common method for feedback is to multiply the output by a matrix K and
setting this as the input to the system:      u  ( t ) = K  y  ( t )
{\displaystyle \mathbf {u} (t)=K\mathbf {y} (t)}  [\mathbf {u} (t)=K\mathbf {y}
(t)]. Since the values of K are unrestricted the values can easily be negated
for negative_feedback. The presence of a negative sign (the common notation) is
merely a notational one and its absence has no impact on the end results.
             x  &#x02D9;    ( t ) = A  x  ( t ) + B  u  ( t )   {\displaystyle
      {\dot {\mathbf {x} }}(t)=A\mathbf {x} (t)+B\mathbf {u} (t)}  [{\dot
      {\mathbf {x} }}(t)=A\mathbf {x} (t)+B\mathbf {u} (t)]
          y  ( t ) = C  x  ( t ) + D  u  ( t )   {\displaystyle \mathbf {y}
      (t)=C\mathbf {x} (t)+D\mathbf {u} (t)}  [\mathbf {y} (t)=C\mathbf {x}
      (t)+D\mathbf {u} (t)]
becomes
             x  &#x02D9;    ( t ) = A  x  ( t ) + B K  y  ( t )
      {\displaystyle {\dot {\mathbf {x} }}(t)=A\mathbf {x} (t)+BK\mathbf {y}
      (t)}  [{\dot {\mathbf {x} }}(t)=A\mathbf {x} (t)+BK\mathbf {y} (t)]
          y  ( t ) = C  x  ( t ) + D K  y  ( t )   {\displaystyle \mathbf {y}
      (t)=C\mathbf {x} (t)+DK\mathbf {y} (t)}  [\mathbf {y} (t)=C\mathbf {x}
      (t)+DK\mathbf {y} (t)]
solving the output equation for      y  ( t )   {\displaystyle \mathbf {y} (t)}
[\mathbf {y} (t)] and substituting in the state equation results in
             x  &#x02D9;    ( t ) =  (  A + B K   (  I &#x2212; D K  )
      &#x2212; 1   C  )   x  ( t )   {\displaystyle {\dot {\mathbf {x} }}
      (t)=\left(A+BK\left(I-DK\right)^{-1}C\right)\mathbf {x} (t)}  [{\dot
      {\mathbf {x} }}(t)=\left(A+BK\left(I-DK\right)^{-1}C\right)\mathbf {x}
      (t)]
          y  ( t ) =   (  I &#x2212; D K  )   &#x2212; 1   C  x  ( t )
      {\displaystyle \mathbf {y} (t)=\left(I-DK\right)^{-1}C\mathbf {x} (t)}
      [\mathbf {y} (t)=\left(I-DK\right)^{-1}C\mathbf {x} (t)]
The advantage of this is that the eigenvalues of A can be controlled by setting
K appropriately through eigendecomposition of      (  A + B K   (  I &#x2212; D
K  )   &#x2212; 1   C  )    {\displaystyle \left(A+BK\left(I-DK\right)^{-
1}C\right)}  [\left(A+BK\left(I-DK\right)^{-1}C\right)]. This assumes that the
closed-loop system is controllable or that the unstable eigenvalues of A can be
made stable through appropriate choice of K.
*** Example[edit] ***
For a strictly proper system D equals zero. Another fairly common situation is
when all states are outputs, i.e. y = x, which yields C = I, the Identity
matrix. This would then result in the simpler equations
             x  &#x02D9;    ( t ) =  (  A + B K  )   x  ( t )   {\displaystyle
      {\dot {\mathbf {x} }}(t)=\left(A+BK\right)\mathbf {x} (t)}  [{\dot
      {\mathbf {x} }}(t)=\left(A+BK\right)\mathbf {x} (t)]
          y  ( t ) =  x  ( t )   {\displaystyle \mathbf {y} (t)=\mathbf {x}
      (t)}  [\mathbf {y} (t)=\mathbf {x} (t)]
This reduces the necessary eigendecomposition to just     A + B K
{\displaystyle A+BK}  [A+BK].
**** Feedback with setpoint (reference) input[edit] ****
Output feedback with set point
In addition to feedback, an input,     r ( t )   {\displaystyle r(t)}  [r(t)],
can be added such that      u  ( t ) = &#x2212; K  y  ( t ) +  r  ( t )
{\displaystyle \mathbf {u} (t)=-K\mathbf {y} (t)+\mathbf {r} (t)}  [\mathbf {u}
(t)=-K\mathbf {y} (t)+\mathbf {r} (t)].
             x  &#x02D9;    ( t ) = A  x  ( t ) + B  u  ( t )   {\displaystyle
      {\dot {\mathbf {x} }}(t)=A\mathbf {x} (t)+B\mathbf {u} (t)}  [{\dot
      {\mathbf {x} }}(t)=A\mathbf {x} (t)+B\mathbf {u} (t)]
          y  ( t ) = C  x  ( t ) + D  u  ( t )   {\displaystyle \mathbf {y}
      (t)=C\mathbf {x} (t)+D\mathbf {u} (t)}  [\mathbf {y} (t)=C\mathbf {x}
      (t)+D\mathbf {u} (t)]
becomes
             x  &#x02D9;    ( t ) = A  x  ( t ) &#x2212; B K  y  ( t ) + B  r
      ( t )   {\displaystyle {\dot {\mathbf {x} }}(t)=A\mathbf {x} (t)-
      BK\mathbf {y} (t)+B\mathbf {r} (t)}  [{\dot {\mathbf {x} }}(t)=A\mathbf
      {x} (t)-BK\mathbf {y} (t)+B\mathbf {r} (t)]
          y  ( t ) = C  x  ( t ) &#x2212; D K  y  ( t ) + D  r  ( t )
      {\displaystyle \mathbf {y} (t)=C\mathbf {x} (t)-DK\mathbf {y}
      (t)+D\mathbf {r} (t)}  [\mathbf {y} (t)=C\mathbf {x} (t)-DK\mathbf {y}
      (t)+D\mathbf {r} (t)]
solving the output equation for      y  ( t )   {\displaystyle \mathbf {y} (t)}
[\mathbf {y} (t)] and substituting in the state equation results in
             x  &#x02D9;    ( t ) =  (  A &#x2212; B K   (  I + D K  )
      &#x2212; 1   C  )   x  ( t ) + B  (  I &#x2212; K   (  I + D K  )
      &#x2212; 1   D  )   r  ( t )   {\displaystyle {\dot {\mathbf {x} }}
      (t)=\left(A-BK\left(I+DK\right)^{-1}C\right)\mathbf {x} (t)+B\left(I-
      K\left(I+DK\right)^{-1}D\right)\mathbf {r} (t)}  [{\dot {\mathbf {x} }}
      (t)=\left(A-BK\left(I+DK\right)^{-1}C\right)\mathbf {x} (t)+B\left(I-
      K\left(I+DK\right)^{-1}D\right)\mathbf {r} (t)]
          y  ( t ) =   (  I + D K  )   &#x2212; 1   C  x  ( t ) +   (  I + D K
      )   &#x2212; 1   D  r  ( t )   {\displaystyle \mathbf {y} (t)=\left
      (I+DK\right)^{-1}C\mathbf {x} (t)+\left(I+DK\right)^{-1}D\mathbf {r} (t)}
      [\mathbf {y} (t)=\left(I+DK\right)^{-1}C\mathbf {x} (t)+\left
      (I+DK\right)^{-1}D\mathbf {r} (t)]
One fairly common simplification to this system is removing D, which reduces
the equations to
             x  &#x02D9;    ( t ) =  (  A &#x2212; B K C  )   x  ( t ) + B  r
      ( t )   {\displaystyle {\dot {\mathbf {x} }}(t)=\left(A-BKC\right)\mathbf
      {x} (t)+B\mathbf {r} (t)}  [{\dot {\mathbf {x} }}(t)=\left(A-
      BKC\right)\mathbf {x} (t)+B\mathbf {r} (t)]
          y  ( t ) = C  x  ( t )   {\displaystyle \mathbf {y} (t)=C\mathbf {x}
      (t)}  [\mathbf {y} (t)=C\mathbf {x} (t)]
**** Moving object example[edit] ****
A classical linear system is that of one-dimensional movement of an object.
Newton's_laws_of_motion for an object moving horizontally on a plane and
attached to a wall with a spring
         m    y &#x00A8;    ( t ) = u ( t ) &#x2212; b    y &#x02D9;    ( t )
      &#x2212; k y ( t )   {\displaystyle m{\ddot {y}}(t)=u(t)-b{\dot {y}}(t)-
      ky(t)}  [m{\ddot {y}}(t)=u(t)-b{\dot {y}}(t)-ky(t)]
where
    *    y ( t )   {\displaystyle y(t)}  [y(t)] is position;        y &#x02D9;
      ( t )   {\displaystyle {\dot {y}}(t)}  [{\dot {y}}(t)] is velocity;
      y &#x00A8;    ( t )   {\displaystyle {\ddot {y}}(t)}  [{\ddot {y}}(t)] is
      acceleration
    *    u ( t )   {\displaystyle u(t)}  [u(t)] is an applied force
    *    b   {\displaystyle b}  [b] is the viscous friction coefficient
    *    k   {\displaystyle k}  [k] is the spring constant
    *    m   {\displaystyle m}  [m] is the mass of the object
The state equation would then become
          [          x &#x02D9;     1    ( t )          x &#x02D9;     2    ( t
      )     ]  =  [     0   1     &#x2212;   k m     &#x2212;   b m       ]
      [       x  1    ( t )       x  2    ( t )     ]  +  [     0       1 m
      ]   u  ( t )   {\displaystyle \left[{\begin{matrix}\mathbf {{\dot {x}}_
      {1}} (t)\\\mathbf {{\dot {x}}_{2}} (t)\end{matrix}}\right]=\left[{\begin
      {matrix}0&1\\-{\frac {k}{m}}&-{\frac {b}{m}}\end{matrix}}\right]\left[
      {\begin{matrix}\mathbf {x_{1}} (t)\\\mathbf {x_{2}} (t)\end
      {matrix}}\right]+\left[{\begin{matrix}0\\{\frac {1}{m}}\end
      {matrix}}\right]\mathbf {u} (t)}  [\left[{\begin{matrix}\mathbf {{\dot
      {x}}_{1}} (t)\\\mathbf {{\dot {x}}_{2}} (t)\end{matrix}}\right]=\left[
      {\begin{matrix}0&1\\-{\frac {k}{m}}&-{\frac {b}{m}}\end
      {matrix}}\right]\left[{\begin{matrix}\mathbf {x_{1}} (t)\\\mathbf {x_{2}}
      (t)\end{matrix}}\right]+\left[{\begin{matrix}0\\{\frac {1}{m}}\end
      {matrix}}\right]\mathbf {u} (t)]
          y  ( t ) =  [     1   0     ]   [       x  1    ( t )       x  2
      ( t )     ]    {\displaystyle \mathbf {y} (t)=\left[{\begin
      {matrix}1&0\end{matrix}}\right]\left[{\begin{matrix}\mathbf {x_{1}}
      (t)\\\mathbf {x_{2}} (t)\end{matrix}}\right]}  [\mathbf {y} (t)=\left[
      {\begin{matrix}1&0\end{matrix}}\right]\left[{\begin{matrix}\mathbf {x_
      {1}} (t)\\\mathbf {x_{2}} (t)\end{matrix}}\right]]
where
    *     x  1   ( t )   {\displaystyle x_{1}(t)}  [x_{1}(t)] represents the
      position of the object
    *     x  2   ( t ) =     x &#x02D9;     1   ( t )   {\displaystyle x_{2}
      (t)={\dot {x}}_{1}(t)}  [x_{2}(t)={\dot {x}}_{1}(t)] is the velocity of
      the object
    *        x &#x02D9;     2   ( t ) =     x &#x00A8;     1   ( t )
      {\displaystyle {\dot {x}}_{2}(t)={\ddot {x}}_{1}(t)}  [{\dot {x}}_{2}(t)=
      {\ddot {x}}_{1}(t)] is the acceleration of the object
    * the output      y  ( t )   {\displaystyle \mathbf {y} (t)}  [\mathbf {y}
      (t)] is the position of the object
The controllability test is then
          [     B   A B     ]  =  [      [     0       1 m       ]     [     0
      1     &#x2212;   k m     &#x2212;   b m       ]   [     0       1 m
      ]      ]  =  [     0     1 m         1 m     &#x2212;   b  m  2         ]
      {\displaystyle \left[{\begin{matrix}B&AB\end{matrix}}\right]=\left[
      {\begin{matrix}\left[{\begin{matrix}0\\{\frac {1}{m}}\end
      {matrix}}\right]&\left[{\begin{matrix}0&1\\-{\frac {k}{m}}&-{\frac {b}
      {m}}\end{matrix}}\right]\left[{\begin{matrix}0\\{\frac {1}{m}}\end
      {matrix}}\right]\end{matrix}}\right]=\left[{\begin{matrix}0&{\frac {1}
      {m}}\\{\frac {1}{m}}&-{\frac {b}{m^{2}}}\end{matrix}}\right]}  [\left[
      {\begin{matrix}B&AB\end{matrix}}\right]=\left[{\begin{matrix}\left[
      {\begin{matrix}0\\{\frac {1}{m}}\end{matrix}}\right]&\left[{\begin
      {matrix}0&1\\-{\frac {k}{m}}&-{\frac {b}{m}}\end{matrix}}\right]\left[
      {\begin{matrix}0\\{\frac {1}{m}}\end{matrix}}\right]\end
      {matrix}}\right]=\left[{\begin{matrix}0&{\frac {1}{m}}\\{\frac {1}{m}}&-
      {\frac {b}{m^{2}}}\end{matrix}}\right]]
which has full rank for all     b   {\displaystyle b}  [b] and     m
{\displaystyle m}  [m].
The observability test is then
          [     C     C A     ]  =  [      [     1   0     ]       [     1   0
      ]   [     0   1     &#x2212;   k m     &#x2212;   b m       ]      ]  =
      [     1   0     0   1     ]    {\displaystyle \left[{\begin
      {matrix}C\\CA\end{matrix}}\right]=\left[{\begin{matrix}\left[{\begin
      {matrix}1&0\end{matrix}}\right]\\\left[{\begin{matrix}1&0\end
      {matrix}}\right]\left[{\begin{matrix}0&1\\-{\frac {k}{m}}&-{\frac {b}
      {m}}\end{matrix}}\right]\end{matrix}}\right]=\left[{\begin
      {matrix}1&0\\0&1\end{matrix}}\right]}  [\left[{\begin{matrix}C\\CA\end
      {matrix}}\right]=\left[{\begin{matrix}\left[{\begin{matrix}1&0\end
      {matrix}}\right]\\\left[{\begin{matrix}1&0\end{matrix}}\right]\left[
      {\begin{matrix}0&1\\-{\frac {k}{m}}&-{\frac {b}{m}}\end
      {matrix}}\right]\end{matrix}}\right]=\left[{\begin{matrix}1&0\\0&1\end
      {matrix}}\right]]
which also has full rank. Therefore, this system is both controllable and
observable.
***** Nonlinear systems[edit] *****
The more general form of a state-space model can be written as two functions.
            x &#x02D9;    ( t ) =  f  ( t , x ( t ) , u ( t ) )
      {\displaystyle \mathbf {\dot {x}} (t)=\mathbf {f} (t,x(t),u(t))}
      [\mathbf {\dot {x}} (t)=\mathbf {f} (t,x(t),u(t))]
          y  ( t ) =  h  ( t , x ( t ) , u ( t ) )   {\displaystyle \mathbf {y}
      (t)=\mathbf {h} (t,x(t),u(t))}  [\mathbf {y} (t)=\mathbf {h} (t,x(t),u
      (t))]
The first is the state equation and the latter is the output equation. If the
function     f ( &#x22C5; , &#x22C5; , &#x22C5; )   {\displaystyle f(\cdot
,\cdot ,\cdot )}  [f(\cdot ,\cdot ,\cdot )] is a linear combination of states
and inputs then the equations can be written in matrix notation like above. The
u ( t )   {\displaystyle u(t)}  [u(t)] argument to the functions can be dropped
if the system is unforced (i.e., it has no inputs).
**** Pendulum example[edit] ****
A classic nonlinear system is a simple unforced pendulum
         m  &#x2113;  2      &#x03B8; &#x00A8;    ( t ) = &#x2212; m &#x2113; g
      sin &#x2061; &#x03B8; ( t ) &#x2212; k &#x2113;    &#x03B8; &#x02D9;
      ( t )   {\displaystyle m\ell ^{2}{\ddot {\theta }}(t)=-m\ell g\sin \theta
      (t)-k\ell {\dot {\theta }}(t)}  [m\ell ^{2}{\ddot {\theta }}(t)=-m\ell
      g\sin \theta (t)-k\ell {\dot {\theta }}(t)]
where
    *    &#x03B8; ( t )   {\displaystyle \theta (t)}  [\theta (t)] is the angle
      of the pendulum with respect to the direction of gravity
    *    m   {\displaystyle m}  [m] is the mass of the pendulum (pendulum rod's
      mass is assumed to be zero)
    *    g   {\displaystyle g}  [g] is the gravitational acceleration
    *    k   {\displaystyle k}  [k] is coefficient of friction at the pivot
      point
    *    &#x2113;   {\displaystyle \ell }  [\ell ] is the radius of the
      pendulum (to the center of gravity of the mass     m   {\displaystyle m}
      [m])
The state equations are then
             x &#x02D9;     1   ( t ) =  x  2   ( t )   {\displaystyle {\dot
      {x}}_{1}(t)=x_{2}(t)}  [{\displaystyle {\dot {x}}_{1}(t)=x_{2}(t)}]
             x &#x02D9;     2   ( t ) = &#x2212;   g &#x2113;   sin &#x2061;
      x  1    ( t ) &#x2212;   k  m &#x2113;      x  2    ( t )
      {\displaystyle {\dot {x}}_{2}(t)=-{\frac {g}{\ell }}\sin {x_{1}}(t)-
      {\frac {k}{m\ell }}{x_{2}}(t)}  [{\displaystyle {\dot {x}}_{2}(t)=-{\frac
      {g}{\ell }}\sin {x_{1}}(t)-{\frac {k}{m\ell }}{x_{2}}(t)}]
where
    *     x  1   ( t ) = &#x03B8; ( t )   {\displaystyle x_{1}(t)=\theta (t)}
      [x_{1}(t)=\theta (t)] is the angle of the pendulum
    *     x  2   ( t ) =     x &#x02D9;     1   ( t )   {\displaystyle x_{2}
      (t)={\dot {x}}_{1}(t)}  [x_{2}(t)={\dot {x}}_{1}(t)] is the rotational
      velocity of the pendulum
    *        x &#x02D9;     2   =     x &#x00A8;     1     {\displaystyle {\dot
      {x}}_{2}={\ddot {x}}_{1}}  [{\displaystyle {\dot {x}}_{2}={\ddot {x}}_
      {1}}] is the rotational acceleration of the pendulum
Instead, the state equation can be written in the general form
             x  &#x02D9;    ( t ) =  (         x &#x02D9;     1   ( t )
      x &#x02D9;     2   ( t )     )  =  f  ( t , x ( t ) ) =  (      x  2
      ( t )     &#x2212;   g &#x2113;   sin &#x2061;   x  1    ( t ) &#x2212;
      k  m &#x2113;      x  2    ( t )     )  .   {\displaystyle {\dot {\mathbf
      {x} }}(t)=\left({\begin{matrix}{\dot {x}}_{1}(t)\\{\dot {x}}_{2}(t)\end
      {matrix}}\right)=\mathbf {f} (t,x(t))=\left({\begin{matrix}x_{2}(t)\\-
      {\frac {g}{\ell }}\sin {x_{1}}(t)-{\frac {k}{m\ell }}{x_{2}}(t)\end
      {matrix}}\right).}  [{\displaystyle {\dot {\mathbf {x} }}(t)=\left(
      {\begin{matrix}{\dot {x}}_{1}(t)\\{\dot {x}}_{2}(t)\end
      {matrix}}\right)=\mathbf {f} (t,x(t))=\left({\begin{matrix}x_{2}(t)\\-
      {\frac {g}{\ell }}\sin {x_{1}}(t)-{\frac {k}{m\ell }}{x_{2}}(t)\end
      {matrix}}\right).}]
The equilibrium/stationary_points of a system are when        x &#x02D9;    = 0
{\displaystyle {\dot {x}}=0}  [{\dot {x}}=0] and so the equilibrium points of a
pendulum are those that satisfy
          (      x  1        x  2       )  =  (     n &#x03C0;     0     )
      {\displaystyle \left({\begin{matrix}x_{1}\\x_{2}\end
      {matrix}}\right)=\left({\begin{matrix}n\pi \\0\end{matrix}}\right)}
      [\left({\begin{matrix}x_{1}\\x_{2}\end{matrix}}\right)=\left({\begin
      {matrix}n\pi \\0\end{matrix}}\right)]
for integers n.
***** See also[edit] *****
    * Control_engineering
    * Control_theory
    * State_observer
    * Observability
    * Controllability
    * Discretization of state-space models
    * Phase_space for information about phase state (like state space) in
      physics and mathematics.
    * State_space for information about state space with discrete states in
      computer science.
    * State_space_(physics) for information about state space in physics.
    * Kalman_filter for a statistical application.
***** References[edit] *****
   1. ^ Katalin M. Hangos; R. Lakner & M. Gerzson (2001). Intelligent_Control
      Systems:_An_Introduction_with_Examples. Springer. p. 254. ISBN 978-1-
      4020-0134-5.
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
   3. ^ Katalin M. Hangos; JÃ³zsef Bokor & GÃ¡bor SzederkÃ©nyi (2004). Analysis
      and_Control_of_Nonlinear_Process_Systems. Springer. p. 25. ISBN 978-1-
      85233-600-4.
   4. ^Vasilyev A.S.; Ushakov A.V. (2015). "Modeling_of_dynamic_systems_with
      modulation_by_means_of_Kronecker_vector-matrix_representation".
      Scientific and Technical Journal of Information Technologies, Mechanics
      and Optics. 15 (5): 839â848.
   5. ^ Rita Yi Man Li,Kwong Wing Chau (2016) Econometric Analyses of
      International Housing Markets, Routledge, https://books.google.com.hk/
      books?hl=en&lr=&id=xyneCwAAQBAJ&oi=fnd&pg=PA57&dq=%22Rita+yi+man+li%22&ots=7YTLXxGi5z&sig=1j-
      NKyZu1yGUbzUv_O84z2bysTc&redir_esc=y#v=onepage&q=%22Rita%20yi%20man%20li%22&f=false
   6. ^Nise, Norman S. (2010). Control Systems Engineering (6th ed.). John
      Wiley & Sons, Inc. ISBN 978-0-470-54756-4.
   7. ^Brogan, William L. (1974). Modern Control Theory (1st ed.). Quantum
      Publishers, Inc. p. 172.
***** Further reading[edit] *****
    * Antsaklis, P. J.; Michel, A. N. (2007). A Linear Systems Primer.
      Birkhauser. ISBN 978-0-8176-4460-4.
Chen, Chi-Tsong (1999). Linear System Theory and Design (3rd ed.). Oxford
University Press. ISBN 0-19-511777-8.
Khalil, Hassan K. (2001). Nonlinear Systems (3rd ed.). Prentice Hall. ISBN 0-
13-067389-7.
Hinrichsen, Diederich; Pritchard, Anthony J. (2005). Mathematical Systems
Theory I, Modelling, State Space Analysis, Stability and Robustness. Springer.
ISBN 978-3-540-44125-0.
Sontag, Eduardo D. (1999). Mathematical_Control_Theory:_Deterministic_Finite
Dimensional_Systems (PDF) (2nd ed.). Springer. ISBN 0-387-98489-5. Retrieved
June 28, 2012.
Friedland, Bernard (2005). Control System Design: An Introduction to State-
Space Methods. Dover. ISBN 0-486-44278-0.
Zadeh, Lotfi A.; Desoer, Charles A. (1979). Linear System Theory. Krieger Pub
Co. ISBN 978-0-88275-809-1.
  On the applications of state-space models in econometrics
    * Durbin, J.; Koopman, S. (2001). Time series analysis by state space
      methods. Oxford, UK: Oxford University Press. ISBN 978-0-19-852354-3.
***** External links[edit] *****
    * Wolfram_language functions for linear_state-space_models, affine_state-
      space_models, and nonlinear_state-space_models.

Retrieved from "https://en.wikipedia.org/w/index.php?title=State-
space_representation&oldid=891707011"
Categories:
    * Classical_control_theory
    * Mathematical_modeling
    * Time_domain_analysis
    * Time_series_models
Hidden categories:
    * Articles_lacking_in-text_citations_from_May_2009
    * All_articles_lacking_in-text_citations
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
    * CatalÃ 
    * ÄeÅ¡tina
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * ä¸­æ
Edit_links
    * This page was last edited on 9 April 2019, at 17:13 (UTC).
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
