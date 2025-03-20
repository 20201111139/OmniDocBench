```markdown
解法 4: \( F(x) = \frac{g(x)}{f(x)} = \frac{\sin(2x + \frac{\pi}{4})}{\sin(2x - \frac{\pi}{4})} \)，定义域为 \( \left\{ x \mid x \neq \frac{\pi}{8} + \frac{k\pi}{2}, k \in \mathbb{Z} \right\} \)

\[ F'(x) = \frac{2\cos(2x + \frac{\pi}{4})\sin(2x - \frac{\pi}{4}) - 2\cos(2x - \frac{\pi}{4})\sin(2x + \frac{\pi}{4})}{\sin^2(2x - \frac{\pi}{4})} = \frac{-2}{\sin^2(2x - \frac{\pi}{4})} < 0 \]

\(\therefore F(x)\) 的单调递减区间为 \((-\frac{3\pi}{8} + \frac{k\pi}{2}, \frac{\pi}{8} + \frac{k\pi}{2}) k \in \mathbb{Z}\)，无递增区间。

评分标准：
(1) \( g(x) \) 表达式正确 2 分，
(2) 有化简结果正确 2 分：\(-\tan(2x + \frac{\pi}{4})\)，\(\frac{1}{\tan(2x - \frac{\pi}{4})}\)，\(1 + \frac{2}{\tan 2x - 1}\)，\(\sin^2(2x - \frac{\pi}{4}) < 0\)
(3) 单调区间正确 1 分。

---

18. 解：(1) 连接 \( AD \)，因为 \( AE \parallel D_1C_1 \)，所以 \( A, E, C_1, D_1 \) 四点共面，
因为 \( C_1E \parallel \) 平面 \( ADD_1A_1 \)，\( AD \) 是过 \( C_1E \) 的平面 \( AEC_1D_1 \) 与平面 \( ADD_1A_1 \) 的交线
由线面平行的性质定理，知 \( AD \parallel C_1E \)

所以四边形 \( AEC_1D_1 \) 为平行四边形 2 分

所以 \( AE = D_1C_1 = \frac{1}{2}DC = \frac{1}{2} \)

易得 \( \angle A_1AE = 60^\circ \)，又 \( A_1A = 1 \)，

所以 \( A_1E = \sqrt{A_1A^2 + AE^2 - 2A_1A \cdot AE \cdot \cos 60^\circ} = \frac{\sqrt{3}}{2} \)，同时可得 \( A_1E \perp AB \)。

上下底面积分别为 \( S_1, S_2 \)，易求得 \( S_1 = \frac{3}{4} \)，\( S_2 = \frac{3}{2} \)

所以 \( \frac{7\sqrt{3}}{16} = \frac{h}{3}(S_1 + \sqrt{S_1S_2} + S_2) = \frac{h}{3}(\frac{3}{4} + \frac{3}{8} + \frac{3}{2}) = \frac{7}{8}h \)，从而有 \( h = \frac{\sqrt{3}}{2} \) 2 分

所以 \( h = A_1E \)

---

(2) 解法 1：由 (1) 知平面 \( AA_1B_1B \) ⊥ 平面 \( ABCD \)

又 \( BC \perp AB \)，所以 \( BC \perp \) 平面 \( AA_1B_1B \)

所以平面 \( BCC_1B_1 \) ⊥ 平面 \( AA_1B_1B \)

过 \( E \) 作 \( EH \perp BB_1 \) 于 \( H \)，则 \( EH \perp \) 平面 \( BCC_1B_1 \)

从而 \( \angle EC_1H \) 为直线 \( C_1E \) 与平面 \( BCC_1B_1 \) 所成角 2 分

\( EH = BE \sin 60^\circ = \frac{3\sqrt{3}}{4} \)

\( C_1E^2 = C_1B_1^2 + B_1E^2 = C_1B_1^2 + BE^2 + BB_1^2 - 2 \cdot BB_1 \cdot BE \cdot \cos 60^\circ = 2 \)，即 \( C_1E = \sqrt{2} \)

所以 \(\sin \angle EC_1H = \frac{EH}{C_1E} = \frac{3\sqrt{6}}{8}\) 2 分
```