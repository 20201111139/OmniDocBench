```markdown
Y. Sun, P.S.P. Tse/Journal of Computational Physics 230 (2011) 2076-2094

2089

(a) Exact dispersion

(b) Boxscheme

(c) Symplectic method

(d) Yee's method

Fig. 4. The dispersion contours with stepsize \( \Delta x = 0.01 \), \( \Delta t = 0.1 \) for Maxwell's equations (46) from (a) exact dispersion; (b) boxscheme; (c) symplectic method and (d) Yee's method. The constant contour values are \( \omega = 12, 14, 16, 18, 20, 22, 24 \).

\[ \varphi = \tan^{-1} \left( \frac{V_y}{V_x} \right), \quad |V_g| = \sqrt{V_g^x + V_g^y} \]

Substituting into (48) the vectors \( V_g \) and \( V_p \) in polar coordinates (44), and let \( a = k \Delta t \), this yields the propagation angle \( \varphi \) and the propagation speed \( V_p \) for the boxscheme given by

\[ \varphi = \tan^{-1} \left( \frac{\sin(\frac{1}{2} \omega \Delta t) \cos^3(\frac{1}{2} \omega \Delta t) \sin(\frac{1}{2} \omega \Delta t) \cos(\frac{1}{2} \omega \Delta t)}{\cos^3(\frac{1}{2} \omega \Delta t) \sin(\omega \Delta t) \sin(\frac{1}{2} \omega \Delta t)} \right) \]

Taking the Taylor expansion of this expression with respect to \( a = 0 \) yields,

\[ \varphi \approx 0 - \frac{1}{12} \sin(4 \omega \Delta t^2) + O(a^2) \]

Similarly, the Taylor expansion of \( V_p \) at \( a = 0 \) yields,

\[ |V_p| \approx 1 + \left( \frac{1}{16} \cos(4 \omega) - \frac{1}{4} \right) \frac{r^2}{16} + O(a^4) \]
```