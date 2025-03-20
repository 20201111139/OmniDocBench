2. (18%) On FA and Regular Languages
   Say whether each of the following languages is regular or not regular? Prove your answers.
   (a) \( L_1 = \{ w \mid w \in \{0, 1\}^* \text{ and } w \text{ has an equal number of } 0s \text{ and } 1s \} \).
   (b) \( L_2 = \{ w \mid w \in \{0, 1\}^* \text{ and } w \text{ has an equal number of } 01s \text{ and } 10s \} \).

3. (20%) On PDA and Context-Free Languages
   Let \( L_3 = \{ w c a^m b^n \mid w \in \{a, b\}^*, \text{ where } w = w^R, \text{ and } m, n \in \mathbb{N}, n \leq m \leq 2n \} \).
   (a) Give a context-free grammar for the language \( L_3 \).
   (b) Design a PDA \( M = (K, \Sigma, \Gamma, \Delta, s, F) \) accepting the language \( L_3 \).
   **Solution:** (a)

   (b) The PDA \( M = (K, \Sigma, \Gamma, \Delta, s, F) \) is defined below:

   \[
   \begin{array}{|c|c|}
   \hline
   K = \{ \text{________________________________________} \} & (q, \sigma, \beta) \mid (p, \gamma) \\
   \hline
   \Sigma = \{a, b, c\} & \\
   \hline
   \Gamma = \{ \} & \\
   \hline
   s = \text{________________________________________} & \\
   \hline
   F = \{ \text{________________________________________} \} & \\
   \hline
   \end{array}
   \]