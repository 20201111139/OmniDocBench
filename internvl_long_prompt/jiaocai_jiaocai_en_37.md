```markdown
# Theory of Computation Final Exam (Page 2 of 5) 15 Jan, 2015

## 2. (18%) On FA and Regular Languages
Say whether each of the following languages is regular or not regular? Prove your answers.
(a) \( L_1 = \{w \in \{0,1\}^* \text{ and } w \text{ has an equal number of 0s and 1s}\} \).
(b) \( L_2 = \{w \in \{0,1\}^* \text{ and w has an equal number of 01s and 10s}\} \).

## 3. (20%) On PDA and Context-Free Languages
Let \( L_3 = \{wca^b w^R \mid w \in \{a,b\}^*, \text{ and } m, n \in \mathbb{N}, n \leq m \leq 2n\} \).
(a) Give a context-free grammar for the language \( L_3 \).
(b) Design a PDA \( M = (K, \Sigma, \Gamma, \Delta, s, F) \) accepting the language \( L_3 \).

### Solution: (a)
(b) The PDA \( M = (K, \Sigma, \Gamma, \Delta, s, \mathbb{F}) \) is defined below:

<table>
  <tr>
    <th>\( K \)</th>
    <th>\( \Sigma \)</th>
    <th>\( \Gamma \)</th>
    <th>\( \Delta \)</th>
    <th>\( s \)</th>
    <th>\( F \)</th>
  </tr>
  <tr>
    <td>\( \{ \} \)</td>
    <td>\( \{a,b,c\} \)</td>
    <td>\( \{ \} \)</td>
    <td>\( (q, \alpha, \beta) \)</td>
    <td>\( (p, \gamma) \)</td>
  </tr>
</table>
```