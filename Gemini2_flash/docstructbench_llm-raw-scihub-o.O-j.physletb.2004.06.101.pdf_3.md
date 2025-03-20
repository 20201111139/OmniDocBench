S.V. Kuzmin, D.G.C. McKeon / Physics Letters B 596 (2004) 301-305
303
For consistency, the time derivative of the constraints of (10) must vanish and hence they must have vanishing
Poisson bracket with \(H\). Using the fundamental Poisson brackets
\[
[U(x), \Pi^{U}(y)] = \delta(x - y),
\]
etc., we find that the primary constraints of (10) imply the secondary constraints
\[
(\Sigma, \Sigma_{i}) = (-\partial_{k}\Pi^{k}, \epsilon^{ijk}\partial_{j}(\Pi^{B}_{k} - mV_{k}) - \mu^{2}B_{i}).
\]
If \(\mu^{2} = 0\) (the Cremmer-Scherk model Lagrangian [1]), the constraints of (14) would become reducible as then
\(\partial_{i}\Sigma_{i} = 0\) and only the transverse portions of \(\Sigma_{i}\) are constraints. Furthermore, with \(\mu^{2} \neq 0\), the requirement \(\dot{\Sigma}_{i} = 0\)
leads to a tertiary constraint
\[
T_{k} = \mu^{2}\Pi^{B}_{k} = 0
\]
with \(\Sigma_{i}\) and \(T_{k}\) constituting second class constraints as
\[
[T_{k}(x), \Sigma_{i}(y)] = \mu^{4}\delta_{ik}\delta(x - y).
\]
All other constraints are first class and no further constraints need to be imposed for consistency. There are
consequently five first class constraints (\(\Phi^{U}, \Phi^{A}_{k}\) and \(\Sigma\)) and six second class constraints (\(\Sigma_{i}\) and \(T_{k}\)). The con-
straints \(\Phi^{U}\) and \(\Sigma\) correspond to the usual gauge transformations \(\delta W_{0} = \partial_{0}\Omega\), \(\delta W_{i} = \partial_{i}\Omega\) associated with a gauge
field \(W_{\mu}\), while \(\Phi^{A}_{k}\) is associated with the fact that in (12) \(A_{k}\) acts merely as a Lagrange multiplier (i.e., it is not
dynamical) and hence its value is completely arbitrary. Suitable gauge conditions associated with the first class
constraints are
\[
(\gamma^{U}, \gamma^{A}_{k}, \gamma^{V}) = (U, A_{k}, \partial_{k}V_{k}) = 0.
\]
From (10), (14), (15) and (17) it is evident that the only dynamical degrees of freedom are
\[
V^{T}_{i} = (\delta_{ij} - \partial_{i}\partial_{j}/\nabla^{2})V_{j}.
\]
We can verify this directly by explicitly eliminating the non-physical degrees of freedom in (4). First, one
decomposes \(V_{k}\), \(A_{k}\) and \(B_{k}\) into transverse \((T)\) and longitudinal \((L)\) parts where
\[
\nabla \times V^{L} = 0 = \nabla \cdot V^{T},
\]
etc., (4) now becomes
\[
\begin{aligned}
2L = (\dot{B}^{L})^{2} - (\nabla \cdot B^{L})^{2} + [B^{T} - \nabla \times A^{T}]^{2} + (\dot{V}^{T})^{2} - (\nabla \times V^{T})^{2} + [\dot{V}^{L} - \nabla U]^{2} \\
+ 2m [V^{T} \cdot (\nabla \times A^{T}) + B^{L} \cdot \dot{V}^{L} + B^{T} \cdot \dot{V}^{T} - B^{L} \cdot \nabla U] + 2\mu^{2}[A^{T} \cdot B^{T} + A^{L} \cdot B^{L}].
\end{aligned}
\]
The equations of motion for \(A^{L}\) and \(U\), respectively, imply that
\[
B^{L} = 0 = \dot{V}^{L} - \nabla U,
\]
reducing (20) to
\[
2L = (\dot{V}^{T})^{2} - (\nabla \times V^{T})^{2} + [B^{T} - \nabla \times A^{T}]^{2} + 2mV^{T} \cdot (\nabla \times A^{T}) + 2mB^{T} \cdot \dot{V}^{T} + 2\mu^{2}A^{T} \cdot B^{T}.
\]
Since
\[
A^{T} \cdot B^{T} = -(\nabla \times A^{T}) \cdot (\nabla^{2})^{-1} (\nabla \times B^{T}),
\]
we can eliminate \(\nabla \times A^{T}\) from (22) to obtain
\[
\nabla \times A^{T} = \dot{B}^{T} - mV^{T} + \mu^{2}(\nabla^{2})^{-1} (\nabla \times B^{T}).
\]