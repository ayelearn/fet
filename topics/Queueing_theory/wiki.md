The following text has been accessed from https://en.wikipedia.org/wiki/Queueing_theory at Fri Aug 9 02:31:10 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Queueing theory ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
Queue_networks are systems in which single queues are connected by a routing
network. In this image, servers are represented by circles, queues by a series
of rectangles and the routing network by arrows. In the study of queue networks
one typically tries to obtain the equilibrium_distribution of the network,
although in many applications the study of the transient_state is fundamental.
Queueing theory is the mathematical study of waiting lines, or queues.[1] A
queueing model is constructed so that queue lengths and waiting time can be
predicted.[1] Queueing theory is generally considered a branch of operations
research because the results are often used when making business decisions
about the resources needed to provide a service.
Queueing theory has its origins in research by Agner_Krarup_Erlang when he
created models to describe the Copenhagen telephone exchange.[1] The ideas have
since seen applications including telecommunication, traffic_engineering,
computing[2] and, particularly in industrial_engineering, in the design of
factories, shops, offices and hospitals, as well as in project management.[3]
[4]
⁰
***** Contents *****
    * 1_Spelling
    * 2_Single_queueing_nodes
    * 3_Overview_of_the_development_of_the_theory
    * 4_Service_disciplines
    * 5_Simple_two-equation_queue
    * 6_Queueing_networks
          o 6.1_Example_analysis_of_an_M/M/1_queue
          o 6.2_Routing_algorithms
    * 7_Mean_field_limits
    * 8_Fluid_limits
    * 9_Heavy_traffic/diffusion_approximations
    * 10_See_also
    * 11_References
    * 12_Further_reading
    * 13_External_links
***** Spelling[edit] *****
The spelling "queueing" over "queuing" is typically encountered in the academic
research field. In fact, one of the flagship journals of the profession is
named Queueing_Systems.
"Queueing" is, incidentally, the only English word having more than four
consecutive vowels.
***** Single queueing nodes[edit] *****
  Simple description and analogy
A queue, or "queueing node" can be thought of as nearly a black_box. Jobs or
"customers" arrive to the queue, possibly wait some time, take some time being
processed, and then depart from the queue (see_Fig._1).
Fig. 1. A black box. Jobs arrive to, and depart from, the queue.
The queueing node is not quite a pure black box, however, since there is some
information we need to specify about the inside of the queuing node. The queue
has one or more "servers" which can each be paired with an arriving job until
it departs, after which that server will be free to be paired with another
arriving job (see_Fig._2).
Fig. 2. A queueing node with 3 servers. Server a is idle, and thus an arrival
is given to it to process. Server b is currently busy and will take some time
before it can complete service of its job. Server c has just completed service
of a job and thus will be next to receive an arriving job.
An analogy often used is that of the cashier at a supermarket. There are other
models, but this is one commonly encountered in the literature. Customers
arrive, are processed by the cashier, and depart. Each cashier processes one
customer at a time, and hence this is a queueing node with only one server. A
setting, where a customer will leave immediately, when in arriving he finds the
cashier busy, is called a queue with no buffer (or no "waiting area", or
similar terms). A setting with a waiting zone for up to n customers is called a
queue with a buffer of size n.
  Birth-death process
The behaviour / state of a single queue (also called a "queueing node") can be
described by a Birth-death_process, which describe the arrivals and departures
from the queue, along with the number of jobs (also called "customers" or
"requests", or any number of other things, depending on the field) currently in
the system. An arrival increases the number of jobs by 1, and a departure (a
job completing its service) decreases k by 1 (see_Fig._3).
Fig. 3. Birth / death process. The values in the circles represent the state of
the birth-death process, k. The system transitions between values of k by
"births" and "deaths" which occur at rates given by various values of Î»i and
Î¼i, respectively. For a queueing system, k is the number of jobs in the system
(either being serviced or waiting if the queue has a buffer of waiting jobs).
Further, for a queue, the arrival rates and departure rates are generally
considered not to vary with the number of jobs in the queue so that we consider
a single average rate of arrivals/departures per unit time to the queue. Hence,
for a queue, this diagram has arrival rates of Î» = Î»1, Î»2, â¦, Î»k and
departure rates of Î¼ = Î¼1, Î¼2, â¦, Î¼k (see_Fig._4).
Fig. 4. A queue with 1 server, arrival rate Î» and departure rate Î¼.
  Kendall's notation
