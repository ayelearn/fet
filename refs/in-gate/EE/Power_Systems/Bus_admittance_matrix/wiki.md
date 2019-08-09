The following text has been accessed from https://en.wikipedia.org/wiki/Nodal_admittance_matrix at Thu Aug 8 22:53:25 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Nodal admittance matrix ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
This article is about the admittance matrix in electrical engineering. For the
graph theoretic admittance matrix, see Laplacian_matrix.
In power_engineering, nodal admittance matrix (or just admittance matrix) or Y
Matrix or Ybus is an N x N matrix describing a power system with N buses. It
represents the nodal admittance of the buses in a power system. In realistic
systems which contain thousands of buses, the Y matrix is quite sparse. Each
bus in a real power system is usually connected to only a few other buses
through the transmission_lines. The Y Matrix is also one of the data
requirements needed to formulate a power_flow_study.
⁰
***** Contents *****
    * 1_Context
    * 2_Construction
    * 3_See_also
    * 4_References
    * 5_External_links
***** Context[edit] *****
Electric_power_transmission needs optimization in order to determine the
necessary real and reactive power flows in a system for a given set of loads,
as well as the voltages and currents in the system. Power flow studies are used
not only to analyze current power flow situations, but also to plan ahead for
anticipated disturbances to the system, such as the loss of a transmission line
to maintenance and repairs. The power flow study would determine whether or not
the system could continue functioning properly without the transmission line.
Only computer_simulation allows the complex handling required in power flow
analysis because in most realistic situations the system is very complex and
extensive and would be impractical to solve by hand. The Y Matrix is a tool in
that domain. It provides a method of systematically reducing a complex system
to a matrix that can be solved by a computer program. The equations used to
construct the Y matrix come from the application of Kirchhoffâs current law
and Kirchhoffâs voltage law to a circuit with steady-state sinusoidal
operation. These laws give us that the sum of currents entering a node in the
circuit is zero, and the sum of voltages around a closed loop starting and
ending at a node is also zero. These principles are applied to all the nodes in
a power flow system and thereby determine the elements of the admittance
matrix, which represents the admittance relationships between nodes, which then
determine the voltages, currents and power flows in the system.
***** Construction[edit] *****
Starting from the single_line_diagram of a power system, there are three main
steps before writing the equations that form the     Y   {\displaystyle Y}  [Y]
Matrix. First, the single line diagram is converted to an impedance diagram.
Next, all voltage sources are converted to their equivalent current source
representations. From here, the impedance diagram is then converted to an
admittance diagram. Following these three steps, the admittance matrix can be
created in a straightforward manner: For an admittance diagram with     N
{\displaystyle N}  [N] buses, the admittance between the bus in consideration,
k, and another bus, i, connected to k, can be described by      y  i k   =  g
i k   + j  b  i k     {\displaystyle y_{ik}=g_{ik}+jb_{ik}}  [{\displaystyle y_
{ik}=g_{ik}+jb_{ik}}]. The term      y  k     {\displaystyle y_{k}}  [y_{k}]
should be introduced here; this term accounts for the admittance of linear
loads connected to bus     k   {\displaystyle k}  [k] as well as the
admittance-to-ground at bus     k   {\displaystyle k}  [k]. The general
mathematical expression follows:
          Y  i j   =   {     y  i   +  &#x2211;    k = 1 , 2 , &#x2026; , N   k
      &#x2260; i       y  i k    ,     if    i = j     &#x2212;  y  i j   ,
      if    i &#x2260; j         {\displaystyle Y_{ij}={\begin{cases}y_{i}+\sum
      _{k=1,2,\ldots ,N \atop k\neq i}{y_{ik}},&{\mbox{if}}\quad i=j\\-y_{ij},&
      {\mbox{if}}\quad i\neq j\end{cases}}}  [
      Y_{ij} = \begin{cases}
        y_{i} + \sum_{k=1, 2, \ldots, N \atop k \neq i} {y_{ik}}, & \mbox{if}
      \quad i = j \\
        -y_{ij},  & \mbox{if} \quad i \neq j
      \end{cases}
      ]
