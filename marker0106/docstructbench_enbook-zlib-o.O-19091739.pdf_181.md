Model We are asked to find the magnetic field due to a simple current distribution, so this example is a typical problem for which the Biot-Savart law is appropriate. We must find the field contribution from a small element of current and then integrate over the current distribution from 0, to 0,, as shown in Figure 29.3b.

Analyse Let's start by considering a length element d s located a distance r from P. The direction of the magnetic field at point P due to the current in this element is out of the page because d 3 × î is out of the page. In fact, because all the current elements I d & lie in the plane of the page, they all produce a magnetic field directed out of the page at point P. Therefore, the direction of the magnetic field at point P is out of the page and we need only find the magnitude of the field. We place the origin at O and let point P be along the positive y axis, with k being a unit vector pointing out of the page.

From the geometry in Figure 29.3a, we can see that the angle between the vectors d $ and T

71 is radians.

Evaluate the cross product in the Biot-Savart law:

$d\,\hat{\bf s}\times\hat{\bf r}=|d\,\hat{\bf s}\times\hat{\bf r}|\hat{\bf k}=\left[\,dx\,\sin(\frac{\pi}{2}-\theta)\right]\hat{\bf k}=(dx\,\cos\theta)\hat{\bf k}$

Substitute into Equation 29.1:

$d\mathbf{B}=(dB)\mathbf{k}=\frac{\mu_{0}I\ dx\cos\theta}{4\pi}\mathbf{k}$

From the geometry in Figure 29.3a, express r in terms of 0:

$$r={\frac{a}{\cos\theta}}$$

Notice that tan 0 = - x/a from the right triangle in Figure 29.3a (the negative sign is necessary because d3 is located at a negative value of x) and solve for x:

$x\:=\:-a\tan\theta$  
  
. 

Find the differential dx:

$$dx=-a\sec^{2}\theta\,d\theta=-\frac{a\,d\theta}{\cos^{2}\theta}\tag{3}$$

(1)

(2)

Substitute Equations (2) and (3) into the magnitude of the field from Equation (1):

$$dB=-\frac{\mu_{0}l}{4\pi}\Bigg{(}\frac{a\,d\theta}{\cos^{2}\theta}\Bigg{)}\Bigg{(}\frac{\cos^{2}\theta}{a^{2}}\Bigg{)}\cos\theta=-\frac{\mu_{0}l}{4\pi a}\cos\theta\,d\theta\tag{4}$$

Integrate Equation (4) over all length elements on the wire, where the subtending angles range from 0, to 0, as defined in Figure 29.3b:

$$B=-\frac{\mu_{0}l}{4\pi a}\int_{\theta_{1}}^{\theta_{2}}\cos\theta d\theta=\frac{\mu_{0}l}{4\pi a}(\sin\theta_{1}-\sin\theta_{2})\tag{29.4}$$

Check the dimensions, noting that the quantity in brackets is dimensi

[MQ${}^{-1}$T${}^{-1}$] = [MLQ${}^{-2}$][QT${}^{-1}$]/[L] = [MQ${}^{-1}$T${}^{-1}$] (5)

(B) Find an expression for the field at a point near a very long current-carrying wire.

## Solution

We can use Equation 29.4 to find the magnetic field of any straight current-carrying wire if we know the geometry and hence the angles 0, and 0, If the wire in Figure 29.3b becomes infinitely long, we see that 0, = m/2 and 0, = - m/2 for

![](_page_0_Figure_25.jpeg)

![](_page_0_Figure_26.jpeg)

current I (b) The angles 0, and θ, are used for determining the net field.

![](_page_0_Figure_28.jpeg)

xample 29.1 co

