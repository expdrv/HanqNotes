<script type="text/javascript"
       src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>

<style>
*{
    font-family:'Segoe UI';
    font-size:25px
}
</style>
# Macro Economics Ch1
## Solow Growth Model
2 perspectives$\begin{cases}
    time \ \ series\\
    cross \ \ sectional
\end{cases}$
    

## Assumption:
 $Y_t=F(K_t,A_tL_t)$ (production function) 
$A_t$ is ```Knowledge``` as well as ```effectiveness of labor```
$A_tL_t$ is ```effective labor```
### Aside:
$Y=F(KL)$: ```labor arrangement``` or ```harrod neutral``` 
$Y=F(AK,L)$:```capital arrangement```
$Y=AF(K,L)$:```Hicks neutral```
$Y=F(K,A,L)$
### Constant return to scale

$F(cK,cAL)=cF(K,AL)$

```more realistic for large economy```
$\frac{1}{AL}F(K,AL)=F(\frac{K}{AL},1)$
define $k=\frac{K}{AL}$,```capital per unit ofeffective labor```
$y=\frac{Y}{AL}=F(k,1)=f(k)$ ```return per ...```

### Assumption on f

$f(0)=0,\ f(k)^\prime>0,\ f(k)^{\prime\prime}<0$

### Exercise:

prove that $\frac{\partial F(K,AL)}{\partial K}=f\prime(k)$

### More restrictions on f(k)

Inada Condition: 
$\lim\limits_{k \to \infty}f\prime(k)=0,\lim\limits_{k \to0}f\prime(k)=\infty$
### Cobb-Douglas function

$F(K,AL)=K^\alpha (AL)^{1-\alpha}$

## Exogenous Growth rate of labor & knowledge

$\dot{L}(t)=nL(t),\dot{A}(t)=gA(t)$
for $\dot{F}(t)=\frac{\partial F(t)}{\partial t}$

```!!!!!```$\frac{\dot{A(t)L(t)}}{A(t)L(t)}=g+n$```!!!!!```


## Exogenous saving rate s saving rate s is constant across time(strong assumption)

```Exogenous is strong because it simplized the model```
```constant across time is strong for similar reason```

capital depreciation rate $\delta>0$
dynamics of capital: $\dot{K_t}=sY_t-\delta K_{t}$

### investigate of dynamics of  $\dot{k_t}$
$\dot{k_t}=\frac{\partial k(t)}{\partial t}=\frac{\partial\frac{K(t)}{AL(t)}}{\partial t}=\frac{AL(t)\dot{K}(t)-K(t)AL\prime(t)}{AL^2(t)}=\frac{\dot{K(t)}}{AL(t)}-\frac{(g+n)K(t)}{AL(t)}=sy(t)-\delta k(t)-(g+n)k(t)$

$=sy(t)-(g+n+\delta)k(t) $
first part is called extra investment
the second part is called break even investment 


### phase diagram for solow model

## Balanced Growth Path

$K,Y,Y/K,Y/L,K/L$
$\underline{K}=AL(t)k^*(t)$
$\underline{Y}=AL(t)y^*(t)$
$\underline{Y}/K=y^*/k^*$
$\underline{Y}/L=A(t)y^* \to g$
$\underline{K}/L=A(t)k^* \to g$ ```!!!!!!!!!!!!!!!```
 
so it's clear that capital accumulation can't result in sustainable growth. what's important is g&n

## Balanced growth path
<img style="width: 400px" src="200px-solow_growth_model2.png">

### Exercise graph for $\ln(\underline{Y}/L)$

### Conclusion: 
```a change in saving rate has a level effect but not a growth effect```

## the impact on consumption c
