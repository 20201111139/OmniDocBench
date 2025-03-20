![img-0.jpeg](img-0.jpeg)

Fig. 4. The dispersion contours with stepsizes $\Delta t=0.01, \Delta=0.1$ for Maxwell's equations (46) from (a) exact dispersion; (b) boxscheme; (c) symplectic method and (d) Yee's method. The constant contour values are $\omega \in[2,4,6, \ldots, 24]$.

$$
\varphi=\tan ^{-1}\left(\frac{\left(v_{g}\right)_{y}}{\left(v_{g}\right)_{x}}\right), \quad\left|v_{g}\right|=\sqrt{\left(v_{g}\right)_{x}^{2}+\left(v_{g}\right)_{y}^{2}}
$$

Substituting into (48) the vectors $\kappa$ and $v_{g}$ in polar coordinates (44), and let $a=|\kappa| \Delta$, this yields the propagation angle $\varphi$ and the propagation speed $\left|v_{g}\right|$ in terms of $a$ and $\theta$.

For example, $\varphi$ for the boxscheme is given by

$$
\varphi=\tan ^{-1}\left(\frac{\sin \left(\frac{1}{2} \sin (\theta) a\right) \cos ^{3}\left(\frac{1}{2} \cos (\theta) a\right)}{\cos ^{3}\left(\frac{1}{2} \sin (\theta) a\right) \sin \left(\frac{1}{2} \cos (\theta) a\right)}\right)
$$

Taking the Taylor expansion of this expression with respect to $a=0$ yields,

$$
\varphi \approx \theta-\frac{1}{12} \sin \left(4 \theta\right) a^{2}+O\left(a^{3}\right)
$$

Similarly, the Taylor expansion of $\left|v_{g}\right|$ at $a=0$ yields,

$$
\left|v_{g}\right| \approx 1+\left(\frac{1}{16} \cos (4 \theta)-\frac{r^{2}}{4}+\frac{3}{16}\right) a^{2}+O\left(a^{4}\right)
$$