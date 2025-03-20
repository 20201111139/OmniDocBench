10. Proof. We omit (a) since is standard. For (b), if \( u \) attains an interior maximum, then the conclusion follows from strong maximum principle.

If not, then for some \( {x}^{0} \in  \partial U, u\left( {x}^{0}\right)  > u\left( x\right) \forall x \in  U \) . Then Hopf’s lemma implies \( \frac{\partial u}{\partial \nu }\left( {x}^{0}\right)  > 0 \) , which is a contradiction.

Remark 2. A generalization of this problem to mixed boundary conditions is recorded in Gilbarg-Trudinger, Elliptic PDEs of second order, Problem 3.1.

11. Proof. Define

\[
B\left\lbrack  {u, v}\right\rbrack   = {\int }_{U}\mathop{\sum }\limits_{{i, j}}{a}^{ij}{u}_{{x}_{i}}{v}_{{x}_{j}}{dx}\text{ for }u \in  {H}^{1}\left( U\right) , v \in  {H}_{0}^{1}\left( U\right) .
\]

By Exercise \( {5.17},\phi \left( u\right)  \in  {H}^{1}\left( U\right) \) . Then, for all \( v \in  {C}_{c}^{\infty }\left( U\right) , v \geq  0 \) ,

\[
B\left\lbrack  {\phi \left( u\right) , v}\right\rbrack   = {\int }_{U}\mathop{\sum }\limits_{{i, j}}{a}^{ij}{\left( \phi \left( u\right) \right) }_{{x}_{i}}{v}_{{x}_{j}}{dx}
\]

\[
= {\int }_{U}\mathop{\sum }\limits_{{i, j}}{a}^{ij}{\phi }^{\prime }\left( u\right) {u}_{{x}_{i}}{v}_{{x}_{j}}{dx},\left( {{\phi }^{\prime }\left( u\right) }\right. \text{is bounded since}\mathrm{u}\text{is bounded})
\]

\[
= {\int }_{U}\mathop{\sum }\limits_{{i, j}}{a}^{ij}{u}_{{x}_{i}}{\left( {\phi }^{\prime }\left( u\right) v\right) }_{{x}_{j}} - \mathop{\sum }\limits_{{i, j}}{a}_{ij}{\phi }^{\prime \prime }\left( u\right) {u}_{{x}_{i}}{u}_{{x}_{j}}{vdx}
\]

\[
\leq  0 - {\int }_{U}{\phi }^{\prime \prime }\left( u\right) v{\left| Du\right| }^{2}{dx} \leq  0\text{, by convexity of}\phi \text{.}
\]

(We don’t know whether the product of two \( {H}^{1} \) functions is weakly differentiable. This is why we do not take \( v \in  {H}_{0}^{1} \) .) Now we complete the proof with the standard density argument.

12. Proof. Given \( u \in  {C}^{2}\left( U\right)  \cap  C\left( \bar{U}\right) \) with \( {Lu} \leq  0 \) in \( U \) and \( u \leq  0 \) on \( \partial U \) . Since \( \bar{U} \) is compact and \( v \in  C\left( \bar{U}\right) , v \geq  c > 0 \) . So \( w \mathrel{\text{:=}} \frac{u}{v} \in  {C}^{2}\left( U\right)  \cap  C\left( \bar{U}\right) \) . Brutal computation gives us

\[
- {a}^{ij}{w}_{{x}_{i}{x}_{j}} = \frac{-{a}^{ij}{u}_{{x}_{i}{x}_{j}}v + {a}^{ij}{v}_{{x}_{i}{x}_{j}}u}{{v}^{2}} + \frac{{a}^{ij}{v}_{{x}_{i}}{u}_{{x}_{j}} - {a}^{ij}{u}_{{x}_{i}}{v}_{{x}_{j}}}{{v}^{2}} - {a}^{ij}\frac{2}{v}{v}_{{x}_{j}}\frac{{v}_{{x}_{i}}u - v{u}_{{x}_{i}}}{{v}^{2}}
\]

\[
= \frac{\left( {{Lu} - {b}^{i}{u}_{{x}_{i}} - {cu}}\right) v + \left( {-{Lv} + {b}^{i}{v}_{{x}_{i}} + {cv}}\right) u}{{v}^{2}} + 0 + {a}^{ij}\frac{2}{v}{v}_{{x}_{j}}{w}_{{x}_{i}},\text{ since }{a}^{ij} = {a}^{ji}.
\]

\[
= \frac{Lu}{v} - \frac{uLv}{{v}^{2}} - {b}^{i}{w}_{{x}_{i}} + {a}^{ij}\frac{2}{v}{v}_{{x}_{j}}{w}_{{x}_{i}}
\]

Therefore,

\[
{Mw} \mathrel{\text{:=}}  - {a}^{ij}{w}_{{x}_{i}{x}_{j}} + {w}_{{x}_{i}}\left\lbrack  {{b}^{i} - {a}^{ij}\frac{2}{v}{v}_{{x}_{j}}}\right\rbrack   = \frac{Lu}{v} - \frac{uLv}{{v}^{2}} \leq  0\text{ on }\{ x \in  \bar{U} : u > 0\}  \subseteq  U
\]

If \( \{ x \in  \bar{U} : u > 0\} \) is not empty, Weak maximum principle to the operator \( M \) with bounded coefficeints (since \( v \in  {C}^{1}\left( \bar{U}\right) \) ) will lead a contradiction that

\[
0 < \mathop{\max }\limits_{{\{ u > 0\} }}w = \mathop{\max }\limits_{{\partial \{ u > 0\} }}w = \frac{0}{v} = 0
\]

Hence \( u \leq  0 \) in \( U \) .