It is important to note that      y  k i     {\displaystyle y_{ki}}  [
{\displaystyle y_{ki}}] is non-zero only where a physical connection exists
between two buses.[1] This consideration is not seen in the following example
because each node is connected to both of the other nodes. Each      y  k i
{\displaystyle y_{ki}}  [{\displaystyle y_{ki}}] defines one element of the
N &#x00D7;  N    {\displaystyle N\times {N}}  [{\displaystyle N\times {N}}]
matrix. From the general case where N is greater than 2, it is desirable to
solve these equations as a system, namely through matrix algebra. The general
matrix appears as follows: The nodal admittance matrix form:     Y =   [     Y
11      Y  12     &#x22EF;    Y  1 n        Y  21      Y  22     &#x22EF;    Y
2 n       &#x22EF;   &#x22EF;   &#x22EF;   &#x22EF;      Y  n 1      Y  n 2
&#x22EF;    Y  n n      ]     {\displaystyle Y={\begin{bmatrix}Y_{11}&Y_
{12}&\cdots &Y_{1n}\\Y_{21}&Y_{22}&\cdots &Y_{2n}\\\cdots &\cdots &\cdots
&\cdots \\Y_{n1}&Y_{n2}&\cdots &Y_{nn}\end{bmatrix}}}  [Y={\begin{bmatrix}Y_{
{11}}&Y_{{12}}&\cdots &Y_{{1n}}\\Y_{{21}}&Y_{{22}}&\cdots &Y_{{2n}}\\\cdots
&\cdots &\cdots &\cdots \\Y_{{n1}}&Y_{{n2}}&\cdots &Y_{{nn}}\end{bmatrix}}]
The admittance diagram of a three bus network.
Once the admittance matrix has been formed, the admittance matrix can be input
to solve the matrix form of Ohm's Law--the equation     Y &#x2217; V = I
{\displaystyle Y*V=I}  [{\displaystyle Y*V=I}]. In this instance     V
{\displaystyle V}  [V] is an     N &#x00D7;  1    {\displaystyle N\times {1}}
[{\displaystyle N\times {1}}] vector of the voltage at each node and     I
{\displaystyle I}  [I] is the     N &#x00D7;  1    {\displaystyle N\times {1}}
[{\displaystyle N\times {1}}] vector of corresponding currents. In matrix form,
Ohm's Law is as follows:
           (     Y  11      Y  12     &#x22EF;    Y  1 N        Y  21      Y
      22     &#x22EF;    Y  2 N       &#x22EE;   &#x22F1;   &#x22EF;   &#x22EE;
      Y  N N      Y  N 2     &#x22EF;    Y  N N      )   &#x2217;   (     V  1
      V  2       &#x22EE;      V  N      )   =   (     I  1        I  2
      &#x22EE;      I  N      )     {\displaystyle {\begin{pmatrix}Y_{11}&Y_
      {12}&\cdots &Y_{1N}\\Y_{21}&Y_{22}&\cdots &Y_{2N}\\\vdots &\ddots &\cdots
      &\vdots \\Y_{NN}&Y_{N2}&\cdots &Y_{NN}\\\end{pmatrix}}*{\begin{pmatrix}V_
      {1}\\V_{2}\\\vdots \\V_{N}\\\end{pmatrix}}={\begin{pmatrix}I_{1}\\I_
      {2}\\\vdots \\I_{N}\\\end{pmatrix}}}  [{\displaystyle {\begin{pmatrix}Y_
      {11}&Y_{12}&\cdots &Y_{1N}\\Y_{21}&Y_{22}&\cdots &Y_{2N}\\\vdots &\ddots
      &\cdots &\vdots \\Y_{NN}&Y_{N2}&\cdots &Y_{NN}\\\end{pmatrix}}*{\begin
      {pmatrix}V_{1}\\V_{2}\\\vdots \\V_{N}\\\end{pmatrix}}={\begin{pmatrix}I_
      {1}\\I_{2}\\\vdots \\I_{N}\\\end{pmatrix}}}]
To illustrate this process with the admittance matrix of the three bus network
in the figure would be:
         Y =   (     y  1   +  y  12   +  y  13     &#x2212;  y  12
      &#x2212;  y  13       &#x2212;  y  12      y  2   +  y  12   +  y  23
      &#x2212;  y  23       &#x2212;  y  13     &#x2212;  y  23      y  3   +
      y  13   +  y  23      )     {\displaystyle Y={\begin{pmatrix}y_{1}+y_
      {12}+y_{13}&-y_{12}&-y_{13}\\-y_{12}&y_{2}+y_{12}+y_{23}&-y_{23}\\-y_
      {13}&-y_{23}&y_{3}+y_{13}+y_{23}\\\end{pmatrix}}}  [{\displaystyle Y=
      {\begin{pmatrix}y_{1}+y_{12}+y_{13}&-y_{12}&-y_{13}\\-y_{12}&y_{2}+y_
      {12}+y_{23}&-y_{23}\\-y_{13}&-y_{23}&y_{3}+y_{13}+y_{23}\\\end
      {pmatrix}}}]
