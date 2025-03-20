# 奇点分类（III）

- \(\Delta = 0 \, A\)，有两个相同的特征值

\[ 
\text{P}^{-1} \text{AP} = 
\begin{pmatrix} 
\lambda & 1 \\ 
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
\frac{du}{dt} = \text{P}^{-1} \text{AP} u 
\]

\[
\alpha = \text{tr}(\text{A}) = \lambda_1 + \lambda_2
\]

\[
\beta = |\text{A}| = \lambda_1 \lambda_2
\]