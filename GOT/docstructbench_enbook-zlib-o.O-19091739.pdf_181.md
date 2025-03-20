Model We are asked to find the magnetic field due to a simple current distribution, so this example is a typical problem for which the Biot-Savart law is appropriate. We must find the field contribution from a small element of current and then integrate over the current distribution from \(\theta_{1}\) to \(\theta_{2}\), as shown in Figure 29.3b.
Analyses Let's start by considering a length element \(\boldsymbol{d} \boldsymbol{s}\) located a distance \(r\) from \(P\). The direction of the magnetic field at point \(P\) due to the current in this element is out of the page because \(\boldsymbol{d} \boldsymbol{s} \times \boldsymbol{r}\) is out of the page. In fact, because all the current elements \(l \boldsymbol{d} \boldsymbol{s}\) lie in the plane of the page, they all produce a magnetic field directed out of the page at point \(P\) Therefore, the direction of the magnetic field at point \(P\) is out of the page and we need only find the magnitude of the field. We place the origin at \(\mathrm{O}\) and let point \(P\) be along the positive \(y\) axis, with \(\boldsymbol{k}\) being a unit vector pointing out of the page.
From the geometry in Figure 29.3a, we can see that the angle between the vectors \(\boldsymbol{d} \boldsymbol{s}\) and \(\tilde{\mathbf{r}}\) is \(\left(\frac{\pi}{2}-\theta\right)\) radians.
Evaluate the cross product in the Biot-Savart law:
\[
d \tilde{\mathbf{s}} \times \hat{\mathbf{r}}=|d \tilde{\mathbf{s}} \times \hat{\mathbf{r}}| \hat{\mathbf{k}}=|d x \sin \left(\frac{\pi}{2}-\theta\right)| \hat{\mathbf{k}}=(d x \cos \theta) \hat{\mathbf{k}}
\]
Substitute into Equation 29.1:
\[
d \tilde{\mathbf{B}}=(d B) \hat{\mathbf{k}}=\frac{\mu_{0} I}{4 \pi} \frac{d x \cos \theta}{r^{2}} \hat{\mathbf{k}}
\]
From the geometry in Figure 29.3a, express \(r\) in terms of \(\theta\) :
\[
r=\frac{a}{\cos \theta}
\]
Notice that \(\tan \theta=-x / a\) from the right triangle in Figure 29.3a (the negative sign is necessary because \(d \tilde{\mathbf{s}}\) is located at a negative value of \(x\) ) and solve for \(x\) :
\[
x=-a \tan \theta
\]
Find the differential \(d x\) :
\[
d x=-a \sec ^{2} \theta d \theta=-\frac{a d \theta}{\cos ^{2} \theta}
\]
Substitute Equations (2) and (3) into the magnitude of the field from Equation (1):
\[
d B=-\frac{\mu_{0} I}{4 \pi} \int_{\theta_{1}}^{a} \cos \theta d \theta=\frac{\mu_{0} I}{4 \pi a} \left(\sin \theta_{1}-\sin \theta_{2}\right)
\]
Integrate Equation (4) over all length elements on the wire, where the subtending angles range from \(\theta_{1}\) to \(\theta_{2}\) as defined in Figure 29.3b:
\[
B=-\frac{\mu_{0} I}{4 \pi a} \int_{\theta_{1}}^{a} \cos \theta d \theta =\frac{\mu_{0} I}{4 \pi a} \left(\sin \theta _{1}-\sin \theta_{2}\right)
\]
Check the dimensions, noting that the quantity in brackets is dimensionless:
\[
\left[\mathrm{MQ}^{-1} \mathrm{~T}^{-1}\right]=\left[\mathrm{MLQ}^{-2}\right]\left[\mathrm{QT}^{-1}\right] /\left[\mathrm{L}\right]=\left[\mathrm{MQ}^{-1} \mathrm{~T}^{-1} \right] \otimes
\]
(B) Find an expression for the field at a point near a very long current-carrying wire.
\section*{Solution}
We can use Equation 29.4 to find the magnetic field of any straight current-carrying wire if we know the geometry and hence the angles \(\theta_{1}\) and \(\theta_{2}\). If the wire in Figure 29.3b becomes infinitely long, we see that \(\theta_{1}=\pi / 2\) and \(\theta_{2}=-\pi / 2\) for