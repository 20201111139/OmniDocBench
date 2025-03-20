![](images/fb8842802f3fe75d27d674d76a76a47d9c01422933ff88a2a2a5f952ff875c9f.jpg)  
Fig. 4. The dispersion contours with stepsizes  $\Delta t=0.01$   $\Delta=0.1$  for Maxwel's equations (46) from (a) exact dispersion; (b) boxscheme; (c) symplectic method and (d) Yee's method. The constant contour values are  $\omega\in[2,4,6,\ldots,24]$  

$$
\varphi=\mathsf{t a n}^{-1}\left(\frac{(\upsilon_{g})_{y}}{(\upsilon_{g})_{x}}\right),\quad|\upsilon_{g}|=\sqrt{(\upsilon_{g})_{x}^{2}+(\upsilon_{g})_{y}^{2}}.
$$  

Substituting into (48) the vectors  $\kappa$  and  $\nu_{g}$  in polar coordinates (44), and let  $a=|\kappa|\Delta,$   this yields the propagation angle  $\varphi$  and the propagation speed  $|\nu_{\mathrm{g}}|$  in terms of  $a$  and  $\theta$  

For example,  $\varphi$  for the boxscheme is given by  

$$
\begin{array}{r}{\varphi=\tan^{-1}\left(\frac{\sin\big(\frac{1}{2}\sin(\theta)a\big)\cos^{3}\big(\frac{1}{2}\cos(\theta)a\big)}{\cos^{3}\big(\frac{1}{2}\sin(\theta)a\big)\sin\big(\frac{1}{2}\cos(\theta)a\big)}\right).}\end{array}
$$  

Taking the Taylor expansion of this expression with respect to  $a=0$  yields,  

$$
\varphi\approx\theta-{\frac{1}{12}}\sin(4\theta)a^{2}+O(a^{3}).
$$  

Similarly, the Taylor expansion of  $|\nu_{\mathrm{g}}|$  at  $a=0$  yields,  

$$
|\nu_{g}|\approx1+\bigg(\frac{1}{16}\cos(4\theta)-\frac{r^{2}}{4}+\frac{3}{16}\bigg)a^{2}+O(a^{4}),
$$  