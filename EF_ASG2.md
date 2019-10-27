<script type="text/javascript"
       src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>

# <center><font size =10>Economics Assignment2</font></center><font size=5>
## &#8544;.
$SARP$ suggests that all elements in the choice set make up some graphs without direction, and there is no circle in the graphs. In other words, the preference relationships between nodes(choices) are transtive and nonreversible. <center>$\neg WARP:\exists x_1{\succ}_dx_2, \  x_2{\succ}_dx_1 \\ \neg SARP:\exists x_1{\succ}_r x_1 \\ \neg WARP\Longrightarrow \neg SARP \\ SARP \Longrightarrow WARP$.</center> 
 
But not vise versa cause we can give samples as follwing:
</font>
|$Choice, Price$ |$P_1=(3,4,5)$|$P_2=(4,5,3)$|$P_3=(5,3,4)$|
|----------------|------------|------------|------------|
|$x_1=(3,4,5)$    |$50$        |$47*$       |$47$        |
|$x_2=(5,3,4)$    |$47*$       |$47$        |$50$        |
|$x_3=(4,5,3)$    |$47$        |$50$        |$47*$       |
<font size=5>In this case, the consumer choose  $x_1$ under $P_2$,$x_2$ under $P_1$, $x_3$ under $P_3$.
it's intuitive that: <center>$x_1{\succ}_dx_2, \  x_2{\succ}_dx_3, \ x_3{\succ}_dx_1$</center> 
It's consistent with $WARP$ but against $SARP$ because we can infer from the case that:<center>$x_1{\succ}_rx_1, \  x_2{\succ}_rx_2, \ x_3{\succ}_rx_3$</center> 

## &#8545;.
### Shephard's lemma
We have<center>$e(p,x)=px^*$ where  $x*\in H(p,x)$</center>
so that means <center>$u=\prod_{i=1}^n x_i^{*\alpha_i} =U$ 
 and $L=\sum p_i x_i+\lambda (\prod x_i^{\alpha_i}-U)$</center>
 differentiate this Lagrangian function and we get:<center>
 $\frac{\partial L}{\partial x_i}=p_i+\alpha_i\lambda x_1^{\alpha_1}x_2^{\alpha_2}...x_i^{1-\alpha_i}..x_n^{\alpha_n}=0\\ \frac{p_i x_i}{p_j x_j}=\frac{\alpha_i}{\alpha_j}\\\frac{p_i x_i}{p_1 x_1}=\frac{\alpha_i}{\alpha_1} \\ x_i=\frac{p_1x_1\alpha_i}{\alpha_1p_i} \\ \\  \prod x_i^{\alpha_i}=\frac{p_1x_1\prod \alpha_i^{\alpha_i}}{\alpha_1 \prod p_i^{\alpha_i}}=U $  </center>
 and we know that<center>
 $p_1x_1^*=\frac{U\alpha_1\prod p_i^{\alpha_i}}{\prod \alpha_i^{\alpha_i}} \\ \frac{\partial e(p,x)}{\partial p_1}=\frac{U\alpha_1\alpha_1 \frac{\prod p_i^{\alpha_i}}{p_1}}{\prod \alpha_i^{\alpha_i}}+\frac{U\alpha_2\alpha_1 \frac{\prod p_i^{\alpha_i}}{p_1}}{\prod \alpha_i^{\alpha_i}}+... \\ =\frac{U\alpha_1\sum \alpha_i \frac{\prod p_i^{\alpha_i}}{\prod \alpha_i^{\alpha_i}}}{p_1}=\frac{U\alpha_1\frac{\prod p_i^{\alpha_i}}{\prod \alpha_i^{\alpha_i}}}{p_1}=x_1^*\\ so \  \frac{\partial e(p,x)}{\partial p_i}=x_i^*. QED.$  

 </center>


### Roy's Identity

Without loss of generality, say the consumer consumes goods $(x_1,x_2)$ under $(P_1,P_2)$. and the $v(p,w)$ in Cobb-Douglas form is $u=x_1^{*\alpha} x_2^{*1-\alpha}$. And to maximize his utility, he should run out of his budget so $w=P_1 x_1+P_2 x_2$ and by calculation in Shephard's lemma, $\frac{p_1x_1^*}{p_2x_2^*}=\frac{\alpha_1}{\alpha_2},x_1^*=\frac{\alpha_1w}{P_1},x_2^*=\frac{\alpha_2w}{P_1}$
so <center>$v(p_1,w)=(\frac{\alpha w}{P_1})^{\alpha} (\frac{(1-\alpha)w }{P_2})^{1-\alpha} \\ -\frac{\partial v(p_1,w)/\partial p_1}{\partial v(p_1,w)/\partial w}=x_1^* \\ -\frac{\partial v(p_2,w)/\partial p_2}{\partial v(p_2,w)/\partial w}=x_2^*$ </center>
Where $(x_1^*, x_2^*)\in D(p,w)$, so Roy's Identity by now is verified. 


## &#8546;.
When $\pi=q$, assume that one will spend $qv$ on insurance and the expected wealth of this one is:<center>$E(w)=(1-\pi)(w-vq)+\pi(w-vq-l+v)$
$=w-\pi l$</center>
So no matter how much insurance one buys, his expected wealth stays indifferent. And  there is a low with the  $ \ vNW $ utility:<center>$u(E(w))\geq E(u(w))$</center>
One will buy insurance worthy of $\pi l$, which means $v=l$ to maximize his utility and here his loss is fully covered because: <center>$w_{occur}=w_{not occur}=w-\pi l=w-\pi l-l+\frac{\pi l}{q}$</center>
But when $q>\pi$, things are different, if this one  buys insurance worthy of $qv$, his expected wealth is:<center>$E(w)=(1-\pi)(w-vq)+\pi(w-vq-l+v)$
$=w-\pi l-(q-\pi)v$</center>
If he still buys insurance in which $v=l$ to fully cover his potential loss, his expected wealth is $E(w)=w-ql$ ,less than $w-\pi l$.
And we differentiate the $vNW$ utility function at this point: <center>$
\frac{\partial E(u(w;v))}{\partial v}=(1-\pi )u\prime(w-vq)(-q)+ \\ \pi (1-q)u\prime (w-vq-l+v)\\=\pi(1-q)u\prime(w-ql)-q(1-\pi)u\prime(w-ql)$</center>
And for $q>\pi$, $\ 
\frac{\partial E(u(w;v))}{\partial v}<0$.
So one will buy less than $ql$ insurance and then his potential loss will not be fully covered.
</font>
<hr/>
<div style="width:600px;height:120px; margin:auto;border:0px solid black">
            <div style="float: left;border:0px  paleturquoise">
                <img src="Hanqing.jpeg"style="width:400px">
            </div>
            <div style="font-size:24px;text-align: center;margin-top: 15px; float:left;">
                杜瑞琛 <br/>
                2019100505<br/>
                drcuibe@163.com
            </div>
        </div>