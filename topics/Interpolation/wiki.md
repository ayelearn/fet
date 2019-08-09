The following text has been accessed from https://en.wikipedia.org/wiki/Interpolation at Fri Aug 9 02:34:42 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Interpolation ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other uses, see Interpolation_(disambiguation).
 This article includes a list_of_references, but its sources remain unclear
 because it has insufficient inline_citations. Please help to improve this
 article by introducing more precise citations. (October 2016)(Learn_how_and
 when_to_remove_this_template_message)
In the mathematical field of numerical_analysis, interpolation is a method of
constructing new data_points within the range of a discrete_set of known data
points.
In engineering and science, one often has a number of data points, obtained by
sampling or experimentation, which represent the values of a function for a
limited number of values of the independent_variable. It is often required to
interpolate, i.e., estimate the value of that function for an intermediate
value of the independent variable.
A closely related problem is the approximation of a complicated function by a
simple function. Suppose the formula for some given function is known, but too
complicated to evaluate efficiently. A few data points from the original
function can be interpolated to produce a simpler function which is still
fairly close to the original. The resulting gain in simplicity may outweigh the
loss from interpolation error.
An interpolation of a finite set of points on an epitrochoid. The points in red
are connected by blue interpolated spline_curves deduced only from the red
points. The interpolated curves have polynomial formulas much simpler than that
of the original epitrochoid curve.
⁰
***** Contents *****
    * 1_Example
          o 1.1_Piecewise_constant_interpolation
          o 1.2_Linear_interpolation
          o 1.3_Polynomial_interpolation
          o 1.4_Spline_interpolation
    * 2_Function_approximation
    * 3_Via_Gaussian_processes
    * 4_Other_forms
    * 5_In_higher_dimensions
    * 6_In_digital_signal_processing
    * 7_Related_concepts
    * 8_Generalization
    * 9_See_also
    * 10_References
    * 11_External_links
***** Example[edit] *****
This table gives some values of an unknown function     f ( x )
{\displaystyle f(x)}  [f(x)].
Plot of the data points as given in the table.
 x     f(x)
 0   0
 1   0 . 8415
 2   0 . 9093
 3   0 . 1411
 4  −. 7568
 5  −. 9589
 6  −. 2794
Interpolation provides a means of estimating the function at intermediate
points, such as     x = 2.5   {\displaystyle x=2.5}  [x=2.5].
We describe some methods of interpolation, differing in such properties as:
accuracy, cost, number of data points needed, and smoothness of the resulting
interpolant function.
**** Piecewise constant interpolation[edit] ****
Piecewise constant interpolation, or nearest-neighbor_interpolation.
Further information: Nearest-neighbor_interpolation
The simplest interpolation method is to locate the nearest data value, and
assign the same value. In simple problems, this method is unlikely to be used,
as linear interpolation (see below) is almost as easy, but in higher-
dimensional multivariate_interpolation, this could be a favourable choice for
its speed and simplicity.
**** Linear interpolation[edit] ****
Plot of the data with linear interpolation superimposed
Main article: Linear_interpolation
One of the simplest methods is linear interpolation (sometimes known as lerp).
Consider the above example of estimating f(2.5). Since 2.5 is midway between 2
and 3, it is reasonable to take f(2.5) midway between f(2) = 0.9093 and f(3) =
0.1411, which yields 0.5252.
Generally, linear interpolation takes two data points, say (xa,ya) and (xb,yb),
and the interpolant is given by:
         y =  y  a   +  (   y  b   &#x2212;  y  a    )     x &#x2212;  x  a
      x  b   &#x2212;  x  a       &#xA0;at the point&#xA0;   (  x , y  )
      {\displaystyle y=y_{a}+\left(y_{b}-y_{a}\right){\frac {x-x_{a}}{x_{b}-x_
      {a}}}{\text{ at the point }}\left(x,y\right)}  [y=y_{a}+\left(y_{b}-y_
      {a}\right){\frac {x-x_{a}}{x_{b}-x_{a}}}{\text{ at the point }}\left
      (x,y\right)]

            y &#x2212;  y  a      y  b   &#x2212;  y  a      =    x &#x2212;  x
      a      x  b   &#x2212;  x  a        {\displaystyle {\frac {y-y_{a}}{y_
      {b}-y_{a}}}={\frac {x-x_{a}}{x_{b}-x_{a}}}}  [{\frac {y-y_{a}}{y_{b}-y_
      {a}}}={\frac {x-x_{a}}{x_{b}-x_{a}}}]

            y &#x2212;  y  a     x &#x2212;  x  a      =     y  b   &#x2212;  y
      a      x  b   &#x2212;  x  a        {\displaystyle {\frac {y-y_{a}}{x-x_
      {a}}}={\frac {y_{b}-y_{a}}{x_{b}-x_{a}}}}  [{\frac {y-y_{a}}{x-x_{a}}}=
      {\frac {y_{b}-y_{a}}{x_{b}-x_{a}}}]

