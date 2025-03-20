# 2024年全国硕士研究生招生考试试题与答案（数学一）  

# 数学  

本试卷共4页，22题．全卷满分150分，考试用时120分钟  

# 注意事项：  

1.答卷前，考生务必将自己的姓名、准考证号填写在答题卡上.  
2.回答选择题时，用铅笔把答题卡上对应题目的答案标号涂黑，写在本试卷上无效.  
3.考试结束后，将本试卷和答题卡一并交回.  
4.本试卷由kmath.cn自动生成.  

<td><table  border="1"><thead><tr><td><b>得分</b></td><td></td></tr></thead><tbody><tr><td>阅卷人</td></tr></tbody></table></td>  

# 一、单选题：本题共10小题，每小题5分，共40分．在每小题给出的四个选项中，只有一项是符合题目要求的。  

1．已知函数 $f(x)=\int_{0}^{x}e^{\cos t}d t,g(x)=\int_{0}^{\sin x}e^{t^{2}}d t,$ 则  

A. $f(x)$ 是奇函数， $g(x)$ 是偶函数B. $f(x)$ 足偶函数， $g(x)$ 足奇函数C. $f(x)$ 与 $g(x)$ 均为奇函数D. $f(x)$ 与 $g(x)$ 均为周期函数  

[答案]:C[解析]：【解析】由于 $e^{\cos t}$ 是偶函数，所以 $f(x)=\int_{0}^{x}e^{\cos t}d t$ 是奇函数，又 $g^{\prime}(x)=e^{(\sin x)^{2}}\cos x$ 是偶函数，所以 $g(x)$ 是奇函数.故选C.  

2.设 $P=P(x,y,z)\Omega Q=Q(x,y,z)$ 均为连续函数, $\sum$ 为曲面 $Z={\sqrt{1-x^{2}-y^{2}}}(x\leqslant0,y\geqslant0)$ 的上侧，则  

$$
\begin{array}{l}{\displaystyle{\left\iint_{S}P d y d z+Q d z d x=\right.}}\\ {\displaystyle{\left\iint_{S}\left(\frac{x}{z}P+\frac{y}{z}Q\right)d x d y}}\\ {\displaystyle{\left\iint_{S}\left(\frac{x}{z}P-\frac{y}{z}Q\right)d x d y}}\end{array}
$$  

[答案]:A [解析]:【解析】转换投影法,  $z=\sqrt{1-x^{2}-y^{2}},\frac{\partial z}{\partial x}=-\frac{x}{z},\frac{\partial z}{\partial y}=-\frac{y}{z}$  

$$
\iint_{\Sigma}P d y d z+Q d z d x=\iint_{\Sigma}\left(\frac{x}{z}P+\frac{y}{z}Q\right)d x d y
$$  

故选A.  

3.已知幂级数  $\sum_{n=0}^{\infty}a_{n}x^{n}$  的和函数为  $\ln(2+x)$  ，则  $\sum_{n=0}^{\infty}n a_{2n}=$  

$-{\frac{1}{6}}$  1  $\frac{1}{6}$  1 A. B. C D. 3 3  

[答案]:A[解析]：【解析】方法1: $\ln(2+x)=\ln2\left(1+{\frac{1}{2}}x\right)=\ln2+\ln\left(1+{\frac{1}{2}}x\right)$  

$$
=\ln2+\sum_{n=1}^{\infty}(-1)^{n-1}{\frac{\left({\frac{1}{2}}x\right)^{n}}{n}}
$$  

