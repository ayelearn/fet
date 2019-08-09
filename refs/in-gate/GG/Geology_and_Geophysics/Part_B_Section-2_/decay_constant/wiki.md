The following text has been accessed from https://en.wikipedia.org/wiki/Exponential_decay at Thu Aug 8 23:20:50 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Exponential decay ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
A quantity undergoing exponential decay. Larger decay constants make the
quantity vanish much more rapidly. This plot shows decay for decay constant
(Î») of 25, 5, 1, 1/5, and 1/25 for x from 0 to 5.
A quantity is subject to exponential decay if it decreases at a rate
proportional to its current value. Symbolically, this process can be expressed
by the following differential_equation, where N is the quantity and Î» (lambda)
is a positive rate called the exponential decay constant:
            d N   d t    = &#x2212; &#x03BB; N .   {\displaystyle {\frac {dN}
      {dt}}=-\lambda N.}  [{\frac {dN}{dt}}=-\lambda N.]
The solution to this equation (see derivation below) is:
         N ( t ) =  N  0    e  &#x2212; &#x03BB; t   ,   {\displaystyle N(t)=N_
      {0}e^{-\lambda t},}  [{\displaystyle N(t)=N_{0}e^{-\lambda t},}]
where N(t) is the quantity at time t, and N0 = N(0) is the initial quantity,
i.e. the quantity at time t = 0.
⁰
***** Contents *****
    * 1_Measuring_rates_of_decay
          o 1.1_Mean_lifetime
          o 1.2_Half-life
    * 2_Solution_of_the_differential_equation
          o 2.1_Derivation_of_the_mean_lifetime
          o 2.2_Decay_by_two_or_more_processes
    * 3_Applications_and_examples
          o 3.1_Natural_sciences
          o 3.2_Social_sciences
          o 3.3_Computer_science
    * 4_See_also
    * 5_References
    * 6_External_links
***** Measuring rates of decay[edit] *****
**** Mean lifetime[edit] ****
If the decaying quantity, N(t), is the number of discrete elements in a certain
set, it is possible to compute the average length of time that an element
remains in the set. This is called the mean lifetime (or simply the lifetime),
where the exponential time_constant,     &#x03C4;   {\displaystyle \tau }
[\tau ], relates to the decay rate, λ, in the following way:
         &#x03C4; =   1 &#x03BB;   .   {\displaystyle \tau ={\frac {1}{\lambda
      }}.}  [\tau ={\frac {1}{\lambda }}.]
The mean lifetime can be looked at as a "scaling time", because the exponential
decay equation can be written in terms of the mean lifetime,     &#x03C4;
{\displaystyle \tau }  [\tau ], instead of the decay constant, λ:
         N ( t ) =  N  0    e  &#x2212; t  /  &#x03C4;   ,   {\displaystyle N
      (t)=N_{0}e^{-t/\tau },}  [{\displaystyle N(t)=N_{0}e^{-t/\tau },}]
and that     &#x03C4;   {\displaystyle \tau }  [\tau ] is the time at which the
population of the assembly is reduced to 1/e_â_0.367879441 times its initial
value.
For example, if the initial population of the assembly, N(0), is 1000, then the
population at time     &#x03C4;   {\displaystyle \tau }  [\tau ],     N
( &#x03C4; )   {\displaystyle N(\tau )}  [{\displaystyle N(\tau )}], is 368.
A very similar equation will be seen below, which arises when the base of the
exponential is chosen to be 2, rather than e. In that case the scaling time is
the "half-life".
**** Half-life[edit] ****
Main article: Half-life
A more intuitive characteristic of exponential decay for many people is the
time required for the decaying quantity to fall to one half of its initial
value. This time is called the half-life, and often denoted by the symbol t1/2.
The half-life can be written in terms of the decay constant, or the mean
lifetime, as:
          t  1  /  2   =    ln &#x2061; ( 2 )  &#x03BB;   = &#x03C4; ln
      &#x2061; ( 2 ) .   {\displaystyle t_{1/2}={\frac {\ln(2)}{\lambda }}=\tau
      \ln(2).}  [t_{1/2}={\frac {\ln(2)}{\lambda }}=\tau \ln(2).]
