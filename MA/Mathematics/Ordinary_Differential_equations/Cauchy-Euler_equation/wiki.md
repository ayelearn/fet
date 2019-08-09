The following text has been accessed from https://en.wikipedia.org/wiki/Cauchy%E2%80%93Euler_equation at Fri Aug 9 02:32:07 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** CauchyâEuler equation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, a Cauchy-Euler equation (most commonly known as the Euler-
Cauchy equation, or simply Euler's equation) is a linear homogeneous ordinary
differential_equation with variable_coefficients. It is sometimes referred to
as an equidimensional equation. Because of its particularly simple
equidimensional structure the differential equation can be solved explicitly.
⁰
***** Contents *****
    * 1_The_equation
          o 1.1_Second_order_â_solving_through_trial_solution
          o 1.2_Second_order_â_solution_through_change_of_variables
          o 1.3_Example
    * 2_Difference_equation_analogue
    * 3_See_also
    * 4_References
    * 5_Bibliography
***** The equation[edit] *****
Let y(n)(x) be the nth derivative of the unknown function y(x). Then a
CauchyâEuler equation of order n has the form
          a  n    x  n    y  ( n )   ( x ) +  a  n &#x2212; 1    x  n &#x2212;
      1    y  ( n &#x2212; 1 )   ( x ) + &#x22EF; +  a  0   y ( x ) = 0.
      {\displaystyle a_{n}x^{n}y^{(n)}(x)+a_{n-1}x^{n-1}y^{(n-1)}(x)+\cdots +a_
      {0}y(x)=0.}  [a_{{n}}x^{n}y^{{(n)}}(x)+a_{{n-1}}x^{{n-1}}y^{{(n-1)}}
      (x)+\cdots +a_{0}y(x)=0.]
The substitution     x =  e  u     {\displaystyle x=e^{u}}  [x=e^{u}] (that is,
u = l n ( x )   {\displaystyle u=ln(x)}  [{\displaystyle u=ln(x)}]; for     x <
0   {\displaystyle x<0}  [x<0], one might replace all instances of     x
{\displaystyle x}  [x] by      |  x  |    {\displaystyle |x|}  [|x|], which
extends the solution's domain to      R  0     {\displaystyle R_{0}}  [R_{0}])
may be used to reduce this equation to a linear differential equation with
constant coefficients. Alternatively, the trivial solution     y =  x  m
{\displaystyle y=x^{m}}  [y=x^{m}] may be used to directly solve for the basic
solutions.[1]
**** Second order â solving through trial solution[edit] ****
Typical solution curves for a second-order EulerâCauchy equation for the case
of two real roots
Typical solution curves for a second-order EulerâCauchy equation for the case
of a double root
Typical solution curves for a second-order EulerâCauchy equation for the case
of complex roots
The most common CauchyâEuler equation is the second-order equation, appearing
in a number of physics and engineering applications, such as when solving
Laplace's_equation in polar coordinates. The second order Cauchy-Euler equation
is[1]
          x  2       d  2   y   d  x  2      + a x    d y   d x    + b y = 0.
      {\displaystyle x^{2}{\frac {d^{2}y}{dx^{2}}}+ax{\frac {dy}{dx}}+by=0.\,}
      [x^{2}{\frac  {d^{2}y}{dx^{2}}}+ax{\frac  {dy}{dx}}+by=0.\,]
We assume a trial solution[1]
         y =  x  m   .    {\displaystyle y=x^{m}.\,}  [y=x^{m}.\,]
Differentiating gives
            d y   d x    = m  x  m &#x2212; 1      {\displaystyle {\frac {dy}
      {dx}}=mx^{m-1}\,}  [{\frac  {dy}{dx}}=mx^{{m-1}}\,]
