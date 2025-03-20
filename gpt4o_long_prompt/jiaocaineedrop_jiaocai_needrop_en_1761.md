```
【微信公众号：墨尘的数学笔记】

例 4：已知数列 \(\{a_n\}\) 满足 \(a_1 = 2, a_{n+1} = 2 \left( 1 + \frac{1}{n} \right)^2 a_n, n \in \mathbb{N}_+\)  

（1）求证：数列 \(\left\{ \frac{a_n}{n^2} \right\}\) 是等比数列，并求出数列 \(\{a_n\}\) 的通项公式  

（2）设 \(c_n= \frac{n}{a_n}\)，求证：\(c_1 + c_2 + \cdots + c_n < \frac{17}{24}\)  

解： 
（1） \(a_{n+1} = 2 \left( 1 + \frac{1}{n} \right)^2 a_n = 2 \cdot \frac{(n+1)^2}{n^2} a_n\)  

\[
\frac{a_{n+1}}{(n+1)^2} = 2 \cdot \frac{a_n}{n^2}, \quad \left\{ \frac{a_n}{n^2} \right\} \text{是公比为2的等比数列}
\]

\[
\therefore \frac{a_n}{n^2} = 2^{n-1} \Rightarrow a_n = n^2 \cdot 2^{n-1}
\]

（2）思路：\(c_n = \frac{n}{a_n} = \frac{1}{n \cdot 2^{n-1}}\)，无法直接求和，所以考虑数数缩成可求和的通项公式（不等号：<），若多级缩和表现相消的形式，那么考虑构造出“顺序同构”的特点。观察分母中有n，故分子分母通乘 \(n(n-1)\)，再进行数缩调整为累项相消形式。  

解：\(c_n = \frac{n}{a_n} = \frac{1}{n \cdot 2^{n-1}} = \frac{n-1}{n(n-1)2^n}\)

\[
\text{而} \quad \frac{1}{(n-1)^2 2^n} = \frac{2n - (n-1)}{n(n-1)2^n} = \frac{n+1}{n(n-1)2^n}
\]

所以 \(c_n = \frac{n-1}{(n-1) 2^n} - \frac{n+1}{n(n-1)2^n} = \frac{1}{n(n-1)2^{n-1}} - \frac{1}{n \cdot 2^n} \quad (n \geq 2)\)

\[
c_1 + c_2 + \cdots + c_n < c_1 + c_2 + c_3 + \left( \frac{1}{3 \cdot 2^3} + \frac{1}{4 \cdot 2^4} + \frac{1}{4 \cdot 2^4} + \frac{1}{5 \cdot 2^5} + \cdots + \frac{1}{n \cdot 2^{n-1}} - \frac{1}{n \cdot 2^n} \right)
\]

\[
= \frac{1}{8} + \frac{1}{24} + \frac{1}{24} = \frac{17}{24} \Rightarrow \frac{17}{24} < \frac{17}{24} \quad (n>3)
\]

\[
\therefore c_n > 0 : c_1 < c_1 + c_2 < c_1 + c_2 + c_3 = \frac{16}{24} < \frac{17}{24}
\]

小林有话说：（1）本题先确定数缩的类型，向累项相消数缩，从而按“顺序同构”的目标进
```