10. Proof. We omit (a) since is standard. For (b), if $u$ attains an interior maximum, then the conclusion follows from strong maximum principle.
If not, then for some $x^{0} \in \partial U, u\left(x^{0}\right)>u(x) \forall x \in U$. Then Hopf's lemma implies $\frac{\partial u}{\partial v}\left(x^{0}\right)>0$, which is a contradiction.

Remark 2. A generalization of this problem to mixed boundary conditions is recorded in Gilbarg-Trudinger, Elliptic PDEs of second order, Problem 3.1.
11. Proof. Define

$$
B[u, v]=\int_{U} \sum_{i, j} a^{i j} u_{x_{i}} v_{x_{j}} d x \text { for } u \in H^{1}(U), v \in H_{0}^{1}(U)
$$

By Exercise $5.17, \phi(u) \in H^{1}(U)$. Then, for all $v \in C_{c}^{\infty}(U), v \geq 0$,

$$
\begin{aligned}
B[\phi(u), v] & =\int_{U} \sum_{i, j} a^{i j}(\phi(u))_{x_{i}} v_{x_{j}} d x \\
& =\int_{U} \sum_{i, j} a^{i j} \phi^{\prime}(u) u_{x_{i}} v_{x_{j}} d x,\left(\phi^{\prime}(u) \text { is bounded since } u \text { is bounded }\right) \\
& =\int_{U} \sum_{i, j} a^{i j} u_{x_{i}}\left(\phi^{\prime}(u) v\right)_{x_{j}}-\sum_{i, j} a_{i j} \phi^{\prime \prime}(u) u_{x_{i}} u_{x_{j}} v d x \\
& \leq 0-\int_{U} \phi^{\prime \prime}(u) v|D u|^{2} d x \leq 0, \text { by convexity of } \phi
\end{aligned}
$$

(We don't know whether the product of two $H^{1}$ functions is weakly differentiable. This is why we do not take $v \in H_{0}^{1}$.) Now we complete the proof with the standard density argument.
12. Proof. Given $u \in C^{2}(U) \cap C(\bar{U})$ with $L u \leq 0$ in $U$ and $u \leq 0$ on $\partial U$. Since $\bar{U}$ is compact and $v \in C(\bar{U}), v \geq c>0$. So $w:=\frac{u}{v} \in C^{2}(U) \cap C(\bar{U})$. Brutal computation gives us

$$
\begin{aligned}
-a^{i j} w_{x_{i} x_{j}} & =\frac{-a^{i j} u_{x_{i} x_{j}} v+a^{i j} v_{x_{i} x_{j}} u}{v^{2}}+\frac{a^{i j} v_{x_{i}} u_{x_{j}}-a^{i j} u_{x_{i}} v_{x_{j}}}{v^{2}}-a^{i j} \frac{2}{v} v_{x_{j}} \frac{v_{x_{i}} u-v u_{x_{i}}}{v^{2}} \\
& =\frac{\left(L u-b^{i} u_{x_{i}}-c u\right) v+\left(-L v+b^{i} v_{x_{i}}+c v\right) u}{v^{2}}+0+a^{i j} \frac{2}{v} v_{x_{j}} w_{x_{i}}, \text { since } a^{i j}=a^{j i} \\
& =\frac{L u}{v}-\frac{u L v}{v^{2}}-b^{i} w_{x_{i}}+a^{i j} \frac{2}{v} v_{x_{j}} w_{x_{i}}
\end{aligned}
$$

Therefore,

$$
M w:=-a^{i j} w_{x_{i} x_{j}}+w_{x_{i}}\left[b^{i}-a^{i j} \frac{2}{v} v_{x_{j}}\right]=\frac{L u}{v}-\frac{u L v}{v^{2}} \leq 0 \text { on }\{x \in \bar{U}: u>0\} \subseteq U
$$

If $\{x \in \bar{U}: u>0\}$ is not empty, Weak maximum principle to the operator $M$ with bounded coefficeints (since $v \in C^{1}(\bar{U})$ ) will lead a contradiction that

$$
0<\max _{\{u>0\}} w=\max _{\partial\{u>0\}} w=\frac{0}{v}=0
$$

Hence $u \leq 0$ in $U$.