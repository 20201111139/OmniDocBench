```markdown
## (II) 解法 1: 由 (I) 知, ∠A'OC = 120°

如图建系 O-xyz, B(1, 0, 0), 设 OC = b, OA' = a, 则 C(0, b, 0), A'(0, -\frac{1}{2}a, \frac{\sqrt{3}}{2}a)

BC = (-1, b, 0)

平面 A'DB 的法向量为 \(\vec{n} = (0, \sqrt{3}, 1)\)

\(\sin 45° = \left| \cos \left< \vec{n}, \vec{BC} \right> \right| = \left| \frac{\vec{n} \cdot \vec{BC}}{\left| \vec{n} \right| \left| \vec{BC} \right|} \right|\)

解得 \(b = \sqrt{2}\), BC = \(\sqrt{3}\)

解法 2: 由 (I) 知, ∠A'OC = 120°

过 C 作 CH ⊥ A'O, BD ⊥ 平面 A'OC,

∴ BD ⊥ CH, CH ⊥ A'O, CH ⊥ 平面 A'BD

∠CBH 就是 BC 与平面 A'BD 所成角

设 CO = x, 则 CH = \(\frac{\sqrt{3}}{2}x\), CB = \(\sqrt{2}CH = \frac{\sqrt{6}}{2}x\),

CB = \(\sqrt{OB^2 + OC^2} = \sqrt{1 + x^2}\), 则 \(\frac{\sqrt{6}}{2}x = \sqrt{1 + x^2}\)

解得 \(x = \sqrt{2}\), BC = \(\sqrt{3}\)

## 21. 解:

(I) 联立方程组 \(\begin{cases} y = kx + 1 \\ x^2 - 4y^2 = 4 \end{cases}\) 消 y 得: \((1 - 4k^2)x^2 - 8kx - 8 = 0\)

\(\begin{cases} 1 - 4k^2 \neq 0 \\ \Delta = 32 - 64k^2 > 0 \end{cases}\) 解得 \(-\frac{\sqrt{2}}{2} < k < \frac{\sqrt{2}}{2}\) 且 \(k \neq \pm \frac{1}{2}\)

(漏 \(k \neq \pm \frac{1}{2}\) 得 4 分)

(II) 设 M, N 坐标分别为 \((x_1, y_1)\), \((x_2, y_2)\), A(-2, 0), 由 (I) 知

\(\begin{cases} x_1 + x_2 = \frac{8k}{1 - 4k^2} \\ x_1 \cdot x_2 = \frac{-8}{1 - 4k^2} \end{cases}\)

直线 MA 的方程为 \(y = \frac{y_1}{x_1 + 2}(x + 2)\), 令 \(x = 0\) 可得点 P 坐标为 \(\left( 0, \frac{2y_1}{x_1 + 2} \right)\)

同理点 Q 坐标为 \(\left( 0, \frac{2y_2}{x_2 + 2} \right)\)

\(|PQ| = 1 \Rightarrow \left| \frac{y_1}{x_1 + 2} - \frac{y_2}{x_2 + 2} \right| = \frac{1}{2} \Rightarrow \left| \frac{(x_1 - x_2)(1 - 2k)}{(x_1 + 2)(x_2 + 2)} \right| = \frac{1}{2}\)

\(|4\sqrt{2}\sqrt{1 - 2k^2}(1 - 2k)| = 2(2k - 1)^2\)
```