The Y Matrix diagonal elements      Y  11   ,  Y  22   , . . . ,  Y  n n
{\displaystyle Y_{11},Y_{22},...,Y_{nn}}  [Y_{{11}},Y_{{22}},...,Y_{{nn}}] are
called the self-admittances at the nodes, and each equals the sum of all the
admittances terminating on the node identified by the repeated subscripts. The
other admittances are the mutual admittances of the nodes, and each equals the
negative of the sum of all admittances connected directly between the nodes
identified by the double subscripts. The admittance matrix     Y
{\displaystyle Y}  [Y] is typically a symmetric_matrix as      y  m n   =  y  n
m     {\displaystyle y_{mn}=y_{nm}}  [y_{mn} = y_{nm}]. However, extensions of
the line model and models of other components such as transformers may make
Y   {\displaystyle Y}  [Y] asymmetrical.[2]
For small transmission systems of about less than 10 nodes or buses, the Y
matrix can be calculated manually. But for a realistic system with relatively
large number of nodes or buses, say 1000 nodes, a computer program for
computing Y is more practical to use.
Node Network Courtesy of scialert.net
To help motivate the importance of using a system of equations in matrix form,
see the adjacent figure. Not only does it become impractical to calculate the
current vector     V   {\displaystyle V}  [V] by hand, it becomes necessary to
use computational power to form the admittance matrix itself.

Example:[3]
Two node power flow diagram courtesy of Grainger and Stevenson
To take a look at a generalizable     2 &#x00D7; 2   {\displaystyle 2\times 2}
[2\times2] matrix, consider the figure of the two-node network. By Kirchhoff's
Current_Law, it can be shown that :      (     I  m        I  n      )   =
(    1     1    )   &#x2217;  I  a     {\displaystyle {\begin{pmatrix}I_{m}\\I_
{n}\\\end{pmatrix}}={\begin{pmatrix}1\\1\\\end{pmatrix}}*I_{a}}  [
{\displaystyle {\begin{pmatrix}I_{m}\\I_{n}\\\end{pmatrix}}={\begin
{pmatrix}1\\1\\\end{pmatrix}}*I_{a}}] since there are no other currents
entering or exiting nodes     m   {\displaystyle m}  [m] or     n
{\displaystyle n}  [n]. The voltage drop across the line can be expressed as :
V  a   =   (    1 &#x2217; &#x2212; 1    )   &#x2217;   (     V  m        V  n
)     {\displaystyle V_{a}={\begin{pmatrix}1*-1\\\end{pmatrix}}*{\begin
{pmatrix}V_{m}\\V_{n}\\\end{pmatrix}}}  [{\displaystyle V_{a}={\begin
{pmatrix}1*-1\\\end{pmatrix}}*{\begin{pmatrix}V_{m}\\V_{n}\\\end{pmatrix}}}].
Next, use Ohm's_Law with admittance instead of impedance. Using substitution to
get :      (     Y  a     &#x2212;  Y  a       &#x2212;  Y  a      Y  a      )
&#x2217;   (     V  m        V  n      )   =   (     I  m        I  n      )
{\displaystyle {\begin{pmatrix}Y_{a}&-Y_{a}\\-Y_{a}&Y_{a}\end{pmatrix}}*{\begin
{pmatrix}V_{m}\\V_{n}\\\end{pmatrix}}={\begin{pmatrix}I_{m}\\I_{n}\\\end
{pmatrix}}}  [{\displaystyle {\begin{pmatrix}Y_{a}&-Y_{a}\\-Y_{a}&Y_{a}\end
{pmatrix}}*{\begin{pmatrix}V_{m}\\V_{n}\\\end{pmatrix}}={\begin{pmatrix}I_
{m}\\I_{n}\\\end{pmatrix}}}]. To reintroduce some generality,      Y  11   =  Y
m m   ,  Y  21   =  Y  n m   ,  Y  12   =  Y  m n   ,   {\displaystyle Y_
{11}=Y_{mm},Y_{21}=Y_{nm},Y_{12}=Y_{mn},}  [{\displaystyle Y_{11}=Y_{mm},Y_
{21}=Y_{nm},Y_{12}=Y_{mn},}] and      Y  22   =  Y  n n     {\displaystyle Y_
{22}=Y_{nn}}  [{\displaystyle Y_{22}=Y_{nn}}]. Thus, this example can be taken
as a first step in understanding how to generally construct an     N x N
{\displaystyle NxN}  [{\displaystyle NxN}] matrix by hand.
***** See also[edit] *****
    * Admittance_parameters
    * Zbus
***** References[edit] *****
   1. ^McCalley, James. "The_Power_Flow_Equations" (PDF). Iowa State
      Engineering.
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
   3. ^Grainger, John (1994). Power_System_Analysis. McGraw-Hill Science/
      Engineering/Math. ISBN 978-0070612938.
   4. ^Grainger, John (1994). Power System Analysis (1 ed.). McGraw-Hill
      Science/Engineering/Math. pp. 240â241. ISBN 978-0070612938.
***** External links[edit] *****
    * A_C/C++_Program_and_Source_Code_for_Computing_Ybus_and_Zbus_Matrices

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Nodal_admittance_matrix&oldid=898438700"
Categories:
    * Electrical_engineering
    * Electric_power
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
    * This page was last edited on 23 May 2019, at 15:36 (UTC).
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