When this expression is inserted for     &#x03C4;   {\displaystyle \tau }
[\tau ] in the exponential equation above, and ln 2 is absorbed into the base,
this equation becomes:
         N ( t ) =  N  0    2  &#x2212; t  /   t  1  /  2     .
      {\displaystyle N(t)=N_{0}2^{-t/t_{1/2}}.\,}  [N(t)=N_{0}2^{-t/t_{1/
      2}}.\,]
Thus, the amount of material left is 2â1 = 1/2 raised to the (whole or
fractional) number of half-lives that have passed. Thus, after 3 half-lives
there will be 1/23 = 1/8 of the original material left.
Therefore, the mean lifetime     &#x03C4;   {\displaystyle \tau }  [\tau ] is
equal to the half-life divided by the natural log of 2, or:
         &#x03C4; =    t  1  /  2    ln &#x2061; ( 2 )    &#x2248; 1.44
      &#x22C5;  t  1  /  2   .   {\displaystyle \tau ={\frac {t_{1/2}}{\ln
      (2)}}\approx 1.44\cdot t_{1/2}.}  [{\displaystyle \tau ={\frac {t_{1/2}}
      {\ln(2)}}\approx 1.44\cdot t_{1/2}.}]
E.g. polonium-210 has a half-life of 138 days, and a mean lifetime of 200 days.
***** Solution of the differential equation[edit] *****
The equation that describes exponential decay is
            d N   d t    = &#x2212; &#x03BB; N   {\displaystyle {\frac {dN}
      {dt}}=-\lambda N}  [{\frac {dN}{dt}}=-\lambda N]
or, by rearranging (applying the technique called separation_of_variables),
            d N  N   = &#x2212; &#x03BB; d t .   {\displaystyle {\frac {dN}
      {N}}=-\lambda dt.}  [{\frac {dN}{N}}=-\lambda dt.]
Integrating, we have
         ln &#x2061; N = &#x2212; &#x03BB; t + C    {\displaystyle \ln N=-
      \lambda t+C\,}  [\ln N=-\lambda t+C\,]
where C is the constant_of_integration, and hence
         N ( t ) =  e  C    e  &#x2212; &#x03BB; t   =  N  0    e  &#x2212;
      &#x03BB; t      {\displaystyle N(t)=e^{C}e^{-\lambda t}=N_{0}e^{-\lambda
      t}\,}  [N(t)=e^{C}e^{-\lambda t}=N_{0}e^{-\lambda t}\,]
where the final substitution, N0 = eC, is obtained by evaluating the equation
at t = 0, as N0 is defined as being the quantity at t = 0.
This is the form of the equation that is most commonly used to describe
exponential decay. Any one of decay constant, mean lifetime, or half-life is
sufficient to characterise the decay. The notation Î» for the decay constant is
a remnant of the usual notation for an eigenvalue. In this case, Î» is the
eigenvalue of the negative of the differential_operator with N(t) as the
corresponding eigenfunction. The units of the decay constant are sâ1[citation
needed].
**** Derivation of the mean lifetime[edit] ****
Given an assembly of elements, the number of which decreases ultimately to
zero, the mean lifetime,     &#x03C4;   {\displaystyle \tau }  [\tau ], (also
called simply the lifetime) is the expected_value of the amount of time before
an object is removed from the assembly. Specifically, if the individual
lifetime of an element of the assembly is the time elapsed between some
reference time and the removal of that element from the assembly, the mean
lifetime is the arithmetic_mean of the individual lifetimes.
Starting from the population formula
         N =  N  0    e  &#x2212; &#x03BB; t   ,    {\displaystyle N=N_{0}e^{-
      \lambda t},\,}  [N=N_{0}e^{-\lambda t},\,]
first let c be the normalizing factor to convert to a probability_density
function:
         1 =  &#x222B;  0   &#x221E;   c &#x22C5;  N  0    e  &#x2212; &#x03BB;
      t    d t = c &#x22C5;    N  0   &#x03BB;     {\displaystyle 1=\int _{0}^
      {\infty }c\cdot N_{0}e^{-\lambda t}\,dt=c\cdot {\frac {N_{0}}{\lambda }}}
      [1=\int _{0}^{\infty }c\cdot N_{0}e^{-\lambda t}\,dt=c\cdot {\frac {N_
      {0}}{\lambda }}]
or, on rearranging,
         c =   &#x03BB;  N  0     .   {\displaystyle c={\frac {\lambda }{N_
      {0}}}.}  [c={\frac {\lambda }{N_{0}}}.]
