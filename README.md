# Shock-Turbulence Interaction (STI): Theoretical &  Numerical Study

## Project Overview
This repository presents a theoretical & numerical study **Shock-Turbulence Interaction(STI)**, focusing on how a shock wave modifies statistical & structural properties of turbulence. The project systematically 
analyzes four foundational STI models- Ribner, Jacquin, Lele and Zank(MHD extension)-to understand the physical mechanisms governing turbulence amplification, distortion, and anisotropy induced by shock passage.
The work emphasizes model-level understanding rather than full-scale CFD, bridging analytical theroy with targeted numerical evaluationsof model predictions.

## Motivation
Shock-Turbulence Interaction plays a central role in:
- High-speed aerodynamics(scramjets, blast waves)
- Astrophysical waves(supernova shocks, accretion disks)
- Magnetized plasma(solar wind, interstellar medium)

  Despite its importance, STI remains theroetically subtle due to the interplay between compressibility, vorticity generation, and shock distortion. This project aims to develop physical intuitionby comparing classical
  and modern theoretical frameworks.

## Model Studied
### Ribner Model(Linear Interaction Analysis-LIA)
- Treats turbulence as a superposition of linear acoustic and vortical modes.
- captures compressibilty effects and pressure-velocity coupling
- Applicable in the weak-shock, low Mach-number regime

  Key focus:
  - Turbulence amplification factor
  - Spectral redistribution across shock

### Jacquin Model(Rapid Distortion Theory-RDT)
 - Accounts for mean flow gradients imposed by shock
 - Predicts turbulence amplification and length-scale compression
 - Introduces anisotropy due to differential distortion of velocity components

   Key focus:
   - Turbulent kinetic energy amplification
   - Post-Shock anisotropy

### Lele Model(Spectral/Numerical perspective)
- Emphasizes shock corrugation and distortion by incoming turbulence
- Highlights coupling between shock unsteadiness and turbulent fluctuation
- Relevant to DNS/LES-informed interpretations

  key focus:
  - Shock distortion mechanism
  - Mode coupling between turbulence and shock motion
 
### Zank Model(MHD extension)
- Extends STI concepts to Magnetohydrodynamics(MHD) turbulence
- Incoporates magnetic pressure, Alfven modes and plasma compressibilty
- Relevant for astrophysical and space plasma shocks

  Key focus:
  - Vorticity and magnetic field amplification
  - Modifications of turbulence spectra across MHD shocks
 
 ## Numerical Implementation
 Rather than full Navier-stokes simulation, this project focuses on numerical evaluation of theretical predictions, including:
 - Computation of turbulence amplification factor
 - Analysis of length-scale distortionacross shock
 - Parametric dependence on:
     - Shock Strength
     - Mach Number
     - Compressibility

 ## Key Results & Insights
 - Different STI models emphasize different physical mechanism, yet converge on similar qualititative trends in weak-skock limits.
 - Linear and RDT-based models remains valuable for interpretation and scaling arguments, even when DNS is infeasible.
 - MHD effects modifies classical STI behaviour through Alfvenic coupling and magnetic tension.

 ## References
 [1] Zank, G. P., Ye Zhou, W. H. Matthaeus, and W. K. M. Rice. “The Interaction of Turbulence with Shock Waves: A Basic Model.” PHYSICS OF FLUIDS 14, no. 11 (2002).
 
 [2] Kitamura T, Nagata K, Sakai Y, Sasoh A, Ito Y. Rapid distortion theory analysis on the interaction between homogeneous turbulence and a planar shock wave. <i>Journal of Fluid Mechanics</i>. 2016;802:108-146. https://doi:10.1017/jfm.2016.313 <div></div>

 [3] Yiannis Andreopoulos, Juan H. Agui, George Briassulis. 2000. Shock Wave—Turbulence Interactions. Annual Review Fluid Mechanics. 32:309-345. https://doi.org/10.1146/annurev.fluid.32.1.309
