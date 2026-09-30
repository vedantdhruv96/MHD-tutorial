# MHD numerics tutorial

This notebook accompanies a tutorial on magnetohydrodynamics (MHD) that I gave at Alex and Yajie's group meeting at WashU. It is meant as a self-contained introduction to the subject, 
with the code written in the style of HARM-based GRMHD codes (flux-CT for the field update, a second-order predictor-corrector timestepper) so that it carries over to production codes.

The notebook builds up a conservative finite volume scheme step by step. It starts with 1D linear advection to introduce reconstruction (donor cell, piecewise linear, slope limiters) 
and upwind fluxes, then moves to ideal MHD with the Brio-Wu shock tube to cover ghost zones, Riemann solvers, the CFL condition, and the predictor-corrector time-stepping scheme. It 
closes with the 2D Orszag-Tang vortex, which is used to explain the flux-CT routine.

If something is unclear, or you have a suggestion, please let me know!

*Disclaimer: Claude Code was used in developing this notebook, primarily for the code.*
