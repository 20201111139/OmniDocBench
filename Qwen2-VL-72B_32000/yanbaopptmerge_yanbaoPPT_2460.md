# 奇点分类（III）

- \(\Delta = 0\) A，有两个相同的特征值

\[
P = \begin{pmatrix}
1 & 2 \\
1 & 2
\end{pmatrix} \quad P^{-1}AP = \begin{pmatrix}
\lambda & 0 \\
0 & \lambda
\end{pmatrix}
\]

\[
\begin{cases}
\frac{du}{dt} = \lambda u \\
\frac{dv}{dt} = \lambda v
\end{cases}
\]

\[
\begin{cases}
u = u_0 e^{\lambda t} \\
v = v_0 e^{\lambda t}
\end{cases}
\]

\[
\frac{u}{v} = \frac{u_0}{v_0}
\]

- \(\alpha < 0, \lambda < 0\)
- \(\alpha > 0, \lambda > 0\)

\[
\frac{du}{dt} = P^{-1}APu
\]

\[
\alpha = \text{tr}(A) = \lambda_1 + \lambda_2
\]

\[
\beta = |A| = \lambda_1 \lambda_2
\]