Single queueing nodes are usually described using Kendall's_notation in the
form A/S/c where A describes the distribution of durations between each arrival
to the queue, S the distribution of service times for jobs and c the number of
servers at the node.[5][6] For an example of the notation, the M/M/1_queue is a
simple model where a single server serves jobs that arrive according to a
Poisson_process (inter-arrival durations are exponentially_distributed) and
have exponentially distributed service times. In an M/G/1_queue, the G stands
for general and indicates an arbitrary probability_distribution for service
times.
***** Overview of the development of the theory[edit] *****
In 1909, Agner_Krarup_Erlang, a Danish engineer who worked for the Copenhagen
Telephone Exchange, published the first paper on what would now be called
queueing theory.[7][8][9] He modeled the number of telephone calls arriving at
an exchange by a Poisson_process and solved the M/D/1_queue in 1917 and M/D/
k_queueing model in 1920.[10] In Kendall's notation:
    * M stands for Markov or memoryless and means arrivals occur according to a
      Poisson process;
    * D stands for deterministic and means jobs arriving at the queue which
      require a fixed amount of service;
    * k describes the number of servers at the queueing node (k = 1, 2, â¦).
If there are more jobs at the node than there are servers, then jobs will queue
and wait for service
The M/G/1 queue was solved by Felix_Pollaczek in 1930,[11] a solution later
recast in probabilistic terms by Aleksandr_Khinchin and now known as the
PollaczekâKhinchine_formula.[10][12]
After the 1940s queueing theory became an area of research interest to
mathematicians.[12] In 1953 David_George_Kendall solved the GI/M/k queue[13]
and introduced the modern notation for queues, now known as Kendall's_notation.
In 1957 Pollaczek studied the GI/G/1 using an integral_equation.[14] John
Kingman gave a formula for the mean_waiting_time in a G/G/1_queue: Kingman's
formula.[15]
Leonard_Kleinrock worked on the application of queueing theory to message
switching and packet_switching. His initial contribution to this field was his
doctoral thesis at the Massachusetts_Institute_of_Technology in 1962, published
in book form in 1964 in the field of digital message switching. His theoretical
work after 1967 underpinned the use of packing switching in the ARPANET, a
forerunner to the Internet.
The matrix_geometric_method and matrix_analytic_methods have allowed queues
with phase-type_distributed inter-arrival and service time distributions to be
considered.[16]
Problems such as performance metrics for the M/G/k_queue remain an open
problem.[10][12]
***** Service disciplines[edit] *****
First in first out (FIFO) queue example.
Various scheduling policies can be used at queuing nodes:
  First_in_first_out
      Also called first-come, first-served (FCFS),[17] this principle states
      that customers are served one at a time and that the customer that has
      been waiting the longest is served first.[18]
  Last_in_first_out
      This principle also serves customers one at a time, but the customer with
      the shortest waiting_time will be served first.[18] Also known as a
      stack.
  Processor_sharing
      Service capacity is shared equally between customers.[18]
  Priority
      Customers with high priority are served first.[18] Priority queues can be
      of two types, non-preemptive (where a job in service cannot be
      interrupted) and preemptive (where a job in service can be interrupted by
      a higher-priority job). No work is lost in either model.[19]
  Shortest_job_first
      The next job to be served is the one with the smallest size
  Preemptive shortest job first
      The next job to be served is the one with the original smallest size[20]
  Shortest_remaining_processing_time
      The next job to serve is the one with the smallest remaining processing
      requirement.[21]
  Service facility
    * Single server: customers line up and there is only one server
    * Several parallel serversâSingle queue: customers line up and there are
      several servers
    * Several serversâSeveral queues: there are many counters and customers
      can decide going where to queue
  Customer's behavior of waiting
    * Balking: customers deciding not to join the queue if it is too long
    * Jockeying: customers switch between queues if they think they will get
      served faster by doing so
    * Reneging: customers leave the queue if they have waited too long for
      service
