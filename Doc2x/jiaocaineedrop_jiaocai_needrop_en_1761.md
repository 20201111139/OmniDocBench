例 4: 已知数列 \( \left\{  {a}_{n}\right\} \) 满足 \( {a}_{1} = 2,{a}_{n + 1} = 2{\left( 1 + \frac{1}{n}\right) }^{2}{a}_{n}, n \in  {N}_{ + } \)

( 1 )求证:数列 \( \left\{  \frac{{a}_{n}}{{n}^{2}}\right\} \) 是等比数列,并求出数列 \( \left\{  {a}_{n}\right\} \) 的通项公式

(2)设 \( {c}_{n} = \frac{n}{{a}_{n}} \) ,求证: \( {c}_{1} + {c}_{2} + \cdots  + {c}_{n} < \frac{17}{24} \)

解: (1) \( {a}_{n + 1} = 2{\left( 1 + \frac{1}{n}\right) }^{2}{a}_{n} = 2 \cdot  \frac{{\left( n + 1\right) }^{2}}{{n}^{2}}{a}_{n} \)

\( \therefore \frac{{a}_{n + 1}}{{\left( n + 1\right) }^{2}} = 2 \cdot  \frac{{a}_{n}}{{n}^{2}}\;\therefore \left\{  \frac{{a}_{n}}{{n}^{2}}\right\} \) 是公比为 2 的等比数列

\( \therefore \frac{{a}_{n}}{{n}^{2}} = \left( \frac{{a}_{1}}{{1}^{2}}\right)  \cdot  {2}^{n - 1} = {2}^{n} \)

\( \therefore {a}_{n} = {n}^{2} \cdot  {2}^{n} \)

(2)思路: \( {c}_{n} = \frac{n}{{a}_{n}} = \frac{1}{n \cdot  {2}^{n}} \) ,无法直接求和,所以考虑放缩成为可求和的通项公式(不等号:<),若要放缩为裂项相消的形式,那么需要构造出“顺序同构”的特点。观察分母中有 \( n \) ,故分子分母通乘以(n - 1),再进行放缩调整为裂项相消形式。

解: \( {c}_{n} = \frac{n}{{a}_{n}} = \frac{1}{n \cdot  {2}^{n}} = \frac{n - 1}{n\left( {n - 1}\right) {2}^{n}} \)

而 \( \frac{1}{\left( {n - 1}\right) {2}^{n - 1}} - \frac{1}{n \cdot  {2}^{n}} = \frac{{2n} - \left( {n - 1}\right) }{n\left( {n - 1}\right) {2}^{n}} = \frac{n + 1}{n\left( {n - 1}\right) {2}^{n}} \)

所以 \( {c}_{n} = \frac{n - 1}{n\left( {n - 1}\right) {2}^{n}} < \frac{n + 1}{n\left( {n - 1}\right) {2}^{n}} = \frac{1}{\left( {n - 1}\right) {2}^{n - 1}} - \frac{1}{n \cdot  {2}^{n}}\left( {n \geq  2}\right) \)

\[
{c}_{1} + {c}_{2} + \cdots  + {c}_{n} < {c}_{1} + {c}_{2} + {c}_{3} + \left( {\frac{1}{3 \cdot  {2}^{3}} - \frac{1}{4 \cdot  {2}^{4}} + \frac{1}{4 \cdot  {2}^{4}} - \frac{1}{5 \cdot  {2}^{5}} + \cdots  + \frac{1}{\left( {n - 1}\right) {2}^{n - 1}} - \frac{1}{n \cdot  {2}^{n}}}\right)
\]

\[
= \frac{1}{2} + \frac{1}{8} + \frac{1}{24} + \frac{1}{24} - \frac{1}{n \cdot  {2}^{n}} = \frac{17}{24} - \frac{1}{n \cdot  {2}^{n}} < \frac{17}{24}\;\left( {n > 3}\right)
\]

\[
\because {c}_{n} > 0\;\therefore {c}_{1} < {c}_{1} + {c}_{2} < {c}_{1} + {c}_{2} + {c}_{3} = \frac{16}{24} < \frac{17}{24}
\]

小炼有话说:(1)本题先确定放缩的类型,向裂项相消放缩,从而按“依序同构”的目标进