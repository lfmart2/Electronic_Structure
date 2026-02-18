# VASP Workflows

This folder contains VASP-oriented examples for topological materials, with emphasis on supercell/slab-like configurations useful for surface-state analysis.

## Focus areas

- Surface/supercell electronic-structure calculations
- Band structure analysis
- Density of States (DOS)
- Fermi-surface / spectral-function style studies

## Suggested organization for future additions

For each new material, consider grouping files as:

- `input/` (`INCAR`, `KPOINTS`, `POSCAR`, `POTCAR` notes)
- `runs/` (SCF, NSCF, bands)
- `postprocessing/` (DOS/band plotting data)
- `figures/` (final publication/interview visuals)

This structure makes your work easier to review during interviews and collaborations.