Arriving customers not served (either due to the queue having no buffer, or due
to balking or reneging by the customer) are also known as dropouts and the
average rate of dropouts is a significant parameter describing a queue.
***** Simple two-equation queue[edit] *****
A common basic queuing system is attributed to Erlang, and is a modification of
Little's_Law. Given an arrival rate Î», a dropout rate Ï, and a departure rate
Î¼, length of the queue L is defined as:
         L =    &#x03BB; &#x2212; &#x03C3;  &#x03BC;   .   {\displaystyle L=
      {\frac {\lambda -\sigma }{\mu }}.}  [{\displaystyle L={\frac {\lambda -
      \sigma }{\mu }}.}]
Assuming an exponential distribution for the rates, the waiting time W can be
defined as the proportion of arrivals that are served. This is equal to the
exponential survival rate of those who do not drop out over the waiting period,
giving:
           &#x03BC; &#x03BB;   =  e  &#x2212; W  &#x03BC;      {\displaystyle
      {\frac {\mu }{\lambda }}=e^{-W{\mu }}}  [{\displaystyle {\frac {\mu }
      {\lambda }}=e^{-W{\mu }}}]
The second equation is commonly rewritten as:
         W =   1 &#x03BC;    l n    &#x03BB; &#x03BC;     {\displaystyle W=
      {\frac {1}{\mu }}\mathrm {ln} {\frac {\lambda }{\mu }}}  [{\displaystyle
      W={\frac {1}{\mu }}\mathrm {ln} {\frac {\lambda }{\mu }}}]
The two-stage one-box model is common in epidemiology.[22]
***** Queueing networks[edit] *****
Networks of queues are systems in which a number of queues are connected by
what's known as customer routing. When a customer is serviced at one node it
can join another node and queue for service, or leave the network.
For networks of m nodes, the state of the system can be described by an
mâdimensional vector (x1, x2, â¦, xm) where xi represents the number of
customers at each node.
The simplest non-trivial network of queues is called tandem_queues.[23] The
first significant results in this area were Jackson_networks,[24][25] for which
an efficient product-form_stationary_distribution exists and the mean_value
analysis[26] which allows average metrics such as throughput and sojourn times
to be computed.[27] If the total number of customers in the network remains
constant the network is called a closed network and has also been shown to have
a productâform stationary distribution in the GordonâNewell_theorem.[28]
This result was extended to the BCMP_network[29] where a network with very
general service time, regimes and customer routing is shown to also exhibit a
product-form stationary distribution. The normalizing_constant can be
calculated with the Buzen's_algorithm, proposed in 1973.[30]
Networks of customers have also been investigated, Kelly_networks where
customers of different classes experience different priority levels at
different service nodes.[31] Another type of network are G-networks first
proposed by Erol_Gelenbe in 1993:[32] these networks do not assume exponential
time distributions like the classic Jackson Network.
**** Example analysis of an M/M/1 queue[edit] ****
Consider a queue with 1 server and the following variables:
    * Î»: the average arrival rate (customers arriving to the system per unit
      time, e.g. per 30 seconds);
    * Î¼: the average departure rate (customers leaving the systemâcompleting
      serviceâper the same unit time, e.g. per 30 seconds);
    * n: the number of customers in the system at the given time;
    * Pn: the probability of there being n customers in the system.
