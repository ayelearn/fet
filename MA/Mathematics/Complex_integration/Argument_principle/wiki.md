The following text has been accessed from https://en.wikipedia.org/wiki/Argument_principle at Fri Aug 9 02:37:30 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Argument principle ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
The simple contour C (black), the zeros of f (blue) and the poles of f (red).
Here we have         &#x222E;       C   &#x2061;     f &#x2032;  ( z )   f ( z
)     d z = 2 &#x03C0; i ( 4 &#x2212; 5 )   {\displaystyle \oint _{C}{f'(z)
\over f(z)}\,dz=2\pi i(4-5)}  [\oint_{C} {f'(z) \over f(z)}\, dz=2\pi i (4-5)].
In complex_analysis, the argument principle (or Cauchy's argument principle)
relates the difference between the number of zeros_and_poles of a meromorphic
function to a contour_integral of the function's logarithmic_derivative.
Specifically, if f(z) is a meromorphic function inside and on some closed
contour C, and f has no zeros or poles on C, then
             &#x222E;       C   &#x2061;     f &#x2032;  ( z )   f ( z )     d
      z = 2 &#x03C0; i ( Z &#x2212; P )   {\displaystyle \oint _{C}{f'(z) \over
      f(z)}\,dz=2\pi i(Z-P)}  [{\displaystyle \oint _{C}{f'(z) \over f
      (z)}\,dz=2\pi i(Z-P)}]
where Z and P denote respectively the number of zeros and poles of f(z) inside
the contour C, with each zero and pole counted as many times as its
multiplicity and order, respectively, indicate. This statement of the theorem
assumes that the contour C is simple, that is, without self-intersections, and
that it is oriented counter-clockwise.
More generally, suppose that f(z) is a meromorphic function on an open_set Î©
in the complex_plane and that C is a closed curve in Î© which avoids all zeros
and poles of f and is contractible to a point inside Î©. For each point z â
Î©, let n(C,z) be the winding_number of C around z. Then
             &#x222E;       C   &#x2061;     f &#x2032;  ( z )   f ( z )     d
      z = 2 &#x03C0; i  (   &#x2211;  a   n ( C , a ) &#x2212;  &#x2211;  b   n
      ( C , b )  )    {\displaystyle \oint _{C}{\frac {f'(z)}{f(z)}}\,dz=2\pi
      i\left(\sum _{a}n(C,a)-\sum _{b}n(C,b)\right)}  [\oint_{C} \frac{f'(z)}{f
      (z)}\, dz = 2\pi i \left(\sum_a n(C,a) - \sum_b n(C,b)\right)]
where the first summation is over all zeros a of f counted with their
multiplicities, and the second summation is over the poles b of f counted with
their orders.
⁰
***** Contents *****
    * 1_Interpretation_of_the_contour_integral
    * 2_Proof_of_the_argument_principle
    * 3_Applications_and_consequences
    * 4_Generalized_argument_principle
    * 5_History
    * 6_See_also
    * 7_References
***** Interpretation of the contour integral[edit] *****
The contour_integral         &#x222E;       C   &#x2061;     f &#x2032;  ( z )
f ( z )     d z   {\displaystyle \oint _{C}{\frac {f'(z)}{f(z)}}\,dz}  [\oint_
{C} \frac{f'(z)}{f(z)}\, dz] can be interpreted as 2πi times the winding number
of the path f(C) around the origin, using the substitution w = f(z):
             &#x222E;       C   &#x2061;     f &#x2032;  ( z )   f ( z )     d
      z =     &#x222E;       f ( C )   &#x2061;   1 w    d w   {\displaystyle
      \oint _{C}{\frac {f'(z)}{f(z)}}\,dz=\oint _{f(C)}{\frac {1}{w}}\,dw}
      [\oint_{C} \frac{f'(z)}{f(z)}\, dz = \oint_{f(C)} \frac{1}{w}\, dw]
That is, it is the total change in the argument of f(z) as z travels around C,
explaining the name of the theorem; this follows from
           d  d z    log &#x2061; ( f ( z ) ) =     f &#x2032;  ( z )   f ( z )
      {\displaystyle {\frac {d}{dz}}\log(f(z))={\frac {f'(z)}{f(z)}}}  [\frac
      {d}{dz}\log(f(z))=\frac{f'(z)}{f(z)}]
and the relation between arguments and logarithms.
***** Proof of the argument principle[edit] *****
Let zZ be a zero of f. We can write f(z) = (z − zZ)kg(z) where k is the
multiplicity of the zero, and thus g(zZ) â  0. We get
          f &#x2032;  ( z ) = k ( z &#x2212;  z  Z    )  k &#x2212; 1   g ( z )
      + ( z &#x2212;  z  Z    )  k    g &#x2032;  ( z )     {\displaystyle f'
      (z)=k(z-z_{Z})^{k-1}g(z)+(z-z_{Z})^{k}g'(z)\,\!}  [{\displaystyle f'(z)=k
      (z-z_{Z})^{k-1}g(z)+(z-z_{Z})^{k}g'(z)\,\!}]
and
             f &#x2032;  ( z )   f ( z )    =   k  z &#x2212;  z  Z      +
      g &#x2032;  ( z )   g ( z )    .   {\displaystyle {f'(z) \over f(z)}={k
      \over z-z_{Z}}+{g'(z) \over g(z)}.}  [{\displaystyle {f'(z) \over f(z)}=
      {k \over z-z_{Z}}+{g'(z) \over g(z)}.}]
Since g(zZ) â  0, it follows that g'(z)/g(z) has no singularities at zZ, and
thus is analytic at zZ, which implies that the residue of f′(z)/f(z) at zZ
is k.
Let zP be a pole of f. We can write f(z) = (z − zP)−mh(z) where m is the order
of the pole, and h(zP) â  0. Then,
          f &#x2032;  ( z ) = &#x2212; m ( z &#x2212;  z  P    )  &#x2212; m
      &#x2212; 1   h ( z ) + ( z &#x2212;  z  P    )  &#x2212; m    h &#x2032;
      ( z )   .   {\displaystyle f'(z)=-m(z-z_{P})^{-m-1}h(z)+(z-z_{P})^{-m}h'
      (z)\,\!.}  [f'(z)=-m(z-z_P)^{-m-1}h(z)+(z-z_P)^{-m}h'(z)\,\!.]
and
             f &#x2032;  ( z )   f ( z )    =    &#x2212; m   z &#x2212;  z  P
      +     h &#x2032;  ( z )   h ( z )      {\displaystyle {f'(z) \over f(z)}=
      {-m \over z-z_{P}}+{h'(z) \over h(z)}}  [{f'(z)\over f(z)}={-m \over z-
      z_P}+{h'(z)\over h(z)}]
similarly as above. It follows that h′(z)/h(z) has no singularities at zP since
h(zP) â  0 and thus it is analytic at zP. We find that the residue of f′(z)/f
(z) at zP is −m.
Putting these together, each zero zZ of multiplicity k of f creates a simple
pole for f′(z)/f(z) with the residue being k, and each pole zP of order m of f
creates a simple pole for f′(z)/f(z) with the residue being −m. (Here, by a
simple pole we mean a pole of order one.) In addition, it can be shown that f′
(z)/f(z) has no other poles, and so no other residues.
By the residue_theorem we have that the integral about C is the product of 2Ïi
and the sum of the residues. Together, the sum of the k 's for each zero zZ is
the number of zeros counting multiplicities of the zeros, and likewise for the
poles, and so we have our result.
***** Applications and consequences[edit] *****
The argument principle can be used to efficiently locate zeros or poles of
meromorphic functions on a computer. Even with rounding errors, the expression
1  2 &#x03C0; i        &#x222E;       C   &#x2061;     f &#x2032;  ( z )   f
( z )     d z   {\displaystyle {1 \over 2\pi i}\oint _{C}{f'(z) \over f
(z)}\,dz}  [{1\over 2\pi i}\oint_{C} {f'(z) \over f(z)}\, dz] will yield
results close to an integer; by determining these integers for different
contours C one can obtain information about the location of the zeros and
poles. Numerical tests of the Riemann_hypothesis use this technique to get an
upper bound for the number of zeros of Riemann's_____&#x03BE;_(_s_)___
{\displaystyle_\xi_(s)}__[\xi(s)]_function inside a rectangle intersecting the
critical line.
The proof of RouchÃ©'s_theorem uses the argument principle.
Modern books on feedback control theory quite frequently use the argument
principle to serve as the theoretical basis of the Nyquist_stability_criterion.
A consequence of the more general formulation of the argument principle is
that, under the same hypothesis, if g is an analytic function in Î©, then
           1  2 &#x03C0; i        &#x222E;       C   &#x2061; g ( z )     f
      &#x2032;  ( z )   f ( z )     d z =  &#x2211;  a   n ( C , a ) g ( a )
      &#x2212;  &#x2211;  b   n ( C , b ) g ( b ) .   {\displaystyle {\frac {1}
      {2\pi i}}\oint _{C}g(z){\frac {f'(z)}{f(z)}}\,dz=\sum _{a}n(C,a)g(a)-\sum
      _{b}n(C,b)g(b).}  [ \frac{1}{2\pi i} \oint_C g(z)\frac{f'(z)}{f(z)}\, dz
      = \sum_a n(C,a)g(a) - \sum_b n(C,b)g(b).]
For example, if f is a polynomial having zeros z1, ..., zp inside a simple
contour C, and g(z) = zk, then
           1  2 &#x03C0; i        &#x222E;       C   &#x2061;  z  k       f
      &#x2032;  ( z )   f ( z )     d z =  z  1   k   +  z  2   k   + &#x22EF;
      +  z  p   k   ,   {\displaystyle {\frac {1}{2\pi i}}\oint _{C}z^{k}{\frac
      {f'(z)}{f(z)}}\,dz=z_{1}^{k}+z_{2}^{k}+\cdots +z_{p}^{k},}  [
      {\displaystyle {\frac {1}{2\pi i}}\oint _{C}z^{k}{\frac {f'(z)}{f
      (z)}}\,dz=z_{1}^{k}+z_{2}^{k}+\cdots +z_{p}^{k},}]
is power_sum_symmetric_polynomial of the roots of f.
Another consequence is if we compute the complex integral:
             &#x222E;       C   &#x2061; f ( z )     g &#x2032;  ( z )   g ( z
      )     d z   {\displaystyle \oint _{C}f(z){g'(z) \over g(z)}\,dz}
      [\oint_C f(z){g'(z) \over g(z)}\, dz]
for an appropriate choice of g and f we have the AbelâPlana_formula:
          &#x2211;  n = 0   &#x221E;   f ( n ) &#x2212;  &#x222B;  0   &#x221E;
      f ( x )  d x = f ( 0 )  /  2 + i  &#x222B;  0   &#x221E;      f ( i t )
      &#x2212; f ( &#x2212; i t )    e  2 &#x03C0; t   &#x2212; 1     d t
      {\displaystyle \sum _{n=0}^{\infty }f(n)-\int _{0}^{\infty }f(x)\,dx=f
      (0)/2+i\int _{0}^{\infty }{\frac {f(it)-f(-it)}{e^{2\pi t}-1}}\,dt}
      [  \sum_{n=0}^{\infty}f(n)-\int_{0}^{\infty}f(x)\,dx= f(0)/2+i\int_{0}^
      {\infty}\frac{f(it)-f(-it)}{e^{2\pi t}-1}\, dt ]
which expresses the relationship between a discrete sum and its integral.
***** Generalized argument principle[edit] *****
There is an immediate generalization of the argument principle. Suppose that g
is analytic in the region     &#x03A9;   {\displaystyle \Omega }  [\Omega ].
Then
             &#x222E;       C   &#x2061;     f &#x2032;  ( z )   f ( z )    g
      ( z )  d z = 2 &#x03C0; i  (   &#x2211;  a   g ( a ) n ( C , a ) &#x2212;
      &#x2211;  b   g ( b ) n ( C , b )  )    {\displaystyle \oint _{C}{f'(z)
      \over f(z)}g(z)\,dz=2\pi i\left(\sum _{a}g(a)n(C,a)-\sum _{b}g(b)n
      (C,b)\right)}  [\oint_{C} {f'(z) \over f(z)} g(z) \, dz = 2\pi i \left
      (\sum_a g(a) n(C,a) - \sum_b g(b) n(C,b)\right)]
where the first summation is again over all zeros a of f counted with their
multiplicities, and the second summation is again over the poles b of f counted
with their orders.
***** History[edit] *****
According to the book by Frank_Smithies (Cauchy and the Creation of Complex
Function Theory, Cambridge University Press, 1997, p. 177), Augustin-Louis
Cauchy presented a theorem similar to the above on 27 November 1831, during his
self-imposed exile in Turin (then capital of the Kingdom of Piedmont-Sardinia)
away from France. However, according to this book, only zeroes were mentioned,
not poles. This theorem by Cauchy was only published many years later in 1874
in a hand-written form and so is quite difficult to read. Cauchy published a
paper with a discussion on both zeroes and poles in 1855, two years before his
death.
***** See also[edit] *****
    * Logarithmic_derivative
    * Nyquist_stability_criterion
***** References[edit] *****
    * Rudin, Walter (1986). Real and Complex Analysis (International Series in
      Pure and Applied Mathematics). McGraw-Hill. ISBN 978-0-07-054234-1.
Ahlfors, Lars (1979). Complex analysis: an introduction to the theory of
analytic functions of one complex variable. McGraw-Hill. ISBN 978-0-07-000657-
7.
Churchill, Ruel Vance; Brown, James Ward (1989). Complex Variables and
Applications. McGraw-Hill. ISBN 978-0-07-010905-6.
Backlund, R.-J. (1914) Sur les zÃ©ros de la fonction zeta(s) de Riemann, C. R.
Acad. Sci. Paris 158, 1979â1982.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Argument_principle&oldid=895164651"
Categories:
    * Theorems_in_complex_analysis
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
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * ×¢××¨××ª
    * Lumbaart
    * Magyar
    * æ¥æ¬èª
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Svenska
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 2 May 2019, at 12:34 (UTC).
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
