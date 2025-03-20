```markdown
808

2.9 Elimination of secondary structures

Based on the superposition principle, vortices and vortical shear layers from blades passing the measurement window are identified and removed from the image such that the vortex of interest remains almost unaffected. Thereafter, its parameters can be identified without being biased by disturbing structures. Currently, this is performed manually in the measurements and only for the in-plane velocities. The disturbing vortex is identified by a best fit to a Vatistas swirl model and its contribution is then subtracted from the entire velocity field. This can also be done iteratively until no fragments of the disturbing structure could be remained. In general, both more structures as well as not implemented yet.

An example is given in Fig. 10a where two vortices of opposite sense of rotation are close to each other, and both are affecting the vortex center. The other was monotonely flow field to the centre of the disturbing structure, using the scalar field of λ2-convolution. After elimination of this remaining vortex using a best fit of Vatistas swirl model the parameters of interest are clearly unaffected by other structures (b) and its parameters can be identified. To do even more, the shear layer at the lower left of the image could be eliminated by the same procedure.

2.10 Identification of vortex parameters

The identification of the swirl and the axial velocity profiles, the core radius and the circulation is often hindered by other flow structures in close proximity of the vortex of interest. These are in layers with vorticity and additional vortices shed by other blades just passing the measurement window, especially where BVI takes place.

Using a best fit of a Vatistas vortex swirl model [26], the parameters describing the vortex are identified. This model is written in terms of the maximum swirl velocity Vmax, the core radius r0, the shape parameter n that defines the shape x of an exponential function defining the parameter x to the inclusion of the vortex age θ, the model at the core radius r0 the maximum swirl velocity Vmax describes the distribution of vorticity (and therefore with the distribution of λ2 and Q), and the radial distance from the vortex centre. The development of vortex circulation, and thus the fraction of total circulation at the core radius, is connected to the swirl velocity profile as well. All relations for the Vatistas vortex are given [27]. Note that all variables are made non-dimensional, i.e., the velocities are divided by Q, circulation and kinematic viscosity by Q, vorticity by Q, coordinates by the core radius r0, the core radius by r, and the flow field operators by Q^2.

\[ V_s = V_{s0} \left(1 + \frac{r^2}{r_0^2}\right)^{1/n} \]

\[ V_{s0} = V_{smax} 2^{1/n} = \frac{\Gamma_v}{2 \pi r_0} \]

Alternatively, the Lamb-Oseen [10, 18] or Newman [17] vortex can be fitted to the data. These are also written in terms of Vmax and rcut, but the radial distribution function is different and a factor of an exponential function defines the shape x. Expanding the Vatistas model using a least squares error method. The best fit is performed at a radial extension of 2-3 core radii.

\[ V_s = V_{s0} \frac{1 - e^{-r^2}}{r} \]

\[ V_{s0} = \frac{V_{smax}}{1 - e^{-r_c^2}} \frac{\Gamma_v}{2 \pi r_c} \]

Vatistas model is used here, since with the shape parameter n a wide range of swirl shapes can be defined, covering the Scully vortex (n=1), the Lamb-Oseen vortex (n≈2), or the Rankine vortex (n=∞). When the data are cleaned from spurious vectors (n≈2), mean values of the flow subtracted and rotated into the vortex axis system, the distribution of swirl velocities of all vectors is fitted, the distribution of swirl velocities of all vectors is fitted with the Vatistas model using a least squares error method. The best fit is performed at a radical extension of 2-3 core radii.
```