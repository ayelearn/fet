The following text has been accessed from https://en.wikipedia.org/wiki/Frobenius_method at Fri Aug 9 02:32:25 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Frobenius method ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
In mathematics, the method of Frobenius, named after Ferdinand_Georg_Frobenius,
is a way to find an infinite_series solution for a second-order ordinary
differential_equation of the form
          z  2    u &#x2033;  + p ( z ) z  u &#x2032;  + q ( z ) u = 0
      {\displaystyle z^{2}u''+p(z)zu'+q(z)u=0}  [z^{2}u''+p(z)zu'+q(z)u=0]
with
          u &#x2032;  &#x2261;    d u   d z      {\displaystyle u'\equiv {{du}
      \over {dz}}}  [u'\equiv {{du} \over {dz}}]   and        u &#x2033;
      &#x2261;     d  2   u   d  z  2        {\displaystyle u''\equiv {{d^{2}u}
      \over {dz^{2}}}}  [u''\equiv {{d^{2}u} \over {dz^{2}}}]
in the vicinity of the regular_singular_point     z = 0   {\displaystyle z=0}
[z=0]. One can divide by      z  2     {\displaystyle z^{2}}  [z^2] to obtain a
differential equation of the form
          u &#x2033;  +    p ( z )  z    u &#x2032;  +    q ( z )   z  2     u
      = 0   {\displaystyle u''+{p(z) \over z}u'+{q(z) \over z^{2}}u=0}  [u''+{p
      (z) \over z}u'+{q(z) \over z^{2}}u=0]
which will not be solvable with regular power_series_methods if either p(z)/
z or q(z)/z2 are not analytic at z = 0. The Frobenius method enables one to
create a power series solution to such a differential equation, provided that p
(z) and q(z) are themselves analytic at 0 or, being analytic elsewhere, both
their limits at 0 exist (and are finite).
⁰
***** Contents *****
    * 1_Explanation
    * 2_Example
    * 3_Roots_separated_by_an_integer
    * 4_See_also
    * 5_External_links
***** Explanation[edit] *****
The method of Frobenius is to seek a power series solution of the form
         u ( z ) =  &#x2211;  k = 0   &#x221E;    A  k    z  k + r   ,  (  A  0
      &#x2260; 0 )   {\displaystyle u(z)=\sum _{k=0}^{\infty }A_{k}z^
      {k+r},\qquad (A_{0}\neq 0)}  [u(z)=\sum _{{k=0}}^{\infty }A_{k}z^{
      {k+r}},\qquad (A_{0}\neq 0)]
Differentiating:
          u &#x2032;  ( z ) =  &#x2211;  k = 0   &#x221E;   ( k + r )  A  k
      z  k + r &#x2212; 1     {\displaystyle u'(z)=\sum _{k=0}^{\infty }(k+r)A_
      {k}z^{k+r-1}}  [u'(z)=\sum _{{k=0}}^{\infty }(k+r)A_{k}z^{{k+r-1}}]
          u &#x2033;  ( z ) =  &#x2211;  k = 0   &#x221E;   ( k + r &#x2212; 1
      ) ( k + r )  A  k    z  k + r &#x2212; 2     {\displaystyle u''(z)=\sum _
      {k=0}^{\infty }(k+r-1)(k+r)A_{k}z^{k+r-2}}  [u''(z)=\sum _{{k=0}}^{\infty
      }(k+r-1)(k+r)A_{k}z^{{k+r-2}}]
