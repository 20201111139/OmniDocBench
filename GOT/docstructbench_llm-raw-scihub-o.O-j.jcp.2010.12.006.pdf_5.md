\[
\partial_{\mathbf{z}}I_{i j,k}^{j}=\frac{z_{i j,k}^{j}-z_{i j,k}}{\Delta t},\quad \partial_{\mathbf{z}}I_{z j,k}^{j}=\frac{z_{i j,k}^{j}-z^{\prime}_{i j,k}}{2\Delta t},\quad \partial_{\mathbf{x}}z_{i j,k}^{j}=\frac{z_{i-1}^{j}-z_{i j,k}}{\Delta x_{1}},\quad \partial_{\mathbf{x}}z_{i j,k}^{j} = \frac{z_{i-1}^{j}-z_{i-1}^{j}}{2\Delta x_{1}},\quad \partial_{\mathbf{x}}z_{i j, k}^{j} = \frac{z_{i-1}^{j}-z_{j-1}^{j}}{2\Delta x_{1}}.
\]
where the difference operators \(\partial_{\mathbf{t}}, \bar{o}\) are the discretization of \(\frac{\partial}{\partial \mathbf{t}}\), and the difference operators \(\partial_{\mathbf{x}_{1}}, \bar{o}_{\mathbf{x}_{2}}\) are the discretization of \(\frac{\partial}{\partial \mathbf{t}} \). Via these notations and the properties of the difference operators, \({ }^{6}\) we present the statement of the local/global conservation laws for the different numerical methods.
\subsection*{3.1. Symplectic method for Maxwell's equations}
The following method is constructed based on the method of lines, i.e. discretizing the Hamiltonian PDEs in space, then applying the symplectic method to the resulting Hamiltonian ODEs (see for example [6,. Later, we will show the method is also multisymplectic in the corresponding statement of multisymplecticity.
For Maxwell's equations in Hamiltonian form, we use the central finite difference in space (which is leapfrog discretization) and implicit midpoint rule (which is symplectic) in time, it is easy to show that the Hamiltonian formulations in (5) and (7) for Maxwell's equations reduce to the same discretized system,
\[
\partial_{\mathbf{z}}I_{j,k}^{j}+M^{-1}K_{1}\frac{\partial_{\mathbf{x}_{1}}z_{i j,k}^{j}}{\Delta t}+M^{-1}K_{2}\frac{\partial_{\mathbf{x}_{2}}z_{i j,k}^{j}}{\Delta t}+M^{-1} K_{3}\frac{\partial_{\mathbf{x}_{3}}z_{i j,k}^{j}}{\Delta t}=0,
\]
where indices \(i, j, k\) denote spatial increments and index \(l\) denotes time increment, and matrices \(M, K_{1}, \ldots\) as in (10). We refer to this particular discretization as the symplectic method, though it is also multisymplectic.
The symplectic method (18) is second-order in space and time, and is unconditionally stable. Furthermore, this discrete system preserves two discretized global conservation laws: the first one is the discrete quadratic global conservation law based on (8),
\[
\frac{1}{2} \partial_{\mathbf{t}}\left[\mu \mathbf{H}_{i j,k}^{\dagger} \cdot \mathbf{H}_{i j,k}^{\dagger}+\varrho \mathbf{E}_{i j,k}^{\dagger} \cdot \mathbf{E}_{i j,k}^{\dagger}\right]=0
\]
The second discretized global conservation law for symplectic method is based on the helicity Hamiltonian functional (6)
\[
\frac{1}{\partial t}\left[\frac{1}{2} \mathbf{H}_{i j,k}^{\dagger} \cdot \widetilde{\nabla} \times \mathbf{H}_{i j,k}^{\dagger}+\frac{1}{2} \mu \mathbf{E}_{i j,k}^{\dagger} \cdot \widetilde{\nabpsilon} \times \mathbf{E}_{i j,k}^{\dagger}\right]=0
,
\]
where \(\widetilde{\nabla} \times=\mathbf{R}_{1} \partial_{\mathbf{x}_{1}}+R_{2} \partial_{\mathbf{x}_{2}}+R_{3} \partial_{\mathbf{x}_{3}}\). Furthermore, the scheme (18) is proved to be multisymplectic, since it preserves the following multisymplectic conservation law
\[
\begin{array}{l}
\partial_{\mathbf{t}}\left[d \mathbf{E}_{i j,k}^{\dagger} \wedge d \mathbf{H}_{i j,k}^{\dagger}\right]+\partial_{\mathbf{x}_{1}}\left[\frac{1}{2} \mathbf{E} \mathbf{d} \mathbf{H}_{i j,k}^{\dagger-1} \wedge R_{1} \mathbf{d} \mathbf{H}_{i j,k}^{\mathbf{+1}}+\frac{1}{2} \mathbf{d} \mathbf{E}_{i j,k}^{\dagger-1} \wedge R_{1} d \mathbf{E}_{i j,k}^{\dagger-1}\right]+\partial_{\mathbf{x}_{2}}\left[\frac{1}{2} \mathbf{d} \mathbf{H}_{i j,k}^{\mathrm{+1}-1} \wedge R_{2} d \mathbf{H}_{i j,k}^{\mathrm{+1}-1}+\frac{1}{2} \mathbf{d} \mathbf{E}_{\mathbf{d}^{\prime-1}+1}^{\mathrm{+}}\right] \\
+\partial_{\mathbf{x}_{3}}\left[\frac{1}{2} \mathbf{E} \mathbf{\mathbf{d} \mathbf{H}_{i j,k}^{\dagger}-1} \wedge R_{3} d \mathbf{H}_{i j,k}^{\dagger-1}+\frac{1}{2} \mathbf{d} \mathbf{e}_{i j,k}^{\dagger-1} \wedge R_{3} d \mathbf{E}_{i j,k}^{\dagger-1}\mathbf{]}=0
\end{array}
\]
Besides the global conservation laws, for the scheme (18) applied to Maxwell's equations, we also have the following local conservation laws based on (13)-(15):
The discrete quadratic conservation law is
\[
\begin{array}{l}
\frac{1}{2} \partial_{\mathbf{t}}\left[\mathbf{\mu} \mathbf{H}_{i j,k}^{\dagger} \cdot \mathcal{H}_{i j,k}^{\dagger}+\varrho \mathbf{ E}_{i j,k}^{\dagger} \cdot \mathbf{E}_{i i j,k}^{\dagger}\right]+\frac{1}{2} \partial_{\mathbf{x}_{1}}\left[\mathbf{H}_{i j,k}^{\dagger} \cdot \mathbf R_{1} \mathbf{E}_{i i j,k}^{\dagger-1}+\mathbf{H}_{i j,k}^{\dagger} \mathbf{H}_{i j,k}^{\dagger}-\mathbf{R}_{1} \mathbf{E}_{i i j,k}^{\dagger-1}\right]+\frac{1}{2} \partial_{\mathbf{x}_{2}}\left[\mathbf{H}_{i j,k}^{\dagger-1} \cdot \mathbf{R}_{2} \mathbf{E}_{i j,k}^{\dagger-1}+\mathbf{H}_{i j,k-1}^{\dagger} \cdot \mathbf R_{2} \mathbf{E}_{i j,k}^{\dagger-1}\right] \\
\quad+\frac{1}{2} \partial_{\mathbf{x}_{3}}\left[\mathbf{H}_{i j,k}^{\dagger} \bullet \mathbf{R}_{3} \mathbf{E}_{i j,k}^{\dagger-1}+\boldsymbol{H}_{i j,k}^{\dagger-1} \cdot \mathbf R_{3} \mathbf{E}_{i j,k}^{\dagger-1}\right]=0
\end{array}
\]
The discrete energy conservation law is
\[
\begin{array}{l}
\partial_{\mathbf{t}}^{\dagger}\left[\frac{1}{2} \mathbf{E} \mathbf{h}_{i j,k}^{\dagger} \cdot \widetilde{\nabacket} \times \mathbf{E} \mathbf{h}_{i j,k}^{\dprime}+\frac{1}{2} \mathbf{E} \mathbf{H}_{i j,k}^{\dagger} \cdot \widehat{\nabla} \times \mathbf{E}^{\dagger} \mathbf{h}_{i j,k}^{\dagger}\right]+\partial_{\mathbf{x}_{2}}\left[\frac{1}{\mathbf{E}^{\dagger}} \partial_{\mathbf{t}}\mathbf{H}_{i j,k}^{\dagger} \cdot \mathbf{\mathbf R}_{1} \mathbf{H}_{i j,k}^{\dagger-1}+\frac{\mathbf{1}}{\mathbf{2}} \partial_{\mathbf{t}}\mathbf{H}_{i j,k}\left.\cdot \mathbf{R}_{1} \mathbf{H}_{i j,k}^{\dagger-1}\right.+\frac{\mathbf{1}}{\mathbf{2}} \partial_{\mathcal{t}}\mathbf{H}_{i j,k}^{\dagger} \bullet \mathbf{\mathbf R}_{1}^{\dagger} \mathbf{H}_{i j,k}^{\dprime-1} \right] \\
\quad+\partial_{\mathbf{x}_{2}}\left[\frac{1}{2} \partial_{\mathbf{t}}\mathbf{H}_{i j,k}^{i} \cdot \mathbf{R}_{2} \mathbf{H}_{i j,k}^{\dagger-1}+\mathbf{1}}{\partial_{\mathbf{t}}\mathbf{H}_{i j,k}^i \cdot \mathbf{R}_{2} \mathbf{H}_{i j,k}\left.\cdot \mathbf{R}_{2}^{\dagger} \mathbf{H}_{i j,k}^{\d�-1}\right.+\mathbf{1}}\right]+\partial_{\mathbf{x}_{2}}\left[\frac{1}{2}\partial_{\mathbf{t}}\mathbf{H}_{i j,k}^{} \cdot \mathbf{R}_{3} \mathbf{H}_{i j,k}^{\dagger-1}+\left.1}{\Omega^{\mathbf{t}}\mathbf{H}_{i j,k}^{\dagger}\cdot \mathbf{R}_{3} \mathbf{H}_{i j,k}^{i-1}}\right]=0
\end{array}
\]
The discrete momentum conservation law is
\footnotetext{
\({ }^{6}\) Let \(p_{i}\) and \(q_{i}\) are the functions at grid \(i, \partial, \bar{u}\) are the difference operators, then
\[
\begin{array}{l}
\partial_{\mathbf{t}}(q_{i} p_{i}]=q_{i+1} \partial_{\mathbf{t}} p_{i}+\partial_{\mathbf{t}} q_{i} p_{i}=0 q_{i} p_{i+1}+q_{i} \partial_{\mathbf{t}} p_{i}, \\
\partial_{\mathbf{t}}(q_{i+1} p_{i}]=\partial_{\mathbf{t}} q_{i+1} p_{i+1}+q_{i+1} \partial_{\mathbf{t}} p_{i}, \\
\partial_{\hat{\mathbf{t}}}(q_{i} p_{i}]=\partial_{\hat{\mathbf{t}}}(q_{i} p_{i+1}+q_{i-1} \partial_{\hat{\mathbf{t}}} p_{i}=0 p_{i} p_{i+1}+p_{i-1} \partial_{\hat{\mathbf{t}}}(q_{i} p_{i+2} p_{i+1}+q_{i-1} \partial_{\hat{t}} p_{i}, \\
\partial_{\hat{\mathbf{t}}}\left(q_{i} p_{i+1}\right]=q_{i+1} \partial_{\hat{\mathbf{t}}+1}+\partial_{\hat{\mathbf{t}}} q_{i} p_{i} .
\end{array}
\]