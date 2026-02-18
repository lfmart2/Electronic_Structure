# Electronic Structure Portfolio: DFT Workflows for Topological Materials

> A recruiter-friendly portfolio of **first-principles simulation workflows** using **Quantum ESPRESSO** and **VASP**.

This repository is structured to demonstrate practical, end-to-end computational materials science work: from simulation setup, to execution stages, to post-processing-ready artifacts.

---

## What this repository demonstrates

- Multi-code experience: **Quantum ESPRESSO + VASP**
- Workflow literacy: **Relaxation → SCF/NSCF → Bands/DOS/PDOS → Wannier90/TB preparation**
- Physics-focused modeling choices: **SOC vs non-SOC**, **spin-polarized vs non-spin**, **adsorbate coverage variants**
- Reproducible project organization for HPC-based research

---

## Repository layout (organized for review)

```text
Electronic_Structure/
├── README.md                       # portfolio-level overview (this file)
├── QuantumEspresso/
│   ├── README.md                   # QE workflow guide
│   ├── NbP_scf.in, NbP_nscf.in     # top-level example inputs
│   ├── NbP_bands.in, pp.*.in       # post-processing examples
│   ├── NbP_nspin/                  # non-spin baseline workflow
│   └── NbP_spin/                   # spin-polarized workflow
└── VASP/
    ├── README.md                   # VASP workflow map + case descriptions
    ├── nSOC_nH_S117/               # non-SOC, no-H configuration
    ├── nSOC_H_S117/                # non-SOC, H-adsorbed configuration
    ├── SOC_nH_S117/                # SOC, no-H configuration
    └── SOC_H_S117/                 # SOC, H-adsorbed configuration
```

---

## Quick start (for reviewers)

If you are reviewing this repository for internships, graduate roles, or research positions:

1. Open [`VASP/README.md`](VASP/README.md) to see complete workflow variants and folder naming conventions.
2. Open [`QuantumEspresso/README.md`](QuantumEspresso/README.md) for a compact NbP-focused QE pipeline.
3. Inspect representative stage folders (`Relaxation`, `SCF`, `Bandstructure`, `Wannier90`, `V2W`, `ZPE`) for production-style inputs.

---

## Workflow coverage

| Area | Examples in repository |
|---|---|
| Ground-state setup | SCF/NSCF inputs, INCAR/KPOINTS/POSCAR stacks |
| Band calculations | QE bands flow, VASP bandstructure stage folders |
| DOS/PDOS | QE `pp.dos` / `pp.pdos` input-output traces |
| SOC/Spin analysis | SOC and non-SOC + spin/non-spin configurations |
| Model building | Wannier90 preparation and VASP-to-Wannier flow |

---

## Portfolio talking points (for interviews)

- I can set up and compare **multiple spin/SOC regimes** for the same material system.
- I maintain **stage-separated workflows** that make reruns and debugging easier.
- I preserve input/output artifacts to support **traceability and reproducibility**.
- I can bridge DFT outputs toward **model Hamiltonian workflows** (Wannier90/TB).

---

## Suggested next enhancements

To make this portfolio even stronger for hiring managers:

- Add one figure-based case study (band structure + short interpretation)
- Add a reproducibility note per case (code version, pseudopotentials, cutoff/k-grid convergence)
- Add lightweight scripts to parse and plot selected outputs automatically

---

## Contact

If you are a recruiter, collaborator, or research group interested in this work, feel free to connect via my GitHub profile.
