
\[
{\partial }_{t}{z}_{i, j, k}^{l} = \frac{{z}_{i, j, k}^{l + 1} - {z}_{i, j, k}^{l}}{\Delta t},\;{\bar{\partial }}_{t}{z}_{i, j, k}^{l} = \frac{{z}_{i, j, k}^{l + 1} - {z}_{i, j, k}^{l - 1}}{2\Delta t},\;{\partial }_{{x}_{1}}{z}_{i, j, k}^{l} = \frac{{z}_{i + 1, j, k}^{l} - {z}_{i, j, k}^{l}}{\Delta {x}_{1}},\;{\bar{\partial }}_{{x}_{1}}{z}_{i, j, k}^{l} = \frac{{z}_{i + 1, j, k}^{l} - {z}_{i - 1, j, k}^{l}}{{2\Delta }{x}_{1}},
\]

where the difference operators \( {\partial }_{t},{\bar{\partial }}_{t} \) are the discretization of \( \frac{\partial }{\partial t} \) , and the difference operators \( {\partial }_{{x}_{1}},{\bar{\partial }}_{{x}_{1}} \) are the discretization of \( \frac{\partial }{\partial {x}_{1}} \) . Via these notations and the properties of the difference operators, \( {}^{6} \) we present the statement of the local/global conservation laws for the different numerical methods.

### 3.1. Symplectic method for Maxwell's equations

The following method is constructed based on the method of lines, i.e. discretizing the Hamiltonian PDEs in space, then applying the symplectic method to the resulting Hamiltonian ODEs (see for example [6,22]). Later, we will show the method is also multisymplectic in the corresponding statement of multisymplecticity.

For Maxwell's equations in Hamiltonian form, we use the central finite difference in space (which is leapfrog discretiza-tion) and implicit midpoint rule (which is symplectic) in time, it is easy to show that the Hamiltonian formulations in (5) and (7) for Maxwell's equations reduce to the same discretized system,

\[
{\partial }_{t}{z}_{i, j, k}^{l} + {M}^{-1}{K}_{1}{\bar{\partial }}_{{x}_{1}}{z}_{i, j, k}^{l + \frac{1}{2}} + {M}^{-1}{K}_{2}{\bar{\partial }}_{{x}_{2}}{z}_{i, j, k}^{l + \frac{1}{2}} + {M}^{-1}{K}_{3}{\bar{\partial }}_{{x}_{3}}{z}_{i, j, k}^{l + \frac{1}{2}} = 0, \tag{18}
\]

where indices \( i, j, k \) denote spatial increments and index \( l \) denotes time increment, and matrices \( M,{K}_{1},\ldots \) as in (10). We refer to this particular discretization as the symplectic method, though it is also multisymplectic.

The symplectic method (18) is second-order in space and time, and is unconditionally stable. Furthermore, this discrete system preserves two discretized global conservation laws: the first one is the discrete quadratic global conservation law based on (8),

\[
\frac{1}{2}{\partial }_{t}\left\lbrack  {\mu {\mathbf{H}}_{i, j, k}^{l} \cdot  {\mathbf{H}}_{i, j, k}^{l} + \varepsilon {\mathbf{E}}_{i, j, k}^{l} \cdot  {\mathbf{E}}_{i, j, k}^{l}}\right\rbrack   = 0. \tag{19}
\]

The second discretized global conservation law for symplectic method is based on the helicity Hamiltonian functional (6)

\[
{\partial }_{t}\left\lbrack  {\frac{1}{2\varepsilon }{\mathbf{H}}_{i, j, k}^{l} \cdot  \widehat{\nabla } \times  {\mathbf{H}}_{i, j, k}^{l} + \frac{1}{2\mu }{\mathbf{E}}_{i, j, k}^{l} \cdot  \widehat{\nabla } \times  {\mathbf{E}}_{i, j, k}^{l}}\right\rbrack   = 0, \tag{20}
\]