This previous equation states that the slope of the new line between     (  x
a   ,  y  a   )   {\displaystyle (x_{a},y_{a})}  [(x_{a},y_{a})] and     ( x ,
y )   {\displaystyle (x,y)}  [(x,y)] is the same as the slope of the line
between     (  x  a   ,  y  a   )   {\displaystyle (x_{a},y_{a})}  [(x_{a},y_
{a})] and     (  x  b   ,  y  b   )   {\displaystyle (x_{b},y_{b})}  [(x_{b},y_
{b})]
Linear interpolation is quick and easy, but it is not very precise. Another
disadvantage is that the interpolant is not differentiable at the point xk.
The following error estimate shows that linear interpolation is not very
precise. Denote the function which we want to interpolate by g, and suppose
that x lies between xa and xb and that g is twice continuously differentiable.
Then the linear interpolation error is
          |  f ( x ) &#x2212; g ( x )  |  &#x2264; C (  x  b   &#x2212;  x  a
      )  2     where   C =   1 8    max  r &#x2208; [  x  a   ,  x  b   ]    |
      g &#x2033;  ( r )  |  .   {\displaystyle |f(x)-g(x)|\leq C(x_{b}-x_{a})^
      {2}\quad {\text{where}}\quad C={\frac {1}{8}}\max _{r\in [x_{a},x_
      {b}]}|g''(r)|.}  [|f(x)-g(x)|\leq C(x_{b}-x_{a})^{2}\quad {\text
      {where}}\quad C={\frac {1}{8}}\max _{r\in [x_{a},x_{b}]}|g''(r)|.]
In words, the error is proportional to the square of the distance between the
data points. The error in some other methods, including polynomial
interpolation and spline interpolation (described below), is proportional to
higher powers of the distance between the data points. These methods also
produce smoother interpolants.
**** Polynomial interpolation[edit] ****
Plot of the data with polynomial interpolation applied
Main article: Polynomial_interpolation
Polynomial interpolation is a generalization of linear interpolation. Note that
the linear interpolant is a linear_function. We now replace this interpolant
with a polynomial of higher degree.
Consider again the problem given above. The following sixth degree polynomial
goes through all the seven points:
         f ( x ) = &#x2212; 0.0001521  x  6   &#x2212; 0.003130  x  5   +
      0.07321  x  4   &#x2212; 0.3577  x  3   + 0.2255  x  2   + 0.9038 x .
      {\displaystyle f(x)=-0.0001521x^{6}-0.003130x^{5}+0.07321x^{4}-0.3577x^
      {3}+0.2255x^{2}+0.9038x.}  [f(x)=-0.0001521x^{6}-0.003130x^{5}+0.07321x^
      {4}-0.3577x^{3}+0.2255x^{2}+0.9038x.]