Exponential decay is a scalar_multiple of the exponential_distribution (i.e.
the individual lifetime of each object is exponentially distributed), which has
a well-known_expected_value. We can compute it here using integration_by_parts.
         &#x03C4; = &#x27E8; t &#x27E9; =  &#x222B;  0   &#x221E;   t &#x22C5;
      c &#x22C5;  N  0    e  &#x2212; &#x03BB; t    d t =  &#x222B;  0
      &#x221E;   &#x03BB; t  e  &#x2212; &#x03BB; t    d t =   1 &#x03BB;   .
      {\displaystyle \tau =\langle t\rangle =\int _{0}^{\infty }t\cdot c\cdot
      N_{0}e^{-\lambda t}\,dt=\int _{0}^{\infty }\lambda te^{-\lambda t}\,dt=
      {\frac {1}{\lambda }}.}  [\tau =\langle t\rangle =\int _{0}^{\infty
      }t\cdot c\cdot N_{0}e^{-\lambda t}\,dt=\int _{0}^{\infty }\lambda te^{-
      \lambda t}\,dt={\frac {1}{\lambda }}.]
**** Decay by two or more processes[edit] ****
See also: Branching_fraction
A quantity may decay via two or more different processes simultaneously. In
general, these processes (often called "decay modes", "decay channels", "decay
routes" etc.) have different probabilities of occurring, and thus occur at
different rates with different half-lives, in parallel. The total decay rate of
the quantity N is given by the sum of the decay routes; thus, in the case of
two processes:
         &#x2212;    d N ( t )   d t    = N  &#x03BB;  1   + N  &#x03BB;  2   =
      (  &#x03BB;  1   +  &#x03BB;  2   ) N .   {\displaystyle -{\frac {dN(t)}
      {dt}}=N\lambda _{1}+N\lambda _{2}=(\lambda _{1}+\lambda _{2})N.}  [-
      {\frac {dN(t)}{dt}}=N\lambda _{1}+N\lambda _{2}=(\lambda _{1}+\lambda _
      {2})N.]
The solution to this equation is given in the previous section, where the sum
of      &#x03BB;  1   +  &#x03BB;  2      {\displaystyle \lambda _{1}+\lambda _
{2}\,}  [\lambda _{1}+\lambda _{2}\,] is treated as a new total decay constant
&#x03BB;  c     {\displaystyle \lambda _{c}}  [\lambda _{c}].
         N ( t ) =  N  0    e  &#x2212; (  &#x03BB;  1   +  &#x03BB;  2   ) t
      =  N  0    e  &#x2212; (  &#x03BB;  c   ) t   .   {\displaystyle N(t)=N_
      {0}e^{-(\lambda _{1}+\lambda _{2})t}=N_{0}e^{-(\lambda _{c})t}.}  [N
      (t)=N_{0}e^{-(\lambda _{1}+\lambda _{2})t}=N_{0}e^{-(\lambda _{c})t}.]
Partial mean life associated with individual processes is by definition the
multiplicative_inverse of corresponding partial decay constant:     &#x03C4; =
1  /  &#x03BB;   {\displaystyle \tau =1/\lambda }  [\tau =1/\lambda ]. A
combined      &#x03C4;  c     {\displaystyle \tau _{c}}  [\tau _{c}] can be
given in terms of     &#x03BB;   {\displaystyle \lambda }  [\lambda ]s:
           1  &#x03C4;  c     =  &#x03BB;  c   =  &#x03BB;  1   +  &#x03BB;  2
      =   1  &#x03C4;  1     +   1  &#x03C4;  2       {\displaystyle {\frac {1}
      {\tau _{c}}}=\lambda _{c}=\lambda _{1}+\lambda _{2}={\frac {1}{\tau _
      {1}}}+{\frac {1}{\tau _{2}}}}  [{\frac {1}{\tau _{c}}}=\lambda _
      {c}=\lambda _{1}+\lambda _{2}={\frac {1}{\tau _{1}}}+{\frac {1}{\tau _
      {2}}}]
          &#x03C4;  c   =     &#x03C4;  1    &#x03C4;  2      &#x03C4;  1   +
      &#x03C4;  2      .   {\displaystyle \tau _{c}={\frac {\tau _{1}\tau _{2}}
      {\tau _{1}+\tau _{2}}}.}  [\tau _{c}={\frac {\tau _{1}\tau _{2}}{\tau _
      {1}+\tau _{2}}}.]
