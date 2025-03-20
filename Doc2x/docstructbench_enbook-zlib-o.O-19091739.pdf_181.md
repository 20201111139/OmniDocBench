Model We are asked to find the magnetic field due to a simple current distribution, so this example is a typical problem for which the Biot-Savart law is appropriate. We must find the field contribution from a small element of current and then integrate over the current distribution from \( {\theta }_{1} \) to \( {\theta }_{2} \) , as shown in Figure 29.3b.

![01954570-0ae4-7850-9883-6d4528d537b3_0_1298_178_343_691_0.jpg](images/01954570-0ae4-7850-9883-6d4528d537b3_0_1298_178_343_691_0.jpg)

Analyse Let’s start by considering a length element \( d\overrightarrow{\mathbf{s}} \) located a distance \( r \) from \( P \) . The direction of the magnetic field at point \( P \) due to the current in this element is out of the page because \( d\overrightarrow{\mathbf{s}} \times  \widehat{\mathbf{r}} \) is out of the page. In fact, because all the current elements \( {Id}\overrightarrow{\mathbf{s}} \) lie in the plane of the page, they all produce a magnetic field directed out of the page at point \( P \) . Therefore, the direction of the magnetic field at point \( P \) is out of the page and we need only find the magnitude of the field. We place the origin at \( O \) and let point \( P \) be along the positive \( y \) axis, with \( \widehat{\mathbf{k}} \) being a unit vector pointing out of the page.

From the geometry in Figure 29.3a, we can see that the angle between the vectors \( d\overrightarrow{\mathbf{s}} \) and \( \overrightarrow{\mathbf{r}} \) is \( \left( {\frac{\pi }{2} - \theta }\right) \) radians.

Evaluate the cross product in the Biot-Savart law:

\[
d\overrightarrow{\mathbf{s}} \times  \widehat{\mathbf{r}} = \left| {d\overrightarrow{\mathbf{s}} \times  \widehat{\mathbf{r}}}\right| \widehat{\mathbf{k}} = \left\lbrack  {{dx}\sin \left( {\frac{\pi }{2} - \theta }\right) }\right\rbrack  \widehat{\mathbf{k}} = \left( {{dx}\cos \theta }\right) \widehat{\mathbf{k}}
\]

-b

Substitute into Equation 29.1: Figure 29.3

\[
d\overrightarrow{\mathbf{B}} = \left( {dB}\right) \widehat{\mathbf{k}} = \frac{{\mu }_{0}I}{4\pi }\frac{{dx}\cos \theta }{{r}^{2}}\widehat{\mathbf{k}}
\]

(Example 29.1) (a) A thin,(1)straight wire carrying a current \( I \) (b) The angles \( {\theta }_{1} \) and

From the geometry in Figure 29.3a, express \( r \) in terms of \( \theta \) : \( {\theta }_{2} \) are used for determining the net field.

\[
r = \frac{a}{\cos \theta } \tag{2}
\]

Notice that \( \tan \theta  =  - x/a \) from the right triangle in Figure 29.3a (the negative sign is necessary because \( d\overrightarrow{\mathbf{s}} \) is located at a negative value of \( x \) ) and solve for \( x \) :

\[
x =  - a\tan \theta
\]

Find the differential \( {dx} \) :

\[
{dx} =  - a{\sec }^{2}{\theta d\theta } =  - \frac{ad\theta }{{\cos }^{2}\theta } \tag{3}
\]

Substitute Equations (2) and (3) into the magnitude of the field from Equation (1):

\[
{dB} =  - \frac{{\mu }_{0}I}{4\pi }\left( \frac{ad\theta }{{\cos }^{2}\theta }\right) \left( \frac{{\cos }^{2}\theta }{{a}^{2}}\right) \cos \theta  =  - \frac{{\mu }_{0}I}{4\pi a}\cos {\theta d\theta } \tag{4}
\]

Integrate Equation (4) over all length elements on the wire, where the subtending angles range from \( {\theta }_{1} \) to \( {\theta }_{2} \) as defined in Figure 29.3b:

\[
B =  - \frac{{\mu }_{0}I}{4\pi a}{\int }_{{\theta }_{1}}^{{\theta }_{2}}\cos {\theta d\theta } = \frac{{\mu }_{0}I}{4\pi a}\left( {\sin {\theta }_{1} - \sin {\theta }_{2}}\right)  \tag{29.4}
\]

Check the dimensions, noting that the quantity in brackets is dimensionless:

\[
\left\lbrack  {{\mathrm{{MQ}}}^{-1}{\mathrm{\;T}}^{-1}}\right\rbrack   = \left\lbrack  {\mathrm{{MLQ}}}^{-2}\right\rbrack  \left\lbrack  {\mathrm{{QT}}}^{-1}\right\rbrack  /\left\lbrack  \mathrm{L}\right\rbrack   = \left\lbrack  {{\mathrm{{MQ}}}^{-1}{\mathrm{\;T}}^{-1}}\right\rbrack   \tag{c}
\]

(B) Find an expression for the field at a point near a very long current-carrying wire.

## Solution

We can use Equation 29.4 to find the magnetic field of any straight current-carrying wire if we know the geometry and hence the angles \( {\theta }_{1} \) and \( {\theta }_{2} \) . If the wire in Figure 29.3b becomes infinitely long, we see that \( {\theta }_{1} = \pi /2 \) and \( {\theta }_{2} =  - \pi /2 \) for