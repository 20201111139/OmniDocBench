```markdown
10. **Proof.** We omit (a) since is standard. For (b), if \( u \) attains an interior maximum, then the conclusion follows from strong maximum principle.

If not, then for some \( x^0 \in U, u(x^0) > u(x) \forall x \in U \). Then Hopf's lemma implies \( \frac{2\mu}{\partial \nu} (x^0) > 0 \), which is a contradiction.

**Remark 2.** A generalization of this problem to mixed boundary conditions is recorded in Gilbarg-Trudinger. *Elliptic PDEs of second order, Problem 3.1.*

11. **Proof Define**
\[ B[u,v] = \int_U \sum_{i,j} a^{ij} u_{x_i} v_{x_j} \, dx \text{ for } u \in H^1(U), v \in H^1_0(U). \]

By Exercise 5.17, \( \phi(u) \in H^1(U) \). Then, for all \( v \in C^\infty_0(U), v \geq 0 \),

\[
\begin{aligned}
B[\phi(u), v] &= \int_U \sum_{i,j} a^{ij} \phi'(u) u_{x_i} v_{x_j} \, dx \\
&= \int_U \sum_{i,j} a^{ij} \phi''(u) u_{x_i} u_{x_j} v \, dx \\
&\leq 0 - \int_U \phi''(u) v |Du|^2 \, dx \leq 0, \text{ by convexity of } \phi.
\end{aligned}
\]

(We don't know whether the product of two \( H^1 \) functions is weakly differentiable. This is why we do not take \( v \in H^1_0(U) \). Now we complete the proof with the standard density argument.)

12. **Proof.** Given \( u \in C^2(U) \cap C(U) \) with \( Lu \leq 0 \) in \( U \) and \( u \leq 0 \) on \( \partial U \). Since \( U \) is compact and \( v \in C(U), v \geq 0 \). So \( w := \phi \in C^2(U) \cap C(U) \). Brutal computation gives us

\[
\begin{aligned}
-a^{ij} w_{x_i x_j} &= -a^{ij} u_{x_i x_j} \phi' + a^{ij} v_{x_i x_j} u \phi'' + a^{ij} v_{x_i x_j} u \phi'' \\
&= \frac{(Lu - b u_{x_i} - cu) \phi' + (-Lu + b u_{x_i} + cu) \phi''}{v^2} + a^{ij} \frac{v_{x_i x_j}}{v} w, \text{ since } a^{ij} = a^{ji}, \\
&= \frac{Lu}{v} - \frac{uLv}{v^2} - b \frac{w_{x_i}}{v} + a^{ij} \frac{v_{x_i x_j}}{v} u,
\end{aligned}
\]

Therefore,

\[
Mw := -a^{ij} w_{x_i x_j} + a^{ij} v_{x_i x_j} w = \left[ \frac{Lu}{v} - \frac{uLv}{v^2} - \frac{b w_{x_i}}{v} + a^{ij} \frac{v_{x_i} v_{x_j}}{v} u \right] \leq 0 \text{ on } \{ x \in U : u > 0 \} \subseteq U
\]

If \( \{ x \in U : u > 0 \} \) is not empty, Weak maximum principle to the operator \( M \) with bounded coefficients (since \( v \in C^1(U) \)) will lead a contradiction that

\[
0 < \max w = \max_{(u \geq 0)} \phi(u) = \phi(0) = 0
\]

Hence \( u \leq 0 \) in \( U \).
```