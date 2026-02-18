# Quantum ESPRESSO Workflows

This folder contains Quantum ESPRESSO examples for topological-material studies (NbP-focused), including both spin and non-spin workflows.

## Contents

- SCF/NSCF setup files
- Band-structure inputs and generated data
- DOS/PDOS post-processing inputs/outputs
- Pseudopotential files used in sample runs

## Notable subfolders

- `NbP_spin/`:
  Spin-polarized example workflow with SCF, NSCF, bands, and PDOS processing.
- `NbP_nspin/`:
  Non-spin counterpart for comparison and baseline checks.

## Typical run sequence

1. `scf` calculation
2. `nscf` calculation
3. `bands` (or DOS/PDOS) post-processing
4. plotting/analysis (`*.gnuplot`, `*.dat`, `*.ps`)

## Notes

- Input parameters are examples and should be converged for each new material.
- Update pseudopotentials and cutoffs as required by your target system.
