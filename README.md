# Practical Guide to Bioinformatics Tools

## Recommended Order
TODO: Add image of recommended prereqs

- **Note:** Tutorials are presented in the recommended order of completion.
- **Note:** ๐ก = general info, ๐ = file format, ๐๏ธ = database, ๐ = web service, ๐งฐ = offline tool, ๐งช = experimental method

## ๐ก Genetic codes

- [The Genetic Codes (NCBI)](https://www.ncbi.nlm.nih.gov/Taxonomy/Utils/wprintgc.cgi)

## ๐ FASTA file format (`.fasta`, `.fna`, `.faa`)

- `.fasta`, `.fa`. generic FASTA
- `.fna`. FASTA nucleic acid
- `.frn`. FASTA non-coding RNA
- `.faa`. FASTA amino acid
- `.ffn`. FASTA nucleotide of gene regions (i.e. coding regions)

## ๐๏ธ GenBank

_Uncurated, archival database of nucleic acid and protein sequences from labs around the world._

### Tutorials
- [GenBank Sample Record with explanations](https://www.ncbi.nlm.nih.gov/Sitemap/samplerecord.html).

## ๐๏ธ RefSeq

_Curated, non-redundant database of DNA, mRNA, and protein sequences sourced from GenBank._

### Notes
- Updates denoted by increment to the numeric version after the decimal; e.g. `NM_xxx.2` ([source](https://archive.is/W6CyS))
- [General information about RefSeq (part of Frequently Asked Questions)](https://www.ncbi.nlm.nih.gov/books/NBK50679/#RefSeqFAQ.General_Information_about_RefS)
- [NCBI Handbook, Chapter 18: The RefSeq Database (2002)](https://www.ncbi.nlm.nih.gov/books/NBK21091/)

## ๐งฐ Muscle

_A multiple sequence alignment tool._

- [Project website](https://drive5.com/muscle/)

### Alternatives
- [Clustal Omega](http://www.clustal.org/omega/). The latest addition to the Clustal multiple sequence alignment software family. Clustal Omega scales well to hundreds of thousands of sequences (aligned in a few hours).


## ๐งฐ AliView

_A multiple sequence alignment viewer written in Java._

- Supported on Windows, macOS, and Linux.

## ๐๏ธ Gene

_Database of genes integrated information from multiple data sources._

- [Documentation for the Gene Database](https://www.ncbi.nlm.nih.gov/books/NBK3839/)
  - [Documentation on Advanced Search Queries](https://www.ncbi.nlm.nih.gov/books/NBK3841/)

## ๐ Entrez

_NCBI's global database search engine._

### Programmatic Access: Entrez API
- [Entrez Programming Utilities (E-utilities)](https://www.ncbi.nlm.nih.gov/books/NBK25501/)
  - [Entrez Direct: E-utilities on the Unix Command Line](https://www.ncbi.nlm.nih.gov/books/NBK179288/)

## ๐๏ธ dbVar

_NCBI's archival (uncurated) database of large scale genomic variants (insertions, deletions, inversions)._

## ๐งฐ bedtools

_Genome feature manipulation tool._

Developed by the [Quinlan Lab at the University of Utah](http://quinlanlab.org/).

### Tutorials
1. [Description of the BED (Browser Extensible Data) file format.](http://genome.ucsc.edu/FAQ/FAQformat.html#format1)
    - BED files provide a flexible way to define the data lines that are displayed in an genome annotation track.
2. [Introduction to bedtools (sandbox.bio)](https://sandbox.bio/tutorials/?id=bedtools-intro)

## ๐ SAM/BAM file format (`.sam`, `.bam`)

_Sequence alignment/mapping file format._

## ๐งฐ bowtie2

_Aligns reads from a sequencer against a reference genome._

- `bowtie2` generates SAM files as output.
- [Github repository](https://github.com/BenLangmead/bowtie2)

## ๐งฐ samtools

_Suite of tools for viewing and manipulating SAM/BAM files._

- [Github repository](https://github.com/samtools/samtools)

## ๐ VCF/BCF file format (`.vcf`, `.bcf`)

_Variant call format (and binary counterpart) files are used to describe sequence variations in genomic data._

- Types of variations include
  - Single nucleotide variants
  - Insertions
  - Deletions

### Tutorials
- [NYU Genomics Core Learning Modules: VCF file format](https://learn.gencore.bio.nyu.edu/ngs-file-formats/vcf-format/)

## ๐งฐ bcftools

_Utilities for viewing and manipulating VCF/BCF files._

- [Github repository](https://github.com/samtools/bcftools)

## ๐ General Feature Format (GFF3) file format (`.gff`)

_Most flexible file format used to annotate genomic sequences with features._

- [NYU Genomics Core Learning Modules: GFF3 file format](https://learn.gencore.bio.nyu.edu/ngs-file-formats/gff3-format/)

## ๐งฐ ChromHMM

_Chromatin state discovery and characterization software._

- [Project website](http://compbio.mit.edu/ChromHMM/)
- [Chromatin-state discovery and genome annotation with ChromHMM](https://www.nature.com/articles/nprot.2017.124)

## ๐งช ChIP-seq

_Chromatin immunoprecipitation with sequencing: a way to analyze protein interactions with DNA, often in epigenomics._

### Lectures

- [UCLA QCBio Collaboratory: ChIP-seq analysis I](https://www.youtube.com/watch?v=uWM5WT3Dt0k)
- [UCLA QCBio Collaboratory: ChIP-seq analysis II](https://www.youtube.com/watch?v=7xre8FmUb8A)
- [UCLA QCBio Collaboratory: ChIP-seq analysis III](https://www.youtube.com/watch?v=JYBP5BpRfTM)

## ๐งช RNA sequencing (RNA-seq)

## ๐งช Single cell RNA sequencing (scRNA-seq)

## Protein-ligand interactions

### ๐ Protein-ligand Interaction Profiler (PLIP)

_Identifies non-covalent interactions between biological macromolecules and their ligands._

- [Link to web service](https://plip-tool.biotec.tu-dresden.de/plip-web/plip/index)

### ๐ Protein Plus

_Another protein-ligand prediction program._

- [Link to web service](https://proteins.plus/)

## PyMOL

### PDB2PQR and APBS (Adaptive Poisson-Boltzmann Solver)

_Two tools used together to visualize electrostatics in molecules._

## Psi4 and Psikit

## Molecular Docking

### AutoDock 4

### AutoDock Vina


