The following text has been accessed from https://en.wikipedia.org/wiki/Indeterminate_form at Fri Aug 9 03:19:01 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Indeterminate form ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (June 2019)(Learn_how_and_when
 to_remove_this_template_message)
In calculus and other branches of mathematical_analysis, limits involving an
algebraic combination of functions in an independent variable may often be
evaluated by replacing these functions by their limits; if the expression
obtained after this substitution does not give enough information to determine
the original limit, it is said to take on an indeterminate form. The term was
originally introduced by Cauchy's student Moigno in the middle of the 19th
century.
The indeterminate forms typically considered in the literature are denoted:
     0 0   , &#xA0;   &#x221E; &#x221E;   , &#xA0; 0 &#x00D7; &#x221E; , &#xA0;
1  &#x221E;   , &#xA0; &#x221E; &#x2212; &#x221E; , &#xA0;  0  0
&#xA0;and&#xA0;   &#x221E;  0   .   {\displaystyle {\frac {0}{0}},~{\frac
{\infty }{\infty }},~0\times \infty ,~1^{\infty },~\infty -\infty ,~0^{0}{\text
{ and }}\infty ^{0}.}  [{\displaystyle {\frac {0}{0}},~{\frac {\infty }{\infty
}},~0\times \infty ,~1^{\infty },~\infty -\infty ,~0^{0}{\text{ and }}\infty ^
{0}.}]
The most common example of an indeterminate form occurs as the ratio of two
functions, in which both of these functions tend to zero in the limit, and is
referred to as "the indeterminate form 0/0". As x approaches 0, the ratios x/
x3, x/x, and x2/x go to â, 1, and 0 respectively. In each case, if the limits
of the numerator and denominator are substituted, the resulting expression is
0/0, which is undefined. So, in a manner of speaking, 0/0 can take on the
values 0, 1, or â, and it is possible to construct similar examples for which
the limit is any particular value.
More formally, when given that the functions f(x) and g(x) both approach 0 as x
approaches some limit_point c one does not have enough information to evaluate
the limit
    lim  x &#x2192; c      f ( x )   g ( x )    .   {\displaystyle \lim _{x\to
c}{\frac {f(x)}{g(x)}}.}  [{\displaystyle \lim _{x\to c}{\frac {f(x)}{g(x)}}.}]
Not every undefined algebraic expression corresponds to an indeterminate form.
For example, the expression 1/0 is undefined as a real_number but does not
correspond to an indeterminate form, because any limit that gives rise to this
form will diverge_to_infinity.
An indeterminate form expression may have a value in some contexts. For
example, if Îº is an infinite cardinal_number, then expressions 0Îº, 00, 1Îº
and Îº0 are well defined in the context of cardinal_arithmetic. See also Zero
to_the_power_of_zero. Note that zero_to_the_power_infinity_is_not_an
indeterminate_form.
⁰
***** Contents *****
    * 1_Some_examples_and_non-examples
          o 1.1_Indeterminate_form_0/0
          o 1.2_Indeterminate_form_00
          o 1.3_Expressions_that_are_not_indeterminate_forms
    * 2_Evaluating_indeterminate_forms
          o 2.1_Equivalent_infinitesimal
          o 2.2_L'HÃ´pital's_rule
    * 3_List_of_indeterminate_forms
    * 4_See_also
    * 5_References
***** Some examples and non-examples[edit] *****
**** Indeterminate form 0/0[edit] ****
    * Fig. 1: y = x/x
    * Fig. 2: y = x2/x
    * Fig. 3: y = sin x/x
    * Fig. 4: y = x − 49/√x − 7
    * Fig. 5: y = ax/x where x = 2
    * Fig. 6: y = x/x3
