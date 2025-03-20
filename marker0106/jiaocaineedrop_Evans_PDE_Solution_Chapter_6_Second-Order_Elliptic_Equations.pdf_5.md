- 10. Proof. We omit (a) since is standard. For (b), if u attains an interior maximum, then the conclusion follows from strong maximum principle.
If not, then for some xº E dU, u(xº) > u(x) Vx ∈ U. Then Hopf's lemma implies ¶(xº) > 0, □ which is a contradiction.

Remark 2. A generalization of this problem to mixed boundary conditions is recorded in Gilbarg-Trudinger, Elliptic PDEs of second order, Problem 3.1.

- 11. Proof. Define

$$B[u,v]=\int_{U}\sum_{i,j}a^{i j}u_{x_{i}}v_{x_{j}}\,d x\ \mathrm{for}\ u\in H^{1}(U),v\in H^{1}_{0}(U).$$

By Exercise 5.17, ¢(u) € H+(U). Then, for all v E C (U), v ≥ 0,

$$B[\phi(u),v]=\int_{U}\sum_{i,j}a^{ij}(\phi(u))_{x_{i}}v_{x_{j}}\,dx$$
 
$$=\int_{U}\sum_{i,j}a^{ij}\phi^{\prime}(u)u_{x_{i}}v_{x_{j}}\,dx,\,(\phi^{\prime}(u)\text{is bounded since u is bounded})$$
 
$$=\int_{U}\sum_{i,j}a^{ij}u_{x_{i}}(\phi^{\prime}(u)v)_{x_{j}}-\sum_{i,j}a_{ij}\phi^{\prime\prime}(u)u_{x_{i}}u_{x_{j}}v\,dx$$
 
$$\leq0-\int_{U}\phi^{\prime\prime}(u)v|Du|^{2}\,dx\leq0,\text{by convexity of}\phi.$$

(We don't know whether the product of two H+ functions is weakly differentiable. This is why we do not take v ∈ H☆.) Now we complete the proof with the standard density argument. 

- 12. Proof. Given u € C2(U) C(U) with Lu ≤ 0 in U and u ≤ 0 on aU. Since U is compact and v E C(U), v ≥ c > 0. So w := ; ∈ C2(U) ∩C(U). Brutal computation gives us

$$-a^{ij}w_{x_{i}x_{j}}=\frac{-a^{ij}u_{x_{i}x_{j}}v+a^{ij}v_{x_{i}x_{j}}u}{v^{2}}+\frac{a^{ij}v_{x_{i}}u_{x_{j}}-a^{ij}u_{x_{i}}v_{x_{j}}}{v^{2}}-a^{ij}\frac{2}{v}v_{x_{i}}\frac{v_{x_{i}}u-vu_{x_{i}}}{v^{2}}$$
 
$$=\frac{(Lu-b^{i}u_{x_{i}}-cu)v+(-Lv+b^{i}v_{x_{i}}+cv)u}{v^{2}}+\mathbb{O}+a^{ij}\frac{2}{v}v_{x_{i}}w_{x_{i}},\text{since}a^{ij}=a^{ji}.$$
 
$$=\frac{Lu}{v}-\frac{uLv}{v^{2}}-b^{i}w_{x_{i}}+a^{ij}\frac{2}{v}v_{x_{j}}w_{x_{i}}$$

Therefore,

$$Mw:=-a^{ij}w_{x_{i}x_{j}}+w_{x_{i}}[b^{i}-a^{ij}\frac{2}{v}v_{x_{j}}]=\frac{Lu}{v}-\frac{uLv}{v^{2}}\leq0\;\;\mbox{on}\;\{x\in\bar{U}:u>0\}\subseteq U.$$

If {x E U : u > 0} is not empty, Weak maximum principle to the operator M with bounded coefficeints (since v E C+(U)) will lead a contradiction that

0 < max w = max w = 0<u>0} 10×1

■

Hence u < 0 in U.