Since half-lives differ from mean life     &#x03C4;   {\displaystyle \tau }
[\tau ] by a constant factor, the same equation holds in terms of the two
corresponding half-lives:
          T  1  /  2   =     t  1    t  2      t  1   +  t  2
      {\displaystyle T_{1/2}={\frac {t_{1}t_{2}}{t_{1}+t_{2}}}}  [T_{1/2}=
      {\frac {t_{1}t_{2}}{t_{1}+t_{2}}}]
where      T  1  /  2     {\displaystyle T_{1/2}}  [T_{1/2}] is the combined or
total half-life for the process,      t  1     {\displaystyle t_{1}}  [t_{1}]
and      t  2     {\displaystyle t_{2}}  [t_{2}] are so-named partial half-
lives of corresponding processes. Terms "partial half-life" and "partial mean
life" denote quantities derived from a decay constant as if the given decay
mode were the only decay mode for the quantity. The term "partial half-life" is
misleading, because it cannot be measured as a time interval for which a
certain quantity is halved.
In terms of separate decay constants, the total half-life      T  1  /  2
{\displaystyle T_{1/2}}  [T_{1/2}] can be shown to be
          T  1  /  2   =    ln &#x2061; 2   &#x03BB;  c     =    ln &#x2061; 2
      &#x03BB;  1   +  &#x03BB;  2      .   {\displaystyle T_{1/2}={\frac {\ln
      2}{\lambda _{c}}}={\frac {\ln 2}{\lambda _{1}+\lambda _{2}}}.}  [T_{1/2}=
      {\frac {\ln 2}{\lambda _{c}}}={\frac {\ln 2}{\lambda _{1}+\lambda _
      {2}}}.]
For a decay by three simultaneous exponential processes the total half-life can
be computed as above:
          T  1  /  2   =    ln &#x2061; 2   &#x03BB;  c     =    ln &#x2061; 2
      &#x03BB;  1   +  &#x03BB;  2   +  &#x03BB;  3      =     t  1    t  2
      t  3     (  t  1    t  2   ) + (  t  1    t  3   ) + (  t  2    t  3   )
      .   {\displaystyle T_{1/2}={\frac {\ln 2}{\lambda _{c}}}={\frac {\ln 2}
      {\lambda _{1}+\lambda _{2}+\lambda _{3}}}={\frac {t_{1}t_{2}t_{3}}{(t_
      {1}t_{2})+(t_{1}t_{3})+(t_{2}t_{3})}}.}  [T_{1/2}={\frac {\ln 2}{\lambda
      _{c}}}={\frac {\ln 2}{\lambda _{1}+\lambda _{2}+\lambda _{3}}}={\frac {t_
      {1}t_{2}t_{3}}{(t_{1}t_{2})+(t_{1}t_{3})+(t_{2}t_{3})}}.]
