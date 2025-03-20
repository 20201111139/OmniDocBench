Model We are asked to find the magneti field due to a simple current distribution, so this example is a typical problem for which the Biot-Savart law is appropriate. We must find the field contribution from a small element of current and then integrate over the current distribution from$\theta _{1}to\theta _{2},$as shown in Figure 29.3b.

1Uo1.6ZelduexE

Analyse Let's start by considering a length element ds located a distancer from P.The direction of the magnetic field at point P due to the current in this element is out of the page because$d\overline {s}\times \hat {r}$is out of the page. In fact, because all the current elements I ds lie in the plane of the page, they all produce a magnetic field directed out of the page at point P.Therefore, the direction of the magnetic field at point P is out of the page and we need only find the magnitude of the field. We place the origin at O and let point P be along the positive yaxis,with k being a unit vector pointing out of the page.

From the geometry in Figure 29.3a, we can see that the angle between the vectors d s and i is$(\frac {\pi }{2}-\theta )radians.$

Evaluate the cross product in the Biot-Savartlaw:

$d\overline {s}\times \overline {r}=\vert d\overline {s}\times \dot {r}\vert \hat {k}=[dx\sin (\frac {\pi }{2}-\theta )]\dot {k}=(dx\cos \theta )\hat {k}$

Substitute into Equation 29.1:

$d\overrightarrow {B}=(dB)\hat {K}=\frac {\mu _{0}I}{4\pi }\frac {dx\cos \theta }{r^{2}}\hat {K}$ (1)

From the geometry in Figure 29.3a, express r in terms of θ:

$r=\frac {a}{\cos \theta }$ (2)

<!-- \vert d \overrightarrow { s } \vert = d x y P T/ θ a r. d \overrightarrow { s } x x O I  -->
![](https://web-api.textin.com/ocr_image/external/90860aff15d1f7cf.jpg)

a

<!-- y P \theta _ { 1 } \theta _ { 2 } x  -->
![](https://web-api.textin.com/ocr_image/external/73ea867148afab55.jpg)

Figure 29.3

(Example 29.1) (a) A thin,

straight wire carrying a current I(b) The angles θ, and θ,are used for determining the net field.

Notice that tanθ=-x/afrom the right triangle in Figure 29.3a (the negative sign is necessary because ds is located at a negative value of x) and solve for x:

x=-atanθ

Find the differential dx:

$dx=-a\sec ^{2}\theta d\theta =-\frac {ad\theta }{\cos ^{2}\theta }$ (3)

Substitute Equations (2) and (3) into the magnitude of the field from Equation (1):

$dB=-\frac {\mu _{0}I}{4\pi }(\frac {ad\theta }{\cos ^{2}\theta })(\frac {\cos ^{2}\theta }{a^{2}})\cos \theta =-\frac {\mu _{0}I}{4\pi a}\cos \theta d\theta$ (4)

Integrate Equation (4) over all length elements on the wire, where the subtending angles range from$\theta _{1}$to$\theta _{2}$as defined in Figure 29.3b:

$B=-\frac {\mu _{0}I}{4\pi a}\int _{\theta _{1}}^{\theta _{2}}\cos \theta d\theta =\frac {\mu _{0}I}{4\pi a}(\sin \theta _{1}-\sin \theta _{2})$ (29.4)

Check the dimensions, noting that the quantity in brackets is dimensionless:

$[MQ^{-1}T^{-1}]=[MLQ^{-2}][QT^{-1}]/[L]=[MQ^{-1}T^{-1}]$②

(B) Find an expression for the field at a point near a very long current-carrying wire.

## Solution

We can use Equation 29.4 to find the magnetic field of any straight current-carrying wire if we know the geometry and hence the angles$\theta _{1}$and$\theta _{2}.$If the wire in Figure 29.3b becomes infinitely long, we see that$\theta _{1}=\pi /$and$\theta _{2}=-\pi /2$for

