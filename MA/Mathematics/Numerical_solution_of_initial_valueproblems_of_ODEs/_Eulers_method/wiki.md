The following text has been accessed from https://en.wikipedia.org/wiki/Euler_method at Fri Aug 9 02:31:59 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Euler method ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For integrating with respect to the Euler characteristic, see Euler_calculus.
For Euler's method for factorizing an integer, see Euler's_factorization
method.
Illustration of the Euler method. The unknown curve is in blue, and its
polygonal approximation is in red.
Euler's method is a numerical_method to solve first order first degree
differential_equation with a given initial value. It is the most basic explicit
method for numerical_integration_of_ordinary_differential_equations and is the
simplest RungeâKutta_method. The Euler method is named after Leonhard_Euler,
who treated it in his book Institutionum_calculi_integralis (published
1768â1870).[1]
The Euler method is a first-order method, which means that the local error
(error per step) is proportional to the square of the step size, and the global
error (error at a given time) is proportional to the step size. The Euler
method often serves as the basis to construct more complex methods, e.g.,
predictorâcorrector_method.
⁰
***** Contents *****
    * 1_Informal_geometrical_description
    * 2_Example
          o 2.1_Using_step_size_equal_to_1_(h_=_1)
          o 2.2_MATLAB_code_example
          o 2.3_R_code_example
          o 2.4_Using_other_step_sizes
    * 3_Derivation
    * 4_Local_truncation_error
    * 5_Global_truncation_error
    * 6_Numerical_stability
    * 7_Rounding_errors
    * 8_Modifications_and_extensions
    * 9_In_popular_culture
    * 10_See_also
    * 11_Notes
    * 12_References
    * 13_External_links
***** Informal geometrical description[edit] *****
Consider the problem of calculating the shape of an unknown curve which starts
at a given point and satisfies a given differential equation. Here, a
differential equation can be thought of as a formula by which the slope of the
tangent_line to the curve can be computed at any point on the curve, once the
position of that point has been calculated.
The idea is that while the curve is initially unknown, its starting point,
which we denote by      A  0   ,   {\displaystyle A_{0},}  [A_{0},] is known
(see the picture on top right). Then, from the differential equation, the slope
to the curve at      A  0     {\displaystyle A_{0}}  [A_{0}] can be computed,
and so, the tangent line.
Take a small step along that tangent line up to a point      A  1   .
{\displaystyle A_{1}.}  [A_{1}.] Along this small step, the slope does not
change too much, so      A  1     {\displaystyle A_{1}}  [A_{1}] will be close
to the curve. If we pretend that      A  1     {\displaystyle A_{1}}  [A_{1}]
is still on the curve, the same reasoning as for the point      A  0
{\displaystyle A_{0}}  [A_{0}] above can be used. After several steps, a
polygonal_curve      A  0    A  1    A  2    A  3   &#x2026;   {\displaystyle
A_{0}A_{1}A_{2}A_{3}\dots }  [A_{0}A_{1}A_{2}A_{3}\dots ] is computed. In
general, this curve does not diverge too far from the original unknown curve,
and the error between the two curves can be made small if the step size is
small enough and the interval of computation is finite:[2]
          y &#x2032;  ( t ) = f ( t , y ( t ) ) ,  y (  t  0   ) =  y  0   .
      {\displaystyle y'(t)=f(t,y(t)),\qquad y(t_{0})=y_{0}.}  [{\displaystyle
      y'(t)=f(t,y(t)),\qquad y(t_{0})=y_{0}.}]
Choose a value     h   {\displaystyle h}  [h] for the size of every step and
set      t  n   =  t  0   + n h   {\displaystyle t_{n}=t_{0}+nh}  [t_{n}=t_
{0}+nh]. Now, one step of the Euler method from      t  n     {\displaystyle t_
{n}}  [t_{n}] to      t  n + 1   =  t  n   + h   {\displaystyle t_{n+1}=t_
{n}+h}  [t_{n+1}=t_{n}+h] is:[3]
          y  n + 1   =  y  n   + h f (  t  n   ,  y  n   ) .   {\displaystyle
      y_{n+1}=y_{n}+hf(t_{n},y_{n}).}  [y_{n+1}=y_{n}+hf(t_{n},y_{n}).]
The value of      y  n     {\displaystyle y_{n}}  [y_{n}] is an approximation
of the solution to the ODE at time      t  n     {\displaystyle t_{n}}  [t_
{n}]:      y  n   &#x2248; y (  t  n   )   {\displaystyle y_{n}\approx y(t_
{n})}  [y_{n}\approx y(t_{n})]. The Euler method is explicit, i.e. the solution
y  n + 1     {\displaystyle y_{n+1}}  [y_{n+1}] is an explicit function of
y  i     {\displaystyle y_{i}}  [y_{i}] for     i &#x2264; n   {\displaystyle
i\leq n}  [i\leq n].
While the Euler method integrates a first-order ODE, any ODE of order N can be
represented as a first-order ODE: to treat the equation
          y  ( N )   ( t ) = f ( t , y ( t ) ,  y &#x2032;  ( t ) , &#x2026; ,
      y  ( N &#x2212; 1 )   ( t ) )   {\displaystyle y^{(N)}(t)=f(t,y(t),y'
      (t),\ldots ,y^{(N-1)}(t))}  [y^{(N)}(t)=f(t,y(t),y'(t),\ldots ,y^{(N-1)}
      (t))],