Substituting x = 2.5, we find that f(2.5) = 0.5965.
Generally, if we have n data points, there is exactly one polynomial of degree
at most n−1 going through all the data points. The interpolation error is
proportional to the distance between the data points to the power n.
Furthermore, the interpolant is a polynomial and thus infinitely
differentiable. So, we see that polynomial interpolation overcomes most of the
problems of linear interpolation.
However, polynomial interpolation also has some disadvantages. Calculating the
interpolating polynomial is computationally expensive (see computational
complexity) compared to linear interpolation. Furthermore, polynomial
interpolation may exhibit oscillatory artifacts, especially at the end points
(see Runge's_phenomenon).
Polynomial interpolation can estimate local maxima and minima that are outside
the range of the samples, unlike linear interpolation. For example, the
interpolant above has a local maximum at x â 1.566, f(x) â 1.003 and a
local minimum at x â 4.708, f(x) â â1.003. However, these maxima and
minima may exceed the theoretical range of the functionâfor example, a
function that is always positive may have an interpolant with negative values,
and whose inverse therefore contains false vertical_asymptotes.
More generally, the shape of the resulting curve, especially for very high or
low values of the independent variable, may be contrary to commonsense, i.e. to
what is known about the experimental system which has generated the data
points. These disadvantages can be reduced by using spline interpolation or
restricting attention to Chebyshev_polynomials.
**** Spline interpolation[edit] ****
Plot of the data with spline interpolation applied
Main article: Spline_interpolation
Remember that linear interpolation uses a linear function for each of intervals
[xk,xk+1]. Spline interpolation uses low-degree polynomials in each of the
intervals, and chooses the polynomial pieces such that they fit smoothly
together. The resulting function is called a spline.
For instance, the natural_cubic_spline is piecewise cubic and twice
continuously differentiable. Furthermore, its second derivative is zero at the
end points. The natural cubic spline interpolating the points in the table
above is given by
         f ( x ) =   {    &#x2212; 0.1522  x  3   + 0.9937 x ,    if&#xA0;  x
      &#x2208; [ 0 , 1 ] ,     &#x2212; 0.01258  x  3   &#x2212; 0.4189  x  2
      + 1.4126 x &#x2212; 0.1396 ,    if&#xA0;  x &#x2208; [ 1 , 2 ] ,
      0.1403  x  3   &#x2212; 1.3359  x  2   + 3.2467 x &#x2212; 1.3623 ,
      if&#xA0;  x &#x2208; [ 2 , 3 ] ,     0.1579  x  3   &#x2212; 1.4945  x  2
      + 3.7225 x &#x2212; 1.8381 ,    if&#xA0;  x &#x2208; [ 3 , 4 ] ,
      0.05375  x  3   &#x2212; 0.2450  x  2   &#x2212; 1.2756 x + 4.8259 ,
      if&#xA0;  x &#x2208; [ 4 , 5 ] ,     &#x2212; 0.1871  x  3   + 3.3673  x
      2   &#x2212; 19.3370 x + 34.9282 ,    if&#xA0;  x &#x2208; [ 5 , 6 ] .
      {\displaystyle f(x)={\begin{cases}-0.1522x^{3}+0.9937x,&{\text{if }}x\in
      [0,1],\\-0.01258x^{3}-0.4189x^{2}+1.4126x-0.1396,&{\text{if }}x\in
      [1,2],\\0.1403x^{3}-1.3359x^{2}+3.2467x-1.3623,&{\text{if }}x\in
      [2,3],\\0.1579x^{3}-1.4945x^{2}+3.7225x-1.8381,&{\text{if }}x\in
      [3,4],\\0.05375x^{3}-0.2450x^{2}-1.2756x+4.8259,&{\text{if }}x\in
      [4,5],\\-0.1871x^{3}+3.3673x^{2}-19.3370x+34.9282,&{\text{if }}x\in
      [5,6].\end{cases}}}  [f(x)={\begin{cases}-0.1522x^{3}+0.9937x,&{\text{if
      }}x\in [0,1],\\-0.01258x^{3}-0.4189x^{2}+1.4126x-0.1396,&{\text{if }}x\in
      [1,2],\\0.1403x^{3}-1.3359x^{2}+3.2467x-1.3623,&{\text{if }}x\in
      [2,3],\\0.1579x^{3}-1.4945x^{2}+3.7225x-1.8381,&{\text{if }}x\in
      [3,4],\\0.05375x^{3}-0.2450x^{2}-1.2756x+4.8259,&{\text{if }}x\in
      [4,5],\\-0.1871x^{3}+3.3673x^{2}-19.3370x+34.9282,&{\text{if }}x\in
      [5,6].\end{cases}}]
In this case we get f(2.5) = 0.5972.
Like polynomial interpolation, spline interpolation incurs a smaller error than
linear interpolation and the interpolant is smoother. However, the interpolant
is easier to evaluate than the high-degree polynomials used in polynomial
interpolation. However, the global nature of the basis functions leads to ill-
conditioning. This is completely mitigated by using splines of compact support,
such as are implemented in Boost.Math and discussed in Kress.[1]
***** Function approximation[edit] *****
Interpolation is a common way to approximate functions. Given a function     f
: [ a , b ] &#x2192;  R    {\displaystyle f:[a,b]\to \mathbb {R} }  [
{\displaystyle f:[a,b]\to \mathbb {R} }] with a set of points      x  1   ,  x
2   , &#x2026; ,  x  n   &#x2208; [ a , b ]   {\displaystyle x_{1},x_{2},\dots
,x_{n}\in [a,b]}  [{\displaystyle x_{1},x_{2},\dots ,x_{n}\in [a,b]}] one can
form a function     s : [ a , b ] &#x2192;  R    {\displaystyle s:[a,b]\to
\mathbb {R} }  [{\displaystyle s:[a,b]\to \mathbb {R} }] such that     f (  x
i   ) = s (  x  i   )   {\displaystyle f(x_{i})=s(x_{i})}  [{\displaystyle f(x_
{i})=s(x_{i})}] for     i = 1 , 2 , &#x2026; , n   {\displaystyle i=1,2,\dots
,n}  [{\displaystyle i=1,2,\dots ,n}] (that is that     s   {\displaystyle s}
[s] interpolates     f   {\displaystyle f}  [f] at these points). In general,
an interpolant need not be a good approximation, but there are well known and
often reasonable conditions where it will. For example, if     f &#x2208;  C  4
( [ a , b ] )   {\displaystyle f\in C^{4}([a,b])}  [{\displaystyle f\in C^{4}(
[a,b])}] (four times continuously differentiable) then cubic_spline
interpolation has an error bound given by     &#x2016; f &#x2212; s  &#x2016;
&#x221E;   &#x2264; C &#x2016;  f  ( 4 )    &#x2016;  &#x221E;    h  4
{\displaystyle \|f-s\|_{\infty }\leq C\|f^{(4)}\|_{\infty }h^{4}}  [
{\displaystyle \|f-s\|_{\infty }\leq C\|f^{(4)}\|_{\infty }h^{4}}] where     h
max  i = 1 , 2 , &#x2026; , n &#x2212; 1    |   x  i + 1   &#x2212;  x  i    |
{\displaystyle h\max _{i=1,2,\dots ,n-1}|x_{i+1}-x_{i}|}  [{\displaystyle h\max
_{i=1,2,\dots ,n-1}|x_{i+1}-x_{i}|}] and     C   {\displaystyle C}  [C] is a
constant.[2]
***** Via Gaussian processes[edit] *****
Gaussian_process is a powerful non-linear interpolation tool. Many popular
interpolation tools are actually equivalent to particular Gaussian processes.
Gaussian processes can be used not only for fitting an interpolant that passes
exactly through the given data points but also for regression, i.e., for
fitting a curve through noisy data. In the geostatistics community Gaussian
process regression is also known as Kriging.
***** Other forms[edit] *****
Other forms of interpolation can be constructed by picking a different class of
interpolants. For instance, rational interpolation is interpolation by rational
functions using PadÃ©_approximant, and trigonometric_interpolation is
interpolation by trigonometric_polynomials using Fourier_series. Another
possibility is to use wavelets.
The WhittakerâShannon_interpolation_formula can be used if the number of data
points is infinite.
Sometimes, we know not only the value of the function that we want to
interpolate, at some points, but also its derivative. This leads to Hermite
interpolation problems.
When each data point is itself a function, it can be useful to see the
interpolation problem as a partial advection problem between each data point.
This idea leads to the displacement_interpolation problem used in
transportation_theory.
***** In higher dimensions[edit] *****
Comparison of some 1- and 2-dimensional interpolations. Black and red/yellow/
green/blue dots correspond to the interpolated point and neighbouring samples,
respectively. Their heights above the ground correspond to their values.
Main article: Multivariate_interpolation
Multivariate interpolation is the interpolation of functions of more than one
variable. Methods include bilinear_interpolation and bicubic_interpolation in
two dimensions, and trilinear_interpolation in three dimensions. They can be
applied to gridded or scattered data.
    * Nearest neighbor
    * Bilinear
    * Bicubic
