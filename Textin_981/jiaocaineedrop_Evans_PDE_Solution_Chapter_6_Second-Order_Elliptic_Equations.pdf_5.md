## 10.Proof. We omit (a) since is standard. For (b), if u attains an interior maximum, then the conclusion follows from strong maximum principle.

If not,then for some$x^{0}\in \partial U,u(x^{0})>u(x)\forall x\in U$. Then Hopf's lemma implies $\frac {\partial u}{\partial v}(x^{0})>0,$which is a contradiction. □

Remark 2. A generalization of this problem to mixed boundary conditions is recorded in Gilbarg-Trudinger,Elliptic PDEs of second order, Problem 3.1.

11.Proof. Define

$B[u,v]=\int _{U}\sum _{i,j}a^{ij}u_{x_{i}}v_{x_{j}}dxforu\in H^{1}(U),v\in H_{0}^{1}(U).$

By Exercise 5.17,$\phi (u)\in H^{1}(U)$.Then,for all$v\in C_{c}^{\infty }(U),v\geq 0,$

$B[\phi (u),v]=\int _{U}\sum _{i,j}a^{ij}(\phi (u))x_{i}v_{xj}dx$

$=\int _{U}\sum _{i,j}a^{ij}\phi ^{\prime }(u)u_{x_{i}}v_{x_{j}}dx,(\phi ^{\prime }(u)$is bounded since u is bounded)

$=\int _{U}\sum _{i,j}a^{ij}u_{x_{i}}(\phi ^{\prime }(u)v)x_{j}-\sum _{i,j}a_{ij}\phi ^{\prime \prime }(u)u_{x_{i}}u_{x_{j}}vdx$

$\leq 0-\int _{U}\phi ^{\prime \prime }(u)v\vert Du\vert ^{2}dx\leq 0,$byconvexityofφ.

(We don't know whether the product of two H1 functions is weakly differentiable. This is why we do not take$v\in H_{0}^{1}.)$ Now we complete the proof with the standard density argument. □

12. Proof. Given$u\in C^{2}(U)\cap C(\overline {U})$ withLu≤0inUandu≤0on∂U.Since Uis compact and $v\in C(\overline {U}),$v≥c&gt;0.$.Sow:=\frac {u}{v}\in C^{2}(U)\cap C(\overline {U})$. Brutal computation gives us

$-a^{ij}vv_{x,x_{1}}v_{x,x_{1}}=\frac {-a^{ij}v_{x,x_{1},v}v+a^{ij}v_{x,x_{1},v_{3}}{v^{2}}-a^{ij}v_{x_{1$

$=\frac {(Lu-b^{i}u_{x_{i}}-calv+(-Lv+b^{i}v_{x_{i}}+cv)u}{v^{2}}+0+a^{ij}\frac {2}{v}v_{x_{i}}v_{x_{i}},\sin eee^$

$=\frac {Lu}{v}-\frac {uLv}{v^{2}}-b^{i}w_{x_{i}}+a^{ij}\frac {2}{v}v_{x_{j}}w_{x_{i}}$

Therefore,

$Mw:=-a^{ij}w_{x_{i}x_{j}}+w_{x_{i}}[b^{i}-a^{ij}\frac {2}{v}v_{x_{j}}]=\frac {Lu}{v}-\frac {uLv}{v^{2}}\leq 0$on$\{x\in \overline {U}:u>0\}\subseteq U$

If$\{x\in \overline {U}:u>0\}$is not empty, Weak maximum principle to the operator M with bounded coefficeints(since$v\in C^{1}$ $(\overline {U}))$will lead a contradiction that

$0<\max _{\{\overline {u}>0\}}w=\max _{\partial \{u>0\}}w=\frac {0}{v}=0$

Henceu≤0∈U.

