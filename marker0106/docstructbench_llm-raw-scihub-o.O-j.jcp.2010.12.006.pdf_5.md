
$$\partial_{t}z^{i}_{i,j,k}=\frac{z^{i}_{i,j,k}-z^{i}_{i,j,k}}{\Delta t},\quad\overline{\partial}_{t}z^{i}_{i,j,k}=\frac{z^{i}_{i,j,k}-z^{i}_{i,j,k}}{2\Delta t},\quad\partial_{x_{i}}z^{i}_{i,j,k}=\frac{z^{i}_{i+1,j,k}-z^{i}_{i,j,k}}{\Delta x_{1}},\quad\overline{\partial}_{x_{i}}z^{i}_{i,j,k}=\frac{z^{i}_{i+1,j,k}-z^{i}_{i-1,j,k}}{2\Delta x_{1}},$$

where the difference operators 0, 22 are the discretization of % and the difference operators 0%, ax, are the discretization of 2. Via these notations and the properties of the difference operators, we present the statement of the local/global conservation laws for the different numerical methods.

## 3.1. Symplectic method for Maxwell's equations

The following method is constructed based on the method of lines, i.e. discretizing the Hamiltonian PDEs in space, then applying the symplectic method to the resulting Hamiltonian ODEs (see for example [6,22]). Later, we will show the method is also multisymplectic in the corresponding statement of multisymplecticity.

For Maxwell's equations in Hamiltonian form, we use the central finite difference in space (which is leapfrog discretization) and implicit midpoint rule (which is symplectic) in time, it is easy to show that the Hamiltonian formulations in (5) and (7) for Maxwell's equations reduce to the same discretized system,

$$\partial_{t}x^{l}_{i,k}+M^{-1}K_{1}\,\overline{\partial}_{x_{i}}z^{l+1}_{i,k}+M^{-1}K_{2}\,\overline{\partial}_{x_{i}}z^{l+1}_{i,k}+M^{-1}K_{3}\,\overline{\partial}_{x_{i}}z^{l+1}_{i,k}=0,\tag{18}$$

where indices i, j, k denote spatial increments and index I denotes time increment, and matrices M, K, . . as in (10). We refer to this particular discretization as the symplectic method, though it is also multisymplectic.

The symplectic method (18) is second-order in space and time, and is unconditionally stable. Furthermore, this discrete system preserves two discretized global conservation laws: the first one is the discrete quadratic global conservation law based on (8),

$$\frac{1}{2}\partial_{i}\left[\mu{\bf H}^{i}_{j,k}\cdot{\bf H}^{i}_{j,k}+\varepsilon{\bf E}^{i}_{j,k}\cdot{\bf E}^{i}_{j,k}\right]=0.\tag{19}$$

The second discretized global conservation law for symplectic method is based on the helicity Hamiltonian functional (6)

$$\partial_{t}\left[\frac{1}{2\mu}\mathbf{H}_{i,k}^{t}\cdot\widehat{\nabla}\times\mathbf{H}_{i,k}^{t}+\frac{1}{2\mu}\mathbf{E}_{i,k}^{t}\cdot\widehat{\nabla}\times\mathbf{E}_{i,k}^{t}\right]=0,\tag{20}$$

where V x = R10x + B20x + R323x + R323x + R323x + R2 scheme (18) is proved to be multisymplectic, since it preserves the following multisymplectic conservation law

(21)

Besides the global conservation laws, for the scheme (18) applied to Maxwell's equations, we also have the following local conservation laws based on (13)-(15):

The discrete quadratic conservation law is

(22)

The discrete energy conservation law is

k R2E 2 1 k (23)

The discrete momentum conservation law is

6 Let pi and q; are the functions at grid i, 0, 0 are the difference operators, then

0[q;p;] = qi+1 2p; + 2q;Pi+1 + q;op;

$\delta[q_{1+1}p_{1}]=\delta q_{1+1}p_{1+1}+q_{1+1}\delta p_{1}$.  
  

0[q;P;] = 0q;Pi+1 + 9;-1 0P; = 0p;9;+1 + Pi-1 0q;

a[q;Pi+1] = qi+1 opi+1 + dq;Pi.

2080

