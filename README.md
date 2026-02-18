# Electronic Structure Workflows for Topological Materials

A curated collection of **first-principles simulation inputs and outputs** for electronic-structure studies, focused on topological materials.

This repository is designed to showcase practical computational workflows used in research and engineering contexts:

- SCF/NSCF ground-state calculations
- Band structure analysis
- DOS/PDOS post-processing
- Spin-polarized and SOC/non-SOC setups
- Surface/supercell-oriented studies

---

## Why this repository is useful

For recruiters, collaborators, and research teams, this repository demonstrates:

- Ability to prepare reproducible DFT workflows
- Familiarity with multiple codes (**Quantum ESPRESSO** and **VASP**)
- Understanding of post-processing pipelines for physically meaningful outputs
- Organized, project-based simulation data management

---

## Repository structure

```text
Electronic_Structure/
├── README.md
├── QuantumEspresso/
│   ├── README.md
│   ├── *.in                 # SCF/NSCF/BANDS/PDOS input files
│   ├── *.out                # output logs
│   ├── NbP_nspin/           # non-spin/SOC workflow example
│   └── NbP_spin/            # spin-polarized workflow example
└── VASP/
    └── README.md
```

---

## Included workflows

### 1) Quantum ESPRESSO
Examples include input decks and outputs for NbP-related calculations:

- `scf`, `nscf`, and `bands` workflows
- spin-polarized and non-spin variants
- pseudopotential usage and post-processing inputs (`pp.bands`, `pp.dos`, `pp.pdos`)

See details in [`QuantumEspresso/README.md`](QuantumEspresso/README.md).

### 2) VASP
The VASP section contains examples relevant to topological materials and slab/surface-style calculations.

See details in [`VASP/README.md`](VASP/README.md).

---

## Recommended usage

1. Choose a workflow folder (`QuantumEspresso/` or `VASP/`).
2. Inspect the local `README.md` and input files.
3. Adjust:
   - lattice/atomic structure
   - pseudopotentials or POTCAR setup
   - k-point mesh and cutoffs
   - spin/SOC flags based on target physics
4. Run on your local cluster/HPC system.

---

## Interview-friendly highlights

If you are using this repository as part of your portfolio, point reviewers to:

- Multi-code computational skillset (QE + VASP)
- End-to-end workflow thinking (inputs → outputs → plots)
- Domain focus in topological materials
- Reusable file templates for future projects

---

## Future improvements (roadmap)

- Add standardized folder templates for each new material
- Include convergence-test examples (`ecut`, `k-grid`, slab thickness)
- Provide sample plotting scripts (bands/DOS/PDOS)
- Add environment/setup notes for reproducibility

---

## Contact

If you are a recruiter or collaborator interested in this work, feel free to connect through my GitHub profile.