we introduce auxiliary variables      z  1   ( t ) = y ( t ) ,  z  2   ( t ) =
y &#x2032;  ( t ) , &#x2026; ,  z  N   ( t ) =  y  ( N &#x2212; 1 )   ( t )
{\displaystyle z_{1}(t)=y(t),z_{2}(t)=y'(t),\ldots ,z_{N}(t)=y^{(N-1)}(t)}  [z_
{1}(t)=y(t),z_{2}(t)=y'(t),\ldots ,z_{N}(t)=y^{(N-1)}(t)] and obtain the
equivalent equation:
           z  &#x2032;  ( t ) =   (     z  1  &#x2032;  ( t )     &#x22EE;
      z  N &#x2212; 1  &#x2032;  ( t )      z  N  &#x2032;  ( t )    )   =
      (     y &#x2032;  ( t )     &#x22EE;      y  ( N &#x2212; 1 )   ( t )
      y  ( N )   ( t )    )   =   (     z  2   ( t )     &#x22EE;      z  N
      ( t )     f ( t ,  z  1   ( t ) , &#x2026; ,  z  N   ( t ) )    )
      {\displaystyle \mathbf {z} '(t)={\begin{pmatrix}z_{1}'(t)\\\vdots \\z_{N-
      1}'(t)\\z_{N}'(t)\end{pmatrix}}={\begin{pmatrix}y'(t)\\\vdots \\y^{(N-1)}
      (t)\\y^{(N)}(t)\end{pmatrix}}={\begin{pmatrix}z_{2}(t)\\\vdots \\z_{N}
      (t)\\f(t,z_{1}(t),\ldots ,z_{N}(t))\end{pmatrix}}}  [\mathbf {z} '(t)=
      {\begin{pmatrix}z_{1}'(t)\\\vdots \\z_{N-1}'(t)\\z_{N}'(t)\end{pmatrix}}=
      {\begin{pmatrix}y'(t)\\\vdots \\y^{(N-1)}(t)\\y^{(N)}(t)\end{pmatrix}}=
      {\begin{pmatrix}z_{2}(t)\\\vdots \\z_{N}(t)\\f(t,z_{1}(t),\ldots ,z_{N}
      (t))\end{pmatrix}}]
This is a first-order system in the variable      z  ( t )   {\displaystyle
\mathbf {z} (t)}  [\mathbf {z} (t)] and can be handled by Euler's method or, in
fact, by any other scheme for first-order systems.[4]
***** Example[edit] *****
Given the initial value problem
          y &#x2032;  = y ,  y ( 0 ) = 1 ,   {\displaystyle y'=y,\quad y(0)=1,}
      [y'=y,\quad y(0)=1,]
we would like to use the Euler method to approximate     y ( 4 )
{\displaystyle y(4)}  [y(4)].[5]
**** Using step size equal to 1 (h = 1)[edit] ****
Illustration of numerical integration for the equation      y &#x2032;  = y , y
( 0 ) = 1.   {\displaystyle y'=y,y(0)=1.}  [y'=y,y(0)=1.] Blue is the Euler
method; green, the midpoint_method; red, the exact solution,     y =  e  t   .
{\displaystyle y=e^{t}.}  [y=e^{t}.] The step size is h = 1.0 .
The Euler method is
          y  n + 1   =  y  n   + h f (  t  n   ,  y  n   ) .     {\displaystyle
      y_{n+1}=y_{n}+hf(t_{n},y_{n}).\qquad \qquad }  [y_{n+1}=y_{n}+hf(t_{n},y_
      {n}).\qquad \qquad ]
so first we must compute     f (  t  0   ,  y  0   )   {\displaystyle f(t_
{0},y_{0})}  [f(t_{0},y_{0})]. In this simple differential equation, the
function     f   {\displaystyle f}  [f] is defined by     f ( t , y ) = y
{\displaystyle f(t,y)=y}  [f(t,y)=y]. We have
         f (  t  0   ,  y  0   ) = f ( 0 , 1 ) = 1.     {\displaystyle f(t_
      {0},y_{0})=f(0,1)=1.\qquad \qquad }  [f(t_{0},y_{0})=f(0,1)=1.\qquad
      \qquad ]
By doing the above step, we have found the slope of the line that is tangent to
the solution curve at the point     ( 0 , 1 )   {\displaystyle (0,1)}  [(0,1)].
Recall that the slope is defined as the change in     y   {\displaystyle y}
[y] divided by the change in     t   {\displaystyle t}  [t], or     &#x0394; y
/  &#x0394; t   {\displaystyle \Delta y/\Delta t}  [\Delta y/\Delta t].
The next step is to multiply the above value by the step size     h
{\displaystyle h}  [h], which we take equal to one here:
         h &#x22C5; f (  y  0   ) = 1 &#x22C5; 1 = 1.     {\displaystyle h\cdot
      f(y_{0})=1\cdot 1=1.\qquad \qquad }  [h\cdot f(y_{0})=1\cdot 1=1.\qquad
      \qquad ]
Since the step size is the change in     t   {\displaystyle t}  [t], when we
multiply the step size and the slope of the tangent, we get a change in     y
{\displaystyle y}  [y] value. This value is then added to the initial     y
{\displaystyle y}  [y] value to obtain the next value to be used for
computations.
          y  0   + h f (  y  0   ) =  y  1   = 1 + 1 &#x22C5; 1 = 2.
      {\displaystyle y_{0}+hf(y_{0})=y_{1}=1+1\cdot 1=2.\qquad \qquad }  [y_
      {0}+hf(y_{0})=y_{1}=1+1\cdot 1=2.\qquad \qquad ]
The above steps should be repeated to find      y  2     {\displaystyle y_{2}}
[y_{2}],      y  3     {\displaystyle y_{3}}  [y_{3}] and      y  4
{\displaystyle y_{4}}  [y_{4}].
              y  2      =  y  1   + h f (  y  1   ) = 2 + 1 &#x22C5; 2 = 4 ,
      y  3      =  y  2   + h f (  y  2   ) = 4 + 1 &#x22C5; 4 = 8 ,      y  4
      =  y  3   + h f (  y  3   ) = 8 + 1 &#x22C5; 8 = 16.       {\displaystyle
      {\begin{aligned}y_{2}&=y_{1}+hf(y_{1})=2+1\cdot 2=4,\\y_{3}&=y_{2}+hf(y_
      {2})=4+1\cdot 4=8,\\y_{4}&=y_{3}+hf(y_{3})=8+1\cdot 8=16.\end{aligned}}}
      [{\begin{aligned}y_{2}&=y_{1}+hf(y_{1})=2+1\cdot 2=4,\\y_{3}&=y_{2}+hf(y_
      {2})=4+1\cdot 4=8,\\y_{4}&=y_{3}+hf(y_{3})=8+1\cdot 8=16.\end{aligned}}]
Due to the repetitive nature of this algorithm, it can be helpful to organize
computations in a chart form, as seen below, to avoid making errors.
                                                      f (  t  n
         n               y  n           t  n       ,  y  n   )       h              &#x0394; y      y  n + 1
      {\displaystyle {\displaystyle {\displaystyle {\displaystyle {\displaystyle {\displaystyle {\displaystyle
      n}  [n]        y_{n}}  [y_    t_{n}}  [t_    f(t_{n},y_     h}  [h]        \Delta y}      y_{n+1}}  [y_
                     {n}]           {n}]           {n})}  [f(t_                  [\Delta y]     {n+1}]
                                                   {n},y_{n})]
      0              1              0              1              1              1              2
      1              2              1              2              1              2              4
      2              4              2              4              1              4              8
      3              8              3              8              1              8              16
The conclusion of this computation is that      y  4   = 16   {\displaystyle y_
{4}=16}  [y_{4}=16]. The exact solution of the differential equation is     y
( t ) =  e  t     {\displaystyle y(t)=e^{t}}  [y(t)=e^{t}], so     y ( 4 ) =  e
4   &#x2248; 54.598   {\displaystyle y(4)=e^{4}\approx 54.598}  [y(4)=e^
{4}\approx 54.598]. Although the approximation of the Euler method was not very
precise in this specific case, particularly due to a large value step size
h   {\displaystyle h}  [h], its behaviour is qualitatively correct as the
figure shows.
**** MATLAB code example[edit] ****
clear; clc; close('all');
y0 = 1;
t0 = 0;
h = 1; % try: h = 0.01
tn = 4; % equal to: t0 + h*n, with n the number of steps
[t, y] = Euler(t0, y0, h, tn);
plot(t, y, 'b');

    % exact solution (y = e^t):
    tt = (t0:0.001:tn)';
    yy = exp(tt);
    hold('on');
    plot(tt, yy, 'r');
    hold('off');
    legend('Euler', 'Exact');

function [t, y] = Euler(t0, y0, h, tn)
    fprintf('%10s%10s%10s%15s\n', 'i', 'yi', 'ti', 'f(yi,ti)');
    fprintf('%10d%+10.2f%+10.2f%+15.2f\n', 0, y0, t0, f(y0,t0));
    t = (t0:h:tn)';
    y = zeros(size(t));
    y(1) = y0;
    for i = 1:1:length(t)-1
        y(i+1) = y(i) + h*f(y(i),t(i));
        fprintf('%10d%+10.2f%+10.2f%+15.2f\n', i, y(i+1), t(i+1), f(y(i+1),t
(i+1)));
    end
end

% in this case, f(y,t) = f(y)
function dydt = f(y,t)
    dydt = y;
end

% OUTPUT:
%         i        yi        ti       f(yi,ti)
%         0     +1.00     +0.00          +1.00
%         1     +2.00     +1.00          +2.00
%         2     +4.00     +2.00          +4.00
%         3     +8.00     +3.00          +8.00
%         4    +16.00     +4.00         +16.00
% NOTE: Code also outputs a comparison plot
**** R code example[edit] ****
Graphical output of the R programming language code for the posed example
Below is the code of the example in the R_programming_language.
# ============
# SOLUTION to
#   y' = y,   where y' = f(t,y)
# then:
f <- function(ti,y) y

# INITIAL VALUES:
t0 <- 0
y0 <- 1
h  <- 1
tn <- 4

# Euler's method: function definition
Euler <- function(t0, y0, h, tn, dy.dt) {
  # dy.dt: derivative function

  # t sequence:
  tt <- seq(t0, tn, by=h)
  # table with as many rows as tt elements:
  tbl <- data.frame(ti=tt)
  tbl$yi <- y0 # Initializes yi with y0
  tbl$Dy.dt[1] <- dy.dt(tbl$ti[1],y0) # derivative
  for (i in 2:nrow(tbl)) {
    tbl$yi[i] <- tbl$yi[i-1] + h*tbl$Dy.dt[i-1]
    # For next iteration:
    tbl$Dy.dt[i] <- dy.dt(tbl$ti[i],tbl$yi[i])
  }
  return(tbl)
}

# Euler's method: function application
r <- Euler(t0, y0, h, tn, f)
rownames(r) <- 0:(nrow(r)-1) # to coincide with index n

# Exact solution for this case: y = exp(t)
#       added as an additional column to r
r$y <- exp(r$ti)

# TABLE with results:
print(r)

plot(r$ti, r$y, type="l", col="red", lwd=2)
lines(r$ti, r$yi, col="blue", lwd=2)
grid(col="black")
legend("top",  legend = c("Exact", "Euler"), lwd=2,  col = c("red", "blue"))

# OUTPUT:
#
#   ti yi Dy.dt         y
# 0  0  1     1  1.000000
# 1  1  2     2  2.718282
# 2  2  4     4  7.389056
# 3  3  8     8 20.085537
# 4  4 16    16 54.598150
# NOTE: Code also outputs a comparison plot
**** Using other step sizes[edit] ****
The same illustration for h = 0.25.
As suggested in the introduction, the Euler method is more accurate if the step
size     h   {\displaystyle h}  [h] is smaller. The table below shows the
result with different step sizes. The top row corresponds to the example in the
previous section, and the second row is illustrated in the figure.
      step size result of Euler's method error
      1         16.00                    38.60
      0.25      35.53                    19.07
      0.1       45.26                    9.34
      0.05      49.56                    5.04
      0.025     51.98                    2.62
      0.0125    53.26                    1.34
The error recorded in the last column of the table is the difference between
the exact solution at     t = 4   {\displaystyle t=4}  [t=4] and the Euler
approximation. In the bottom of the table, the step size is half the step size
in the previous row, and the error is also approximately half the error in the
previous row. This suggests that the error is roughly proportional to the step
size, at least for fairly small values of the step size. This is true in
general, also for other equations; see the section Global_truncation_error for
more details.
Other methods, such as the midpoint_method also illustrated in the figures,
behave more favourably: the global error of the midpoint method is roughly
proportional to the square of the step size. For this reason, the Euler method
is said to be a first-order method, while the midpoint method is second order.
We can extrapolate from the above table that the step size needed to get an
answer that is correct to three decimal places is approximately 0.00001,
meaning that we need 400,000 steps. This large number of steps entails a high
computational cost. For this reason, people usually employ alternative, higher-
order methods such as RungeâKutta_methods or linear_multistep_methods,
especially if a high accuracy is desired.[6]
***** Derivation[edit] *****
The Euler method can be derived in a number of ways. Firstly, there is the
geometrical description above.
Another possibility is to consider the Taylor_expansion of the function     y
{\displaystyle y}  [y] around      t  0     {\displaystyle t_{0}}  [t_{0}]:
         y (  t  0   + h ) = y (  t  0   ) + h  y &#x2032;  (  t  0   ) +   1 2
      h  2    y &#x2033;  (  t  0   ) + O (  h  3   ) .   {\displaystyle y(t_
      {0}+h)=y(t_{0})+hy'(t_{0})+{\frac {1}{2}}h^{2}y''(t_{0})+O(h^{3}).}  [y
      (t_{0}+h)=y(t_{0})+hy'(t_{0})+{\frac {1}{2}}h^{2}y''(t_{0})+O(h^{3}).]
The differential equation states that      y &#x2032;  = f ( t , y )
{\displaystyle y'=f(t,y)}  [y'=f(t,y)]. If this is substituted in the Taylor
expansion and the quadratic and higher-order terms are ignored, the Euler
method arises.[7] The Taylor expansion is used below to analyze the error
committed by the Euler method, and it can be extended to produce RungeâKutta
methods.
A closely related derivation is to substitute the forward finite_difference
formula for the derivative,
          y &#x2032;  (  t  0   ) &#x2248;    y (  t  0   + h ) &#x2212; y (  t
      0   )  h     {\displaystyle y'(t_{0})\approx {\frac {y(t_{0}+h)-y(t_{0})}
      {h}}}  [y'(t_{0})\approx {\frac {y(t_{0}+h)-y(t_{0})}{h}}]
in the differential equation      y &#x2032;  = f ( t , y )   {\displaystyle
y'=f(t,y)}  [y'=f(t,y)]. Again, this yields the Euler method.[8] A similar
computation leads to the midpoint_method and the backward_Euler_method.
Finally, one can integrate the differential equation from      t  0
{\displaystyle t_{0}}  [t_{0}] to      t  0   + h   {\displaystyle t_{0}+h}
[t_{0}+h] and apply the fundamental_theorem_of_calculus to get:
         y (  t  0   + h ) &#x2212; y (  t  0   ) =  &#x222B;   t  0      t  0
      + h   f ( t , y ( t ) )   d  t .   {\displaystyle y(t_{0}+h)-y(t_
      {0})=\int _{t_{0}}^{t_{0}+h}f(t,y(t))\,\mathrm {d} t.}  [y(t_{0}+h)-y(t_
      {0})=\int _{t_{0}}^{t_{0}+h}f(t,y(t))\,\mathrm {d} t.]