and
             d  2   y   d  x  2      = m ( m &#x2212; 1 )  x  m &#x2212; 2   .
      {\displaystyle {\frac {d^{2}y}{dx^{2}}}=m(m-1)x^{m-2}.\,}  [{\frac  {d^
      {2}y}{dx^{2}}}=m(m-1)x^{{m-2}}.\,]
Substituting into the original equation leads to requiring
          x  2   ( m ( m &#x2212; 1 )  x  m &#x2212; 2   ) + a x ( m  x  m
      &#x2212; 1   ) + b (  x  m   ) = 0    {\displaystyle x^{2}(m(m-1)x^{m-
      2})+ax(mx^{m-1})+b(x^{m})=0\,}  [x^{2}(m(m-1)x^{{m-2}})+ax(mx^{{m-1}})+b
      (x^{m})=0\,]
Rearranging and factoring gives the indicial equation
          m  2   + ( a &#x2212; 1 ) m + b = 0.    {\displaystyle m^{2}+(a-
      1)m+b=0.\,}  [m^{2}+(a-1)m+b=0.\,]
We then solve for m. There are three particular cases of interest:
    * Case #1 of two distinct roots, m1 and m2;
    * Case #2 of one real repeated root, m;
    * Case #3 of complex roots, Î± Â± Î²i.
In case #1, the solution is
         y =  c  1    x   m  1     +  c  2    x   m  2        {\displaystyle
      y=c_{1}x^{m_{1}}+c_{2}x^{m_{2}}\,}  [y=c_{1}x^{{m_{{1}}}}+c_{2}x^{{m_
      {2}}}\,]
In case #2, the solution is
         y =  c  1    x  m   ln &#x2061; ( x ) +  c  2    x  m
      {\displaystyle y=c_{1}x^{m}\ln(x)+c_{2}x^{m}\,}  [y=c_{1}x^{m}\ln(x)+c_
      {2}x^{m}\,]
To get to this solution, the method of reduction_of_order must be applied after
having found one solution y = xm.
In case #3, the solution is
         y =  c  1    x  &#x03B1;   cos &#x2061; ( &#x03B2; ln &#x2061; ( x ) )
      +  c  2    x  &#x03B1;   sin &#x2061; ( &#x03B2; ln &#x2061; ( x ) )
      {\displaystyle y=c_{1}x^{\alpha }\cos(\beta \ln(x))+c_{2}x^{\alpha }\sin
      (\beta \ln(x))\,}  [y=c_{1}x^{\alpha }\cos(\beta \ln(x))+c_{2}x^{\alpha
      }\sin(\beta \ln(x))\,]
         &#x03B1; =   R e   &#x2061; ( m )    {\displaystyle \alpha =\mathop
      {\rm {Re}} (m)\,}  [\alpha ={\mathop  {{\rm {Re}}}}(m)\,]
         &#x03B2; =   I m   &#x2061; ( m )    {\displaystyle \beta =\mathop
      {\rm {Im}} (m)\,}  [\beta ={\mathop  {{\rm {Im}}}}(m)\,]
For      c  1   ,  c  2     {\displaystyle c_{1},c_{2}}  [c_{1},c_{2}] â â
.
This form of the solution is derived by setting x = et and using Euler's
formula
**** Second order â solution through change of variables[edit] ****
          x  2       d  2   y   d  x  2      + a x    d y   d x    + b y = 0
      {\displaystyle x^{2}{\frac {d^{2}y}{dx^{2}}}+ax{\frac {dy}{dx}}+by=0\,}
      [x^{2}{\frac  {d^{2}y}{dx^{2}}}+ax{\frac  {dy}{dx}}+by=0\,]
We operate the variable substitution defined by
         t = ln &#x2061; ( x ) .    {\displaystyle t=\ln(x).\,}  [t=\ln(x).\,]
         y ( x ) = &#x03D5; ( ln &#x2061; ( x ) ) = &#x03D5; ( t ) .
      {\displaystyle y(x)=\phi (\ln(x))=\phi (t).\,}  [y(x)=\phi (\ln(x))=\phi
      (t).\,]
