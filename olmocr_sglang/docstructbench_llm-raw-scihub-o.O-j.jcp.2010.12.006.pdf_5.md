\[
\frac{\partial z_{1,j,k}^l}{\Delta t} = \frac{z_{1,j,k}^{l+1} - z_{1,j,k}^{l}}{\Delta t}, \quad \frac{\partial z_{2,j,k}^l}{\Delta t} = \frac{z_{2,j,k}^{l+1} - z_{2,j,k}^{l}}{2\Delta t}, \quad \partial_{\alpha_1} z_{1,j,k}^l = \frac{z_{1,j,k+1}^l - z_{1,j,k-1}^l}{\Delta x_1}, \quad \partial_{\alpha_2} z_{2,j,k}^l = \frac{z_{2,j+1,k}^l - z_{2,j-1,k}^l}{2\Delta x_1},
\]
where the difference operators \(\partial_{\alpha_1}, \partial_{\alpha_2}\) are the discretization of \(\frac{\partial}{\partial x}\) and the difference operators \(\partial_{\alpha_1}, \partial_{\alpha_2}\) are the discretization of \(\frac{\partial}{\partial t}\). Via these notations and the properties of the difference operators, we present the statement of the local/global conservation laws for the different numerical methods.

3.1. Symplectic method for Maxwell’s equations

The following method is constructed based on the method of lines, i.e. discretizing the Hamiltonian PDEs in space, then applying the symplectic method to the resulting Hamiltonian ODEs (see for example [6,22]). Later, we will show the method is also multisymplectic in the corresponding statement of multisymplecticity.

For Maxwell’s equations in Hamiltonian form, we use the central finite difference in space (which is leapfrog discretization) and implicit midpoint rule (which is symplectic) in time, it is easy to show that the Hamiltonian formulations in (5) and (7) for Maxwell’s equations reduce to the same discretized system,

\[
\partial_t z_{1,j,k}^l + M^{-1} K_1 \partial_{\alpha_1} z_{1,j,k}^{l+\frac{1}{2}} + M^{-1} K_2 \partial_{\alpha_2} z_{1,j,k}^{l+\frac{1}{2}} + M^{-1} K_3 \partial_{\alpha_3} z_{1,j,k}^{l+\frac{1}{2}} = 0,
\]

where indices \(i,j,k\) denote spatial increments and index \(l\) denotes time increment, and matrices \(M, K_1, \ldots\) as in (10). We refer to this particular discretization as the symplectic method, though it is also multisymplectic.

The symplectic method (18) is second-order in space and time, and is unconditionally stable. Furthermore, this discrete system preserves two discretized global conservation laws: the first one is the discrete quadratic global conservation law based on (8),

\[
\frac{1}{2} \partial_{\alpha_1} \left[ \mu H_{1,j,k} \cdot H_{1,j,k} + \varepsilon E_{1,j,k} \cdot E_{1,j,k} \right] = 0.
\]

The second discretized global conservation law for symplectic method is based on the helicity Hamiltonian functional (6)

\[
\partial_{\alpha_2} \left[ \frac{1}{2\mu} H_{1,j,k} \cdot \nabla \times H_{1,j,k} + \frac{1}{\varepsilon} E_{1,j,k} \cdot \nabla \times E_{1,j,k} \right] = 0,
\]

where \(\nabla \times = \partial_{x_2} \partial_{x_1} - \partial_{x_1} \partial_{x_2}\). Furthermore, the scheme (18) is proved to be multisymplectic, since it preserves the following multisymplectic conservation law

\[
\partial_t \left[ \frac{dE_{1,j,k}^{l+1}}{dt} \wedge dH_{1,j,k}^{l+1} \right] + \partial_{\alpha_1} \left[ \frac{1}{\varepsilon} \frac{dH_{1,j,k}^{l+1}}{dt} \wedge R_1 dH_{1,j,k}^{l+1} + \frac{1}{\mu} dE_{1,j,k}^{l+1} \wedge R_t dE_{1,j,k}^{l+1} \right] + \partial_{\alpha_2} \left[ \frac{1}{\mu} dH_{1,j,k}^{l+1} \wedge R_2 dH_{1,j,k}^{l+1} + \frac{1}{\varepsilon} dE_{1,j,k}^{l+1} \wedge R_2 dE_{1,j,k}^{l+1} \right]
\]

Besides the global conservation laws, for the scheme (18) applied to Maxwell’s equations, we also have the following local conservation laws based on (13)–(15):

The discrete quadratic conservation law is

\[
\frac{1}{2} \partial_{\alpha_1} \left[ \mu H_{1,j,k} \cdot H_{1,j,k} + \varepsilon E_{1,j,k} \cdot E_{1,j,k} \right] + \frac{1}{2} \partial_{\alpha_2} \left[ H_{1,j,k} \cdot R_1 E_{1,j,k} + \frac{1}{\varepsilon} H_{1,j,k} \cdot R_1 E_{1,j,k} \right] + \frac{1}{2} \partial_{\alpha_3} \left[ H_{1,j,k} \cdot R_2 E_{1,j,k} + \frac{1}{\mu} H_{1,j,k} \cdot R_2 E_{1,j,k} \right]
\]

The discrete energy conservation law is

\[
\partial_{\alpha_1} \left[ \frac{1}{2\mu} H_{1,j,k} \cdot \nabla \times H_{1,j,k} + \frac{1}{\varepsilon} E_{1,j,k} \cdot \nabla \times E_{1,j,k} \right] + \partial_{\alpha_2} \left[ \frac{1}{2\mu} \partial_t H_{1,j,k} \cdot R_1 H_{1,j,k+1} + \frac{1}{2\mu} \partial_t E_{1,j,k} \cdot R_1 E_{1,j,k+1} \right] + \partial_{\alpha_3} \left[ \frac{1}{2\mu} \partial_t H_{1,j,k} \cdot R_2 H_{1,j,k+1} + \frac{1}{2\mu} \partial_t E_{1,j,k} \cdot R_2 E_{1,j,k+1} \right] = 0.
\]

The discrete momentum conservation law is

\[
\frac{\partial}{\partial t} [q_i p_i] = q_{i+1} p_i - q_i p_{i+1} + q_i \partial_t p_i,
\]

\[
\frac{\partial}{\partial t} [q_i p_i] = \partial_{\alpha_1} q_{i-1} p_{i+1} + q_{i-1} \partial_{\alpha_1} p_i,
\]

\[
\frac{\partial}{\partial t} [q_i p_i] = \partial_{\alpha_2} q_{i+1} p_{i+1} + q_{i-1} \partial_{\alpha_2} p_i,
\]

\[
\frac{\partial}{\partial t} [q_i p_i] = q_{i-1} \partial_{\alpha_3} p_{i+1} + \partial_{\alpha_3} q_{i+1} p_{i+1}.
\]

\[
\frac{\partial}{\partial t} [q_{i+1} p_i] = q_{i+1} \partial_{\alpha_1} p_i + \partial_{\alpha_1} q_{i+1} p_{i+1},
\]

\[
\frac{\partial}{\partial t} [q_{i+1} p_i] = \partial_{\alpha_2} q_{i+1} p_{i+1} + q_{i+1} \partial_{\alpha_2} p_i,
\]

\[
\frac{\partial}{\partial t} [q_{i+1} p_i] = q_{i+1} \partial_{\alpha_3} p_{i+1} + \partial_{\alpha_3} q_{i+1} p_{i+1}.
\]