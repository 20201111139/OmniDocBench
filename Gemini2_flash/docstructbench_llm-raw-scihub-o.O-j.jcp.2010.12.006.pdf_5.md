```markdown
2080 Y. Sun, P.S.P. Tse/Journal of Computational Physics 230 (2011) 2076-2094

\(\partial_t z_{i,j,k} = \frac{z_{i,j,k}^{l+1} - z_{i,j,k}^{l}}{\Delta t}\), \(\overline{\partial_t} z_{i,j,k} = \frac{z_{i,j,k}^{l+1} - z_{i,j,k}^{l-1}}{2\Delta t}\), \(\partial_{x_1} z_{i,j,k} = \frac{z_{i+1,j,k}^{l} - z_{i,j,k}^{l}}{\Delta x_1}\), \(\overline{\partial_{x_1}} z_{i,j,k} = \frac{z_{i+1,j,k}^{l} - z_{i-1,j,k}^{l}}{2\Delta x_1}\),

where the difference operators \(\partial_t\), \(\overline{\partial_t}\) are the discretization of \(\frac{\partial}{\partial t}\) and the difference operators \(\partial_{x_1}\), \(\overline{\partial_{x_1}}\) are the discretization of \(\frac{\partial}{\partial x_1}\). Via these notations and the properties of the difference operators, we present the statement of the local/global conservation laws for the different numerical methods.

3.1. Symplectic method for Maxwell's equations

The following method is constructed based on the method of lines, i.e. discretizing the Hamiltonian PDEs in space, then applying the symplectic method to the resulting Hamiltonian ODEs (see for example [6,22]). Later, we will show the method is also multisymplectic in the corresponding statement of multisymplecticity.

For Maxwell's equations in Hamiltonian form, we use the central finite difference in space (which is leapfrog discretization) and implicit midpoint rule (which is symplectic) in time, it is easy to show that the Hamiltonian formulations in (5) and (7) for Maxwell's equations reduce to the same discretized system,

\[ \partial_t z_{i,j,k}^{l+1} + M^{-1}K_1 \partial_{x_1} z_{i,j,k}^{l+\frac{1}{2}} + M^{-1}K_2 \overline{\partial_{x_2}} z_{i,j,k}^{l+\frac{1}{2}} + M^{-1}K_3 \overline{\partial_{x_3}} z_{i,j,k}^{l+\frac{1}{2}} = 0, \ \ \ \ (18) \]

where indices i, j, k denote spatial increments and index l denotes time increment, and matrices M, \(K_1\),... as in (10). We refer to this particular discretization as the **symplectic method**, though it is also multisymplectic.

The symplectic method (18) is second-order in space and time, and is unconditionally stable. Furthermore, this discrete system preserves two discretized global conservation laws: the first one is the discrete quadratic global conservation law based on (8),

\[ \frac{1}{2} \partial_t [\mu \textbf{H}_{i,j,k}^l \cdot \textbf{H}_{i,j,k}^l + \varepsilon \textbf{E}_{i,j,k}^l \cdot \textbf{E}_{i,j,k}^l] = 0. \ \ \ \ (19) \]

The second discretized global conservation law for symplectic method is based on the helicity Hamiltonian functional (6)

\[ \partial_t [\frac{1}{2\varepsilon} \textbf{H}_{i,j,k}^l \cdot \bigtriangledown \times \textbf{H}_{i,j,k}^l + \frac{1}{2\mu} \textbf{E}_{i,j,k}^l \cdot \bigtriangledown \times \textbf{E}_{i,j,k}^l] = 0, \ \ \ \ (20) \]

where \(\bigtriangledown \times = R_1 \partial_{x_1} + R_2 \partial_{x_2} + R_3 \partial_{x_3}\). Furthermore, the scheme (18) is proved to be multisymplectic, since it preserves the following multisymplectic conservation law

\[ \partial_t [d\textbf{E}_{i,j,k}^l \wedge d\textbf{H}_{i,j,k}^l] + \partial_{x_1} [\frac{1}{\varepsilon} d\textbf{H}_{i-1,j,k}^{l+\frac{1}{2}} \wedge R_1 d\textbf{H}_{i,j,k}^{l+\frac{1}{2}} + \frac{1}{\mu} d\textbf{E}_{i-1,j,k}^{l+\frac{1}{2}} \wedge R_1 d\textbf{E}_{i,j,k}^{l+\frac{1}{2}}] \]
\[ + \partial_{x_2} [\frac{1}{\varepsilon} d\textbf{H}_{i,j-1,k}^{l+\frac{1}{2}} \wedge R_2 d\textbf{H}_{i,j,k}^{l+\frac{1}{2}} + \frac{1}{\mu} d\textbf{E}_{i,j-1,k}^{l+\frac{1}{2}} \wedge R_2 d\textbf{E}_{i,j,k}^{l+\frac{1}{2}}] \]
\[ + \partial_{x_3} [\frac{1}{\varepsilon} d\textbf{H}_{i,j,k-1}^{l+\frac{1}{2}} \wedge R_3 d\textbf{H}_{i,j,k}^{l+\frac{1}{2}} + \frac{1}{\mu} d\textbf{E}_{i,j,k-1}^{l+\frac{1}{2}} \wedge R_3 d\textbf{E}_{i,j,k}^{l+\frac{1}{2}}] = 0. \ \ \ \ (21) \]

Besides the global conservation laws, for the scheme (18) applied to Maxwell's equations, we also have the following local conservation laws based on (13)-(15):

The discrete quadratic conservation law is

\[ \frac{1}{2} \partial_t [\mu \textbf{H}_{i,j,k}^l \cdot \textbf{H}_{i,j,k}^l + \varepsilon \textbf{E}_{i,j,k}^l \cdot \textbf{E}_{i,j,k}^l] + \frac{1}{2} \partial_{x_1} [\textbf{H}_{i,j,k}^{l+\frac{1}{2}} \cdot R_1 \textbf{E}_{i-1,j,k}^{l+\frac{1}{2}} + \textbf{H}_{i-1,j,k}^{l+\frac{1}{2}} \cdot R_1 \textbf{E}_{i,j,k}^{l+\frac{1}{2}}] \]
\[ + \frac{1}{2} \partial_{x_2} [\textbf{H}_{i,j,k}^{l+\frac{1}{2}} \cdot R_2 \textbf{E}_{i,j-1,k}^{l+\frac{1}{2}} + \textbf{H}_{i,j-1,k}^{l+\frac{1}{2}} \cdot R_2 \textbf{E}_{i,j,k}^{l+\frac{1}{2}}] \]
\[ + \frac{1}{2} \partial_{x_3} [\textbf{H}_{i,j,k}^{l+\frac{1}{2}} \cdot R_3 \textbf{E}_{i,j,k-1}^{l+\frac{1}{2}} + \textbf{H}_{i,j,k-1}^{l+\frac{1}{2}} \cdot R_3 \textbf{E}_{i,j,k}^{l+\frac{1}{2}}] = 0. \ \ \ \ (22) \]

The discrete energy conservation law is

\[ \partial_t [\frac{1}{2\varepsilon} \textbf{H}_{i,j,k}^l \cdot \bigtriangledown \times \textbf{H}_{i,j,k}^l + \frac{1}{2\mu} \textbf{E}_{i,j,k}^l \cdot \bigtriangledown \times \textbf{E}_{i,j,k}^l] + \partial_{x_1} [\frac{1}{2\varepsilon} \partial_t \textbf{H}_{i,j,k}^l \cdot R_1 \textbf{H}_{i-1,j,k}^{l+\frac{1}{2}} + \frac{1}{2\mu} \partial_t \textbf{E}_{i,j,k}^l \cdot R_1 \textbf{E}_{i-1,j,k}^{l+\frac{1}{2}}] \]
\[ + \partial_{x_2} [\frac{1}{2\varepsilon} \partial_t \textbf{H}_{i,j,k}^l \cdot R_2 \textbf{H}_{i,j-1,k}^{l+\frac{1}{2}} + \frac{1}{2\mu} \partial_t \textbf{E}_{i,j,k}^l \cdot R_2 \textbf{E}_{i,j-1,k}^{l+\frac{1}{2}}] \]
\[ + \partial_{x_3} [\frac{1}{2\varepsilon} \partial_t \textbf{H}_{i,j,k}^l \cdot R_3 \textbf{H}_{i,j,k-1}^{l+\frac{1}{2}} + \frac{1}{2\mu} \partial_t \textbf{E}_{i,j,k}^l \cdot R_3 \textbf{E}_{i,j,k-1}^{l+\frac{1}{2}}] = 0. \ \ \ \ (23) \]

The discrete momentum conservation law is

6 Let \(p_i\) and \(q_i\) are the functions at grid i, \(\overline{\partial}\), \(\partial\) are the difference operators, then

\(\partial[q_i p_i] = q_{i+1}\overline{\partial} p_i + \partial q_i p_i = \partial q_i p_{i+1} + q_i \partial p_i\),

\(\partial[q_{i+1} p_i] = \partial q_{i+1} p_i + q_{i+1} \partial p_i\),

\(\overline{\partial}[q_i p_i] = \partial q_i p_{i+1} + q_{i-1} \partial p_i = \partial p_i q_{i+1} + p_{i-1} \overline{\partial} q_i\),

\(\overline{\partial}[q_i p_{i+1}] = q_{i+1} \overline{\partial} p_{i+1} + \overline{\partial} q_i p_{i+1}\).
```