Differentiating gives
            d y   d x    =   1 x      d &#x03D5;   d t      {\displaystyle
      {\frac {dy}{dx}}={\frac {1}{x}}{\frac {d\phi }{dt}}}  [{\frac  {dy}{dx}}=
      {\frac  {1}{x}}{\frac  {d\phi }{dt}}]
             d  2   y   d  x  2      =   1  x  2       (       d  2   &#x03D5;
      d  t  2      &#x2212;    d &#x03D5;   d t      )   .   {\displaystyle
      {\frac {d^{2}y}{dx^{2}}}={\frac {1}{x^{2}}}{\bigg (}{\frac {d^{2}\phi }
      {dt^{2}}}-{\frac {d\phi }{dt}}{\bigg )}.}  [{\frac  {d^{2}y}{dx^{2}}}=
      {\frac  {1}{x^{2}}}{\bigg (}{\frac  {d^{2}\phi }{dt^{2}}}-{\frac  {d\phi
      }{dt}}{\bigg )}.]
Substituting     &#x03D5; ( t )   {\displaystyle \phi (t)}  [\phi (t)] the
differential equation becomes
             d  2   &#x03D5;   d  t  2      + ( a &#x2212; 1 )    d &#x03D5;
      d t    + b &#x03D5; = 0.    {\displaystyle {\frac {d^{2}\phi }{dt^{2}}}+
      (a-1){\frac {d\phi }{dt}}+b\phi =0.\,}  [{\frac  {d^{2}\phi }{dt^{2}}}+
      (a-1){\frac  {d\phi }{dt}}+b\phi =0.\,]
This equation in     &#x03D5; ( t )   {\displaystyle \phi (t)}  [\phi (t)] is
solved via its characteristic polynomial
          &#x03BB;  2   + ( a &#x2212; 1 ) &#x03BB; + b = 0.   {\displaystyle
      \lambda ^{2}+(a-1)\lambda +b=0.}  [\lambda ^{2}+(a-1)\lambda +b=0.]
Now let      &#x03BB;  1     {\displaystyle \lambda _{1}}  [\lambda _{1}] and
&#x03BB;  2     {\displaystyle \lambda _{2}}  [\lambda _{2}] denote the two
roots of this polynomial. We analyze the two main cases: distinct roots and
double roots:
If the roots are distinct, the general solution is
         &#x03D5; ( t ) =  c  1    e   &#x03BB;  1   t   +  c  2    e
      &#x03BB;  2   t     {\displaystyle \phi (t)=c_{1}e^{\lambda _{1}t}+c_
      {2}e^{\lambda _{2}t}}  [\phi (t)=c_{1}e^{{\lambda _{1}t}}+c_{2}e^{
      {\lambda _{2}t}}], where the exponentials may be complex.
If the roots are equal, the general solution is
         &#x03D5; ( t ) =  c  1    e   &#x03BB;  1   t   +  c  2   t  e
      &#x03BB;  1   t   .   {\displaystyle \phi (t)=c_{1}e^{\lambda _{1}t}+c_
      {2}te^{\lambda _{1}t}.}  [\phi (t)=c_{1}e^{{\lambda _{1}t}}+c_{2}te^{
      {\lambda _{1}t}}.]
In both cases, the solution     y ( x )   {\displaystyle y(x)}  [y(x)] may be
found by setting     t = ln &#x2061; ( x )   {\displaystyle t=\ln(x)}  [t=\ln
(x)].
Hence, in the first case,
         y ( x ) =  c  1    x   &#x03BB;  1     +  c  2    x   &#x03BB;  2
      {\displaystyle y(x)=c_{1}x^{\lambda _{1}}+c_{2}x^{\lambda _{2}}}  [y
      (x)=c_{1}x^{{\lambda _{1}}}+c_{2}x^{{\lambda _{2}}}],
and in the second case,
         y ( x ) =  c  1    x   &#x03BB;  1     +  c  2   ln &#x2061; ( x )  x
      &#x03BB;  1     .   {\displaystyle y(x)=c_{1}x^{\lambda _{1}}+c_{2}\ln
      (x)x^{\lambda _{1}}.}  [y(x)=c_{1}x^{{\lambda _{1}}}+c_{2}\ln(x)x^{
      {\lambda _{1}}}.]
**** Example[edit] ****
Given
          x  2    u &#x2033;  &#x2212; 3 x  u &#x2032;  + 3 u = 0  ,
      {\displaystyle x^{2}u''-3xu'+3u=0\,,}  [x^{2}u''-3xu'+3u=0\,,]
