2. (18\%) On FA and Regular Languages
Say whether each of the following languages is regular or not regular? Prove your answers.
(a) \(L_{1}=\{w \mid w \in\{0,1\}^{*}\) and \(w\) has an equal number of 0 s and \(1 s\}\).
(b) \(L_{2}=\{w \mid w \in\{0,1\}^{*}\right.\) and \(w\) has an equal number of 01 s and 10 s\}.
3. (20\%) On PDA and Context-Free Languages
Let \(L_{3}=\left\{w c a^{m} b^{n} \mid w \in\{a, b\}^{*}\right.\), where \(w=w^{R}\), and \(m, n \in \mathbb{N}, n \leq m \leq 2 n\}\).
(a) Give a context-free grammar for the language \(L_{3}\).
(b) Design a PDA \(M=(K, \Sigma, \Gamma, \Delta, s, F)\) accepting the language \(L_{3}\).
Solution: (a)
(b) The PDA \(M=(K, \Sigma, \Gamma, \Delta, s, F\) ) is defined below:
\[
\begin{array}{c}
K=\{\square \quad \square \quad \square \quad \square \quad \square \quad \square \quad \\
\sum=\{a, b, c\} \\
\Gamma=\{\quad \} \\
s=\square \\
F=\{\quad \}
\end{array}
\]