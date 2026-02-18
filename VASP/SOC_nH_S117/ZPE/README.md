# Input file
Input files: INCAR, POSCAR, KPOINTS and relevant vasp.nclout files for the ZPE calculation. The POTCAR file has been omitted.
Here, we have calculated the ZPE phonon modes by letting the first bilayer and the adsorbed hydrogen to move (phonon modes) and fixing the rest of iones of the slab (POSCAR.2).

In order to continue the ZPE calculation (POSCAR.2), you have to (calculate and then) substract the ZPE and Entrophy energy from the clean slab without the adsorbed atom.