Substituting:
          z  2    &#x2211;  k = 0   &#x221E;   ( k + r &#x2212; 1 ) ( k + r )
      A  k    z  k + r &#x2212; 2   + z p ( z )  &#x2211;  k = 0   &#x221E;
      ( k + r )  A  k    z  k + r &#x2212; 1   + q ( z )  &#x2211;  k = 0
      &#x221E;    A  k    z  k + r     {\displaystyle z^{2}\sum _{k=0}^{\infty
      }(k+r-1)(k+r)A_{k}z^{k+r-2}+zp(z)\sum _{k=0}^{\infty }(k+r)A_{k}z^{k+r-
      1}+q(z)\sum _{k=0}^{\infty }A_{k}z^{k+r}}  [z^{2}\sum _{{k=0}}^{\infty }
      (k+r-1)(k+r)A_{k}z^{{k+r-2}}+zp(z)\sum _{{k=0}}^{\infty }(k+r)A_{k}z^{
      {k+r-1}}+q(z)\sum _{{k=0}}^{\infty }A_{k}z^{{k+r}}]
         =  &#x2211;  k = 0   &#x221E;   ( k + r &#x2212; 1 ) ( k + r )  A  k
      z  k + r   + p ( z )  &#x2211;  k = 0   &#x221E;   ( k + r )  A  k    z
      k + r   + q ( z )  &#x2211;  k = 0   &#x221E;    A  k    z  k + r
      {\displaystyle =\sum _{k=0}^{\infty }(k+r-1)(k+r)A_{k}z^{k+r}+p(z)\sum _
      {k=0}^{\infty }(k+r)A_{k}z^{k+r}+q(z)\sum _{k=0}^{\infty }A_{k}z^{k+r}}
      [=\sum _{{k=0}}^{\infty }(k+r-1)(k+r)A_{k}z^{{k+r}}+p(z)\sum _{{k=0}}^
      {\infty }(k+r)A_{k}z^{{k+r}}+q(z)\sum _{{k=0}}^{\infty }A_{k}z^{{k+r}}]
         =  &#x2211;  k = 0   &#x221E;   [ ( k + r &#x2212; 1 ) ( k + r )  A  k
      z  k + r   + p ( z ) ( k + r )  A  k    z  k + r   + q ( z )  A  k    z
      k + r   ]   {\displaystyle =\sum _{k=0}^{\infty }[(k+r-1)(k+r)A_{k}z^
      {k+r}+p(z)(k+r)A_{k}z^{k+r}+q(z)A_{k}z^{k+r}]}  [=\sum _{{k=0}}^{\infty }
      [(k+r-1)(k+r)A_{k}z^{{k+r}}+p(z)(k+r)A_{k}z^{{k+r}}+q(z)A_{k}z^{{k+r}}]]
         =  &#x2211;  k = 0   &#x221E;    [  ( k + r &#x2212; 1 ) ( k + r ) + p
      ( z ) ( k + r ) + q ( z )  ]   A  k    z  k + r     {\displaystyle =\sum
      _{k=0}^{\infty }\left[(k+r-1)(k+r)+p(z)(k+r)+q(z)\right]A_{k}z^{k+r}}
      [=\sum _{{k=0}}^{\infty }\left[(k+r-1)(k+r)+p(z)(k+r)+q(z)\right]A_{k}z^{
      {k+r}}]
         =  [  r ( r &#x2212; 1 ) + p ( z ) r + q ( z )  ]   A  0    z  r   +
      &#x2211;  k = 1   &#x221E;    [  ( k + r &#x2212; 1 ) ( k + r ) + p ( z )
      ( k + r ) + q ( z )  ]   A  k    z  k + r     {\displaystyle =\left[r(r-
      1)+p(z)r+q(z)\right]A_{0}z^{r}+\sum _{k=1}^{\infty }\left[(k+r-1)(k+r)+p
      (z)(k+r)+q(z)\right]A_{k}z^{k+r}}  [=\left[r(r-1)+p(z)r+q(z)\right]A_
      {0}z^{r}+\sum _{{k=1}}^{\infty }\left[(k+r-1)(k+r)+p(z)(k+r)+q
      (z)\right]A_{k}z^{{k+r}}]
The expression
         r  (  r &#x2212; 1  )  + p  ( 0 )  r + q  ( 0 )  = I ( r )
      {\displaystyle r\left(r-1\right)+p\left(0\right)r+q\left(0\right)=I(r)}
      [r\left(r-1\right)+p\left(0\right)r+q\left(0\right)=I(r)]
is known as the indicial polynomial, which is quadratic in r. The general
definition of the indicial polynomial is the coefficient of the lowest power of
z in the infinite series. In this case it happens to be that this is the rth
coefficient but, it is possible for the lowest possible exponent to be r â 2,
r â 1 or, something else depending on the given differential equation. This
detail is important to keep in mind. In the process of synchronizing all the
series of the differential equation to start at the same index value (which in
the above expression is k = 1), one can end up with complicated expressions.
However, in solving for the indicial roots attention is focused only on the
coefficient of the lowest power of z.
Using this, the general expression of the coefficient of zk + r is
         I ( k + r )  A  k   +  &#x2211;  j = 0   k &#x2212; 1      ( j + r )
      p  ( k &#x2212; j )   ( 0 ) +  q  ( k &#x2212; j )   ( 0 )   ( k &#x2212;
      j ) !     A  j     {\displaystyle I(k+r)A_{k}+\sum _{j=0}^{k-1}{(j+r)p^{
      (k-j)}(0)+q^{(k-j)}(0) \over (k-j)!}A_{j}}  [I(k+r)A_{k}+\sum _{{j=0}}^{
      {k-1}}{(j+r)p^{{(k-j)}}(0)+q^{{(k-j)}}(0) \over (k-j)!}A_{j}],
These coefficients must be zero, since they should be solutions of the
differential equation, so
         I ( k + r )  A  k   +  &#x2211;  j = 0   k &#x2212; 1      ( j + r )
      p  ( k &#x2212; j )   ( 0 ) +  q  ( k &#x2212; j )   ( 0 )   ( k &#x2212;
      j ) !     A  j   = 0   {\displaystyle I(k+r)A_{k}+\sum _{j=0}^{k-1}{
      (j+r)p^{(k-j)}(0)+q^{(k-j)}(0) \over (k-j)!}A_{j}=0}  [I(k+r)A_{k}+\sum _
      {{j=0}}^{{k-1}}{(j+r)p^{{(k-j)}}(0)+q^{{(k-j)}}(0) \over (k-j)!}A_{j}=0]
          &#x2211;  j = 0   k &#x2212; 1      ( j + r )  p  ( k &#x2212; j )
      ( 0 ) +  q  ( k &#x2212; j )   ( 0 )   ( k &#x2212; j ) !     A  j   =
      &#x2212; I ( k + r )  A  k     {\displaystyle \sum _{j=0}^{k-1}{(j+r)p^{
      (k-j)}(0)+q^{(k-j)}(0) \over (k-j)!}A_{j}=-I(k+r)A_{k}}  [\sum _{{j=0}}^{
      {k-1}}{(j+r)p^{{(k-j)}}(0)+q^{{(k-j)}}(0) \over (k-j)!}A_{j}=-I(k+r)A_
      {k}]
           1  &#x2212; I ( k + r )     &#x2211;  j = 0   k &#x2212; 1      ( j
      + r )  p  ( k &#x2212; j )   ( 0 ) +  q  ( k &#x2212; j )   ( 0 )   ( k
      &#x2212; j ) !     A  j   =  A  k     {\displaystyle {1 \over -I
      (k+r)}\sum _{j=0}^{k-1}{(j+r)p^{(k-j)}(0)+q^{(k-j)}(0) \over (k-j)!}A_
      {j}=A_{k}}  [{1 \over -I(k+r)}\sum _{{j=0}}^{{k-1}}{(j+r)p^{{(k-j)}}
      (0)+q^{{(k-j)}}(0) \over (k-j)!}A_{j}=A_{k}]