***** Applications and examples[edit] *****
Exponential decay occurs in a wide variety of situations. Most of these fall
into the domain of the natural_sciences.
Many decay processes that are often treated as exponential, are really only
exponential so long as the sample is large and the law_of_large_numbers holds.
For small samples, a more general analysis is necessary, accounting for a
Poisson_process.
**** Natural sciences[edit] ****
    * Chemical_reactions: The rates of certain types of chemical_reactions
      depend on the concentration of one or another reactant. Reactions whose
      rate depends only on the concentration of one reactant (known as first-
      order_reactions) consequently follow exponential decay. For instance,
      many enzyme-catalyzed reactions behave this way.
    * Electrostatics: The electric_charge (or, equivalently, the potential)
      contained in a capacitor (capacitance C) changes exponentially, if the
      capacitor experiences a constant external_load (resistance R). The
      exponential time-constant Ï for the process is R C, and the half-life is
      therefore R C ln2. This applies to both charging and discharging, i.e. a
      capacitor charges or discharges according to the same law. The same
      equations can be applied to the current in an inductor. (Furthermore, the
      particular case of a capacitor or inductor changing through several
      parallel resistors makes an interesting example of multiple decay
      processes, with each resistor representing a separate process. In fact,
      the expression for the equivalent_resistance of two resistors in parallel
      mirrors the equation for the half-life with two decay processes.)
    * Geophysics: Atmospheric_pressure decreases approximately exponentially
      with increasing height above sea level, at a rate of about 12% per 1000m.
      [citation_needed]
    * Heat_transfer: If an object at one temperature is exposed to a medium of
      another temperature, the temperature difference between the object and
      the medium follows exponential decay (in the limit of slow processes;
      equivalent to "good" heat conduction inside the object, so that its
      temperature remains relatively uniform through its volume). See also
      Newton's_law_of_cooling.
    * Luminescence: After excitation, the emission intensity â which is
      proportional to the number of excited atoms or molecules â of a
      luminescent material decays exponentially. Depending on the number of
      mechanisms involved, the decay can be mono- or multi-exponential.
    * Pharmacology and toxicology: It is found that many administered
      substances are distributed and metabolized (see clearance) according to
      exponential decay patterns. The biological_half-lives "alpha half-life"
      and "beta half-life" of a substance measure how quickly a substance is
      distributed and eliminated.
    * Physical_optics: The intensity of electromagnetic_radiation such as light
      or X-rays or gamma rays in an absorbent medium, follows an exponential
      decrease with distance into the absorbing medium. This is known as the
      Beer-Lambert law.
    * Radioactivity: In a sample of a radionuclide that undergoes radioactive
      decay to a different state, the number of atoms in the original state
      follows exponential decay as long as the remaining number of atoms is
      large. The decay product is termed a radiogenic nuclide.
    * Thermoelectricity: The decline in resistance of a Negative Temperature
      Coefficient Thermistor as temperature is increased.
    * Vibrations: Some vibrations may decay exponentially; this characteristic
      is often found in damped_mechanical_oscillators, and used in creating
      ADSR_envelopes in synthesizers. An overdamped system will simply return
      to equilibrium via an exponential decay.
    * Beer froth: Arnd Leike, of the Ludwig_Maximilian_University_of_Munich,
      won an Ig_Nobel_Prize for demonstrating that beer froth obeys the law of
      exponential decay.[1]
**** Social sciences[edit] ****
    * Finance: a retirement fund will decay exponentially being subject to
      discrete payout amounts, usually monthly, and an input subject to a
      continuous interest rate. A differential equation dA/dt = input â
      output can be written and solved to find the time to reach any amount A,
      remaining in the fund.
    * In simple glottochronology, the (debatable) assumption of a constant
      decay rate in languages allows one to estimate the age of single
      languages. (To compute the time of split between two languages requires
      additional assumptions, independent of exponential decay).
**** Computer science[edit] ****
    * The core routing_protocol on the Internet, BGP, has to maintain a routing
      table in order to remember the paths a packet can be deviated to. When
      one of these paths repeatedly changes its state from available to not
      available (and vice versa), the BGP router controlling that path has to
      repeatedly add and remove the path record from its routing table (flaps
      the path), thus spending local resources such as CPU and RAM and, even
      more, broadcasting useless information to peer routers. To prevent this
      undesired behavior, an algorithm named route flapping damping assigns
      each route a weight that gets bigger each time the route changes its
      state and decays exponentially with time. When the weight reaches a
      certain limit, no more flapping is done, thus suppressing the route.
Graphs comparing doubling times and half lives of exponential growths (bold
lines) and decay (faint lines), and their 70/t and 72/t approximations. In the
SVG_version, hover over a graph to highlight it and its complement.
***** See also[edit] *****
    * Exponential_formula
    * Exponential_growth
    * Radioactive_decay for the mathematics of chains of exponential processes
      with differing constants
***** References[edit] *****
   1. ^Leike, A. (2002). "Demonstration of the exponential decay law using beer
      froth". European Journal of Physics. 23: 21. Bibcode:2002EJPh...23...21L.
      CiteSeerX 10.1.1.693.5948. doi:10.1088/0143-0807/23/1/304.
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
***** External links[edit] *****
    * Exponential_decay_calculator
    * A_stochastic_simulation_of_exponential_decay
    * Tutorial_on_time_constants

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Exponential_decay&oldid=888853992"
Categories:
    * Exponentials
Hidden categories:
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_November_2016
    * Articles_with_unsourced_statements_from_November_2017
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
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Esperanto
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Italiano
    * ×¢××¨××ª
    * á¥áá áá£áá
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Suomi
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 21 March 2019, at 20:43 (UTC).
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
