\[ \Lambda(r) = \lambda_{\text{bed}}(r) + K_1 \left( \frac{u_c}{u_0} f(R - r) \right) \lambda_f \]  
(17)

The damping function \( f(R - r) \) remains the same as for the mass transfer (Eq. (11)), while the slope parameter and the damping parameter are slightly modified, respectively,

\[ K_1 = \frac{1}{8} \]  
(18)

\[ K_2 = 0.44 + 4 \exp \left( -\frac{Re_d}{70} \right) \]  
(19)

The heat release by adsorption, see [19] for \( \Delta H_{\text{ads}} \), is derived in the last term on the right-hand side of Eq. (14) from the change of solids load with time. This very term couples the energy with the mass balance, so that both have to be solved simultaneously in order to account for thermal effects. Heat transfer resistances to or in the particles are neglected. The terms \( \delta_{\text{ads}}(r) \) and \( \lambda_{\text{ads}}(r) \) in Eqs. (8), (10), (15) and (17) describe the isotropic effective diffusivity and thermal conductivity of the bed without fluid flow. Boundary and initial conditions for Eqs. (7) and (14) are recapitulated in Tab. 1.

On the basis of the above described general model various reductions are possible by neglecting thermal effects, the radial coordinate or gas-to-particle and intraparticle mass transfer resistances. From such reduced versions the following has been considered in more detail in the present work:
1) plug-flow model (1-D) with local equilibrium between the gas and the solids,

2) plug-flow model (1-D) with mass transfer resistance to the solids,

3) 2-D maldistribution model with local equilibrium,

4) 2-D maldistribution model with mass transfer resistance to the solids.

In our terminology “plug flow” means that every influence of the radial coordinate is neglected, including the influence of the wall on porosity and flow velocity. However, axial dispersion, as expressed by the dispersion coefficient \( D_{\text{ax}} \), is accounted for, so that the equation

\[ \psi \frac{\partial Y}{\partial t} = D_{\text{ax}} \frac{\partial^2 Y}{\partial z^2} - u_0 \frac{\partial Y}{\partial z} - \left[ 1 - \psi \right] \frac{\partial X p}{\partial t} \]  
(20)

applies to the isothermal plug flow models (models 1 and 2).

Eq. (20) is the classical, conventional way to model packed bed adsorbers. Local equilibrium corresponds, in terms of the two-layers model from [19], to the limiting case of \( \beta_f \to \infty \) and \( \beta_p \to \infty \). At this limit, equilibrium is considered to be sufficient for calculating the response of the solid phase to changes of the concentration in the fluid. Model 4 is our complete, highest order model, as previously outlined and in exact correspondence to [13–18]. Mainly this model has been evaluated for both isothermal and non-isothermal conditions.

### 4 Numerical Solution and its Validation

The partial differential equation or equations of the various models have been solved by the method of lines. The numerical calculations were conducted for different mesh densities, and the results accepted when the calculated gas moisture content values was lower than 0.05 % of the maximal difference of gas moisture content appearing in the packed bed. When the error was bigger, the mesh was made denser. Since the width of the concentration front is, in many cases, not much smaller than the length of the bed, equidistant meshes have been used in the axial direction. In the maldistribution models (models 3 and 4 in the previous section) meshes that were denser near the wall than in the center of the tube have been applied.

To check the numerical procedure, respective results have been compared with available analytical solutions. One of such a solution is attributed to Anselius [1] and refers to model 2 after the classification of section 3, additionally reduced by neglecting axial dispersion \( D_{\text{ax}} = 0 \). Furthermore, it is assumed that the sorption equilibrium is throughout linear (“Henry’s law”), and that the bed is long. The mass transfer resistance is attributed to the fluid phase. Then, axial profiles can be derived to

\[ \frac{C}{C_{\text{in}}} = \frac{1}{2} \text{erfc} \left( \sqrt{\xi - \tau} \right) \]  
(21)

with

\[ \xi = 6 \frac{\beta_c}{d_p} \frac{1 - \phi}{2} \]  
(22)

and

\[ \tau = 6 \frac{\beta_c}{d_p} \lambda \left( 1 - \frac{z}{L} \right) \]  
(23)

In Eq. (21) the concentration of adsorbate in the gas phase, \( C \), is used instead of the content, \( Y \), assuming an ini-

| \( t > 0 \) | \( 0 \leq r \leq R \) | \( z = 0 \) | \( Y = Y_{\text{in}} \) | \( u_0(Y_{\text{in}} - Y) = -D_{\text{ax}} \frac{\partial Y}{\partial t} \) | \( T = T_{\text{in}} \) |
| \( t > 0 \) | \( 0 \leq z \leq L \) | \( r = 0 \) | \( \frac{\partial Y}{\partial r} = 0 \) | \( \frac{\partial Y}{\partial t} = 0 \) | \( \frac{\partial T}{\partial t} = 0 \) |
| \( t = 0 \) | \( 0 \leq r \leq R \) | \( 0 \leq z \leq L \) | \( X(r,z) = X_0 \) | \( Y(r,z) = Y_0 \) | \( T(r,z) = T_0 \) |

Table 1. Boundary and initial conditions for models.