The indeterminate form 0/0 is particularly common in calculus because it often
arises in the evaluation of derivatives using their limit definition.
As mentioned above,
    lim  x &#x2192; 0     x x   = 1 ,    {\displaystyle \lim _{x\to 0}{\frac
{x}{x}}=1,\qquad }  [{\displaystyle \lim _{x\to 0}{\frac {x}{x}}=1,\qquad }]
(see fig.1)
while
    lim  x &#x2192; 0      x  2   x   = 0 ,    {\displaystyle \lim _{x\to 0}
{\frac {x^{2}}{x}}=0,\qquad }  [{\displaystyle \lim _{x\to 0}{\frac {x^{2}}
{x}}=0,\qquad }] (see fig.2)
This is enough to show that 0/0 is an indeterminate form. Other examples with
this indeterminate form include
    lim  x &#x2192; 0      sin &#x2061; ( x )  x   = 1 ,    {\displaystyle \lim
_{x\to 0}{\frac {\sin(x)}{x}}=1,\qquad }  [{\displaystyle \lim _{x\to 0}{\frac
{\sin(x)}{x}}=1,\qquad }] (see fig.3)
and
    lim  x &#x2192; 49      x &#x2212; 49     x    &#x2212; 7    = 14 ,
{\displaystyle \lim _{x\to 49}{\frac {x-49}{{\sqrt {x}}\,-7}}=14,\qquad }  [
{\displaystyle \lim _{x\to 49}{\frac {x-49}{{\sqrt {x}}\,-7}}=14,\qquad }] (see
fig.4)
Direct substitution of the number that x approaches into any of these
expressions shows that these are examples of the indeterminate form 0/0, but
these limits take many different values. Any desired value a can be obtained
for this indeterminate form as follows:
    lim  x &#x2192; 0      a x  x   = a .    {\displaystyle \lim _{x\to 0}
{\frac {ax}{x}}=a.\qquad }  [{\displaystyle \lim _{x\to 0}{\frac {ax}
{x}}=a.\qquad }] (see fig.5)
The value infinity can also be obtained (in the sense of divergence to
infinity):
    lim  x &#x2192; 0     x  x  3     = &#x221E; .    {\displaystyle \lim _
{x\to 0}{\frac {x}{x^{3}}}=\infty .\qquad }  [{\displaystyle \lim _{x\to 0}
{\frac {x}{x^{3}}}=\infty .\qquad }] (see fig.6)
**** Indeterminate form 00[edit] ****
Main article: Zero_to_the_power_of_zero
    * Fig. 7: y = x0
    * Fig. 8: y = 0x
The following limits illustrate that the expression 00 is an indeterminate
form:
    lim  x &#x2192;  0  +      x  0   = 1 ,    {\displaystyle \lim _{x\to 0^
{+}}x^{0}=1,\qquad }  [{\displaystyle \lim _{x\to 0^{+}}x^{0}=1,\qquad }] (see
fig.7)
    lim  x &#x2192;  0  +      0  x   = 0.    {\displaystyle \lim _{x\to 0^
{+}}0^{x}=0.\qquad }  [{\displaystyle \lim _{x\to 0^{+}}0^{x}=0.\qquad }] (see
fig.8)
Thus, in general, knowing that       lim  x &#x2192; c   f ( x )  =  0
{\displaystyle \textstyle \lim _{x\to c}f(x)\;=\;0\!}  [{\displaystyle
\textstyle \lim _{x\to c}f(x)\;=\;0\!}] and       lim  x &#x2192; c   g ( x )
=  0    {\displaystyle \textstyle \lim _{x\to c}g(x)\;=\;0}  [{\displaystyle
\textstyle \lim _{x\to c}g(x)\;=\;0}] is not sufficient to calculate the limit
    lim  x &#x2192; c   f ( x  )  g ( x )   .   {\displaystyle \lim _{x\to c}f
