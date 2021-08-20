# Molecular orbital visualization with psi4 and PyMol

## Install software

1. Install psi4 and RDkit
 
```console
$ conda install psi4 -c psi4
$ conda install rdkit -c rdkit
```

2. Install psikit (integrates psi4 and RDkit)
```console
$ pip install psikit
```

## Generating Cube Files
- References
  - [Psithon: Structuring an input file](https://psicode.org/psi4manual/master/psithoninput.html#sec-psithoninput)
  - [Generation of Cube Files: `cubeprop()`](https://psicode.org/psi4manual/master/cubeprop.html)


## Visualize HOMO and LUMO

```
# in pymol
isomesh HOMO_A,  Psi_a_16_16-A, -0.02
isomesh HOMO_B,  Psi_b_16_16-A, 0.02
color blue, HOMO_A
color red, HOMO_B
```

## Other references
- [Visualize molecular orbital with PyMol and psikit](https://archive.is/tyLZX)
- [Calculate HOMO and LUMO with Psi4](https://archive.is/kUKP3)