Further, let En represent the number of times the system enters state n, and Ln
represent the number of times the system leaves state n. For all n, we have |En
â Ln| â {0, 1}, that is, the number of times the system leaves a state
differs by at most 1 from the number of times it enters that state, since it
will either return into that state at some time in the future (En = Ln) or not
(|En â Ln| = 1).
When the system arrives at a steady state, the arrival rate should be equal to
the departure rate.
  Balance_equation
      situation 0:      &#x03BC;  1    P  1   =  &#x03BB;  0    P  0
      {\displaystyle \mu _{1}P_{1}=\lambda _{0}P_{0}}  [{\displaystyle \mu _
      {1}P_{1}=\lambda _{0}P_{0}}]
      situation 1:      &#x03BB;  0    P  0   +  &#x03BC;  2    P  2   =
      (  &#x03BB;  1   +  &#x03BC;  1   )  P  1     {\displaystyle \lambda _
      {0}P_{0}+\mu _{2}P_{2}=(\lambda _{1}+\mu _{1})P_{1}}  [{\displaystyle
      \lambda _{0}P_{0}+\mu _{2}P_{2}=(\lambda _{1}+\mu _{1})P_{1}}]
      situation n:      &#x03BB;  n &#x2212; 1    P  n &#x2212; 1   +  &#x03BC;
      n + 1    P  n + 1   = (  &#x03BB;  n   +  &#x03BC;  n   )  P  n
      {\displaystyle \lambda _{n-1}P_{n-1}+\mu _{n+1}P_{n+1}=(\lambda _{n}+\mu
      _{n})P_{n}}  [{\displaystyle \lambda _{n-1}P_{n-1}+\mu _{n+1}P_{n+1}=
      (\lambda _{n}+\mu _{n})P_{n}}]
      By balance equation,      P  1   =    &#x03BB;  0    &#x03BC;  1      P
      0       P  2   =    &#x03BB;  1    &#x03BC;  2      P  1   +   1
      &#x03BC;  2     (  &#x03BC;  1    P  1   &#x2212;  &#x03BB;  0    P  0
      ) =    &#x03BB;  1    &#x03BC;  2      P  1   =     &#x03BB;  1
      &#x03BB;  0      &#x03BC;  2    &#x03BC;  1       P  0     {\displaystyle
      P_{1}={\frac {\lambda _{0}}{\mu _{1}}}P_{0}\;\;\;P_{2}={\frac {\lambda _
      {1}}{\mu _{2}}}P_{1}+{\frac {1}{\mu _{2}}}(\mu _{1}P_{1}-\lambda _{0}P_
      {0})={\frac {\lambda _{1}}{\mu _{2}}}P_{1}={\frac {\lambda _{1}\lambda _
      {0}}{\mu _{2}\mu _{1}}}P_{0}}  [{\displaystyle P_{1}={\frac {\lambda _
      {0}}{\mu _{1}}}P_{0}\;\;\;P_{2}={\frac {\lambda _{1}}{\mu _{2}}}P_{1}+
      {\frac {1}{\mu _{2}}}(\mu _{1}P_{1}-\lambda _{0}P_{0})={\frac {\lambda _
      {1}}{\mu _{2}}}P_{1}={\frac {\lambda _{1}\lambda _{0}}{\mu _{2}\mu _
      {1}}}P_{0}}]
      By mathematical induction,      P  n   =     &#x03BB;  n &#x2212; 1
      &#x03BB;  n &#x2212; 2   &#x22EF;  &#x03BB;  0      &#x03BC;  n
      &#x03BC;  n &#x2212; 1   &#x22EF;  &#x03BC;  1       P  0   =  P  0
      &#x220F;  i = 0   n &#x2212; 1      &#x03BB;  i    &#x03BC;  i + 1
      {\displaystyle P_{n}={\frac {\lambda _{n-1}\lambda _{n-2}\cdots \lambda _
      {0}}{\mu _{n}\mu _{n-1}\cdots \mu _{1}}}P_{0}=P_{0}\prod _{i=0}^{n-1}
      {\frac {\lambda _{i}}{\mu _{i+1}}}}  [{\displaystyle P_{n}={\frac
      {\lambda _{n-1}\lambda _{n-2}\cdots \lambda _{0}}{\mu _{n}\mu _{n-
      1}\cdots \mu _{1}}}P_{0}=P_{0}\prod _{i=0}^{n-1}{\frac {\lambda _{i}}{\mu
      _{i+1}}}}]
      Because      &#x2211;  n = 0   &#x221E;    P  n   =  P  0   +  P  0
      &#x2211;  n = 1   &#x221E;    &#x220F;  i = 0   n &#x2212; 1
      &#x03BB;  i    &#x03BC;  i + 1     = 1   {\displaystyle \sum _{n=0}^
      {\infty }P_{n}=P_{0}+P_{0}\sum _{n=1}^{\infty }\prod _{i=0}^{n-1}{\frac
      {\lambda _{i}}{\mu _{i+1}}}=1}  [{\displaystyle \sum _{n=0}^{\infty }P_
      {n}=P_{0}+P_{0}\sum _{n=1}^{\infty }\prod _{i=0}^{n-1}{\frac {\lambda _
      {i}}{\mu _{i+1}}}=1}]
      We get      P  0   =   1  1 +  &#x2211;  n = 1   &#x221E;    &#x220F;  i
      = 0   n &#x2212; 1      &#x03BB;  i    &#x03BC;  i + 1
      {\displaystyle P_{0}={\frac {1}{1+\sum _{n=1}^{\infty }\prod _{i=0}^{n-1}
      {\frac {\lambda _{i}}{\mu _{i+1}}}}}}  [{\displaystyle P_{0}={\frac {1}
      {1+\sum _{n=1}^{\infty }\prod _{i=0}^{n-1}{\frac {\lambda _{i}}{\mu _
      {i+1}}}}}}]
