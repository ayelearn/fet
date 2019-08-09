The following text has been accessed from https://en.wikipedia.org/wiki/Simulated_annealing at Thu Aug 8 23:28:41 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Simulated annealing ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Probabilistic optimization technique and metaheuristic
 This article needs additional citations for verification. Please help improve_this
 article by adding_citations_to_reliable_sources. Unsourced material may be challenged
 and removed.
 Find sources: "Simulated_annealing" â news Â· newspapers Â· books Â· scholar Â·
 JSTOR (December 2009)(Learn_how_and_when_to_remove_this_template_message)
Simulated Annealing can be used to solve combinatorial problems. Here it is
applied to the travelling_salesman_problem to minimize the length of a route
that connects all 125 points.
Simulated annealing (SA) is a probabilistic_technique for approximating the
global_optimum of a given function. Specifically, it is a metaheuristic to
approximate global_optimization in a large search_space for an optimization
problem. It is often used when the search space is discrete (e.g., the
traveling_salesman_problem). For problems where finding an approximate global
optimum is more important than finding a precise local optimum in a fixed
amount of time, simulated annealing may be preferable to alternatives such as
gradient_descent.
The name and inspiration come from annealing_in_metallurgy, a technique
involving heating and controlled cooling of a material to increase the size of
its crystals and reduce their defects. Both are attributes of the material that
depend on its thermodynamic free energy. Heating and cooling the material
affects both the temperature and the thermodynamic free energy. The simulation
of annealing can be used to find an approximation of a global minimum for a
function with a large number of variables.[1][2]
This notion of slow cooling implemented in the simulated annealing algorithm is
interpreted as a slow decrease in the probability of accepting worse solutions
as the solution space is explored. Accepting worse solutions is a fundamental
property of metaheuristics because it allows for a more extensive search for
the global optimal solution. In general, the simulated annealing algorithms
work as follows. At each time step, the algorithm randomly selects a solution
close to the current one, measures its quality, and then decides to move to it
or to stay with the current solution based on either one of two probabilities
between which it chooses on the basis of the fact that the new solution is
better or worse than the current one. During the search, the temperature is
progressively decreased from an initial positive value to zero and affects the
two probabilities: at each step, the probability of moving to a better new
solution is either kept to 1 or is changed towards a positive value; on the
other hand, the probability of moving to a worse new solution is progressively
changed towards zero.
The simulation can be performed either by a solution of kinetic equations for
density functions[1][2] or by using the stochastic sampling method.[3][4][5]
The method is an adaptation of the MetropolisâHastings_algorithm, a Monte
Carlo_method to generate sample states of a thermodynamic system, published by
N._Metropolis et al. in 1953.[6]
⁰
***** Contents *****
    * 1_Overview
          o 1.1_The_basic_iteration
          o 1.2_The_neighbours_of_a_state
          o 1.3_Acceptance_probabilities
          o 1.4_The_annealing_schedule
    * 2_Pseudocode
    * 3_Selecting_the_parameters
          o 3.1_Sufficiently_near_neighbour
          o 3.2_Transition_probabilities
          o 3.3_Acceptance_probabilities
          o 3.4_Efficient_candidate_generation
          o 3.5_Barrier_avoidance
          o 3.6_Cooling_schedule
    * 4_Restarts
    * 5_Related_methods
    * 6_See_also
    * 7_References
    * 8_Further_reading
    * 9_External_links
