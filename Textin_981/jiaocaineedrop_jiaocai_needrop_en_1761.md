例4：已知数列$\{a_{n}\}$满足$a_{1}=2,a_{n+1}=2(1+\frac {1}{n})^{2}a_{n},n\in N_{+}$

（1）求证：数列$\{\frac {a_{n}}{n^{2}}\}$是等比数列，并求出数列$\{a_{n}\}$的通项公式

（2）设$c_{n}=\frac {n}{a_{n}}$，求证： $c_{1}+c_{2}+\cdots +c_{n}<\frac {17}{24}$

解：（1） $a_{n+1}=2(1+\frac {1}{n})^{2}a_{n}=2\cdot \frac {(n+1)^{2}}{n^{2}}a_{n}$

$\therefore \frac {a_{n+1}}{(n+1)^{2}}=2\cdot \frac {a_{n}}{n^{2}}$ $\therefore \{\frac {a_{n}}{n^{2}}\}$是公比为2的等比数列

$\cdot \frac {a_{n}}{n^{2}}=(\frac {a_{1}}{1^{2}})\cdot 2^{n-1}=2^{n}$

$\therefore a_{n}=n^{2}\cdot 2^{n}$

（2）思路： $c_{n}=\frac {n}{a_{n}}=\frac {1}{n\cdot 2^{n}}$，无法直接求和，所以考虑放缩成为可求和的通项公式（不等号：&lt;)，若要放缩为裂项相消的形式，那么需要构造出“顺序同构”的特点。观察分母中有n，故分子分母通乘以(n-1)，再进行放缩调整为裂项相消形式。

解： $c_{n}=\frac {n}{a_{n}}=\frac {1}{n\cdot 2^{n}}=\frac {n-1}{n(n-1)2^{n}}$

而$\frac {1}{(n-1)2^{n-1}}-\frac {1}{n\cdot 2^{n}}=\frac {2n-(n-1)}{n(n-1)2^{n}}=\frac {n+1}{n(n-1)2^{n}}$

所以$c_{n}=\frac {n-1}{n(n-1)2^{n}}<\frac {n+1}{n(n-1)2^{n}}=\frac {1}{(n-1)2^{n-1}}-\frac {1}{n\cdot 2^{n}}(n\geq 2)$

$c_{1}+c_{2}+\cdots +c_{n}<c_{1}+c_{2}+c_{3}+(\frac {1}{3\cdot 2^{3}}-\frac {1}{4\cdot 2^{4}}+\frac {1}{4\cdot 2^{4}}-\frac {1}{5\cdot 2^{5}}+\cdots +\frac {$

$=\frac {1}{2}+\frac {1}{8}+\frac {1}{24}+\frac {1}{24}-\frac {1}{n\cdot 2^{n}}=\frac {17}{24}-\frac {1}{n\cdot 2^{n}}<\frac {17}{24}$ (n&gt;3)

.$\cdot c_{n}>0\therefore c_{1}<c_{1}+c_{2}<c_{1}+c_{2}+c_{3}=\frac {16}{24}<\frac {17}{24}$

小炼有话说：（1）本题先确定放缩的类型，向裂项相消放缩，从而按“依序同构”的目标进

