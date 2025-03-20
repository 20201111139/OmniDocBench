```markdown
where the difference operators \(\bar{\partial}_x, \bar{\partial}_z\) are the discretization of \(\frac{\partial}{\partial x}, \frac{\partial}{\partial z}\), and the difference operators \(\bar{\delta}_x, \bar{\delta}_z\) are the discretization of \(\frac{\delta}{\delta x}, \frac{\delta}{\delta z}\). Via these notations and the properties of the difference operators,\(^6\) we present the statement of the local/global conservation laws for the different numerical methods.

### 3. Symplectic method for Maxwell's equations

The following method is constructed based on the method of lines, i.e. discretizing the Hamiltonian PDEs in space, then applying the symplectic method to the resulting Hamiltonian ODEs (see for example [6,22]). Later, we will show the method is also multisymplectic in the corresponding statement of multisymplecticity.

For Maxwell's equations in Hamiltonian form, we use the central finite difference in space (which is leapfrog discretization) and implicit midpoint rule (which is symplectic) in time, it is easy to show that the Hamiltonian formulations in (5) and (7) for Maxwell's equations reduce to the same discretized system,

\[
\bar{\partial}_t z_{i,j,k} + M^{-1}K_1 \bar{\partial}_x z_{i,j,k} + M^{-1}K_2 \bar{\partial}_y z_{i,j,k} + M^{-1}K_3 \bar{\partial}_z z_{i,j,k} = 0,
\]

where indices \(i, j, k\) denote spatial increments and index \(t\) denotes time increment, and matrices \(M, K_1, \ldots\) are as in (10). We refer to this particular discretization as the **symplectic method**, though it is also multisymplectic.

The symplectic method (18) is second-order in space and time, and is unconditionally stable. Furthermore, this discrete system preserves two discretized global conservation laws: the first one is the **discrete quadratic global conservation law** based on (8),

\[
\frac{1}{2} \partial_t \left[ \mathbf{H} \cdot \mathbf{H}_{i,j,k} + \varepsilon \mathbf{E} \cdot \mathbf{E}_{i,j,k} \right] = 0.
\]

The second discretized global conservation law for symplectic method is based on the helicity Hamiltonian functional (6)

\[
\partial_t \left[ \frac{1}{2c} \mathbf{H}_{i,j,k} \cdot \nabla \times \mathbf{H} + \frac{1}{2\mu} \mathbf{E}_{i,j,k} \cdot \nabla \times \mathbf{E} \right] = 0,
\]

where \(\nabla \times = \mathbf{R}_x \partial_x + \mathbf{R}_y \partial_y + \mathbf{R}_z \partial_z\). Furthermore, the scheme (18) is proved to be multisymplectic, since it preserves the following multisymplectic conservation law

\[
\partial_t \left[ \mathbf{dE}_{i,j,k} \wedge \mathbf{dH}_{i,j+1,k} \right] + \partial_x \left[ \frac{1}{c} \mathbf{dH}_{i,j,k+1} \wedge \mathbf{R} \mathbf{dH}_{i,j,k}^h \right] 
+ \partial_y \left[ \frac{1}{\mu} \mathbf{dE}_{i,j,k+1} \wedge \mathbf{R}_2 \mathbf{dE}_{i,j,k}^h \right] = 0.
\]

Besides the global conservation laws, for the scheme (18) applied to Maxwell's equations, we also have the following local conservation laws based on (13)-(15):

The **discrete quadratic conservation law** is

\[
\frac{1}{2} \partial_t \left[ \mathbf{H} \cdot \mathbf{H}_{i,j,k} + \varepsilon \mathbf{E} \cdot \mathbf{E}_{i,j,k} \right] + \frac{1}{2} \partial_x \left[ \mathbf{H}_{i+1,j,k} \cdot \mathbf{R} \mathbf{E}_{i,j+1,k} \right] 
+ \frac{1}{2} \partial_y \left[ \mathbf{H}_{i,j+1,k} \cdot \mathbf{R} \mathbf{E}_{i,j,k+1} \right] = 0.
\]

The **discrete energy conservation law** is

\[
\partial_t \left[ \frac{1}{2c} \mathbf{H} \cdot \mathbf{R} \mathbf{H}_{i,j,k} + \frac{1}{2\mu} \mathbf{E} \cdot \mathbf{R} \mathbf{E}_{i,j,k} \right] = 0,
\]

\[
+ \partial_x \left[ \frac{1}{2c} \mathbf{H} \cdot \mathbf{R} \mathbf{E}_{i+1,j,k} + \frac{1}{2\mu} \mathbf{E} \cdot \mathbf{R} \mathbf{E}_{i,j+1,k} \right],
\]

\[
+ \partial_y \left[ \frac{1}{2c} \mathbf{H} \cdot \mathbf{R} \mathbf{E}_{i,j,k+1} + \frac{1}{2\mu} \mathbf{E} \cdot \mathbf{R} \mathbf{E}_{i,j,k-1} \right] = 0.
\]

The **discrete momentum conservation law** is

---
\(^6\) Let \(q_1\) and \(q_2\) are the functions at grid 1, \(\bar{\partial}\) are the difference operators, then

\(\partial_t q_1 = q_{11} \wedge q_{12} \wedge \bar{\partial} \cdot q_1 \wedge \bar{\partial} \cdot q_2 , \)

\(\partial_t q_2 = q_{21} \wedge q_{22} \wedge \bar{\partial} \cdot q_2 \wedge \bar{\partial} \cdot q_1 , \)
```