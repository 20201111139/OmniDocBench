## 数 学

本试卷共 4 页， 22 题。全卷满分 150 分，考试用时 120 分钟。

## 注意事项:

1. 答卷前，考生务必将自己的姓名，准考证号填写在答题卡上。
2. 回答选择题时，用铅笔把答题卡上对应题目的答案标号涂黑，写在本试卷上无效。
3. 考试结束后，将本试卷和答题卡一并交回。
4. 本试卷由 kmath.cn 自动生成。

| 得分 |  |
| :-- | :-- |
| 闰卷人 |  |

一、 单选题：本题共 10 个题，每小题 5 分，共 40 分。在每小题给出的四个选项中，只有一项是符合题目要求的。

1. 设 $f(x)=\left|\begin{array}{cccc}2 x & x & 1 & 0 \\ 1 & x & 2 & 3 \\ 2 & 3 & x & 2 \\ 1 & 1 & 2 & 2 x\end{array}\right|$ 中, 则 $x^{3}$ 的系数是
A. -2
B. 2
C. 4
D. -4
[答案]: A [解析]: 解析： $x$ 的关联项是 $\alpha_{12} \alpha_{21} \alpha_{33} \alpha_{44}$ ，前面需要有一个 $(-1)^{t}$ 他的逆序数是 $t(2143)=1$ 所以, -2
2. 在下列 5 阶行列式中, 符号为正的项是
A. $\alpha_{13} \alpha_{24} \alpha_{33} \alpha_{41} \alpha_{55}$
B. $\alpha_{13} \alpha_{21} \alpha_{22} \alpha_{44} \alpha_{53}$
C. $\alpha_{23} \alpha_{32} \alpha_{41} \alpha_{15} \alpha_{54}$
D. $\alpha_{31} \alpha_{35} \alpha_{43} \alpha_{14} \alpha_{52}$
[答案]:B [解析]:
3. 已知矩阵 $A=\left(\begin{array}{ccc}1 & 2 & 1 \\ -1 & 0 & 1 \\ 0 & 1 & 0\end{array}\right), A^{*}$ 为 $A$ 的伴随矩阵，则 $\left|A^{*}\right|=$
A. $-\frac{1}{2}$
B. $\frac{1}{4}$
C. 2
D. 4
[答案]:D [解析]: 先记住一个结论 $\left|A^{*}\right|=\left|A\right|^{\alpha-1}$ 其中 $n$ 为行列式的阶数. 所以, $\left|A^{*}\right|=\left|A\right|^{2}=4$
4. 设 $A=\left(\begin{array}{ll}2 & 3 \\ 3 & 0 \\ 1 & 2\end{array}\right), B=\left(\begin{array}{rrr}2 & 1 & 3 \\ -3 & 0 & -1\end{array}\right)$, 则 $|A B|=$
A. 0
B. 4
C. 6
D. 8

数学试题第 1 页（共 0 页）
[答案]: A [解析]: 本题, 很多同学容易想到 $|A B|=|A| \cdot|B|$ 但是, 他的前提是 $A, B$ 都是方阵, 所以本题不能直接使用这个公式. 计算可得

$$
A B=\left(\begin{array}{ccc}
-5 & 2 & 3 \\
6 & 3 & 9 \\
-4 & 1 & 1
\end{array}\right)_{3 \times 3} \quad|A B|=\left|\begin{array}{ccc}
-5 & 2 & 3 \\
6 & 3 & 9 \\
-4 & 1 & 1
\end{array}\right|
$$

然后利用初等变换可以得到结果是 0
5. 已知 $A, B$ 都是 $n$ 阶矩阵, 且 $A B=0$, 则必有
A. $A=0$ 或 $B=0$
B. $|A|=|B|=0$
C. $A=B=0$
D. $|A|=0$ 或 $|B|=0$
[答案]:D [解析]: 本题考查的基本概念, 例如 $A=\left(\begin{array}{ll}1 & 0 \\ 0 & 0\end{array}\right) \quad B=\left(\begin{array}{ll}0 & 0 \\ 0 & 1\end{array}\right) \quad A B=\left(\begin{array}{ll}0 & 0 \\ 0 & 0\end{array}\right)$ 但是 $A, B$ 都不是零.

由 $A B=0$ 同时取行列式 $\begin{aligned} & |A B|=|0|=0 \\ & |A| \cdot|B|=0\end{aligned}$ 所以, 选 D
6. 可量组 $\alpha_{1}=(1,1,1,1)^{T}, \alpha_{2}=(1,2,3,4)^{T}, \alpha_{3}=(0,1,2,3)^{T}$ 的称为
A. 1
B. 2
C. 3
D. 4

[答案]:B [解析]: 根据三秩相等定理：列向量组的秩等于列向量组所构成的秩，等于矩阵行向量组的秩. $R\left(\alpha_{1}, \alpha_{2}, \alpha_{3}\right)=R(A)$ 而

$$
A=\left(\begin{array}{lll}
1 & 1 & 0 \\
1 & 2 & 1 \\
1 & 3 & 2 \\
1 & 4 & 3
\end{array}\right)
$$

对 A 进行初等变换求秩

$$
A=\left(\begin{array}{lll}
1 & 1 & 0 \\
1 & 2 & 1 \\
1 & 3 & 2 \\
1 & 4 & 3
\end{array}\right) \Leftrightarrow\left(\begin{array}{lll}
1 & 1 & 0 \\
0 & 1 & 1 \\
0 & 0 & 0 \\
0 & 0 & 0
\end{array}\right)
$$

可见秩为 2
7. 设 $A$ 是 3 阶矩阵, 且 $|A|=-2$ 则 $\left|\left(\frac{1}{12} A\right)^{-1}+(3 A)^{*}\right|=$
A. -108
B. 108
C. 54
D. -54
[答案]:B [解析]: 对于矩阵有一个性质, 如果 A 可逆, 那么 $(\lambda A)^{-1}=\frac{1}{\lambda} \cdot A^{-1}$ 所以, $\left(\frac{1}{12} A\right)^{-1}=12 A^{-1}$而对于伴随矩阵的性质有 $A^{-1}=\frac{1}{|A|} \cdot A^{*}$