Now approximate the integral by the left-hand rectangle_method (with only one
rectangle):
          &#x222B;   t  0      t  0   + h   f ( t , y ( t ) )   d  t &#x2248; h
      f (  t  0   , y (  t  0   ) ) .   {\displaystyle \int _{t_{0}}^{t_{0}+h}f
      (t,y(t))\,\mathrm {d} t\approx hf(t_{0},y(t_{0})).}  [\int _{t_{0}}^{t_
      {0}+h}f(t,y(t))\,\mathrm {d} t\approx hf(t_{0},y(t_{0})).]
Combining both equations, one finds again the Euler method.[9] This line of
thought can be continued to arrive at various linear_multistep_methods.
***** Local truncation error[edit] *****
The local_truncation_error of the Euler method is the error made in a single
step. It is the difference between the numerical solution after one step,
y  1     {\displaystyle y_{1}}  [y_{1}], and the exact solution at time      t
1   =  t  0   + h   {\displaystyle t_{1}=t_{0}+h}  [t_{1}=t_{0}+h]. The
numerical solution is given by
          y  1   =  y  0   + h f (  t  0   ,  y  0   ) .    {\displaystyle y_
      {1}=y_{0}+hf(t_{0},y_{0}).\quad }  [y_{1}=y_{0}+hf(t_{0},y_{0}).\quad ]
