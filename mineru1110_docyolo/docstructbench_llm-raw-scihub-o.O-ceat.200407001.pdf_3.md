$$
\begin{array}{r l r}{\Lambda_{\mathrm{r}}({\bf r})}&{{}=}&{\lambda_{\mathrm{bed}}({\bf r})+\bf K_{1}\;\;{\sf P e}_{0}\;\;\frac{u_{\mathrm{c}}}{\bar{u}_{0}}\;\;{\bf f}({\bf R}-{\bf r})\;\lambda_{\mathrm{f}}}\end{array}
$$  

The damping function  $\operatorname{f}(\mathbf{R}{\mathrm{-}}\mathbf{r})$   remains the same as for the mass transfer (Eq.(11)), while the slope parameter and the damping parameter are slightly modified to, respectively,  

$$
\mathbf{K}_{1}=\frac{1}{8}
$$  

and  $\upbeta_{\mathrm{p}}\rightarrow\infty$  . At this limit, equilibrium is considered to be sufficient for calculating the response of the solid phase to changes of the concentration in the fluid. Model 4 is our complete, highest order model, as previously outlined and in exact correspondence to [13-18]. Mainly this model has been evaluated for both isothermal and non-isothermal conditions.  

$$
\mathbf{K}_{2}~=~0.44~+~4~\mathrm{exp}\biggl(-\frac{\mathbf{Re}_{0}}{70}\biggr)
$$  

The heat release by adsorption, see [19] for  $\Delta\mathrm{H_{ad}}$  ,is derived in the last term on the right-hand side of Eq.(14) from the change of solids load with time. This very term couples the energy with the mass balance, so that both have to be solved simultaneously in order to account for thermal effects. Heat transfer resistances to or in the particles are neglected. The terms  $\updelta_{\mathrm{bed}}(\mathbf{r})$  and  $\lambda_{\mathrm{bed}}(\mathbf{r})$  in Eqs. (8), (10), (15) and (17) describe the isotropic effective diffusivity and thermal conductivity of the bed without fluid flow. Boundary and initial conditions for Eqs. (7) and (14) are recapitulated in Tab. 1.  

On the basis of the above described general model various reductions are possible by neglecting thermal effects, the radial coordinate or gas-to-particle and intraparticle mass transfer resistances. From such reduced versions the following has been considered in more detail in the present work:  

1) plug-flow model (1-D) with local equilibrium between the gas and the solids, the solids,   
3) 2-D maldistribution model with local equilibrium,   
4) 2-D maldistribution model with mass transfer resistance to the solids.  

In our terminology “plug flow" means that every influence of the radial coordinate is neglected, including the influence of the wall on porosity and flow velocity. However, axial dispersion, as expressed by the dispersion coefficient  $\mathrm{D}_{\mathrm{ax}}$  ,is accounted for, so that the equation  

# 4 Numerical Solution and its Validation  

The partial differential equation or equations of the various models have been solved by the method of lines. The numerical calculations were conducted for different mesh densities, and the results accepted when the change of calculated gas moisture content values was lower than  $0.05\,\%$  of the maximal difference of gas moisture content appearing in the packed bed. When the error was bigger, the mesh was made denser. Since the width of the concentration front is, in many cases, not much smaller than the length of the bed, equidistant meshes have been used in the axial direction. In the maldistribution models (models 3 and 4 in the previous section) meshes that were denser near the wall than in the center of the tube have been applied.  

To check the numerical procedure, respective results have been compared with available analytical solutions. One of such a solution is attributed to Anzelius [1] and refers to model 2 after the classification of section 3, additionally reduced by neglecting axial dispersion  $(\mathbf{D}_{\mathbf{ax}}=0)$  ).Furthermore, it is assumed that the sorption equilibrium is throughout linear ("Henry's law"), and that the bed is long. The mass transfer resistance is attributed to the fluid phase. Then, axial profiles can be derived to  

$$
{\frac{\mathbf{C}}{\mathbf{C}_{\mathrm{in}}}}={\frac{1}{2}}\operatorname{erfc}\!\left({\sqrt{\xi}}-{\sqrt{\uptau}}\right)
$$  

with  

$$
\bar{\mathsf{\xi}}=6\frac{\mathsf{\beta}_{\mathrm{f}}}{\mathsf{d}_{\mathrm{p}}}\frac{\mathsf{Z}}{\mathsf{u}}\frac{1-\uppsi}{\uppsi}
$$  

$$
\bar{\Psi}\frac{\partial\mathbf{Y}}{\partial\ t}=\mathbf{D}_{\mathrm{ax}}\,\frac{\partial^{2}\mathbf{Y}}{\partial\ z^{2}}-\bar{\mathbf{u}}_{0}\,\frac{\partial\mathbf{Y}}{\partial\ z}-[1-\bar{\Psi}]\frac{\partial\mathbf{X}}{\partial\ t}\frac{\partial_{\mathrm{p}}}{\rho_{\mathrm{f}}}
$$  

applies to the isothermal plug flow models (models 1 and 2). Eq. (20) is the classical, conventional way to model packed bed adsorbers. Local equilibrium corresponds, in terms of the two-layers model from [19], to the limiting case of  $\upbeta_{\mathrm{f}}\to\infty$  

and  

$$
\uptau=6\frac{\upbeta_{\mathrm{f}}}{\mathrm{d}_{\mathrm{p}}\mathrm{K}}\left(\up t-\frac{\mathrm{Z}}{\upmu}\right)
$$  

Table 1. Boundary and initial conditions for models.   


<td><table  border="1"><thead><tr><td><b>t>0</b></td><td><b>O≤r≤R</b></td><td><b>Z=0</b></td><td></td><td><b>Y = Yin or uo(Yin -Y)= -D</b></td><td><b>T=Tin</b></td></tr><tr><td></td><td></td><td><b>z=L</b></td><td><b>=0</b></td><td><b>W=0</b></td><td><b>=0</b></td></tr></thead><tbody><tr><td>t>0</td><td>O≤z≤L</td><td>r=0</td><td>=0</td><td>%=0</td><td>=0</td></tr><tr><td></td><td></td><td>r=R</td><td>=0</td><td>=0</td><td>T=Tw</td></tr><tr><td>t=0</td><td>O≤r≤R</td><td>O≤z≤L</td><td>X(r,z) = Xo</td><td>Y(r,z)= Y。</td><td>T(r,z)= To</td></tr></tbody></table></td>  

In Eq. (21) the concentration of adsorbate in the gas phase,  $C_{v}$  . is used instead of the content, Y, assuming an ini  