where \( \widehat{\nabla } \times   = {R}_{1}{\partial }_{{x}_{1}} + {R}_{2}{\partial }_{{x}_{2}} + {R}_{3}{\partial }_{{x}_{3}} \) . Furthermore, the scheme (18) is proved to be multisymplectic, since it preserves the following multisymplectic conservation law

\[
{\partial }_{t}\left\lbrack  {d{\mathbf{E}}_{i, j, k}^{l} \land  d{\mathbf{H}}_{i, j, k}^{l}}\right\rbrack   + {\partial }_{{x}_{1}}\left\lbrack  {\frac{1}{\varepsilon }d{\mathbf{H}}_{i - 1, j, k}^{l + \frac{1}{2}} \land  {R}_{1}d{\mathbf{H}}_{i, j, k}^{l + \frac{1}{2}} + \frac{1}{\mu }d{\mathbf{E}}_{i - 1, j, k}^{l + \frac{1}{2}} \land  {R}_{1}d{\mathbf{E}}_{i, j, k}^{l + \frac{1}{2}}}\right\rbrack   + {\partial }_{{x}_{2}}\left\lbrack  {\frac{1}{\varepsilon }d{\mathbf{H}}_{i, j - 1, k}^{l + \frac{1}{2}} \land  {R}_{2}d{\mathbf{H}}_{i, j, k}^{l + \frac{1}{2}} + \frac{1}{\mu }d{\mathbf{E}}_{i, j - 1, k}^{l + \frac{1}{2}} \land  {R}_{2}d{\mathbf{E}}_{i, j, k}^{l + \frac{1}{2}}}\right\rbrack
\]

\[
+ {\partial }_{{x}_{3}}\left\lbrack  {\frac{1}{\varepsilon }d{\mathbf{H}}_{i, j, k - 1}^{l + \frac{1}{2}} \land  {R}_{3}d{\mathbf{H}}_{i, j, k}^{l + \frac{1}{2}} + \frac{1}{\mu }d{\mathbf{E}}_{i, j, k - 1}^{l + \frac{1}{2}} \land  {R}_{3}d{\mathbf{E}}_{i, j, k}^{l + \frac{1}{2}}}\right\rbrack   = 0. \tag{21}
\]

Besides the global conservation laws, for the scheme (18) applied to Maxwell's equations, we also have the following local conservation laws based on (13)-(15):

The discrete quadratic conservation law is

\[
\frac{1}{2}{\partial }_{t}\left\lbrack  {\mu {\mathbf{H}}_{i, j, k}^{l} \cdot  {\mathbf{H}}_{i, j, k}^{l} + \varepsilon {\mathbf{E}}_{i, j, k}^{l} \cdot  {\mathbf{E}}_{i, j, k}^{l}}\right\rbrack   + \frac{1}{2}{\partial }_{{x}_{1}}\left\lbrack  {{\mathbf{H}}_{i, j, k}^{l + \frac{1}{2}} \cdot  {R}_{1}{\mathbf{E}}_{i - 1, j, k}^{l + \frac{1}{2}} + {\mathbf{H}}_{i - 1, j, k}^{l + \frac{1}{2}} \cdot  {R}_{1}{\mathbf{E}}_{i, j, k}^{l + \frac{1}{2}}}\right\rbrack   + \frac{1}{2}{\partial }_{{x}_{2}}\left\lbrack  {{\mathbf{H}}_{i, j, k}^{l + \frac{1}{2}} \cdot  {R}_{2}{\mathbf{E}}_{i, j - 1, k}^{l + \frac{1}{2}} + {\mathbf{H}}_{i, j - 1, k}^{l + \frac{1}{2}} \cdot  {R}_{2}{\mathbf{E}}_{i, j, k}^{l + \frac{1}{2}}}\right\rbrack
\]