For the exact solution, we use the Taylor expansion mentioned in the section
Derivation above:
         y (  t  0   + h ) = y (  t  0   ) + h  y &#x2032;  (  t  0   ) +   1 2
      h  2    y &#x2033;  (  t  0   ) + O (  h  3   ) .   {\displaystyle y(t_
      {0}+h)=y(t_{0})+hy'(t_{0})+{\frac {1}{2}}h^{2}y''(t_{0})+O(h^{3}).}  [y
      (t_{0}+h)=y(t_{0})+hy'(t_{0})+{\frac {1}{2}}h^{2}y''(t_{0})+O(h^{3}).]
The local truncation error (LTE) introduced by the Euler method is given by the
difference between these equations:
          L T E  = y (  t  0   + h ) &#x2212;  y  1   =   1 2    h  2    y
      &#x2033;  (  t  0   ) + O (  h  3   ) .   {\displaystyle \mathrm {LTE} =y
      (t_{0}+h)-y_{1}={\frac {1}{2}}h^{2}y''(t_{0})+O(h^{3}).}  [\mathrm {LTE}
      =y(t_{0}+h)-y_{1}={\frac {1}{2}}h^{2}y''(t_{0})+O(h^{3}).]
This result is valid if     y   {\displaystyle y}  [y] has a bounded third
derivative.[10]
This shows that for small     h   {\displaystyle h}  [h], the local truncation
error is approximately proportional to      h  2     {\displaystyle h^{2}}  [h^
{2}]. This makes the Euler method less accurate (for small     h
{\displaystyle h}  [h]) than other higher-order techniques such as Runge-Kutta
methods and linear_multistep_methods, for which the local truncation error is
proportional to a higher power of the step size.
A slightly different formulation for the local truncation error can be obtained
by using the Lagrange form for the remainder term in Taylor's_theorem. If     y
{\displaystyle y}  [y] has a continuous second derivative, then there exists a
&#x03BE; &#x2208; [  t  0   ,  t  0   + h ]   {\displaystyle \xi \in [t_{0},t_
{0}+h]}  [\xi \in [t_{0},t_{0}+h]] such that
          L T E  = y (  t  0   + h ) &#x2212;  y  1   =   1 2    h  2    y
      &#x2033;  ( &#x03BE; ) .   {\displaystyle \mathrm {LTE} =y(t_{0}+h)-y_
      {1}={\frac {1}{2}}h^{2}y''(\xi ).}  [\mathrm {LTE} =y(t_{0}+h)-y_{1}=
      {\frac {1}{2}}h^{2}y''(\xi ).][11]
