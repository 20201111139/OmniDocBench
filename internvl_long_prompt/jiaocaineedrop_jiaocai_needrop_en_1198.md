```markdown
所以 \( x_1 + x_2 = \frac{8k^2}{3 + 4k^2}, x_1 x_2 = \frac{4k^2 - 12}{3 + 4k^2} \),

\[
\begin{aligned}
(\text{法一}) |AF| \cdot |FB| &= \sqrt{(x_1 - 1)^2 + y_1^2} \cdot \sqrt{(x_2 - 1)^2 + y_2^2} \\
&= \sqrt{1 + k^2} \cdot |x_1 - 1| \cdot \sqrt{1 + k^2} \cdot |x_2 - 1| \\
&= (1 + k^2) \cdot |x_1 x_2 - (x_1 + x_2) + 1| \\
&= (1 + k^2) \cdot \left| \frac{4k^2 - 12}{3 + 4k^2} - \frac{8k^2}{3 + 4k^2} + 1 \right| \\
&= (1 + k^2) \cdot \left| \frac{9}{3 + 4k^2} \right| \\
&= \frac{9}{3 + 4k^2} \cdot (1 + k^2) \\
&= \frac{9}{3 + 4k^2} \cdot \left( 1 + \frac{1}{3 + 4k^2} \right) \\
&= \frac{9}{3 + 4k^2} \cdot (3 + 4k^2) \\
&= 9
\end{aligned}
\]

当 \( k^2 = 0 \) 时, 取最大值为 3, 所以 \( |AF| \cdot |FB| \) 的取值范围 \( \left( \frac{9}{4}, 3 \right] \).

又当 \( k \) 不存在, 即 \( AB \) 上 \( x \) 轴时, \( |AF| \cdot |FB| \) 取值为 \( \frac{9}{4} \).

所以 \( |AF| \cdot |FB| \) 的取值范围 \( \left( 0, \frac{9}{4} \right] \).

\[
\begin{aligned}
(\text{法二}) |AF| \cdot |FB| &= |AF| \cdot |FB| = -|AF| \cdot |FB| = -(x_1 - 1) \cdot (x_2 - 1) - 9y_1 y_2 \\
&= -(x_1 - 1) \cdot (x_2 - 1) - k^2 \cdot (x_1 - 1) \cdot (x_2 - 1) \\
&= -(1 + k^2) \cdot \left[ x_1 x_2 - (x_1 + x_2) + 1 \right] \\
&= -(1 + k^2) \cdot \left[ \frac{4k^2 - 12}{3 + 4k^2} + \frac{8k^2}{3 + 4k^2} + 1 - (1 + k^2) \right] \\
&= -(1 + k^2) \cdot \left[ \left( \frac{4k^2 - 12}{3 + 4k^2} = \frac{8k^2}{3 + 4k^2} \right) + 1 - (1 + k^2) \right] \\
&= -(1 - k^2) \cdot \left[ \frac{9}{3 + 4k^2} \right] \\
&= \frac{9}{3 + 4k^2} \cdot (k^2 - 1) \\
&= \frac{9}{3 + 4k^2} \cdot k^2
\end{aligned}
\]

当 \( k^2 = 0 \) 时，取最大值为 3, 所以 \( |AF| \cdot |FB| \)的取值范围 \( \left( \frac{9}{4}, 3 \right]  \).

又当 \( k \) 不存在, 即 \( AB \) 上 \( x  \) 轴时, \( |AF| \cdot |FB| \) 取值范围 \( \left( 0, \frac{9}{4} \right]  \).

例26. (2022-全国·南京外国语学校模拟预测) 已知抛物线 \( C: x^2 = 4y, F \) 为其焦点, 过 \( P \) 的直线 \( l \) 与 \( C \) 交于不同的两点 \( A, B \).

(1) 若直线 \( l \) 斜率为 3, 求 \( AB \);

(2) 如图, \( C \) 在点 \( A \) 处的切线与在点 \( B \) 处的切线交于点 \( P \), 连接 \( PF \), 证明: \( |PF|^2 = |AF| \cdot |BF| \).

【解析】(1) 由抛物线 \( C: x^2 = 4y \), 得 \( F(0, 1) \).

设直线 \( l \) 的方程为 \( y = 3x + 1 \),

设 \( A(x_1, y_1), B(x_2, y_2) \).

由 \( \begin{cases} y = 3x + 1 \\ x^2 = 4y \end{cases} \) 消去 \( y \) 得 \( x^2 - 12x - 4 = 0 \), 所以 \( \Delta > 0, x_1 + x_2 = 12 \),

所以 \( |AB| = |AF| + |FB| = y_1 + 1 + y_2 + 1 = 3(x_1 + x_2) + 4 = 40 \).

(2) 证明: 由题可知, 直线 \( l \) 的斜率存在, 设直线 \( l \) 的方程为 \( y = kx + 1, A(x_1, y_1) \),

\( B(x_2, y_2) \).

抛物线方程为 \( x^2 = 4y \), 即 \( y = \frac{x^2}{4}, y' = \frac{x}{2} \),

所以 \( A, B \) 为切点的切线方程分别为 \( y = 2y_1, x = 2x_1 + 2y_1 \).

由 \( \begin{cases} y = kx + 1 \\ x^2 = 4y \end{cases} \)  消去 \( y \) 得 \( x^2 - 4kx - 4 = 0 \), 所以 \( \Delta > 0, x1 + x_2 = 4k, x_1 x_2 = -4 \).

这两条切线的斜率分别为 \( k_1 = \frac{x_1}{2}, k_2 = \frac{x_2}{2} \).

由 \( k_1 k_2 = \frac{x_1 x_2}{4} = -1 \), 且 \( PA \perp PB \).

设 \( P(x_0, y_0) \), 则由 \( \begin{cases} y = 2y_1 + 2y_1 \\ y = 2y_2 + 2y_2 \end{cases} \) 得 \( x_0 = \frac{2(y_1 - y_2)}{k_1 - k_2} = 2k, y_0 = \frac{1}{2} (2y_1 + 2y_2) = kx_0 - y_0 = -1 \),

当 \( k = 0 \) 时, \( x_0 = 0 \), 可得 \( AB \perp PF \);

当 \( k \neq 0 \) 时, \( x_0 \neq 0, k_{AB} = \frac{y_1 - y_2}{x_1 - x_2} = \frac{k}{2}, k_{PP} = -\frac{2}{x_0} \), 所以 \( k_{AB} \cdot k_{PP} = -\frac{2}{x_0} = -1 \).
```