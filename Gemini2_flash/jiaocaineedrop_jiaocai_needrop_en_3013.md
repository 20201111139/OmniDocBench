1. 获取已知数据\(X_0, y_0, f, X_{s1}, Y_{s1}, Z_{s1}, \phi_1, \omega_1, \kappa_1, X_{s2}, Y_{s2}, Z_{s2}, \phi_2, \omega_2, \kappa_2\)

2. 量测像点坐标\(x_1, y_1, x_2, y_2\)

3. 由外方位线元素计算基线分量\(B_x, B_y, B_z\)

4. 由外方位角元素计算像空间辅助坐标\(X_1, Y_1, Z_1, X_2, Y_2, Z_2\)(需要旋转矩阵R)
\[
\begin{aligned}
B_x &= X_{s2} - X_{s1} = N_1X_1 - N_2X_2 \\
B_y &= Y_{s2} - Y_{s1} = N_1Y_1 - N_2Y_2 \\
B_z &= Z_{s2} - Z_{s1} = N_1Z_1 - N_2Z_2
\end{aligned}
\]

\[
\begin{aligned}
N_1 &= \frac{B_xZ_2 - B_zX_2}{X_1Z_2 - X_2Z_1} \\
N_2 &= \frac{B_xZ_1 - B_zX_1}{X_1Z_2 - X_2Z_1}
\end{aligned}
\]

5. 计算投影系数\(N_1, N_2\)

6. 计算地面坐标\(X_A, Y_A, Z_A\)

## 利用立体像对确定地面点

*   共线条件严密解法

*   空间后方交会-空间前方交会解法
