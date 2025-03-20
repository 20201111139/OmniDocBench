```markdown
## Example 29.1 cont.

### Model

We are asked to find the magnetic field due to a simple current distribution, so this example is a typical problem for which the Biot–Savart law is appropriate. We must find the field contribution from a small element of current and then integrate over the current distribution from \( \theta_1 \) to \( \theta_2 \), as shown in Figure 29.3b.

### Analyse

Let's start by considering a length element \( ds \) located a distance \( r \) from \( P \). The direction of the magnetic field at point \( P \) due to the current in this element is out of the page because \( ds \times \hat{k} \) is out of the page. In fact, because all the current elements \( Ids \) lie in the plane of the page, they all produce a magnetic field directed out of the page at point \( P \). Therefore, the direction of the magnetic field at point \( P \) is out of the page and we need only find the magnitude of the field. We place the origin at \( O \) and let point \( P \) be along the positive \( y \) axis, with \( \hat{k} \) being a unit vector pointing out of the page.

From the geometry in Figure 29.3a, we can see that the angle between the vectors \( ds \) and \( \vec{r} \) is \( \left( \frac{\pi}{2} - \theta \right) \) radians.

Evaluate the cross product in the Biot–Savart law:

\[ ds \times \hat{r} = |ds \times \hat{k}| \hat{k} = \left[ dx \sin \left( \frac{\pi}{2} - \theta \right) \right] \hat{k} = (dx \cos \theta) \hat{k} \]

Substitute into Equation 29.1:

\[
d\vec{B} = (d\vec{B}) \hat{k} = \frac{\mu_0 I}{4 \pi} \frac{dx \cos \theta}{r^2} \hat{k} \tag{1}
\]

From the geometry in Figure 29.3a, express \( r \) in terms of \( \theta \):

\[ 
r = \frac{a}{\cos \theta} \tag{2} 
\]

Notice that \( \tan \theta = -x/a \) from the right triangle in Figure 29.3a (the negative sign is necessary because \( ds \) is located at a negative value of \( x \)) and solve for \( x \):

\[ 
x = -a \tan \theta 
\]

Find the differential \( dx \):

\[ 
dx = -a \sec^2 \theta \, d\theta = -\frac{a \, d\theta}{\cos^2 \theta} \tag{3} 
\]

Substitute Equations (2) and (3) into the magnitude of the field from Equation (1):

\[
dB = -\frac{\mu_0 I}{4 \pi} \left( \frac{a \, d\theta}{a^2} \right) \left( \cos^3 \theta \right) = -\frac{\mu_0 I}{4 \pi a} \cos \theta \, d\theta \tag{4}
\]

Integrate Equation (4) over all length elements on the wire, where the subtending angles range from \( \theta_1 \) to \( \theta_2 \) as defined in Figure 29.3b:

\[ 
B = -\frac{\mu_0 I}{4 \pi a} \int_{\theta_1}^{\theta_2} \cos \theta \, d\theta = \frac{\mu_0 I}{4 \pi a} (\sin \theta_1 - \sin \theta_2) \tag{29.4} 
\]

Check the dimensions, noting that the quantity in brackets is dimensionless:

\[ 
[MQ^{-1}T] = [MLQ^{-2}IQ^{T-1}][L] = [MQ^{-1}T-1] 
\]

(B) Find an expression for the field at a point near a very long current-carrying wire.

### Solution

We can use Equation 29.4 to find the magnetic field of any straight current-carrying wire if we know the geometry and hence the angles \( \theta_1 \) and \( \theta_2 \). If the wire in Figure 29.3b becomes infinitely long, we see that \( \theta_1 = \pi/2 \) and \( \theta_2 = -\pi/2 \) for
```
