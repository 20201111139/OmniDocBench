

![01954280-2f1a-7791-8c98-120d858647b4_0_204_160_1281_1333_0.jpg](images/01954280-2f1a-7791-8c98-120d858647b4_0_204_160_1281_1333_0.jpg)

Fig. 4. The dispersion contours with stepsizes \( {\Delta t} = {0.01},\Delta  = {0.1} \) for Maxwell’s equations (46) from (a) exact dispersion; (b) boxscheme; (c) symplectic method and (d) Yee’s method. The constant contour values are \( \omega  \in  \left\lbrack  {2,4,6,\ldots ,{24}}\right\rbrack \) .

\[
\varphi  = {\tan }^{-1}\left( \frac{{\left( {v}_{g}\right) }_{y}}{{\left( {v}_{g}\right) }_{x}}\right) ,\;\left| {v}_{g}\right|  = \sqrt{{\left( {v}_{g}\right) }_{x}^{2} + {\left( {v}_{g}\right) }_{y}^{2}}. \tag{48}
\]

Substituting into (48) the vectors \( \kappa \) and \( {v}_{\mathrm{g}} \) in polar coordinates (44), and let \( a = \left| \kappa \right| \Delta \) , this yields the propagation angle \( \varphi \) and the propagation speed \( \left| {v}_{g}\right| \) in terms of \( a \) and \( \theta \) .

For example, \( \varphi \) for the boxscheme is given by

\[
\varphi  = {\tan }^{-1}\left( \frac{\sin \left( {\frac{1}{2}\sin \left( \theta \right) a}\right) {\cos }^{3}\left( {\frac{1}{2}\cos \left( \theta \right) a}\right) }{{\cos }^{3}\left( {\frac{1}{2}\sin \left( \theta \right) a}\right) \sin \left( {\frac{1}{2}\cos \left( \theta \right) a}\right) }\right) .
\]

Taking the Taylor expansion of this expression with respect to \( a = 0 \) yields,

\[
\varphi  \approx  \theta  - \frac{1}{12}\sin \left( {4\theta }\right) {a}^{2} + O\left( {a}^{3}\right) . \tag{49}
\]

Similarly, the Taylor expansion of \( \left| {v}_{g}\right| \) at \( a = 0 \) yields,

\[
\left| {v}_{g}\right|  \approx  1 + \left( {\frac{1}{16}\cos \left( {4\theta }\right)  - \frac{{r}^{2}}{4} + \frac{3}{16}}\right) {a}^{2} + O\left( {a}^{4}\right) , \tag{50}
\]
