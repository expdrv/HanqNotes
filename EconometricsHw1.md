<script type="text/javascript"
       src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
# Econometrics Assignment1

## 1.
- $\hat{\beta}=argmin||(Y-X\beta)^{\intercal}(Y-X\beta)||$, in this case, $\frac{\partial\sum\epsilon^2}{\partial{\beta}}=\sum(y_i-x_i\beta)x_i=0$
  so $\hat{\beta}=\frac{\sum{x_iy_i}}{\sum x_i^2}$ and $var(\hat{\beta})=E((\hat{\beta}-\beta)^2)=E((\frac{\sum{x_iy_i}}{\sum x_i^2}-\beta)^2)=\frac{\sigma^2}{\sum x_i^2}$
- $E(\tilde{\beta}-\beta)=E(n^{-1}\sum(\frac{y_i}{x_i}-\beta))=n^{-1}\sum 0=0$ and  $E(\bar{\beta}-\beta)=E(\frac{\bar{y}-\bar{x}\beta}{\bar{x}})=0$
- $var(\tilde{\beta})=E((n^{-1}\sum(\frac{y_i}{x_i}-\beta)^2)=n^{-2}\sigma^2\sum\frac{1}{x_i^2}, var(\bar{\beta})=E((\frac{\bar{y}}{\bar{x}}-\beta)^2)=\sigma^2\frac{n}{(\sum x_i)^2}$
  of course they are larger than OLS estimator according to BLUE.

## 2.
$P_1+P_2=X_1(X_1^\intercal X_1)^{-1}X_1+X_2(X_2^\intercal X_2)^{-1}X_2$
$P=\left[\begin{matrix}X_1&X_2\end{matrix}\right](\left[\begin{matrix}X_1^\intercal \\X_2^\intercal\end{matrix}\right]\left[\begin{matrix}X_1&X_2\end{matrix}\right])^{-1}\left[\begin{matrix}X_1^\intercal \\X_2^\intercal\end{matrix}\right]$ from the lemma, $(\left[\begin{matrix}X_1^\intercal \\X_2^\intercal\end{matrix}\right]\left[\begin{matrix}X_1 & X_2\end{matrix}\right])^{-1}=\left[\begin{matrix}X_1^\intercal X_1& \boldsymbol{0} \\\boldsymbol{0}&X_2^\intercal X_2\end{matrix}\right]^{-1}=\left[\begin{matrix}(X_1^\intercal X_1)^{-1}& \boldsymbol{0} \\\boldsymbol{0}&(X_2^\intercal X_2)^{-1}
\end{matrix}\right]$ then 


$P=\left[\begin{matrix}X_1&X_2\end{matrix}\right]\left[\begin{matrix}(X_1^\intercal X_1)^{-1}& \boldsymbol{0}\\\boldsymbol{0}&(X_2^\intercal X_2)^{-1}\end{matrix}\right]\left[\begin{matrix}X_1^\intercal \\X_2^\intercal\end{matrix}\right]=$



$\left[\begin{matrix}{X_1(X_1^\intercal X_1)^{-1}X_1^\intercal}_{n\times n}+{X_2(X_2^\intercal X_2)^{-1}X_2^\intercal}_{n\times n}\end{matrix}\right]_{n\times n}=P_1+P_2$, $QED$

## 3.
- $M_1 y=M_1 X_1\beta_1+M_1X_2\beta_2 +M_1 \epsilon$ we know $M_1X_1=\boldsymbol{0}$,  so $M_1y=M_1X_2\beta_2 +M_1 \epsilon$ 
  
  according to OLS, $\hat{\beta_2}=(X_2^\intercal M_1^\intercal M_1X_2)^{-1}X_2^\intercal M_1^\intercal M_1y=(X_2^\intercal M_1X_2)^{-1}X_2^\intercal M_1 y ,\quad $and

    
    $ \: vise \: versa\quad \hat{\beta_1}=(X_1^\intercal M_2X_1)^{-1}X_1^\intercal M_2 y.$ 
- $E(\hat{\beta_1}-\beta_1)=E((X_1^\intercal M_2X_1)^{-1}X_1^\intercal M_2 y-\beta_1)=$
  
  
  
  $E((X_1^\intercal M_2X_1)^{-1}X_1^\intercal M_2  (X_1\beta_1+X_2\beta_2+\epsilon)-\beta_1)=E((X_1^\intercal M_2X_1)^{-1}X_1^\intercal M_2X_1\beta_1-\beta_1)=\boldsymbol{0}$
- $var(\hat{\beta_1})=E((X_1^\intercal M_2X_1)^{-1}X_1^\intercal M_2\epsilon_1((X_1^\intercal M_2X_1)^{-1}X_1^\intercal M_2\epsilon_1)^\intercal))=E((X_1^\intercal M_2X_1)^{-1}X_1^\intercal M_2\epsilon_1\epsilon_1^\intercal M_2^\intercal X_1 (X_1^\intercal M_2X_1)^{-1})=\sigma^2E((X_1^\intercal M_2X_1)^{-1}X_1^\intercal M_2 I_n M_2^\intercal X_1 (X_1^\intercal M_2X_1)^{-1})=\sigma^2(X_1^\intercal M_2X_1)^{-1}$
  
