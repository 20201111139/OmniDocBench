For consistency, the time derivative of the constraints of (10) must vanish and hence they must have vanishing Poisson bracket with $H$. Using the fundamental Poisson brackets

$$ [U(x), \Pi^U(y)] = \delta(x - y), \quad \text{etc.}, $$

we find that the primary constraints of (10) imply the secondary constraints

$$ (\Sigma, \Sigma_i) = (-\partial_k \Pi^V_k, \epsilon^{ijk} \partial_j (\Pi^B_k - m V_k) - \mu^2 B_i). \quad \text{(14)} $$

If $\mu^2 = 0$ (the Cremmer–Scherk model Lagrangian [1]), the constraints of (14) would become reducible as then $\partial_i \Sigma_i = 0$ and only the transverse portions of $\Sigma_i$ are constraints. Furthermore, with $\mu^2 \neq 0$, the requirement $\Sigma_i = 0$ leads to a tertiary constraint

$$ T_k \equiv \mu^2 \Pi^B_k = 0 \quad \text{(15)} $$

with $\Sigma_i$ and $T_k$ constituting second class constraints as

$$ [T_k(x), \Sigma_i(y)] = \mu^2 \delta_{ik} \delta(x - y). \quad \text{(16)} $$

All other constraints are first class and no further constraints need to be imposed for consistency. There are consequently five first class constraints ($\Phi^U$, $\Phi^A_k$ and $\Sigma$) and six second class constraints ($\Sigma_i$ and $T_k$). The constraints $\Phi^U$ and $\Sigma$ correspond to the usual gauge transformations $\delta W_0 = \partial_0 \Omega$, $\delta W_1 = \partial_1 \Omega$ associated with a gauge field $W_\mu$, while $\Phi^A_k$ is associated with the fact that in (12) $A_k$ acts merely as a Lagrange multiplier (i.e., it is not dynamical) and hence its value is completely arbitrary. Suitable gauge conditions associated with the first class constraints are

$$ (\gamma^U, \gamma_k^A, \gamma^V) = (U, A_k, \partial_k V_k) = 0. \quad \text{(17)} $$

From (10), (14), (15) and (17) it is evident that the only dynamical degrees of freedom are

$$ V_i^T \equiv (\delta_{ij} - \partial_i \partial_j / \partial^2) V_j. \quad \text{(18)} $$

We can verify this directly by explicitly eliminating the non-physical degrees of freedom in (4). First, one decomposes $V_k$, $A_k$ and $B_k$ into transverse ($T$) and longitudinal ($L$) parts where

$$ \nabla \times V^T \equiv 0 \equiv \nabla \cdot V^T, \quad \text{(19)} $$

eqc., (4) now becomes

$$ 2L = (\dot{B}^L)^2 - (\nabla \cdot B^L)^2 + [\dot{B}^T - \nabla \times A^T]^2 + (\dot{V}^T)^2 - (\nabla \times V^T)^2 + [\dot{V}^L - \nabla U]^2 + 2m [\dot{V}^T \cdot (\nabla \times A^T) + B^L \cdot \dot{V}^L + B^T \cdot \dot{V}^T - B^L \cdot \nabla U] + 2\mu^2 [A^T \cdot B^T + A^T \cdot B^L]. \quad \text{(20)} $$

The equations of motion for $A^L$ and $U$, respectively, imply that

$$ B^L = 0 \equiv \dot{V}^L - \nabla U, \quad \text{(21)} $$

reducing (20) to

$$ 2L = (\dot{V}^T)^2 - (\nabla \times V^T)^2 + [\dot{B}^T - \nabla \times A^T]^2 + 2m V^T \cdot (\nabla \times A^T) + 2m B^T \cdot \dot{V}^T + 2\mu^2 A^T \cdot B^T. \quad \text{(22)} $$

Since

$$ A^T \cdot B^T = - (\nabla \times A^T) \cdot (\nabla^2)^{-1} (\nabla \times B^T), \quad \text{(23)} $$

we can eliminate $\nabla \times A^T$ from (22) to obtain

$$ \nabla \times A^T = \dot{B}^T - m V^T + \mu^2 (\nabla^2)^{-1} (\nabla \times B^T). \quad \text{(24)} $$