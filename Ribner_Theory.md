# RIBNER- Linear Interaction Approximation (LIA)
## Physical Motivation

When a turbulent flow encounters a shock wave, the shock does not merely compress the mean flow; it also interacts with turbulent fluctuations. These interactions modify turbulence intensity, redistribute energy among modes, and generate new fluctuations downstream.

Ribner's model provides one of the earliest and most fundamental theoretical descriptions of this process by treating shock-turbulence interaction(STI) as a linear problem. The key idea is that small-amplitude turbulent fluctuations interact with a thin, planar shock in a predictable and mode-dependent manner.

This model serves as a baseline theory for STI, against which more advanced models(eg, rapid distortion theory, shock distortion models and MHD extension) can be compared.

## Core Assumptions

The Ribner model rests on several crucial assumptions:
1. **Small perturbations**
   Turbulent fluctuations are assumed to be small compared to the mean flow quantities. This allows linearizations of the governing equations and shock jump conditions.

2. **Thin, planar shock**
    The shock thickness is negligible compared to turbulent length scales, and the shock is treated as a sharp discontinuity.

3. **Linear Interaction Approximation(LIA)**
     Each turbulent mode interacts independently with the shock. Nonlinear mode-mode coupling at the shock is neglected.

4. **No back reaction on the shock structure**
     Turbulence does not significantly alter the mean shock strength or position; the shock responds only weakly to incoming fluctuations.


These assumptions restrict the validity of the model to weak-to-moderate shocks and low turbulent Mach number, but they make the physics analytically transparent.
    

## Mode Decomposition of Turbulence 

A central idea in Ribner'approach is that turbulence can be decomposed into fundamental linear modes:
- Acoustic modes (pressure–velocity coupled)
- Entropy modes (density fluctuations with no pressure fluctuation)
- Vortical modes (rotational velocity fluctuations)

Upstream turbulence is represented as a superposition of these modes.

Because the governing equations are linearized, each mode interacts with the shock independently, and the downstream flow is obtained by summing their transmitted and reflected components.

This decomposition allows Ribner to identify which physical mechanisms are reponsible for specific downstream effects.

## Linearized Shock Interaction

The interaction between turbulence and the shock is governed by the linearized Rankine–Hugoniot conditions, applied at a slightly perturbed shock surface.

Physically, this means:

- The shock responds weakly to incoming fluctuations by undergoing small displacements.
- Fluctuations in velocity, pressure, and density are transmitted and modified as they cross the shock.
- The jump conditions act as a filter, amplifying or attenuating different modes.

The shock therefore acts not merely as a compressive discontinuity, but as a mode-converting interface.

## Key predictions of Ribner Model
The Ribner model predicts several qualitative and quantitative features of STI:

- Amplification of velocity fluctuations across the shock
- Generation of pressure and density fluctuations downstream
- Redistribution of energy among acoustic, vortical, and entropy modes
- Dependence of amplification factors on upstream Mach number

Importantly, these predictions arise without invoking nonlinear turbulence dynamics, highlighting the dominant role of shock-induced distortion and mode conversion.
## Limitations and Scope of Validity

While foundational, the Ribner model has clear limitations:

- It cannot capture shock distortion by strong turbulence
- It neglects nonlinear mode coupling
- It does not predict long-term downstream turbulence evolution
- It is not suitable for strong shocks or high turbulence intensity

For these reasons, Ribner’s model is best viewed as a first-order, interpretive framework, rather than a complete predictive theory.
## Mathematical Theory

This section summarizes the mathematical formulation of the Ribner model. Detailed derivations are included for completeness and reference; the main physical interpretation is discussed in the preceding sections.
**Physical Idea**

Treat the shock as a mean discontinuity with small oscillations due to incident disturbances.

Upstream turbulence is decomposed into linear modes:
- Acoustic (pressure-density coupled)
- Entropy (density-only fluctuations)
- Vorticity (transverse velocity only)

Each interacts linearly with the shocks, producing transmitted and reflected waves.

**Assumptions**

- Small amplitude turbulence $|u'|/a_1 << 1$ (linear regime) where $a_1$ is upstream sound speed & u' is turbulent velocity
- Shock is nominally planar, with perturbations $ \xi(y,t)$
- Mean shock obeys Rankine-Hugoniot(RH) relations & perturbations satisfy linearized RH conditions.



Now, Mean quantities:- $\large \bar{u_1}, \bar{u_2}, \bar{\rho_1}, \bar{\rho_2}, \bar{p_1}, \bar{p_2}$

Satisfy the Rankine-Hugonoit(RH) conditions:

$ \large \bar{\rho_1} \bar{u_1} = \bar{\rho_2} \bar{u_2}$

$ \large \bar{p_2} - \bar{p_1} = \bar{\rho_1} \bar{u_1} (\bar{u_1} - \bar{u_2})$ 

Now introduce small perturbations upstream & downstream:

$\large u_i = \bar{u_i} + u'_i$

$\large p_i = \bar{p_i} + p'_i$

$\large \rho_i = \bar{\rho_i} + \rho'_i$

and let the shock surface be displaced to x = $ \xi(y, t)$

Shock perturbation $ \large \xi(y, t) = \xi_o e^{i(ky - wt)}$  Here k -> tangential wavenumber, w -> angular frequency

We now linearize the full RH conditions(mass, momentum) at the perturbed shock.
This means:- expand quantities at x = $ \xi$ around x = 0 and retain only first-order terms.

(a) Kinematic condition:
Fluid on both sides must satisfy that the shock waves with the local normal velocity -

$\Large \frac{D\xi}{Dt} = u'_n |_{x=0}$

For small angles, $\Large u'_n \thickapprox u'_x$

So, 
     $ \Large \partial_t \xi = u'_x(0, t)$

(b) Linearized jump condition:
Start with exact RH-

$\Large [\rho(u_n - \dot{\xi})] = 0$, $\Large [\rho(u_n - \dot{\xi}) + p] = 0$ , $\Large [\rho(u_n - \dot{\xi}) u_t] = 0$

Linearize about the mean.

After substituting $\Large u_i = \bar{u_i} + u'_i$, $\Large p_i = \bar{p_i} + p'_i$, $\Large \rho_i = \bar{\rho_i} + \rho'_i$ and retaining first-order we get-
Mass continuity:- $\Large [\bar{\rho}(u'_n - \partial_t \xi) + \bar{u} \rho'] = 0$                   
                                                                                                              
Normal momentum:- $\Large [\bar{\rho} \bar{u} (u'_n - \partial_t \xi) + \bar{u^2} \rho' + p'] = 0$                 

Tangential momentum:- $\Large [\bar{\rho} \bar{u} u'_t] = 0$

They connect upstream/downstream perturbation & shock motion $\Large \partial_t \xi$.
     

For acoustic mode:

$\Large \frac{p'}{\bar p} = \gamma \frac{\rho'}{\bar \rho} = \frac{\gamma}{a^2} \bar{\rho} \bar{u} u'_n$

For vorticity mode:
   
   $\Large p'=0$, $\large \rho'=0$, $\large \nabla.(u')=0$

For entropy mode:

   $\Large p'=0$, $\Large \frac{\rho'}{\bar{\rho}} = -\frac{s'}{c_p}$



For a vorticity wave incident on a shock:
- Normal velocity component --> amplified strongly, especially at higher Shock Mach number
- Tangential velocity component --> slightly reduced due to compression ratio
- Pressure & density fluctuations --> generated downstream even though upstream had none (Baroclinic effect)


**The LIA provides an analytical map of how each turbulent mode changes across a shock. It's valid for small $M_t$ (turbulent Mach number), and weak shock distortion.**
