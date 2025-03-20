解法 4: \( F(x) = g(x) \cdot f(x) = \frac{\sin(2x + \frac{\pi}{4})}{\sin(2x - \frac{\pi}{4})} \), 定义域为 \( \left\{ x \mid x \neq \frac{\pi}{8} + \frac{k\pi}{2}, k \in \mathbb{Z} \right\} \)

\[
F'(x) = \frac{2\cos(2x + \frac{\pi}{4}) \sin(2x - \frac{\pi}{4}) - 2\cos(2x - \frac{\pi}{4}) \sin(2x + \frac{\pi}{4})}{\sin^2(2x - \frac{\pi}{4})} = \frac{-2}{\sin^2(2x - \frac{\pi}{4})} < 0
\]

\( \therefore \) \( F(x) \) 的单调递减区间为 \( \left( -\frac{3\pi}{8} + \frac{k\pi}{2}, \frac{\pi}{8} + \frac{k\pi}{2} \right) k \in \mathbb{Z} \), 无递增区间。

评分标准:
(1) \( g(x) \) 表达式正确 2 分，
(2) 有化简结果正确 2 分：\( -\tan(2x + \frac{\pi}{4}), \frac{1}{\tan(2x - \frac{\pi}{4})}, \frac{1}{\tan 2x - 1}, \frac{-2}{\sin^2(2x - \frac{\pi}{4})} \), 无递增区
(3) 单调区间正确 1 分。

注：1. 有正确的体积公式，h 没算对，这 2 分也给！
2. 没有写出以上的任何一个解与点，去证明 A1E 垂直与平面 ABCD 的，给 2 分

18. 通过 \( \triangle A_1D_1C_1 \)，因为 \( A_1E \parallel D_1C_1 \)，故 \( A_1E \parallel \triangle B_1C_1D_1 \)

所以四面体 \( A_1EB_1C_1D_1 \) 为平行四边形 2 分

所以 \( A_1E = D_1C_1 = \frac{1}{2} BC = \frac{1}{2} \)

易得 \( \angle A_1AE = 60^\circ \)，即 \( A_1E = A_1E \)

所以 \( A_1E = \sqrt{AA_1^2 + AE^2 - 2 \cdot AA_1 \cdot AE \cdot \cos 60^\circ} = \frac{\sqrt{3}}{2} \)

上下底面面积分别为 \( S_1, S_2 \), 求的 \( S_1 = 9 \cdot \frac{3}{4}, S_2 = \frac{9}{4} \)

所以 \( \frac{7\sqrt{3} - h^2}{9} + \frac{5h^2}{2} = \frac{\sqrt{3}}{2} \), 从而有 \( h = \frac{\sqrt{3}}{2} \)

所以 \( h = \frac{\sqrt{3}}{2} \)

(2) 解法 1: 由 (1) 知平面 \( A_1A_2B_2B_1 \) 与平面 \( A_1C_1B_1 \)

又 \( BC \perp AB \)，所以 \( BC \perp 平面 A_1A_2B_2B_1 \)

所以平面 \( BCC_1B_1 \) 与平面 \( A_1A_2B_2B_1 \) 2 分

过 \( E \) 作 \( EH \perp BB_1 \) 于 \( H \)，则 \( EH \perp 平面 BCC_1B_1 \)

从而 \( \angle C_1EH \) 为直线 \( C_1E \) 与平面 \( BCC_1B_1 \) 所成角 2 分

\[
EH = BE \sin 60^\circ = \frac{3\sqrt{3}}{4}
\]

\[
C_1E = C_1B_1 + B_1E = C_1B_1 + BB_1 - 2BB_1 \cdot BE \cdot \cos 60^\circ = 2
\]

所以 \( C_1E = \sqrt{2} \)

所以 \( \sin \angle C_1EH = \frac{EH}{C_1E} = \frac{3\sqrt{6}}{8} \) 2 分