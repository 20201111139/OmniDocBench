Y. Sun, PS.P Tse / Journal of Computational Physics 230 (2011) 2076-2094

Zifk Zijk d.2ijk Zk_ 238 dx,Zijk Zi+jk Zjk _ 8x,Zjk Z+jk-4-1jk

At 2At Ax1 2Ax1 where the difference operators dt, dt are the discretization of % and the difference operators &x1 ax, are the discretization of dx1. Via these notations and the properties of the difference operators, we present the statement of the local/global conservation laws for the different numerical methods.

# 3.1. Symplectic method for Maxwell's equations

The following method is constructed based on the method of lines, i.e. discretizing the Hamiltonian PDEs in space; then applying the symplectic method to the resulting Hamiltonian ODEs (see for example [6,22]). Later; we will show the method is also multisymplectic in the corresponding statement of multisymplecticity:

For Maxwell's equations in Hamiltonian form; we use the central finite difference in space (which is leapfrog discretization) and implicit midpoint rule (which is symplectic) in time, it is easy to show that the Hamiltonian formulations in (5) and (7 for Maxwell's equations reduce to the same discretized system.

8.2ijk 0 (18) where indices i,j,k denote spatial increments and index denotes time increment, and matrices M, K1, as in (10). We refer to this particular discretization as the symplectic method, though it is also multisymplectic.

The symplectic method (18) is second-order in space and time, and is unconditionally stable. Furthermore, this discrete system preserves two discretized global conservation laws: the first one is the discrete quadratic global conservation law based on (8),

=0. 197

The second discretized global conservation law for symplectic method is based on the helicity Hamiltonian functional (6)

0: [22Hjk Hijk 2Ej4 XEijk] 0. 207 where Rjax, + Rzoxz + Rzax;: Furthermore, the scheme (18) is proved to be multisymplectic, since it preserves the following multisymplectic conservation law

04| dE'jk dHIjk] + &x[axt j - R1 R1 + 8x2 dH}-,k - dH};k dE;-1k dEJk| = 0.

Besides the global conservation laws, for the scheme (18) applied to Maxwell's equations, we also have the following local conservation laws based on (13)-(15):

The discrete quadratic conservation law is

H{j,k ` RzE;jk] (22)

The discrete energy conservation law is

-Hijk" Hijk = 1 Eijk ' xEjk/ + 8x1 0 [2e +21 +0x [22o,H,jk RzH;j-1k + 8x3 =0. (23)

The discrete momentum conservation law is

Let pi and qi are the functions at grid 0, & are the difference operators, then

aiq,p;] 9i+1dp; + dq;P; dq,Pi+1 + q,dp;, d[qi+1P] dqi+1Pi+1 + Qi+1 dp;; o[qiP;] Oq,Pin1 + Qi-1 dp; Dp,qi+1 + Pi-1dqi.

Djq,Pi+1] dqiPi: = Qi+dpi+