## 4.

- $E(\beta^*-\beta)=E(\hat{\beta}-(X^\intercal X)^{-1}R^\intercal (R(X^\intercal X)^{-1}R^\intercal)^{-1}(R\hat{\beta}-c)-\beta)$
  
  $=E(-(X^\intercal X)^{-1}R^\intercal (R(X^\intercal X)^{-1}R^\intercal)^{-1}(R\beta-c))=\boldsymbol{0}$

- $var(\beta^*)=var((\hat{\beta}-\beta)-(X^\intercal X)^{-1}R^\intercal (R(X^\intercal X)^{-1}R^\intercal)^{-1}(R\hat{\beta-c}))$
  $=var(\hat{\beta}-(X^\intercal X)^{-1}R^\intercal (R(X^\intercal X)^{-1}R^\intercal)^{-1}R\hat{\beta})$
  $=var(\hat{\beta})+var((X^\intercal X)^{-1}R^\intercal (R(X^\intercal X)^{-1}R^\intercal)^{-1}R\hat{\beta})-2cov(\hat{\beta},(X^\intercal X)^{-1}R^\intercal (R(X^\intercal X)^{-1}R^\intercal)^{-1}R\hat{\beta})$
  $=\sigma^2(X^\intercal X)^{-1}+\sigma^2(X^\intercal X)^{-1}R^\intercal (R(X^\intercal X)^{-1}R^\intercal)^{-1}R(X^\intercal X)^{-1}R^\intercal (R(X^\intercal X)^{-1}R^\intercal)^{-1}R(X^\intercal X)^{-1}$
  $-2\sigma^2(X^\intercal X)^{-1}R^\intercal (R(X^\intercal X)^{-1}R^\intercal)^{-1}R(X^\intercal X)^{-1}$
  $=\sigma^2((X^\intercal X)^{-1})+(X^\intercal X)^{-1}R^\intercal(R(X^\intercal X)^{-1}R^\intercal)^{-1}R(X^\intercal X)^{-1}-2(X^\intercal X)^{-1}R^\intercal(R(X^\intercal X)^{-1}R^\intercal)^{-1}R(X^\intercal X)^{-1})$
  $=\sigma^2((X^\intercal X)^{-1})-(X^\intercal X)^{-1}R^\intercal(R(X^\intercal X)^{-1}R^\intercal)^{-1}R(X^\intercal X)^{-1}$
   so $var(\hat{\beta})>var(\beta^*)\quad$because it is larger  by one  positive semi-define matrix.

## 5. 
$F=\frac{\hat{\epsilon^*}^\intercal\hat{\epsilon^*}-\hat{\epsilon}^\intercal\hat{\epsilon}}{\hat{\epsilon}^\intercal\hat{\epsilon}}\times \frac{n-K}{J}$

$\frac{\hat{\epsilon^*}^\intercal\hat{\epsilon^*}-\hat{\epsilon}^\intercal\hat{\epsilon}}{\hat{\epsilon}^\intercal\hat{\epsilon}}=\frac{(y-\beta^*X)(y-\beta^*X)^\intercal-(y-\hat{\beta}X)(y-\hat{\beta}X)^\intercal}{(y-\hat{\beta}X)(y-\hat{\beta}X)^\intercal}=s^{-2}(R\hat{\beta}-c)(R^\intercal(X^\intercal X)^{-1}R)^{-1}(R\hat{\beta}-c)/(n-K)$ so F-test equals to W-test statistic.