In the above expressions for the error, the second derivative of the unknown
exact solution     y   {\displaystyle y}  [y] can be replaced by an expression
involving the right-hand side of the differential equation. Indeed, it follows
from the equation      y &#x2032;  = f ( t , y )   {\displaystyle y'=f(t,y)}
[y'=f(t,y)] that
          y &#x2033;  (  t  0   ) =    &#x2202; f   &#x2202; t    (  t  0   , y
      (  t  0   ) ) +    &#x2202; f   &#x2202; y    (  t  0   , y (  t  0   ) )
      f (  t  0   , y (  t  0   ) ) .   {\displaystyle y''(t_{0})={\partial f
      \over \partial t}(t_{0},y(t_{0}))+{\partial f \over \partial y}(t_{0},y
      (t_{0}))\,f(t_{0},y(t_{0})).}  [y''(t_{0})={\partial f \over \partial t}
      (t_{0},y(t_{0}))+{\partial f \over \partial y}(t_{0},y(t_{0}))\,f(t_{0},y
      (t_{0})).][12]
***** Global truncation error[edit] *****
The global_truncation_error is the error at a fixed time     t   {\displaystyle
t}  [t], after however many steps the methods needs to take to reach that time
from the initial time. The global truncation error is the cumulative effect of
the local truncation errors committed in each step.[13] The number of steps is
easily determined to be     ( t &#x2212;  t  0   )  /  h   {\displaystyle (t-t_
{0})/h}  [(t-t_{0})/h], which is proportional to     1  /  h   {\displaystyle
1/h}  [1/h], and the error committed in each step is proportional to      h  2
{\displaystyle h^{2}}  [h^{2}] (see the previous section). Thus, it is to be
expected that the global truncation error will be proportional to     h
{\displaystyle h}  [h].[14]
This intuitive reasoning can be made precise. If the solution     y
{\displaystyle y}  [y] has a bounded second derivative and     f
{\displaystyle f}  [f] is Lipschitz_continuous in its second argument, then the
global truncation error (GTE) is bounded by
          |   GTE   |  &#x2264;    h M   2 L    (  e  L ( t &#x2212;  t  0   )
      &#x2212; 1 )     {\displaystyle |{\text{GTE}}|\leq {\frac {hM}{2L}}(e^{L
      (t-t_{0})}-1)\qquad \qquad }  [|{\text{GTE}}|\leq {\frac {hM}{2L}}(e^{L
      (t-t_{0})}-1)\qquad \qquad ]