The series solution with Ak above,
          U  r   ( z ) =  &#x2211;  k = 0   &#x221E;    A  k    z  k + r
      {\displaystyle U_{r}(z)=\sum _{k=0}^{\infty }A_{k}z^{k+r}}  [U_{{r}}
      (z)=\sum _{{k=0}}^{{\infty }}A_{k}z^{{k+r}}]
satisfies
          z  2    U  r   ( z  ) &#x2033;  + p ( z ) z  U  r   ( z  ) &#x2032;
      + q ( z )  U  r   ( z ) = I ( r )  z  r     {\displaystyle z^{2}U_{r}
      (z)''+p(z)zU_{r}(z)'+q(z)U_{r}(z)=I(r)z^{r}}  [z^{2}U_{{r}}(z)''+p(z)zU_{
      {r}}(z)'+q(z)U_{{r}}(z)=I(r)z^{r}]
If we choose one of the roots to the indicial polynomial for r in Ur(z), we
gain a solution to the differential equation. If the difference between the
roots is not an integer, we get another, linearly independent solution in the
other root.
***** Example[edit] *****
Let us solve
          z  2    f &#x2033;  &#x2212; z  f &#x2032;  + ( 1 &#x2212; z ) f = 0
      {\displaystyle z^{2}f''-zf'+(1-z)f=0\,}  [z^{2}f''-zf'+(1-z)f=0\,]
