```markdown
# CHAPTER 29 MAGNETIC FIELDS

## Example 29.1

**Model** We are asked to find the magnetic field due to a simple current distribution, so this example is a typical problem for which the Biot-Savart law is appropriate. We must find the field contribution from a small element of current and then integrate over the current distribution from θ1 to θ2, as shown in Figure 29.3b.

**Analyse** Let's start by considering a length element dℓ located a distance r from P. The direction of the magnetic field at point P due to the current in this element is out of the page because dℓ × r is out of the page. In fact, because all the current elements dℓ lie in the plane of the page, they all produce a magnetic field directed out of the page at point P. Therefore, the direction of the magnetic field at point P is out of the page and we need only find the magnitude of the field. We place the origin at O and let point P be along the positive y axis, with k being a unit vector pointing out of the page.

From the geometry in Figure 29.3a, we can see that the angle between the vectors dℓ and r is

\[ \theta = \frac{\pi}{2} - \theta \]

radians.

Evaluate the cross product in the Biot-Savart law:

\[ dℓ \times r = |dℓ| \times |r| \sin \left( \frac{\pi}{2} - \theta \right) \hat{k} = |dℓ| \cos \theta \hat{k} \]

Substitute into Equation 29.1:

\[ d\vec{B} = \frac{\mu_0}{4\pi} \frac{I}{r^2} dℓ \cos \theta \hat{k} \]

From the geometry in Figure 29.3a, express r in terms of θ:

\[ r = \frac{a}{\cos \theta} \]

Notice that tan θ = -x/a from the right triangle in Figure 29.3a (the negative sign is necessary because dℓ is located at a negative value of x) and solve for x:

\[ x = -a \tan \theta \]

Find the differential dx:

\[ dx = -a \sec^2 \theta d\theta \]

Substitute Equations (2) and (3) into the magnitude of the field from Equation (1):

\[ d\vec{B} = \frac{\mu_0}{4\pi} a \cos \theta \left( \frac{a}{\cos \theta} \right)^2 \frac{a d\theta}{\cos \theta} = \frac{\mu_0 I a^3 d\theta}{4\pi a^3 \cos^3 \theta} \]

Integrate Equation (4) over all length elements on the wire, where the subtending angles range from θ1 to θ2, as defined in Figure 29.3b:

\[ \vec{B} = -\frac{\mu_0 I}{4\pi a} \int_{\theta_1}^{\theta_2} \cos \theta d\theta = \frac{\mu_0 I}{4\pi a} (\sin \theta_1 - \sin \theta_2) \]

Check the dimensions, noting that the quantity in brackets is dimensionless:

\[ [\text{M} \cdot \text{Q} \cdot \text{T}^{-1}] = [\text{M} \cdot \text{Q} \cdot \text{T}^{-2}] \cdot [\text{L}] = [\text{M} \cdot \text{Q} \cdot \text{T}] \]

(B) Find an expression for the field at a point near a very long current-carrying wire.

**Solution** We can use Equation 29.4 to find the magnetic field of any straight current-carrying wire if we know the geometry and hence the angles θ1 and θ2. If the wire in Figure 29.3b becomes infinitely long, we see that θ1 = π/2 and θ2 = -π/2 for

```