For consistency, the time derivative of the constraints of (10) must vanish and hence they must have vanishing Poisson bracket with $H$. Using the fundamental Poisson brackets

$$\left[ U(x), \Pi^U(y) \right] = \delta(x - y), \tag{13}$$

eq., we find that the primary constraints of (10) imply the secondary constraints

$$\left( \Sigma, \Sigma_i \right) = \left( -\partial_k \Pi_k^V \cdot \epsilon^{ijk} \partial_j \left( \Pi_k^B - mV_k \right) - \mu^2 B_i \right). \tag{14}$$

If $\mu^2 = 0$ (the Cremmer–Scherk model Lagrangian [1]), the constraints of (14) would become reducible as then $\partial_i \Sigma_i = 0$ and only the transverse portions of $\Sigma_i$ are constraints. Furthermore, with $\mu^2 \neq 0$, the requirement $\Sigma_i = 0$ leads to a tertiary constraint

$$T_k \equiv \mu^2 \Pi_k^B = 0 \tag{15}$$

with $\Sigma_i$ and $T_k$ constituting second class constraints as

$$\left[ T_k(x), \Sigma_i(y) \right] = \mu^4 \delta_{ik} \delta(x - y). \tag{16}$$

All other constraints are first class and no further constraints need to be imposed for consistency. There are consequently five first class constraints ($\Phi^U, \Phi^A_k$ and $\Sigma$) and six second class constraints ($\Sigma_i$ and $T_k$). The constraints $\Phi^U$ and $\Sigma$ correspond to the usual gauge transformations $\delta W_0 = \partial_0 \Omega, \delta W_i = \partial_i \Omega$ associated with a gauge field $W_\mu$, while $\Phi^A_k$ is associated with the fact that in (12) $A_k$ acts merely as a Lagrange multiplier (i.e., it is not dynamical) and hence its value is completely arbitrary. Suitable gauge conditions associated with the first class constraints are

$$\left( \gamma^U, \gamma^A_k, \gamma^V \right) = (U, A_k, \partial_k V_k) = 0. \tag{17}$$

From (10), (14), (15) and (17) it is evident that the only dynamical degrees of freedom are

$$V^T_j \equiv \left( \delta_{ij} - \partial_i \partial_j / \partial^2 \right) V_j. \tag{18}$$

We can verify this directly by explicitly eliminating the non-physical degrees of freedom in (4). First, one decomposes $V_k, A_k$ and $B_k$ into transverse ($T$) and longitudinal ($L$) parts where

$$\nabla \times V^L = 0 \equiv \nabla \cdot V^T, \tag{19}$$

eq., (4) now becomes

$$2L = \left( \dot{B}^L \right)^2 - \left( \nabla \cdot B^L \right)^2 + \left[ \dot{B}^T - \nabla \times A^T \right]^2 + \left( \dot{V}^T \right)^2 - \left( \nabla \times V^T \right)^2 + \left[ \dot{V}^L - \nabla U \right]^2 + 2m \left[ \dot{V}^T \cdot \left( \nabla \times A^T \right) + B^L \cdot \dot{V}^L + B^T \cdot \dot{V}^T - B^L \cdot \nabla U \right] + 2\mu^2 \left[ A^T \cdot B^T + A^L \cdot B^L \right]. \tag{20}$$

The equations of motion for $A^L$ and $U$, respectively, imply that

$$B^L = 0 = \dot{V}^L - \nabla U, \tag{21}$$

reducing (20) to

$$2L = \left( \dot{V}^T \right)^2 - \left( \nabla \times V^T \right)^2 + \left[ \dot{B}^T - \nabla \times A^T \right]^2 + 2m \dot{V}^T \cdot \left( \nabla \times A^T \right) + 2m B^T \cdot \dot{V}^T + 2\mu^2 A^T \cdot B^T. \tag{22}$$

Since

$$A^T \cdot B^T = -\left( \nabla \times A^T \right) \cdot \left( \nabla^2 \right)^{-1} \left( \nabla \times B^T \right), \tag{23}$$

we can eliminate $\nabla \times A^T$ from (22) to obtain

$$\nabla \times A^T = \dot{B}^T - m \dot{V}^T + \mu^2 \left( \nabla^2 \right)^{-1} \left( \nabla \times B^T \right). \tag{24}$$