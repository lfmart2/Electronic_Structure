# Quantum ESPRESSO Workflow Collection

This folder contains Quantum ESPRESSO examples centered on NbP workflows for electronic-structure analysis in topological-material contexts.

## What is included

- SCF and NSCF input files
- Band-structure setup and generated data files
- DOS/PDOS post-processing inputs and outputs
- Example pseudopotential files used in these runs

## Subfolders

- `NbP_nspin/`:
  non-spin baseline workflow useful for comparison and validation
- `NbP_spin/`:
  spin-polarized workflow including SCF, NSCF, bands, and PDOS artifacts

## Typical execution order

1. `scf` calculation
2. `nscf` calculation
3. `bands` or DOS/PDOS post-processing (`pp.bands`, `pp.dos`, `pp.pdos`)
4. plotting/analysis from generated `*.dat`, `*.gnuplot`, `*.ps`

## Reuse notes

- Treat these inputs as templates and re-converge for any new material.
- Update pseudopotentials, cutoff energies, and k-point meshes per target system.
- Keep output logs with each stage to preserve reproducibility for publication/interview review.
