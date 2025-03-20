# 奇点分类 (III)

- Δ=0 A, 有两个相同的特征值

\[
\mathbf{P}^{-1} \mathbf{A} \mathbf{P} = \begin{pmatrix} \lambda & 0 \\ 0 & \lambda \end{pmatrix}
\]

\[
\begin{cases}
\frac{du}{dt} = \lambda u \\
\frac{dv}{dt} = \lambda v
\end{cases}
\quad
\begin{cases}
u = u_0 e^{\lambda t} \\
v = v_0 e^{\lambda t}
\end{cases}
\quad
\begin{cases}
\frac{u}{v} = \frac{u_0}{v_0}
\end{cases}
\]

- α < 0, λ < 0
- α > 0, λ > 0

\[
\frac{du}{dt} = \mathbf{P}^{-1} \mathbf{A} \mathbf{P u}
\]

\[
\alpha = \text{tr}(\mathbf{A}) = \lambda_1 + \lambda_2
\]

\[
\beta = |\mathbf{A}| = \lambda_1 \lambda_2
\]