***** Overview[edit] *****
The state of some physical_systems, and the function E(s) to be minimized, is
analogous to the internal_energy of the system in that state. The goal is to
bring the system, from an arbitrary initial state, to a state with the minimum
possible energy.
Simulated annealing searching for a maximum. The objective here is to get to
the highest point; however, it is not enough to use a simple hill_climb
algorithm, as there are many local_maxima. By cooling the temperature slowly
the global maximum is found.
**** The basic iteration[edit] ****
At each step, the simulated annealing heuristic considers some neighboring
state s* of the current state s, and probabilistically decides between moving
the system to state s* or staying in-state s. These probabilities ultimately
lead the system to move to states of lower energy. Typically this step is
repeated until the system reaches a state that is good enough for the
application, or until a given computation budget has been exhausted.
**** The neighbours of a state[edit] ****
Optimization of a solution involves evaluating the neighbours of a state of the
problem, which are new states produced through conservatively altering a given
state. For example, in the travelling_salesman_problem each state is typically
defined as a permutation of the cities to be visited, and its neighbours are
the set of permutations produced by reversing the order of any two successive
cities. The well-defined way in which the states are altered to produce
neighbouring states is called a "move", and different moves give different sets
of neighbouring states. These moves usually result in minimal alterations of
the last state, in an attempt to progressively improve the solution through
iteratively improving its parts (such as the city connections in the traveling
salesman problem).
Simple heuristics like hill_climbing, which move by finding better neighbour
after better neighbour and stop when they have reached a solution which has no
neighbours that are better solutions, cannot guarantee to lead to any of the
existing better solutions – their outcome may easily be just a local_optimum,
while the actual best solution would be a global_optimum that could be
different. Metaheuristics use the neighbours of a solution as a way to explore
the solutions space, and although they prefer better neighbours, they also
accept worse neighbours in order to avoid getting stuck in local optima; they
can find the global optimum if run for a long enough amount of time.
**** Acceptance probabilities[edit] ****
The probability of making the transition from the current state     s
{\displaystyle s}  [s] to a candidate new state      s &#x2032;
{\displaystyle s'}  [s'] is specified by an acceptance probability function
P ( e ,  e &#x2032;  , T )   {\displaystyle P(e,e',T)}  [P(e,e',T)], that
depends on the energies     e = E ( s )   {\displaystyle e=E(s)}  [e=E(s)] and
e &#x2032;  = E (  s &#x2032;  )   {\displaystyle e'=E(s')}  [e'=E(s')] of the
two states, and on a global time-varying parameter     T   {\displaystyle T}
[T] called the temperature. States with a smaller energy are better than those
with a greater energy. The probability function     P   {\displaystyle P}  [P]
must be positive even when      e &#x2032;    {\displaystyle e'}  [e'] is
greater than     e   {\displaystyle e}  [e]. This feature prevents the method
from becoming stuck at a local minimum that is worse than the global one.
When     T   {\displaystyle T}  [T] tends to zero, the probability     P ( e ,
e &#x2032;  , T )   {\displaystyle P(e,e',T)}  [P(e,e',T)] must tend to zero if
e &#x2032;  > e   {\displaystyle e'>e}  [e'>e] and to a positive value
otherwise. For sufficiently small values of     T   {\displaystyle T}  [T], the
system will then increasingly favor moves that go "downhill" (i.e., to lower
energy values), and avoid those that go "uphill." With     T = 0
{\displaystyle T=0}  [T=0] the procedure reduces to the greedy_algorithm, which
makes only the downhill transitions.
In the original description of simulated annealing, the probability     P ( e ,
e &#x2032;  , T )   {\displaystyle P(e,e',T)}  [P(e,e',T)] was equal to 1 when
e &#x2032;  < e   {\displaystyle e'<e}  [e'<e]âi.e., the procedure always
moved downhill when it found a way to do so, irrespective of the temperature.
Many descriptions and implementations of simulated annealing still take this
condition as part of the method's definition. However, this condition is not
essential for the method to work.
The     P   {\displaystyle P}  [P] function is usually chosen so that the
probability of accepting a move decreases when the difference      e &#x2032;
&#x2212; e   {\displaystyle e'-e}  [e'-e] increasesâthat is, small uphill
moves are more likely than large ones. However, this requirement is not
strictly necessary, provided that the above requirements are met.
Given these properties, the temperature     T   {\displaystyle T}  [T] plays a
crucial role in controlling the evolution of the state     s   {\displaystyle
s}  [s] of the system with regard to its sensitivity to the variations of
system energies. To be precise, for a large     T   {\displaystyle T}  [T], the
evolution of     s   {\displaystyle s}  [s] is sensitive to coarser energy
variations, while it is sensitive to finer energy variations when     T
{\displaystyle T}  [T] is small.
**** The annealing schedule[edit] ****
The name and inspiration of the algorithm demand an interesting feature related
to the temperature variation to be embedded in the operational characteristics
of the algorithm. This necessitates a gradual reduction of the temperature as
the simulation proceeds. The algorithm starts initially with     T
{\displaystyle T}  [T] set to a high value (or infinity), and then it is
decreased at each step following some annealing scheduleâwhich may be
specified by the user, but must end with     T = 0   {\displaystyle T=0}  [T=0]
towards the end of the allotted time budget. In this way, the system is
expected to wander initially towards a broad region of the search space
containing good solutions, ignoring small features of the energy function; then
drift towards low-energy regions that become narrower and narrower; and finally
move downhill according to the steepest_descent heuristic.
Fast Slow
Example illustrating the effect of cooling schedule on the performance of
simulated annealing. The problem is to rearrange the pixels of an image so as
to minimize a certain potential_energy function, which causes similar colours
to attract at short range and repel at a slightly larger distance. The
elementary moves swap two adjacent pixels. These images were obtained with a
fast cooling schedule (left) and a slow cooling schedule (right), producing
results similar to amorphous and crystalline_solids, respectively.
For any given finite problem, the probability that the simulated annealing
algorithm terminates with a global_optimal solution approaches 1 as the
annealing schedule is extended.[7] This theoretical result, however, is not
particularly helpful, since the time required to ensure a significant
probability of success will usually exceed the time required for a complete
search of the solution_space.[citation_needed]
***** Pseudocode[edit] *****
The following pseudocode presents the simulated annealing heuristic as
described above. It starts from a state s0 and continues until a maximum of
kmax steps have been taken. In the process, the call neighbour(s) should
generate a randomly chosen neighbour of a given state s; the call random(0, 1)
should pick and return a value in the range [0, 1], uniformly_at_random. The
annealing schedule is defined by the call temperature(r), which should yield
the temperature to use, given the fraction r of the time budget that has been
expended so far.
    * Let s = s0
    * For k = 0 through kmax (exclusive):
          o T â temperature( kmax/(k+1) )
          o Pick a random neighbour, snew â neighbour(s)
          o If P(E(s), E(snew), T) â¥ random(0, 1):
                # s â snew
    * Output: the final state s
***** Selecting the parameters[edit] *****
In order to apply the simulated annealing method to a specific problem, one
must specify the following parameters: the state space, the energy (goal)
function E(), the candidate generator procedure neighbour(), the acceptance
probability function P(), and the annealing schedule temperature() AND initial
temperature <init temp>. These choices can have a significant impact on the
method's effectiveness. Unfortunately, there are no choices of these parameters
that will be good for all problems, and there is no general way to find the
best choices for a given problem. The following sections give some general
guidelines.
**** Sufficiently near neighbour[edit] ****
Simulated annealing may be modeled as a random walk on a search graph, whose
vertices are all possible states, and whose edges are the candidate moves. An
essential requirement for the neighbour() function is that it must provide a
sufficiently short path on this graph from the initial state to any state which
may be the global optimum – the diameter of the search graph must be small. In
the traveling salesman example above, for instance, the search space for n = 20
cities has n! = 2,432,902,008,176,640,000 (2.4 quintillion) states; yet the
neighbor generator function that swaps two consecutive cities can get from any
state (tour) to any other state in at most      &#x2211;  k = 1   n &#x2212; 1
k =    n ( n &#x2212; 1 )  2   = 190   {\displaystyle \sum _{k=1}^{n-1}k={\frac
{n(n-1)}{2}}=190}  [{\displaystyle \sum _{k=1}^{n-1}k={\frac {n(n-1)}{2}}=190}]
steps.
**** Transition probabilities[edit] ****
To investigate the behavior of simulated annealing on a particular problem, it
can be useful to consider the transition probabilities that result from the
various design choices made in the implementation of the algorithm. For each
edge     ( s ,  s &#x2032;  )   {\displaystyle (s,s')}  [(s,s')] of the search
graph, the transition probability is defined as the probability that the
simulated annealing algorithm will move to state      s &#x2032;
{\displaystyle s'}  [s'] when its current state is     s   {\displaystyle s}
[s]. This probability depends on the current temperature as specified by
temperature(), on the order in which the candidate moves are generated by the
neighbour() function, and on the acceptance probability function P(). (Note
that the transition probability is not simply     P ( e ,  e &#x2032;  , T )
{\displaystyle P(e,e',T)}  [P(e,e',T)], because the candidates are tested
serially.)
**** Acceptance probabilities[edit] ****
The specification of neighbour(), P(), and temperature() is partially
redundant. In practice, it's common to use the same acceptance function P() for
many problems, and adjust the other two functions according to the specific
problem.
In the formulation of the method by Kirkpatrick et al., the acceptance
probability function     P ( e ,  e &#x2032;  , T )   {\displaystyle P(e,e',T)}
[P(e,e',T)] was defined as 1 if      e &#x2032;  < e   {\displaystyle e'<e}
[e'<e], and     exp &#x2061; ( &#x2212; (  e &#x2032;  &#x2212; e )  /  T )
{\displaystyle \exp(-(e'-e)/T)}  [\exp(-(e'-e)/T)] otherwise. This formula was
superficially justified by analogy with the transitions of a physical system;
it corresponds to the MetropolisâHastings_algorithm, in the case where T=1
and the proposal distribution of MetropolisâHastings is symmetric. However,
this acceptance probability is often used for simulated annealing even when the
neighbour() function, which is analogous to the proposal distribution in
MetropolisâHastings, is not symmetric, or not probabilistic at all. As a
result, the transition probabilities of the simulated annealing algorithm do
not correspond to the transitions of the analogous physical system, and the
long-term distribution of states at a constant temperature     T
{\displaystyle T}  [T] need not bear any resemblance to the thermodynamic
equilibrium distribution over states of that physical system, at any
temperature. Nevertheless, most descriptions of simulated annealing assume the
original acceptance function, which is probably hard-coded in many
implementations of SA.
**** Efficient candidate generation[edit] ****
When choosing the candidate generator neighbour(), one must consider that after
a few iterations of the simulated annealing algorithm, the current state is
expected to have much lower energy than a random state. Therefore, as a general
rule, one should skew the generator towards candidate moves where the energy of
the destination state      s &#x2032;    {\displaystyle s'}  [s'] is likely to
be similar to that of the current state. This heuristic (which is the main
principle of the MetropolisâHastings_algorithm) tends to exclude "very good"
candidate moves as well as "very bad" ones; however, the former are usually
much less common than the latter, so the heuristic is generally quite
effective.
In the traveling salesman problem above, for example, swapping two consecutive
cities in a low-energy tour is expected to have a modest effect on its energy
(length); whereas swapping two arbitrary cities is far more likely to increase
its length than to decrease it. Thus, the consecutive-swap neighbour generator
is expected to perform better than the arbitrary-swap one, even though the
latter could provide a somewhat shorter path to the optimum (with     n
&#x2212; 1   {\displaystyle n-1}  [n-1] swaps, instead of     n ( n &#x2212; 1
)  /  2   {\displaystyle n(n-1)/2}  [n(n-1)/2]).
A more precise statement of the heuristic is that one should try first
candidate states      s &#x2032;    {\displaystyle s'}  [s'] for which     P
( E ( s ) , E (  s &#x2032;  ) , T )   {\displaystyle P(E(s),E(s'),T)}  [P(E
(s),E(s'),T)] is large. For the "standard" acceptance function     P
{\displaystyle P}  [P] above, it means that     E (  s &#x2032;  ) &#x2212; E
( s )   {\displaystyle E(s')-E(s)}  [E(s')-E(s)] is on the order of     T
{\displaystyle T}  [T] or less. Thus, in the traveling salesman example above,
one could use a neighbour() function that swaps two random cities, where the
probability of choosing a city pair vanishes as their distance increases beyond
T   {\displaystyle T}  [T].
**** Barrier avoidance[edit] ****
When choosing the candidate generator neighbour() one must also try to reduce
the number of "deep" local minimaâstates (or sets of connected states) that
have much lower energy than all its neighbouring states. Such "closed catchment
basins" of the energy function may trap the simulated annealing algorithm with
high probability (roughly proportional to the number of states in the basin)
and for a very long time (roughly exponential on the energy difference between
the surrounding states and the bottom of the basin).
As a rule, it is impossible to design a candidate generator that will satisfy
this goal and also prioritize candidates with similar energy. On the other
hand, one can often vastly improve the efficiency of simulated annealing by
relatively simple changes to the generator. In the traveling salesman problem,
for instance, it is not hard to exhibit two tours     A   {\displaystyle A}
[A],     B   {\displaystyle B}  [B], with nearly equal lengths, such that (1)
A   {\displaystyle A}  [A] is optimal, (2) every sequence of city-pair swaps
that converts     A   {\displaystyle A}  [A] to     B   {\displaystyle B}  [B]
goes through tours that are much longer than both, and (3)     A
{\displaystyle A}  [A] can be transformed into     B   {\displaystyle B}  [B]
by flipping (reversing the order of) a set of consecutive cities. In this
example,     A   {\displaystyle A}  [A] and     B   {\displaystyle B}  [B] lie
in different "deep basins" if the generator performs only random pair-swaps;
but they will be in the same basin if the generator performs random segment-
flips.
**** Cooling schedule[edit] ****
The physical analogy that is used to justify simulated annealing assumes that
the cooling rate is low enough for the probability distribution of the current
state to be near thermodynamic_equilibrium at all times. Unfortunately, the
relaxation timeâthe time one must wait for the equilibrium to be restored
after a change in temperatureâstrongly depends on the "topography" of the
energy function and on the current temperature. In the simulated annealing
algorithm, the relaxation time also depends on the candidate generator, in a
very complicated way. Note that all these parameters are usually provided as
black_box_functions to the simulated annealing algorithm. Therefore, the ideal
cooling rate cannot be determined beforehand, and should be empirically
adjusted for each problem. Adaptive_simulated_annealing algorithms address this
problem by connecting the cooling schedule to the search progress. Other
adaptive approach as Thermodynamic Simulated Annealing[8], automatically
adjusts the temperature at each step based on the energy difference between the
two states, according to the laws of thermodynamics.
***** Restarts[edit] *****
Sometimes it is better to move back to a solution that was significantly better
rather than always moving from the current state. This process is called
restarting of simulated annealing. To do this we set s and e to sbest and ebest
and perhaps restart the annealing schedule. The decision to restart could be
based on several criteria. Notable among these include restarting based on a
fixed number of steps, based on whether the current energy is too high compared
to the best energy obtained so far, restarting randomly, etc.
***** Related methods[edit] *****
    * Interacting_MetropolisâHasting_algorithms (a.k.a. Sequential_Monte
      Carlo[9]) combined simulated annealing moves with an acceptance-rejection
      of the best fitted individuals equipped with an interacting recycling
      mechanism.
    * Quantum_annealing uses "quantum fluctuations" instead of thermal
      fluctuations to get through high but thin barriers in the target
      function.
    * Stochastic_tunneling attempts to overcome the increasing difficulty
      simulated annealing runs have in escaping from local minima as the
      temperature decreases, by 'tunneling' through barriers.
    * Tabu_search normally moves to neighbouring states of lower energy, but
      will take uphill moves when it finds itself stuck in a local minimum; and
      avoids cycles by keeping a "taboo list" of solutions already seen.
    * Dual-phase_evolution is a family of algorithms and processes (to which
      simulated annealing belongs) that mediate between local and global search
      by exploiting phase changes in the search space.
    * Reactive_search_optimization focuses on combining machine learning with
      optimization, by adding an internal feedback loop to self-tune the free
      parameters of an algorithm to the characteristics of the problem, of the
      instance, and of the local situation around the current solution.
    * Stochastic_gradient_descent runs many greedy searches from random initial
      locations.
    * Genetic_algorithms maintain a pool of solutions rather than just one. New
      candidate solutions are generated not only by "mutation" (as in SA), but
      also by "recombination" of two solutions from the pool. Probabilistic
      criteria, similar to those used in SA, are used to select the candidates
      for mutation or combination, and for discarding excess solutions from the
      pool.
    * Graduated_optimization digressively "smooths" the target function while
      optimizing.
    * Ant_colony_optimization (ACO) uses many ants (or agents) to traverse the
      solution space and find locally productive areas.
    * The cross-entropy_method (CE) generates candidates solutions via a
      parameterized probability distribution. The parameters are updated via
      cross-entropy minimization, so as to generate better samples in the next
      iteration.
    * Harmony_search mimics musicians in improvisation process where each
      musician plays a note for finding a best harmony all together.
    * Stochastic_optimization is an umbrella set of methods that includes
      simulated annealing and numerous other approaches.
    * Particle_swarm_optimization is an algorithm modelled on swarm
      intelligence that finds a solution to an optimization problem in a search
      space, or model and predict social behavior in the presence of
      objectives.
    * The runner-root algorithm (RRA) is a meta-heuristic optimization
      algorithm for solving unimodal and multimodal problems inspired by the
      runners and roots of plants in nature.
    * Intelligent_water_drops_algorithm (IWD) which mimics the behavior of
      natural water drops to solve optimization problems
    * Parallel_tempering is a simulation of model copies at different
      temperatures (or Hamiltonians) to overcome the potential barriers.
***** See also[edit] *****
    * Adaptive_simulated_annealing
    * Markov_chain
    * Combinatorial_optimization
    * Dual-phase_evolution
    * Automatic_label_placement
    * Multidisciplinary_optimization
    * Place_and_route
    * Molecular_dynamics
    * Traveling_salesman_problem
    * Graph_cuts_in_computer_vision
    * Particle_swarm_optimization
    * Intelligent_water_drops_algorithm
***** References[edit] *****
   1. ^ a bKhachaturyan, A.; Semenovskaya, S.; Vainshtein, B. (1979).
      "Statistical-Thermodynamic Approach to Determination of Structure
      Amplitude Phases". Sov.Phys. Crystallography. 24 (5): 519â524.
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
   3. ^ a bKhachaturyan, A.; Semenovskaya, S.; Vainshtein, B. (1981). "The
      Thermodynamic Approach to the Structure Analysis of Crystals". Acta
      Crystallographica. 37 (A37): 742â754. Bibcode:1981AcCrA..37..742K. doi:
      10.1107/S0567739481001630.
   4. ^Kirkpatrick, S.; Gelatt Jr, C. D.; Vecchi, M. P. (1983). "Optimization
      by Simulated Annealing". Science. 220 (4598): 671â680. Bibcode:
      1983Sci...220..671K. CiteSeerX 10.1.1.123.7607. doi:10.1126/
      science.220.4598.671. JSTOR 1690046. PMID 17813860.
   5. ^ÄernÃ½, V. (1985). "Thermodynamical approach to the traveling salesman
      problem: An efficient simulation algorithm". Journal of Optimization
      Theory and Applications. 45: 41â51. doi:10.1007/BF00940812.
   6. ^Semenovskaya, S.; Khachaturyan, K.; Khachaturyan, A. (1985).
      "Statistical Mechanics Approach to the Determination of a Crystal". Acta
      Crystallographica. 41 (A41): 268â273. doi:10.1107/S0108767385000563.
   7. ^Metropolis, Nicholas; Rosenbluth, Arianna W.; Rosenbluth, Marshall N.;
      Teller, Augusta H.; Teller, Edward (1953). "Equation of State
      Calculations by Fast Computing Machines". The Journal of Chemical
      Physics. 21 (6): 1087. Bibcode:1953JChPh..21.1087M. doi:10.1063/
      1.1699114.
   8. ^Granville, V.; Krivanek, M.; Rasson, J.-P. (1994). "Simulated annealing:
      A proof of convergence". IEEE Transactions on Pattern Analysis and
      Machine Intelligence. 16 (6): 652â656. doi:10.1109/34.295910.
   9. ^De Vicente, Juan; Lanchares, Juan; Hermida, RomÃ¡n (2003). "Placement by
      thermodynamic simulated annealing". Physics Letters A. 317 (5â6):
      415â423. Bibcode:2003PhLA..317..415D. doi:10.1016/
      j.physleta.2003.08.070.
  10. ^Del Moral, Pierre; Doucet, Arnaud; Jasra, Ajay (2006). "Sequential Monte
      Carlo samplers - P. Del Moral - A. Doucet - A. Jasra - 2006 - Journal of
      the Royal Statistical Society: Series B (Statistical Methodology) - Wiley
      Online Library". Journal of the Royal Statistical Society, Series B. 68
      (3): 411â436. arXiv:cond-mat/0212648. doi:10.1111/j.1467-
      9868.2006.00553.x.
***** Further reading[edit] *****
    * A. Das and B. K. Chakrabarti (Eds.), Quantum_Annealing_and_Related
      Optimization_Methods, Lecture Note in Physics, Vol. 679, Springer,
      Heidelberg (2005)
    * Weinberger, E. (1990). "Correlated and uncorrelated fitness landscapes
      and how to tell the difference". Biological Cybernetics. 63 (5):
      325â336. doi:10.1007/BF00202749.
Press, WH; Teukolsky, SA; Vetterling, WT; Flannery, BP (2007). "Section_10.12.
Simulated_Annealing_Methods". Numerical Recipes: The Art of Scientific
Computing (3rd ed.). New York: Cambridge University Press. ISBN 978-0-521-
88068-8
Strobl, M.A.R.; Barker, D. (2016). "On_simulated_annealing_phase_transitions_in
phylogeny_reconstruction". Molecular Phylogenetics and Evolution. 101: 46â55.
doi:10.1016/j.ympev.2016.05.001. PMC 4912009. PMID 27150349.
V.Vassilev, A.Prahova: "The Use of Simulated Annealing in the Control of
Flexible Manufacturing Systems", International Journal INFORMATION THEORIES &
APPLICATIONS, VOLUME_6/1999
***** External links[edit] *****
    * Simulated_Annealing A Javascript app that allows you to experiment with
      simulated annealing. Source code included.
    * "General_Simulated_Annealing_Algorithm" An open-source MATLAB program for
      general simulated annealing exercises.
    * Self-Guided_Lesson_on_Simulated_Annealing A Wikiversity project.
    * Google_in_superposition_of_using,_not_using_quantum_computer Ars Technica
      discusses the possibility that the D-Wave computer being used by Google
      may, in fact, be an efficient simulated annealing co-processor.
    * v
    * t
    * e
Major_subfields_of_optimization
    * Convex_programming
    * Integer_programming
    * Quadratic_programming
    * Nonlinear_programming
    * Stochastic_programming
    * Robust_optimization
    * Combinatorial_optimization
    * Infinite-dimensional_optimization
    * Metaheuristics
    * Constraint_satisfaction
    * Multiobjective_optimization

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Simulated_annealing&oldid=907842705"
Categories:
    * Metaheuristics
    * Optimization_algorithms_and_methods
    * Monte_Carlo_methods
Hidden categories:
    * Articles_with_short_description
    * Articles_needing_additional_references_from_December_2009
    * All_articles_needing_additional_references
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_June_2011
    * Articles_with_inconsistent_citation_formats
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
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Bahasa_Indonesia
    * Italiano
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * à¹à¸à¸¢
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 25 July 2019, at 16:52 (UTC).
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
