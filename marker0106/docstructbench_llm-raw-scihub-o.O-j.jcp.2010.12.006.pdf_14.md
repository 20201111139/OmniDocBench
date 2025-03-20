![](_page_0_Figure_1.jpeg)

Fig. 4. The dispersion contours with stepsizes Δt = 0.01, Δ = 0.1 for Maxwell's equations (46) from (a) exact dispersion: (b) boxscheme; (c) symplectic method and (d) Yee's method. The constant contour values are @ E [2,4,6, ... , 24].

$$\varphi=\tan^{-1}\left(\frac{\left(\nu_{L}\right)_{y}}{\left(\nu_{L}\right)_{x}}\right),\quad\left|\nu_{L}\right|=\sqrt{\left(\nu_{L}\right)_{x}^{2}+\left(\nu_{L}\right)_{y}^{2}},\tag{48}$$

Substituting into (48) the vectors κ and ½ in polar coordinates (44), and let α = |κ|Δ, this yields the propagation angle φ and the propagation speed |vg| in terms of a and 0.

For example, o for the boxscheme is given by

$\varphi=\tan^{-1}\left(\frac{\sin\left(\frac{1}{2}\sin(\theta)a\right)\cos^{3}\left(\frac{1}{2}\cos(\theta)a\right)}{\cos^{3}\left(\frac{1}{2}\sin(\theta)a\right)\sin\left(\frac{1}{2}\cos(\theta)a\right)}\right)$.  
  

Taking the Taylor expansion of this expression with respect to a = 0 yields,

$$\varphi\approx\theta-\frac{1}{12}\sin(4\theta)a^{2}+O(a^{3}).\tag{49}$$

Similarly, the Taylor expansion of |vg at a = 0 yields,

$$|\alpha_{2}|\approx1+\left(\frac{1}{16}\cos(4\theta)-\frac{r^{2}}{4}+\frac{3}{16}\right)a^{2}+O(a^{4}),\tag{50}$$

