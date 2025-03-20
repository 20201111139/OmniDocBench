Theory of Computation
Final Exam (Page 2 of 5)
15 Jan., 2015
2. (18\%) On FA and Regular Languages

Say whether each of the following languages is regular or not regular? Prove your answers.
(a) $L_{1}=\left\{w \mid w \in\{0,1\}^{*}\right.$ and $w$ has an equal number of 0 s and 1 s$\}$.
(b) $L_{2}=\left\{w \mid w \in\{0,1\}^{*}\right.$ and $w$ has an equal number of 01s and 10s $\}$.
3. $\mathbf{( 2 0 \% )}$ On PDA and Context-Free Languages

Let $L_{3}=\left\{w c a^{m} b^{n} \mid w \in\{a, b\}^{*}\right.$, where $w=w^{R}$, and $\left.m, n \in \mathbb{N}, n \leq m \leq 2 n\right\}$.
(a) Give a context-free grammar for the language $L_{3}$.
(b) Design a PDA $M=(K, \Sigma, \Gamma, \Delta, s, F)$ accepting the language $L_{3}$.

Solution: (a)
(b) The PDA $M=(K, \Sigma, \Gamma, \Delta, s, F)$ is defined below:
<table border=1>
<tr>
<td></td>
<td>$(q,\sigma,\beta)$</td>
<td>$(p,\gamma)$</td>
</tr>
<tr>
<td>
$K=\{\longrightarrow$ 江 $\}$
</td>
<td></td>
<td></td>
</tr>
<tr>
<td>$\Sigma=\{a,b,c\}$</td>
<td></td>
<td></td>
</tr>
<tr>
<td>$\Gamma=\{\quad\}$</td>
<td></td>
<td></td>
</tr>
<tr>
<td>$s=$</td>
<td></td>
<td></td>
</tr>
<tr>
<td>F={⟶</td>
<td></td>
<td></td>
</tr>
</table>