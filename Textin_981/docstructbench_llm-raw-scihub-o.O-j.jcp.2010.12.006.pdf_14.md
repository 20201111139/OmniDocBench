<!-- 30 Exact dispersion 20 10 立 0 -10 -20 -30 -20 -10 0 10 20 30 kx  -->
![](https://web-api.textin.com/ocr_image/external/de3aea30f480b38b.jpg)

(a)

<!-- 30 Boxscheme 20 10 立 0 -10 -20 -30 -20 -10 0 10 20 30 kx  -->
![](https://web-api.textin.com/ocr_image/external/aa3888c89cbfb5fd.jpg)

(b)

<!-- 30 Symplectic method 20 10 立 0 -10 -20 -30 -20 -10 0 10 20 30 kx  -->
![](https://web-api.textin.com/ocr_image/external/b03575c9b7c801e7.jpg)

(c)

<!-- 30 Yee's method 20 10 立 0 -10 -20 -30 -20 -10 0 10 20 30 kx  -->
![](https://web-api.textin.com/ocr_image/external/9c094fc2d7d5169c.jpg)

(d)

Fig. 4. The dispersion contours with stepsizesΔt=0.01,Δ=0. for Maxwell's equations (46) from (a) exact dispersion; (b) boxscheme; (c) symplectic method and (d)Yee's method. The constant contour values areω∈[2,4,6,⋯,24]

$\varphi =\tan ^{-1}(\frac {v_{g})_{y}}{(v_{g})_{x}}),$ $\vert v_{g}\vert =\sqrt {(v_{g})_{X}^{2}+(v_{g})_{y}^{2}}.$ (48)

Substituting into (48) the vectors k and$v_{g}$in polar coordinates (44), and leta=|k|Δ,this yields the propagation angle φ and the propagation speed$\vert v_{}\vert$in terms of a and 0.

For example, φ for the boxscheme is given by

$\varphi =\tan ^{-1}(\frac {\sin (\frac {1}{2}\sin (\theta )a)\cos ^{3}(\frac {1}{2}\cos (\theta )a)}{\cos ^{3}(\frac {1}{2}\sin (\theta )a)\sin (\frac {1}{2}\cos (\theta )a)})$

Taking the Taylor expansion of this expression with respect toa=0yields,

$\varphi \approx \theta -\frac {1}{12}\sin (4\theta )a^{2}+O(a^{3}).$ (49)

Similarly,the Taylor expansion of$\vert v_{g}\vert$ata=0yields,

$\vert v_{g}\vert \approx 1+(\frac {1}{16}\cos (4\theta )-\frac {r^{2}}{4}+\frac {3}{16})a^{2}+O(a^{4}),$ (50)

