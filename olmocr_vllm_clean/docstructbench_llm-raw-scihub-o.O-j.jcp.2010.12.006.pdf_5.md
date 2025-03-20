\[\partial_t z_{ij,k}^{l} = \frac{z_{ij,k}^{l+1} - z_{ij,k}^{l}}{\Delta t}, \quad \partial_t z_{ij,k}^{l} = \frac{z_{ij,k}^{l} - z_{ij,k}^{l-1}}{2\Delta t}, \quad \partial_{x_i} z_{ij,k}^{l} = \frac{z_{i+1,j,k}^{l} - z_{i,j,k}^{l}}{\Delta x_i}, \quad \partial_{x_i} z_{ij,k}^{l} = \frac{z_{i,j+1,k}^{l} - z_{i,j-1,k}^{l}}{2\Delta x_1},\]

where the difference operators \(\partial_t, \partial_t\) are the discretization of \(\frac{\partial}{\partial t}\), and the difference operators \(\partial_{x_i}, \partial_{x_i}\) are the discretization of \(\frac{\partial}{\partial x_i}\). Via these notations and the properties of the difference operators,\(^6\) we present the statement of the local/global conservation laws for the different numerical methods.

3.1. Symplectic method for Maxwell's equations

The following method is constructed based on the method of lines, i.e. discretizing the Hamiltonian PDEs in space, then applying the symplectic method to the resulting Hamiltonian ODEs (see for example [6,22]). Later, we will show the method is also multisymplectic in the corresponding statement of multisymplecticity.

For Maxwell's equations in Hamiltonian form, we use the central finite difference in space (which is leapfrog discretization) and implicit midpoint rule (which is symplectic) in time, it is easy to show that the Hamiltonian formulations in (5) and (7) for Maxwell's equations reduce to the same discretized system,

\[\partial_t z_{ij,k}^{l} + M^{-1}K_1 \partial_{x_i} z_{ij,k}^{l+\frac{1}{2}} + M^{-1}K_2 \partial_{x_i} z_{ij,k}^{l+\frac{1}{2}} + M^{-1}K_3 \partial_{x_i} z_{ij,k}^{l+\frac{1}{2}} = 0,\]

where indices \(i, j, k\) denote spatial increments and index \(l\) denotes time increment, and matrices \(M, K_1, \ldots, K_3\) as in (10). We refer to this particular discretization as the **symplectic method**, though it is also multisymplectic.

The symplectic method (18) is second-order in space and time, and is unconditionally stable. Furthermore, this discrete system preserves two discretized global conservation laws: the first one is the **discrete quadratic global conservation law** based on (8),

\[\frac{1}{2} \partial_t \left[ \mu H_{ij,k}^{l} \cdot H_{ij,k}^{l} + \epsilon E_{ij,k}^{l} \cdot E_{ij,k}^{l} \right] = 0.\]

The second discretized global conservation law for symplectic method is based on the helicity Hamiltonian functional (6)

\[\partial_t \left[ \frac{1}{2\epsilon} H_{ij,k}^{l} \cdot \nabla \times H_{ij,k}^{l} + \frac{1}{2\mu} E_{ij,k}^{l} \cdot \nabla \times E_{ij,k}^{l} \right] = 0,\]

where \(\nabla \times = R_1 \partial_{x_1} + R_2 \partial_{x_2} + R_3 \partial_{x_3}\). Furthermore, the scheme (18) is proved to be multisymplectic, since it preserves the following multisymplectic conservation law

\[\partial_t \left[ \frac{1}{2\epsilon} H_{ij,k}^{l} \cdot H_{ij,k}^{l} + \epsilon E_{ij,k}^{l} \cdot E_{ij,k}^{l} \right] + \partial_{x_1} \left[ \frac{1}{2\epsilon} H_{ij,k}^{l} \cdot R_1 E_{ij,k}^{l+\frac{1}{2}} + \frac{1}{2\mu} E_{ij,k}^{l+\frac{1}{2}} \cdot R_1 E_{ij,k}^{l+\frac{1}{2}} \right] + \partial_{x_2} \left[ \frac{1}{2\epsilon} H_{ij,k}^{l} \cdot R_2 E_{ij,k}^{l+\frac{1}{2}} + \frac{1}{2\mu} E_{ij,k}^{l+\frac{1}{2}} \cdot R_2 E_{ij,k}^{l+\frac{1}{2}} \right] + \partial_{x_3} \left[ \frac{1}{2\epsilon} H_{ij,k}^{l} \cdot R_3 E_{ij,k}^{l+\frac{1}{2}} + \frac{1}{2\mu} E_{ij,k}^{l+\frac{1}{2}} \cdot R_3 E_{ij,k}^{l+\frac{1}{2}} \right] = 0.\]

Besides the global conservation laws, for the scheme (18) applied to Maxwell’s equations, we also have the following local conservation laws based on (13)-(15):