**** Routing algorithms[edit] ****
In discrete time networks where there is a constraint on which service nodes
can be active at any time, the max-weight scheduling algorithm chooses a
service policy to give optimal throughput in the case that each job visits only
a single person [17] service node. In the more general case where jobs can
visit more than one node, backpressure_routing gives optimal throughput. A
network_scheduler must choose a queuing_algorithm, which affects the
characteristics of the larger network[citation_needed]. See also Stochastic
scheduling for more about scheduling of queueing systems.
***** Mean field limits[edit] *****
Mean_field_models consider the limiting behaviour of the empirical_measure
(proportion of queues in different states) as the number of queues (m above)
goes to infinity. The impact of other queues on any given queue in the network
is approximated by a differential equation. The deterministic model converges
to the same stationary distribution as the original model.[33]
***** Fluid limits[edit] *****
Main article: fluid_limit
Fluid models are continuous deterministic analogs of queueing networks obtained
by taking the limit when the process is scaled in time and space, allowing
heterogeneous objects. This scaled trajectory converges to a deterministic
equation which allows the stability of the system to be proven. It is known
that a queueing network can be stable, but have an unstable fluid limit.[34]
***** Heavy traffic/diffusion approximations[edit] *****
Main article: heavy_traffic_approximation
In a system with high occupancy rates (utilisation near 1) a heavy traffic
approximation can be used to approximate the queueing length process by a
reflected_Brownian_motion,[35] OrnsteinâUhlenbeck_process or more general
diffusion_process.[36] The number of dimensions of the RBM is equal to the
number of queueing nodes and the diffusion is restricted to the non-negative
orthant.
***** See also[edit] *****
    * Ehrenfest_model
    * Erlang_unit
    * Industrial_engineering
    * Leonard_Kleinrock
    * Network_simulation
    * Poisson_distribution
    * Project_Production_Management
    * Queue_area
    * Queueing_delay
    * Queue_management_system
    * Queuing_Rule_of_Thumb
    * Queueing_Systems â a journal of queueing theory
    * Random_early_detection
    * Renewal_theory
    * Throughput
    * Scheduling_(computing)
    * Traffic_jam
    * Traffic_generation_model
    * Flow_network
    * Stochastic_scheduling
