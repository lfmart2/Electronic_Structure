# Input file
Input files: INCAR, POSCAR, KPOINTS and relevant vasp.nclout files for the ZPE calculation. The POTCAR file has been omitted.
Here, we have calculated the ZPE phonon modes by:
- Freezing the slab's ions and letting the adsorbed hydrogen atom to freele move (POSCAR.1),
We have omitted the second calculation we inmplemented in the non Collinear case, where we let the first substrate of the Weyl semimetal to freely move. This is because the energy correction by considering the first substrate layer was found to be small. Thus, no further ZPE calculations are required for the Supercell 1x1x7 with collinear spin (non SOC) are needed.