where     M   {\displaystyle M}  [M] is an upper bound on the second derivative
of     y   {\displaystyle y}  [y] on the given interval and     L
{\displaystyle L}  [L] is the Lipschitz constant of     f   {\displaystyle f}
[f].[15]
The precise form of this bound is of little practical importance, as in most
cases the bound vastly overestimates the actual error committed by the Euler
method.[16] What is important is that it shows that the global truncation error
is (approximately) proportional to     h   {\displaystyle h}  [h]. For this
reason, the Euler method is said to be first order.[17]
***** Numerical stability[edit] *****
Solution of      y &#x2032;  = &#x2212; 2.3 y   {\displaystyle y'=-2.3y}  [y'=-
2.3y] computed with the Euler method with step size     h = 1   {\displaystyle
h=1}  [h=1] (blue squares) and     h = 0.7   {\displaystyle h=0.7}  [h=0.7]
(red circles). The black curve shows the exact solution.
The Euler method can also be numerically unstable, especially for stiff
equations, meaning that the numerical solution grows very large for equations
where the exact solution does not. This can be illustrated using the linear
equation
          y &#x2032;  = &#x2212; 2.3 y ,  y ( 0 ) = 1.   {\displaystyle y'=-
      2.3y,\qquad y(0)=1.}  [y'=-2.3y,\qquad y(0)=1.]
The exact solution is     y ( t ) =  e  &#x2212; 2.3 t     {\displaystyle y
(t)=e^{-2.3t}}  [y(t)=e^{-2.3t}], which decays to zero as     t &#x2192;
&#x221E;   {\displaystyle t\to \infty }  [t\to \infty ]. However, if the Euler
method is applied to this equation with step size     h = 1   {\displaystyle
h=1}  [h=1], then the numerical solution is qualitatively wrong: It oscillates
and grows (see the figure). This is what it means to be unstable. If a smaller
step size is used, for instance     h = 0.7   {\displaystyle h=0.7}  [
{\displaystyle h=0.7}], then the numerical solution does decay to zero.
The pink disk shows the stability region for the Euler method.
If the Euler method is applied to the linear equation      y &#x2032;  = k y
{\displaystyle y'=ky}  [y'=ky], then the numerical solution is unstable if the
product     h k   {\displaystyle hk}  [hk] is outside the region
         { z &#x2208;  C  &#x2223;  |  z + 1  |  &#x2264; 1 } ,
      {\displaystyle \{z\in \mathbf {C} \mid |z+1|\leq 1\},}  [\{z\in \mathbf
      {C} \mid |z+1|\leq 1\},]
illustrated on the right. This region is called the (linear) stability region.
[18] In the example,     k   {\displaystyle k}  [k] is â2.3, so if     h = 1
{\displaystyle h=1}  [h=1] then     h k = &#x2212; 2.3   {\displaystyle hk=-
2.3}  [hk=-2.3] which is outside the stability region, and thus the numerical
solution is unstable.
This limitation âalong with its slow convergence of error with hâ means
that the Euler method is not often used, except as a simple example of
numerical integration.
***** Rounding errors[edit] *****
The discussion up to now has ignored the consequences of rounding_error. In
step n of the Euler method, the rounding error is roughly of the magnitude Îµyn
where Îµ is the machine_epsilon. Assuming that the rounding errors are all of
approximately the same size, the combined rounding error in N steps is roughly
NÎµy0 if all errors points in the same direction. Since the number of steps is
inversely proportional to the step size h, the total rounding error is
proportional to Îµ / h. In reality, however, it is extremely unlikely that all
rounding errors point in the same direction. If instead it is assumed that the
rounding errors are independent random variables, then the expected total
rounding error is proportional to     &#x03B5;  /    h     {\displaystyle
\varepsilon /{\sqrt {h}}}  [\varepsilon /{\sqrt {h}}].[19]
Thus, for extremely small values of the step size, the truncation error will be
small but the effect of rounding error may be big. Most of the effect of
rounding error can be easily avoided if compensated_summation is used in the
formula for the Euler method.[20]
***** Modifications and extensions[edit] *****
A simple modification of the Euler method which eliminates the stability
problems noted in the previous section is the backward_Euler_method:
          y  n + 1   =  y  n   + h f (  t  n + 1   ,  y  n + 1   ) .
      {\displaystyle y_{n+1}=y_{n}+hf(t_{n+1},y_{n+1}).}  [y_{n+1}=y_{n}+hf(t_
      {n+1},y_{n+1}).]