we substitute the simple solution xm:
          x  2   ( m ( m &#x2212; 1 )  x  m &#x2212; 2   ) &#x2212; 3 x ( m  x
      m &#x2212; 1   ) + 3  x  m   = m ( m &#x2212; 1 )  x  m   &#x2212; 3 m  x
      m   + 3  x  m   = (  m  2   &#x2212; 4 m + 3 )  x  m   = 0  .
      {\displaystyle x^{2}(m(m-1)x^{m-2})-3x(mx^{m-1})+3x^{m}=m(m-1)x^{m}-3mx^
      {m}+3x^{m}=(m^{2}-4m+3)x^{m}=0\,.}  [{\displaystyle x^{2}(m(m-1)x^{m-2})-
      3x(mx^{m-1})+3x^{m}=m(m-1)x^{m}-3mx^{m}+3x^{m}=(m^{2}-4m+3)x^{m}=0\,.}]
For xm to be a solution, either x = 0, which gives the trivial solution, or the
coefficient of xm is zero. Solving the quadratic equation, we get m = 1, 3. The
general solution is therefore
         u =  c  1   x +  c  2    x  3    .   {\displaystyle u=c_{1}x+c_{2}x^
      {3}\,.}  [u=c_{1}x+c_{2}x^{3}\,.]
***** Difference equation analogue[edit] *****
There is a difference_equation analogue to the Cauchy–Euler equation. For a
fixed m > 0, define the sequence Æm(n) as
          f  m   ( n ) := n ( n + 1 ) &#x22EF; ( n + m &#x2212; 1 ) .
      {\displaystyle f_{m}(n):=n(n+1)\cdots (n+m-1).}  [f_{m}(n):=n(n+1)\cdots
      (n+m-1).]
Applying the difference operator to      f  m     {\displaystyle f_{m}}  [f_
{m}], we find that
             D  f  m   ( n )    =  f  m   ( n + 1 ) &#x2212;  f  m   ( n )
      = m ( n + 1 ) ( n + 2 ) &#x22EF; ( n + m &#x2212; 1 ) =   m n    f  m
      ( n ) .       {\displaystyle {\begin{aligned}Df_{m}(n)&=f_{m}(n+1)-f_{m}
      (n)\\&=m(n+1)(n+2)\cdots (n+m-1)={\frac {m}{n}}f_{m}(n).\end{aligned}}}
      [{\begin{aligned}Df_{m}(n)&=f_{{m}}(n+1)-f_{m}(n)\\&=m(n+1)(n+2)\cdots
      (n+m-1)={\frac  {m}{n}}f_{m}(n).\end{aligned}}]
If we do this k times, we find that
              f  m   ( k )   ( n )    =    m ( m &#x2212; 1 ) &#x22EF; ( m
      &#x2212; k + 1 )   n ( n + 1 ) &#x22EF; ( n + k &#x2212; 1 )     f  m
      ( n )       = m ( m &#x2212; 1 ) &#x22EF; ( m &#x2212; k + 1 )     f  m
      ( n )    f  k   ( n )    ,       {\displaystyle {\begin{aligned}f_{m}^{
      (k)}(n)&={\frac {m(m-1)\cdots (m-k+1)}{n(n+1)\cdots (n+k-1)}}f_{m}
      (n)\\&=m(m-1)\cdots (m-k+1){\frac {f_{m}(n)}{f_{k}(n)}},\end{aligned}}}
      [{\begin{aligned}f_{m}^{{(k)}}(n)&={\frac  {m(m-1)\cdots (m-k+1)}{n
      (n+1)\cdots (n+k-1)}}f_{m}(n)\\&=m(m-1)\cdots (m-k+1){\frac  {f_{m}(n)}
      {f_{k}(n)}},\end{aligned}}]
where the superscript (k) denotes applying the difference operator k times.
Comparing this to the fact that the k-th derivative of xm equals
         m ( m &#x2212; 1 ) &#x22EF; ( m &#x2212; k + 1 )    x  m    x  k
      {\displaystyle m(m-1)\cdots (m-k+1){\frac {x^{m}}{x^{k}}}}  [m(m-1)\cdots
      (m-k+1){\frac  {x^{m}}{x^{k}}}]
suggests that we can solve the N-th order difference equation
          f  N   ( n )  y  ( N )   ( n ) +  a  N &#x2212; 1    f  N &#x2212; 1
      ( n )  y  ( N &#x2212; 1 )   ( n ) + &#x22EF; +  a  0   y ( n ) = 0 ,
      {\displaystyle f_{N}(n)y^{(N)}(n)+a_{N-1}f_{N-1}(n)y^{(N-1)}(n)+\cdots
      +a_{0}y(n)=0,}  [f_{N}(n)y^{{(N)}}(n)+a_{{N-1}}f_{{N-1}}(n)y^{{(N-1)}}
      (n)+\cdots +a_{0}y(n)=0,]
in a similar manner to the differential equation case. Indeed, substituting the
trial solution
         y ( n ) =  f  m   ( n )    {\displaystyle y(n)=f_{m}(n)\,}  [y(n)=f_
      {m}(n)\,]
brings us to the same situation as the differential equation case,
         m ( m &#x2212; 1 ) &#x22EF; ( m &#x2212; N + 1 ) +  a  N &#x2212; 1
      m ( m &#x2212; 1 ) &#x22EF; ( m &#x2212; N + 2 ) + &#x22EF; +  a  1   m +
      a  0   = 0.   {\displaystyle m(m-1)\cdots (m-N+1)+a_{N-1}m(m-1)\cdots (m-
      N+2)+\cdots +a_{1}m+a_{0}=0.}  [m(m-1)\cdots (m-N+1)+a_{{N-1}}m(m-
      1)\cdots (m-N+2)+\cdots +a_{1}m+a_{0}=0.]
One may now proceed as in the differential equation case, since the general
solution of an N-th order linear difference equation is also the linear
combination of N linearly independent solutions. Applying reduction of order in
case of a multiple root m1 will yield expressions involving a discrete version
of ln,
         &#x03C6; ( n ) =  &#x2211;  k = 1   n     1  k &#x2212;  m  1      .
      {\displaystyle \varphi (n)=\sum _{k=1}^{n}{\frac {1}{k-m_{1}}}.}
      [\varphi (n)=\sum _{{k=1}}^{n}{\frac  {1}{k-m_{1}}}.]
(Compare with:     ln &#x2061; ( x &#x2212;  m  1   ) =  &#x222B;  1 +  m  1
x     1  t &#x2212;  m  1       d t .   {\displaystyle \ln(x-m_{1})=\int _{1+m_
{1}}^{x}{\frac {1}{t-m_{1}}}\,dt.}  [\ln(x-m_{1})=\int _{{1+m_{1}}}^{x}{\frac
{1}{t-m_{1}}}\,dt.])
In cases where fractions become involved, one may use
          f  m   ( n ) :=    &#x0393; ( n + m )   &#x0393; ( n )
      {\displaystyle f_{m}(n):={\frac {\Gamma (n+m)}{\Gamma (n)}}}  [f_{m}(n):=
      {\frac  {\Gamma (n+m)}{\Gamma (n)}}]
instead (or simply use it in all cases), which coincides with the definition
before for integer m.
***** See also[edit] *****
    * Hypergeometric_differential_equation
    * CauchyâEuler_operator
***** References[edit] *****
   1. ^ a b cKreyszig, Erwin (May 10, 2006). Advanced Engineering Mathematics.
      Wiley. ISBN 978-0-470-08484-7.
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
***** Bibliography[edit] *****
    * Weisstein,_Eric_W. "CauchyâEuler_equation". MathWorld.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=CauchyâEuler_equation&oldid=894113422"
Categories:
    * Ordinary_differential_equations
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
    * ÄeÅ¡tina
    * Deutsch
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * ×¢××¨××ª
    * Magyar
    * áá¶áá¶ááááá
    * PiemontÃ¨is
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 25 April 2019, at 18:45 (UTC).
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