***** References[edit] *****
   1. ^ a b cSundarapandian, V. (2009). "7. Queueing Theory". Probability,
      Statistics and Queueing Theory. PHI Learning. ISBN 978-8120338449.
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
   3. ^Lawrence W. Dowdy, Virgilio A.F. Almeida, Daniel A. Menasce.
      "Performance_by_Design:_Computer_Capacity_Planning_by_Example".
   4. ^Schlechter, Kira (March 2, 2009). "Hershey_Medical_Center_to_open
      redesigned_emergency_room". The Patriot-News.
   5. ^Mayhew, Les; Smith, David (December 2006). Using_queuing_theory_to
      analyse_completion_times_in_accident_and_emergency_departments_in_the
      light_of_the_Government_4-hour_target. Cass_Business_School. ISBN 978-1-
      905752-06-5. Retrieved 2008-05-20.
   6. [permanent_dead_link]
   7. ^ Tijms, H.C, Algorithmic Analysis of Queues", Chapter 9 in A First
      Course in Stochastic Models, Wiley, Chichester, 2003
   8. ^Kendall,_D._G. (1953). "Stochastic Processes Occurring in the Theory of
      Queues and their Analysis by the Method of the Imbedded Markov Chain".
      The Annals of Mathematical Statistics. 24 (3): 338â354. doi:10.1214/
      aoms/1177728975. JSTOR 2236285.
   9. ^"Agner_Krarup_Erlang_(1878-1929)_|_plus.maths.org". Pass.maths.org.uk.
      1997-04-30. Retrieved 2013-04-22.
  10. ^Asmussen, S. R.; Boxma,_O._J. (2009). "Editorial introduction". Queueing
      Systems. 63 (1â4): 1â2. doi:10.1007/s11134-009-9151-8.
  11. ^Erlang,_Agner_Krarup (1909). "The_theory_of_probabilities_and_telephone
      conversations" (PDF). NYT Tidsskrift for Matematik B. 20: 33â39.
      Archived from the_original (PDF) on 2011-10-01.
  12. ^ a b cKingman,_J._F._C. (2009). "The first Erlang centuryâand the
      next". Queueing_Systems. 63 (1â4): 3â4. doi:10.1007/s11134-009-9147-
      4.
  13. ^ Pollaczek, F., Ueber eine Aufgabe der Wahrscheinlichkeitstheorie, Math.
      Z. 1930
  14. ^ a b cWhittle,_P. (2002). "Applied Probability in Great Britain".
      Operations_Research. 50 (1): 227â239. doi:10.1287/opre.50.1.227.17792.
      JSTOR 3088474.
  15. ^ Kendall, D.G.:Stochastic processes occurring in the theory of queues
      and their analysis by the method of the imbedded Markov chain, Ann. Math.
      Stat. 1953
  16. ^ Pollaczek, F., ProblÃ¨mes Stochastiques posÃ©s par le phÃ©nomÃ¨ne de
      formation d'une queue
  17. ^Kingman,_J._F._C.; Atiyah (October 1961). "The single server queue in
      heavy traffic". Mathematical_Proceedings_of_the_Cambridge_Philosophical
      Society. 57 (4): 902. doi:10.1017/S0305004100036094. JSTOR 2984229.
  18. ^Ramaswami, V. (1988). "A stable recursion for the steady state vector in
      markov chains of m/g/1 type". Communications in Statistics. Stochastic
      Models. 4: 183â188. doi:10.1080/15326348808807077.
  19. ^ a bManuel, Laguna (2011). Business_Process_Modeling,_Simulation_and
      Design. Pearson Education India. p. 178. ISBN 9788131761359. Retrieved 6
      October 2017.
  20. ^ a b c d Penttinen A., Chapter 8 – Queueing Systems, Lecture Notes: S-
      38.145 - Introduction to Teletraffic Theory.
  21. ^Harchol-Balter,_M. (2012). "Scheduling: Non-Preemptive, Size-Based
      Policies". Performance Modeling and Design of Computer Systems.
      pp. 499â507. doi:10.1017/CBO9781139226424.039. ISBN 9781139226424.
  22. ^Harchol-Balter,_M. (2012). "Scheduling: Preemptive, Size-Based
      Policies". Performance Modeling and Design of Computer Systems.
      pp. 508â517. doi:10.1017/CBO9781139226424.040. ISBN 9781139226424.
  23. ^Harchol-Balter,_M. (2012). "Scheduling: SRPT and Fairness". Performance
      Modeling and Design of Computer Systems. pp. 518â530. doi:10.1017/
      CBO9781139226424.041. ISBN 9781139226424.
  24. ^HernÃ¡ndez-Suarez, Carlos (2010). "An application of queuing theory to
      SIS and SEIS epidemic models". Math. Biosci. 7 (4): 809â823. doi:
      10.3934/mbe.2010.7.809. PMID 21077709.
  25. ^ http://www.stats.ox.ac.uk/~winkel/bs3a07l13-14.pdf#page=4
  26. ^Jackson,_J._R. (1957). "Networks of Waiting Lines". Operations Research.
      5 (4): 518â521. doi:10.1287/opre.5.4.518. JSTOR 167249.
  27. ^Jackson, James R. (Oct 1963). "Jobshop-like Queueing Systems".
      Management_Science. 10 (1): 131â142. doi:10.1287/mnsc.1040.0268.
      JSTOR 2627213.
  28. ^Reiser, M.; Lavenberg, S. S. (1980). "Mean-Value Analysis of Closed
      Multichain Queuing Networks". Journal_of_the_ACM. 27 (2): 313. doi:
      10.1145/322186.322195.
  29. ^Van Dijk, N. M. (1993). "On the arrival theorem for communication
      networks". Computer Networks and ISDN Systems. 25 (10): 1135â2013. doi:
      10.1016/0169-7552(93)90073-D.
  30. ^Gordon, W. J.; Newell,_G._F. (1967). "Closed Queuing Systems with
      Exponential Servers". Operations_Research. 15 (2): 254. doi:10.1287/
      opre.15.2.254. JSTOR 168557.
  31. ^Baskett, F.; Chandy,_K._Mani; Muntz, R.R.; Palacios, F.G. (1975). "Open,
      closed and mixed networks of queues with different classes of customers".
      Journal of the ACM. 22 (2): 248â260. doi:10.1145/321879.321887.
  32. ^Buzen,_J._P. (1973). "Computational_algorithms_for_closed_queueing
      networks_with_exponential_servers" (PDF). Communications of the ACM. 16
      (9): 527â531. doi:10.1145/362342.362345.
  33. ^Kelly,_F._P. (1975). "Networks of Queues with Customers of Different
      Types". Journal of Applied Probability. 12 (3): 542â554. doi:10.2307/
      3212869. JSTOR 3212869.
  34. ^Gelenbe,_Erol (Sep 1993). "G-Networks with Triggered Customer Movement".
      Journal of Applied Probability. 30 (3): 742â748. doi:10.2307/3214781.
      JSTOR 3214781.
  35. ^Bobbio, A.; Gribaudo, M.; Telek, M. S. (2008). "Analysis of Large Scale
      Interacting Systems by Mean Field Method". 2008 Fifth International
      Conference on Quantitative Evaluation of Systems. p. 215. doi:10.1109/
      QEST.2008.47. ISBN 978-0-7695-3360-5.
  36. ^Bramson, M. (1999). "A stable queueing network with unstable fluid
      model". The Annals of Applied Probability. 9 (3): 818â853. doi:10.1214/
      aoap/1029962815. JSTOR 2667284.
  37. ^Chen, H.; Whitt, W. (1993). "Diffusion approximations for open queueing
      networks with service interruptions". Queueing_Systems. 13 (4): 335. doi:
      10.1007/BF01149260.
  38. ^Yamada, K. (1995). "Diffusion Approximation for Open State-Dependent
      Queueing Networks in the Heavy Traffic Situation". The Annals of Applied
      Probability. 5 (4): 958â982. doi:10.1214/aoap/1177004602.
      JSTOR 2245101.