The discrete quadratic conservation law is

\[\frac{1}{2} \partial_t \left[ \frac{1}{2\epsilon} H_{ij,k}^{l} \cdot H_{ij,k}^{l} + \epsilon E_{ij,k}^{l} \cdot E_{ij,k}^{l} \right] + \frac{1}{2\epsilon} \partial_{x_1} \left[ H_{ij,k}^{l} \cdot R_1 E_{ij,k}^{l+\frac{1}{2}} + H_{ij,k}^{l+\frac{1}{2}} \cdot R_1 E_{ij,k}^{l} \right] + \frac{1}{2\mu} \partial_{x_1} \left[ E_{ij,k}^{l} \cdot R_1 E_{ij,k}^{l+\frac{1}{2}} + E_{ij,k}^{l+\frac{1}{2}} \cdot R_1 E_{ij,k}^{l} \right] + \frac{1}{2\epsilon} \partial_{x_2} \left[ H_{ij,k}^{l} \cdot R_2 E_{ij,k}^{l+\frac{1}{2}} + H_{ij,k}^{l+\frac{1}{2}} \cdot R_2 E_{ij,k}^{l} \right] + \frac{1}{2\mu} \partial_{x_2} \left[ E_{ij,k}^{l} \cdot R_2 E_{ij,k}^{l+\frac{1}{2}} + E_{ij,k}^{l+\frac{1}{2}} \cdot R_2 E_{ij,k}^{l} \right] + \frac{1}{2\epsilon} \partial_{x_3} \left[ H_{ij,k}^{l} \cdot R_3 E_{ij,k}^{l+\frac{1}{2}} + H_{ij,k}^{l+\frac{1}{2}} \cdot R_3 E_{ij,k}^{l} \right] + \frac{1}{2\mu} \partial_{x_3} \left[ E_{ij,k}^{l} \cdot R_3 E_{ij,k}^{l+\frac{1}{2}} + E_{ij,k}^{l+\frac{1}{2}} \cdot R_3 E_{ij,k}^{l} \right] = 0.\]

The discrete energy conservation law is

\[\partial_t \left[ \frac{1}{2\epsilon} H_{ij,k}^{l} \cdot H_{ij,k}^{l} + \epsilon E_{ij,k}^{l} \cdot E_{ij,k}^{l} \right] + \frac{1}{2\epsilon} \partial_{x_1} \left[ H_{ij,k}^{l} \cdot R_1 E_{ij,k}^{l+\frac{1}{2}} + H_{ij,k}^{l+\frac{1}{2}} \cdot R_1 E_{ij,k}^{l} \right] + \frac{1}{2\mu} \partial_{x_1} \left[ E_{ij,k}^{l} \cdot R_1 E_{ij,k}^{l+\frac{1}{2}} + E_{ij,k}^{l+\frac{1}{2}} \cdot R_1 E_{ij,k}^{l} \right] + \frac{1}{2\epsilon} \partial_{x_2} \left[ H_{ij,k}^{l} \cdot R_2 E_{ij,k}^{l+\frac{1}{2}} + H_{ij,k}^{l+\frac{1}{2}} \cdot R_2 E_{ij,k}^{l} \right] + \frac{1}{2\mu} \partial_{x_2} \left[ E_{ij,k}^{l} \cdot R_2 E_{ij,k}^{l+\frac{1}{2}} + E_{ij,k}^{l+\frac{1}{2}} \cdot R_2 E_{ij,k}^{l} \right] + \frac{1}{2\epsilon} \partial_{x_3} \left[ H_{ij,k}^{l} \cdot R_3 E_{ij,k}^{l+\frac{1}{2}} + H_{ij,k}^{l+\frac{1}{2}} \cdot R_3 E_{ij,k}^{l} \right] + \frac{1}{2\mu} \partial_{x_3} \left[ E_{ij,k}^{l} \cdot R_3 E_{ij,k}^{l+\frac{1}{2}} + E_{ij,k}^{l+\frac{1}{2}} \cdot R_3 E_{ij,k}^{l} \right] = 0.\]

---

\(^6\) Let \(p_i\) and \(q_i\) are the functions at grid \(i\), \(\partial_t, \partial_{x_i}\) are the difference operators, then

\[\partial_t [q_i p_i] = \partial_t [q_i] p_i + q_i \partial_t [p_i], \quad \partial_{x_i} [q_i p_i] = \partial_{x_i} [q_i] p_i + q_i \partial_{x_i} [p_i], \]

\[\partial_{x_i} [q_i] = \partial_{x_i} q_i, \quad \partial_{x_i} [p_i] = \partial_{x_i} p_i, \quad \partial_{x_i} [q_i, p_i] = \partial_{x_i} [q_i] p_i + q_i \partial_{x_i} [p_i].\]