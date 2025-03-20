10. Proof. We omit (a) since is standard. For (b), if  $u$   attains an interior maximum, then the conclusion follows from strong maximum principle.  

If not, then for some  $x^{0}\in\partial U,u(x^{0})>u(x)\ \forall x\in U$  . Then Hopf's lemma implies  ${\frac{\partial u}{\partial\nu}}(x^{0})>0$  which is a contradiction.  

Remark 2. A generalization of this problem to mixed boundary conditions is recorded in Gilbarg- Trudinger, Elliptic PDEs of second order, Problem 3.1.  

11. Proof. Define  

$$
B[u,v]=\int_{U}\sum_{i,j}a^{i j}u_{x_{i}}v_{x_{j}}\,d x\mathrm{~for~}u\in H^{1}(U),v\in H_{0}^{1}(U).
$$  

By Exercise 5.17,  $\phi(u)\in H^{1}(U)$  . Then, for all  $v\in C_{c}^{\infty}(U),\,v\geq0$  

$$
\begin{array}{r l r}{\lefteqn{B[\phi(u),v]=\int_{U}\sum_{i,j}a^{i j}(\phi(u))_{x_{i}}v_{x_{j}}\,d x}}\\ &{}&{=\int_{U}\sum_{i,j}a^{i j}\phi^{\prime}(u)u_{x_{i}}v_{x_{j}}\,d x,\;(\phi^{\prime}(u)\mathrm{~is~bounded~since~u~is~bounded})}\\ &{}&{=\int_{U}\sum_{i,j}a^{i j}u_{x_{i}}(\phi^{\prime}(u)v)_{x_{j}}-\sum_{i,j}a_{i j}\phi^{\prime\prime}(u)u_{x_{i}}u_{x_{j}}v\,d x}\\ &{}&{\le0-\int_{U}\phi^{\prime\prime}(u)v|D u|^{2}\,d x\le0,\;\mathrm{by~convexity~of}\;\phi.}\end{array}
$$  

(We don't know whether the product of two  $H^{1}$  functions is weakly differentiable. This is why we do not take  $v\in H_{0}^{1}$  ) Now we complete the proof with the standard density argument.  

12. Proof. Given  $u\in C^{2}(U)\cap C(\bar{U})$  with  $L u\le0$  in  $U$   and  $u\leq0$  on  $\partial U$  .Since  $\bar{U}$  is compact and  $v\in C(\bar{U})$  ，  $v\geq c>0$  . So  $\begin{array}{r}{w:=\frac{u}{v}\in C^{2}(U)\cap C(\bar{U})}\end{array}$  . Brutal computation gives us  

$$
{\begin{array}{r l}&{-a^{i j}w_{x_{i}x_{j}}={\frac{-a^{i j}u_{x_{i}x_{j}}v+a^{i j}v_{x_{i}x_{j}}u}{v^{2}}}+{\frac{a^{i j}v_{x_{i}}u_{x_{j}}-a^{i j}u_{x_{i}}v_{x_{j}}}{v^{2}}}-a^{i j}{\frac{2}{v}}v_{x_{j}}{\frac{v_{x_{i}}u-v u_{x_{i}}}{v^{2}}}}\\ &{\qquad={\frac{(L u-b^{i}u_{x_{i}}-c u)v+(-L v+b^{i}v_{x_{i}}+c v)u}{v^{2}}}+0+a^{i j}{\frac{2}{v}}v_{x_{j}}w_{x_{i}},{\mathrm{~since~}}a^{i j}=1}\\ &{\qquad={\frac{L u}{v}}-{\frac{u L v}{v^{2}}}-b^{i}w_{x_{i}}+a^{i j}{\frac{2}{v}}v_{x_{j}}w_{x_{i}}}\end{array}}
$$
  $a^{i j}=a^{j i}$  

Therefore,  

$$
{\cal M}w:=-a^{i j}w_{x_{i}x_{j}}+w_{x_{i}}\big[b^{i}-a^{i j}{\textstyle\frac{2}{v}}v_{x_{j}}\big]={\frac{L u}{v}}-{\frac{u L v}{v^{2}}}\le0\;\;\mathrm{on}\;\big\{x\in{\bar{U}}:u>0\big\}\subseteq{\cal U}
$$  

If  $\{x\in U:u>0\}$  is not empty, Weak maximum principle to the operator  $M$  with bounded coefficeints (since  $v\in C^{1}(U)$  ) will lead a contradiction that  

$$
0<\operatorname*{max}_{\{\overline{{u>0}}\}}w=\operatorname*{max}_{\partial\{u>0\}}w=\frac{0}{v}=0
$$  

Hence  $u\leq0$  in  $U$  