# Worked examples

Choose a case by its writing task. Figures and benchmarks marked illustrative are teaching inputs; [primary sources](sources.md#physics-background-for-the-examples) supply the physical context.

| Field | Theory | Computation | Experiment |
| --- | --- | --- | --- |
| Condensed matter | [1. Fractional Chern states](#1-condensed-matter-theory) | [2. Tensor-network convergence](#2-condensed-matter-computation) | [3. Moiré transport caption](#3-condensed-matter-experiment) |
| Statistical physics | [4. Anomalous spin transport](#4-statistical-physics-theory) | [5. Trajectory-ensemble caption](#5-statistical-physics-computation) | [6. Active-matter mechanisms](#6-statistical-physics-experiment) |
| High energy / gravity | [7. Tidal Love coefficients](#7-gravity-theory) | [8. Waveform comparison](#8-gravity-computation) | [9. Collider entanglement](#9-high-energy-experiment) |

## 1. Condensed matter theory

**Context:** A chiral magic-angle graphene model assumes zero same-sublattice tunnelling, spin and valley polarization, a layer-independent sublattice potential isolating one Chern band, and specified projected pseudopotential interactions. An analytic construction supplies exact Laughlin-type ground states.

**Write**

> The specified projected interactions admit exact Laughlin-type ground states in the isolated Chern band of this chiral model.

Attach “exact” to the construction and its assumptions. State what has been established directly.

## 2. Condensed matter computation

**Illustrative inputs:** For optimized infinite projected entangled-pair states (iPEPS), energy per site and correlation length $\xi$ are extrapolated in contraction dimension $\chi$ at bond dimensions $D=4,6,8$. With $J$ the Hamiltonian's energy scale, energy changes by less than $10^{-4}J$, while $\xi$ grows from 4 to 11 lattice spacings.

**Write**

> After extrapolating both observables in $\chi$, increasing $D$ from 4 to 8 changes the energy per site by less than $10^{-4}J$, while $\xi$ grows from 4 to 11 lattice spacings. These calculations do not establish a gapped phase.

Name the observable and numerical control separately. In these optimized states, finite $D$ can truncate critical correlations. PEPS also admit critical finite-$D$ constructions.

## 3. Condensed matter experiment

**Illustrative caption**

> **Figure 1. Transport in rhombohedral pentalayer graphene on hexagonal boron nitride at 30 mK.** The gate-induced displacement field is fixed at $D/\epsilon_0=0.92$ V/nm, positive toward the aligned substrate. (a) Hall resistance magnitude $|R_{xy}|$ and (b) longitudinal resistance $R_{xx}$ versus moiré filling $\nu$ (electrons per moiré cell), at perpendicular magnetic fields $B=+0.1$ T (blue) and $-0.1$ T (orange). Resistances are in units of $h/e^2$. The dashed line in (a) marks $3h/(2e^2)$.

State the actual fields, units, and panel encodings. Add definitions for any displayed uncertainties; keep author queries outside the caption.

## 4. Statistical physics theory

**Context:** An isotropic spin-1/2 chain has $H=J\sum_j\mathbf S_j\cdot\mathbf S_{j+1}$, with $\mathbf S=\boldsymbol{\sigma}/2$. Use the infinite-temperature full-trace ensemble, zero mean magnetization, lattice spacing 1, and time in $\hbar/J$.

**Write**

> Taking $L\to\infty$ before long times, the Kardar–Parisi–Zhang (KPZ) ansatz for $C(j,t)=2^{-L}\operatorname{Tr}[S_j^z(t)S_0^z]$ is
>
> $$C(j,t)\simeq \frac{1}{4(\Gamma t)^{2/3}}f_{\mathrm{KPZ}}\!\left(\frac{j}{(\Gamma t)^{2/3}}\right),$$
>
> where $L$ is chain length, $f_{\mathrm{KPZ}}$ has unit integral, and $\Gamma$ is nonuniversal. The spin-correlation profile therefore broadens as $t^{2/3}$.

Identify the observable, normalization, units, limits, and status of the expression. An asymptotic ansatz and an exact finite-time identity make different claims.

## 5. Statistical physics computation

**Illustrative caption**

> **Figure 2. Activity in biased East-model trajectories.** Periodic chains use equilibrium concentration parameter $c=0.1$ and attempt time $\tau_0$, starting from equilibrium conditioned on at least one excitation. Relative to the unbiased distribution $P_0$, trajectory weights are $P_s\propto P_0e^{-sK}$; $K$ counts configuration changes and $s$ is dimensionless. Mean activity $k=\langle K\rangle_s/(Nt_{\mathrm{obs}})$, in $\tau_0^{-1}$, is plotted versus $s$. (a) $N=64,128,256$ sites at $t_{\mathrm{obs}}=1000\tau_0$. (b) $t_{\mathrm{obs}}=500,1000,2000\tau_0$ at $N=256$. Shading gives pointwise 95% bootstrap intervals from 20 independent run means per setting.

Check autocorrelation and sampling convergence; with cloning, assess population bias and use independent runs as replicates. Examine finite-size and finite-time behavior before claiming a singular limit.

## 6. Statistical physics experiment

**Context:** In colloidal-roller experiments, dense arrested domains coexist with a polar liquid. A hydrodynamic model with density-dependent motility reproduces coexistence and moving interfaces; the microscopic cause of slowing remains unresolved.

**Write**

> Particle speed decreases with local area fraction. The model reproduces coexistence and moving interfaces, supporting a motility-driven explanation. Lubrication interactions remain a proposed microscopic origin of the slowing.

Keep the observed behavior direct. Distinguish measurement, model-supported explanation, and microscopic conjecture.

## 7. Gravity theory

**Context:** Effective-field-theory matching establishes vanishing conservative static tidal Love coefficients for Kerr black holes in four-dimensional classical general relativity.

**Draft**

> The conservative static Love coefficients vanish for Kerr black holes in four-dimensional classical general relativity. Of course, this does not settle every question about black holes.

**Revision**

> The conservative static Love coefficients vanish for Kerr black holes in four-dimensional classical general relativity.

The coefficient, response regime, theory, and dimensionality already scope the result. End there.

## 8. Gravity computation

**Illustrative inputs:** For one binary configuration, an analytic general-relativistic model and a numerical-relativity waveform share an early-inspiral alignment. Their dominant-mode merger phases differ by 0.20 rad. Resolution and extraction variations change that phase by 0.02 and 0.01 rad.

**Write**

> For this configuration and alignment, the analytic model differs from the numerical merger phase by 0.20 rad, exceeding the tested resolution and extraction variations of 0.02 and 0.01 rad.

Report variations as variations. A quantitative error bound or statistical significance requires its own analysis; identify the model comparison being made.

## 9. High-energy experiment

**Reported context:** ATLAS observes top-pair spin entanglement in a near-threshold selection, $340<m_{t\bar t}<380$ GeV, using a particle-level witness and its corresponding mapped separability threshold.

**Write**

> The selected top-pair sample exhibits spin entanglement, with the no-entanglement hypothesis excluded at more than five standard deviations.

The witness tests separability, not a Bell inequality. Preserve the tested hypothesis, selected phase space, and reported strength. Use the threshold corresponding to the observable's reconstruction level.
