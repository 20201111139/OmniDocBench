Λr (r) = λbed(r) + K₁ Pe₀ \( \frac{u_c}{u_0} \) f(R − r) λf (17)

The damping function f(R−r) remains the same as for the mass transfer (Eq.(11)), while the slope parameter and the damping parameter are slightly modified to, respectively,

K₁ = \( \frac{1}{8} \) (18)

K₂ = 0.44 + 4 exp\( (-\frac{Re_0}{70}) \) (19)

The heat release by adsorption, see [19] for ∆Had, is derived in the last term on the right-hand side of Eq.(14) from the change of solids load with time. This very term couples the energy with the mass balance, so that both have to be solved simultaneously in order to account for thermal effects. Heat transfer resistances to or in the particles are neglected. The terms δbed(r) and λbed(r) in Eqs. (8), (10), (15) and (17) describe the isotropic effective diffusivity and thermal conductivity of the bed without fluid flow. Boundary and initial conditions for Eqs. (7) and (14) are recapitulated in Tab. 1.

On the basis of the above described general model various reductions are possible by neglecting thermal effects, the radial coordinate or gas-to-particle and intraparticle mass transfer resistances. From such reduced versions the following has been considered in more detail in the present work:
1) plug-flow model (1-D) with local equilibrium between the gas and the solids,
2) plug-flow model (1-D) with mass transfer resistance to the solids,
3) 2-D maldistribution model with local equilibrium,
4) 2-D maldistribution model with mass transfer resistance to the solids.

In our terminology "plug flow" means that every influence of the radial coordinate is neglected, including the influence of the wall on porosity and flow velocity. However, axial dispersion, as expressed by the dispersion coefficient Dax, is accounted for, so that the equation

Ψ \( \frac{∂Y}{∂t} \) = Dax \( \frac{∂²Y}{∂z²} \) - u₀ \( \frac{∂Y}{∂z} \) - [1 − ψ] \( \frac{∂X}{∂t} \)\( \frac{ρ_p}{ρ_f} \) (20)

applies to the isothermal plug flow models (models 1 and 2). Eq. (20) is the classical, conventional way to model packed bed adsorbers. Local equilibrium corresponds, in terms of the two-layers model from [19], to the limiting case of βf → ∞

and βp → ∞. At this limit, equilibrium is considered to be sufficient for calculating the response of the solid phase to changes of the concentration in the fluid. Model 4 is our complete, highest order model, as previously outlined and in exact correspondence to [13-18]. Mainly this model has been evaluated for both isothermal and non-isothermal conditions.

### 4 Numerical Solution and its Validation

The partial differential equation or equations of the various models have been solved by the method of lines. The numerical calculations were conducted for different mesh densities, and the results accepted when the change of calculated gas moisture content values was lower than 0.05 % of the maximal difference of gas moisture content appearing in the packed bed. When the error was bigger, the mesh was made denser. Since the width of the concentration front is, in many cases, not much smaller than the length of the bed, equidistant meshes have been used in the axial direction. In the maldistribution models (models 3 and 4 in the previous section) meshes that were denser near the wall than in the center of the tube have been applied.

To check the numerical procedure, respective results have been compared with available analytical solutions. One of such a solution is attributed to Anzelius [1] and refers to model 2 after the classification of section 3, additionally reduced by neglecting axial dispersion (Dax = 0). Furthermore, it is assumed that the sorption equilibrium is throughout linear ("Henry's law"), and that the bed is long. The mass transfer resistance is attributed to the fluid phase. Then, axial profiles can be derived to

\( \frac{C}{C_{in}} \) = \( \frac{1}{2} \) erfc(\( \sqrt{\xi} \) − \( \sqrt{τ} \)) (21)

with

ξ = 6 \( \frac{β_f}{d_p} \)\( \frac{z}{u} \)\( \frac{1-ψ}{ψ} \) (22)

and

τ = 6 \( \frac{β_f}{d_p} \)\( \frac{K}{u} \) (t − \( \frac{z}{u} \)) (23)

In Eq. (21) the concentration of adsorbate in the gas phase, C, is used instead of the content, Y, assuming an ini-

<table>
 <tr>
 <td>t>0</td>
 <td>0≤ r ≤ R</td>
 <td>z = 0</td>
 <td>Y = Yin
 or
 u₀(Yin Y) = -Dax \( \frac{∂Y}{∂z} \)
 </td>
 <td>T = Tin</td>
 </tr>
 <tr>
 <td></td>
 <td></td>
 <td>z = L</td>
 <td>\( \frac{∂X}{∂z} \) = 0</td>
 <td>\( \frac{∂Y}{∂z} \) = 0</td>
 <td>\( \frac{∂T}{∂z} \) = 0</td>
 </tr>
 <tr>
 <td>t>0</td>
 <td>0≤ z ≤ L</td>
 <td>r = 0</td>
 <td>\( \frac{∂X}{∂r} \) = 0</td>
 <td>\( \frac{∂Y}{∂r} \) = 0</td>
 <td>\( \frac{∂T}{∂r} \) = 0</td>
 </tr>
 <tr>
 <td></td>
 <td></td>
 <td>r = R</td>
 <td>\( \frac{∂X}{∂r} \) = 0</td>
 <td>\( \frac{∂Y}{∂r} \) = 0</td>
 <td>T = Tw</td>
 </tr>
 <tr>
 <td>t = 0</td>
 <td>0≤ r ≤ R</td>
 <td>0≤ z ≤ L</td>
 <td>X(r,z) = X₀</td>
 <td>Y(r,z) = Y₀</td>
 <td>T(r,z) = T₀</td>
 </tr>
</table>