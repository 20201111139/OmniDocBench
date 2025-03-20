```markdown
# 4 Numerical Solution and its Validation

The partial differential equation or equations of the various models have been solved by the method of lines. The numerical calculations were conducted for different mesh densities, and the results accepted when the change of calculated gas maximal difference content values was lower than 0.05% in the evaluated moisture content of gas moisture content appearing in selected terms \( \partial_{\text{ax}} f(r) \) and \( \partial_{\text{ax}} f(r) \) in Eqs. (8), (10), (15) and (17) describe the isotropic effective diffusivity and boundary conditions for the bed. The initial conditions for Eqs. (7) and (14) are recapitulated in Tab. 1.

On the basis of the above described general model various reductions are possible by neglecting thermal effects, the radial coordinate or gas-to-particle and intraparticle mass transfer resistances. From such detailed versions the following models have been considered in more detail in the follow-ing sections: 1) plug-flow model (1-D) with local equilibrium between the gas and the solids, 2) plug-flow model (1-D) with mass transfer resistance to the solids, 3) 2-D mal-distribution model with local equilibrium, 4) 2-D mal-distribution model with mass transfer resistance to the solids.

In our terminology "plug flow" means that every influence of the radial coordinate is neglected, including the axial dispersion on the basis of velocity. However, the influence of the radial on the radial coordinate is neglected, including the axial dispersion on the basis of velocity. However, the in-fluence of the radial on the radial coordinate is neglected, including the axial dispersion on the basis of velocity.

The mass transfer resistance is attributed to the fluid phase. Then, axial profiles can be derived to

\[ C_{\text{in}} = \frac{2}{\text{erfc}(\sqrt{\frac{V_{\text{in}}}{D_{\text{ax}}}} - \sqrt{\frac{V_{\text{in}}}{D_{\text{ax}}}}} \]

with

\[ \xi = \frac{\beta_{\text{in}} z_{\text{in}} - \nu}{\delta_{\text{in}} \mu} \]

and

\[ \frac{\partial Y}{\partial \theta} = D_{\text{ax}} \frac{\partial^2 Y}{\partial z^2} - \frac{\partial Y}{\partial z} \left[ 1 - \frac{\partial X_{\text{in}}}{\partial \theta} \right] \]

\[ r = \frac{\beta_{\text{in}}}{\delta_{\text{in}}} \left( 1 - \frac{z}{L} \right) \]

In Eq. (21) the concentration of adsorbate in the gas phase, C, is used instead of the content, Y, assuming an in-itial equilibrium.

Eq. (20) applies to the isothermal plug flow models (models 1 and 2). Eq. (20) is the classical, conventional way to model packed bed adsorbers. Local equilibrium corresponds, in terms of the two-layers model from [19], to the limiting case of \( \beta_{\text{in}} \rightarrow \infty \).

<table>
  <tr>
    <th>t > 0</th>
    <th>0 ≤ r ≤ R</th>
    <th>z = 0</th>
    <th>Y = Y_{\text{in}} or</th>
    <th>Y_{\text{in}}(Y_{\text{in}} - Y) = D_{\text{ax}} \frac{\partial Y}{\partial z} \bigg|_{z=0} \frac{\partial Y}{\partial z} \bigg|_{z=0} = 0</th>
    <th>T = T_{\text{in}}</th>
  </tr>
  <tr>
    <td></td>
    <td>z = L</td>
    <td>Y = 0</td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>t = 0</td>
    <td>0 ≤ z ≤ L</td>
    <td>r = 0</td>
    <td>Y = 0</td>
    <td></td> 
    <td>T = T_{\text{in}}</td>
  </tr>
  <tr>
    <td></td>
    <td>r = R</td>
    <td>Y = 0</td>
    <td></td></td>
    <td></td>
  </tr>
  <tr>
    </td>
    <td>0 ≤ r ≤ R</td>
    <td>0 ≤ z ≤ L</td>
    <td>X(z, t) = X_{\text{in}}</td>
    <td>Y(z, t) = Y_{\text{in}}</td>
    <td>T(z, t) = T_{\text{in}}</td>
  </tr>
</table>

Chem. Eng. Technol. 2004, 27, No. 11
http://www.ceet-journal.de
© 2004 WILEY-VCH Verlag GmbH & Co. KGaA, Weinheim
1181
```