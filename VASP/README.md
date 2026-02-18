# VASP Workflow Collection

This directory contains portfolio-ready VASP setups for topological/surface-oriented studies across multiple spin-orbit and adsorbate configurations.

## Naming convention used in this folder

Each main case follows:

- `SOC` or `nSOC`: with/without spin-orbit coupling
- `H` or `nH`: with/without adsorbed hydrogen
- `S117`: slab/supercell identifier used in this project

Examples:

- `nSOC_nH_S117` → non-SOC, no hydrogen
- `SOC_H_S117` → SOC enabled, hydrogen adsorbed

## Stage-oriented project structure

Typical stage folders you will see inside each case:

- `Relaxation/` → structure optimization
- `SCF/` → self-consistent electronic ground state
- `Bandstructure/` or `V2W/` → non-self-consistent paths / VASP-to-Wannier pipeline
- `Wannier90/` → Wannier input setup for TB/model analysis
- `ZPE/` → zero-point-energy related setup

This stage separation mirrors production HPC workflows and improves rerun/debug traceability.

## Included configurations

- Collinear spin, **non-SOC**, supercell `1×1×7`, no adsorbed H
- Collinear spin, **non-SOC**, supercell `1×1×7`, high H coverage
- Non-collinear spin, **SOC**, supercell `1×1×7`, no adsorbed H
- Non-collinear spin, **SOC**, supercell `1×1×7`, high H coverage
- Non-collinear spin, **SOC**, supercell `2×1×7`, no adsorbed H
- Non-collinear spin, **SOC**, low-coverage H case (as labeled in project folders)

## Typical run sequences

### Sequence A: band-focused

1. `Relaxation`
2. `SCF`
3. `Bandstructure` (or equivalent NSCF path)
4. post-processing / plotting

### Sequence B: model-building-focused

1. `Relaxation`
2. `SCF`
3. `V2W`
4. `Wannier90`
5. tight-binding/model analysis

## Recruiter/interview note

This folder is organized to show practical DFT engineering habits:

- clear stage decomposition
- explicit case variants (SOC/non-SOC, H/non-H)
- reusable templates for extension to new materials or slab sizes
