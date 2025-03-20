```markdown
S.V. Kuzmin, D.G.C. McKeon / Physics Letters B 596 (2004) 301–305

For consistency, the time derivative of the constraints of (10) must vanish and hence they must have vanishing Poisson bracket with \( H \). Using the fundamental Poisson brackets

\[
[U(x), T^{\nu}(y)] = 8 \delta(x - y),
\]

etc., we find that the primary constraints of (10) imply the secondary constraints

\[
(\Sigma_i, \Sigma_i) = (-\partial_k \Pi^k_i, e^{i j k} \partial_j (\Pi^k_B - m V^k) - \mu^2 B_i).
\]

If \(\mu^2 = 0\) (the Cremmer-Scherk model Lagrangian [11]), the constraints of (14) would become reducible as then

\[
\partial_i \Sigma_i = 0
\]

and only the transverse portions of \(\Sigma_i\) are constraints. Furthermore, with \(\mu^2 \neq 0\), the requirement \(\dot{\Sigma}_i = 0\) leads to a tertiary constraint

\[
T_i = \mu^2 \Pi^k_B = 0
\]

with \(\Sigma_i\) and \(T_i\) constituting second class constraints as

\[
(T_i(x), \Sigma_i(y)) = \mu^2 \delta_{i j} \delta(x - y).
\]

All other constraints are first class and no further constraints need to be imposed for consistency. There are consequently five first class constraints \(\phi^U\), \(\phi^A\), \(\phi^B\) and \(\Sigma_i\) and six second class constraints \(\Sigma_i\) and \(T_i\). The constraints \(\phi^U\) and \(\Sigma_i\) correspond to the usual gauge transformations \(\delta \omega = \partial \Omega\), \(\delta W = \partial \Omega\) associated with a gauge field \(\omega\) while \(\phi^A\) and \(\phi^B\) act merely as a Lagrange multiplier (i.e., it is not dynamical) and hence its value is completely arbitrary. Suitable gauge conditions associated with the first class constraints are

\[
(\phi^U, A_i, \phi^B, V^{\nu}) = (U, A_i, \partial_k V^k) = 0.
\]

From (10), (14), (15) and (17) it is evident that the only dynamical degrees of freedom are

\[
V^T_i = (\delta_{i j} - \partial_i \partial_j / \partial^2) V^j_i.
\]

We can verify this directly by explicitly eliminating the non-physical degrees of freedom in (4). First, one decomposes \(V_i\), \(A_i\) and \(B_i\) into transverse (T) and longitudinal (L) parts where

\[
V \times V^L = 0 = V \cdot V^T,
\]

etc., (4) now becomes

\[
2 L = (V^T_i)^2 - (V \times V^T_i)^2 + [B^T_i - V \times A^T_i]^2 + (V \times V^T_i)^2 - (V \times V^T_i)^2 + (V^L_i)^2 + 2 \mu^2 [V^T_i \cdot B^T_i + V^L_i \cdot A^L_i + \mu^2 A^L_i \cdot B^L_i].
\]

The equations of motion for \(A^T_i\) and \(U\), respectively, imply that

\[
B^L_i = 0 = V^L_i - V U_i.
\]

reducing (20) to

\[
2 L = (V^T_i)^2 - (V \times V_i^T)^2 + [B^T_i - V \times A^T_i]^2 + 2 \mu V^T_i \cdot (V \times A^T_i) + 2 \mu^2 A^T_i \cdot B^T_i.
\]

Since

\[
A^T_i B^T_i = -(V \times A^T_i) \cdot (V^{-1} (V \times B^T_i)),
\]

we can eliminate \(V \times A^T_i\) from (22) to obtain

\[
V \times A^T_i = B^T_i - m V^T_i + \mu^2 (V^{-1} (V \times B^T_i)).
\]
```