\[
+ \frac{1}{2}{\partial }_{{x}_{3}}\left\lbrack  {{\mathbf{H}}_{i, j, k}^{l + \frac{1}{2}} \cdot  {R}_{3}{\mathbf{E}}_{i, j, k - 1}^{l + \frac{1}{2}} + {\mathbf{H}}_{i, j, k - 1}^{l + \frac{1}{2}} \cdot  {R}_{3}{\mathbf{E}}_{i, j, k}^{l + \frac{1}{2}}}\right\rbrack   = 0. \tag{22}
\]

The discrete energy conservation law is

\[
{\partial }_{t}\left\lbrack  {\frac{1}{2\varepsilon }{\mathbf{H}}_{i, j, k}^{l} \cdot  \widehat{\nabla } \times  {\mathbf{H}}_{i, j, k}^{l} + \frac{1}{2\mu }{\mathbf{E}}_{i, j, k}^{l} \cdot  \widehat{\nabla } \times  {\mathbf{E}}_{i, j, k}^{l}}\right\rbrack   + {\partial }_{{x}_{1}}\left\lbrack  {\frac{1}{2\varepsilon }{\partial }_{t}{\mathbf{H}}_{i, j, k}^{l} \cdot  {R}_{1}{\mathbf{H}}_{i - 1, j, k}^{l + \frac{1}{2}} + \frac{1}{2\mu }{\partial }_{t}{\mathbf{E}}_{i, j, k}^{l} \cdot  {R}_{1}{\mathbf{E}}_{i - 1, j, k}^{l + \frac{1}{2}}}\right\rbrack
\]

\[
+ {\partial }_{{x}_{2}}\left\lbrack  {\frac{1}{2\varepsilon }{\partial }_{t}{\mathbf{H}}_{i, j, k}^{l} \cdot  {R}_{2}{\mathbf{H}}_{i, j - 1, k}^{l + \frac{1}{2}} + \frac{1}{2\mu }{\partial }_{t}{\mathbf{E}}_{i, j, k}^{l} \cdot  {R}_{2}{\mathbf{E}}_{i, j - 1, k}^{l + \frac{1}{2}}}\right\rbrack   + {\partial }_{{x}_{3}}\left\lbrack  {\frac{1}{2\varepsilon }{\partial }_{t}{\mathbf{H}}_{i, j, k}^{l} \cdot  {R}_{3}{\mathbf{H}}_{i, j, k - 1}^{l + \frac{1}{2}} + \frac{1}{2\mu }{\partial }_{t}{\mathbf{E}}_{i, j, k}^{l} \cdot  {R}_{3}{\mathbf{E}}_{i, j, k - 1}^{l + \frac{1}{2}}}\right\rbrack   = 0. \tag{23}
\]

The discrete momentum conservation law is

---

\( {}^{6} \) Let \( {p}_{i} \) and \( {q}_{i} \) are the functions at grid \( i,\partial ,\bar{\partial } \) are the difference operators, then

\[
\partial \left\lbrack  {{q}_{i}{p}_{i}}\right\rbrack   = {q}_{i + 1}\partial {p}_{i} + \partial {q}_{i}{p}_{i} = \partial {q}_{i}{p}_{i + 1} + {q}_{i}\partial {p}_{i},
\]

\[
\partial \left\lbrack  {{q}_{i + 1}{p}_{i}}\right\rbrack   = \partial {q}_{i + 1}{p}_{i + 1} + {q}_{i + 1}\partial {p}_{i},
\]

\[
\bar{\partial }\left\lbrack  {{q}_{i}{p}_{i}}\right\rbrack   = \bar{\partial }{q}_{i}{p}_{i + 1} + {q}_{i - 1}\bar{\partial }{p}_{i} = \bar{\partial }{p}_{i}{q}_{i + 1} + {p}_{i - 1}\bar{\partial }{q}_{i},
\]

\[
\bar{\partial }\left\lbrack  {{q}_{i}{p}_{i + 1}}\right\rbrack   = {q}_{i + 1}\bar{\partial }{p}_{i + 1} + \bar{\partial }{q}_{i}{p}_{i}.
\]

---