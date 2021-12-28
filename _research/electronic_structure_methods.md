---
title: "Electronic-Structure Methods for Large-Scale Condensed-Phase Systems"
excerpt: "Towards Accurate and Efficient Denisty Functional Theory<br/><img src='http://www.quantum-espresso.org/user/themes/quantum/images/logo_header.jpg' width='300'>"
permalink: /research/electronic-structure
collection: research
---

<a name="exx">
# O(N) Exact-Exchange Algorithms (exx)
</a>

By admixing a fraction of exact exchange (EXX), hybrid functionals reduce the self-interaction error in semilocal density functional theory (DFT) and thereby furnish a more accurate and reliable description of the underlying electronic structure in systems throughout biology, chemistry, physics, and materials science.
However, applicability of hybrid DFT in the treating complex condensed-phase materials remains rather limited due to the high computational cost associated with the evaluation of the necessary EXX-related quantities.

In this work, we overcome this limitation via a linear-scaling approach that uses a local representation of the occupied orbitals (e.g., maximally localized Wannier functions (MLWFs)) to exploit the sparsity in the real-space evaluation of the quantum mechanical exchange interaction in finite-gap systems.
Our effort has yield a massively parallel (hybrid MPI/OpenMP) implementation (exx) in the open-source Quantum ESPRESSO package.
We found that this implementation is highly efficiently high-performance computing (HPC) resources available on current- and next-generation supercomputer architectures.
With sufficient HPC resources, we demonstrated that exx enables hybrid DFT-based *ab initio* molecular dynamics (AIMD) simulations of condensed-phase systems containing 500–1000 atoms (e.g., (H2O)256) with a wall time cost that is comparable to that of semilocal DFT.
As such, exx takes us one step closer to routinely performing AIMD simulations of complex and large-scale condensed-phase systems for sufficiently long time scales at the hybrid DFT level of theory.

<u><a href="https://pubs.acs.org/doi/10.1021/acs.jctc.9b01167"><img src='/images/research_exx-paper-1.png' width='300'></a></u>

## Reference
- H.-Y. Ko, J. Jia, B. Santra, X. Wu, R. Car, and R. A. DiStasio Jr., *J. Chem. Theory Comput.* **16**, 3757 (2020). DOI: <u><a href="https://pubs.acs.org/doi/10.1021/acs.jctc.9b01167">10.1021/acs.jctc.9b01167</a></u>; alternative: <u><a href="https://arxiv.org/abs/1911.10630">arXiv</a></u>
- H.-Y. Ko, B. Santra, and R. A. DiStasio Jr., *J. Chem. Theory Comput.* **17**, 7789 (2021). DOI: <u><a href="https://pubs.acs.org/doi/10.1021/acs.jctc.0c01194">10.1021/acs.jctc.0c01194</a></u>; alternative: <u><a href="https://arxiv.org/abs/2011.07209">arXiv</a></u>

# Constant-Pressure and General-Cell Extensions to exx
TODO

# Quantum ESPRESSO
TODO