Divide throughout by z2 to give
          f &#x2033;  &#x2212;   1 z    f &#x2032;  +    1 &#x2212; z   z  2
      f =  f &#x2033;  &#x2212;   1 z    f &#x2032;  +  (    1  z  2
      &#x2212;   1 z    )  f = 0   {\displaystyle f''-{1 \over z}f'+{1-z \over
      z^{2}}f=f''-{1 \over z}f'+\left({1 \over z^{2}}-{1 \over z}\right)f=0}
      [f''-{1 \over z}f'+{1-z \over z^{2}}f=f''-{1 \over z}f'+\left({1 \over z^
      {2}}-{1 \over z}\right)f=0]
which has the requisite singularity at z = 0.
Use the series solution
             f    =  &#x2211;  k = 0   &#x221E;    A  k    z  k + r        f
      &#x2032;     =  &#x2211;  k = 0   &#x221E;   ( k + r )  A  k    z  k + r
      &#x2212; 1        f &#x2033;     =  &#x2211;  k = 0   &#x221E;   ( k + r
      ) ( k + r &#x2212; 1 )  A  k    z  k + r &#x2212; 2
      {\displaystyle {\begin{aligned}f&=\sum _{k=0}^{\infty }A_{k}z^
      {k+r}\\f'&=\sum _{k=0}^{\infty }(k+r)A_{k}z^{k+r-1}\\f''&=\sum _{k=0}^
      {\infty }(k+r)(k+r-1)A_{k}z^{k+r-2}\end{aligned}}}  [{\begin
      {aligned}f&=\sum _{{k=0}}^{\infty }A_{k}z^{{k+r}}\\f'&=\sum _{{k=0}}^
      {\infty }(k+r)A_{k}z^{{k+r-1}}\\f''&=\sum _{{k=0}}^{\infty }(k+r)(k+r-
      1)A_{k}z^{{k+r-2}}\end{aligned}}]
Now, substituting
              &#x2211;  k = 0   &#x221E;      ( k + r ) ( k + r &#x2212; 1 )  A
      k    z  k + r &#x2212; 2   &#x2212;   1 z    &#x2211;  k = 0   &#x221E;
      ( k + r )  A  k    z  k + r &#x2212; 1   +  (    1  z  2     &#x2212;   1
      z    )   &#x2211;  k = 0   &#x221E;    A  k    z  k + r         =
      &#x2211;  k = 0   &#x221E;   ( k + r ) ( k + r &#x2212; 1 )  A  k    z  k
      + r &#x2212; 2   &#x2212;   1 z    &#x2211;  k = 0   &#x221E;   ( k + r )
      A  k    z  k + r &#x2212; 1   +   1  z  2      &#x2211;  k = 0   &#x221E;
      A  k    z  k + r   &#x2212;   1 z    &#x2211;  k = 0   &#x221E;    A  k
      z  k + r         =  &#x2211;  k = 0   &#x221E;   ( k + r ) ( k + r
      &#x2212; 1 )  A  k    z  k + r &#x2212; 2   &#x2212;  &#x2211;  k = 0
      &#x221E;   ( k + r )  A  k    z  k + r &#x2212; 2   +  &#x2211;  k = 0
      &#x221E;    A  k    z  k + r &#x2212; 2   &#x2212;  &#x2211;  k = 0
      &#x221E;    A  k    z  k + r &#x2212; 1         =  &#x2211;  k = 0
      &#x221E;   ( k + r ) ( k + r &#x2212; 1 )  A  k    z  k + r &#x2212; 2
      &#x2212;  &#x2211;  k = 0   &#x221E;   ( k + r )  A  k    z  k + r
      &#x2212; 2   +  &#x2211;  k = 0   &#x221E;    A  k    z  k + r &#x2212; 2
      &#x2212;  &#x2211;  k &#x2212; 1 = 0   &#x221E;    A  k &#x2212; 1    z
      k &#x2212; 1 + r &#x2212; 1         =  &#x2211;  k = 0   &#x221E;   ( k +
      r ) ( k + r &#x2212; 1 )  A  k    z  k + r &#x2212; 2   &#x2212;
      &#x2211;  k = 0   &#x221E;   ( k + r )  A  k    z  k + r &#x2212; 2   +
      &#x2211;  k = 0   &#x221E;    A  k    z  k + r &#x2212; 2   &#x2212;
      &#x2211;  k = 1   &#x221E;    A  k &#x2212; 1    z  k + r &#x2212; 2
      =  {   &#x2211;  k = 0   &#x221E;    (  ( k + r ) ( k + r &#x2212; 1 )
      &#x2212; ( k + r ) + 1  )   A  k    z  k + r &#x2212; 2    }  &#x2212;
      &#x2211;  k = 1   &#x221E;    A  k &#x2212; 1    z  k + r &#x2212; 2
      =  {   (  r ( r &#x2212; 1 ) &#x2212; r + 1  )   A  0    z  r &#x2212; 2
      +  &#x2211;  k = 1   &#x221E;    (  ( k + r ) ( k + r &#x2212; 1 )
      &#x2212; ( k + r ) + 1  )   A  k    z  k + r &#x2212; 2    }  &#x2212;
      &#x2211;  k = 1   &#x221E;    A  k &#x2212; 1    z  k + r &#x2212; 2
      = ( r &#x2212; 1  )  2    A  0    z  r &#x2212; 2   +  {   &#x2211;  k =
      1   &#x221E;   ( k + r &#x2212; 1  )  2    A  k    z  k + r &#x2212; 2
      &#x2212;  &#x2211;  k = 1   &#x221E;    A  k &#x2212; 1    z  k + r
      &#x2212; 2    }        = ( r &#x2212; 1  )  2    A  0    z  r &#x2212; 2
      +  &#x2211;  k = 1   &#x221E;    (  ( k + r &#x2212; 1  )  2    A  k
      &#x2212;  A  k &#x2212; 1    )   z  k + r &#x2212; 2
      {\displaystyle {\begin{aligned}\sum _{k=0}^{\infty }&(k+r)(k+r-1)A_{k}z^
      {k+r-2}-{\frac {1}{z}}\sum _{k=0}^{\infty }(k+r)A_{k}z^{k+r-1}+\left(
      {\frac {1}{z^{2}}}-{\frac {1}{z}}\right)\sum _{k=0}^{\infty }A_{k}z^
      {k+r}\\&=\sum _{k=0}^{\infty }(k+r)(k+r-1)A_{k}z^{k+r-2}-{\frac {1}
      {z}}\sum _{k=0}^{\infty }(k+r)A_{k}z^{k+r-1}+{\frac {1}{z^{2}}}\sum _
      {k=0}^{\infty }A_{k}z^{k+r}-{\frac {1}{z}}\sum _{k=0}^{\infty }A_{k}z^
      {k+r}\\&=\sum _{k=0}^{\infty }(k+r)(k+r-1)A_{k}z^{k+r-2}-\sum _{k=0}^
      {\infty }(k+r)A_{k}z^{k+r-2}+\sum _{k=0}^{\infty }A_{k}z^{k+r-2}-\sum _
      {k=0}^{\infty }A_{k}z^{k+r-1}\\&=\sum _{k=0}^{\infty }(k+r)(k+r-1)A_{k}z^
      {k+r-2}-\sum _{k=0}^{\infty }(k+r)A_{k}z^{k+r-2}+\sum _{k=0}^{\infty }A_
      {k}z^{k+r-2}-\sum _{k-1=0}^{\infty }A_{k-1}z^{k-1+r-1}\\&=\sum _{k=0}^
      {\infty }(k+r)(k+r-1)A_{k}z^{k+r-2}-\sum _{k=0}^{\infty }(k+r)A_{k}z^
      {k+r-2}+\sum _{k=0}^{\infty }A_{k}z^{k+r-2}-\sum _{k=1}^{\infty }A_{k-
      1}z^{k+r-2}\\&=\left\{\sum _{k=0}^{\infty }\left((k+r)(k+r-1)-
      (k+r)+1\right)A_{k}z^{k+r-2}\right\}-\sum _{k=1}^{\infty }A_{k-1}z^{k+r-
      2}\\&=\left\{\left(r(r-1)-r+1\right)A_{0}z^{r-2}+\sum _{k=1}^{\infty
      }\left((k+r)(k+r-1)-(k+r)+1\right)A_{k}z^{k+r-2}\right\}-\sum _{k=1}^
      {\infty }A_{k-1}z^{k+r-2}\\&=(r-1)^{2}A_{0}z^{r-2}+\left\{\sum _{k=1}^
      {\infty }(k+r-1)^{2}A_{k}z^{k+r-2}-\sum _{k=1}^{\infty }A_{k-1}z^{k+r-
      2}\right\}\\&=(r-1)^{2}A_{0}z^{r-2}+\sum _{k=1}^{\infty }\left((k+r-1)^
      {2}A_{k}-A_{k-1}\right)z^{k+r-2}\end{aligned}}}  [{\displaystyle {\begin
      {aligned}\sum _{k=0}^{\infty }&(k+r)(k+r-1)A_{k}z^{k+r-2}-{\frac {1}
      {z}}\sum _{k=0}^{\infty }(k+r)A_{k}z^{k+r-1}+\left({\frac {1}{z^{2}}}-
      {\frac {1}{z}}\right)\sum _{k=0}^{\infty }A_{k}z^{k+r}\\&=\sum _{k=0}^
      {\infty }(k+r)(k+r-1)A_{k}z^{k+r-2}-{\frac {1}{z}}\sum _{k=0}^{\infty }
      (k+r)A_{k}z^{k+r-1}+{\frac {1}{z^{2}}}\sum _{k=0}^{\infty }A_{k}z^{k+r}-
      {\frac {1}{z}}\sum _{k=0}^{\infty }A_{k}z^{k+r}\\&=\sum _{k=0}^{\infty }
      (k+r)(k+r-1)A_{k}z^{k+r-2}-\sum _{k=0}^{\infty }(k+r)A_{k}z^{k+r-2}+\sum
      _{k=0}^{\infty }A_{k}z^{k+r-2}-\sum _{k=0}^{\infty }A_{k}z^{k+r-
      1}\\&=\sum _{k=0}^{\infty }(k+r)(k+r-1)A_{k}z^{k+r-2}-\sum _{k=0}^{\infty
      }(k+r)A_{k}z^{k+r-2}+\sum _{k=0}^{\infty }A_{k}z^{k+r-2}-\sum _{k-1=0}^
      {\infty }A_{k-1}z^{k-1+r-1}\\&=\sum _{k=0}^{\infty }(k+r)(k+r-1)A_{k}z^
      {k+r-2}-\sum _{k=0}^{\infty }(k+r)A_{k}z^{k+r-2}+\sum _{k=0}^{\infty }A_
      {k}z^{k+r-2}-\sum _{k=1}^{\infty }A_{k-1}z^{k+r-2}\\&=\left\{\sum _{k=0}^
      {\infty }\left((k+r)(k+r-1)-(k+r)+1\right)A_{k}z^{k+r-2}\right\}-\sum _
      {k=1}^{\infty }A_{k-1}z^{k+r-2}\\&=\left\{\left(r(r-1)-r+1\right)A_{0}z^
      {r-2}+\sum _{k=1}^{\infty }\left((k+r)(k+r-1)-(k+r)+1\right)A_{k}z^{k+r-
      2}\right\}-\sum _{k=1}^{\infty }A_{k-1}z^{k+r-2}\\&=(r-1)^{2}A_{0}z^{r-
      2}+\left\{\sum _{k=1}^{\infty }(k+r-1)^{2}A_{k}z^{k+r-2}-\sum _{k=1}^
      {\infty }A_{k-1}z^{k+r-2}\right\}\\&=(r-1)^{2}A_{0}z^{r-2}+\sum _{k=1}^
      {\infty }\left((k+r-1)^{2}A_{k}-A_{k-1}\right)z^{k+r-2}\end{aligned}}}]
From (r â 1)2 = 0 we get a double root of 1. Using this root, we set the
coefficient of zk + r â 2 to be zero (for it to be a solution), which gives
us:
         ( k + 1 &#x2212; 1  )  2    A  k   &#x2212;  A  k &#x2212; 1   =  k  2
      A  k   &#x2212;  A  k &#x2212; 1   = 0   {\displaystyle (k+1-1)^{2}A_{k}-
      A_{k-1}=k^{2}A_{k}-A_{k-1}=0}  [(k+1-1)^{2}A_{k}-A_{{k-1}}=k^{2}A_{k}-A_{
      {k-1}}=0]
hence we have the recurrence relation:
          A  k   =    A  k &#x2212; 1    k  2       {\displaystyle A_{k}={\frac
      {A_{k-1}}{k^{2}}}}  [A_{k}={\frac  {A_{{k-1}}}{k^{2}}}]
Given some initial conditions, we can either solve the recurrence entirely or
obtain a solution in power series form.
Since the ratio of coefficients      A  k    /   A  k &#x2212; 1
{\displaystyle A_{k}/A_{k-1}}  [A_{k}/A_{{k-1}}] is a rational_function, the
power series can be written as a generalized_hypergeometric_series.
***** Roots separated by an integer[edit] *****
The previous example involved an indicial polynomial with a repeated root,
which gives only one solution to the given differential equation. In general,
the Frobenius method gives two independent solutions provided that the indicial
equation's roots are not separated by an integer (including zero).
If the root is repeated or the roots differ by an integer, then the second
solution can be found using:
          y  2   = C  y  1   ln &#x2061; x +  &#x2211;  k = 0   &#x221E;    B
      k    x  k +  r  2       {\displaystyle y_{2}=Cy_{1}\ln x+\sum _{k=0}^
      {\infty }B_{k}x^{k+r_{2}}}  [y_{2}=Cy_{1}\ln x+\sum _{{k=0}}^{\infty }B_
      {k}x^{{k+r_{2}}}]
where      y  1   ( x )   {\displaystyle y_{1}(x)}  [y_{1}(x)] is the first
solution (based on the larger root in the case of unequal roots),      r  2
{\displaystyle r_{2}}  [r_{2}] is the smaller root, and the constant C and the
coefficients      B  k     {\displaystyle B_{k}}  [B_{k}] are to be determined.
Once      B  0     {\displaystyle B_{0}}  [B_{0}] is chosen (for example by
setting it to 1) then C and the      B  k     {\displaystyle B_{k}}  [B_{k}]
are determined up to but not including      B   r  1   &#x2212;  r  2
{\displaystyle B_{r_{1}-r_{2}}}  [{\displaystyle B_{r_{1}-r_{2}}}], which can
be set arbitrarily. This then determines the rest of the      B  k   .
{\displaystyle B_{k}.}  [{\displaystyle B_{k}.}] In some cases the constant C
must be zero. For example, consider the following differential equation
(Kummer's_equation with a = 1 and b = 2):
         z  u &#x2033;  + ( 2 &#x2212; z )  u &#x2032;  &#x2212; u = 0
      {\displaystyle zu''+(2-z)u'-u=0}  [{\displaystyle zu''+(2-z)u'-u=0}]
The roots of the indicial equation are â1 and 0. Two independent solutions
are     1  /  z   {\displaystyle 1/z}  [1/z] and     (  e  z   )  /  z ,
{\displaystyle (e^{z})/z,}  [{\displaystyle (e^{z})/z,}] so we see that the
logarithm does not appear in any solution. The solution     (  e  z   &#x2212;
1 )  /  z   {\displaystyle (e^{z}-1)/z}  [{\displaystyle (e^{z}-1)/z}] has a
power series starting with the power zero. In a power series starting with
z  &#x2212; 1     {\displaystyle z^{-1}}  [z^{-1}] the recurrence relation
places no restriction on the coefficient for the term      z  0   ,
{\displaystyle z^{0},}  [{\displaystyle z^{0},}] which can be set arbitrarily.
If it is set to zero then with this differential equation all the other
coefficients will be zero and we obtain the solution 1/z.
***** See also[edit] *****
    * Fuchs'_theorem
    * Regular_singular_point
    * Complex_differential_equation
    * Laurent_series
***** External links[edit] *****
    * Weisstein,_Eric_W. "Frobenius_Method". MathWorld.
Teschl,_Gerald (2012). Ordinary_Differential_Equations_and_Dynamical_Systems.
Providence: American_Mathematical_Society. ISBN 978-0-8218-8328-0.
 (Draft version available online at http://www.mat.univie.ac.at/~gerald/ftp/
book-ode/). Chapter 4 contains the full method including proofs.

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Frobenius_method&oldid=852249145"
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
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * Nederlands
    * áá¶áá¶ááááá
    * PortuguÃªs
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * à¹à¸à¸¢
Edit_links
    * This page was last edited on 27 July 2018, at 16:16 (UTC).
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