(x)^{g(x)}.}  [\lim_{x \to c} f(x)^{g(x)} .]
If the functions f and g are analytic at c, and f is positive for x
sufficiently close (but not equal) to c, then the limit of f(x) g(x) will be 1.
[1] Otherwise, use the transformation in the table below to evaluate the limit.
**** Expressions that are not indeterminate forms[edit] ****
The expression 1/0 is not commonly regarded as an indeterminate form because
there is not an infinite range of values that f/g could approach. Specifically,
if f approaches 1 and g approaches 0, then f and g may be chosen so that (1) f/
g approaches +â, (2) f/g approaches ââ, or (3) the limit fails to exist.
In each case the absolute value |f/g| approaches +â, and so the quotient f/
g must diverge, in the sense of the extended_real_numbers. (In the framework of
the projectively_extended_real_line, the limit is the unsigned_infinity â in
all three cases.) Similarly, any expression of the form a/0, with a â  0
(including a = +â and a = ââ), is not an indeterminate form since a
quotient giving rise to such an expression will always diverge.
The expression 0â is not an indeterminate form. The expression 0+â has the
limiting value 0 for the given individual limits, and the expression 0ââ is
equivalent to 1/0.
To see this, let     L =  lim  x &#x2192; c   f ( x  )  g ( x )   ,
{\displaystyle L=\lim _{x\to c}f(x)^{g(x)},}  [{\displaystyle L=\lim _{x\to c}f
(x)^{g(x)},}] where      lim  x &#x2192; c    f ( x )  = 0 ,   {\displaystyle
\lim _{x\to c}{f(x)}=0,}  [{\displaystyle \lim _{x\to c}{f(x)}=0,}] and
lim  x &#x2192; c    g ( x )  = &#x221E; .   {\displaystyle \lim _{x\to c}{g
(x)}=\infty .}  [{\displaystyle \lim _{x\to c}{g(x)}=\infty .}] Take the
natural logarithm of both sides:     ln &#x2061; L =  lim  x &#x2192; c   (  g
( x )  &#x00D7; ln &#x2061;  f ( x )  ) = &#x221E; &#x00D7;  &#x2212; &#x221E;
,   {\displaystyle \ln L=\lim _{x\to c}({g(x)}\times \ln {f(x)})=\infty \times
{-\infty },}  [{\displaystyle \ln L=\lim _{x\to c}({g(x)}\times \ln {f
(x)})=\infty \times {-\infty },}] and     L =   e   &#x2212; &#x221E;   = 0.
{\displaystyle L={e}^{-\infty }=0.}  [{\displaystyle L={e}^{-\infty }=0.}]
***** Evaluating indeterminate forms[edit] *****
The adjective indeterminate does not imply that the limit does not exist, as
many of the examples above show. In many cases, algebraic elimination,
L'HÃ´pital's_rule, or other methods can be used to manipulate the expression so
that the limit can be evaluated.
For example, the expression x2/x can be simplified to x at any point other than
x = 0. Thus, the limit of this expression as x approaches 0 (which depends only
on points near 0, not at x = 0 itself) is the limit of x, which is 0. Most of
the other examples above can also be evaluated using algebraic simplification.
**** Equivalent infinitesimal[edit] ****
When two variables     &#x03B1;   {\displaystyle \alpha }  [\alpha ] and
&#x03B2;   {\displaystyle \beta }  [\beta ] converge to zero at the same point
and     lim   &#x03B2; &#x03B1;   = 1   {\displaystyle \lim {\frac {\beta }
{\alpha }}=1}  [\lim {\frac  {\beta }{\alpha }}=1], they are called equivalent
infinitesimal.
Suppose there are two equivalent infinitesimals     &#x03B1; &#x223C;  &#x03B1;
&#x2032;    {\displaystyle \alpha \sim \alpha '}  [\alpha \sim \alpha '] and
&#x03B2; &#x223C;  &#x03B2; &#x2032;    {\displaystyle \beta \sim \beta '}
[\beta \sim \beta ']. Then
   lim   &#x03B2; &#x03B1;   = lim    &#x03B2; &#x2032;   &#x03B1; &#x2032;
{\displaystyle \lim {\frac {\beta }{\alpha }}=\lim {\frac {\beta '}{\alpha '}}}
[{\displaystyle \lim {\frac {\beta }{\alpha }}=\lim {\frac {\beta '}{\alpha
'}}}]
For the evaluation of the indeterminate form 0/0, we can use the following
equivalent infinitesimals:[2]
   x &#x223C; sin &#x2061; x ,   {\displaystyle x\sim \sin x,}  [x\sim \sin x,]
   x &#x223C; arcsin &#x2061; x ,   {\displaystyle x\sim \arcsin x,}  [x\sim
\arcsin x,]
   x &#x223C; sinh &#x2061; x ,   {\displaystyle x\sim \sinh x,}  [
{\displaystyle x\sim \sinh x,}]
   x &#x223C; tan &#x2061; x ,   {\displaystyle x\sim \tan x,}  [x\sim \tan x,]
   x &#x223C; arctan &#x2061; x ,   {\displaystyle x\sim \arctan x,}  [x\sim
\arctan x,]
   x &#x223C; ln &#x2061; ( 1 + x ) ,   {\displaystyle x\sim \ln(1+x),}  [x\sim
\ln(1+x),]
   1 &#x2212; cos &#x2061; x &#x223C;    x  2   2   ,   {\displaystyle 1-\cos
x\sim {\frac {x^{2}}{2}},}  [{\displaystyle 1-\cos x\sim {\frac {x^{2}}{2}},}]
   cosh &#x2061; x &#x2212; 1 &#x223C;    x  2   2   ,   {\displaystyle \cosh