This differs from the (standard, or forward) Euler method in that the function
f   {\displaystyle f}  [f] is evaluated at the end point of the step, instead
of the starting point. The backward Euler method is an implicit_method, meaning
that the formula for the backward Euler method has      y  n + 1
{\displaystyle y_{n+1}}  [y_{n+1}] on both sides, so when applying the backward
Euler method we have to solve an equation. This makes the implementation more
costly.
Other modifications of the Euler method that help with stability yield the
exponential_Euler_method or the semi-implicit_Euler_method.
More complicated methods can achieve a higher order (and more accuracy). One
possibility is to use more function evaluations. This is illustrated by the
midpoint_method which is already mentioned in this article:
          y  n + 1   =  y  n   + h f   (    t  n   +    1 2    h ,  y  n   +
      1 2    h f (  t  n   ,  y  n   )   )     {\displaystyle y_{n+1}=y_{n}+hf
      {\Big (}t_{n}+{\tfrac {1}{2}}h,y_{n}+{\tfrac {1}{2}}hf(t_{n},y_{n}){\Big
      )}}  [{\displaystyle y_{n+1}=y_{n}+hf{\Big (}t_{n}+{\tfrac {1}{2}}h,y_
      {n}+{\tfrac {1}{2}}hf(t_{n},y_{n}){\Big )}}].
This leads to the family of RungeâKutta_methods.
The other possibility is to use more past values, as illustrated by the two-
step AdamsâBashforth method:
          y  n + 1   =  y  n   +    3 2    h f (  t  n   ,  y  n   ) &#x2212;
      1 2    h f (  t  n &#x2212; 1   ,  y  n &#x2212; 1   ) .   {\displaystyle
      y_{n+1}=y_{n}+{\tfrac {3}{2}}hf(t_{n},y_{n})-{\tfrac {1}{2}}hf(t_{n-1},y_
      {n-1}).}  [y_{n+1}=y_{n}+{\tfrac {3}{2}}hf(t_{n},y_{n})-{\tfrac {1}{2}}hf
      (t_{n-1},y_{n-1}).]
This leads to the family of linear_multistep_methods. There are other
modifications which uses techniques from compressive sensing to minimize memory
usage[21]
***** In popular culture[edit] *****
In the film Hidden_Figures, Katherine_Goble resorts to the Euler method in
calculating the re-entry of astronaut John_Glenn from Earth orbit.[22]
***** See also[edit] *****
    * CrankâNicolson_method
    * Dynamic_errors_of_numerical_methods_of_ODE_discretization
    * Gradient_descent similarly uses finite steps, here to find minima of
      functions
    * List_of_Runge-Kutta_methods
    * Linear_multistep_method
    * Numerical_integration (for calculating definite integrals)
    * Numerical_methods_for_ordinary_differential_equations
