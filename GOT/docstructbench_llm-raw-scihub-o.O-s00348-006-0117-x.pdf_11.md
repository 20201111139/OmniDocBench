\subsection*{2.9 Elimination of secondary structures}
Based on the superposition principle, vortices and vortical shear layers from blades passing the measurement window are identified and numerically removed from the image such that the vortex of interest remains almost unaffected. Thereafter, its parameters can be identified without being biased by disturbing structures. Currently, this is performed manually in the measurement plane, and only for the in-plane velocities. The disturbing vortex is identified by a best fit to a Vatistas swirl model and its contribution is then subtracted from the entire velocity field. This can also be done iteratively until no fragments of the disturbing structure remain. In general, both (or more) structures could be identified simultaneously, but this is complicated by different orientation of their vortex axis with respect to the measurement plane, and the second one is shown in Fig. 10a
An example is given in Fig. 10a where two vortices of opposite sense of rotation are close to each other, and both are affecting the other vortex flow field adversely. In (a) the vortex centre was manually set to the centre of the disturbing structure, using the scalar field of \(\lambda_{2}\)-convolution. After elimination of this structure using a best fit to Vatistas swirl model the remaining vortex is clearly unaffected by other structures (b) and its parameters can be identified. To do even more, the shear layer at the lower left of the image could be eliminated by the same procedure.
\subsection*{2.10 Identification of vortex parameters}
The identification of the swirl and the axial velocity profiles, the core radius and the circulation is often hindered by other flow structures in close proximity of the vortex of interest. These are shear layers with vorticity and additional vortices shed by other blades just passing the measurement window, especially where BVI takes a \(10 \mathrm{~cm}\) depth.
Using a best fit of a Vatistas vortex swirl model , the parameters describing the vortex are identified. This model is written in terms of the maximum swirl velocity \(V_{x, \max }\) at the core radius \(r_{c}\), the shape parameter \(n\) that describes the distribution of vorticity (and therewith the distribution of \(\lambda_{2}\) and \(Q\) ), and the radial distance from the vortex centre. The development of vortex circulation, and thus the fraction of total circulation at the core radius, is connected to the swirl velocity profile as well. All relations for the Vatistas vortex are given . Note that all variables are made non-dimensional, i.e., the velocities are divided by \(\Omega R\), circulation and kinematic viscosity by \(\Omega\) \(R^{2}\), vorticity of \(\Omega\), coordinates by the core radius \(r_{f}\), the core radius by \(R\), and the flow field operators by \(\Omega^{2}\).
\[
\begin{array}{l}
V_{s}=V_{s 0} \frac{r}{\left(1+r^{2 n}\right)^{1 / n}} \\
V_{s 0}=V_{s, \max } 2^{1 / n}=\frac{\Gamma_{v}}{2 \pi r_{c}}
\end{array}
\]

(a) original data

(b) counter-rotating vortex removed
Fig. 10 Elimination of disturbing structures. BL, pos. 47 of Fig. 1 simple average
Alternatively, the Lamb-Oseen [10,  or Newman  vortex can be fitted to the data. These are also written in terms of \(V_{x, \max }\) and \(r_{c}\), but the radial distribution function is different and a factor \(\alpha\) of an exponential function defines the shape. Expanding the parameter \(\alpha\) to the inclusion of the vortex age \(\psi_{c}\) the Hamel-Oseen  model can be used as well.
\[
\begin{array}{l}
V_{s}=V_{s 0}=\frac{1-e^{-\alpha \gamma^{2}}}{r} \\
V_{s 0}=\frac{V_{s, \max }}{1-e^{-\alpha}}=\frac{\Gamma_{v}}{2 \pi r_{c}}
\end{array} \quad
\]
Vatistas model is used here, since with the shape parameter \(n\) a wide range of swirl shapes can be defined, covering the Scully vortex \((n=1)\), the Lamb-Oseen vortex \((n \approx 2)\), or the Rankine vortex \((n=\infty)\). When the data are cleaned from spurious vectors, mean values of the flow subtracted and rotated into the vortex axis system, the distribution of swirl velocities of all vectors is fitted with the Vatistas model using a least squares error method. The best fit is performed at a radial extension of 2-3 core radii.