# Docking

## Background

- two major tasks
  - sampling algorithm: predict conformations, referred to as **poses**, of the
    ligand in the binding/active pocket.
  - scoring function: predict the binding energy between ligand and receptor for each predicted pose
- limitations
  - static nature of receptor: receptors are dynamic
  - limitations in sampling algorithms and scoring functions
  - requirement for training sets leads to accuracy being highly target dependent

### A. Receptor structure preparation

- Easy
  - Adding hydrogens
  - Adding atom-type charges
- Medium
  - Ensure that missing side chains are added
  - Missing bonds and molecule chain breaks are detected and fixed
  - Bond orders are assigned
  - When alternate positions are present, atoms with highest frequencies are selected
- Difficult
  - Determining protonation states
    - His
    - Asp (deprot)
    - Glu (deprot)
    - Arg (prot)
    - Lys (prot)
  - Identifying which water molecules should remain in the receptor structure


## AutoDock 4, AutoDock Vina, AutoDockTools

### File formats
- PDB. Protein Data Bank file
- PDBQT. Protein Data Bank with partial charge (Q) and atom type (T) format
- GPF. Grid Parameter File
- GLG. Grid Log File
- DPF. Docking Parameter File
- DLG. Docking Log File
