$\partial _{t}z_{ij,k}^{1}=\frac {z_{ijk}^{1+1}-z_{ijk}^{1}}{\Delta t},$ $\overline {\partial }_{t}z_{ijk}^{1}=\frac {z_{ijk}^{1+1}-z_{ijk}^{1-1}}{2\Delta t}$ $\partial _{x_{1}}Z_{ijk}^{1}=\frac {z_{i+1}^{1}jk-z_{ijk}^{1}}{\Delta x_{1}}$ $\overline {\partial }_{x_{1}}Z_{ijk}^{1}=\frac {z_{i+1}^{1}jk-z_{i-1}^{1}jk}{2\Delta x_{1}}$

where the difference operators$\theta _{t},\overline {\theta }_{t}$are the discretization of$\frac {\partial }{\partial t},$and the difference operators$\partial _{x_{1}},$ $\overline {\theta }_{x_{1}}$are the discretization of $\frac {\partial }{\partial x_{1}}.$Via these notations and the properties of the difference operators, we present the statement of the local/global conser-vation laws for the different numerical methods.

## 3.1. Symplectic method for Maxwell's equations

The following method is constructed based on the method of lines, i.e. discretizing the Hamiltonian PDEs in space, then applying the symplectic method to the resulting Hamiltonian ODEs (see for example [6,22]). Later, we will show the method is also multisymplectic in the corresponding statement of multisymplectcity.

For Maxwell's equations in Hamiltonian form, we use the central finite difference in space (which is leapfrog discretiza-tion) and implicit midpoint rule (which is symplectic) in time, it is easy to show that the Hamiltonian formulations in (5) and (7) for Maxwell's equations reduce to the same discretized system,

$\partial _{r}z_{ij,k}^{1}+M^{-1}K_{1}\overline {a}_{x_{1}}z_{ij,k}^{-1}+M^{-1}K_{2}\overline {a}_{x_{2}}^{-1}\frac {1}{2}+\frac {1}{k}}$ (18)

where indices i, j, k denote spatial increments and index I denotes time increment, and matrices M,K1,...as in(10).We refer to this particular discretization as the symplectic method, though it is also multisymplectic.

The symplectic method (18) is second-order in space and time, and is unconditionally stable. Furthermore, this discrete system preserves two discretized global conservation laws: the first one is the discrete quadratic global conservation law based on(8),

$\frac {1}{2}\partial _{t}[\mu H_{ijk}^{1}\cdot H_{ijk}^{1}+\epsilon E_{ijk}^{1}\cdot E_{ijk}^{1}]=0.$ (19)

The second discretized global conservation law for symplectic method is based on the helicity Hamiltonian functional (6)

$\partial _{t}[\frac {1}{2\epsilon }H_{ij,k}^{\prime }\cdot \hat {\nabla }\times H_{ij,k}^{\prime }+\frac {1}{2\mu }E_{ij,k}^{\prime }\cdot \hat {\nabla }\times E_{ij,k}^{\prime }]=0,$ (20)

where$\hat {V}\times =R_{1}\partial _{x_{1}}+R_{2}\partial _{x_{2}}+R_{3}\partial _{x_{3}}$. Furthermore, the scheme (18) is proved to be multisymplectic, since it preserves the fol-lowing multisymplectic conservation law

$\partial _{1}[E_{1}^{\prime }Ad_{1}^{\prime }+\partial _{0}[\frac {1}{\epsilon }m^{\prime }_{1}]_{1}^{\prime }+R_{1}a^{\prime 2}+R_{1}e^{\prime }]+0_{0}[\frac {1}{\epsilon }d_{1$

$+\partial _{x3}[\frac {1}{\epsilon }dH_{ijk-1}^{k-1}\wedge R_{3}dH_{ijk}^{l-\frac {1}{2}}+\frac {1}{\mu }dE_{ijjk-1}^{k-1}\wedge R_{3}dE_{ijk}^{k$ (21)

Besides the global conservation laws, for the scheme (18) applied to Maxwell's equations, we also have the following local conservation laws based on (13)-(15):

The discrete quadratic conservation law is

$\frac {1}{2}\partial _{t}[\mu _{1x}^{\prime }+\epsilon _{1x}^{\prime }+\epsilon _{1x}^{\prime }-E_{1y}^{\prime }-R_{1y}^{\prime }+R_{1y}^{\prime }+R_{1y}^{\prime }+\frac {1}{2}\partial _$

$+\frac {1}{2}\partial _{x3}[H_{ij,k}^{1+\frac {1}{2}}\cdot R_{3}E_{ij,k-1}^{1+\frac {1}{2}}+H_{ij,k-1}^{1+\frac {1}{2}}\cdot R_{ij,k}E_{k$ (22)

The discrete energy conservation law is

$0.[\frac {1}{2e}H_{ijk}^{\prime }、G\times H_{ijk}^{\prime }+\frac {1}{2\mu }E_{ijk}^{\prime }+\nabla \times E_{ijk}^{\prime }]+\partial _{x}[\frac {1}{2e}\partial _{ijk}\cdot R_{1}$

$+\partial _{\infty }[\frac {1}{2c}\partial H_{1k}^{*}\cdot R_{2k}^{*j}+\frac {1}{2\mu }\partial E_{1jk}^{\prime }-RE_{1j-k}^{\prime 2}]+\partial _{0}[\frac {1}{2c}\partial _{1k}^{\prime$ (23)

The discrete momentum conservation law is

6Let piand aare the functions at grid i,0,ð are the difference operators, then

$\partial [q_{i}p_{i}]=q_{i+1}+\partial p_{i}+\partial q_{i}p_{i}=\partial q_{i}p_{i+1}+q_{i}\partial p_{i},$

$\partial [q_{i+1}p_{i}]=\partial q_{i+1}p_{i+1}+q_{i+1}\partial p_{i},$

$\overline {a}(q_{i}p_{i}]=\overline {a}q_{i}p_{i+1}+q_{i-1}\overline {a}p_{i}=\overline {\sigma }p_{i}q_{i+1}+p_{i-1}\overline {a}q_{i},$

$\overline {a}[q_{i}p_{i+1}]=q_{i+1}\overline {a}p_{i+1}+\overline {a}q_{i}p_{i}.$

