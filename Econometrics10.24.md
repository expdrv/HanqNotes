# Econometrics  OLS textbook

### Claim 16
$s^2=(n-k)^{-1} \hat{\epsilon}^\intercal\epsilon$ is the unbiased estimator of $\sigma^2$.And theproof is written on textbook.

$trace(X(X^\intercal X)^{-1})X^\intercal)=trace((X^\intercal X)^{-1})XX^\intercal)=K$ <!--it's on footer lol-->

### Claim 17
gives a way to estimate $\hat{Var}(\hat{\beta})$

### Claim 18
$\hat{\beta}-\beta=(X^\intercal X)^{-1})X\epsilon=A\epsilon\sim N(A\Sigma A^\intercal)$ because $A\epsilon$ is the linear combination of $\epsilon$.

as for $(n-K)\frac{s^2}{\sigma^2}$, from [Green2007](M has to be an idenpotent matrix),we know that it follows the distribution.

for independece, they both follow normal distribution, so linear independence(showed in textbook) totally equals to independence.

## 2.4

$R^2=\frac{ESS}{TSS}=1-\frac{RSS}{TSS}=1-\frac{\hat{\epsilon}^\intercal\epsilon}{y^\intercal M_0y}$ and $M_0=I_n-ll^\intercal/n$ where $ll^\intercal$ is a matrix full of 1, this is the matrix form of deaveraged y.

the adjusted $R^2$ will weaken the effect of adding explaining variables, concentrating on model.

### Information Criterion

SIC and AIC

# OLS test
## 2.4 Constrained Least Squares

Uniside test is more likely to be signifigant Multiside test.

## 2.3.3 J Linear Restrictions (F/Wald Test)
should notice that F is better in small amount samples, with bigger observation, Wald could be as good.
discrepancy: difference

### Wald Test
$H_0:R\beta=c$ then $R(\hat{\beta}-\beta)$~$N(0,R\sigma^2(X^\intercal X)^{-1}R^\intercal)$

$R\hat{\beta}-c\sim N(0,R\sigma^2(X^\intercal X)^{-1}R^\intercal)$

according to [Green2012] $(\sigma^2)^{-1}(R\hat{\beta}-c)^\intercal (R(X^\intercal X)^{-1}R^\intercal)^{-1}(R\hat{\beta}-c)\sim{\chi}^2_{j}$

$(n-K)\frac{s^2}{\sigma^2}\sim \chi^2_{(n-K)}$

so the dividend follows the F-distribution.

## Non-Spherical Disturbances
- (A5**) 
- Example1 : Heteroskedasticity
- Example2 : Serial Correlation
- Example3 : Panel Data with Random Effect