***** In digital signal processing[edit] *****
In the domain of digital signal processing, the term interpolation refers to
the process of converting a sampled digital signal (such as a sampled audio
signal) to that of a higher sampling rate (Upsampling) using various digital
filtering techniques (e.g., convolution with a frequency-limited impulse
signal). In this application there is a specific requirement that the harmonic
content of the original signal be preserved without creating aliased harmonic
content of the original signal above the original Nyquist limit of the signal
(i.e., above fs/2 of the original signal sample rate). An early and fairly
elementary discussion on this subject can be found in Rabiner and Crochiere's
book Multirate Digital Signal Processing.[3]
***** Related concepts[edit] *****
The term extrapolation is used to find data points outside the range of known
data points.
In curve_fitting problems, the constraint that the interpolant has to go
exactly through the data points is relaxed. It is only required to approach the
data points as closely as possible (within some other constraints). This
requires parameterizing the potential interpolants and having some way of
measuring the error. In the simplest case this leads to least_squares
approximation.
Approximation_theory studies how to find the best approximation to a given
function by another function from some predetermined class, and how good this
approximation is. This clearly yields a bound on how well the interpolant can
approximate the unknown function.
***** Generalization[edit] *****
If we consider     x   {\displaystyle x}  [x] as a variable in a topological
space, with and the function     f ( x )   {\displaystyle f(x)}  [f(x)] mapping
to a Banach_space, then the problem is treated as "interpolation of operators".
[4] The classical results about interpolation of operators are the
RieszâThorin_theorem and the Marcinkiewicz_theorem. There are also many other
subsequent results.
***** See also[edit] *****
    * Barycentric_coordinates_â_for_interpolating_within_on_a_triangle_or
      tetrahedron
    * Bilinear_interpolation
    * Brahmagupta's_interpolation_formula
    * Extrapolation
    * Fractal_interpolation
    * Imputation_(statistics)
    * Lagrange_interpolation
    * Missing_data
    * Multivariate_interpolation
    * NewtonâCotes_formulas
    * Polynomial_interpolation
    * Radial_basis_function_interpolation
    * Simple_rational_approximation
