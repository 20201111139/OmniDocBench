Theory of Computation Final Exam (Page 2 of 5) 15 Jan., 2015

2. (18%) On FA and Regular Languages
Say whether each of the following languages is regular or not regular? Prove your
answers.
(a) \( L_1 \) = {\(w|w \in {0,1}^* \) and w has an equal number of 0s and 1s}.
(b) \( L_2 \) = {\(w|w \in {0,1}^* \) and w has an equal number of 01s and 10s}.

3. (20%) On PDA and Context-Free Languages
Let \( L_3 \) = {\(wca^mb^n|w \in {a,b}^*, \) where \( w = w^R \), and \( m, n \in N, n \leq m \leq 2n \)}.
(a) Give a context-free grammar for the language \( L_3 \).
(b) Design a PDA \( M = (K, \Sigma, \Gamma, \Delta, s, F) \) accepting the language \( L_3 \).
Solution: (a)
(b) The PDA \( M = (K, \Sigma, \Gamma, \Delta, s, F) \) is defined below:

<table>
<tr>
<th>(q,σ, β)</th>
<th>(p, γ)</th>
</tr>
<tr>
<td>K = {</td>
<td>}</td>
</tr>
<tr>
<td>\( \Sigma \) = {a, b, c}</td>
</tr>
<tr>
<td>\( \Gamma \) = {</td>
<td>}</td>
</tr>
<tr>
<td>s=</td>
</tr>
<tr>
<td>F ={</td>
<td>}</td>
</tr>
</table>