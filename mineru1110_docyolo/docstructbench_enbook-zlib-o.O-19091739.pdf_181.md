Model We are asked to find the magnetic field due to a simple current distribution, so this example is a typical problem for which the Biot-Savart law is appropriate. We must find the field contribution from a small element of current and then integrate over the current distribution from  $\theta_{\mathrm{{1}}}$  to  $\theta_{2},$  as shown in Figure 29.3b.  

AnalyseLet's start by considering a length element  $d\vec{\bf s}$  located a distance  $r$  from  $P_{c}$  The direction of the magnetic field at point  $P$  due to the current in this element is out of the page because  $d\vec{\bf s}\times\hat{\bf r}$  is out of the page. In fact, because all the current elements  $I d\,{\vec{\mathbf{s}}}$  lie in the plane of the page, they all produce a magnetic field directed out of the page at point  $P_{\cdot}$  Therefore, the direction of the magnetic field at point  $P$  is out of the page and we need only find the magnitude of the field. We place the origin at  $O$  and let point  $P$  be along the positive  $y$  axis, with  $\bar{\mathbf{k}}$  being a unit vector pointing out of the page.  

From the geometry in Figure 29.3a, we can see that the angle between the vectors  $d\,\vec{\mathbf{s}}$  andr is  $\left({\frac{\pi}{2}}\,-\theta\right)$  radians.  

Evaluate the cross product in the Biot-Savart law:  

$$
d\,{\vec{\mathbf{s}}}\times{\hat{\mathbf{r}}}=\left|d{\vec{\mathbf{s}}}\times{\hat{\mathbf{r}}}\right|{\hat{\mathbf{k}}}={\bigg[}d x\,\sin\!\left({\frac{\pi}{2}}-\theta\right){\bigg]}{\hat{\mathbf{k}}}=(d x\cos\theta){\hat{\mathbf{k}}}
$$  

Substitute into Equation 29.1:  

$$
d{\vec{\mathbf{B}}}=(d B){\hat{\mathbf{k}}}={\frac{\mu_{0}I}{4\pi}}{\frac{d x\cos\theta}{r^{2}}}{\hat{\mathbf{k}}}
$$  

From the geometry in Figure 29.3a, express  $r$  in terms of  $\theta$  

![](images/19f06a9d4bf86dbaaffed92bfdd857d6aef407f75408634a348f4e1e42767acd.jpg)  
Figure 29.3 (Example29.1) (a)Athin, straight wire carrying a current  $I$  (b) The angles  $\theta_{_1}$  and  $\theta_{2}$  are used for determining the net field.  

$$
r={\frac{a}{\cos\theta}}
$$  

Notice that tan  $\theta=-x/a$  from the right triangle inigure29.3a(thenegative sign is necesarybecaue  $d\vec{\mathbf{s}}$  is located at a negative value of  $\boldsymbol{\mathscr{x}}$  ) and solve for  $_{\mathscr{x}}$  

$$
x=-a\tan\theta
$$  

Find the differential  $d x$  

$$
d x=-a\sec^{2}\theta\,d\theta=-{\frac{a\,d\theta}{\cos^{2}\theta}}
$$  

Substitute Equations (2) and (3) into the magnitude of the field from Equation (1):  

$$
d B=-{\frac{\mu_{0}I}{4\pi}}\bigg({\frac{a\,d\theta}{\cos^{2}\theta}}\bigg)\bigg({\frac{\cos^{2}\theta}{a^{2}}}\bigg)\cos\theta=-{\frac{\mu_{0}I}{4\pi a}}\cos\theta\,d\theta
$$  

Integrate Equation (4) over allength elements on the wire, where the subtending angles range from  $\theta_{_1}$   $\theta_{2}$  as defined in Figure29.3b:  

$$
B=-\frac{\mu_{0}I}{4\pi a}{\int}_{\theta_{1}}^{\theta_{2}}\cos{\theta}d\theta=\frac{\mu_{0}I}{4\pi a}(\sin{\theta_{1}}-\sin{\theta_{2}})
$$  

Check the dimensions, noting that the quantity in brackets is dimensionless:  

$$
[\mathrm{MQ^{-1}T^{-1}}]=[\mathrm{MLQ^{-2}}][\mathrm{QT^{-1}}]/[\mathrm{L}]=[\mathrm{MQ^{-1}T^{-1}}]\circledast
$$  

(B) Find an expression for the field at a point near a very long current-carrying wire.  

# Solution  

We can use Equation 29.4 to find the magnetic field of any straight current-carrying wire if we know the geometry and hence the angles  $\theta_{_1}$  and  $\theta_{2}$   If the wire in Figure 29.3b becomes infinitely long, we see that  $\theta_{\mathrm{{1}}}=\pi/2$  and  $\theta_{{}_{2}}=-\pi/2$  for  