所以, $a_{n}\,=\,\left\{\begin{array}{c l}{{\ln2,}}&{{n=0}}\\ {{(-1)^{n-1}{\frac{1}{n2^{n}}},}}&{{n>0}}\end{array}\right.$ 当 $n\,>\,0,a_{2n}\,=\,-\frac{1}{2n\cdot2^{2n}}$ 所以， $\sum_{n=0}^{\infty}n a_{2n}\,=\,\sum_{n=1}^{\infty}n a_{2n}\,=$  $\sum_{n=1}^{\infty}n\cdot\left(-{\frac{1}{2n\cdot2^{2n}}}\right)=-\sum_{n=1}^{\infty}{\frac{1}{2^{2n+1}}}=-{\frac{\left({\frac{1}{2}}\right)^{3}}{1-{\frac{1}{4}}}}=-{\frac{1}{6}}$ 故选A.方法 2:  

$$
[\ln(2+x)]^{\prime}={\frac{1}{2+x}}={\frac{1}{2\left(1+{\frac{x}{2}}\right)}}={\frac{1}{2}}\sum_{n=0}^{\infty}(-1)^{n}\left({\frac{x}{2}}\right)^{n}
$$  

$$
\ln(2+x)=\sum_{n=0}^{\infty}(-1)^{n}{\frac{{\big(}{\frac{1}{2}}x{\big)}^{n+1}}{n+1}}+C=\sum_{n=1}^{\infty}(-1)^{n-1}{\frac{{\big(}{\frac{1}{2}}x{\big)}^{n}}{n}}+C
$$  

$$
S(0)=C=\ln(2+0)=\ln2
$$  

$a_{n}=\left\{\begin{array}{c c}{{\ln2,}}&{{n=0}}\\ {{(-1)^{n-1}{\frac{1}{n2^{n}}},}}&{{n>0}}\end{array}\right.$  

$\sum_{n=0}^{\infty}n a_{2n}=\sum_{n=1}^{\infty}n a_{2n}=\sum_{n=1}^{\infty}n\cdot\left(-{\frac{1}{2n\cdot2^{2n}}}\right)=-\sum_{n=1}^{\infty}{\frac{1}{2^{2n+1}}}=-{\frac{\left({\frac{1}{2}}\right)^{3}}{1-{\frac{1}{4}}}}=-{\frac{1}{6}}$  

4.设函数  $f(x)$  在区间  $(-1,1)$  上有定义，且  $\operatorname*{lim}_{x\to0}f(x)=0$  则  

A.当 $\operatorname*{lim}_{x\to0}{\frac{f(x)}{x}}=m$ 时， $f^{\prime}(0)=m$ B.当 $f^{\prime}(0)=m$ 时， $\operatorname*{lim}_{x\to0}{\frac{f(x)}{x}}=m$ C.当 $\operatorname*{lim}_{x\to0}f^{\prime}(x)=m$ 时， $f^{\prime}(0)=m$ D.当 $f^{\prime}(0)=m$ 时， $\operatorname*{lim}_{x\to0}f^{\prime}(x)=m$  

[答案]:B[解析]【解析】因为  $f^{\prime}(0)=m$  所以  $f(x)$  在  $x=0$  处连续，从而  $\operatorname*{lim}_{x\to0}f(x)=f(0)=0$  所以  $\operatorname*{lim}_{x\to0}{\frac{f(x)}{x}}=\operatorname*{lim}_{x\to0}{\frac{f(x)-f(0)}{x-0}}=m,$  故选B.  

对于 A 选项, $\operatorname*{lim}_{x\rightarrow0}{\frac{f(x)}{x}}=m$ 推不出来 $f^{\prime}(0)=m$ ；对于 $\mathrm{C}$ 选项， $f^{\prime}(x)$ 在 $x=0$ 处不一定连续；对于D 选项, $f^{\prime}(x)$ 在 $x=0$ 处极限末必存在,  

5．在空间直角坐标系 $O-x y z$ 中，三张平面 $\pi_{i}:a_{i}x+b_{i}y+c_{i}z=d_{i}(i=1,2,3)$ 的位置关系如图所示,记  $\alpha_{i}=(a_{i},b_{i},c_{i},d_{i})$  ，若  $r\left(\begin{array}{c}{{\alpha_{1}}}\\ {{\alpha_{2}}}\\ {{\alpha_{3}}}\end{array}\right)=m,r\left(\begin{array}{c}{{\beta_{1}}}\\ {{\beta_{2}}}\\ {{\beta_{3}}}\end{array}\right)=n,$  则  

![](images/08140eb433352ce2a810d1a4c1f6591a07ff30c96863ee66ba630416224a428b.jpg)  

A.m=1,n=2 B.  $m=n=2$  C.  $m=2,n=3$  D.  $m=n=3$  