***** Further reading[edit] *****
    * Gross, Donald; Carl M. Harris (1998). Fundamentals of Queueing Theory.
      Wiley. ISBN 978-0-471-32812-4.
 Online
Deitel, Harvey M. (1984) [1982]. An_introduction_to_operating_systems
(revisited first ed.). Addison-Wesley. p. 673. ISBN 978-0-201-14502-1.
 chap.15, pp. 380â412
Kleinrock,_Leonard (2 January 1975). Queueing Systems: Volume I â Theory. New
York: Wiley Interscience. p. 417. ISBN 978-0471491101.
Kleinrock,_Leonard (22 April 1976). Queueing Systems: Volume II â Computer
Applications. New York: Wiley Interscience. p. 576. ISBN 978-0471491118.
Lazowska, Edward D.; John Zahorjan; G. Scott Graham; Kenneth C. Sevcik (1984).
Quantitative_System_Performance:_Computer_System_Analysis_Using_Queueing
Network_Models. Prentice-Hall, Inc. ISBN 978-0-13-746975-8.
Zukerman, Moshe. Introduction_to_Queueing_Theory_and_Stochastic_Teletraffic
Models (PDF).
***** External links[edit] *****
 This article's use of external_links may not follow Wikipedia's policies or
 guidelines. Please improve_this_article by removing excessive or inappropriate
 external links, and converting useful links where appropriate into footnote
 references. (May 2017)(Learn_how_and_when_to_remove_this_template_message)
    * Queueing_theory_calculator
    * Teknomo's_Queueing_theory_tutorial_and_calculators
    * Office_Fire_Emergency_Evacuation_Simulation on YouTube
    * Virtamo's_Queueing_Theory_Course
    * Myron_Hlynka's_Queueing_Theory_Page
    * Queueing_Theory_Basics
    * A_free_online_tool_to_solve_some_classical_queueing_systems
    * JMT:_an_open_source_graphical_environment_for_queueing_theory
    * LINE:_a_general-purpose_engine_to_solve_queueing_models
    * What_You_Hate_Most_About_Waiting_in_Line:_(Itâs_not_the_length_of_the
      wait.), by Seth Stevenson, Slate, 2012 â popular introduction
    * v
    * t
    * e
