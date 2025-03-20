<!-- C PE αT  -->
![](https://web-api.textin.com/ocr_image/external/6175bd710e99f43b.jpg)

$\wedge _{r}(r)=\lambda _{bed}(r)+K_{1}Pe_{0}\frac {u_{c}}{\overline {u_{0}}}f(R-r)\lambda _{f}$ (17)

The damping functionf(R-r) remains the same as for the mass transfer (Eq.(11)), while the slope parameter and the damping parameter are slightly modified to, respectively,

$K_{1}=\frac {1}{8}$ (18)

$K_{2}=0.44+4\exp (-\frac {Re_{0}}{70})$ (19)

The heat release by adsorption, see [19]for Δ$H_{ad},$is de-rived in the last term on the right-hand sideof Eq.(14)from the change of solids load with time. This very term couples the energy with the mass balance, so that both have to be solved simultaneously in order to account for thermal ef-fects. Heat transfer resistances to or in the particles are ne-glected. The terms$\delta _{bcd}(r)$and入bed（r）in Eqs．（8），（10），（15）and (17) describe the isotropic effective diffusivity and ther-mal conductivity of the bed without fluid flow. Boundary and initial conditions for Eqs. (7) and (14) are recapitulated in Tab.1.

On the basis of the above described general model various reductions are possible by neglecting thermal effects,the ra-dial coordinate or gas-to-particle and intraparticle mass transfer resistances. From such reduced versions the follow-ing has been considered in more detail in the present work:

1) plug-flow model (1-D) with local equilibrium between the gas and the solids,

2) plug-flow model (1-D) with mass transfer resistance to the solids,

3) 2-D maldistribution model with local equilibrium,

4) 2-D maldistribution model with mass transfer resistance to the solids.

In our terminology “plug flow” means that every influence of the radial coordinate is neglected, including the influence of the wall on porosity and flow velocity. However, axial dis-persion, as expressed by thedispersion coefficient$D_{ax}$is ac-counted for, so that the equation

$\overline {v}\frac {\partial Y}{\partial t}=D_{ax}\frac {\partial ^{2}Y}{\partial t^{2}}-a_{0}\frac {\partial Y}{\partial Z}-[1-\overline {\psi }]\frac {\partial X}{\partial t}\frac {\rho _{p}}{\rho _{f}}$ (20)

applies to the isothermal plug flow models (models 1 and 2).Eq.(20) is the classical,conventional way to model packed bed adsorbers. Local equilibrium corresponds, in terms of the two-layers model from [19],to the limiting case of$\beta _{f}\rightarrow \infty$

and$\beta _{p}\rightarrow \infty .$At this limit, equilibrium is considered to be sufficient for calculating the response of the solid phase to changes of the concentration in the fluid. Model 4 is our complete, highest order model, as previously outlined and in exact correspondence to [13-18].Mainly this model has been evaluated for both isothermal and non-isothermal condi-tions.

## 4 Numerical Solution and its Validation

The partial differential equation or equations of the var-ious models have been solved by the method of lines. The numerical calculations were conducted for different mesh densities, and the results accepted when the change of calcu-lated gas moisture content values was lower than 0.05% of the maximal difference of gas moisture content appearing in the packed bed. When the error was bigger,the mesh was made denser. Since the width of the concentration front is,in many cases, not much smaller than the length of the bed,equidistant meshes have been used in the axial direction. In the maldistribution models (models 3 and 4 in the previous section) meshes that were denser near the wall than in the center of the tube have been applied.

To check the numerical procedure, respective results have been compared with available analytical solutions. One of such a solution is attributed to Anzelius [1] and refers to model 2 after the classification of section 3, additionally re-duced by neglecting axial dispersion$(D_{ax}=0).$Furthermore,it is assumed that thesorption equilibrium is throughout lin-ear (“Henry's law”), and that the bed is long. The mass transfer resistance is attributed to the fluid phase. Then,ax-ial profiles can be derived to

$\frac {C}{C_{\in }}=\frac {1}{2}erfc(\sqrt {\xi }-\sqrt {\tau })$ (21)

with

$\xi =6\frac {\beta _{f}}{d_{p}}\frac {Z1-\psi }{u}$ (22)

and

$\tau =6\frac {\beta _{f}}{d_{p}K}(t-\frac {Z}{u})$ (23)

In Eq. (21) the concentration of adsorbate in the gas phase, C, is used instead of the content, Y,assuming an ini-

Table 1.Boundary and initial conditions for models.


| $t>0$ | $0\leq r\leq R$ | $z=0$ |  | $Y=Y_{\in }$ or $u_{0}(Y_{\in }-Y)=-D_{ax}\frac {\partial Y}{\partial Z}$ $\frac {\partial Y}{\partial Z}=0$ | $T=T_{\in }$ $\frac {\partial T}{\partial Z}=0$ |
| -- | -- | -- | -- | -- | -- |
| $t>0$ | $0\leq r\leq R$ | $Z=L$ | $\frac {\partial x}{\partial z}=0$ | $Y=Y_{\in }$ or $u_{0}(Y_{\in }-Y)=-D_{ax}\frac {\partial Y}{\partial Z}$ $\frac {\partial Y}{\partial Z}=0$ | $T=T_{\in }$ $\frac {\partial T}{\partial Z}=0$ |
| $t>0$ | $0\leq z\leq L$ | $r=0$ $r=R$ | $\frac {\partial x}{\partial r}=0$ $\frac {\partial x}{\partial r}=0$ | $\frac {\partial Y}{\partial T}=0$ $\frac {\partial Y}{\partial T}=0$ | $\frac {\partial T}{\partial T}=0$ $T=T_{w}$ |
| $t=0$ | $0\leq r\leq R$ | $0\leq z\leq L$ | $X(r,z)=X_{0}$ | $Y(r,Z)=Y_{0}$ | $T(r,z)=T_{0}$ |