x-1\sim {\frac {x^{2}}{2}},}  [{\displaystyle \cosh x-1\sim {\frac {x^{2}}
{2}},}]
    a  x   &#x2212; 1 &#x223C; x ln &#x2061; a ,   {\displaystyle a^{x}-1\sim
x\ln a,}  [a^{x}-1\sim x\ln a,]
    e  x   &#x2212; 1 &#x223C; x ,   {\displaystyle e^{x}-1\sim x,}  [
{\displaystyle e^{x}-1\sim x,}]
   ( 1 + x  )  a   &#x2212; 1 &#x223C; a x .   {\displaystyle (1+x)^{a}-1\sim
ax.}  [(1+x)^{a}-1\sim ax.]
For example:
    lim  x &#x2192; 0     1  x  3      [    (    2 + cos &#x2061; x  3   )   x
&#x2212; 1  ]  =  lim  x &#x2192; 0       e  x ln &#x2061;    2 + cos &#x2061;
x  3     &#x2212; 1   x  3     =  lim  x &#x2192; 0     1  x  2     ln &#x2061;
2 + cos &#x2061; x  3   =  lim  x &#x2192; 0     1  x  2     ln &#x2061;
(     cos &#x2061; x &#x2212; 1  3   + 1  )  =  lim  x &#x2192; 0      cos
&#x2061; x &#x2212; 1   3  x  2      = &#x2212;   1 6     {\displaystyle \lim _
{x\to 0}{\frac {1}{x^{3}}}\left[\left({\frac {2+\cos x}{3}}\right)^{x}-
1\right]=\lim _{x\to 0}{\frac {e^{x\ln {\frac {2+\cos x}{3}}}-1}{x^{3}}}=\lim _
{x\to 0}{\frac {1}{x^{2}}}\ln {\frac {2+\cos x}{3}}=\lim _{x\to 0}{\frac {1}{x^
{2}}}\ln \left({\frac {\cos x-1}{3}}+1\right)=\lim _{x\to 0}{\frac {\cos x-1}
{3x^{2}}}=-{\frac {1}{6}}}  [{\displaystyle \lim _{x\to 0}{\frac {1}{x^
{3}}}\left[\left({\frac {2+\cos x}{3}}\right)^{x}-1\right]=\lim _{x\to 0}{\frac
{e^{x\ln {\frac {2+\cos x}{3}}}-1}{x^{3}}}=\lim _{x\to 0}{\frac {1}{x^{2}}}\ln
{\frac {2+\cos x}{3}}=\lim _{x\to 0}{\frac {1}{x^{2}}}\ln \left({\frac {\cos x-
1}{3}}+1\right)=\lim _{x\to 0}{\frac {\cos x-1}{3x^{2}}}=-{\frac {1}{6}}}]
Here is a brief proof:
Suppose there are two equivalent infinitesimals     &#x03B1; &#x223C;  &#x03B1;
&#x2032;    {\displaystyle \alpha \sim \alpha '}  [\alpha \sim \alpha '] and
&#x03B2; &#x223C;  &#x03B2; &#x2032;    {\displaystyle \beta \sim \beta '}
[\beta \sim \beta '].
   lim   &#x03B2; &#x03B1;   = lim    &#x03B2;  &#x03B2; &#x2032;   &#x03B1;
&#x2032;     &#x03B2; &#x2032;   &#x03B1; &#x2032;  &#x03B1;    = lim
&#x03B2;  &#x03B2; &#x2032;    lim    &#x03B1; &#x2032;  &#x03B1;   lim
&#x03B2; &#x2032;   &#x03B1; &#x2032;    = lim    &#x03B2; &#x2032;   &#x03B1;
&#x2032;      {\displaystyle \lim {\frac {\beta }{\alpha }}=\lim {\frac {\beta
\beta '\alpha '}{\beta '\alpha '\alpha }}=\lim {\frac {\beta }{\beta '}}\lim
{\frac {\alpha '}{\alpha }}\lim {\frac {\beta '}{\alpha '}}=\lim {\frac {\beta
'}{\alpha '}}}  [\lim {\frac  {\beta }{\alpha }}=\lim {\frac  {\beta \beta
'\alpha '}{\beta '\alpha '\alpha }}=\lim {\frac  {\beta }{\beta '}}\lim {\frac
{\alpha '}{\alpha }}\lim {\frac  {\beta '}{\alpha '}}=\lim {\frac  {\beta '}
{\alpha '}}]
**** L'HÃ´pital's rule[edit] ****
Main article: L'HÃ´pital's_rule
L'HÃ´pital's rule is a general method for evaluating the indeterminate forms 0/
0 and â/â. This rule states that (under appropriate conditions)
    lim  x &#x2192; c      f ( x )   g ( x )    =  lim  x &#x2192; c       f
&#x2032;  ( x )    g &#x2032;  ( x )    ,    {\displaystyle \lim _{x\to c}
{\frac {f(x)}{g(x)}}=\lim _{x\to c}{\frac {f'(x)}{g'(x)}},\!}  [ \lim_{x \to c}
\frac{f(x)}{g(x)} = \lim_{x \to c} \frac{f'(x)}{g'(x)} , \! ]
where f' and g' are the derivatives of f and g. (Note that this rule does not
apply to expressions â/0, 1/0, and so on; these expressions are not
indeterminate forms.) These derivatives will allow one to perform algebraic
simplification and eventually evaluate the limit.
L'HÃ´pital's rule can also be applied to other indeterminate forms, using first
an appropriate algebraic transformation. For example, to evaluate the form 00:
   ln &#x2061;  lim  x &#x2192; c   f ( x  )  g ( x )   =  lim  x &#x2192; c
ln &#x2061; f ( x )   1  /  g ( x )    .    {\displaystyle \ln \lim _{x\to c}f
(x)^{g(x)}=\lim _{x\to c}{\frac {\ln f(x)}{1/g(x)}}.\!}  [ \ln \lim_{x \to c} f
(x)^{g(x)} = \lim_{x \to c} \frac{\ln f(x)}{1/g(x)} . \! ]
The right-hand side is of the form â/â, so L'HÃ´pital's rule applies to it.
Note that this equation is valid (as long as the right-hand side is defined)
because the natural_logarithm (ln) is a continuous_function; it is irrelevant
how well-behaved f and g may (or may not) be as long as f is asymptotically
positive.
Although L'HÃ´pital's rule applies both to 0/0 and to â/â, one of these
forms may be more useful than the other in a particular case (because of the
possibility of algebraic simplification afterwards). One can change between
these forms, if necessary, by transforming f/g to (1/g)/(1/f).
***** List of indeterminate forms[edit] *****
The following table lists the most common indeterminate forms and the
transformations for applying l'HÃ´pital's rule.
 _____________________________________________________________________________
|Indeterminate form|Conditions        |Transformation to  |Transformation to  |
|__________________|__________________|0/0________________|â/â______|
|                  |                  |                   |    lim  x &#x2192;|
|                  |    lim  x        |                   |c      f ( x )   g |
|                  |&#x2192; c   f ( x|                   |( x )    =  lim  x |
|                  |) = 0 , &#xA0;    |                   |&#x2192; c      1  |
|                  |lim  x &#x2192; c |                   |/  g ( x )   1  /  |
|                  |g ( x ) = 0       |                   |f ( x )            |
|   0  /  0        |{\displaystyle    |                   |{\displaystyle \lim|
|{\displaystyle 0/ |\lim _{x\to c}f   |         —       |_{x\to c}{\frac {f |
|0}  [0/0]         |(x)=0,\ \lim _    |                   |(x)}{g(x)}}=\lim _ |
|                  |{x\to c}g(x)=0\!} |                   |{x\to c}{\frac {1/g|
|                  |[ \lim_{x \to c} f|                   |(x)}{1/f(x)}}\!}   |
|                  |(x) = 0,\  \lim_{x|                   |[ \lim_{x \to c}   |
|                  |\to c} g(x) = 0 \!|                   |\frac{f(x)}{g(x)} =|
|                  |]                 |                   |\lim_{x \to c}     |
|                  |                  |                   |\frac{1/g(x)}{1/f  |
|__________________|__________________|___________________|(x)}_\!_]__________|
|                  |    lim  x        |    lim  x &#x2192;|                   |
|                  |&#x2192; c   f ( x|c      f ( x )   g |                   |
|                  |) = &#x221E; ,    |( x )    =  lim  x |                   |
|                  |&#xA0;  lim  x    |&#x2192; c      1  |                   |
|                  |&#x2192; c   g ( x|/  g ( x )   1  /  |                   |
|   &#x221E;  /    |) = &#x221E;      |f ( x )            |                   |
|&#x221E;          |{\displaystyle    |{\displaystyle \lim|                   |
|{\displaystyle    |\lim _{x\to c}f   |_{x\to c}{\frac {f |         —       |
|\infty /\infty }  |(x)=\infty ,\ \lim|(x)}{g(x)}}=\lim _ |                   |
|[{\displaystyle   |_{x\to c}g        |{x\to c}{\frac {1/g|                   |
|\infty /\infty }] |(x)=\infty \!}    |(x)}{1/f(x)}}\!}   |                   |
|                  |[ \lim_{x \to c} f|[ \lim_{x \to c}   |                   |
|                  |(x) = \infty,\    |\frac{f(x)}{g(x)} =|                   |
|                  |\lim_{x \to c} g  |\lim_{x \to c}     |                   |
|                  |(x) = \infty \! ] |\frac{1/g(x)}{1/f  |                   |
|__________________|__________________|(x)}_\!_]__________|___________________|
|                  |    lim  x        |    lim  x &#x2192;|    lim  x &#x2192;|
|                  |&#x2192; c   f ( x|c   f ( x ) g ( x )|c   f ( x ) g ( x )|
|                  |) = 0 , &#xA0;    |=  lim  x &#x2192; |=  lim  x &#x2192; |
|                  |lim  x &#x2192; c |c      f ( x )   1 |c      g ( x )   1 |
|   0 &#x22C5;     |g ( x ) = &#x221E;|/  g ( x )         |/  f ( x )         |
|&#x221E;          |{\displaystyle    |{\displaystyle \lim|{\displaystyle \lim|
|{\displaystyle    |\lim _{x\to c}f   |_{x\to c}f(x)g     |_{x\to c}f(x)g     |
|0\cdot \infty }   |(x)=0,\ \lim _    |(x)=\lim _{x\to c} |(x)=\lim _{x\to c} |
|[0\cdot \infty ]  |{x\to c}g         |{\frac {f(x)}{1/g  |{\frac {g(x)}{1/f  |
|                  |(x)=\infty \!}    |(x)}}\!}  [ \lim_{x|(x)}}\!}  [ \lim_{x|
|                  |[ \lim_{x \to c} f|\to c} f(x)g(x) =  |\to c} f(x)g(x) =  |
|                  |(x) = 0,\  \lim_{x|\lim_{x \to c}     |\lim_{x \to c}     |
|                  |\to c} g(x) =     |\frac{f(x)}{1/g(x)}|\frac{g(x)}{1/f(x)}|
|__________________|\infty_\!_]_______|\!_]_______________|\!_]_______________|
|                  |                  |    lim  x &#x2192;|    lim  x &#x2192;|
|                  |                  |c   ( f ( x )      |c   ( f ( x )      |
|                  |    lim  x        |&#x2212; g ( x ) ) |&#x2212; g ( x ) ) |
|                  |&#x2192; c   f ( x|=  lim  x &#x2192; |= ln &#x2061;  lim |
|                  |) = &#x221E; ,    |c      1  /  g ( x |x &#x2192; c      e|
|                  |&#xA0;  lim  x    |) &#x2212; 1  /  f |f ( x )    e  g ( x|
|                  |&#x2192; c   g ( x|( x )   1  /  ( f  |)                  |
|   &#x221E;       |) = &#x221E;      |( x ) g ( x ) )    |{\displaystyle \lim|
|&#x2212; &#x221E; |{\displaystyle    |{\displaystyle \lim|_{x\to c}(f(x)-g   |
|{\displaystyle    |\lim _{x\to c}f   |_{x\to c}(f(x)-g   |(x))=\ln \lim _    |
|\infty -\infty }  |(x)=\infty ,\ \lim|(x))=\lim _{x\to c}|{x\to c}{\frac {e^ |
|[\infty -\infty ] |_{x\to c}g        |{\frac {1/g(x)-1/f |{f(x)}}{e^{g       |
|                  |(x)=\infty \!}    |(x)}{1/(f(x)g      |(x)}}}\!}  [ \lim_ |
|                  |[ \lim_{x \to c} f|(x))}}\!}  [ \lim_ |{x \to c} (f(x) - g|
|                  |(x) = \infty,\    |{x \to c} (f(x) - g|(x)) = \ln \lim_{x |
|                  |\lim_{x \to c} g  |(x)) = \lim_{x \to |\to c} \frac{e^{f  |
|                  |(x) = \infty \! ] |c} \frac{1/g(x) -  |(x)}}{e^{g(x)}} \! |
|                  |                  |1/f(x)}{1/(f(x)g   |]                  |
|__________________|__________________|(x))}_\!_]_________|___________________|
|                  |                  |    lim  x &#x2192;|    lim  x &#x2192;|
|                  |    lim  x        |c   f ( x  )  g ( x|c   f ( x  )  g ( x|
|                  |&#x2192; c   f ( x|)   = exp &#x2061; |)   = exp &#x2061; |
|                  |) =  0  +   ,  lim|lim  x &#x2192; c  |lim  x &#x2192; c  |
|                  |x &#x2192; c   g  |g ( x )   1  /  ln |ln &#x2061; f ( x )|
|                  |( x ) = 0         |&#x2061; f ( x )   |1  /  g ( x )      |
|    0  0          |{\displaystyle    |{\displaystyle \lim|{\displaystyle \lim|
|{\displaystyle 0^ |\lim _{x\to c}f   |_{x\to c}f(x)^{g   |_{x\to c}f(x)^{g   |
|{0}}  [0^{0}]     |(x)=0^{+},\lim _  |(x)}=\exp \lim _   |(x)}=\exp \lim _   |
|                  |{x\to c}g(x)=0\!} |{x\to c}{\frac {g  |{x\to c}{\frac {\ln|
|                  |[ \lim_{x \to c} f|(x)}{1/\ln f       |f(x)}{1/g(x)}}\!}  |
|                  |(x) = 0^+, \lim_{x|(x)}}\!}  [ \lim_{x|[ \lim_{x \to c} f |
|                  |\to c} g(x) = 0 \!|\to c} f(x)^{g(x)} |(x)^{g(x)} = \exp  |
|                  |]                 |= \exp \lim_{x \to |\lim_{x \to c}     |
|                  |                  |c} \frac{g(x)}{1/  |\frac{\ln f(x)}{1/g|
|__________________|__________________|\ln_f(x)}_\!_]_____|(x)}_\!_]__________|
|                  |                  |    lim  x &#x2192;|    lim  x &#x2192;|
|                  |    lim  x        |c   f ( x  )  g ( x|c   f ( x  )  g ( x|
|                  |&#x2192; c   f ( x|)   = exp &#x2061; |)   = exp &#x2061; |
|                  |) = 1 , &#xA0;    |lim  x &#x2192; c  |lim  x &#x2192; c  |
|                  |lim  x &#x2192; c |ln &#x2061; f ( x )|g ( x )   1  /  ln |
|                  |g ( x ) = &#x221E;|1  /  g ( x )      |&#x2061; f ( x )   |
|    1  &#x221E;   |{\displaystyle    |{\displaystyle \lim|{\displaystyle \lim|
|{\displaystyle 1^ |\lim _{x\to c}f   |_{x\to c}f(x)^{g   |_{x\to c}f(x)^{g   |
|{\infty }}  [1^   |(x)=1,\ \lim _    |(x)}=\exp \lim _   |(x)}=\exp \lim _   |
|{\infty }]        |{x\to c}g         |{x\to c}{\frac {\ln|{x\to c}{\frac {g  |
|                  |(x)=\infty \!}    |f(x)}{1/g(x)}}\!}  |(x)}{1/\ln f       |
|                  |[ \lim_{x \to c} f|[ \lim_{x \to c} f |(x)}}\!}  [ \lim_{x|
|                  |(x) = 1,\  \lim_{x|(x)^{g(x)} = \exp  |\to c} f(x)^{g(x)} |
|                  |\to c} g(x) =     |\lim_{x \to c}     |= \exp \lim_{x \to |
|                  |\infty \! ]       |\frac{\ln f(x)}{1/g|c} \frac{g(x)}{1/  |
|__________________|__________________|(x)}_\!_]__________|\ln_f(x)}_\!_]_____|
|                  |                  |    lim  x &#x2192;|    lim  x &#x2192;|
|                  |    lim  x        |c   f ( x  )  g ( x|c   f ( x  )  g ( x|
|                  |&#x2192; c   f ( x|)   = exp &#x2061; |)   = exp &#x2061; |
|                  |) = &#x221E; ,    |lim  x &#x2192; c  |lim  x &#x2192; c  |
|                  |&#xA0;  lim  x    |g ( x )   1  /  ln |ln &#x2061; f ( x )|
|    &#x221E;  0   |&#x2192; c   g ( x|&#x2061; f ( x )   |1  /  g ( x )      |
|{\displaystyle    |) = 0             |{\displaystyle \lim|{\displaystyle \lim|
|\infty ^{0}}  [   |{\displaystyle    |_{x\to c}f(x)^{g   |_{x\to c}f(x)^{g   |
|{\displaystyle    |\lim _{x\to c}f   |(x)}=\exp \lim _   |(x)}=\exp \lim _   |
|\infty ^{0}}]     |(x)=\infty ,\ \lim|{x\to c}{\frac {g  |{x\to c}{\frac {\ln|
|                  |_{x\to c}g(x)=0\!}|(x)}{1/\ln f       |f(x)}{1/g(x)}}\!}  |
|                  |[ \lim_{x \to c} f|(x)}}\!}  [ \lim_{x|[ \lim_{x \to c} f |
|                  |(x) = \infty,\    |\to c} f(x)^{g(x)} |(x)^{g(x)} = \exp  |
|                  |\lim_{x \to c} g  |= \exp \lim_{x \to |\lim_{x \to c}     |
|                  |(x) = 0 \! ]      |c} \frac{g(x)}{1/  |\frac{\ln f(x)}{1/g|
|__________________|__________________|\ln_f(x)}_\!_]_____|(x)}_\!_]__________|
***** See also[edit] *****
    * Defined_and_undefined
    * Division_by_zero
    * Extended_real_number_line
    * L'HÃ´pital's_rule
***** References[edit] *****
   1. ^Louis M. Rotando; Henry Korn (January 1977). "The indeterminate form
      00". Mathematics Magazine. 50 (1): 41â42. doi:10.2307/2689754.
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
   3. ^"Table_of_equivalent_infinitesimals" (PDF). Vaxa Software.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Indeterminate_form&oldid=904898176"
Categories:
    * Limits_(mathematics)
Hidden categories:
    * Articles_lacking_in-text_citations_from_June_2019
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
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * CatalÃ 
    * Deutsch
    * EspaÃ±ol
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Italiano
    * Polski
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 5 July 2019, at 11:11 (UTC).
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