Queueing theory
                          * D/M/1_queue
                          * M/D/1_queue
                          * M/D/c_queue
                          * M/M/1_queue
                                o Burke's_theorem
                          * M/M/c_queue
                          * M/M/â_queue
                          * M/G/1_queue
Single queueing nodes           o PollaczekâKhinchine_formula
                                o Matrix_analytic_method
                          * M/G/k_queue
                          * G/M/1_queue
                          * G/G/1_queue
                                o Kingman's_formula
                                o Lindley_equation
                          * Forkâjoin_queue
                          * Bulk_queue
                          * Poisson_process
Arrival processes         * Markovian_arrival_process
                          * Rational_arrival_process
                          * Jackson_network
                                o Traffic_equations
                          * GordonâNewell_theorem
Queueing networks               o Mean_value_analysis
                                o Buzen's_algorithm
                          * Kelly_network
                          * G-network
                          * BCMP_network
                          * FIFO
                          * LIFO
Service policies          * Processor_sharing
                          * Round-robin
                          * Shortest_job_first
                          * Shortest_remaining_time
                          * Continuous-time_Markov_chain
                          * Kendall's_notation
                          * Little's_law
                          * Product-form_solution
Key concepts                    o Balance_equation
                                o Quasireversibility
                                o Flow-equivalent_server_method
                          * Arrival_theorem
                          * Decomposition_method
                          * BeneÅ¡_method
                          * Fluid_limit
Limit theorems            * Mean_field_theory
                          * Heavy_traffic_approximation
                                o Reflected_Brownian_motion
                          * Fluid_queue
                          * Layered_queueing_network
Extensions                * Polling_system
                          * Adversarial_queueing_network
                          * Loss_network
                          * Retrial_queue
                          * Data_buffer
                          * Erlang_(unit)
                          * Erlang_distribution
                          * Flow_control_(data)
                          * Message_queue
Information_systems       * Network_congestion
                          * Network_scheduler
                          * Pipeline_(software)
                          * Quality_of_service
                          * Scheduling_(computing)
                          * Teletraffic_engineering
[Category] Category
                                              * BNF: cb12647707b (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4255044-0
                                              * LCCN: sh85109832
                                              * NDL: 00567524

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Queueing_theory&oldid=909518895"
Categories:
    * Stochastic_processes
    * Production_planning
    * Customer_experience
    * Operations_research
    * Formal_sciences
    * Queueing_theory
    * Rationing
    * Network_performance
    * Markov_models
    * Markov_processes
Hidden categories:
    * All_articles_with_dead_external_links
    * Articles_with_dead_external_links_from_April_2018
    * Articles_with_permanently_dead_external_links
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_August_2017
    * Wikipedia_external_links_cleanup_from_May_2017
    * Wikipedia_spam_cleanup_from_May_2017
    * Wikipedia_articles_with_BNF_identifiers
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
    * AzÉrbaycanca
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 5 August 2019, at 23:17 (UTC).
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
