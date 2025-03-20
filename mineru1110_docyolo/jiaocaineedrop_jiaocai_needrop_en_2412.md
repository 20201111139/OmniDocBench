设  $u\left(x\right)=\ln\left(x+1\right)-x\;,$  则  $u^{\prime}\!\left(x\right)\!=\!\frac{1}{x+1}\!-\!1\!=\!\frac{-x}{x+1}\,,$    
所以当 $-1<x<0$ 时， $u^{\prime}(x)>0$ ：当 $x>0$ 时， $u^{\prime}(x)\!<\!0$ 所以 $u\left(x\right)$ 在 $(-1,0)$ 上为增函数，在 $(0,+\infty)$ 上为减函数，  
故 $u\left(x\right)_{\mathrm{max}}=u\left(0\right)=0$ ，所以 $\ln{\bigl(}x+1{\bigr)}\leq x$ 成立.由上还不等式可得，当 $t>1$ 时， $\ln{\left(1+\frac{1}{t}\right)}\le\frac{1}{t}<\frac{2}{t+1}$ 故 $S^{\prime}(t)\!<\!0$ 恒成立,故  $S\left(t\right)$  在  $(1,+\infty)$  上为减函数，则  $S\left(t\right)<S\left(1\right)=0$    
所以 $\left(t-1\right)\ln\left(t+1\right)-t\ln t<0$ 成立，即 $x_{1}+x_{2}<e$ 成立.综上所述， $\ln\left(a+b\right)<\ln\left(a b\right)+1$  

核心考点五：极最值问题  

# 【规律方法】  

利用导数求函数的极最值问题．解题方法是利用导函数与单调性关系确定单调区间，从而求得极最值．只是对含有参数的极最值问题，需要对导函数进行二次讨论，对导函数或其中部分函数再一次求导，确定单调性，零点的存在性及唯一性等，由于零点的存在性与参数有关，因此对函数的极最值又需引入新函数，对新函数再用导数进行求值、证明等操作.  

# 【典型例题】  

3春·江西鹰潭·高三贵溪市实验中学校考阶段练习）已知函数 $f\left(x\right)={\frac{1}{3}}x^{3}-a x+a,a\in\mathbf{R}$  

(1)当 $a=-1$ 时，求 $f\left(x\right)$ 在 $[-2,2]$ 上的最值；  
(2)讨论  $f\left(x\right)$  的极值点的个数. 【解析】（1）当 $a=-1$ 时， $f(x)\!=\!\frac{1}{3}x^{3}\!+\!x\!-\!1,~~x\!\in\![-2,2]$   
 $f^{\prime}(x)=x^{2}+1>0$ ，故 $f\left(x\right)$ 在[-2, 2] 上单调递增， $\therefore f\left(x\right)_{\mathrm{min}}=f\left(-2\right)=-{\frac{17}{3}}{\mathrm{\boldmath~\nabla~}}\cdot f\left(x\right)_{\mathrm{max}}=f\left(2\right)={\frac{11}{3}}.$    
(2)  $f^{'}(x)=x^{2}-a\,,$   $\textcircled{1}$ 当 $a\!\lesssim\!0$ 时, $f^{\prime}(x)\geq0$ 恒成立,此时 $f(\v{x})$ 在 $\mathbf{R}$ 上单调递增，不存在极值点.  
 $\circled{2}$ 当 $a>0$ 时,令 $f^{\prime}(x)>0$ ,即 $x^{2}-a>0$ ，解得： $x<-{\sqrt{a}}$ 或 $x>{\sqrt{a}}$ 令  $f^{\prime}(x)<0$  ,即  $\ x^{2}-a<0$  ，解得  $x\in(-{\sqrt{a}},{\sqrt{a}})$    
故此时 $f(x)$ 在 $(-\infty,-\sqrt{a})$ 递增,在 $(-{\sqrt{a}},{\sqrt{a}})$ 递减,在 $(\sqrt{a},+\infty)$ 递增，所以 $f(x)$ 在 $x=-{\sqrt{a}}$ 时取得极大值，在 $x={\sqrt{a}}$ 时取得极小值，故此时极值点个数为2，综上所述： $a{\leq}0$ 时， $f(x)$ 无极值点，  