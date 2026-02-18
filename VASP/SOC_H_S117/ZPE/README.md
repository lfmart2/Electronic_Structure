# Input file
Input files: INCAR, POSCAR, KPOINTS and relevant vasp.nclout files for the ZPE calculation. The POTCAR file has been omitted.
Here, we have calculated the ZPE phonon modes by:
- Freezing the slab's ions and letting the adsorbed hydrogen atom to freele move (POSCAR.1),
- Letting the first bilayer and the adsorbed hydrogen to move (phonon modes) and fixing the rest of iones of the slab (POSCAR.2).

Note that the iones positions (POSCAR.1 and POSCAR.2) have to be the slab's relaxed file. In order to follow the second ZPE calculation (POSCAR.2), you have to (calculate and then) substract the ZPE and Entrophy energy from the clean slab without the adsorbed atom (see folder [ZPE_SOC_1x1x7](https://github.com/RibeiroGroup/Chemistry-with-Topological-Materials/tree/main/Fernando/Codes/VASP/Input%20files/SOC_nH_S117/ZPE))
