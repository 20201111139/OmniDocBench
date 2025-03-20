```markdown
1. 获取已知数据 \( X_{s1}, Y_{s1}, X_{s2}, Y_{s2}, Z_{s1}, Z_{s2}, \phi_{s1}, \omega_{s1}, K_{s1}, X_{s1}, Y_{s1}, Z_{s1}, \phi_{s2}, \omega_{s2}, K_{s2} \)
2. 量测像点坐标 \( X_{s1}, Y_{s1}, X_{s2}, Y_{s1} \)
3. 由外方位线元素计算基线分量 \( B_X, B_Y, B_Z \)
4. 由外方位角元素计算像空间辅助坐标 \( X_1, Y_1, Z_1, X_2, Y_2, Z_2 \) 需要旋转矩阵 \( R \)

\[
\begin{aligned}
B_X &= X_{s2} - X_{s1} = N_1 X_1 - N_2 X_2 \\
B_Y &= Y_{s2} - Y_{s1} = N_1 Y_1 - N_2 Y_2 \\
B_Z &= Z_{s2} - Z_{s1} = N_1 Z_1 - N_2 Z_2
\end{aligned}
\]

\[
\begin{aligned}
N_1 &= \frac{B_X Z_2 - B_X Z_1}{X_1 Z_2 - X_2 Z_1} \\
N_2 &= \frac{B_X Z_1 - B_X Z_2}{X_1 Z_2 - X_2 Z_1}
\end{aligned}
\]

5. 计算投影系数 \( N_1, N_2 \)
6. 计算地面坐标 \( X_A, Y_A, Z_A \)

# 利用立体像对确定地面点

- 共线条件严密解法
- 空间后方交会-空间前方交会解法
```