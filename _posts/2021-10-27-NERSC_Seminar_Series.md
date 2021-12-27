---
title: 'Invited to Talk at NERSC'
date: 2021-10-27
permalink: /posts/2021/10/27/
tags:
  - invited talk
---

I wanted to thank NERSC again for the kind invitation to <u><a href="https://www.nersc.gov/science/nersc-hpc-achievement-awards/achievement-award-seminar-series/">talk about my research.</a></u>

## Towards an Accurate and Efficient Order-N HPC Framework for Large-Scale Condensed-Phase Hybrid Density Functional Theory
###October 27, 2021
###12:00-1:00 Pacific Time
### abstract

By including a fraction of exact exchange (EXX), hybrid functionals reduce the self-interaction error in semi-local density functional theory (DFT), thereby providing a more accurate and reliable description of the electronic structure in systems throughout chemistry, physics, and materials science. However, the high computational cost associated with hybrid DFT limits its applicability when treating large-scale and complex condensed-phase systems in many practical applications (e.g., design of fuel cells). To overcome this limitation, we have devised a highly accurate and linear-scaling (order-N) approach based on a local (e.g., MLWF) representation of the occupied space that exploits sparsity when evaluating the EXX interaction in real space. Powered by NERSC resources over the past several years, our development has evolved into a general-purpose algorithmic framework (exx) capable of efficiently using several modern HPC architectures [1]. The exx code already enabled several large-scale hybrid DFT-based applications in its pilot forms, e.g., unraveling the qualitative/substantial difference between the structural diffusions of H3O+ and OH- in aqueous solutions. Recently, we further extended exx to a black-box solver by eliminating its system-dependent parameters. With this new extension, exx brings us one step closer to the routine use of more reliable hybrid DFT for studying large-scale condensed-phase systems relevant to energy sciences and beyond.

[1] J Chem Theory Comput 16, 3757 (2020).