***** Notes[edit] *****
   1. ^ Butcher_2003, p. 45; Hairer,_NÃ¸rsett_&_Wanner_1993, p. 35
   2. ^ Atkinson_1989, p. 342; Butcher_2003, p. 60
   3. ^ Butcher_2003, p. 45; Hairer,_NÃ¸rsett_&_Wanner_1993, p. 36
   4. ^ Butcher_2003, p. 3; Hairer,_NÃ¸rsett_&_Wanner_1993, p. 2
   5. ^ See also Atkinson_1989, p. 344
   6. ^ Hairer,_NÃ¸rsett_&_Wanner_1993, p. 40
   7. ^ Atkinson_1989, p. 342; Hairer,_NÃ¸rsett_&_Wanner_1993, p. 36
   8. ^ Atkinson_1989, p. 342
   9. ^ Atkinson_1989, p. 343
  10. ^ Butcher_2003, p. 60
  11. ^ Atkinson_1989, p. 342
  12. ^ Stoer_&_Bulirsch_2002, p. 474
  13. ^ Atkinson_1989, p. 344
  14. ^ Butcher_2003, p. 49
  15. ^ Atkinson_1989, p. 346; Lakoba_2012, equation (1.16)
  16. ^ Iserles_1996, p. 7
  17. ^ Butcher_2003, p. 63
  18. ^ Butcher_2003, p. 70; Iserles_1996, p. 57
  19. ^ Butcher_2003, pp. 74â75
  20. ^ Butcher_2003, pp. 75â78
  21. ^Unni, M. P.; Chandra, M. G.; Kumar, A. A. (March 2017). "Memory
      reduction_for_numerical_solution_of_differential_equations_using
      compressive_sensing". 2017 IEEE 13th International Colloquium on Signal
      Processing its Applications (CSPA): 79â84. doi:10.1109/
      CSPA.2017.8064928.
  22. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
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
  23. ^Khan, Amina. "Meet_the_'Hidden_Figures'_mathematician_who_helped_send
      Americans_into_space". Los Angeles Times. Retrieved 12 February 2017.
***** References[edit] *****
    * Atkinson, Kendall A. (1989). An Introduction to Numerical Analysis (2nd
      ed.). New York: John_Wiley_&_Sons. ISBN 978-0-471-50023-0.
Ascher, Uri M.; Petzold,_Linda_R. (1998). Computer_Methods_for_Ordinary
Differential_Equations_and_Differential-Algebraic_Equations. Philadelphia:
Society_for_Industrial_and_Applied_Mathematics. ISBN 978-0-89871-412-8.
Butcher,_John_C. (2003). Numerical Methods for Ordinary Differential Equations.
New York: John_Wiley_&_Sons. ISBN 978-0-471-96758-3.
Hairer, Ernst; NÃ¸rsett, Syvert Paul; Wanner, Gerhard (1993). Solving ordinary
differential equations I: Nonstiff problems. Berlin, New York: Springer-Verlag.
ISBN 978-3-540-56670-0.
Iserles,_Arieh (1996). A_First_Course_in_the_Numerical_Analysis_of_Differential
Equations. Cambridge_University_Press. ISBN 978-0-521-55655-2.
Stoer, Josef; Bulirsch, Roland (2002). Introduction to Numerical Analysis (3rd
ed.). Berlin, New York: Springer-Verlag. ISBN 978-0-387-95452-3.
Lakoba, Taras I. (2012), Simple_Euler_method_and_its_modifications (PDF)
(Lecture notes for MATH334), University of Vermont, retrieved 29 February 2012
Unni, M P. (2017). Memory_reduction_for_numerical_solution_of_differential
equations_using_compressive_sensing. IEEE_CSPA. ISBN 978-1-5090-1184-1.
***** External links[edit] *****
 The Wikibook Calculus has a page on the topic of: Euler's_Method
    *  Media related to Euler_method at Wikimedia Commons
    * Euler_method_implementations_in_different_languages by Rosetta_Code
    * v
    * t
    * e
Numerical_methods_for_integration
                         * Euler method
First-order_methods      * Backward_Euler
                         * Semi-implicit_Euler
                         * Exponential_Euler
                         * Verlet_integration
                         * Velocity_Verlet
                         * Trapezoidal_rule
Second-order_methods     * Beeman's_algorithm
                         * Midpoint_method
                         * Heun's_method
                         * Newmark-beta_method
                         * Leapfrog_integration
                         * Exponential_integrator
                         * RungeâKutta_methods
                         * List_of_RungeâKutta_methods
Higher-order_methods     * Linear_multistep_method
                         * General_linear_methods
                         * Backward_differentiation_formula
                         * Yoshida
Theory                   * Symplectic_integrator

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Euler_method&oldid=907454399"
Categories:
    * Numerical_differential_equations
    * RungeâKutta_methods
    * First_order_methods
    * Leonhard_Euler
Hidden categories:
    * Commons_category_link_from_Wikidata
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
    * Deutsch
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * FranÃ§ais
    * íêµ­ì´
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Suomi
    * Svenska
    * Tagalog
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * ä¸­æ
Edit_links
    * This page was last edited on 23 July 2019, at 00:57 (UTC).
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
