---
title: "Electronic-Structure Methods for Large-Scale Condensed-Phase Systems"
excerpt: "Towards Accurate and Efficient Denisty Functional Theory<br/><img src='http://www.quantum-espresso.org/user/themes/quantum/images/logo_header.jpg' width='300'>"
permalink: /research/electronic-structure
collection: research
---

Due to the favorable balance of accuracy and computational cost, Kohn−Sham (KS) density functional theory (DFT)
has become the most widely used electronic structure method for simulating large molecules and complex condensed-phase materials.
While DFT is an exact theory in principle, the exact expression of the exchange-correlation energy (Exc) as a functional of density remains unknown to date.
The approximated treatment of Exc remains an active field of research often described as the rungs of "Jacob's Ladder,"
connecting the Hartree (inaccurate but computationally efficient) to the heaven of chemical accuracy (accurate but computationally very demanding).
My focus along this research thrust is developing theoretical methods and computational algorithms for
enabling routine use of highly accurate and reliable DFT approximations on complex condensed-phase systems for chemistry, physics, and materials science.


#Quantum ESPRESSO (QE)
<a name="qe"></a>

I am an active and long-term developer of the Quantum ESPRESSO (QE) package, covering, e.g.,
linear-scaling exact-exchange, Tkatchenko-Scheffler (TS) and many-body dispersion (MBD), meta-generalized gradient approximation (meta-GGA) functionals.
My development mostly starts within the Car-Parrinello (CP) *ab initio* molecular dynamics (AIMD) framework as standalone modules for portability to
the QE ecosystem and potentially other ab initio simulation packages.

## References
- "Advanced capabilities for materials modelling with Quantum ESPRESSO" 
P. Giannozzi, O. Andreussi, T. Brumme, O. Bunau, M. B. Nardelli, M. Calandra, R. Car, C. Cavazzoni, D. Ceresoli, M. Cococcioni, N. Colonna, I. Carnimeo, A. D. Corso, S. de Gironcoli, P. Delugas, R. A. DiStasio Jr., A. Ferretti, A. Floris, G. Fratesi, G. Fugallo, R. Gebauer, U. Gerstmann, F. Giustino, T. Gorni, J. Jia, M. Kawamura, **H.-Y. Ko**, A. Kokalj, E. Küçükbenli, M. Lazzeri, M. Marsili, N. Marzari, F. Mauri, N. L. Nguyen, H.-V. Nguyen, A. Otero-de-la-Roza, L. Paulatto, S. Poncé, D. Rocca, R. Sabatini, B. Santra, M. Schlipf, A. P. Seitsonen, A. Smogunov, I. Timrov, T. Thonhauser, P. Umari, N. Vast, X. Wu, and S. Baroni, *J. Phys.: Condens. Matter* **29**, 465901 (2017).
DOI: <u><a href="https://doi.org/10.1088/1361-648x/aa8f79">10.1088/1361-648X/aa8f79</a></u>; alternative: <u><a href="https://arxiv.org/abs/1709.10010">arXiv</a></u>



#O(N) Exact-Exchange Algorithms (exx)
<a name="exx-paper-1"></a>

By admixing a fraction of exact exchange (EXX), hybrid functionals reduce the self-interaction error in semilocal density functional theory (DFT) and thereby furnish a more accurate and reliable description of the underlying electronic structure in systems throughout biology, chemistry, physics, and materials science.
However, applicability of hybrid DFT in the treating complex condensed-phase materials remains rather limited due to the high computational cost associated with the evaluation of the necessary EXX-related quantities.

In this work, we overcome this limitation via a linear-scaling approach that uses a local representation of the occupied orbitals (e.g., maximally localized Wannier functions (MLWFs)) to exploit the sparsity in the real-space evaluation of the quantum mechanical exchange interaction in finite-gap systems.
Our effort has yield a massively parallel (hybrid MPI/OpenMP) implementation (exx) in the open-source Quantum ESPRESSO package.
We found that this implementation is highly efficiently high-performance computing (HPC) resources available on current- and next-generation supercomputer architectures.
With sufficient HPC resources, we demonstrated that exx enables hybrid DFT-based *ab initio* molecular dynamics (AIMD) simulations of condensed-phase systems containing 500–1000 atoms (e.g., (H2O)256) with a wall time cost that is comparable to that of semilocal DFT.
As such, exx takes us one step closer to routinely performing AIMD simulations of complex and large-scale condensed-phase systems for sufficiently long time scales at the hybrid DFT level of theory.

<u><a href="https://pubs.acs.org/doi/10.1021/acs.jctc.9b01167"><img src='/images/research_exx-paper-1.png' width='600'></a></u>

## References
- **H.-Y. Ko**, J. Jia, B. Santra, X. Wu, R. Car, and R. A. DiStasio Jr., *J. Chem. Theory Comput.* **16**, 3757 (2020). DOI: <u><a href="https://pubs.acs.org/doi/10.1021/acs.jctc.9b01167">10.1021/acs.jctc.9b01167</a></u>; alternative: <u><a href="https://arxiv.org/abs/1911.10630">arXiv</a></u>



#O(N) Exact-Exchange Extension to Constant-Pressure Ensembles
<a name="exx-paper-2"></a>
## References
- H.-Y. Ko, B. Santra, and R. A. DiStasio Jr., *J. Chem. Theory Comput.* **17**, 7789 (2021). DOI: <u><a href="https://pubs.acs.org/doi/10.1021/acs.jctc.0c01194">10.1021/acs.jctc.0c01194</a></u>; alternative: <u><a href="https://arxiv.org/abs/2011.07209">arXiv</a></u>
TODO

#O(N) Exact-Exchange for Heterogeneous Systems
<a name="exx-paper-3"></a>
TODO

