```markdown
Y. Sun, P.S. Tseng/Journal of Computational Physics 230 (2011) 2076-2094

\[
\begin{aligned}
\partial_{i} \mathcal{H}_{jk} &= \frac{1}{\Delta t} \left( \mathcal{H}_{jk}^{i+1} - \mathcal{H}_{jk}^{i-1} \right), \quad \partial_{i} \mathcal{E}_{jk} = \frac{1}{\Delta t} \left( \mathcal{E}_{jk}^{i+1} - \mathcal{E}_{jk}^{i-1} \right), \\
\partial_{j} \mathcal{H}_{ik} &= \frac{1}{\Delta t} \left( \mathcal{H}^{j+1}_{ik} - \mathcal{H}^{j-1}_{ik} \right), \quad \partial_{j} \mathcal{E}_{ik} = \frac{1}{\Delta t} \left( \mathcal{E}^{j+1}_{ik} - \mathcal{E}^{j-1}_{ik} \right), \\
\partial_{k} \mathcal{H}_{ij} &= \frac{1}{\Delta t} \left( \mathcal{H}_{{ij}}^{k+1} - \mathcal{H}_{{ij}}^{k-1} \right), \quad \partial_{k} \mathcal{E}_{ij} = \frac{1}{\Delta t} \left( \mathcal{E}_{{ij}}^{k+1} - \mathcal{E}_{{ij}}^{k-1} \right),
\end{aligned}
\]

where the difference operators \(\partial_{i}\), \(\partial_{j}\), \(\partial_{k}\) are the discretization of \(\partial_{x}\), \(\partial_{y}\), \(\partial_{z}\) and the difference operators \(\partial_{i}^{0}\), \(\partial_{j}^{0}\), \(\partial_{k}^{0}\) are the discretization of \(\partial_{t}\). Via these notations and the properties of the difference operators,\(^{6}\) we present the statement of the local/global conservation laws for the different numerical methods.

## 3.1. Symplectic method for Maxwell's equations

The following method is constructed based on the method of lines, i.e. discretizing the Hamiltonian PDEs in space, then applying the symplectic method to the resulting Hamiltonian ODEs (see for example (6.22)). Later, we will show the method is also multisymplectic in the corresponding statement of the multisymplecticity. For Maxwell's equations in the form (5), we use the central difference in space (which is leapfrog discretization) and implicit midpoint rule (which is symplectic) in time, it is easy to show that the Hamiltonian formulations in (5) and (7) for Maxwell's equations reduce to the same discretized system,

\[
\begin{aligned}
\partial_{i} \mathcal{H}_{jk}\mathcal{H}_{jk}^{i+1} + \partial_{i} \mathcal{E}_{jk}\mathcal{E}_{jk}^{i+1} + \partial_{j} \mathcal{H}_{ik}\mathcal{H}_{ik}^{j+1} + \partial_{j} \mathcal{E}_{ik}\mathcal{E}_{ik}^{j+1} + \partial_{k} \mathcal{H}_{ij}\mathcal{H}_{ij}^{k+1} + \partial_{k} \mathcal{E}_{ij}\mathcal{E}_{ij}^{k+1} = 0,
\end{aligned}
\]

where indices \(i, j, k\) denote spatial increments and index \(l\) denotes time increment, and matrices \(M_{1}, M_{2}, \ldots\) as in (10). We refer to this particular discretization as the second-order in method, though it is also unconditionally multisymplectic. Furthermore, this discrete system preserves two discretized global conservation laws: the first one is the discrete quadratic global conservation law based on (8),

\[
\frac{1}{2} \partial_{i} \left[ \mathcal{H}_{jk}^{i+1} \cdot \mathcal{H}_{jk}^{i-1} + \mathcal{E}_{jk}^{i+1} \cdot \mathcal{E}_{jk}^{i-1} \right] = 0,
\]

The second discretized global conservation law for symplectic method is based on the helicity Hamiltonian functional (6)

\[
\partial_{t} \left[ \frac{1}{2\mu} \mathcal{H}_{jk} \cdot \nabla \times \mathcal{H}_{jk} + \frac{1}{2\epsilon} \mathcal{E}_{jk} \cdot \nabla \times \mathcal{E}_{jk} \right] = 0,
\]

where \(\nabla \times = R_{i} \partial_{i} + R_{j} \partial_{j} + R_{k} \partial_{k}\). Furthermore, the scheme (18) is proved to be multisymplectic, since it preserves the following multisymplectic conservation law

\[
\begin{aligned}
\partial_{i} \left[ \mathcal{H}_{jk}^{i+1}\mathcal{H}_{jk}^{i-1} + \mathcal{E}_{ik}^{i+1}\mathcal{E}_{ik}^{i-1} \right] + \partial_{j} \left[ \mathcal{H}_{ik}^{j+1}\mathcal{H}_{ik}^{j-1} + \mathcal{E}_{ij}^{j+1}\mathcal{E}_{ij}^{j-1} \right] + \partial_{k} \left[ \mathcal{H}_{ij}^{k+1}\mathcal{H}_{ij}^{k-1} + \mathcal{E}_{ij}^{k+1}\mathcal{E}_{ij}^{k-1} \right] = 0.
\end{aligned}
\]

Besides the global conservation laws, for the scheme (18) applied to Maxwell's equations, we also have the following local conservation laws based on (13)-(15) law is

\[
\begin{aligned}
\frac{1}{2} \partial_{i} \left[ \mathcal{E}_{jk}^{i+1} \cdot \mathcal{H}_{jk}^{j+1} + \mathcal{E}_{jk}^{i+1} \cdot \nabla \times \mathcal{H}_{jk}^{i+1} + \mathcal{E}_{ik}^{i+1} \cdot \nabla \times \mathcal{H}^{i+1}_{ik} + \mathcal{E}_{ij}^{i+1} \cdot \nabla \times \mathcal{H}_{{ij}}^{i+1} \right] + \frac{1}{2} \partial_{j} \left[ \mathcal{E}_{jk}^{j+1} \cdot \mathcal{H}_{jk}^{i+1} + \mathcal{E}^{j+1}_{jk} \cdot \nabla \times \mathcal{H}_{jk}^{j+1} + \mathcal{E}^{j+1}_{ik} \cdot \nabla \times \mathcal{H}_{ik}^{j+1} + \mathcal{E}^{j+1}_{ij} \cdot \nabla \times \mathcal{H}_{ij}^{j+1} \right] \\
+ \frac{1}{2} \partial_{k} \left[ \mathcal{E}_{jk}^{k+1} \cdot \mathcal{H}_{jk}^{i+1} +  \mathcal{E}^{k+1}_{jk} \cdot \nabla \times \mathcal{H}_{ik}^{k+1} + \mathcal{E}^{k+1}_{ik} \cdot \nabla \times \mathcal{H}_{ij}^{k+1} + \mathcal{E}^{k+1}_{ij} \cdot \nabla \times \mathcal{H}_{jk}^{k+1} \right] = 0.
\end{aligned}
\]

The discrete energy conservation law is

\[
\begin{aligned}
\partial_{t} \left[ \frac{1}{2\mu} \mathbb{H}_{jk} \cdot \nabla \times \mathbb{H}_{jk} + \frac{1}{2\epsilon} \mathbb{E}_{jk} \cdot \nabla \times \mathbb{E}_{jk} \right] + \frac{1}{2\mu} \partial_{i} \left[ \mathbb{H}_{jk}^{i+1} \cdot \mathbb{H}_{jk}^{i-1} + \mathbb{E}_{jk}^{i+1} \cdot \mathbb{E}_{jk}^{i-1} \right] + \frac{1}{2\epsilon} \partial_{i} \left[ \mathbb{E}_{jk}^{i+1} \cdot \mathbb{H}_{jk}^{j+1} + \mathbb{E}_{ik}^{i+1} \cdot \mathbb{H}_{ik}^{i+1} + \mathbb{E}_{ij}^{i+1} \cdot \mathbb{H}_{ij}^{i+1} \right] = 0.
\end{aligned}
\]

The discrete momentum conservation law is

\[
\begin{aligned}
\partial_{t} \left[  \frac{1}{2\mu} \mathbb{H}_{jk} \cdot R_{i} \mathbb{H}_{jk} + \frac{1}{2\epsilon} \nabla \times \mathbb{E}_{jk} \cdot R_{i} \mathbb{E}_{jk} \right] + \frac{1}{2\epsilon} \partial_{i}  \left[ \mathbb{E}_{jk}^{i+1} \cdot R_{i} \mathbb{E}_{jk}^{i+1} + \mathbb{E}_{ik}^{i+1} \cdot R_{i} \mathbb{E}_{ik}^{i+1} + \mathbb{E}_{ij}^{i-1} \cdot R_{i} \mathbb{E}_{ij}^{i-1} \right] = 0.
\end{aligned}
\]

\(^{6}\) Let \(p\), \(q\) and \(a\) be the functions at grid \(i\), \(\partial_{i}\) are the difference operators, then

\[
\begin{aligned}
\partial_{i} p_{i} q_{i} &= \partial_{i} p_{i} \cdot q_{i} + p_{i} \cdot \partial_{i} q_{i}, \\
\partial_{i} \left( p_{i} q_{i} \right) &= \partial_{i} p_{i} \cdot q_{i} + p_{j} \cdot \partial_{i} q_{i}, \\
\partial_{i} \mathbb{P}_{i} \mathbb{Q}_{i} &= \partial_{i} p_{i} \cdot q_{i} + \mathbb{P}_{i} \cdot \partial_{i} q_{i}, \\
\partial_{i} p_{i} q_{i} &= \partial_{i} q_{i} \cdot p_{i} + q_{i} \cdot \partial_{i} p_{i}.
\end{aligned}
\]
```