***** References[edit] *****
   1. ^Kress, Rainer (1998). Numerical Analysis.
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
   3. ^Hall, Charles A.; Meyer, Weston W. (1976). "Optimal Error Bounds for
      Cubic Spline Interpolation". Journal of Approximation Theory. 16 (2):
      105â122.
   4. ^ R.E._Crochiere_and_L.R._Rabiner._(1983)._Multirate_Digital_Signal
      Processing._Englewood_Cliffs,_NJ:_PrenticeâHall.
   5. ^ Colin Bennett, Robert C. Sharpley, Interpolation of Operators, Academic
      Press 1988
***** External links[edit] *****
    * Online tools for linear, quadratic, cubic_spline, and polynomial
      interpolation with visualisation and JavaScript source code.
    * Sol_Tutorials_-_Interpolation_Tricks
    * Compactly_Supported_Cubic_B-Spline_interpolation_in_Boost.Math
    * Barycentric_rational_interpolation_in_Boost.Math
    * Interpolation_via_the_Chebyshev_transform_in_Boost.Math

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Interpolation&oldid=906603157"
Categories:
    * Interpolation
    * Video
    * Video_signal
Hidden categories:
    * Articles_lacking_in-text_citations_from_October_2016
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
**** In other projects ****
    * Wikimedia_Commons
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * AzÉrbaycanca
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Gaeilge
    * íêµ­ì´
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Italiano
    * ×¢××¨××ª
    * à²à²¨à³à²¨à²¡
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * Magyar
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * à®¤à®®à®¿à®´à¯
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 16 July 2019, at 22:58 (UTC).
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
